# Comparing `tmp/rlogging-1.0.7.tar.gz` & `tmp/rlogging-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.0.7.tar", max compression
+gzip compressed data, was "rlogging-1.1.0.tar", max compression
```

## Comparing `rlogging-1.0.7.tar` & `rlogging-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0     1375 2023-04-05 07:19:05.449274 rlogging-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      456 2023-04-05 07:19:05.449274 rlogging-1.0.7/readme.md
--rw-r--r--   0        0        0       65 2023-04-05 07:19:05.449274 rlogging-1.0.7/rlogging/__init__.py
--rw-r--r--   0        0        0     2608 2023-04-05 07:19:05.449274 rlogging-1.0.7/rlogging/adapters.py
--rw-r--r--   0        0        0      270 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/filters.py
--rw-r--r--   0        0        0     2240 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/formatters.py
--rw-r--r--   0        0        0      945 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-04-05 07:22:09.436162 rlogging-1.0.7/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 07:22:09.436162 rlogging-1.0.7/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 07:22:09.436162 rlogging-1.0.7/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      739 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      267 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-04-05 07:22:09.436162 rlogging-1.0.7/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-04-05 07:22:09.436162 rlogging-1.0.7/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/namespaces.py
--rw-r--r--   0        0        0     1851 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/settings.py
--rw-r--r--   0        0        0     1509 2023-04-05 07:19:05.453274 rlogging-1.0.7/rlogging/utils.py
--rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 rlogging-1.0.7/setup.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rlogging-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1393 2023-04-15 17:09:46.635115 rlogging-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      456 2023-04-05 07:19:05.449274 rlogging-1.1.0/readme.md
+-rw-r--r--   0        0        0       65 2023-04-15 17:09:46.635115 rlogging-1.1.0/rlogging/__init__.py
+-rw-r--r--   0        0        0     3236 2023-04-15 17:09:46.635115 rlogging-1.1.0/rlogging/adapters.py
+-rw-r--r--   0        0        0      270 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/filters.py
+-rw-r--r--   0        0        0     2339 2023-04-15 17:09:46.635115 rlogging-1.1.0/rlogging/formatters.py
+-rw-r--r--   0        0        0      945 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      740 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      125 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/admin.py
+-rw-r--r--   0        0        0      267 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1483 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0       72 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/models.py
+-rw-r--r--   0        0        0     2019 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1509 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/utils.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rlogging-1.1.0/PKG-INFO
```

### Comparing `rlogging-1.0.7/pyproject.toml` & `rlogging-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 django = "^4.1.7"
 black = "^23.1.0"
 ruff = "^0.0.257"
+isort = "^5.12.0"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 120
 
 [tool.isort]
 profile = "black"
```

### Comparing `rlogging-1.0.7/rlogging/formatters.py` & `rlogging-1.1.0/rlogging/formatters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from rlogging import utils
-
-import logging
 import json
+import logging
+
+from rlogging import utils
 
 
 class RsFormatter(logging.Formatter):
     """Кастомный форматер модуля"""
 
+    def enrichment(self, record: logging.LogRecord):
+        pass
+
     def format(self, record: logging.LogRecord):
         return super().format(record)
 
 
 class JsonFormatter(RsFormatter):
     """Форматер в json"""
 
@@ -55,14 +58,15 @@
 
         if self.exclude_fields:
             return {k: v for k, v in record_data.items() if k not in self.exclude_fields}
 
         return record_data
 
     def format(self, record: logging.LogRecord):
+        self.enrichment(record)
         record_data = self.get_data_from_record(record)
         return self.json_serializer(record_data, default=self.json_default, cls=self.json_cls)
 
 
 class ElkFormatter(JsonFormatter):
     def get_data_from_record(self, record: logging.LogRecord) -> dict:
         return utils.flatten_dict(super().get_data_from_record(record))
```

### Comparing `rlogging-1.0.7/rlogging/handlers.py` & `rlogging-1.1.0/rlogging/handlers.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from logging import FileHandler
-import time
 import os
+import time
+from logging import FileHandler
 
 
 class DailyFileHandler(FileHandler):
     DATE_FORMAT = '%Y-%m-%d'
 
     _origin_filename__name: str
     _origin_filename__ext: str
```

### Comparing `rlogging-1.0.7/rlogging/integration/django/adapters.py` & `rlogging-1.1.0/rlogging/integration/django/adapters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from rlogging import HttpLoggerAdapter
-from django.http import HttpRequest, HttpResponse
 from django.core.handlers.wsgi import WSGIRequest
+from django.http import HttpRequest, HttpResponse
+
+from rlogging import HttpLoggerAdapter
 
 
 class DjangoLoggerAdapter(HttpLoggerAdapter):
     def request(self, request: WSGIRequest, *args, **kwargs):
         kwargs.setdefault('stacklevel', 5)
 
         path = request.path
```

### Comparing `rlogging-1.0.7/rlogging/integration/django/middleware.py` & `rlogging-1.1.0/rlogging/integration/django/middleware.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
+from typing import Any
 
-from django.http import HttpResponse
 from django.core.handlers.wsgi import WSGIRequest
-from typing import Any
-from rlogging.integration.django.adapters import DjangoLoggerAdapter
-from rlogging import namespaces
 from django.db import connection
+from django.http import HttpResponse
 
+from rlogging import namespaces
+from rlogging.integration.django.adapters import DjangoLoggerAdapter
 from rlogging.utils import LazyStrCallable
 
 
 class LoggingMiddleware(object):
     def __init__(self, get_response):
         self.get_response = get_response
```

### Comparing `rlogging-1.0.7/rlogging/integration/django/signals.py` & `rlogging-1.1.0/rlogging/integration/django/signals.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.0.7/rlogging/utils.py` & `rlogging-1.1.0/rlogging/utils.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import traceback
 import types
-from typing import Any, Callable
 import uuid
+from typing import Any, Callable
 
 
 class LazyStrCallable(object):
     def __init__(self, target_func: Callable, *args, **kwargs) -> None:
         self.target = target_func
         self.args = args
         self.kwargs = kwargs
```

### Comparing `rlogging-1.0.7/PKG-INFO` & `rlogging-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlogging
-Version: 1.0.7
+Version: 1.1.0
 Summary: 
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

