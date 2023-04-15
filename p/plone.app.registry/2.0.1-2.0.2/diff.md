# Comparing `tmp/plone.app.registry-2.0.1.tar.gz` & `tmp/plone.app.registry-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.registry-2.0.1.tar", last modified: Sat Dec 10 02:13:13 2022, max compression
+gzip compressed data, was "plone.app.registry-2.0.2.tar", last modified: Sat Apr 15 07:47:22 2023, max compression
```

## Comparing `plone.app.registry-2.0.1.tar` & `plone.app.registry-2.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.241673 plone.app.registry-2.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    10759 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    39675 2022-12-10 02:13:13.241799 plone.app.registry-2.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    27968 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.231382 plone.app.registry-2.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1112 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      747 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)    78923 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/configuration_registry_add_record_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)    55440 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/configuration_registry_edit_record_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)    52471 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/configuration_registry_export_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)    55001 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/configuration_registry_import_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)   152613 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/docs/configuration_registry_screenshot.jpg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.231835 plone.app.registry-2.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.233717 plone.app.registry-2.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.234813 plone.app.registry-2.0.1/plone/app/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     1791 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)       49 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.236447 plone.app.registry-2.0.1/plone/app/registry/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1345 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2935 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      972 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     2380 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     4958 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/exportxml.py
--rw-r--r--   0 maurits    (501) staff       (20)     7845 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/records.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.237073 plone.app.registry-2.0.1/plone/app/registry/browser/resources/
--rw-r--r--   0 maurits    (501) staff       (20)      267 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/resources/icon.png
--rw-r--r--   0 maurits    (501) staff       (20)      490 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/resources/style.css
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.238277 plone.app.registry-2.0.1/plone/app/registry/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      866 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/templates/controlpanel_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1449 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/templates/delete_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)      871 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/templates/edit_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1173 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/templates/exportxml.pt
--rw-r--r--   0 maurits    (501) staff       (20)     8023 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/browser/templates/records.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.239373 plone.app.registry-2.0.1/plone/app/registry/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      914 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2008 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/exportimport/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)    16074 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/exportimport/handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     2360 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/exportimport/handlers.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.227285 plone.app.registry-2.0.1/plone/app/registry/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.240311 plone.app.registry-2.0.1/plone/app/registry/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      240 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      469 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      179 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      161 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/profiles/default/toolset.xml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/registry.py
--rw-r--r--   0 maurits    (501) staff       (20)      819 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.241491 plone.app.registry-2.0.1/plone/app/registry/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      410 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/tests/data.py
--rw-r--r--   0 maurits    (501) staff       (20)     3548 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/tests/test_controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    47016 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/tests/test_exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)      713 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/plone/app/registry/tests/test_setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-10 02:13:13.233466 plone.app.registry-2.0.1/plone.app.registry.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    39675 2022-12-10 02:13:13.000000 plone.app.registry-2.0.1/plone.app.registry.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2147 2022-12-10 02:13:13.000000 plone.app.registry-2.0.1/plone.app.registry.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-12-10 02:13:13.000000 plone.app.registry-2.0.1/plone.app.registry.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-12-10 02:13:13.000000 plone.app.registry-2.0.1/plone.app.registry.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-12-10 02:13:13.000000 plone.app.registry-2.0.1/plone.app.registry.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      157 2022-12-10 02:13:13.000000 plone.app.registry-2.0.1/plone.app.registry.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-12-10 02:13:13.000000 plone.app.registry-2.0.1/plone.app.registry.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      172 2022-12-10 02:13:13.242292 plone.app.registry-2.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1737 2022-12-10 02:13:12.000000 plone.app.registry-2.0.1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.301575 plone.app.registry-2.0.2/
+-rw-r--r--   0 gil       (1000) gil       (1000)    10868 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      149 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    39784 2023-04-15 07:47:22.301575 plone.app.registry-2.0.2/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)    27968 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.297575 plone.app.registry-2.0.2/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1112 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/INSTALL.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      747 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/LICENSE.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    78923 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/configuration_registry_add_record_screenshot.jpg
+-rw-r--r--   0 gil       (1000) gil       (1000)    55440 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/configuration_registry_edit_record_screenshot.jpg
+-rw-r--r--   0 gil       (1000) gil       (1000)    52471 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/configuration_registry_export_screenshot.jpg
+-rw-r--r--   0 gil       (1000) gil       (1000)    55001 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/configuration_registry_import_screenshot.jpg
+-rw-r--r--   0 gil       (1000) gil       (1000)   152613 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/docs/configuration_registry_screenshot.jpg
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.297575 plone.app.registry-2.0.2/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.298575 plone.app.registry-2.0.2/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.298575 plone.app.registry-2.0.2/plone/app/registry/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1791 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/README.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       63 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.299575 plone.app.registry-2.0.2/plone/app/registry/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1284 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2935 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/controlpanel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      972 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/delete.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2380 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/edit.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4958 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/exportxml.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7845 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/records.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.299575 plone.app.registry-2.0.2/plone/app/registry/browser/resources/
+-rw-r--r--   0 gil       (1000) gil       (1000)      267 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/resources/icon.png
+-rw-r--r--   0 gil       (1000) gil       (1000)      490 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/resources/style.css
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.299575 plone.app.registry-2.0.2/plone/app/registry/browser/templates/
+-rw-r--r--   0 gil       (1000) gil       (1000)      965 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/templates/controlpanel_layout.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1780 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/templates/delete_layout.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      993 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/templates/edit_layout.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1200 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/templates/exportxml.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     8023 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/browser/templates/records.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1029 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.300575 plone.app.registry-2.0.2/plone/app/registry/exportimport/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/exportimport/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      931 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/exportimport/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2008 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/exportimport/fields.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    16067 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/exportimport/handler.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2503 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/exportimport/handlers.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.295575 plone.app.registry-2.0.2/plone/app/registry/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.300575 plone.app.registry-2.0.2/plone/app/registry/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)      230 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/profiles/default/componentregistry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      594 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/profiles/default/controlpanel.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      187 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      166 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/profiles/default/toolset.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      274 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/registry.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      818 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.301575 plone.app.registry-2.0.2/plone/app/registry/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      408 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/tests/data.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3546 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/tests/test_controlpanel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    46848 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/tests/test_exportimport.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      711 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/plone/app/registry/tests/test_setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:47:22.297575 plone.app.registry-2.0.2/plone.app.registry.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    39784 2023-04-15 07:47:22.000000 plone.app.registry-2.0.2/plone.app.registry.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     2147 2023-04-15 07:47:22.000000 plone.app.registry-2.0.2/plone.app.registry.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:47:22.000000 plone.app.registry-2.0.2/plone.app.registry.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 07:47:22.000000 plone.app.registry-2.0.2/plone.app.registry.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:47:22.000000 plone.app.registry-2.0.2/plone.app.registry.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      232 2023-04-15 07:47:22.000000 plone.app.registry-2.0.2/plone.app.registry.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:47:22.000000 plone.app.registry-2.0.2/plone.app.registry.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1643 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:47:22.301575 plone.app.registry-2.0.2/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1871 2023-04-15 07:47:21.000000 plone.app.registry-2.0.2/setup.py
```

### Comparing `plone.app.registry-2.0.1/CHANGES.rst` & `plone.app.registry-2.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 2.0.1 (2022-12-10)
 ------------------
 
 Bug fixes:
 
 
 - Fix responsive table.
