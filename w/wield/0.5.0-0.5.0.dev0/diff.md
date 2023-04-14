# Comparing `tmp/wield-0.5.0.tar.gz` & `tmp/wield-0.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wield-0.5.0.tar", last modified: Fri Apr 14 23:49:45 2023, max compression
+gzip compressed data, was "wield-0.5.0.dev0.tar", last modified: Fri Apr 14 23:42:28 2023, max compression
```

## Comparing `wield-0.5.0.tar` & `wield-0.5.0.dev0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:49:45.082846 wield-0.5.0/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:49:45.078846 wield-0.5.0/LICENSES/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-12 20:35:37.000000 wield-0.5.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-12 20:35:37.000000 wield-0.5.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 18:38:36.000000 wield-0.5.0/MANIFEST.in
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 18:38:36.000000 wield-0.5.0/NOTICE
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1206 2023-04-14 23:49:45.082846 wield-0.5.0/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      339 2023-04-14 18:38:36.000000 wield-0.5.0/README.md
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 18:38:36.000000 wield-0.5.0/pyproject.toml
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1075 2023-04-14 23:49:45.082846 wield-0.5.0/setup.cfg
--rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 18:38:36.000000 wield-0.5.0/setup.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:49:45.078846 wield-0.5.0/src/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:49:45.078846 wield-0.5.0/src/wield/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:49:45.078846 wield-0.5.0/src/wield/collection/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      505 2023-04-14 18:38:36.000000 wield-0.5.0/src/wield/collection/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      474 2023-04-14 23:46:18.000000 wield-0.5.0/src/wield/collection/_version.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:49:45.078846 wield-0.5.0/src/wield.egg-info/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1206 2023-04-14 23:49:45.000000 wield-0.5.0/src/wield.egg-info/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      329 2023-04-14 23:49:45.000000 wield-0.5.0/src/wield.egg-info/SOURCES.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-14 23:49:45.000000 wield-0.5.0/src/wield.egg-info/dependency_links.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-14 23:49:45.000000 wield-0.5.0/src/wield.egg-info/top_level.txt
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:49:45.082846 wield-0.5.0/tools/
--rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)     3972 2023-04-14 18:38:36.000000 wield-0.5.0/tools/check_versions.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:42:28.012340 wield-0.5.0.dev0/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:42:28.012340 wield-0.5.0.dev0/LICENSES/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-12 20:35:37.000000 wield-0.5.0.dev0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-12 20:35:37.000000 wield-0.5.0.dev0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 18:38:36.000000 wield-0.5.0.dev0/MANIFEST.in
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 18:38:36.000000 wield-0.5.0.dev0/NOTICE
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1211 2023-04-14 23:42:28.012340 wield-0.5.0.dev0/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      339 2023-04-14 18:38:36.000000 wield-0.5.0.dev0/README.md
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 18:38:36.000000 wield-0.5.0.dev0/pyproject.toml
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1061 2023-04-14 23:42:28.012340 wield-0.5.0.dev0/setup.cfg
+-rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 18:38:36.000000 wield-0.5.0.dev0/setup.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:42:28.008340 wield-0.5.0.dev0/src/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:42:28.008340 wield-0.5.0.dev0/src/wield/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:42:28.012340 wield-0.5.0.dev0/src/wield/collection/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      505 2023-04-14 18:38:36.000000 wield-0.5.0.dev0/src/wield/collection/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1398 2023-04-14 23:28:15.000000 wield-0.5.0.dev0/src/wield/collection/_version.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:42:28.012340 wield-0.5.0.dev0/src/wield.egg-info/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1211 2023-04-14 23:42:27.000000 wield-0.5.0.dev0/src/wield.egg-info/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      329 2023-04-14 23:42:28.000000 wield-0.5.0.dev0/src/wield.egg-info/SOURCES.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-14 23:42:27.000000 wield-0.5.0.dev0/src/wield.egg-info/dependency_links.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-14 23:42:27.000000 wield-0.5.0.dev0/src/wield.egg-info/top_level.txt
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:42:28.012340 wield-0.5.0.dev0/tools/
+-rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)     3972 2023-04-14 18:38:36.000000 wield-0.5.0.dev0/tools/check_versions.py
```

### Comparing `wield-0.5.0/LICENSES/Apache-2.0.txt` & `wield-0.5.0.dev0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `wield-0.5.0/LICENSES/CC0-1.0.txt` & `wield-0.5.0.dev0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `wield-0.5.0/NOTICE` & `wield-0.5.0.dev0/NOTICE`

 * *Files identical despite different names*

### Comparing `wield-0.5.0/PKG-INFO` & `wield-0.5.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield
-Version: 0.5.0
+Version: 0.5.0.dev0
 Summary: Toolkit for modeling interferometers, circuits, signals, and control systems
 Home-page: https://github.com/wieldphysics/wield-collection
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-namespace/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-namespace
```

### Comparing `wield-0.5.0/setup.cfg` & `wield-0.5.0.dev0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wield
-version = 0.5.0
+version = 0.5.0.dev0
 license = Apache-2.0
 license_files = LICENSES/*, NOTICE
 author = Lee McCuller
 author_email = mcculler@caltech.edu
 description = Toolkit for modeling interferometers, circuits, signals, and control systems
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -18,17 +18,16 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 setup_requires = 'setuptools>=45.0.0'
-install_requires = 
 package_dir = 
-	=src
+	= src
 packages = find_namespace:
 
 [options.packages.find]
 where = src
 
 [aliases]
 test = pytest
```

### Comparing `wield-0.5.0/setup.py` & `wield-0.5.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `wield-0.5.0/src/wield.egg-info/PKG-INFO` & `wield-0.5.0.dev0/src/wield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield
-Version: 0.5.0
+Version: 0.5.0.dev0
 Summary: Toolkit for modeling interferometers, circuits, signals, and control systems
 Home-page: https://github.com/wieldphysics/wield-collection
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-namespace/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-namespace
```

### Comparing `wield-0.5.0/tools/check_versions.py` & `wield-0.5.0.dev0/tools/check_versions.py`

 * *Files identical despite different names*

