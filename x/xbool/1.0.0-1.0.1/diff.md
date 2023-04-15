# Comparing `tmp/xbool-1.0.0.tar.gz` & `tmp/xbool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbool-1.0.0.tar", max compression
+gzip compressed data, was "xbool-1.0.1.tar", max compression
```

## Comparing `xbool-1.0.0.tar` & `xbool-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      907 2022-12-26 19:23:12.562950 xbool-1.0.0/LICENSE
--rw-r--r--   0        0        0     2476 2022-12-26 19:23:12.562950 xbool-1.0.0/README.md
--rw-r--r--   0        0        0     1400 2022-12-26 19:23:12.562950 xbool-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3520 2022-12-26 19:23:12.562950 xbool-1.0.0/xbool/__init__.py
--rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 xbool-1.0.0/setup.py
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 xbool-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:11:21.341333 xbool-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2476 2023-04-15 14:11:21.341333 xbool-1.0.1/README.md
+-rw-r--r--   0        0        0     1444 2023-04-15 14:11:21.341333 xbool-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3520 2023-04-15 14:11:21.345333 xbool-1.0.1/xbool/__init__.py
+-rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 xbool-1.0.1/PKG-INFO
```

### Comparing `xbool-1.0.0/README.md` & `xbool-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xbool-1.0.0/pyproject.toml` & `xbool-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "xbool"
-version = "1.0.0"
+version = "1.0.1"
 description = "General purpose bool/boolean utilities, extracting bools from strings."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xbool"}]
 readme = "README.md"
-license = "MIT"
 repository = "https://github.com/xyngular/py-xbool"
 keywords = ["bool", "booltostr", "str", "environmental variable", "utilites"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `xbool-1.0.0/xbool/__init__.py` & `xbool-1.0.1/xbool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.util import strtobool
 from typing import Any
 import os
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 
 def bool_value(value: Any):
     """
     Does our best to get the 'bool' value from any other value.
     If you pass in a string, we use the built-in `distutils.util.strtobool` function to parse bool
     values from strings/text.
```

### Comparing `xbool-1.0.0/PKG-INFO` & `xbool-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: xbool
-Version: 1.0.0
+Version: 1.0.1
 Summary: General purpose bool/boolean utilities, extracting bools from strings.
 Home-page: https://github.com/xyngular/py-xbool
-License: MIT
 Keywords: bool,booltostr,str,environmental variable,utilites
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
 Project-URL: Repository, https://github.com/xyngular/py-xbool
```

