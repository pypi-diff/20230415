# Comparing `tmp/xsettings-1.3.0.tar.gz` & `tmp/xsettings-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsettings-1.3.0.tar", max compression
+gzip compressed data, was "xsettings-1.3.1.tar", max compression
```

## Comparing `xsettings-1.3.0.tar` & `xsettings-1.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      907 2023-03-27 20:35:07.193029 xsettings-1.3.0/LICENSE
--rw-r--r--   0        0        0     5147 2023-03-27 20:35:07.193029 xsettings-1.3.0/README.md
--rw-r--r--   0        0        0     1614 2023-03-27 20:35:07.193029 xsettings-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      277 2023-03-27 20:35:07.193029 xsettings-1.3.0/xsettings/__init__.py
--rw-r--r--   0        0        0     1378 2023-03-27 20:35:07.193029 xsettings-1.3.0/xsettings/default_converters.py
--rw-r--r--   0        0        0     1014 2023-03-27 20:35:07.193029 xsettings-1.3.0/xsettings/env_settings.py
--rw-r--r--   0        0        0      274 2023-03-27 20:35:07.193029 xsettings-1.3.0/xsettings/errors.py
--rw-r--r--   0        0        0    23318 2023-03-27 20:35:07.197030 xsettings-1.3.0/xsettings/fields.py
--rw-r--r--   0        0        0     3886 2023-03-27 20:35:07.197030 xsettings-1.3.0/xsettings/retreivers.py
--rw-r--r--   0        0        0    28058 2023-03-27 20:35:07.197030 xsettings-1.3.0/xsettings/settings.py
--rw-r--r--   0        0        0     6130 1970-01-01 00:00:00.000000 xsettings-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:12:05.477291 xsettings-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5147 2023-04-15 14:12:05.477291 xsettings-1.3.1/README.md
+-rw-r--r--   0        0        0     1658 2023-04-15 14:12:05.477291 xsettings-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-04-15 14:12:05.477291 xsettings-1.3.1/xsettings/__init__.py
+-rw-r--r--   0        0        0     1378 2023-04-15 14:12:05.477291 xsettings-1.3.1/xsettings/default_converters.py
+-rw-r--r--   0        0        0     1014 2023-04-15 14:12:05.477291 xsettings-1.3.1/xsettings/env_settings.py
+-rw-r--r--   0        0        0      274 2023-04-15 14:12:05.477291 xsettings-1.3.1/xsettings/errors.py
+-rw-r--r--   0        0        0    23318 2023-04-15 14:12:05.477291 xsettings-1.3.1/xsettings/fields.py
+-rw-r--r--   0        0        0     3886 2023-04-15 14:12:05.477291 xsettings-1.3.1/xsettings/retreivers.py
+-rw-r--r--   0        0        0    28058 2023-04-15 14:12:05.477291 xsettings-1.3.1/xsettings/settings.py
+-rw-r--r--   0        0        0     6131 1970-01-01 00:00:00.000000 xsettings-1.3.1/PKG-INFO
```

### Comparing `xsettings-1.3.0/README.md` & `xsettings-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `xsettings-1.3.0/pyproject.toml` & `xsettings-1.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "xsettings"
-version = "1.3.0"
+version = "1.3.1"
 description = "Ways to document, centeralize, retreive and validate settings."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xsettings"}]
 readme = "README.md"
-license = "MIT"
 repository = "https://github.com/xyngular/py-xsettings"
 keywords = ["settings", "lazy", "configuration"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 xsentinels = "^1.2.0"
 xinject = "^1.2.0"
```

### Comparing `xsettings-1.3.0/xsettings/default_converters.py` & `xsettings-1.3.1/xsettings/default_converters.py`

 * *Files identical despite different names*

### Comparing `xsettings-1.3.0/xsettings/env_settings.py` & `xsettings-1.3.1/xsettings/env_settings.py`

 * *Files identical despite different names*

### Comparing `xsettings-1.3.0/xsettings/fields.py` & `xsettings-1.3.1/xsettings/fields.py`

 * *Files identical despite different names*

### Comparing `xsettings-1.3.0/xsettings/retreivers.py` & `xsettings-1.3.1/xsettings/retreivers.py`

 * *Files identical despite different names*

### Comparing `xsettings-1.3.0/xsettings/settings.py` & `xsettings-1.3.1/xsettings/settings.py`

 * *Files identical despite different names*

### Comparing `xsettings-1.3.0/PKG-INFO` & `xsettings-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: xsettings
-Version: 1.3.0
+Version: 1.3.1
 Summary: Ways to document, centeralize, retreive and validate settings.
 Home-page: https://github.com/xyngular/py-xsettings
-License: MIT
 Keywords: settings,lazy,configuration
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ciso8601 (>=2.3.0,<3.0.0)
```

