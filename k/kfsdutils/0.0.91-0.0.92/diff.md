# Comparing `tmp/kfsdutils-0.0.91.tar.gz` & `tmp/kfsdutils-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsdutils-0.0.91.tar", last modified: Thu Apr 13 14:52:07 2023, max compression
+gzip compressed data, was "kfsdutils-0.0.92.tar", last modified: Sat Apr 15 04:22:44 2023, max compression
```

## Comparing `kfsdutils-0.0.91.tar` & `kfsdutils-0.0.92.tar`

### file list

```diff
@@ -1,93 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.313054 kfsdutils-0.0.91/kfsdutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/browser.html
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/tests/test_apibrowserview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/views/apibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/basehandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetstext.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/basemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/baseview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/tokenuser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseformview.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/basetemplateview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.313054 kfsdutils-0.0.91/kfsdutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.956761 kfsdutils-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-15 04:22:44.952761 kfsdutils-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.932761 kfsdutils-0.0.92/kfsdutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.936761 kfsdutils-0.0.92/kfsdutils/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.936761 kfsdutils-0.0.92/kfsdutils/apps/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/core/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.936761 kfsdutils-0.0.92/kfsdutils/apps/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.940761 kfsdutils-0.0.92/kfsdutils/apps/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/templates/browser.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/templates/skeleton.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.940761 kfsdutils-0.0.92/kfsdutils/apps/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/tests/test_apibrowserview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.940761 kfsdutils-0.0.92/kfsdutils/apps/docs/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/docs/views/apibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.940761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.940761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.944761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/handlers/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/handlers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/handlers/core/apikeyuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/handlers/core/basehandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.944761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/middleware/be_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.944761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/renderers/kubefacetstext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.944761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/serializers/basemodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.944761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.948761 kfsdutils-0.0.92/kfsdutils/apps/endpoints/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/endpoints/views/baseview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.948761 kfsdutils-0.0.92/kfsdutils/apps/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.948761 kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/tokenuser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.948761 kfsdutils-0.0.92/kfsdutils/apps/frontend/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/permissions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/permissions/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.952761 kfsdutils-0.0.92/kfsdutils/apps/frontend/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/views/baseformview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/views/basetemplateview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/frontend/views/baseview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.952761 kfsdutils-0.0.92/kfsdutils/apps/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/middleware/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/middleware/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/middleware/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.952761 kfsdutils-0.0.92/kfsdutils/apps/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/apps/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/kfsdutils/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:22:44.932761 kfsdutils-0.0.92/kfsdutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-15 04:22:44.000000 kfsdutils-0.0.92/kfsdutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-15 04:22:44.000000 kfsdutils-0.0.92/kfsdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:22:44.000000 kfsdutils-0.0.92/kfsdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:22:44.000000 kfsdutils-0.0.92/kfsdutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 04:22:44.000000 kfsdutils-0.0.92/kfsdutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 04:22:44.000000 kfsdutils-0.0.92/kfsdutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:22:44.956761 kfsdutils-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-15 04:22:31.000000 kfsdutils-0.0.92/setup.py
```

### Comparing `kfsdutils-0.0.91/LICENSE` & `kfsdutils-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/core/configuration.py` & `kfsdutils-0.0.92/kfsdutils/apps/core/configuration.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/core/logger.py` & `kfsdutils-0.0.92/kfsdutils/apps/core/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 from enum import Enum
 from functools import wraps
 from kfsdutils.apps.core.singleton import Singleton
 
 import logging
 
+
 class Logger:
