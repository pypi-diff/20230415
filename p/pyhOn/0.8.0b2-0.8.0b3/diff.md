# Comparing `tmp/pyhOn-0.8.0b2.tar.gz` & `tmp/pyhOn-0.8.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.8.0b2.tar", last modified: Sat Apr 15 02:19:58 2023, max compression
+gzip compressed data, was "pyhOn-0.8.0b3.tar", last modified: Sat Apr 15 20:02:07 2023, max compression
```

## Comparing `pyhOn-0.8.0b2.tar` & `pyhOn-0.8.0b3.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.273452 pyhOn-0.8.0b2/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.273452 pyhOn-0.8.0b2/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.273452 pyhOn-0.8.0b2/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.586464 pyhOn-0.8.0b3/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/setup.py
```

### Comparing `pyhOn-0.8.0b2/LICENSE` & `pyhOn-0.8.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/PKG-INFO` & `pyhOn-0.8.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b2
+Version: 0.8.0b3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.0b2/README.md` & `pyhOn-0.8.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.0b3/pyhOn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b2
+Version: 0.8.0b3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.8.0b2/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.8.0b3/pyhOn.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,8 +21,12 @@
 pyhon/appliances/td.py
 pyhon/appliances/wd.py
 pyhon/appliances/wm.py
 pyhon/connection/__init__.py
 pyhon/connection/api.py
 pyhon/connection/auth.py
 pyhon/connection/device.py
-pyhon/connection/handler.py
+pyhon/connection/handler/__init__.py
+pyhon/connection/handler/anonym.py
+pyhon/connection/handler/auth.py
+pyhon/connection/handler/base.py
+pyhon/connection/handler/hon.py
```

### Comparing `pyhOn-0.8.0b2/pyhon/__main__.py` & `pyhOn-0.8.0b3/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/pyhon/appliance.py` & `pyhOn-0.8.0b3/pyhon/appliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import importlib
 from contextlib import suppress
-from typing import Optional, Dict
+from typing import Optional, Dict, Any
+from typing import TYPE_CHECKING
 
 from pyhon import helper
 from pyhon.commands import HonCommand
 from pyhon.parameter import HonParameterFixed
 
+if TYPE_CHECKING:
+    from pyhon import HonAPI
+
 
 class HonAppliance:
-    def __init__(self, api, info: Dict, zone: int = 0) -> None:
+    def __init__(
+        self, api: Optional["HonAPI"], info: Dict[str, Any], zone: int = 0
+    ) -> None:
         if attributes := info.get("attributes"):
             info["attributes"] = {v["parName"]: v["parValue"] for v in attributes}
-        self._info = info
-        self._api = api
-        self._appliance_model = {}
-
-        self._commands = {}
-        self._statistics = {}
-        self._attributes = {}
+        self._info: Dict = info
+        self._api: Optional[HonAPI] = api
+        self._appliance_model: Dict = {}
+
+        self._commands: Dict = {}
+        self._statistics: Dict = {}
+        self._attributes: Dict = {}
         self._zone = zone
 
         try:
             self._extra = importlib.import_module(
                 f"pyhon.appliances.{self.appliance_type.lower()}"
             ).Appliance()
         except ModuleNotFoundError:
@@ -54,22 +60,26 @@
         middle = " Z" if frontend else "_z"
         if (attribute := self._info.get(name, "")) and self._zone:
             return f"{attribute}{middle}{self._zone}"
         return attribute
 
     @property
     def appliance_model_id(self) -> str:
-        return self._info.get("applianceModelId")
+        return self._info.get("applianceModelId", "")
 
     @property
     def appliance_type(self) -> str:
-        return self._info.get("applianceTypeName")
+        return self._info.get("applianceTypeName", "")
 
     @property
     def mac_address(self) -> str:
+        return self.info.get("macAddress", "")
+
+    @property
+    def unique_id(self) -> str:
         return self._check_name_zone("macAddress", frontend=False)
 
     @property
     def model_name(self) -> str:
         return self._check_name_zone("modelName")
 
     @property
