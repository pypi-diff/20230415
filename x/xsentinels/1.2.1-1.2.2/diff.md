# Comparing `tmp/xsentinels-1.2.1.tar.gz` & `tmp/xsentinels-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsentinels-1.2.1.tar", max compression
+gzip compressed data, was "xsentinels-1.2.2.tar", max compression
```

## Comparing `xsentinels-1.2.1.tar` & `xsentinels-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      907 2023-02-03 15:53:56.980393 xsentinels-1.2.1/LICENSE
--rw-r--r--   0        0        0      997 2023-02-03 15:53:56.980393 xsentinels-1.2.1/README.md
--rw-r--r--   0        0        0      911 2023-02-03 15:53:56.980393 xsentinels-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-03 15:53:56.984393 xsentinels-1.2.1/xsentinels/__init__.py
--rw-r--r--   0        0        0      924 2023-02-03 15:53:56.984393 xsentinels-1.2.1/xsentinels/default.py
--rw-r--r--   0        0        0     2957 2023-02-03 15:53:56.984393 xsentinels-1.2.1/xsentinels/null.py
--rw-r--r--   0        0        0       71 2023-02-03 15:53:56.984393 xsentinels-1.2.1/xsentinels/sentinel.py
--rw-r--r--   0        0        0     3427 2023-02-03 15:53:56.984393 xsentinels-1.2.1/xsentinels/singleton.py
--rw-r--r--   0        0        0     2154 2023-02-03 15:53:56.984393 xsentinels-1.2.1/xsentinels/unwrap.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 xsentinels-1.2.1/setup.py
--rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 xsentinels-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:11:49.706179 xsentinels-1.2.2/LICENSE
+-rw-r--r--   0        0        0      997 2023-04-15 14:11:49.706179 xsentinels-1.2.2/README.md
+-rw-r--r--   0        0        0      953 2023-04-15 14:11:49.710179 xsentinels-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-04-15 14:11:49.710179 xsentinels-1.2.2/xsentinels/__init__.py
+-rw-r--r--   0        0        0      924 2023-04-15 14:11:49.710179 xsentinels-1.2.2/xsentinels/default.py
+-rw-r--r--   0        0        0     2957 2023-04-15 14:11:49.710179 xsentinels-1.2.2/xsentinels/null.py
+-rw-r--r--   0        0        0       71 2023-04-15 14:11:49.710179 xsentinels-1.2.2/xsentinels/sentinel.py
+-rw-r--r--   0        0        0     3427 2023-04-15 14:11:49.710179 xsentinels-1.2.2/xsentinels/singleton.py
+-rw-r--r--   0        0        0     2154 2023-04-15 14:11:49.710179 xsentinels-1.2.2/xsentinels/unwrap.py
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 xsentinels-1.2.2/PKG-INFO
```

### Comparing `xsentinels-1.2.1/README.md` & `xsentinels-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xsentinels-1.2.1/pyproject.toml` & `xsentinels-1.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "xsentinels"
 description = "Sentinels for Defaults, Null and for creating sentinels/singletons."
-version = "1.2.1"
+version = "1.2.2"
 authors = ["Josh Orr <josh@orr.blue>"]
 readme = "README.md"
 packages = [{include = "xsentinels"}]
-license = "MIT-0"
 repository = "https://github.com/xyngular/py-xsentinels"
 keywords = ["singleton", "type", "guards", "sentinels", "sentinel", "default", "null"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typing-inspect = "^0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `xsentinels-1.2.1/xsentinels/default.py` & `xsentinels-1.2.2/xsentinels/default.py`

 * *Files identical despite different names*

### Comparing `xsentinels-1.2.1/xsentinels/null.py` & `xsentinels-1.2.2/xsentinels/null.py`

 * *Files identical despite different names*

### Comparing `xsentinels-1.2.1/xsentinels/singleton.py` & `xsentinels-1.2.2/xsentinels/singleton.py`

 * *Files identical despite different names*

### Comparing `xsentinels-1.2.1/xsentinels/unwrap.py` & `xsentinels-1.2.2/xsentinels/unwrap.py`

 * *Files identical despite different names*

### Comparing `xsentinels-1.2.1/PKG-INFO` & `xsentinels-1.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: xsentinels
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sentinels for Defaults, Null and for creating sentinels/singletons.
 Home-page: https://github.com/xyngular/py-xsentinels
-License: MIT-0
 Keywords: singleton,type,guards,sentinels,sentinel,default,null
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: typing-inspect (>=0,<1)
```

