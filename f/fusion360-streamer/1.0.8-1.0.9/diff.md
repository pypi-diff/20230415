# Comparing `tmp/fusion360-streamer-1.0.8.tar.gz` & `tmp/fusion360-streamer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion360-streamer-1.0.8.tar", last modified: Thu Mar 23 11:30:05 2023, max compression
+gzip compressed data, was "fusion360-streamer-1.0.9.tar", last modified: Thu Mar 23 11:39:40 2023, max compression
```

## Comparing `fusion360-streamer-1.0.8.tar` & `fusion360-streamer-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:30:05.881126 fusion360-streamer-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-23 11:30:05.881126 fusion360-streamer-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:30:05.881126 fusion360-streamer-1.0.8/fusion360_streamer/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/fusion360_streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/fusion360_streamer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/fusion360_streamer/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/fusion360_streamer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/fusion360_streamer/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/fusion360_streamer/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:30:05.881126 fusion360-streamer-1.0.8/fusion360_streamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-23 11:30:05.000000 fusion360-streamer-1.0.8/fusion360_streamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-23 11:30:05.000000 fusion360-streamer-1.0.8/fusion360_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 11:30:05.000000 fusion360-streamer-1.0.8/fusion360_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-23 11:30:05.000000 fusion360-streamer-1.0.8/fusion360_streamer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-23 11:30:05.000000 fusion360-streamer-1.0.8/fusion360_streamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-23 11:30:05.000000 fusion360-streamer-1.0.8/fusion360_streamer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 11:30:05.881126 fusion360-streamer-1.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      876 2023-03-23 11:30:04.000000 fusion360-streamer-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:39:40.980125 fusion360-streamer-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-23 11:39:40.980125 fusion360-streamer-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:39:40.980125 fusion360-streamer-1.0.9/fusion360_streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:39:40.980125 fusion360-streamer-1.0.9/fusion360_streamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/fusion360_streamer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 11:39:40.980125 fusion360-streamer-1.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      876 2023-03-23 11:39:40.000000 fusion360-streamer-1.0.9/setup.py
```

### Comparing `fusion360-streamer-1.0.8/LICENSE` & `fusion360-streamer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fusion360-streamer-1.0.8/PKG-INFO` & `fusion360-streamer-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion360-streamer
-Version: 1.0.8
+Version: 1.0.9
 Summary: Autodesk Fusion 360 Streamer python implementation
 Home-page: https://github.com/dzervas/fusion360-streamer
 Author: Dimitris Zervas
 Author-email: dzervas@dzervas.gr
 License: GPLv3
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `fusion360-streamer-1.0.8/README.md` & `fusion360-streamer-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fusion360-streamer-1.0.8/fusion360_streamer/__main__.py` & `fusion360-streamer-1.0.9/fusion360_streamer/__main__.py`

 * *Files identical despite different names*

### Comparing `fusion360-streamer-1.0.8/fusion360_streamer/application.py` & `fusion360-streamer-1.0.9/fusion360_streamer/application.py`

 * *Files identical despite different names*

### Comparing `fusion360-streamer-1.0.8/fusion360_streamer/constants.py` & `fusion360-streamer-1.0.9/fusion360_streamer/constants.py`

 * *Files identical despite different names*

### Comparing `fusion360-streamer-1.0.8/fusion360_streamer/gui.py` & `fusion360-streamer-1.0.9/fusion360_streamer/gui.py`

 * *Files identical despite different names*

### Comparing `fusion360-streamer-1.0.8/fusion360_streamer/package.py` & `fusion360-streamer-1.0.9/fusion360_streamer/package.py`

 * *Files identical despite different names*

### Comparing `fusion360-streamer-1.0.8/fusion360_streamer.egg-info/PKG-INFO` & `fusion360-streamer-1.0.9/fusion360_streamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion360-streamer
-Version: 1.0.8
+Version: 1.0.9
 Summary: Autodesk Fusion 360 Streamer python implementation
 Home-page: https://github.com/dzervas/fusion360-streamer
 Author: Dimitris Zervas
 Author-email: dzervas@dzervas.gr
 License: GPLv3
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `fusion360-streamer-1.0.8/setup.py` & `fusion360-streamer-1.0.9/setup.py`

 * *Files identical despite different names*

