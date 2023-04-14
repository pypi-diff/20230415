# Comparing `tmp/raclients-3.1.2.tar.gz` & `tmp/raclients-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raclients-3.1.2.tar", max compression
+gzip compressed data, was "raclients-3.1.3.tar", max compression
```

## Comparing `raclients-3.1.2.tar` & `raclients-3.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0        0        0        0 2023-04-14 23:11:56.903014 raclients-3.1.2/LICENSES/
--rw-r--r--   0        0        0     1039 2023-04-14 23:11:56.904014 raclients-3.1.2/README.md
--rw-r--r--   0        0        0     1049 2023-04-14 23:11:58.108134 raclients-3.1.2/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-14 23:11:56.905014 raclients-3.1.2/raclients/__init__.py
--rw-r--r--   0        0        0     6858 2023-04-14 23:11:56.905014 raclients-3.1.2/raclients/auth.py
--rw-r--r--   0        0        0       99 2023-04-14 23:11:56.906015 raclients-3.1.2/raclients/graph/__init__.py
--rw-r--r--   0        0        0     7259 2023-04-14 23:11:56.906015 raclients-3.1.2/raclients/graph/client.py
--rw-r--r--   0        0        0     9291 2023-04-14 23:11:56.906015 raclients-3.1.2/raclients/graph/transport.py
--rw-r--r--   0        0        0     3105 2023-04-14 23:11:56.906015 raclients-3.1.2/raclients/graph/util.py
--rw-r--r--   0        0        0       99 2023-04-14 23:11:56.906015 raclients-3.1.2/raclients/modelclient/__init__.py
--rw-r--r--   0        0        0     4356 2023-04-14 23:11:56.907015 raclients-3.1.2/raclients/modelclient/base.py
--rw-r--r--   0        0        0     1940 2023-04-14 23:11:56.907015 raclients-3.1.2/raclients/modelclient/lora.py
--rw-r--r--   0        0        0     5320 2023-04-14 23:11:56.907015 raclients-3.1.2/raclients/modelclient/mo.py
--rw-r--r--   0        0        0        0 2023-04-14 23:11:56.972021 raclients-3.1.2/raclients/py.typed
--rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 raclients-3.1.2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-14 23:15:33.026518 raclients-3.1.3/LICENSES/
+-rw-r--r--   0        0        0     1039 2023-04-14 23:15:33.026518 raclients-3.1.3/README.md
+-rw-r--r--   0        0        0     1054 2023-04-14 23:15:34.236638 raclients-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/__init__.py
+-rw-r--r--   0        0        0     6858 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/auth.py
+-rw-r--r--   0        0        0       99 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/graph/__init__.py
+-rw-r--r--   0        0        0     7259 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/graph/client.py
+-rw-r--r--   0        0        0     9291 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/graph/transport.py
+-rw-r--r--   0        0        0     3105 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/graph/util.py
+-rw-r--r--   0        0        0       99 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/__init__.py
+-rw-r--r--   0        0        0     4356 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/base.py
+-rw-r--r--   0        0        0     1940 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/lora.py
+-rw-r--r--   0        0        0     5320 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/mo.py
+-rw-r--r--   0        0        0        0 2023-04-14 23:15:33.072522 raclients-3.1.3/raclients/py.typed
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 raclients-3.1.3/PKG-INFO
```

### Comparing `raclients-3.1.2/README.md` & `raclients-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/pyproject.toml` & `raclients-3.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raclients"
-version = "3.1.2"
+version = "3.1.3"
 description = "Clients for OS2mo/LoRa"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ra-clients"
 keywords = ["os2mo", "lora"]
@@ -14,15 +14,15 @@
 python = "^3.10"
 tqdm = "^4.65.0"
 pydantic = "^1.10.5"
 fastapi = ">=0.88,<1.0"
 httpx = ">=0.23.3,<0.25.0"
 Authlib = "^1.2.0"
 gql = "^3.4.0"
-structlog = "^22.3.0"
+structlog = ">=22.3,<24.0"
 tenacity = "^8.2.2"
 more-itertools = "^9.1.0"
 ramodels = "^18.5.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.18.3"
```

### Comparing `raclients-3.1.2/raclients/auth.py` & `raclients-3.1.3/raclients/auth.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/raclients/graph/client.py` & `raclients-3.1.3/raclients/graph/client.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/raclients/graph/transport.py` & `raclients-3.1.3/raclients/graph/transport.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/raclients/graph/util.py` & `raclients-3.1.3/raclients/graph/util.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/raclients/modelclient/base.py` & `raclients-3.1.3/raclients/modelclient/base.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/raclients/modelclient/lora.py` & `raclients-3.1.3/raclients/modelclient/lora.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/raclients/modelclient/mo.py` & `raclients-3.1.3/raclients/modelclient/mo.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.2/PKG-INFO` & `raclients-3.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raclients
-Version: 3.1.2
+Version: 3.1.3
 Summary: Clients for OS2mo/LoRa
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,lora
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Requires-Dist: Authlib (>=1.2.0,<2.0.0)
 Requires-Dist: fastapi (>=0.88,<1.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.25.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: ramodels (>=18.5.2,<19.0.0)
-Requires-Dist: structlog (>=22.3.0,<23.0.0)
+Requires-Dist: structlog (>=22.3,<24.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/ra-clients
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>
```

