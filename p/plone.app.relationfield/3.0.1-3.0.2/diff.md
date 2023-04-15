# Comparing `tmp/plone.app.relationfield-3.0.1.tar.gz` & `tmp/plone.app.relationfield-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.relationfield-3.0.1.tar", last modified: Mon Dec  5 09:05:31 2022, max compression
+gzip compressed data, was "plone.app.relationfield-3.0.2.tar", last modified: Sat Apr 15 08:03:23 2023, max compression
```

## Comparing `plone.app.relationfield-3.0.1.tar` & `plone.app.relationfield-3.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.203088 plone.app.relationfield-3.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     5267 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      150 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     6869 2022-12-05 09:05:31.203210 plone.app.relationfield-3.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      714 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.190877 plone.app.relationfield-3.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      703 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      752 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.191144 plone.app.relationfield-3.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.193350 plone.app.relationfield-3.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.200731 plone.app.relationfield-3.0.1/plone/app/relationfield/
--rw-r--r--   0 maurits    (501) staff       (20)      281 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      553 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)     1212 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)     2714 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      758 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/demo.py
--rw-r--r--   0 maurits    (501) staff       (20)      485 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/demo.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1407 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/event.py
--rw-r--r--   0 maurits    (501) staff       (20)      138 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      825 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/marshaler.py
--rw-r--r--   0 maurits    (501) staff       (20)     2376 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/marshaler.rst
--rw-r--r--   0 maurits    (501) staff       (20)      382 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/marshaler.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      767 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/monkey.py
--rw-r--r--   0 maurits    (501) staff       (20)      843 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/path.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.188033 plone.app.relationfield-3.0.1/plone/app/relationfield/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.201295 plone.app.relationfield-3.0.1/plone/app/relationfield/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)       23 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/profiles/default/install_relations.txt
--rw-r--r--   0 maurits    (501) staff       (20)      164 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2845 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     6006 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1200 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5812 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor_contenttree.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1116 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1425 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/source.py
--rw-r--r--   0 maurits    (501) staff       (20)     2109 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     5860 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/supermodel.txt
--rw-r--r--   0 maurits    (501) staff       (20)      409 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/supermodel.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5985 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/supermodel_contenttree.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3719 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.202861 plone.app.relationfield-3.0.1/plone/app/relationfield/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      683 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/tests/test_marshall.py
--rw-r--r--   0 maurits    (501) staff       (20)      289 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/tests/test_marshall.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      988 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/tests/test_schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)      992 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/tests/test_supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2278 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/tests/test_widget.py
--rw-r--r--   0 maurits    (501) staff       (20)     5964 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/widget.py
--rw-r--r--   0 maurits    (501) staff       (20)     1159 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/plone/app/relationfield/widget.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-05 09:05:31.193079 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     6869 2022-12-05 09:05:31.000000 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1899 2022-12-05 09:05:31.000000 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-12-05 09:05:31.000000 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-12-05 09:05:31.000000 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-12-05 09:05:31.000000 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      354 2022-12-05 09:05:31.000000 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-12-05 09:05:31.000000 plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      461 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      290 2022-12-05 09:05:31.203709 plone.app.relationfield-3.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2043 2022-12-05 09:05:30.000000 plone.app.relationfield-3.0.1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/
+-rw-r--r--   0 gil       (1000) gil       (1000)     5376 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      150 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     6978 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      714 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.651490 plone.app.relationfield-3.0.2/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)      703 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/docs/INSTALL.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      752 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.651490 plone.app.relationfield-3.0.2/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.652490 plone.app.relationfield-3.0.2/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/plone/app/relationfield/
+-rw-r--r--   0 gil       (1000) gil       (1000)      257 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      524 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/adapter.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1165 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/behavior.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2768 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      731 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/demo.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      457 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/demo.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     1378 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/event.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      114 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      779 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2376 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      393 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      743 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/monkey.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      806 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/path.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.650490 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)       23 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/default/install_relations.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      181 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2786 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6006 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1205 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     5812 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor_contenttree.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1092 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/setuphandlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1362 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/source.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1921 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5860 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      406 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     5985 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel_contenttree.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     3670 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.655490 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      659 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_marshall.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      321 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_marshall.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      647 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_schemaeditor.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      651 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_supermodel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2254 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_widget.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5571 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/widget.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1141 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone/app/relationfield/widget.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:03:23.652490 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     6978 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1899 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      512 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1694 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 08:03:23.656490 plone.app.relationfield-3.0.2/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     2292 2023-04-15 08:03:23.000000 plone.app.relationfield-3.0.2/setup.py
```

### Comparing `plone.app.relationfield-3.0.1/CHANGES.rst` & `plone.app.relationfield-3.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 3.0.1 (2022-12-05)
 ------------------
 
 Bug fixes:
 
 
 - Remove deprecated ``plone.app.widgets`` code.
```

### Comparing `plone.app.relationfield-3.0.1/PKG-INFO` & `plone.app.relationfield-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.relationfield
-Version: 3.0.1
+Version: 3.0.2
 Summary: Plone support for z3c.relationfield
 Home-page: https://pypi.org/project/plone.app.relationfield
 Author: Alec Mitchell
 Author-email: apm13@columbia.edu
 License: GPL
 Keywords: dexterity relations plone zc.relation
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 3.0.1 (2022-12-05)
 ------------------
 
 Bug fixes:
 
 
 - Remove deprecated ``plone.app.widgets`` code.
