# Comparing `tmp/plone.alterego-1.1.5.tar.gz` & `tmp/plone.alterego-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.alterego-1.1.5.tar", last modified: Mon Apr 20 09:22:40 2020, max compression
+gzip compressed data, was "plone.alterego-1.1.6.tar", last modified: Sat Apr 15 07:51:42 2023, max compression
```

## Comparing `plone.alterego-1.1.5.tar` & `plone.alterego-1.1.6.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/
--rw-r--r--   0 maurits    (501) staff       (20)     6405 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     6405 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      602 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       33 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       49 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone.alterego.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      423 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      142 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     1222 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)      743 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1663 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/plone/alterego/
--rw-r--r--   0 maurits    (501) staff       (20)     1058 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/plone/alterego/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     4955 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/plone/alterego/alterego.txt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/plone/alterego/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1199 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/plone/alterego/dynamic.py
--rw-r--r--   0 maurits    (501) staff       (20)      806 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/plone/alterego/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)      115 2020-04-20 09:22:40.000000 plone.alterego-1.1.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2833 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2020-04-20 09:22:39.000000 plone.alterego-1.1.5/CHANGES.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1286 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      142 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     5305 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2960 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.571155 plone.alterego-1.1.6/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1222 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/docs/INSTALL.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      743 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.571155 plone.alterego-1.1.6/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/plone/alterego/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4427 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/alterego.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1166 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/dynamic.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1029 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      277 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone/alterego/tests.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:51:42.571155 plone.alterego-1.1.6/plone.alterego.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     5305 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      561 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)       49 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/plone.alterego.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1643 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:51:42.572155 plone.alterego-1.1.6/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1632 2023-04-15 07:51:42.000000 plone.alterego-1.1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.alterego-1.1.5/plone.alterego.egg-info/SOURCES.txt` & `plone.alterego-1.1.6/plone.alterego.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.alterego.egg-info/PKG-INFO
 plone.alterego.egg-info/SOURCES.txt
 plone.alterego.egg-info/dependency_links.txt
-plone.alterego.egg-info/entry_points.txt
 plone.alterego.egg-info/namespace_packages.txt
 plone.alterego.egg-info/not-zip-safe
 plone.alterego.egg-info/requires.txt
 plone.alterego.egg-info/top_level.txt
 plone/alterego/__init__.py
 plone/alterego/alterego.txt
 plone/alterego/dynamic.py
```

### Comparing `plone.alterego-1.1.5/docs/LICENSE.GPL` & `plone.alterego-1.1.6/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.5/docs/INSTALL.txt` & `plone.alterego-1.1.6/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.5/docs/LICENSE.txt` & `plone.alterego-1.1.6/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.alterego-1.1.5/setup.py` & `plone.alterego-1.1.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,50 @@
-# -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '1.1.5'
+version = "1.1.6"
 
 setup(
-    name='plone.alterego',
+    name="plone.alterego",
     version=version,
-    description='Low level support for dynamic modules',
-    long_description=(open('README.rst').read() + '\n' +
-                      open('CHANGES.rst').read()),
+    description="Low level support for dynamic modules",
+    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     # Get more strings from
     # https://pypi.org/classifiers/
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Framework :: Plone',
-        'Framework :: Plone :: 4.3',
-        'Framework :: Plone :: 5.0',
-        'Framework :: Plone :: 5.1',
-        'Framework :: Plone :: 5.2',
-        'Framework :: Plone :: Core',
-        'License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Development Status :: 5 - Production/Stable",
+        "Framework :: Plone",
+        "Framework :: Plone :: 4.3",
+        "Framework :: Plone :: 5.0",
+        "Framework :: Plone :: 5.1",
+        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: Core",
+        "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    keywords='Plone schema interface',
-    author='Laurence Rowe',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://github.com/plone/plone.alterego',
-    license='LGPL',
+    keywords="Plone schema interface",
+    author="Laurence Rowe",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://github.com/plone/plone.alterego",
+    license="LGPL",
     packages=find_packages(),
-    namespace_packages=['plone'],
+    namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
-        'setuptools',
-        'zope.component',
-        'zope.interface',
+        "setuptools",
+        "zope.component",
+        "zope.interface",
     ],
