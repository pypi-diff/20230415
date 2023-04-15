# Comparing `tmp/plone.base-1.1.0.tar.gz` & `tmp/plone.base-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.base-1.1.0.tar", last modified: Mon Mar 13 17:07:22 2023, max compression
+gzip compressed data, was "plone.base-1.1.1.tar", last modified: Sat Apr 15 09:08:27 2023, max compression
```

## Comparing `plone.base-1.1.0.tar` & `plone.base-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:22.564992 plone.base-1.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)     3854 2023-03-13 17:07:21.000000 plone.base-1.1.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      105 2023-03-13 17:07:21.000000 plone.base-1.1.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     6837 2023-03-13 17:07:22.565116 plone.base-1.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2026 2023-03-13 17:07:21.000000 plone.base-1.1.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      948 2023-03-13 17:07:21.000000 plone.base-1.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1804 2023-03-13 17:07:22.566043 plone.base-1.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       39 2023-03-13 17:07:21.000000 plone.base-1.1.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:22.544973 plone.base-1.1.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:22.548106 plone.base-1.1.0/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:22.554392 plone.base-1.1.0/src/plone/base/
--rw-r--r--   0 maurits    (501) staff       (20)      238 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2894 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/batch.py
--rw-r--r--   0 maurits    (501) staff       (20)     5502 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)    12074 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/i18nl10n.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:22.562716 plone.base-1.1.0/src/plone/base/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)     2622 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      305 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/atd.py
--rw-r--r--   0 maurits    (501) staff       (20)      289 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/basetool.py
--rw-r--r--   0 maurits    (501) staff       (20)      151 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/breadcrumbs.py
--rw-r--r--   0 maurits    (501) staff       (20)     3060 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)    63997 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      403 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)      652 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/events.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/images.py
--rw-r--r--   0 maurits    (501) staff       (20)      529 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/installable.py
--rw-r--r--   0 maurits    (501) staff       (20)      697 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/language.py
--rw-r--r--   0 maurits    (501) staff       (20)     1993 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/login.py
--rw-r--r--   0 maurits    (501) staff       (20)      853 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/migration.py
--rw-r--r--   0 maurits    (501) staff       (20)     1471 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/password_reset.py
--rw-r--r--   0 maurits    (501) staff       (20)      243 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)      496 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/properties.py
--rw-r--r--   0 maurits    (501) staff       (20)     4824 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/resources.py
--rw-r--r--   0 maurits    (501) staff       (20)      585 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/siteroot.py
--rw-r--r--   0 maurits    (501) staff       (20)      453 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/structure.py
--rw-r--r--   0 maurits    (501) staff       (20)     6328 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/syndication.py
--rw-r--r--   0 maurits    (501) staff       (20)     1499 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/translationservice.py
--rw-r--r--   0 maurits    (501) staff       (20)      159 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/interfaces/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2196 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/navigationroot.py
--rw-r--r--   0 maurits    (501) staff       (20)     2267 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:22.564624 plone.base-1.1.0/src/plone/base/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3507 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/tests/messages.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1387 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/tests/test_batch.py
--rw-r--r--   0 maurits    (501) staff       (20)      226 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)    17956 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/tests/test_i18nl10n.py
--rw-r--r--   0 maurits    (501) staff       (20)     6869 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    20178 2023-03-13 17:07:21.000000 plone.base-1.1.0/src/plone/base/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-13 17:07:22.551107 plone.base-1.1.0/src/plone.base.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     6837 2023-03-13 17:07:22.000000 plone.base-1.1.0/src/plone.base.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1673 2023-03-13 17:07:22.000000 plone.base-1.1.0/src/plone.base.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-13 17:07:22.000000 plone.base-1.1.0/src/plone.base.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-13 17:07:22.000000 plone.base-1.1.0/src/plone.base.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-13 17:07:22.000000 plone.base-1.1.0/src/plone.base.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      334 2023-03-13 17:07:22.000000 plone.base-1.1.0/src/plone.base.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-13 17:07:22.000000 plone.base-1.1.0/src/plone.base.egg-info/top_level.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.479372 plone.base-1.1.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3963 2023-04-15 09:08:26.000000 plone.base-1.1.1/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      105 2023-04-15 09:08:26.000000 plone.base-1.1.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     6946 2023-04-15 09:08:27.479372 plone.base-1.1.1/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2026 2023-04-15 09:08:26.000000 plone.base-1.1.1/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     2834 2023-04-15 09:08:26.000000 plone.base-1.1.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1623 2023-04-15 09:08:27.479372 plone.base-1.1.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)       39 2023-04-15 09:08:26.000000 plone.base-1.1.1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.474372 plone.base-1.1.1/src/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.474372 plone.base-1.1.1/src/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.476372 plone.base-1.1.1/src/plone/base/
+-rw-r--r--   0 gil       (1000) gil       (1000)      238 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2894 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/batch.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5502 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/defaultpage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    12074 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/i18nl10n.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.478372 plone.base-1.1.1/src/plone/base/interfaces/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2622 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      305 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/atd.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      289 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/basetool.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      151 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/breadcrumbs.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3060 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/constrains.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    63997 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/controlpanel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      403 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/defaultpage.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      652 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/events.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      776 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/images.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      529 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/installable.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      697 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/interface.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      229 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/language.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1993 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/login.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      853 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/migration.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1471 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/password_reset.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      243 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/patterns.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      496 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/properties.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4824 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/resources.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      585 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/siteroot.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      453 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/structure.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6328 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/syndication.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1499 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/translationservice.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      159 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/interfaces/workflow.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2196 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/navigationroot.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2267 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/permissions.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.479372 plone.base-1.1.1/src/plone/base/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3507 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/messages.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1387 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_batch.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      226 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_doctests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    17956 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_i18nl10n.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6869 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/tests/test_utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    20178 2023-04-15 09:08:26.000000 plone.base-1.1.1/src/plone/base/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:08:27.475372 plone.base-1.1.1/src/plone.base.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     6946 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1673 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      152 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 09:08:27.000000 plone.base-1.1.1/src/plone.base.egg-info/top_level.txt
```

### Comparing `plone.base-1.1.0/CHANGES.rst` & `plone.base-1.1.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 1.1.0 (2023-03-13)
 ------------------
 
 New features:
 
 
 - Move `plone.app.layout.navigation.root.getNavigationRoot` to `.navigationroot.get_navigation_root`.
