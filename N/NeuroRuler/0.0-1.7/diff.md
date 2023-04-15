# Comparing `tmp/NeuroRuler-0.0.tar.gz` & `tmp/NeuroRuler-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroRuler-0.0.tar", last modified: Sat Apr 15 15:34:28 2023, max compression
+gzip compressed data, was "NeuroRuler-1.7.tar", last modified: Sat Apr 15 15:33:02 2023, max compression
```

## Comparing `NeuroRuler-0.0.tar` & `NeuroRuler-1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:34:28.069156 NeuroRuler-0.0/
--rw-r--r--   0 jesse      (501) staff       (20)     1105 2023-04-03 23:13:14.000000 NeuroRuler-0.0/LICENSE
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:34:28.066259 NeuroRuler-0.0/NeuroRuler.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:34:28.000000 NeuroRuler-0.0/NeuroRuler.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)      313 2023-04-15 15:34:28.000000 NeuroRuler-0.0/NeuroRuler.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-15 15:34:28.000000 NeuroRuler-0.0/NeuroRuler.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)      142 2023-04-15 15:34:28.000000 NeuroRuler-0.0/NeuroRuler.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)        4 2023-04-15 15:34:28.000000 NeuroRuler-0.0/NeuroRuler.egg-info/top_level.txt
--rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:34:28.068935 NeuroRuler-0.0/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     2794 2023-04-15 13:56:33.000000 NeuroRuler-0.0/README.md
--rw-r--r--   0 jesse      (501) staff       (20)     1445 2023-04-15 15:03:14.000000 NeuroRuler-0.0/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)       38 2023-04-15 15:34:28.069225 NeuroRuler-0.0/setup.cfg
--rw-r--r--   0 jesse      (501) staff       (20)     2114 2023-04-15 15:26:51.000000 NeuroRuler-0.0/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:34:28.063399 NeuroRuler-0.0/src/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:34:28.067536 NeuroRuler-0.0/src/GUI/
--rw-r--r--   0 jesse      (501) staff       (20)     1622 2023-04-15 15:34:19.000000 NeuroRuler-0.0/src/GUI/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     6001 2023-04-15 13:24:15.000000 NeuroRuler-0.0/src/GUI/helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)    39894 2023-04-15 13:38:34.000000 NeuroRuler-0.0/src/GUI/main.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:34:28.068393 NeuroRuler-0.0/tests/
--rw-r--r--   0 jesse      (501) staff       (20)     2707 2023-04-15 13:24:15.000000 NeuroRuler-0.0/tests/test_img_helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)    12447 2023-04-15 13:38:34.000000 NeuroRuler-0.0/tests/test_imgproc.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.396332 NeuroRuler-1.7/
+-rw-r--r--   0 jesse      (501) staff       (20)     1105 2023-04-03 23:13:14.000000 NeuroRuler-1.7/LICENSE
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.394270 NeuroRuler-1.7/NeuroRuler.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)      313 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)      142 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        4 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/top_level.txt
+-rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:33:02.396123 NeuroRuler-1.7/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     2794 2023-04-15 13:56:33.000000 NeuroRuler-1.7/README.md
+-rw-r--r--   0 jesse      (501) staff       (20)     1445 2023-04-15 15:03:14.000000 NeuroRuler-1.7/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-04-15 15:33:02.396397 NeuroRuler-1.7/setup.cfg
+-rw-r--r--   0 jesse      (501) staff       (20)     2114 2023-04-15 15:26:51.000000 NeuroRuler-1.7/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.392259 NeuroRuler-1.7/src/
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.395072 NeuroRuler-1.7/src/GUI/
+-rw-r--r--   0 jesse      (501) staff       (20)     1622 2023-04-15 15:27:32.000000 NeuroRuler-1.7/src/GUI/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6001 2023-04-15 13:24:15.000000 NeuroRuler-1.7/src/GUI/helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)    39894 2023-04-15 13:38:34.000000 NeuroRuler-1.7/src/GUI/main.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.395671 NeuroRuler-1.7/tests/
+-rw-r--r--   0 jesse      (501) staff       (20)     2707 2023-04-15 13:24:15.000000 NeuroRuler-1.7/tests/test_img_helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)    12447 2023-04-15 13:38:34.000000 NeuroRuler-1.7/tests/test_imgproc.py
```

### Comparing `NeuroRuler-0.0/LICENSE` & `NeuroRuler-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0/NeuroRuler.egg-info/PKG-INFO` & `NeuroRuler-1.7/NeuroRuler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroRuler
-Version: 0.0
+Version: 1.7
 Summary: A program that calculates head circumference from MRI data (.nii, .nii.gz, .nrrd).
 Home-page: https://github.com/COMP523TeamD/HeadCircumferenceTool
 Download-URL: https://github.com/COMP523TeamD/HeadCircumferenceTool/releases
 Author: COMP523 Team D
 Author-email: Peifeng He <hankhe@ad.unc.edu>, Madison Lester <madiali@email.unc.edu>, Eric Schneider <eric@cs.unc.edu>, Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/COMP523TeamD/HeadCircumferenceTool
 Project-URL: Bug Tracker, https://github.com/COMP523TeamD/HeadCircumferenceTool/issues
```

### Comparing `NeuroRuler-0.0/PKG-INFO` & `NeuroRuler-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroRuler
-Version: 0.0
+Version: 1.7
 Summary: A program that calculates head circumference from MRI data (.nii, .nii.gz, .nrrd).
 Home-page: https://github.com/COMP523TeamD/HeadCircumferenceTool
 Download-URL: https://github.com/COMP523TeamD/HeadCircumferenceTool/releases
 Author: COMP523 Team D
 Author-email: Peifeng He <hankhe@ad.unc.edu>, Madison Lester <madiali@email.unc.edu>, Eric Schneider <eric@cs.unc.edu>, Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/COMP523TeamD/HeadCircumferenceTool
 Project-URL: Bug Tracker, https://github.com/COMP523TeamD/HeadCircumferenceTool/issues
```

### Comparing `NeuroRuler-0.0/README.md` & `NeuroRuler-1.7/README.md`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0/pyproject.toml` & `NeuroRuler-1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0/setup.py` & `NeuroRuler-1.7/setup.py`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0/src/GUI/__init__.py` & `NeuroRuler-1.7/src/GUI/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import sys
 import os
 import src.GUI.main as main
 import src.utils.parser as parser
 
 # TODO: Modify when refactoring
-__version__ = "0.0"
+__version__ = "1.7"
 
 def gui() -> None:
     """Start GUI."""
     # Source: https://stackoverflow.com/questions/5047734/in-osx-change-application-name-from-python
     if sys.platform.startswith("darwin"):
         # Set app name, if PyObjC is installed
         # Python 2 has PyObjC preinstalled
```

### Comparing `NeuroRuler-0.0/src/GUI/helpers.py` & `NeuroRuler-1.7/src/GUI/helpers.py`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0/src/GUI/main.py` & `NeuroRuler-1.7/src/GUI/main.py`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0/tests/test_img_helpers.py` & `NeuroRuler-1.7/tests/test_img_helpers.py`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0/tests/test_imgproc.py` & `NeuroRuler-1.7/tests/test_imgproc.py`

 * *Files identical despite different names*