```

### Comparing `plone.app.registry-2.0.1/PKG-INFO` & `plone.app.registry-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.registry
-Version: 2.0.1
+Version: 2.0.2
 Summary: Zope 2 and Plone  integration for plone.registry
 Home-page: https://pypi.org/project/plone.app.registry
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
 License: GPL
 Keywords: plone registry settings configuration
 Classifier: Development Status :: 5 - Production/Stable
@@ -753,14 +753,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 2.0.1 (2022-12-10)
 ------------------
 
 Bug fixes:
 
 
 - Fix responsive table.
```

### Comparing `plone.app.registry-2.0.1/README.rst` & `plone.app.registry-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/INSTALL.txt` & `plone.app.registry-2.0.2/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/LICENSE.GPL` & `plone.app.registry-2.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/LICENSE.txt` & `plone.app.registry-2.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/configuration_registry_add_record_screenshot.jpg` & `plone.app.registry-2.0.2/docs/configuration_registry_add_record_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/configuration_registry_edit_record_screenshot.jpg` & `plone.app.registry-2.0.2/docs/configuration_registry_edit_record_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/configuration_registry_export_screenshot.jpg` & `plone.app.registry-2.0.2/docs/configuration_registry_export_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/configuration_registry_import_screenshot.jpg` & `plone.app.registry-2.0.2/docs/configuration_registry_import_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/docs/configuration_registry_screenshot.jpg` & `plone.app.registry-2.0.2/docs/configuration_registry_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/README.txt` & `plone.app.registry-2.0.2/plone/app/registry/README.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ======================
 
 
 
 class IMyPackage(Interface):
 
     field1 = TextLine(title="Field1", default="")
-    field2 = TextLine(title="Field2", defualt="Initial value")
+    field2 = TextLine(title="Field2", default="Initial value")
 
 
 
 #1 - change proposed
 
 XML:
 <records interface="my.package.IMyPackage" />
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/configure.zcml` & `plone.app.registry-2.0.2/plone/app/registry/browser/configure.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <include package="plone.app.z3cform" />
-    <include package="plone.autoform" />
+  <include package="plone.app.z3cform" />
+  <include package="plone.autoform" />
 
-    <!-- <browser:resourceDirectory
+  <!-- <browser:resourceDirectory
         name="plone.app.registry"
         directory="resources"
         /> -->
 
-    <browser:defaultView
-        for="plone.registry.interfaces.IRegistry"
-        name="configuration_registry"
-        />
-
-    <browser:page
-        name="configuration_registry"
-        for="plone.registry.interfaces.IRegistry"
-        class=".records.RecordsControlPanel"
-        permission="cmf.ManagePortal"
-        />
-
-    <browser:page
-        name="edit"
-        for="plone.registry.interfaces.IRegistry"
-        class=".edit.RecordEditView"
-        template="templates/edit_layout.pt"
-        permission="cmf.ManagePortal"
-        />
-
-    <browser:page
-        name="delete-record"
-        for="plone.registry.interfaces.IRegistry"
-        class=".delete.RecordDeleteView"
-        template="templates/delete_layout.pt"
-        permission="cmf.ManagePortal"
-        />
-
-    <browser:page
-        for="plone.registry.interfaces.IRegistry"
-        name="configuration_registry_export_xml"
-        class=".exportxml.RegistryExporterView"
-        permission="cmf.ManagePortal"
-        />
+  <browser:defaultView
+      name="configuration_registry"
+      for="plone.registry.interfaces.IRegistry"
+      />
+
+  <browser:page
+      name="configuration_registry"
+      for="plone.registry.interfaces.IRegistry"
+      class=".records.RecordsControlPanel"
+      permission="cmf.ManagePortal"
+      />
+
+  <browser:page
+      name="edit"
+      for="plone.registry.interfaces.IRegistry"
+      class=".edit.RecordEditView"
+      template="templates/edit_layout.pt"
+      permission="cmf.ManagePortal"
+      />
+
+  <browser:page
+      name="delete-record"
+      for="plone.registry.interfaces.IRegistry"
+      class=".delete.RecordDeleteView"
+      template="templates/delete_layout.pt"
+      permission="cmf.ManagePortal"
+      />
+
+  <browser:page
+      name="configuration_registry_export_xml"
+      for="plone.registry.interfaces.IRegistry"
+      class=".exportxml.RegistryExporterView"
+      permission="cmf.ManagePortal"
+      />
 
 </configure>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/controlpanel.py` & `plone.app.registry-2.0.2/plone/app/registry/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/delete.py` & `plone.app.registry-2.0.2/plone/app/registry/browser/delete.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/edit.py` & `plone.app.registry-2.0.2/plone/app/registry/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/exportxml.py` & `plone.app.registry-2.0.2/plone/app/registry/browser/exportxml.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/records.py` & `plone.app.registry-2.0.2/plone/app/registry/browser/records.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/templates/controlpanel_layout.pt` & `plone.app.registry-2.0.2/plone/app/registry/browser/templates/controlpanel_layout.pt`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="context/@@prefs_main_template/macros/master"
-      i18n:domain="plone">
+      xml:lang="en"
+      i18n:domain="plone"
+>
 
-<body>
-<tal:main metal:fill-slot="prefs_configlet_main">
+  <body>
+    <tal:main metal:fill-slot="prefs_configlet_main">
 
-  <header>
+      <header>
 
-    <h1 tal:content="view/label">View Title</h1>
-    <p class="lead" tal:condition="view/description | nothing" tal:content="structure view/description">View Description</p>
+        <h1 tal:content="view/label">View Title</h1>
+        <p class="lead"
+           tal:condition="view/description | nothing"
+           tal:content="structure view/description"
+        >View Description</p>
 
-  </header>
+      </header>
 
-  <div metal:use-macro="context/@@global_statusmessage/macros/portal_message">
+      <div metal:use-macro="context/@@global_statusmessage/macros/portal_message">
     Portal status message
-  </div>
+      </div>
 
-  <div id="content-core">
-    <div id="layout-contents">
-      <span tal:replace="structure view/contents" />
-    </div>
-  </div>
+      <div id="content-core">
+        <div id="layout-contents">
+          <span tal:replace="structure view/contents"></span>
+        </div>
+      </div>
 
-</tal:main>
-</body>
+    </tal:main>
+  </body>
 </html>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/templates/delete_layout.pt` & `plone.app.registry-2.0.2/plone/app/registry/browser/templates/delete_layout.pt`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,60 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="context/@@prefs_main_template/macros/master"
