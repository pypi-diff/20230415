# Comparing `tmp/Products.CMFDynamicViewFTI-7.0.0a1.tar.gz` & `tmp/Products.CMFDynamicViewFTI-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.CMFDynamicViewFTI-7.0.0a1.tar", last modified: Wed Jan 19 14:14:46 2022, max compression
+gzip compressed data, was "Products.CMFDynamicViewFTI-7.0.1.tar", last modified: Sat Apr 15 09:00:34 2023, max compression
```

## Comparing `Products.CMFDynamicViewFTI-7.0.0a1.tar` & `Products.CMFDynamicViewFTI-7.0.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.136972 Products.CMFDynamicViewFTI-7.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)       84 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)     8026 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      171 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     9958 2022-01-19 14:14:46.137115 Products.CMFDynamicViewFTI-7.0.0a1/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.126978 Products.CMFDynamicViewFTI-7.0.0a1/Products/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.131620 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/
--rw-r--r--   0 maurits    (501) staff       (20)      985 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.133139 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/browser/
--rw-r--r--   0 maurits    (501) staff       (20)       34 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1324 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/browser/addWithPresettings.pt
--rw-r--r--   0 maurits    (501) staff       (20)      450 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/browser/typeinfo.py
--rw-r--r--   0 maurits    (501) staff       (20)    10171 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/browserdefault.py
--rw-r--r--   0 maurits    (501) staff       (20)     1144 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      776 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/content_for_tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     8101 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/fti.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.133409 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/images/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/images/typeinfo.gif
--rw-r--r--   0 maurits    (501) staff       (20)      284 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     4058 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      152 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.123298 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.133694 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/sample_types/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.134240 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/sample_types/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1175 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynDocument.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1058 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynFolder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      270 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/sample_types/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.136123 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     1929 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/CMFDVFTITestCase.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      341 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/browserdefault.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2236 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/test_browserdefault.py
--rw-r--r--   0 maurits    (501) staff       (20)     9676 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/test_fti.py
--rw-r--r--   0 maurits    (501) staff       (20)      244 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.129409 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     9958 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1514 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      200 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1108 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6155 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/bootstrap.py
--rw-r--r--   0 maurits    (501) staff       (20)      327 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-01-19 14:14:46.136730 Products.CMFDynamicViewFTI-7.0.0a1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      533 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/docs/AUTHORS.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2179 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2022-01-19 14:14:46.137571 Products.CMFDynamicViewFTI-7.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1616 2022-01-19 14:14:45.000000 Products.CMFDynamicViewFTI-7.0.0a1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.141006 Products.CMFDynamicViewFTI-7.0.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1019 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/.editorconfig
+-rw-r--r--   0 gil       (1000) gil       (1000)       84 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/.gitignore
+-rw-r--r--   0 gil       (1000) gil       (1000)      128 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/.meta.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      973 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 gil       (1000) gil       (1000)     8229 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      171 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    10214 2023-04-15 09:00:34.141006 Products.CMFDynamicViewFTI-7.0.1/PKG-INFO
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.139006 Products.CMFDynamicViewFTI-7.0.1/Products/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.140006 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/
+-rw-r--r--   0 gil       (1000) gil       (1000)      913 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.140006 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)       34 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/browser/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2054 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/browser/addWithPresettings.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      450 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/browser/typeinfo.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    10091 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/browserdefault.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1195 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      765 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/content_for_tests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8005 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/fti.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.140006 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/images/
+-rw-r--r--   0 gil       (1000) gil       (1000)      145 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/images/typeinfo.gif
+-rw-r--r--   0 gil       (1000) gil       (1000)     4031 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      153 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/permissions.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.137006 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.140006 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/sample_types/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.141006 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/sample_types/types/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1299 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynDocument.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1186 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynFolder.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      324 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/sample_types/types.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.141006 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3051 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/CMFDVFTITestCase.py
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      362 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/browserdefault.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2182 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/test_browserdefault.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9350 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/test_fti.py
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/Products/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.139006 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    10214 2023-04-15 09:00:34.000000 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1518 2023-04-15 09:00:34.000000 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:00:34.000000 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        9 2023-04-15 09:00:34.000000 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:00:34.000000 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      173 2023-04-15 09:00:34.000000 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        9 2023-04-15 09:00:34.000000 Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1108 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      327 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/buildout.cfg
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:00:34.141006 Products.CMFDynamicViewFTI-7.0.1/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)      533 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/docs/AUTHORS.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2179 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1643 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 09:00:34.142006 Products.CMFDynamicViewFTI-7.0.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1665 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1733 2023-04-15 09:00:33.000000 Products.CMFDynamicViewFTI-7.0.1/tox.ini
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/CHANGES.rst` & `Products.CMFDynamicViewFTI-7.0.1/CHANGES.rst`

 * *Files 3% similar despite different names*

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
+  [plone devs] (3333c742)
+
+
+7.0.0 (2022-12-01)
+------------------
+
+Bug fixes:
+
+
+- Final release for Plone 6.0.0. (#600)
+
+
 7.0.0a1 (2022-01-19)
 --------------------
 
 Breaking changes:
 
 
 - Plone 6: always use lines for the view_methods property.
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/PKG-INFO` & `Products.CMFDynamicViewFTI-7.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: Products.CMFDynamicViewFTI
-Version: 7.0.0a1
+Version: 7.0.1
 Summary: CMFDynamicViewFTI is a product for dynamic views in CMF.
 Home-page: https://pypi.org/project/Products.CMFDynamicViewFTI
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: ZPL
 Keywords: Zope CMF Plone dynamic view
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Overview
 ========
 
 CMFDynamicViewFTI is a product for dynamic views in CMF.
 The product contains an additional base class for types and a new factory type information (FTI).
@@ -55,14 +56,33 @@
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
+  [plone devs] (3333c742)
+
+
+7.0.0 (2022-12-01)
+------------------
+
+Bug fixes:
+
+
+- Final release for Plone 6.0.0. (#600)
+
+
 7.0.0a1 (2022-01-19)
 --------------------
 
 Breaking changes:
 
 
 - Plone 6: always use lines for the view_methods property.
@@ -421,9 +441,7 @@
 - Stop Acquisition for default_page.
   [panjunyong]
 
 1.0.0 - 2005-07-29
 ------------------
 
 - Initial release.
-
-
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/__init__.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,30 +3,22 @@
 from Products.CMFCore.permissions import AddPortalFolders
 from Products.CMFDynamicViewFTI import content_for_tests
 from Products.CMFDynamicViewFTI.fti import DynamicViewTypeInformation
 
 
 def initialize(context):
     # (DynamicViewTypeInformation factory is created from ZCML)
-    cmf_utils.registerIcon(
-        DynamicViewTypeInformation,
-        'images/typeinfo.gif',
-        globals()
-    )
+    cmf_utils.registerIcon(DynamicViewTypeInformation, "images/typeinfo.gif", globals())
 
     context.registerClass(
         content_for_tests.DynFolder,
         permission=AddPortalFolders,
-        constructors=(
-            ('addDynFolder', content_for_tests.addDynFolder),
-        ),
-        icon='images/typeinfo.gif'
+        constructors=(("addDynFolder", content_for_tests.addDynFolder),),
+        icon="images/typeinfo.gif",
     )
 
     context.registerClass(
         content_for_tests.DynDocument,
         permission=AddPortalContent,
-        constructors=(
-            ('addDynDocument', content_for_tests.addDynDocument),
-        ),
-        icon='images/typeinfo.gif'
+        constructors=(("addDynDocument", content_for_tests.addDynDocument),),
+        icon="images/typeinfo.gif",
     )
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/browser/addWithPresettings.pt` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/browser/addWithPresettings.pt`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,79 @@
 <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN" "http://www.w3.org/TR/REC-html40/loose.dtd">
 <html>
-<head>
-<meta http-equiv="content-type" content="text/html;charset=utf-8" />
+  <head>
+    <meta http-equiv="content-type"
+          content="text/html;charset=utf-8"
+    />
 
-</head>
-<body>
+  </head>
+  <body>
 
-<h1 tal:content="view/title">FORM TITLE</h1>
+    <h1 tal:content="view/title">FORM TITLE</h1>
 
-<p class="form-help" tal:content="view/description">DESCRIPTION TEXT.</p>
+    <p class="form-help"
+       tal:content="view/description"
+    >DESCRIPTION TEXT.</p>
 
-<form action="." method="post"
-   tal:attributes="action request/ACTUAL_URL">
-<table cellspacing="0" cellpadding="2" border="0">
- <tr>
-  <td>
-   <div class="form-label">ID</div>
-  </td>
-  <td>
-   <input type="text" name="add_input_name" size="40" />
-  </td>
- </tr>
- <tr tal:condition="view/getProfileInfos">
-  <td>
-   <div class="form-label">Presettings</div>
-  </td>
-  <td>
-   <select name="settings_id">
-    <option value="" selected="selected">(None)</option>
-    <optgroup label="PROFILE_TITLE"
-       tal:repeat="profile view/getProfileInfos"
-       tal:attributes="label profile/title">
-     <option value="SETTINGS_ID"
-             tal:repeat="obj_id profile/obj_ids"
-             tal:attributes="value string:${profile/id}/${obj_id}"
-             tal:content="obj_id">OBJ ID</option></optgroup>
-   </select>
-  </td>
- </tr>
- <tr>
-  <td>
+    <form action="."
+          method="post"
+          tal:attributes="
+            action request/ACTUAL_URL;
+          "
+    >
+      <table border="0"
+             cellpadding="2"
+             cellspacing="0"
+      >
+        <tr>
+          <td>
+            <div class="form-label">ID</div>
+          </td>
+          <td>
+            <input name="add_input_name"
+                   size="40"
+                   type="text"
+            />
+          </td>
+        </tr>
+        <tr tal:condition="view/getProfileInfos">
+          <td>
+            <div class="form-label">Presettings</div>
+          </td>
+          <td>
+            <select name="settings_id">
+              <option selected="selected"
+                      value=""
+              >(None)</option>
+              <optgroup label="PROFILE_TITLE"
+                        tal:repeat="profile view/getProfileInfos"
+                        tal:attributes="
+                          label profile/title;
+                        "
+              >
+                <option value="SETTINGS_ID"
+                        tal:repeat="obj_id profile/obj_ids"
+                        tal:content="obj_id"
+                        tal:attributes="
+                          value string:${profile/id}/${obj_id};
+                        "
+                >OBJ ID</option></optgroup>
+            </select>
+          </td>
+        </tr>
+        <tr>
+          <td>
    &nbsp;
-  </td>
-  <td>
-   <input class="form-element" type="submit" name="submit_add" value="Add" />
-  </td>
- </tr>
-</table>
-</form>
+          </td>
+          <td>
+            <input class="form-element"
+                   name="submit_add"
+                   type="submit"
+                   value="Add"
+            />
+          </td>
+        </tr>
+      </table>
+    </form>
 
-</body>
+  </body>
 </html>
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/browserdefault.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/browserdefault.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 This module contains a mixin-class to support selecting default layout
 templates and/or default pages (in the style of default_page/index_html).
 The implementation extends TemplateMixin from Archetypes, and implements
 the ISelectableBrowserDefault interface from CMFPlone.
 """
 from AccessControl import ClassSecurityInfo
-from Acquisition import aq_base
 from AccessControl.class_init import InitializeClass
+from Acquisition import aq_base
 from ExtensionClass import Base
 from Products.CMFCore.permissions import View
 from Products.CMFCore.utils import getToolByName
 from Products.CMFDynamicViewFTI.fti import DynamicViewTypeInformation
 from Products.CMFDynamicViewFTI.interfaces import ISelectableBrowserDefault
 from Products.CMFDynamicViewFTI.permissions import ModifyViewTemplate
 from zope.browsermenu.interfaces import IBrowserMenu
@@ -35,21 +35,21 @@
     object's id as a default_page (acting in the same way as index_html)
 
     Note: folderish content types should overwrite HEAD like ATContentTypes
     """
 
     _at_fti_meta_type = fti_meta_type
     aliases = {
-        '(Default)': '(dynamic view)',
-        'view': '(selected layout)',
-        'edit': 'base_edit',
-        'properties': 'base_metadata',
-        'sharing': 'folder_localrole_form',
-        'gethtml': '',
-        'mkdir': '',
+        "(Default)": "(dynamic view)",
+        "view": "(selected layout)",
+        "edit": "base_edit",
+        "properties": "base_metadata",
+        "sharing": "folder_localrole_form",
+        "gethtml": "",
+        "mkdir": "",
     }
 
     default_view = "base_view"
     suppl_views = ()
 
     security = ClassSecurityInfo()
 
@@ -88,15 +88,15 @@
     def getDefaultPage(self):
         # Return the id of the default page, or None if none is set.
         # The default page must be contained within this (folderish) item.
         fti = self.getTypeInfo()
         if fti is None:
             return None
 
-        plone_utils = getToolByName(self, 'plone_utils', None)
+        plone_utils = getToolByName(self, "plone_utils", None)
         if plone_utils is not None:
             return plone_utils.getDefaultPage(self)
 
         return fti.getDefaultPage(self, check_exists=True)
 
     @security.protected(View)
     def getLayout(self, **kw):
@@ -109,15 +109,15 @@
 
     @security.public
     def canSetDefaultPage(self):
         # Check if the user has permission to select a default page on this
         # (folderish) item, and the item is folderish.
         if not self.isPrincipiaFolderish:
             return False
-        mtool = getToolByName(self, 'portal_membership')
+        mtool = getToolByName(self, "portal_membership")
         member = mtool.getAuthenticatedMember()
         return member.has_permission(ModifyViewTemplate, self)
 
     @security.protected(ModifyViewTemplate)
     def setDefaultPage(self, objectId):
         # Set the default page to display in this (folderish) object.
 
@@ -126,83 +126,82 @@
         # default_page/index_html object of this (folderish) object. This will
         # override the current layout template returned by getLayout().
         # Pass None for objectId to turn off the default page and return to
         # using the selected layout template.
         new_page = old_page = None
         if objectId is not None:
             new_page = getattr(self, objectId, None)
-        if self.hasProperty('default_page'):
-            pages = self.getProperty('default_page', '')
+        if self.hasProperty("default_page"):
+            pages = self.getProperty("default_page", "")
             if isinstance(pages, (list, tuple)):
                 for page in pages:
                     old_page = getattr(self, page, None)
                     if page is not None:
                         break
             elif isinstance(pages, str):
                 old_page = getattr(self, pages, None)
 
             if objectId is None:
-                self.manage_delProperties(['default_page'])
+                self.manage_delProperties(["default_page"])
             else:
                 self.manage_changeProperties(default_page=objectId)
         else:
             if objectId is not None:
-                self.manage_addProperty('default_page', objectId, 'string')
+                self.manage_addProperty("default_page", objectId, "string")
         if new_page != old_page:
             if new_page is not None:
-                new_page.reindexObject(['is_default_page'])
+                new_page.reindexObject(["is_default_page"])
             if old_page is not None:
-                old_page.reindexObject(['is_default_page'])
+                old_page.reindexObject(["is_default_page"])
 
     @security.protected(ModifyViewTemplate)
     def setLayout(self, layout):
         # Set the layout as the current view.
 
         # 'layout' should be one of the list returned by getAvailableLayouts(),
         # but it is not enforced. If a default page has been set with
         # setDefaultPage(), it is turned off by calling setDefaultPage(None).
         if not (layout and isinstance(layout, str)):
             raise ValueError(
-                "layout must be a non empty string, got %s(%s)" %
-                (layout, type(layout))
+                f"layout must be a non empty string, got {layout}({type(layout)})"
             )
 
         defaultPage = self.getDefaultPage()
         if defaultPage is None and layout == self.getLayout():
             return
 
-        if self.hasProperty('layout'):
+        if self.hasProperty("layout"):
             self.manage_changeProperties(layout=layout)
         else:
-            if getattr(aq_base(self), 'layout', _marker) is not _marker:
+            if getattr(aq_base(self), "layout", _marker) is not _marker:
                 # Archetypes remains? clean up
                 old = self.layout
                 if old and not isinstance(old, str):
                     raise RuntimeError(
-                        "layout attribute exists on %s and is no string: %s" %
-                        (self, type(old))
+                        "layout attribute exists on %s and is no string: %s"
+                        % (self, type(old))
                     )
-                delattr(self, 'layout')
+                delattr(self, "layout")
 
-            self.manage_addProperty('layout', layout, 'string')
+            self.manage_addProperty("layout", layout, "string")
 
         self.setDefaultPage(None)
 
     @security.protected(View)
     def getDefaultLayout(self):
         # Get the default layout method.
         fti = self.getTypeInfo()
         if fti is None:
             return "base_view"  # XXX
         return fti.getDefaultViewMethod(self)
 
     @security.public
     def canSetLayout(self):
         # Check if the current authenticated user is permitted to select a layout.
-        mtool = getToolByName(self, 'portal_membership')
+        mtool = getToolByName(self, "portal_membership")
         member = mtool.getAuthenticatedMember()
         return member.has_permission(ModifyViewTemplate, self)
 
     @security.protected(View)
     def getAvailableLayouts(self):
         # Get the layouts registered for this object from its FTI.
         fti = self.getTypeInfo()
@@ -213,18 +212,15 @@
         spec = (providedBy(self), providedBy(self.REQUEST))
         gsm = getSiteManager()
         for mid in method_ids:
             if not isinstance(mid, str):
                 mid = mid.decode()
             factory = gsm.adapters.lookup(spec, Interface, mid)
             if factory is not None:
-                menu = getUtility(
-                    IBrowserMenu,
-                    'plone_displayviews'
-                )
+                menu = getUtility(IBrowserMenu, "plone_displayviews")
                 item = menu.getMenuItemByAction(self, self.REQUEST, mid)
                 title = item and item.title or mid
                 result.append((mid, title))
             else:
                 method = getattr(self, mid, None)
                 if method is not None:
                     # a method might be a template, script or method
@@ -241,24 +237,24 @@
 
 def check_default_page(obj, event):
     """event subscriber, unset default page if target no longer exists
 
     used by default for zope.container.interfaces.IContainerModifiedEvent
     """
     container = obj
-    default_page_id = container.getProperty('default_page', '')
+    default_page_id = container.getProperty("default_page", "")
     if default_page_id and not (default_page_id in container.objectIds()):
         ISelectableBrowserDefault(container).setDefaultPage(None)
 
 
 def rename_default_page(obj, event):
-    """event subscriber, rename default page if targte was renamed
+    """event subscriber, rename default page if target was renamed
 
     used by default for zope.lifecycleevent.interfaces.IObjectMovedEvent
     """
     newParent = event.newParent
     if newParent != event.oldParent:
         return
     elif ISelectableBrowserDefault.providedBy(newParent):
-        default_page_id = newParent.getProperty('default_page', '')
+        default_page_id = newParent.getProperty("default_page", "")
         if default_page_id == event.oldName:
             ISelectableBrowserDefault(newParent).setDefaultPage(event.newName)
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/configure.zcml` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 <configure
-   xmlns="http://namespaces.zope.org/zope"
-   xmlns:browser="http://namespaces.zope.org/browser"
-   xmlns:five="http://namespaces.zope.org/five"
-   i18n_domain="cmf_default">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:browser="http://namespaces.zope.org/browser"
+    xmlns:five="http://namespaces.zope.org/five"
+    i18n_domain="cmf_default"
+    >
 
   <include package="Products.CMFCore" />
 
   <browser:page
