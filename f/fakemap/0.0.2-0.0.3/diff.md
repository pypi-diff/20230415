# Comparing `tmp/fakemap-0.0.2.tar.gz` & `tmp/fakemap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakemap-0.0.2.tar", last modified: Wed Apr  5 02:05:20 2023, max compression
+gzip compressed data, was "fakemap-0.0.3.tar", last modified: Sat Apr 15 00:25:08 2023, max compression
```

## Comparing `fakemap-0.0.2.tar` & `fakemap-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 02:05:20.970905 fakemap-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-05 02:05:09.000000 fakemap-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-05 02:05:09.000000 fakemap-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-05 02:05:20.970905 fakemap-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-05 02:05:09.000000 fakemap-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 02:05:20.970905 fakemap-0.0.2/fakemap/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-05 02:05:09.000000 fakemap-0.0.2/fakemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-05 02:05:09.000000 fakemap-0.0.2/fakemap/fakemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 02:05:20.970905 fakemap-0.0.2/fakemap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-05 02:05:20.000000 fakemap-0.0.2/fakemap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-05 02:05:20.000000 fakemap-0.0.2/fakemap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 02:05:20.000000 fakemap-0.0.2/fakemap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 02:05:20.000000 fakemap-0.0.2/fakemap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 02:05:20.000000 fakemap-0.0.2/fakemap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 02:05:20.000000 fakemap-0.0.2/fakemap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 02:05:09.000000 fakemap-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-05 02:05:20.970905 fakemap-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-05 02:05:09.000000 fakemap-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:25:08.067051 fakemap-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 00:24:57.000000 fakemap-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 00:24:57.000000 fakemap-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-15 00:25:08.067051 fakemap-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-15 00:24:57.000000 fakemap-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:25:08.067051 fakemap-0.0.3/fakemap/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-15 00:24:57.000000 fakemap-0.0.3/fakemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-15 00:24:57.000000 fakemap-0.0.3/fakemap/fakemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-15 00:24:57.000000 fakemap-0.0.3/fakemap/foliummap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:25:08.067051 fakemap-0.0.3/fakemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-15 00:25:08.000000 fakemap-0.0.3/fakemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 00:25:08.000000 fakemap-0.0.3/fakemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 00:25:08.000000 fakemap-0.0.3/fakemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:25:08.000000 fakemap-0.0.3/fakemap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 00:25:08.000000 fakemap-0.0.3/fakemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 00:25:08.000000 fakemap-0.0.3/fakemap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 00:24:57.000000 fakemap-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 00:25:08.067051 fakemap-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 00:24:57.000000 fakemap-0.0.3/setup.py
```

### Comparing `fakemap-0.0.2/LICENSE` & `fakemap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fakemap-0.0.2/PKG-INFO` & `fakemap-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakemap
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/MattAGUT/fakemap
 Author: Matthew Gerloff
 Author-email: mapache.tn@gmail.com
 License: MIT license
 Keywords: fakemap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fakemap-0.0.2/README.md` & `fakemap-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fakemap-0.0.2/fakemap.egg-info/PKG-INFO` & `fakemap-0.0.3/fakemap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakemap
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/MattAGUT/fakemap
 Author: Matthew Gerloff
 Author-email: mapache.tn@gmail.com
 License: MIT license
 Keywords: fakemap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fakemap-0.0.2/setup.py` & `fakemap-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='fakemap',
     name='fakemap',
     packages=find_packages(include=['fakemap', 'fakemap.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MattAGUT/fakemap',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

