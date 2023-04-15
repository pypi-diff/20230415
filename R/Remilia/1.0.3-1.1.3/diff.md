# Comparing `tmp/Remilia-1.0.3.tar.gz` & `tmp/Remilia-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Remilia-1.0.3.tar", last modified: Wed Apr  5 03:48:40 2023, max compression
+gzip compressed data, was "Remilia-1.1.3.tar", last modified: Sat Apr 15 03:22:22 2023, max compression
```

## Comparing `Remilia-1.0.3.tar` & `Remilia-1.1.3.tar`

### file list

```diff
@@ -1,71 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-05 03:48:28.000000 Remilia-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-05 03:48:40.709884 Remilia-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-05 03:48:28.000000 Remilia-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.705884 Remilia-1.0.3/Remilia/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-05 03:48:40.000000 Remilia-1.0.3/Remilia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.705884 Remilia-1.0.3/Remilia/base/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/base/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/base/directorys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/base/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/base/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.705884 Remilia-1.0.3/Remilia/jsondb/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/jsondb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/jsondb/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/jsondb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/jsondb/dbbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/lite/
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteData.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteI18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LitePGL.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteResource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/LiteThread.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/lite/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/v2/ClassMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/v2/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/v2/DictoryTreeBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/lite/v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/DecoratorUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/SignParas.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/cli/async_app/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/async_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/cli/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/prompts/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/prompts/confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/prompts/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/prompts/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/net/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/net/pixiv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/os/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/os/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/os/win/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/os/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/os/win/exeutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.709884 Remilia-1.0.3/Remilia/utils/thread/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/thread/Timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-05 03:48:28.000000 Remilia-1.0.3/Remilia/utils/thread/terminable_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:48:40.705884 Remilia-1.0.3/Remilia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-05 03:48:40.000000 Remilia-1.0.3/Remilia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-05 03:48:40.000000 Remilia-1.0.3/Remilia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 03:48:40.000000 Remilia-1.0.3/Remilia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-05 03:48:40.000000 Remilia-1.0.3/Remilia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 03:48:40.000000 Remilia-1.0.3/Remilia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 03:48:40.709884 Remilia-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-05 03:48:28.000000 Remilia-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-15 03:22:11.000000 Remilia-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-15 03:22:22.483135 Remilia-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-15 03:22:11.000000 Remilia-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/directorys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/jsondb/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/dbbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/lite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LitePGL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteResource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/lite/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/ClassMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/DictoryTreeBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/InstanceManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/DecoratorUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/SignParas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/cli/prompts_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/cli/prompts_extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/net/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/net/pixiv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/os/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/os/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/os/win/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/os/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/os/win/exeutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/thread/Timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/thread/terminable_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:22:22.483135 Remilia-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-15 03:22:11.000000 Remilia-1.1.3/setup.py
```

### Comparing `Remilia-1.0.3/LICENSE` & `Remilia-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/PKG-INFO` & `Remilia-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Remilia
-Version: 1.0.3
+Version: 1.1.3
 Summary: Use python with dignity,here offer a tookit
 Home-page: https://github.com/IAXRetailer/Remilia
 Author: h2sxxa
 Author-email: H2Sxxa0w0@gmail.com
 Maintainer: h2sxxa
 Maintainer-email: H2Sxxa0w0@gmail.com
 License: MIT License
```

### Comparing `Remilia-1.0.3/README.md` & `Remilia-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/base/events.py` & `Remilia-1.1.3/Remilia/base/events.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/base/files.py` & `Remilia-1.1.3/Remilia/base/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from abc import ABC,abstractmethod
 
-from ..lite.LiteResource import File,Directory, PathError
-
+from ..lite.LiteResource import Directory, PathError
 
+from ..lite.LiteResource import File
 class CommonFileBase(ABC):
     def __init__(
         self,
-        File:File,
+        _file:File,
         noneText:str=""
         ) -> None:
         self.noneText=noneText