-     for="zope.browser.interfaces.IAdding"
-     name="addDVFactoryTypeInformation.html"
-     template="browser/addWithPresettings.pt"
-     class=".browser.typeinfo.DVFactoryTypeInformationAddView"
-     permission="cmf.ManagePortal"
-     />
+      name="addDVFactoryTypeInformation.html"
+      for="zope.browser.interfaces.IAdding"
+      class=".browser.typeinfo.DVFactoryTypeInformationAddView"
+      template="browser/addWithPresettings.pt"
+      permission="cmf.ManagePortal"
+      />
 
   <five:registerClass
-     class=".fti.DynamicViewTypeInformation"
-     meta_type="Factory-based Type Information with dynamic views"
-     addview="addDVFactoryTypeInformation.html"
-     permission="cmf.ManagePortal"
-     global="False"
-     />
+      class=".fti.DynamicViewTypeInformation"
+      permission="cmf.ManagePortal"
+      addview="addDVFactoryTypeInformation.html"
+      global="False"
+      meta_type="Factory-based Type Information with dynamic views"
+      />
 
   <permission
-    id="cmf.ModifyViewTemplate"
-    title="Modify view template"
-    />
+      id="cmf.ModifyViewTemplate"
+      title="Modify view template"
+      />
 
   <subscriber
