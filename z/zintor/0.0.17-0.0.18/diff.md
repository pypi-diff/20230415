# Comparing `tmp/zintor-0.0.17.tar.gz` & `tmp/zintor-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zintor-0.0.17.tar", last modified: Sun Apr  9 15:10:19 2023, max compression
+gzip compressed data, was "zintor-0.0.18.tar", last modified: Sat Apr 15 08:32:44 2023, max compression
```

## Comparing `zintor-0.0.17.tar` & `zintor-0.0.18.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.594263 zintor-0.0.17/
--rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-09 15:10:19.594263 zintor-0.0.17/PKG-INFO
--rw-r--r--   0 dzung     (1000) dzung     (1000)       38 2023-04-09 15:10:19.594263 zintor-0.0.17/setup.cfg
--rw-r--r--   0 dzung     (1000) dzung     (1000)     1362 2023-04-09 15:10:14.000000 zintor-0.0.17/setup.py
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.584263 zintor-0.0.17/zintor/
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.584263 zintor-0.0.17/zintor/src/
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.594263 zintor-0.0.17/zintor/src/zintor.egg-info/
--rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/PKG-INFO
--rw-r--r--   0 dzung     (1000) dzung     (1000)      233 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/SOURCES.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)        1 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/dependency_links.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)       74 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/requires.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)        7 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/top_level.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)     3130 2023-04-09 15:09:12.000000 zintor-0.0.17/zintor/src/zintor.py
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-15 08:32:44.374474 zintor-0.0.18/PKG-INFO
+-rw-r--r--   0 dzung     (1000) dzung     (1000)       38 2023-04-15 08:32:44.374474 zintor-0.0.18/setup.cfg
+-rw-r--r--   0 dzung     (1000) dzung     (1000)     1362 2023-04-15 08:32:40.000000 zintor-0.0.18/setup.py
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/zintor/
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/zintor/src/
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/zintor/src/zintor.egg-info/
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/PKG-INFO
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      233 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/SOURCES.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)        1 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/dependency_links.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)       74 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/requires.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)        7 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/top_level.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)     3130 2023-04-15 08:25:00.000000 zintor-0.0.18/zintor/src/zintor.py
```

### Comparing `zintor-0.0.17/setup.py` & `zintor-0.0.18/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zintor",                             # This is the name of the package
-    version="0.0.17",                        # The initial release version
+    version="0.0.18",                        # The initial release version
     author="__Async__",                     # Full name of the author
     description="Python Admin Package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `zintor-0.0.17/zintor/src/zintor.py` & `zintor-0.0.18/zintor/src/zintor.py`

 * *Files identical despite different names*

