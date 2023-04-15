# Comparing `tmp/plone.app.contentlisting-3.0.2.tar.gz` & `tmp/plone.app.contentlisting-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contentlisting-3.0.2.tar", last modified: Thu Apr  6 10:28:49 2023, max compression
+gzip compressed data, was "plone.app.contentlisting-3.0.3.tar", last modified: Sat Apr 15 08:09:46 2023, max compression
```

## Comparing `plone.app.contentlisting-3.0.2.tar` & `plone.app.contentlisting-3.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:49.048473 plone.app.contentlisting-3.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      270 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      128 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)      973 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)     6755 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      144 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    17345 2023-04-06 10:28:49.048618 plone.app.contentlisting-3.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     9752 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:49.040634 plone.app.contentlisting-3.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      686 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:49.040934 plone.app.contentlisting-3.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:49.043839 plone.app.contentlisting-3.0.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:49.046592 plone.app.contentlisting-3.0.2/plone/app/contentlisting/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1455 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     5990 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1677 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5954 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/contentlisting.py
--rw-r--r--   0 maurits    (501) staff       (20)     2165 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3769 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/realobject.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:49.048130 plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1726 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     8027 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/integration.rst
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/test_integration_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)    16709 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/test_integration_unit.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:28:49.043536 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    17345 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1135 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      224 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1670 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-06 10:28:49.049152 plone.app.contentlisting-3.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1846 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1282 2023-04-06 10:28:48.000000 plone.app.contentlisting-3.0.2/tox.ini
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.808544 plone.app.contentlisting-3.0.3/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1019 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/.editorconfig
+-rw-r--r--   0 gil       (1000) gil       (1000)      270 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/.gitignore
+-rw-r--r--   0 gil       (1000) gil       (1000)      128 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/.meta.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      973 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 gil       (1000) gil       (1000)     6949 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      144 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    17539 2023-04-15 08:09:46.809544 plone.app.contentlisting-3.0.3/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     9752 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.806544 plone.app.contentlisting-3.0.3/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      686 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.806544 plone.app.contentlisting-3.0.3/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.807544 plone.app.contentlisting-3.0.3/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.808544 plone.app.contentlisting-3.0.3/plone/app/contentlisting/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1455 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/browser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5990 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/catalog.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1677 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     5954 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/contentlisting.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2165 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3769 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/realobject.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.808544 plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1726 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/base.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8027 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/integration.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      591 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/test_integration_doctest.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    16709 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/test_integration_unit.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:09:46.807544 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    17539 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1135 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/entry_points.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      201 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1670 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 08:09:46.809544 plone.app.contentlisting-3.0.3/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1812 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1282 2023-04-15 08:09:46.000000 plone.app.contentlisting-3.0.3/tox.ini
```

### Comparing `plone.app.contentlisting-3.0.2/.editorconfig` & `plone.app.contentlisting-3.0.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/.pre-commit-config.yaml` & `plone.app.contentlisting-3.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/CHANGES.rst` & `plone.app.contentlisting-3.0.3/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Drop p.a.contenttypes install dependency, it is actually a soft one only.
+  This allows to break a cyclic dependency.
+  [gforcada] (#3764)
+
+
 3.0.2 (2023-04-06)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentlisting-3.0.2/PKG-INFO` & `plone.app.contentlisting-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentlisting
-Version: 3.0.2
+Version: 3.0.3
 Summary: Listing of content for the Plone CMS
 Home-page: https://pypi.org/project/plone.app.contentlisting
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: content list Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -283,14 +283,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Drop p.a.contenttypes install dependency, it is actually a soft one only.
+  This allows to break a cyclic dependency.
+  [gforcada] (#3764)
+
+
 3.0.2 (2023-04-06)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentlisting-3.0.2/README.rst` & `plone.app.contentlisting-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/docs/LICENSE.GPL` & `plone.app.contentlisting-3.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/docs/LICENSE.txt` & `plone.app.contentlisting-3.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/browser.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/browser.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/catalog.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/configure.zcml` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/contentlisting.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/contentlisting.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/interfaces.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/realobject.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/realobject.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/base.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/integration.rst` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/integration.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/test_integration_doctest.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/test_integration_doctest.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone/app/contentlisting/tests/test_integration_unit.py` & `plone.app.contentlisting-3.0.3/plone/app/contentlisting/tests/test_integration_unit.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/PKG-INFO` & `plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentlisting
-Version: 3.0.2
+Version: 3.0.3
 Summary: Listing of content for the Plone CMS
 Home-page: https://pypi.org/project/plone.app.contentlisting
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: content list Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -283,14 +283,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Drop p.a.contenttypes install dependency, it is actually a soft one only.
+  This allows to break a cyclic dependency.
+  [gforcada] (#3764)
+
+
 3.0.2 (2023-04-06)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentlisting-3.0.2/plone.app.contentlisting.egg-info/SOURCES.txt` & `plone.app.contentlisting-3.0.3/plone.app.contentlisting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/pyproject.toml` & `plone.app.contentlisting-3.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.2/setup.py` & `plone.app.contentlisting-3.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
-version = "3.0.2"
+version = "3.0.3"
 
 long_description = "{}\n\n{}".format(read("README.rst"), read("CHANGES.rst"))
 
 setup(
     name="plone.app.contentlisting",
     version=version,
     description="Listing of content for the Plone CMS",
@@ -40,15 +40,14 @@
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "setuptools",
         "plone.base",
         "Products.MimetypesRegistry",
         "Products.ZCatalog",
-        "plone.app.contenttypes",
         "plone.i18n",
         "plone.registry",
         "plone.rfc822",
         "plone.uuid",
     ],
     extras_require={
         "test": [
```

### Comparing `plone.app.contentlisting-3.0.2/tox.ini` & `plone.app.contentlisting-3.0.3/tox.ini`

 * *Files identical despite different names*