-    for=".interfaces.ISelectableBrowserDefault
-         zope.container.interfaces.IContainerModifiedEvent"
-    handler=".browserdefault.check_default_page" />
+      for=".interfaces.ISelectableBrowserDefault
+           zope.container.interfaces.IContainerModifiedEvent"
+      handler=".browserdefault.check_default_page"
+      />
 
   <subscriber
-    for="*
-         zope.lifecycleevent.interfaces.IObjectMovedEvent"
-    handler=".browserdefault.rename_default_page" />
+      for="*
+           zope.lifecycleevent.interfaces.IObjectMovedEvent"
+      handler=".browserdefault.rename_default_page"
+      />
 
 </configure>
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/content_for_tests.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/content_for_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from Products.CMFCore.PortalFolder import PortalFolder
 from Products.CMFCore.PortalContent import PortalContent
+from Products.CMFCore.PortalFolder import PortalFolder
 from Products.CMFDynamicViewFTI.browserdefault import BrowserDefaultMixin
 
 
 class DynFolder(PortalFolder, BrowserDefaultMixin):
     pass
 
 
 class DynDocument(PortalContent, BrowserDefaultMixin):
-
     def __init__(self, id, title):
         self.id = id
         self.title = title
 
 
-def addDynFolder(self, id, title='', REQUEST=None):
-    """Add a new DynFolder object with id *id*.
-    """
+def addDynFolder(self, id, title="", REQUEST=None):
+    """Add a new DynFolder object with id *id*."""
     ob = DynFolder(id, title)
     self._setObject(id, ob, suppress_events=True)
 
 
