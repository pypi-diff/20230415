# Comparing `tmp/xmodel-0.3.0.tar.gz` & `tmp/xmodel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmodel-0.3.0.tar", max compression
+gzip compressed data, was "xmodel-0.3.1.tar", max compression
```

## Comparing `xmodel-0.3.0.tar` & `xmodel-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1211 2023-04-15 03:16:28.299921 xmodel-0.3.0/LICENSE
--rw-r--r--   0        0        0      697 2023-04-15 03:16:28.299921 xmodel-0.3.0/README.md
--rw-r--r--   0        0        0     1965 2023-04-15 03:16:28.299921 xmodel-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    20864 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/__init__.py
--rw-r--r--   0        0        0       18 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/__init__.py
--rw-r--r--   0        0        0       33 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/api/__init__.py
--rw-r--r--   0        0        0     7004 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/api/state.py
--rw-r--r--   0        0        0      828 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/api/utils.py
--rw-r--r--   0        0        0      191 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/__init__.py
--rw-r--r--   0        0        0    48954 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/api.py
--rw-r--r--   0        0        0    35396 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/fields.py
--rw-r--r--   0        0        0    29418 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/model.py
--rw-r--r--   0        0        0    21759 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/structure.py
--rw-r--r--   0        0        0        1 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/__init__.py
--rw-r--r--   0        0        0    13348 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/children.py
--rw-r--r--   0        0        0     1943 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/lazy.py
--rw-r--r--   0        0        0      963 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/types.py
--rw-r--r--   0        0        0     1635 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/unwrap.py
--rw-r--r--   0        0        0     2555 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/utils.py
--rw-r--r--   0        0        0     7716 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/converters.py
--rw-r--r--   0        0        0       89 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/errors.py
--rw-r--r--   0        0        0      804 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/json.py
--rw-r--r--   0        0        0      273 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/__init__.py
--rw-r--r--   0        0        0    30698 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/api.py
--rw-r--r--   0        0        0     7828 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/client.py
--rw-r--r--   0        0        0      301 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/errors.py
--rw-r--r--   0        0        0     2235 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/model.py
--rw-r--r--   0        0        0     3112 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/options.py
--rw-r--r--   0        0        0    12775 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/response_state.py
--rw-r--r--   0        0        0     6709 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/structure.py
--rw-r--r--   0        0        0     7935 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/weak_cache_pool.py
--rw-r--r--   0        0        0      240 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/util.py
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 xmodel-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:12:05.475085 xmodel-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1046 2023-04-15 14:12:05.475085 xmodel-0.3.1/README.md
+-rw-r--r--   0        0        0     2072 2023-04-15 14:12:05.475085 xmodel-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    20864 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/api/__init__.py
+-rw-r--r--   0        0        0     7004 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/api/state.py
+-rw-r--r--   0        0        0      828 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/api/utils.py
+-rw-r--r--   0        0        0      191 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/base/__init__.py
+-rw-r--r--   0        0        0    48954 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/base/api.py
+-rw-r--r--   0        0        0    35396 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/base/fields.py
+-rw-r--r--   0        0        0    29418 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/base/model.py
+-rw-r--r--   0        0        0    21759 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/base/structure.py
+-rw-r--r--   0        0        0        1 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/__init__.py
+-rw-r--r--   0        0        0    13348 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/children.py
+-rw-r--r--   0        0        0     1943 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/lazy.py
+-rw-r--r--   0        0        0      963 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/types.py
+-rw-r--r--   0        0        0     1635 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/unwrap.py
+-rw-r--r--   0        0        0     2555 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/utils.py
+-rw-r--r--   0        0        0     7716 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/converters.py
+-rw-r--r--   0        0        0       89 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/errors.py
+-rw-r--r--   0        0        0      804 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/json.py
+-rw-r--r--   0        0        0      273 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/__init__.py
+-rw-r--r--   0        0        0    30698 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/api.py
+-rw-r--r--   0        0        0     7828 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/client.py
+-rw-r--r--   0        0        0      301 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/errors.py
+-rw-r--r--   0        0        0     2235 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/model.py
+-rw-r--r--   0        0        0     3112 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/options.py
+-rw-r--r--   0        0        0    12775 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/response_state.py
+-rw-r--r--   0        0        0     6709 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/structure.py
+-rw-r--r--   0        0        0     7935 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/weak_cache_pool.py
+-rw-r--r--   0        0        0      240 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/util.py
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 xmodel-0.3.1/PKG-INFO
```

### Comparing `xmodel-0.3.0/LICENSE` & `xmodel-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/pyproject.toml` & `xmodel-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "xmodel"
-version = "0.3.0"
+version = "0.3.1"
 description = "Models for working with JSON, ie: JsonModel"
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xmodel"}]
 readme = "README.md"