```

### Comparing `plone.base-1.1.0/PKG-INFO` & `plone.base-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.1.0
+Version: 1.1.1
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -81,14 +81,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 1.1.0 (2023-03-13)
 ------------------
 
 New features:
 
 
 - Move `plone.app.layout.navigation.root.getNavigationRoot` to `.navigationroot.get_navigation_root`.
```

### Comparing `plone.base-1.1.0/README.rst` & `plone.base-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/setup.cfg` & `plone.base-1.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.1.0
+version = 1.1.1
 name = plone.base
 description = Plone Interface contracts, plus basic features and utilities
 long_description = file: README.rst, CHANGES.rst
 keywords = plone
 author = Jens W. Klein
 author_email = jk@kleinundpartner.at
 maintainer = Plone Release Team
@@ -25,73 +25,54 @@
 	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	setuptools
-	AccessControl
-	Acquisition
-	ZODB
-	Zope>=5
 	plone.batching
 	plone.registry
 	plone.schema
 	plone.z3cform
-	Products.BTreeFolder2
 	Products.CMFCore
 	Products.CMFDynamicViewFTI
-	transaction
-	zExceptions
-	zope.component
-	zope.deprecation
-	zope.i18n
-	zope.i18nmessageid
-	zope.interface
-	zope.publisher
-	zope.schema
 namespace_packages = 
 	plone
 package_dir = 
 	= src
 packages = find:
 zip_safe = False
 
 [options.extras_require]
 test = 
 	plone.subrequest