```

### Comparing `pyhOn-0.8.0b2/pyhon/appliances/ov.py` & `pyhOn-0.8.0b3/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/pyhon/commands.py` & `pyhOn-0.8.0b3/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/pyhon/connection/api.py` & `pyhOn-0.8.0b3/pyhon/connection/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from typing_extensions import Self
 
 from aiohttp import ClientSession
 
 from pyhon import const, exceptions
 from pyhon.appliance import HonAppliance
 from pyhon.connection.auth import HonAuth
-from pyhon.connection.handler import HonConnectionHandler, HonAnonymousConnectionHandler
+from pyhon.connection.handler.hon import HonConnectionHandler
+from pyhon.connection.handler.anonym import HonAnonymousConnectionHandler
 
 _LOGGER = logging.getLogger()
 
 
 class HonAPI:
     def __init__(
         self,
```

### Comparing `pyhOn-0.8.0b2/pyhon/connection/auth.py` & `pyhOn-0.8.0b3/pyhon/connection/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,268 +1,273 @@
 import json
 import logging
 import re
 import secrets
 import urllib
+from contextlib import suppress
+from dataclasses import dataclass
 from datetime import datetime, timedelta
 from pprint import pformat
-from typing import List, Tuple
+from typing import Dict, Optional, List
 from urllib import parse
 from urllib.parse import quote
 
+from aiohttp import ClientResponse
 from yarl import URL
 
 from pyhon import const, exceptions
+from pyhon.connection.handler.auth import HonAuthConnectionHandler
 
 _LOGGER = logging.getLogger(__name__)
 
 
+@dataclass
+class HonLoginData:
+    url: str = ""
+    email: str = ""
+    password: str = ""
+    fw_uid: str = ""
+    loaded: Optional[Dict] = None
+
+
 class HonAuth:
     _TOKEN_EXPIRES_AFTER_HOURS = 8
     _TOKEN_EXPIRE_WARNING_HOURS = 7
 
     def __init__(self, session, email, password, device) -> None:
         self._session = session
-        self._email = email
-        self._password = password
+        self._request = HonAuthConnectionHandler(session)
+        self._login_data = HonLoginData()
+        self._login_data.email = email
+        self._login_data.password = password
         self._access_token = ""
         self._refresh_token = ""
         self._cognito_token = ""
         self._id_token = ""
         self._device = device
-        self._called_urls: List[Tuple[int, str]] = []
         self._expires: datetime = datetime.utcnow()
 
     @property
-    def cognito_token(self):
+    def cognito_token(self) -> str:
         return self._cognito_token
 
     @property
-    def id_token(self):
+    def id_token(self) -> str:
         return self._id_token
 
     @property
-    def access_token(self):
+    def access_token(self) -> str:
         return self._access_token
 
     @property
-    def refresh_token(self):
+    def refresh_token(self) -> str:
         return self._refresh_token
 
-    def _check_token_expiration(self, hours):
+    def _check_token_expiration(self, hours: int) -> bool:
         return datetime.utcnow() >= self._expires + timedelta(hours=hours)
 
     @property
     def token_is_expired(self) -> bool:
         return self._check_token_expiration(self._TOKEN_EXPIRES_AFTER_HOURS)
 
     @property
     def token_expires_soon(self) -> bool:
         return self._check_token_expiration(self._TOKEN_EXPIRE_WARNING_HOURS)
 
-    async def _error_logger(self, response, fail=True):
-        result = "hOn Authentication Error\n"
-        for i, (status, url) in enumerate(self._called_urls):
-            result += f" {i + 1: 2d}     {status} - {url}\n"
-        result += f"ERROR - {response.status} - {response.request_info.url}\n"
-        result += f"{15 * '='} Response {15 * '='}\n{await response.text()}\n{40 * '='}"
-        _LOGGER.error(result)
+    async def _error_logger(self, response: ClientResponse, fail: bool = True) -> None:
+        output = "hOn Authentication Error\n"
+        for i, (status, url) in enumerate(self._request.called_urls):
+            output += f" {i + 1: 2d}     {status} - {url}\n"
+        output += f"ERROR - {response.status} - {response.request_info.url}\n"
+        output += f"{15 * '='} Response {15 * '='}\n{await response.text()}\n{40 * '='}"
+        _LOGGER.error(output)
         if fail:
             raise exceptions.HonAuthenticationError("Can't login")
 
-    async def _load_login(self):
+    @staticmethod
+    def _generate_nonce() -> str:
         nonce = secrets.token_hex(16)
-        nonce = f"{nonce[:8]}-{nonce[8:12]}-{nonce[12:16]}-{nonce[16:20]}-{nonce[20:]}"
+        return f"{nonce[:8]}-{nonce[8:12]}-{nonce[12:16]}-{nonce[16:20]}-{nonce[20:]}"
+
+    async def _load_login(self) -> bool:
+        login_url = await self._introduce()
+        login_url = await self._handle_redirects(login_url)
+        return await self._login_url(login_url)
+
+    async def _introduce(self) -> str:
+        redirect_uri = urllib.parse.quote(f"{const.APP}://mobilesdk/detect/oauth/done")
         params = {
             "response_type": "token+id_token",
             "client_id": const.CLIENT_ID,
-            "redirect_uri": urllib.parse.quote(
-                f"{const.APP}://mobilesdk/detect/oauth/done"
-            ),
+            "redirect_uri": redirect_uri,
             "display": "touch",
             "scope": "api openid refresh_token web",
-            "nonce": nonce,
+            "nonce": self._generate_nonce(),
         }
-        params = "&".join([f"{k}={v}" for k, v in params.items()])
-        async with self._session.get(
-            f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params}"
-        ) as response:
-            self._called_urls.append((response.status, response.request_info.url))
+        params_encode = "&".join([f"{k}={v}" for k, v in params.items()])
+        url = f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params_encode}"
+        async with self._request.get(url) as response:
             text = await response.text()
             self._expires = datetime.utcnow()
             if not (login_url := re.findall("url = '(.+?)'", text)):
                 if "oauth/done#access_token=" in text:
                     self._parse_token_data(text)
                     raise exceptions.HonNoAuthenticationNeeded()
                 await self._error_logger(response)