```

### Comparing `plone.app.relationfield-3.0.1/README.rst` & `plone.app.relationfield-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/docs/INSTALL.txt` & `plone.app.relationfield-3.0.2/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/docs/LICENSE.GPL` & `plone.app.relationfield-3.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/docs/LICENSE.txt` & `plone.app.relationfield-3.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/adapter.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/adapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from plone.uuid.interfaces import ATTRIBUTE_NAME
 from plone.uuid.interfaces import IUUID
 from z3c.relationfield.interfaces import IRelationValue
 from zope.component import adapter
 from zope.interface import implementer
 
 
 @implementer(IUUID)
 @adapter(IRelationValue)
 def rvUUID(context):
-    """ Vocabulary validation via p.a.vocabularies CatalogSource
-        requires the UUID of the target object to verify membership
+    """Vocabulary validation via p.a.vocabularies CatalogSource
+    requires the UUID of the target object to verify membership
     """
     return getattr(aq_base(context.to_object), ATTRIBUTE_NAME, None)
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/behavior.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/behavior.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-# -*- coding: utf-8 -*-
 from plone.app.dexterity import _
 from plone.app.z3cform.widget import RelatedItemsFieldWidget
 from plone.autoform import directives as form
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.supermodel import model
 from plone.supermodel.directives import fieldset
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope.interface import provider
 
 
 @provider(IFormFieldProvider)
 class IRelatedItems(model.Schema):
-    """Behavior interface to make a Dexterity type support related items.
-    """
+    """Behavior interface to make a Dexterity type support related items."""
 
     relatedItems = RelationList(
-        title=_(u'label_related_items', default=u'Related Items'),
+        title=_("label_related_items", default="Related Items"),
         default=[],
         value_type=RelationChoice(
-            title=u'Related', vocabulary='plone.app.vocabularies.Catalog'
+            title="Related", vocabulary="plone.app.vocabularies.Catalog"
         ),
         required=False,
     )
     form.widget(
-        'relatedItems',
+        "relatedItems",
         RelatedItemsFieldWidget,
-        vocabulary='plone.app.vocabularies.Catalog',
+        vocabulary="plone.app.vocabularies.Catalog",
         pattern_options={
-            'recentlyUsed': True  # Just turn on. Config in plone.app.widgets.
+            "recentlyUsed": True  # Just turn on. Config in plone.app.widgets.
         },
     )
 
-    fieldset(
-        'categorization', label=_(u'Categorization'), fields=['relatedItems']
-    )
+    fieldset("categorization", label=_("Categorization"), fields=["relatedItems"])
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/configure.zcml` & `plone.app.relationfield-3.0.2/plone/app/relationfield/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    xmlns:plone="http://namespaces.plone.org/plone"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    xmlns:plone="http://namespaces.plone.org/plone">
+    >
 
   <!-- Only use intids for objects with relations -->
   <include package="plone.app.intid" />
   <include package="z3c.relationfield" />
 
   <utility factory=".path.Zope2ObjectPath" />
 
   <!-- setup GS profile -->
   <genericsetup:registerProfile
       name="default"
       title="Relation Field"
       description="Adds support for content relationships defined using z3c.relationfield"
-      directory="profiles/default"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       for="Products.CMFPlone.interfaces.IPloneSiteRoot"
+      directory="profiles/default"
       />
 
   <genericsetup:importStep
       name="import-relations-utils"
       title="Import Relations Utils"
       description="Import relation utility."
-      handler=".setuphandlers.installRelations">
-     <depends name="toolset"/>
+      handler=".setuphandlers.installRelations"
+      >
+    <depends name="toolset" />
   </genericsetup:importStep>
 
   <!-- Dexterity Content will support incoming and outgoing relations -->
   <configure zcml:condition="installed plone.dexterity">
-    <include package="plone.behavior" file="meta.zcml" />
+    <include
+        package="plone.behavior"
+        file="meta.zcml"
+        />
     <class class="plone.dexterity.content.DexterityContent">
       <implements interface=".interfaces.IDexterityHasRelations" />
     </class>
     <subscriber
-      for="plone.dexterity.interfaces.IDexterityContent
-           zope.lifecycleevent.interfaces.IObjectModifiedEvent"
-      handler=".event.update_behavior_relations"
-      />
+        for="plone.dexterity.interfaces.IDexterityContent
+             zope.lifecycleevent.interfaces.IObjectModifiedEvent"
+        handler=".event.update_behavior_relations"
+        />
     <!-- Make 'related items' behavior available if plone.behavior is present. -->
     <plone:behavior
-        zcml:condition="installed plone.behavior"
-        title="Related items"
         name="plone.relateditems"
+        title="Related items"
         description="Adds the ability to assign related items"
         provides=".behavior.IRelatedItems"
+        zcml:condition="installed plone.behavior"
         />
   </configure>
 
   <!-- Archetypes Content will support incoming relations -->
-  <class zcml:condition="installed Products.Archetypes"
-         class="Products.Archetypes.BaseObject.BaseObject">
+  <class
+      class="Products.Archetypes.BaseObject.BaseObject"
+      zcml:condition="installed Products.Archetypes"
+      >
     <implements interface="z3c.relationfield.interfaces.IHasIncomingRelations" />
   </class>
 
   <!-- p.a.vocabularies needs UUID support from RelatedValues -->
   <adapter factory=".adapter.rvUUID" />
 
   <!-- widgets setup -->
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/event.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.behavior.interfaces import IBehaviorAssignable
 from z3c.relationfield.event import _setRelation
 from z3c.relationfield.interfaces import IRelation
 from z3c.relationfield.interfaces import IRelationList
 from zope.schema import getFields
 
 
@@ -27,11 +26,10 @@
                     continue
                 if rel_list is not None:
                     for relation in rel_list:
                         yield behavior.interface, name, relation
 
 
 def update_behavior_relations(obj, event):
-    """Re-register relations in behaviors
-    """
+    """Re-register relations in behaviors"""
     for behavior_interface, name, relation in extract_relations(obj):
         _setRelation(obj, name, relation)
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/marshaler.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-# -*- coding: utf-8 -*-
 from plone.rfc822.defaultfields import BaseFieldMarshaler
 from z3c.relationfield import RelationValue
 
-import six
-
 
 class RelationFieldMarshaler(BaseFieldMarshaler):
     """Field marshaler for z3c.relationfield IRelation and IRelationChoice
     fields
     """
 
     ascii = True
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         if value is None:
             return None
         return str(value.to_id)
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
-        if isinstance(value, six.binary_type):
+        if isinstance(value, bytes):
             value = value.decode(charset)
         try:
             toId = int(value)
         except TypeError as e:
             raise ValueError(e)
         return RelationValue(toId)
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/marshaler.rst` & `plone.app.relationfield-3.0.2/plone/app/relationfield/marshaler.rst`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/monkey.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/monkey.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# -*- coding: utf-8 -*-
 from z3c.relationfield.relation import _object
 from z3c.relationfield.relation import RelationValue
 from zope.component import getUtility
 from zope.intid.interfaces import IIntIds
 
 
 PATCHES = None
 
 
 def get_from_object(self):
-    if getattr(self, '_from_id', None):
+    if getattr(self, "_from_id", None):
         return _object(self._from_id)
     else:
         intids = getUtility(IIntIds)
 
         # Heya, is there no from_object? Please have a look at #12802
 
-        self._from_id = intids.register(self.__dict__['from_object'])
+        self._from_id = intids.register(self.__dict__["from_object"])
         return _object(self._from_id)
 
 
 def set_from_object(self, obj):
     if not obj:
         return
     intids = getUtility(IIntIds)
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/path.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/path.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# -*- coding: utf-8 -*-
 from z3c.objpath.interfaces import IObjectPath
 from zExceptions import NotFound
 from zope.component.hooks import getSite
 from zope.interface import implementer
 
 
 @implementer(IObjectPath)
-class Zope2ObjectPath(object):
-    """Path representation for Zope 2 objects.
-    """
+class Zope2ObjectPath:
+    """Path representation for Zope 2 objects."""
 
     def path(self, obj):
         try:
-            return '/'.join(obj.getPhysicalPath())
+            return "/".join(obj.getPhysicalPath())
         except AttributeError:
             raise ValueError(obj)
 
     def resolve(self, path):
         site = getSite()
         if site is None:
             raise ValueError(path)
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.vocabularies.catalog import CatalogSource
 from plone.schemaeditor.fields import FieldFactory
 from plone.schemaeditor.interfaces import IFieldEditFormSchema
 from plone.schemaeditor.interfaces import IFieldFactory
 from z3c.relationfield import interfaces
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
@@ -10,93 +9,90 @@
 from zope.component import adapter
 from zope.component import queryUtility
 from zope.i18n import MessageFactory
 from zope.interface import implementer
 from zope.intid.interfaces import IIntIds
 
 
-_ = MessageFactory('plone')
+_ = MessageFactory("plone")
 
 
 @implementer(IFieldFactory)
 class RelationFieldFactory(FieldFactory):
     def available(self):
         return queryUtility(IIntIds) is not None
 
 
 class IRelationFieldSettings(schema.interfaces.IField):
-
     portal_type = schema.Set(
-        title=_(u'Types'),
-        description=_(u'Allowed target types'),
+        title=_("Types"),
+        description=_("Allowed target types"),
         value_type=schema.Choice(
-            title=_(u'Type'),
-            vocabulary='plone.app.vocabularies.ReallyUserFriendlyTypes',
+            title=_("Type"),
+            vocabulary="plone.app.vocabularies.ReallyUserFriendlyTypes",
         ),
         required=False,
     )
 
 
 @adapter(interfaces.IRelationChoice)
 @implementer(IFieldEditFormSchema)
 def getRelationChoiceEditFormSchema(field):
     return IRelationFieldSettings
 
 
-class RelationChoiceEditFormAdapter(object):
+class RelationChoiceEditFormAdapter:
     def __init__(self, field):
         self.field = field
 
     @property
     def portal_type(self):
         field = self.field
         types = []
-        types.extend(field.source.query.get('portal_type') or [])
+        types.extend(field.source.query.get("portal_type") or [])
         return types
 
     @portal_type.setter
     def portal_type(self, value):
         field = self.field
         if value:
-            field.source.query['portal_type'] = list(value)
-        elif 'portal_type' in field.source.query:
-            del field.source.query['portal_type']
+            field.source.query["portal_type"] = list(value)
+        elif "portal_type" in field.source.query:
+            del field.source.query["portal_type"]
 
 
 RelationChoiceFactory = RelationFieldFactory(
-    RelationChoice, _('Relation Choice'), source=CatalogSource()
+    RelationChoice, _("Relation Choice"), source=CatalogSource()
 )
 
 
 @adapter(interfaces.IRelationList)
 @implementer(IFieldEditFormSchema)
 def getRelationListEditFormSchema(field):
     return IRelationFieldSettings
 
 
-class RelationListEditFormAdapter(object):
+class RelationListEditFormAdapter:
     def __init__(self, field):
         self.field = field
 
     @property
     def portal_type(self):
         field = self.field.value_type
         types = []
-        types.extend(field.source.query.get('portal_type') or [])
+        types.extend(field.source.query.get("portal_type") or [])
         return set(types)
 
     @portal_type.setter
     def portal_type(self, value):
         field = self.field.value_type
         if value:
-            field.source.query['portal_type'] = list(value)
-        elif 'portal_type' in field.source.query:
-            del field.source.query['portal_type']
+            field.source.query["portal_type"] = list(value)
+        elif "portal_type" in field.source.query:
+            del field.source.query["portal_type"]
 
 
 RelationListFactory = RelationFieldFactory(
     RelationList,
-    _('Relation List'),
-    value_type=RelationChoice(
-        title=_(u'Relation Choice'), source=CatalogSource()
-    ),
+    _("Relation List"),
+    value_type=RelationChoice(title=_("Relation Choice"), source=CatalogSource()),
 )
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor.txt` & `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor.zcml` & `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    i18n_domain="plone.app.relationfield">
+    i18n_domain="plone.app.relationfield"
+    >
 
   <include package="plone.schemaeditor" />
 
   <adapter
+      factory=".schemaeditor.getRelationChoiceEditFormSchema"
       provides="plone.schemaeditor.interfaces.IFieldEditFormSchema"
       for="z3c.relationfield.interfaces.IRelationChoice"
-      factory=".schemaeditor.getRelationChoiceEditFormSchema"
       />
 
   <adapter
+      factory=".schemaeditor.RelationChoiceEditFormAdapter"
       provides=".schemaeditor.IRelationFieldSettings"
       for="z3c.relationfield.interfaces.IRelationChoice"
-      factory=".schemaeditor.RelationChoiceEditFormAdapter"
       />
 
   <utility
       name="z3c.relationfield.schema.RelationChoice"
       component=".schemaeditor.RelationChoiceFactory"
       />
 
   <adapter
+      factory=".schemaeditor.getRelationListEditFormSchema"
       provides="plone.schemaeditor.interfaces.IFieldEditFormSchema"
       for="z3c.relationfield.interfaces.IRelationList"
-      factory=".schemaeditor.getRelationListEditFormSchema"
       />
 
   <adapter
+      factory=".schemaeditor.RelationListEditFormAdapter"
       provides=".schemaeditor.IRelationFieldSettings"
       for="z3c.relationfield.interfaces.IRelationList"
-      factory=".schemaeditor.RelationListEditFormAdapter"
       />
 
   <utility
       name="z3c.relationfield.schema.RelationList"
       component=".schemaeditor.RelationListFactory"
       />
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/schemaeditor_contenttree.txt` & `plone.app.relationfield-3.0.2/plone/app/relationfield/schemaeditor_contenttree.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/setuphandlers.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/setuphandlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-# -*- coding: utf-8 -*-
 from five.intid.intid import IntIds
 from five.intid.site import addUtility
 from z3c.relationfield.index import RelationCatalog
 from z3c.relationfield.interfaces import IRelationValue
 from zc.relation.interfaces import ICatalog
 from zope.intid.interfaces import IIntIds
 
 import BTrees
 
 
 PLONE_RELATION_INDEXES = [
-    {'element': IRelationValue['from_id']},
-    {'element': IRelationValue['to_id']},
+    {"element": IRelationValue["from_id"]},
+    {"element": IRelationValue["to_id"]},
     {
-        'element': IRelationValue['from_attribute'],
-        'kwargs': {'btree': BTrees.family32.OI},
+        "element": IRelationValue["from_attribute"],
+        "kwargs": {"btree": BTrees.family32.OI},
     },
 ]
 
 
 def relation_catalog_factory():
     return RelationCatalog(indexes=PLONE_RELATION_INDEXES)
 
 
 def add_relations(context):
     addUtility(
         context,
         ICatalog,
         relation_catalog_factory,
-        ofs_name='relations',
+        ofs_name="relations",
         findroot=False,
     )
 
 
 def add_intids(context):
-    addUtility(context, IIntIds, IntIds, ofs_name='intids', findroot=False)
+    addUtility(context, IIntIds, IntIds, ofs_name="intids", findroot=False)
 
 
 def installRelations(context):
-    if context.readDataFile('install_relations.txt') is None:
+    if context.readDataFile("install_relations.txt") is None:
         return
     portal = context.getSite()
     add_relations(portal)
-    return 'Added relations utility.'
+    return "Added relations utility."
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/source.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 from Products.CMFCore.utils import getToolByName
 from z3c.formwidget.query.interfaces import IQuerySource
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.intid.interfaces import IIntIds
 from zope.schema.vocabulary import SimpleVocabulary
 
 
 @implementer(IQuerySource)
-class CMFContentSearchSource(object):
+class CMFContentSearchSource:
     def __init__(self, context):
         self.context = context
         self.intid_utility = getUtility(IIntIds)
 
     def __contains__(self, term):
         return self.intid_utility.queryId(term) is not None
 
@@ -27,18 +26,16 @@
             obj, self.intid_utility.getId(obj), obj.Title()
         )
 
     def getTermByToken(self, value):
         return self.getTerm(self.intid_utility.getObject(int(value)))
 
     def search(self, query_string):
-        catalog = getToolByName(self.context, 'portal_catalog')
-        result = catalog(
-            SearchableText='{0:s}*'.format(query_string), sort_limit=20
-        )
+        catalog = getToolByName(self.context, "portal_catalog")
+        result = catalog(SearchableText=f"{query_string:s}*", sort_limit=20)
         terms = []
         for brain in result:
             try:
                 term = self.getTerm(brain.getObject())
             except KeyError:
                 # An object without an intid in the catalog results
                 continue
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/supermodel.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-# -*- coding: utf-8 -*-
 from plone.app.vocabularies.catalog import CatalogSource
 from plone.supermodel.exportimport import BaseHandler
 from plone.supermodel.utils import valueToElement
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope import schema
 
 
 class RelationChoiceBaseHandler(BaseHandler):
-
     filteredAttributes = BaseHandler.filteredAttributes.copy()
     filteredAttributes.update(
         {
-            'portal_type': 'w',
-            'source': 'rw',
-            'vocabulary': 'rw',
-            'vocabularyName': 'rw',
+            "portal_type": "w",
+            "source": "rw",
+            "vocabulary": "rw",
+            "vocabularyName": "rw",
         }
     )
 
     def __init__(self, klass):
-        super(RelationChoiceBaseHandler, self).__init__(klass)
+        super().__init__(klass)
 
-        self.fieldAttributes['portal_type'] = schema.List(
-            __name__='portal_type',
-            title=u'Allowed target types',
-            value_type=schema.Text(title=u'Type'),
+        self.fieldAttributes["portal_type"] = schema.List(
+            __name__="portal_type",
+            title="Allowed target types",
+            value_type=schema.Text(title="Type"),
         )
 
     def _constructField(self, attributes):
         portal_type = (
-            attributes.get('portal_type')
-            or attributes.get('portal_types')
-            or []
+            attributes.get("portal_type") or attributes.get("portal_types") or []
         )
-        if 'portal_type' in attributes:
-            del attributes['portal_type']
+        if "portal_type" in attributes:
+            del attributes["portal_type"]
 
         if not portal_type:
-            attributes['source'] = CatalogSource()
+            attributes["source"] = CatalogSource()
         else:
-            attributes['source'] = CatalogSource(portal_type=portal_type)
+            attributes["source"] = CatalogSource(portal_type=portal_type)
 
-        return super(RelationChoiceBaseHandler, self)._constructField(
-            attributes
-        )
+        return super()._constructField(attributes)
 
-    def write(self, field, name, type, elementName='field'):
-        element = super(RelationChoiceBaseHandler, self).write(
-            field, name, type, elementName
-        )
+    def write(self, field, name, type, elementName="field"):
+        element = super().write(field, name, type, elementName)
         portal_type = []
 
-        portal_type.extend(field.source.query.get('portal_type') or [])
+        portal_type.extend(field.source.query.get("portal_type") or [])
 
         if portal_type:
-            attributeField = self.fieldAttributes['portal_type']
+            attributeField = self.fieldAttributes["portal_type"]
             child = valueToElement(
-                attributeField, portal_type, name='portal_type', force=True
+                attributeField, portal_type, name="portal_type", force=True
             )
             element.append(child)
 
         return element
 
 
 RelationChoiceHandler = RelationChoiceBaseHandler(RelationChoice)
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/supermodel.txt` & `plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/supermodel_contenttree.txt` & `plone.app.relationfield-3.0.2/plone/app/relationfield/supermodel_contenttree.txt`

 * *Files identical despite different names*

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/testing.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from persistent import Persistent
 from plone.app.relationfield import HAS_CONTENTTYPES
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from z3c.relationfield import RelationList
 from z3c.relationfield.interfaces import IHasRelations
@@ -13,39 +12,39 @@
 
 
 if HAS_CONTENTTYPES:
     from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 
 
 class IAddress(Interface):
-    streetname = zope.schema.TextLine(title=u'Street name')
-    city = zope.schema.TextLine(title=u'City')
+    streetname = zope.schema.TextLine(title="Street name")
+    city = zope.schema.TextLine(title="City")
 
 
 @implementer(IAddress, IHasRelations)
 class Address(Persistent):
-    __name__ = u''
-    streetname = u''
-    city = u''
+    __name__ = ""
+    streetname = ""
+    city = ""
 
     def __init__(self, streetname, city):
         self.streetname = streetname
         self.city = city
-        __name__ = '{streetname} - {city}'.format(**locals())
+        self.__name__ = f"{streetname} - {city}"
 
 
 class IPerson(zope.interface.Interface):
-    name = zope.schema.TextLine(title=u'Name', default=u'<no name>')
-    phone = zope.schema.TextLine(title=u'Phone')
-    addresses = RelationList(title=u'Addresses')
+    name = zope.schema.TextLine(title="Name", default="<no name>")
+    phone = zope.schema.TextLine(title="Phone")
+    addresses = RelationList(title="Addresses")
 
 
 @implementer(IPerson, IHasRelations)
 class Person(Persistent):
-    name = u''
+    name = ""
 
     def __init__(self, name):
         self.name = name
 
 
 class PloneAppRelationfieldFixture(PloneSandboxLayer):
     if HAS_CONTENTTYPES:
@@ -55,25 +54,24 @@
 
     def setUpZope(self, app, configurationContext):
         import plone.app.relationfield
 
         self.loadZCML(package=plone.app.relationfield)
 
     def setUpPloneSite(self, portal):
-        self.applyProfile(portal, 'plone.app.relationfield:default')
+        self.applyProfile(portal, "plone.app.relationfield:default")
 
 
 FIXTURE = PloneAppRelationfieldFixture()
 FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(FIXTURE,), name='plone.app.relationfield:Functional'
+    bases=(FIXTURE,), name="plone.app.relationfield:Functional"
 )
 
 
 class PloneAppRelationfieldContentTreeFixture(PloneSandboxLayer):
-
     if HAS_CONTENTTYPES:
         defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
     else:
         defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import plone.app.dexterity
@@ -85,29 +83,28 @@
         self.loadZCML(package=plone.formwidget.contenttree)
 
         import plone.app.relationfield
 
         self.loadZCML(package=plone.app.relationfield)
 
     def setUpPloneSite(self, portal):
-        self.applyProfile(portal, 'plone.app.dexterity:default')
-        self.applyProfile(portal, 'plone.formwidget.contenttree:default')
-        self.applyProfile(portal, 'plone.app.relationfield:default')
+        self.applyProfile(portal, "plone.app.dexterity:default")
+        self.applyProfile(portal, "plone.formwidget.contenttree:default")
+        self.applyProfile(portal, "plone.app.relationfield:default")
 
 
 CONTENTTREE_FIXTURE = PloneAppRelationfieldContentTreeFixture()
 
 FUNCTIONAL_CONTENTTREE_TESTING = FunctionalTesting(
     bases=(CONTENTTREE_FIXTURE,),
-    name='plone.app.relationfield.contenttree:Functional',
+    name="plone.app.relationfield.contenttree:Functional",
 )
 
 
 class PloneAppRelationfieldWidgetsFixture(PloneSandboxLayer):
-
     if HAS_CONTENTTYPES:
         defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
     else:
         defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import plone.app.dexterity
@@ -115,17 +112,17 @@
         self.loadZCML(package=plone.app.dexterity)
 
         import plone.app.relationfield
 
         self.loadZCML(package=plone.app.relationfield)
 
     def setUpPloneSite(self, portal):
-        self.applyProfile(portal, 'plone.app.dexterity:default')
-        self.applyProfile(portal, 'plone.app.relationfield:default')
+        self.applyProfile(portal, "plone.app.dexterity:default")
+        self.applyProfile(portal, "plone.app.relationfield:default")
 
 
 WIDGETS_FIXTURE = PloneAppRelationfieldWidgetsFixture()
 
 FUNCTIONAL_WIDGETS_TESTING = FunctionalTesting(
     bases=(WIDGETS_FIXTURE,),
-    name='plone.app.relationfield.contenttree:Functional',
+    name="plone.app.relationfield.contenttree:Functional",
 )
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/tests/test_schemaeditor.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_marshall.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,27 @@
-# -*- coding: utf-8 -*-
-from plone.app.relationfield.testing import FUNCTIONAL_WIDGETS_TESTING
 from plone.testing import layered
+from plone.testing.zca import ZCMLSandbox
+from unittest import TestSuite
 
 import doctest
-import os
-import six
-import re
-import unittest
+import plone.app.relationfield.tests
 
 
-optionflags = doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
-
-
-class Py23DocChecker(doctest.OutputChecker):
-    def check_output(self, want, got, optionflags):
-        if six.PY2:
-            got = re.sub("u'(.*?)'", "'\\1'", got)
-        return doctest.OutputChecker.check_output(self, want, got, optionflags)
+ZCML_SANDBOX = ZCMLSandbox(
+    filename="test_marshall.zcml", package=plone.app.relationfield.tests
+)
 
 
 def test_suite():
-    suite = unittest.TestSuite()
-    suite.addTests(
-        [
-            layered(
-                doctest.DocFileSuite(
-                    os.path.join(os.path.pardir, 'schemaeditor.txt'),
-                    optionflags=optionflags,
-                    checker=Py23DocChecker(),
-                ),
-                FUNCTIONAL_WIDGETS_TESTING,
-            )
-        ]
+    suite = TestSuite()
+    OPTIONFLAGS = doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
+    suite.addTest(
+        layered(
+            doctest.DocFileSuite(
+                "../marshaler.rst",
+                optionflags=OPTIONFLAGS,
+                package="plone.app.relationfield.tests",
+            ),
+            layer=ZCML_SANDBOX,
+        )
     )
     return suite
-
-
-if __name__ == '__main__':
-    unittest.main(default='test_suite')
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/tests/test_widget.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/tests/test_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.relationfield.testing import Address
 from plone.app.relationfield.testing import FUNCTIONAL_TESTING
 from plone.app.relationfield.testing import IPerson
 from plone.app.relationfield.testing import Person
 from plone.app.relationfield.widget import RelationListDictDataManager
 from z3c.form.interfaces import IDataManager
 from z3c.relationfield.interfaces import IRelationValue
@@ -13,49 +12,49 @@
 import unittest
 
 
 class RelationListDictDataManagerTest(unittest.TestCase):
     layer = FUNCTIONAL_TESTING
 
     def setUp(self):
-        portal = self.layer['portal']
+        portal = self.layer["portal"]
         intids = getUtility(IIntIds)
 
-        self.person = portal.person = person = Person('Roel Bruggink')
+        self.person = portal.person = person = Person("Roel Bruggink")
         person.__parent__ = portal
 
         self.addresses = person.addresses = addresses = []
-        for streetname in ['Jansbinnensingel', 'Willemsplein']:
-            address = Address(streetname, 'Arnhem')
+        for streetname in ["Jansbinnensingel", "Willemsplein"]:
+            address = Address(streetname, "Arnhem")
             addresses.append(address)
 
             # five.intids' register expect aq wrapped objects, but __parent__
             # works just fine.
             address.__parent__ = portal
 
             intids.register(address)
 
     def test_get_datamanger(self):
-        dm = getMultiAdapter(({}, IPerson['addresses']), IDataManager)
+        dm = getMultiAdapter(({}, IPerson["addresses"]), IDataManager)
         self.assertTrue(isinstance(dm, RelationListDictDataManager))
 
     def test_datamanager_get_empty(self):
-        dm = RelationListDictDataManager({}, IPerson['addresses'])
+        dm = RelationListDictDataManager({}, IPerson["addresses"])
         self.assertEqual(dm.get(), [])
 
     def test_datamanager_set_empty(self):
-        dm = RelationListDictDataManager({}, IPerson['addresses'])
+        dm = RelationListDictDataManager({}, IPerson["addresses"])
         dm.set([])
         self.assertEqual(dm.get(), [])
 
     def test_datamanager_set_nonempty(self):
-        dm = RelationListDictDataManager({}, IPerson['addresses'])
+        dm = RelationListDictDataManager({}, IPerson["addresses"])
         dm.set(self.person.addresses)
         self.assertEqual(dm.get(), self.person.addresses)
 
     def test_datamanager_should_contain_relationvalues(self):
-        dm = RelationListDictDataManager({}, IPerson['addresses'])
+        dm = RelationListDictDataManager({}, IPerson["addresses"])
         dm.set(self.person.addresses)
 
-        storage = dm.data['addresses']
+        storage = dm.data["addresses"]
         self.assertNotEqual(storage, [])
         self.assertNotEqual(filter(IRelationValue.providedBy, storage), [])
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/widget.py` & `plone.app.relationfield-3.0.2/plone/app/relationfield/widget.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from z3c.form.datamanager import AttributeField
 from z3c.form.datamanager import DictionaryField
 from z3c.form.interfaces import NO_VALUE
 from z3c.relationfield.interfaces import IRelation
 from z3c.relationfield.interfaces import IRelationList
 from z3c.relationfield.interfaces import IRelationValue
 from z3c.relationfield.relation import RelationValue
@@ -18,55 +17,55 @@
     """A data manager which uses the z3c.relationfield api to set
     relationships using a schema field."""
 
     def get(self):
         """Gets the target"""
         rel = None
         try:
-            rel = super(RelationDataManager, self).get()
+            rel = super().get()
         except AttributeError:
             # Not set yet
             pass
         if rel is not None:
             if rel.isBroken():
                 # XXX: should log or take action here
                 return
             return rel.to_object
 
     def set(self, value):
         """Sets the relationship target"""
         if value is None:
-            return super(RelationDataManager, self).set(None)
+            return super().set(None)
 
         current = None
         try:
-            current = super(RelationDataManager, self).get()
+            current = super().get()
         except AttributeError:
             pass
         intids = getUtility(IIntIds)
         to_id = intids.getId(value)
         if IRelationValue.providedBy(current):
             # If we already have a relation, just set the to_id
             current.to_id = to_id
         else:
             # otherwise create a relationship
             rel = RelationValue(to_id)
-            super(RelationDataManager, self).set(rel)
+            super().set(rel)
 
 
 @adapter(dict, IRelation)
 class RelationDictDataManager(DictionaryField):
     """A data manager which uses the z3c.relationfield api to set
     relationships using a schema field, for dict-like contexts."""
 
     def get(self):
         """Gets the target"""
         rel = None
         try:
-            rel = super(RelationDictDataManager, self).get()
+            rel = super().get()
         except AttributeError:
             # Not set yet
             pass
         if rel is not None:
             if rel.isBroken():
                 # XXX: should log or take action here
                 return
@@ -76,50 +75,50 @@
         """See z3c.form.interfaces.IDataManager"""
         try:
             return self.get()
         except ForbiddenAttribute as e:
             raise e
         except AttributeError:
             if default == NO_VALUE:
-                return super(RelationDictDataManager, self).query()
+                return super().query()
             else:
                 return default
 
     def set(self, value):
         """Sets the relationship target"""
         if value is None:
-            return super(RelationDictDataManager, self).set(None)
+            return super().set(None)
 
         current = None
         try:
-            current = super(RelationDictDataManager, self).get()
+            current = super().get()
         except AttributeError:
             pass
         intids = getUtility(IIntIds)
         to_id = intids.getId(value)
         if IRelationValue.providedBy(current):
             # If we already have a relation, just set the to_id
             current.to_id = to_id
         else:
             # otherwise create a relationship
             rel = RelationValue(to_id)
-            super(RelationDictDataManager, self).set(rel)
+            super().set(rel)
 
 
 @adapter(Interface, IRelationList)
 class RelationListDataManager(AttributeField):
     """A data manager which sets a list of relations"""
 
     def get(self):
         """Gets the target"""
         rel_list = []
 
         # Calling query() here will lead to infinite recursion!
         try:
-            rel_list = super(RelationListDataManager, self).get()
+            rel_list = super().get()
 
         except AttributeError:
             rel_list = None
 
         if not rel_list:
             return []
 
@@ -136,28 +135,28 @@
         value = value or []
         new_relationships = []
         intids = getUtility(IIntIds)
         for item in value:
             # otherwise create one
             to_id = intids.getId(item)
             new_relationships.append(RelationValue(to_id))
-        super(RelationListDataManager, self).set(new_relationships)
+        super().set(new_relationships)
 
 
 @adapter(dict, IRelationList)
 class RelationListDictDataManager(DictionaryField):
     """A data manager which sets a list of relations on dictionary"""
 
     def get(self):
         """Gets the target"""
         rel_list = []
 
         # Calling query() here will lead to infinite recursion!
         try:
-            rel_list = super(RelationListDictDataManager, self).get()
+            rel_list = super().get()
         except AttributeError:
             rel_list = None
 
         if not rel_list:
             return []
 
         resolved_list = []
@@ -182,8 +181,8 @@
         value = value or []
         new_relationships = []
         intids = getUtility(IIntIds)
         for item in value:
             # otherwise create one
             to_id = intids.getId(item)
             new_relationships.append(RelationValue(to_id))
-        super(RelationListDictDataManager, self).set(new_relationships)
+        super().set(new_relationships)
```

### Comparing `plone.app.relationfield-3.0.1/plone/app/relationfield/widget.zcml` & `plone.app.relationfield-3.0.2/plone/app/relationfield/widget.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:zcml="http://namespaces.zope.org/zcml"
     xmlns:browser="http://namespaces.zope.org/browser"
-    i18n_domain="plone.app.relationfield">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone.app.relationfield"
+    >
 
   <!-- Widget setup -->
 
   <adapter factory=".widget.RelationDataManager" />
   <adapter factory=".widget.RelationDictDataManager" />
   <adapter factory=".widget.RelationListDataManager" />
   <adapter factory=".widget.RelationListDictDataManager" />
 
-  <utility component=".source.CMFContentSearchSource"
-           name="plone.formwidget.relations.cmfcontentsearch"
-           provides="zope.schema.interfaces.IVocabularyFactory"
-           />
+  <utility
+      provides="zope.schema.interfaces.IVocabularyFactory"
+      name="plone.formwidget.relations.cmfcontentsearch"
+      component=".source.CMFContentSearchSource"
+      />
 
   <configure zcml:condition="installed plone.formwidget.contenttree">
-    <adapter factory="plone.formwidget.contenttree.ContentTreeFieldWidget"
-             for="z3c.relationfield.interfaces.IRelationChoice
-                  z3c.form.interfaces.IFormLayer"
-             />
-
-    <adapter factory="plone.formwidget.contenttree.MultiContentTreeFieldWidget"
-             for="z3c.relationfield.interfaces.IRelationList
-                  z3c.form.interfaces.IFormLayer"
-             />
+    <adapter
+        factory="plone.formwidget.contenttree.ContentTreeFieldWidget"
+        for="z3c.relationfield.interfaces.IRelationChoice
+             z3c.form.interfaces.IFormLayer"
+        />
+
+    <adapter
+        factory="plone.formwidget.contenttree.MultiContentTreeFieldWidget"
+        for="z3c.relationfield.interfaces.IRelationList
+             z3c.form.interfaces.IFormLayer"
+        />
   </configure>
 
 </configure>
```

### Comparing `plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/PKG-INFO` & `plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.relationfield
-Version: 3.0.1
+Version: 3.0.2
 Summary: Plone support for z3c.relationfield
 Home-page: https://pypi.org/project/plone.app.relationfield
 Author: Alec Mitchell
 Author-email: apm13@columbia.edu
 License: GPL
 Keywords: dexterity relations plone zc.relation
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 3.0.1 (2022-12-05)
 ------------------
 
 Bug fixes:
 
 
 - Remove deprecated ``plone.app.widgets`` code.
```

### Comparing `plone.app.relationfield-3.0.1/plone.app.relationfield.egg-info/SOURCES.txt` & `plone.app.relationfield-3.0.2/plone.app.relationfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

