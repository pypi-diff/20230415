# Comparing `tmp/salix-containers-0.2.1.tar.gz` & `tmp/salix-containers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salix-containers-0.2.1.tar", max compression
+gzip compressed data, was "salix-containers-0.3.0.tar", max compression
```

## Comparing `salix-containers-0.2.1.tar` & `salix-containers-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0      331 2022-04-18 10:58:42.281417 salix-containers-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       84 2022-04-18 10:50:50.871417 salix-containers-0.2.1/salix_containers/__init__.py
--rw-r--r--   0        0        0     1617 2022-04-16 20:28:31.676860 salix-containers-0.2.1/salix_containers/casttypes.py
--rw-r--r--   0        0        0      535 2022-04-18 10:59:24.215276 salix-containers-0.2.1/setup.py
--rw-r--r--   0        0        0      489 2022-04-18 10:59:24.215474 salix-containers-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      331 2023-04-15 16:50:32.069609 salix-containers-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/__init__.py
+-rw-r--r--   0        0        0      763 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/caselessmapping.py
+-rw-r--r--   0        0        0     1617 2022-04-16 20:28:31.676860 salix-containers-0.3.0/salix_containers/casttypes.py
+-rw-r--r--   0        0        0        0 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/tests/__init__.py
+-rw-r--r--   0        0        0     1450 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/tests/test_caselessdict.py
+-rw-r--r--   0        0        0      561 2023-04-15 16:51:54.696066 salix-containers-0.3.0/setup.py
+-rw-r--r--   0        0        0      489 2023-04-15 16:51:54.696210 salix-containers-0.3.0/PKG-INFO
```

### Comparing `salix-containers-0.2.1/salix_containers/casttypes.py` & `salix-containers-0.3.0/salix_containers/casttypes.py`

 * *Files identical despite different names*

### Comparing `salix-containers-0.2.1/setup.py` & `salix-containers-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['salix_containers']
+['salix_containers', 'salix_containers.tests']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'salix-containers',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Occasionally handy container types',
     'long_description': None,
     'author': 'Salix',
     'author_email': 'salix@pilae.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