-                return False
-        async with self._session.get(login_url[0], allow_redirects=False) as redirect1:
-            self._called_urls.append((redirect1.status, redirect1.request_info.url))
-            if not (url := redirect1.headers.get("Location")):
-                await self._error_logger(redirect1)
-                return False
-        async with self._session.get(url, allow_redirects=False) as redirect2:
-            self._called_urls.append((redirect2.status, redirect2.request_info.url))
-            if not (
-                url := redirect2.headers.get("Location")
-                + "&System=IoT_Mobile_App&RegistrationSubChannel=hOn"
-            ):
-                await self._error_logger(redirect2)
-                return False
-        async with self._session.get(
-            URL(url, encoded=True), headers={"user-agent": const.USER_AGENT}
-        ) as login_screen:
-            self._called_urls.append(
-                (login_screen.status, login_screen.request_info.url)
-            )
-            if context := re.findall(
-                '"fwuid":"(.*?)","loaded":(\\{.*?})', await login_screen.text()
-            ):
+        return login_url[0]
+
+    async def _manual_redirect(self, url: str) -> str:
+        async with self._request.get(url, allow_redirects=False) as response:
+            if not (new_location := response.headers.get("Location", "")):
+                await self._error_logger(response)
+        return new_location
+
+    async def _handle_redirects(self, login_url) -> str:
+        redirect1 = await self._manual_redirect(login_url)
+        redirect2 = await self._manual_redirect(redirect1)
+        return f"{redirect2}&System=IoT_Mobile_App&RegistrationSubChannel=hOn"
+
+    async def _login_url(self, login_url: str) -> bool:
+        headers = {"user-agent": const.USER_AGENT}
+        url = URL(login_url, encoded=True)
+        async with self._request.get(url, headers=headers) as response:
+            text = await response.text()
+            if context := re.findall('"fwuid":"(.*?)","loaded":(\\{.*?})', text):
                 fw_uid, loaded_str = context[0]
