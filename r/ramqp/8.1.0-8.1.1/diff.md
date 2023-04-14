# Comparing `tmp/ramqp-8.1.0.tar.gz` & `tmp/ramqp-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.1.0.tar", max compression
+gzip compressed data, was "ramqp-8.1.1.tar", max compression
```

## Comparing `ramqp-8.1.0.tar` & `ramqp-8.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-04-11 08:09:00.135649 ramqp-8.1.0/LICENSES/
--rw-r--r--   0        0        0    15177 2023-04-11 08:09:00.135649 ramqp-8.1.0/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-04-11 08:09:00.136649 ramqp-8.1.0/README.md
--rw-r--r--   0        0        0     1460 2023-04-11 08:09:12.955474 ramqp-8.1.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-11 08:09:00.137649 ramqp-8.1.0/ramqp/__init__.py
--rw-r--r--   0        0        0    13047 2023-04-11 08:09:00.138649 ramqp-8.1.0/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-04-11 08:09:00.138649 ramqp-8.1.0/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-04-11 08:09:00.138649 ramqp-8.1.0/ramqp/config.py
--rw-r--r--   0        0        0     8841 2023-04-11 08:09:00.138649 ramqp-8.1.0/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-04-11 08:09:00.139649 ramqp-8.1.0/ramqp/metrics.py
--rw-r--r--   0        0        0     8249 2023-04-11 08:09:00.139649 ramqp-8.1.0/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-04-11 08:09:00.209653 ramqp-8.1.0/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-04-11 08:09:00.139649 ramqp-8.1.0/ramqp/utils.py
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.1.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-14 22:44:19.033020 ramqp-8.1.1/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-04-14 22:44:19.033020 ramqp-8.1.1/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-04-14 22:44:19.034021 ramqp-8.1.1/README.md
+-rw-r--r--   0        0        0     1460 2023-04-14 22:44:36.229732 ramqp-8.1.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-04-14 22:44:19.035020 ramqp-8.1.1/ramqp/__init__.py
+-rw-r--r--   0        0        0    13047 2023-04-14 22:44:19.035020 ramqp-8.1.1/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-04-14 22:44:19.035020 ramqp-8.1.1/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-04-14 22:44:19.036021 ramqp-8.1.1/ramqp/config.py
+-rw-r--r--   0        0        0     8841 2023-04-14 22:44:19.036021 ramqp-8.1.1/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-04-14 22:44:19.036021 ramqp-8.1.1/ramqp/metrics.py
+-rw-r--r--   0        0        0     8249 2023-04-14 22:44:19.036021 ramqp-8.1.1/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-04-14 22:44:19.170034 ramqp-8.1.1/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-04-14 22:44:19.037021 ramqp-8.1.1/ramqp/utils.py
+-rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.1.1/PKG-INFO
```

### Comparing `ramqp-8.1.0/LICENSES/MPL-2.0.txt` & `ramqp-8.1.1/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/README.md` & `ramqp-8.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/pyproject.toml` & `ramqp-8.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.1.0"
+version = "8.1.1"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-8.1.0/ramqp/abstract.py` & `ramqp-8.1.1/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/ramqp/amqp.py` & `ramqp-8.1.1/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/ramqp/config.py` & `ramqp-8.1.1/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/ramqp/depends.py` & `ramqp-8.1.1/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/ramqp/metrics.py` & `ramqp-8.1.1/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/ramqp/mo.py` & `ramqp-8.1.1/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/ramqp/utils.py` & `ramqp-8.1.1/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.0/PKG-INFO` & `ramqp-8.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.1.0
+Version: 8.1.1
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

