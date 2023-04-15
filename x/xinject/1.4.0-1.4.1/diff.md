# Comparing `tmp/xinject-1.4.0.tar.gz` & `tmp/xinject-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinject-1.4.0.tar", max compression
+gzip compressed data, was "xinject-1.4.1.tar", max compression
```

## Comparing `xinject-1.4.0.tar` & `xinject-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      907 2023-02-19 03:58:21.637686 xinject-1.4.0/LICENSE
--rw-r--r--   0        0        0     2421 2023-02-19 03:58:21.637686 xinject-1.4.0/README.md
--rw-r--r--   0        0        0     1614 2023-02-19 03:58:21.637686 xinject-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      211 2023-02-19 03:58:21.637686 xinject-1.4.0/xinject/__init__.py
--rw-r--r--   0        0        0      390 2023-02-19 03:58:21.637686 xinject-1.4.0/xinject/_private/__init__.py
--rw-r--r--   0        0        0      377 2023-02-19 03:58:21.637686 xinject-1.4.0/xinject/_private/classproperty.py
--rw-r--r--   0        0        0    61555 2023-02-19 03:58:21.637686 xinject-1.4.0/xinject/context.py
--rw-r--r--   0        0        0    31037 2023-02-19 03:58:21.641686 xinject-1.4.0/xinject/dependency.py
--rw-r--r--   0        0        0       41 2023-02-19 03:58:21.641686 xinject-1.4.0/xinject/errors.py
--rw-r--r--   0        0        0     5956 2023-02-19 03:58:21.641686 xinject-1.4.0/xinject/proxy.py
--rw-r--r--   0        0        0     2559 2023-02-19 03:58:21.641686 xinject-1.4.0/xinject/pytest_plugin.py
--rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 xinject-1.4.0/setup.py
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 xinject-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:11:35.210221 xinject-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2421 2023-04-15 14:11:35.210221 xinject-1.4.1/README.md
+-rw-r--r--   0        0        0     1658 2023-04-15 14:11:35.210221 xinject-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/__init__.py
+-rw-r--r--   0        0        0      390 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/_private/__init__.py
+-rw-r--r--   0        0        0      377 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/_private/classproperty.py
+-rw-r--r--   0        0        0    61555 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/context.py
+-rw-r--r--   0        0        0    31037 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/dependency.py
+-rw-r--r--   0        0        0       41 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/errors.py
+-rw-r--r--   0        0        0     5956 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/proxy.py
+-rw-r--r--   0        0        0     2559 2023-04-15 14:11:35.214221 xinject-1.4.1/xinject/pytest_plugin.py
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 xinject-1.4.1/PKG-INFO
```

### Comparing `xinject-1.4.0/README.md` & `xinject-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `xinject-1.4.0/pyproject.toml` & `xinject-1.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "xinject"
-version = "1.4.0"
+version = "1.4.1"
 description = "Lazy dependency injection."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xinject"}]
 readme = "README.md"
-license = "MIT"
 repository = "https://github.com/xyngular/py-xinject"
 keywords = ["dependency", "injection", "lazy", "resource"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 xsentinels = "^1.2.0"
```

### Comparing `xinject-1.4.0/xinject/context.py` & `xinject-1.4.1/xinject/context.py`

 * *Files identical despite different names*

### Comparing `xinject-1.4.0/xinject/dependency.py` & `xinject-1.4.1/xinject/dependency.py`

 * *Files identical despite different names*

### Comparing `xinject-1.4.0/xinject/proxy.py` & `xinject-1.4.1/xinject/proxy.py`

 * *Files identical despite different names*

### Comparing `xinject-1.4.0/xinject/pytest_plugin.py` & `xinject-1.4.1/xinject/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `xinject-1.4.0/PKG-INFO` & `xinject-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: xinject
-Version: 1.4.0
+Version: 1.4.1
 Summary: Lazy dependency injection.
 Home-page: https://github.com/xyngular/py-xinject
-License: MIT
 Keywords: dependency,injection,lazy,resource
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
 Requires-Dist: xsentinels (>=1.2.0,<2.0.0)
```

