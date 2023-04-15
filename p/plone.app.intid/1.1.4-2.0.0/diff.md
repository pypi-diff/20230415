# Comparing `tmp/plone.app.intid-1.1.4.tar.gz` & `tmp/plone.app.intid-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.app.intid-1.1.4.tar", last modified: Mon Apr 20 10:32:50 2020, max compression
+gzip compressed data, was "plone.app.intid-2.0.0.tar", last modified: Sat Apr 15 07:57:48 2023, max compression
```

## Comparing `plone.app.intid-1.1.4.tar` & `plone.app.intid-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/
--rw-r--r--   0 maurits    (501) staff       (20)     4801 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     4801 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       16 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      848 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       53 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)      117 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone.app.intid.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      146 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     1594 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone/app/intid/
--rw-r--r--   0 maurits    (501) staff       (20)      986 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1120 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone/app/intid/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     2602 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       24 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2363 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/setuphandlers.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone/app/intid/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/plone/app/intid/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)       23 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/profiles/default/install_intids.txt
--rw-r--r--   0 maurits    (501) staff       (20)       68 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       23 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/profiles/default/intid_register_content.txt
--rw-r--r--   0 maurits    (501) staff       (20)      521 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/app/intid/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/plone/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       67 2020-04-20 10:32:50.000000 plone.app.intid-1.1.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      446 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      730 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2363 2020-04-20 10:32:49.000000 plone.app.intid-1.1.4/CHANGES.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.535512 plone.app.intid-2.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2538 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)    17987 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      730 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      146 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     3850 2023-04-15 07:57:48.535512 plone.app.intid-2.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      446 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.533512 plone.app.intid-2.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.534512 plone.app.intid-2.0.0/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.534512 plone.app.intid-2.0.0/plone/app/intid/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1027 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.532512 plone.app.intid-2.0.0/plone/app/intid/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.534512 plone.app.intid-2.0.0/plone/app/intid/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)       23 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/profiles/default/install_intids.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       23 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/profiles/default/intid_register_content.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       85 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1097 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/profiles.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2049 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/setuphandlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      492 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.535512 plone.app.intid-2.0.0/plone/app/intid/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2581 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone/app/intid/tests/test_setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:57:48.533512 plone.app.intid-2.0.0/plone.app.intid.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3850 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      848 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/entry_points.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      139 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/plone.app.intid.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1643 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:57:48.535512 plone.app.intid-2.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1596 2023-04-15 07:57:48.000000 plone.app.intid-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.app.intid-1.1.4/plone.app.intid.egg-info/SOURCES.txt` & `plone.app.intid-2.0.0/plone.app.intid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.intid-1.1.4/LICENSE.GPL` & `plone.app.intid-2.0.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.intid-1.1.4/setup.py` & `plone.app.intid-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,57 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
+
 import os
 
