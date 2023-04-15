# Comparing `tmp/pygpt-net-0.9.3.tar.gz` & `tmp/pygpt-net-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt-net-0.9.3.tar", last modified: Fri Apr 14 00:01:14 2023, max compression
+gzip compressed data, was "pygpt-net-0.9.4.tar", last modified: Sat Apr 15 04:40:42 2023, max compression
```

## Comparing `pygpt-net-0.9.3.tar` & `pygpt-net-0.9.4.tar`

### file list

```diff
@@ -1,98 +1,110 @@
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1077 2023-04-10 01:01:37.000000 pygpt-net-0.9.3/LICENSE
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    17182 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/PKG-INFO
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    15095 2023-04-14 00:01:05.000000 pygpt-net-0.9.3/README.md
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     1146 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/pyproject.toml
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/setup.cfg
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     1470 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/setup.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.015881 pygpt-net-0.9.3/src/
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      245 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/src/pygpt_net/CHANGELOG.txt
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      844 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/src/pygpt_net/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      553 2023-04-13 21:40:18.000000 pygpt-net-0.9.3/src/pygpt_net/app.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/core/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/__init__.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     4245 2023-04-12 18:28:43.000000 pygpt-net-0.9.3/src/pygpt_net/core/app.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    15134 2023-04-13 23:44:00.000000 pygpt-net-0.9.3/src/pygpt_net/core/config.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13292 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/context.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/core/controller/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/__init__.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1662 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/confirm.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5161 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/context.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1516 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/debug.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4793 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/image.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1806 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/info.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4325 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/input.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    10565 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/lang.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1340 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/launcher.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1968 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/main.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    12782 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/model.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3123 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/output.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      657 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/plugins.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    11561 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/presets.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13921 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/settings.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     7164 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/theme.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2601 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/ui.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/core/debug/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/__init__.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      988 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/config.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2110 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/context.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1554 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/models.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1954 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/presets.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3699 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/debugger.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9122 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/gpt.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1737 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/history.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2467 2023-04-11 05:25:57.000000 pygpt-net-0.9.3/src/pygpt_net/core/image.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      832 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/info.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1926 2023-04-13 23:39:46.000000 pygpt-net-0.9.3/src/pygpt_net/core/locale.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2431 2023-04-11 05:19:58.000000 pygpt-net-0.9.3/src/pygpt_net/core/settings.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4501 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/tokens.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/core/ui/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3043 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/chatbox.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3324 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/contexts.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3170 2023-04-13 23:41:43.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/about.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1724 2023-04-13 23:40:57.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/changelog.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      966 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/ctx_rename.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1253 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/debug.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2334 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/editor.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1817 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/image.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6330 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/preset.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9119 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/settings.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2300 2023-04-13 23:40:50.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/start.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      822 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/update.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4169 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialogs.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3899 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/input.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2426 2023-04-12 19:39:35.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/main.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8459 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/menu.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1008 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/status.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8550 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/toolbox.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    24147 2023-04-13 23:40:34.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/widgets.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6275 2023-04-13 21:15:52.000000 pygpt-net-0.9.3/src/pygpt_net/core/updater.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1220 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/utils.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/config/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1052 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/config.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      669 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/models.json
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      255 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/batman_and_joker.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      287 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/current.chat.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      276 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/current.completion.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      259 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/current.img.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      273 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/dalle_covboy_tokio.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      525 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3461 2023-04-09 19:13:26.000000 pygpt-net-0.9.3/src/pygpt_net/data/icon.ico
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13970 2023-04-09 19:12:56.000000 pygpt-net-0.9.3/src/pygpt_net/data/icon.png
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/locale/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5410 2023-04-12 07:50:37.000000 pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.en.ini
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5935 2023-04-12 07:50:37.000000 pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.pl.ini
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9703 2023-04-09 19:29:44.000000 pygpt-net-0.9.3/src/pygpt_net/data/logo.png
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net.egg-info/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    17182 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/PKG-INFO
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     2939 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/SOURCES.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)        1 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/dependency_links.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       49 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/entry_points.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      138 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/requires.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       10 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/top_level.txt
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1077 2023-04-10 01:01:37.000000 pygpt-net-0.9.4/LICENSE
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)    18300 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/PKG-INFO
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    16213 2023-04-15 03:36:32.000000 pygpt-net-0.9.4/README.md
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     1146 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/pyproject.toml
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/setup.cfg
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     1470 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/setup.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.436739 pygpt-net-0.9.4/src/
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.436739 pygpt-net-0.9.4/src/pygpt_net/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      290 2023-04-15 00:06:51.000000 pygpt-net-0.9.4/src/pygpt_net/CHANGELOG.txt
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      844 2023-04-14 20:15:03.000000 pygpt-net-0.9.4/src/pygpt_net/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      553 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/app.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/__init__.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     5068 2023-04-15 04:06:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/app.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    15069 2023-04-15 04:04:45.000000 pygpt-net-0.9.4/src/pygpt_net/core/config.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13637 2023-04-15 04:18:58.000000 pygpt-net-0.9.4/src/pygpt_net/core/context.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/controller/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1662 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/confirm.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5161 2023-04-15 04:10:26.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/context.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1516 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/debug.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     4969 2023-04-15 01:05:50.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/image.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1806 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/info.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5700 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/input.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    10570 2023-04-14 23:30:39.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/lang.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1340 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/launcher.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2040 2023-04-15 04:09:34.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/main.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    12782 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/model.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3558 2023-04-15 02:57:48.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/output.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13609 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/plugins.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    14522 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/presets.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13247 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/settings.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9135 2023-04-14 22:32:15.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/theme.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2601 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/ui.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/debug/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      988 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/config.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2110 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/context.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1554 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/models.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     1638 2023-04-15 04:02:02.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/plugins.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1954 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/presets.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3800 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/core/debugger.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8506 2023-04-15 03:04:36.000000 pygpt-net-0.9.4/src/pygpt_net/core/gpt.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1737 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/history.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2467 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/image.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      832 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/info.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1926 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/locale.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/plugin/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      488 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/__init__.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     2062 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/base_plugin.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/plugin/real_time/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      488 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/real_time/__init__.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     4205 2023-04-15 03:28:35.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/real_time/plugin.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/plugin/self_loop/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      488 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/self_loop/__init__.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     4421 2023-04-15 03:28:35.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/self_loop/plugin.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     2775 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugins.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2467 2023-04-15 00:16:54.000000 pygpt-net-0.9.4/src/pygpt_net/core/settings.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     4501 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/tokens.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/ui/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3238 2023-04-14 23:23:11.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/chatbox.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3324 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/contexts.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3170 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/about.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1724 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/changelog.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      966 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/ctx_rename.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1518 2023-04-15 03:49:50.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/debug.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2334 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/editor.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1817 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/image.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     6929 2023-04-14 23:06:24.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/plugins.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6330 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/preset.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9119 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/settings.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2300 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/start.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      822 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/update.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     4238 2023-04-14 22:11:32.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialogs.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3904 2023-04-15 01:39:43.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/input.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2186 2023-04-14 17:23:37.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/main.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9065 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/menu.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1008 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/status.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8550 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/toolbox.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    24651 2023-04-15 01:39:43.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/widgets.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6588 2023-04-15 04:07:29.000000 pygpt-net-0.9.4/src/pygpt_net/core/updater.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1464 2023-04-15 04:03:17.000000 pygpt-net-0.9.4/src/pygpt_net/core/utils.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/config/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1357 2023-04-15 04:24:04.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/config.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      669 2023-04-15 04:24:04.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/models.json
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      255 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      287 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/current.chat.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      276 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/current.completion.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      259 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/current.img.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      273 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/dalle_covboy_tokio.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      525 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3461 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/icon.ico
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13970 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/icon.png
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/locale/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5548 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.en.ini
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6082 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.pl.ini
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9703 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/logo.png
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.436739 pygpt-net-0.9.4/src/pygpt_net.egg-info/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)    18300 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/PKG-INFO
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     3312 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)        1 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       49 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/entry_points.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      138 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/requires.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       10 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/top_level.txt
```

### Comparing `pygpt-net-0.9.3/LICENSE` & `pygpt-net-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/PKG-INFO` & `pygpt-net-0.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 0.9.3
+Version: 0.9.4
 Summary: A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
 Home-page: https://github.com/szczyglis-dev/py-gpt
 Author: Marcin Szczygliński
 Author-email: Marcin Szczygliński <info@pygpt.net>
 Maintainer: Marcin Szczygliński
 Maintainer-email: info@pygpt.net
 License: MIT License
@@ -34,26 +34,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Current release: **0.9.3** (build: **2023.04.14**)
-
-Official website: https://pygpt.net
+# PYGPT
 