-def addDynDocument(self, id, title='', REQUEST=None):
-    """Add a new DynDocument object with id *id*.
-    """
+def addDynDocument(self, id, title="", REQUEST=None):
+    """Add a new DynDocument object with id *id*."""
     ob = DynDocument(id, title)
     self._setObject(id, ob, suppress_events=True)
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/fti.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/fti.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from AccessControl import ClassSecurityInfo
-from Acquisition import aq_base
 from AccessControl.class_init import InitializeClass
+from Acquisition import aq_base
 from Products.CMFCore.permissions import View
 from Products.CMFCore.TypesTool import FactoryTypeInformation
 from Products.CMFCore.utils import getToolByName
 from Products.CMFDynamicViewFTI.interfaces import IDynamicViewTypeInformation
 from zope.interface import implementer
 
 
@@ -17,42 +17,42 @@
     implement our own hasattr() replacement.
     """
     return getattr(obj, name, _marker) is not _marker
 
 
 def safe_callable(obj):
     """Make sure our callable checks are ConflictError safe."""
-    if safe_hasattr(obj, '__class__'):
-        if safe_hasattr(obj, '__call__'):
+    if safe_hasattr(obj, "__class__"):
+        if safe_hasattr(obj, "__call__"):
             return True
         else:
             return isinstance(obj, type)
     else:
         return callable(obj)
 
 
 def om_has_key(context, key):
     """Object Manager has_key method with optimization for btree folders
 
     Zope's OFS.ObjectManager has no method for checking if an object with an id
     exists inside a folder.
     """
-    klass = getattr(aq_base(context), '__class__', None)
-    if hasattr(klass, 'has_key'):
+    klass = getattr(aq_base(context), "__class__", None)
+    if hasattr(klass, "has_key"):
         # BTreeFolder2 optimization
         if key in context:
             return True
     else:
         # standard ObjectManager api
         if key in context.objectIds():
             return True
     return False
 
 
-fti_meta_type = 'Factory-based Type Information with dynamic views'
+fti_meta_type = "Factory-based Type Information with dynamic views"
 
 
 @implementer(IDynamicViewTypeInformation)
 class DynamicViewTypeInformation(FactoryTypeInformation):
     """FTI with dynamic views
 
     A value of (dynamic view) as alias is replaced by the output of
@@ -60,85 +60,79 @@
     """
 
     meta_type = fti_meta_type
     security = ClassSecurityInfo()
 
     _properties = FactoryTypeInformation._properties + (
         {
-            'id': 'default_view',
-            'type': 'string',
-            'mode': 'w',
-            'label': 'Default view method',
+            "id": "default_view",
+            "type": "string",
+            "mode": "w",
+            "label": "Default view method",
         },
         {
-            'id': 'view_methods',
-            'type': 'lines',
-            'mode': 'w',
-            'label': 'Available view methods'
+            "id": "view_methods",
+            "type": "lines",
+            "mode": "w",
+            "label": "Available view methods",
         },
         {
-            'id': 'default_view_fallback',
-            'type': 'boolean',
-            'mode': 'w',
-            'label': 'Fall back to default view?'
+            "id": "default_view_fallback",
+            "type": "boolean",
+            "mode": "w",
+            "label": "Fall back to default view?",
         },
     )
 
-    default_view = ''
+    default_view = ""
     view_methods = ()
     default_view_fallback = False
 
     def manage_changeProperties(self, **kw):
         """Overwrite change properties to verify that default_view is in the method
         list
         """
         FactoryTypeInformation.manage_changeProperties(self, **kw)
         default_view = self.default_view
         view_methods = self.view_methods
         if not default_view:
             # TODO: use view action
             self.default_view = default_view = self.immediate_view
         if not view_methods:
-            self.view_methods = view_methods = (default_view, )
+            self.view_methods = view_methods = (default_view,)
         if default_view and default_view not in view_methods:
             raise ValueError(f"{default_view} not in {view_methods}")
 
     @security.protected(View)
     def getDefaultViewMethod(self, context):
         # Get the default view method from the FTI.
         return str(self.default_view)
 
     @security.protected(View)
     def getAvailableViewMethods(self, context):
         # Get a list of registered view methods.
         methods = self.view_methods
         if isinstance(methods, str):
-            methods = (methods, )
+            methods = (methods,)
         return tuple(methods)
 
     @security.protected(View)
-    def getViewMethod(
-        self,
-        context,
-        enforce_available=False,
-        check_exists=False
-    ):
+    def getViewMethod(self, context, enforce_available=False, check_exists=False):
         # Get view method (aka layout) name from context.
         # Return -- view method from context or default view name.
         default = self.getDefaultViewMethod(context)
-        layout = getattr(aq_base(context), 'layout', None)
+        layout = getattr(aq_base(context), "layout", None)
 
         if safe_callable(layout):
             layout = layout()
         if not layout:
             return default
         if not isinstance(layout, str):
             raise TypeError(
-                "layout of %s must be a string, got %s" %
-                (repr(context), type(layout))
+                f"layout of {repr(context)} must be a string, got {type(layout)}"
             )
         if enforce_available:
             available = self.getAvailableViewMethods(context)
             if layout not in available:
                 return default
         if check_exists:
             method = getattr(context, layout, None)
@@ -155,44 +149,44 @@
         #
         # Non folderish objects don't have a default view.
         #
         # If check_exists is enabled the method makes sure the object with the
         # default page id exists.
         #
         # Return -- None for no default page or a string
-        if not getattr(aq_base(context), 'isPrincipiaFolderish', False):
+        if not getattr(aq_base(context), "isPrincipiaFolderish", False):
             # non folderish objects don't have a default page per se
             return None
 
-        default_page = getattr(aq_base(context), 'default_page', None)
+        default_page = getattr(aq_base(context), "default_page", None)
 
         if safe_callable(default_page):
             default_page = default_page()
         if not default_page:
             return None
         if isinstance(default_page, (tuple, list)):
             default_page = default_page[0]
         if not isinstance(default_page, str):
             raise TypeError(
-                "default_page must be a string, got %s(%s):" %
-                (default_page, type(default_page))
+                "default_page must be a string, got %s(%s):"
+                % (default_page, type(default_page))
             )
 
         if check_exists and not om_has_key(context, default_page):
             return None
 
         return default_page
 
     @security.protected(View)
     def defaultView(self, context):
         # Get the current view to use for an object. If a default page is set,
         # use that, else use the currently selected view method/layout.
 
         # Delegate to PloneTool's version if we have it else, use own rules
-        plone_utils = getToolByName(self, 'plone_utils', None)
+        plone_utils = getToolByName(self, "plone_utils", None)
         if plone_utils is not None:
             obj, path = plone_utils.browserDefault(context)
             return path[-1]
         else:
             default_page = self.getDefaultPage(context, check_exists=True)
             if default_page is not None:
                 return default_page
@@ -206,24 +200,21 @@
         # Use "(dynamic view)" as the alias target to look up as per
         # defaultView()
 
         # Use "(selected layout)" as the alias target to look up as per
         # getViewMethod()
 
         methodTarget = FactoryTypeInformation.queryMethodID(
-            self,
-            alias,
-            default=default,
-            context=context
+            self, alias, default=default, context=context
         )
         if not isinstance(methodTarget, str):
             # nothing to do, method_id is probably None
             return methodTarget
 
-        if context is None or default == '':
+        if context is None or default == "":
             # the edit zpts like typesAliases don't apply a context and set the
             # default to ''. We do not want to resolve (dynamic view) for these
             # methods.
             return methodTarget
 
         # Our two special targets:
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/interfaces.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 class IDynamicViewTypeInformation(ITypeInformation):
     """Interface for FTI with dynamic views
 
     A value of (dynamic view) as alias is replaced by the output of getLayout()
     """
 
     def getAvailableViewMethods(context):
-        """Get a list of registered view methods
-        """
+        """Get a list of registered view methods"""
 
     def getViewMethod(context, enforce_available=True):
         """Get view method name from context
 
         Return -- view method from context or default view name
         """
 
     def getDefaultViewMethod(context):
-        """Get the default view method from the FTI
-        """
+        """Get the default view method from the FTI"""
 
     def getDefaultPage(context, check_exists=False):
         """Get the default page from a folderish object
 
         Non folderish objects don't have a default view.
 
         If check_exists is enabled the method makes sure the object with the