-	__defaultFormat = '[%(asctime)s][%(name)s][%(levelname)s] %(message)s'
-	
-	def __init__(self, fileName, logLevel):
-		self.__logger = logging.getLogger(fileName)
-		self.__loglevel = self.__getLoggerLevel(logLevel)
-		self.setFormat(self.__defaultFormat)
-
-	@classmethod
-	@Singleton
-	def getSingleton(cls, fileName, logLevel):
-		return cls(fileName, logLevel)
-
-	def setFormat(self, format):
-		formatter = logging.Formatter(format)
-		stream_handler = logging.StreamHandler()
-		stream_handler.setFormatter(formatter)
-		self.__logger.addHandler(stream_handler)
-
-	def __getLogger(self):
-		return self.__logger
-
-	def debug(self, msg, *args, **kwargs):
-		self.__getLogger().debug(msg, *args, **kwargs)
-
-	def info(self, msg, *args, **kwargs):
-		self.__getLogger().info(msg, *args, **kwargs)
-
-	def error(self, msg, *args, **kwargs):
-		self.__getLogger().error(msg, *args, **kwargs)
-
-	def warn(self, msg, *args, **kwargs):
-		self.__getLogger().warn(msg, *args, **kwargs)
-
-	def exception(self, msg, *args, **kwargs):
-		self.__getLogger().exception(msg, *args, **kwargs)
-
-	def critical(self, msg, *args, **kwargs):
-		self.__getLogger().critical(msg, *args, **kwargs)
-
-	def __getLoggerLevel(self, logLevel):
-		if logLevel is not None:
-			loggerLevelDict = {}
-			loggerLevelDict[str(LogLevel.CRITICAL)] = logging.CRITICAL
-			loggerLevelDict[str(LogLevel.ERROR)] = logging.ERROR
-			loggerLevelDict[str(LogLevel.WARNING)] = logging.WARNING
-			loggerLevelDict[str(LogLevel.INFO)] = logging.INFO
-			loggerLevelDict[str(LogLevel.DEBUG)] = logging.DEBUG
-			loggerLevelDict[str(LogLevel.NOTSET)] = logging.NOTSET
-			loggingLevel = loggerLevelDict[str(logLevel)] if str(logLevel) in loggerLevelDict else logging.NOTSET
-			return self.__logger.setLevel(loggingLevel)
+    __defaultFormat = '[%(asctime)s][%(name)s][%(levelname)s] %(message)s'
+
+    def __init__(self, fileName, logLevel):
+        self.__logger = logging.getLogger(fileName)
+        self.__loglevel = self.__getLoggerLevel(logLevel)
+        self.setFormat(self.__defaultFormat)
+
+    @classmethod
+    @Singleton
+    def getSingleton(cls, fileName, logLevel):
+        return cls(fileName, logLevel)
+
+    def setFormat(self, format):
+        formatter = logging.Formatter(format)
+        stream_handler = logging.StreamHandler()
+        stream_handler.setFormatter(formatter)
+        self.__logger.addHandler(stream_handler)
+
+    def __getLogger(self):
+        return self.__logger
+
+    def debug(self, msg, *args, **kwargs):
+        self.__getLogger().debug(msg, *args, **kwargs)
+
+    def info(self, msg, *args, **kwargs):
+        self.__getLogger().info(msg, *args, **kwargs)
+
+    def error(self, msg, *args, **kwargs):
+        self.__getLogger().error(msg, *args, **kwargs)
+
+    def warn(self, msg, *args, **kwargs):
+        self.__getLogger().warn(msg, *args, **kwargs)
+
+    def exception(self, msg, *args, **kwargs):
+        self.__getLogger().exception(msg, *args, **kwargs)
+
+    def critical(self, msg, *args, **kwargs):
+        self.__getLogger().critical(msg, *args, **kwargs)
+
+    def __getLoggerLevel(self, logLevel):
+        if logLevel is not None:
+            loggerLevelDict = {}
+            loggerLevelDict[str(LogLevel.CRITICAL)] = logging.CRITICAL
+            loggerLevelDict[str(LogLevel.ERROR)] = logging.ERROR
+            loggerLevelDict[str(LogLevel.WARNING)] = logging.WARNING
+            loggerLevelDict[str(LogLevel.INFO)] = logging.INFO
+            loggerLevelDict[str(LogLevel.DEBUG)] = logging.DEBUG
+            loggerLevelDict[str(LogLevel.NOTSET)] = logging.NOTSET
+            loggingLevel = loggerLevelDict[str(logLevel)] if str(logLevel) in loggerLevelDict else logging.NOTSET
+            return self.__logger.setLevel(loggingLevel)
 
-		return self.__logger.setLevel(logging.NOTSET)
+        return self.__logger.setLevel(logging.NOTSET)
 
 
 class LogLevel(Enum):
-	CRITICAL = 0
-	ERROR = 1
-	WARNING = 2
-	INFO = 3
-	DEBUG = 4
-	NOTSET = 5
+    CRITICAL = 0
+    ERROR = 1
+    WARNING = 2
+    INFO = 3
+    DEBUG = 4
+    NOTSET = 5
+
 
 def InstanceDebug(func):
-	@wraps(func)
-	def wrapper(*args, **kwargs):
-		selfObj = args[0]
-		result = func(*args, **kwargs)
-		selfObj.getLogObj().debug("Input:{}, Output: {}".format(args, result))
-		return result
-	return wrapper
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        selfObj = args[0]
+        result = func(*args, **kwargs)
+        selfObj.getLogObj().debug("Input:{}, Output: {}".format(args, result))
+        return result
+    return wrapper
+
 
 def Debug(logger):
