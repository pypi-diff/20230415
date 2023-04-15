# Comparing `tmp/sabledocs-0.1.tar.gz` & `tmp/sabledocs-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.1.tar", last modified: Sat Apr 15 20:04:30 2023, max compression
+gzip compressed data, was "sabledocs-0.1.43.tar", last modified: Sat Apr 15 20:04:38 2023, max compression
```

## Comparing `sabledocs-0.1.tar` & `sabledocs-0.1.43.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:30.192961 sabledocs-0.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 20:04:17.000000 sabledocs-0.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 20:04:17.000000 sabledocs-0.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3483 2023-04-15 20:04:30.192961 sabledocs-0.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-04-15 20:04:17.000000 sabledocs-0.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-04-15 20:04:17.000000 sabledocs-0.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2023-04-15 20:04:30.196961 sabledocs-0.1/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:30.184961 sabledocs-0.1/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:30.188961 sabledocs-0.1/src/sabledocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13639 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:30.184961 sabledocs-0.1/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:30.192961 sabledocs-0.1/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1850 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:30.192961 sabledocs-0.1/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 20:04:17.000000 sabledocs-0.1/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:30.188961 sabledocs-0.1/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3483 2023-04-15 20:04:30.000000 sabledocs-0.1/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 20:04:30.000000 sabledocs-0.1/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 20:04:30.000000 sabledocs-0.1/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 20:04:30.000000 sabledocs-0.1/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 20:04:30.000000 sabledocs-0.1/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:38.244964 sabledocs-0.1.43/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 20:04:17.000000 sabledocs-0.1.43/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 20:04:17.000000 sabledocs-0.1.43/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3486 2023-04-15 20:04:38.244964 sabledocs-0.1.43/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-04-15 20:04:17.000000 sabledocs-0.1.43/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-04-15 20:04:17.000000 sabledocs-0.1.43/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-04-15 20:04:38.244964 sabledocs-0.1.43/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:38.240964 sabledocs-0.1.43/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:38.240964 sabledocs-0.1.43/src/sabledocs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13639 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:38.240964 sabledocs-0.1.43/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:38.240964 sabledocs-0.1.43/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1850 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:38.240964 sabledocs-0.1.43/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 20:04:17.000000 sabledocs-0.1.43/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 20:04:38.240964 sabledocs-0.1.43/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3486 2023-04-15 20:04:38.000000 sabledocs-0.1.43/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 20:04:38.000000 sabledocs-0.1.43/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 20:04:38.000000 sabledocs-0.1.43/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 20:04:38.000000 sabledocs-0.1.43/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 20:04:38.000000 sabledocs-0.1.43/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.1/LICENSE` & `sabledocs-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/PKG-INFO` & `sabledocs-0.1.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.1
+Version: 0.1.43
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.1/README.md` & `sabledocs-0.1.43/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/pyproject.toml` & `sabledocs-0.1.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/__main__.py` & `sabledocs-0.1.43/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.1.43/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/proto_model.py` & `sabledocs-0.1.43/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/sable_config.py` & `sabledocs-0.1.43/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/base.html` & `sabledocs-0.1.43/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.1.43/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/index.html` & `sabledocs-0.1.43/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/message.html` & `sabledocs-0.1.43/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/package.html` & `sabledocs-0.1.43/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/service.html` & `sabledocs-0.1.43/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.1.43/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.1.43/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.1.43/src/sabledocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.1
+Version: 0.1.43
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.1/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.1.43/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

