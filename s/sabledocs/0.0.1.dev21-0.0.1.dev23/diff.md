# Comparing `tmp/sabledocs-0.0.1.dev21.tar.gz` & `tmp/sabledocs-0.0.1.dev23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.0.1.dev21.tar", last modified: Sat Apr 15 11:54:02 2023, max compression
+gzip compressed data, was "sabledocs-0.0.1.dev23.tar", last modified: Sat Apr 15 12:04:32 2023, max compression
```

## Comparing `sabledocs-0.0.1.dev21.tar` & `sabledocs-0.0.1.dev23.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:54:02.720501 sabledocs-0.0.1.dev21/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-04-15 11:54:02.720501 sabledocs-0.0.1.dev21/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      325 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 11:54:02.720501 sabledocs-0.0.1.dev21/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:54:02.716501 sabledocs-0.0.1.dev21/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:54:02.716501 sabledocs-0.0.1.dev21/src/sabledocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2201 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13572 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1903 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:54:02.716501 sabledocs-0.0.1.dev21/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:54:02.720501 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:54:02.720501 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 11:53:51.000000 sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 11:54:02.720501 sabledocs-0.0.1.dev21/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-04-15 11:54:02.000000 sabledocs-0.0.1.dev21/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 11:54:02.000000 sabledocs-0.0.1.dev21/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 11:54:02.000000 sabledocs-0.0.1.dev21/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 11:54:02.000000 sabledocs-0.0.1.dev21/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 11:54:02.000000 sabledocs-0.0.1.dev21/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:32.935319 sabledocs-0.0.1.dev23/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-04-15 12:04:32.935319 sabledocs-0.0.1.dev23/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      325 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 12:04:32.935319 sabledocs-0.0.1.dev23/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:32.931318 sabledocs-0.0.1.dev23/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:32.931318 sabledocs-0.0.1.dev23/src/sabledocs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2201 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13572 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1903 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:32.931318 sabledocs-0.0.1.dev23/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:32.935319 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:32.935319 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 12:04:21.000000 sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 12:04:32.935319 sabledocs-0.0.1.dev23/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-04-15 12:04:32.000000 sabledocs-0.0.1.dev23/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 12:04:32.000000 sabledocs-0.0.1.dev23/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 12:04:32.000000 sabledocs-0.0.1.dev23/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 12:04:32.000000 sabledocs-0.0.1.dev23/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 12:04:32.000000 sabledocs-0.0.1.dev23/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.0.1.dev21/LICENSE` & `sabledocs-0.0.1.dev23/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/PKG-INFO` & `sabledocs-0.0.1.dev23/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.1.dev21
+Version: 0.0.1.dev23
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.0.1.dev21/pyproject.toml` & `sabledocs-0.0.1.dev23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/__main__.py` & `sabledocs-0.0.1.dev23/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.0.1.dev23/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/proto_model.py` & `sabledocs-0.0.1.dev23/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/sable_config.py` & `sabledocs-0.0.1.dev23/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/base.html` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/index.html` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/message.html` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/package.html` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/service.html` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.0.1.dev23/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.0.1.dev23/src/sabledocs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.1.dev21
+Version: 0.0.1.dev23
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.0.1.dev21/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.0.1.dev23/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

