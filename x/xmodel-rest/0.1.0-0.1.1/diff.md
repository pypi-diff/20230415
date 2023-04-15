# Comparing `tmp/xmodel_rest-0.1.0.tar.gz` & `tmp/xmodel_rest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmodel_rest-0.1.0.tar", max compression
+gzip compressed data, was "xmodel_rest-0.1.1.tar", max compression
```

## Comparing `xmodel_rest-0.1.0.tar` & `xmodel_rest-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1211 2023-04-14 23:23:16.919357 xmodel_rest-0.1.0/LICENSE
--rw-r--r--   0        0        0      348 2023-04-14 23:23:16.919357 xmodel_rest-0.1.0/README.md
--rw-r--r--   0        0        0     2361 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      506 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/__init__.py
--rw-r--r--   0        0        0     8247 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/api.py
--rw-r--r--   0        0        0     2996 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/auth.py
--rw-r--r--   0        0        0    98796 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/client.py
--rw-r--r--   0        0        0      625 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/default_model_urls.py
--rw-r--r--   0        0        0      165 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/errors.py
--rw-r--r--   0        0        0       25 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/meta.json
--rw-r--r--   0        0        0     1476 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/model.py
--rw-r--r--   0        0        0     1746 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/session.py
--rw-r--r--   0        0        0     5706 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/settings.py
--rw-r--r--   0        0        0     6500 2023-04-14 23:23:16.923358 xmodel_rest-0.1.0/xmodel_rest/structure.py
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 xmodel_rest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/LICENSE
+-rw-r--r--   0        0        0      712 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/README.md
+-rw-r--r--   0        0        0     2253 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/__init__.py
+-rw-r--r--   0        0        0     8247 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/api.py
+-rw-r--r--   0        0        0     2996 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/auth.py
+-rw-r--r--   0        0        0    98796 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/client.py
+-rw-r--r--   0        0        0      625 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/default_model_urls.py
+-rw-r--r--   0        0        0      165 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/errors.py
+-rw-r--r--   0        0        0       25 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/meta.json
+-rw-r--r--   0        0        0     1476 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/model.py
+-rw-r--r--   0        0        0     1746 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/session.py
+-rw-r--r--   0        0        0     5706 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/settings.py
+-rw-r--r--   0        0        0     6500 2023-04-15 14:12:30.437543 xmodel_rest-0.1.1/xmodel_rest/structure.py
+-rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 xmodel_rest-0.1.1/PKG-INFO
```

### Comparing `xmodel_rest-0.1.0/LICENSE` & `xmodel_rest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/pyproject.toml` & `xmodel_rest-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 [tool.poetry]
 name = "xmodel_rest"
-version = "0.1.0"
+version = "0.1.1"
 description = "Builds on xmodel, adds ability to get/send/update objects to/from rest API; especially if api uses JSON as it’s request/response body format."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xmodel_rest"}]
 readme = "README.md"
-license = "The Unlicense (Unlicense)"
 repository = "https://github.com/xyngular/py-xmodel-rest"
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-
-# Right now, we are compatiable with both v2 and v3 of xyn-resource.
-#xyn-model = "^1.1.0"
-#xyn-resource = ">=2.1.2,<4"
-#xyn-types = "^1.1.0"
-#xyn-url = "^1.1.0"
-#xyn-dateutils = "^1.1.0"
-#xyn-settings = "^1.4.0"
-
 requests = "^2.26.0"
 requests-mock = "^1.9.3"
 xmodel = "^0.2.0"
 xinject = "^1.4.0"
 xloop = "^1.0.1"
 xsentinels = "^1.2.1"
 xurls = "^0.2.0"
```

### Comparing `xmodel_rest-0.1.0/xmodel_rest/api.py` & `xmodel_rest-0.1.1/xmodel_rest/api.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/xmodel_rest/auth.py` & `xmodel_rest-0.1.1/xmodel_rest/auth.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/xmodel_rest/client.py` & `xmodel_rest-0.1.1/xmodel_rest/client.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/xmodel_rest/default_model_urls.py` & `xmodel_rest-0.1.1/xmodel_rest/default_model_urls.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/xmodel_rest/model.py` & `xmodel_rest-0.1.1/xmodel_rest/model.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/xmodel_rest/session.py` & `xmodel_rest-0.1.1/xmodel_rest/session.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/xmodel_rest/settings.py` & `xmodel_rest-0.1.1/xmodel_rest/settings.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/xmodel_rest/structure.py` & `xmodel_rest-0.1.1/xmodel_rest/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel_rest-0.1.0/PKG-INFO` & `xmodel_rest-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: xmodel-rest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Builds on xmodel, adds ability to get/send/update objects to/from rest API; especially if api uses JSON as it’s request/response body format.
 Home-page: https://github.com/xyngular/py-xmodel-rest
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
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: requests-mock (>=1.9.3,<2.0.0)
 Requires-Dist: xinject (>=1.4.0,<2.0.0)
 Requires-Dist: xloop (>=1.0.1,<2.0.0)
 Requires-Dist: xmodel (>=0.2.0,<0.3.0)
 Requires-Dist: xsentinels (>=1.2.1,<2.0.0)
 Requires-Dist: xsettings (>=1.3.0,<2.0.0)
 Requires-Dist: xurls (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/xyngular/py-xmodel-rest
 Description-Content-Type: text/markdown
 
+![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)
+![PyPI version](https://badge.fury.io/py/xmodel-rest.svg?)
+
+## Documentation
+
+**[📄 Detailed Documentation](https://xyngular.github.io/py-xmodel-rest/latest/)** | **[🐍 PyPi](https://pypi.org/project/xmodel-rest/)**
+
 ## Getting Started
 
 **warning "Alpha Software!"**
 
 This is pre-release Alpha software, based on another code base and
 the needed changes to make a final release version are not yet
 completed. Everything is subject to change; and documentation needs
```

