# Comparing `tmp/sabledocs-0.0.1.dev27.tar.gz` & `tmp/sabledocs-0.0.2.dev29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.0.1.dev27.tar", last modified: Sat Apr 15 12:59:38 2023, max compression
+gzip compressed data, was "sabledocs-0.0.2.dev29.tar", last modified: Sat Apr 15 13:02:27 2023, max compression
```

## Comparing `sabledocs-0.0.1.dev27.tar` & `sabledocs-0.0.2.dev29.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2096 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1555 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 12:59:38.676445 sabledocs-0.0.1.dev27/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/src/sabledocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2260 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13581 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2116 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 12:59:21.000000 sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:59:38.672445 sabledocs-0.0.1.dev27/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2096 2023-04-15 12:59:38.000000 sabledocs-0.0.1.dev27/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 12:59:38.000000 sabledocs-0.0.1.dev27/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 12:59:38.000000 sabledocs-0.0.1.dev27/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 12:59:38.000000 sabledocs-0.0.1.dev27/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 12:59:38.000000 sabledocs-0.0.1.dev27/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.885470 sabledocs-0.0.2.dev29/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:02:27.885470 sabledocs-0.0.2.dev29/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 13:02:27.885470 sabledocs-0.0.2.dev29/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2260 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13581 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2116 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.0.1.dev27/LICENSE` & `sabledocs-0.0.2.dev29/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/PKG-INFO` & `sabledocs-0.0.2.dev29/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.1.dev27
+Version: 0.0.2.dev29
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sable-docs
+# sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
 
 A simple static documentation generator for Protobuf and gRPC contracts.
 
 ## How to use
```

### Comparing `sabledocs-0.0.1.dev27/README.md` & `sabledocs-0.0.2.dev29/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# sable-docs
+# sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
 
 A simple static documentation generator for Protobuf and gRPC contracts.
 
 ## How to use
```

### Comparing `sabledocs-0.0.1.dev27/pyproject.toml` & `sabledocs-0.0.2.dev29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sabledocs"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mark Vincze", email="mrk.vincze@gmail.com" },
 ]
 description = "Static documentation generator for Protobuf and gRPC"
 readme = "README.md"
 requires-python = ">=3.11.0"
 classifiers = [
```

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/__main__.py` & `sabledocs-0.0.2.dev29/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.0.2.dev29/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/proto_model.py` & `sabledocs-0.0.2.dev29/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/sable_config.py` & `sabledocs-0.0.2.dev29/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/base.html` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/index.html` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/message.html` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/package.html` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/service.html` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.0.2.dev29/src/sabledocs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.1.dev27
+Version: 0.0.2.dev29
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sable-docs
+# sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
 
 A simple static documentation generator for Protobuf and gRPC contracts.
 
 ## How to use
```

### Comparing `sabledocs-0.0.1.dev27/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.0.2.dev29/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