-Documentation: https://pygpt.readthedocs.io
+Current release: **0.9.4** (build: **2023.04.15**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
 
 PyPi: https://pypi.org/project/pygpt-net
 
 ### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
 
-# PYGPT
-
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
 artificial intelligence models such as **GPT4** and **GPT3** using your
 own computer and `OpenAI API`. It allows you to talk in chat mode and in
 completion mode, as well as generate images using **DALL-E 2**.
 Moreover, the application has implemented context memory support,
@@ -79,14 +75,15 @@
 - allows you to easily manage prompts with handly editable presets
 - intuitive operation and interface
 - allows you to use all the powerful features of `GPT4` and `GPT3`
 - no knowledge of using AI models required
 - enables easy and convenient generation of images using `DALL-E 2`
 - has the ability to support future OpenAI models
 - fully configurable
+- plugins support
 - built-in tokens usage calculation
 - it\'s open source, source code is available on `GitHub`
 - **uses the user\'s API key**
 
 The application is free, open source and runs on PC with `Windows 10`,
 `Windows 11` and `Linux`. The full **Python** source code is available
 on `GitHub`.
@@ -126,14 +123,29 @@
 
 3. Once installed run the command to start the application:
 
 ``` commandline
 pygpt
 ```
 
+**Troubleshooting**: 
+
+If you have problems with xcb plugin with newer versions of PySide on Linux, e.g. like this:
+
+```commandline
+qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+```
+
+...then try downgrading PySide to `PySide6-Essentials==6.4.2`:
+
+```commandline
+pip install PySide6-Essentials==6.4.2
+```
+
 ### Running from GitHub source code
 
 1. Clone git repository or download .zip file:
 
 ```commandline
 git clone https://github.com/szczyglis-dev/py-gpt.git
 cd py-gpt
@@ -155,14 +167,17 @@
 4. Run the application:
 
 ```commandline
 cd src/pygpt_net
 python app.py
 ```
 
+**Tip**: you can use `PyInstaller` to create a compiled version of
+the application for your system.
+
 ## Other requirements
 
 To operate, you need an Internet connection (for API connection),
 registered OpenAI account and an active API key, which must be entered
 in the program.
 
 
@@ -336,14 +351,25 @@
 **Tip:** with presets, you can save prepared prompts and use them later
 when generating subsequent images.
 
 All queries are saved in the history, thanks to which you can return to
 a given session at any time and use old queries to, for example,
 generate new content.
 
+## Plugins
+
+The application allows you to use plugins to extend its functionality.
+Currently, the following plugins are available:
+
+- **SelfLoop** - allows to run GPT in a self-loop, which allows you to
+  generate a continuous conversation between AI <> AI. In this mode model talks to itself.
+
+- **RealTime** - auto-append current date and time to the prompt. It tells
+  the model what time it is in real time.
+
 
 # Tokens calculation
 
 ## Input tokens
 
 Calculation of tokens is implemented in the application. The application
 tries to predict the number of tokens that will be used for a given
@@ -490,15 +516,19 @@
 
 Support for plug-ins and voice recognition and synthesis will be added
 in future versions of the application.
 
 
 # CHANGELOG
 
-## v0.9.3 (2023.04.13)
+## v0.9.4 (2023.04.15)
+
+- added plugins support
+
+## v0.9.3 (2023.04.14)
 
 - packed into PyPI package
 
 ## v0.9.2 (2023.04.12)
 
 - added theme color settings
 - small UI fixes
@@ -508,21 +538,23 @@
 - added organization key configuration (by @kaneda2004, PR#1)
 - added config versions patching
 
 ## v0.9.0 (2023.04.09)
 
 - initial release
 
-# Credits
+# Credits and links
 
 **Official website:** <https://pygpt.net>
 
 **Documentation:** <https://pygpt.readthedocs.io>
 
 **GitHub:** <https://github.com/szczyglis-dev/py-gpt>
 
+**PyPI:** <https://pypi.org/project/pygpt-net>
+
 **Author:** Marcin Szczygliński (Poland, UE)
 
 **Contact:** <info@pygpt.net>
 
 **License:** MIT License
```

### Comparing `pygpt-net-0.9.3/README.md` & `pygpt-net-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-Current release: **0.9.3** (build: **2023.04.14**)
-
-Official website: https://pygpt.net
+# PYGPT
 
-Documentation: https://pygpt.readthedocs.io
+Current release: **0.9.4** (build: **2023.04.15**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
 
 PyPi: https://pypi.org/project/pygpt-net
 
 ### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
 
-# PYGPT
-
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
 artificial intelligence models such as **GPT4** and **GPT3** using your
 own computer and `OpenAI API`. It allows you to talk in chat mode and in
 completion mode, as well as generate images using **DALL-E 2**.
 Moreover, the application has implemented context memory support,
@@ -39,14 +35,15 @@
 - allows you to easily manage prompts with handly editable presets
 - intuitive operation and interface
 - allows you to use all the powerful features of `GPT4` and `GPT3`
 - no knowledge of using AI models required
 - enables easy and convenient generation of images using `DALL-E 2`
 - has the ability to support future OpenAI models
 - fully configurable
+- plugins support
 - built-in tokens usage calculation
 - it\'s open source, source code is available on `GitHub`
 - **uses the user\'s API key**
 
 The application is free, open source and runs on PC with `Windows 10`,
 `Windows 11` and `Linux`. The full **Python** source code is available
 on `GitHub`.
@@ -86,14 +83,29 @@
 
 3. Once installed run the command to start the application:
 
 ``` commandline
 pygpt
 ```
 
+**Troubleshooting**: 
+
+If you have problems with xcb plugin with newer versions of PySide on Linux, e.g. like this:
+
+```commandline
+qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+```
+
+...then try downgrading PySide to `PySide6-Essentials==6.4.2`:
+
+```commandline
+pip install PySide6-Essentials==6.4.2
+```
+
 ### Running from GitHub source code
 
 1. Clone git repository or download .zip file:
 
 ```commandline
 git clone https://github.com/szczyglis-dev/py-gpt.git
 cd py-gpt
@@ -115,14 +127,17 @@
 4. Run the application:
 
 ```commandline
 cd src/pygpt_net
 python app.py
 ```
 
+**Tip**: you can use `PyInstaller` to create a compiled version of
+the application for your system.
+
 ## Other requirements
 
 To operate, you need an Internet connection (for API connection),
 registered OpenAI account and an active API key, which must be entered
 in the program.
 
 
@@ -296,14 +311,25 @@
 **Tip:** with presets, you can save prepared prompts and use them later
 when generating subsequent images.
 
 All queries are saved in the history, thanks to which you can return to
 a given session at any time and use old queries to, for example,
 generate new content.
 
+## Plugins
+
+The application allows you to use plugins to extend its functionality.
+Currently, the following plugins are available:
+
+- **SelfLoop** - allows to run GPT in a self-loop, which allows you to
+  generate a continuous conversation between AI <> AI. In this mode model talks to itself.
+
+- **RealTime** - auto-append current date and time to the prompt. It tells
+  the model what time it is in real time.
+
 
 # Tokens calculation
 
 ## Input tokens
 
 Calculation of tokens is implemented in the application. The application
 tries to predict the number of tokens that will be used for a given
@@ -450,15 +476,19 @@
 
 Support for plug-ins and voice recognition and synthesis will be added
 in future versions of the application.
 
 
 # CHANGELOG
 
-## v0.9.3 (2023.04.13)
+## v0.9.4 (2023.04.15)
+
+- added plugins support
+
+## v0.9.3 (2023.04.14)
 
 - packed into PyPI package
 
 ## v0.9.2 (2023.04.12)
 
 - added theme color settings
 - small UI fixes
@@ -468,21 +498,23 @@
 - added organization key configuration (by @kaneda2004, PR#1)
 - added config versions patching
 
 ## v0.9.0 (2023.04.09)
 
 - initial release
 
-# Credits
+# Credits and links
 
 **Official website:** <https://pygpt.net>
 
 **Documentation:** <https://pygpt.readthedocs.io>
 
 **GitHub:** <https://github.com/szczyglis-dev/py-gpt>
 
+**PyPI:** <https://pypi.org/project/pygpt-net>
+
 **Author:** Marcin Szczygliński (Poland, UE)
 
 **Contact:** <info@pygpt.net>
 
 **License:** MIT License
```

### Comparing `pygpt-net-0.9.3/pyproject.toml` & `pygpt-net-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygpt-net"
-version = "0.9.3"
+version = "0.9.4"
 description = "A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation"
 readme = "README.md"
 authors = [{ name = "Marcin Szczygliński", email = "info@pygpt.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pygpt-net-0.9.3/setup.py` & `pygpt-net-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.9.3'
+VERSION = '0.9.4'
 DESCRIPTION = 'A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation'
 LONG_DESCRIPTION = 'A package containing a GPT4, GPT3, ChatGPT and DALL-E 2 desktop chatbot, ' \
                    'text completion and image generation app, using OpenAI API and your own API Key. ' \
                    'It includes context memory and history, editable presets, customizable UI and more.'
 
 setup(
     name='pygpt-net',
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/__init__.py` & `pygpt-net-0.9.4/src/pygpt_net/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.12 09:00:00                  #
+# Updated Date: 2023.04.15 09:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2023, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "0.9.3"
-__build__ = "2023.04.14"
+__version__ = "0.9.4"
+__build__ = "2023.04.15"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __email__ = "info@pygpt.net"
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/app.py` & `pygpt-net-0.9.4/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/config.py` & `pygpt-net-0.9.4/src/pygpt_net/core/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.13 23:00:00                  #
+# Updated Date: 2023.04.15 02:00:00                  #
 # ================================================== #
 
 import datetime
 import os
 import re
 from pathlib import Path
 import shutil
@@ -79,17 +79,22 @@
     def get_version(self):
         """
         Returns version
 
         :return: version string
         """
         path = os.path.abspath(os.path.join(self.get_root_path(), '__init__.py'))
-        result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format("__version__"),
-                           open(path).read())
-        return result.group(1)
+        try:
+            f = open(path, "r", encoding="utf-8")
+            data = f.read()
+            f.close()
+            result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format("__version__"), data)
+            return result.group(1)
+        except Exception as e:
+            print(e)
 
     def load(self, all=True):
         """
         Loads config
 
         :param all: load all configs
         """
@@ -121,27 +126,29 @@
         path = os.path.join(self.path, 'models.json')
         if not os.path.exists(path):
             print("FATAL ERROR: {} not found!".format(path))
             return None
         try:
             f = open(path, "r", encoding="utf-8")
             self.models = json.load(f)
+            self.models = dict(sorted(self.models.items(), key=lambda item: item[0]))  # sort by key
             f.close()
         except Exception as e:
             print(e)
 
     def load_config(self):
         """Loads app config from JSON file"""
         path = os.path.join(self.path, 'config.json')
         if not os.path.exists(path):
             print("FATAL ERROR: {} not found!".format(path))
             return None
         try:
             f = open(path, "r", encoding="utf-8")
             self.data = json.load(f)
+            self.data = dict(sorted(self.data.items(), key=lambda item: item[0]))  # sort by key
             f.close()
         except Exception as e:
             print(e)
 
     def sort_presets_by_name(self):
         """Sorts presets by name"""
         self.presets = dict(sorted(self.presets.items(), key=lambda item: item[1]['name']))
@@ -374,15 +381,14 @@
     def get_preset_duplicate_name(self, name):
         """
         Prepares name for duplicated preset
 
         :param name: name of preset
         :return: name of duplicated preset
         """
-
         old_name = self.presets[name]['name']
         i = 1
         while True:
             new_name = name + '_' + str(i)
             if new_name not in self.presets:
                 return new_name, old_name + ' (' + str(i) + ')'
             i += 1
@@ -404,26 +410,14 @@
         """Saves config into file"""
         self.data['__meta__'] = self.append_meta()
         dump = json.dumps(self.data, indent=4)
         path = os.path.join(self.path, 'config.json')
         try:
             with open(path, 'w', encoding="utf-8") as f:
                 f.write(dump)
-                f.close()
-        except Exception as e:
-            print(e)
-
-    def save_config(self):
-        """Saves config into file"""
-        self.data['__meta__'] = self.append_meta()
-        dump = json.dumps(self.data, indent=4)
-        path = os.path.join(self.path, 'config.json')
-        try:
-            with open(path, 'w', encoding="utf-8") as f:
-                f.write(dump)
                 f.close()
         except Exception as e:
             print(e)
 
     def save_models(self):
         """Saves models config into file"""
         self.models['__meta__'] = self.append_meta()
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/context.py` & `pygpt-net-0.9.4/src/pygpt_net/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,31 +31,39 @@
         self.current_ctx = None
 
     def load_list(self):
         """Loads contexts list from file"""
         path = os.path.join(self.config.path, 'context.json')
         try:
             if os.path.exists(path):
-                with open(path, "r", encoding="utf-8") as file:
+                with open(path, 'r', encoding="utf-8") as file:
                     self.contexts = json.load(file)['items']
+                    file.close()
         except Exception as e:
             print(e)
             self.contexts = {}
 
     def load(self, name):
         """
         Loads context from file
 
         :param name: context name (id)
         :return: context items
         """
         path = os.path.join(self.config.path, 'context', name + '.json')
         if os.path.exists(path):
-            with open(path, "r", encoding="utf-8") as file:
-                return self.parse(json.load(file))
+            try:
+                with open(path, 'r', encoding="utf-8") as file:
+                    data = self.parse(json.load(file))
+                    file.close()
+                    return data
+            except Exception as e:
+                print("Error while loading context: {}".format(name))
+                print(e)
+                return []
         else:
             return []
 
     def parse(self, data):
         """
         Parses context data
 
@@ -124,14 +132,15 @@
             data['__meta__'] = self.config.append_meta()
             dump = json.dumps(data, indent=4)
             with open(index_path, 'w', encoding="utf-8") as f:
                 f.write(dump)
                 f.close()
 
         except Exception as e:
+            print("Error while dumping context: {}".format(name))
             print(e)
 
     def get_list(self):
         """
         Gets context items sorted descending by date
 
         :return: contexts dict
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/confirm.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/context.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/context.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/debug.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/image.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/image.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Created Date: 2023.04.09 20:00:00                  #
 # ================================================== #
 
 import os
 import shutil
+import webbrowser
 from showinfm import show_in_file_manager
 
 from PySide6 import QtGui, QtCore
-import webbrowser
-
 from PySide6.QtWidgets import QFileDialog
 
 from ..context import ContextItem
 from ..utils import trans
 
 
 class Image:
@@ -47,27 +46,29 @@
                 num_of_images = 4
 
         self.window.set_status(trans('status.sending'))
 
         # create ctx item
         ctx = ContextItem()
         ctx.set_input(text, self.window.config.data['user_name'])
+        ctx = self.window.controller.plugins.apply('ctx.before', ctx)  # apply plugins
         self.window.gpt.context.add(ctx)
         self.window.controller.output.append_input(ctx)
 
         # call DALL-E 2 API and generate images
         try:
             paths = self.window.images.generate(text, num_of_images)
             string = ""
             i = 1
             for path in paths:
                 string += "{} - {}".format(i, path) + "\n"
                 i += 1
             self.open_images(paths)
             ctx.set_output(string.strip())
+            ctx = self.window.controller.plugins.apply('ctx.after', ctx)  # apply plugins
             self.window.controller.output.append_output(ctx)
             self.window.gpt.context.store()
             self.window.set_status("OK.")
         except Exception as e:
             print(e)
             self.window.ui.dialogs.alert(str(e))
             self.window.set_status(trans('status.error'))
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/info.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/info.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/input.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/input.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         Input controller
 
         :param window: main window
         """
         self.window = window
 
     def setup(self):
-        """Setups input"""
+        """Sets up input"""
         if self.window.config.data['send_clear']:
             self.window.data['input.send_clear'].setChecked(True)
         else:
             self.window.data['input.send_clear'].setChecked(False)
 
         if self.window.config.data['send_shift_enter']:
             self.window.data['input.send_shift_enter'].setChecked(True)
@@ -60,36 +60,68 @@
         """
         Sends text to GPT
 
         :param text: text to send
         """
         self.window.set_status(trans('status.sending'))
 
+        # prepare names
+        user_name = self.window.controller.plugins.apply('user.name', self.window.config.data['user_name'])
+        ai_name = self.window.controller.plugins.apply('ai.name', self.window.config.data['ai_name'])
+
         # create ctx item
         ctx = ContextItem()
-        ctx.set_input(text, self.window.config.data['user_name'])
+        ctx.set_input(text, user_name)
+        ctx.set_output(None, ai_name)
+
+        # apply plugins
+        ctx = self.window.controller.plugins.apply('ctx.before', ctx)
+
+        # apply cfg
+        self.window.gpt.user_name = ctx.input_name
+        self.window.gpt.ai_name = ctx.output_name
+        self.window.gpt.system_prompt = self.window.controller.plugins.apply('system.prompt',
+                                                                             self.window.config.data['prompt'])
         self.window.controller.output.append_input(ctx)
 
         # call GPT
         try:
-            ctx = self.window.gpt.call(text, ctx)
+            try:
+                ctx = self.window.gpt.call(text, ctx)
+            except Exception as e:
+                print(e)
+                self.window.ui.dialogs.alert(str(e))
+                self.window.set_status(trans('status.error'))
+
+            ctx = self.window.controller.plugins.apply('ctx.after', ctx)  # apply plugins
             self.window.controller.output.append_output(ctx)
             self.window.gpt.context.store()
             self.window.set_status(
                 trans('status.tokens') + ": {} + {} = {}".format(ctx.input_tokens, ctx.output_tokens, ctx.total_tokens))
         except Exception as e:
             print(e)
             self.window.ui.dialogs.alert(str(e))
             self.window.set_status(trans('status.error'))
 
-    def send(self):
+        return ctx
+
+    def user_send(self, text=None):
+        """Sends real user input"""
+        text = self.window.controller.plugins.apply('user.send', text)
+        self.send(text)
+
+    def send(self, text=None):
         """
         Sends input text to API
         """
-        text = self.window.data['input'].toPlainText().strip()
+        ctx = None
+        if text is None:
+            text = self.window.data['input'].toPlainText().strip()
+        text = self.window.controller.plugins.apply('input.before', text)
+
         if len(text) > 0:
             if self.window.config.data['send_clear']:
                 self.window.data['input'].clear()
 
             # check API key
             if self.window.config.data['api_key'] is None or self.window.config.data['api_key'] == '':
                 self.window.controller.launcher.show_api_monit()
@@ -103,18 +135,19 @@
             # prepare context
             if len(self.window.gpt.context.contexts) == 0:
                 self.window.gpt.context.new()
                 self.window.controller.context.update()
 
             # send to API
             if self.window.config.data['mode'] == 'img':
-                self.window.controller.image.send_text(text)
+                ctx = self.window.controller.image.send_text(text)
             else:
-                self.window.controller.input.send_text(text)
+                ctx = self.window.controller.input.send_text(text)
 
+        ctx = self.window.controller.plugins.apply('ctx.end', ctx)  # apply plugins
         self.window.controller.ui.update()
 
     def append(self, text):
         """
         Appends text to input
 
         :param text: text to append
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/lang.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/lang.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,14 @@
 
         # menu
         self.window.menu['menu.app'].setTitle(trans("menu.file"))
         self.window.menu['app.exit'].setText(trans("menu.file.exit"))
         self.window.menu['app.clear_history'].setText(trans("menu.file_clear_history"))
 
         self.window.menu['menu.plugins'].setTitle(trans("menu.plugins"))
-        self.window.menu['plugins.empty'].setText(trans("coming_soon"))
 
         self.window.menu['menu.audio'].setTitle(trans("menu.audio"))
         self.window.menu['audio.empty'].setText(trans("coming_soon"))
 
         self.window.menu['menu.config'].setTitle(trans("menu.config"))
         self.window.menu['config.settings'].setText(trans("menu.config.settings"))
         self.window.menu['config.edit.config'].setText(trans("menu.config.edit.config"))
@@ -191,13 +190,16 @@
         self.window.menu['info.github'].setText(trans("menu.info.github"))
 
         # start
         self.window.data['start.title'].setText(trans('dialog.start.title.text'))
         self.window.data['start.settings'].setText(trans('dialog.start.settings.text'))
         self.window.data['start.btn'].setText(trans('dialog.start.btn'))
 
+        # plugins info
+        self.window.controller.plugins.update_info()
+
         for theme in self.window.menu['theme']:
             name = self.window.controller.theme.trans_theme(theme)
             self.window.menu['theme'][theme].setText(name)
 
         self.window.controller.model.update()
         self.window.set_status('')
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/launcher.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/main.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         self.launcher = Launcher(window)
         self.lang = Lang(window)
         self.image = Image(window)
         self.theme = Theme(window)
 
     def setup(self):
         """Setups controller"""
+        # setup plugins settings
+        self.plugins.setup_settings()
+
         # init material theme
         self.theme.setup()
 
         # setup all controllers
         self.lang.setup()
         self.model.setup()
         self.input.setup()
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/model.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/model.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/output.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,31 +50,41 @@
 
     def append_input(self, item):
         """
         Appends input to output
 
         :param item: context item
         """
+        if item.input is None or item.input == "":
+            return
         if self.window.config.data['output_timestamp'] and item.input_timestamp is not None:
+            name = ""
+            if item.input_name is not None and item.input_name != "":
+                name = item.input_name + " "
             ts = datetime.fromtimestamp(item.input_timestamp)
             hour = ts.strftime("%H:%M:%S")
-            self.append("{}: > {}".format(hour, item.input))
+            self.append("{}{}: > {}".format(name, hour, item.input))
         else:
             self.append("> {}".format(item.input))
 
     def append_output(self, item):
         """
         Appends output to output
 
         :param item: context item
         """
+        if item.output is None or item.output == "":
+            return
         if self.window.config.data['output_timestamp'] and item.output_timestamp is not None:
+            name = ""
+            if item.output_name is not None and item.output_name != "":
+                name = item.output_name + " "
             ts = datetime.fromtimestamp(item.output_timestamp)
             hour = ts.strftime("%H:%M:%S")
-            self.append("{}: {}".format(hour, item.output) + "\n")
+            self.append("{}{}: {}".format(name, hour, item.output) + "\n")
         else:
             self.append(item.output + "\n")
 
     def append(self, text):
         """
         Appends text to output
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/plugins.py` & `pygpt-net-0.9.4/src/pygpt_net/core/info.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Created Date: 2023.04.09 20:00:00                  #
 # ================================================== #
 
-class Plugins:
+class Info:
     def __init__(self, window=None):
         """
-        Plugins controller
+        Info handler
 
-        :param window: main window
+        :param window main window
         """
         self.window = window
+
+        # prepare info ids
+        self.ids = ['about', 'changelog']
+        self.active = {}
+
+        # prepare active
+        for id in self.ids:
+            self.active[id] = False
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/settings.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.11 05:00:00                  #
+# Updated Date: 2023.04.15 02:00:00                  #
 # ================================================== #
 
 import os
 
 from showinfm import show_in_file_manager
 from ..utils import trans
 
@@ -32,24 +32,24 @@
         """
         if id == "settings":
             self.window.config.data['api_key'] = self.window.config_option['api_key'].text()
             self.window.config.data['organization_key'] = self.window.config_option['organization_key'].text()
             self.window.config.data['img_resolution'] = self.window.config_option['img_resolution'].text()
 
         info = trans('info.settings.saved')
-        self.window.config.save_config()
+        self.window.config.save()
         self.window.set_status(info)
         self.close_window(id)
         self.update_font_size()
         self.window.controller.ui.update()
 
     def save_all(self):
         """Saves all settings"""
         info = trans('info.settings.all.saved')
-        self.window.config.save_config()
+        self.window.config.save()
         self.window.config.save_presets()
         self.window.ui.dialogs.alert(info)
         self.window.set_status(info)
         self.window.controller.ui.update()
 
     def start_settings(self):
         """Opens settings at first launch (no API key)"""
@@ -145,15 +145,15 @@
                 if id in self.window.settings.active and self.window.settings.active[id]:
                     self.window.menu['config.' + id].setChecked(True)
                 else:
                     self.window.menu['config.' + id].setChecked(False)
 
     def init(self, id):
         """
-        Inits settings
+        Initializes settings
 
         :param id: settings window id
         """
         if id == 'settings':
             # slider + input
             self.apply('temperature', self.window.config.data['temperature'])
             self.apply('top_p', self.window.config.data['top_p'])
@@ -178,25 +178,25 @@
         """
         Toggles checkbox
 
         :param id: checkbox option id
         :param value: checkbox option value
         :param section: settings section
         """
+        # dialog: preset
         if id.startswith('preset.'):
-            preset = self.window.config.data['preset']  # current preset
-            is_current = True
-            if section == 'preset.editor':
-                preset = self.window.config_option['preset.filename'].text()  # editing preset
-                is_current = False
-            self.window.controller.presets.update_field(id, value, preset, is_current)
-            txt = '{}'.format(value)
-            self.window.config_option[id].box.setChecked(value)
+            self.window.controller.presets.config_toggle(id, value, section)
+            return
+
+        # dialog: plugin
+        elif id.startswith('plugin.'):
+            self.window.controller.plugins.config_toggle(id, value)
             return
 
+        # dialog: settings
         if id == 'store_history':
             self.window.config.data['store_history'] = value
         elif id == 'store_history_time':
             self.window.config.data['store_history_time'] = value
         elif id == 'use_context':
             self.window.config.data['use_context'] = value
 
@@ -206,32 +206,25 @@
         """
         Changes input value
 
         :param id: input option id
         :param value: input option value
         :param section: settings section
         """
-        # validate filename
-        if id == 'preset.filename':
-            value = self.window.controller.presets.validate_filename(value)
-            self.window.config_option[id].setText(value)
-
-        # current prompt update
+        # dialog: preset
         if id.startswith('preset.'):
-            preset = self.window.config.data['preset']  # current preset
-            is_current = True
-            if section == 'preset.editor':
-                preset = self.window.config_option['preset.filename'].text()  # editing preset
-                is_current = False
-            self.window.controller.presets.update_field(id, value, preset, is_current)
-            txt = '{}'.format(value)
-            self.window.config_option[id].setText(txt)
+            self.window.controller.presets.config_change(id, value, section)
+            return
+
+        # dialog: plugin
+        elif id.startswith('plugin.'):
+            self.window.controller.plugins.config_change(id, value)
             return
 
-        # settings update
+        # dialog: settings
         if id == 'temperature' \
                 or id == 'top_p' \
                 or id == 'frequency_penalty' \
                 or id == 'presence_penalty':
             if value < 0:
                 value = 0.0
             elif value > 2:
@@ -254,32 +247,38 @@
         Applies slider + input value
 
         :param id: option id
         :param value: option value
         :param type: option type (slider, input, None)
         :param section: option section (settings, preset.editor, None)
         """
+        # dialog: preset
+        if id.startswith('preset.'):
+            self.window.controller.presets.config_slider(id, value, type, section)
+            return
+
+        # dialog: plugin
+        elif id.startswith('plugin.'):
+            self.window.controller.plugins.config_slider(id, value, type)
+            return
+
+        # dialog: settings
         integer_values = ['max_output_tokens', 'max_total_tokens', 'context_threshold', 'img_variants', 'font_size']
+        params_values = ['temperature', 'current_temperature', 'top_p', 'frequency_penalty', 'presence_penalty']
 
         if id in integer_values:
             try:
                 value = int(value)
             except:
                 value = 0
                 self.window.config_option[id].input.setText(str(value))
 
         multiplier = 1
-        if id == 'temperature' \
-                or id == 'current_temperature' \
-                or id == 'preset.temperature' \
-                or id == 'top_p' \
-                or id == 'frequency_penalty' \
-                or id == 'presence_penalty':
+        if id in params_values:
             multiplier = 100
-
             # fix / validate
             if type != 'slider':
                 try:
                     value = float(value)
                 except:
                     value = 0.0
                     self.window.config_option[id].input.setText(str(value))
@@ -300,15 +299,15 @@
                 if value < 1:
                     value = 1
                 elif value > 4:
                     value = 4
                 self.window.config_option[id].input.setText(str(value))
 
         # font size
-        if id == 'font_size':
+        elif id == 'font_size':
             # fix / validate
             if type != 'slider':
                 try:
                     value = int(value)
                 except:
                     value = 8
                 if value < 8:
@@ -320,56 +319,51 @@
         slider_value = round(float(value) * multiplier, 0)
         input_value = value
         if type == 'slider':
             input_value = value / multiplier
             if id in integer_values:
                 input_value = round(int(input_value), 0)
 
-        if id.startswith('preset.') or id == 'current_temperature':
+        # update current preset temperature if changed global temperature
+        if id == 'current_temperature':
             preset = self.window.config.data['preset']  # current preset
             is_current = True
             if section == 'preset.editor':
                 preset = self.window.config_option['preset.filename'].text()  # editing preset
                 is_current = False
             self.window.controller.presets.update_field(id, input_value, preset, is_current)
+            self.window.controller.presets.update_field('preset.temperature', input_value, True)
         else:
             if id not in integer_values:
                 self.window.config.data[id] = float(input_value)
             else:
                 self.window.config.data[id] = round(int(input_value), 0)
 
-        # update current prompt temperature
-        if id == 'current_temperature':
-            self.window.controller.presets.update_field('preset.temperature', input_value, True)
-
         # update from slider
         if type == 'slider':
             txt = '{}'.format(input_value)
             self.window.config_option[id].input.setText(txt)
-        # or update from input
+
+        # update from input
         elif type == 'input':
-            if id == 'temperature' \
-                    or id == 'current_temperature' \
-                    or id == 'preset.temperature' \
-                    or id == 'top_p' \
-                    or id == 'frequency_penalty' \
-                    or id == 'presence_penalty':
+            if id in params_values:
                 if slider_value < 1:
                     slider_value = 1
                 elif slider_value > 200:
                     slider_value = 200
             elif id == 'max_output_tokens' \
                     or id == 'max_total_tokens':
                 if slider_value < 1:
                     slider_value = 1
                 elif slider_value > 32000:
                     slider_value = 32000
             self.window.config_option[id].slider.setValue(slider_value)
+
+        # update from raw value
         else:
-            # or update from raw value
             txt = '{}'.format(value)
             self.window.config_option[id].input.setText(txt)
             self.window.config_option[id].slider.setValue(slider_value)
 
     def open_config_dir(self):
         """Opens user config directory"""
         if os.path.exists(self.window.config.path):
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/theme.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/theme.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.12 08:00:00                  #
+# Updated Date: 2023.04.15 00:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction
 
 from ..utils import trans
 
 
@@ -35,38 +35,73 @@
         self.window.set_theme(name + '.xml')
         self.update()
 
     def apply(self):
         """Applies theme fixes"""
         self.window.setStyleSheet(self.get_style('line_edit'))
         self.window.menu['menu.lang'].setStyleSheet(self.get_style('menu'))
-        self.window.menu['menu.theme'].setStyleSheet(self.get_style('theme'))
+        self.window.menu['menu.theme'].setStyleSheet(self.get_style('menu'))
+        self.window.menu['menu.plugins'].setStyleSheet(self.get_style('menu'))
         self.window.data['output'].setStyleSheet(self.get_style('chat_output'))
         self.window.data['output.timestamp'].setStyleSheet(self.get_style('checkbox'))
         self.window.data['input.send_enter'].setStyleSheet(self.get_style('radio'))
         self.window.data['input.send_shift_enter'].setStyleSheet(self.get_style('radio'))
         self.window.data['input.send_clear'].setStyleSheet(self.get_style('checkbox'))
 
         # dialog: ctx rename
         self.window.dialog['ctx.rename'].input.setStyleSheet(self.get_style('line_edit'))
 
         # ai, user names
         self.window.data['preset.ai_name'].setStyleSheet(self.get_style('line_edit'))
         self.window.data['preset.user_name'].setStyleSheet(self.get_style('line_edit'))
 
+        # current temperature / img variants
+        self.window.config_option['current_temperature'].input.setStyleSheet(self.get_style('line_edit'))
+        self.window.config_option['img_variants'].input.setStyleSheet(self.get_style('line_edit'))
+
         # dialog: settings
         self.window.config_option['use_context'].box.setStyleSheet(self.get_style('checkbox'))
         self.window.config_option['store_history'].box.setStyleSheet(self.get_style('checkbox'))
         self.window.config_option['store_history_time'].box.setStyleSheet(self.get_style('checkbox'))
 
         # dialog: preset editor
         self.window.config_option['preset.chat'].box.setStyleSheet(self.get_style('checkbox'))
         self.window.config_option['preset.completion'].box.setStyleSheet(self.get_style('checkbox'))
         self.window.config_option['preset.img'].box.setStyleSheet(self.get_style('checkbox'))
 
+        # dialog: plugin settings
+        self.apply_plugins_settings()
+
+    def apply_plugins_settings(self):
+        """Applies theme to plugin settings"""
+        for id in self.window.controller.plugins.handler.plugins:
+            if id not in self.window.plugin_option:
+                continue
+            plugin = self.window.controller.plugins.handler.plugins[id]
+            if plugin.options is not None:
+                for key in plugin.options:
+                    option = plugin.options[key]
+                    if 'type' in option:
+                        # checkbox
+                        if option['type'] == 'bool':
+                            if key in self.window.plugin_option[id]:
+                                self.window.plugin_option[id][key].box.setStyleSheet(self.get_style('checkbox'))
+                        # text input
+                        elif option['type'] == 'text':
+                            if key in self.window.plugin_option[id]:
+                                self.window.plugin_option[id][key].input.setStyleSheet(self.get_style('line_edit'))
+
+                        # input with slider
+                        elif option['type'] == 'int' or option['type'] == 'float':
+                            if key in self.window.plugin_option[id]:
+                                if 'slider' in option and option['slider']:
+                                    self.window.plugin_option[id][key].input.setStyleSheet(self.get_style('line_edit'))
+                                else:
+                                    self.window.plugin_option[id][key].setStyleSheet(self.get_style('line_edit'))
+
     def get_style(self, element):
         """
         Returns style for element
 
         :param element: element name
         :return: style
         """
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/controller/ui.py` & `pygpt-net-0.9.4/src/pygpt_net/core/controller/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/debug/config.py` & `pygpt-net-0.9.4/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/debug/context.py` & `pygpt-net-0.9.4/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/debug/models.py` & `pygpt-net-0.9.4/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/debug/presets.py` & `pygpt-net-0.9.4/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/debugger.py` & `pygpt-net-0.9.4/src/pygpt_net/core/debugger.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Created Date: 2023.04.09 20:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QStandardItemModel
+
 from .debug.config import ConfigDebug
 from .debug.context import ContextDebug
 from .debug.presets import PresetsDebug
 from .debug.models import ModelsDebug
+from .debug.plugins import PluginsDebug
 
 
 class Debug:
     DBG_KEY, DBG_VALUE = range(2)
 
     def __init__(self, window=None):
         """
@@ -30,14 +32,15 @@
 
         # setup workers
         self.workers = {}
         self.workers['config'] = ConfigDebug(self.window)
         self.workers['context'] = ContextDebug(self.window)
         self.workers['presets'] = PresetsDebug(self.window)
         self.workers['models'] = ModelsDebug(self.window)
+        self.workers['plugins'] = PluginsDebug(self.window)
 
         # prepare debug ids
         self.ids = self.workers.keys()
         self.models = {}
         self.initialized = {}
         self.active = {}
         self.idx = {}
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/gpt.py` & `pygpt-net-0.9.4/src/pygpt_net/core/gpt.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 
         :param config: Config object
         """
         self.config = config
         self.context = Context(config)
         self.history = History(config)
 
+        self.ai_name = None
+        self.user_name = None
+        self.system_prompt = None
+
         if not self.config.initialized:
             self.config.init()
 
     def init(self):
         """Initializes OpenAI API key"""
         openai.api_key = self.config.data["api_key"]
         openai.organization = self.config.data["organization_key"]
@@ -44,16 +48,16 @@
         :return: Response dict
         """
         # build prompt message
         message = self.build_completion(prompt)
 
         # prepare stop word if user_name is set
         stop = None
-        if self.config.data['user_name'] is not None and self.config.data['user_name'] != '':
-            stop = [self.config.data['user_name'] + ':']
+        if self.user_name is not None and self.user_name != '':
+            stop = [self.user_name + ':']
 
         response = openai.Completion.create(
             prompt=message,
             model=self.config.data['model'],
             max_tokens=int(max_tokens),
             temperature=self.config.data['temperature'],
             top_p=self.config.data['top_p'],
@@ -95,41 +99,31 @@
         messages = []
 
         model = self.config.data['model']
         used_tokens = self.count_used_tokens(prompt)
         max_tokens = self.config.data['max_total_tokens']
 
         # append initial (system) message
-        if self.config.data['prompt'] is not None and self.config.data['prompt'] != "":
-            messages.append({"role": "system", "content": self.config.data['prompt']})
+        if self.system_prompt is not None and self.system_prompt != "":
+            messages.append({"role": "system", "content": self.system_prompt})
 
         # append messages from context (memory)
         if self.config.data['use_context']:
             items = self.context.get_prompt_items(model, used_tokens, max_tokens)
             for item in items:
                 # input
-                if item.input_name is not None and item.input_name != "":
-                    messages.append({"role": "user", "content": item.input})
-                    # TODO: messages.append({"role": "user", "name": item.input_name, "content": item.input})
-                else:
+                if item.input is not None and item.input != "":
                     messages.append({"role": "user", "content": item.input})
 
                 # output
-                if item.output_name is not None and item.output_name != "":
-                    messages.append({"role": "assistant", "content": item.output})
-                    # TODO: messages.append({"role": "assistant", "name": item.output_name, "content": item.output})
-                else:
+                if item.output is not None and item.output != "":
                     messages.append({"role": "assistant", "content": item.output})
 
         # append current prompt
-        if self.config.data['user_name'] is not None and self.config.data['user_name'] != "":
-            messages.append({"role": "user", "content": str(prompt)})
-            # TODO: messages.append({"role": "user", "name": self.config.data['user_name'], "content": str(prompt)})
-        else:
-            messages.append({"role": "user", "content": str(prompt)})
+        messages.append({"role": "user", "content": str(prompt)})
 
         return messages
 
     def build_completion(self, prompt):
         """
         Builds completion string
 
@@ -137,53 +131,57 @@
         :return: Message string (parsed with context)
         """
         message = ""
         model = self.config.data['model']
         used_tokens = self.count_used_tokens(prompt)
         max_tokens = self.config.data['max_total_tokens']
 
-        if self.config.data['prompt'] is not None and self.config.data['prompt'] != "":
-            message += self.config.data['prompt']
+        if self.system_prompt is not None and self.system_prompt != "":
+            message += self.system_prompt
 
         if self.config.data['use_context']:
             items = self.context.get_prompt_items(model, used_tokens, max_tokens)
             for item in items:
                 if item.input_name is not None \
                         and item.output_name is not None \
                         and item.input_name != "" \
                         and item.output_name != "":
-                    message += "\n" + item.input_name + ": " + item.input
-                    message += "\n" + item.output_name + ": " + item.output
+                    if item.input is not None and item.input != "":
+                        message += "\n" + item.input_name + ": " + item.input
+                    if item.output is not None and item.output != "":
+                        message += "\n" + item.output_name + ": " + item.output
                 else:
-                    message += "\n" + item.input
-                    message += "\n" + item.output
-
-        if self.config.data['user_name'] is not None \
-                and self.config.data['ai_name'] is not None \
-                and self.config.data['user_name'] != "" \
-                and self.config.data['ai_name'] != "":
-            message += "\n" + self.config.data['user_name'] + ": " + str(prompt)
-            message += "\n" + self.config.data['ai_name'] + ":"
+                    if item.input is not None and item.input != "":
+                        message += "\n" + item.input
+                    if item.output is not None and item.output != "":
+                        message += "\n" + item.output
+
+        if self.user_name is not None \
+                and self.ai_name is not None \
+                and self.user_name != "" \
+                and self.ai_name != "":
+            message += "\n" + self.user_name + ": " + str(prompt)
+            message += "\n" + self.ai_name + ":"
         else:
             message += "\n" + str(prompt)
 
         return message
 
     def count_used_tokens(self, input_text):
         """
         Counts used tokens
 
         :param input_text: Input text
         :return: Used tokens
         """
         model = self.config.data['model']
         tokens = 0
-        tokens += num_tokens_prompt(self.config.data['prompt'], self.config.data['user_name'],
+        tokens += num_tokens_prompt(self.system_prompt, self.user_name,
                                     model)  # init (system) prompt
-        tokens += num_tokens_prompt(input_text, self.config.data['user_name'], model)  # current input
+        tokens += num_tokens_prompt(input_text, self.user_name, model)  # current input
         tokens += self.config.data['context_threshold']  # context threshold (reserved for next output)
         tokens += num_tokens_extra(model)  # extra tokens (required for output)
         return tokens
 
     def call(self, prompt, ctx=None):
         """
         Calls OpenAI API
@@ -227,17 +225,17 @@
             output = response["choices"][0]["text"].strip()
         elif self.config.data['mode'] == "chat":
             output = response["choices"][0]["message"]["content"].strip()
 
         # store context (memory)
         if ctx is None:
             ctx = ContextItem(self.config.data['mode'])
-            ctx.set_input(prompt, self.config.data['user_name'])
+            ctx.set_input(prompt, self.user_name)
 
-        ctx.set_output(output, self.config.data['ai_name'])
+        ctx.set_output(output, self.ai_name)
         ctx.set_tokens(response["usage"]["prompt_tokens"], response["usage"]["completion_tokens"])
         self.context.add(ctx)
 
         # store history
         if self.config.data['store_history']:
             self.history.save(output)
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/history.py` & `pygpt-net-0.9.4/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/image.py` & `pygpt-net-0.9.4/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/locale.py` & `pygpt-net-0.9.4/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/settings.py` & `pygpt-net-0.9.4/src/pygpt_net/core/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.window.set_status("Loaded defaults from file: {}".format(file))
 
     def save_editor(self):
         """Saves file to disk"""
         file = self.window.dialog['config.editor'].file
         path = os.path.join(self.window.config.path, file)
         try:
-            with open(path, 'w') as f:
+            with open(path, 'w', encoding="utf-8") as f:
                 f.write(self.window.editor['config'].toPlainText())
                 f.close()
             self.window.set_status("Saved file: {}".format(path))
             self.window.ui.dialogs.alert("Saved file: {}".format(path))
         except Exception as e:
             self.window.set_status("Error saving file: {}".format(path))
             print(e)
@@ -62,13 +62,13 @@
         :param id: file id
         """
         # load file
         path = os.path.join(self.window.config.path, file)
         self.window.path_label['config'].setText(path)
         self.window.dialog['config.editor'].file = file
         try:
-            with open(path, 'r') as f:
+            with open(path, 'r', encoding="utf-8") as f:
                 txt = f.read()
                 f.close()
                 self.window.editor['config'].setPlainText(txt)
         except Exception as e:
             print(e)
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/tokens.py` & `pygpt-net-0.9.4/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/chatbox.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/chatbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,20 @@
         self.window.data['chat.model'] = QLabel("")
         self.window.data['chat.model'].setAlignment(Qt.AlignRight)
         context_layout = self.setup_context()
 
         self.window.data['chat.label'] = QLabel(trans("chatbox.label"))
         self.window.data['chat.label'].setStyleSheet(self.window.controller.theme.get_style('text_bold'))
 
+        self.window.data['chat.plugins'] = QLabel("+ 2 plugins")
+        self.window.data['chat.plugins'].setAlignment(Qt.AlignCenter)
+
         header = QHBoxLayout()
         header.addWidget(self.window.data['chat.label'])
+        header.addWidget(self.window.data['chat.plugins'])
         header.addWidget(self.window.data['chat.model'])
 
         layout = QVBoxLayout()
         layout.addLayout(header)
         layout.addWidget(self.window.data['output'])
         layout.addLayout(context_layout)
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/contexts.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/contexts.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/about.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/changelog.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/ctx_rename.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/ctx_rename.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/debug.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/debug.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Created Date: 2023.04.09 20:00:00                  #
 # ================================================== #
 
-from PySide6.QtWidgets import QTreeView, QGridLayout
+from PySide6.QtWidgets import QTreeView, QGridLayout, QAbstractItemView, QScrollArea
 
 from ..widgets import DebugDialog
 
 
 class Debug:
     def __init__(self, window=None):
         """
@@ -27,14 +27,20 @@
         """
         Setups debug dialog
 
         :param id: debug id
         """
         self.window.debug[id] = QTreeView()
         self.window.debug[id].setRootIsDecorated(False)
+        self.window.debug[id].setEditTriggers(QAbstractItemView.NoEditTriggers)
+        self.window.debug[id].setWordWrap(True)
+
+        scroll = QScrollArea()
+        scroll.setWidget(self.window.debug[id])
+        scroll.setWidgetResizable(True)
 
         layout = QGridLayout()
-        layout.addWidget(self.window.debug[id], 1, 0)
+        layout.addWidget(scroll, 1, 0)
 
         self.window.dialog['debug.' + id] = DebugDialog(self.window, id)
         self.window.dialog['debug.' + id].setLayout(layout)
         self.window.dialog['debug.' + id].setWindowTitle("Debug" + ": " + id)
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/editor.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/image.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/preset.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/settings.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/start.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/update.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialogs.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialogs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Created Date: 2023.04.09 20:00:00                  #
+# Updated Date: 2023.04.14 20:00:00                  #
 # ================================================== #
 
 from .dialog.settings import Settings
 from .dialog.preset import Preset
 from .dialog.debug import Debug
 from .dialog.about import About
 from .dialog.changelog import Changelog
 from .dialog.editor import Editor
 from .dialog.ctx_rename import CtxRename
 from .dialog.start import Start
 from .dialog.update import Update
 from .dialog.image import Image
+from .dialog.plugins import Plugins
 from .widgets import AlertDialog, ConfirmDialog
 
 
 class Dialogs:
     def __init__(self, window=None):
         """
         Dialogs setup
@@ -72,15 +73,15 @@
         update = Update(self.window)
         update.setup()
 
         # setup image dialog
         image = Image(self.window)
         image.setup()
 
-        # alert / confirm
+        self.window.plugin_settings = Plugins(self.window)
         self.window.dialog['alert'] = AlertDialog(self.window)
         self.window.dialog['confirm'] = ConfirmDialog(self.window)
 
     def confirm(self, type, id, msg):
         """
         Shows confirm dialog
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/input.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             self.window.controller.theme.get_style('checkbox'))  # Windows fix
         self.window.data['input.send_clear'].stateChanged.connect(
             lambda: self.window.controller.input.toggle_send_clear(self.window.data['input.send_clear'].isChecked()))
 
         # send button
         self.window.data['input.send_btn'] = QPushButton(trans("input.btn.send"))
         self.window.data['input.send_btn'].clicked.connect(
-            lambda: self.window.controller.input.send())
+            lambda: self.window.controller.input.user_send())
 
         # send layout
         send_layout = QHBoxLayout()
         send_layout.addWidget(self.window.data['input.send_clear'])
         send_layout.addWidget(self.window.data['input.send_enter'])
         send_layout.addWidget(self.window.data['input.send_shift_enter'])
         send_layout.addWidget(self.window.data['input.send_btn'])
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/main.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Created Date: 2023.04.09 20:00:00                  #
+# Updated Date: 2023.04.14 20:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QSplitter, QWidget
 
 from .chatbox import ChatBox
 from .toolbox import Toolbox
@@ -24,18 +24,20 @@
         """
         UI (main)
 
         :param window: main UI window object
         """
         self.window = window
         self.window.data = {}
+        self.window.plugin_data = {}
         self.window.menus = {}
         self.window.models = {}
         self.window.path_label = {}
         self.window.config_option = {}
+        self.window.plugin_option = {}
 
         self.chat = ChatBox(window)
         self.toolbox = Toolbox(window)
         self.contexts = Contexts(window)
         self.menu = Menu(window)
         self.dialogs = Dialogs(window)
 
@@ -47,27 +49,23 @@
 
         # ctx
         self.window.ctx = QWidget()
         self.window.ctx.setLayout(self.contexts.setup())
 
         # set width
         self.window.ctx.setMinimumWidth(200)
-        # self.window.ctx.setMaximumWidth(self.window.config.data['ui.ctx.max_width'])
-        # self.window.toolbox.setMinimumWidth(self.window.config.data['ui.toolbox.min_width'])
-        # self.window.toolbox.setMaximumWidth(self.window.config.data['ui.toolbox.max_width'])
 
         # horizontal splitter
         splitter = QSplitter(Qt.Horizontal)
         splitter.addWidget(self.window.ctx)  # contexts
         splitter.addWidget(self.window.toolbox)  # toolbox
         splitter.addWidget(self.window.chat)  # chat box
         splitter.setStretchFactor(0, 3)
         splitter.setStretchFactor(1, 3)
         splitter.setStretchFactor(2, 9)
-        # splitter.setSizes([1, 1, 7])
 
         # menu
         self.menu.setup()
 
         # dialogs
         self.dialogs.setup()
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/menu.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,24 @@
 
         self.window.menu['menu.app'] = self.window.menuBar().addMenu(trans("menu.file"))
         self.window.menu['menu.app'].addAction(self.window.menu['app.clear_history'])
         self.window.menu['menu.app'].addAction(self.window.menu['app.exit'])
 
     def setup_plugins(self):
         """Setups plugins menu"""
-        self.window.menu['plugins.empty'] = QAction(QIcon.fromTheme("help-about"), trans("coming_soon"),
-                                                    self.window)
+        self.window.menu['plugins.settings'] = QAction(trans("menu.plugins.settings"),
+                                                       self.window)
+
+        self.window.menu['plugins.settings'].triggered.connect(
+            lambda: self.window.controller.plugins.toggle_settings())
+
+        self.window.menu['plugins'] = {}
         self.window.menu['menu.plugins'] = self.window.menuBar().addMenu(trans("menu.plugins"))
-        self.window.menu['menu.plugins'].addAction(self.window.menu['plugins.empty'])
+        self.window.menu['menu.plugins'].setStyleSheet(self.window.controller.theme.get_style('menu'))  # Windows fix
+        self.window.menu['menu.plugins'].addAction(self.window.menu['plugins.settings'])
 
     def setup_audio(self):
         """Setups audio menu"""
         self.window.menu['audio.empty'] = QAction(QIcon.fromTheme("help-about"), trans("coming_soon"),
                                                   self.window)
         self.window.menu['menu.audio'] = self.window.menuBar().addMenu(trans("menu.audio"))
         self.window.menu['menu.audio'].addAction(self.window.menu['audio.empty'])
@@ -103,29 +109,33 @@
 
     def setup_debug(self):
         """Setups debug menu"""
         self.window.menu['debug.config'] = QAction(trans("menu.debug.config"), self.window, checkable=True)
         self.window.menu['debug.context'] = QAction(trans("menu.debug.context"), self.window, checkable=True)
         self.window.menu['debug.presets'] = QAction(trans("menu.debug.presets"), self.window, checkable=True)
         self.window.menu['debug.models'] = QAction(trans("menu.debug.models"), self.window, checkable=True)
+        self.window.menu['debug.plugins'] = QAction(trans("menu.debug.plugins"), self.window, checkable=True)
 
         self.window.menu['debug.config'].triggered.connect(
             lambda: self.window.controller.debug.toggle('config'))
         self.window.menu['debug.context'].triggered.connect(
             lambda: self.window.controller.debug.toggle('context'))
         self.window.menu['debug.presets'].triggered.connect(
             lambda: self.window.controller.debug.toggle('presets'))
         self.window.menu['debug.models'].triggered.connect(
             lambda: self.window.controller.debug.toggle('models'))
+        self.window.menu['debug.plugins'].triggered.connect(
+            lambda: self.window.controller.debug.toggle('plugins'))
 
         self.window.menu['menu.debug'] = self.window.menuBar().addMenu(trans("menu.debug"))
         self.window.menu['menu.debug'].addAction(self.window.menu['debug.config'])
         self.window.menu['menu.debug'].addAction(self.window.menu['debug.context'])
         self.window.menu['menu.debug'].addAction(self.window.menu['debug.presets'])
         self.window.menu['menu.debug'].addAction(self.window.menu['debug.models'])
+        self.window.menu['menu.debug'].addAction(self.window.menu['debug.plugins'])
 
     def setup_lang(self):
         """Setups lang menu"""
         self.window.menu['lang'] = {}
         self.window.menu['menu.lang'] = self.window.menuBar().addMenu(trans("menu.lang"))
         self.window.menu['menu.lang'].setStyleSheet(self.window.controller.theme.get_style('menu'))  # Windows fix
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/status.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/status.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/toolbox.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/toolbox.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/ui/widgets.py` & `pygpt-net-0.9.4/src/pygpt_net/core/ui/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.13 23:00:00                  #
+# Updated Date: 2023.04.15 02:00:00                  #
 # ================================================== #
 import os
 
 from PySide6 import QtCore
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QAction, QIcon, QPixmap
 from PySide6.QtWidgets import QLineEdit, QTreeView, QAbstractItemView, QMenu, QDialog, QLabel, QCheckBox, QHBoxLayout, \
@@ -62,17 +62,17 @@
         """
         super(ChatInput, self).keyPressEvent(event)
         self.window.controller.ui.update()
         if event.key() == QtCore.Qt.Key_Return or event.key() == QtCore.Qt.Key_Enter:
             if self.window.config.data['send_shift_enter']:
                 modifiers = QApplication.keyboardModifiers()
                 if modifiers == QtCore.Qt.ShiftModifier:
-                    self.window.controller.input.send()
+                    self.window.controller.input.user_send()
             else:
-                self.window.controller.input.send()
+                self.window.controller.input.user_send()
             self.setFocus()
 
 
 class ChatOutput(QTextEdit):
     def __init__(self, window=None):
         """
         Chat input
@@ -454,15 +454,14 @@
             lambda: self.window.controller.settings.toggle(self.id, self.box.isChecked(), self.section))
 
         # windows style fix (without this checkboxes are invisible!)
         self.box.setStyleSheet(self.window.controller.theme.get_style('checkbox'))
 
         self.layout = QHBoxLayout()
         self.layout.addWidget(self.box)
-        # self.layout.addWidget(self.label)
 
         self.setLayout(self.layout)
 
 
 class SettingsInputInline(QLineEdit):
     def __init__(self, window=None, id=None, section=None):
         """
@@ -567,14 +566,36 @@
         :param event: close event
         """
         self.window.settings.active[self.id] = False
         self.window.controller.settings.close(self.id)
         self.window.controller.settings.update()
 
 
+class PluginSettingsDialog(QDialog):
+    def __init__(self, window=None, id=None):
+        """
+        Plugin settings dialog
+
+        :param window: main window
+        :param id: settings id
+        """
+        super(PluginSettingsDialog, self).__init__(window)
+        self.window = window
+        self.id = id
+
+    def closeEvent(self, event):
+        """
+        Close event
+
+        :param event: close event
+        """
+        self.window.controller.plugins.config_dialog = False
+        self.window.controller.plugins.update()
+
+
 class EditorDialog(QDialog):
     def __init__(self, window=None, id=None, data_id=None):
         """
         EditorDialog
 
         :param window: main window
         :param id: configurator id
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/updater.py` & `pygpt-net-0.9.4/src/pygpt_net/core/updater.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.13 23:00:00                  #
+# Updated Date: 2023.04.15 02:00:00                  #
 # ================================================== #
 
 from urllib.request import urlopen, Request
 from packaging.version import parse as parse_version
 import json
 import ssl
 from .utils import trans
@@ -130,16 +130,23 @@
         version = "0.0.0"
         updated = False
         if '__meta__' in data and 'version' in data['__meta__']:
             version = data['__meta__']['version']
         old = parse_version(version)
         current = parse_version(self.window.version)
         if old < current:
+            if old < parse_version("0.9.4"):
+                print("Migrating config from < 0.9.4...")
+                if 'plugins' not in data:
+                    data['plugins'] = {}
+                if 'plugins_enabled' not in data:
+                    data['plugins_enabled'] = {}
+                updated = True
             if old < parse_version("0.9.2"):
-                print("Migrating config from 0.9.2...")
+                print("Migrating config from < 0.9.2...")
                 keys_to_remove = ['ui.ctx.min_width',
                                   'ui.ctx.max_width',
                                   'ui.toolbox.min_width',
                                   'ui.toolbox.max_width',
                                   'ui.dialog.settings.width',
                                   'ui.dialog.settings.height',
                                   'ui.chatbox.font.color']
@@ -147,23 +154,23 @@
                     if key in data:
                         del data[key]
                 if 'theme' not in data:
                     data['theme'] = "dark_teal"
                 updated = True
 
             if old < parse_version("0.9.1"):
-                print("Migrating config from 0.9.1...")
+                print("Migrating config from < 0.9.1...")
                 keys_to_remove = ['user_id', 'custom']  # not needed anymore
                 for key in keys_to_remove:
                     if key in data:
                         del data[key]
                 keys_to_add = ['organization_key']
                 for key in keys_to_add:
                     if key not in data:
                         data[key] = ""
                 updated = True
 
         # update file
         if updated:
             print("Migrated config.json.")
             self.window.config.data = data
-            self.window.config.save_config()
+            self.window.config.save()
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/core/utils.py` & `pygpt-net-0.9.4/src/pygpt_net/core/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Created Date: 2023.04.09 20:00:00                  #
+# Updated Date: 2023.04.15 02:00:00                  #
 # ================================================== #
 
 import os
 import re
 from .locale import Locale
 
 locale = None
@@ -30,15 +30,24 @@
     if reload:
         locale.reload()
     return locale.get(key)
 
 
 def get_init_value(key="__version__"):
     """
-    Returns version
+    Returns config value from __init__.py
 
-    :return: version string
+    :return: config value
     """
-    path = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '__init__.py'))
-    result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(key),
-                       open(path, "r", encoding="utf-8").read())
-    return result.group(1)
+    if __file__.endswith('.pyc'):  # if compiled with pyinstaller
+        root = '.'
+    else:
+        root = os.path.join(os.path.dirname(__file__), os.pardir)
+    path = os.path.abspath(os.path.join(root, '__init__.py'))
+    try:
+        f = open(path, "r", encoding="utf-8")
+        data = f.read()
+        f.close()
+        result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(key), data)
+        return result.group(1)
+    except Exception as e:
+        print(e)
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/config/config.json` & `pygpt-net-0.9.4/src/pygpt_net/data/config/config.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'__meta__'": "{'version': '0.9.4', 'app.version': '0.9.4', 'updated_at': '2023-04-15T07:25:00'}",*

 * * "'plugins'": "OrderedDict([('self_loop', OrderedDict([('iterations', 5), ('clear_output', True), "*

 * *              "('reverse_roles', True)])), ('real_time', OrderedDict([('hour', True), ('date', "*

 * *              "True), ('tpl', ' Current time is {time}.')]))])",*

 * * "'plugins_enabled'": "OrderedDict([('self_loop', False), ('real_time', False)])"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "0.9.2",
-        "updated_at": "2023-04-12T07:25:00",
-        "version": "0.9.2"
+        "app.version": "0.9.4",
+        "updated_at": "2023-04-15T07:25:00",
+        "version": "0.9.4"
     },
     "ai_name": "",
     "api_key": "",
     "context_threshold": 200,
     "ctx": "",
     "current_model": {
         "chat": "gpt-3.5-turbo",
@@ -28,14 +28,30 @@
     "max_output_tokens": 1024,
     "max_tokens_length": 32000,
     "max_total_tokens": 4096,
     "mode": "chat",
     "model": "gpt-3.5-turbo",
     "organization_key": "",
     "output_timestamp": true,
+    "plugins": {
+        "real_time": {
+            "date": true,
+            "hour": true,
+            "tpl": " Current time is {time}."
+        },
+        "self_loop": {
+            "clear_output": true,
+            "iterations": 5,
+            "reverse_roles": true
+        }
+    },
+    "plugins_enabled": {
+        "real_time": false,
+        "self_loop": false
+    },
     "presence_penalty": 0.0,
     "preset": "current.chat",
     "prompt": "",
     "send_clear": true,
     "send_shift_enter": false,
     "store_history": true,
     "store_history_time": true,
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/config/models.json` & `pygpt-net-0.9.4/src/pygpt_net/data/config/models.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'__meta__'": "{'version': '0.9.4', 'app.version': '0.9.4', 'updated_at': '2023-04-15T07:25:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "0.9.2",
-        "updated_at": "2023-04-12T07:25:00",
-        "version": "0.9.2"
+        "app.version": "0.9.4",
+        "updated_at": "2023-04-15T07:25:00",
+        "version": "0.9.4"
     },
     "gpt-3.5-turbo": {
         "id": "gpt-3.5-turbo",
         "mode": [
             "chat"
         ],
         "name": "gpt-3.5-turbo",
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json` & `pygpt-net-0.9.4/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/icon.ico` & `pygpt-net-0.9.4/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/icon.png` & `pygpt-net-0.9.4/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.en.ini` & `pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.en.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [LOCALE]
 about.thanks = Special thanks to GitHub community
 alert.preset.empty_id = ID (filename) is required!
 alert.preset.no_chat_completion = At least one of chat or completion option is required!
 alert.title = Info
 chatbox.label = Chat
+chatbox.plugins = plugin(s)
 coming_soon = Coming soon...
 confirm.preset.clear = Are you sure to clear preset?
 confirm.preset.delete = Are you sure to delete this preset?
 confirm.preset.overwrite = Preset exists. Overwrite?
 confirm.img.delete = Delete file from disk?
 context.btn.clear = Clear memory
 context.items = items
@@ -37,14 +38,15 @@
 dialog.editor.btn.defaults = Restore
 dialog.editor.btn.save = Save changes
 dialog.editor.label = Editing config file - app restart is required to apply changes.
 dialog.editor.title = Edit JSON file
 dialog.preset = Preset editor
 dialog.preset.btn.current = Use current
 dialog.preset.btn.save = Save changes
+dialog.plugin_settings = Plugins settings
 dialog.settings = Settings
 dialog.settings.btn.defaults = Restore
 dialog.settings.btn.save = Save changes
 dialog.start.btn = Go to settings...
 dialog.start.title.text = Your API key is not configured yet...\nYou will obtain an API key by registering an account on the OpenAI website:
 dialog.start.link = https://platform.openai.com/account/api-keys
 dialog.start.settings.text = If you already have an API KEY then you can configure it in the settings window.\nClick on button GO TO SETTINGS and then paste your API KEY into API KEY field.
@@ -70,24 +72,26 @@
 menu.config.save = Save config
 menu.config.settings = Settings...
 menu.debug = Debug
 menu.debug.config = Config...
 menu.debug.context = Context...
 menu.debug.models = Models...
 menu.debug.presets = Presets...
+menu.debug.plugins = Plugins...
 menu.file = File
 menu.file.exit = Exit
 menu.file_clear_history = Clear history...
 menu.info = About
 menu.info.about = About
 menu.info.changelog = Changelog
 menu.info.github = GitHub project page...
 menu.info.website = Official website - pygpt.net
 menu.lang = Language
 menu.plugins = Plugins
+menu.plugins.settings = Settings...
 menu.theme = Theme
 mode.chat = Chat
 mode.completion = Completion
 mode.img = Image (DALL-E 2)
 output.timestamp = Show time
 preset.action.delete = Delete
 preset.action.duplicate = Duplicate
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [LOCALE]
 about.thanks = Specjalne podziękowania dla społeczności GitHub-a
 alert.preset.empty_id = ID (nazwa dla pliku) jest wymagana!
 alert.preset.no_chat_completion = Przynajmniej jedna opcja (czat completion albo obraz) jest wymagana!
 alert.title = Informacja
 chatbox.label = Czat
+chatbox.plugins = plugin(ów)
 coming_soon = Dostępne wkrótce...
 confirm.preset.clear = Na pewno wyczyścić preset?
 confirm.preset.delete = Na pewno chcesz usunąć ten preset?
 confirm.preset.overwrite = Preset już istnieje. Czy zastąpić plik?
 confirm.img.delete = Usunąć obraz z dysku?
 context.btn.clear = Wyczyść pamięć
 context.items = elementy
@@ -34,17 +35,18 @@
 dialog.ctx.rename.dismiss = Anuluj
 dialog.ctx.rename.title = Zmień nazwę wpisu
 dialog.ctx.rename.update = Zmień nazwę
 dialog.editor.btn.defaults = Przywróć
 dialog.editor.btn.save = Zapis zmiany
 dialog.editor.label = Edytujesz plik konfiguracyjny - wymagany restart aplikacji aby załadować zmiany.
 dialog.editor.title = Edycja pliku JSON
-dialog.preset = Edytorów presetów
+dialog.preset = Edytor presetów
 dialog.preset.btn.current = Użyj aktualnego
 dialog.preset.btn.save = Zapisz zmiany
+dialog.plugin_settings = Ustawienia pluginów
 dialog.settings = Ustawienia
 dialog.settings.btn.defaults = Przywróć
 dialog.settings.btn.save = Zapisz zmiany
 dialog.start.btn = PRZEJDŹ DO USTAWIEŃ...
 dialog.start.title.text = Nie skonfigurowałeś jeszcze klucza API...\nKlucz API uzyskasz rejestrując konto na stronie internetowej OpenAI:
 dialog.start.link = https://platform.openai.com/account/api-keys
 dialog.start.settings.text = Jeśli posiadasz już klucz API możesz go skonfigurować w oknie ustawień.\nAby to zrobić, kliknij na przycisk poniżej i wklej swój klucz API do pola Klucz API.
@@ -70,24 +72,26 @@
 menu.config.save = Zapisz ustawienia
 menu.config.settings = Ustawienia...
 menu.debug = Debug
 menu.debug.config = Konfiguracja...
 menu.debug.context = Kontekst...
 menu.debug.models = Modele...
 menu.debug.presets = Presety...
+menu.debug.plugins = Pluginy...
 menu.file = Plik
 menu.file.exit = Zakończ
 menu.file_clear_history = Usuń historię...
 menu.info = Informacje
 menu.info.about = O programie
 menu.info.changelog = Dziennik zmian
 menu.info.github = Strona na GitHub-ie...
 menu.info.website = Strona projektu - pygpt.net
 menu.lang = Język
 menu.plugins = Pluginy
+menu.plugins.settings = Ustawienia...
 menu.theme = Motyw
 mode.chat = Czat
 mode.completion = Uzupełnianie
 mode.img = Obraz (DALL-E 2)
 output.timestamp = Pokaż czas
 preset.action.delete = Usuń
 preset.action.duplicate = Duplikuj
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net/data/logo.png` & `pygpt-net-0.9.4/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.3/src/pygpt_net.egg-info/PKG-INFO` & `pygpt-net-0.9.4/src/pygpt_net.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 0.9.3
+Version: 0.9.4
 Summary: A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
 Home-page: https://github.com/szczyglis-dev/py-gpt
 Author: Marcin Szczygliński
 Author-email: Marcin Szczygliński <info@pygpt.net>
 Maintainer: Marcin Szczygliński
 Maintainer-email: info@pygpt.net
 License: MIT License
@@ -34,26 +34,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Current release: **0.9.3** (build: **2023.04.14**)
-
-Official website: https://pygpt.net
+# PYGPT
 
-Documentation: https://pygpt.readthedocs.io
+Current release: **0.9.4** (build: **2023.04.15**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
 
 PyPi: https://pypi.org/project/pygpt-net
 
 ### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
 
-# PYGPT
-
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
 artificial intelligence models such as **GPT4** and **GPT3** using your
 own computer and `OpenAI API`. It allows you to talk in chat mode and in
 completion mode, as well as generate images using **DALL-E 2**.
 Moreover, the application has implemented context memory support,
@@ -79,14 +75,15 @@
 - allows you to easily manage prompts with handly editable presets
 - intuitive operation and interface
 - allows you to use all the powerful features of `GPT4` and `GPT3`
 - no knowledge of using AI models required
 - enables easy and convenient generation of images using `DALL-E 2`
 - has the ability to support future OpenAI models
 - fully configurable
+- plugins support
 - built-in tokens usage calculation
 - it\'s open source, source code is available on `GitHub`
 - **uses the user\'s API key**
 
 The application is free, open source and runs on PC with `Windows 10`,
 `Windows 11` and `Linux`. The full **Python** source code is available
 on `GitHub`.
@@ -126,14 +123,29 @@
 
 3. Once installed run the command to start the application:
 
 ``` commandline
 pygpt
 ```
 
+**Troubleshooting**: 
+
+If you have problems with xcb plugin with newer versions of PySide on Linux, e.g. like this:
+
+```commandline
+qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
+This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
+```
+
+...then try downgrading PySide to `PySide6-Essentials==6.4.2`:
+
+```commandline
+pip install PySide6-Essentials==6.4.2
+```
+
 ### Running from GitHub source code
 
 1. Clone git repository or download .zip file:
 
 ```commandline
 git clone https://github.com/szczyglis-dev/py-gpt.git
 cd py-gpt
@@ -155,14 +167,17 @@
 4. Run the application:
 
 ```commandline
 cd src/pygpt_net
 python app.py
 ```
 
+**Tip**: you can use `PyInstaller` to create a compiled version of
+the application for your system.
+
 ## Other requirements
 
 To operate, you need an Internet connection (for API connection),
 registered OpenAI account and an active API key, which must be entered
 in the program.
 
 
@@ -336,14 +351,25 @@
 **Tip:** with presets, you can save prepared prompts and use them later
 when generating subsequent images.
 
 All queries are saved in the history, thanks to which you can return to
 a given session at any time and use old queries to, for example,
 generate new content.
 
+## Plugins
+
+The application allows you to use plugins to extend its functionality.
+Currently, the following plugins are available:
+
+- **SelfLoop** - allows to run GPT in a self-loop, which allows you to
+  generate a continuous conversation between AI <> AI. In this mode model talks to itself.
+
+- **RealTime** - auto-append current date and time to the prompt. It tells
+  the model what time it is in real time.
+
 
 # Tokens calculation
 
 ## Input tokens
 
 Calculation of tokens is implemented in the application. The application
 tries to predict the number of tokens that will be used for a given
@@ -490,15 +516,19 @@
 
 Support for plug-ins and voice recognition and synthesis will be added
 in future versions of the application.
 
 
 # CHANGELOG
 
-## v0.9.3 (2023.04.13)
+## v0.9.4 (2023.04.15)
+
+- added plugins support
+
+## v0.9.3 (2023.04.14)
 
 - packed into PyPI package
 
 ## v0.9.2 (2023.04.12)
 
 - added theme color settings
 - small UI fixes
@@ -508,21 +538,23 @@
 - added organization key configuration (by @kaneda2004, PR#1)
 - added config versions patching
 
 ## v0.9.0 (2023.04.09)
 
 - initial release
 
-# Credits
+# Credits and links
 
 **Official website:** <https://pygpt.net>
 
 **Documentation:** <https://pygpt.readthedocs.io>
 
 **GitHub:** <https://github.com/szczyglis-dev/py-gpt>
 
+**PyPI:** <https://pypi.org/project/pygpt-net>
+
 **Author:** Marcin Szczygliński (Poland, UE)
 
 **Contact:** <info@pygpt.net>
 
 **License:** MIT License
```

### Comparing `pygpt-net-0.9.3/src/pygpt_net.egg-info/SOURCES.txt` & `pygpt-net-0.9.4/src/pygpt_net.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/pygpt_net/core/context.py
 src/pygpt_net/core/debugger.py
 src/pygpt_net/core/gpt.py
 src/pygpt_net/core/history.py
 src/pygpt_net/core/image.py
 src/pygpt_net/core/info.py
 src/pygpt_net/core/locale.py
+src/pygpt_net/core/plugins.py
 src/pygpt_net/core/settings.py
 src/pygpt_net/core/tokens.py
 src/pygpt_net/core/updater.py
 src/pygpt_net/core/utils.py
 src/pygpt_net/core/controller/__init__.py
 src/pygpt_net/core/controller/confirm.py
 src/pygpt_net/core/controller/context.py
@@ -42,15 +43,22 @@
 src/pygpt_net/core/controller/settings.py
 src/pygpt_net/core/controller/theme.py
 src/pygpt_net/core/controller/ui.py
 src/pygpt_net/core/debug/__init__.py
 src/pygpt_net/core/debug/config.py
 src/pygpt_net/core/debug/context.py
 src/pygpt_net/core/debug/models.py
+src/pygpt_net/core/debug/plugins.py
 src/pygpt_net/core/debug/presets.py
+src/pygpt_net/core/plugin/__init__.py
+src/pygpt_net/core/plugin/base_plugin.py
+src/pygpt_net/core/plugin/real_time/__init__.py
+src/pygpt_net/core/plugin/real_time/plugin.py
+src/pygpt_net/core/plugin/self_loop/__init__.py
+src/pygpt_net/core/plugin/self_loop/plugin.py
 src/pygpt_net/core/ui/__init__.py
 src/pygpt_net/core/ui/chatbox.py
 src/pygpt_net/core/ui/contexts.py
 src/pygpt_net/core/ui/dialogs.py
 src/pygpt_net/core/ui/input.py
 src/pygpt_net/core/ui/main.py
 src/pygpt_net/core/ui/menu.py
@@ -60,14 +68,15 @@
 src/pygpt_net/core/ui/dialog/__init__.py
 src/pygpt_net/core/ui/dialog/about.py
 src/pygpt_net/core/ui/dialog/changelog.py
 src/pygpt_net/core/ui/dialog/ctx_rename.py
 src/pygpt_net/core/ui/dialog/debug.py
 src/pygpt_net/core/ui/dialog/editor.py
 src/pygpt_net/core/ui/dialog/image.py
+src/pygpt_net/core/ui/dialog/plugins.py
 src/pygpt_net/core/ui/dialog/preset.py
 src/pygpt_net/core/ui/dialog/settings.py
 src/pygpt_net/core/ui/dialog/start.py
 src/pygpt_net/core/ui/dialog/update.py
 src/pygpt_net/data/icon.ico
 src/pygpt_net/data/icon.png
 src/pygpt_net/data/logo.png
```

