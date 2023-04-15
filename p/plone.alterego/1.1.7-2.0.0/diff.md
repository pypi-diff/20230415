# Comparing `tmp/plone.alterego-1.1.7.tar.gz` & `tmp/plone.alterego-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.alterego-1.1.7.tar", last modified: Sat Apr 15 08:28:57 2023, max compression
+gzip compressed data, was "plone.alterego-2.0.0.tar", last modified: Sat Apr 15 07:53:47 2023, max compression
```

## Comparing `plone.alterego-1.1.7.tar` & `plone.alterego-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:28:57.926665 plone.alterego-1.1.7/
--rw-r--r--   0 gil       (1000) gil       (1000)     1490 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      142 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)     5486 2023-04-15 08:28:57.927665 plone.alterego-1.1.7/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     2960 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:28:57.925665 plone.alterego-1.1.7/docs/
--rw-r--r--   0 gil       (1000) gil       (1000)     1222 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/docs/INSTALL.txt
--rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/docs/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      743 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/docs/LICENSE.txt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:28:57.925665 plone.alterego-1.1.7/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       80 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:28:57.926665 plone.alterego-1.1.7/plone/alterego/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone/alterego/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4955 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone/alterego/alterego.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1199 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone/alterego/dynamic.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1058 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone/alterego/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)      806 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone/alterego/tests.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:28:57.926665 plone.alterego-1.1.7/plone.alterego.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)     5486 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone.alterego.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      561 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone.alterego.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone.alterego.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone.alterego.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone.alterego.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)       49 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone.alterego.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/plone.alterego.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      423 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      115 2023-04-15 08:28:57.927665 plone.alterego-1.1.7/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     1663 2023-04-15 08:28:57.000000 plone.alterego-1.1.7/setup.py
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

### Comparing `plone.alterego-1.1.7/CHANGES.rst` & `plone.alterego-2.0.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-1.1.7 (2023-04-15)
+2.0.0 (2023-04-15)
 ------------------
 
