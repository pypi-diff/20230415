# Comparing `tmp/barbell2_castor-0.1.0.tar.gz` & `tmp/barbell2_castor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbell2_castor-0.1.0.tar", last modified: Sat Apr 15 12:23:48 2023, max compression
+gzip compressed data, was "dist/barbell2_castor-0.2.0.tar", last modified: Sat Apr 15 12:30:05 2023, max compression
```

## Comparing `barbell2_castor-0.1.0.tar` & `barbell2_castor-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 12:23:48.268604 barbell2_castor-0.1.0/
--rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 12:23:48.268365 barbell2_castor-0.1.0/PKG-INFO
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 12:23:48.266910 barbell2_castor-0.1.0/barbell2_castor/
--rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-15 12:23:37.000000 barbell2_castor-0.1.0/barbell2_castor/__init__.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 12:23:48.268057 barbell2_castor-0.1.0/barbell2_castor.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 12:23:48.000000 barbell2_castor-0.1.0/barbell2_castor.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      272 2023-04-15 12:23:48.000000 barbell2_castor-0.1.0/barbell2_castor.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.1.0/barbell2_castor.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 12:23:48.000000 barbell2_castor-0.1.0/barbell2_castor.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.1.0/barbell2_castor.egg-info/not-zip-safe
--rw-r--r--   0 ralph      (501) staff       (20)       16 2023-04-15 12:23:48.000000 barbell2_castor-0.1.0/barbell2_castor.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 12:23:48.268674 barbell2_castor-0.1.0/setup.cfg
--rw-r--r--   0 ralph      (501) staff       (20)     1317 2023-04-15 12:21:56.000000 barbell2_castor-0.1.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 12:30:05.578523 barbell2_castor-0.2.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 12:30:05.578286 barbell2_castor-0.2.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 12:30:05.576269 barbell2_castor-0.2.0/barbell2_castor/
+-rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-15 12:30:01.000000 barbell2_castor-0.2.0/barbell2_castor/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     8904 2023-04-15 12:26:19.000000 barbell2_castor-0.2.0/barbell2_castor/api.py
+-rw-r--r--   0 ralph      (501) staff       (20)    14709 2023-04-15 12:29:33.000000 barbell2_castor-0.2.0/barbell2_castor/castor2sqlite.py
+-rw-r--r--   0 ralph      (501) staff       (20)      628 2023-04-15 12:26:09.000000 barbell2_castor-0.2.0/barbell2_castor/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 12:30:05.577964 barbell2_castor-0.2.0/barbell2_castor.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      784 2023-04-15 12:30:05.000000 barbell2_castor-0.2.0/barbell2_castor.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      391 2023-04-15 12:30:05.000000 barbell2_castor-0.2.0/barbell2_castor.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:30:05.000000 barbell2_castor-0.2.0/barbell2_castor.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 12:30:05.000000 barbell2_castor-0.2.0/barbell2_castor.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 12:23:48.000000 barbell2_castor-0.2.0/barbell2_castor.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       34 2023-04-15 12:30:05.000000 barbell2_castor-0.2.0/barbell2_castor.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       16 2023-04-15 12:30:05.000000 barbell2_castor-0.2.0/barbell2_castor.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 12:30:05.578596 barbell2_castor-0.2.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1372 2023-04-15 12:28:09.000000 barbell2_castor-0.2.0/setup.py
```

### Comparing `barbell2_castor-0.1.0/PKG-INFO` & `barbell2_castor-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2_castor
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_castor
```

### Comparing `barbell2_castor-0.1.0/barbell2_castor.egg-info/PKG-INFO` & `barbell2_castor-0.2.0/barbell2_castor.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2-castor
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utilities for interfacing with Castor EDC
 Home-page: https://github.com/rbrecheisen/barbell2_castor
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_castor
```

### Comparing `barbell2_castor-0.1.0/setup.py` & `barbell2_castor-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import os
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 requirements = [
+    'oauthlib',
+    'requests-oauthlib',
+    'pandas',
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
```

