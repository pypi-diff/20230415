# Comparing `tmp/data_connection-0.0.3.tar.gz` & `tmp/data_connection-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_connection-0.0.3.tar", max compression
+gzip compressed data, was "data_connection-0.0.4.tar", max compression
```

## Comparing `data_connection-0.0.3.tar` & `data_connection-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0      932 2022-10-31 13:07:12.379021 data_connection-0.0.3/README.md
--rw-r--r--   0        0        0     5948 2022-10-31 12:04:59.957417 data_connection-0.0.3/data_connection/abstract_side.py
--rw-r--r--   0        0        0     6106 2022-10-31 11:20:38.271719 data_connection-0.0.3/data_connection/datapoint.py
--rw-r--r--   0        0        0     3066 2022-10-31 12:05:54.652780 data_connection-0.0.3/data_connection/reader_side.py
--rw-r--r--   0        0        0     3488 2022-10-31 12:07:26.879568 data_connection-0.0.3/data_connection/writer_side.py
--rw-r--r--   0        0        0      992 2022-11-01 05:49:58.679972 data_connection-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 data_connection-0.0.3/setup.py
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 data_connection-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      932 2022-11-01 16:00:44.359327 data_connection-0.0.4/README.md
+-rw-r--r--   0        0        0      255 2022-11-10 16:23:10.432530 data_connection-0.0.4/data_connection/__init__.py
+-rw-r--r--   0        0        0     6887 2022-11-10 16:23:10.432530 data_connection-0.0.4/data_connection/abstract_side.py
+-rw-r--r--   0        0        0      683 2022-11-10 16:23:10.432530 data_connection-0.0.4/data_connection/base_model.py
+-rw-r--r--   0        0        0     8462 2022-11-10 16:23:10.432530 data_connection-0.0.4/data_connection/field.py
+-rw-r--r--   0        0        0     4818 2022-11-10 16:23:10.432530 data_connection-0.0.4/data_connection/reader_side.py
+-rw-r--r--   0        0        0       98 2022-11-10 16:23:10.432530 data_connection-0.0.4/data_connection/readers/__init__.py
+-rw-r--r--   0        0        0     1709 2022-11-12 11:57:48.422402 data_connection-0.0.4/data_connection/readers/mbtcp_client.py
+-rw-r--r--   0        0        0     8848 2022-11-12 11:58:27.417893 data_connection-0.0.4/data_connection/readers/opcua_client.py
+-rw-r--r--   0        0        0     5428 2022-11-10 16:23:10.436530 data_connection-0.0.4/data_connection/writer_side.py
+-rw-r--r--   0        0        0     1089 2022-11-12 11:58:36.969769 data_connection-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 data_connection-0.0.4/setup.py
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 data_connection-0.0.4/PKG-INFO
```

### Comparing `data_connection-0.0.3/README.md` & `data_connection-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `data_connection-0.0.3/data_connection/abstract_side.py` & `data_connection-0.0.4/data_connection/abstract_side.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,55 @@
 """Абстрактный класс для передачи данных."""
 
 # pyright: reportUnusedFunction=false
 
 import asyncio
 import ipaddress
 import logging
+import pickle  # noqa: S403
 from time import perf_counter_ns
-from typing import Any, Final, Generic, TypeVar
+from typing import Any, Final, Generic, Iterable, TypeVar
 
 from fastapi import FastAPI, WebSocket
 from pydantic import BaseModel
 from websockets.exceptions import ConnectionClosed, ConnectionClosedOK
 from websockets.legacy import client
 
-from .datapoint import Datapoint
+from .field import Field
 
 log: logging.Logger = logging.getLogger(__name__)
-log.setLevel(logging.DEBUG)
+log.setLevel(logging.INFO)
 
 NS_IN_S: Final[float] = 1e9
 URL: Final[str] = "ws://{host}:{port}{endpoint}"
-TBaseModel = TypeVar("TBaseModel", bound=BaseModel)  # noqa: WPS111
+TBaseModel = TypeVar("TBaseModel", bound=BaseModel)
+TModelField = Field[Any] | dict[str, Any]
+
+
+def isinstance_iterable(
+    __obj: Iterable[TModelField],
+    __class_or_tuple: type,
+) -> bool:
+    """Все элементы последовательности соответстуют типу.
+
+    Parameters
+    ----------
+    __obj: Iterable[TModelField]
+        Последовательность объектов
+    __class_or_tuple: type
+        Тип для проверки
+
+    Returns
+    -------
+    True - все элементы соответсвуют
+    """
+    for __obj_item in __obj:
+        if not isinstance(__obj_item, __class_or_tuple):
+            return False
+    return True
 
 
 class AbstractSide(Generic[TBaseModel]):  # noqa: WPS214
     """Абстрактный класс для передачи данных."""
 
     __data_ext: TBaseModel
     __data_int: TBaseModel
@@ -116,21 +141,21 @@
             объект для работы с протоколом websocket, созданный fastapi.
         """
         await websocket.accept()
         log.info("connection open with client: {0}".format(websocket.client))
         while True:  # noqa: WPS457
             begin: int = perf_counter_ns()
             data_xch: TBaseModel = self.__model.construct()
-            self._prepare_send(
+            self._prepare_send_model(
                 data_xch=data_xch,
                 data_int=self.__data_int,
                 data_ext=self.__data_ext,
             )
             try:
-                await websocket.send_text(data_xch.json(by_alias=True))
+                await websocket.send_bytes(pickle.dumps(data_xch))
             except ConnectionClosedOK:
                 log.info(
                     "connection closed from client: {0}".format(
                         websocket.client,
                     ),
                 )
                 break
@@ -145,35 +170,44 @@
             endpoint=self.__other_endpoint,
         )
         websocket_client = client.connect(url)
         websocket_client.BACKOFF_MAX = 10
         async for websocket in websocket_client:
             try:
                 async for message in websocket:
-                    log.debug("recieved message: {0}".format(message))
-                    msg_model: TBaseModel = self.__model.parse_raw(message)
-                    self._prepare_rcv(
+                    msg_model: TBaseModel = self.__model.parse_raw(
+                        b=message,
+                        content_type="application/pickle",
+                        allow_pickle=True,
+                    )
+                    log.debug("recieved message: {0}".format(msg_model))
+                    self._prepare_rcv_model(
                         data_xch=msg_model,
                         data_int=self.__data_int,
                         data_ext=self.__data_ext,
                     )
             except ConnectionClosed:
                 await asyncio.sleep(1)
 
-    def _prepare_send(
+    def _prepare_send_model(
         self,
         data_xch: TBaseModel,
         data_int: TBaseModel,
         data_ext: TBaseModel,
     ) -> None:
         raise NotImplementedError
 
-    def _prepare_rcv(
+    def _prepare_rcv_model(
         self,
         data_xch: TBaseModel,
         data_int: TBaseModel,
         data_ext: TBaseModel,
     ) -> None:
         raise NotImplementedError
 
-    def _is_datapoint(self, field: Any) -> bool:
-        return isinstance(field, Datapoint)
+    def _field_to_datapoint(
+        self,
+        field: Field[Any] | Any,
+    ) -> Field[Any] | None:
+        if not isinstance(field, Field):
+            return None
+        return field
```