-Bug fixes:
+Breaking changes:
 
 
-- Reverted accidental changes introduced in previous release.
-  The 1.x series are meant to be Plone 5.2 and Python 2.7 compatible.
+- Drop python 2 support.
   [gforcada] (#1)
 
 
 1.1.6 (2023-04-15)
 ------------------
 
 Internal:
```

### Comparing `plone.alterego-1.1.7/PKG-INFO` & `plone.alterego-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.alterego
-Version: 1.1.7
+Version: 2.0.0
 Summary: Low level support for dynamic modules
 Home-page: https://github.com/plone/plone.alterego
 Author: Laurence Rowe
 Author-email: plone-developers@lists.sourceforge.net
 License: LGPL
 Keywords: Plone schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Provides-Extra: test
 
 ==============
 plone.alterego
 ==============
 
 Now you see it, it now you don't!
@@ -126,22 +127,21 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-1.1.7 (2023-04-15)
+2.0.0 (2023-04-15)
 ------------------
 
-Bug fixes:
+Breaking changes:
 
 
-- Reverted accidental changes introduced in previous release.
-  The 1.x series are meant to be Plone 5.2 and Python 2.7 compatible.
+- Drop python 2 support.
   [gforcada] (#1)
 
 
 1.1.6 (2023-04-15)
 ------------------
 
 Internal:
```

### Comparing `plone.alterego-1.1.7/README.rst` & `plone.alterego-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.7/docs/INSTALL.txt` & `plone.alterego-2.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.7/docs/LICENSE.GPL` & `plone.alterego-2.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.7/docs/LICENSE.txt` & `plone.alterego-2.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.7/plone/alterego/alterego.txt` & `plone.alterego-2.0.0/plone/alterego/alterego.txt`

 * *Files 5% similar despite different names*

```diff
@@ -104,32 +104,22 @@
     <InterfaceClass plone.alterego.tests.dynamic.IOne>
 
 We could then create an on-demand interface easily:
 
     >>> interface.alsoProvides(c1, dynamic.ITwo)
     Creating ITwo in plone.alterego.tests.dynamic
 
-    >>> list(interface.providedBy(c1).flattened()) # doctest: +NORMALIZE_WHITESPACE +SKIP_PYTHON_3
-    [<InterfaceClass plone.alterego.tests.dynamic.ITwo>,
-     <InterfaceClass __builtin__.IContent>,
-     <InterfaceClass zope.interface.Interface>]
-
-    >>> list(interface.providedBy(c1).flattened()) # doctest: +NORMALIZE_WHITESPACE +SKIP_PYTHON_2
+    >>> list(interface.providedBy(c1).flattened()) # doctest: +NORMALIZE_WHITESPACE
     [<InterfaceClass plone.alterego.tests.dynamic.ITwo>,
      <InterfaceClass builtins.IContent>,
      <InterfaceClass zope.interface.Interface>]
 
 Crucially, so long as the factory always returns the same thing, the same
 objects will be returned each time the module is accessed.
 
     >>> del dynamic
     >>> del dynamic_module
 
-    >>> list(interface.providedBy(c1).flattened()) # doctest: +NORMALIZE_WHITESPACE +SKIP_PYTHON_3
-    [<InterfaceClass plone.alterego.tests.dynamic.ITwo>,
-     <InterfaceClass __builtin__.IContent>,
-     <InterfaceClass zope.interface.Interface>]
-
-    >>> list(interface.providedBy(c1).flattened()) # doctest: +NORMALIZE_WHITESPACE +SKIP_PYTHON_2
+    >>> list(interface.providedBy(c1).flattened()) # doctest: +NORMALIZE_WHITESPACE
     [<InterfaceClass plone.alterego.tests.dynamic.ITwo>,
      <InterfaceClass builtins.IContent>,
      <InterfaceClass zope.interface.Interface>]
```

### Comparing `plone.alterego-1.1.7/plone/alterego/dynamic.py` & `plone.alterego-2.0.0/plone/alterego/dynamic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-# -*- coding: utf-8 -*-
 from plone.alterego.interfaces import IDynamicModule
 from plone.alterego.interfaces import IDynamicObjectFactory
 from types import ModuleType
 from zope.component import queryUtility
 from zope.interface import implementer
 
 import sys
 
 
 @implementer(IDynamicModule)
 class DynamicModule(ModuleType):
-    """A module that can create objects on the fly.
-    """
+    """A module that can create objects on the fly."""
 
     def __getattr__(self, name):
-
-        if name == '__path__':
-            raise AttributeError('Dynamic modules do not have __path__')
+        if name == "__path__":
+            raise AttributeError("Dynamic modules do not have __path__")
 
         factory = queryUtility(IDynamicObjectFactory, name=self.__name__)
         if factory is None:
             raise AttributeError(
-                'Cannot find dynamic object factory for module {0}'.format(
+                "Cannot find dynamic object factory for module {}".format(
                     self.__name__,
                 )
             )
 
         obj = factory(name, self)
         if obj is None:
             raise AttributeError(
-                'Dynamic module factory did not want to create '
-                '{0} in {1}'.format(name, self.__name__)
+                "Dynamic module factory did not want to create "
+                "{} in {}".format(name, self.__name__)
             )
 
         return obj
 
 
 def create(dotted_name):
     dynamic = DynamicModule(dotted_name)
     sys.modules[dotted_name] = dynamic
     return dynamic
 
 
-__all__ = ('create',)
+__all__ = ("create",)
```

### Comparing `plone.alterego-1.1.7/plone/alterego/interfaces.py` & `plone.alterego-2.0.0/plone/alterego/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Interface
 
 
 class IDynamicModule(Interface):
-    """Marker interface for dynamic modules
-    """
+    """Marker interface for dynamic modules"""
 
 
 class IDynamicObjectFactory(Interface):
     """A factory capable of creating objects on the fly.
 
     This should be registered as a named utility. The name is the name of
     the dynamic module. Thus, there is a one-to-one mapping between the
```

### Comparing `plone.alterego-1.1.7/plone.alterego.egg-info/PKG-INFO` & `plone.alterego-2.0.0/plone.alterego.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.alterego
-Version: 1.1.7
+Version: 2.0.0
 Summary: Low level support for dynamic modules
 Home-page: https://github.com/plone/plone.alterego
 Author: Laurence Rowe
 Author-email: plone-developers@lists.sourceforge.net
 License: LGPL
 Keywords: Plone schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Provides-Extra: test
 
 ==============
 plone.alterego
 ==============
 
 Now you see it, it now you don't!
@@ -126,22 +127,21 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-1.1.7 (2023-04-15)
+2.0.0 (2023-04-15)
 ------------------
 
-Bug fixes:
+Breaking changes:
 
 
-- Reverted accidental changes introduced in previous release.
-  The 1.x series are meant to be Plone 5.2 and Python 2.7 compatible.
+- Drop python 2 support.
   [gforcada] (#1)
 
 
 1.1.6 (2023-04-15)
 ------------------
 
 Internal:
```

### Comparing `plone.alterego-1.1.7/plone.alterego.egg-info/SOURCES.txt` & `plone.alterego-2.0.0/plone.alterego.egg-info/SOURCES.txt`

 * *Files identical despite different names*

