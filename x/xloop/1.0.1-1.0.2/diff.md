# Comparing `tmp/xloop-1.0.1.tar.gz` & `tmp/xloop-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xloop-1.0.1.tar", max compression
+gzip compressed data, was "xloop-1.0.2.tar", max compression
```

## Comparing `xloop-1.0.1.tar` & `xloop-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      907 2022-12-26 19:23:16.146055 xloop-1.0.1/LICENSE
--rw-r--r--   0        0        0     1063 2022-12-26 19:23:16.146055 xloop-1.0.1/README.md
--rw-r--r--   0        0        0     1374 2022-12-26 19:23:16.146055 xloop-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5405 2022-12-26 19:23:16.146055 xloop-1.0.1/xloop/__init__.py
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 xloop-1.0.1/setup.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 xloop-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:11:48.844024 xloop-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1063 2023-04-15 14:11:48.844024 xloop-1.0.2/README.md
+-rw-r--r--   0        0        0     1418 2023-04-15 14:11:48.844024 xloop-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5405 2023-04-15 14:11:48.844024 xloop-1.0.2/xloop/__init__.py
+-rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 xloop-1.0.2/PKG-INFO
```

### Comparing `xloop-1.0.1/README.md` & `xloop-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xloop-1.0.1/pyproject.toml` & `xloop-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "xloop"
-version = "1.0.1"
+version = "1.0.2"
 description = "General purpose for/iterator looping generators/utilities."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xloop"}]
 readme = "README.md"
-license = "MIT"
 repository = "https://github.com/xyngular/py-xloop"
 keywords = ["forloop", "loop", "list", "generator", "utilites"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `xloop-1.0.1/xloop/__init__.py` & `xloop-1.0.2/xloop/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union, Iterator, Iterable, TypeVar, Set, Type, Tuple
 
 T = TypeVar("T")
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 DEFAULT_NOT_ITERATE = (str, int, bytes)
 
 
 def xloop(
     *args: Union[Iterable[T], T],
     not_iterate: Iterable[Type] = DEFAULT_NOT_ITERATE,
```

### Comparing `xloop-1.0.1/PKG-INFO` & `xloop-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: xloop
-Version: 1.0.1
+Version: 1.0.2
 Summary: General purpose for/iterator looping generators/utilities.
 Home-page: https://github.com/xyngular/py-xloop
-License: MIT
 Keywords: forloop,loop,list,generator,utilites
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
 Project-URL: Repository, https://github.com/xyngular/py-xloop
```