-      i18n:domain="plone">
-
-<metal:block fill-slot="top_slot"
-             tal:define="dummy python:request.set('disable_border',1)" />
-
-<body>
-<div id="content" metal:fill-slot="prefs_configlet_content">
-
-    <h1 class="documentFirstHeading" i18n:translate="">Delete Record</h1>
-
-    <p class="documentDescription" i18n:translate="description_record_delete">
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <metal:block fill-slot="top_slot"
+               tal:define="
+                 dummy python:request.set('disable_border',1);
+               "
+  />
+
+  <body>
+    <div id="content"
+         metal:fill-slot="prefs_configlet_content"
+    >
+
+      <h1 class="documentFirstHeading"
+          i18n:translate=""
+      >Delete Record</h1>
+
+      <p class="documentDescription"
+         i18n:translate="description_record_delete"
+      >
         Are you certain you want to delete this record? This can not be undone
         and can be potentially harmful if you don't know what you are doing.
-    </p>
+      </p>
 
-    <b i18n:translate="">Record</b>: ${request/form/name}
+      <b i18n:translate="">Record</b>: ${request/form/name}
 
-    <form method="POST">
-      <input type="hidden" name="name" value="${request/form/name}" />
-      <div class="formControls">
-        <input id="form-buttons-delete" name="form.buttons.delete" i18n:attributes="value"
-               class="submit-widget button-field btn btn-danger" value="Yes, delete" type="submit">
-        <input id="form-buttons-cancel" name="form.buttons.cancel" i18n:attributes="value"
-               class="submit-widget button-field btn btn-secondary" value="Cancel" type="submit">
-      </div>
-    </form>
+      <form method="POST">
+        <input name="name"
+               type="hidden"
+               value="${request/form/name}"
+        />
+        <div class="formControls">
+          <input class="submit-widget button-field btn btn-danger"
+                 id="form-buttons-delete"
+                 name="form.buttons.delete"
+                 type="submit"
+                 value="Yes, delete"
+                 i18n:attributes="value"
+          />
+          <input class="submit-widget button-field btn btn-secondary"
+                 id="form-buttons-cancel"
+                 name="form.buttons.cancel"
+                 type="submit"
+                 value="Cancel"
+                 i18n:attributes="value"
+          />
+        </div>
+      </form>
 
