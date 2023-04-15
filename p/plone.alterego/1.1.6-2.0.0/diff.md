# Comparing `tmp/plone.alterego-1.1.6.tar.gz` & `tmp/plone.alterego-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.alterego-1.1.6.tar", last modified: Sat Apr 15 07:51:42 2023, max compression
+gzip compressed data, was "plone.alterego-2.0.0.tar", last modified: Sat Apr 15 07:53:47 2023, max compression
```

## Comparing `plone.alterego-1.1.6.tar` & `plone.alterego-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/
--rw-r--r--   0 gil       (1000) gil       (1000)     1286 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      142 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)     5305 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     2960 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.571155 plone.alterego-1.1.6/docs/
--rw-r--r--   0 gil       (1000) gil       (1000)     1222 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/docs/INSTALL.txt
--rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/docs/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      743 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/docs/LICENSE.txt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.571155 plone.alterego-1.1.6/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/plone/alterego/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4427 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/alterego.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1166 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/dynamic.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1029 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)      277 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/tests.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.571155 plone.alterego-1.1.6/plone.alterego.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)     5305 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      561 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)       49 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1643 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     1632 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:53:47.789426 plone.alterego-2.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1390 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      142 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     5409 2023-04-15 07:53:47.789426 plone.alterego-2.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2960 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:53:47.787426 plone.alterego-2.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1222 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/docs/INSTALL.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      743 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:53:47.787426 plone.alterego-2.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:53:47.789426 plone.alterego-2.0.0/plone/alterego/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone/alterego/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4427 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone/alterego/alterego.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1166 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone/alterego/dynamic.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1029 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone/alterego/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      277 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone/alterego/tests.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:53:47.788426 plone.alterego-2.0.0/plone.alterego.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     5409 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone.alterego.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      561 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone.alterego.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone.alterego.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone.alterego.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone.alterego.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)       49 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone.alterego.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/plone.alterego.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1643 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:53:47.789426 plone.alterego-2.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1632 2023-04-15 07:53:47.000000 plone.alterego-2.0.0/setup.py
```

### Comparing `plone.alterego-1.1.6/CHANGES.rst` & `plone.alterego-2.0.0/CHANGES.rst`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.0 (2023-04-15)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2 support.
+  [gforcada] (#1)
+
+
 1.1.6 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.alterego-1.1.6/PKG-INFO` & `plone.alterego-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.alterego
-Version: 1.1.6
+Version: 2.0.0
 Summary: Low level support for dynamic modules
 Home-page: https://github.com/plone/plone.alterego
 Author: Laurence Rowe
 Author-email: plone-developers@lists.sourceforge.net
 License: LGPL
 Keywords: Plone schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -127,14 +127,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.0 (2023-04-15)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2 support.
+  [gforcada] (#1)
+
+
 1.1.6 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.alterego-1.1.6/README.rst` & `plone.alterego-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/docs/INSTALL.txt` & `plone.alterego-2.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/docs/LICENSE.GPL` & `plone.alterego-2.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/docs/LICENSE.txt` & `plone.alterego-2.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/plone/alterego/alterego.txt` & `plone.alterego-2.0.0/plone/alterego/alterego.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/plone/alterego/dynamic.py` & `plone.alterego-2.0.0/plone/alterego/dynamic.py`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/plone/alterego/interfaces.py` & `plone.alterego-2.0.0/plone/alterego/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/plone.alterego.egg-info/PKG-INFO` & `plone.alterego-2.0.0/plone.alterego.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.alterego
-Version: 1.1.6
+Version: 2.0.0
 Summary: Low level support for dynamic modules
 Home-page: https://github.com/plone/plone.alterego
 Author: Laurence Rowe
 Author-email: plone-developers@lists.sourceforge.net
 License: LGPL
 Keywords: Plone schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -127,14 +127,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.0 (2023-04-15)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2 support.
+  [gforcada] (#1)
+
+
 1.1.6 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.alterego-1.1.6/plone.alterego.egg-info/SOURCES.txt` & `plone.alterego-2.0.0/plone.alterego.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/pyproject.toml` & `plone.alterego-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.6/setup.py` & `plone.alterego-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "1.1.6"
+version = "2.0.0"
 
 setup(
     name="plone.alterego",
     version=version,
     description="Low level support for dynamic modules",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     # Get more strings from
```