-    extras_require={
-        'test': []
-    },
+    extras_require={"test": []},
     entry_points="""
     # -*- Entry points: -*-
     """,
 )
```

### Comparing `plone.alterego-1.1.5/plone/alterego/interfaces.py` & `plone.alterego-1.1.6/plone/alterego/interfaces.py`

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

### Comparing `plone.alterego-1.1.5/plone/alterego/alterego.txt` & `plone.alterego-1.1.6/plone/alterego/alterego.txt`

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

### Comparing `plone.alterego-1.1.5/plone/alterego/dynamic.py` & `plone.alterego-1.1.6/plone/alterego/dynamic.py`

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

### Comparing `plone.alterego-1.1.5/README.rst` & `plone.alterego-1.1.6/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -8,79 +8,88 @@
 dynamic module on demand.
 
 Usage
 -----
 
 To use this package, you should:
 
- - Identify an appropriate parent module where the dynamic module will live.
+- Identify an appropriate parent module where the dynamic module will live.
 
- - Ensure that plone.alterego.dynamic.create() is called with this module and
-   a dynamic module name. Typically, you'd do this in the parent module
-   itself, so that the dynamic module is instantiated as soon as the parent
-   module is imported.
-
- - Register a named utility providing IDynamicObjectFactory. The name should
-   be the same as the full dotted path to the dynamic module. This utility
-   will be responsible for creating the objects that inhabit the dynamic
-   module.
+- Ensure that plone.alterego.dynamic.create() is called with this module and a dynamic module name. 
+  Typically, you'd do this in the parent module itself, so that the dynamic module is instantiated as soon as the parent module is imported.
+
+- Register a named utility providing IDynamicObjectFactory. 
+  The name should be the same as the full dotted path to the dynamic module. 
+  This utility will be responsible for creating the objects that inhabit the dynamicmodule.
 
 Example
 -------
 
 For a more fully-featured example, see the alterego.txt doctest.
 
 Let's say we have a generic content class that should get a unique interface
 for each instance.
 
+.. code-block:: python
+
     >>> from zope import interface
     >>> class IContent(interface.Interface):
     ...     pass
     >>> class Content(object):
     ...     interface.implements(IContent)
 
     >>> c1 = Content()
 
 To create the unique interface, we will use a dynamic module. There is a
 helper method to make this easier. It takes a parent module and a name as
 arguments:
 
+.. code-block:: python
+
     >>> from plone.alterego.dynamic import create
     >>> dynamic = create('plone.alterego.tests.dynamic')
 
 We can now import this module:
 
+.. code-block:: python
+
     >>> from plone.alterego.tests import dynamic
 
 To make objects on demand, we'll need to register a utility that can act
 as a factory.
 
+.. code-block:: python
+
     >>> from plone.alterego.interfaces import IDynamicObjectFactory
     >>> from zope.interface.interface import InterfaceClass
     >>> class InterfaceOnDemand(object):
     ...     interface.implements(IDynamicObjectFactory)
     ...
     ...     def __call__(self, name, module):
     ...         schema = InterfaceClass(name, (interface.Interface,), __module__=module.__name__)
     ...         setattr(module, name, schema)
     ...         return schema
 
 This utility should have a name that corresponds to the full,
 dotted name to the dynamic module. This way, we can have different factories
-for different dynamic modules. We'd register this in ZCML like so::
+for different dynamic modules. We'd register this in ZCML like so:
+
+.. code-block:: XML
 
     <utility
         name="plone.alterego.tests.dynamic"
         provides="plone.alterego.interfaces.IDynamicObjectFactory"
         factory=".factory.InterfaceOnDemand"
         />
 
 From this point forward, when we access an attribute of the dynamic module,
 the factory will be used:
 
+.. code-block:: python
+
     >>> dynamic.IOne
     <InterfaceClass plone.alterego.tests.dynamic.IOne>
 
 Note that so long as the setattr() call above is executed, the factory is
 called only once. That is, you'll always get the same object each time you
 access a given attribute of the dynamic module.
```

### Comparing `plone.alterego-1.1.5/CHANGES.rst` & `plone.alterego-1.1.6/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.6 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 1.1.5 (2020-04-20)
 ------------------
 
 Bug fixes:
 
 
 - Minor packaging updates. (#1)
```