-        self.File=File
+        
+        if isinstance(File,File):
+            _file=File(File)
+        
+        self.File=_file
         if not File.isexist or File.text == "":
             File.write("w",noneText)
     
     @abstractmethod
     def _read(
         self,
         *args,
```

### Comparing `Remilia-1.0.3/Remilia/base/types.py` & `Remilia-1.1.3/Remilia/base/types.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/jsondb/db.py` & `Remilia-1.1.3/Remilia/jsondb/db.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/jsondb/dbbase.py` & `Remilia-1.1.3/Remilia/jsondb/dbbase.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/LiteData.py` & `Remilia-1.1.3/Remilia/lite/LiteData.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/LiteFunctions.py` & `Remilia-1.1.3/Remilia/lite/utils.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/LiteLog.py` & `Remilia-1.1.3/Remilia/lite/LiteLog.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/LiteMixin.py` & `Remilia-1.1.3/Remilia/lite/LiteMixin.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/LiteResource.py` & `Remilia-1.1.3/Remilia/lite/LiteResource.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/LiteThread.py` & `Remilia-1.1.3/Remilia/lite/LiteThread.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/v2/ClassMixin.py` & `Remilia-1.1.3/Remilia/lite/v2/ClassMixin.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/lite/v2/ConfigManager.py` & `Remilia-1.1.3/Remilia/lite/v2/ConfigManager.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,24 @@
         '''
         for k,v in kwargs.items():
             setattr(self,k,v)
         if not self.path:
             raise ConfigError("can't go on without a path")
         else:
             self.model_ins=self.model(File(self.path))
+            
+    def replace_ins(self,path:str):
+        self.path=path
+        self.model_ins=self.model(File(self.path))
+        return self
+    
+    def replace_model(self,model:KVFileBase):
+        self.model=model
+        return self
+    
 class Cate:
     def __call__(self,obj) -> "_getObj":
         self._obj=obj()
         obj=self._obj
         return self
     
     def _withObj(self,obj):
@@ -64,14 +74,16 @@
     
     def _toDict(self) -> dict:
         fin={}
         for liter in collect_attr(self._obj):
             for k,v in liter.items():
                 if isinstance(v,Cate):
                     fin.update({k:v._toDict()})
+                elif isinstance(v,Temp):
+                    fin.update({k:v.__to_dict__()})
                 else:
                     fin.update({k:v})
         return fin
 
 class Config:
     def __init__(self,setting:ConfigSetting) -> None:
         self._setting=setting
@@ -84,51 +96,61 @@
         for liter in collect_attr(target):
             for k,v in liter.items():
                 if isinstance(v,Cate):
                     self._setting.model_ins.write(k,v._toDict())
                 elif isinstance(v,Temp):
                     self._setting.model_ins.write(k,v.__to_dict__())
                 else:
+                    #print(v,type(v))
                     self._setting.model_ins.write(k,v)
-
+        return self
     def _get(self,target):
         for k,v in self._setting.model_ins.FileDict.items():
             if isinstance(v,dict):
                 if hasattr(target,k) and isinstance(getattr(target,k),Cate):
                     safe_mixin(getattr(target,k),Temp().__to_class__(v))
                     safe_mixin(getattr(target,k)._getObj(),Temp().__to_class__(v))
                 elif isinstance(getattr(target,k),Cate):
                     fin=Cate()._handle_temp(Temp().__to_class__(v))
                     safe_mixin(fin,Temp().__to_class__(v))
                     setattr(target,k,fin)
                 else:
                     setattr(target,k,v)
             else:
                 setattr(target,k,v)
-                
+        return self
     def _sync(self):
         try:
             self._get(self._obj)
         except:
             pass
         self._push(self._obj)
         self._get(self._obj)
-        
+        return self
+    
     def _regenerate(self):
         try:
             self._get(self._obj)
         except:
             pass
         for liter in collect_attr(self._obj):
             for k,v in liter.items():
                 if hasattr(self._rawobj,k):
                     setattr(self._rawobj,k,v)
         self._setting.model_ins.File.write("w","{}")
         self._push(self._rawobj)
-        
+        return self
+    
+    def _modify(self,name,obj):
+        setattr(self._obj,name,obj)
+        return self
+    
+    def _modify_push(self,name,obj):
+        return self._modify(name,obj)._push(self._obj)._get(self._obj)
+    
     def __call__(self,obj):
         self._rawobj=obj()
         obj=obj()
         self._obj=obj
         if self._setting.regenerate:
             self._regenerate()
         self._sync()
```

### Comparing `Remilia-1.0.3/Remilia/lite/v2/DictoryTreeBuilder.py` & `Remilia-1.1.3/Remilia/lite/v2/DictoryTreeBuilder.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/utils/DecoratorUtils.py` & `Remilia-1.1.3/Remilia/utils/DecoratorUtils.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/utils/SignParas.py` & `Remilia-1.1.3/Remilia/utils/SignParas.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/utils/net/pixiv.py` & `Remilia-1.1.3/Remilia/utils/net/pixiv.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/utils/thread/Timeout.py` & `Remilia-1.1.3/Remilia/utils/thread/Timeout.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia/utils/thread/terminable_thread.py` & `Remilia-1.1.3/Remilia/utils/thread/terminable_thread.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.0.3/Remilia.egg-info/PKG-INFO` & `Remilia-1.1.3/Remilia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Remilia
-Version: 1.0.3
+Version: 1.1.3
 Summary: Use python with dignity,here offer a tookit
 Home-page: https://github.com/IAXRetailer/Remilia
 Author: h2sxxa
 Author-email: H2Sxxa0w0@gmail.com
 Maintainer: h2sxxa
 Maintainer-email: H2Sxxa0w0@gmail.com
 License: MIT License
```

### Comparing `Remilia-1.0.3/Remilia.egg-info/SOURCES.txt` & `Remilia-1.1.3/Remilia.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,39 +15,33 @@
 Remilia/base/types.py
 Remilia/jsondb/__init__.py
 Remilia/jsondb/builder.py
 Remilia/jsondb/db.py
 Remilia/jsondb/dbbase.py
 Remilia/lite/LiteData.py
 Remilia/lite/LiteEvent.py
-Remilia/lite/LiteFunctions.py
-Remilia/lite/LiteI18n.py
 Remilia/lite/LiteLog.py
 Remilia/lite/LiteMixin.py
 Remilia/lite/LitePGL.py
 Remilia/lite/LiteResource.py
-Remilia/lite/LiteTasks.py
 Remilia/lite/LiteThread.py
 Remilia/lite/__init__.py
+Remilia/lite/utils.py
 Remilia/lite/v2/ClassMixin.py
 Remilia/lite/v2/ConfigManager.py
 Remilia/lite/v2/DictoryTreeBuilder.py
+Remilia/lite/v2/InstanceManager.py
 Remilia/lite/v2/__init__.py
+Remilia/lite/v2/i18n.py
 Remilia/lite/v2/utils.py
 Remilia/utils/DecoratorUtils.py
 Remilia/utils/SignParas.py
 Remilia/utils/__init__.py
 Remilia/utils/cli/__init__.py
-Remilia/utils/cli/utils.py
-Remilia/utils/cli/async_app/__init__.py
-Remilia/utils/cli/prompts/__init__.py
-Remilia/utils/cli/prompts/checkbox.py
-Remilia/utils/cli/prompts/confirm.py
-Remilia/utils/cli/prompts/input.py
-Remilia/utils/cli/prompts/list.py
+Remilia/utils/cli/prompts_extension/__init__.py
 Remilia/utils/net/__init__.py
 Remilia/utils/net/pixiv.py
 Remilia/utils/os/__init__.py
 Remilia/utils/os/win/__init__.py
 Remilia/utils/os/win/exeutils.py
 Remilia/utils/thread/Timeout.py
 Remilia/utils/thread/__init__.py
```

### Comparing `Remilia-1.0.3/setup.py` & `Remilia-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 # coding=utf-8
 
+from time import localtime, strftime
 from setuptools import setup, find_packages
 from requests import get
 from requests import get
 from json import loads
+from sys import argv
 
-ver=loads(get("https://api.github.com/repos/IAXRetailer/Remilia/releases/latest").text)["tag_name"]
+ver=loads(get("https://api.github.com/repos/IAXRetailer/Remilia/releases").text)[0]["tag_name"]
 
 with open("Remilia/__init__.py","r",encoding="utf-8") as pkg:
     text=pkg.read().replace("#__VERSION__#","__version__=\"%s\""%ver)
     
 with open("Remilia/__init__.py","w",encoding="utf-8") as pkg:
     pkg.write(text)
 
@@ -39,9 +41,10 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     ],
     install_requires = [
         "colorama",
         "pyyaml",
+        "noneprompt",
         ]
 )
```

