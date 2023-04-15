# Comparing `tmp/Allagash-0.4.2.tar.gz` & `tmp/Allagash-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Allagash-0.4.2.tar", last modified: Mon Apr  3 01:12:43 2023, max compression
+gzip compressed data, was "Allagash-0.4.3.tar", last modified: Sat Apr 15 12:48:25 2023, max compression
```

## Comparing `Allagash-0.4.2.tar` & `Allagash-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 allagash  (1000) allagash  (1000)        0 2023-04-03 01:12:43.462592 Allagash-0.4.2/
-drwxr-xr-x   0 allagash  (1000) allagash  (1000)        0 2023-04-03 01:12:43.458592 Allagash-0.4.2/Allagash.egg-info/
--rw-r--r--   0 allagash  (1000) allagash  (1000)     3627 2023-04-03 01:12:43.000000 Allagash-0.4.2/Allagash.egg-info/PKG-INFO
--rw-r--r--   0 allagash  (1000) allagash  (1000)      253 2023-04-03 01:12:43.000000 Allagash-0.4.2/Allagash.egg-info/SOURCES.txt
--rw-r--r--   0 allagash  (1000) allagash  (1000)        1 2023-04-03 01:12:43.000000 Allagash-0.4.2/Allagash.egg-info/dependency_links.txt
--rw-r--r--   0 allagash  (1000) allagash  (1000)       81 2023-04-03 01:12:43.000000 Allagash-0.4.2/Allagash.egg-info/requires.txt
--rw-r--r--   0 allagash  (1000) allagash  (1000)        9 2023-04-03 01:12:43.000000 Allagash-0.4.2/Allagash.egg-info/top_level.txt
--rw-r--r--   0 allagash  (1000) allagash  (1000)     1069 2023-04-03 01:07:15.000000 Allagash-0.4.2/LICENSE
--rw-r--r--   0 allagash  (1000) allagash  (1000)     3627 2023-04-03 01:12:43.462592 Allagash-0.4.2/PKG-INFO
--rw-r--r--   0 allagash  (1000) allagash  (1000)     3096 2023-04-03 01:07:15.000000 Allagash-0.4.2/README.md
-drwxr-xr-x   0 allagash  (1000) allagash  (1000)        0 2023-04-03 01:12:43.458592 Allagash-0.4.2/allagash/
--rw-r--r--   0 allagash  (1000) allagash  (1000)      411 2023-04-03 01:07:16.000000 Allagash-0.4.2/allagash/__init__.py
--rw-r--r--   0 allagash  (1000) allagash  (1000)    17009 2023-04-03 01:07:16.000000 Allagash-0.4.2/allagash/coverage.py
--rw-r--r--   0 allagash  (1000) allagash  (1000)    21098 2023-04-03 01:07:16.000000 Allagash-0.4.2/allagash/problem.py
--rw-r--r--   0 allagash  (1000) allagash  (1000)      738 2023-04-03 01:07:15.000000 Allagash-0.4.2/pyproject.toml
--rw-r--r--   0 allagash  (1000) allagash  (1000)       38 2023-04-03 01:12:43.462592 Allagash-0.4.2/setup.cfg
+drwxr-xr-x   0 allagash  (1000) allagash  (1000)        0 2023-04-15 12:48:25.631712 Allagash-0.4.3/
+drwxr-xr-x   0 allagash  (1000) allagash  (1000)        0 2023-04-15 12:48:25.627712 Allagash-0.4.3/Allagash.egg-info/
+-rw-r--r--   0 allagash  (1000) allagash  (1000)     3627 2023-04-15 12:48:25.000000 Allagash-0.4.3/Allagash.egg-info/PKG-INFO
+-rw-r--r--   0 allagash  (1000) allagash  (1000)      253 2023-04-15 12:48:25.000000 Allagash-0.4.3/Allagash.egg-info/SOURCES.txt
+-rw-r--r--   0 allagash  (1000) allagash  (1000)        1 2023-04-15 12:48:25.000000 Allagash-0.4.3/Allagash.egg-info/dependency_links.txt
+-rw-r--r--   0 allagash  (1000) allagash  (1000)       81 2023-04-15 12:48:25.000000 Allagash-0.4.3/Allagash.egg-info/requires.txt
+-rw-r--r--   0 allagash  (1000) allagash  (1000)        9 2023-04-15 12:48:25.000000 Allagash-0.4.3/Allagash.egg-info/top_level.txt
+-rw-r--r--   0 allagash  (1000) allagash  (1000)     1069 2023-04-15 12:41:56.000000 Allagash-0.4.3/LICENSE
+-rw-r--r--   0 allagash  (1000) allagash  (1000)     3627 2023-04-15 12:48:25.627712 Allagash-0.4.3/PKG-INFO
+-rw-r--r--   0 allagash  (1000) allagash  (1000)     3096 2023-04-15 12:41:56.000000 Allagash-0.4.3/README.md
+drwxr-xr-x   0 allagash  (1000) allagash  (1000)        0 2023-04-15 12:48:25.627712 Allagash-0.4.3/allagash/
+-rw-r--r--   0 allagash  (1000) allagash  (1000)      340 2023-04-15 12:41:56.000000 Allagash-0.4.3/allagash/__init__.py
+-rw-r--r--   0 allagash  (1000) allagash  (1000)    17009 2023-04-15 12:41:56.000000 Allagash-0.4.3/allagash/coverage.py
+-rw-r--r--   0 allagash  (1000) allagash  (1000)    21098 2023-04-15 12:41:56.000000 Allagash-0.4.3/allagash/problem.py
+-rw-r--r--   0 allagash  (1000) allagash  (1000)      738 2023-04-15 12:41:56.000000 Allagash-0.4.3/pyproject.toml
+-rw-r--r--   0 allagash  (1000) allagash  (1000)       38 2023-04-15 12:48:25.631712 Allagash-0.4.3/setup.cfg
```

### Comparing `Allagash-0.4.2/Allagash.egg-info/PKG-INFO` & `Allagash-0.4.3/Allagash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Allagash
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python Spatial Optimization Library
 Author-email: Aaron Pulver <apulverizer@gmail.com>
 License: MIT
 Project-URL: Homepage, https://apulverizer.github.io/allagash
 Project-URL: Bug Tracker, https://github.com/apulverizer/allagash/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Allagash-0.4.2/LICENSE` & `Allagash-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Allagash-0.4.2/PKG-INFO` & `Allagash-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Allagash
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python Spatial Optimization Library
 Author-email: Aaron Pulver <apulverizer@gmail.com>
 License: MIT
 Project-URL: Homepage, https://apulverizer.github.io/allagash
 Project-URL: Bug Tracker, https://github.com/apulverizer/allagash/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Allagash-0.4.2/README.md` & `Allagash-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Allagash-0.4.2/allagash/coverage.py` & `Allagash-0.4.3/allagash/coverage.py`

 * *Files identical despite different names*

### Comparing `Allagash-0.4.2/allagash/problem.py` & `Allagash-0.4.3/allagash/problem.py`

 * *Files identical despite different names*

### Comparing `Allagash-0.4.2/pyproject.toml` & `Allagash-0.4.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Allagash"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Aaron Pulver", email="apulverizer@gmail.com" },
 ]
 description = "A Python Spatial Optimization Library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

