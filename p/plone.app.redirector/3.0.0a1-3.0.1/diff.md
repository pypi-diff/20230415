# Comparing `tmp/plone.app.redirector-3.0.0a1.tar.gz` & `tmp/plone.app.redirector-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.redirector-3.0.0a1.tar", last modified: Thu Apr  7 22:08:42 2022, max compression
+gzip compressed data, was "plone.app.redirector-3.0.1.tar", last modified: Sat Apr 15 07:59:59 2023, max compression
```

## Comparing `plone.app.redirector-3.0.0a1.tar` & `plone.app.redirector-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-04-07 22:08:42.262188 plone.app.redirector-3.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)     6413 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      162 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     8786 2022-04-07 22:08:42.262348 plone.app.redirector-3.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1496 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-04-07 22:08:42.255303 plone.app.redirector-3.0.0a1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      682 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-04-07 22:08:42.255571 plone.app.redirector-3.0.0a1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-04-07 22:08:42.257903 plone.app.redirector-3.0.0a1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-04-07 22:08:42.260039 plone.app.redirector-3.0.0a1/plone/app/redirector/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7556 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)      855 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2592 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      662 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/policy.py
--rw-r--r--   0 maurits    (501) staff       (20)     7742 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)     1405 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)      909 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-04-07 22:08:42.261939 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2111 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     6405 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_events.py
--rw-r--r--   0 maurits    (501) staff       (20)     4480 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_performance.py
--rw-r--r--   0 maurits    (501) staff       (20)      697 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)    20820 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_storage.py
--rw-r--r--   0 maurits    (501) staff       (20)     9179 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_view.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-04-07 22:08:42.257636 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     8786 2022-04-07 22:08:41.000000 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1036 2022-04-07 22:08:42.000000 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-04-07 22:08:41.000000 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-04-07 22:08:41.000000 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-04-07 22:08:41.000000 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       82 2022-04-07 22:08:41.000000 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-04-07 22:08:41.000000 plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      172 2022-04-07 22:08:42.262860 plone.app.redirector-3.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1355 2022-04-07 22:08:40.000000 plone.app.redirector-3.0.0a1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:59:59.871679 plone.app.redirector-3.0.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)     6613 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      162 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     9039 2023-04-15 07:59:59.871679 plone.app.redirector-3.0.1/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1496 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:59:59.868679 plone.app.redirector-3.0.1/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      682 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:59:59.868679 plone.app.redirector-3.0.1/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:59:59.869679 plone.app.redirector-3.0.1/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:59:59.870679 plone.app.redirector-3.0.1/plone/app/redirector/
+-rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7556 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/browser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      820 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2592 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      662 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/policy.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7742 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/storage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1405 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/subscribers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      908 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:59:59.871679 plone.app.redirector-3.0.1/plone/app/redirector/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2111 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/tests/test_browser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6405 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/tests/test_events.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4480 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/tests/test_performance.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      697 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/tests/test_setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    20820 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/tests/test_storage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9179 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone/app/redirector/tests/test_view.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:59:59.869679 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     9039 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1036 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      181 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/plone.app.redirector.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1690 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:59:59.871679 plone.app.redirector-3.0.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1670 2023-04-15 07:59:59.000000 plone.app.redirector-3.0.1/setup.py
```

### Comparing `plone.app.redirector-3.0.0a1/CHANGES.rst` & `plone.app.redirector-3.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,34 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (93e1ab65)
+
+
+3.0.0 (2022-11-30)
+------------------
+
+Bug fixes:
+
+
+- Final release.
+  [gforcada] (#600)
+
+
 3.0.0a1 (2022-04-08)
 --------------------
 
 Breaking changes:
 
 
 - Plone 6 only, remove Archetypes specific code.
@@ -255,15 +275,15 @@
   [wichert]
 
 - Move event subscribers to a separate zcml file so they can easily be
   excluded.
   [wichert]
 
 - Update browser view to handle environments where the storage utility is not
-  availbale.
+  available.
   [wichert]
 
 
 1.0.11 - 2009-04-05
 -------------------
 
 - Fixed multiple steps circular references #8840
```

### Comparing `plone.app.redirector-3.0.0a1/PKG-INFO` & `plone.app.redirector-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.app.redirector
-Version: 3.0.0a1
+Version: 3.0.1
 Summary: redirection tool
 Home-page: https://github.com/plone/plone.app.redirector
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: links redirect
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 by Martin Aspeli <optilude@gmx.net> based on work by Helge Tesdal
 (RedirectionTool) and Whit Morriss (topp.rose).
@@ -64,14 +65,34 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (93e1ab65)
+
+
+3.0.0 (2022-11-30)
+------------------
+
+Bug fixes:
+
+
+- Final release.
+  [gforcada] (#600)
+
+
 3.0.0a1 (2022-04-08)
 --------------------
 
 Breaking changes:
 
 
 - Plone 6 only, remove Archetypes specific code.
@@ -315,15 +336,15 @@
   [wichert]
 
 - Move event subscribers to a separate zcml file so they can easily be
   excluded.
   [wichert]
 
 - Update browser view to handle environments where the storage utility is not
-  availbale.
+  available.
   [wichert]
 
 
 1.0.11 - 2009-04-05
 -------------------
 
 - Fixed multiple steps circular references #8840
@@ -390,9 +411,7 @@
 
 
 1.0 - 2007-08-17
 ----------------
 
 - Initial release.
   [optilude]
-
-
```

### Comparing `plone.app.redirector-3.0.0a1/README.rst` & `plone.app.redirector-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/docs/LICENSE.GPL` & `plone.app.redirector-3.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/docs/LICENSE.txt` & `plone.app.redirector-3.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/browser.py` & `plone.app.redirector-3.0.1/plone/app/redirector/browser.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/configure.zcml` & `plone.app.redirector-3.0.1/plone/app/redirector/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:browser="http://namespaces.zope.org/browser">
+    xmlns:browser="http://namespaces.zope.org/browser"
+    >
 
-    <adapter factory=".policy.RedirectionPolicy" />
+  <adapter factory=".policy.RedirectionPolicy" />
 
-    <!-- Register a page the UI -->
-    <browser:page
-        name="plone_redirector_view"
-        for="*"
-        class=".browser.FourOhFourView"
-        permission="zope2.View"
-        allowed_interface=".interfaces.IFourOhFourView"
-        />
-
-    <!-- Remember the movements of CMF objects -->
-    <subscriber
-        for="Products.CMFCore.interfaces.IContentish
-             zope.lifecycleevent.interfaces.IObjectMovedEvent"
-        handler=".subscribers.objectMoved"
-        />
-
-    <subscriber
-        for="Products.CMFCore.interfaces.IContentish
-             zope.lifecycleevent.interfaces.IObjectRemovedEvent"
-        handler=".subscribers.objectRemoved"
-        />
+  <!-- Register a page the UI -->
+  <browser:page
+      name="plone_redirector_view"
+      for="*"
+      class=".browser.FourOhFourView"
+      allowed_interface=".interfaces.IFourOhFourView"
+      permission="zope2.View"
+      />
+
+  <!-- Remember the movements of CMF objects -->
+  <subscriber
+      for="Products.CMFCore.interfaces.IContentish
+           zope.lifecycleevent.interfaces.IObjectMovedEvent"
+      handler=".subscribers.objectMoved"
+      />
+
+  <subscriber
+      for="Products.CMFCore.interfaces.IContentish
+           zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+      handler=".subscribers.objectRemoved"
+      />
 
 
 </configure>
```

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/interfaces.py` & `plone.app.redirector-3.0.1/plone/app/redirector/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/policy.py` & `plone.app.redirector-3.0.1/plone/app/redirector/policy.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/storage.py` & `plone.app.redirector-3.0.1/plone/app/redirector/storage.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/subscribers.py` & `plone.app.redirector-3.0.1/plone/app/redirector/subscribers.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/testing.py` & `plone.app.redirector-3.0.1/plone/app/redirector/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
 from zope.configuration import xmlconfig
 
 
 class PloneAppRedirector(PloneSandboxLayer):
-
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import plone.app.redirector
 
         xmlconfig.file(
             "configure.zcml", plone.app.redirector, context=configurationContext
```

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_browser.py` & `plone.app.redirector-3.0.1/plone/app/redirector/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_events.py` & `plone.app.redirector-3.0.1/plone/app/redirector/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_performance.py` & `plone.app.redirector-3.0.1/plone/app/redirector/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_setup.py` & `plone.app.redirector-3.0.1/plone/app/redirector/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_storage.py` & `plone.app.redirector-3.0.1/plone/app/redirector/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/plone/app/redirector/tests/test_view.py` & `plone.app.redirector-3.0.1/plone/app/redirector/tests/test_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from plone.app.redirector.interfaces import IRedirectionStorage
 from plone.app.redirector.testing import PLONE_APP_REDIRECTOR_INTEGRATION_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
+from plone.base.interfaces import ISearchSchema
 from plone.registry.interfaces import IRegistry
-from Products.CMFPlone.interfaces import ISearchSchema
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 
 import unittest
 
 
 class TestRedirectorView(unittest.TestCase):
@@ -181,16 +181,16 @@
         urls = sorted(b.getURL() for b in view.search_for_similar())
         self.assertEqual(1, len(urls))
         self.assertEqual(fu + "/f1/p1", urls[0])
 
     def test_search_query_parser_error(self):
         view = self.view(self.portal, self.portal.absolute_url() + "/&")
         try:
-            urls = view.search_for_similar()
-        except:
+            _ = view.search_for_similar()
+        except Exception:
             self.fail("Query parsing error was not handled.")
 
     def test_search_blacklisted(self):
         self.folder.invokeFactory("Folder", "f1")
         self.folder.invokeFactory("Folder", "f2")
         self.folder.f1.invokeFactory("Document", "p1")
         self.folder.f1.invokeFactory("Document", "p2")
```

### Comparing `plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/PKG-INFO` & `plone.app.redirector-3.0.1/plone.app.redirector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.app.redirector
-Version: 3.0.0a1
+Version: 3.0.1
 Summary: redirection tool
 Home-page: https://github.com/plone/plone.app.redirector
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: links redirect
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 by Martin Aspeli <optilude@gmx.net> based on work by Helge Tesdal
 (RedirectionTool) and Whit Morriss (topp.rose).
@@ -64,14 +65,34 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (93e1ab65)
+
+
+3.0.0 (2022-11-30)
+------------------
+
+Bug fixes:
+
+
+- Final release.
+  [gforcada] (#600)
+
+
 3.0.0a1 (2022-04-08)
 --------------------
 
 Breaking changes:
 
 
 - Plone 6 only, remove Archetypes specific code.
@@ -315,15 +336,15 @@
   [wichert]
 
 - Move event subscribers to a separate zcml file so they can easily be
   excluded.
   [wichert]
 
 - Update browser view to handle environments where the storage utility is not
-  availbale.
+  available.
   [wichert]
 
 
 1.0.11 - 2009-04-05
 -------------------
 
 - Fixed multiple steps circular references #8840
@@ -390,9 +411,7 @@
 
 
 1.0 - 2007-08-17
 ----------------
 
 - Initial release.
   [optilude]
-
-
```

### Comparing `plone.app.redirector-3.0.0a1/plone.app.redirector.egg-info/SOURCES.txt` & `plone.app.redirector-3.0.1/plone.app.redirector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.redirector-3.0.0a1/setup.py` & `plone.app.redirector-3.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.0a1"
+version = "3.0.1"
 
 setup(
     name="plone.app.redirector",
     version=version,
     description="redirection tool",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
@@ -15,27 +15,41 @@
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="links redirect",
     author="Plone Foundation",
     author_email="plone-developers@lists.sourceforge.net",
     url="https://github.com/plone/plone.app.redirector",
     license="GPL version 2",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
         "setuptools",
         "plone.memoize",
         "Zope>=5",
+        "BTrees",
+        "Products.CMFCore",
+        "Products.ZCatalog",
+        "persistent",
     ],
-    extras_require={"test": ["plone.app.testing", "plone.app.contenttypes"]},
+    extras_require={
+        "test": [
+            "plone.app.testing",
+            "plone.app.contenttypes[test]",
+            "plone.base",
+            "plone.registry",
+            "plone.testing",
+        ]
+    },
 )
```