### Comparing `data_connection-0.0.3/pyproject.toml` & `data_connection-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 
 [tool.black]
-line-length = 79
+line-length = 80
 
 
 [tool.poetry]
 authors = ["konstantin-dudersky <konstantin.dudersky@gmail.com>"]
 description = "Передача данных между сервисами"
 name = "data-connection"
 readme = "README.md"
 repository = "https://github.com/Konstantin-Dudersky/data_exchange.git"
-version = "0.0.3"
+version = "0.0.4"
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "3.11"
 
+asyncua = { version = "1.*", optional = true }
 fastapi = "0.*"
 pydantic = "1.*"
+pymodbus = { version = "3.*", optional = true }
 websockets = "10.*"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 wemake-python-styleguide = "0.17.0"
 poethepoet = "*"
 
 
+[tool.poetry.extras]
+opcua = ["asyncua"]
+modbus = ["pymodbus"]
+
+
 [tool.poe.tasks]
-lint = ["lint_flake8", "lint_pyright"]
-lint_flake8 = { shell = 'flake8 datapoints/' }
-lint_pyright = { shell = 'pyright' }           # npm install --global pyright
-main = { script = "src.main:entry" }
+lint = ["lint_pyright", "lint_flake8"]
+lint_flake8 = { shell = 'flake8 data_connection/' }
+lint_pyright = { shell = 'pyright' }
 
 
 [tool.pyright]
 pythonPlatform = "Linux"
 pythonVersion = "3.11"
+reportUnnecessaryTypeIgnoreComment = true
 stubPath = '.venv/typings'
 typeCheckingMode = "strict"
-venvPath = ".venv/bin/python3"
```

### Comparing `data_connection-0.0.3/setup.py` & `data_connection-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['data_connection']
+['data_connection', 'data_connection.readers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['fastapi<1.0.0', 'pydantic>=1.0.0,<2.0.0', 'websockets>=10.0.0,<11.0.0']
 
+extras_require = \
+{'modbus': ['pymodbus>=3.0.0,<4.0.0'], 'opcua': ['asyncua>=1.0.0,<2.0.0']}
+
 setup_kwargs = {
     'name': 'data-connection',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Передача данных между сервисами',
     'long_description': '# data_exchange\n\n## Описание\n\nОбмен данными между микросервисами\n\n- signal - элементарный тип данных. Кроме значения, хранит также время последнего чтения / записи, код качества, единицу измерения, пределы измерения.\n\n- channel - объект для связи signal с периферийными значениями.\n\n- driver - управляет объектами channel.\n\n- datapoint - объект для храненения данных. Связывает signal и channel.\n\n## Разработка\n\nУстановить виртуальное окружение\n\n```sh\npoetry install\n```\n\nСобрать пакет\n\n```sh\npoetry build\n```\n\nОпубликовать пакет\n\n```sh\npoetry publish --username Konstantin.Dudersky@gmail.com --password __TOKEN__\n```\n',
     'author': 'konstantin-dudersky',
     'author_email': 'konstantin.dudersky@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Konstantin-Dudersky/data_exchange.git',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.11,<4.0',
+    'extras_require': extras_require,
+    'python_requires': '>=3.11,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `data_connection-0.0.3/PKG-INFO` & `data_connection-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: data-connection
-Version: 0.0.3
+Version: 0.0.4
 Summary: Передача данных между сервисами
 Home-page: https://github.com/Konstantin-Dudersky/data_exchange.git
 Author: konstantin-dudersky
 Author-email: konstantin.dudersky@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: modbus
+Provides-Extra: opcua
+Requires-Dist: asyncua (>=1.0.0,<2.0.0); extra == "opcua"
 Requires-Dist: fastapi (<1.0.0)
 Requires-Dist: pydantic (>=1.0.0,<2.0.0)
+Requires-Dist: pymodbus (>=3.0.0,<4.0.0); extra == "modbus"
 Requires-Dist: websockets (>=10.0.0,<11.0.0)
 Project-URL: Repository, https://github.com/Konstantin-Dudersky/data_exchange.git
 Description-Content-Type: text/markdown
 
 # data_exchange
 
 ## Описание
```

