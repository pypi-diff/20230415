# Comparing `tmp/databutton_logger-0.9.2.tar.gz` & `tmp/databutton_logger-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databutton_logger-0.9.2.tar", max compression
+gzip compressed data, was "databutton_logger-0.9.3.tar", max compression
```

## Comparing `databutton_logger-0.9.2.tar` & `databutton_logger-0.9.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       77 2023-04-15 16:09:06.118775 databutton_logger-0.9.2/databutton_logger/__init__.py
--rw-r--r--   0        0        0     3021 2023-04-15 16:08:33.162604 databutton_logger-0.9.2/databutton_logger/logger.py
--rw-r--r--   0        0        0     1335 2023-04-15 16:08:33.162604 databutton_logger-0.9.2/databutton_logger/middleware.py
--rw-r--r--   0        0        0      838 2023-04-15 16:09:06.126774 databutton_logger-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 databutton_logger-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-04-15 16:18:50.427987 databutton_logger-0.9.3/databutton_logger/__init__.py
+-rw-r--r--   0        0        0     3021 2023-04-15 16:18:29.339751 databutton_logger-0.9.3/databutton_logger/logger.py
+-rw-r--r--   0        0        0     1335 2023-04-15 16:18:29.339751 databutton_logger-0.9.3/databutton_logger/middleware.py
+-rw-r--r--   0        0        0      869 2023-04-15 16:18:50.435988 databutton_logger-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 databutton_logger-0.9.3/PKG-INFO
```

### Comparing `databutton_logger-0.9.2/databutton_logger/logger.py` & `databutton_logger-0.9.3/databutton_logger/logger.py`

 * *Files identical despite different names*

### Comparing `databutton_logger-0.9.2/databutton_logger/middleware.py` & `databutton_logger-0.9.3/databutton_logger/middleware.py`

 * *Files identical despite different names*

### Comparing `databutton_logger-0.9.2/pyproject.toml` & `databutton_logger-0.9.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "databutton-logger"
-version = "0.9.2"
+version = "0.9.3"
 description = "Logger utilities for databutton"
 authors = ["Databutton"]
 packages = [
   { include = "databutton_logger"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-asgi-correlation-id = "^4.1.0"
-fastapi = ">=0.80"
-loguru = "^0.7.0"
-httpx = "^0.24.0"
+asgi-correlation-id = ">=3.0.0,<5.0.0"
+fastapi = ">=0.65.0,<1.0"
+loguru = ">=0.5.0,<1.0.0"
+httpx = ">=0.18.0,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.8.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 python-semantic-release = "^7.31.4"
```

### Comparing `databutton_logger-0.9.2/PKG-INFO` & `databutton_logger-0.9.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: databutton-logger
-Version: 0.9.2
+Version: 0.9.3
 Summary: Logger utilities for databutton
 Author: Databutton
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asgi-correlation-id (>=4.1.0,<5.0.0)
-Requires-Dist: fastapi (>=0.80)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: asgi-correlation-id (>=3.0.0,<5.0.0)
+Requires-Dist: fastapi (>=0.65.0,<1.0)
+Requires-Dist: httpx (>=0.18.0,<1.0.0)
+Requires-Dist: loguru (>=0.5.0,<1.0.0)
```