-</div>
-</body>
+    </div>
+  </body>
 </html>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/templates/edit_layout.pt` & `plone.app.registry-2.0.2/plone/app/registry/browser/templates/edit_layout.pt`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,38 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="context/@@prefs_main_template/macros/master"
-      i18n:domain="plone">
-
-<metal:block fill-slot="top_slot"
-             tal:define="dummy python:request.set('disable_border',1)" />
-
-<body>
-<div id="content" metal:fill-slot="prefs_configlet_content">
-
-    <h1 class="documentFirstHeading" tal:content="view/label">View Title</h1>
-
-    <p class="documentDescription" i18n:translate="description_record_edit">
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <metal:block fill-slot="top_slot"
+               tal:define="
+                 dummy python:request.set('disable_border',1);
+               "
+  />
+
+  <body>
+    <div id="content"
+         metal:fill-slot="prefs_configlet_content"
+    >
+
+      <h1 class="documentFirstHeading"
+          tal:content="view/label"
+      >View Title</h1>
+
+      <p class="documentDescription"
+         i18n:translate="description_record_edit"
+      >
         Use the form below to edit the value of this particular record.
-    </p>
+      </p>
 
-    <div id="layout-contents">
-        <span tal:replace="structure view/contents" />
-    </div>
+      <div id="layout-contents">
+        <span tal:replace="structure view/contents"></span>
+      </div>
 
-</div>
-</body>
+    </div>
+  </body>
 </html>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/templates/exportxml.pt` & `plone.app.registry-2.0.2/plone/app/registry/browser/templates/exportxml.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,75 @@
-00000000: 3c74 616c 3e0a 2020 2020 3c68 3320 6931  <tal>.    <h3 i1
-00000010: 386e 3a74 7261 6e73 6c61 7465 3d22 7265  8n:translate="re
-00000020: 6769 7374 7279 5f65 7870 6f72 745f 7061  gistry_export_pa
-00000030: 7274 735f 6865 6164 696e 6722 3e45 7870  rts_heading">Exp
-00000040: 6f72 7420 7061 7274 733c 2f68 333e 0a20  ort parts</h3>. 
-00000050: 2020 203c 7020 6931 386e 3a74 7261 6e73     <p i18n:trans
-00000060: 6c61 7465 3d22 7265 6769 7374 7279 5f65  late="registry_e
-00000070: 7870 6f72 745f 7061 7274 735f 7465 7874  xport_parts_text
-00000080: 223e 0a20 2020 2020 2044 6f77 6e6c 6f61  ">.      Downloa
-00000090: 6420 6f66 2061 2058 4d4c 2d66 696c 6520  d of a XML-file 
-000000a0: 6f70 7469 6d69 7a65 6420 746f 2062 6520  optimized to be 
-000000b0: 7573 6564 2069 6e20 6120 4765 6e65 7269  used in a Generi
-000000c0: 6353 6574 7570 2070 726f 6669 6c65 206f  cSetup profile o
-000000d0: 6620 616e 2061 6464 2d6f 6e20 6f72 2070  f an add-on or p
-000000e0: 6f6c 6963 7920 7072 6f66 696c 652e 0a20  olicy profile.. 
-000000f0: 2020 2020 2049 7420 636f 6e74 6169 6e73       It contains
-00000100: 206f 6e6c 7920 7468 6520 7365 6c65 6374   only the select
-00000110: 6564 2070 6172 7473 2e0a 2020 2020 3c2f  ed parts..    </
-00000120: 703e 0a0a 2020 2020 3c64 6976 2063 6c61  p>..    <div cla
-00000130: 7373 3d22 7061 742d 6175 746f 746f 6320  ss="pat-autotoc 
-00000140: 6175 746f 7461 6273 220a 2020 2020 2020  autotabs".      
-00000150: 2020 2064 6174 612d 7061 742d 6175 746f     data-pat-auto
-00000160: 746f 633d 226c 6576 656c 733a 2068 333b  toc="levels: h3;
-00000170: 2073 6563 7469 6f6e 3a20 6469 762e 6578   section: div.ex
-00000180: 706f 7274 7461 623b 2063 6c61 7373 4e61  porttab; classNa
-00000190: 6d65 3a20 6175 746f 7461 6273 223e 0a20  me: autotabs">. 
-000001a0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000001b0: 733d 2265 7870 6f72 7474 6162 220a 2020  s="exporttab".  
-000001c0: 2020 2020 2020 2020 2020 2069 643d 2265             id="e
-000001d0: 7870 6f72 742d 7365 6374 696f 6e2d 696e  xport-section-in
-000001e0: 7465 7266 6163 6573 223e 0a20 2020 2020  terfaces">.     
-000001f0: 2020 2020 203c 6833 2069 3138 6e3a 7472       <h3 i18n:tr
-00000200: 616e 736c 6174 653d 2272 6567 6973 7472  anslate="registr
-00000210: 795f 6578 706f 7274 5f70 6172 7473 5f6c  y_export_parts_l
-00000220: 6162 656c 5f69 6661 6365 2220 6964 3d22  abel_iface" id="
-00000230: 6833 2d69 6e74 6572 6661 6365 7322 3e62  h3-interfaces">b
-00000240: 7920 496e 7465 7266 6163 653c 2f68 333e  y Interface</h3>
-00000250: 0a20 2020 2020 2020 2020 203c 756c 2063  .          <ul c
-00000260: 6c61 7373 3d22 636f 6c6c 6170 7365 5f69  lass="collapse_i
-00000270: 6e74 6572 6661 6365 7322 3e0a 2020 2020  nterfaces">.    
-00000280: 2020 2020 2020 2020 3c6c 6920 7461 6c3a          <li tal:
-00000290: 7265 7065 6174 3d22 7072 6566 6978 2070  repeat="prefix p
-000002a0: 7974 686f 6e3a 7669 6577 2e69 6e74 6572  ython:view.inter
-000002b0: 6661 6365 7328 2922 3e3c 6120 7461 7267  faces()"><a targ
-000002c0: 6574 3d22 5f62 6c61 6e6b 2220 6872 6566  et="_blank" href
-000002d0: 3d22 247b 7079 7468 6f6e 3a70 7265 6669  ="${python:prefi
-000002e0: 785b 315d 7d22 3e24 7b70 7974 686f 6e3a  x[1]}">${python:
-000002f0: 7072 6566 6978 5b30 5d7d 3c2f 613e 3c2f  prefix[0]}</a></
-00000300: 6c69 3e0a 2020 2020 2020 2020 2020 3c2f  li>.          </
-00000310: 756c 3e0a 2020 2020 2020 2020 3c2f 6469  ul>.        </di
-00000320: 763e 0a20 2020 2020 2020 203c 6469 7620  v>.        <div 
-00000330: 636c 6173 733d 2265 7870 6f72 7474 6162  class="exporttab
-00000340: 220a 2020 2020 2020 2020 2020 2020 2069  ".             i
-00000350: 643d 2265 7870 6f72 742d 7365 6374 696f  d="export-sectio
-00000360: 6e2d 7072 6566 6978 6573 223e 0a20 2020  n-prefixes">.   
-00000370: 2020 2020 2020 203c 6833 2069 3138 6e3a         <h3 i18n:
-00000380: 7472 616e 736c 6174 653d 2272 6567 6973  translate="regis
-00000390: 7472 795f 6578 706f 7274 5f70 6172 7473  try_export_parts
-000003a0: 5f6c 6162 656c 5f70 7265 6669 7822 2069  _label_prefix" i
-000003b0: 643d 2268 332d 7072 6566 6978 6573 223e  d="h3-prefixes">
-000003c0: 6279 2050 7265 6669 783c 2f68 333e 0a20  by Prefix</h3>. 
-000003d0: 2020 2020 2020 2020 203c 756c 3e0a 2020           <ul>.  
-000003e0: 2020 2020 2020 2020 2020 3c6c 6920 7461            <li ta
-000003f0: 6c3a 7265 7065 6174 3d22 7072 6566 6978  l:repeat="prefix
-00000400: 2070 7974 686f 6e3a 7669 6577 2e70 7265   python:view.pre
-00000410: 6669 7865 7328 2922 3e3c 6120 7461 7267  fixes()"><a targ
-00000420: 6574 3d22 5f62 6c61 6e6b 2220 6872 6566  et="_blank" href
-00000430: 3d22 247b 7079 7468 6f6e 3a70 7265 6669  ="${python:prefi
-00000440: 785b 315d 7d22 3e24 7b70 7974 686f 6e3a  x[1]}">${python:
-00000450: 7072 6566 6978 5b30 5d7d 3c2f 613e 3c2f  prefix[0]}</a></
-00000460: 6c69 3e0a 2020 2020 2020 2020 2020 3c2f  li>.          </
-00000470: 756c 3e0a 2020 2020 2020 2020 3c2f 6469  ul>.        </di
-00000480: 763e 0a20 2020 203c 2f64 6976 3e0a 3c2f  v>.    </div>.</
-00000490: 7461 6c3e 0a                             tal>.
+00000000: 3c74 616c 3e0a 2020 3c68 3320 6931 386e  <tal>.  <h3 i18n
+00000010: 3a74 7261 6e73 6c61 7465 3d22 7265 6769  :translate="regi
+00000020: 7374 7279 5f65 7870 6f72 745f 7061 7274  stry_export_part
+00000030: 735f 6865 6164 696e 6722 3e45 7870 6f72  s_heading">Expor
+00000040: 7420 7061 7274 733c 2f68 333e 0a20 203c  t parts</h3>.  <
+00000050: 7020 6931 386e 3a74 7261 6e73 6c61 7465  p i18n:translate
+00000060: 3d22 7265 6769 7374 7279 5f65 7870 6f72  ="registry_expor
+00000070: 745f 7061 7274 735f 7465 7874 223e 0a20  t_parts_text">. 
+00000080: 2020 2020 2044 6f77 6e6c 6f61 6420 6f66       Download of
+00000090: 2061 2058 4d4c 2d66 696c 6520 6f70 7469   a XML-file opti
+000000a0: 6d69 7a65 6420 746f 2062 6520 7573 6564  mized to be used
+000000b0: 2069 6e20 6120 4765 6e65 7269 6353 6574   in a GenericSet
+000000c0: 7570 2070 726f 6669 6c65 206f 6620 616e  up profile of an
+000000d0: 2061 6464 2d6f 6e20 6f72 2070 6f6c 6963   add-on or polic
+000000e0: 7920 7072 6f66 696c 652e 0a20 2020 2020  y profile..     
+000000f0: 2049 7420 636f 6e74 6169 6e73 206f 6e6c   It contains onl
+00000100: 7920 7468 6520 7365 6c65 6374 6564 2070  y the selected p
+00000110: 6172 7473 2e0a 2020 3c2f 703e 0a0a 2020  arts..  </p>..  
+00000120: 3c64 6976 2063 6c61 7373 3d22 7061 742d  <div class="pat-
+00000130: 6175 746f 746f 6320 6175 746f 7461 6273  autotoc autotabs
+00000140: 220a 2020 2020 2020 2064 6174 612d 7061  ".       data-pa
+00000150: 742d 6175 746f 746f 633d 226c 6576 656c  t-autotoc="level
+00000160: 733a 2068 333b 2073 6563 7469 6f6e 3a20  s: h3; section: 
+00000170: 6469 762e 6578 706f 7274 7461 623b 2063  div.exporttab; c
+00000180: 6c61 7373 4e61 6d65 3a20 6175 746f 7461  lassName: autota
+00000190: 6273 220a 2020 3e0a 2020 2020 3c64 6976  bs".  >.    <div
+000001a0: 2063 6c61 7373 3d22 6578 706f 7274 7461   class="exportta
+000001b0: 6222 0a20 2020 2020 2020 2020 6964 3d22  b".         id="
+000001c0: 6578 706f 7274 2d73 6563 7469 6f6e 2d69  export-section-i
+000001d0: 6e74 6572 6661 6365 7322 0a20 2020 203e  nterfaces".    >
+000001e0: 0a20 2020 2020 203c 6833 2069 643d 2268  .      <h3 id="h
+000001f0: 332d 696e 7465 7266 6163 6573 220a 2020  3-interfaces".  
+00000200: 2020 2020 2020 2020 6931 386e 3a74 7261          i18n:tra
+00000210: 6e73 6c61 7465 3d22 7265 6769 7374 7279  nslate="registry
+00000220: 5f65 7870 6f72 745f 7061 7274 735f 6c61  _export_parts_la
+00000230: 6265 6c5f 6966 6163 6522 0a20 2020 2020  bel_iface".     
+00000240: 203e 6279 2049 6e74 6572 6661 6365 3c2f   >by Interface</
+00000250: 6833 3e0a 2020 2020 2020 3c75 6c20 636c  h3>.      <ul cl
+00000260: 6173 733d 2263 6f6c 6c61 7073 655f 696e  ass="collapse_in
+00000270: 7465 7266 6163 6573 223e 0a20 2020 2020  terfaces">.     
+00000280: 2020 203c 6c69 2074 616c 3a72 6570 6561     <li tal:repea
+00000290: 743d 2270 7265 6669 7820 7079 7468 6f6e  t="prefix python
+000002a0: 3a76 6965 772e 696e 7465 7266 6163 6573  :view.interfaces
+000002b0: 2829 223e 3c61 2068 7265 663d 2224 7b70  ()"><a href="${p
+000002c0: 7974 686f 6e3a 7072 6566 6978 5b31 5d7d  ython:prefix[1]}
+000002d0: 220a 2020 2020 2020 2020 2020 2020 2074  ".             t
+000002e0: 6172 6765 743d 225f 626c 616e 6b22 0a20  arget="_blank". 
+000002f0: 2020 2020 2020 2020 203e 247b 7079 7468           >${pyth
+00000300: 6f6e 3a70 7265 6669 785b 305d 7d3c 2f61  on:prefix[0]}</a
+00000310: 3e3c 2f6c 693e 0a20 2020 2020 203c 2f75  ></li>.      </u
+00000320: 6c3e 0a20 2020 203c 2f64 6976 3e0a 2020  l>.    </div>.  
+00000330: 2020 3c64 6976 2063 6c61 7373 3d22 6578    <div class="ex
+00000340: 706f 7274 7461 6222 0a20 2020 2020 2020  porttab".       
+00000350: 2020 6964 3d22 6578 706f 7274 2d73 6563    id="export-sec
+00000360: 7469 6f6e 2d70 7265 6669 7865 7322 0a20  tion-prefixes". 
+00000370: 2020 203e 0a20 2020 2020 203c 6833 2069     >.      <h3 i
+00000380: 643d 2268 332d 7072 6566 6978 6573 220a  d="h3-prefixes".
+00000390: 2020 2020 2020 2020 2020 6931 386e 3a74            i18n:t
+000003a0: 7261 6e73 6c61 7465 3d22 7265 6769 7374  ranslate="regist
+000003b0: 7279 5f65 7870 6f72 745f 7061 7274 735f  ry_export_parts_
+000003c0: 6c61 6265 6c5f 7072 6566 6978 220a 2020  label_prefix".  
+000003d0: 2020 2020 3e62 7920 5072 6566 6978 3c2f      >by Prefix</
+000003e0: 6833 3e0a 2020 2020 2020 3c75 6c3e 0a20  h3>.      <ul>. 
+000003f0: 2020 2020 2020 203c 6c69 2074 616c 3a72         <li tal:r
+00000400: 6570 6561 743d 2270 7265 6669 7820 7079  epeat="prefix py
+00000410: 7468 6f6e 3a76 6965 772e 7072 6566 6978  thon:view.prefix
+00000420: 6573 2829 223e 3c61 2068 7265 663d 2224  es()"><a href="$
+00000430: 7b70 7974 686f 6e3a 7072 6566 6978 5b31  {python:prefix[1
+00000440: 5d7d 220a 2020 2020 2020 2020 2020 2020  ]}".            
+00000450: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000460: 0a20 2020 2020 2020 2020 203e 247b 7079  .          >${py
+00000470: 7468 6f6e 3a70 7265 6669 785b 305d 7d3c  thon:prefix[0]}<
+00000480: 2f61 3e3c 2f6c 693e 0a20 2020 2020 203c  /a></li>.      <
+00000490: 2f75 6c3e 0a20 2020 203c 2f64 6976 3e0a  /ul>.    </div>.
+000004a0: 2020 3c2f 6469 763e 0a3c 2f74 616c 3e0a    </div>.</tal>.
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/browser/templates/records.pt` & `plone.app.registry-2.0.2/plone/app/registry/browser/templates/records.pt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/configure.zcml` & `plone.app.registry-2.0.2/plone/app/registry/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:gs="http://namespaces.zope.org/genericsetup"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <include package="Products.CMFCore" file="permissions.zcml" />
+  <include
+      package="Products.CMFCore"
+      file="permissions.zcml"
+      />
+
+  <include package="plone.registry" />
+
+  <include package=".exportimport" />
+  <include package=".browser" />
+
+  <five:registerClass
+      class=".registry.Registry"
+      permission="cmf.ManagePortal"
+      meta_type="Plone Configuration Registry"
+      />
 
-    <include package="plone.registry" />
-
-    <include package=".exportimport" />
-    <include package=".browser" />
-
-    <five:registerClass
-        class=".registry.Registry"
-        meta_type="Plone Configuration Registry"
+  <class class=".registry.Registry">
+    <require
         permission="cmf.ManagePortal"
+        interface="plone.registry.interfaces.IRegistry"
         />
+  </class>
 
-    <class class=".registry.Registry">
-        <require
-            permission="cmf.ManagePortal"
-            interface="plone.registry.interfaces.IRegistry"
-            />
-    </class>
-
-    <gs:registerProfile
-        name="default"
-        directory="profiles/default"
-        title="Configuration registry"
-        description="A 'Mozilla about:config' style configuration registry"
-        for="Products.CMFPlone.interfaces.IPloneSiteRoot"
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        />
+  <gs:registerProfile
+      name="default"
+      title="Configuration registry"
+      description="A 'Mozilla about:config' style configuration registry"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="Products.CMFPlone.interfaces.IPloneSiteRoot"
+      directory="profiles/default"
+      />
 
 </configure>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/exportimport/configure.zcml` & `plone.app.registry-2.0.2/plone/app/registry/exportimport/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 <configure
-    i18n_domain="plone"
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:gs="http://namespaces.zope.org/genericsetup">
+    xmlns:gs="http://namespaces.zope.org/genericsetup"
+    i18n_domain="plone"
+    >
 
   <include package="plone.supermodel" />
   <include file="handlers.zcml" />
 
   <!-- export/import steps -->
   <gs:importStep
+      name="plone.app.registry"
+      title="Configuration Registry (Plone)"
       description="Import into plone.app.registry records/settings, the central configuration key-value store, from registry.xml or a registry folder."
       handler=".handler.importRegistry"
-      name="plone.app.registry"
-      title="Configuration Registry (Plone)">
+      >
     <depends name="componentregistry" />
     <depends name="toolset" />
-    <depends name="typeinfo"/>
+    <depends name="typeinfo" />
   </gs:importStep>
 
   <gs:exportStep
-      description="Export plone.app.registry, the central configuration key-value store, into a XML file."
-      handler=".handler.exportRegistry"
       name="plone.app.registry"
       title="Configuration Registry (Plone)"
-  />
+      description="Export plone.app.registry, the central configuration key-value store, into a XML file."
+      handler=".handler.exportRegistry"
+      />
 
 </configure>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/exportimport/fields.py` & `plone.app.registry-2.0.2/plone/app/registry/exportimport/fields.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/plone/app/registry/exportimport/handler.py` & `plone.app.registry-2.0.2/plone/app/registry/exportimport/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
                 return False
             else:
                 return True
     return True
 
 
 def importRegistry(context):
-
     logger = context.getLogger("plone.app.registry")
     registry = queryUtility(IRegistry)
 
     if registry is None:
         logger.info("Cannot find registry")
         return
 
@@ -77,15 +76,14 @@
         __traceback_info__ = filepath
         body = context.readDataFile(filepath)
         if body is not None:
             importer.importDocument(body)
 
 
 def exportRegistry(context):
-
     logger = context.getLogger("plone.app.registry")
     registry = queryUtility(IRegistry)
 
     if registry is None:
         logger.info("Cannot find registry")
         return
 
@@ -183,15 +181,15 @@
                     "Failed to import interface {} for "
                     "record {}".format(interfaceName, name)
                 )
                 interface = None
                 field = None
             except KeyError:
                 self.logger.warning(
-                    "Interface {} specified for record %s has "
+                    "Interface {} specified for record {} has "
                     "no field {}.".format(interfaceName, name, fieldName)
                 )
                 interface = None
                 field = None
             except TypeError:
                 self.logger.warning(
                     "Field {} in interface {} specified for record {} "
@@ -279,15 +277,14 @@
             value_purge = True
 
         if existing_record is not None:
             if change_field:
                 existing_record.field = field
             existing_value = existing_record.value
             if change_field or value != existing_value:
-
                 if not value_purge and type(value) == type(existing_value):
                     if isinstance(value, list):
                         value = existing_value + [
                             v for v in value if v not in existing_value
                         ]
                     elif isinstance(value, tuple):
                         value = existing_value + tuple(
@@ -300,15 +297,15 @@
                             frozenset,
                         ),
                     ):
                         value = existing_value.union(value)
                     elif isinstance(value, dict):
                         for key, value in value.items():
                             # check if value is list, if so, let's add
-                            # instead of overridding
+                            # instead of overriding
                             if (
                                 type(value) == list
                                 and key in existing_value
                                 and not shouldPurgeList(value_node, key)
                             ):
                                 existing = existing_value[key]
                                 for item in existing:
@@ -323,15 +320,14 @@
                         value = existing_value
 
                 existing_record.value = value
         else:
             self.context.records[name] = Record(field, value)
 
     def importRecords(self, node):
-
         # May raise ImportError if interface can't be found or KeyError if
         # attribute is missing.
 
         interfaceName = node.attrib.get("interface", None)
         if interfaceName is None:
             raise KeyError("A <records /> node must have an 'interface' attribute.")
 
@@ -398,15 +394,14 @@
                 remove=repr(remove).lower(),
             )
             field.append(value)
             self.importRecord(field)
 
 
 class RegistryExporter:
-
     LOGGER_ID = "plone.app.registry"
 
     def __init__(self, context, environ):
         self.context = context
         self.environ = environ
         self.logger = environ.getLogger(self.LOGGER_ID)
 
@@ -416,15 +411,14 @@
         for record in self.context.records.values():
             node = self.exportRecord(record)
             root.append(node)
 
         return prettyXML(root)
 
     def exportRecord(self, record):
-
         node = etree.Element("record")
         node.attrib["name"] = record.__name__
 
         if IInterfaceAwareRecord.providedBy(record):
             node.attrib["interface"] = record.interfaceName
             node.attrib["field"] = record.fieldName
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/exportimport/handlers.zcml` & `plone.app.registry-2.0.2/plone/app/registry/exportimport/handlers.zcml`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,99 @@
 <configure
