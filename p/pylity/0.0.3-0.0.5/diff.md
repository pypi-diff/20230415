# Comparing `tmp/pylity-0.0.3.tar.gz` & `tmp/pylity-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylity-0.0.3.tar", max compression
+gzip compressed data, was "pylity-0.0.5.tar", max compression
```

## Comparing `pylity-0.0.3.tar` & `pylity-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-15 12:29:15.075935 pylity-0.0.3/LICENSE
--rw-r--r--   0        0        0     4740 2023-04-15 12:29:15.075935 pylity-0.0.3/README.md
--rw-r--r--   0        0        0      882 2023-04-15 12:29:15.079934 pylity-0.0.3/pylity/Async.py
--rw-r--r--   0        0        0     4509 2023-04-15 12:29:15.079934 pylity-0.0.3/pylity/Function.py
--rw-r--r--   0        0        0     1825 2023-04-15 12:29:15.079934 pylity-0.0.3/pylity/Path.py
--rw-r--r--   0        0        0      473 2023-04-15 12:29:15.079934 pylity-0.0.3/pylity/String.py
--rw-r--r--   0        0        0      116 2023-04-15 12:29:15.079934 pylity-0.0.3/pylity/__init__.py
--rw-r--r--   0        0        0      713 2023-04-15 12:29:15.079934 pylity-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 pylity-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 16:46:34.425188 pylity-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4740 2023-04-15 16:46:34.425188 pylity-0.0.5/README.md
+-rw-r--r--   0        0        0      882 2023-04-15 16:46:34.425188 pylity-0.0.5/pylity/Async.py
+-rw-r--r--   0        0        0     1035 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/Collection.py
+-rw-r--r--   0        0        0     4509 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/Function.py
+-rw-r--r--   0        0        0     4819 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/Path.py
+-rw-r--r--   0        0        0      473 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/String.py
+-rw-r--r--   0        0        0      116 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/__init__.py
+-rw-r--r--   0        0        0      713 2023-04-15 16:46:34.429188 pylity-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 pylity-0.0.5/PKG-INFO
```

### Comparing `pylity-0.0.3/LICENSE` & `pylity-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylity-0.0.3/README.md` & `pylity-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pylity-0.0.3/pylity/Async.py` & `pylity-0.0.5/pylity/Async.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.3/pylity/Function.py` & `pylity-0.0.5/pylity/Function.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.3/pyproject.toml` & `pylity-0.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "pylity"
-version = "0.0.3"
+version = "0.0.5"
 description = "A collection of utility functions for Python. pylity means Python Utility "
 authors = ["Payadel <payadelteam@gmail.com>"]
 license = "GPLV3"
 readme = "README.md"
 repository = "https://github.com/Payadel/pylity"
 keywords = ['utility', 'helpers']
 packages = [{ include = "pylity" }]
```

### Comparing `pylity-0.0.3/PKG-INFO` & `pylity-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylity
-Version: 0.0.3
+Version: 0.0.5
 Summary: A collection of utility functions for Python. pylity means Python Utility 
 Home-page: https://github.com/Payadel/pylity
 License: GPLV3
 Keywords: utility,helpers
 Author: Payadel
 Author-email: payadelteam@gmail.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylity Version: 0.0.3 Summary: A collection of
+Metadata-Version: 2.1 Name: pylity Version: 0.0.5 Summary: A collection of
 utility functions for Python. pylity means Python Utility Home-page: https://
 github.com/Payadel/pylity License: GPLV3 Keywords: utility,helpers Author:
 Payadel Author-email: payadelteam@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: on-rails
 (==4.0.1) Project-URL: Repository, https://github.com/Payadel/pylity
```

