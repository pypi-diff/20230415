# Comparing `tmp/sabledocs-0.1.51.tar.gz` & `tmp/sabledocs-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.1.51.tar", last modified: Sat Apr 15 20:20:51 2023, max compression
+gzip compressed data, was "sabledocs-0.1.54.tar", last modified: Sat Apr 15 20:28:03 2023, max compression
```

## Comparing `sabledocs-0.1.51.tar` & `sabledocs-0.1.54.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:51.318294 sabledocs-0.1.51/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 20:20:40.000000 sabledocs-0.1.51/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 20:20:40.000000 sabledocs-0.1.51/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3486 2023-04-15 20:20:51.318294 sabledocs-0.1.51/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-04-15 20:20:40.000000 sabledocs-0.1.51/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-04-15 20:20:40.000000 sabledocs-0.1.51/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-04-15 20:20:51.322294 sabledocs-0.1.51/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:51.318294 sabledocs-0.1.51/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:51.318294 sabledocs-0.1.51/src/sabledocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13639 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:51.318294 sabledocs-0.1.51/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:51.318294 sabledocs-0.1.51/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1850 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:51.318294 sabledocs-0.1.51/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 20:20:40.000000 sabledocs-0.1.51/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:20:51.318294 sabledocs-0.1.51/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3486 2023-04-15 20:20:51.000000 sabledocs-0.1.51/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 20:20:51.000000 sabledocs-0.1.51/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 20:20:51.000000 sabledocs-0.1.51/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 20:20:51.000000 sabledocs-0.1.51/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 20:20:51.000000 sabledocs-0.1.51/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:28:03.572740 sabledocs-0.1.54/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-04-15 20:27:44.000000 sabledocs-0.1.54/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-04-15 20:27:44.000000 sabledocs-0.1.54/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3486 2023-04-15 20:28:03.572740 sabledocs-0.1.54/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2950 2023-04-15 20:27:44.000000 sabledocs-0.1.54/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-04-15 20:27:44.000000 sabledocs-0.1.54/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       73 2023-04-15 20:28:03.576740 sabledocs-0.1.54/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:28:03.572740 sabledocs-0.1.54/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:28:03.572740 sabledocs-0.1.54/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2227 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13639 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2719 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:28:03.572740 sabledocs-0.1.54/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:28:03.572740 sabledocs-0.1.54/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:28:03.572740 sabledocs-0.1.54/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   257737 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-04-15 20:27:44.000000 sabledocs-0.1.54/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 20:28:03.572740 sabledocs-0.1.54/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3486 2023-04-15 20:28:03.000000 sabledocs-0.1.54/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-04-15 20:28:03.000000 sabledocs-0.1.54/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-15 20:28:03.000000 sabledocs-0.1.54/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-15 20:28:03.000000 sabledocs-0.1.54/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-04-15 20:28:03.000000 sabledocs-0.1.54/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.1.51/LICENSE` & `sabledocs-0.1.54/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/PKG-INFO` & `sabledocs-0.1.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.1.51
+Version: 0.1.54
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
```

### Comparing `sabledocs-0.1.51/README.md` & `sabledocs-0.1.54/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/pyproject.toml` & `sabledocs-0.1.54/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "sabledocs"
 version = "0.1"
 authors = [
   { name="Mark Vincze", email="mrk.vincze@gmail.com" },
 ]
 description = "Static documentation generator for Protobuf and gRPC"
 readme = "README.md"
-requires-python = ">=3.10.0"
+requires-python = ">=3.11.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `sabledocs-0.1.51/src/sabledocs/__main__.py` & `sabledocs-0.1.54/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.1.54/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/proto_model.py` & `sabledocs-0.1.54/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/sable_config.py` & `sabledocs-0.1.54/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/base.html` & `sabledocs-0.1.54/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.1.54/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/index.html` & `sabledocs-0.1.54/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/message.html` & `sabledocs-0.1.54/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/package.html` & `sabledocs-0.1.54/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/service.html` & `sabledocs-0.1.54/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.1.54/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.1.54/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.51/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.1.54/src/sabledocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.1.51
+Version: 0.1.54
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
```

### Comparing `sabledocs-0.1.51/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.1.54/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