-version = '1.1.4'
+
+version = "2.0.0"
 
 setup(
-    name='plone.app.intid',
+    name="plone.app.intid",
     version=version,
-    description="Installation and migration support for five.intid within "
-                "Plone/CMF",
-    long_description='%s\n%s' % (
+    description="Installation and migration support for five.intid within " "Plone/CMF",
+    long_description="{}\n{}".format(
         open("README.rst").read(),
         open(os.path.join("CHANGES.rst")).read(),
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.0",
-        "Framework :: Plone :: 5.1",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    keywords='plone zope five intid',
-    author='Alec Mitchell',
-    author_email='apm13@columbia.edu',
-    url='https://github.com/plone/plone.app.intid',
-    license='GPL',
+    keywords="plone zope five intid",
+    author="Alec Mitchell",
+    author_email="apm13@columbia.edu",
+    url="https://github.com/plone/plone.app.intid",
+    license="GPL",
     packages=find_packages(),
-    namespace_packages=['plone', 'plone.app'],
+    namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
-        'setuptools',
-        'zope.intid',
-        'zope.lifecycleevent',
-        'five.intid>=1.0',
-        'Products.CMFCore',
+        "setuptools",
+        "zope.intid",
+        "zope.lifecycleevent",
+        "five.intid>=1.0",
+        "Products.CMFCore",
+        "Products.GenericSetup",
     ],
     extras_require={
-        'test': [
-            'plone.app.testing',
-            'plone.dexterity',
+        "test": [
+            "plone.app.testing",
+            "plone.dexterity",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
 )
```

### Comparing `plone.app.intid-1.1.4/plone/app/intid/configure.zcml` & `plone.app.intid-2.0.0/plone/app/intid/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone.app.intid">
+    i18n_domain="plone.app.intid"
+    >
 
-  <include package="five.intid" file="base.zcml" />
-  <include package="five.intid" file="cmfdirectoryview.zcml" />
+  <include
+      package="five.intid"
+      file="base.zcml"
+      />
+  <include
+      package="five.intid"
+      file="cmfdirectoryview.zcml"
+      />
   <include file="profiles.zcml" />
 
   <!-- Register intid handlers for all CMF/Plone content -->
   <subscriber
-      handler="five.intid.intid.addIntIdSubscriber"
       for="Products.CMFCore.interfaces.IDynamicType
            zope.lifecycleevent.interfaces.IObjectAddedEvent"
+      handler="five.intid.intid.addIntIdSubscriber"
       />
   <subscriber
-      handler="five.intid.intid.removeIntIdSubscriber"
       for="Products.CMFCore.interfaces.IDynamicType
            zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+      handler="five.intid.intid.removeIntIdSubscriber"
       />
   <subscriber
-      handler="five.intid.intid.moveIntIdSubscriber"
       for="Products.CMFCore.interfaces.IDynamicType
            zope.lifecycleevent.interfaces.IObjectMovedEvent"
+      handler="five.intid.intid.moveIntIdSubscriber"
       />
 
 </configure>
```

### Comparing `plone.app.intid-1.1.4/plone/app/intid/profiles.zcml` & `plone.app.intid-2.0.0/plone/app/intid/profiles.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    i18n_domain="plone.app.intid">
+    i18n_domain="plone.app.intid"
+    >
 
-    <genericsetup:registerProfile
-        name="default"
-        title="plone.app.intid: install utility"
-        directory="profiles/default"
-        description="Extension profile to install an intid utility in a Plone site"
-        for="Products.CMFCore.interfaces.ISiteRoot"
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        />
+  <genericsetup:registerProfile
+      name="default"
+      title="plone.app.intid: install utility"
+      description="Extension profile to install an intid utility in a Plone site"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      directory="profiles/default"
+      />
 
-    <genericsetup:importStep
-        name="import-intid-util"
-        title="Import IntId Utility"
-        description="Import intid utility."
-        handler=".setuphandlers.installIntIds">
-      <depends name="toolset"/>
-    </genericsetup:importStep>
+  <genericsetup:importStep
+      name="import-intid-util"
+      title="Import IntId Utility"
+      description="Import intid utility."
+      handler=".setuphandlers.installIntIds"
+      >
+    <depends name="toolset" />
+  </genericsetup:importStep>
 
-    <genericsetup:importStep
-        name="intid-register-content"
-        title="Register content with IntId utility"
-        description="Register all plone content with intid utility."
-        handler=".setuphandlers.registerContent">
-      <depends name="catalog"/>
-      <depends name="import-intid-util"/>
-    </genericsetup:importStep>
+  <genericsetup:importStep
+      name="intid-register-content"
+      title="Register content with IntId utility"
+      description="Register all plone content with intid utility."
+      handler=".setuphandlers.registerContent"
+      >
+    <depends name="catalog" />
+    <depends name="import-intid-util" />
+  </genericsetup:importStep>
 
-</configure>
+</configure>
```

### Comparing `plone.app.intid-1.1.4/plone/app/intid/tests/test_setup.py` & `plone.app.intid-2.0.0/plone/app/intid/tests/test_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.intid.testing import SETUP_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.dexterity.fti import DexterityFTI
 from Products.CMFCore.utils import getToolByName
 from zope.component import getUtility
 from zope.intid.interfaces import IIntIds
@@ -10,58 +9,58 @@
 import unittest
 
 
 class TestSetup(unittest.TestCase):
     layer = SETUP_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        # XXX below code is only needed if theres no Folder FTI already setup.
-        typetool = getToolByName(self.portal, 'portal_types')
-        if 'Folder' not in typetool.objectIds():
+        self.portal = self.layer["portal"]
+        # XXX below code is only needed if there's no Folder FTI already setup.
+        typetool = getToolByName(self.portal, "portal_types")
+        if "Folder" not in typetool.objectIds():
             # XXX Check if this is needed for Plone 5.0! In 4.3 the FTI is
             # already setup
-            fti = DexterityFTI('Folder')
-            typetool._setObject('Folder', fti)
+            fti = DexterityFTI("Folder")
+            typetool._setObject("Folder", fti)
 
     def tearDown(self):
-        setRoles(self.portal, TEST_USER_ID, ['Member'])
+        setRoles(self.portal, TEST_USER_ID, ["Member"])
 
     def test_already_installed(self):
         """plone.app.intid is a dependency of plone.app.linkintegrity
         which is a dependency of CMFPlone, so it is always installed.
         This tests if this is true.
         """
         # we create a folder
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
-        folder_id = self.portal.invokeFactory('Folder', 'folder')
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+        folder_id = self.portal.invokeFactory("Folder", "folder")
         folder = self.portal[folder_id]
         intids = getUtility(IIntIds)
         self.assertIsNotNone(intids.getId(folder))
 
-    @unittest.skip('p.a.intid is always installed')
+    @unittest.skip("p.a.intid is always installed")
     def test_install(self):
-        """When p.app.intid is intalled it registers some utility
+        """When p.app.intid is installed it registers some utility
         from zope.intid and five.intid and search in portal_catalog
         all contents in order to register them in these utilities.
 
         This test checks that all pre existing contents
         are registered correctly
         """
         from plone.app.intid.setuphandlers import add_intids
         from plone.app.testing import applyProfile
 
-        # we create a folder before the intallation of plone.app.intid
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
-        folder_id = self.portal.invokeFactory('Folder', 'folder')
+        # we create a folder before the installation of plone.app.intid
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+        folder_id = self.portal.invokeFactory("Folder", "folder")
         folder = self.portal[folder_id]
 
         # now we install manually the intid utilities
         add_intids(self.portal)
         intids = getUtility(IIntIds)
 
         # this folder is not referenced by intid utility
         self.assertRaises(KeyError, intids.getId, folder)
 
         # when we install p.app.intid our folder is referencend by intid
-        applyProfile(self.portal, 'plone.app.intid:default')
+        applyProfile(self.portal, "plone.app.intid:default")
         self.assertIsNotNone(intids.getId(folder))
```

### Comparing `plone.app.intid-1.1.4/plone/app/intid/setuphandlers.py` & `plone.app.intid-2.0.0/plone/app/intid/setuphandlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,34 @@
-# -*- coding: utf-8 -*-
 from five.intid.intid import IntIds
 from five.intid.site import addUtility
 from Products.CMFCore.interfaces import IContentish
 from Products.CMFCore.utils import getToolByName
 from zope.component import getUtility
 from zope.intid.interfaces import IIntIds
 
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
-try:
-    # XXX here we must consider plone.app.multilingual as well!
-    import Products.LinguaPlone
-    Products.LinguaPlone
-    HAS_LINGUAPLONE = True
-except ImportError:
-    HAS_LINGUAPLONE = False
-
-
 def register_all_content_for_intids(portal):
     """Registers all existing content with the intid utility.
     This will not be fast."""
-    cat = getToolByName(portal, 'portal_catalog', None)
+    cat = getToolByName(portal, "portal_catalog", None)
     if cat is None:
         return
     intids = getUtility(IIntIds)
     # Take advantage of paths stored in keyreferences in five.intid to optimize
     # registration
-    registered_paths = {
-        ref.path for ref in intids.ids
-        if hasattr(ref, 'path')
-    }
+    registered_paths = {ref.path for ref in intids.ids if hasattr(ref, "path")}
     # Count how many objects we register
     registered = 0
     existing = 0
-    query = {'object_provides': IContentish.__identifier__}
-    if HAS_LINGUAPLONE:
-        query['Language'] = 'all'
+    query = {"object_provides": IContentish.__identifier__}
     for brain in cat(query):
         if brain.getPath() in registered_paths:
             existing += 1
             continue
         try:
             obj = brain.getObject()
             intids.register(obj)
@@ -52,26 +37,27 @@
             # "TypeError" happens on a "could not adapt" - this may happen
             # for some contenttypes and must not stop this from working.
             logger.exception(brain.getURL())
     return registered, existing
 
 
 def add_intids(context):
-    addUtility(context, IIntIds, IntIds, ofs_name='intids',
-               findroot=False)
+    addUtility(context, IIntIds, IntIds, ofs_name="intids", findroot=False)
 
 
 def installIntIds(context):
-    if context.readDataFile('install_intids.txt') is None:
+    if context.readDataFile("install_intids.txt") is None:
         return
     portal = context.getSite()
     add_intids(portal)
-    return 'Added intid utility.'
+    return "Added intid utility."
 
 
 def registerContent(context):
-    if context.readDataFile('intid_register_content.txt') is None:
+    if context.readDataFile("intid_register_content.txt") is None:
         return
     portal = context.getSite()
     registered, existing = register_all_content_for_intids(portal)
-    return ('Assigned intids to {0} content objects, {1} objects '
-            'already had intids.'.format(registered, existing))
+    return (
+        "Assigned intids to {} content objects, {} objects "
+        "already had intids.".format(registered, existing)
+    )
```

### Comparing `plone.app.intid-1.1.4/LICENSE.txt` & `plone.app.intid-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.intid-1.1.4/CHANGES.rst` & `plone.app.intid-2.0.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,31 @@
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
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3b8337e6)
+
+
 1.1.4 (2020-04-20)
 ------------------
 
 Bug fixes:
 
 
 - Minor packaging updates. (#1)
@@ -108,15 +125,15 @@
 
 - Made compatible with Plone 3.3
   [alecm]
 
 1.0b2 2010-02-22
 -------------------
 
-- fixed dependecy of import profiles
+- fixed dependency of import profiles
   [naro]
 
 1.0b1 2010-02-07
 -------------------
 
 - Initial release
   [alecm]
```