@@ -74,16 +72,15 @@
     def getLayout(**kw):
         """Get the selected layout template.
 
         Note that a selected default page will override the layout template.
         """
 
     def getDefaultLayout():
-        """Get the default layout template.
-        """
+        """Get the default layout template."""
 
 
 class ISelectableBrowserDefault(IBrowserDefault):
     """Content supporting operations to explicitly set the default layout
     template or default page object.
     """
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynFolder.xml` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynDocument.xml`

 * *Files 18% similar despite different names*

#### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynFolder.xml` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/profiles/sample_types/types/DynDocument.xml`

```diff
@@ -1,22 +1,23 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="DynFolder" meta_type="Factory-based Type Information with dynamic views">
-  <property name="title">DynFolder</property>
-  <property name="content_icon">folder_icon.gif</property>
-  <property name="content_meta_type">DynFolder</property>
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Factory-based Type Information with dynamic views" name="DynDocument">
+  <property name="title">DynDocument</property>
+  <property name="description">A page in the site. Can contain rich text.</property>
+  <property name="content_icon">document_icon.gif</property>
+  <property name="content_meta_type">DynDocument</property>
   <property name="product">CMFDynamicViewFTI</property>
-  <property name="factory">addDynFolder</property>
-  <property name="immediate_view">folder_edit_form</property>
+  <property name="factory">addDynDocument</property>
+  <property name="immediate_view">metadata_edit_form</property>
   <property name="global_allow">True</property>
-  <property name="filter_content_types">False</property>
+  <property name="filter_content_types">True</property>
+  <property name="allowed_content_types"/>
   <property name="default_view">index_html</property>
   <property name="view_methods">
-    <element value="index_html"/>
+    <element value="document_view"/>
     <element value="custom_view"/>
-    <element value="zope3_view"/>
   </property>
   <alias from="(Default)" to="(Dynamic view)"/>
   <alias from="view" to="(Selected layout)"/>
-  <action title="View" action_id="view" category="object" condition_expr="" url_expr="string:${object_url}" visible="True">
+  <action action_id="view" category="object" condition_expr="" title="View" url_expr="string:${object_url}/view" visible="True">
     <permission value="View"/>
   </action>
 </object>
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/CMFDVFTITestCase.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/CMFDVFTITestCase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,87 @@
 from plone.app import testing
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
+from plone.base.utils import unrestricted_construct_instance
 from Products.CMFCore.interfaces import ISiteRoot
 from Products.CMFCore.utils import getToolByName
-from Products.CMFPlone.utils import _createObjectByType
-from Products.GenericSetup import EXTENSION, profile_registry
+from Products.GenericSetup import EXTENSION
+from Products.GenericSetup import profile_registry
+
 import transaction
 import unittest
 
 
 class CMFDynamicViewFTIFixture(PloneSandboxLayer):
-
-    defaultBases = (PLONE_FIXTURE, )
+    defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         profile_registry.registerProfile(
-            'CMFDVFTI_sampletypes',
-            'CMFDynamicViewFTI Sample Content Types',
-            'Extension profile including CMFDVFTI sample content types',
-            'profiles/sample_types',
-            'CMFDynamicViewFTI',
+            "CMFDVFTI_sampletypes",
+            "CMFDynamicViewFTI Sample Content Types",
+            "Extension profile including CMFDVFTI sample content types",
+            "profiles/sample_types",
+            "CMFDynamicViewFTI",
             EXTENSION,
-            for_=ISiteRoot
+            for_=ISiteRoot,
         )
         import Products.CMFDynamicViewFTI.tests
-        self.loadZCML(name='browserdefault.zcml',
-                      package=Products.CMFDynamicViewFTI.tests)
 
-    def setUpPloneSite(self, portal):
-        self.applyProfile(portal, 'CMFDynamicViewFTI:CMFDVFTI_sampletypes')
+        self.loadZCML(
+            name="browserdefault.zcml", package=Products.CMFDynamicViewFTI.tests
+        )
 
+        from plone.testing.zope import _INSTALLED_PRODUCTS
+
+        if "Products.CMFDynamicViewFTI" not in _INSTALLED_PRODUCTS.keys():
+            # replicate plone.testing.zope.installProduct
+            # when running the tests via tox Products.CMFDynamicViewFTI
+            # folder location is different than the other Products.*
+            # packages.
+            # `installProduct` checks for that and bails out otherwise.
+            from AccessControl.class_init import InitializeClass
+            from OFS.Application import get_folder_permissions
+            from OFS.Application import install_product
+            from OFS.Folder import Folder
+            from pathlib import Path
+
+            import inspect
+
+            module_path = Path(inspect.getfile(Products.CMFDynamicViewFTI))
+            product_folder = str(module_path.parent.parent)
+
+            install_product(
+                app,
+                product_folder,
+                "CMFDynamicViewFTI",
+                [],
+                get_folder_permissions(),
+                raise_exc=1,
+            )
+            InitializeClass(Folder)
+
+    def setUpPloneSite(self, portal):
+        self.applyProfile(portal, "CMFDynamicViewFTI:CMFDVFTI_sampletypes")
 
-    def tearDownZope(self, app):
-        pass
 
 CDV_FIXTURE = CMFDynamicViewFTIFixture()
 CDV_FUNCTIONAL_TESTING = testing.FunctionalTesting(
-    bases=(CDV_FIXTURE, ), name='CMFDynamicViewFTI Testing:Functional')
+    bases=(CDV_FIXTURE,), name="CMFDynamicViewFTI Testing:Functional"
+)
 
 
 class CMFDVFTITestCase(unittest.TestCase):
     """This is a stub now, but in case you want to try
-       something fancy on Your Branch (tm), put it here.
+    something fancy on Your Branch (tm), put it here.
     """
+
     layer = CDV_FUNCTIONAL_TESTING
 
     def setUp(self):
         """Set up before each test."""
-        self.app = self.layer['app']
-        self.portal = self.layer['portal']
-        _createObjectByType('DynFolder', self.portal, id='folder')
+        self.app = self.layer["app"]
+        self.portal = self.layer["portal"]
+        unrestricted_construct_instance("DynFolder", self.portal, id="folder")
         self.folder = self.portal.folder
-        self.types = getToolByName(self.portal, 'portal_types')
-        self.fti = self.types['DynFolder']
+        self.types = getToolByName(self.portal, "portal_types")
+        self.fti = self.types["DynFolder"]
         transaction.commit()
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/test_browserdefault.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/test_browserdefault.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-from Products.CMFCore.utils import getToolByName
 from Products.CMFDynamicViewFTI.browserdefault import BrowserDefaultMixin
 from Products.CMFDynamicViewFTI.interfaces import IBrowserDefault
 from Products.CMFDynamicViewFTI.interfaces import ISelectableBrowserDefault
 from Products.CMFDynamicViewFTI.tests import CMFDVFTITestCase
 from zope.interface import directlyProvides
 from zope.interface import Interface
 from zope.interface.verify import verifyClass
 from zope.publisher.browser import TestRequest
 
 
 class DummyFolder(BrowserDefaultMixin):
-
     def getTypeInfo(self):
         return self.fti
 
 
 class IDummy(Interface):
-    """ marker interface for a zope 3 view """
+    """marker interface for a zope 3 view"""
 
 
 class TestBrowserDefault(CMFDVFTITestCase.CMFDVFTITestCase):
-
     def test_doesImplementISelectableBrowserDefault(self):
         iface = ISelectableBrowserDefault
         self.assertTrue(iface.implementedBy(BrowserDefaultMixin))
         self.assertTrue(verifyClass(iface, BrowserDefaultMixin))
 
     def test_extendsInterface(self):
         self.assertTrue(ISelectableBrowserDefault.extends(IBrowserDefault))
 
 
 class TestAvailableLayouts(CMFDVFTITestCase.CMFDVFTITestCase):
-
     def setUp(self):
         super().setUp()
         self.dfolder = DummyFolder()
-        self.dfolder.fti = self.types['DynFolder']
+        self.dfolder.fti = self.types["DynFolder"]
 
     def test_Zope3View(self):
         dfolder = self.dfolder
-        dfolder.layout = 'zope3_view'
+        dfolder.layout = "zope3_view"
         dfolder.REQUEST = TestRequest()
         view_methods = dfolder.getAvailableLayouts()
         view_ids = [view_id for view_id, foo in view_methods]
         self.assertNotIn(dfolder.layout, view_ids)
 
         # Mark the object with interface connected to the zope 3 view
         directlyProvides(dfolder, IDummy)
         view_methods = dfolder.getAvailableLayouts()
         view_ids = [view_id for view_id, foo in view_methods]
         self.assertIn(dfolder.layout, view_ids)
 
     def test_Zope3ViewTitle(self):
         dfolder = self.dfolder
-        dfolder.layout = 'zope3_view'
+        dfolder.layout = "zope3_view"
         dfolder.REQUEST = TestRequest()
         directlyProvides(dfolder, IDummy)
         view_methods = dfolder.getAvailableLayouts()
 
         for id, title in view_methods:
             if id == dfolder.layout:
-                self.assertEqual(title, 'Zope3 Test View')
+                self.assertEqual(title, "Zope3 Test View")
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products/CMFDynamicViewFTI/tests/test_fti.py` & `Products.CMFDynamicViewFTI-7.0.1/Products/CMFDynamicViewFTI/tests/test_fti.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from plone.app.testing import TEST_USER_NAME
-from plone.app.testing import TEST_USER_PASSWORD
 from Products.CMFCore.interfaces import ITypeInformation
 from Products.CMFDynamicViewFTI.fti import DynamicViewTypeInformation
 from Products.CMFDynamicViewFTI.interfaces import IDynamicViewTypeInformation
 from Products.CMFDynamicViewFTI.tests import CMFDVFTITestCase
 from zope.interface.verify import verifyObject
 
 import transaction
 
 
 fti_meta_type = DynamicViewTypeInformation.meta_type
 
 
 class TestFTI(CMFDVFTITestCase.CMFDVFTITestCase):
-
     def _makeOne(self):
         # Create and return a DynFolder
-        self.folder.invokeFactory('DynFolder', id='dynfolder')
+        self.folder.invokeFactory("DynFolder", id="dynfolder")
         return self.folder.dynfolder
 
     def test_doesImplementITypeInformation(self):
         iface = ITypeInformation
         self.assertTrue(iface.providedBy(self.fti))
         self.assertTrue(verifyObject(iface, self.fti))
 
@@ -33,215 +30,195 @@
         self.assertEqual(self.fti.meta_type, fti_meta_type)
 
     def test_paranoid_subclass_test(self):
         self.assertTrue(isinstance(self.fti, DynamicViewTypeInformation))
 
     def test_CreateDynFolder(self):
         dynfolder = self._makeOne()
-        self.assertEqual(dynfolder.getPortalTypeName(), 'DynFolder')
+        self.assertEqual(dynfolder.getPortalTypeName(), "DynFolder")
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getId(), 'DynFolder')
-        self.assertEqual(info.Title(), 'DynFolder')
-        self.assertEqual(info.getDefaultViewMethod(dynfolder), 'index_html')
+        self.assertEqual(info.getId(), "DynFolder")
+        self.assertEqual(info.Title(), "DynFolder")
+        self.assertEqual(info.getDefaultViewMethod(dynfolder), "index_html")
         self.assertEqual(
             info.getAvailableViewMethods(dynfolder),
-            ('index_html', 'custom_view', 'zope3_view')
+            ("index_html", "custom_view", "zope3_view"),
         )
 
     def test_DynFolderDefaultView(self):
         dynfolder = self._makeOne()
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getViewMethod(dynfolder), 'index_html')
+        self.assertEqual(info.getViewMethod(dynfolder), "index_html")
 
     def test_DynFolderCustomView(self):
         dynfolder = self._makeOne()
-        self.types.DynFolder.manage_changeProperties(
-            default_view='custom_view'
-        )
+        self.types.DynFolder.manage_changeProperties(default_view="custom_view")
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getViewMethod(dynfolder), 'custom_view')
+        self.assertEqual(info.getViewMethod(dynfolder), "custom_view")
 
     def test_DynFolderViewFromLayout(self):
         dynfolder = self._makeOne()
-        dynfolder.layout = 'custom_view'
+        dynfolder.layout = "custom_view"
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getViewMethod(dynfolder), 'custom_view')
+        self.assertEqual(info.getViewMethod(dynfolder), "custom_view")
 
     def test_DynFolderViewFromCallableLayout(self):
         dynfolder = self._makeOne()
-        dynfolder.layout = lambda: 'custom_view'
+        dynfolder.layout = lambda: "custom_view"
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getViewMethod(dynfolder), 'custom_view')
+        self.assertEqual(info.getViewMethod(dynfolder), "custom_view")
 
     def test_NoneLayoutReturnsDefaultView(self):
         dynfolder = self._makeOne()
         dynfolder.layout = None
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getViewMethod(dynfolder), 'index_html')
+        self.assertEqual(info.getViewMethod(dynfolder), "index_html")
 
     def test_EmptyLayoutReturnsDefaultView(self):
         dynfolder = self._makeOne()
-        dynfolder.layout = ''
+        dynfolder.layout = ""
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getViewMethod(dynfolder), 'index_html')
+        self.assertEqual(info.getViewMethod(dynfolder), "index_html")
 
     def test_InvalidLayoutRaisesTypeError(self):
         dynfolder = self._makeOne()
         dynfolder.layout = object()
         info = self.types.getTypeInfo(dynfolder)
         self.assertRaises(TypeError, info.getViewMethod, dynfolder)
 
     def test_EnforceLayoutAvailable(self):
         dynfolder = self._makeOne()
-        dynfolder.layout = 'custom_view'
+        dynfolder.layout = "custom_view"
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(
-            info.getViewMethod(dynfolder, enforce_available=True),
-            'custom_view'
+            info.getViewMethod(dynfolder, enforce_available=True), "custom_view"
         )
 
     def test_UnavailableLayoutReturnsDefaultView(self):
         dynfolder = self._makeOne()
-        dynfolder.layout = 'bad_view'
+        dynfolder.layout = "bad_view"
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(
-            info.getViewMethod(dynfolder, enforce_available=True),
-            'index_html'
+            info.getViewMethod(dynfolder, enforce_available=True), "index_html"
         )
 
     def test_CheckLayoutExists(self):
         dynfolder = self._makeOne()
-        dynfolder.manage_addDTMLMethod('custom_view', file='')
-        dynfolder.layout = 'custom_view'
+        dynfolder.manage_addDTMLMethod("custom_view", file="")
+        dynfolder.layout = "custom_view"
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(
-            info.getViewMethod(dynfolder, check_exists=True),
-            'custom_view'
+            info.getViewMethod(dynfolder, check_exists=True), "custom_view"
         )
 
     def test_MissingLayoutReturnsDefaultView(self):
         dynfolder = self._makeOne()
-        dynfolder.layout = 'bad_view'
+        dynfolder.layout = "bad_view"
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(
-            info.getViewMethod(dynfolder, check_exists=True),
-            'index_html'
-        )
+        self.assertEqual(info.getViewMethod(dynfolder, check_exists=True), "index_html")
 
     def test_DynFolderDefaultPage(self):
         dynfolder = self._makeOne()
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(info.getDefaultPage(dynfolder), None)
 
     def test_DynFolderDefaultPageFromAttribute(self):
         dynfolder = self._makeOne()
-        dynfolder.default_page = 'custom_page'
+        dynfolder.default_page = "custom_page"
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getDefaultPage(dynfolder), 'custom_page')
+        self.assertEqual(info.getDefaultPage(dynfolder), "custom_page")
 
     def test_DynFolderDefaultPageFromCallable(self):
         dynfolder = self._makeOne()
-        dynfolder.default_page = lambda: 'custom_page'
+        dynfolder.default_page = lambda: "custom_page"
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(info.getDefaultPage(dynfolder), 'custom_page')
+        self.assertEqual(info.getDefaultPage(dynfolder), "custom_page")
 
     def test_NoneDefaultPageReturnsNone(self):
         dynfolder = self._makeOne()
         dynfolder.default_page = None
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(info.getDefaultPage(dynfolder), None)
 
     def test_EmptyDefaultPageReturnsNone(self):
         dynfolder = self._makeOne()
-        dynfolder.default_page = ''
+        dynfolder.default_page = ""
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(info.getDefaultPage(dynfolder), None)
 
     def test_InvalidDefaultPageRaisesTypeError(self):
         dynfolder = self._makeOne()
         dynfolder.default_page = object()
         info = self.types.getTypeInfo(dynfolder)
         self.assertRaises(TypeError, info.getDefaultPage, dynfolder)
 
     def test_CheckDefaultPageExists(self):
         dynfolder = self._makeOne()
-        dynfolder.manage_addDTMLMethod('custom_page', file='')
-        dynfolder.default_page = 'custom_page'
+        dynfolder.manage_addDTMLMethod("custom_page", file="")
+        dynfolder.default_page = "custom_page"
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(
-            info.getDefaultPage(dynfolder, check_exists=True),
-            'custom_page'
+            info.getDefaultPage(dynfolder, check_exists=True), "custom_page"
         )
 
     def test_MissingDefaultPageReturnsNone(self):
         dynfolder = self._makeOne()
-        dynfolder.default_page = 'bad_page'
+        dynfolder.default_page = "bad_page"
         info = self.types.getTypeInfo(dynfolder)
-        self.assertEqual(
-            info.getDefaultPage(dynfolder, check_exists=True),
-            None
-        )
+        self.assertEqual(info.getDefaultPage(dynfolder, check_exists=True), None)
 
     def test_NonFolderishObjectReturnsNone(self):
         dynfolder = self._makeOne()
         dynfolder.isPrincipiaFolderish = 0
-        dynfolder.default_page = 'custom_page'
+        dynfolder.default_page = "custom_page"
         info = self.types.getTypeInfo(dynfolder)
         self.assertEqual(info.getDefaultPage(dynfolder), None)
 
     def test_DefaultViewWithBadLayoutUseFallback(self):
         dynfolder = self._makeOne()
-        dynfolder.layout = 'bad_view'
+        dynfolder.layout = "bad_view"
         info = self.types.getTypeInfo(dynfolder)
         # fallback not returned if not activated
         self.assertFalse(info.default_view_fallback)
-        self.assertEqual(
-            info.defaultView(dynfolder),
-            'bad_view'
-        )
+        self.assertEqual(info.defaultView(dynfolder), "bad_view")
         # enable fallback
         info.default_view_fallback = True
-        self.assertEqual(
-            info.defaultView(dynfolder),
-            info.default_view
-        )
+        self.assertEqual(info.defaultView(dynfolder), info.default_view)
 
 
 class TestModifyDefaultPage(CMFDVFTITestCase.CMFDVFTITestCase):
-
     def _makeOne(self):
         # Create and return a DynFolder
-        self.folder.invokeFactory('DynFolder', id='dynfolder')
+        self.folder.invokeFactory("DynFolder", id="dynfolder")
         dynfolder = self.folder.dynfolder
-        dynfolder.invokeFactory('DynDocument', id='default_document')
-        dynfolder.setDefaultPage('default_document')
+        dynfolder.invokeFactory("DynDocument", id="default_document")
+        dynfolder.setDefaultPage("default_document")
         return dynfolder
 
     def test_rename_default_page(self):
         dynfolder = self._makeOne()
-        self.assertEqual(dynfolder.getDefaultPage(), 'default_document')
+        self.assertEqual(dynfolder.getDefaultPage(), "default_document")
         transaction.commit()
-        dynfolder.manage_renameObject('default_document', 'renamed_default')
-        self.assertFalse('default_document' in dynfolder.objectIds())
-        self.assertTrue('renamed_default' in dynfolder.objectIds())
-        self.assertEqual(dynfolder.getDefaultPage(), 'renamed_default')
-        self.assertEqual(dynfolder.getProperty('default_page', ''),
-                         'renamed_default')
+        dynfolder.manage_renameObject("default_document", "renamed_default")
+        self.assertFalse("default_document" in dynfolder.objectIds())
+        self.assertTrue("renamed_default" in dynfolder.objectIds())
+        self.assertEqual(dynfolder.getDefaultPage(), "renamed_default")
+        self.assertEqual(dynfolder.getProperty("default_page", ""), "renamed_default")
 
     def test_delete_default_page(self):
         dynfolder = self._makeOne()
-        self.assertEqual(dynfolder.getDefaultPage(), 'default_document')
-        dynfolder.manage_delObjects(['default_document'])
-        self.assertFalse('default_document' in dynfolder.objectIds())
+        self.assertEqual(dynfolder.getDefaultPage(), "default_document")
+        dynfolder.manage_delObjects(["default_document"])
+        self.assertFalse("default_document" in dynfolder.objectIds())
         self.assertEqual(dynfolder.getDefaultPage(), None)
-        self.assertEqual(dynfolder.getProperty('default_page', ''), '')
+        self.assertEqual(dynfolder.getProperty("default_page", ""), "")
 
     def test_cut_default_page(self):
         dynfolder = self._makeOne()
-        self.assertEqual(dynfolder.getDefaultPage(), 'default_document')
+        self.assertEqual(dynfolder.getDefaultPage(), "default_document")
         transaction.commit()
-        clipboard = dynfolder.manage_cutObjects(['default_document'])
+        clipboard = dynfolder.manage_cutObjects(["default_document"])
         self.folder.manage_pasteObjects(clipboard)
-        self.assertFalse('default_document' in dynfolder.objectIds())
-        self.assertTrue('default_document' in self.folder.objectIds())
+        self.assertFalse("default_document" in dynfolder.objectIds())
+        self.assertTrue("default_document" in self.folder.objectIds())
         self.assertEqual(dynfolder.getDefaultPage(), None)
-        self.assertEqual(dynfolder.getProperty('default_page', ''), '')
+        self.assertEqual(dynfolder.getProperty("default_page", ""), "")
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/PKG-INFO` & `Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: Products.CMFDynamicViewFTI
-Version: 7.0.0a1
+Version: 7.0.1
 Summary: CMFDynamicViewFTI is a product for dynamic views in CMF.
 Home-page: https://pypi.org/project/Products.CMFDynamicViewFTI
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: ZPL
 Keywords: Zope CMF Plone dynamic view
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Overview
 ========
 
 CMFDynamicViewFTI is a product for dynamic views in CMF.
 The product contains an additional base class for types and a new factory type information (FTI).
@@ -55,14 +56,33 @@
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
+  [plone devs] (3333c742)
+
+
+7.0.0 (2022-12-01)
+------------------
+
+Bug fixes:
+
+
+- Final release for Plone 6.0.0. (#600)
+
+
 7.0.0a1 (2022-01-19)
 --------------------
 
 Breaking changes:
 
 
 - Plone 6: always use lines for the view_methods property.
@@ -421,9 +441,7 @@
 - Stop Acquisition for default_page.
   [panjunyong]
 
 1.0.0 - 2005-07-29
 ------------------
 
 - Initial release.
-
-
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/Products.CMFDynamicViewFTI.egg-info/SOURCES.txt` & `Products.CMFDynamicViewFTI-7.0.1/Products.CMFDynamicViewFTI.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+.editorconfig
 .gitignore
+.meta.toml
+.pre-commit-config.yaml
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
-bootstrap.py
 buildout.cfg
 pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 Products/__init__.py
 Products.CMFDynamicViewFTI.egg-info/PKG-INFO
 Products.CMFDynamicViewFTI.egg-info/SOURCES.txt
 Products.CMFDynamicViewFTI.egg-info/dependency_links.txt
 Products.CMFDynamicViewFTI.egg-info/namespace_packages.txt
 Products.CMFDynamicViewFTI.egg-info/not-zip-safe
 Products.CMFDynamicViewFTI.egg-info/requires.txt
 Products.CMFDynamicViewFTI.egg-info/top_level.txt
 Products/CMFDynamicViewFTI/__init__.py
 Products/CMFDynamicViewFTI/browserdefault.py
 Products/CMFDynamicViewFTI/configure.zcml
 Products/CMFDynamicViewFTI/content_for_tests.py
 Products/CMFDynamicViewFTI/fti.py
-Products/CMFDynamicViewFTI/interface.py
 Products/CMFDynamicViewFTI/interfaces.py
 Products/CMFDynamicViewFTI/permissions.py
 Products/CMFDynamicViewFTI/browser/__init__.py
 Products/CMFDynamicViewFTI/browser/addWithPresettings.pt
 Products/CMFDynamicViewFTI/browser/typeinfo.py
 Products/CMFDynamicViewFTI/images/typeinfo.gif
 Products/CMFDynamicViewFTI/profiles/sample_types/types.xml
```

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/README.rst` & `Products.CMFDynamicViewFTI-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/docs/AUTHORS.txt` & `Products.CMFDynamicViewFTI-7.0.1/docs/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFDynamicViewFTI-7.0.0a1/docs/LICENSE.txt` & `Products.CMFDynamicViewFTI-7.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

