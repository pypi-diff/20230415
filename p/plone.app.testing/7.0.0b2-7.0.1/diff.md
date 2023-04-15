# Comparing `tmp/plone.app.testing-7.0.0b2.tar.gz` & `tmp/plone.app.testing-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.testing-7.0.0b2.tar", last modified: Tue Oct 11 21:05:46 2022, max compression
+gzip compressed data, was "plone.app.testing-7.0.1.tar", last modified: Sat Apr 15 08:08:30 2023, max compression
```

## Comparing `plone.app.testing-7.0.0b2.tar` & `plone.app.testing-7.0.1.tar`

### file list

```diff
@@ -1,51 +1,49 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.587843 plone.app.testing-7.0.0b2/
--rw-r--r--   0 maurits    (501) staff       (20)    12293 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      175 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    70132 2022-10-11 21:05:46.587986 plone.app.testing-7.0.0b2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    56770 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1953 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.580947 plone.app.testing-7.0.0b2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      674 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)    56770 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7041 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)      498 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1451 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/isolation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5253 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/views.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1437 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/docs/zope-testbrowser.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      645 2022-10-11 21:05:46.588600 plone.app.testing-7.0.0b2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2655 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      116 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/sphinx.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.575727 plone.app.testing-7.0.0b2/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.581161 plone.app.testing-7.0.0b2/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.583258 plone.app.testing-7.0.0b2/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.587216 plone.app.testing-7.0.0b2/src/plone/app/testing/
--rw-r--r--   0 maurits    (501) staff       (20)     1826 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3703 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/bbb.py
--rw-r--r--   0 maurits    (501) staff       (20)     4512 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/bbb_at.py
--rw-r--r--   0 maurits    (501) staff       (20)      973 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/cleanup.py
--rw-r--r--   0 maurits    (501) staff       (20)      891 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/cleanup.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16564 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/helpers.py
--rw-r--r--   0 maurits    (501) staff       (20)    19785 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/helpers.rst
--rw-r--r--   0 maurits    (501) staff       (20)      423 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    15630 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/layers.py
--rw-r--r--   0 maurits    (501) staff       (20)    17393 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/layers.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4926 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/layers_zserver.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.587458 plone.app.testing-7.0.0b2/src/plone/app/testing/profile/
--rw-r--r--   0 maurits    (501) staff       (20)      121 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/profile/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     7273 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/selenium.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3683 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/selenium_layers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1404 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)      972 2022-10-11 21:05:45.000000 plone.app.testing-7.0.0b2/src/plone/app/testing/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 21:05:46.582945 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    70132 2022-10-11 21:05:46.000000 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1169 2022-10-11 21:05:46.000000 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-11 21:05:46.000000 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-10-11 21:05:46.000000 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-11 21:05:46.000000 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      475 2022-10-11 21:05:46.000000 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-10-11 21:05:46.000000 plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/top_level.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.629654 plone.app.testing-7.0.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)    12498 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      175 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    70444 2023-04-15 08:08:30.629654 plone.app.testing-7.0.1/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)    56770 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1953 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/buildout.cfg
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.627654 plone.app.testing-7.0.1/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      674 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    56770 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     7122 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/conf.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      498 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/index.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1452 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/isolation.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     5253 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/views.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1437 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/docs/zope-testbrowser.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1736 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      277 2023-04-15 08:08:30.630654 plone.app.testing-7.0.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     2682 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      116 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/sphinx.cfg
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.625654 plone.app.testing-7.0.1/src/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.627654 plone.app.testing-7.0.1/src/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.627654 plone.app.testing-7.0.1/src/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.629654 plone.app.testing-7.0.1/src/plone/app/testing/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1781 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3647 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/bbb.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      936 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/cleanup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      891 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/cleanup.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)    16534 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/helpers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    19786 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/helpers.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      403 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14580 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/layers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    17383 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/layers.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.629654 plone.app.testing-7.0.1/src/plone/app/testing/profile/
+-rw-r--r--   0 gil       (1000) gil       (1000)      138 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/profile/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     7273 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/selenium.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     3631 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/selenium_layers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      833 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/tests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      885 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone/app/testing/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:08:30.627654 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    70444 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1096 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      501 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:08:30.000000 plone.app.testing-7.0.1/src/plone.app.testing.egg-info/top_level.txt
```

### Comparing `plone.app.testing-7.0.0b2/CHANGES.rst` & `plone.app.testing-7.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+7.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (434550cc)
+
+
+7.0.0 (2022-12-02)
+------------------
+
+Bug fixes:
+
+
+- Final release for Plone 6.0.0. (#600)
+
+
 7.0.0b2 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Restore the previously used admin password for tests ("secret") [davisagli] (#79)
@@ -185,15 +204,15 @@
   For Plone 5.2 the bbb.PloneTestCase will uses Dexterity instead of Archetypes.
   Adding bbb_at.PloneTestCase for them to use allows to keep the AT tests working.
   See https://github.com/plone/plone.app.testing/pull/51
   [pbauer]
 
 Bug fixes:
 
-- Amended the doctests to work with automatical layer port picking from plone.testing.
+- Amended the doctests to work with automatically layer port picking from plone.testing.
   [Rotonen]
 
 
 5.0.8 (2017-10-25)
 ------------------
 
 Bug fixes:
@@ -339,15 +358,15 @@
   [davisagli]
 
 - fix: ``Products.CMFPlone`` needs the ``gopip`` index from
   ``plone.app.folder``. So latter has to be initialized before CMFPlones
   profile is applied (which installs the index to catalog). At the moment
   CMFPlone therefore registers the index itself, but plone.app.folder
   registers it too, which resulted in plone/Products.CMFPlone#313
-  "GopipIndex registered twice" In tests the registration does not succedd,
+  "GopipIndex registered twice" In tests the registration does not succeed,
   because plone.app.folder was never initialized as z2 products. In order to
   remove the misleading regisatration from CMFPlone we must take care that the
   index is available, which is achieved with this change. Also minor pep8
   optimizations in the file touched.
   [jensens]
 
 - create memberfolder, if it is not there for testing.
```

### Comparing `plone.app.testing-7.0.0b2/PKG-INFO` & `plone.app.testing-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: plone.app.testing
-Version: 7.0.0b2
+Version: 7.0.1
 Summary: Testing tools for Plone-the-application, based on plone.testing.
 Home-page: https://pypi.org/project/plone.app.testing
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone tests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 4
+Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: robot
 
 Introduction
 ============
 
 .. contents:: Table of contents
@@ -1588,14 +1591,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+7.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (434550cc)
+
+
+7.0.0 (2022-12-02)
+------------------
+
+Bug fixes:
+
+
+- Final release for Plone 6.0.0. (#600)
+
+
 7.0.0b2 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Restore the previously used admin password for tests ("secret") [davisagli] (#79)
@@ -1769,15 +1791,15 @@
   For Plone 5.2 the bbb.PloneTestCase will uses Dexterity instead of Archetypes.
   Adding bbb_at.PloneTestCase for them to use allows to keep the AT tests working.
   See https://github.com/plone/plone.app.testing/pull/51
   [pbauer]
 
 Bug fixes:
 
-- Amended the doctests to work with automatical layer port picking from plone.testing.
+- Amended the doctests to work with automatically layer port picking from plone.testing.
   [Rotonen]
 
 
 5.0.8 (2017-10-25)
 ------------------
 
 Bug fixes:
@@ -1923,15 +1945,15 @@
   [davisagli]
 
 - fix: ``Products.CMFPlone`` needs the ``gopip`` index from
   ``plone.app.folder``. So latter has to be initialized before CMFPlones
   profile is applied (which installs the index to catalog). At the moment
   CMFPlone therefore registers the index itself, but plone.app.folder
   registers it too, which resulted in plone/Products.CMFPlone#313
-  "GopipIndex registered twice" In tests the registration does not succedd,
+  "GopipIndex registered twice" In tests the registration does not succeed,
   because plone.app.folder was never initialized as z2 products. In order to
   remove the misleading regisatration from CMFPlone we must take care that the
   index is available, which is achieved with this change. Also minor pep8
   optimizations in the file touched.
   [jensens]
 
 - create memberfolder, if it is not there for testing.
```

### Comparing `plone.app.testing-7.0.0b2/README.rst` & `plone.app.testing-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/buildout.cfg` & `plone.app.testing-7.0.1/buildout.cfg`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/docs/LICENSE.GPL` & `plone.app.testing-7.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/docs/LICENSE.txt` & `plone.app.testing-7.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/docs/README.rst` & `plone.app.testing-7.0.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/docs/conf.py` & `plone.app.testing-7.0.1/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,216 +1,224 @@
-# -*- coding: utf-8 -*-
 #
 # plone.app.testing documentation build configuration file, created by
 # sphinx-quickstart on Sat Feb  9 11:31:41 2013.
 #
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys, os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = []
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'plone.app.testing'
-copyright = u'2018, Plone Foundation'
+project = "plone.app.testing"
+copyright = "2018, Plone Foundation"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '5.0'
+version = "5.0"
 # The full version, including alpha/beta/rc tags.
-release = '5.0'
+release = "5.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'ploneapptestingdoc'
+htmlhelp_basename = "ploneapptestingdoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 # The paper size ('letter' or 'a4').
-#latex_paper_size = 'letter'
+# latex_paper_size = 'letter'
 
 # The font size ('10pt', '11pt' or '12pt').
-#latex_font_size = '10pt'
+# latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'ploneapptesting.tex', u'plone.app.testing Documentation',
-   u'Plone Foundation', 'manual'),
+    (
+        "index",
+        "ploneapptesting.tex",
+        "plone.app.testing Documentation",
+        "Plone Foundation",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Additional stuff for the LaTeX preamble.
-#latex_preamble = ''
+# latex_preamble = ''
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'ploneapptesting', u'plone.app.testing Documentation',
-     [u'Plone Foundation'], 1)
+    (
+        "index",
+        "ploneapptesting",
+        "plone.app.testing Documentation",
+        ["Plone Foundation"],
+        1,
+    )
 ]
```

### Comparing `plone.app.testing-7.0.0b2/docs/isolation.rst` & `plone.app.testing-7.0.1/docs/isolation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Test Isolation is hard
 ======================
 
 At the moment, it is not possible to just run all tests at once.
-Therfore we have an alltests script that groups tests together.
+Therefore we have an alltests script that groups tests together.
 
 You may wonder, why and which tests need to be separated.
 
 plone.app.testing vs ZopeTestCase
 ---------------------------------
 
 plone.app.testing goes at great lengths to isolate tests.
```

### Comparing `plone.app.testing-7.0.0b2/docs/views.rst` & `plone.app.testing-7.0.1/docs/views.rst`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/docs/zope-testbrowser.rst` & `plone.app.testing-7.0.1/docs/zope-testbrowser.rst`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/__init__.py` & `plone.app.testing-7.0.1/src/plone/app/testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-# flake8: NOQA: F401
 from plone.app.testing.cleanup import cleanUpMultiPlugins
 from plone.app.testing.helpers import applyProfile
 from plone.app.testing.helpers import login
 from plone.app.testing.helpers import logout
 from plone.app.testing.helpers import PloneSandboxLayer
 from plone.app.testing.helpers import ploneSite
 from plone.app.testing.helpers import PloneWithPackageLayer
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/bbb.py` & `plone.app.testing-7.0.1/src/plone/app/testing/bbb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Backwards-compatibility test class for PloneTestCase for Dexterity."""
 
 from AccessControl import getSecurityManager
 from plone.app import testing
 from plone.testing import zope
 from Products.CMFPlone.utils import _createObjectByType
 from Testing.ZopeTestCase.functional import Functional
@@ -11,103 +10,102 @@
 import unittest
 
 
 def _createMemberarea(portal, user_id):
     mtool = portal.portal_membership
     members = mtool.getMembersFolder()
     if members is None:
-        _createObjectByType('Folder', portal, id='Members')
+        _createObjectByType("Folder", portal, id="Members")
     if not mtool.getMemberareaCreationFlag():
         mtool.setMemberareaCreationFlag()
     mtool.createMemberArea(user_id)
     if mtool.getMemberareaCreationFlag():
         mtool.setMemberareaCreationFlag()
 
 
 class PloneTestCaseFixture(testing.PloneSandboxLayer):
-
     defaultBases = (testing.PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import plone.app.contenttypes
+
         self.loadZCML(package=plone.app.contenttypes)
 
     def setUpPloneSite(self, portal):
         # restore default workflow
-        testing.applyProfile(portal, 'Products.CMFPlone:testfixture')
+        testing.applyProfile(portal, "Products.CMFPlone:testfixture")
 
         # add default content
-        testing.applyProfile(portal, 'plone.app.contenttypes:plone-content')
+        testing.applyProfile(portal, "plone.app.contenttypes:plone-content")
 
         # add home folder for default test user
         _createMemberarea(portal, testing.TEST_USER_ID)
 
 
 PTC_FIXTURE = PloneTestCaseFixture()
 PTC_FUNCTIONAL_TESTING = testing.FunctionalTesting(
-    bases=(PTC_FIXTURE,), name='PloneTestCase:Functional')
+    bases=(PTC_FIXTURE,), name="PloneTestCase:Functional"
+)
 
 
 class PloneTestCase(Functional, unittest.TestCase):
-
     layer = PTC_FUNCTIONAL_TESTING
 
     def setUp(self):
         """Set up before each test."""
         self.beforeSetUp()
-        self.app = self.layer['app']
-        self.portal = self.layer['portal']
-        self.folder = self.portal.portal_membership.getHomeFolder(
-            testing.TEST_USER_ID)
+        self.app = self.layer["app"]
+        self.portal = self.layer["portal"]
+        self.folder = self.portal.portal_membership.getHomeFolder(testing.TEST_USER_ID)
         transaction.commit()
         self.afterSetUp()
 
     def beforeSetUp(self):
         """Hook to do setup before the portal is created."""
         pass
 
     def afterSetUp(self):
         """Hook to do setup after the portal is created."""
 
     def tearDown(self):
         """Tear down after each test."""
         self.beforeTearDown()
         transaction.abort()
-        super(PloneTestCase, self).tearDown()
+        super().tearDown()
         self.afterTearDown()
 
     def beforeTearDown(self):
         """Hook to do teardown before the portal is removed."""
 
     def afterTearDown(self):
         """Hook to do teardown after the portal is removed."""
 
     def setRoles(self, roles, name=testing.TEST_USER_ID):
         """Set the effective roles of a user."""
         testing.setRoles(self.portal, name, roles)
 
     def setGroups(self, groups, name=testing.TEST_USER_ID):
-        '''Changes the user's groups.'''
-        uf = self.portal['acl_users']
+        """Changes the user's groups."""
+        uf = self.portal["acl_users"]
         uf.userSetGroups(name, list(groups))
         user = getSecurityManager().getUser()
         if name == user.getId():
             self.login(user.getUserName())
 
-    def setPermissions(self, permissions, role='Member'):
+    def setPermissions(self, permissions, role="Member"):
         """Changes the permissions assigned to role."""
         self.portal.manage_role(role, list(permissions))
 
     def login(self, userName=testing.TEST_USER_NAME):
         """Log in to the portal as the given user."""
         testing.login(self.portal, userName)
 
     def loginAsPortalOwner(self, userName=testing.SITE_OWNER_NAME):
         """Log in to the portal as the user who created it."""
-        zope.login(self.app['acl_users'], userName)
+        zope.login(self.app["acl_users"], userName)
 
     def logout(self):
         """Log out, i.e. become anonymous."""
         testing.logout()
 
     def createMemberarea(self, name):
         """Create a minimal memberarea."""
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/cleanup.py` & `plone.app.testing-7.0.1/src/plone/app/testing/cleanup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# -*- coding: utf-8 -*-
 """Cleanup handlers for various global registries
 """
 
 from zope.testing.cleanup import addCleanUp
 
 
 # Make sure cleanup handlers from GenericSetup are registered
 try:
     import Products.GenericSetup.zcml
 except ImportError:
     pass
 
 # Make sure cleanup handlers from PAS are registered
 try:
-    import Products.PluggableAuthService.zcml  # NOQA: F401
+    import Products.PluggableAuthService.zcml  # noqa: F401
 except ImportError:
     pass
 
 
 def cleanUpMultiPlugins():
     try:
-        from Products.PluggableAuthService.PluggableAuthService import MultiPlugins  # NOQA: E501
+        from Products.PluggableAuthService.PluggableAuthService import MultiPlugins
+
     except ImportError:
         pass
     else:
-
         zap = []
 
         # Don't stomp on the things the other cleanup handler will deal with
         from Products.PluggableAuthService import zcml
+
         for plugin in MultiPlugins:
             if plugin not in zcml._mt_regs:
                 zap.append(plugin)
 
         for plugin in zap:
             MultiPlugins.remove(plugin)
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/cleanup.rst` & `plone.app.testing-7.0.1/src/plone/app/testing/cleanup.rst`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/helpers.py` & `plone.app.testing-7.0.1/src/plone/app/testing/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Helper functions for Plone testing. Also importable from plone.app.testing
 # directly
 
 from plone.app.testing import layers
 from plone.app.testing.interfaces import PLONE_SITE_ID
 from plone.app.testing.interfaces import SITE_OWNER_NAME
 from plone.app.testing.interfaces import TEST_USER_NAME
@@ -20,32 +19,29 @@
 import contextlib
 
 
 # User management
 
 
 def login(portal, userName):
-    """Log in as the given user in the given Plone site
-    """
+    """Log in as the given user in the given Plone site"""
 
-    zope.login(portal['acl_users'], userName)
+    zope.login(portal["acl_users"], userName)
 
 
 def logout():
-    """Log out, i.e. become anonymous
-    """
+    """Log out, i.e. become anonymous"""
 
     zope.logout()
 
 
 def setRoles(portal, userId, roles):
-    """Set the given user's roles to a tuple of roles.
-    """
+    """Set the given user's roles to a tuple of roles."""
 
-    userFolder = portal['acl_users']
+    userFolder = portal["acl_users"]
     zope.setRoles(userFolder, userId, roles)
 
 
 def tearDownMultiPluginRegistration(pluginName):
     """Remove the given PAS MultiPlugin name from the global PAS registry.
     Does nothing if the plugin name is not registered.
 
@@ -71,22 +67,22 @@
     """Install a product using the add-ons control panel (portal setup).
 
     If ``reinstall`` is false and the product is already installed, do nothing.
     If ``reinstall`` is true, perform an uninstall and install if the product
     is installed already.
     """
 
-    from Acquisition import aq_parent
     from AccessControl import getSecurityManager
     from AccessControl.SecurityManagement import setSecurityManager
+    from Acquisition import aq_parent
 
     sm = getSecurityManager()
     app = aq_parent(portal)
 
-    zope.login(app['acl_users'], SITE_OWNER_NAME)
+    zope.login(app["acl_users"], SITE_OWNER_NAME)
 
     from Products.CMFPlone.utils import get_installer
 
     qi = get_installer(portal)
 
     try:
         if not qi.is_product_installed(productName):
@@ -98,39 +94,45 @@
         portal.clearCurrentSkin()
         portal.setupCurrentSkin(portal.REQUEST)
 
     finally:
         setSecurityManager(sm)
 
 
-def applyProfile(portal, profileName, purge_old=None,
-                 ignore_dependencies=False, archive=None,
-                 blacklisted_steps=None):
+def applyProfile(
+    portal,
+    profileName,
+    purge_old=None,
+    ignore_dependencies=False,
+    archive=None,
+    blacklisted_steps=None,
+):
     """Install an extension profile into the portal. The profile name
     should be a package name and a profile name, e.g. 'my.product:default'.
     """
 
-    from Acquisition import aq_parent
     from AccessControl import getSecurityManager
     from AccessControl.SecurityManagement import setSecurityManager
+    from Acquisition import aq_parent
 
     sm = getSecurityManager()
     app = aq_parent(portal)
 
-    zope.login(app['acl_users'], SITE_OWNER_NAME)
+    zope.login(app["acl_users"], SITE_OWNER_NAME)
 
     try:
-        setupTool = portal['portal_setup']
-        profileId = 'profile-{0}'.format(profileName)
+        setupTool = portal["portal_setup"]
+        profileId = f"profile-{profileName}"
         setupTool.runAllImportStepsFromProfile(
             profileId,
             purge_old=purge_old,
             ignore_dependencies=ignore_dependencies,
             archive=archive,
-            blacklisted_steps=blacklisted_steps)
+            blacklisted_steps=blacklisted_steps,
+        )
 
         portal.clearCurrentSkin()
         portal.setupCurrentSkin(portal.REQUEST)
 
     finally:
         setSecurityManager(sm)
 
@@ -154,15 +156,15 @@
     site = getSite()
 
     localSiteManager = portal.getSiteManager()
 
     current = zca.pushGlobalRegistry(new=new)
 
     if current not in localSiteManager.__bases__:
-        localSiteManager.__bases__ = (current, )
+        localSiteManager.__bases__ = (current,)
 
     if site is not None:
         setHooks()
         setSite(site)
 
     return current
 
@@ -212,14 +214,15 @@
 
     Until at least Products.GenericSetup 1.8.3 this is a standard
     non-persistent dictionary, which means a transaction rollback does
     not rollback changes to this dictionary.  So we make it a persistent
     mapping.  Call this once in layer setup and you have easy rollback.
     """
     from persistent.mapping import PersistentMapping
+
     puv = portal.portal_setup._profile_upgrade_versions
     if isinstance(puv, PersistentMapping):
         return
     portal.portal_setup._profile_upgrade_versions = PersistentMapping(puv)
 
 
 @contextlib.contextmanager
@@ -241,15 +244,15 @@
 
     flavour ... either `plone.testing.z2` resp. `plone.testing.zope` for WSGI
                 or `plone.testing.zserver` for ZServer
     """
     setHooks()
     site = getSite()
 
-    with getattr(flavour, 'zopeApp')(db, connection, environ) as app:
+    with getattr(flavour, "zopeApp")(db, connection, environ) as app:
         portal = app[PLONE_SITE_ID]
 
         setSite(portal)
         login(portal, TEST_USER_NAME)
 
         try:
             yield portal
@@ -269,15 +272,15 @@
     Base classes must override and implemented ``setUpPloneSite()``. They
     may also implement ``tearDownPloneSite()``, and can optionally change
     the ``defaultBases`` tuple.
     """
 
     # The default list of bases.
 
-    defaultBases = (layers.PLONE_FIXTURE, )
+    defaultBases = (layers.PLONE_FIXTURE,)
 
     # Hooks
 
     def setUpZope(self, app, configurationContext):
         """Set up Zope.
 
         ``app`` is the Zope application root.
@@ -310,35 +313,38 @@
         pass
 
     def tearDownPloneSite(self, portal):
         """Tear down the Plone site.
 
         Implementing this is optional. If the changes made during the
         ``setUpPloneSite()`` method were confined to the ZODB and the global
-        component regsitry, those changes will be torn down automatically.
+        component registry, those changes will be torn down automatically.
         """
 
         pass
 
     # Boilerplate
 
     def setUp(self):
         try:
             # Push a new database storage so that database changes
-            # commited during layer setup can be easily torn down
-            self['zodbDB'] = zodb.stackDemoStorage(self.get('zodbDB'),
-                                                   name=self.__name__)
+            # committed during layer setup can be easily torn down
+            self["zodbDB"] = zodb.stackDemoStorage(
+                self.get("zodbDB"), name=self.__name__
+            )
 
             # Push a new configuration context so that it's possible to
             # re-import ZCML files after tear-down
-            name = self.__name__ if self.__name__ is not None else 'not-named'
-            contextName = 'PloneSandboxLayer-{0}'.format(name)
-            self['configurationContext'] = configurationContext = (
-                zca.stackConfigurationContext(self.get('configurationContext'),
-                                              name=contextName))
+            name = self.__name__ if self.__name__ is not None else "not-named"
+            contextName = f"PloneSandboxLayer-{name}"
+            self[
+                "configurationContext"
+            ] = configurationContext = zca.stackConfigurationContext(
+                self.get("configurationContext"), name=contextName
+            )
 
             with ploneSite() as portal:
                 setHooks()
 
                 # Make sure there's no local site manager while we load ZCML
                 setSite(None)
 
@@ -351,15 +357,17 @@
                 persist_profile_upgrade_versions(portal)
 
                 # Make sure zope.security checkers can be set up and torn down
                 # reliably
 
                 security.pushCheckers()
 
-                from Products.PluggableAuthService.PluggableAuthService import MultiPlugins  # noqa
+                from Products.PluggableAuthService.PluggableAuthService import (
+                    MultiPlugins,
+                )
 
                 preSetupMultiPlugins = MultiPlugins[:]
 
                 # Allow subclass to load ZCML and products
                 self.setUpZope(portal.getPhysicalRoot(), configurationContext)
 
                 # Snapshot Dexterity schemas
@@ -369,23 +377,21 @@
                 setSite(portal)
                 self.setUpPloneSite(portal)
                 setSite(None)
 
             # Keep track of PAS plugins that were added during setup
             self.snapshotMultiPlugins(preSetupMultiPlugins)
         except Exception:
-            del self['configurationContext']
-            self['zodbDB'].close()
-            del self['zodbDB']
+            del self["configurationContext"]
+            self["zodbDB"].close()
+            del self["zodbDB"]
             raise
 
     def tearDown(self):
-
         with zope.zopeApp() as app:
-
             portal = app[PLONE_SITE_ID]
             setHooks()
             setSite(portal)
 
             # Allow subclass to tear down persistent fixture
             self.tearDownPloneSite(portal)
 
@@ -406,43 +412,52 @@
             # Remove PAS plugins
             self.tearDownMultiPlugins()
 
             # Allow subclass to tear down products
             self.tearDownZope(app)
 
         # Zap the configuration context
-        del self['configurationContext']
+        del self["configurationContext"]
 
         # Pop the demo storage, thus restoring the database to the
         # previous state
-        self['zodbDB'].close()
-        del self['zodbDB']
+        self["zodbDB"].close()
+        del self["zodbDB"]
 
     # Helpers
-    def applyProfile(self, portal, profileName, purge_old=None,
-                     ignore_dependencies=False, archive=None,
-                     blacklisted_steps=None):
-        return applyProfile(portal, profileName, purge_old,
-                            ignore_dependencies, archive,
-                            blacklisted_steps)
+    def applyProfile(
+        self,
+        portal,
+        profileName,
+        purge_old=None,
+        ignore_dependencies=False,
+        archive=None,
+        blacklisted_steps=None,
+    ):
+        return applyProfile(
+            portal,
+            profileName,
+            purge_old,
+            ignore_dependencies,
+            archive,
+            blacklisted_steps,
+        )
 
-    def loadZCML(self, name='configure.zcml', **kw):
-        kw.setdefault('context', self['configurationContext'])
+    def loadZCML(self, name="configure.zcml", **kw):
+        kw.setdefault("context", self["configurationContext"])
         return xmlconfig.file(name, **kw)
 
     def snapshotMultiPlugins(self, preSetupMultiPlugins):
         """Save a snapshot of all PAS multi plugins that were added during
         setup, by comparing to the list of plugins passed in.
         """
 
         self._addedMultiPlugins = set()
 
-        from Products.PluggableAuthService.PluggableAuthService import (
-            MultiPlugins
-        )
+        from Products.PluggableAuthService.PluggableAuthService import MultiPlugins
 
         for plugin in MultiPlugins:
             if plugin not in preSetupMultiPlugins:
                 self._addedMultiPlugins.add(plugin)
 
     def tearDownMultiPlugins(self):
         """Delete all PAS multi plugins that were added during setup, as
@@ -451,35 +466,43 @@
 
         for pluginName in self._addedMultiPlugins:
             tearDownMultiPluginRegistration(pluginName)
 
     def snapshotGeneratedSchemas(self):
         """Save a snapshot of the plone.dexterity.schema.generated module"""
         from plone.dexterity.schema import generated
+
         self._generatedSchemas = generated.__dict__.copy()
         todelete = []
         for k in generated.__dict__:
-            if not k.startswith('_'):
+            if not k.startswith("_"):
                 todelete.append(k)
         for k in todelete:
             del generated.__dict__[k]
 
     def tearDownGeneratedSchemas(self):
         """Reset plone.dexterity.schema.generated to its previous state"""
         from plone.dexterity.schema import generated
+
         generated.__dict__.clear()
         generated.__dict__.update(self._generatedSchemas)
 
 
 class PloneWithPackageLayer(PloneSandboxLayer):
-
-    def __init__(self, bases=None, name=None, module=None, zcml_filename=None,
-                 zcml_package=None, gs_profile_id=None,
-                 additional_z2_products=()):
-        super(PloneWithPackageLayer, self).__init__(bases, name, module)
+    def __init__(
+        self,
+        bases=None,
+        name=None,
+        module=None,
+        zcml_filename=None,
+        zcml_package=None,
+        gs_profile_id=None,
+        additional_z2_products=(),
+    ):
+        super().__init__(bases, name, module)
         self.zcml_filename = zcml_filename
         self.zcml_package = zcml_package
         self.gs_profile_id = gs_profile_id
         self.additional_z2_products = additional_z2_products
 
     def setUpZope(self, app, configurationContext):
         """Set up Zope.
@@ -492,19 +515,18 @@
 
     def setUpZCMLFiles(self):
         """Load default ZCML.
 
         Can be overridden to load more ZCML.
         """
         if self.zcml_filename is None:
-            raise ValueError('ZCML file name has not been provided.')
+            raise ValueError("ZCML file name has not been provided.")
         if self.zcml_package is None:
             raise ValueError(
-                'The package that contains the ZCML file '
-                'has not been provided.'
+                "The package that contains the ZCML file " "has not been provided."
             )
         self.loadZCML(self.zcml_filename, package=self.zcml_package)
 
     def setUpPloneSite(self, portal):
         """Set up the Plone site.
 
         Only install GenericSetup profiles
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/helpers.rst` & `plone.app.testing-7.0.1/src/plone/app/testing/helpers.rst`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     >>> class HelperDemos(Layer):
     ...     defaultBases = (PLONE_FIXTURE,)
     ...
     ...     def setUp(self):
     ...
     ...         # Push a new database storage so that database changes
-    ...         # commited during layer setup can be easily torn down
+    ...         # committed during layer setup can be easily torn down
     ...         self['zodbDB'] = zodb.stackDemoStorage(self.get('zodbDB'), name='HelperDemos')
     ...
     ...         # Push a new configuration context so that it's possible to re-import
     ...         # ZCML files after tear-down
     ...         self['configurationContext'] = zca.stackConfigurationContext(self.get('configurationContext'))
     ...
     ...         with helpers.ploneSite() as portal:
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/layers.py` & `plone.app.testing-7.0.1/src/plone/app/testing/layers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Layers setting up fixtures with a Plone site. Also importable from
 # plone.app.testing directly
 
 from Acquisition import aq_base
 from plone.app.testing.interfaces import DEFAULT_LANGUAGE
 from plone.app.testing.interfaces import PLONE_SITE_ID
 from plone.app.testing.interfaces import PLONE_SITE_TITLE
@@ -23,15 +22,14 @@
 from zope.component import getSiteManager
 from zope.component import getUtility
 from zope.component.hooks import setSite
 from zope.dottedname.resolve import resolve
 from zope.event import notify
 from zope.traversing.interfaces import BeforeTraverseEvent
 
-import six
 import transaction
 
 
 class PloneFixture(Layer):
     """This layer sets up a basic Plone site, with:
 
     * No content
@@ -41,223 +39,191 @@
       role, ``Member``.
     """
 
     defaultBases = (zope.STARTUP,)
 
     # Products that will be installed, plus options
     products = (
-        ('Products.GenericSetup', {'loadZCML': True}, ),
-        ('Products.DCWorkflow', {'loadZCML': True}, ),
-        ('Products.ZCTextIndex', {'loadZCML': True}, ),
-        ('Products.DateRecurringIndex', {'loadZCML': False}, ),
-        ('Products.PageTemplates', {'loadZCML': True}, ),
-        ('Products.CMFUid', {'loadZCML': True}, ),
-        ('Products.CMFCore', {'loadZCML': True}, ),
-        ('Products.PluggableAuthService', {'loadZCML': True}, ),
-        ('Products.PluginRegistry', {'loadZCML': True}, ),
-        ('Products.PlonePAS', {'loadZCML': True}, ),
+        ("Products.GenericSetup", {"loadZCML": True}),
+        ("Products.DCWorkflow", {"loadZCML": True}),
+        ("Products.ZCTextIndex", {"loadZCML": True}),
+        ("Products.DateRecurringIndex", {"loadZCML": False}),
+        ("Products.PageTemplates", {"loadZCML": True}),
+        ("Products.CMFUid", {"loadZCML": True}),
+        ("Products.CMFCore", {"loadZCML": True}),
+        ("Products.PluggableAuthService", {"loadZCML": True}),
+        ("Products.PluginRegistry", {"loadZCML": True}),
+        ("Products.PlonePAS", {"loadZCML": True}),
         # product for Plone 5.2 only, be silent when not available on Plone 6:
-        ('Products.CMFFormController', {'loadZCML': True, 'silent': True}, ),
-        ('Products.CMFDynamicViewFTI', {'loadZCML': True}, ),
-        ('Products.CMFPlacefulWorkflow', {'loadZCML': True}, ),
-        ('Products.MimetypesRegistry', {'loadZCML': True}, ),
-        ('Products.PortalTransforms', {'loadZCML': True}, ),
-        ('Products.ExtendedPathIndex', {'loadZCML': True}, ),
-        ('Products.SiteAccess', {'loadZCML': False}, ),
-        ('Products.CMFEditions', {'loadZCML': True}, ),
-        ('Products.CMFDiffTool', {'loadZCML': True}, ),
-        ('plone.i18n', {'loadZCML': True, 'install': False}, ),
-        ('plonetheme.barceloneta', {'loadZCML': True, 'install': False}, ),
-        ('Products.CMFPlone', {'loadZCML': True}, ),
-        ('Products.PythonScripts', {'loadZCML': False}, ),
+        ("Products.CMFFormController", {"loadZCML": True, "silent": True}),
+        ("Products.CMFDynamicViewFTI", {"loadZCML": True}),
+        ("Products.CMFPlacefulWorkflow", {"loadZCML": True}),
+        ("Products.MimetypesRegistry", {"loadZCML": True}),
+        ("Products.PortalTransforms", {"loadZCML": True}),
+        ("Products.ExtendedPathIndex", {"loadZCML": True}),
+        ("Products.SiteAccess", {"loadZCML": False}),
+        ("Products.CMFEditions", {"loadZCML": True}),
+        ("Products.CMFDiffTool", {"loadZCML": True}),
+        ("plone.i18n", {"loadZCML": True, "install": False}),
+        ("plonetheme.barceloneta", {"loadZCML": True, "install": False}),
+        ("Products.CMFPlone", {"loadZCML": True}),
+        ("Products.PythonScripts", {"loadZCML": False}),
     )
-    if six.PY2:
-        products += (
-            ('Products.ExternalEditor', {'loadZCML': True}, ),
-        )
-
-        try:
-            # Since gopipindex moved to plone.folder only with Archetypes
-            import plone.app.folder
-            # Prevent trying to load plone.app.folder if it is a module alias
-            if hasattr(plone.app.folder, "__file__"):
-                products += (
-                    ('plone.app.folder', {'loadZCML': True}, ),
-                )
-        except ImportError:
-            pass
 
     # Extension profiles to be installed with site setup
-    extensionProfiles = (
-        'plonetheme.barceloneta:default',
-    )
+    extensionProfiles = ("plonetheme.barceloneta:default",)
 
     # Layer lifecycle
 
     def setUp(self):
-
         # Stack a new DemoStorage on top of the one from zope.STARTUP.
-        self['zodbDB'] = zodb.stackDemoStorage(
-            self.get('zodbDB'),
-            name='PloneFixture'
-        )
+        self["zodbDB"] = zodb.stackDemoStorage(self.get("zodbDB"), name="PloneFixture")
 
         self.setUpZCML()
 
         # Set up products and the default content
         with zope.zopeApp() as app:
             self.setUpProducts(app)
             self.setUpDefaultContent(app)
             # If there is no savepoint most tests fail with a PosKeyError
             # See https://github.com/plone/Products.CMFPlone/issues/3467
             transaction.savepoint(optimistic=True)
 
     def tearDown(self):
-
         # Tear down products
         with zope.zopeApp() as app:
             # note: content tear-down happens by squashing the ZODB
             self.tearDownProducts(app)
 
         self.tearDownZCML()
 
         # Zap the stacked ZODB
-        self['zodbDB'].close()
-        del self['zodbDB']
+        self["zodbDB"].close()
+        del self["zodbDB"]
 
     def setUpZCML(self):
         """Stack a new global registry and load ZCML configuration of Plone
         and the core set of add-on products into it. Also set the
         ``disable-autoinclude`` ZCML feature so that Plone does not attempt to
         auto-load ZCML using ``z3c.autoinclude``.
         """
 
         # Create a new global registry
         zca.pushGlobalRegistry()
 
         from zope.configuration import xmlconfig
-        self['configurationContext'] = context = zca.stackConfigurationContext(
-            self.get('configurationContext')
+
+        self["configurationContext"] = context = zca.stackConfigurationContext(
+            self.get("configurationContext")
         )
 
         # Turn off z3c.autoinclude
 
-        xmlconfig.string("""\
+        xmlconfig.string(
+            """\
 <configure xmlns="http://namespaces.zope.org/zope"
            xmlns:meta="http://namespaces.zope.org/meta">
     <meta:provides feature="disable-autoinclude" />
 </configure>
-""", context=context)
+""",
+            context=context,
+        )
 
         # Load dependent products's ZCML - Plone doesn't specify dependencies
         # on Products.* packages fully
 
         def loadAll(filename):
             for p, config in self.products:
-                if not config['loadZCML']:
+                if not config["loadZCML"]:
                     continue
                 try:
                     package = resolve(p)
                 except ImportError:
                     continue
                 try:
                     xmlconfig.file(filename, package, context=context)
-                except IOError:
+                except OSError:
                     pass
 
-        loadAll('meta.zcml')
-        loadAll('configure.zcml')
-        loadAll('overrides.zcml')
+        loadAll("meta.zcml")
+        loadAll("configure.zcml")
+        loadAll("overrides.zcml")
 
     def tearDownZCML(self):
         """Pop the global component registry stack, effectively unregistering
         all global components registered during layer setup.
         """
         # Pop the global registry
         zca.popGlobalRegistry()
 
         # Zap the stacked configuration context
-        del self['configurationContext']
+        del self["configurationContext"]
 
     def setUpProducts(self, app):
         """Install all old-style products listed in the the ``products`` tuple
         of this class.
         """
 
         for p, config in self.products:
-            if config.get('install', True):
-                if config.get('silent'):
+            if config.get("install", True):
+                if config.get("silent"):
                     # When product is not available, do not complain or warn.
                     try:
                         resolve(p)
                     except ImportError:
                         continue
                 zope.installProduct(app, p)
 
     def tearDownProducts(self, app):
         """Uninstall all old-style products listed in the the ``products``
         tuple of this class.
         """
         for p, config in reversed(self.products):
-            if config.get('install', True):
+            if config.get("install", True):
                 zope.uninstallProduct(app, p)
 
-        # Clean up Wicked turds
-        # XXX: This may tear down too much state
-        try:
-            from wicked.fieldevent import meta
-            meta.cleanUp()
-        except ImportError:
-            pass
-
     def setUpDefaultContent(self, app):
         """Add the site owner user to the root user folder and log in as that
         user. Create the Plone site, installing the extension profiles listed
         in the ``extensionProfiles`` layer class variable. Create the test
         user inside the site, and disable the default workflow.
 
         Note: There is no explicit tear-down of this setup operation, because
         all persistent changes are torn down when the stacked ZODB
         ``DemoStorage`` is popped.
         """
 
         # Create the owner user and "log in" so that the site object gets
         # the right ownership information
-        app['acl_users'].userFolderAddUser(
-            SITE_OWNER_NAME,
-            SITE_OWNER_PASSWORD,
-            ['Manager'],
-            []
+        app["acl_users"].userFolderAddUser(
+            SITE_OWNER_NAME, SITE_OWNER_PASSWORD, ["Manager"], []
         )
 
-        zope.login(app['acl_users'], SITE_OWNER_NAME)
+        zope.login(app["acl_users"], SITE_OWNER_NAME)
 
         # Create the site with the default set of extension profiles
         from Products.CMFPlone.factory import addPloneSite
+
         addPloneSite(
             app,
             PLONE_SITE_ID,
             title=PLONE_SITE_TITLE,
             setup_content=False,
             default_language=DEFAULT_LANGUAGE,
             extension_ids=self.extensionProfiles,
         )
 
         # Turn off default workflow
-        app[PLONE_SITE_ID]['portal_workflow'].setDefaultChain('')
+        app[PLONE_SITE_ID]["portal_workflow"].setDefaultChain("")
 
         # Create the test user. (Plone)PAS does not have an API to create a
         # user with different userid and login name, so we call the plugin
         # directly.
-        pas = app[PLONE_SITE_ID]['acl_users']
-        pas.source_users.addUser(
-            TEST_USER_ID,
-            TEST_USER_NAME,
-            TEST_USER_PASSWORD
-        )
+        pas = app[PLONE_SITE_ID]["acl_users"]
+        pas.source_users.addUser(TEST_USER_ID, TEST_USER_NAME, TEST_USER_PASSWORD)
         for role in TEST_USER_ROLES:
             pas.portal_role_manager.doAssignRoleToPrincipal(TEST_USER_ID, role)
 
         # Log out again
         zope.logout()
 
 
@@ -272,67 +238,64 @@
     e. g. to use the FTP server.
 
     """
 
     defaultBases = (zserver.STARTUP,)
 
     def setUp(self):
-
         # Stack a new DemoStorage on top of the one from zserver.STARTUP.
-        self['zodbDB'] = zodb.stackDemoStorage(
-            self.get('zodbDB'),
-            name='PloneZServerFixture'
+        self["zodbDB"] = zodb.stackDemoStorage(
+            self.get("zodbDB"), name="PloneZServerFixture"
         )
 
         self.setUpZCML()
 
         # Set up products and the default content
         with zserver.zopeApp() as app:
             self.setUpProducts(app)
             self.setUpDefaultContent(app)
 
     def tearDown(self):
-
         # Tear down products
         with zserver.zopeApp() as app:
             # note: content tear-down happens by squashing the ZODB
             self.tearDownProducts(app)
 
         self.tearDownZCML()
 
         # Zap the stacked ZODB
-        self['zodbDB'].close()
-        del self['zodbDB']
+        self["zodbDB"].close()
+        del self["zodbDB"]
 
 
 PLONE_ZSERVER_FIXTURE = PloneZServerFixture()
 
 
-class PloneTestLifecycle(object):
+class PloneTestLifecycle:
     """Mixin class for Plone test lifecycle. This exposes the ``portal``
     resource and resets the environment between each test.
 
     This class is used as a mixing for the IntegrationTesting and
     FunctionalTesting classes below, which also mix in the z2 versions of
     the same.
     """
 
     defaultBases = (PLONE_FIXTURE,)
 
     def testSetUp(self):
-        super(PloneTestLifecycle, self).testSetUp()
+        super().testSetUp()
 
-        self['portal'] = portal = self['app'][PLONE_SITE_ID]
+        self["portal"] = portal = self["app"][PLONE_SITE_ID]
         self.setUpEnvironment(portal)
 
     def testTearDown(self):
-        self.tearDownEnvironment(self['portal'])
-        del self['portal']
+        self.tearDownEnvironment(self["portal"])
+        del self["portal"]
 
-        super(PloneTestLifecycle, self).testTearDown()
+        super().testTearDown()
 
     def setUpEnvironment(self, portal):
         """Set up the local component site, reset skin data and log in as
         the test user.
         """
 
         # Set up the local site manager
@@ -341,33 +304,37 @@
         # Reset skin data
         portal.clearCurrentSkin()
         portal.setupCurrentSkin(portal.REQUEST)
         notify(BeforeTraverseEvent(portal, portal.REQUEST))
 
         # Pseudo-login as the test user
         from plone.app.testing import helpers
+
         helpers.login(portal, TEST_USER_NAME)
 
     def tearDownEnvironment(self, portal):
         """Log out, invalidate standard RAM caches, and unset the local
         component site to clean up after tests.
         """
 
         # Clear the security manager
         from plone.app.testing import helpers
+
         helpers.logout()
 
         # Clear any cached data using plone.memoize's RAM caches
         from plone.memoize.ram import global_cache
+
         global_cache.invalidateAll()
 
-        from zope.component import queryUtility
         from plone.memoize.ram import IRAMCache
+        from zope.component import queryUtility
+
         cache = queryUtility(IRAMCache)
-        if cache and getattr(cache, '_cacheId', None):
+        if cache and getattr(cache, "_cacheId", None):
             cache.invalidateAll()
 
         # Unset the local component site
         setSite(None)
 
 
 class PloneZServerTestLifecycle(PloneTestLifecycle):
@@ -376,38 +343,38 @@
     defaultBases = (PLONE_ZSERVER_FIXTURE,)
 
 
 class MockMailHostLayer(Layer):
     """Layer for setting up a MockMailHost to store all sent messages as
     strings into a list at portal.MailHost.messages
     """
+
     defaultBases = (PLONE_FIXTURE,)
 
     def testSetUp(self):
         with zope.zopeApp() as app:
             portal = app[PLONE_SITE_ID]
             registry = getUtility(IRegistry, context=portal)
 
             if not registry["plone.email_from_address"]:
-                portal._original_email_address = registry["plone.email_from_address"]  # noqa: E501
+                portal._original_email_address = registry["plone.email_from_address"]
                 registry["plone.email_from_address"] = "noreply@example.com"
 
             if not registry["plone.email_from_name"]:
                 portal._original_email_name = registry["plone.email_from_name"]
-                registry["plone.email_from_name"] = u"Plone site"
+                registry["plone.email_from_name"] = "Plone site"
 
             portal._original_MailHost = portal.MailHost
-            portal.MailHost = mailhost = MockMailHost('MailHost')
+            portal.MailHost = mailhost = MockMailHost("MailHost")
 
             sm = getSiteManager(context=portal)
             sm.unregisterUtility(provided=IMailHost)
             sm.registerUtility(mailhost, provided=IMailHost)
 
     def testTearDown(self):
-
         with zope.zopeApp() as app:
             portal = app[PLONE_SITE_ID]
             registry = getUtility(IRegistry, context=portal)
 
             portal.MailHost = portal._original_MailHost
 
             sm = getSiteManager(context=portal)
@@ -415,56 +382,49 @@
             sm.registerUtility(aq_base(portal.MailHost), provided=IMailHost)
 
             if hasattr(portal, "_original_email_name"):
                 registry["plone.email_from_name"] = portal._original_email_name
                 delattr(portal, "_original_email_name")
 
             if hasattr(portal, "_original_email_address"):
-                registry["plone.email_from_address"] = portal._original_email_address  # noqa: E501
+                registry["plone.email_from_address"] = portal._original_email_address
                 delattr(portal, "_original_email_address")
 
             delattr(portal, "_original_MailHost")
 
 
 MOCK_MAILHOST_FIXTURE = MockMailHostLayer()
 
 
 class IntegrationTesting(PloneTestLifecycle, zope.IntegrationTesting):
-    """Plone version of the integration testing layer
-    """
+    """Plone version of the integration testing layer"""
 
 
 class FunctionalTesting(PloneTestLifecycle, zope.FunctionalTesting):
-    """Plone version of the functional testing layer
-    """
+    """Plone version of the functional testing layer"""
 
 
-class ZServerFunctionalTesting(
-        PloneZServerTestLifecycle, zserver.FunctionalTesting):
-    """Plone version of the functional testing layer using ZServer.
-    """
+class ZServerFunctionalTesting(PloneZServerTestLifecycle, zserver.FunctionalTesting):
+    """Plone version of the functional testing layer using ZServer."""
+
 
 #
 # Layer instances
 #
 # Note: PLONE_FIXTURE is defined above
 
 
 PLONE_INTEGRATION_TESTING = IntegrationTesting(
-    bases=(PLONE_FIXTURE, ),
-    name='Plone:Integration'
+    bases=(PLONE_FIXTURE,), name="Plone:Integration"
 )
 
 PLONE_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(PLONE_FIXTURE, ),
-    name='Plone:Functional'
+    bases=(PLONE_FIXTURE,), name="Plone:Functional"
 )
 
 PLONE_WSGISERVER = PLONE_ZSERVER = FunctionalTesting(
-    bases=(PLONE_FIXTURE, zope.WSGI_SERVER_FIXTURE),
-    name='Plone:WSGIServer'
+    bases=(PLONE_FIXTURE, zope.WSGI_SERVER_FIXTURE), name="Plone:WSGIServer"
 )
 
 PLONE_FTP_SERVER = ZServerFunctionalTesting(
-    bases=(PLONE_ZSERVER_FIXTURE, zserver.FTP_SERVER_FIXTURE),
-    name='Plone:FTPServer'
+    bases=(PLONE_ZSERVER_FIXTURE, zserver.FTP_SERVER_FIXTURE), name="Plone:FTPServer"
 )
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/layers.rst` & `plone.app.testing-7.0.1/src/plone/app/testing/layers.rst`

 * *Files 1% similar despite different names*

```diff
@@ -333,15 +333,15 @@
 
 We can now look for this new object through the server.
 
     >>> portal_url = portal.absolute_url()
     >>> portal_url.split(':')[:-1]
     ['http', '//localhost']
 
-    >>> from six.moves.urllib.request import urlopen
+    >>> from urllib.request import urlopen
     >>> conn = urlopen(portal_url, timeout=10)
     >>> responseBody = conn.read()
     >>> b"Fancy Portal" in responseBody
     True
     >>> conn.close()
 
 Test tear-down does nothing beyond what the base layers do.
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/selenium.rst` & `plone.app.testing-7.0.1/src/plone/app/testing/selenium.rst`

 * *Files identical despite different names*

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/selenium_layers.py` & `plone.app.testing-7.0.1/src/plone/app/testing/selenium_layers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,77 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import TEST_USER_NAME
 from plone.app.testing import TEST_USER_PASSWORD
 from plone.testing import Layer
 from plone.testing import zope
 
 import os
 import transaction
 
 
 class SeleniumLayer(Layer):
-    defaultBases = (zope.ZSERVER_FIXTURE, )
+    defaultBases = (zope.ZSERVER_FIXTURE,)
 
     def testSetUp(self):
         # Start up Selenium
-        driver = os.environ.get('SELENIUM_DRIVER', '').lower() or 'firefox'
+        driver = os.environ.get("SELENIUM_DRIVER", "").lower() or "firefox"
         webdriver = __import__(
-            'selenium.webdriver.{0}.webdriver'.format(driver),
-            fromlist=['WebDriver']
+            f"selenium.webdriver.{driver}.webdriver", fromlist=["WebDriver"]
         )
-        args = [arg.strip() for arg in
-                os.environ.get('SELENIUM_ARGS', '').split()
-                if arg.strip()]
-        self['selenium'] = webdriver.WebDriver(*args)
+        args = [
+            arg.strip()
+            for arg in os.environ.get("SELENIUM_ARGS", "").split()
+            if arg.strip()
+        ]
+        self["selenium"] = webdriver.WebDriver(*args)
 
     def testTearDown(self):
-        self['selenium'].quit()
-        del self['selenium']
+        self["selenium"].quit()
+        del self["selenium"]
 
 
 SELENIUM_FIXTURE = SeleniumLayer()
 SELENIUM_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(SELENIUM_FIXTURE, ),
-    name='SeleniumTesting:Functional')
+    bases=(SELENIUM_FIXTURE,), name="SeleniumTesting:Functional"
+)
 SELENIUM_PLONE_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(SELENIUM_FIXTURE, PLONE_FIXTURE),
-    name='SeleniumTesting:Functional')
+    bases=(SELENIUM_FIXTURE, PLONE_FIXTURE), name="SeleniumTesting:Functional"
+)
 
 
 # Helper functions
 
 
 def open(selenium, url):
     # ensure we have a clean starting point
     transaction.commit()
     selenium.get(url)
 
 
 def login(selenium, portal, username=False, password=False):
-
     if not username:
         username = TEST_USER_NAME
     if not password:
         password = TEST_USER_PASSWORD
 
-    open(selenium, portal.absolute_url() + '/login_form')
-    selenium.find_element_by_name('__ac_name').send_keys(username)
-    selenium.find_element_by_name('__ac_password').send_keys(password)
-    selenium.find_element_by_name('submit').click()
+    open(selenium, portal.absolute_url() + "/login_form")
+    selenium.find_element_by_name("__ac_name").send_keys(username)
+    selenium.find_element_by_name("__ac_password").send_keys(password)
+    selenium.find_element_by_name("submit").click()
 
 
 def click(selenium, xpath):
-    if xpath.count('link='):
-        link = xpath.split('link=')[-1]
+    if xpath.count("link="):
+        link = xpath.split("link=")[-1]
         element = selenium.find_element_by_partial_link_text(link)
-    elif xpath.count('//'):
+    elif xpath.count("//"):
         element = selenium.find_element_by_xpath(xpath)
-    elif xpath.count('#'):
-        eleName = xpath.split('#')[-1]
+    elif xpath.count("#"):
+        eleName = xpath.split("#")[-1]
         element = selenium.find_element_by_id(eleName)
     else:
         element = selenium.find_element_by_name(xpath)
 
     element.click()
 
 
@@ -89,37 +88,37 @@
     The workaround is to use this handle trick,
     which is currently unsupported in chrome.
     See issue #405 for more.
     In general there are still a lot of open issues on frame support so if
     this breaks it won't be a surprise.
     """
     handle = selenium.current_window_handle
-    selenium.switch_to_frame('form.text_ifr')
-    ele = selenium.find_element_by_xpath('//p')
+    selenium.switch_to_frame("form.text_ifr")
+    ele = selenium.find_element_by_xpath("//p")
     ele.send_keys(value)
     selenium.switch_to_window(handle)
 
 
 def clear(selenium, name):
     selenium.find_element_by_name(name).clear()
 
 
-def select(selenium, xpath1, xpath2=''):
+def select(selenium, xpath1, xpath2=""):
     xpath = xpath1
     if xpath2:
-        xpath = "{0}['{1}']".format(xpath1, xpath2)
+        xpath = f"{xpath1}['{xpath2}']"
         xpath = xpath.replace("select['label=", "select/option['text()=")
     selenium.find_element_by_xpath(xpath).click()
 
 
 def waitForPageToLoad(selenium, foo):
     # this does nothing but make us lazy folks happy
     pass
 
 
 def publish(selenium):
     click(selenium, "//dl[@id='plone-contentmenu-workflow']/dt/a")
-    click(selenium, '#workflow-transition-publish')
+    click(selenium, "#workflow-transition-publish")
 
 
 def submit(selenium, formId):
     selenium.find_element_by_id(formId).submit()
```

### Comparing `plone.app.testing-7.0.0b2/src/plone/app/testing/utils.py` & `plone.app.testing-7.0.1/src/plone/app/testing/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-# -*- coding: utf-8 -*-
 from persistent.list import PersistentList
 from Products.MailHost.MailHost import _mungeHeaders
 from Products.MailHost.MailHost import MailBase
 
 
 class MockMailHost(MailBase):
-    """A MailHost that collects messages instead of sending them.
-    """
+    """A MailHost that collects messages instead of sending them."""
 
     def __init__(self, id):
         self.reset()
 
     def reset(self):
         self.messages = PersistentList()
 
     def _send(self, mfrom, mto, messageText, immediate=False):
-        """ Send the message """
+        """Send the message"""
         self.messages.append(messageText)
 
-    def send(self, messageText, mto=None, mfrom=None, subject=None,
-             encode=None, immediate=False, charset=None, msg_type=None):
-        messageText, mto, mfrom = _mungeHeaders(messageText,
-                                                mto, mfrom, subject,
-                                                charset=charset,
-                                                msg_type=msg_type)
+    def send(
+        self,
+        messageText,
+        mto=None,
+        mfrom=None,
+        subject=None,
+        encode=None,
+        immediate=False,
+        charset=None,
+        msg_type=None,
+    ):
+        messageText, mto, mfrom = _mungeHeaders(
+            messageText, mto, mfrom, subject, charset=charset, msg_type=msg_type
+        )
         self.messages.append(messageText)
```

### Comparing `plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/PKG-INFO` & `plone.app.testing-7.0.1/src/plone.app.testing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: plone.app.testing
-Version: 7.0.0b2
+Version: 7.0.1
 Summary: Testing tools for Plone-the-application, based on plone.testing.
 Home-page: https://pypi.org/project/plone.app.testing
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone tests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 4
+Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: robot
 
 Introduction
 ============
 
 .. contents:: Table of contents
@@ -1588,14 +1591,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+7.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (434550cc)
+
+
+7.0.0 (2022-12-02)
+------------------
+
+Bug fixes:
+
+
+- Final release for Plone 6.0.0. (#600)
+
+
 7.0.0b2 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Restore the previously used admin password for tests ("secret") [davisagli] (#79)
@@ -1769,15 +1791,15 @@
   For Plone 5.2 the bbb.PloneTestCase will uses Dexterity instead of Archetypes.
   Adding bbb_at.PloneTestCase for them to use allows to keep the AT tests working.
   See https://github.com/plone/plone.app.testing/pull/51
   [pbauer]
 
 Bug fixes:
 
-- Amended the doctests to work with automatical layer port picking from plone.testing.
+- Amended the doctests to work with automatically layer port picking from plone.testing.
   [Rotonen]
 
 
 5.0.8 (2017-10-25)
 ------------------
 
 Bug fixes:
@@ -1923,15 +1945,15 @@
   [davisagli]
 
 - fix: ``Products.CMFPlone`` needs the ``gopip`` index from
   ``plone.app.folder``. So latter has to be initialized before CMFPlones
   profile is applied (which installs the index to catalog). At the moment
   CMFPlone therefore registers the index itself, but plone.app.folder
   registers it too, which resulted in plone/Products.CMFPlone#313
-  "GopipIndex registered twice" In tests the registration does not succedd,
+  "GopipIndex registered twice" In tests the registration does not succeed,
   because plone.app.folder was never initialized as z2 products. In order to
   remove the misleading regisatration from CMFPlone we must take care that the
   index is available, which is achieved with this change. Also minor pep8
   optimizations in the file touched.
   [jensens]
 
 - create memberfolder, if it is not there for testing.
```

### Comparing `plone.app.testing-7.0.0b2/src/plone.app.testing.egg-info/SOURCES.txt` & `plone.app.testing-7.0.1/src/plone.app.testing.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,19 @@
 src/plone.app.testing.egg-info/namespace_packages.txt
 src/plone.app.testing.egg-info/not-zip-safe
 src/plone.app.testing.egg-info/requires.txt
 src/plone.app.testing.egg-info/top_level.txt
 src/plone/app/__init__.py
 src/plone/app/testing/__init__.py
 src/plone/app/testing/bbb.py
-src/plone/app/testing/bbb_at.py
 src/plone/app/testing/cleanup.py
 src/plone/app/testing/cleanup.rst
 src/plone/app/testing/helpers.py
 src/plone/app/testing/helpers.rst
 src/plone/app/testing/interfaces.py
 src/plone/app/testing/layers.py
 src/plone/app/testing/layers.rst
-src/plone/app/testing/layers_zserver.rst
 src/plone/app/testing/selenium.rst
 src/plone/app/testing/selenium_layers.py
 src/plone/app/testing/tests.py
 src/plone/app/testing/utils.py
 src/plone/app/testing/profile/metadata.xml
```