+    xmlns="http://namespaces.zope.org/zope"
     i18n_domain="plone"
-    xmlns="http://namespaces.zope.org/zope">
+    >
   <include package="plone.supermodel" />
   <!-- plone.supermodel field handlers -->
   <utility
+      name="plone.registry.field.Bytes"
       component=".fields.BytesHandler"
-      name="plone.registry.field.Bytes" />
+      />
   <utility
+      name="plone.registry.field.BytesLine"
       component=".fields.BytesLineHandler"
-      name="plone.registry.field.BytesLine" />
+      />
   <utility
+      name="plone.registry.field.ASCII"
       component=".fields.ASCIIHandler"
-      name="plone.registry.field.ASCII" />
+      />
   <utility
+      name="plone.registry.field.ASCIILine"
       component=".fields.ASCIILineHandler"
-      name="plone.registry.field.ASCIILine" />
+      />
   <utility
+      name="plone.registry.field.Text"
       component=".fields.TextHandler"
-      name="plone.registry.field.Text" />
+      />
   <utility
+      name="plone.registry.field.TextLine"
       component=".fields.TextLineHandler"
-      name="plone.registry.field.TextLine" />
+      />
   <utility
+      name="plone.registry.field.Bool"
       component=".fields.BoolHandler"
-      name="plone.registry.field.Bool" />
+      />
   <utility