-	zope.tal
+	plone.portlets  # transitive undeclared by plone.protect (over plone.subrequest)
 
 [options.packages.find]
 where = 
 	src
 
 [bdist_wheel]
 universal = 0
 
-[check-manifest]
-ignore = 
-	*.cfg
-	*.json
-	*.yml
-	.coveragerc
-	.editorconfig
-	.gitattributes
-	.meta.toml
-	.pre-commit-config.yaml
-	tox.ini
-
 [flake8]
 doctests = 1
 ignore = 
 	E501,
 	W503,
 	E203,
 	E231,
 per-file-ignores = 
 	src/plone/base/interfaces/__init__.py:F401
 	src/plone/base/permissions.py:F401,E402
 
+[check-manifest]
+ignore = 
+	.editorconfig
+	.meta.toml
+	.pre-commit-config.yaml
+	tox.ini
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `plone.base-1.1.0/src/plone/base/batch.py` & `plone.base-1.1.1/src/plone/base/batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/defaultpage.py` & `plone.base-1.1.1/src/plone/base/defaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/i18nl10n.py` & `plone.base-1.1.1/src/plone/base/i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/__init__.py` & `plone.base-1.1.1/src/plone/base/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/constrains.py` & `plone.base-1.1.1/src/plone/base/interfaces/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/controlpanel.py` & `plone.base-1.1.1/src/plone/base/interfaces/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/events.py` & `plone.base-1.1.1/src/plone/base/interfaces/events.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/images.py` & `plone.base-1.1.1/src/plone/base/interfaces/images.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/installable.py` & `plone.base-1.1.1/src/plone/base/interfaces/installable.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/interface.py` & `plone.base-1.1.1/src/plone/base/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/login.py` & `plone.base-1.1.1/src/plone/base/interfaces/login.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/migration.py` & `plone.base-1.1.1/src/plone/base/interfaces/migration.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/password_reset.py` & `plone.base-1.1.1/src/plone/base/interfaces/password_reset.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/resources.py` & `plone.base-1.1.1/src/plone/base/interfaces/resources.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/siteroot.py` & `plone.base-1.1.1/src/plone/base/interfaces/siteroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/syndication.py` & `plone.base-1.1.1/src/plone/base/interfaces/syndication.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/interfaces/translationservice.py` & `plone.base-1.1.1/src/plone/base/interfaces/translationservice.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/navigationroot.py` & `plone.base-1.1.1/src/plone/base/navigationroot.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/permissions.py` & `plone.base-1.1.1/src/plone/base/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/tests/messages.rst` & `plone.base-1.1.1/src/plone/base/tests/messages.rst`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/tests/test_batch.py` & `plone.base-1.1.1/src/plone/base/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/tests/test_i18nl10n.py` & `plone.base-1.1.1/src/plone/base/tests/test_i18nl10n.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/tests/test_utils.py` & `plone.base-1.1.1/src/plone/base/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone/base/utils.py` & `plone.base-1.1.1/src/plone/base/utils.py`

 * *Files identical despite different names*

### Comparing `plone.base-1.1.0/src/plone.base.egg-info/PKG-INFO` & `plone.base-1.1.1/src/plone.base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.base
-Version: 1.1.0
+Version: 1.1.1
 Summary: Plone Interface contracts, plus basic features and utilities
 Home-page: https://github.com/plone/plone.base
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -81,14 +81,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+1.1.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 1.1.0 (2023-03-13)
 ------------------
 
 New features:
 
 
 - Move `plone.app.layout.navigation.root.getNavigationRoot` to `.navigationroot.get_navigation_root`.
```

### Comparing `plone.base-1.1.0/src/plone.base.egg-info/SOURCES.txt` & `plone.base-1.1.1/src/plone.base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

