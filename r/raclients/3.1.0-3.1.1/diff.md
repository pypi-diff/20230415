# Comparing `tmp/raclients-3.1.0.tar.gz` & `tmp/raclients-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raclients-3.1.0.tar", max compression
+gzip compressed data, was "raclients-3.1.1.tar", max compression
```

## Comparing `raclients-3.1.0.tar` & `raclients-3.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0        0        0        0 2023-03-31 12:32:06.101789 raclients-3.1.0/LICENSES/
--rw-r--r--   0        0        0     1039 2023-03-31 12:32:06.101789 raclients-3.1.0/README.md
--rw-r--r--   0        0        0     1040 2023-03-31 12:32:07.270955 raclients-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      300 2023-03-31 12:32:06.103789 raclients-3.1.0/raclients/__init__.py
--rw-r--r--   0        0        0     6858 2023-03-31 12:32:06.103789 raclients-3.1.0/raclients/auth.py
--rw-r--r--   0        0        0       99 2023-03-31 12:32:06.103789 raclients-3.1.0/raclients/graph/__init__.py
--rw-r--r--   0        0        0     7259 2023-03-31 12:32:06.103789 raclients-3.1.0/raclients/graph/client.py
--rw-r--r--   0        0        0     9291 2023-03-31 12:32:06.103789 raclients-3.1.0/raclients/graph/transport.py
--rw-r--r--   0        0        0     3105 2023-03-31 12:32:06.104789 raclients-3.1.0/raclients/graph/util.py
--rw-r--r--   0        0        0       99 2023-03-31 12:32:06.104789 raclients-3.1.0/raclients/modelclient/__init__.py
--rw-r--r--   0        0        0     4356 2023-03-31 12:32:06.104789 raclients-3.1.0/raclients/modelclient/base.py
--rw-r--r--   0        0        0     1940 2023-03-31 12:32:06.104789 raclients-3.1.0/raclients/modelclient/lora.py
--rw-r--r--   0        0        0     5320 2023-03-31 12:32:06.104789 raclients-3.1.0/raclients/modelclient/mo.py
--rw-r--r--   0        0        0        0 2023-03-31 12:32:06.148796 raclients-3.1.0/raclients/py.typed
--rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 raclients-3.1.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-14 22:54:44.438256 raclients-3.1.1/LICENSES/
+-rw-r--r--   0        0        0     1039 2023-04-14 22:54:44.438256 raclients-3.1.1/README.md
+-rw-r--r--   0        0        0     1040 2023-04-14 22:54:45.976409 raclients-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-14 22:54:44.440256 raclients-3.1.1/raclients/__init__.py
+-rw-r--r--   0        0        0     6858 2023-04-14 22:54:44.440256 raclients-3.1.1/raclients/auth.py
+-rw-r--r--   0        0        0       99 2023-04-14 22:54:44.440256 raclients-3.1.1/raclients/graph/__init__.py
+-rw-r--r--   0        0        0     7259 2023-04-14 22:54:44.441256 raclients-3.1.1/raclients/graph/client.py
+-rw-r--r--   0        0        0     9291 2023-04-14 22:54:44.441256 raclients-3.1.1/raclients/graph/transport.py
+-rw-r--r--   0        0        0     3105 2023-04-14 22:54:44.441256 raclients-3.1.1/raclients/graph/util.py
+-rw-r--r--   0        0        0       99 2023-04-14 22:54:44.441256 raclients-3.1.1/raclients/modelclient/__init__.py
+-rw-r--r--   0        0        0     4356 2023-04-14 22:54:44.441256 raclients-3.1.1/raclients/modelclient/base.py
+-rw-r--r--   0        0        0     1940 2023-04-14 22:54:44.441256 raclients-3.1.1/raclients/modelclient/lora.py
+-rw-r--r--   0        0        0     5320 2023-04-14 22:54:44.442256 raclients-3.1.1/raclients/modelclient/mo.py
+-rw-r--r--   0        0        0        0 2023-04-14 22:54:44.490261 raclients-3.1.1/raclients/py.typed
+-rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 raclients-3.1.1/PKG-INFO
```

### Comparing `raclients-3.1.0/README.md` & `raclients-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/pyproject.toml` & `raclients-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raclients"
-version = "3.1.0"
+version = "3.1.1"
 description = "Clients for OS2mo/LoRa"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ra-clients"
 keywords = ["os2mo", "lora"]
```

### Comparing `raclients-3.1.0/raclients/auth.py` & `raclients-3.1.1/raclients/auth.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/raclients/graph/client.py` & `raclients-3.1.1/raclients/graph/client.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/raclients/graph/transport.py` & `raclients-3.1.1/raclients/graph/transport.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/raclients/graph/util.py` & `raclients-3.1.1/raclients/graph/util.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/raclients/modelclient/base.py` & `raclients-3.1.1/raclients/modelclient/base.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/raclients/modelclient/lora.py` & `raclients-3.1.1/raclients/modelclient/lora.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/raclients/modelclient/mo.py` & `raclients-3.1.1/raclients/modelclient/mo.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.0/PKG-INFO` & `raclients-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raclients
-Version: 3.1.0
+Version: 3.1.1
 Summary: Clients for OS2mo/LoRa
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,lora
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