-license = "The Unlicense (Unlicense)"
 repository = "https://github.com/xyngular/py-xmodel"
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typing-inspect = "^0"
 xloop = "^1.0.1"
 xinject = "^1.4.0"
 xsentinels = "^1.2.1"
```

### Comparing `xmodel-0.3.0/xmodel/__init__.py` & `xmodel-0.3.1/xmodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,8 +497,8 @@
     'BaseStructure',
     'Field',
     'Converter',
     'XModelError',
     'JsonModel'
 ]
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
```

### Comparing `xmodel-0.3.0/xmodel/_private/api/state.py` & `xmodel-0.3.1/xmodel/_private/api/state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/_private/api/utils.py` & `xmodel-0.3.1/xmodel/_private/api/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/base/api.py` & `xmodel-0.3.1/xmodel/base/api.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/base/fields.py` & `xmodel-0.3.1/xmodel/base/fields.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/base/model.py` & `xmodel-0.3.1/xmodel/base/model.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/base/structure.py` & `xmodel-0.3.1/xmodel/base/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/common/children.py` & `xmodel-0.3.1/xmodel/common/children.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/common/lazy.py` & `xmodel-0.3.1/xmodel/common/lazy.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/common/types.py` & `xmodel-0.3.1/xmodel/common/types.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/common/unwrap.py` & `xmodel-0.3.1/xmodel/common/unwrap.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/common/utils.py` & `xmodel-0.3.1/xmodel/common/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/converters.py` & `xmodel-0.3.1/xmodel/converters.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/json.py` & `xmodel-0.3.1/xmodel/json.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/remote/api.py` & `xmodel-0.3.1/xmodel/remote/api.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/remote/client.py` & `xmodel-0.3.1/xmodel/remote/client.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/remote/model.py` & `xmodel-0.3.1/xmodel/remote/model.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/remote/options.py` & `xmodel-0.3.1/xmodel/remote/options.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/remote/response_state.py` & `xmodel-0.3.1/xmodel/remote/response_state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/remote/structure.py` & `xmodel-0.3.1/xmodel/remote/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/xmodel/remote/weak_cache_pool.py` & `xmodel-0.3.1/xmodel/remote/weak_cache_pool.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.0/PKG-INFO` & `xmodel-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: xmodel
-Version: 0.3.0
+Version: 0.3.1
 Summary: Models for working with JSON, ie: JsonModel
 Home-page: https://github.com/xyngular/py-xmodel
-License: The Unlicense (Unlicense)
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ciso8601 (>=2.3.0,<3.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: typing-inspect (>=0,<1)
 Requires-Dist: xinject (>=1.4.0,<2.0.0)
 Requires-Dist: xloop (>=1.0.1,<2.0.0)
 Requires-Dist: xsentinels (>=1.2.1,<2.0.0)
 Requires-Dist: xurls (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/xyngular/py-xmodel
 Description-Content-Type: text/markdown
 
 # Json Modeling Library
 
 Provides easy way to map dict to/from Full-Fledged 'JsonModel' object.
 
+![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)
+![PyPI version](https://badge.fury.io/py/xmodel.svg?)
+
+## Documentation
+
+**[📄 Detailed Documentation](https://xyngular.github.io/py-xmodel/latest/)** | **[🐍 PyPi](https://pypi.org/project/xmodel/)**
+
 ## Getting Started
 
 ???+ warning "Alpha Software!"
     This is pre-release Alpha software, based on another code base and
     the needed changes to make a final release version are not yet
     completed. Everything is subject to change!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

