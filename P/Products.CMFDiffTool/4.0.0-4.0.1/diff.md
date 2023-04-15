# Comparing `tmp/Products.CMFDiffTool-4.0.0.tar.gz` & `tmp/Products.CMFDiffTool-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.CMFDiffTool-4.0.0.tar", last modified: Tue Mar 14 22:24:08 2023, max compression
+gzip compressed data, was "Products.CMFDiffTool-4.0.1.tar", last modified: Sat Apr 15 09:02:51 2023, max compression
```

## Comparing `Products.CMFDiffTool-4.0.0.tar` & `Products.CMFDiffTool-4.0.1.tar`

### file list

```diff
@@ -1,76 +1,80 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.044893 Products.CMFDiffTool-4.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      101 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/.isort.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     7615 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     9262 2023-03-14 22:24:08.045036 Products.CMFDiffTool-4.0.0/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.028375 Products.CMFDiffTool-4.0.0/Products/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.036232 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/
--rw-r--r--   0 maurits    (501) staff       (20)     4257 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/BaseDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     1955 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/BinaryDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     1160 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/CMFDTHtmlDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     6146 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/CMFDiffTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     6239 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/ChangeSet.py
--rw-r--r--   0 maurits    (501) staff       (20)     4117 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/FieldDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     6207 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/ListDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     3979 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/TextDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     1613 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2909 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/choicediff.py
--rw-r--r--   0 maurits    (501) staff       (20)      140 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6223 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/dexteritydiff.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.037128 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)       41 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      883 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2912 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/exportimport/difftool.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.038021 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)      182 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/interfaces/IChangeSet.py
--rw-r--r--   0 maurits    (501) staff       (20)     4560 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      260 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/interfaces/portal_diff.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.038624 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/libs/
--rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/libs/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     8085 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/libs/htmldiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     4838 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/namedfile.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.024886 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.039242 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      254 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)       68 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      422 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3806 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.043444 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      405 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/BaseTestCase.py
--rw-r--r--   0 maurits    (501) staff       (20)       67 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    11018 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testChangeSet.py
--rw-r--r--   0 maurits    (501) staff       (20)     4383 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testDiffTool.py
--rw-r--r--   0 maurits    (501) staff       (20)     6773 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testFieldDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     8367 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testListDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     4878 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testTextDiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     2282 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_astextdiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     4086 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_binarydiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     2474 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_choicediff.py
--rw-r--r--   0 maurits    (501) staff       (20)     5317 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_dexteritydiff.py
--rw-r--r--   0 maurits    (501) staff       (20)     2788 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_filelistdiff.py
--rw-r--r--   0 maurits    (501) staff       (20)      565 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_install.py
--rw-r--r--   0 maurits    (501) staff       (20)     2924 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_richtextdiff.py
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tool.gif
--rw-r--r--   0 maurits    (501) staff       (20)     1114 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.043750 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/zpt/
--rw-r--r--   0 maurits    (501) staff       (20)     3070 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/zpt/editCMFDiffTool.zpt
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.030915 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     9262 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2255 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      199 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      860 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:24:08.044652 Products.CMFDiffTool-4.0.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/docs/CREDITS.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     1038 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2023-03-14 22:24:08.045668 Products.CMFDiffTool-4.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1671 2023-03-14 22:24:07.000000 Products.CMFDiffTool-4.0.0/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.905277 Products.CMFDiffTool-4.0.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1019 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/.editorconfig
+-rw-r--r--   0 gil       (1000) gil       (1000)       97 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/.gitignore
+-rw-r--r--   0 gil       (1000) gil       (1000)      101 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/.isort.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)      128 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/.meta.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      973 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 gil       (1000) gil       (1000)     7724 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      146 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     9371 2023-04-15 09:02:51.905277 Products.CMFDiffTool-4.0.1/PKG-INFO
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.900277 Products.CMFDiffTool-4.0.1/Products/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.902277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4253 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/BaseDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1949 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/BinaryDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1058 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/CMFDTHtmlDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6056 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/CMFDiffTool.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6150 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/ChangeSet.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4118 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/FieldDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6297 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/ListDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3966 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/TextDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1578 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2929 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/choicediff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      141 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     6215 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/dexteritydiff.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.903277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/exportimport/
+-rw-r--r--   0 gil       (1000) gil       (1000)       17 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/exportimport/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      906 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/exportimport/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2864 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/exportimport/difftool.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.903277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/interfaces/
+-rw-r--r--   0 gil       (1000) gil       (1000)      158 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/interfaces/IChangeSet.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4475 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/interfaces/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      236 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/interfaces/portal_diff.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.903277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/libs/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/libs/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8055 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/libs/htmldiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5256 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/namedfile.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.898277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.903277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)      296 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/profiles/default/componentregistry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)       85 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      427 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/profiles.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     3775 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.905277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)      372 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/BaseTestCase.py
+-rw-r--r--   0 gil       (1000) gil       (1000)       43 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    10603 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testChangeSet.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4345 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testDiffTool.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6742 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testFieldDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8190 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testListDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4855 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testTextDiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2224 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_astextdiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4100 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_binarydiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2447 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_choicediff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5260 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_dexteritydiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2724 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_filelistdiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      514 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_install.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2868 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_richtextdiff.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      166 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tool.gif
+-rw-r--r--   0 gil       (1000) gil       (1000)     1115 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.905277 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/zpt/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4187 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/zpt/editCMFDiffTool.zpt
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.901277 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     9371 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2312 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/entry_points.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        9 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      205 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        9 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      860 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:02:51.905277 Products.CMFDiffTool-4.0.1/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)      123 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/docs/CREDITS.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)     1038 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1806 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 09:02:51.906277 Products.CMFDiffTool-4.0.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1623 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1721 2023-04-15 09:02:51.000000 Products.CMFDiffTool-4.0.1/tox.ini
```

### Comparing `Products.CMFDiffTool-4.0.0/CHANGES.rst` & `Products.CMFDiffTool-4.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 4.0.0 (2023-03-14)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility with Plone 5.2, Python 2, Archetypes.
```

### Comparing `Products.CMFDiffTool-4.0.0/PKG-INFO` & `Products.CMFDiffTool-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CMFDiffTool
-Version: 4.0.0
+Version: 4.0.1
 Summary: Diff tool for Plone
 Home-page: https://github.com/plone/Products.CMFDiffTool
 Author: Brent Hendricks
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Diff Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,14 +52,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 4.0.0 (2023-03-14)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility with Plone 5.2, Python 2, Archetypes.
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/BaseDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/BaseDiff.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """CMFDiffTool.py
 
    Calculate differences between content objects
 """
 
 from AccessControl.class_init import InitializeClass
 from Acquisition import aq_base
@@ -16,72 +15,79 @@
 
 import Acquisition
 
 
 @implementer(IDifference)
 class BaseDiff:
     """Basic diff type"""
+
     __allow_access_to_unprotected_subobjects__ = 1
-    meta_type = 'Base Diff'
+    meta_type = "Base Diff"
 
-    def __init__(self, obj1, obj2, field, id1=None, id2=None,
-                 field_name=None, field_label=None, schemata=None):
+    def __init__(
+        self,
+        obj1,
+        obj2,
+        field,
+        id1=None,
+        id2=None,
+        field_name=None,
+        field_label=None,
+        schemata=None,
+    ):
         self.field = field
         self.oldValue = _getValue(obj1, field, field_name)
         self.newValue = _getValue(obj2, field, field_name)
-        self.same = (self.oldValue == self.newValue)
-        if not id1 and safe_hasattr(obj1, 'getId'):
+        self.same = self.oldValue == self.newValue
+        if not id1 and safe_hasattr(obj1, "getId"):
             id1 = obj1.getId()
-        if not id2 and safe_hasattr(obj2, 'getId'):
+        if not id2 and safe_hasattr(obj2, "getId"):
             id2 = obj2.getId()
         self.id1 = id1
         self.id2 = id2
         self.label = field_label or field
-        self.schemata = schemata or 'default'
+        self.schemata = schemata or "default"
         fld1 = _getValue(obj1, field, field_name, convert_to_str=False)
         fld2 = _getValue(obj2, field, field_name, convert_to_str=False)
-        if safe_hasattr(fld1, 'getFilename'):
+        if safe_hasattr(fld1, "getFilename"):
             self.oldFilename = fld1.getFilename()
         else:
             self.oldFilename = None
-        if safe_hasattr(fld2, 'getFilename'):
+        if safe_hasattr(fld2, "getFilename"):
             self.newFilename = fld2.getFilename()
         else:
             self.newFilename = None
-        if self.oldFilename is not None and self.newFilename is not None \
-           and self.same:
-            self.same = (self.oldFilename == self.newFilename)
+        if self.oldFilename is not None and self.newFilename is not None and self.same:
+            self.same = self.oldFilename == self.newFilename
 
     def testChanges(self, ob):
         """Test the specified object to determine if the change set
         will apply without errors"""
         pass
 
     def applyChanges(self, ob):
         """Update the specified object with the difference"""
         pass
 
     def filenameTitle(self, filename):
-        """Translate the filename leading text
-        """
-        msg = _(u'Filename: ${filename}',
-                mapping={'filename': filename})
+        """Translate the filename leading text"""
+        msg = _("Filename: ${filename}", mapping={"filename": filename})
         return translate(msg)
 
 
 def _getValue(ob, field, field_name, convert_to_str=True):
     # Check for the attribute without acquisition.  If it's there,
     # grab it *with* acquisition, so things like ComputedAttribute
     # will work
     if IDexterityContent.providedBy(ob) and field:
         # we need a special handling for subjects because the field is stored
         # as `subject` attribute but the schema name is `subjects`
         # see plone.app.dexterity.behaviors.metadata.ICategorization and
         # plone.dexterity.content.DexterityContent
-        if field == 'subjects':
+        if field == "subjects":
             value = ob.Subject()
         else:
             value = getattr(ob, field, None)
     elif field and safe_hasattr(aq_base(ob), field):
         value = getattr(ob, field)
     else:
         raise AttributeError(field)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/BinaryDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/BinaryDiff.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
 from AccessControl.class_init import InitializeClass
 from os import linesep
 from Products.CMFDiffTool.BaseDiff import _getValue
 from Products.CMFDiffTool.FieldDiff import FieldDiff
 from Products.CMFDiffTool.utils import html_escape
 
 
 class BinaryDiff(FieldDiff):
     """Simple binary difference"""
 
-    meta_type = 'Binary Diff'
+    meta_type = "Binary Diff"
     inlinediff_fmt = """
 <div class="%s">
     <del>%s</del>
     <ins>%s</ins>
 </div>
 """
 
@@ -29,34 +28,38 @@
     def testChanges(self, ob):
         """
         Test the specified object to determine if the change set will
         apply without errors
         """
         value = _getValue(ob, self.field)
         if not self.same and value != self.oldValue:
-            raise ValueError('Conflict Error during merge',
-                             self.field, value, self.oldValue)
+            raise ValueError(
+                "Conflict Error during merge", self.field, value, self.oldValue
+            )
 
     def applyChanges(self, ob):
         """Update the specified object with the difference"""
         # Simplistic update
         self.testChanges(ob)
         if not self.same:
             setattr(ob, self.field, self.newValue)
 
     def inline_diff(self):
         """Simple inline diff that just checks that the filename
         has changed."""