+      name="plone.registry.field.Int"
       component=".fields.IntHandler"
-      name="plone.registry.field.Int" />
+      />
   <utility
+      name="plone.registry.field.Float"
       component=".fields.FloatHandler"
-      name="plone.registry.field.Float" />
+      />
   <utility
+      name="plone.registry.field.Tuple"
       component=".fields.TupleHandler"
-      name="plone.registry.field.Tuple" />
+      />
   <utility
+      name="plone.registry.field.List"
       component=".fields.ListHandler"
-      name="plone.registry.field.List" />
+      />
   <utility
+      name="plone.registry.field.Set"
       component=".fields.SetHandler"
-      name="plone.registry.field.Set" />
+      />
   <utility
+      name="plone.registry.field.FrozenSet"
       component=".fields.FrozenSetHandler"
-      name="plone.registry.field.FrozenSet" />
+      />
   <utility
+      name="plone.registry.field.Password"
       component=".fields.PasswordHandler"
-      name="plone.registry.field.Password" />
+      />
   <utility
+      name="plone.registry.field.Dict"
       component=".fields.DictHandler"
-      name="plone.registry.field.Dict" />
+      />
   <utility
+      name="plone.registry.field.Datetime"
       component=".fields.DatetimeHandler"
-      name="plone.registry.field.Datetime" />
+      />
   <utility
+      name="plone.registry.field.Date"
       component=".fields.DateHandler"
-      name="plone.registry.field.Date" />
+      />
   <utility
+      name="plone.registry.field.SourceText"
       component=".fields.SourceTextHandler"
-      name="plone.registry.field.SourceText" />
+      />
   <utility
+      name="plone.registry.field.URI"
       component=".fields.URIHandler"
-      name="plone.registry.field.URI" />
+      />
   <utility
+      name="plone.registry.field.Id"
       component=".fields.IdHandler"
