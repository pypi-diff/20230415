# Comparing `tmp/fastramqpi-1.3.8.tar.gz` & `tmp/fastramqpi-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-1.3.8.tar", max compression
+gzip compressed data, was "fastramqpi-1.3.9.tar", max compression
```

## Comparing `fastramqpi-1.3.8.tar` & `fastramqpi-1.3.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0        0        0        0 2023-02-27 10:14:27.528277 fastramqpi-1.3.8/LICENSES/
--rw-r--r--   0        0        0    15177 2023-02-27 10:14:27.528277 fastramqpi-1.3.8/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     2932 2023-02-27 10:14:27.529277 fastramqpi-1.3.8/README.md
--rw-r--r--   0        0        0       85 2023-02-27 10:14:27.529277 fastramqpi-1.3.8/fastramqpi/__init__.py
--rw-r--r--   0        0        0     2208 2023-02-27 10:14:27.529277 fastramqpi-1.3.8/fastramqpi/config.py
--rw-r--r--   0        0        0     1144 2023-02-27 10:14:27.529277 fastramqpi-1.3.8/fastramqpi/context.py
--rw-r--r--   0        0        0     7194 2023-02-27 10:14:27.529277 fastramqpi-1.3.8/fastramqpi/fastapi.py
--rw-r--r--   0        0        0     1558 2023-02-27 10:14:27.529277 fastramqpi-1.3.8/fastramqpi/healthcheck.py
--rw-r--r--   0        0        0     3899 2023-02-27 10:14:27.529277 fastramqpi-1.3.8/fastramqpi/main.py
--rw-r--r--   0        0        0        0 2023-02-27 10:14:27.596282 fastramqpi-1.3.8/fastramqpi/py.typed
--rw-r--r--   0        0        0     1377 2023-02-27 10:14:47.404552 fastramqpi-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 fastramqpi-1.3.8/setup.py
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 fastramqpi-1.3.8/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-03-08 12:47:24.103878 fastramqpi-1.3.9/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     2932 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/README.md
+-rw-r--r--   0        0        0       85 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     2208 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/config.py
+-rw-r--r--   0        0        0     1144 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/context.py
+-rw-r--r--   0        0        0     7194 2023-03-08 12:47:24.104878 fastramqpi-1.3.9/fastramqpi/fastapi.py
+-rw-r--r--   0        0        0     1573 2023-03-08 12:47:24.105878 fastramqpi-1.3.9/fastramqpi/healthcheck.py
+-rw-r--r--   0        0        0     3899 2023-03-08 12:47:24.105878 fastramqpi-1.3.9/fastramqpi/main.py
+-rw-r--r--   0        0        0        0 2023-03-08 12:47:24.151884 fastramqpi-1.3.9/fastramqpi/py.typed
+-rw-r--r--   0        0        0     1377 2023-03-08 12:47:40.872265 fastramqpi-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 fastramqpi-1.3.9/PKG-INFO
```

### Comparing `fastramqpi-1.3.8/LICENSES/MPL-2.0.txt` & `fastramqpi-1.3.9/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.8/README.md` & `fastramqpi-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.8/fastramqpi/config.py` & `fastramqpi-1.3.9/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.8/fastramqpi/context.py` & `fastramqpi-1.3.9/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.8/fastramqpi/fastapi.py` & `fastramqpi-1.3.9/fastramqpi/fastapi.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.8/fastramqpi/healthcheck.py` & `fastramqpi-1.3.9/fastramqpi/healthcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,14 @@
 
     Returns:
         Whether the client is healthy or not.
     """
     model_client = context["model_client"]
 
     try:
-        response = await model_client.get("/service/o/")
+        response = await model_client.async_httpx_client("/service/o/")
         result = response.json()
         if one(result)["uuid"]:
             return True
     except Exception:  # pylint: disable=broad-except
         logger.exception("Exception occured during GraphQL healthcheck")
     return False
```

### Comparing `fastramqpi-1.3.8/fastramqpi/main.py` & `fastramqpi-1.3.9/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.3.8/pyproject.toml` & `fastramqpi-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "1.3.8"
+version = "1.3.9"
 description = "Rammearkitektur AMQP framework (FastAPI + RAMQP)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo", "amqp"]
```

### Comparing `fastramqpi-1.3.8/PKG-INFO` & `fastramqpi-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastramqpi
-Version: 1.3.8
+Version: 1.3.9
 Summary: Rammearkitektur AMQP framework (FastAPI + RAMQP)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