-	def debugWrapper(func):
-		@wraps(func)
-		def wrapper(*args, **kwargs):
-			result = func(*args, **kwargs)
-			logger.debug("Input:{}, Output: {}".format(args, result))
-			return result
-		return wrapper
-	return debugWrapper
+    def debugWrapper(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            result = func(*args, **kwargs)
+            logger.debug("Input:{}, Output: {}".format(args, result))
+            return result
+        return wrapper
+    return debugWrapper
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/core/utils.py` & `kfsdutils-0.0.92/kfsdutils/apps/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,23 @@
-import functools, os, shutil, json, zlib, secrets, urllib.parse, requests, binascii
+import functools
+import os
+import shutil
+import json
+import zlib
+import secrets
+import urllib.parse
+import requests
+import binascii
 from collections.abc import Mapping
 from kfsdutils.apps.core.logger import Logger, LogLevel
 from kfsdutils.apps.endpoints.exceptions import KubefacetsAPIException
 from rest_framework import status
 import http.cookies
 
+
 class HTTPUtils:
     @staticmethod
     def cookieToHeaderStr(request, cookieFilterKeys):
         cookie_string = ''
         if request.COOKIES:
             cookie = http.cookies.SimpleCookie()
             filteredCookies = DictUtils.filterDictByKeysList(request.COOKIES, cookieFilterKeys)
@@ -21,32 +30,32 @@
 
     @staticmethod
     def isValidResponse(expStatus, obsStatus, resp):
         if isinstance(expStatus, int) and not expStatus == obsStatus:
             raise KubefacetsAPIException(
                 resp.json()["detail"], resp.json()["code"], obsStatus
             )
-        
-        if isinstance(expStatus, list) and not obsStatus in expStatus:
+
+        if isinstance(expStatus, list) and obsStatus not in expStatus:
             raise KubefacetsAPIException(
                 resp.json()["detail"], resp.json()["code"], obsStatus
             )
-        
+
         return True
 
     @staticmethod
     def request(method, url, expStatus, **kwargs):
         try:
             resp = method(url, **kwargs)
             if HTTPUtils.isValidResponse(expStatus, resp.status_code, resp):
                 return resp
         except requests.exceptions.Timeout:
             raise KubefacetsAPIException(
                 "The server took too long to respond to your request. Please try again later.",
-                "server_timed_out", 
+                "server_timed_out",
                 status.HTTP_408_REQUEST_TIMEOUT
             )
         except requests.exceptions.ConnectionError:
             raise KubefacetsAPIException(
                 "Service temporarily unavailable. Please try again later.",
                 "service_unavailable",
                 status.HTTP_503_SERVICE_UNAVAILABLE
@@ -60,14 +69,15 @@
     def get(url, expStatus, **kwargs):
         return HTTPUtils.request(requests.get, url, expStatus, **kwargs)
 
     @staticmethod
     def delete(url, expStatus, **kwargs):
         return HTTPUtils.request(requests.delete, url, expStatus, **kwargs)
 
+
 class GeneralUtils:
     def __init__(self):
         self.__logger = Logger.getSingleton(__name__, LogLevel.DEBUG)
 
     @staticmethod
     def genChecksum(data):
         return zlib.adler32(data.encode("utf-8")) & 0xffffffff
@@ -84,34 +94,35 @@
     def genKey(len):
         api_key_bytes = secrets.token_bytes(len)
         return binascii.hexlify(api_key_bytes).decode('utf-8')
 
     @staticmethod
     def getEnv(key):
         return os.getenv(key)
-    
+
     @staticmethod
     def genUrlEncode(urlstr):
         return urllib.parse.quote(urlstr)
 
+
 class ArrUtils:
     def __init__(self):
         self.__logger = Logger.getSingleton(__name__, LogLevel.DEBUG)
 
     @staticmethod
     def joinArrayToStr(joinByStr, arr):
         return joinByStr.join(arr)
 
     @staticmethod
     def intersection(arr1, arr2):
         return list((set(arr1) & set(arr2)))
 
     @staticmethod
     def mergeByMatchingDictItemKeyInArray(dict1, dict2, matchKey):
-        return [ DictUtils.mergeDicts(x,y) if x[matchKey] == y[matchKey] else x  for x in dict1 for y in dict2 ]
+        return [DictUtils.mergeDicts(x, y) if x[matchKey] == y[matchKey] else x for x in dict1 for y in dict2]
 
     @staticmethod
     def mergeArray(d, u):
         uniq_list = []
         all_list = d + u
         for i in all_list:
             if i not in uniq_list:
@@ -135,14 +146,15 @@
     def getAllSubsetKeys(arr, parentArr):
         return [x for x in arr if ArrUtils.isSubset(parentArr, x)]
 
     @staticmethod
     def toDict(arr, key):
         return {item[key]: item for item in arr}
 
+
 class FileUtils():
     def __init__(self):
         self.__logger = Logger.getSingleton(__name__, LogLevel.DEBUG)
 
     def constructPath(self, dir, dest):
         return os.path.join(dir, dest)
 
@@ -171,15 +183,15 @@
             fileStr = file.read()
         return fileStr.replace("\n", " ") if removeLineBreaks else fileStr
 
     def readFile(self, filePath, startLineNum=0, endLineNum=None, removeLineBreaks=True):
         lines = []
         with open(filePath, 'r') as file:
             lines = file.readlines()
-        return [x.replace("\n","") for x in lines][startLineNum:endLineNum] if removeLineBreaks else lines[startLineNum:endLineNum]
+        return [x.replace("\n", "") for x in lines][startLineNum:endLineNum] if removeLineBreaks else lines[startLineNum:endLineNum]
 
     def writeToFile(self, filePath, data):
         with open(filePath, 'w') as file:
             file.write(data)
             file.close()
 
     def updateJsonFile(self, jsonFilePath, dictData):
@@ -193,17 +205,20 @@
         shutil.copy(srcFile, destFilePath)
 
     def rmDir(self, dirPath):
         if self.pathExists(dirPath):
             shutil.rmtree(dirPath)
 
 # https://github.com/kdart/pycopia/blob/1446fabaedf8c6bdd4ab1fc3f0ea731e0ef8da9d/aid/pycopia/dictlib.py
+
+
 class AttrDict(dict):
     """A dictionary with attribute-style access. It maps attribute access to
     the real dictionary.  """
+
     def __init__(self, *args, **kwargs):
         dict.__init__(self, *args, **kwargs)
 
     @staticmethod
     def formatList(value):
         return [AttrDict.formattedValueByType(item) for item in value]
 
@@ -247,22 +262,23 @@
 
     __getattr__ = __getitem__
     __setattr__ = __setitem__
 
     def copy(self):
         return AttrDict(self)
 
+
 class DictUtils:
     @staticmethod
     def getAllDictKeys(arr, d):
         for k, v in d.items():
             arr.append(k)
             if isinstance(d.get(k), dict) and isinstance(v, Mapping):
                 DictUtils.getAllDictKeys(arr, d.get(k, {}))
-                
+
     @staticmethod
     def getDictValue(d: dict, k: str, default=None):
         if k in d:
             return d[k]
         return default
 
     @staticmethod
@@ -276,52 +292,52 @@
     @staticmethod
     def isKeyInDict(d: dict, k: str) -> bool:
         if k in d:
             return True
         return False
 
     @staticmethod
-    def getValueFromKeyPath(key:str, dictionary: dict):
+    def getValueFromKeyPath(key: str, dictionary: dict):
         keys = key.split(".")
         return functools.reduce(lambda d, key: (d.get(key) if isinstance(d, dict) else None) if d else None, keys, dictionary)
 
     @staticmethod
     def mergeDicts(d, u):
         for k, v in u.items():
             if isinstance(d.get(k), dict) and isinstance(v, Mapping):
                 d[k] = DictUtils.mergeDicts(d.get(k, {}), v)
             else:
                 d[k] = v
         return d
 
     @staticmethod
     def filterDictByKeysList(dictionary: dict, visibleKeys: list) -> dict:
-        return {k: v for k, v in dictionary.items() if k in visibleKeys }
+        return {k: v for k, v in dictionary.items() if k in visibleKeys}
 
     @staticmethod
     def filterDictByKeysListNeg(dictionary: dict, visibleKeys: list) -> dict:
-        return {k: v for k, v in dictionary.items() if k not in visibleKeys }
+        return {k: v for k, v in dictionary.items() if k not in visibleKeys}
 
     @staticmethod
     def isAllKeyInDict(d: dict, keys: list) -> bool:
-        if all(key in d for key in keys): 
+        if all(key in d for key in keys):
             return True
         return False
 
     @staticmethod
     def createSubDict(d, keys):
-        return {x:d[x] for x in keys}
+        return {x: d[x] for x in keys}
 
     @staticmethod
     def createDic(**kwargs):
         return kwargs
 
     @staticmethod
     def sortByValues(d, isReverse):
-        sortedD = sorted(d.items(), key=lambda x:x[1], reverse=isReverse)
+        sortedD = sorted(d.items(), key=lambda x: x[1], reverse=isReverse)
         return dict(sortedD)
 
 
 class InstanceUtils():
     def __init__(self, instance):
         self.__instance = instance
         self.__modelSerializer = None
@@ -334,40 +350,41 @@
         return self.__instance
 
     def setModel(self, model):
         self.__model = model
 
     def setDataIndex(self, flag):
         self.__dataIndex = flag
-    
+
     def setModelSerializer(self, modelSerializer):
         self.__modelSerializer = modelSerializer
 
     def setQS(self, qs):
         self.__qs = qs
-    
+
     def getName(self):
         return self.__model.__name__
 
     def getQS(self):
         return self.__qs
-    
+
     def getModel(self):
         return self.__model
 
     def isDataIndex(self):
         return self.__dataIndex
-    
+
     def getModelSerializer(self):
         return self.__modelSerializer
 
 
 class Relation():
     ARG_QS = "qs"
     ARG_INSTANCE_UTILS = "instance_utils"
+
     def __init__(self, **kwargs):
         self.__instanceUtils = DictUtils.getDictValue(kwargs, self.ARG_INSTANCE_UTILS)
         self.__qs = DictUtils.getDictValue(kwargs, self.ARG_QS)
         self.__source = self.__instanceUtils(self.__qs.source)
         self.__target = self.__instanceUtils(self.__qs.target)
 
     def getTarget(self):
@@ -379,18 +396,18 @@
     def setName(self, newName):
         self.__qs.name = newName
 
     def getName(self):
         if hasattr(self.__qs, 'name'):
             return self.__qs.name
         return None
-    
+
     def getData(self):
         return self.__qs.getModelQSData()
-    
+
     def getTargetIdentifier(self):
         return self.__target.getInstance().identifier
 
     def getTargetExternalIdentifier(self):
         return self.__target.getInstance().external_identifier
 
     def getSourceIdentifier(self):
@@ -425,35 +442,36 @@
             linkVal = ":".join(self.getLink())
         return (self.getName(), self.getSourceIdentifier(), self.getSourceType(), self.getTargetIdentifier(), self.getTargetType(), linkVal)
 
 
 class Relations():
     def __init__(self):
         self.__dict = {}
-    
+
     def add(self, relation):
         key = relation.getUniqKey()
-        if not key in self.__dict:
+        if key not in self.__dict:
             self.__dict[key] = relation
 
     def get(self, key):
         return DictUtils.getDictValue(self.__dict, key)
 
     def remove(self, key):
         self.__dict.pop(key, None)
-            
+
     def getAll(self):
         return self.__dict
 
     def getIdentifiers(self):
-        identifiersSet =  {relation.getTargetIdentifier() for relation in self.__dict.values()}
+        identifiersSet = {relation.getTargetIdentifier() for relation in self.__dict.values()}
         return list(identifiersSet)
 
     def getExternalIdentifiers(self):
-        identifiersSet =  {relation.getTargetExternalIdentifier() for relation in self.__dict.values()}
+        identifiersSet = {relation.getTargetExternalIdentifier() for relation in self.__dict.values()}
         return list(identifiersSet)
 
+
 class ConfigUtils:
     @staticmethod
     def findConfigValues(config, paths):
         configs = [DictUtils.getValueFromKeyPath(path, config) for path in paths]
-        return configs 
+        return configs
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/core/yaml.py` & `kfsdutils-0.0.92/kfsdutils/apps/core/yaml.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/docs/templates/browser.html` & `kfsdutils-0.0.92/kfsdutils/apps/docs/templates/browser.html`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/docs/templates/skeleton.html` & `kfsdutils-0.0.92/kfsdutils/apps/docs/templates/skeleton.html`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/docs/views/apibrowser.py` & `kfsdutils-0.0.92/kfsdutils/apps/docs/views/apibrowser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """General API Views"""
 from typing import Any
 
 from django.urls import reverse
 from kfsdutils.apps.frontend.views.basetemplateview import BaseTemplateView
 from kfsdutils.apps.frontend.permissions.common import SignInRequired, IsStaff
 
+
 class APIBrowserView(BaseTemplateView):
     """Show browser view based on rapi-doc"""
 
     template_name = "browser.html"
     permission_classes = [SignInRequired, IsStaff]
 
     def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/endpoints/exceptions.py` & `kfsdutils-0.0.92/kfsdutils/apps/endpoints/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from rest_framework.exceptions import ValidationError
 from rest_framework.exceptions import APIException
-from rest_framework.exceptions import ValidationError
 from rest_framework.views import Response, exception_handler
 from rest_framework import status
 from django.core.exceptions import ValidationError as CoreValidationError
 from django.db import IntegrityError
 from django.conf import settings
-import json, traceback
+import json
+import traceback
+
 
 class KubefacetsAPIException(APIException):
     default_detail = "Unexpected Error"
     status_code = 500
     default_code = "unexpected_error"
 
     def __init__(self, detail, defaultCode, statusCode):
@@ -80,8 +81,8 @@
         response = Response(
             {
                 'detail': ex.detail,
                 'code': ex.default_code
             },
             status=ex.status_code
         )
-    return response
+    return response
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/basehandler.py` & `kfsdutils-0.0.92/kfsdutils/apps/endpoints/handlers/core/basehandler.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py` & `kfsdutils-0.0.92/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py` & `kfsdutils-0.0.92/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py` & `kfsdutils-0.0.92/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from rest_framework.test import APITestCase
 from django.urls import reverse
-from kfsdutils.apps.endpoints.handlers.core.utils import FileUtils, DictUtils
+from kfsdutils.apps.core.utils import FileUtils, DictUtils
+
 
 class EndpointsTestHandler(APITestCase):
 
     def setUp(self):
         self.__fileUtils = FileUtils()
         return super().setUp()
 
@@ -37,15 +38,14 @@
             for item in results:
                 strippedItem = self.stripCommonAttrs(item)
                 formattedResults.append(strippedItem)
 
         resp["results"] = formattedResults
         return resp
 
-
     def list(self, url, currentPg, expStatus, stripCommonAttrs=True):
         paginatedUrl = self.fetchPg(url, currentPg)
         response = self.client.get(paginatedUrl, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
         return self.stripCommonAttrsFromResults(response.data) if stripCommonAttrs else response.data
 
     def get(self, name, identifier, expStatus, stripCommonAttrs=True):
@@ -71,8 +71,7 @@
         return self.stripCommonAttrs(response.data) if stripCommonAttrs else response.data
 
     def delete(self, name, identifier, expStatus):
         detailUrl = self.detailView(name, identifier)
         response = self.client.delete(detailUrl, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
         return response
-
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/baseview.py` & `kfsdutils-0.0.92/kfsdutils/apps/endpoints/views/baseview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from rest_framework.pagination import PageNumberPagination
 from rest_framework import viewsets, filters
 from rest_framework.renderers import JSONRenderer
 from rest_framework import generics, status
 from rest_framework.views import Response
 
+
 class ModelPagination(PageNumberPagination):
     page_size = 20
 
+
 class BaseModelViewSet(viewsets.ModelViewSet):
     http_method_names = ['get', 'post', 'patch', 'delete']
     renderer_classes = [JSONRenderer]
     pagination_class = ModelPagination
     filter_backends = [filters.OrderingFilter]
     ordering = ['created']
 
+
 class CustomModelViewSet(viewsets.ModelViewSet):
     http_method_names = ['get', 'post', 'patch', 'delete']
     renderer_classes = [JSONRenderer]
     pagination_class = ModelPagination
     filter_backends = [filters.OrderingFilter]
     ordering = ['created']
     lookup_field = "identifier"
@@ -38,22 +41,23 @@
         if page is not None:
             serializer = self.get_serializer(page, many=True)
             return self.get_paginated_response(serializer.data)
 
         serializer = self.get_serializer(queryset, many=True)
         return Response(serializer.data)
 
+
 class CustomViewSet(generics.GenericAPIView):
     renderer_classes = [JSONRenderer]
     pagination_class = ModelPagination
 
     def processRequest(self, request):
         serializer = self.serializer_class(data=request.data)
         if serializer.is_valid():
             validated_data = serializer.validated_data
             validated_data["request"] = request
             return serializer.eval(validated_data)
         else:
-           return Response(serializer.errors, status.HTTP_400_BAD_REQUEST)
+            return Response(serializer.errors, status.HTTP_400_BAD_REQUEST)
 
     def post(self, request, *args, **kwargs):
-        return self.processRequest(request)
+        return self.processRequest(request)
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/apiclient.py` & `kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/apiclient.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/login.py` & `kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.auth.models import AnonymousUser
 from rest_framework import status
 from http import HTTPStatus
 
-from kfsdutils.apps.core.utils import DictUtils, ConfigUtils, GeneralUtils, HTTPUtils
+from kfsdutils.apps.core.utils import DictUtils, ConfigUtils, GeneralUtils
 from kfsdutils.apps.frontend.handlers.apiclient import APIClient
 from kfsdutils.apps.frontend.handlers.tokenuser import TokenUser
 
 
 class LoginHandler:
     EXPIRY_IN_MINS = "expiry_in_mins"
 
@@ -20,15 +20,15 @@
 
     def getRuntimeConfig(self):
         if getattr(self.__request, "config"):
             return self.__request.config
 
     def getConfigData(self):
         return self.getRuntimeConfig().getFinalConfig()
-    
+
     def getApplicationAuthReqHttpHeaders(self):
         return {
             'Content-Type': 'application/json',
             'X-CSRFToken': self.getRequest().COOKIES.get('csrftoken'),
             'X-APIKey': DictUtils.getValueFromKeyPath("auth_api.api_key", self.getConfigData())
         }
 
@@ -46,25 +46,25 @@
         return "/".join(args)
 
     def findConfigs(self, paths):
         return ConfigUtils.findConfigValues(
             self.getConfigData(),
             paths
         )
-    
+
     def getRegisterSuccessUrl(self):
         registerVerifySuccessUri = self.findConfigs(["auth_fe.register_verify_success_url"])[0]
         return registerVerifySuccessUri
 
     def getVerifyTempTokens(self, code):
         authHost, verifyTokensUri = self.findConfigs(["auth_api.host", "auth_api.verify_tmp_tokens_url"])
         verifyTokensUri = verifyTokensUri.format(code)
         verifyTokensUrl = self.formatUrl([authHost, verifyTokensUri])
         return self.httpGet(verifyTokensUrl, HTTPStatus.OK, self.getApplicationAuthReqHttpHeaders())
-    
+
     def userExists(self, email):
         authHost, userExistsUri, userIdentifierPrefix = self.findConfigs(["auth_api.host", "auth_api.user_exists_url", "auth_api.user_identifier_prefix"])
         userIdentifier = userIdentifierPrefix.format(email)
         userExistsUri = userExistsUri.format(GeneralUtils.genUrlEncode(userIdentifier))
         userExistsUrl = self.formatUrl([authHost, userExistsUri])
         return self.httpGet(userExistsUrl, HTTPStatus.OK, self.getApplicationAuthReqHttpHeaders())
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/tokenuser.py` & `kfsdutils-0.0.92/kfsdutils/apps/frontend/handlers/tokenuser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from rest_framework import status
 from django.utils.functional import cached_property
 
-from kfsdutils.apps.core.utils import ConfigUtils, DictUtils, HTTPUtils
+from kfsdutils.apps.core.utils import ConfigUtils, DictUtils
 from kfsdutils.apps.frontend.handlers.apiclient import APIClient
 
+
 class TokenUser:
     is_active = True
 
     def __init__(self, request, token):
         self.__client = APIClient()
         self.__token = token
         self.__request = request
         self.__tokenPayload = self.genTokenPayload()
         if not self.__tokenPayload:
             raise Exception("Invalid token data found")
 
     def getConfigData(self):
         return self.getRequest().config.getFinalConfig()
-    
+
     def getRequest(self):
         return self.__request
-    
+
     def findConfigs(self, paths):
         return ConfigUtils.findConfigValues(
             self.getConfigData(),
             paths
         )
-    
+
     def formatUrl(self, args):
         return "/".join(args)
-    
+
     def getHttpHeaders(self):
         return {
             'Content-Type': 'application/json',
             'X-CSRFToken': self.getRequest().COOKIES.get('csrftoken'),
             'X-APIKey': DictUtils.getValueFromKeyPath("auth_api.api_key", self.getConfigData())
         }
 
@@ -61,18 +62,18 @@
         return DictUtils.getDictValue(self.__tokenPayload, "last_name")
 
     def is_staff(self):
         return DictUtils.getDictValue(self.__tokenPayload, "is_staff", False)
 
     def is_superuser(self):
         return DictUtils.getDictValue(self.__tokenPayload, "is_superuser", False)
-    
+
     def is_email_verified(self):
         return DictUtils.getDictValue(self.__tokenPayload, "is_email_verified", False)
-    
+
     @cached_property
     def is_anonymous(self):
         return False
 
     @cached_property
     def is_authenticated(self):
         return True
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/base.py` & `kfsdutils-0.0.92/kfsdutils/apps/frontend/permissions/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from kfsdutils.apps.core.utils import DictUtils
 
+
 class BasePermission:
     def __init__(self, request):
         self.__request = request
 
     def getRequest(self):
         return self.__request
-    
+
     def getConfigData(self):
         return self.__request.config.getFinalConfig()
-    
+
     def getUser(self):
         return self.getRequest().user
-    
+
     def getConfigValue(self, path):
         return DictUtils.getValueFromKeyPath(path, self.getConfigData())
-    
+
     def constructUrl(self, paths):
         return "/".join(paths)
-    
+
     def getConfigPaths(self, paths):
-        return [ DictUtils.getValueFromKeyPath(path, self.getConfigData()) for path in paths]
-    
+        return [DictUtils.getValueFromKeyPath(path, self.getConfigData()) for path in paths]
+
     def getHttpHost(self):
         return self.getRequest().META.get('HTTP_HOST')
-    
+
     def getHttpPath(self):
         return self.getRequest().META.get('PATH_INFO')
-    
+
     def getRefererUrl(self):
         return self.getRequest().META.get('HTTP_REFERER')
-    
+
     def getCurrentRequestUrl(self):
         return self.getRequest().build_absolute_uri()
-
-    
-
-
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/common.py` & `kfsdutils-0.0.92/kfsdutils/apps/frontend/permissions/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,110 @@
 from kfsdutils.apps.frontend.permissions.base import BasePermission
 from kfsdutils.apps.frontend.exceptions import FEException
 from kfsdutils.apps.core.utils import GeneralUtils
 from http import HTTPStatus
 
+
 class SignInRequired(BasePermission):
     def __init__(self, request):
         BasePermission.__init__(self, request)
 
     def __str__(self):
         return "Is authenticated check"
 
     def is_valid(self):
-       if self.getUser().is_authenticated:
-           return True
-       return False
-       
+        if self.getUser().is_authenticated:
+            return True
+        return False
+
     def raise_exception(self):
         raise FEException(self.__str__(), HTTPStatus.TEMPORARY_REDIRECT, self.redirect_url())
-    
+
     def redirect_url(self):
         loginUrl = self.constructUrl(self.getConfigPaths(["auth_fe.host", "auth_fe.login_url"]))
         loginUrl += "?next={}".format(GeneralUtils.genUrlEncode(self.getCurrentRequestUrl()))
         return loginUrl
-    
+
     def redirect_url_neg(self):
         verifiedFinalUrl = self.constructUrl(self.getConfigPaths(["auth_fe.register_verify_success_url"]))
         return verifiedFinalUrl
-    
+
     def raise_exception_neg(self):
         raise FEException(self.__str__(), HTTPStatus.TEMPORARY_REDIRECT, self.redirect_url_neg())
-    
+
 
 class SignUpEmailVerifiedStatusRequired(BasePermission):
     def __init__(self, request):
         BasePermission.__init__(self, request)
 
     def __str__(self):
         return "Is email verified check"
 
     def is_valid(self):
-       if self.getUser().is_authenticated and self.getUser().is_email_verified():
-           return True
-       return False
-       
+        if self.getUser().is_authenticated and self.getUser().is_email_verified():
+            return True
+        return False
+
     def raise_exception(self):
         raise FEException(self.__str__(), HTTPStatus.TEMPORARY_REDIRECT, self.redirect_url())
-    
+
     def redirect_url(self):
         verifyEmailUrl = self.constructUrl(self.getConfigPaths(["auth_fe.host", "auth_fe.verify_email_url"]))
-        verifyEmailUrl +="?next={}".format(GeneralUtils.genUrlEncode(self.getCurrentRequestUrl()))
+        verifyEmailUrl += "?next={}".format(GeneralUtils.genUrlEncode(self.getCurrentRequestUrl()))
         return verifyEmailUrl
-    
+
     def redirect_url_neg(self):
         verifiedFinalUrl = self.constructUrl(self.getConfigPaths(["auth_fe.register_verify_success_url"]))
         return verifiedFinalUrl
-    
+
     def raise_exception_neg(self):
         raise FEException(self.__str__(), HTTPStatus.TEMPORARY_REDIRECT, self.redirect_url_neg())
-    
+
 
 class IsStaff(BasePermission):
     def __init__(self, request):
         BasePermission.__init__(self, request)
 
     def __str__(self):
         return "Is staff check"
 
     def is_valid(self):
-       if self.getUser().is_authenticated and self.getUser().is_email_verified() and self.getUser().is_staff():
-           return True
-       return False
-       
+        if self.getUser().is_authenticated and self.getUser().is_email_verified() and self.getUser().is_staff():
+            return True
+        return False
+
     def raise_exception(self):
         raise FEException(self.__str__(), HTTPStatus.FORBIDDEN, None)
-    
+
     def redirect_url(self):
         return ""
-    
+
     def redirect_url_neg(self):
         return ""
-    
+
     def raise_exception_neg(self):
         raise FEException(self.__str__(), HTTPStatus.FORBIDDEN, None)
-    
+
 
 class IsSuperUser(BasePermission):
     def __init__(self, request):
         BasePermission.__init__(self, request)
 
     def __str__(self):
         return "Is staff check"
 
     def is_valid(self):
-       if self.getUser().is_authenticated and self.getUser().is_email_verified() and self.getUser().is_superuser():
-           return True
-       return False
-       
+        if self.getUser().is_authenticated and self.getUser().is_email_verified() and self.getUser().is_superuser():
+            return True
+        return False
+
     def raise_exception(self):
         raise FEException(self.__str__(), HTTPStatus.FORBIDDEN, None)
-    
+
     def redirect_url(self):
         return ""
-    
+
     def redirect_url_neg(self):
         return ""
-    
+
     def raise_exception_neg(self):
-        raise FEException(self.__str__(), HTTPStatus.FORBIDDEN, None)
+        raise FEException(self.__str__(), HTTPStatus.FORBIDDEN, None)
```

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseformview.py` & `kfsdutils-0.0.92/kfsdutils/apps/frontend/views/baseformview.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseview.py` & `kfsdutils-0.0.92/kfsdutils/apps/frontend/views/baseview.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/middleware/configuration.py` & `kfsdutils-0.0.92/kfsdutils/apps/middleware/configuration.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.91/kfsdutils/apps/models/basemodel.py` & `kfsdutils-0.0.92/kfsdutils/apps/models/basemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def get_by_natural_key(self, identifier):
         return self.get(identifier=identifier)
 
 
 class BaseModel(models.Model):
     class Meta:
         abstract = True
-        
+
     identifier = models.CharField(
         unique=True,
         max_length=MAX_LENGTH,
         validators=[
             RegexValidator(
                 regex=IDENTIFIER_REGEX_CONDITION,
                 message="identifier doesnt match condition {}".format(IDENTIFIER_REGEX_CONDITION)
```

### Comparing `kfsdutils-0.0.91/kfsdutils.egg-info/SOURCES.txt` & `kfsdutils-0.0.92/kfsdutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 kfsdutils/__init__.py
+kfsdutils/asgi.py
+kfsdutils/settings.py
+kfsdutils/urls.py
+kfsdutils/wsgi.py
 kfsdutils.egg-info/PKG-INFO
 kfsdutils.egg-info/SOURCES.txt
 kfsdutils.egg-info/dependency_links.txt
 kfsdutils.egg-info/not-zip-safe
 kfsdutils.egg-info/requires.txt
 kfsdutils.egg-info/top_level.txt
 kfsdutils/apps/__init__.py
@@ -27,17 +31,21 @@
 kfsdutils/apps/docs/tests/__init__.py
 kfsdutils/apps/docs/tests/test_apibrowserview.py
 kfsdutils/apps/docs/views/__init__.py
 kfsdutils/apps/docs/views/apibrowser.py
 kfsdutils/apps/endpoints/__init__.py
 kfsdutils/apps/endpoints/apps.py
 kfsdutils/apps/endpoints/exceptions.py
+kfsdutils/apps/endpoints/urls.py
 kfsdutils/apps/endpoints/handlers/__init__.py
 kfsdutils/apps/endpoints/handlers/core/__init__.py
+kfsdutils/apps/endpoints/handlers/core/apikeyuser.py
 kfsdutils/apps/endpoints/handlers/core/basehandler.py
+kfsdutils/apps/endpoints/middleware/__init__.py
+kfsdutils/apps/endpoints/middleware/be_auth.py
 kfsdutils/apps/endpoints/renderers/__init__.py
 kfsdutils/apps/endpoints/renderers/kubefacetsjson.py
 kfsdutils/apps/endpoints/renderers/kubefacetstext.py
 kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py
 kfsdutils/apps/endpoints/serializers/__init__.py
 kfsdutils/apps/endpoints/serializers/base.py
 kfsdutils/apps/endpoints/serializers/basemodel.py
```