-      name="plone.registry.field.Id" />
+      />
   <utility
+      name="plone.registry.field.DottedName"
       component=".fields.DottedNameHandler"
-      name="plone.registry.field.DottedName" />
+      />
   <utility
+      name="plone.registry.field.Choice"
       component=".fields.ChoiceHandler"
-      name="plone.registry.field.Choice" />
+      />
   <utility
+      name="plone.registry.field.JSONField"
       component=".fields.JSONFieldHandler"
-      name="plone.registry.field.JSONField" />
+      />
 </configure>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/testing.py` & `plone.app.registry-2.0.2/plone/app/registry/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from zope.configuration import xmlconfig
 
 
 class PloneAppRegistry(PloneSandboxLayer):
-
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load ZCML
         import plone.app.registry
 
         xmlconfig.file(
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/tests/test_controlpanel.py` & `plone.app.registry-2.0.2/plone/app/registry/tests/test_controlpanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 from plone.registry.field import TextLine
 from zope.component import getMultiAdapter
 
 import unittest
 
 
 class TestRegistryBaseControlpanel(unittest.TestCase):
-
     layer = PLONE_APP_REGISTRY_INTEGRATION_TESTING
 
     def test_registry_base_controlpanel__control_panel_url(self):
         """Test, if control_panel_url property of the base controlpanel returns
         the correct url.
         """
         view = ControlPanelFormWrapper(None, None)
         self.assertEqual(
             view.control_panel_url, "http://nohost/plone/@@overview-controlpanel"
         )
 
 
 class TestRecordsControlPanel(unittest.TestCase):
-
     layer = PLONE_APP_REGISTRY_INTEGRATION_TESTING
 
     def setUp(self):
         self.request = self.layer["request"]
         self.portal = self.layer["portal"]
 
     def test_records_control_panel__control_panel_url(self):
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/tests/test_exportimport.py` & `plone.app.registry-2.0.2/plone/app/registry/tests/test_exportimport.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,26 +31,24 @@
     <include package="plone.registry" />
     <include package="plone.app.registry.exportimport" file="handlers.zcml" />
 </configure>
 """
 
 
 class DummyImportContext(BaseDummyImportContext):
-
     _directories = {}
 
     def listDirectory(self, path):
         return self._directories.get(path, [])
 
     def isDirectory(self, path):
         return path in self._directories
 
 
 class ExportImportTest(unittest.TestCase):
-
     layer = zca.UNIT_TESTING
 
     def setUp(self):
         self.site = ObjectManager("plone")
         self.registry = Registry("portal_registry")
         provideUtility(provides=IRegistry, component=self.registry)
         context = xmlconfig.string(configuration, execute=True)
@@ -67,49 +65,46 @@
             import Zope2.App.zcml
 
             Zope2.App.zcml._context = self._context
         except ImportError:
             pass
 
     def assertXmlEquals(self, expected, actual):
-
         expected_tree = etree.XML(expected)
         actual_tree = etree.XML(actual)
 
         if etree.tostring(expected_tree) != etree.tostring(actual_tree):
             print()
             print("Expected:")
             print(prettyXML(expected_tree))
             print()
 
             print()
             print("Actual:")
             print(prettyXML(actual_tree))
             print()
 
-            raise AssertionError("XML mis-match")
+            raise AssertionError("XML mismatch")
 
 
 class TestImport(ExportImportTest):
     def test_empty_import_no_purge(self):
-
         xml = "<registry/>"
         context = DummyImportContext(self.site, purge=False)
         context._files = {"registry.xml": xml}
 
         self.registry.records["test.export.simple"] = Record(
             field.TextLine(title="Simple record", default="N/A"),
             value="Sample value",
         )
         importRegistry(context)
 
         self.assertEqual(1, len(self.registry.records))
 
     def test_import_purge(self):
-
         xml = "<registry/>"
         context = DummyImportContext(self.site, purge=True)
         context._files = {"registry.xml": xml}
 
         self.registry.records["test.export.simple"] = Record(
             field.TextLine(title="Simple record", default="N/A"),
             value="Sample value",
@@ -331,26 +326,26 @@
         self.assertEqual(
             self.registry["plone.app.registry.tests.data.SomethingElse.age"], 42
         )
 
     def test_import_records_nonexistant_interface(self):
         xml = """\
 <registry>
-    <records interface="non.existant.ISchema" />
+    <records interface="non.existent.ISchema" />
 </registry>
 """
         context = DummyImportContext(self.site, purge=False)
         context._files = {"registry.xml": xml}
 
         self.assertRaises(ImportError, importRegistry, context)
 
-    def test_import_records_nonexistant_interface_condition_not_installed(self):  # noqa
+    def test_import_records_nonexistant_interface_condition_not_installed(self):
         xml = """\
 <registry>
-    <records interface="non.existant.ISchema"
+    <records interface="non.existent.ISchema"
              condition="not-installed non" />
 </registry>
 """
         context = DummyImportContext(self.site, purge=False)
         context._files = {"registry.xml": xml}
 
         self.assertRaises(ImportError, importRegistry, context)
@@ -464,21 +459,19 @@
         importRegistry(context)
 
         self.assertEqual(1, len(self.registry.records))
         self.assertEqual(
             "Age",
             self.registry.records[
                 "plone.app.registry.tests.data.ITestSettingsDisallowed.age"
-            ].field.title,  # noqa
+            ].field.title,
         )
         self.assertEqual(
             2,
-            self.registry[
-                "plone.app.registry.tests.data.ITestSettingsDisallowed.age"
-            ],  # noqa
+            self.registry["plone.app.registry.tests.data.ITestSettingsDisallowed.age"],
         )
 
     def test_import_interface_with_differnet_name(self):
         xml = """\
 <registry>
     <record name="plone.registry.oops" interface="plone.app.registry.tests.data.ITestSettingsDisallowed" field="age">
         <value>2</value>
@@ -508,21 +501,19 @@
         importRegistry(context)
 
         self.assertEqual(1, len(self.registry.records))
         self.assertEqual(
             "Name",
             self.registry.records[
                 "plone.app.registry.tests.data.ITestSettingsDisallowed.name"
-            ].field.title,  # noqa
+            ].field.title,
         )
         self.assertEqual(
             "Mr. Registry",
-            self.registry[
-                "plone.app.registry.tests.data.ITestSettingsDisallowed.name"
-            ],  # noqa
+            self.registry["plone.app.registry.tests.data.ITestSettingsDisallowed.name"],
         )
 
     def test_import_field_only(self):
         xml = """\
 <registry>
     <record name="test.registry.field">
         <field type="plone.registry.field.TextLine">
@@ -578,17 +569,15 @@
         )
         self.assertEqual(
             "Simple record",
             self.registry.records["test.registry.field.override"].field.title,
         )
         self.assertEqual(
             "value",
-            self.registry.records[
-                "test.registry.field.override"
-            ].field.__name__,  # noqa
+            self.registry.records["test.registry.field.override"].field.__name__,
         )
         self.assertEqual("Another value", self.registry["test.registry.field.override"])
 
     def test_import_field_and_interface(self):
         xml = """\
 <registry>
     <record name="test.registry.field" interface="plone.app.registry.tests.data.ITestSettingsDisallowed" field="age">