-        css_class = 'FilenameDiff'
+        css_class = "FilenameDiff"
         html = []
         if self.oldFilename != self.newFilename:
             html.append(
-                self.inlinediff_fmt % (css_class,
-                                       self.filenameTitle(html_escape(self.oldFilename)),
-                                       self.filenameTitle(html_escape(self.newFilename))),
+                self.inlinediff_fmt
+                % (
+                    css_class,
+                    self.filenameTitle(html_escape(self.oldFilename)),
+                    self.filenameTitle(html_escape(self.newFilename)),
+                ),
             )
 
         if html:
             return linesep.join(html)
 
 
 InitializeClass(BinaryDiff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/CMFDTHtmlDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/CMFDTHtmlDiff.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# -*- coding: utf-8 -*-
 from AccessControl.class_init import InitializeClass
 from Products.CMFDiffTool.libs import htmldiff
 from Products.CMFDiffTool.TextDiff import TextDiff
 from Products.CMFDiffTool.utils import html_safe
 
 
 # Give it a dumb name so it doesn't conflict with all the other html diffs
 # around.  This uses Ian Bicking's very nice htmldiff.py from Web Ware for
 # Python.
 class CMFDTHtmlDiff(TextDiff):
     """Text difference"""
 
-    meta_type = 'HTML Diff'
+    meta_type = "HTML Diff"
 
     def inline_diff(self):
         """Return a specialized diff for HTML"""
-        a = '\n'.join(self._parseField(self.oldValue,
-                                       filename=self.oldFilename))
-        b = '\n'.join(self._parseField(self.newValue,
-                                       filename=self.newFilename))
+        a = "\n".join(self._parseField(self.oldValue, filename=self.oldFilename))
+        b = "\n".join(self._parseField(self.newValue, filename=self.newFilename))
         return htmldiff.htmldiff(html_safe(a), html_safe(b))
 
     def _parseField(self, value, filename=None):
         """Use the field's raw value if available."""
         if value is None:
-            value = ''
+            value = ""
         else:
-            value = getattr(value, 'raw', value)
+            value = getattr(value, "raw", value)
         return TextDiff._parseField(self, value, filename)
 
 
 InitializeClass(CMFDTHtmlDiff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/CMFDiffTool.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/CMFDiffTool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """CMFDiffTool.py
 
    Calculate differences between content objects
 """
 from AccessControl import ClassSecurityInfo
 from AccessControl.class_init import InitializeClass
 from Acquisition import aq_base
@@ -18,120 +17,119 @@
 from zope.interface import implementer
 
 
 @implementer(IDiffTool)
 class CMFDiffTool(UniqueObject, SimpleItem):
     """ """
 
-    id = 'portal_diff'
-    meta_type = 'CMF Diff Tool'
+    id = "portal_diff"
+    meta_type = "CMF Diff Tool"
 
     security = ClassSecurityInfo()
 
-    manage_options = (({'label': 'Configure', 'action': 'manage_difftypes'},
-                      {'label': 'Overview', 'action': 'manage_overview'},
-                       ) + SimpleItem.manage_options
-                      )
+    manage_options = (
+        {"label": "Configure", "action": "manage_difftypes"},
+        {"label": "Overview", "action": "manage_overview"},
+    ) + SimpleItem.manage_options
 
     #  Internal attributes
     _difftypes = {}
 
     def __init__(self):
         self._pt_diffs = {}
 
-    security.declareProtected(ManagePortal, 'manage_difftypes')  # NOQA
-    manage_difftypes = PageTemplateFile('zpt/editCMFDiffTool', globals())
+    security.declareProtected(ManagePortal, "manage_difftypes")  # NOQA
+    manage_difftypes = PageTemplateFile("zpt/editCMFDiffTool", globals())
 
     def manage_editDiffFields(self, updates, REQUEST=None):
         """Edit the portal type fields"""
 
         # Clear the old values
         del self._pt_diffs
         self._pt_diffs = {}
         for r in updates:
-            if r.get('delete', None):
+            if r.get("delete", None):
                 continue
             self.setDiffField(r.pt_name, r.field, r.diff)
 
         self._p_changed = 1
 
         if REQUEST:
-            return self.manage_difftypes(
-                manage_tabs_message='Diff mappings updated')
+            return self.manage_difftypes(manage_tabs_message="Diff mappings updated")
 
-    security.declareProtected(ManagePortal, 'listDiffTypes')  # NOQA
+    security.declareProtected(ManagePortal, "listDiffTypes")  # NOQA
 
     def manage_addDiffField(self, pt_name, field, diff, REQUEST=None):
         """Add a new diff field from the ZMI"""
         self.setDiffField(pt_name, field, diff)
         if REQUEST:
-            return self.manage_difftypes(manage_tabs_message='Field added')
+            return self.manage_difftypes(manage_tabs_message="Field added")
 
     def setDiffField(self, pt_name, field, diff):
         """
         Set the diff type for 'field' on the portal type 'pt_name' to 'diff'
         """
         if pt_name not in self.portal_types.listContentTypes():
-            raise BadRequest('Error: invalid portal type')
+            raise BadRequest("Error: invalid portal type")
 
         elif not field:
-            raise BadRequest('Error: no field specified')
+            raise BadRequest("Error: no field specified")
 
         elif diff not in self.listDiffTypes():
-            raise BadRequest('Error: invalid diff type')
+            raise BadRequest("Error: invalid diff type")
 
         else:
             self._pt_diffs.setdefault(pt_name, {})[field] = diff
             self._p_changed = 1
 
     #  Interface fulfillment
-    security.declareProtected(ManagePortal, 'listDiffTypes')  # NOQA
+    security.declareProtected(ManagePortal, "listDiffTypes")  # NOQA
 
     def listDiffTypes(self):
         """List the names of the registered difference types"""
         return list(self._difftypes)
 
-    security.declareProtected(ManagePortal, 'getDiffType')  # NOQA
+    security.declareProtected(ManagePortal, "getDiffType")  # NOQA
 
     def getDiffType(self, diff):
         """Return a class corresponding to the specified diff type.
         Instances of the class will implement the IDifference
         interface"""
         return self._difftypes.get(diff, None)
 
-    security.declareProtected(ManagePortal, 'setDiffForPortalType')  # NOQA
+    security.declareProtected(ManagePortal, "setDiffForPortalType")  # NOQA
 
     def setDiffForPortalType(self, pt_name, mapping):
         """Set the difference type(self, s) for the specific portal type
 
         mapping is a dictionary where each key is an attribute or
         method on the given portal type, and the value is the name of
         a difference type."""
         # FIXME: Do some error checking
         self._pt_diffs[pt_name] = mapping.copy()
         self._p_changed = 1
 
-    security.declareProtected(ManagePortal, 'getDiffForPortalType')  # NOQA
+    security.declareProtected(ManagePortal, "getDiffForPortalType")  # NOQA
 
     def getDiffForPortalType(self, pt_name):
         """Returns a dictionary where each key is an attribute or
         method on the given portal type, and the value is the name of
         a difference type."""
         # Return a copy so we don't have to worry about the user changing it
         return self._pt_diffs.get(pt_name, {}).copy()
 
-    security.declarePublic('computeDiff')  # NOQA
+    security.declarePublic("computeDiff")  # NOQA
 
     def computeDiff(self, ob1, ob2, id1=None, id2=None):
         """Compute the differences between two objects and return the
         results as a list.  Each object in the list will implement the
         IDifference interface"""
 
         # Try to get the portal type from obj1 first.  If that fails, use obj2
-        pt_name = ''
+        pt_name = ""
         try:
             pt_name = aq_base(ob1).portal_type
         except AttributeError:
             try:
                 pt_name = aq_base(ob2).portal_type
             except AttributeError:
                 pass
@@ -139,27 +137,27 @@
         diff_map = self._pt_diffs.get(pt_name, {})
 
         diffs = []
         for field, klass_name in diff_map.items():
             klass = self._difftypes[klass_name]
             f_diff = klass(ob1, ob2, field, id1=id1, id2=id2)
             # handle compound diff types
-            if safe_hasattr(f_diff, '__getitem__'):
+            if safe_hasattr(f_diff, "__getitem__"):
                 diffs.extend(f_diff)
             else:
                 diffs.append(f_diff)
         return diffs
 
-    security.declarePublic('createChangeSet')  # NOQA
+    security.declarePublic("createChangeSet")  # NOQA
 
     def createChangeSet(self, ob1, ob2, id1=None, id2=None):
         """Returns a ChangeSet object that represents the differences
         between ob1 and ob2 (ie. ob2 - ob1) ."""
         # FIXME: Pick a better ID
-        cs = BaseChangeSet('Changes').__of__(self)
+        cs = BaseChangeSet("Changes").__of__(self)
         cs.computeDiff(ob1, ob2, id1=id1, id2=id2)
         return aq_base(cs)
 
 
 def registerDiffType(klass):
     """Register a class for computing differences.
 
@@ -175,8 +173,8 @@
     Instances of the class must implement the IDifference
     interface."""
 
     del CMFDiffTool._difftypes[klass.meta_type]
 
 
 InitializeClass(CMFDiffTool)
-registerToolInterface('portal_diff', IDiffTool)
+registerToolInterface("portal_diff", IDiffTool)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/ChangeSet.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/ChangeSet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # ChangeSet.py - Zope object representing the differences between
 # objects
 #
 # Code by Brent Hendricks
 #
 # (C) 2003 Brent Hendricks - licensed under the terms of the
@@ -16,84 +15,82 @@
 from Products.CMFCore.utils import getToolByName
 from Products.CMFDiffTool.interfaces import IChangeSet
 from zope.interface import implementer
 
 import logging
 
 
-logger = logging.getLogger('CMFDiffTool')
+logger = logging.getLogger("CMFDiffTool")
 
 
 @implementer(IChangeSet)
 class BaseChangeSet(Implicit):
     """A ChangeSet represents the set of differences between two objects"""
+
     # This should really not be needed just for same, we should use a method
     __allow_access_to_unprotected_subobjects__ = 1
     security = ClassSecurityInfo()
 
-    def __init__(self, id, title=''):
+    def __init__(self, id, title=""):
         """ChangeSet constructor"""
         self.id = id
         self.title = title
         self._diffs = []
         self._added = []
         self._removed = []
         self.ob1_path = []
         self.ob2_path = []
         self._changesets = {}
         self.recursive = 0
 
-    security.declarePublic('getId')  # NOQA
+    security.declarePublic("getId")  # NOQA
 
     def getId(self):
         """ChangeSet id"""
         return self.id
 
     def __getitem__(self, key):
         return self._changesets[key]
 
     def _isSame(self):
         """Returns true if there are no differences between the two objects"""
         return reduce(lambda x, y: x and y, [d.same for d in self._diffs], 1)
 
-    security.declarePublic('same')  # NOQA
+    security.declarePublic("same")  # NOQA
     same = ComputedAttribute(_isSame)
 
-    security.declarePublic('computeDiff')  # NOQA
+    security.declarePublic("computeDiff")  # NOQA
 
-    def computeDiff(self, ob1, ob2, recursive=1, exclude=None,
-                    id1=None, id2=None):
+    def computeDiff(self, ob1, ob2, recursive=1, exclude=None, id1=None, id2=None):
         """Compute the differences from ob1 to ob2 (ie. ob2 - ob1).
 
         The results can be accessed through getDiffs()"""
 
         if exclude is None:
             exclude = []
 
         # Reset state
         self._diffs = []
         self._added = []
         self._removed = []
         self._changed = []
         self._changesets = {}
 
-        purl = getToolByName(self, 'portal_url', None)
+        purl = getToolByName(self, "portal_url", None)
         if purl is not None:
             try:
                 self.ob1_path = purl.getRelativeContentPath(ob1)
                 self.ob2_path = purl.getRelativeContentPath(ob2)
             except AttributeError:
                 # one or both of the objects may not have a path
                 return
-        diff_tool = getToolByName(self, 'portal_diff')
+        diff_tool = getToolByName(self, "portal_diff")
         self._diffs = diff_tool.computeDiff(ob1, ob2, id1=id1, id2=id2)
 
-        if (recursive and
-                ob1.isPrincipiaFolderish and
-                ob2.isPrincipiaFolderish):
+        if recursive and ob1.isPrincipiaFolderish and ob2.isPrincipiaFolderish:
             self.recursive = 1
             ids1 = set(ob1.objectIds())
             ids2 = set(ob2.objectIds())
             self._changed = ids1.intersection(ids2)
             self._removed = ids1.difference(ids2)
             self._added = ids2.difference(ids1)
 
@@ -116,35 +113,35 @@
             # XXX this is a little strange as self._changed doesn't appear
             # to list changed objects, but rather objects which have been
             # reordered or renamed.
             for id in self._changed:
                 self._addSubSet(id, ob1, ob2, exclude, id1, id2)
 
     def _addSubSet(self, id, ob1, ob2, exclude, id1, id2):
-        cs = BaseChangeSet(id, title='Changes to: %s' % id)
+        cs = BaseChangeSet(id, title="Changes to: %s" % id)
         cs = cs.__of__(self)
         cs.computeDiff(ob1[id], ob2[id], exclude=exclude, id1=id1, id2=id2)
         self._changesets[id] = aq_base(cs)
 
-    security.declarePublic('testChanges')  # NOQA
+    security.declarePublic("testChanges")  # NOQA
 
     def testChanges(self, ob):
         """
         Test the specified object to determine if the change set
         will apply without errors
         """
         for d in self._diffs:
             d.testChanges(ob)
 
         for id in self._changed:
             cs = self[id]
             child = ob[id]
             cs.testChanges(child)
 
-    security.declarePublic('applyChanges')  # NOQA
+    security.declarePublic("applyChanges")  # NOQA
 
     def applyChanges(self, ob):
         """Apply the change set to the specified object"""
         for d in self._diffs:
             d.applyChanges(ob)
 
         if self._removed:
@@ -155,45 +152,45 @@
             ob.manage_clone(child, id)
 
         for id in self._changed:
             cs = self[id]
             child = ob[id]
             cs.applyChanges(child)
 
-    security.declarePublic('getDiffs')  # NOQA
+    security.declarePublic("getDiffs")  # NOQA
 
     def getDiffs(self):
         """
         Returns the list differences between the two objects.
 
         Each difference is a single object implementing
         the IDifference interface
         """
         return self._diffs
 
-    security.declarePublic('getSubDiffs')  # NOQA
+    security.declarePublic("getSubDiffs")  # NOQA
 
     def getSubDiffs(self):
         """If the ChangeSet was computed recursively, returns a list
-           of ChangeSet objects representing subjects differences
+        of ChangeSet objects representing subjects differences
 
-           Each ChangeSet will have the same ID as the objects whose
-           difference it represents.
-           """
+        Each ChangeSet will have the same ID as the objects whose
+        difference it represents.
+        """
         return [self[id] for id in self._changed]
 
-    security.declarePublic('getAddedItems')  # NOQA
+    security.declarePublic("getAddedItems")  # NOQA
 
     def getAddedItems(self):
         """If the ChangeSet was computed recursively, returns the list
         of IDs of items that were added.
 
         A copy of these items is available as a cubject of the ChangeSet
         """
         return list(self._added)
 
-    security.declarePublic('getRemovedItems')  # NOQA
+    security.declarePublic("getRemovedItems")  # NOQA
 
     def getRemovedItems(self):
         """If the ChangeSet was computed recursively, returns the list
         of IDs of items that were removed"""
         return list(self._removed)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/FieldDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/FieldDiff.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import difflib
 
 
 class FieldDiff(BaseDiff):
     """Text difference"""
 
-    meta_type = 'Field Diff'
+    meta_type = "Field Diff"
 
     same_fmt = """<div class="%s">%s</div>"""
     inlinediff_fmt = """<div class="%s">
     <div class="diff_sub">%s</div>
     <div class="diff_add">%s</div>
 </div>"""
 
@@ -37,80 +37,81 @@
     def testChanges(self, ob):
         """
         Test the specified object to determine if the change set
         will apply without errors
         """
         value = _getValue(ob, self.field)
         if not self.same and value != self.oldValue:
-            raise ValueError('Conflict Error during merge',
-                             self.field, value, self.oldValue)
+            raise ValueError(
+                "Conflict Error during merge", self.field, value, self.oldValue
+            )
 
     def applyChanges(self, ob):
         """Update the specified object with the difference"""
         # Simplistic update
         self.testChanges(ob)
         if not self.same:
             setattr(ob, self.field, self.newValue)
 
     def ndiff(self):
         """Return a textual diff"""
         r = []
         a = self._parseField(self.oldValue, filename=self.oldFilename)
         b = self._parseField(self.newValue, filename=self.newFilename)
         for tag, alo, ahi, blo, bhi in self.getLineDiffs():
-            if tag == 'replace':
+            if tag == "replace":
                 plain_replace(a, alo, ahi, b, blo, bhi, r)
-            elif tag == 'delete':
-                dump('-', a, alo, ahi, r)
-            elif tag == 'insert':
-                dump('+', b, blo, bhi, r)
-            elif tag == 'equal':
-                dump(' ', a, alo, ahi, r)
+            elif tag == "delete":
+                dump("-", a, alo, ahi, r)
+            elif tag == "insert":
+                dump("+", b, blo, bhi, r)
+            elif tag == "equal":
+                dump(" ", a, alo, ahi, r)
             else:
-                raise ValueError('unknown tag %r', tag)
-        return '\n'.join(r)
+                raise ValueError("unknown tag %r", tag)
+        return "\n".join(r)
 
     def inline_diff(self):
-        css_class = 'InlineDiff'
+        css_class = "InlineDiff"
         inlinediff_fmt = self.inlinediff_fmt
         same_fmt = self.same_fmt
         r = []
         a = self._parseField(self.oldValue, filename=self.oldFilename)
         b = self._parseField(self.newValue, filename=self.newFilename)
         for tag, alo, ahi, blo, bhi in self.getLineDiffs():
-            if tag == 'replace':
+            if tag == "replace":
                 for i in range(alo, ahi):
-                    r.append(inlinediff_fmt % (css_class, html_escape(a[i]), ''))
+                    r.append(inlinediff_fmt % (css_class, html_escape(a[i]), ""))
                 for i in range(blo, bhi):
-                    r.append(inlinediff_fmt % (css_class, '', html_escape(b[i])))
-            elif tag == 'delete':
+                    r.append(inlinediff_fmt % (css_class, "", html_escape(b[i])))
+            elif tag == "delete":
                 for i in range(alo, ahi):
-                    r.append(inlinediff_fmt % (css_class, html_escape(a[i]), ''))
-            elif tag == 'insert':
+                    r.append(inlinediff_fmt % (css_class, html_escape(a[i]), ""))
+            elif tag == "insert":
                 for i in range(blo, bhi):
-                    r.append(inlinediff_fmt % (css_class, '', html_escape(b[i])))
-            elif tag == 'equal':
+                    r.append(inlinediff_fmt % (css_class, "", html_escape(b[i])))
+            elif tag == "equal":
                 for i in range(alo, ahi):
                     r.append(same_fmt % (css_class, html_escape(a[i])))
             else:
                 raise ValueError('unknown tag "%s"' % tag)
-        return '\n'.join(r)
+        return "\n".join(r)
 
 
 InitializeClass(FieldDiff)
 
 
 def dump(tag, x, lo, hi, r):
     for i in range(lo, hi):
-        r.append(tag + ' %s' % x[i])
+        r.append(tag + " %s" % x[i])
 
 
 def plain_replace(a, alo, ahi, b, blo, bhi, r):
     assert alo < ahi and blo < bhi
     # dump the shorter block first -- reduces the burden on short-term
     # memory if the blocks are of very different sizes
     if bhi - blo < ahi - alo:
-        dump('+', b, blo, bhi, r)
-        dump('-', a, alo, ahi, r)
+        dump("+", b, blo, bhi, r)
+        dump("-", a, alo, ahi, r)
     else:
-        dump('-', a, alo, ahi, r)
-        dump('+', b, blo, bhi, r)
+        dump("-", a, alo, ahi, r)
+        dump("+", b, blo, bhi, r)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/ListDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/ListDiff.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,44 +5,53 @@
 from Products.CMFDiffTool.FieldDiff import FieldDiff
 from Products.CMFDiffTool.utils import html_escape
 
 
 class ListDiff(FieldDiff):
     """Text difference"""
 
-    meta_type = 'List Diff'
+    meta_type = "List Diff"
 
-    def __init__(self, obj1, obj2, field, id1=None, id2=None, field_name=None,
-                 field_label=None, schemata=None):
-        FieldDiff.__init__(self, obj1, obj2, field, id1, id2, field_name,
-                           field_label, schemata)
+    def __init__(
+        self,
+        obj1,
+        obj2,
+        field,
+        id1=None,
+        id2=None,
+        field_name=None,
+        field_label=None,
+        schemata=None,
+    ):
+        FieldDiff.__init__(
+            self, obj1, obj2, field, id1, id2, field_name, field_label, schemata
+        )
         self._vocabulary = None
 
         # Tries to find a vocabulary. First we need to find an object and
         # the field instance.
         obj = obj1 if (obj1 is not None) else obj2
         field_name = field_name or field
         if obj and field_name and IDexterityContent.providedBy(obj):
             field_instance = get_field_object(obj, field_name)
             if field_instance is not None:
                 # Binding the field to an object will construct the vocabulary
                 # using a factory if necessary.
                 try:
-                    self._vocabulary = field_instance.value_type.bind(obj).\
-                        vocabulary
+                    self._vocabulary = field_instance.value_type.bind(obj).vocabulary
                 except Exception:
                     pass
 
     def chk_hashable(self, value):
         if self._vocabulary is not None:
             value = title_or_value(self._vocabulary, value)
         try:
             hash(value)
         except TypeError as e:
-            value = repr(e) + ': ' + repr(value)
+            value = repr(e) + ": " + repr(value)
         return value
 
     def _parseField(self, value, filename=None):
         """Parse a field value in preparation for diffing"""
         if type(value) is list or type(value) is tuple:
             values = []
             for v in value:
@@ -52,107 +61,110 @@
             if type(value) is set:
                 return list(value)
             else:
                 return [self.chk_hashable(value)]
 
 
 class RelationListDiff(FieldDiff):
-
-    meta_type = 'Related List Diff'
+    meta_type = "Related List Diff"
 
     same_fmt = """<div class="%s"><a target="_blank" href="%s">%s</a></div>"""
     inlinediff_fmt = """<div class="%s">
         <div class="%s"><a target="_blank" href="%s">%s</a></div>
     </div>"""
 
     def _parseField(self, value, filename=None):
-        """ Take RelationValues and just return the target UID
-            so we can compare """
+        """Take RelationValues and just return the target UID
+        so we can compare"""
 
         if filename is None:
             # Since we only want to compare a single field, make a
             # one-item list out of it
-            return ['/'.join(val.getPhysicalPath()) for val in value]
+            return ["/".join(val.getPhysicalPath()) for val in value]
         else:
             return [
                 self.filenameTitle(filename),
-                ['/'.join(val.getPhysicalPath()) for val in value],
+                ["/".join(val.getPhysicalPath()) for val in value],
             ]
 
     def inline_diff(self):
-        css_class = 'InlineDiff'
+        css_class = "InlineDiff"
         inlinediff_fmt = self.inlinediff_fmt
         same_fmt = self.same_fmt
         r = []
         for tag, alo, ahi, blo, bhi in self.getLineDiffs():
-            if tag == 'replace':
+            if tag == "replace":
                 for i in range(alo, ahi):
                     obj = self.oldValue[i]
                     obj_title = html_escape(obj.Title())
                     obj_url = obj.absolute_url()
-                    r.append(inlinediff_fmt %
-                             (css_class, 'diff_sub', obj_url, obj_title))
+                    r.append(
+                        inlinediff_fmt % (css_class, "diff_sub", obj_url, obj_title)
+                    )
                 for i in range(blo, bhi):
                     obj = self.newValue[i]
                     obj_title = html_escape(obj.Title())
                     obj_url = obj.absolute_url()
-                    r.append(inlinediff_fmt %
-                             (css_class, 'diff_add', obj_url, obj_title))
-            elif tag == 'delete':
+                    r.append(
+                        inlinediff_fmt % (css_class, "diff_add", obj_url, obj_title)
+                    )
+            elif tag == "delete":
                 for i in range(alo, ahi):
                     obj = self.oldValue[i]
                     obj_title = html_escape(obj.Title())
                     obj_url = obj.absolute_url()
-                    r.append(inlinediff_fmt %
-                             (css_class, 'diff_sub', obj_url, obj_title))
-            elif tag == 'insert':
+                    r.append(
+                        inlinediff_fmt % (css_class, "diff_sub", obj_url, obj_title)
+                    )
+            elif tag == "insert":
                 for i in range(blo, bhi):
                     obj = self.newValue[i]
                     obj_title = html_escape(obj.Title())
                     obj_url = obj.absolute_url()
-                    r.append(inlinediff_fmt %
-                             (css_class, 'diff_add', obj_url, obj_title))
-            elif tag == 'equal':
+                    r.append(
+                        inlinediff_fmt % (css_class, "diff_add", obj_url, obj_title)
+                    )
+            elif tag == "equal":
                 for i in range(alo, ahi):
                     obj = self.oldValue[i]
                     obj_title = html_escape(obj.Title())
                     obj_url = obj.absolute_url()
                     r.append(same_fmt % (css_class, obj_url, obj_title))
             else:
-                raise ValueError('unknown tag %s' % tag)
-        return '\n'.join(r)
+                raise ValueError("unknown tag %s" % tag)
+        return "\n".join(r)
 
     def ndiff(self):
-        """ Return a textual diff """
+        """Return a textual diff"""
         r = []
         for tag, alo, ahi, blo, bhi in self.getLineDiffs():
-            if tag == 'replace':
+            if tag == "replace":
                 for i in range(alo, ahi):
                     obj = self.oldValue[i]
                     obj_url = obj.absolute_url()
-                    r.append('- %s' % obj_url)
+                    r.append("- %s" % obj_url)
                 for i in range(blo, bhi):
                     obj = self.newValue[i]
                     obj_url = obj.absolute_url()
-                    r.append('+ %s' % obj_url)
-            elif tag == 'delete':
+                    r.append("+ %s" % obj_url)
+            elif tag == "delete":
                 for i in range(alo, ahi):
                     obj = self.oldValue[i]
                     obj_url = obj.absolute_url()
-                    r.append('- %s' % obj_url)
-            elif tag == 'insert':
+                    r.append("- %s" % obj_url)
+            elif tag == "insert":
                 for i in range(blo, bhi):
                     obj = self.newValue[i]
                     obj_url = obj.absolute_url()
-                    r.append('+ %s' % obj_url)
-            elif tag == 'equal':
+                    r.append("+ %s" % obj_url)
+            elif tag == "equal":
                 for i in range(alo, ahi):
                     obj = self.oldValue[i]
                     obj_url = obj.absolute_url()
-                    r.append('  %s' % obj_url)
+                    r.append("  %s" % obj_url)
             else:
-                raise ValueError('unknown tag %r', tag)
-        return '\n'.join(r)
+                raise ValueError("unknown tag %r", tag)
+        return "\n".join(r)
 
 
 InitializeClass(ListDiff)
 InitializeClass(RelationListDiff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/TextDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/TextDiff.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 import difflib
 
 
 class TextDiff(FieldDiff):
     """Text difference"""
 
-    meta_type = 'Lines Diff'
+    meta_type = "Lines Diff"
     inlinediff_fmt = """
 <div class="%s">
     <del>%s</del>
     <ins>%s</ins>
 </div>
 """
 
     def _parseField(self, value, filename=None):
         """Parse a field value in preparation for diffing"""
         if value is None:
-            value = ''
+            value = ""
         if filename is None:
             # Split the text into a list for diffs
             return value.splitlines()
         else:
             return [self.filenameTitle(filename)] + value.splitlines()
 
     def unified_diff(self):
@@ -41,50 +41,53 @@
         cleanargs = [i for i in cleanargs if i]
         return linesep.join(difflib.unified_diff(*cleanargs))
 
     def html_diff(self, context=True, wrapcolumn=40):
         """Return an HTML table showing differences"""
         # difflib is not Unicode-aware, so we need to force everything to
         # utf-8 manually
-        a = [safe_unicode(i) for i in
-             self._parseField(self.oldValue, filename=self.oldFilename)]
-        b = [safe_unicode(i) for i in
-             self._parseField(self.newValue, filename=self.newFilename)]
+        a = [
+            safe_unicode(i)
+            for i in self._parseField(self.oldValue, filename=self.oldFilename)
+        ]
+        b = [
+            safe_unicode(i)
+            for i in self._parseField(self.newValue, filename=self.newFilename)
+        ]
         vis_diff = difflib.HtmlDiff(wrapcolumn=wrapcolumn)
         diff = vis_diff.make_table(
-            a,
-            b,
-            safe_unicode(self.id1),
-            safe_unicode(self.id2),
-            context=context)
+            a, b, safe_unicode(self.id1), safe_unicode(self.id2), context=context
+        )
         return diff
 
     def inline_diff(self):
         """Simple inline diff that just assumes that either the filename
         has changed, or the text has been completely replaced."""
-        css_class = 'InlineDiff'
-        old_attr = self._parseField(self.oldValue,
-                                    filename=self.oldFilename)
-        new_attr = self._parseField(self.newValue,
-                                    filename=self.newFilename)
+        css_class = "InlineDiff"
+        old_attr = self._parseField(self.oldValue, filename=self.oldFilename)
+        new_attr = self._parseField(self.newValue, filename=self.newFilename)
         if old_attr:
             old_fname = old_attr.pop(0)
         else:
             old_fname = None
         if new_attr:
             new_fname = new_attr.pop(0)
         else:
             new_fname = None
         a = linesep.join(old_attr or [])
         b = linesep.join(new_attr or [])
         html = []
         if old_fname != new_fname:
             html.append(
-                self.inlinediff_fmt % ('%s FilenameDiff' % css_class,
-                                       html_escape(old_fname), html_escape(new_fname)),
+                self.inlinediff_fmt
+                % (
+                    "%s FilenameDiff" % css_class,
+                    html_escape(old_fname),
+                    html_escape(new_fname),
+                ),
             )
         if a != b:
             html.append(
                 self.inlinediff_fmt % (css_class, html_escape(a), html_escape(b)),
             )
         if html:
             return linesep.join(html)
@@ -98,19 +101,19 @@
     Specialization of `TextDiff` that converts any value to text in order to
     provide an inline diff visualization. Also translated (i18n) the
     strings `True` and `False`.
     """
 
     def _parseField(self, value, filename=None):
         if value is None:
-            value = ''
+            value = ""
 
         # In tests translation is not available, so we account for this
         # case here.
-        translate = getattr(getSite(), 'translate', None)
+        translate = getattr(getSite(), "translate", None)
         if translate is not None:
             value = translate(_(value))
 
         return TextDiff._parseField(self, safe_unicode(value), filename)
 
 
 InitializeClass(AsTextDiff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/__init__.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 """Initialize CMFDiffTool Product"""
 # Set up a MessageFactory for the cmfdifftool domain
 from zope.i18nmessageid import MessageFactory
 
 
-CMFDiffToolMessageFactory = MessageFactory('plone')
+CMFDiffToolMessageFactory = MessageFactory("plone")
 
 from Products.CMFCore.utils import ToolInit  # NOQA
 from Products.CMFDiffTool import BinaryDiff  # NOQA
 from Products.CMFDiffTool import CMFDiffTool  # NOQA
 from Products.CMFDiffTool import CMFDTHtmlDiff  # NOQA
 from Products.CMFDiffTool import FieldDiff  # NOQA
 from Products.CMFDiffTool import ListDiff  # NOQA
@@ -37,15 +36,16 @@
     from Products.CMFDiffTool import dexteritydiff
 except ImportError:
     pass
 else:
     CMFDiffTool.registerDiffType(choicediff.ChoiceDiff)
     CMFDiffTool.registerDiffType(dexteritydiff.DexterityCompoundDiff)
 
-tools = (CMFDiffTool.CMFDiffTool, )
+tools = (CMFDiffTool.CMFDiffTool,)
 
 
 def initialize(context):
-    ToolInit('CMF Diff Tool',
-             tools=tools,
-             icon='tool.gif',
-             ).initialize(context)
+    ToolInit(
+        "CMF Diff Tool",
+        tools=tools,
+        icon="tool.gif",
+    ).initialize(context)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/choicediff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/choicediff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from AccessControl.class_init import InitializeClass
 from plone.dexterity.interfaces import IDexterityFTI
 from plone.dexterity.utils import getAdditionalSchemata
 from Products.CMFDiffTool.TextDiff import AsTextDiff
 from zope.component import getUtility
 
 
@@ -48,37 +47,46 @@
 
     It's implemented as an specialization of `AsTextDiff`. The difference is
     that this class tries to obtain the title corresponding to the value from
     the vocabulary associated with the field in order to provide an
     user-friendlier inline diff to the user.
     """
 
-    def __init__(self, obj1, obj2, field, id1=None, id2=None, field_name=None,
-                 field_label=None, schemata=None):
-        AsTextDiff.__init__(self, obj1, obj2, field, id1, id2, field_name,
-                            field_label, schemata)
+    def __init__(
+        self,
+        obj1,
+        obj2,
+        field,
+        id1=None,
+        id2=None,
+        field_name=None,
+        field_label=None,
+        schemata=None,
+    ):
+        AsTextDiff.__init__(
+            self, obj1, obj2, field, id1, id2, field_name, field_label, schemata
+        )
         self._vocabulary = None
 
         # Tries to find a vocabulary. First we need to find an object and
         # the field instance.
         obj = obj1 if (obj1 is not None) else obj2
         field_name = field_name or field
         field_instance = (
-            get_field_object(obj, field_name) if (obj and field_name)
-            else None
+            get_field_object(obj, field_name) if (obj and field_name) else None
         )
 
         if field_instance is not None:
             # Binding the field to an object will construct the vocabulary
             # using a factory if necessary.
             self._vocabulary = field_instance.bind(obj).vocabulary
 
     def _parseField(self, value, filename=None):
         if value is None:
-            value = ''
+            value = ""
         elif self._vocabulary is not None:
             value = title_or_value(self._vocabulary, value)
 
         return AsTextDiff._parseField(self, value, filename)
 
 
 InitializeClass(ChoiceDiff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/dexteritydiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/dexteritydiff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.textfield import RichText
 from plone.dexterity.browser.edit import DefaultEditForm
 from Products.CMFDiffTool.choicediff import ChoiceDiff
 from Products.CMFDiffTool.CMFDTHtmlDiff import CMFDTHtmlDiff
 from Products.CMFDiffTool.FieldDiff import FieldDiff
 from Products.CMFDiffTool.ListDiff import ListDiff
 from Products.CMFDiffTool.ListDiff import RelationListDiff
@@ -27,18 +26,18 @@
 # TODO: Perhaps this can be replaced with some kind of Zope 3 style
 # adaptation, in order to provide better extensibility.
 FIELDS_AND_DIFF_TYPES_RELATION = [
     (FILE_FIELD_TYPES, NamedFileBinaryDiff),
     ((RelationList,), RelationListDiff),
     ((Iterable, Container), ListDiff),
     ((Date, Datetime, Time), AsTextDiff),
-    ((Bool, ), AsTextDiff),
-    ((Choice, ), ChoiceDiff),
+    ((Bool,), AsTextDiff),
+    ((Choice,), ChoiceDiff),
     ((Text, Bytes), TextDiff),
-    ((RichText, ), CMFDTHtmlDiff),
+    ((RichText,), CMFDTHtmlDiff),
 ]
 
 """
 Relates field types (`zope.schema.Field` subclasses) and "diff types"
 (`Products.CMFEditions.BaseDiff.BaseDiff` subclasses).
 
 To find the best diff type for a field type this list will be searched until
@@ -60,22 +59,22 @@
 When a field is detected to be a list-like field we use this list in the same
 fashion as `FIELDS_AND_DIFF_TYPES_RELATION` to try to find the best "diff type
 " according to the "value type" of the field, i.e the type of the elements in
 the list. If a match is not found then a fall back is used.
 """
 
 # TODO: provide an easier way to exclude fields.
-EXCLUDED_FIELDS = ('modification_date', 'IVersionable.changeNote')
+EXCLUDED_FIELDS = ("modification_date", "IVersionable.changeNote")
 """Names of fields not to compare."""
 
 
-class DexterityCompoundDiff(object):
+class DexterityCompoundDiff:
     """text difference for Dexterity"""
 
-    meta_type = 'Compound Diff for Dexterity types'
+    meta_type = "Compound Diff for Dexterity types"
 
     def __init__(self, obj1, obj2, field, id1=None, id2=None):
         self.id1 = id1 or obj1.getId()
         self.id2 = id2 or obj2.getId()
         self.obj1 = obj1
         self._diffs = self._diff(obj1, obj2)
 
@@ -94,16 +93,17 @@
 
         Return: a sequence of `IDifference` objects.
         """
 
         diffs = []
         for field, field_name in self._compute_fields_order(obj1):
             if field_name not in EXCLUDED_FIELDS:
-                schema_name = '.' in field_name and \
-                    field_name.split('.')[0] or 'default'
+                schema_name = (
+                    "." in field_name and field_name.split(".")[0] or "default"
+                )
                 diffs.append(self._diff_field(obj1, obj2, field, schema_name))
 
         return diffs
 
     def _diff_field(self, obj1, obj2, field, schema_name):
         """
         Compute the differences between 2 objects in respect to the given
@@ -124,22 +124,22 @@
         )
 
     def _get_diff_type(self, field):
         """
         Return a subclass of `Products.CMFEditions.BaseDiff.BaseDiff` suitable
         for the given `zope.schema.Field` instance.
         """
-        diff_type = self._compute_diff_type(
-            field, FIELDS_AND_DIFF_TYPES_RELATION)
+        diff_type = self._compute_diff_type(field, FIELDS_AND_DIFF_TYPES_RELATION)
 
         if diff_type is ListDiff:
             return (
                 self._compute_diff_type(
-                    field.value_type, VALUE_TYPES_AND_DIFF_TYPES_RELATION) or
-                diff_type
+                    field.value_type, VALUE_TYPES_AND_DIFF_TYPES_RELATION
+                )
+                or diff_type
             )
 
         return diff_type or FALL_BACK_DIFF_TYPE
 
     def _compute_diff_type(self, field, relation):
         """
         Return the best "diff type" (subclass of
@@ -151,15 +151,15 @@
         field -- `zope.schema.Field` instance.
         relation -- Sequence of tuples (field_types, diff_type) where
             field_types is a tuple of `zope.schema.Field` subclasses
             and diff_type is a `Products.CMFEditions.BaseDiff.BaseDiff`
             subclass.
         """
 
-        for (field_types, diff_type) in relation:
+        for field_types, diff_type in relation:
             if isinstance(field, field_types):
                 return diff_type
 
         return None
 
     def _compute_fields_order(self, obj):
         """
@@ -170,11 +170,12 @@
         form = DefaultEditForm(obj, getRequest())
         form.portal_type = obj.portal_type
         form.updateFields()
         all_fields = list()
         all_fields += [(form.fields[name].field, name) for name in form.fields]
         if form.groups:
             for group in form.groups:
-                all_fields += [(group.fields[name].field, name)
-                               for name in group.fields]
+                all_fields += [
+                    (group.fields[name].field, name) for name in group.fields
+                ]
 
         return all_fields
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/exportimport/configure.zcml` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/exportimport/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 <configure
-   xmlns="http://namespaces.zope.org/zope"
-   xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-   i18n_domain="cmf"
-   >
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    i18n_domain="cmf"
+    >
 
   <genericsetup:importStep
       name="difftool"
-      handler="Products.CMFDiffTool.exportimport.difftool.importDiffTool"
       title="Diff Tool"
-      description="Import CMFDiffTool settings">
+      description="Import CMFDiffTool settings"
+      handler="Products.CMFDiffTool.exportimport.difftool.importDiffTool"
+      >
     <depends name="toolset" />
     <depends name="componentregistry" />
   </genericsetup:importStep>
 
   <genericsetup:exportStep
       name="difftool"
-      handler="Products.CMFDiffTool.exportimport.difftool.exportDiffTool"
       title="Diff Tool"
-      description="Export CMFDiffTool settings"/>
+      description="Export CMFDiffTool settings"
+      handler="Products.CMFDiffTool.exportimport.difftool.exportDiffTool"
+      />
 
   <adapter
-     factory=".difftool.DiffToolXMLAdapter"
-     provides="Products.GenericSetup.interfaces.IBody"
-     for="Products.CMFDiffTool.interfaces.IDiffTool
-          Products.GenericSetup.interfaces.ISetupEnviron"
-     />
+      factory=".difftool.DiffToolXMLAdapter"
+      provides="Products.GenericSetup.interfaces.IBody"
+      for="Products.CMFDiffTool.interfaces.IDiffTool
+           Products.GenericSetup.interfaces.ISetupEnviron"
+      />
 
 </configure>
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/interfaces/__init__.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/interfaces/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 # Interface definitions
 from zope.interface import Attribute
 from zope.interface import Interface
 
 
 class IDiffTool(Interface):
     """An interface to compute object differences via pluggable
-       difference engine"""
+    difference engine"""
 
-    id = Attribute('id', 'Must be set to "portal_diff"')
+    id = Attribute("id", 'Must be set to "portal_diff"')
 
     def listDiffTypes():
         """List the names of the available difference types"""
 
     def setDiffForPortalType(pt_name, mapping):
         """Set the difference type(s) for the specific portal type
 
@@ -37,38 +36,41 @@
         between ob1 and ob2 (ie. ob2 - ob1) ."""
 
 
 class IDifference(Interface):
     """An interface for interacting with the difference between two
     objects"""
 
-    meta_type = Attribute('title', 'A human readable name for the diff type')
-    field = Attribute('field', 'The name of the field being compared')
-    same = Attribute('same',
-                     'True if the fields are the "same" '
-                     '(whatever that means for this difference)')
-    oldValue = Attribute('oldValue', 'The old field value being compared')
-    newValue = Attribute('newValue', 'The new field value being compared')
-    oldFilename = Attribute('oldFilename',
-                            'The old filename for the field being compared')
-    newFilename = Attribute('newFilename',
-                            'The new filename for the field being compared')
+    meta_type = Attribute("title", "A human readable name for the diff type")
+    field = Attribute("field", "The name of the field being compared")
+    same = Attribute(
+        "same",
+        'True if the fields are the "same" '
+        "(whatever that means for this difference)",
+    )
+    oldValue = Attribute("oldValue", "The old field value being compared")
+    newValue = Attribute("newValue", "The new field value being compared")
+    oldFilename = Attribute(
+        "oldFilename", "The old filename for the field being compared"
+    )
+    newFilename = Attribute(
+        "newFilename", "The new filename for the field being compared"
+    )
 
     def testChanges(ob):
         """Test the specified object to determine if the change set will apply cleanly.
 
-        Returns None if there would be no erros
+        Returns None if there would be no errors
         """
 
     def applyChanges(ob):
         """Update the specified object with the difference"""
 
     def filenameTitle(self, filename):
-        """Translate the filename leading text
-        """
+        """Translate the filename leading text"""
 
 
 class IStringDifference(IDifference):
     """An anterface for interacting with the difference between two
     string (text) objects"""
 
     def getLineDiffs():
@@ -80,47 +82,47 @@
 
         The interpretation of these tuples depends on the difference class"""
 
 
 class IChangeSet(Interface):
     """And interface representing all of the differences between two objects"""
 
-    same = Attribute('same', 'True if the fields are the "same"')
+    same = Attribute("same", 'True if the fields are the "same"')
 
     def computeDiff(ob1, ob2, recursive=1, exclude=None):
         """Compute the differences from ob1 to ob2 (ie. ob2 - ob1).
 
-        If resursive is 1, compute differences between subobjects of
+        If recursive is 1, compute differences between subobjects of
         ob1 and ob2 as well, excluding any subobjects whose IDs are
         listed in exclude
 
         The results can be accessed through getDiffs()"""
 
     def testChanges(ob):
         """Test the specified object to determine if the change set will apply cleanly.
 
-        Returns None if there would be no erros
+        Returns None if there would be no errors
         """
 
     def applyChanges(ob):
         """Apply the computed changes to the specified object"""
 
     def getDiffs():
         """Returns the list of differences between the two objects.
 
         Each difference is a single object implementing the
         IDifference interface"""
 
     def getSubDiffs():
         """If the ChangeSet was computed recursively, returns a list
-           of ChangeSet objects representing subobject differences
+        of ChangeSet objects representing subobject differences
 
-           Each ChangeSet will have the same ID as the objects whose
-           difference it represents.
-           """
+        Each ChangeSet will have the same ID as the objects whose
+        difference it represents.
+        """
 
     def getAddedItems():
         """If the ChangeSet was computed recursively, returns the list
         of IDs of items that were added.
 
         A copy of these items is available as a cubject of the ChangeSet
         """
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/libs/htmldiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/libs/htmldiff.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,21 +17,20 @@
 import re
 
 
 def htmlEncode(s, esc=escape):
     return esc(s, 1)
 
 
-commentRE = re.compile(r'<!--.*?-->', re.S)
-tagRE = re.compile(r'<.*?>', re.S)
-headRE = re.compile(r'<\s*head\s*>', re.S | re.I)
+commentRE = re.compile(r"<!--.*?-->", re.S)
+tagRE = re.compile(r"<.*?>", re.S)
+headRE = re.compile(r"<\s*head\s*>", re.S | re.I)
 
 
 class HTMLMatcher(SequenceMatcher):
-
     def __init__(self, source1, source2):
         SequenceMatcher.__init__(self, None, source1, source2)
 
     def set_seq1(self, a):
         SequenceMatcher.set_seq1(self, self.splitHTML(a))
 
     def set_seq2(self, b):
@@ -41,134 +40,133 @@
         result = []
         pos = 0
         while 1:
             match = tagRE.search(t, pos=pos)
             if not match:
                 result.append(t[pos:])
                 break
-            result.append(t[pos:match.start()])
+            result.append(t[pos : match.start()])
             result.append(match.group(0))
             pos = match.end()
         return result
 
     def splitWords(self, t):
         return t.strip().split()
 
     def splitHTML(self, t):
-        t = commentRE.sub('', t)
+        t = commentRE.sub("", t)
         r = self.splitTags(t)
         result = []
         for item in r:
-            if item.startswith('<'):
+            if item.startswith("<"):
                 result.append(item)
             else:
                 result.extend(self.splitWords(item))
         return result
 
     def htmlDiff(self, addStylesheet=False):
         opcodes = self.get_opcodes()
         a = self.a
         b = self.b
         out = StringIO()
         #  print [o[0] for o in opcodes]
         for tag, i1, i2, j1, j2 in opcodes:
-            if tag == 'equal':
+            if tag == "equal":
                 for item in a[i1:i2]:
                     out.write(item)
-                    out.write(' ')
-            if tag == 'delete' or tag == 'replace':
+                    out.write(" ")
+            if tag == "delete" or tag == "replace":
                 self.textDelete(a[i1:i2], out)
-            if tag == 'insert' or tag == 'replace':
+            if tag == "insert" or tag == "replace":
                 self.textInsert(b[j1:j2], out)
         html = out.getvalue()
         out.close()
         if addStylesheet:
             html = self.addStylesheet(html, self.stylesheet())
         return html
 
     def textDelete(self, lst, out):
         inSpan = False
         for item in lst:
-            if item.startswith('<'):
+            if item.startswith("<"):
                 if inSpan:
                     out.write(self.endDeleteText())
                     inSpan = False
                 out.write(self.formatDeleteTag(item))
             else:
                 if not inSpan:
                     out.write(self.startDeleteText())
                     inSpan = True
                 out.write(item)
-                out.write(' ')
+                out.write(" ")
         if inSpan:
             out.write(self.endDeleteText())
 
     def textInsert(self, lst, out):
         inSpan = False
         for item in lst:
-            if item.startswith('<'):
+            if item.startswith("<"):
                 if inSpan:
                     out.write(self.endInsertText())
                     inSpan = False
                 out.write(self.formatInsertTag(item))
                 out.write(item)
-                out.write(' ')
+                out.write(" ")
             else:
                 if not inSpan:
                     out.write(self.startInsertText())
                     inSpan = True
                 out.write(item)
-                out.write(' ')
+                out.write(" ")
         if inSpan:
             out.write(self.endInsertText())
 
     def stylesheet(self):
-        return '''
+        return """
 .insert { background-color: #aaffaa }
 .delete { background-color: #ff8888 }
 .tagInsert { background-color: #007700; color: #ffffff }
 .tagDelete { background-color: #770000; color: #ffffff }
-'''
+"""
 
     def addStylesheet(self, html, ss):
         match = headRE.search(html)
         if match:
             pos = match.end()
         else:
             pos = 0
-        return ('{0}<style type="text/css"><!--\n{1}\n--></style>{2}'.format(
-            html[:pos], ss, html[pos:]))
+        return '{}<style type="text/css"><!--\n{}\n--></style>{}'.format(
+            html[:pos], ss, html[pos:]
+        )
 
     def startInsertText(self):
         return '<span class="insert">'
 
     def endInsertText(self):
-        return '</span> '
+        return "</span> "
 
     def startDeleteText(self):
         return '<span class="delete">'
 
     def endDeleteText(self):
-        return '</span> '
+        return "</span> "
 
     def formatInsertTag(self, tag):
-        return ('<span class="tagInsert">insert: <tt>%s</tt></span> ' %
-                htmlEncode(tag))
+        return '<span class="tagInsert">insert: <tt>%s</tt></span> ' % htmlEncode(tag)
 
     def formatDeleteTag(self, tag):
-        return ('<span class="tagDelete">delete: <tt>%s</tt></span> ' %
-                htmlEncode(tag))
+        return '<span class="tagDelete">delete: <tt>%s</tt></span> ' % htmlEncode(tag)
 
 
 class NoTagHTMLMatcher(HTMLMatcher):
     def formatInsertTag(self, tag):
-        return ''
+        return ""
 
     def formatDeleteTag(self, tag):
-        return ''
+        return ""
 
 
 def htmldiff(source1, source2, addStylesheet=False):
     """
     Return the difference between two pieces of HTML
 
         >>> htmldiff('test1', 'test2')
@@ -190,30 +188,30 @@
 
 class SimpleHTMLMatcher(HTMLMatcher):
     """
     Like HTMLMatcher, but returns a simpler diff
     """
 
     def startInsertText(self):
-        return '+['
+        return "+["
 
     def endInsertText(self):
-        return ']'
+        return "]"
 
     def startDeleteText(self):
-        return '-['
+        return "-["
 
     def endDeleteText(self):
-        return ']'
+        return "]"
 
     def formatInsertTag(self, tag):
-        return '+[%s]' % tag
+        return "+[%s]" % tag
 
     def formatDeleteTag(self, tag):
-        return '-[%s]' % tag
+        return "-[%s]" % tag
 
 
 def simplehtmldiff(source1, source2):
     """
     Simpler form of htmldiff; mostly for testing, like:
 
         >>> simplehtmldiff('test1', 'test2')
@@ -222,56 +220,57 @@
         '-[<b>]+[<i>]<i> Hello -[world! ]-[</b>]+[you! ]+[</i>]</i> '
     """
     h = SimpleHTMLMatcher(source1, source2)
     return h.htmlDiff()
 
 
 class TextMatcher(HTMLMatcher):
-
     def set_seq1(self, a):
-        SequenceMatcher.set_seq1(self, a.split('\n'))
+        SequenceMatcher.set_seq1(self, a.split("\n"))
 
     def set_seq2(self, b):
-        SequenceMatcher.set_seq2(self, b.split('\n'))
+        SequenceMatcher.set_seq2(self, b.split("\n"))
 
     def htmlDiff(self, addStylesheet=False):
         opcodes = self.get_opcodes()
         a = self.a
         b = self.b
         out = StringIO()
         for tag, i1, i2, j1, j2 in opcodes:
-            if tag == 'equal':
+            if tag == "equal":
                 self.writeLines(a[i1:i2], out)
-            if tag == 'delete' or tag == 'replace':
+            if tag == "delete" or tag == "replace":
                 out.write(self.startDeleteText())
                 self.writeLines(a[i1:i2], out)
                 out.write(self.endDeleteText())
-            if tag == 'insert' or tag == 'replace':
+            if tag == "insert" or tag == "replace":
                 out.write(self.startInsertText())
                 self.writeLines(b[j1:j2], out)
                 out.write(self.endInsertText())
         html = out.getvalue()
         out.close()
         if addStylesheet:
             html = self.addStylesheet(html, self.stylesheet())
         return html
 
     def writeLines(self, lines, out):
         for line in lines:
             line = htmlEncode(line)
-            line = line.replace('  ', '&nbsp; ')
-            line = line.replace('\t', '&nbsp; &nbsp; &nbsp; &nbsp; ')
-            if line.startswith(' '):
-                line = '&nbsp;' + line[1:]
-            out.write('<tt>%s</tt><br>\n' % line)
+            line = line.replace("  ", "&nbsp; ")
+            line = line.replace("\t", "&nbsp; &nbsp; &nbsp; &nbsp; ")
+            if line.startswith(" "):
+                line = "&nbsp;" + line[1:]
+            out.write("<tt>%s</tt><br>\n" % line)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import sys
+
     if not sys.argv[1:]:
-        print('Usage: %s file1 file2' % sys.argv[0])  # NOQA
-        print('or to test: %s test' % sys.argv[0])  # NOQA
-    elif sys.argv[1] == 'test' and not sys.argv[2:]:
+        print("Usage: %s file1 file2" % sys.argv[0])  # NOQA
+        print("or to test: %s test" % sys.argv[0])  # NOQA
+    elif sys.argv[1] == "test" and not sys.argv[2:]:
         import doctest
+
         doctest.testmod()
     else:
         print(diffFiles(sys.argv[1], sys.argv[2]))  # NOQA
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/namedfile.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/namedfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,94 @@
-# -*- coding: utf-8 -*-
 from AccessControl.class_init import InitializeClass
 from plone.namedfile import NamedFile
 from Products.CMFDiffTool.BinaryDiff import BinaryDiff
 from Products.CMFDiffTool.ListDiff import ListDiff
 from Products.CMFDiffTool.TextDiff import TextDiff
 from Products.CMFDiffTool.utils import html_escape
 
 
 FILE_FIELD_TYPES = []
 
 try:
     from plone.namedfile import field
+
     FILE_FIELD_TYPES.extend([field.NamedFile, field.NamedImage])
 
-    if getattr(field, 'HAVE_BLOBS', True):
+    if getattr(field, "HAVE_BLOBS", True):
         FILE_FIELD_TYPES.extend([field.NamedBlobFile, field.NamedBlobImage])
 except ImportError:
     pass
 
 FILE_FIELD_TYPES = tuple(FILE_FIELD_TYPES)
 
 
 def named_file_as_str(f):
-    return '' if f is None else '%s (%d bytes)' % (f.filename, len(f.data))
+    return "" if f is None else "%s (%d bytes)" % (f.filename, len(f.data))
 
 
 def is_same(old_data, old_filename, new_data, new_filename):
     if old_data != new_data:
         return False
 
     if (old_filename is not None) and (new_filename is not None):
         return old_filename == new_filename
 
     return True
 
 
 class NamedFileBinaryDiff(BinaryDiff):
-
-    def __init__(self, obj1, obj2, field, id1=None, id2=None, field_name=None,
-                 field_label=None, schemata=None):
-
+    def __init__(
+        self,
+        obj1,
+        obj2,
+        field,
+        id1=None,
+        id2=None,
+        field_name=None,
+        field_label=None,
+        schemata=None,
+    ):
         self.field = field
         self.label = field_label or field
-        self.schemata = schemata or 'default'
+        self.schemata = schemata or "default"
         self.field_name = field_name or field
 
         old_field = getattr(obj1, field)
         new_field = getattr(obj2, field)
 
-        self.oldValue = getattr(old_field, 'data', None)
-        self.newValue = getattr(new_field, 'data', None)
+        self.oldValue = getattr(old_field, "data", None)
+        self.newValue = getattr(new_field, "data", None)
 
-        self.id1 = id1 or getattr(obj1, 'getId', lambda: None)()
-        self.id2 = id2 or getattr(obj2, 'getId', lambda: None)()
+        self.id1 = id1 or getattr(obj1, "getId", lambda: None)()
+        self.id2 = id2 or getattr(obj2, "getId", lambda: None)()
 
-        self.oldFilename = getattr(old_field, 'filename', None)
-        self.newFilename = getattr(new_field, 'filename', None)
+        self.oldFilename = getattr(old_field, "filename", None)
+        self.newFilename = getattr(new_field, "filename", None)
 
         self.same = is_same(
-            self.oldValue, self.oldFilename, self.newValue, self.newFilename)
+            self.oldValue, self.oldFilename, self.newValue, self.newFilename
+        )
 
     def _parseField(self, value, filename=None):
         return [
-            '' if (value is None)
+            ""
+            if (value is None)
             else named_file_as_str(NamedFile(data=value, filename=filename)),
         ]
 
     def inline_diff(self):
-        css_class = 'InlineDiff'
+        css_class = "InlineDiff"
         old = self._parseField(self.oldValue, self.oldFilename)[0]
         new = self._parseField(self.newValue, self.newFilename)[0]
 
-        return '' if self.same else self.inlinediff_fmt % (css_class, html_escape(old), html_escape(new))
+        return (
+            ""
+            if self.same
+            else self.inlinediff_fmt % (css_class, html_escape(old), html_escape(new))
+        )
 
 
 InitializeClass(NamedFileBinaryDiff)
 
 
 def make_lists_same_length(s1, s2, dummy_element):
     if len(s1) > len(s2):
@@ -86,61 +99,84 @@
 
 class NamedFileListDiff(ListDiff):
     """Specialization of `ListDiff` to handle lists of files better."""
 
     same_fmt = """<div class="%s">%s</div>"""
     inlinediff_fmt = TextDiff.inlinediff_fmt
 
-    def __init__(self, obj1, obj2, field, id1=None, id2=None, field_name=None,
-                 field_label=None, schemata=None):
-        ListDiff.__init__(self, obj1, obj2, field, id1, id2, field_name,
-                          field_label, schemata)
+    def __init__(
+        self,
+        obj1,
+        obj2,
+        field,
+        id1=None,
+        id2=None,
+        field_name=None,
+        field_label=None,
+        schemata=None,
+    ):
+        ListDiff.__init__(
+            self, obj1, obj2, field, id1, id2, field_name, field_label, schemata
+        )
         old_values = list(self.oldValue or [])
         new_values = list(self.newValue or [])
 
         self.same = True
         if len(old_values) != len(new_values):
             self.same = False
         else:
-            for (old, new) in zip(old_values, new_values):
+            for old, new in zip(old_values, new_values):
                 if not is_same(old.data, old.filename, new.data, new.filename):
                     self.same = False
                     break
 
     def _parseField(self, value, filename=None):
         value = value or []
         return [named_file_as_str(f) for f in value]
 
     def inline_diff(self):
         if self.same:
             return None
 
-        css_class = 'InlineDiff'
+        css_class = "InlineDiff"
 
         old_reprs = self._parseField(self.oldValue, None)
         new_reprs = self._parseField(self.newValue, None)
 
         old_data = [
-            {'repr': repr, 'data': value.data, 'filename': value.filename}
+            {"repr": repr, "data": value.data, "filename": value.filename}
             for (repr, value) in zip(old_reprs, self.oldValue or [])
         ]
         new_data = [
-            {'repr': repr, 'data': value.data, 'filename': value.filename}
+            {"repr": repr, "data": value.data, "filename": value.filename}
             for (repr, value) in zip(new_reprs, self.newValue or [])
         ]
 
-        dummy_dict = {'repr': '', 'data': None, 'filename': None}
+        dummy_dict = {"repr": "", "data": None, "filename": None}
         make_lists_same_length(old_data, new_data, dummy_dict)
 
         def is_same_dict(d1, d2):
             return is_same(
-                d1['data'], d1['filename'], d2['data'], d2['filename'],
+                d1["data"],
+                d1["filename"],
+                d2["data"],
+                d2["filename"],
             )
 
-        return '\n'.join([
-            ((self.same_fmt % (css_class, html_escape(d_old['repr'])))
-             if is_same_dict(d_old, d_new) else self.inlinediff_fmt
-             % (css_class, html_escape(d_old['repr']), html_escape(d_new['repr']))
-             ) for (d_old, d_new) in zip(old_data, new_data)])
+        return "\n".join(
+            [
+                (
+                    (self.same_fmt % (css_class, html_escape(d_old["repr"])))
+                    if is_same_dict(d_old, d_new)
+                    else self.inlinediff_fmt
+                    % (
+                        css_class,
+                        html_escape(d_old["repr"]),
+                        html_escape(d_new["repr"]),
+                    )
+                )
+                for (d_old, d_new) in zip(old_data, new_data)
+            ]
+        )
 
 
 InitializeClass(NamedFileListDiff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/testing.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/testing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,63 @@
-# -*- coding: utf-8 -*-
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import PloneSandboxLayer
 from plone.dexterity.fti import DexterityFTI
 from Products.CMFCore.utils import getToolByName
 from zope.component import getSiteManager
 from zope.schema.interfaces import IVocabularyFactory
 from zope.schema.vocabulary import SimpleTerm
 from zope.schema.vocabulary import SimpleVocabulary
 
 
-TEST_CONTENT_TYPE_ID = 'TestContentType'
+TEST_CONTENT_TYPE_ID = "TestContentType"
 
 VOCABULARY_TUPLES = [
-    (u'first_value', u'First Title'),
-    (u'second_value', None),
-    (u'third_value', u'Third Title'),
+    ("first_value", "First Title"),
+    ("second_value", None),
+    ("third_value", "Third Title"),
 ]
 
 VOCABULARY = SimpleVocabulary(
-    [SimpleTerm(value=v, title=t) for (v, t) in VOCABULARY_TUPLES])
+    [SimpleTerm(value=v, title=t) for (v, t) in VOCABULARY_TUPLES]
+)
 
 
 def vocabulary_factory(context):
     return VOCABULARY
 
 
 class DXLayer(PloneSandboxLayer):
-
-    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE, )
+    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpPloneSite(self, portal):
-        '''Set up additional products and ZCML required to test
+        """Set up additional products and ZCML required to test
         this product.
-        '''
+        """
         # setup dexterity
-        types_tool = getToolByName(portal, 'portal_types')
+        types_tool = getToolByName(portal, "portal_types")
 
         sm = getSiteManager(portal)
         sm.registerUtility(
             component=vocabulary_factory,
             provided=IVocabularyFactory,
-            name=u'Products.CMFDiffTool.testing.VOCABULARY',
+            name="Products.CMFDiffTool.testing.VOCABULARY",
         )
 
         fti = DexterityFTI(
             TEST_CONTENT_TYPE_ID,
             factory=TEST_CONTENT_TYPE_ID,
             global_allow=True,
             behaviors=(
-                'plone.app.versioningbehavior.behaviors.IVersionable',
-                'plone.app.dexterity.behaviors.metadata.IBasic',
-                'plone.app.relationfield.behavior.IRelatedItems',
-                'plone.app.contenttypes.behaviors.collection.ICollection',
+                "plone.app.versioningbehavior.behaviors.IVersionable",
+                "plone.app.dexterity.behaviors.metadata.IBasic",
+                "plone.app.relationfield.behavior.IRelatedItems",
+                "plone.app.contenttypes.behaviors.collection.ICollection",
             ),
-            model_source='''
+            model_source="""
             <model xmlns='http://namespaces.plone.org/supermodel/schema'>
                 <schema>
                     <field name='text' type='zope.schema.Text'>
                         <title>Text</title>
                         <required>False</required>
                     </field>
                     <field name='file' type='plone.namedfile.field.NamedFile'>
@@ -86,16 +85,17 @@
                         <required>False</required>
                         <value_type type="zope.schema.Choice">
                             <vocabulary>Products.CMFDiffTool.testing.VOCABULARY</vocabulary>
                         </value_type>
                     </field>
                 </schema>
             </model>
-            ''',
+            """,
         )
         types_tool._setObject(TEST_CONTENT_TYPE_ID, fti)
 
 
 PACKAGE_DX_FIXTURE = DXLayer()
 
 CMFDiffToolDXLayer = FunctionalTesting(
-    bases=(PACKAGE_DX_FIXTURE, ), name='Products.CMFDiffTool.DX:functional')
+    bases=(PACKAGE_DX_FIXTURE,), name="Products.CMFDiffTool.DX:functional"
+)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testChangeSet.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testChangeSet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 #
 # CMFDiffTool tests
 #
 from Acquisition import aq_base
 from os import linesep
-from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING  # NOQA
+from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.base.utils import safe_hasattr
 from Products.CMFCore.utils import getToolByName
 from Products.CMFDiffTool.ChangeSet import BaseChangeSet
 from Products.CMFDiffTool.dexteritydiff import DexterityCompoundDiff
 from unittest import TestCase
@@ -16,65 +15,60 @@
 
 class TestChangeSet(TestCase):
     """Tests for ChangeSet objects"""
 
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
         self.folder = self.portal
-        self.p_diff = getToolByName(self.portal, 'portal_diff')
-        cs = BaseChangeSet('my_changeset')
+        self.p_diff = getToolByName(self.portal, "portal_diff")
+        cs = BaseChangeSet("my_changeset")
         # ChangeSet needs an acquisition wrapper
         self.cs = cs.__of__(self.portal)
-        setRoles(self.portal, TEST_USER_ID, ['Contributor'])
+        setRoles(self.portal, TEST_USER_ID, ["Contributor"])
 
     def testInterface(self):
         """Ensure that tool instances implement the portal_diff interface"""
         from Products.CMFDiffTool.interfaces import IChangeSet
+
         self.assertTrue(IChangeSet.implementedBy(BaseChangeSet))
 
     def setupTestObjects(self):
-        self.folder.invokeFactory('Document', 'doc1', title='My Title')
-        self.folder.manage_pasteObjects(
-            self.folder.manage_copyObjects(['doc1']))
-        cdd = DexterityCompoundDiff(self.folder['doc1'], self.folder['doc1'],
-                                    '')
+        self.folder.invokeFactory("Document", "doc1", title="My Title")
+        self.folder.manage_pasteObjects(self.folder.manage_copyObjects(["doc1"]))
+        cdd = DexterityCompoundDiff(self.folder["doc1"], self.folder["doc1"], "")
         self.len_diff = len(cdd._diffs)
 
     def setupTestFolders(self):
-        self.folder.invokeFactory('Folder', 'folder1', title='My Folder Title')
-        self.folder.folder1.invokeFactory('Document', 'doc1',
-                                          title='My Title1')
-        self.folder.folder1.invokeFactory('Document', 'doc2',
-                                          title='My Title2')
-        self.folder.folder1.invokeFactory('Document', 'doc3',
-                                          title='My Title3')
-        self.folder.manage_pasteObjects(
-            self.folder.manage_copyObjects(['folder1']))
+        self.folder.invokeFactory("Folder", "folder1", title="My Folder Title")
+        self.folder.folder1.invokeFactory("Document", "doc1", title="My Title1")
+        self.folder.folder1.invokeFactory("Document", "doc2", title="My Title2")
+        self.folder.folder1.invokeFactory("Document", "doc3", title="My Title3")
+        self.folder.manage_pasteObjects(self.folder.manage_copyObjects(["folder1"]))
         cdd = DexterityCompoundDiff(
-            self.folder['folder1']['doc1'], self.folder['folder1']['doc1'], '')
+            self.folder["folder1"]["doc1"], self.folder["folder1"]["doc1"], ""
+        )
         self.len_diff = len(cdd._diffs)
 
     def testChangeSetUnchanged(self):
         self.setupTestObjects()
-        self.cs.computeDiff(self.folder['doc1'], self.folder['copy_of_doc1'])
+        self.cs.computeDiff(self.folder["doc1"], self.folder["copy_of_doc1"])
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), self.len_diff)
         self.assertTrue(diffs[0].same)
 
     def testChangeSetChanged(self):
         self.setupTestObjects()
-        self.folder.copy_of_doc1.setTitle('My New Title')
+        self.folder.copy_of_doc1.setTitle("My New Title")
         self.cs.computeDiff(self.folder.doc1, self.folder.copy_of_doc1)
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), self.len_diff)
         self.assertFalse(diffs[0].same)
-        self.assertEqual(diffs[0].ndiff(),
-                         '- My Title%s+ My New Title' % linesep)
+        self.assertEqual(diffs[0].ndiff(), "- My Title%s+ My New Title" % linesep)
 
     def testChangeSetFolderUnchanged(self):
         self.setupTestFolders()
         self.cs.computeDiff(self.folder.folder1, self.folder.copy_of_folder1)
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), 14)
         self.assertTrue(diffs[0].same)
@@ -86,59 +80,61 @@
             self.assertEqual(len(sub_diffs), self.len_diff)
             self.assertTrue(sub_cs[0].same)
             self.assertTrue(sub_cs[1].same)
             self.assertTrue(sub_cs[2].same)
 
     def testChangeSetFolderChanged(self):
         self.setupTestFolders()
-        self.folder.copy_of_folder1.setTitle('My New Title')
+        self.folder.copy_of_folder1.setTitle("My New Title")
         self.cs.computeDiff(self.folder.folder1, self.folder.copy_of_folder1)
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), 14)
         self.assertFalse(diffs[0].same)
-        self.assertEqual(diffs[0].ndiff(),
-                         '- My Folder Title%s+ My New Title' % linesep)
+        self.assertEqual(
+            diffs[0].ndiff(), "- My Folder Title%s+ My New Title" % linesep
+        )
         self.assertFalse(self.cs._added)
         self.assertFalse(self.cs._removed)
         sub_cs = self.cs.getSubDiffs()
         self.assertEqual(len(sub_cs), 3)
         # The sub diffs should show no changes
         for i in range(len(sub_cs)):
             self.assertTrue(isinstance(sub_cs[i], BaseChangeSet))
             sub_diffs = sub_cs[i].getDiffs()
             self.assertEqual(len(sub_diffs), self.len_diff)
             self.assertTrue(sub_diffs[0].same)
 
     def testChangeSetFolderDocChanged(self):
         self.setupTestFolders()
-        self.folder.copy_of_folder1.doc1.setTitle('My New Title')
+        self.folder.copy_of_folder1.doc1.setTitle("My New Title")
         self.cs.computeDiff(self.folder.folder1, self.folder.copy_of_folder1)
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), 14)
         self.assertTrue(diffs[0].same)
         self.assertTrue(diffs[1].same)
         self.assertFalse(self.cs._added)
         self.assertFalse(self.cs._removed)
         sub_cs = self.cs.getSubDiffs()
         self.assertEqual(len(sub_cs), 3)
         for i in range(len(sub_cs)):
             self.assertTrue(isinstance(sub_cs[i], BaseChangeSet))
             sub_diffs = sub_cs[i].getDiffs()
             self.assertEqual(len(sub_diffs), self.len_diff)
             # doc1 has changed
-            if sub_cs[i].getId() == 'doc1':
+            if sub_cs[i].getId() == "doc1":
                 self.assertFalse(sub_diffs[0].same)
-                self.assertEqual(sub_diffs[0].ndiff(),
-                                 '- My Title1%s+ My New Title' % linesep)
+                self.assertEqual(
+                    sub_diffs[0].ndiff(), "- My Title1%s+ My New Title" % linesep
+                )
             else:
                 self.assertTrue(sub_diffs[0].same)
 
     def testChangeSetFolderDocRemoved(self):
         self.setupTestFolders()
-        self.folder.copy_of_folder1.manage_delObjects('doc1')
+        self.folder.copy_of_folder1.manage_delObjects("doc1")
         self.cs.computeDiff(self.folder.folder1, self.folder.copy_of_folder1)
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), 14)
         self.assertTrue(diffs[0].same)
         self.assertTrue(diffs[1].same)
         sub_cs = self.cs.getSubDiffs()
         # We only have two potentially changed objects
@@ -146,44 +142,43 @@
         # The sub diffs should show no changes
         for i in range(len(sub_cs)):
             self.assertTrue(isinstance(sub_cs[i], BaseChangeSet))
             sub_diffs = sub_cs[i].getDiffs()
             self.assertEqual(len(sub_diffs), self.len_diff)
             self.assertTrue(sub_diffs[0].same)
         self.assertFalse(self.cs._added)
-        self.assertEqual(list(self.cs._removed), ['doc1'])
+        self.assertEqual(list(self.cs._removed), ["doc1"])
 
     def testChangeSetFolderDocAdded(self):
         self.setupTestFolders()
-        self.folder.copy_of_folder1.invokeFactory('Document', 'doc4',
-                                                  title='My Doc Title')
+        self.folder.copy_of_folder1.invokeFactory(
+            "Document", "doc4", title="My Doc Title"
+        )
         self.cs.computeDiff(self.folder.folder1, self.folder.copy_of_folder1)
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), 14)
         self.assertTrue(diffs[0].same)
         self.assertTrue(diffs[1].same)
         sub_cs = self.cs.getSubDiffs()
         self.assertEqual(len(sub_cs), 3)
         # The sub diffs should show no changes
         for i in range(len(sub_cs)):
             self.assertTrue(isinstance(sub_cs[i], BaseChangeSet))
             sub_diffs = sub_cs[i].getDiffs()
             self.assertEqual(len(sub_diffs), self.len_diff)
             self.assertTrue(sub_diffs[0].same)
         self.assertFalse(self.cs._removed)
-        self.assertEqual(list(self.cs._added), ['doc4'])
+        self.assertEqual(list(self.cs._added), ["doc4"])
 
     def testChangeSetFolderReordered(self):
         self.setupTestFolders()
-        if safe_hasattr(aq_base(self.folder.copy_of_folder1),
-                        'moveObjectsToTop'):
-            self.folder.copy_of_folder1.moveObjectsToTop(['doc3'])
-        elif safe_hasattr(aq_base(self.folder.copy_of_folder1),
-                          'moveObjectsByDelta'):
-            self.folder.copy_of_folder1.moveObjectsByDelta(['doc3'], -3)
+        if safe_hasattr(aq_base(self.folder.copy_of_folder1), "moveObjectsToTop"):
+            self.folder.copy_of_folder1.moveObjectsToTop(["doc3"])
+        elif safe_hasattr(aq_base(self.folder.copy_of_folder1), "moveObjectsByDelta"):
+            self.folder.copy_of_folder1.moveObjectsByDelta(["doc3"], -3)
         else:
             # We don't have an orderable folder give up
             return
         self.cs.computeDiff(self.folder.folder1, self.folder.copy_of_folder1)
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), 14)
         self.assertTrue(diffs[0].same)
@@ -198,50 +193,50 @@
             self.assertEqual(len(sub_diffs), self.len_diff)
             self.assertTrue(sub_diffs[0].same)
         # XXX we need an explicit way of noting reorders
 
     def testChangeSetFolderComplex(self):
         self.setupTestFolders()
         # Add a new sub object
-        self.folder.copy_of_folder1.invokeFactory('Document', 'doc4',
-                                                  title='My Doc Title')
+        self.folder.copy_of_folder1.invokeFactory(
+            "Document", "doc4", title="My Doc Title"
+        )
         # Delete a sub object
-        self.folder.copy_of_folder1.manage_delObjects('doc2')
+        self.folder.copy_of_folder1.manage_delObjects("doc2")
         # Change one object
-        self.folder.copy_of_folder1.doc3.setTitle('My New Title')
+        self.folder.copy_of_folder1.doc3.setTitle("My New Title")
         # Change the folder itself
-        self.folder.copy_of_folder1.setTitle('My New Title')
+        self.folder.copy_of_folder1.setTitle("My New Title")
         # Move the changed object
-        if safe_hasattr(aq_base(self.folder.copy_of_folder1),
-                        'moveObjectsToTop'):
-            self.folder.copy_of_folder1.moveObjectsToTop(['doc3'])
-        elif safe_hasattr(aq_base(self.folder.copy_of_folder1),
-                          'moveObjectsByDelta'):
-            self.folder.copy_of_folder1.moveObjectsByDelta(['doc3'], -3)
+        if safe_hasattr(aq_base(self.folder.copy_of_folder1), "moveObjectsToTop"):
+            self.folder.copy_of_folder1.moveObjectsToTop(["doc3"])
+        elif safe_hasattr(aq_base(self.folder.copy_of_folder1), "moveObjectsByDelta"):
+            self.folder.copy_of_folder1.moveObjectsByDelta(["doc3"], -3)
         else:
             # We don't have an orderable folder give up
             return
 
-        self.cs.computeDiff(self.folder['folder1'],
-                            self.folder['copy_of_folder1'])
+        self.cs.computeDiff(self.folder["folder1"], self.folder["copy_of_folder1"])
         diffs = self.cs.getDiffs()
         self.assertEqual(len(diffs), 14)
         self.assertFalse(diffs[0].same)
-        self.assertEqual(diffs[0].ndiff(),
-                         '- My Folder Title%s+ My New Title' % linesep)
-        self.assertEqual(list(self.cs._added), ['doc4'])
-        self.assertEqual(list(self.cs._removed), ['doc2'])
+        self.assertEqual(
+            diffs[0].ndiff(), "- My Folder Title%s+ My New Title" % linesep
+        )
+        self.assertEqual(list(self.cs._added), ["doc4"])
+        self.assertEqual(list(self.cs._removed), ["doc2"])
         sub_cs = self.cs.getSubDiffs()
         # We only have two potentially changed objects
         self.assertEqual(len(sub_cs), 2)
         # The sub diffs should show no changes
         for i in range(len(sub_cs)):
             self.assertTrue(isinstance(sub_cs[i], BaseChangeSet))
             sub_diffs = sub_cs[i].getDiffs()
             self.assertEqual(len(sub_diffs), self.len_diff)
-            if sub_cs[i].getId() == 'doc3':
+            if sub_cs[i].getId() == "doc3":
                 self.assertFalse(sub_diffs[0].same)
-                self.assertEqual(sub_diffs[0].ndiff(),
-                                 '- My Title3%s+ My New Title' % linesep)
+                self.assertEqual(
+                    sub_diffs[0].ndiff(), "- My Title3%s+ My New Title" % linesep
+                )
             else:
                 self.assertTrue(sub_diffs[1].same)
         # XXX we need an explicit way of noting reorders
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testDiffTool.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testDiffTool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,112 @@
-# -*- coding: utf-8 -*-
 #
 # CMFDiffTool tests
 #
 
 from plone.app.testing import PLONE_INTEGRATION_TESTING
 from Products.CMFCore.utils import getToolByName
 from Products.CMFDiffTool.CMFDiffTool import registerDiffType
 from Products.CMFDiffTool.CMFDiffTool import unregisterDiffType
 from unittest import TestCase
 from zExceptions import BadRequest
 
 
 class DummyDiff:
-    meta_type = 'Dummy Diff Type'
+    meta_type = "Dummy Diff Type"
 
 
 class DummyDiff2:
-    meta_type = 'Second Dummy Diff Type'
+    meta_type = "Second Dummy Diff Type"
 
 
 class TestDiffTool(TestCase):
     """Test the portal_diff tool"""
 
     layer = PLONE_INTEGRATION_TESTING
 
     def setUp(self):
-        self.p_diff = getToolByName(self.layer['portal'], 'portal_diff')
+        self.p_diff = getToolByName(self.layer["portal"], "portal_diff")
         # clear pt_diff registry
         self.p_diff._pt_diffs = {}
 
         # patch portal_types to list `Document` in the listContentTypes
-        # a plausability check is done in the `setDiffForPortalType` method
+        # a plausibility check is done in the `setDiffForPortalType` method
         # but we have no content registry
-        portal_types = getToolByName(self.layer['portal'], 'portal_types')
+        portal_types = getToolByName(self.layer["portal"], "portal_types")
         self._old_listContentTypes = portal_types.listContentTypes
-        portal_types.listContentTypes = lambda: ['Document']
+        portal_types.listContentTypes = lambda: ["Document"]
         registerDiffType(DummyDiff)
 
     def tearDown(self):
-        portal_types = getToolByName(self.layer['portal'], 'portal_types')
+        portal_types = getToolByName(self.layer["portal"], "portal_types")
         portal_types.listContentTypes = self._old_listContentTypes
 
     def testInterface(self):
         """Ensure that tool instances implement the portal_diff interface"""
         from Products.CMFDiffTool.interfaces.portal_diff import portal_diff
+
         self.assertTrue(portal_diff.providedBy(self.p_diff))
 
     def testRegisterDiffType(self):
         """Test registration of Diff types"""
         unregisterDiffType(DummyDiff)
-        self.assertNotIn('Dummy Diff Type', self.p_diff.listDiffTypes())
+        self.assertNotIn("Dummy Diff Type", self.p_diff.listDiffTypes())
         registerDiffType(DummyDiff)
-        self.assertIn('Dummy Diff Type', self.p_diff.listDiffTypes())
+        self.assertIn("Dummy Diff Type", self.p_diff.listDiffTypes())
 
     def testSetDiff(self):
         """Test setDiffForPortalType() method"""
-        d = {'field1': 'TestDiff', 'field2': 'Dummy Diff Type'}
-        self.p_diff.setDiffForPortalType('Document', d)
-        self.assertEqual(self.p_diff.getDiffForPortalType('Document'), d)
+        d = {"field1": "TestDiff", "field2": "Dummy Diff Type"}
+        self.p_diff.setDiffForPortalType("Document", d)
+        self.assertEqual(self.p_diff.getDiffForPortalType("Document"), d)
 
     def testSetDiffReplaces(self):
         """Test that setDiffForPortalType() replaces old data"""
-        d1 = {'field1': 'TestDiff', 'field2': 'Dummy Diff Type'}
-        d2 = {'field3': 'Dummy Diff Type'}
-        self.p_diff.setDiffForPortalType('Document', d1)
-        self.p_diff.setDiffForPortalType('Document', d2)
-        self.assertEqual(self.p_diff.getDiffForPortalType('Document'), d2)
+        d1 = {"field1": "TestDiff", "field2": "Dummy Diff Type"}
+        d2 = {"field3": "Dummy Diff Type"}
+        self.p_diff.setDiffForPortalType("Document", d1)
+        self.p_diff.setDiffForPortalType("Document", d2)
+        self.assertEqual(self.p_diff.getDiffForPortalType("Document"), d2)
 
     def testSingleSetDiffField(self):
         """Test setDiffField method"""
-        self.p_diff.setDiffField('Document', 'title', 'Dummy Diff Type')
-        self.assertEqual(self.p_diff.getDiffForPortalType('Document'),
-                         {'title': 'Dummy Diff Type'})
+        self.p_diff.setDiffField("Document", "title", "Dummy Diff Type")
+        self.assertEqual(
+            self.p_diff.getDiffForPortalType("Document"), {"title": "Dummy Diff Type"}
+        )
 
     def testMultipleSetDiffField(self):
         """
         Test setDiffField method adding a second field to one content type
         """
-        self.p_diff.setDiffField('Document', 'title', 'Dummy Diff Type')
-        self.p_diff.setDiffField('Document', 'description', 'Dummy Diff Type')
-        d = {'title': 'Dummy Diff Type', 'description': 'Dummy Diff Type'}
-        self.assertEqual(self.p_diff.getDiffForPortalType('Document'), d)
+        self.p_diff.setDiffField("Document", "title", "Dummy Diff Type")
+        self.p_diff.setDiffField("Document", "description", "Dummy Diff Type")
+        d = {"title": "Dummy Diff Type", "description": "Dummy Diff Type"}
+        self.assertEqual(self.p_diff.getDiffForPortalType("Document"), d)
 
     def testReplaceSetDiffField(self):
         """Test that setDiffField does a replace for existing fields"""
         registerDiffType(DummyDiff2)
-        self.p_diff.setDiffField('Document', 'title', 'Dummy Diff Type')
-        self.p_diff.setDiffField('Document', 'title', 'Second Dummy Diff Type')
-        d = {'title': 'Second Dummy Diff Type'}
-        self.assertEqual(self.p_diff.getDiffForPortalType('Document'), d)
+        self.p_diff.setDiffField("Document", "title", "Dummy Diff Type")
+        self.p_diff.setDiffField("Document", "title", "Second Dummy Diff Type")
+        d = {"title": "Second Dummy Diff Type"}
+        self.assertEqual(self.p_diff.getDiffForPortalType("Document"), d)
         unregisterDiffType(DummyDiff2)
 
     def testSetDiffFieldNameFailure(self):
-        self.assertRaises(BadRequest, self.p_diff.setDiffField,
-                          'Bob', 'title', 'Dummy Diff Type')
+        self.assertRaises(
+            BadRequest, self.p_diff.setDiffField, "Bob", "title", "Dummy Diff Type"
+        )
 
     def testSetDiffFieldBlankFieldFailure(self):
-        self.assertRaises(BadRequest, self.p_diff.setDiffField,
-                          'Document', '', 'Dummy Diff Type')
+        self.assertRaises(
+            BadRequest, self.p_diff.setDiffField, "Document", "", "Dummy Diff Type"
+        )
 
     def testSetDiffFieldInvalidDiffFailure(self):
-        self.assertRaises(BadRequest, self.p_diff.setDiffField,
-                          'Document', 'title', 'NoDiff')
+        self.assertRaises(
+            BadRequest, self.p_diff.setDiffField, "Document", "title", "NoDiff"
+        )
 
     def beforeTearDown(self):
         # Undo changes that don't get rolled back (i.e. module level changes)
         unregisterDiffType(DummyDiff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testFieldDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testFieldDiff.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-# -*- coding: utf-8 -*-
 #
 # CMFDiffTool tests
 #
 from os import linesep
 from plone.app.testing import PLONE_INTEGRATION_TESTING
 from Products.CMFDiffTool.FieldDiff import dump
 from Products.CMFDiffTool.FieldDiff import FieldDiff
 from unittest import TestCase
 
 
 _marker = []
 
 
 class A:
-    attribute = 'value'
+    attribute = "value"
 
     def method(self):
-        return 'method value'
+        return "method value"
 
 
 class B:
-    attribute = 'different value'
+    attribute = "different value"
 
     def method(self):
-        return 'different method value'
+        return "different method value"
 
 
 class U:
-    attribute = u'\xfcnicode value'
+    attribute = "\xfcnicode value"
 
     def method(self):
-        return u'different method val\xfce'
+        return "different method val\xfce"
 
 
 class H:
     attribute = '<script>alert("Hacker value")</script>'
 
     def method(self):
         return '<script>alert("Hacker method value")</script>'
@@ -44,166 +43,167 @@
     """Test the FieldDiff class"""
 
     layer = PLONE_INTEGRATION_TESTING
 
     def testInterface(self):
         """Ensure that tool instances implement the portal_diff interface"""
         from Products.CMFDiffTool.interfaces.portal_diff import IDifference
+
         self.assertTrue(IDifference.implementedBy(FieldDiff))
 
     def testAttributeSame(self):
         """Test attribute with same value"""
         a = A()
-        fd = FieldDiff(a, a, 'attribute')
+        fd = FieldDiff(a, a, "attribute")
         self.assertTrue(fd.same)
         uu = U()
-        fd = FieldDiff(uu, uu, 'attribute')
+        fd = FieldDiff(uu, uu, "attribute")
         self.assertTrue(fd.same)
 
     def testMethodSame(self):
         """Test method with same value"""
         a = A()
-        fd = FieldDiff(a, a, 'method')
+        fd = FieldDiff(a, a, "method")
         self.assertTrue(fd.same)
         uu = U()
-        fd = FieldDiff(uu, uu, 'method')
+        fd = FieldDiff(uu, uu, "method")
         self.assertTrue(fd.same)
 
     def testAttributeDiff(self):
         """Test attribute with different value"""
         a = A()
         b = B()
         uu = U()
-        fd = FieldDiff(a, b, 'attribute')
+        fd = FieldDiff(a, b, "attribute")
         self.assertFalse(fd.same)
-        fd = FieldDiff(a, uu, 'attribute')
+        fd = FieldDiff(a, uu, "attribute")
         self.assertFalse(fd.same)
 
     def testMethodDiff(self):
         """Test method with different value"""
         a = A()
         b = B()
         uu = U()
-        fd = FieldDiff(a, b, 'method')
+        fd = FieldDiff(a, b, "method")
         self.assertFalse(fd.same)
-        fd = FieldDiff(a, uu, 'method')
+        fd = FieldDiff(a, uu, "method")
         self.assertFalse(fd.same)
 
     def testGetLineDiffsSame(self):
         """test getLineDiffs() method with same value"""
         a = A()
-        fd = FieldDiff(a, a, 'attribute')
-        expected = [('equal', 0, 1, 0, 1)]
+        fd = FieldDiff(a, a, "attribute")
+        expected = [("equal", 0, 1, 0, 1)]
         self.assertEqual(fd.getLineDiffs(), expected)
         uu = U()
-        fd = FieldDiff(uu, uu, 'attribute')
-        expected = [('equal', 0, 1, 0, 1)]
+        fd = FieldDiff(uu, uu, "attribute")
+        expected = [("equal", 0, 1, 0, 1)]
         self.assertEqual(fd.getLineDiffs(), expected)
 
     def testGetLineDiffsDifferent(self):
         """test getLineDiffs() method with different value"""
         a = A()
         b = B()
         uu = U()
-        fd = FieldDiff(a, b, 'attribute')
-        expected = [('replace', 0, 1, 0, 1)]
+        fd = FieldDiff(a, b, "attribute")
+        expected = [("replace", 0, 1, 0, 1)]
         self.assertEqual(fd.getLineDiffs(), expected)
-        fd = FieldDiff(a, uu, 'attribute')
-        expected = [('replace', 0, 1, 0, 1)]
+        fd = FieldDiff(a, uu, "attribute")
+        expected = [("replace", 0, 1, 0, 1)]
         self.assertEqual(fd.getLineDiffs(), expected)
 
     def testSameText(self):
         """Test text diff output with same value"""
         a = A()
-        fd = FieldDiff(a, a, 'attribute')
-        self.assertEqual(fd.ndiff(), '  value')
+        fd = FieldDiff(a, a, "attribute")
+        self.assertEqual(fd.ndiff(), "  value")
         uu = U()
-        fd = FieldDiff(uu, uu, 'attribute')
-        self.assertEqual(fd.ndiff(), u'  \xfcnicode value')
+        fd = FieldDiff(uu, uu, "attribute")
+        self.assertEqual(fd.ndiff(), "  \xfcnicode value")
 
     def testDiffText(self):
         """Test text diff output with different value"""
         a = A()
         b = B()
         uu = U()
-        expected = '- value%s+ different value' % linesep
-        fd = FieldDiff(a, b, 'attribute')
+        expected = "- value%s+ different value" % linesep
+        fd = FieldDiff(a, b, "attribute")
         self.assertEqual(fd.ndiff(), expected)
-        expected = u'- value%s+ \xfcnicode value' % linesep
-        fd = FieldDiff(a, uu, 'attribute')
+        expected = "- value%s+ \xfcnicode value" % linesep
+        fd = FieldDiff(a, uu, "attribute")
         self.assertEqual(fd.ndiff(), expected)
 
     def test_dump_text(self):
         """Test dumping a diff of text."""
         diff = []
-        dump('-', ['support'], 0, 1, diff)
-        self.assertEqual(diff, ['- support'])
+        dump("-", ["support"], 0, 1, diff)
+        self.assertEqual(diff, ["- support"])
         # Try unicode, a 'u' with an umlaut.
         diff = []
-        dump('+', [u's\xfcpport'], 0, 1, diff)
-        self.assertEqual(diff, [u'+ s\xfcpport'])
+        dump("+", ["s\xfcpport"], 0, 1, diff)
+        self.assertEqual(diff, ["+ s\xfcpport"])
         # Combine them.
         diff = []
-        dump('-', ['support'], 0, 1, diff)
-        dump('+', [u's\xfcpport'], 0, 1, diff)
-        self.assertEqual(diff, ['- support', u'+ s\xfcpport'])
+        dump("-", ["support"], 0, 1, diff)
+        dump("+", ["s\xfcpport"], 0, 1, diff)
+        self.assertEqual(diff, ["- support", "+ s\xfcpport"])
 
     def test_dump_integer(self):
         """Test dumping a diff of integers."""
         diff = []
-        dump('-', [4], 0, 1, diff)
-        self.assertEqual(diff, ['- 4'])
-        dump('+', [42], 0, 1, diff)
-        self.assertEqual(diff, ['- 4', '+ 42'])
+        dump("-", [4], 0, 1, diff)
+        self.assertEqual(diff, ["- 4"])
+        dump("+", [42], 0, 1, diff)
+        self.assertEqual(diff, ["- 4", "+ 42"])
 
     def test_dump_float(self):
         """Test dumping a diff of floats."""
         diff = []
-        dump('-', [1.1], 0, 1, diff)
-        self.assertEqual(diff, ['- 1.1'])
-        dump('+', [1.2], 0, 1, diff)
-        self.assertEqual(diff, ['- 1.1', '+ 1.2'])
+        dump("-", [1.1], 0, 1, diff)
+        self.assertEqual(diff, ["- 1.1"])
+        dump("+", [1.2], 0, 1, diff)
+        self.assertEqual(diff, ["- 1.1", "+ 1.2"])
 
     def test_dump_boolean(self):
         """Test dumping a diff of booleans."""
         diff = []
-        dump('-', [True], 0, 1, diff)
-        self.assertEqual(diff, ['- True'])
-        dump('+', [False], 0, 1, diff)
-        self.assertEqual(diff, ['- True', '+ False'])
+        dump("-", [True], 0, 1, diff)
+        self.assertEqual(diff, ["- True"])
+        dump("+", [False], 0, 1, diff)
+        self.assertEqual(diff, ["- True", "+ False"])
 
     def test_inline_diff_same(self):
         """Test inline diff for attribute with same value"""
         a = A()
         uu = U()
         h = H()
         # We mostly just want to check that the inline diff renders without error.
-        fd = FieldDiff(a, a, 'attribute')
+        fd = FieldDiff(a, a, "attribute")
         self.assertIn('class="InlineDiff"', fd.inline_diff())
-        fd = FieldDiff(uu, uu, 'attribute')
+        fd = FieldDiff(uu, uu, "attribute")
         self.assertIn('class="InlineDiff"', fd.inline_diff())
         self.assertNotIn("&gt;", fd.inline_diff())
-        fd = FieldDiff(h, h, 'attribute')
+        fd = FieldDiff(h, h, "attribute")
         self.assertIn('class="InlineDiff"', fd.inline_diff())
         # h.attribute contains a script, and this should be escaped.
         self.assertNotIn(h.attribute, fd.inline_diff())
         self.assertIn("&gt;", fd.inline_diff())
 
     def test_inline_diff_different(self):
         """Test inline diff for attribute with different value"""
         a = A()
         uu = U()
         h = H()
-        fd = FieldDiff(a, uu, 'attribute')
+        fd = FieldDiff(a, uu, "attribute")
         self.assertIn('class="InlineDiff"', fd.inline_diff())
-        fd = FieldDiff(uu, a, 'attribute')
+        fd = FieldDiff(uu, a, "attribute")
         self.assertIn('class="InlineDiff"', fd.inline_diff())
         self.assertNotIn("&gt;", fd.inline_diff())
-        fd = FieldDiff(uu, h, 'attribute')
+        fd = FieldDiff(uu, h, "attribute")
         self.assertIn('class="InlineDiff"', fd.inline_diff())
         # h.attribute contains a script, and this should be escaped.
         self.assertNotIn(h.attribute, fd.inline_diff())
-        fd = FieldDiff(h, uu, 'attribute')
+        fd = FieldDiff(h, uu, "attribute")
         self.assertIn('class="InlineDiff"', fd.inline_diff())
         # h.attribute contains a script, and this should be escaped.
         self.assertNotIn(h.attribute, fd.inline_diff())
         self.assertIn("&gt;", fd.inline_diff())
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testListDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testListDiff.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # CMFDiffTool tests
 #
 from os import linesep
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from Products.CMFDiffTool import testing
@@ -23,224 +22,237 @@
 
 
 class HList:
     attribute = ['<script>alert("Hacker value")</script>']
 
 
 class C:
-    attribute = {'a': 1, 'b': 2}
+    attribute = {"a": 1, "b": 2}
 
 
 class D:
-    attribute = {'a': 1, 'b': 2, 'c': 3}
+    attribute = {"a": 1, "b": 2, "c": 3}
 
 
 class HDict:
-    attribute = {'a': '<script>alert("Hacker value")</script>'}
+    attribute = {"a": '<script>alert("Hacker value")</script>'}
 
 
 class TestListDiff(BaseDXTestCase):
     """Test the ListDiff class"""
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        self.portal = self.layer["portal"]
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
+            "obj1",
         )
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
+            "obj2",
         )
 
-        self.obj1 = self.portal['obj1']
-        self.obj2 = self.portal['obj2']
+        self.obj1 = self.portal["obj1"]
+        self.obj2 = self.portal["obj2"]
 
     def testInterface(self):
         """Ensure that tool instances implement the portal_diff interface"""
         self.assertTrue(IDifference.implementedBy(ListDiff))
 
     def testInvalidValue(self):
-        """ Test if no error with invalid values """
+        """Test if no error with invalid values"""
         a = A()
         a.attribute = []
         b = A()
 
         b.attribute = None
-        diff = ListDiff(a, b, 'attribute')
-        self.assertEqual([('insert', 0, 0, 0, 1)], diff.getLineDiffs())
+        diff = ListDiff(a, b, "attribute")
+        self.assertEqual([("insert", 0, 0, 0, 1)], diff.getLineDiffs())
 
         b.attribute = 0
-        diff = ListDiff(a, b, 'attribute')
-        self.assertEqual([('insert', 0, 0, 0, 1)], diff.getLineDiffs())
+        diff = ListDiff(a, b, "attribute")
+        self.assertEqual([("insert", 0, 0, 0, 1)], diff.getLineDiffs())
 
-        b.attribute = ''
-        diff = ListDiff(a, b, 'attribute')
-        self.assertEqual([('insert', 0, 0, 0, 1)], diff.getLineDiffs())
+        b.attribute = ""
+        diff = ListDiff(a, b, "attribute")
+        self.assertEqual([("insert", 0, 0, 0, 1)], diff.getLineDiffs())
 
     def testAttributeSame(self):
         """Test attribute with same value"""
         a = A()
-        diff = ListDiff(a, a, 'attribute')
+        diff = ListDiff(a, a, "attribute")
         self.assertTrue(diff.same)
 
     def testAttributeDiff(self):
         """Test attribute with different value"""
         a = A()
         b = B()
-        diff = ListDiff(a, b, 'attribute')
+        diff = ListDiff(a, b, "attribute")
         self.assertFalse(diff.same)
 
     def testGetLineDiffsSame(self):
         """test getLineDiffs() method with same value"""
         a = A()
-        diff = ListDiff(a, a, 'attribute')
-        expected = [('equal', 0, 3, 0, 3)]
+        diff = ListDiff(a, a, "attribute")
+        expected = [("equal", 0, 3, 0, 3)]
         self.assertEqual(diff.getLineDiffs(), expected)
 
     def testGetLineDiffsDifferent(self):
         """test getLineDiffs() method with different value"""
         a = A()
         b = B()
-        diff = ListDiff(a, b, 'attribute')
-        expected = [('equal', 0, 3, 0, 3), ('insert', 3, 3, 3, 4)]
+        diff = ListDiff(a, b, "attribute")
+        expected = [("equal", 0, 3, 0, 3), ("insert", 3, 3, 3, 4)]
         self.assertEqual(diff.getLineDiffs(), expected)
 
     def testSameText(self):
         """Test text diff output with no diff"""
         a = A()
-        diff = ListDiff(a, a, 'attribute')
-        expected = '  1%(linesep)s  2%(linesep)s  3' % {'linesep': linesep}
+        diff = ListDiff(a, a, "attribute")
+        expected = "  1{linesep}  2{linesep}  3".format(linesep=linesep)
         self.assertEqual(diff.ndiff(), expected)
 
     def testDiffText(self):
         """Test text diff output with no diff"""
         a = A()
         b = B()
-        expected = '  1%(linesep)s  2%(linesep)s  3%(linesep)s+ 4' % \
-                   {'linesep': linesep}
-        diff = ListDiff(a, b, 'attribute')
+        expected = "  1{linesep}  2{linesep}  3{linesep}+ 4".format(linesep=linesep)
+        diff = ListDiff(a, b, "attribute")
         self.assertEqual(diff.ndiff(), expected)
 
     def test_inline_diff(self):
         a = A()
         b = B()
         expected = """<div class="InlineDiff">1</div>
 <div class="InlineDiff">2</div>
 <div class="InlineDiff">3</div>
 <div class="InlineDiff">
     <div class="diff_sub"></div>
     <div class="diff_add">4</div>
 </div>"""
-        diff = ListDiff(a, b, 'attribute')
+        diff = ListDiff(a, b, "attribute")
         self.assertEqual(diff.inline_diff(), expected)
 
     def test_inline_diff_hacker_list(self):
         a = A()
         h = HList()
-        diff = ListDiff(a, h, 'attribute')
+        diff = ListDiff(a, h, "attribute")
         # The script tag should be escaped.
         self.assertNotIn("<script", diff.inline_diff())
         self.assertIn("&gt;", diff.inline_diff())
 
     def test_inline_diff_hacker_dict(self):
         d = D()
         h = HDict()
-        diff = ListDiff(d, h, 'attribute')
+        diff = ListDiff(d, h, "attribute")
         # The script tag should be escaped.
         self.assertNotIn("<script", diff.inline_diff())
         self.assertIn("&gt;", diff.inline_diff())
 
     def test_inline_diff_vocabulary(self):
         # unchanged, with vocabulary title
-        expected = u'<div class="InlineDiff">First Title</div>'
-        self._test_diff_list([testing.VOCABULARY_TUPLES[0][0]],
-                             [testing.VOCABULARY_TUPLES[0][0]], True, expected)
+        expected = '<div class="InlineDiff">First Title</div>'
+        self._test_diff_list(
+            [testing.VOCABULARY_TUPLES[0][0]],
+            [testing.VOCABULARY_TUPLES[0][0]],
+            True,
+            expected,
+        )
         # unchanged, without vocabulary title
-        expected = u'<div class="InlineDiff">second_value</div>'
-        self._test_diff_list([testing.VOCABULARY_TUPLES[1][0]],
-                             [testing.VOCABULARY_TUPLES[1][0]], True, expected)
+        expected = '<div class="InlineDiff">second_value</div>'
+        self._test_diff_list(
+            [testing.VOCABULARY_TUPLES[1][0]],
+            [testing.VOCABULARY_TUPLES[1][0]],
+            True,
+            expected,
+        )
         # changed: add value, with vocabulary title
-        expected = u'''<div class="InlineDiff">
+        expected = """<div class="InlineDiff">
     <div class="diff_sub"></div>
     <div class="diff_add">First Title</div>
-</div>'''
-        self._test_diff_list([],
-                             [testing.VOCABULARY_TUPLES[0][0]],
-                             False, expected)
+</div>"""
+        self._test_diff_list([], [testing.VOCABULARY_TUPLES[0][0]], False, expected)
         # changed: replaced unique value by another one, displaying titles
-        expected = u'''<div class="InlineDiff">
+        expected = """<div class="InlineDiff">
     <div class="diff_sub">First Title</div>
     <div class="diff_add"></div>
 </div>
 <div class="InlineDiff">
     <div class="diff_sub"></div>
     <div class="diff_add">Third Title</div>
-</div>'''
-        self._test_diff_list([testing.VOCABULARY_TUPLES[0][0]],
-                             [testing.VOCABULARY_TUPLES[2][0]],
-                             False, expected)
+</div>"""
+        self._test_diff_list(
+            [testing.VOCABULARY_TUPLES[0][0]],
+            [testing.VOCABULARY_TUPLES[2][0]],
+            False,
+            expected,
+        )
         # changed: replaced multiple values by others, displaying titles
-        expected = u'''<div class="InlineDiff">
+        expected = """<div class="InlineDiff">
     <div class="diff_sub">First Title</div>
     <div class="diff_add"></div>
 </div>
 <div class="InlineDiff">second_value</div>
 <div class="InlineDiff">
     <div class="diff_sub"></div>
     <div class="diff_add">Third Title</div>
-</div>'''
-        self._test_diff_list([testing.VOCABULARY_TUPLES[0][0],
-                              testing.VOCABULARY_TUPLES[1][0]],
-                             [testing.VOCABULARY_TUPLES[1][0],
-                              testing.VOCABULARY_TUPLES[2][0]],
-                             False, expected)
+</div>"""
+        self._test_diff_list(
+            [testing.VOCABULARY_TUPLES[0][0], testing.VOCABULARY_TUPLES[1][0]],
+            [testing.VOCABULARY_TUPLES[1][0], testing.VOCABULARY_TUPLES[2][0]],
+            False,
+            expected,
+        )
         # changed: replaced multiple values by others, displaying titles
-        expected = u'''<div class="InlineDiff">
+        expected = """<div class="InlineDiff">
     <div class="diff_sub"></div>
     <div class="diff_add">Third Title</div>
 </div>
 <div class="InlineDiff">First Title</div>
 <div class="InlineDiff">
     <div class="diff_sub">second_value</div>
     <div class="diff_add"></div>
-</div>'''
-        self._test_diff_list([testing.VOCABULARY_TUPLES[0][0],
-                              testing.VOCABULARY_TUPLES[1][0]],
-                             [testing.VOCABULARY_TUPLES[2][0],
-                              testing.VOCABULARY_TUPLES[0][0]],
-                             False, expected)
+</div>"""
+        self._test_diff_list(
+            [testing.VOCABULARY_TUPLES[0][0], testing.VOCABULARY_TUPLES[1][0]],
+            [testing.VOCABULARY_TUPLES[2][0], testing.VOCABULARY_TUPLES[0][0]],
+            False,
+            expected,
+        )
         # changed: removed values, displaying titles
-        expected = u'''<div class="InlineDiff">
+        expected = """<div class="InlineDiff">
     <div class="diff_sub">First Title</div>
     <div class="diff_add"></div>
 </div>
 <div class="InlineDiff">
     <div class="diff_sub">second_value</div>
     <div class="diff_add"></div>
-</div>'''
-        self._test_diff_list([testing.VOCABULARY_TUPLES[0][0],
-                              testing.VOCABULARY_TUPLES[1][0]],
-                             [], False, expected)
+</div>"""
+        self._test_diff_list(
+            [testing.VOCABULARY_TUPLES[0][0], testing.VOCABULARY_TUPLES[1][0]],
+            [],
+            False,
+            expected,
+        )
 
     def _test_diff_list(self, value1, value2, same, expected):
         self.obj1.choices = value1
         self.obj2.choices = value2
-        diff = ListDiff(self.obj1, self.obj2, 'choices')
+        diff = ListDiff(self.obj1, self.obj2, "choices")
         self.assertEqual(diff.same, same)
         self.assertEqual(diff.inline_diff(), expected)
 
     def testGetLineDictDiffsSame(self):
         """test getLineDiffs() method with dict same value"""
         c = C()
-        diff = ListDiff(c, c, 'attribute')
-        expected = [('equal', 0, 1, 0, 1)]
+        diff = ListDiff(c, c, "attribute")
+        expected = [("equal", 0, 1, 0, 1)]
         self.assertEqual(diff.getLineDiffs(), expected)
 
     def testGetLineDictDiffsDifferent(self):
         """test getLineDiffs() method with dict different value"""
         c = C()
         d = D()
-        diff = ListDiff(c, d, 'attribute')
-        expected = [('replace', 0, 1, 0, 1)]
+        diff = ListDiff(c, d, "attribute")
+        expected = [("replace", 0, 1, 0, 1)]
         self.assertEqual(diff.getLineDiffs(), expected)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/testTextDiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/testTextDiff.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-# -*- coding: utf-8 -*-
-
 from os import linesep
 from plone.app.testing import PLONE_INTEGRATION_TESTING
 from Products.CMFDiffTool.TextDiff import TextDiff
 from unittest import TestCase
 
 
 _marker = []
 
 
 class A:
-    attribute = 'कामसूत्र'
+    attribute = "कामसूत्र"
 
     def method(self):
-        return 'method कामसूत्र'
+        return "method कामसूत्र"
 
 
 class B:
-    attribute = '過労死'
+    attribute = "過労死"
 
     def method(self):
-        return 'method 過労死'
+        return "method 過労死"
 
 
 class H:
     attribute = '<script>alert("Hacker value")</script>'
 
     def method(self):
         return '<script>alert("Hacker method value")</script>'
 
 
 class TestTextDiff(TestCase):
     """Test the TextDiff class"""
+
     layer = PLONE_INTEGRATION_TESTING
 
     def testInterface(self):
         """Ensure that tool instances implement the portal_diff interface"""
         from Products.CMFDiffTool.interfaces import IDifference
+
         self.assertTrue(IDifference.implementedBy(TextDiff))
 
     def testAttributeSame(self):
         """Test attribute with same value"""
         a = A()
-        fd = TextDiff(a, a, 'attribute')
+        fd = TextDiff(a, a, "attribute")
         self.assertTrue(fd.same)
 
     def testMethodSame(self):
         """Test method with same value"""
         a = A()
-        fd = TextDiff(a, a, 'method')
+        fd = TextDiff(a, a, "method")
         self.assertTrue(fd.same)
 
     def testAttributeDiff(self):
         """Test attribute with different value"""
         a = A()
         b = B()
-        fd = TextDiff(a, b, 'attribute')
+        fd = TextDiff(a, b, "attribute")
         self.assertFalse(fd.same)
 
     def testMethodDiff(self):
         """Test method with different value"""
         a = A()
         b = B()
-        fd = TextDiff(a, b, 'method')
+        fd = TextDiff(a, b, "method")
         self.assertFalse(fd.same)
 
     def testGetLineDiffsSame(self):
         """test getLineDiffs() method with same value"""
         a = A()
-        fd = TextDiff(a, a, 'attribute')
-        expected = [('equal', 0, 1, 0, 1)]
+        fd = TextDiff(a, a, "attribute")
+        expected = [("equal", 0, 1, 0, 1)]
         self.assertEqual(fd.getLineDiffs(), expected)
 
     def testGetLineDiffsDifferent(self):
         """test getLineDiffs() method with different value"""
         a = A()
         b = B()
-        fd = TextDiff(a, b, 'attribute')
-        expected = [('replace', 0, 1, 0, 1)]
+        fd = TextDiff(a, b, "attribute")
+        expected = [("replace", 0, 1, 0, 1)]
         self.assertEqual(fd.getLineDiffs(), expected)
 
     def testSameText(self):
         """Test text diff output with same value"""
         a = A()
-        fd = TextDiff(a, a, 'attribute')
-        self.assertEqual(fd.ndiff(), '  कामसूत्र')
+        fd = TextDiff(a, a, "attribute")
+        self.assertEqual(fd.ndiff(), "  कामसूत्र")
 
     def testDiffText(self):
         """Test text diff output with different value"""
         a = A()
         b = B()
-        expected = '- कामसूत्र%s+ 過労死' % linesep
-        fd = TextDiff(a, b, 'attribute')
+        expected = "- कामसूत्र%s+ 過労死" % linesep
+        fd = TextDiff(a, b, "attribute")
         self.assertEqual(fd.ndiff(), expected)
 
     def testUnifiedDiff(self):
         """Test text diff output with different value"""
         a = A()
         b = B()
 
@@ -103,15 +103,15 @@
 
 +++ version2
 
 @@ -1 +1 @@
 
 -कामसूत्र
 +過労死"""
-        fd = TextDiff(a, b, 'attribute', 'version1', 'version2')
+        fd = TextDiff(a, b, "attribute", "version1", "version2")
         self.assertEqual(fd.unified_diff(), expected)
 
     def testHTMLDiff(self):
         """Test text diff output with different value"""
         a = A()
         b = B()
         h = H()
@@ -121,28 +121,28 @@
         <colgroup></colgroup> <colgroup></colgroup> <colgroup></colgroup>
         <colgroup></colgroup> <colgroup></colgroup> <colgroup></colgroup>
         <thead><tr><th class="diff_next"><br /></th><th colspan="2" class="diff_header">None</th><th class="diff_next"><br /></th><th colspan="2" class="diff_header">None</th></tr></thead>
         <tbody>
             <tr><td class="diff_next" id="difflib_chg_to0__0"><a href="#difflib_chg_to0__top">t</a></td><td class="diff_header" id="from0_1">1</td><td nowrap="nowrap"><span class="diff_sub">कामसूत्र</span></td><td class="diff_next"><a href="#difflib_chg_to0__top">t</a></td><td class="diff_header" id="to0_1">1</td><td nowrap="nowrap"><span class="diff_add">過労死</span></td></tr>
         </tbody>
     </table>"""  # NOQA
-        fd = TextDiff(a, b, 'attribute')
+        fd = TextDiff(a, b, "attribute")
         self.assertEqual(fd.html_diff(), expected)
 
-        fd = TextDiff(a, h, 'attribute')
+        fd = TextDiff(a, h, "attribute")
         # h.attribute contains a script, and this should be escaped.
         self.assertNotIn(h.attribute, fd.html_diff())
         self.assertIn("&gt;", fd.html_diff())
 
     def testInlineDiff(self):
         """Test text inline diff output with different value"""
         a = A()
         b = B()
         h = H()
-        fd = TextDiff(a, b, 'attribute')
+        fd = TextDiff(a, b, "attribute")
         self.assertIn('class="InlineDiff FilenameDiff"', fd.inline_diff())
 
-        fd = TextDiff(a, h, 'attribute')
+        fd = TextDiff(a, h, "attribute")
         self.assertIn('class="InlineDiff FilenameDiff"', fd.inline_diff())
         # h.attribute contains a script, and this should be escaped.
         self.assertNotIn(h.attribute, fd.inline_diff())
         self.assertIn("&gt;", fd.inline_diff())
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_astextdiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_astextdiff.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# -*- coding: utf-8 -*-
 from datetime import date
 from Products.CMFDiffTool.interfaces import IDifference
 from Products.CMFDiffTool.TextDiff import AsTextDiff
 
 import unittest
 
 
-class DateDummyType(object):
+class DateDummyType:
     def __init__(self, date):
         self.date = date
 
 
-class BoolDummyType(object):
+class BoolDummyType:
     def __init__(self, bool_field):
         self.bool_field = bool_field
 
 
 class AsTextDiffTestCase(unittest.TestCase):
-
     def test_should_diff_anything_as_text(self):
         self._test_diff_date(date(2011, 1, 1), date(2012, 2, 2), False)
         self._test_diff_date(date(2011, 1, 1), date(2011, 1, 1), True)
         self._test_diff_date(date(2011, 1, 1), None, False)
         self._test_diff_date(None, None, True)
 
     def _test_diff_date(self, d1, d2, same):
-        diff = AsTextDiff(DateDummyType(d1), DateDummyType(d2), 'date')
+        diff = AsTextDiff(DateDummyType(d1), DateDummyType(d2), "date")
         self.assertTrue(IDifference.providedBy(diff))
         self.assertEqual(diff.same, same)
 
         inline_diff = diff.inline_diff()
         if same:
             self.assertFalse(inline_diff)
         else:
@@ -48,19 +46,18 @@
         self._test_diff_bool(False, None, False)
         self._test_diff_bool(True, None, False)
         self._test_diff_bool(None, False, False)
         self._test_diff_bool(None, True, False)
         self._test_diff_bool(None, None, True)
 
     def _test_diff_bool(self, b1, b2, same):
-        diff = AsTextDiff(BoolDummyType(b1), BoolDummyType(b2), 'bool_field')
+        diff = AsTextDiff(BoolDummyType(b1), BoolDummyType(b2), "bool_field")
 
         self.assertTrue(IDifference.providedBy(diff))
         self.assertEqual(diff.same, same)
 
         inline_diff = diff.inline_diff()
         if same:
             self.assertFalse(inline_diff)
         else:
-            self.assertTrue(
-                ('True' in inline_diff) or ('False' in inline_diff))
+            self.assertTrue(("True" in inline_diff) or ("False" in inline_diff))
             # self.assertFalse('None' in inline_diff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_binarydiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_binarydiff.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,111 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.namedfile.file import NamedFile
 from Products.CMFDiffTool import BinaryDiff
 from Products.CMFDiffTool import namedfile
 from Products.CMFDiffTool import testing
 from Products.CMFDiffTool.interfaces import IDifference
 from Products.CMFDiffTool.tests.BaseTestCase import BaseDXTestCase
 
 
 class BinaryDiffTestCase(BaseDXTestCase):
-
     def test_should_detect_different_filename(self):
-        self.portal = self.layer['portal']
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        self.portal = self.layer["portal"]
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
-            file=NamedFile(data='contents', filename=u'blah.txt'),
+            "obj1",
+            file=NamedFile(data="contents", filename="blah.txt"),
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
-            file=NamedFile(data='contents', filename=u'bleh.txt'),
+            "obj2",
+            file=NamedFile(data="contents", filename="bleh.txt"),
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, 'file')
+        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, "file")
         self.assertTrue(IDifference.providedBy(diff))
         self.assertFalse(diff.same)
 
     def test_should_detect_different_data(self):
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
-            file=NamedFile(data='contents', filename=u'f.txt'),
+            "obj1",
+            file=NamedFile(data="contents", filename="f.txt"),
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
-            file=NamedFile(data='different contents', filename=u'f.txt'),
+            "obj2",
+            file=NamedFile(data="different contents", filename="f.txt"),
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, 'file')
+        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, "file")
         self.assertTrue(IDifference.providedBy(diff))
         self.assertFalse(diff.same)
 
     def test_should_detect_same_data_and_filename(self):
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
-            file=NamedFile(data='contents', filename=u'f.txt'),
+            "obj1",
+            file=NamedFile(data="contents", filename="f.txt"),
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
-            file=NamedFile(data='contents', filename=u'f.txt'),
+            "obj2",
+            file=NamedFile(data="contents", filename="f.txt"),
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, 'file')
+        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, "file")
         self.assertTrue(IDifference.providedBy(diff))
         self.assertTrue(diff.same)
 
     def test_should_escape_html(self):
-        self.portal = self.layer['portal']
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        self.portal = self.layer["portal"]
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
-            file=NamedFile(data='contents', filename=u'blah.txt'),
+            "obj1",
+            file=NamedFile(data="contents", filename="blah.txt"),
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
-            file=NamedFile(data='<script>alert("Hacker data")</script>', filename=u'<script>alert("Hacker filename")</script>.txt'),
+            "obj2",
+            file=NamedFile(
+                data='<script>alert("Hacker data")</script>',
+                filename='<script>alert("Hacker filename")</script>.txt',
+            ),
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, 'file')
+        diff = namedfile.NamedFileBinaryDiff(obj1, obj2, "file")
         self.assertTrue(IDifference.providedBy(diff))
         self.assertFalse(diff.same)
         # The script tag should be escaped.
         self.assertNotIn("<script", diff.inline_diff())
         self.assertIn("&gt;", diff.inline_diff())
 
         # Test the more basic BinaryDiff.
         # It only compares the file names.
         # It uses the 'getFilename' method of the file,
         # which namedfiles do not have.  So we hack it.
         obj1.file.getFilename = lambda: obj1.file.filename
         obj2.file.getFilename = lambda: obj2.file.filename
-        diff = BinaryDiff.BinaryDiff(obj1, obj2, 'file')
+        diff = BinaryDiff.BinaryDiff(obj1, obj2, "file")
         self.assertTrue(IDifference.providedBy(diff))
         self.assertFalse(diff.same)
         # The script tag should be escaped.
         self.assertNotIn("<script", diff.inline_diff())
         self.assertIn("&gt;", diff.inline_diff())
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_choicediff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_choicediff.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from Products.CMFDiffTool import testing
 from Products.CMFDiffTool.choicediff import ChoiceDiff
 from Products.CMFDiffTool.choicediff import title_or_value
 from Products.CMFDiffTool.interfaces import IDifference
 from Products.CMFDiffTool.tests.BaseTestCase import BaseDXTestCase
 
 
 class ChoiceDiffTestCase(BaseDXTestCase):
-
     def setUp(self):
-        self.portal = self.layer['portal']
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        self.portal = self.layer["portal"]
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
+            "obj1",
         )
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
+            "obj2",
         )
 
-        self.obj1 = self.portal['obj1']
-        self.obj2 = self.portal['obj2']
+        self.obj1 = self.portal["obj1"]
+        self.obj2 = self.portal["obj2"]
 
     def test_should_diff_choice_field(self):
-        self._test_diff_choice(testing.VOCABULARY_TUPLES[0][0],
-                               testing.VOCABULARY_TUPLES[0][0], True)
-        self._test_diff_choice(testing.VOCABULARY_TUPLES[0][0],
-                               testing.VOCABULARY_TUPLES[1][0], False)
-        self._test_diff_choice(testing.VOCABULARY_TUPLES[1][0],
-                               testing.VOCABULARY_TUPLES[0][0], False)
-        self._test_diff_choice(testing.VOCABULARY_TUPLES[1][0],
-                               testing.VOCABULARY_TUPLES[1][0], True)
+        self._test_diff_choice(
+            testing.VOCABULARY_TUPLES[0][0], testing.VOCABULARY_TUPLES[0][0], True
+        )
+        self._test_diff_choice(
+            testing.VOCABULARY_TUPLES[0][0], testing.VOCABULARY_TUPLES[1][0], False
+        )
+        self._test_diff_choice(
+            testing.VOCABULARY_TUPLES[1][0], testing.VOCABULARY_TUPLES[0][0], False
+        )
+        self._test_diff_choice(
+            testing.VOCABULARY_TUPLES[1][0], testing.VOCABULARY_TUPLES[1][0], True
+        )
 
         self._test_diff_choice(testing.VOCABULARY_TUPLES[0][0], None, False)
         self._test_diff_choice(testing.VOCABULARY_TUPLES[1][0], None, False)
         self._test_diff_choice(None, testing.VOCABULARY_TUPLES[0][0], False)
         self._test_diff_choice(None, testing.VOCABULARY_TUPLES[1][0], False)
         self._test_diff_choice(None, None, True)
 
     def _test_diff_choice(self, value1, value2, same):
         self.obj1.choice = value1
         self.obj2.choice = value2
-        diff = ChoiceDiff(self.obj1, self.obj2, 'choice')
+        diff = ChoiceDiff(self.obj1, self.obj2, "choice")
         self.assertTrue(IDifference.providedBy(diff))
         self.assertEqual(diff.same, same)
 
         inline_diff = diff.inline_diff()
         if same:
             self.assertFalse(inline_diff)
         else:
             if value1 is not None:
                 self.assertTrue(
-                    title_or_value(testing.VOCABULARY, value1) in inline_diff)
+                    title_or_value(testing.VOCABULARY, value1) in inline_diff
+                )
             if value2 is not None:
                 self.assertTrue(
-                    title_or_value(testing.VOCABULARY, value2) in inline_diff)
+                    title_or_value(testing.VOCABULARY, value2) in inline_diff
+                )
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_dexteritydiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_dexteritydiff.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from datetime import date
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.namedfile import NamedFile
 from Products.CMFDiffTool import testing
 from Products.CMFDiffTool.dexteritydiff import DexterityCompoundDiff
 from Products.CMFDiffTool.dexteritydiff import EXCLUDED_FIELDS
@@ -10,150 +9,148 @@
 from Products.CMFDiffTool.tests.BaseTestCase import BaseDXTestCase
 from z3c.relationfield.relation import RelationValue
 from zope.component import getUtility
 from zope.intid.interfaces import IIntIds
 
 
 class DexterityDiffTestCase(BaseDXTestCase):
-
     def setUp(self):
-        self.portal = self.layer['portal']
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        self.portal = self.layer["portal"]
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
     def test_should_diff(self):
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
-            title=u'Object 1',
-            description=u'Desc 1',
-            text=u'Text 1',
+            "obj1",
+            title="Object 1",
+            description="Desc 1",
+            text="Text 1",
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
-            title=u'Object 2',
-            text=u'Text 2',
+            "obj2",
+            title="Object 2",
+            text="Text 2",
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diffs = DexterityCompoundDiff(obj1, obj2, 'any')
+        diffs = DexterityCompoundDiff(obj1, obj2, "any")
         for d in diffs:
             self.assertTrue(IDifference.providedBy(d))
             self.assertFalse(d.field in EXCLUDED_FIELDS)
-            if d.field in ['title', 'description', 'text']:
-                self.assertFalse(
-                    d.same, 'Field %s should be different.' % d.field)
+            if d.field in ["title", "description", "text"]:
+                self.assertFalse(d.same, "Field %s should be different." % d.field)
             else:
-                self.assertTrue(d.same, 'Field %s should be equal.' % d.field)
+                self.assertTrue(d.same, "Field %s should be equal." % d.field)
 
     def test_should_provide_inline_diff_for_date_field(self):
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
+            "obj1",
             date=date(2001, 1, 1),
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
+            "obj2",
             date=date(2001, 1, 2),
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diffs = DexterityCompoundDiff(obj1, obj2, 'any')
+        diffs = DexterityCompoundDiff(obj1, obj2, "any")
         for d in diffs:
-            if d.field == 'date':
+            if d.field == "date":
                 self.assertTrue(d.inline_diff())
 
     def test_should_provide_inline_diff_for_file_list_field(self):
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
+            "obj1",
             files=None,
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
-            files=[NamedFile(data='data', filename=u'a.txt')],
+            "obj2",
+            files=[NamedFile(data="data", filename="a.txt")],
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diffs = DexterityCompoundDiff(obj1, obj2, 'any')
+        diffs = DexterityCompoundDiff(obj1, obj2, "any")
         for d in diffs:
-            if d.field == 'files':
+            if d.field == "files":
                 inline_diff = d.inline_diff()
                 self.assertTrue(inline_diff)
                 self.assertTrue(obj2.files[0].filename in inline_diff)
 
     def test_should_provide_diff_for_behaviors_fields(self):
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
+            "obj1",
             date=date(2001, 1, 1),
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
+            "obj2",
             date=date(2001, 1, 2),
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
-        diffs = DexterityCompoundDiff(obj1, obj2, 'any')
+        diffs = DexterityCompoundDiff(obj1, obj2, "any")
         fields = [d.field for d in diffs]
-        self.assertIn('title', fields)
-        self.assertIn('description', fields)
+        self.assertIn("title", fields)
+        self.assertIn("description", fields)
 
     def test_should_provide_diff_for_related_fields(self):
         intids = getUtility(IIntIds)
 
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj1',
-            title=u'Object 1',
-            description=u'Desc 1',
-            text=u'Text 1',
+            "obj1",
+            title="Object 1",
+            description="Desc 1",
+            text="Text 1",
         )
-        obj1 = self.portal['obj1']
+        obj1 = self.portal["obj1"]
 
         intid = intids.register(obj1)
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj2',
-            title=u'Object 2',
+            "obj2",
+            title="Object 2",
             relatedItems=[RelationValue(intid)],
         )
-        obj2 = self.portal['obj2']
+        obj2 = self.portal["obj2"]
 
         intid = intids.register(obj2)
         self.portal.invokeFactory(
             testing.TEST_CONTENT_TYPE_ID,
-            'obj3',
-            title=u'Object 3',
+            "obj3",
+            title="Object 3",
             relatedItems=[RelationValue(intid)],
         )
-        obj3 = self.portal['obj3']
+        obj3 = self.portal["obj3"]
 
-        diffs = DexterityCompoundDiff(obj2, obj3, 'any')
+        diffs = DexterityCompoundDiff(obj2, obj3, "any")
         for d in diffs:
-            if d.field == 'relatedItems':
+            if d.field == "relatedItems":
                 inline_diff = d.inline_diff()
                 self.assertTrue(inline_diff)
                 i_diff_sub = inline_diff.index('<div class="diff_sub">')
-                i_obj1 = inline_diff.index('Object 1')
+                i_obj1 = inline_diff.index("Object 1")
                 i_diff_add = inline_diff.index('<div class="diff_add">')
-                i_obj2 = inline_diff.index('Object 2')
+                i_obj2 = inline_diff.index("Object 2")
                 self.assertTrue(i_diff_sub < i_obj1 < i_diff_add < i_obj2)
 
                 n_diff = d.ndiff()
                 self.assertTrue(n_diff)
-                i_rem = n_diff.index('-')
-                i_obj1 = n_diff.index('obj1')
-                i_add = n_diff.index('+')
-                i_obj2 = n_diff.index('obj2')
+                i_rem = n_diff.index("-")
+                i_obj1 = n_diff.index("obj1")
+                i_add = n_diff.index("+")
+                i_obj2 = n_diff.index("obj2")
                 self.assertTrue(i_rem < i_obj1 < i_add < i_obj2)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_filelistdiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_filelistdiff.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,81 @@
-# -*- coding: utf-8 -*-
 from plone.namedfile import NamedFile
 from Products.CMFDiffTool import namedfile
 from Products.CMFDiffTool.interfaces import IDifference
 
 import unittest
 
 
-class DummyType(object):
+class DummyType:
     def __init__(self, files):
         """`files` is a sequence of (data, filename) tuples."""
-        self.files = files and [
-            NamedFile(data=d, filename=fn) for (d, fn) in files]
+        self.files = files and [NamedFile(data=d, filename=fn) for (d, fn) in files]
 
 
 class AsTextDiffTestCase(unittest.TestCase):
-
     def test_should_diff_file_lists_correctly(self):
         self._test_diff_files(
-            [('data1', u'filename1')],
-            [('data2', u'filename2')],
+            [("data1", "filename1")],
+            [("data2", "filename2")],
             False,
         )
         self._test_diff_files(
-            [('data1', u'filename1'), ('datax', u'filenamex')],
-            [('data1', u'filename1'), ('datay', u'filenamey')],
+            [("data1", "filename1"), ("datax", "filenamex")],
+            [("data1", "filename1"), ("datay", "filenamey")],
             False,
         )
         self._test_diff_files(
-            [('data1', u'filename1'), ('datax', u'filenamex')],
-            [('datax', u'filenamex'), ('data1', u'filename1')],
+            [("data1", "filename1"), ("datax", "filenamex")],
+            [("datax", "filenamex"), ("data1", "filename1")],
             False,
         )
         self._test_diff_files(
-            [('data1', u'filename1')],
-            [('data1', u'filename1'), ('datax', u'filenamex')],
+            [("data1", "filename1")],
+            [("data1", "filename1"), ("datax", "filenamex")],
             False,
         )
         self._test_diff_files(
-            [('data1', u'filename1')],
-            [('data1', u'filename1')],
+            [("data1", "filename1")],
+            [("data1", "filename1")],
             True,
         )
         self._test_diff_files(
-            [('data1', u'filename1'), ('datax', u'filenamex')],
-            [('data1', u'filename1'), ('datax', u'filenamex')],
+            [("data1", "filename1"), ("datax", "filenamex")],
+            [("data1", "filename1"), ("datax", "filenamex")],
             True,
         )
         self._test_diff_files(
-            [('data1', u'filename1'), ('datax', u'filenamex')],
+            [("data1", "filename1"), ("datax", "filenamex")],
             None,
             False,
         )
         self._test_diff_files(
-            [('data1', u'filename1'), ('datax', u'filenamex')],
+            [("data1", "filename1"), ("datax", "filenamex")],
             [],
             False,
         )
         self._test_diff_files(
             [
-                ('<script>alert("Hacker data 1")</script>', u'filename1'),
-                ('<script>alert("Hacker data 2")</script>', u'filename2'),
+                ('<script>alert("Hacker data 1")</script>', "filename1"),
+                ('<script>alert("Hacker data 2")</script>', "filename2"),
             ],
             [
-                ('data1', u'<script>alert("Hacker data")</script>.txt'),
-                ('<script>alert("Hacker data 2")</script>', u'filename2'),
+                ("data1", '<script>alert("Hacker data")</script>.txt'),
+                ('<script>alert("Hacker data 2")</script>', "filename2"),
             ],
             False,
         )
         self._test_diff_files(None, None, True)
         self._test_diff_files([], [], True)
         self._test_diff_files([], None, True)
 
     def _test_diff_files(self, files1, files2, same):
         diff = namedfile.NamedFileListDiff(
-            DummyType(files1), DummyType(files2), 'files')
+            DummyType(files1), DummyType(files2), "files"
+        )
         self.assertTrue(IDifference.providedBy(diff))
         self.assertEqual(diff.same, same)
         inline = diff.inline_diff()
         self.assertNotEqual(bool(inline), same)
         if inline:
             # No hacker can catch us unawares.
             self.assertNotIn("<script", inline)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_install.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_install.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-# -*- coding: utf-8 -*-
 from Products.CMFCore.utils import getToolByName
 from Products.CMFDiffTool.dexteritydiff import DexterityCompoundDiff
 from Products.CMFDiffTool.tests.BaseTestCase import BaseDXTestCase
 
 
 class InstallTestCase(BaseDXTestCase):
-
     def test_compound_diff_type_should_be_registered(self):
-        diff_tool = getToolByName(self.portal, 'portal_diff')
-        self.assertTrue(
-            DexterityCompoundDiff.meta_type in diff_tool.listDiffTypes())
-        self.assertTrue(
-            diff_tool.getDiffType(DexterityCompoundDiff.meta_type))
+        diff_tool = getToolByName(self.portal, "portal_diff")
+        self.assertTrue(DexterityCompoundDiff.meta_type in diff_tool.listDiffTypes())
+        self.assertTrue(diff_tool.getDiffType(DexterityCompoundDiff.meta_type))
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/tests/test_richtextdiff.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/tests/test_richtextdiff.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,72 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import PLONE_INTEGRATION_TESTING
 from plone.app.textfield.value import RichTextValue
 from Products.CMFDiffTool.CMFDTHtmlDiff import CMFDTHtmlDiff
 from Products.CMFDiffTool.interfaces import IDifference
 
 import unittest
 
 
-class DummyType(object):
+class DummyType:
     def __init__(self, body):
         self.body = body
 
 
 class RichTextDiffTestCase(unittest.TestCase):
     """Test RichTextDiff"""
+
     layer = PLONE_INTEGRATION_TESTING
 
     def test_parseField_value_is_none(self):
         value = None
-        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), 'body')
+        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), "body")
         self.assertEqual(diff._parseField(value), [])
 
     def test_parseField_value_is_not_none(self):
-        value = RichTextValue(u'foo')
-        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), 'body')
-        self.assertEqual(diff._parseField(value), [u'foo'])
+        value = RichTextValue("foo")
+        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), "body")
+        self.assertEqual(diff._parseField(value), ["foo"])
 
     def test_inline_diff_same(self):
-        value = RichTextValue(u'foo')
-        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), 'body')
+        value = RichTextValue("foo")
+        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), "body")
         inline_diff = diff.inline_diff()
 
         self.assertTrue(IDifference.providedBy(diff))
         self.assertEqual(diff.same, True)
-        self.assertEqual(inline_diff, u'foo ')
+        self.assertEqual(inline_diff, "foo ")
 
     def test_inline_diff_same_hacker(self):
-        value = RichTextValue(u'<script>alert("Hacker value")</script>')
-        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), 'body')
+        value = RichTextValue('<script>alert("Hacker value")</script>')
+        diff = CMFDTHtmlDiff(DummyType(value), DummyType(value), "body")
         inline_diff = diff.inline_diff()
         # The script tag should not be escaped, but totally not shown.
         self.assertNotIn("<script", inline_diff)
         self.assertNotIn("&gt;", inline_diff)
 
     def test_inline_diff_different(self):
-        old_value = RichTextValue(u'foo')
-        new_value = RichTextValue(u'foo bar')
-        diff = CMFDTHtmlDiff(
-            DummyType(old_value), DummyType(new_value), 'body')
+        old_value = RichTextValue("foo")
+        new_value = RichTextValue("foo bar")
+        diff = CMFDTHtmlDiff(DummyType(old_value), DummyType(new_value), "body")
 
         inline_diff = diff.inline_diff()
 
         self.assertTrue(IDifference.providedBy(diff))
         self.assertEqual(diff.same, False)
-        self.assertEqual(inline_diff, u'foo <span class="insert">bar </span> ')
+        self.assertEqual(inline_diff, 'foo <span class="insert">bar </span> ')
 
     def test_inline_diff_different_hacker(self):
-        old_value = RichTextValue(u'clean')
-        new_value = RichTextValue(u'<script>alert("Hacker value")</script>')
-        diff = CMFDTHtmlDiff(DummyType(old_value), DummyType(new_value), 'body')
+        old_value = RichTextValue("clean")
+        new_value = RichTextValue('<script>alert("Hacker value")</script>')
+        diff = CMFDTHtmlDiff(DummyType(old_value), DummyType(new_value), "body")
         inline_diff = diff.inline_diff()
         # The script tag should not be escaped, but totally not shown.
         self.assertNotIn("<script", inline_diff)
         self.assertNotIn("&gt;", inline_diff)
 
-        old_value = RichTextValue(u'<script>alert("Hacker value")</script>')
-        new_value = RichTextValue(u'clean')
-        diff = CMFDTHtmlDiff(DummyType(old_value), DummyType(new_value), 'body')
+        old_value = RichTextValue('<script>alert("Hacker value")</script>')
+        new_value = RichTextValue("clean")
+        diff = CMFDTHtmlDiff(DummyType(old_value), DummyType(new_value), "body")
         inline_diff = diff.inline_diff()
         # The script tag should not be escaped, but totally not shown.
         self.assertNotIn("<script", inline_diff)
         self.assertNotIn("&gt;", inline_diff)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/utils.py` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 def safe_unicode(value):
     if isinstance(value, str):
         return value
     try:
         value = str(value)
     except UnicodeDecodeError:
-        value = value.decode('utf-8', 'replace')
+        value = value.decode("utf-8", "replace")
     return value
 
 
 def safe_utf8(value):
-    return safe_unicode(value).encode('utf-8')
+    return safe_unicode(value).encode("utf-8")
 
 
 def scrub_html(value):
     # Strip illegal HTML tags from string text.
     transform = SafeHTML()
     return transform.scrub_html(value)
 
@@ -33,10 +33,11 @@
 # This gets inserted in a string/text.
 
 
 def html_escape(value):
     value = safe_unicode(value)
     return escape(value, 1)
 
+
 def html_safe(value):
     value = safe_unicode(value)
     return scrub_html(value)
```

### Comparing `Products.CMFDiffTool-4.0.0/Products/CMFDiffTool/zpt/editCMFDiffTool.zpt` & `Products.CMFDiffTool-4.0.1/Products/CMFDiffTool/zpt/editCMFDiffTool.zpt`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,154 @@
 <html tal:omit-tag="">
   <span tal:replace="structure here/manage_page_header">Header</span>
-  <span tal:define="manage_tabs_message options/manage_tabs_message | nothing"
-    tal:replace="structure here/manage_tabs">Tabs</span>
+  <span tal:define="
+          manage_tabs_message options/manage_tabs_message | nothing;
+        "
+        tal:replace="structure here/manage_tabs"
+  >Tabs</span>
 
 
   <style>
     #diffTable {
       border-collapse: collapse;
       margin-bottom: 1em;
     }
 
     #diffTable td { padding: 1ex; }
 
-    .lastrow td { 
-      border-bottom: 1px solid black; 
+    .lastrow td {
+      border-bottom: 1px solid black;
     }
   </style>
 
   <h3>Differences by Type</h3>
-  
-  <form action="manage_addDiffField" method="post">
+
+  <form action="manage_addDiffField"
+        method="post"
+  >
     <table>
       <tr>
-    <th>Portal Type</th>
-    <th>Field name</th>
-    <th>Diff Type</th>
+        <th>Portal Type</th>
+        <th>Field name</th>
+        <th>Diff Type</th>
       </tr>
       <tr>
-    <td>
-      <select name="pt_name">
-        <option tal:repeat="pt here/portal_types/listTypeInfo"
-                tal:attributes="value pt/id;"
-                tal:content="pt/id">[group]</option>
-      </select>
-    </td>
-    <td>
-      <input type="text" name="field" />
-    </td>
-    <td>
-      <select name="diff">
-        <option tal:repeat="d here/listDiffTypes"
-            tal:attributes="value d;"
-            tal:content="d">[group]</option>
-      </select>
-    </td>
-    <td>
-      <input type="submit" name="add" value="Add field" />
-    </td>
+        <td>
+          <select name="pt_name">
+            <option tal:repeat="pt here/portal_types/listTypeInfo"
+                    tal:content="pt/id"
+                    tal:attributes="
+                      value pt/id;
+                    "
+            >[group]</option>
+          </select>
+        </td>
+        <td>
+          <input name="field"
+                 type="text"
+          />
+        </td>
+        <td>
+          <select name="diff">
+            <option tal:repeat="d here/listDiffTypes"
+                    tal:content="d"
+                    tal:attributes="
+                      value d;
+                    "
+            >[group]</option>
+          </select>
+        </td>
+        <td>
+          <input name="add"
+                 type="submit"
+                 value="Add field"
+          />
+        </td>
       </tr>
     </table>
   </form>
 
-  <form action="." method="post">
+  <form action="."
+        method="post"
+  >
 
     <table id="diffTable">
       <thead>
-    <tr>
-      <th>Portal Type</th>
-      <th>Field</th>
-      <th>Diff Type</th>
-      <th>Delete</th>
-    </tr>
+        <tr>
+          <th>Portal Type</th>
+          <th>Field</th>
+          <th>Diff Type</th>
+          <th>Delete</th>
+        </tr>
       </thead>
       <tal:p_type tal:repeat="pt_name here/portal_types/listContentTypes">
-    <tal:defs tal:define="diff_map python:here.getDiffForPortalType(pt_name)" tal:condition="diff_map">
-      <tr tal:repeat="pair diff_map/items" tal:attributes="class python:test(repeat['pair'].end, 'lastrow', nothing)">
-        <tal:defs tal:define="field python:pair[0]; difftype python:pair[1];">
-
-          <td class="form-label">
-        <a tal:condition="repeat/pair/start" 
-                   tal:attributes="href string:../portal_types/$pt_name/manage_workspace" 
-                   tal:content="pt_name">[pt_name]</a>
-          </td>
-
-          <td class="form-label" tal:content="field">[field]</td>
-          <td class="form-element">
-        <select name="updates.diff:records">
-          <option tal:repeat="d here/listDiffTypes"
-                   tal:content="d"
-               tal:attributes="value d;
-                                           selected python:test(d == difftype, 'selected' ,nothing);">
+        <tal:defs tal:define="
+                    diff_map python:here.getDiffForPortalType(pt_name);
+                  "
+                  tal:condition="diff_map"
+        >
+          <tr tal:repeat="pair diff_map/items"
+              tal:attributes="
+                class python:test(repeat['pair'].end, 'lastrow', nothing);
+              "
+          >
+            <tal:defs tal:define="
+                        field python:pair[0];
+                        difftype python:pair[1];
+                      ">
+
+              <td class="form-label">
+                <a tal:condition="repeat/pair/start"
+                   tal:content="pt_name"
+                   tal:attributes="
+                     href string:../portal_types/$pt_name/manage_workspace;
+                   "
+                >[pt_name]</a>
+              </td>
+
+              <td class="form-label"
+                  tal:content="field"
+              >[field]</td>
+              <td class="form-element">
+                <select name="updates.diff:records">
+                  <option tal:repeat="d here/listDiffTypes"
+                          tal:content="d"
+                          tal:attributes="
+                            value d;
+                            selected python:test(d == difftype, 'selected' ,nothing);
+                          "
+                  >
             [group]
-          </option>
-        </select>
-          </td>
-          <td align="center">
-        <input type="hidden" name="updates.pt_name:records" tal:attributes="value pt_name" />
-        <input type="hidden" name="updates.field:records" tal:attributes="value field" />
-        <input type="checkbox" name="updates.delete:records" />
-          </td>
+                  </option>
+                </select>
+              </td>
+              <td align="center">
+                <input name="updates.pt_name:records"
+                       type="hidden"
+                       tal:attributes="
+                         value pt_name;
+                       "
+                />
+                <input name="updates.field:records"
+                       type="hidden"
+                       tal:attributes="
+                         value field;
+                       "
+                />
+                <input name="updates.delete:records"
+                       type="checkbox"
+                />
+              </td>
+            </tal:defs>
+          </tr>
         </tal:defs>
-      </tr>   
-    </tal:defs>   
       </tal:p_type>
     </table>
-    
-    <input type="submit" name="manage_editDiffFields:action" value="Update" />
+
+    <input name="manage_editDiffFields:action"
+           type="submit"
+           value="Update"
+    />
   </form>
-  
+
   <span tal:replace="structure here/manage_page_footer">Footer</span>
 </html>
```

### Comparing `Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/PKG-INFO` & `Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CMFDiffTool
-Version: 4.0.0
+Version: 4.0.1
 Summary: Diff tool for Plone
 Home-page: https://github.com/plone/Products.CMFDiffTool
 Author: Brent Hendricks
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Diff Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,14 +52,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 4.0.0 (2023-03-14)
 ------------------
 
 Breaking changes:
 
 
 - Drop compatibility with Plone 5.2, Python 2, Archetypes.
```

### Comparing `Products.CMFDiffTool-4.0.0/Products.CMFDiffTool.egg-info/SOURCES.txt` & `Products.CMFDiffTool-4.0.1/Products.CMFDiffTool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+.editorconfig
 .gitignore
 .isort.cfg
+.meta.toml
+.pre-commit-config.yaml
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 Products/__init__.py
 Products.CMFDiffTool.egg-info/PKG-INFO
 Products.CMFDiffTool.egg-info/SOURCES.txt
 Products.CMFDiffTool.egg-info/dependency_links.txt
 Products.CMFDiffTool.egg-info/entry_points.txt
 Products.CMFDiffTool.egg-info/namespace_packages.txt
 Products.CMFDiffTool.egg-info/not-zip-safe
```

### Comparing `Products.CMFDiffTool-4.0.0/README.rst` & `Products.CMFDiffTool-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFDiffTool-4.0.0/docs/LICENSE.GPL` & `Products.CMFDiffTool-4.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.CMFDiffTool-4.0.0/docs/LICENSE.txt` & `Products.CMFDiffTool-4.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