-                loaded = json.loads(loaded_str)
-                login_url = login_url[0].replace(
+                self._login_data.fw_uid = fw_uid
+                self._login_data.loaded = json.loads(loaded_str)
+                self._login_data.url = login_url.replace(
                     "/".join(const.AUTH_API.split("/")[:-1]), ""
                 )
-                return fw_uid, loaded, login_url
-            await self._error_logger(login_screen)
+                return True
+            await self._error_logger(response)
         return False
 
-    async def _login(self, fw_uid, loaded, login_url):
-        data = {
-            "message": {
-                "actions": [
-                    {
-                        "id": "79;a",
-                        "descriptor": "apex://LightningLoginCustomController/ACTION$login",
-                        "callingDescriptor": "markup://c:loginForm",
-                        "params": {
-                            "username": quote(self._email),
-                            "password": quote(self._password),
-                            "startUrl": parse.unquote(
-                                login_url.split("startURL=")[-1]
-                            ).split("%3D")[0],
-                        },
-                    }
-                ]
+    async def _login(self) -> str:
+        start_url = self._login_data.url.rsplit("startURL=", maxsplit=1)[-1]
+        start_url = parse.unquote(start_url).split("%3D")[0]
+        action = {
+            "id": "79;a",
+            "descriptor": "apex://LightningLoginCustomController/ACTION$login",
+            "callingDescriptor": "markup://c:loginForm",
+            "params": {
+                "username": quote(self._login_data.email),
+                "password": quote(self._login_data.password),
+                "startUrl": start_url,
             },
+        }
+        data = {
+            "message": {"actions": [action]},
             "aura.context": {
                 "mode": "PROD",
-                "fwuid": fw_uid,
+                "fwuid": self._login_data.fw_uid,
                 "app": "siteforce:loginApp2",
-                "loaded": loaded,
+                "loaded": self._login_data.loaded,
                 "dn": [],
                 "globals": {},
                 "uad": False,
             },
-            "aura.pageURI": login_url,
+            "aura.pageURI": self._login_data.url,
             "aura.token": None,
         }
         params = {"r": 3, "other.LightningLoginCustom.login": 1}
-        async with self._session.post(
+        async with self._request.post(
             const.AUTH_API + "/s/sfsites/aura",
             headers={"Content-Type": "application/x-www-form-urlencoded"},
             data="&".join(f"{k}={json.dumps(v)}" for k, v in data.items()),
             params=params,
         ) as response:
-            self._called_urls.append((response.status, response.request_info.url))
             if response.status == 200:
-                try:
-                    data = await response.json()
-                    return data["events"][0]["attributes"]["values"]["url"]
-                except json.JSONDecodeError:
-                    pass
-                except KeyError:
-                    _LOGGER.error(
-                        "Can't get login url - %s", pformat(await response.json())
-                    )
+                with suppress(json.JSONDecodeError, KeyError):
+                    result = await response.json()
+                    return result["events"][0]["attributes"]["values"]["url"]
             await self._error_logger(response)
             return ""
 
-    def _parse_token_data(self, text):
+    def _parse_token_data(self, text: str) -> None:
         if access_token := re.findall("access_token=(.*?)&", text):
             self._access_token = access_token[0]
         if refresh_token := re.findall("refresh_token=(.*?)&", text):
             self._refresh_token = refresh_token[0]
         if id_token := re.findall("id_token=(.*?)&", text):
             self._id_token = id_token[0]
 
-    async def _get_token(self, url):
-        async with self._session.get(url) as response:
-            self._called_urls.append((response.status, response.request_info.url))
+    async def _get_token(self, url: str) -> bool:
+        async with self._request.get(url) as response:
             if response.status != 200:
                 await self._error_logger(response)
                 return False
-            url = re.findall("href\\s*=\\s*[\"'](.+?)[\"']", await response.text())
-            if not url:
+            url_search = re.findall(
+                "href\\s*=\\s*[\"'](.+?)[\"']", await response.text()
+            )
+            if not url_search:
                 await self._error_logger(response)
                 return False
-        if "ProgressiveLogin" in url[0]:
-            async with self._session.get(url[0]) as response:
-                self._called_urls.append((response.status, response.request_info.url))
+        if "ProgressiveLogin" in url_search[0]:
+            async with self._request.get(url_search[0]) as response:
                 if response.status != 200:
                     await self._error_logger(response)
                     return False
-                url = re.findall("href\\s*=\\s*[\"'](.*?)[\"']", await response.text())
-        url = "/".join(const.AUTH_API.split("/")[:-1]) + url[0]
-        async with self._session.get(url) as response:
-            self._called_urls.append((response.status, response.request_info.url))
+                url_search = re.findall(
+                    "href\\s*=\\s*[\"'](.*?)[\"']", await response.text()
+                )
+        url = "/".join(const.AUTH_API.split("/")[:-1]) + url_search[0]
+        async with self._request.get(url) as response:
             if response.status != 200:
                 await self._error_logger(response)
                 return False
             self._parse_token_data(await response.text())
         return True
 
-    async def _api_auth(self):
+    async def _api_auth(self) -> bool:
         post_headers = {"id-token": self._id_token}
         data = self._device.get()
-        async with self._session.post(
+        async with self._request.post(
             f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
         ) as response:
-            self._called_urls.append((response.status, response.request_info.url))
             try:
                 json_data = await response.json()
             except json.JSONDecodeError:
                 await self._error_logger(response)
                 return False
             self._cognito_token = json_data["cognitoUser"]["Token"]
         return True
 
-    async def authenticate(self):
+    async def authenticate(self) -> None:
         self.clear()
         try:
-            if not (login_site := await self._load_login()):
+            if not await self._load_login():
                 raise exceptions.HonAuthenticationError("Can't open login page")
-            if not (url := await self._login(*login_site)):
+            if not (url := await self._login()):
                 raise exceptions.HonAuthenticationError("Can't login")
             if not await self._get_token(url):
                 raise exceptions.HonAuthenticationError("Can't get token")
             if not await self._api_auth():
                 raise exceptions.HonAuthenticationError("Can't get api token")
         except exceptions.HonNoAuthenticationNeeded:
             return
 
-    async def refresh(self):
+    async def refresh(self) -> bool:
         params = {
             "client_id": const.CLIENT_ID,
             "refresh_token": self._refresh_token,
             "grant_type": "refresh_token",
         }
-        async with self._session.post(
+        async with self._request.post(
             f"{const.AUTH_API}/services/oauth2/token", params=params
         ) as response:
-            self._called_urls.append((response.status, response.request_info.url))
             if response.status >= 400:
                 await self._error_logger(response, fail=False)
                 return False
             data = await response.json()
         self._expires = datetime.utcnow()
         self._id_token = data["id_token"]
         self._access_token = data["access_token"]
         return await self._api_auth()
 
-    def clear(self):
+    def clear(self) -> None:
         self._session.cookie_jar.clear_domain(const.AUTH_API.split("/")[-2])
-        self._called_urls = []
+        self._request.called_urls = []
         self._cognito_token = ""
         self._id_token = ""
         self._access_token = ""
         self._refresh_token = ""
```

### Comparing `pyhOn-0.8.0b2/pyhon/connection/device.py` & `pyhOn-0.8.0b3/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/pyhon/helper.py` & `pyhOn-0.8.0b3/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/pyhon/hon.py` & `pyhOn-0.8.0b3/pyhon/hon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
-from typing import List, Optional, Dict
+import copy
+from typing import List, Optional, Dict, Any
 from typing_extensions import Self
 
 from aiohttp import ClientSession
 
 from pyhon import HonAPI, exceptions
 from pyhon.appliance import HonAppliance
 
@@ -35,28 +36,29 @@
         await self.setup()
         return self
 
     @property
     def appliances(self) -> List[HonAppliance]:
         return self._appliances
 
-    async def _create_appliance(self, appliance: Dict, zone=0) -> None:
-        appliance = HonAppliance(self._api, appliance, zone=zone)
+    async def _create_appliance(self, appliance_data: Dict[str, Any], zone=0) -> None:
+        appliance = HonAppliance(self._api, appliance_data, zone=zone)
         if appliance.mac_address is None:
             return
         await asyncio.gather(
             *[
                 appliance.load_attributes(),
                 appliance.load_commands(),
                 appliance.load_statistics(),
             ]
         )
         self._appliances.append(appliance)
 
     async def setup(self):
+        appliance: Dict
         for appliance in (await self._api.load_appliances())["payload"]["appliances"]:
             for zone in range(int(appliance.get("zone", "0"))):
-                await self._create_appliance(appliance, zone=zone + 1)
+                await self._create_appliance(appliance.copy(), zone=zone + 1)
             await self._create_appliance(appliance)
 
     async def close(self):
         await self._api.close()
```

### Comparing `pyhOn-0.8.0b2/pyhon/parameter.py` & `pyhOn-0.8.0b3/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b2/setup.py` & `pyhOn-0.8.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.8.0b2",
+    version="0.8.0b3",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