@@ -1023,15 +1012,15 @@
             "Simple record", self.registry.records["test.registry.field"].field.title
         )
         self.assertEqual(
             ["One", "Two"],
             [
                 t.value
                 for t in self.registry.records["test.registry.field"].field.vocabulary
-            ],  # noqa
+            ],
         )
         self.assertEqual(None, self.registry["test.registry.field"])
 
     def test_import_with_comments(self):
         xml = """\
 <registry>
     <records interface="plone.app.registry.tests.data.ITestSettings" prefix="plone.app.registry.tests.data.SomethingElse">
@@ -1255,24 +1244,22 @@
             },
             self.registry["test.registry.field"],
         )
 
 
 class TestExport(ExportImportTest):
     def test_export_empty(self):
-
         xml = """<registry />"""
         context = DummyExportContext(self.site)
         exportRegistry(context)
 
         self.assertEqual("registry.xml", context._wrote[0][0])
         self.assertXmlEquals(xml, context._wrote[0][1])
 
     def test_export_simple(self):
-
         xml = """\
 <registry>
   <record name="test.export.simple">
     <field type="plone.registry.field.TextLine">
       <default>N/A</default>
       <title>Simple record</title>
     </field>
@@ -1327,15 +1314,14 @@
         context = DummyExportContext(self.site)
         exportRegistry(context)
 
         self.assertEqual("registry.xml", context._wrote[0][0])
         self.assertXmlEquals(xml, context._wrote[0][1])
 
     def test_export_field_ref(self):
-
         xml = """\
 <registry>
   <record name="test.export.simple">
     <field type="plone.registry.field.TextLine">
       <default>N/A</default>
       <title>Simple record</title>
     </field>
@@ -1359,15 +1345,14 @@
         context = DummyExportContext(self.site)
         exportRegistry(context)
 
         self.assertEqual("registry.xml", context._wrote[0][0])
         self.assertXmlEquals(xml, context._wrote[0][1])
 
     def test_export_with_collection(self):
-
         xml = """\
 <registry>
   <record name="test.export.simple">
     <field type="plone.registry.field.List">
       <title>Simple record</title>
       <value_type type="plone.registry.field.Int">
         <title>Val</title>
@@ -1386,15 +1371,14 @@
         context = DummyExportContext(self.site)
         exportRegistry(context)
 
         self.assertEqual("registry.xml", context._wrote[0][0])
         self.assertXmlEquals(xml, context._wrote[0][1])
 
     def test_export_with_dict(self):
-
         xml = """\
 <registry>
   <record name="test.export.dict">
     <field type="plone.registry.field.Dict">
       <default />
       <key_type type="plone.registry.field.ASCIILine">
         <title>Key</title>
@@ -1423,15 +1407,14 @@
         context = DummyExportContext(self.site)
         exportRegistry(context)
 
         self.assertEqual("registry.xml", context._wrote[0][0])
         self.assertXmlEquals(xml, context._wrote[0][1])
 
     def test_export_with_choice(self):
-
         xml = """\
 <registry>
   <record name="test.export.choice">
     <field type="plone.registry.field.Choice">
       <title>Simple record</title>
       <vocabulary>dummy.vocab</vocabulary>
     </field>
@@ -1446,18 +1429,17 @@
         context = DummyExportContext(self.site)
         exportRegistry(context)
 
         self.assertEqual("registry.xml", context._wrote[0][0])
         self.assertXmlEquals(xml, context._wrote[0][1])
 
     def test_export_with_missing_schema_does_not_error(self):
-
         xml = """\
 <registry>
-  <record name="test.export.simple" interface="non.existant.ISchema" field="blah">
+  <record name="test.export.simple" interface="non.existent.ISchema" field="blah">
     <field type="plone.registry.field.TextLine">
       <default>N/A</default>
       <title>Simple record</title>
     </field>
     <value>Sample value</value>
   </record>
 </registry>"""
@@ -1466,27 +1448,26 @@
             field.TextLine(title="Simple record", default="N/A"),
             value="Sample value",
         )
 
         # Note: These are nominally read-only!
         self.registry.records[
             "test.export.simple"
-        ].field.interfaceName = "non.existant.ISchema"  # noqa
+        ].field.interfaceName = "non.existent.ISchema"
         self.registry.records["test.export.simple"].field.fieldName = "blah"
 
         alsoProvides(self.registry.records["test.export.simple"], IInterfaceAwareRecord)
 
         context = DummyExportContext(self.site)
         exportRegistry(context)
 
         self.assertEqual("registry.xml", context._wrote[0][0])
         self.assertXmlEquals(xml, context._wrote[0][1])
 
     def test_export_with_jsonfield(self):
-
         xml = """\
 <registry>
   <record name="test.export.field">
     <field type="plone.registry.field.JSONField">
       <default>{}</default>
       <title>Dict</title>
     </field>
```

### Comparing `plone.app.registry-2.0.1/plone/app/registry/tests/test_setup.py` & `plone.app.registry-2.0.2/plone/app/registry/tests/test_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from plone.registry.interfaces import IRegistry
 from zope.component import getUtility
 
 import unittest
 
 
 class TestSetup(unittest.TestCase):
-
     layer = PLONE_APP_REGISTRY_INTEGRATION_TESTING
 
     def test_tool_installed(self):
-
         portal = self.layer["portal"]
 
         self.assertIn("portal_registry", portal.objectIds())
         self.assertTrue(IRegistry.providedBy(portal.portal_registry))
 
     def test_local_utility_installed(self):
         portal = self.layer["portal"]
```

### Comparing `plone.app.registry-2.0.1/plone.app.registry.egg-info/PKG-INFO` & `plone.app.registry-2.0.2/plone.app.registry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.registry
-Version: 2.0.1
+Version: 2.0.2
 Summary: Zope 2 and Plone  integration for plone.registry
 Home-page: https://pypi.org/project/plone.app.registry
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
 License: GPL
 Keywords: plone registry settings configuration
 Classifier: Development Status :: 5 - Production/Stable
@@ -753,14 +753,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 2.0.1 (2022-12-10)
 ------------------
 
 Bug fixes:
 
 
 - Fix responsive table.
```

### Comparing `plone.app.registry-2.0.1/plone.app.registry.egg-info/SOURCES.txt` & `plone.app.registry-2.0.2/plone.app.registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.1/setup.py` & `plone.app.registry-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.1"
+version = "2.0.2"
 
 setup(
     name="plone.app.registry",
     version=version,
     description="Zope 2 and Plone  integration for plone.registry",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     # Get more strings from
@@ -41,17 +41,22 @@
         "plone.app.z3cform",
         "plone.autoform>=1.0",
         "plone.base",
         "plone.registry>=1.0",
         "plone.supermodel>=1.1",
         "Products.statusmessages",
         "setuptools",
+        "Products.GenericSetup",
+        "plone.z3cform",
+        "z3c.form",
+        "zope.dottedname",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
+            "plone.testing",
         ]
     },
     entry_points="""
     # -*- Entry points: -*-
     """,
 )
```

