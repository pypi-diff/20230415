# Comparing `tmp/nonebot_plugin_arktools-1.0.9.tar.gz` & `tmp/nonebot_plugin_arktools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_arktools-1.0.9.tar", last modified: Sun Feb 19 08:58:57 2023, max compression
+gzip compressed data, was "nonebot_plugin_arktools-1.1.0.tar", last modified: Sat Apr 15 08:12:16 2023, max compression
```

## Comparing `nonebot_plugin_arktools-1.0.9.tar` & `nonebot_plugin_arktools-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.779281 nonebot_plugin_arktools-1.0.9/
--rw-rw-rw-   0        0        0     1067 2022-07-09 04:15:32.000000 nonebot_plugin_arktools-1.0.9/LICENSE
--rw-rw-rw-   0        0        0    13712 2023-02-19 08:58:57.778305 nonebot_plugin_arktools-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    13145 2023-02-19 08:55:44.000000 nonebot_plugin_arktools-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.713849 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/
--rw-rw-rw-   0        0        0       20 2023-02-10 14:33:50.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.723616 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/
--rw-rw-rw-   0        0        0      405 2023-02-13 18:24:52.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.732405 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/configs/
--rw-rw-rw-   0        0        0      117 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/configs/__init__.py
--rw-rw-rw-   0        0        0      279 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/configs/ocr_config.py
--rw-rw-rw-   0        0        0      884 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/configs/path_config.py
--rw-rw-rw-   0        0        0      325 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/configs/proxy_config.py
--rw-rw-rw-   0        0        0      505 2023-02-19 08:19:59.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/configs/scheduler_config.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.735335 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/
--rw-rw-rw-   0        0        0       51 2023-02-11 06:02:39.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.740218 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/database/
--rw-rw-rw-   0        0        0       58 2023-02-11 20:30:55.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/database/__init__.py
--rw-rw-rw-   0        0        0     9610 2023-02-11 20:30:55.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/database/game_sqlite.py
--rw-rw-rw-   0        0        0     1085 2023-02-13 18:36:26.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/database/plugin_sqlite.py
--rw-rw-rw-   0        0        0    49491 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/models_v3.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.741194 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/exceptions/
--rw-rw-rw-   0        0        0      694 2022-09-18 13:14:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.745101 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/game_guess_operator/
--rw-rw-rw-   0        0        0     6131 2023-02-12 15:07:16.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/game_guess_operator/__init__.py
--rw-rw-rw-   0        0        0     7086 2023-02-19 08:54:05.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/game_guess_operator/data_source.py
--rw-rw-rw-   0        0        0     1241 2023-02-13 18:31:34.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/help.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.748031 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_monster_siren/
--rw-rw-rw-   0        0        0     1081 2023-02-12 15:07:16.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-02-11 19:09:55.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.749007 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_operator_birthday/
--rw-rw-rw-   0        0        0     2771 2023-02-16 10:07:49.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.750960 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_announce_push/
--rw-rw-rw-   0        0        0     6874 2023-02-19 08:37:55.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_announce_push/__init__.py
--rw-rw-rw-   0        0        0     1284 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_announce_push/data_source.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.753890 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_open_recruitment/
--rw-rw-rw-   0        0        0     3848 2023-02-16 10:07:49.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py
--rw-rw-rw-   0        0        0    11408 2023-02-16 09:49:30.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.756820 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_operator_info/
--rw-rw-rw-   0        0        0     1817 2023-02-16 10:07:49.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_operator_info/__init__.py
--rw-rw-rw-   0        0        0    19768 2023-02-11 06:35:28.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_operator_info/data_source.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.758773 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_sanity_notify/
--rw-rw-rw-   0        0        0     4980 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.766587 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/
--rw-rw-rw-   0        0        0     2152 2023-02-19 08:34:28.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/__init__.py
--rw-rw-rw-   0        0        0     9845 2023-02-19 08:37:55.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/database.py
--rw-rw-rw-   0        0        0     5954 2023-02-12 16:00:06.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/general.py
--rw-rw-rw-   0        0        0     1859 2023-02-10 17:40:27.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/image.py
--rw-rw-rw-   0        0        0    12552 2023-02-19 08:34:28.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/update.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.776352 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/
--rw-rw-rw-   0        0        0        0 2023-02-11 05:40:06.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-11 05:39:33.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/test_database_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-11 05:39:51.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/test_models_v3.py
--rw-rw-rw-   0        0        0      613 2023-02-12 15:46:38.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/test_open_recruitment.py
--rw-rw-rw-   0        0        0        0 2023-02-11 05:39:26.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/test_operator_info.py
--rw-rw-rw-   0        0        0        0 2023-02-11 05:39:44.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/test_update_utils.py
--rw-rw-rw-   0        0        0     2251 2023-02-11 05:58:04.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-19 08:58:57.720685 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/
--rw-rw-rw-   0        0        0    13712 2023-02-19 08:58:57.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2023-02-19 08:58:57.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 08:58:57.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      232 2023-02-19 08:58:57.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-02-19 08:58:57.000000 nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 08:58:57.779281 nonebot_plugin_arktools-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1256 2023-02-19 08:07:12.000000 nonebot_plugin_arktools-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.253734 nonebot_plugin_arktools-1.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    18443 2023-04-15 08:12:16.252735 nonebot_plugin_arktools-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17876 2023-04-15 07:55:11.000000 nonebot_plugin_arktools-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.063719 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/
+-rw-rw-rw-   0        0        0       20 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.094722 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/
+-rw-rw-rw-   0        0        0      498 2023-04-14 10:56:53.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.117725 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/
+-rw-rw-rw-   0        0        0      145 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/draw_config.py
+-rw-rw-rw-   0        0        0      279 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/ocr_config.py
+-rw-rw-rw-   0        0        0     1003 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/path_config.py
+-rw-rw-rw-   0        0        0      367 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/proxy_config.py
+-rw-rw-rw-   0        0        0      729 2023-04-15 07:42:06.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/configs/scheduler_config.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.125724 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/
+-rw-rw-rw-   0        0        0       51 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.137726 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/
+-rw-rw-rw-   0        0        0       58 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/__init__.py
+-rw-rw-rw-   0        0        0    14379 2023-04-15 06:20:52.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/game_sqlite.py
+-rw-rw-rw-   0        0        0     1897 2023-04-14 11:58:27.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/plugin_sqlite.py
+-rw-rw-rw-   0        0        0    68752 2023-04-15 05:52:38.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/models_v3.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.140727 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/exceptions/
+-rw-rw-rw-   0        0        0     1413 2023-04-14 11:36:38.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.144725 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_draw_card/
+-rw-rw-rw-   0        0        0      629 2023-04-07 10:02:31.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_draw_card/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.152728 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/
+-rw-rw-rw-   0        0        0     6382 2023-04-14 09:17:46.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/__init__.py
+-rw-rw-rw-   0        0        0     7194 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/data_source.py
+-rw-rw-rw-   0        0        0     1321 2023-04-14 10:56:39.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/help.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.160728 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/
+-rw-rw-rw-   0        0        0     1081 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.163728 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_operator_birthday/
+-rw-rw-rw-   0        0        0     2839 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.173729 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/
+-rw-rw-rw-   0        0        0     6874 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/data_source.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.181730 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/
+-rw-rw-rw-   0        0        0     5999 2023-04-15 07:49:18.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/__init__.py
+-rw-rw-rw-   0        0        0     5990 2023-04-15 07:48:53.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_fetch_maa_copilot/data_source.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.189730 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/
+-rw-rw-rw-   0        0        0     3771 2023-04-14 09:06:35.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py
+-rw-rw-rw-   0        0        0    11512 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.197729 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/
+-rw-rw-rw-   0        0        0     1902 2023-03-28 04:16:27.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/__init__.py
+-rw-rw-rw-   0        0        0    19932 2023-04-08 12:40:58.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/data_source.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.202730 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_sanity_notify/
+-rw-rw-rw-   0        0        0     5361 2023-04-14 09:13:06.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.222731 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/
+-rw-rw-rw-   0        0        0     2172 2023-04-07 02:49:03.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/__init__.py
+-rw-rw-rw-   0        0        0    17666 2023-04-15 08:05:19.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/database.py
+-rw-rw-rw-   0        0        0     7997 2023-04-15 07:01:42.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/general.py
+-rw-rw-rw-   0        0        0     1859 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/image.py
+-rw-rw-rw-   0        0        0    13739 2023-04-15 02:39:41.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/update.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.247733 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/
+-rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_database_utils.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_models.py
+-rw-rw-rw-   0        0        0      613 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_open_recruitment.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_operator_info.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_update_utils.py
+-rw-rw-rw-   0        0        0     2251 2023-03-24 02:11:10.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:12:16.086723 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/
+-rw-rw-rw-   0        0        0    18443 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2465 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      234 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-15 08:12:15.000000 nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 08:12:16.254736 nonebot_plugin_arktools-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-04-14 09:22:48.000000 nonebot_plugin_arktools-1.1.0/setup.py
```

### Comparing `nonebot_plugin_arktools-1.0.9/LICENSE` & `nonebot_plugin_arktools-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Number_Sir
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Number_Sir
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_arktools-1.0.9/PKG-INFO` & `nonebot_plugin_arktools-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_arktools
-Version: 1.0.9
-Summary: 基于 OneBot 适配器的 NoneBot2 明日方舟小工具箱插件
-Home-page: https://github.com/NumberSir/nonebot_plugin_arktools
-Author: Number_Sir
-Author-email: Number_Sir@126.com
-Keywords: pip,nonebot2,nonebot,nonebot_plugin
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
   
 # Nonebot_Plugin_ArkTools
   
 _✨ 基于 OneBot 适配器的 [NoneBot2](https://v2.nonebot.dev/) 明日方舟小工具箱插件 ✨_
   
 </div>
 
-[![OSCS Status](https://www.oscs1024.com/platform/badge/NumberSir/nonebot_plugin_arktools.svg?size=small)](https://www.oscs1024.com/project/NumberSir/nonebot_plugin_arktools?ref=badge_small)
+[![OSCS Status](https://www.oscs1024.com/platform/badge/NumberSir/nonebot_plugin_arktools.svg?size=small)](https://www.oscs1024.com/project/NumberSir/nonebot_plugin_arktools?ref=badge_small)  [![star](https://gitee.com/Number_Sir/nonebot_plugin_arktools/badge/star.svg?theme=white)](https://gitee.com/Number_Sir/nonebot_plugin_arktools/stargazers)
 
 本人python小萌新，插件有不完善和可以改进之处欢迎各位多提pr和issue
 
 - [功能](#功能)
 - [安装](#安装)
 - [使用](#如何使用)
 - [示例](#图片示例)
@@ -42,14 +26,15 @@
 1. [x] 可以查询推荐的公招标签(截图识别/手动输文字)
 2. [x] 可以查询干员的技能升级材料、专精材料、精英化材料、模组升级材料
 3. [x] 可以通过网易云点歌，以卡片形式发送
 4. [x] 猜干员小游戏，玩法与 [wordle](https://github.com/noneplugin/nonebot-plugin-wordle) 相同
 5. [x] 可以查看生日为今天的干员
 6. [x] 可以记录当前理智，等回复满后提醒
 7. [x] 指定群聊自动推送最新游戏公告
+8. [x] 查询、订阅、推送 [MAA 作业站](https://prts.plus)的作业
 
 ## 编写中...
 1. [ ] 可以查询某种资源在哪个关卡期望理智最低
 2. [ ] 根据当前有的资源和需要的资源种类、数量测算最优推图计划
 3. [ ] 查询某干员的基础数据：
    1. [ ] 给定等级、信赖、潜能下的基础面板
    2. [ ] 天赋、特性、技能
@@ -58,67 +43,99 @@
 
 # 安装
 - 使用 pip
 ```
 pip install -U nonebot_plugin_arktools
 ```
 
+- 使用 nb-cli
+```
+nb plugin install nonebot_plugin_arktools
+```
+
 # 如何使用
 ## 启动注意
  - 每次启动并连接到客户端后会从 __[明日方舟常用素材库](https://github.com/yuanyan3060/Arknights-Bot-Resource)__(__[yuanyan3060](https://github.com/yuanyan3060)__), __[《明日方舟》游戏数据库](https://github.com/Kengxxiao/ArknightsGameData)__(__[Kengxxiao](https://github.com/Kengxxiao)__), __[Arknight-Images](https://github.com/Aceship/Arknight-Images)__(__[Aceship](https://github.com/Aceship)__) 下载使用插件必需的文本及图片资源到本地，已经下载过的文件不会重复下载。下载根据网络情况不同可能耗时 5 分钟左右
  - 如需手动更新，请用命令 __“更新方舟素材”__ 进行更新
- - 如果自动下载失败，请手动下载发行版中的 __“`data.zip`”__ 压缩文件，解压到 __“`nonebot_plugin_arktools/data`”__ 文件夹下，正确放置的文件夹结构应为：
+ - 如果自动下载失败，请手动下载发行版中的 __“`data.zip`”/“`data.tar.gz`”__ 压缩文件，解压到 “`机器人根目录`” 文件夹下(即运行 `nb run` 命令的文件夹/ `bot.py` 的文件夹)。正确放置的文件夹结构应为：
 ```txt
-nonebot_plugin_arktools
+举例：
 ├── data
-│   ├── arknights
-│   │   ├── gamedata
-│   │   │   └── excel
-│   │   │       └── ...
-│   │   ├── gameimage
-│   │   │   └── ...
-│   │   └── ...
-│   ├── fonts
-│   │   ├── Arknights-en.ttf
-│   │   └── Arknights-zh.otf
-│   ├── guess_character
-│   │   ├── correct.png
-│   │   ├── down.png
-│   │   ├── up.png
-│   │   ├── vague.png
-│   │   └── wrong.png
-│   └── ...
-├── src
-├── test
-├── ...
+│   └── arktools
+│       ├── arknights
+│       │   ├── gamedata
+│       │   │   └── excel
+│       │   │       └── ...
+│       │   ├── gameimage
+│       │   │   └── ...
+│       │   ├── processed_data
+│       │   │   └── nicknames.json
+│       │   └── ...
+│       ├── fonts
+│       │   ├── Arknights-en.ttf
+│       │   └── Arknights-zh.otf
+│       ├── guess_character
+│       │   ├── correct.png
+│       │   ├── down.png
+│       │   ├── up.png
+│       │   ├── vague.png
+│       │   └── wrong.png
+│       └── ...
+├── plugin
+│   └── nonebot_plugin_arktools
+│       ├── src
+│       └── ...
+├── .env
+├── .env.dev
+├── .env.prod
 ...
 ```
 
 ## .env.env 配置项
 
 ```ini
+# 百度 OCR 配置，公招识别截图用
 # 具体见 https://console.bce.baidu.com/ai/?fromai=1#/ai/ocr/app/list
-arknights_baidu_api_key="xxx"    # 【必填】百度 OCR API KEY
-arknights_baidu_secret_key="xxx"   # 【必填】百度 OCR SECRET KEY
+ARKNIGHTS_BAIDU_API_KEY="xxx"    # 【必填】百度 OCR API KEY
+ARKNIGHTS_BAIDU_SECRET_KEY="xxx"   # 【必填】百度 OCR SECRET KEY
 
-github_raw="https://raw.githubusercontent.com"   # 默认为 https://raw.githubusercontent.com，如有镜像源可以替换
-github_site="https://github.com"  # 默认为 https://github.com，如有镜像源可以替换
+# 代理配置，如部署机器人的服务器在国内大陆地区可能需要修改
+GITHUB_RAW="https://raw.githubusercontent.com"   # 默认为 https://raw.githubusercontent.com，如有镜像源可以替换，如 https://ghproxy.com/https://raw.githubusercontent.com
+GITHUB_SITE="https://github.com"  # 默认为 https://github.com，如有镜像源可以替换，如 https://kgithub.com
+RSS_SITE="https://rsshub.app"  # 默认为 https://rsshub.app，如有镜像源可以替换
+
+# 定时任务配置，默认是关闭的
+ANNOUNCE_PUSH_SWITCH=False  # 是否自动推送舟舟最新公告，默认为 False; True 为开启自动检测
+ANNOUNCE_PUSH_INTERVAL=1  # 自动推送最新公告的检测间隔，上述开关开启时有效，默认为 1 分钟
+SANITY_NOTIFY_SWITCH=False  # 是否自动检测理智提醒，默认为 False; True 为开启自动检测
+SANITY_NOTIFY_INTERVAL=10  # 自动检测理智提醒的检测间隔，上述开关开启时有效，默认为 10 分钟
+MAA_COPILOT_SWITCH=False  # 是否自动推送MAA作业站新作业，默认为 False; True 为开启自动检测
+MAA_COPILOT_INTERVAL=60  # 自动推送MAA作业站新作业的检测间隔，上述开关开启时有效，默认为 60 分钟
+
+# 启动前素材检查配置，默认是开启的
+ARKNIGHTS_UPDATE_CHECK_SWITCH=True  # 是否在启动bot时检查素材版本并下载，默认为True; False 为禁用检查
+
+# 资源路径配置，默认在启动机器人的目录中/运行nb run的目录中/放bot.py的目录中
+ARKNIGHTS_DATA_PATH="data/arktools"                                   # 资源根路径，如果修改了根路径，下方路径都要修改
+ARKNIGHTS_FONT_PATH="data/arktools/fonts"                             # 字体路径
+ARKNIGHTS_GAMEDATA_PATH="data/arktools/arknights/gamedata"            # 游戏数据
+ARKNIGHTS_GAMEIMAGE_PATH="data/arktools/arknights/gameimage"          # 游戏图像
+ARKNIGHTS_DB_URL="data/arktools/databases/arknights_sqlite.sqlite3"   # 数据库
 
-announce_push_switch=False  # 是否自动推送舟舟最新公告，默认为 False; True 为开启自动检测
-announce_push_interval=1  # 自动推送最新公告的检测间隔，上述开关开启时有效，默认为 1 分钟
-
-sanity_notify_switch=False  # 是否自动检测理智提醒，默认为 False; True 为开启自动检测
-sanity_notify_interval=10  # 自动检测理智提醒的检测间隔，上述开关开启时有效，默认为 10 分钟
 ...
 ```
 各配置项的含义如上。
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/219335891-37933d79-1b52-4452-8959-04861087f4e8.png" width="700" />
 </div>
 
+
+## 干员昵称
+位置默认在 `data/arknights/processed_data/nicknames.json` 键为干员中文名称，值为昵称，可自行修改。
+
 ## 指令
 <details>
 <summary>点击展开</summary>
 
 ### 详细指令
 使用以下指令触发，需加上指令前缀
 ```text
@@ -166,14 +183,23 @@
 ```
 公告推送
 ```text
 添加方舟推送群 / ADDGROUP   => 添加自动推送的群号
 删除方舟推送群 / DELGROUP   => 删除自动推送的群号
 查看方舟推送群 / GETGROUP   => 查看自动推送的群号
 ```
+MAA 作业站相关
+```text
+maa添加订阅 / ADDMAA [关键词1 关键词2 ...]  => 添加自动推送的关键词
+maa删除订阅 / DELMAA [关键词1 关键词2 ...]  => 删除自动推送的关键词
+maa查看订阅 / GETMAA                      => 查看本群自动推送的关键词
+
+maa查作业 [关键词1 关键词2 ...]                   => 按关键词组合查作业，默认为最新发布的第一个作业
+maa查作业 [关键词1 关键词2 ...] | [热度/最新/访问]  => 同上，不过可以指定按什么顺序查询
+```
 </details>
 
 # 图片示例
 <details>
 <summary>点击展开</summary>
 
 ## 图片们
@@ -221,20 +247,54 @@
 
 # 感谢
  - __[yuanyan3060](https://github.com/yuanyan3060)__ 的 __[明日方舟常用素材库](https://github.com/yuanyan3060/Arknights-Bot-Resource)__
  - __[Kengxxiao](https://github.com/Kengxxiao)__ 的 __[《明日方舟》游戏数据库](https://github.com/Kengxxiao/ArknightsGameData)__
  - __[Aceship](https://github.com/Aceship)__ 的 __[Arknight-Images](https://github.com/Aceship/Arknight-Images)__
  - __[AmiyaBot](https://github.com/AmiyaBot)__ 的 __[Amiya-bot](https://github.com/AmiyaBot/Amiya-Bot)__
  - __[Strelizia02](https://github.com/Strelizia02)__ 的 __[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__
-
+ - __[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ 的 __[MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights)__
 
 # 更新日志
 <details>
 <summary>点击展开</summary>
 
+> 2023-04-15 v1.1.0
+> - 公招查询、猜干员、理智提醒现在均可以私聊进行 (不推荐，私聊发消息可能导致风控)
+> - 简易修复了与其它同用 Tortoise-ORM 的插件初始化冲突的问题 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15)
+> - 添加在群聊查询、订阅、推送 [MAA 作业站](https://prts.plus)作业的功能
+> - 修复了更新数据库中某张表格时会删除所有表格的问题
+> 
+> 2023-04-08 v1.0.20
+> - 修复因素材库更新滞后导致无法查看干员的问题
+> 
+> 2023-04-07 v1.0.19
+> - 修复更新数据库命令不会强制覆盖更新的问题
+> 
+> 2023-04-06 v1.0.18
+> - 修复了舟舟更新数据结构导致的创建表单错误
+>
+> 2023-04-04 v1.0.17
+> - 添加数据库初始化检查，不再每次启动bot时重复创建
+> - 添加每次启动bot时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
+>
+> 2023-03-28 v1.0.15
+> - 猜干员与干员信息功能可以使用干员昵称(可自行增删改查)
+> 
+> 2023-03-24 v1.0.14
+> - 修复阿米娅与近卫阿米娅冲突的问题 [@zx-issue/13](https://github.com/NumberSir/zhenxun_arktools/issues/13)
+> 
+> 2023-03-08 v1.0.12
+> - 添加 rsshub 代理配置项 [@issue/34](https://github.com/NumberSir/nonebot_plugin_arktools/issues/34)
+> - 修复公招命令不处理的问题 [@issue/35](https://github.com/NumberSir/nonebot_plugin_arktools/issues/35)
+> - 添加方舟素材/资源路径配置项，现在默认在机器人根目录下 `data/arktools` 文件夹 [@issue/36](https://github.com/NumberSir/nonebot_plugin_arktools/issues/36)
+> - 修复查询暮落干员信息时会选中空白暮落的问题
+> 
+> 2023-02-20 v1.0.11
+> - 修复最新版本检测出错的问题
+> 
 > 2023-02-19 v1.0.9
 > - 添加定时任务配置项
 > - 修复定时任务导致其它处理器阻塞的问题 [@issue/30](https://github.com/NumberSir/nonebot_plugin_arktools/issues/30) [@zx-issue/9](https://github.com/NumberSir/zhenxun_arktools/issues/9)
 > - 修复猜干员无法判断重复猜的问题 [@zx-issue/10](https://github.com/NumberSir/zhenxun_arktools/issues/10)
 > - 修复猜干员结果图不按顺序绘制的问题
 >
 > 2023-02-16 v1.0.8
```

#### html2text {}

```diff
@@ -1,82 +1,103 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_arktools Version: 1.0.9 Summary:
-åºäº OneBot ééå¨ç NoneBot2 ææ¥æ¹èå°å·¥å·ç®±æä»¶ Home-page:
-https://github.com/NumberSir/nonebot_plugin_arktools Author: Number_Sir Author-
-email: Number_Sir@126.com Keywords: pip,nonebot2,nonebot,nonebot_plugin
-Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
                                    [nonebot]
  # Nonebot_Plugin_ArkTools _â¨ åºäº OneBot ééå¨ç [NoneBot2](https://
              v2.nonebot.dev/) ææ¥æ¹èå°å·¥å·ç®±æä»¶ â¨_
 [![OSCS Status](https://www.oscs1024.com/platform/badge/NumberSir/
 nonebot_plugin_arktools.svg?size=small)](https://www.oscs1024.com/project/
-NumberSir/nonebot_plugin_arktools?ref=badge_small)
+NumberSir/nonebot_plugin_arktools?ref=badge_small) [![star](https://gitee.com/
+Number_Sir/nonebot_plugin_arktools/badge/star.svg?theme=white)](https://
+gitee.com/Number_Sir/nonebot_plugin_arktools/stargazers)
 æ¬äººpythonå°èæ°ï¼æä»¶æä¸å®ååå¯ä»¥æ¹è¿ä¹å¤æ¬¢è¿åä½å¤æpråissue
 - [åè½](#åè½) - [å®è£](#å®è£) - [ä½¿ç¨](#å¦ä½ä½¿ç¨) - [ç¤ºä¾]
 (#å¾çç¤ºä¾) - [æè°¢](#æè°¢) - [æ´æ°æ¥å¿](#æ´æ°æ¥å¿) # åè½ ##
 å·²å®ç°ï¼ 1. [x] å¯ä»¥æ¥è¯¢æ¨èçå¬ææ ç­¾(æªå¾è¯å«/
 æå¨è¾æå­) 2. [x]
 å¯ä»¥æ¥è¯¢å¹²åçæè½åçº§ææãä¸ç²¾ææãç²¾è±åææãæ¨¡ç»åçº§ææ
 3. [x] å¯ä»¥éè¿ç½æäºç¹æ­ï¼ä»¥å¡çå½¢å¼åé 4. [x]
 çå¹²åå°æ¸¸æï¼ç©æ³ä¸ [wordle](https://github.com/noneplugin/nonebot-
 plugin-wordle) ç¸å 5. [x] å¯ä»¥æ¥ççæ¥ä¸ºä»å¤©çå¹²å 6. [x]
 å¯ä»¥è®°å½å½åçæºï¼ç­åå¤æ»¡åæé 7. [x]
-æå®ç¾¤èèªå¨æ¨éææ°æ¸¸æå¬å ## ç¼åä¸­... 1. [ ]
+æå®ç¾¤èèªå¨æ¨éææ°æ¸¸æå¬å 8. [x] æ¥è¯¢ãè®¢éãæ¨é [MAA
+ä½ä¸ç«](https://prts.plus)çä½ä¸ ## ç¼åä¸­... 1. [ ]
 å¯ä»¥æ¥è¯¢æç§èµæºå¨åªä¸ªå³å¡ææçæºæä½ 2. [ ]
 æ ¹æ®å½åæçèµæºåéè¦çèµæºç§ç±»ãæ°éæµç®æä¼æ¨å¾è®¡å
 3. [ ] æ¥è¯¢æå¹²åçåºç¡æ°æ®ï¼ 1. [ ]
 ç»å®ç­çº§ãä¿¡èµãæ½è½ä¸çåºç¡é¢æ¿ 2. [ ]
 å¤©èµãç¹æ§ãæè½ 3. [ ]
 å¹²åç§æãå¿åãèº«é«ç­åºæ¬ä¸ªäººä¿¡æ¯ 4. [ ] å®æ¶æéå¿ç­ /
 èå»ç«  / åçº¦ç­æ´»å¨è¿æ # å®è£ - ä½¿ç¨ pip ``` pip install -
-U nonebot_plugin_arktools ``` # å¦ä½ä½¿ç¨ ## å¯å¨æ³¨æ -
+U nonebot_plugin_arktools ``` - ä½¿ç¨ nb-cli ``` nb plugin install
+nonebot_plugin_arktools ``` # å¦ä½ä½¿ç¨ ## å¯å¨æ³¨æ -
 æ¯æ¬¡å¯å¨å¹¶è¿æ¥å°å®¢æ·ç«¯åä¼ä» __[ææ¥æ¹èå¸¸ç¨ç´ æåº]
 (https://github.com/yuanyan3060/Arknights-Bot-Resource)__(__[yuanyan3060]
 (https://github.com/yuanyan3060)__), __[ãææ¥æ¹èãæ¸¸ææ°æ®åº]
 (https://github.com/Kengxxiao/ArknightsGameData)__(__[Kengxxiao](https://
 github.com/Kengxxiao)__), __[Arknight-Images](https://github.com/Aceship/
 Arknight-Images)__(__[Aceship](https://github.com/Aceship)__)
 ä¸è½½ä½¿ç¨æä»¶å¿éçææ¬åå¾çèµæºå°æ¬å°ï¼å·²ç»ä¸è½½è¿çæä»¶ä¸ä¼éå¤ä¸è½½ãä¸è½½æ ¹æ®ç½ç»æåµä¸åå¯è½èæ¶
 5 åéå·¦å³ - å¦éæå¨æ´æ°ï¼è¯·ç¨å½ä»¤ __âæ´æ°æ¹èç´ æâ__
 è¿è¡æ´æ° - å¦æèªå¨ä¸è½½å¤±è´¥ï¼è¯·æå¨ä¸è½½åè¡çä¸­ç
-__â`data.zip`â__ åç¼©æä»¶ï¼è§£åå° __â`nonebot_plugin_arktools/
-data`â__ æä»¶å¤¹ä¸ï¼æ­£ç¡®æ¾ç½®çæä»¶å¤¹ç»æåºä¸ºï¼ ```txt
-nonebot_plugin_arktools âââ data â âââ arknights â â
+__â`data.zip`â/â`data.tar.gz`â__ åç¼©æä»¶ï¼è§£åå°
+â`æºå¨äººæ ¹ç®å½`â æä»¶å¤¹ä¸(å³è¿è¡ `nb run` å½ä»¤çæä»¶å¤¹/
+`bot.py` çæä»¶å¤¹)ãæ­£ç¡®æ¾ç½®çæä»¶å¤¹ç»æåºä¸ºï¼ ```txt
+ä¸¾ä¾ï¼ âââ data â âââ arktools â âââ arknights â â
 âââ gamedata â â â âââ excel â â â âââ ... â
-â âââ gameimage â â â âââ ... â â âââ ... â
+â âââ gameimage â â â âââ ... â â âââ
+processed_data â â â âââ nicknames.json â â âââ ... â
 âââ fonts â â âââ Arknights-en.ttf â â âââ Arknights-
 zh.otf â âââ guess_character â â âââ correct.png â â
 âââ down.png â â âââ up.png â â âââ vague.png â â
-âââ wrong.png â âââ ... âââ src âââ test âââ
-... ... ``` ## .env.env éç½®é¡¹ ```ini # å·ä½è§ https://
+âââ wrong.png â âââ ... âââ plugin â âââ
+nonebot_plugin_arktools â âââ src â âââ ... âââ .env
+âââ .env.dev âââ .env.prod ... ``` ## .env.env éç½®é¡¹ ```ini #
+ç¾åº¦ OCR éç½®ï¼å¬æè¯å«æªå¾ç¨ # å·ä½è§ https://
 console.bce.baidu.com/ai/?fromai=1#/ai/ocr/app/list
-arknights_baidu_api_key="xxx" # ãå¿å¡«ãç¾åº¦ OCR API KEY
-arknights_baidu_secret_key="xxx" # ãå¿å¡«ãç¾åº¦ OCR SECRET KEY
-github_raw="https://raw.githubusercontent.com" # é»è®¤ä¸º https://
-raw.githubusercontent.comï¼å¦æéåæºå¯ä»¥æ¿æ¢ github_site="https://
-github.com" # é»è®¤ä¸º https://github.comï¼å¦æéåæºå¯ä»¥æ¿æ¢
-announce_push_switch=False # æ¯å¦èªå¨æ¨éèèææ°å¬åï¼é»è®¤ä¸º
-False; True ä¸ºå¼å¯èªå¨æ£æµ announce_push_interval=1 #
+ARKNIGHTS_BAIDU_API_KEY="xxx" # ãå¿å¡«ãç¾åº¦ OCR API KEY
+ARKNIGHTS_BAIDU_SECRET_KEY="xxx" # ãå¿å¡«ãç¾åº¦ OCR SECRET KEY #
+ä»£çéç½®ï¼å¦é¨ç½²æºå¨äººçæå¡å¨å¨å½åå¤§éå°åºå¯è½éè¦ä¿®æ¹
+GITHUB_RAW="https://raw.githubusercontent.com" # é»è®¤ä¸º https://
+raw.githubusercontent.comï¼å¦æéåæºå¯ä»¥æ¿æ¢ï¼å¦ https://
+ghproxy.com/https://raw.githubusercontent.com GITHUB_SITE="https://github.com"
+# é»è®¤ä¸º https://github.comï¼å¦æéåæºå¯ä»¥æ¿æ¢ï¼å¦ https://
+kgithub.com RSS_SITE="https://rsshub.app" # é»è®¤ä¸º https://
+rsshub.appï¼å¦æéåæºå¯ä»¥æ¿æ¢ #
+å®æ¶ä»»å¡éç½®ï¼é»è®¤æ¯å³é­ç ANNOUNCE_PUSH_SWITCH=False #
+æ¯å¦èªå¨æ¨éèèææ°å¬åï¼é»è®¤ä¸º False; True
+ä¸ºå¼å¯èªå¨æ£æµ ANNOUNCE_PUSH_INTERVAL=1 #
 èªå¨æ¨éææ°å¬åçæ£æµé´éï¼ä¸è¿°å¼å³å¼å¯æ¶ææï¼é»è®¤ä¸º
-1 åé sanity_notify_switch=False #
+1 åé SANITY_NOTIFY_SWITCH=False #
 æ¯å¦èªå¨æ£æµçæºæéï¼é»è®¤ä¸º False; True ä¸ºå¼å¯èªå¨æ£æµ
-sanity_notify_interval=10 #
+SANITY_NOTIFY_INTERVAL=10 #
 èªå¨æ£æµçæºæéçæ£æµé´éï¼ä¸è¿°å¼å³å¼å¯æ¶ææï¼é»è®¤ä¸º
-10 åé ... ``` åéç½®é¡¹çå«ä¹å¦ä¸ã
+10 åé MAA_COPILOT_SWITCH=False #
+æ¯å¦èªå¨æ¨éMAAä½ä¸ç«æ°ä½ä¸ï¼é»è®¤ä¸º False; True
+ä¸ºå¼å¯èªå¨æ£æµ MAA_COPILOT_INTERVAL=60 #
+èªå¨æ¨éMAAä½ä¸ç«æ°ä½ä¸çæ£æµé´éï¼ä¸è¿°å¼å³å¼å¯æ¶ææï¼é»è®¤ä¸º
+60 åé # å¯å¨åç´ ææ£æ¥éç½®ï¼é»è®¤æ¯å¼å¯ç
+ARKNIGHTS_UPDATE_CHECK_SWITCH=True #
+æ¯å¦å¨å¯å¨botæ¶æ£æ¥ç´ æçæ¬å¹¶ä¸è½½ï¼é»è®¤ä¸ºTrue; False
+ä¸ºç¦ç¨æ£æ¥ # èµæºè·¯å¾éç½®ï¼é»è®¤å¨å¯å¨æºå¨äººçç®å½ä¸­/
+è¿è¡nb runçç®å½ä¸­/æ¾bot.pyçç®å½ä¸­ ARKNIGHTS_DATA_PATH="data/
+arktools" #
+èµæºæ ¹è·¯å¾ï¼å¦æä¿®æ¹äºæ ¹è·¯å¾ï¼ä¸æ¹è·¯å¾é½è¦ä¿®æ¹
+ARKNIGHTS_FONT_PATH="data/arktools/fonts" # å­ä½è·¯å¾
+ARKNIGHTS_GAMEDATA_PATH="data/arktools/arknights/gamedata" # æ¸¸ææ°æ®
+ARKNIGHTS_GAMEIMAGE_PATH="data/arktools/arknights/gameimage" # æ¸¸æå¾å
+ARKNIGHTS_DB_URL="data/arktools/databases/arknights_sqlite.sqlite3" # æ°æ®åº
+... ``` åéç½®é¡¹çå«ä¹å¦ä¸ã
 [https://user-images.githubusercontent.com/52584526/219335891-37933d79-1b52-
 4452-8959-04861087f4e8.png]
-## æä»¤  ç¹å»å±å¼ ### è¯¦ç»æä»¤
-ä½¿ç¨ä»¥ä¸æä»¤è§¦åï¼éå ä¸æä»¤åç¼ ```text æ ¼å¼ï¼ æä»¤ =>
-å«ä¹ [] ä»£è¡¨åæ° xxx/yyy ä»£è¡¨ xxx æ yyy ``` æé¡¹ ```text
-æ¹èå¸®å© / arkhelp => æ¥çæä»¤åè¡¨ æ´æ°æ¹èç´ æ =>
-æå¨æ´æ°æ¸¸ææ°æ®(json)ä¸å¾ç æ´æ°æ¹èæ°æ®åº =>
-æå¨æ´æ°æ°æ®åº ``` çå¹²å ```text çå¹²å => å¼å§æ°æ¸¸æ #
-[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
+## å¹²åæµç§° ä½ç½®é»è®¤å¨ `data/arknights/processed_data/nicknames.json`
+é®ä¸ºå¹²åä¸­æåç§°ï¼å¼ä¸ºæµç§°ï¼å¯èªè¡ä¿®æ¹ã ## æä»¤
+ç¹å»å±å¼ ### è¯¦ç»æä»¤ ä½¿ç¨ä»¥ä¸æä»¤è§¦åï¼éå ä¸æä»¤åç¼
+```text æ ¼å¼ï¼ æä»¤ => å«ä¹ [] ä»£è¡¨åæ° xxx/yyy ä»£è¡¨ xxx æ yyy
+``` æé¡¹ ```text æ¹èå¸®å© / arkhelp => æ¥çæä»¤åè¡¨
+æ´æ°æ¹èç´ æ => æå¨æ´æ°æ¸¸ææ°æ®(json)ä¸å¾ç
+æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº ``` çå¹²å ```text çå¹²å
+=> å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
 æ¥çç­æ¡å¹²åçä¿¡æ¯ ç»æ => ç»æå½åå±æ¸¸æ ``` ä»æ¥å¹²å
 ```text ä»æ¥å¹²å => æ¥çä»å¤©è¿çæ¥çå¹²å ``` å¡å£¬ç¹æ­ ```text
 å¡å£¬ç¹æ­ [å³é®å­] => ç½æäºç¹æ­ï¼ä»¥å¡çå½¢å¼åå°ç¾¤å ```
 å¹²åä¿¡æ¯ ```text å¹²å [å¹²åå] =>
 æ¥çå¹²åçç²¾è±åãæè½åçº§ãæè½ä¸ç²¾ãæ¨¡ç»è§£ééè¦çææ
 ``` å¬å¼æå ```text å¬æ [å¬æçé¢æªå¾] =>
 æ¥çæ ç­¾ç»ååå¯è½åºç°çå¹²å åå¤æªå¾ï¼å¬æ => åä¸
@@ -84,15 +105,23 @@
 => é»è®¤è®°å½åçæºä¸º0ï¼åæ»¡å°135æ¶æé" çæºæé
 [å½åçæº] [åæ»¡çæº] =>
 åä¸ï¼ä¸è¿æå¨æå®å½åçæºä¸åæ»¡çæº" çæºæ¥ç =>
 æ¥çè·ç¦»çæºåæ»¡è¿æå¤ä¹ï¼ä»¥åå½æçæºä¸ºå¤å°" ```
 å¬åæ¨é ```text æ·»å æ¹èæ¨éç¾¤ / ADDGROUP =>
 æ·»å èªå¨æ¨éçç¾¤å· å é¤æ¹èæ¨éç¾¤ / DELGROUP =>
 å é¤èªå¨æ¨éçç¾¤å· æ¥çæ¹èæ¨éç¾¤ / GETGROUP =>
-æ¥çèªå¨æ¨éçç¾¤å· ```  # å¾çç¤ºä¾  ç¹å»å±å¼ ## å¾çä»¬
+æ¥çèªå¨æ¨éçç¾¤å· ``` MAA ä½ä¸ç«ç¸å³ ```text maaæ·»å è®¢é /
+ADDMAA [å³é®è¯1 å³é®è¯2 ...] => æ·»å èªå¨æ¨éçå³é®è¯
+maaå é¤è®¢é / DELMAA [å³é®è¯1 å³é®è¯2 ...] =>
+å é¤èªå¨æ¨éçå³é®è¯ maaæ¥çè®¢é / GETMAA =>
+æ¥çæ¬ç¾¤èªå¨æ¨éçå³é®è¯ maaæ¥ä½ä¸ [å³é®è¯1 å³é®è¯2 ...]
+=> æå³é®è¯ç»åæ¥ä½ä¸ï¼é»è®¤ä¸ºææ°åå¸çç¬¬ä¸ä¸ªä½ä¸
+maaæ¥ä½ä¸ [å³é®è¯1 å³é®è¯2 ...] | [ç­åº¦/ææ°/è®¿é®] =>
+åä¸ï¼ä¸è¿å¯ä»¥æå®æä»ä¹é¡ºåºæ¥è¯¢ ```  # å¾çç¤ºä¾
+ç¹å»å±å¼ ## å¾çä»¬
 [https://user-images.githubusercontent.com/52584526/218328291-2324ea20-74c4-
 4182-81ed-4b74950c3ef9.png]
 [https://user-images.githubusercontent.com/52584526/218328307-f71e08ff-2370-
 4fb9-8898-c76f7e06a168.png]
 [https://user-images.githubusercontent.com/52584526/218328316-9259d9e6-6c2f-
 40e9-87bd-cee68da240e2.png]
 [https://user-images.githubusercontent.com/52584526/218328320-9ee76c53-dcf2-
@@ -113,16 +142,47 @@
 [ææ¥æ¹èå¸¸ç¨ç´ æåº](https://github.com/yuanyan3060/Arknights-Bot-
 Resource)__ - __[Kengxxiao](https://github.com/Kengxxiao)__ ç __
 [ãææ¥æ¹èãæ¸¸ææ°æ®åº](https://github.com/Kengxxiao/
 ArknightsGameData)__ - __[Aceship](https://github.com/Aceship)__ ç __
 [Arknight-Images](https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot]
 (https://github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/
 Amiya-Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __
-[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__ # æ´æ°æ¥å¿
-ç¹å»å±å¼ > 2023-02-19 v1.0.9 > - æ·»å å®æ¶ä»»å¡éç½®é¡¹ > -
+[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__ - __
+[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ ç __[MAA]
+(https://github.com/MaaAssistantArknights/MaaAssistantArknights)__ #
+æ´æ°æ¥å¿  ç¹å»å±å¼ > 2023-04-15 v1.1.0 > -
+å¬ææ¥è¯¢ãçå¹²åãçæºæéç°å¨åå¯ä»¥ç§èè¿è¡
+(ä¸æ¨èï¼ç§èåæ¶æ¯å¯è½å¯¼è´é£æ§) > -
+ç®æä¿®å¤äºä¸å¶å®åç¨ Tortoise-ORM çæä»¶åå§åå²çªçé®é¢
+[@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15) > -
+æ·»å å¨ç¾¤èæ¥è¯¢ãè®¢éãæ¨é [MAA ä½ä¸ç«](https://
+prts.plus)ä½ä¸çåè½ > -
+ä¿®å¤äºæ´æ°æ°æ®åºä¸­æå¼ è¡¨æ ¼æ¶ä¼å é¤ææè¡¨æ ¼çé®é¢ > >
+2023-04-08 v1.0.20 > -
+ä¿®å¤å ç´ æåºæ´æ°æ»åå¯¼è´æ æ³æ¥çå¹²åçé®é¢ > > 2023-04-07
+v1.0.19 > - ä¿®å¤æ´æ°æ°æ®åºå½ä»¤ä¸ä¼å¼ºå¶è¦çæ´æ°çé®é¢ > >
+2023-04-06 v1.0.18 > -
+ä¿®å¤äºèèæ´æ°æ°æ®ç»æå¯¼è´çåå»ºè¡¨åéè¯¯ > > 2023-04-04
+v1.0.17 > -
+æ·»å æ°æ®åºåå§åæ£æ¥ï¼ä¸åæ¯æ¬¡å¯å¨botæ¶éå¤åå»º > -
+æ·»å æ¯æ¬¡å¯å¨botæ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/39]
+(https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-03-28
+v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
+(å¯èªè¡å¢å æ¹æ¥) > > 2023-03-24 v1.0.14 > -
+ä¿®å¤é¿ç±³å¨ä¸è¿å«é¿ç±³å¨å²çªçé®é¢ [@zx-issue/13](https://
+github.com/NumberSir/zhenxun_arktools/issues/13) > > 2023-03-08 v1.0.12 > -
+æ·»å  rsshub ä»£çéç½®é¡¹ [@issue/34](https://github.com/NumberSir/
+nonebot_plugin_arktools/issues/34) > - ä¿®å¤å¬æå½ä»¤ä¸å¤ççé®é¢
+[@issue/35](https://github.com/NumberSir/nonebot_plugin_arktools/issues/35) > -
+æ·»å æ¹èç´ æ/èµæºè·¯å¾éç½®é¡¹ï¼ç°å¨é»è®¤å¨æºå¨äººæ ¹ç®å½ä¸
+`data/arktools` æä»¶å¤¹ [@issue/36](https://github.com/NumberSir/
+nonebot_plugin_arktools/issues/36) > -
+ä¿®å¤æ¥è¯¢æ®è½å¹²åä¿¡æ¯æ¶ä¼éä¸­ç©ºç½æ®è½çé®é¢ > > 2023-02-20
+v1.0.11 > - ä¿®å¤ææ°çæ¬æ£æµåºéçé®é¢ > > 2023-02-19 v1.0.9 > -
+æ·»å å®æ¶ä»»å¡éç½®é¡¹ > -
 ä¿®å¤å®æ¶ä»»å¡å¯¼è´å¶å®å¤çå¨é»å¡çé®é¢ [@issue/30](https://
 github.com/NumberSir/nonebot_plugin_arktools/issues/30) [@zx-issue/9](https://
 github.com/NumberSir/zhenxun_arktools/issues/9) > -
 ä¿®å¤çå¹²åæ æ³å¤æ­éå¤ççé®é¢ [@zx-issue/10](https://
 github.com/NumberSir/zhenxun_arktools/issues/10) > -
 ä¿®å¤çå¹²åç»æå¾ä¸æé¡ºåºç»å¶çé®é¢ > > 2023-02-16 v1.0.8 > -
 ç§»é¤ `nb plugin install` å®è£å½ä»¤ï¼æ æ³è¯å«ææ°çæ¬å· [@issue/
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/database/game_sqlite.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/database/game_sqlite.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     charId = fields.CharField(null=True, max_length=255, description="干员代码")
     name = fields.CharField(null=True, max_length=255, description="干员中文名")
     description = fields.CharField(null=True, max_length=1024)
     canUseGeneralPotentialItem = fields.BooleanField(null=True)
     canUseActivityPotentialItem = fields.BooleanField(null=True)
     potentialItemId = fields.CharField(null=True, max_length=255)
     activityPotentialItemId = fields.CharField(null=True, max_length=255)
+    classicPotentialItemId = fields.CharField(null=True, max_length=255)
     nationId = fields.CharField(null=True, max_length=255)
     groupId = fields.CharField(null=True, max_length=255)
     teamId = fields.CharField(null=True, max_length=255)
     displayNumber = fields.CharField(null=True, max_length=255)
     tokenKey = fields.CharField(null=True, max_length=255)
     appellation = fields.CharField(null=True, max_length=255, description="干员外文名")
     position = fields.CharField(null=True, max_length=255, description="高台/地面")
@@ -119,14 +120,35 @@
     handbookAvgList = fields.JSONField(null=True, max_length=2048)
     sex = fields.CharField(null=True, max_length=255)
 
     class Meta:
         table = "handbook_info"
 
 
+class HandbookStageModel(Model):
+    """悖论模拟"""
+    charId = fields.CharField(null=True, max_length=255)
+    stageId = fields.CharField(null=True, max_length=255)
+    levelId = fields.CharField(null=True, max_length=255)
+    zoneId = fields.CharField(null=True, max_length=255)
+    code = fields.CharField(null=True, max_length=255)
+    name = fields.CharField(null=True, max_length=255)
+    loadingPicId = fields.CharField(null=True, max_length=255)
+    description = fields.CharField(null=True, max_length=255)
+    unlockParam = fields.JSONField(null=True)
+    rewardItem = fields.JSONField(null=True)
+    stageNameForShow = fields.CharField(null=True, max_length=255)
+    zoneNameForShow = fields.CharField(null=True, max_length=255)
+    picId = fields.CharField(null=True, max_length=255)
+    stageGetTime = fields.BigIntField(null=True)
+
+    class Meta:
+        table = "handbook_stage"
+
+
 class ItemModel(Model):
     """物品"""
     itemId = fields.CharField(null=True, max_length=255)
     name = fields.CharField(null=True, max_length=255)
     description = fields.CharField(null=True, max_length=1024)
     rarity = fields.IntField(null=True)
     iconId = fields.CharField(null=True, max_length=255)
@@ -224,25 +246,106 @@
 
     dynMeta = fields.JSONField(null=True)
 
     class Meta:
         table = "gacha_pool"
 
 
+class SkinModel(Model):
+    """皮肤"""
+    skinId = fields.CharField(null=True, max_length=255, description="皮肤代码")
+    charId = fields.CharField(null=True, max_length=255, description="干员代码")
+    tokenSkinMap = fields.JSONField(null=True)
+    illustId = fields.CharField(null=True, max_length=255)
+    dynIllustId = fields.CharField(null=True, max_length=255)
+    avatarId = fields.CharField(null=True, max_length=255)
+    portraitId = fields.CharField(null=True, max_length=255)
+    dynPortraitId = fields.CharField(null=True, max_length=255)
+    dynEntranceId = fields.CharField(null=True, max_length=255)
+    buildingId = fields.CharField(null=True, max_length=255)
+    battleSkin = fields.JSONField(null=True)
+    isBuySkin = fields.BooleanField(null=True)
+    tmplId = fields.CharField(null=True, max_length=255)
+    voiceId = fields.CharField(null=True, max_length=255)
+    voiceType = fields.CharField(null=True, max_length=255)
+    displaySkin = fields.JSONField(null=True)
+
+    class Meta:
+        table = "skin"
+
+
+class StageModel(Model):
+    """关卡"""
+    stageType = fields.CharField(null=True, max_length=255)
+    difficulty = fields.CharField(null=True, max_length=255)
+    performanceStageFlag = fields.CharField(null=True, max_length=255)
+    diffGroup = fields.CharField(null=True, max_length=255)
+    unlockCondition = fields.JSONField(null=True)
+    stageId = fields.CharField(null=True, max_length=255)
+    levelId = fields.CharField(null=True, max_length=255)
+    zoneId = fields.CharField(null=True, max_length=255)
+    code = fields.CharField(null=True, max_length=255)
+    name = fields.CharField(null=True, max_length=255)
+    description = fields.CharField(null=True, max_length=255)
+    hardStagedId = fields.CharField(null=True, max_length=255)
+    dangerLevel = fields.CharField(null=True, max_length=255)
+    dangerPoint = fields.FloatField(null=True)
+    loadingPicId = fields.CharField(null=True, max_length=255)
+    canPractice = fields.BooleanField(null=True)
+    canBattleReplay = fields.BooleanField(null=True)
+    apCost = fields.IntField(null=True)
+    apFailReturn = fields.IntField(null=True)
+    etItemId = fields.CharField(null=True, max_length=255)
+    etCost = fields.IntField(null=True)
+    etFailReturn = fields.IntField(null=True)
+    etButtonStyle = fields.CharField(null=True, max_length=255)
+    apProtectTimes = fields.IntField(null=True)
+    diamondOnceDrop = fields.IntField(null=True)
+    practiceTicketCost = fields.IntField(null=True)
+    dailyStageDifficulty = fields.IntField(null=True)
+    expGain = fields.IntField(null=True)
+    goldGain = fields.IntField(null=True)
+    loseExpGain = fields.IntField(null=True)
+    loseGoldGain = fields.IntField(null=True)
+    passFavor = fields.IntField(null=True)
+    completeFavor = fields.IntField(null=True)
+    slProgress = fields.IntField(null=True)
+    displayMainItem = fields.CharField(null=True, max_length=255)
+    hilightMark = fields.BooleanField(null=True)
+    bossMark = fields.BooleanField(null=True)
+    isPredefined = fields.BooleanField(null=True)
+    isHardPredefined = fields.BooleanField(null=True)
+    isSkillSelectablePredefined = fields.BooleanField(null=True)
+    isStoryOnly = fields.BooleanField(null=True)
+    appearanceStyle = fields.IntField(null=True)
+    stageDropInfo = fields.JSONField(null=True)
+    startButtonOverrideId = fields.CharField(null=True, max_length=255)
+    isStagePatch = fields.BooleanField(null=True)
+    mainStageId = fields.CharField(null=True, max_length=255)
+
+    extra_can_use = fields.BooleanField(null=True)
+
+    class Meta:
+        table = "stage"
+
+
 GAME_SQLITE_MODEL_MODULE_NAME = __name__
 
 
 __all__ = [
     "BuildingBuffModel",
     "CharacterModel",
     "ConstanceModel",
     "EquipModel",
     "HandbookInfoModel",
+    "HandbookStageModel",
     "ItemModel",
     "RichTextStyleModel",
     "SkillModel",
     "TermDescriptionModel",
     "WorkshopFormulaModel",
     "GachaPoolModel",
+    "SkinModel",
+    "StageModel",
 
     "GAME_SQLITE_MODEL_MODULE_NAME"
 ]
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/core/models_v3.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/core/models_v3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """与tortoise-orm对接，默认数据库是已经连接好的"""
+from pathlib import Path
 from typing import Optional, List, Dict, Any
 from PIL import Image
 import re
 from tortoise.contrib.sqlite.functions import Random
 from nonebot import get_driver, logger
 
 from ..configs.path_config import PathConfig
@@ -10,21 +11,23 @@
 from ..utils import (
     prof_swap,
     sub_prof_swap,
     faction_swap
 )
 from ..exceptions import *
 
-
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
-# pcfg = PathConfig()
+gameimage_path = Path(pcfg.arknights_gameimage_path).absolute()
+gamedata_path = Path(pcfg.arknights_gamedata_path).absolute()
+
 
-##### CHARACTER #####
+"""CHARACTER"""
 class Character:
     """干员"""
+
     def __init__(self, id_: str = None, data: dict = None):
         self._id = id_
         self._data = data
 
         self._avatar = None
 
     async def init(self, id_: str, data: dict = None) -> "Character":
@@ -43,15 +46,15 @@
 
     def __str__(self):
         return f"{self.name}({self.id})"
 
     @staticmethod
     async def parse_name(name: str) -> Optional["Character"]:
         """根据名称查"""
-        data = await CharacterModel.filter(name=name)
+        data = await CharacterModel.filter(name=name).exclude(itemUsage=None)
         if not data:
             raise NamedCharacterNotExistException(details=name)
         return await Character().init(id_=data[0].charId, data=data[0].__dict__) if data else None
 
     @staticmethod
     async def random(
             useful: bool = True,
@@ -162,15 +165,15 @@
         return desc
 
     @property
     def description_plain(self) -> str:
         """特性，纯文字"""
         desc = self.description
         if "<" in desc and ">" in desc:
-            desc = re.split(r"<[@|$|/].*?>", desc)
+            desc = re.split(r"<[@$/].*?>", desc)
             desc = "".join(desc)
         if self.trait:
             desc = self.trait[0].override_description_plain or desc
         return desc
 
     @property
     def nation_id(self) -> str:
@@ -322,18 +325,20 @@
         #     await Skill().init(id_=s["skillId"], cht=self, extra_data=s)
         #     for s in self._data["skills"]
         # ] if self._data["skills"] else []
 
     @property
     def talents(self) -> List["CharacterTalent"]:
         """天赋们"""
-        return [
-            CharacterTalent(cht=self, data=d)
-            for d in self._data["talents"][0]["candidates"]
-        ]
+        results = []
+        for t in self._data["talents"]:
+            results.extend(
+                CharacterTalent(cht=self, data=d) for d in t["candidates"]
+            )
+        return results
 
     @property
     def potential_ranks(self) -> List["CharacterPotentialRank"]:
         """潜能"""
         return  # TODO
 
     @property
@@ -349,14 +354,26 @@
         """所有技能升级相关"""
         return [
             CharacterAllSkill(cht=self, data=d)
             for d in self._data["allSkillLvlup"]
         ]
 
     # 不在 arknights_character_table 中的：
+    async def get_skins(self) -> List["Skin"]:
+        """干员的所有皮肤"""
+        data = await SkinModel.filter(charId=self._id)
+        if not data:
+            return []
+
+        result = []
+        for d in data:
+            skin = await Skin().init(id_=d.__dict__["skinId"], data=d.__dict__)
+            result.append(skin)
+        return result
+
     async def get_equips(self) -> List["Equip"]:
         """干员有的模组"""
         data = await EquipModel.filter(character=self._id, uniEquipIcon__not="original")
         if not data:
             return []
 
         result = []
@@ -383,27 +400,27 @@
 
     async def get_race(self) -> str:
         """种族"""
         return (await self.get_handbook_info()).story_text_audio.race
 
     @property
     def avatar(self) -> Image:
-        return self._avatar or Image.open(pcfg.arknights_gameimage_path / "avatar" / f"{self.id}.png")
+        return self._avatar or Image.open(gameimage_path / "avatar" / f"{self.id}.png")
 
     @avatar.setter
     def avatar(self, avatar: Image):
         self._avatar = avatar
 
     @property
     def skin(self) -> Image:
         """立绘(优先精二)"""
         try:
-            return Image.open(pcfg.arknights_gameimage_path / "skin" / f"{self.id}_2b.png")
+            return Image.open(gameimage_path / "skin" / f"{self.id}_2b.png")
         except FileNotFoundError:
-            return Image.open(pcfg.arknights_gameimage_path / "skin" / f"{self.id}_1b.png")
+            return Image.open(gameimage_path / "skin" / f"{self.id}_1b.png")
 
     # 方便使用的一些判断函数
     @property
     def can_evolve_1(self) -> bool:
         """能精一"""
         return self.rarity > 1  # 三星+
 
@@ -443,18 +460,23 @@
         elif self.rarity == 4:
             tags.append("资深干员")
         elif self.rarity == 5:
             tags.append("高级资深干员")
         return tags
 
     # 猜干员小游戏用
+    async def get_drawer(self) -> str:
+        """获取画师"""
+        skins = await self.get_skins()
+        return skins[0].drawers[0] if skins else ""
 
 
 class Attributes:
     """面板"""
+
     def __init__(self, cht: Character = None, data: Dict[str, Any] = None):
         self._data = data
         self._character = cht
 
     def __str__(self):
         return (
             f"{self.character}("
@@ -584,14 +606,15 @@
     def levitate_immune(self) -> bool:
         """浮空抗性"""
         return self._data["levitateImmune"]
 
 
 class CharacterTrait:
     """特性，如领主远程降攻为80%"""
+
     def __init__(self, cht: Character, data):
         self._character = cht
         self._data = data
 
     def __str__(self):
         return f"{self.character}({self.unlock_condition.phase}-{self.unlock_condition.level}-{self.required_potential_rank})"
 
@@ -600,17 +623,17 @@
 
     @property
     def character(self) -> Character:
         """哪个干员的"""
         return self._character
 
     @property
-    def unlock_condition(self) -> "UnlockCondition":
+    def unlock_condition(self) -> "CharacterUnlockCondition":
         """解锁特性条件"""
-        return UnlockCondition(data=self._data["unlockCondition"])
+        return CharacterUnlockCondition(data=self._data["unlockCondition"])
 
     @property
     def required_potential_rank(self) -> int:
         """需要潜能等级"""
         return self._data["requiredPotentialRank"]
 
     @property
@@ -641,21 +664,22 @@
         return desc
 
     @property
     def override_description_plain(self) -> str:
         """可读"""
         desc = self._override_description_blackboard
         if "<" in desc and ">" in desc:
-            desc = re.split(r"<[@|$|/].*?>", desc)
+            desc = re.split(r"<[@$/].*?>", desc)
             desc = "".join(desc)
         return desc
 
 
 class CharacterPhase:
     """精英化阶段"""
+
     def __init__(self, cht: Character = None, data: Dict[str, Any] = None, *, level: int = -1):
         self._character = cht
         self._data = data
         self._level = level  # 标记符
 
     def __str__(self):
         return f"{self._character}(精{self.level})"
@@ -685,15 +709,17 @@
             f["level"]: Attributes(cht=await self.get_character(), data=f["data"])
             for f in self._data["attributesKeyFrames"]
         }
 
     async def get_elite_cost(self) -> List["Item"]:
         """升级到这一阶段需要材料"""
         cash = [
-            await Item().init(id_="4001", count=(await ConstanceModel.first()).__dict__["evolveGoldCost"][(await self.get_character()).rarity][self.level-1])  # 龙门币
+            await Item().init(id_="4001", count=
+            (await ConstanceModel.first()).__dict__["evolveGoldCost"][(await self.get_character()).rarity][
+                self.level - 1])  # 龙门币
         ]
         if not self._data["evolveCost"]:
             return cash
 
         result = []
         for i in self._data["evolveCost"]:
             item = await Item().init(id_=i["id"], count=i["count"])
@@ -710,20 +736,21 @@
         #         id_="4001",
         #         count=(await ConstanceModel.first()).__dict__["evolveGoldCost"][(await self.get_character()).rarity][self.level-1])  # 龙门币
         # ]
 
 
 class CharacterTalent:
     """天赋"""
+
     def __init__(self, cht: Character, data: Dict[str, Any]):
         self._character = cht
         self._data = data
 
     def __str__(self):
-        return f"{self.cht} - {self.name}"
+        return f"{self.character} - {self.name}"
 
     @property
     def character(self) -> Character:
         """哪个干员的"""
         return self._character
 
     @property
@@ -752,31 +779,32 @@
         return self.description
 
     @property
     def description_plain(self) -> str:
         """可读"""
         desc = self.description
         if "<" in desc and ">" in desc:
-            desc = re.split(r"<[@|$|/].*?>", desc)
+            desc = re.split(r"<[@$/].*?>", desc)
             desc = "".join(desc)
         return desc
 
     @property
     def range_id(self) -> str:
         """?"""
         return self._data["rangeId"] or ""
 
     @property
-    def unlock_condition(self) -> "UnlockCondition":
+    def unlock_condition(self) -> "CharacterUnlockCondition":
         """解锁条件"""
-        return UnlockCondition(data=self._data["unlockCondition"])
+        return CharacterUnlockCondition(data=self._data["unlockCondition"])
 
 
 class CharacterPotentialRank:
     """潜能"""
+
     def __init__(self, cht: Character, data: Dict[str, Any]):
         self._character = cht
         self._data = data
 
     @property
     def character(self) -> Character:
         """哪个干员的"""
@@ -801,14 +829,15 @@
     def equivalent_cost(self) -> str:
         """?"""
         return self._data["equivalentCost"] or ""
 
 
 class CharacterFavorKeyFrame:
     """好感度"""
+
     def __init__(self, cht: Character, data: Dict[str, Any], level: int = -1):
         self._character = cht
         self._data = data
         self._level = level
 
     @property
     def character(self) -> Character:
@@ -824,14 +853,15 @@
     def attributes(self) -> Attributes:
         """面板数据"""
         return Attributes(cht=self.character, data=self._data)
 
 
 class CharacterAllSkill:
     """所有技能升级(0~7)"""
+
     def __init__(self, cht: Character, data: Dict[str, Any]):
         self._character = cht
         self._data = data
 
     def __repr__(self):
         return self.__str__()
 
@@ -840,17 +870,17 @@
 
     @property
     def character(self) -> Character:
         """哪个干员的"""
         return self._character
 
     @property
-    def unlock_condition(self) -> "UnlockCondition":
+    def unlock_condition(self) -> "CharacterUnlockCondition":
         """解锁条件"""
-        return UnlockCondition(data=self._data["unlockCond"])
+        return CharacterUnlockCondition(data=self._data["unlockCond"])
 
     async def get_cost(self) -> List["Item"]:
         """升级材料"""
         result = []
         for d in self._data["lvlUpCost"]:
             item = await Item().init(id_=d["id"], count=d["count"])
             result.append(item)
@@ -859,17 +889,18 @@
 
         # return [
         #     await Item().init(id_=d["id"], count=d["count"])
         #     for d in self._data["lvlUpCost"]
         # ]
 
 
-##### HANDBOOK #####
+"""HANDBOOK"""
 class HandbookInfo:
     """档案"""
+
     def __init__(self, id_: str = None, data: Dict[str, Any] = None):
         self._id = id_
         self._data = data
 
     async def init(self, id_: str, data: dict = None) -> "HandbookInfo":
         """异步实例化"""
         self._id = id_
@@ -905,28 +936,28 @@
             data_basic=self._data["storyTextAudio"][0]["stories"][0],
             data_physic=self._data["storyTextAudio"][1]["stories"][0]
         )
 
 
 class HandbookInfoStoryTextAudio:
     """基本档案数据等"""
+
     def __init__(self, handbook_info: HandbookInfo, data_basic: Dict, data_physic: Dict):
         self._handbook_info = handbook_info
         self._data_basic = data_basic
         self._data_physic = data_physic
 
     @property
     def handbook_info(self) -> HandbookInfo:
         """哪个档案的"""
         return self._handbook_info
 
-    @property
-    def symbol(self) -> str:
+    async def get_symbol(self) -> str:
         """代号，即 character.name"""
-        return self.handbook_info.character.name
+        return (await self.handbook_info.get_character()).name
 
     @property
     def sex(self) -> str:
         """性别"""
         return re.findall(r"【[性别|设定性别]*】(.*?)\n", self._data_basic["storyText"])[0].strip()
 
     @property
@@ -951,24 +982,176 @@
 
     @property
     def height(self) -> str:
         """身高"""
         return re.findall(r"【[身高|高度]*】(.*?)\n", self._data_basic["storyText"])[0].strip()
 
 
-##### SKILL #####
+class HandbookStage:
+    """悖论模拟"""
+
+    def __init__(self, id_: str = None, data: Dict[str, Any] = None):
+        self._id = id_
+        self._data = data
+
+    async def init(self, id_: str, data: dict = None) -> "HandbookStage":
+        """异步实例化"""
+        self._id = id_
+        self._data = data
+        if not self._data:
+            data = await HandbookStageModel.filter(charId=self._id).first()
+            if not data:
+                raise  # TODO
+            self._data = data.__dict__
+        return self
+
+    def __str__(self):
+        return f"{self.id}({self.name})"
+
+    def __repr__(self):
+        return self.__str__()
+
+    @property
+    async def get_character(self) -> "Character":
+        """哪个干员的"""
+        return await Character().init(id_=self.id)
+
+    @property
+    def id(self) -> str:
+        """干员代码名"""
+        return self._id
+
+    @property
+    def stage_id(self) -> str:
+        """关卡代码名 (mem_amgoat_1)"""
+        return self._data["stageId"]
+
+    @property
+    def level_id(self) -> str:
+        """?"""
+        return self._data["levelId"]
+
+    @property
+    def zone_id(self) -> str:
+        """悖论模拟显示的地区id"""
+        return self._data["zoneId"]
+
+    @property
+    def code(self) -> str:
+        """代号 (mem_amgoat_1)"""
+        return self._data["code"]
+
+    @property
+    def name(self) -> str:
+        """悖论模拟显示的关卡名"""
+        return self._data["name"]
+
+    @property
+    def loading_pic_id(self) -> str:
+        """载入图"""
+        return self._data["loadingPicId"]
+
+    @property
+    def description(self) -> str:
+        """简介"""
+        return (self._data["description"] or "").replace("\\n", "")
+
+    @property
+    def description_raw(self) -> str:
+        """简介原文，有<>之类的特殊字符"""
+        return self.description
+
+    @property
+    def description_plain(self) -> str:
+        """简介，纯文字"""
+        desc = self.description
+        if "<" in desc and ">" in desc:
+            desc = re.split(r"<[@$/].*?>", desc)
+            desc = "".join(desc)
+        return desc
+
+    @property
+    def stage_name_for_show(self) -> str:
+        """进关卡时显示的关卡名"""
+        return self._data["stageNameForShow"]
+
+    @property
+    def zome_name_for_show(self) -> str:
+        """进关卡时显示的地区名"""
+        return self._data["zoneNameForShow"]
+
+    @property
+    def pic_id(self) -> str:
+        """?"""
+        return self._data["picId"]
+
+    @property
+    def stage_get_time(self) -> int:
+        """?"""
+        return self._data["stageGetTime"]
+
+    @property
+    def unlock_params(self) -> List["HandbookStageUnlockParam"]:
+        """解锁参数"""
+        return [
+            HandbookStageUnlockParam(self, _)
+            for _ in self._data["unlockParam"]
+        ]
+
+    @property
+    async def get_reward_items(self) -> List["Item"]:
+        """掉落物"""
+        items = []
+        for data in self._data["rewardItem"]:
+            items.append(
+                await Item().init(id_=data["id"], count=data["count"])
+            )
+        return items
+
+
+class HandbookStageUnlockParam:
+    """解锁参数"""
+    def __init__(self, handbook_stage: "HandbookStage", data: dict):
+        self._handbook_stage = handbook_stage
+        self._data = data
+
+    @property
+    def type(self) -> int:
+        """?"""
+        return self._data["unlockType"]
+
+    @property
+    def param1(self) -> str:
+        """?"""
+        return self._data["unlockParam1"]
+
+    @property
+    def param2(self) -> str:
+        """?"""
+        return self._data["unlockParam2"]
+
+    @property
+    def param3(self) -> str:
+        """?"""
+        return self._data["unlockParam3"]
+
+
+"""SKILL"""
 class Skill:
     """干员技能"""
-    def __init__(self, id_: str = None, cht: Character = None, data: Dict[str, Any] = None, extra_data: Dict[str, Any] = None):
+
+    def __init__(self, id_: str = None, cht: Character = None, data: Dict[str, Any] = None,
+                 extra_data: Dict[str, Any] = None):
         self._id = id_
         self._character = cht
         self._data = data
         self._extra_data = extra_data  # 干员的 "skills" 中的内容
 
-    async def init(self, id_: str, cht: Character = None, data: Dict[str, Any] = None, extra_data: Dict[str, Any] = None) -> "Skill":
+    async def init(self, id_: str, cht: Character = None, data: Dict[str, Any] = None,
+                   extra_data: Dict[str, Any] = None) -> "Skill":
         """异步实例化"""
         self._id = id_
         self._character = cht
         self._data = data
         self._extra_data = extra_data  # 干员的 "skills" 中的内容
         if not self._data:
             data = await SkillModel.filter(skillId=self._id).first()
@@ -998,15 +1181,15 @@
         """图标代码名"""
         return self._data["iconId"]
 
     @property
     def levels(self) -> List["SkillLevel"]:
         """七个等级的技能"""
         return [
-            SkillLevel(skill=self, data=d, level=idx+1)
+            SkillLevel(skill=self, data=d, level=idx + 1)
             for idx, d in enumerate(self._data["levels"])
         ]
 
     @property
     def name(self) -> str:
         """中文名"""
         return self._data["name"]
@@ -1048,33 +1231,34 @@
             raise NotImplementedError("未输入干员数据！")
         return [
             SkillLevelUpCondition(skill=self, data=d)
             for d in self._extra_data["levelUpCostCond"]
         ]
 
     @property
-    def unlock_condition(self) -> "UnlockCondition":
+    def unlock_condition(self) -> "CharacterUnlockCondition":
         """解锁(phase, level)"""
         if not self._extra_data:
             raise NotImplementedError("未输入干员数据！")
-        return UnlockCondition(data=self._extra_data["unlockCond"])
+        return CharacterUnlockCondition(data=self._extra_data["unlockCond"])
 
     # 不在 arknights_skill_table 中的
     @property
     def icon(self) -> Image:
         """技能图标"""
-        return Image.open(pcfg.arknights_gameimage_path / "skill" / f"skill_icon_{self.icon_id or self.id}.png")
+        return Image.open(gameimage_path / "skill" / f"skill_icon_{self.icon_id or self.id}.png")
 
     def rank(self, lvl: int = 0) -> Image:
         """专精图标"""
-        return Image.open(pcfg.arknights_gameimage_path / "ui" / "rank" / f"m-{lvl}.png")
+        return Image.open(gameimage_path / "ui" / "rank" / f"m-{lvl}.png")
 
 
 class SkillLevelUpCondition:
     """技能专精"""
+
     def __init__(self, skill: Skill, data: Dict):
         self._skill = skill
         self._data = data
 
     def __str__(self):
         return f"{self.skill}({self.get_cost} - {self.time}s)"
 
@@ -1088,17 +1272,17 @@
 
     @property
     def time(self) -> int:
         """专精耗时（秒）"""
         return self._data["lvlUpTime"]
 
     @property
-    def unlock_condition(self) -> "UnlockCondition":
+    def unlock_condition(self) -> "CharacterUnlockCondition":
         """解锁条件(phase, level)"""
-        return UnlockCondition(data=self._data["unlockCond"])
+        return CharacterUnlockCondition(data=self._data["unlockCond"])
 
     async def get_cost(self) -> List["Item"]:
         """专精耗材"""
         result = []
         for i in self._data["levelUpCost"]:
             item = await Item().init(id_=i["id"], count=i["count"])
             result.append(item)
@@ -1108,14 +1292,15 @@
         #     await Item().init(id_=i["id"], count=i["count"])
         #     for i in self._data["levelUpCost"]
         # ]
 
 
 class SkillLevel:
     """技能等级"""
+
     def __init__(self, skill: Skill, data: Dict, level: int):
         self._skill = skill
         self._data = data
         self._level = level
 
     def __str__(self):
         return f"{self.skill} - {self.name}"
@@ -1163,15 +1348,15 @@
         return desc
 
     @property
     def description_plain(self) -> str:
         """可读"""
         desc = self._description_blackboard
         if "<" in desc and ">" in desc:
-            desc = re.split(r"<[@|$|/].*?>", desc)
+            desc = re.split(r"<[@$/].*?>", desc)
             desc = "".join(desc)
         return desc
 
     @property
     def skill_type(self) -> int:
         """技能类型"""
         return self._data["skillType"]
@@ -1194,14 +1379,15 @@
     def duration(self) -> float:
         """持续时间？"""
         return self._data["duration"]
 
 
 class SkillLevelSpData:
     """技能相关数据"""
+
     def __init__(self, data: Dict[str, Any]):
         self._data = data
 
     @property
     def sp_type(self) -> int:
         """类型"""
         return self._data["spType"]
@@ -1223,15 +1409,15 @@
 
     @property
     def increment(self) -> float:
         """应该是蓝条增加速度"""
         return self._data["increment"]
 
 
-class UnlockCondition:
+class CharacterUnlockCondition:
     """解锁条件（phase, level）"""
 
     def __init__(self, data: Dict):
         self._data = data
 
     @property
     def phase(self) -> int:
@@ -1245,17 +1431,18 @@
 
     @property
     def favor(self) -> int:
         """好感度"""
         return self._data.get("favor", 0)
 
 
-##### ITEM #####
+"""ITEM"""
 class Item:
     """物品"""
+
     def __init__(self, id_: str = None, data: Dict[str, Any] = None, *, count: int = 0, weight: float = 100):
         self._id = id_
         self._count = count  # 有数量需求时填
         self._weight = weight  # 制造产物用
         self._data = data
 
     async def init(self, id_: str, data: Dict[str, Any] = None, *, count: int = 0, weight: float = 100) -> "Item":
@@ -1318,15 +1505,15 @@
         return self.description
 
     @property
     def description_plain(self) -> str:
         """可读"""
         desc = self.description
         if "<" in desc and ">" in desc:
-            desc = re.split(r"<[@|$|/].*?>", desc)
+            desc = re.split(r"<[@$/].*?>", desc)
             desc = "".join(desc)
         return desc
 
     @property
     def rarity(self) -> int:
         """稀有度"""
         return self._data["rarity"]
@@ -1377,25 +1564,26 @@
             result.append(formula)
         return result
 
         # return [
         #     await WorkshopFormula().init(id_=_["formulaId"])
         #     for _ in self._data["buildingProductList"]
         # ] if self._data["buildingProductList"] else []
-    
+
     # 不在 arknights_item_table 中的：
     @property
     def icon(self) -> Image:
         """技能图标"""
-        return Image.open(pcfg.arknights_gameimage_path / "item" / f"{self.icon_id or self.id}.png")
+        return Image.open(gameimage_path / "item" / f"{self.icon_id or self.id}.png")
 
 
-##### WORKSHOP_FORMULA #####
+"""WORKSHOP_FORMULA"""
 class WorkshopFormula:
     """制造站配方"""
+
     def __init__(self, id_: str = None, data: Dict[str, Any] = None):
         self._id = id_
         self._data = data
 
     async def init(self, id_: str, data: Dict[str, Any] = None) -> "WorkshopFormula":
         """异步实例化"""
         self._id = id_
@@ -1503,17 +1691,18 @@
 
     @property
     def require_stages(self) -> List["Stage"]:
         """TODO"""
         return
 
 
-##### EQUIP #####
+"""EQUIP"""
 class Equip:
     """模组"""
+
     def __init__(self, id_: str = None, data: Dict = None):
         self._id = id_
         self._data = data
 
     async def init(self, id_: str, data: Dict = None) -> "Equip":
         """异步实例化"""
         self._id = id_
@@ -1522,23 +1711,22 @@
             data = await EquipModel.filter(uniEquipId=self._id).first()
             if not data:
                 raise  # TODO
             self._data = data.__dict__
         return self
 
     def __str__(self):
-        return f"{self.character} - {self.name}({self.id})"
+        return f"{self.name}({self.id})"
 
     def __repr__(self):
         return self.__str__()
 
-    @property
-    def character(self) -> Character:
+    async def get_character(self) -> Character:
         """哪个干员的"""
-        return Character(id_=self._data["charId"])
+        return await Character().init(id_=self._data["charId"])
 
     @property
     def id(self) -> str:
         """代码名"""
         return self._id
 
     @property
@@ -1560,20 +1748,20 @@
     def type_icon(self) -> str:
         """类型图标名"""
         return self._data["typeIcon"]
 
     @property
     def type_name(self) -> str:
         """类型名"""
-        return f"{self._data['typeName1']}{'-' + self._data['typeName2'] if self._data['typeName2']!='None' else ''}"
+        return f"{self._data['typeName1']}{'-' + self._data['typeName2'] if self._data['typeName2'] != 'None' else ''}"
 
     @property
-    def unlock_condition(self) -> "UnlockCondition":
+    def unlock_condition(self) -> "CharacterUnlockCondition":
         """解锁条件"""
-        return UnlockCondition(
+        return CharacterUnlockCondition(
             data={
                 "phase": self._data["unlockEvolvePhase"],
                 "level": self._data["unlockLevel"],
                 "favor": self._data["unlockFavorPoint"]
             }
         )
 
@@ -1603,18 +1791,18 @@
         #         for i in d
         #     ] for idx, d in enumerate(self._data["itemCost"].values())
         # } if self._data["itemCost"] else {}
 
     # 不在 arknights_equip_table 中的:
     def rank(self, lvl: int = 0):
         """模组1,2,3级图标"""
-        return Image.open(pcfg.arknights_gameimage_path / "equip" / "stage" / f"img_stg{lvl}.png")
+        return Image.open(gameimage_path / "equip" / "stage" / f"img_stg{lvl}.png")
 
 
-##### GACHA_POOL #####
+"""GACHA_POOL"""
 class GachaPool:
     def __init__(self, id_: str = None, data: Dict = None):
         self._id = id_
         self._data = data
 
     async def init(self, id_: str, data: Dict = None) -> "GachaPool":
         """异步实例化"""
@@ -1629,14 +1817,72 @@
 
     def __str__(self):
         return f"{self.name}({self.id})({self.rule_type})"
 
     def __repr__(self):
         return self.__str__()
 
+    @staticmethod
+    async def parse_name(name: str) -> Optional["GachaPool"]:
+        """根据名称查"""
+        data = await GachaPoolModel.filter(gachaPoolName=name).first()
+        if not data:
+            raise NamedPoolNotExistException(details=name)
+        return await GachaPool().init(id_=data.gachaPoolId, data=data.__dict__) if data else None
+
+    @staticmethod
+    async def random(
+            named: bool = True,
+            rule: str = None
+    ) -> Optional["GachaPool"]:
+        """
+        随机返回池子
+        :param named: 有池子专属名字
+        :param rule: 池子类型：ATTAIN, NORMAL, LIMITED, LINKAGE
+        :return:
+        """
+        flags_ex = {}
+        flags = {}
+        if named:
+            flags_ex["gachaPoolName"] = "适合多种场合的强力干员"
+        if rule:
+            flags["gachaRuleType"] = rule if rule in {"ATTAIN", "NORMAL", "LIMITED", "LINKAGE"} else "NORMAL"
+
+        data = await GachaPoolModel.exclude(**flags_ex).filter(**flags).annotate(order=Random()).order_by("order")
+        if not data:
+            return None
+        return await GachaPool().init(id_=data[0].gachaPoolId, data=data[0].__dict__) if data else None
+
+    @staticmethod
+    async def all(
+            named: bool = True,
+            rule: str = None
+    ) -> List["GachaPool"]:
+        """
+        返回所有池子
+        :param named: 有池子专属名字
+        :param rule: 池子类型：ATTAIN, NORMAL, LIMITED, LINKAGE
+        :return:
+        """
+        flags_ex = {}
+        flags = {}
+        if named:
+            flags_ex["gachaPoolName"] = "适合多种场合的强力干员"
+        if rule:
+            flags["gachaRuleType"] = rule if rule in {"ATTAIN", "NORMAL", "LIMITED", "LINKAGE"} else "NORMAL"
+        data = await GachaPoolModel.exclude(**flags_ex).filter(**flags).all()
+        if not data:
+            return []
+
+        result = []
+        for d in data:
+            cht = await GachaPool().init(id_=d.gachaPoolId, data=d.__dict__)
+            result.append(cht)
+        return result
+
     @property
     def id(self) -> str:
         """代码名"""
         return self._data["gachaPoolId"]
 
     @property
     def index(self) -> int:
@@ -1670,14 +1916,516 @@
 
     @property
     def rule_type(self) -> str:
         """池子类型"""
         return self._data["gachaRuleType"]
 
 
+"""SKIN"""
+class Skin:
+    """皮肤"""
+
+    def __init__(self, id_: str = None, data: dict = None):
+        self._id = id_
+        self._data = data
+
+    async def init(self, id_: str, data: dict = None) -> "Skin":
+        """异步实例化"""
+        self._id = id_
+        self._data = data
+        if not self._data:
+            data = await SkinModel.filter(skinId=self._id).first()
+            if not data:
+                raise  # TODO
+            self._data = data.__dict__
+        return self
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        return f"{self.name}({self.id})"
+
+    async def get_character(self) -> "Character":
+        """哪个干员的"""
+        return await Character().init(id_=self._data["charId"])
+
+    @property
+    def id(self) -> str:
+        """皮肤代码"""
+        return self._data["skinId"]
+
+    @property
+    def illust_id(self) -> str:
+        """画师代码"""
+        return self._data["illustId"]
+
+    @property
+    def avatar_id(self) -> str:
+        """干员头图代码"""
+        return self._data["avatarId"]
+
+    @property
+    def portrait_id(self) -> str:
+        """干员半身像代码"""
+        return self._data["portraitId"]
+
+    @property
+    def building_id(self) -> str:
+        """?"""
+        return self._data["buildingId"]
+
+    @property
+    def is_buy_skin(self) -> bool:
+        """?"""
+        return self._data["isBuySkin"]
+
+    @property
+    def display_skin(self) -> "SkinDisplaySkin":
+        """显示信息"""
+        return SkinDisplaySkin(skin=self, data=self._data["displaySkin"])
+
+    # 不在 table 中的
+    @property
+    def name(self) -> str:
+        """名称"""
+        return self.display_skin.name or self.display_skin.group_name
+
+    @property
+    def description(self) -> str:
+        """介绍"""
+        return self.display_skin.description or self.display_skin.content
+
+    @property
+    def drawers(self) -> List[str]:
+        """画师们"""
+        return self.display_skin.drawers
+
+
+class SkinDisplaySkin:
+    """显示信息"""
+
+    def __init__(self, skin: "Skin", data):
+        self._skin = skin
+        self._data = data
+
+    @property
+    def skin(self) -> "Skin":
+        """哪个皮肤的"""
+        return self._skin
+
+    @property
+    def name(self) -> str:
+        """皮肤名"""
+        return self._data["skinName"]
+
+    @property
+    def drawers(self) -> List[str]:
+        """画师们"""
+        return self._data["drawerList"]
+
+    @property
+    def group_id(self) -> str:
+        """分类代码，默认为 “ILLUST_0” """
+        return self._data["skinGroupId"]
+
+    @property
+    def group_name(self) -> str:
+        """分类名，默认为 “默认服装” """
+        return self._data["skinGroupName"]
+
+    @property
+    def content(self) -> str:
+        """介绍？"""
+        return self._data["content"]
+
+    @property
+    def dialog(self) -> str:
+        """也是介绍？"""
+        return self._data["dialog"]
+
+    @property
+    def usage(self) -> str:
+        """还是介绍？"""
+        return self._data["usage"]
+
+    @property
+    def description(self) -> str:
+        """好多介绍"""
+        return self._data["description"]
+
+    @property
+    def obtain(self) -> str:
+        """获取方式"""
+        return self._data["obtainApproach"]
+
+    @property
+    def time(self) -> int:
+        """获取时间"""
+        return self._data["getTime"]
+
+
+"""STAGE"""
+class Stage:
+    """关卡"""
+
+    def __init__(self, id_: str = None, data: dict = None):
+        self._id = id_
+        self._data = data
+
+    async def init(self, id_: str, data: dict = None) -> "Stage":
+        """异步实例化"""
+        self._id = id_
+        self._data = data
+        if not self._data:
+            data = await StageModel.filter(stageId=self._id).first()
+            if not data:
+                raise  # TODO
+            self._data = data.__dict__
+        return self
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        return f"{self.name}({self.id})"
+
+    @property
+    def id(self) -> str:
+        """代码名(键值)"""
+        return self._data["stageId"]
+
+    @property
+    def name(self) -> str:
+        """中文名"""
+        return self._data["name"]
+
+    @property
+    def description(self) -> str:
+        """简介"""
+        return (self._data["description"] or "").replace("\\n", "")
+
+    @property
+    def description_raw(self) -> str:
+        """简介原文，有<>之类的特殊字符"""
+        return self.description
+
+    @property
+    def description_plain(self) -> str:
+        """简介，纯文字"""
+        desc = self.description
+        if "<" in desc and ">" in desc:
+            desc = re.split(r"<[@$/].*?>", desc)
+            desc = "".join(desc)
+        return desc
+
+    @property
+    def type(self) -> str:
+        """关卡类型(主线、活动等)"""
+        return self._data["stageType"]
+
+    @property
+    def difficulty(self) -> str:
+        """关卡难度"""
+        return self._data["difficulty"]
+
+    @property
+    def performance_stage_flag(self) -> str:
+        """?"""
+        return self._data["performanceStageFlag"]
+
+    @property
+    def difficulty_group(self) -> str:
+        """?"""
+        return self._data["diffGroup"]
+
+    @property
+    def unlock_conditions(self) -> List["StageUnlockCondition"]:
+        """解锁条件"""
+        return [
+            StageUnlockCondition(self, cond)
+            for cond in self._data["unlockCondition"]
+        ]
+
+    @property
+    def level_id(self) -> str:
+        """文件路径"""
+        return self._data["levelId"]
+    
+    @property
+    def zone_id(self) -> str:
+        """?"""
+        return self._data["zoneId"] 
+    
+    @property
+    def code(self) -> str:
+        """关卡代号 (CF-EX-8)"""
+        return self._data["code"]
+    
+    @property
+    def hard_stage_id(self) -> str:
+        """?"""
+        return self._data["hardStageId"] 
+    
+    @property
+    def danger_level(self) -> str:
+        """?"""
+        return self._data["dangerLevel"] 
+    
+    @property
+    def danger_point(self) -> float:
+        """?"""
+        return self._data["dangerPoint"] 
+    
+    @property
+    def loading_pic_id(self) -> str:
+        """加载图"""
+        return self._data["loadingPicId"]
+    
+    @property
+    def can_practice(self) -> bool:
+        """演习"""
+        return self._data["canPractice"] 
+    
+    @property
+    def can_battle_replay(self) -> bool:
+        """代理"""
+        return self._data["canBattleReplay"]
+    
+    @property
+    def ap_cost(self) -> int:
+        """消耗理智"""
+        return self._data["apCost"]
+    
+    @property
+    def ap_fail_return(self) -> int:
+        """返还理智"""
+        return self._data["apFailReturn"]
+    
+    @property
+    def ap_protect_times(self) -> int:
+        """?"""
+        return self._data["apProtextTimes"]
+    
+    @property
+    def et_item_id(self) -> str:
+        """?"""
+        return self._data["etItemId"] 
+    
+    @property
+    def et_cost(self) -> int:
+        """?"""
+        return self._data["etCost"] 
+    
+    @property
+    def et_fail_return(self) -> int:
+        """?"""
+        return self._data["etFailReturn"] 
+    
+    @property
+    def et_button_style(self) -> str:
+        """?"""
+        return self._data["etButtonStyle"]
+    
+    @property
+    def diamond_once_drop(self) -> int:
+        """源石"""
+        return self._data["diamondOnceDrop"] 
+    
+    @property
+    def practice_ticket_cost(self) -> int:
+        """消耗演习券"""
+        return self._data["practiceTicketCost"]
+    
+    @property
+    def daily_stage_difficulty(self) -> int:
+        """?"""
+        return self._data["dailyStageDifficulty"]
+    
+    @property
+    def exp_gain(self) -> int:
+        """经验"""
+        return self._data["expGain"]
+    
+    @property
+    def gold_gain(self) -> int:
+        """龙门币"""
+        return self._data["goldGain"]
+    
+    @property
+    def lose_exp_gain(self) -> int:
+        """失败经验"""
+        return self._data["loseExpGain"]
+    
+    @property
+    def lose_gold_gain(self) -> int:
+        """失败龙门币"""
+        return self._data["loseGoldGain"]
+    
+    @property
+    def pass_favor(self) -> int:
+        """?好感度"""
+        return self._data["passFavor"]
+
+    @property
+    def complete_favor(self) -> int:
+        """?好感度"""
+        return self._data["completeFavor"]
+    
+    @property
+    def sl_progress(self) -> int:
+        """?"""
+        return self._data["slProgress"] 
+    
+    @property
+    def display_main_item(self) -> str:
+        """?"""
+        return self._data["displayMainItem"] 
+    
+    @property
+    def highlight_mark(self) -> bool:
+        """?"""
+        return self._data["hilightMark"]
+
+    @property
+    def boss_mark(self) -> bool:
+        """是否 boss 关"""
+        return self._data["bossMark"]
+
+    @property
+    def is_predefined(self) -> bool:
+        """?固定阵容"""
+        return self._data["isPredefined"]
+
+    @property
+    def is_hard_predefined(self) -> bool:
+        """?"""
+        return self._data["isHardPredefined"]
+
+    @property
+    def is_skill_selectable_predefined(self) -> bool:
+        """?固定技能"""
+        return self._data["isSkillSelectablePredefined"]
+
+    @property
+    def is_story_only(self) -> bool:
+        """?过视频"""
+        return self._data["isStoryOnly"]
+
+    @property
+    def appearance_style(self) -> int:
+        """?"""
+        return self._data["appearanceStyle"]
+
+    @property
+    def stage_drop_info(self) -> "StageDropInfo":
+        """掉落信息"""
+        return StageDropInfo(self, self._data["stageDropInfo"])
+
+    @property
+    def start_button_override_id(self) -> str:
+        """?"""
+        return self._data["startButtonOverrideId"]
+
+    @property
+    def is_stage_patch(self) -> bool:
+        """?"""
+        return self._data["isStagePatch"]
+
+    @property
+    def main_stage_id(self) -> str:
+        """?"""
+        return self._data["mainStageId"]
+
+
+class StageUnlockCondition:
+    """解锁条件（stageId, completeState）"""
+
+    def __init__(self, stage: "Stage", data: Dict):
+        self._stage = stage
+        self._data = data
+
+    @property
+    def stage(self) -> "Stage":
+        """哪个关卡的"""
+        return self._stage
+        
+    @property
+    def id(self) -> str:
+        """关卡代码"""
+        return self._data["stageId"]
+    
+    @property
+    def state(self) -> int:
+        """几星完成"""
+        return self._data["completeState"]
+
+
+class StageDropInfo:
+    """掉落信息"""
+
+    def __init__(self, stage: "Stage", data: dict):
+        self._stage = stage
+        self._data = data
+
+    @property
+    def stage(self) -> "Stage":
+        """哪个关卡的"""
+        return self._stage
+
+    @property
+    def first_pass_rewards(self):
+        """TODO, 现在全是 null"""
+        return
+
+    @property
+    def first_complete_rewards(self):
+        """TODO, 现在全是 null"""
+        return
+
+    @property
+    def pass_rewards(self):
+        """TODO, 现在全是 null"""
+        return
+
+    @property
+    def complete_rewards(self):
+        """TODO, 现在全是 null"""
+        return
+
+    @property
+    async def get_display_rewards(self) -> List["Item"]:
+        """?掉落"""
+        items = []
+        for data in self._data["displayRewards"]:
+            items.append(
+                await Item().init(id_=data["id"])
+            )
+        return items
+
+    @property
+    async def get_display_detail_rewards(self):
+        """?掉落"""
+        items = []
+        for data in self._data["displayDetailRewards"]:
+            items.append(
+                await Item().init(id_=data["id"])
+            )
+        return items
+
+
+"""TODO"""
+class Room: ...
+class Mission: ...
+
+
 __all__ = [
     "Character",
+    "HandbookInfo",
+    "HandbookStage",
     "Skill",
     "Item",
     "Equip",
-    "GachaPool"
-]
+    "GachaPool",
+    "Skin",
+    "Stage"
+]
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/exceptions/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/exceptions/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,10 +17,32 @@
 
 class NamedCharacterNotExistException(ArkBaseException):
     """这个名字的干员不存在"""
     def __init__(self, msg: str = "干员不存在！", details: str = ""):
         super().__init__(msg, details)
 
 
+class NamedPoolNotExistException(ArkBaseException):
+    """这个名字的池子不存在"""
+    def __init__(self, msg: str = "卡池不存在！", details: str = ""):
+        super().__init__(msg, details)
+
+
+class MAAFailedResponseException(ArkBaseException):
+    """响应错误"""
+    def __init__(self, msg: str = "作业站响应错误！", details: str = ""):
+        super().__init__(msg, details)
+
+
+class MAANoResultException(ArkBaseException):
+    """没有作业"""
+    def __init__(self, msg: str = "没有查询到结果！", details: str = ""):
+        super().__init__(msg, details)
+
+
 __all__ = [
-    "NamedCharacterNotExistException"
+    "NamedCharacterNotExistException",
+    "NamedPoolNotExistException",
+
+    "MAAFailedResponseException",
+    "MAANoResultException"
 ]
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/game_guess_operator/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 from nonebot import on_shell_command, on_command, on_message
 from nonebot.plugin import PluginMetadata
 from nonebot.params import ShellCommandArgv, CommandArg, EventPlainText
 from nonebot.exception import ParserExit
 from nonebot.rule import Rule, ArgumentParser, to_me
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
-from nonebot.adapters.onebot.v11 import Message, GroupMessageEvent, MessageSegment
+from nonebot.adapters.onebot.v11 import Message, MessageEvent, MessageSegment, GroupMessageEvent
 
 import asyncio
 import shlex
 from typing import List, Dict, Optional
 from io import BytesIO
 from dataclasses import dataclass
 from asyncio import TimerHandle
 
 
 from .data_source import *
 from ..core.models_v3 import Character
+from ..utils.general import nickname_swap
 
 
 GAMES: Dict[str, GuessCharacter] = {}  # 记录游戏数据
 TIMERS: Dict[str, TimerHandle] = {}  # 计时
 
 
 @dataclass
@@ -35,20 +36,20 @@
 parser.add_argument("--hint", action="store_true", help="提示")
 parser.add_argument("--stop", action="store_true", help="结束游戏")
 parser.add_argument("cht_name", nargs="?", help="干员名")
 
 
 arkguess = on_shell_command("猜干员", parser=parser)
 @arkguess.handle()
-async def _(matcher: Matcher, event: GroupMessageEvent, argv: List[str] = ShellCommandArgv()):
+async def _(matcher: Matcher, event: MessageEvent, argv: List[str] = ShellCommandArgv()):
     """开始游戏"""
     await handle_arkguess(matcher, event, argv)
 
 
-async def handle_arkguess(matcher: Matcher, event: GroupMessageEvent, argv: List[str]):
+async def handle_arkguess(matcher: Matcher, event: MessageEvent, argv: List[str]):
     async def send(message: Optional[str] = None, image: Optional[BytesIO] = None):
         if not (message or image):
             await matcher.finish()
         msg_ = Message()
         if image:
             msg_.append(MessageSegment.image(image))
         if message:
@@ -59,15 +60,15 @@
         args = parser.parse_args(argv)
     except ParserExit as e:
         if e.status == 0:
             await send("小笨蛋，命令输错了哦！")
         await send()
 
     options = Options(**vars(args))
-    cid = f"group_{event.group_id}"
+    cid = f"group_{event.group_id}" if isinstance(event, GroupMessageEvent) else f"group_{event.user_id}"
     if not GAMES.get(cid):
         if options.cht_name or options.stop or options.hint:
             await matcher.finish("小笨蛋，没有正在进行的游戏哦！")
 
         character = await get_random_character()
         game = GuessCharacter(cht=character)
         GAMES[cid] = game
@@ -86,14 +87,15 @@
     game = GAMES[cid]
     set_timeout(matcher, cid)
 
     # 提示
     if options.hint:
         await send(message=await game.get_hint())
 
+    options.cht_name = await nickname_swap(options.cht_name)
     cht = await Character.parse_name(options.cht_name)
     result = await game.guess(cht)
     if result in [GuessResult.WIN, GuessResult.LOSE]:
         GAMES.pop(cid)
         await send(
             (
                 "恭喜你猜出了干员！"
@@ -136,25 +138,25 @@
 
 def shortcut(cmd: str, argv: List[str] = None, **kwargs):
     if not argv:
         argv = []
     command = on_command(cmd, **kwargs)
 
     @command.handle()
-    async def _(matcher: Matcher, event: GroupMessageEvent, msg: Message = CommandArg()):
+    async def _(matcher: Matcher, event: MessageEvent, msg: Message = CommandArg()):
         try:
             args = shlex.split(msg.extract_plain_text().strip())
         except Exception as e:
             args = []
         await handle_arkguess(matcher, event, argv + args)
 
 
-def is_game_running(event: GroupMessageEvent) -> bool:
+def is_game_running(event: MessageEvent) -> bool:
     """判断游戏运行"""
-    return bool(GAMES.get(f"group_{event.group_id}"))
+    return bool(GAMES.get(f"group_{event.group_id}")) if isinstance(event, GroupMessageEvent) else bool(GAMES.get(f"group_{event.user_id}"))
 
 
 def get_word_input(state: T_State, msg: str = EventPlainText()) -> bool:
     """获取输入干员"""
     if msg.startswith("#"):
         state["cht_name"] = msg[1:]
         return True
@@ -164,15 +166,15 @@
 shortcut("猜干员", [], rule=to_me())
 shortcut("提示", ["--hint"], rule=is_game_running)
 shortcut("结束", ["--stop"], rule=is_game_running)
 
 
 word_matcher = on_message(Rule(is_game_running) & get_word_input)
 @word_matcher.handle()
-async def _(matcher: Matcher, event: GroupMessageEvent, state: T_State):
+async def _(matcher: Matcher, event: MessageEvent, state: T_State):
     cht_name: str = state["cht_name"]
     await handle_arkguess(matcher, event, [cht_name])
 
 
 __plugin_meta__ = PluginMetadata(
     name="猜干员",
     description="与wordle玩法相同，猜明日方舟干员",
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/game_guess_operator/data_source.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/game_guess_operator/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from pathlib import Path
+
 from ..core.models_v3 import Character
 from ..configs.path_config import PathConfig
 
 from nonebot import get_driver
 
 from typing import List, Set
 from enum import Enum
 from PIL import Image, ImageFont
 from PIL.ImageDraw import Draw
 from io import BytesIO
 
 
 driver = get_driver()
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
-GUESS_IMG_PATH = pcfg.arknights_data_path / "guess_character"
+data_path = Path(pcfg.arknights_data_path).absolute()
+font_path = Path(pcfg.arknights_font_path).absolute()
+GUESS_IMG_PATH = data_path / "guess_character"
 
 
 async def get_all_characters() -> List["Character"]:
     """所有干员"""
     return await Character.all()
 
 
@@ -38,15 +42,15 @@
         self._times: int = 8  # 能猜的次数
         self._guessed: List["Character"] = []  # 猜过的
 
         self._block_size = (40, 40)  # 表情块尺寸
         self._block_padding = (10, 10)  # 表情块之间间距
         self._padding = (20, 20)  # 边界间距
         self._font_size = 32  # 字体大小
-        self._font = ImageFont.truetype((pcfg.arknights_font_path / "Arknights-zh.otf").__str__(), self._font_size)
+        self._font = ImageFont.truetype((font_path / "Arknights-zh.otf").__str__(), self._font_size)
         self._bg_color = (255, 255, 255)  # 背景颜色
 
         self._correct_face = Image.open(GUESS_IMG_PATH / "correct.png", "r").convert("RGBA")  # 完全一致
         self._vague_face = Image.open(GUESS_IMG_PATH / "vague.png", "r").convert("RGBA")  # 职业 / 阵营部分一致 / 答案高台地面均可放，猜高台或地面
         self._wrong_face = Image.open(GUESS_IMG_PATH / "wrong.png", "r").convert("RGBA")  # 完全不同
         self._up_face = Image.open(GUESS_IMG_PATH / "up.png", "r").convert("RGBA")  # 低于目标星级
         self._down_face = Image.open(GUESS_IMG_PATH / "down.png", "r").convert("RGBA")  # 高于目标星级
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/help.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """帮助"""
 from .game_guess_operator import __plugin_meta__ as GUESS_META
 from .misc_operator_birthday import __plugin_meta__ as BIRTHDAY_META
 from .misc_monster_siren import __plugin_meta__ as SIREN_META
 from .tool_announce_push import __plugin_meta__ as ANNOUNCE_META
+from .tool_fetch_maa_copilot import __plugin_meta__ as MAA_META
 from .tool_operator_info import __plugin_meta__ as INFO_META
 from .tool_open_recruitment import __plugin_meta__ as RECRUIT_META
 from .tool_sanity_notify import __plugin_meta__ as SAN_META
 from .utils import __plugin_meta__ as UTILS_META
 
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageSegment
@@ -15,14 +16,15 @@
 
 
 HELP_DATAS = [
     GUESS_META,
     BIRTHDAY_META,
     SIREN_META,
     ANNOUNCE_META,
+    MAA_META,
     INFO_META,
     RECRUIT_META,
     SAN_META,
     UTILS_META
 ]
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_monster_siren/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """干员生日提醒"""
+from pathlib import Path
+
 from nonebot import on_command, get_driver, logger
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import MessageSegment, Message
 from typing import List
 from datetime import datetime
 from PIL import Image, ImageFont
 from PIL.ImageDraw import Draw
@@ -10,14 +12,15 @@
 
 from ..core.models_v3 import Character
 from ..utils import text_border
 from ..configs.path_config import PathConfig
 
 
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
+font_path = Path(pcfg.arknights_font_path).absolute()
 
 
 today_birthday = on_command("今日干员")
 
 
 @today_birthday.handle()
 async def _():
@@ -39,15 +42,15 @@
             cht_bg.paste(im=icon, box=(0, 0), mask=icon.split()[3])
             text_border(
                 cht.name,
                 Draw(cht_bg),
                 x=64,
                 y=(128 + 12 + 152 * (idx // 6)),
                 anchor="mm",
-                font=ImageFont.truetype((pcfg.arknights_font_path / "Arknights-zh.otf").__str__(), 20),
+                font=ImageFont.truetype((font_path / "Arknights-zh.otf").__str__(), 20),
                 fill_colour=(255, 255, 255, 255),
                 shadow_colour=(0, 0, 0, 255)
             )
             main_background.paste(cht_bg, (24+idx*(128+16), 24), mask=cht_bg.split()[3])
     except FileNotFoundError as e:
         logger.error("干员信息缺失，请使用 “更新方舟素材” 命令更新游戏素材后重试")
         await today_birthday.finish("干员信息缺失，请使用 “更新方舟素材” 命令更新游戏素材后重试")
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_announce_push/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_announce_push/data_source.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_announce_push/data_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import feedparser
 from typing import Optional, List
 from nonebot import get_driver
 from datetime import datetime
 
-from ..configs import PathConfig
+from ..configs import PathConfig, ProxyConfig
 from ..core.database import RSSNewsModel
 
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
+xcfg = ProxyConfig.parse_obj(get_driver().config.dict())
 
 
 async def get_news() -> Optional[List["RSSNewsModel"]]:
     """游戏公告/新闻"""
-    url = "https://rsshub.app/arknights/news?filterout_title=封禁&limit=3"
+    url = f"{xcfg.rss_site}/arknights/news?filterout_title=封禁&limit=3"
     rss_data = feedparser.parse(url)
     if not rss_data or rss_data["status"] != 200:
         raise  # TODO
     if not rss_data["entries"]:
         return None
 
     latest_news = []
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """公招筛选"""
 import httpx
 from nonebot import on_command, logger
 from nonebot.plugin import PluginMetadata
-from nonebot.params import Arg, CommandStart
+from nonebot.params import Arg, RawCommand
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot.exception import ActionFailed
-from nonebot.adapters.onebot.v11 import Message, MessageSegment, GroupMessageEvent
+from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
 
 from typing import Union
 
-from .data_source import DrawRecruitmentCard, process_word_tags, baidu_ocr
+from .data_source import BuildRecruitmentCard, process_word_tags, baidu_ocr
 
 
-recruit = on_command("公招", aliases={"公开招募", "方舟公招"})
+recruit = on_command("公招", aliases={"公开招募"})
 
 
 @recruit.handle()
-async def _(state: T_State, event: GroupMessageEvent, matcher: Matcher, start: str = CommandStart()):
+async def _(state: T_State, event: MessageEvent, matcher: Matcher, raw: str = RawCommand()):
     if event.reply:
         event.message = event.reply.message
 
     if event.message.get("image", None):  # 自带图片
         logger.debug("发送公招截图")
         for img in event.message["image"]:
             img_url = img.data.get("url", "")
             state["recruit"] = "image"
             matcher.set_arg("rec", img_url)
 
-    elif event.message.extract_plain_text().replace("公招", "").replace(start, "").strip():  # 文字tag
-        tags = event.message.extract_plain_text().replace("公招", "").replace(start, "").strip()
+    elif event.message.extract_plain_text().replace(raw, "").strip():  # 文字tag
+        tags = event.message.extract_plain_text().replace(raw, "").strip()
         logger.debug("直接输入文字标签")
         state["recruit"] = "str"
         matcher.set_arg("rec", tags)
 
 
 @recruit.got(key="rec", prompt="请发送公招截图:")
 async def _(state: T_State, rec: Union[Message, str] = Arg()):
@@ -56,22 +56,22 @@
         await recruit.finish("百度OCR出错，请检查运行日志！", at_sender=True)
     if not tags:
         await recruit.finish("没有检测到符合要求的公招标签！", at_sender=True)
     logger.debug(f"tags: {tags}")
     await recruit.send(f"检测到的公招标签：{', '.join(list(tags))}")
 
     try:
-        recruit_list = await DrawRecruitmentCard.build_target_characters(tags)
+        recruit_list = await BuildRecruitmentCard.build_target_characters(tags)
     except FileNotFoundError as e:
         logger.error("干员信息缺失，请使用 “更新方舟素材” 命令更新游戏素材后重试")
         await recruit.finish("干员信息缺失，请使用 “更新方舟素材” 命令更新游戏素材后重试")
 
     if not recruit_list:
         await recruit.finish("没有必出稀有干员的标签组合哦！", at_sender=True)
-    draw = DrawRecruitmentCard(recruit_list)
+    draw = BuildRecruitmentCard(recruit_list)
     image = draw.build_main()
     img = MessageSegment.image(image)
     try:
         await recruit.finish(Message(img))
     except ActionFailed as e:
         await recruit.finish(f"图片发送失败：{e}")
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 import httpx
 from aiofiles import open as aopen
 import json
 from typing import Set, List, Tuple, Dict, Any, Union
 from PIL import Image, ImageFont
 from PIL.ImageDraw import Draw
 from itertools import permutations
@@ -12,14 +14,16 @@
 
 from ..core.models_v3 import Character
 from ..configs import BaiduOCRConfig, PathConfig
 from ..utils import text_border, get_recruitment_available
 
 bconfig = BaiduOCRConfig.parse_obj(get_driver().config.dict())
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
+font_path = Path(pcfg.arknights_font_path).absolute()
+gamedata_path = Path(pcfg.arknights_gamedata_path).absolute()
 
 
 async def baidu_ocr(image_url: str, client: httpx.AsyncClient) -> Set[str]:
     """百度ocr"""
     access_token = await get_baidu_ocr_access_token(client)
 
     url = f"https://aip.baidubce.com/rest/2.0/ocr/v1/accurate_basic?access_token={access_token}"
@@ -30,15 +34,15 @@
     try:
         all_words = {_["words"] for _ in response.json()["words_result"]}
     except KeyError as e:
         logger.error("百度ocr识别失败:")
         logger.error(f"{response.json()}")
         return None
 
-    async with aopen(pcfg.arknights_gamedata_path / "excel" / "gacha_table.json", "r", encoding="utf-8") as fp:
+    async with aopen(gamedata_path / "excel" / "gacha_table.json", "r", encoding="utf-8") as fp:
         tags = {_["tagName"] for _ in json.loads(await fp.read())["gachaTags"]}
 
     return {_ for _ in all_words if _ in tags}
 
 
 async def get_baidu_ocr_access_token(client: httpx.AsyncClient) -> str:
     """百度ocr获取token"""
@@ -76,20 +80,20 @@
             tag = tag.replace("术士", "术师")
 
         if tag in {"近卫", "狙击", "重装", "医疗", "辅助", "术师", "特种", "先锋", "男性", "女性"}:
             tags[idx] = f"{tags[idx]}干员"
     return tags
 
 
-class DrawRecruitmentCard:
+class BuildRecruitmentCard:
     """绘图"""
     def __init__(self, result_groups: List[Dict[str, Any]]):
         self.result_groups = result_groups
-        self.font_norm = ImageFont.truetype(str(pcfg.arknights_font_path / "Arknights-zh.otf"), 24)
-        self.font_small = ImageFont.truetype(str(pcfg.arknights_font_path / "Arknights-zh.otf"), 20)
+        self.font_norm = ImageFont.truetype(str(font_path / "Arknights-zh.otf"), 24)
+        self.font_small = ImageFont.truetype(str(font_path / "Arknights-zh.otf"), 20)
 
         self.result_images: List[Tuple[Image, int]] = []
 
     def build_group(self, result_group: Dict[str, Any]):
         """每一个组合绘制"""
         tags: List[str] = result_group["tags"]
         chts: List[Character] = result_group["chts"]
@@ -226,15 +230,15 @@
             result += list(permutations(tags, i))
         return set(result)
 
     @staticmethod
     async def build_target_characters(tags: set) -> List[Dict[str, Union[str, List[Character]]]]:
         """tag-干员组合"""
         chts = [(await Character().init(_)) for _ in await get_recruitment_available()]  # 所有可公招的干员
-        combs = DrawRecruitmentCard.build_combinations(tags)  # 所有可能的tag组合
+        combs = BuildRecruitmentCard.build_combinations(tags)  # 所有可能的tag组合
         cht_tags = {  # 这一条提出来，省了1k倍速度
             _.name: await _.get_tags_for_open_recruitment()
             for _ in chts
         }
 
         result = []
         for comb in combs:
@@ -255,11 +259,11 @@
             flag = all(cht.rarity not in {1, 2} for cht in r["chts"])
             if flag:
                 result_.append(r)
         return result_
 
 
 __all__ = [
-    "DrawRecruitmentCard",
+    "BuildRecruitmentCard",
     "process_word_tags",
     "baidu_ocr"
 ]
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_operator_info/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 from nonebot.plugin import PluginMetadata
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 
 from .data_source import BuildOperatorInfo
 from ..core.models_v3 import Character
 from ..exceptions import *
+from ..utils.general import nickname_swap
 
 operator_info = on_command("方舟干员", aliases={"干员"})
 
 
 @operator_info.handle()
 async def _(arg: Message = CommandArg()):
     name = arg.extract_plain_text().strip()
     if not name:
         await operator_info.finish()
 
     try:
+        name = await nickname_swap(name)
         cht = await Character.parse_name(name)
     except NamedCharacterNotExistException as e:
         await operator_info.finish(e.msg, at_sender=True)
 
     try:
         img_bytes = await BuildOperatorInfo(cht=cht).build_whole_image()
     except FileNotFoundError as e:
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_operator_info/data_source.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_operator_info/data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,23 @@
 from ..utils.image import text_border
 from ..configs.path_config import PathConfig
 
 from nonebot import get_driver
 
 
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
+font_path = Path(pcfg.arknights_font_path).absolute()
+gameimage_path = Path(pcfg.arknights_gameimage_path).absolute()
+gamedata_path = Path(pcfg.arknights_gamedata_path).absolute()
 # pcfg = PathConfig()
 
 
 class BuildOperatorInfo:
     """作图"""
-    def __init__(self, cht: Character, font_en: Union[str, Path] = pcfg.arknights_font_path / "Arknights-en.ttf", font_zh: Union[str, Path] = pcfg.arknights_font_path / "Arknights-zh.otf"):
+    def __init__(self, cht: Character, font_en: Union[str, Path] = font_path / "Arknights-en.ttf", font_zh: Union[str, Path] = font_path / "Arknights-zh.otf"):
         self._operator = cht
         self._font_en = font_en if isinstance(font_en, str) else font_en.__str__()
         self._font_zh = font_zh if isinstance(font_zh, str) else font_zh.__str__()
 
     @property
     def character(self) -> Character:
         return self._operator
@@ -72,15 +75,15 @@
         img_head_shadow = Image.new(mode="RGBA", size=(1056, 24), color=(175, 175, 175, 200))  # 顶部阴影
         main_background.paste(im=img_head_shadow, box=(0, 0), mask=img_head_shadow.split()[3])
 
         backgrounds = []
         for lvl, all_skills in enumerate(self.character.all_skill_level_up):
             background = Image.new(mode="RGBA", size=(352, 96), color=(235, 235, 235, 160))  # 底图
             icon_box = Image.new(mode="RGBA", size=(96, 96), color=(205, 205, 205, 200))  # 左侧阴影
-            rank_icon = Image.open(pcfg.arknights_gameimage_path / "ui" / "rank" / f"{lvl+1}.png").convert("RGBA").resize((96, 96))
+            rank_icon = Image.open(gameimage_path / "ui" / "rank" / f"{lvl+1}.png").convert("RGBA").resize((96, 96))
             icon_box.paste(rank_icon, mask=rank_icon.split()[3])
             background.paste(im=icon_box, box=(0, 0), mask=icon_box.split()[3])
             # text_border(text=f"{lvl}~{lvl + 1}", draw=Draw(background), x=48, y=60, font=font_en, shadow_colour=(0, 0, 0, 255), fill_colour=(255, 255, 255, 255))  # 顶部文字
             for idx, cost_item in enumerate(await all_skills.get_cost()):
                 icon = self.resize(cost_item.icon, 64)  # 材料图标大小
                 text_border(text=str(cost_item.count), draw=Draw(icon), x=45, y=57, font=font_en, shadow_colour=(255, 255, 255, 255), fill_colour=(0, 0, 0, 255))  # 右下角的数字
                 background.paste(im=icon, box=(112 + idx*80, 16), mask=icon.split()[3])  # 透明度粘贴(r,g,b,a)
@@ -127,17 +130,20 @@
         img_head_shadow = Image.new(mode="RGBA", size=(704, 24), color=(175, 175, 175, 200))  # 顶部阴影
         main_background.paste(im=img_head_shadow, box=(0, 0), mask=img_head_shadow.split()[3])
 
         main_backgrounds = []
         for equip in await self.character.get_equips():
             equip_main_backgrounds = Image.new(mode="RGBA", size=(352, 384), color=(235, 235, 235, 160))  # 每个模组的底图
             if equip.type_icon == "original":
-                equip_icon = Image.open(pcfg.arknights_gameimage_path / "equip" / "icon" / "default.png").convert("RGBA").resize((96, 96))
+                equip_icon = Image.open(gameimage_path / "equip" / "icon" / "default.png").convert("RGBA").resize((96, 96))
             else:
-                equip_icon = Image.open(pcfg.arknights_gameimage_path / "equip" / "icon" / f"{equip.icon_id}.png").convert("RGBA").resize((96, 96))
+                try:
+                    equip_icon = Image.open(gameimage_path / "equip" / "icon" / f"{equip.icon_id}.png").convert("RGBA").resize((96, 96))
+                except FileNotFoundError as e:
+                    equip_icon = Image.new(mode="RGBA", size=(96, 96), color=(0, 0, 0, 0))
             icon_shadow = Image.new(mode="RGBA", size=(96, 96), color=(205, 205, 205, 200))  # 左侧阴影
             icon_shadow.paste(im=equip_icon, box=(0, 0), mask=equip_icon.split()[3])
             equip_main_backgrounds.paste(im=icon_shadow, box=(0, 0), mask=icon_shadow.split()[3])
             text_border(text=equip.name, draw=Draw(equip_main_backgrounds), x=224, y=60, font=font_zh, shadow_colour=(0, 0, 0, 255), fill_colour=(255, 255, 255, 255))
 
             backgrounds = []
             for idx, items in (await equip.get_item_cost()).items():
@@ -207,22 +213,18 @@
         backgrounds = []
         for lvl, phase in enumerate(phases):
             if lvl == 0:
                 continue
             background = Image.new(mode="RGBA", size=(432, 96), color=(235, 235, 235, 160))  # 底图
             icon_box = Image.new(mode="RGBA", size=(96, 96), color=(205, 205, 205, 200))  # 左侧阴影
             background.paste(im=icon_box, box=(0, 0), mask=icon_box.split()[3])
-            level_icon = Image.open(pcfg.arknights_gameimage_path / "ui" / "elite" / f"{lvl}.png", mode="r").convert("RGBA")
-            if lvl == 1:
+            level_icon = Image.open(gameimage_path / "ui" / "elite" / f"{lvl}.png", mode="r").convert("RGBA")
+            if lvl in [1, 2]:
                 level_icon = level_icon.resize(size=(96, 93))
                 background.paste(im=level_icon, box=(0, 0), mask=level_icon.split()[3])
-            elif lvl == 2:
-                level_icon = level_icon.resize(size=(96, 93))
-                background.paste(im=level_icon, box=(0, 0), mask=level_icon.split()[3])
-
             costs = await phase.get_elite_cost()
             item_count = 0
             for cost_item in costs:
                 icon = cost_item.icon.resize(size=(64, 64))  # 材料图标大小
                 count = cost_item.count
                 if count >= 10000:
                     count = f"{count / 10000:.0f}w"
@@ -334,14 +336,18 @@
         Draw(bg).text(xy=(528, 216), anchor="ms", align="center", text="该干员无技能专精", font=font_zh, fill=(255, 255, 255, 255))
         return bg
 
     async def _build_skin(self) -> Image:
         """立绘"""
         return self.character.skin.convert(mode="RGBA").resize((1176, 1176))
 
+    async def _build_talent(self) -> Image:
+        """天赋"""
+        ...
+
     @staticmethod
     def resize(img: Image, size: int):
         w, h = img.size
         img = img.resize((int(w*size/h), size)) if w >= h else img.resize((size, int(h*size/h)))
         return img
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """理智恢复提醒"""
 from datetime import datetime
 
 import tortoise.exceptions
 from nonebot import on_command, get_bot, logger, get_driver
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, Message, Bot, MessageSegment
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageEvent, Message, Bot, MessageSegment
 from nonebot.params import CommandArg
 from nonebot.plugin import PluginMetadata
 from nonebot_plugin_apscheduler import scheduler
 
 from ..configs.scheduler_config import SchedulerConfig
 from ..core.database import UserSanityModel
 
 scfg = SchedulerConfig.parse_obj(get_driver().config.dict())
 
 add_notify = on_command("理智提醒", aliases={"ADDSAN"})
 check_notify = on_command("理智查看", aliases={"CHECKSAN"})
 
 
 @add_notify.handle()
-async def _(event: GroupMessageEvent, args: Message = CommandArg()):
+async def _(event: MessageEvent, args: Message = CommandArg()):
     args = args.extract_plain_text().strip().split()
     uid = event.user_id
-    gid = event.group_id
+    gid = event.group_id if isinstance(event, GroupMessageEvent) else 0
     now = datetime.now()
 
     if not args:
         notify_time = datetime.fromtimestamp(now.timestamp() + 135 * 360, tz=now.tzinfo)
         data = await UserSanityModel.filter(gid=gid, uid=uid).first()
         if not data:
             await UserSanityModel.create(
@@ -47,28 +47,27 @@
             )
         else:
             await UserSanityModel.filter(gid=gid, uid=uid).update(
                 record_san=record_san, notify_san=notify_san,
                 record_time=now, notify_time=notify_time, status=1
             )
     else:
-        await add_notify.finish("小笨蛋，命令的格式是：“理智提醒 [当前理智] [回满理智]” 或 “理智提醒” 哦！",
-                                at_sender=True)
+        await add_notify.finish("小笨蛋，命令的格式是：“理智提醒 [当前理智] [回满理智]” 或 “理智提醒” 哦！")
 
-    await add_notify.finish(f"记录成功！将在 {notify_time.__str__()[:-7]} 提醒博士哦！", at_sender=True)
+    await add_notify.finish(f"记录成功！将在 {notify_time.__str__()[:-7]} 提醒博士哦！")
 
 
 @check_notify.handle()
-async def _(event: GroupMessageEvent):
+async def _(event: MessageEvent):
     uid = event.user_id
-    gid = event.group_id
+    gid = event.group_id if isinstance(event, GroupMessageEvent) else 0
 
     data = await UserSanityModel.filter(gid=gid, uid=uid, status=1).first()
     if not data:
-        await check_notify.finish("小笨蛋，你还没有记录过理智提醒哦！", at_sender=True)
+        await check_notify.finish("小笨蛋，你还没有记录过理智提醒哦！")
 
     data = data.__dict__
 
     record_time: datetime = data["record_time"]
     notify_time: datetime = data["notify_time"]
     now = datetime.now(tz=record_time.tzinfo)
 
@@ -97,24 +96,30 @@
             try:
                 data = await UserSanityModel.filter(notify_time__lt=now, status=1).all()
             except tortoise.exceptions.BaseORMException:
                 logger.error("检查理智提醒失败，数据库未初始化")
             else:
                 if data:
                     for model in data:
-                        await bot.send_group_msg(
-                            group_id=model.gid,
-                            message=Message(MessageSegment.at(model.uid) + f"你的理智已经恢复到{model.notify_san}了哦！")
-                        )
+                        if model.gid:
+                            await bot.send_group_msg(
+                                group_id=model.gid,
+                                message=Message(MessageSegment.at(model.uid) + f"你的理智已经恢复到{model.notify_san}了哦！")
+                            )
+                        else:
+                            await bot.send_private_msg(
+                                user_id=model.uid,
+                                message=Message(MessageSegment.at(model.uid) + f"你的理智已经恢复到{model.notify_san}了哦！")
+                            )
                         await UserSanityModel.filter(gid=model.gid, uid=model.uid).update(status=0)
 
 
 __plugin_meta__ = PluginMetadata(
     name="理智提醒",
-    description="在理智回满时@用户提醒",
+    description="在理智回满时提醒用户",
     usage=(
         "命令:"
         "\n    理智提醒 => 默认记当前理智为0，回满到135时提醒"
         "\n    理智提醒 [当前理智] [回满理智] => 同上，不过手动指定当前理智与回满理智"
         "\n    理智查看 => 查看距离理智回满还有多久，以及当期理智为多少"
     ),
     extra={
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/__init__.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
 @update_game_resource.handle()
 async def _():
     await update_game_resource.send("开始更新游戏素材，视网络情况需5分钟左右……")
     try:
         async with httpx.AsyncClient() as client:
             await ArknightsGameData(client).download_files()
-            await ArknightsDB.init_data()
+            await ArknightsDB.init_data(force=True)
             await ArknightsGameImage(client).download_files()
     except (httpx.ConnectError, httpx.RemoteProtocolError, httpx.TimeoutException) as e:
         logger.error("下载方舟游戏素材请求出错或连接超时，请修改代理、重试或手动下载：")
         logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
         await update_game_resource.finish("下载方舟游戏素材请求出错或连接超时，请修改代理、重试或手动下载：\nhttps://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
     else:
         await update_game_resource.finish("游戏素材更新完成！")
 
 
 @init_db.handle()
 async def _():
     await update_game_resource.send("开始更新游戏数据库，视磁盘读写性能需1分钟左右……")
-    await ArknightsDB.init_data()
+    await ArknightsDB.init_data(force=True)
     await update_game_resource.finish("游戏数据库更新完成！")
 
 
 __plugin_meta__ = PluginMetadata(
     name="杂项",
     description="查看指令列表、更新游戏素材、更新本地数据库",
     usage=(
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/general.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/general.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 """通用功能"""
 import json
 import os
 from pathlib import Path
 from typing import Union, Dict, List
 from nonebot import get_driver
 from aiofiles import open as aopen
+from nonebot import logger
 
 from ..configs import PathConfig
 
 
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
+data_path = Path(pcfg.arknights_data_path).absolute()
+gamedata_path = Path(pcfg.arknights_gamedata_path).absolute()
 # pcfg = PathConfig()
 
-CHARACTER_FILE = pcfg.arknights_gamedata_path / "excel" / "character_table.json"
-ITEM_FILE = pcfg.arknights_gamedata_path / "excel" / "item_table.json"
-SUB_PROF_FILE = pcfg.arknights_gamedata_path / "excel" / "uniequip_table.json"
+CHARACTER_FILE = gamedata_path / "excel" / "character_table.json"
+ITEM_FILE = gamedata_path / "excel" / "item_table.json"
+SUB_PROF_FILE = gamedata_path / "excel" / "uniequip_table.json"
 EQUIP_FILE = SUB_PROF_FILE
-TEAM_FILE = pcfg.arknights_gamedata_path / "excel" / "handbook_team_table.json"
-SWAP_PATH = pcfg.arknights_data_path / "arknights" / "processed_data"
-GACHA_PATH = pcfg.arknights_gamedata_path / "excel" / "gacha_table.json"
+TEAM_FILE = gamedata_path / "excel" / "handbook_team_table.json"
+SWAP_PATH = data_path / "arknights" / "processed_data"
+GACHA_PATH = gamedata_path / "excel" / "gacha_table.json"
+STAGE_PATH = gamedata_path / "excel" / "stage_table.json"
+HANDBOOK_STAGE_PATH = gamedata_path / "excel" / "handbook_info_table.json"
 
 
 async def _name_code_swap(
         value: str,
         swap_file: Path,
         source_file: Path,
         type_: str = "name2code",
         *,
         layer: tuple = (0, None),
         name_key: str = "name",
+        code_key: str = None,
         data: Union[Dict, List] = None
 ):
     """
     草，写了一坨屎山参数，自己都看不懂了
 
     :param value: 值
     :param swap_file: 保存的映射文件名
     :param source_file: 源文件
     :param type_: name2code / code2name
     :param layer: 有些源文件不是一层映射，如 arknights_item_table，需要向深 1 层进入 "items"，对应 (1, "items")
     :param name_key: 有些源文件表示名字的键不叫 name，如 uniequip_table 的叫 "subProfessionName",
+    :param code_key: 有些文件要转换的代码名不是键名，如 handbook_stage 的在值中，名为 code
     :param data: 没有源文件的，直接用data写入
     :return:
     """
     if not value:
         return ""
 
     if swap_file.exists():
         async with aopen(swap_file, "r", encoding="utf-8") as fp:
             mapping = json.loads(await fp.read())
-        return mapping[type_].get(value, None)
+        return mapping[type_].get(value, value)
 
     if data:
         async with aopen(swap_file, "w", encoding="utf-8") as fp:
             await fp.write(json.dumps(data, ensure_ascii=False))
-        return data[type_].get(value, None)
+        return data[type_].get(value, value)
 
     os.makedirs(swap_file.parent, exist_ok=True)
     mapping = {"name2code": {}, "code2name": {}}
     async with aopen(source_file, "r", encoding="utf-8") as fp:
         data = json.loads(await fp.read())
     for i in range(layer[0]):
         data = data[layer[i+1]]
 
-    codes = list(data.keys())
+    codes = [_[code_key] for _ in data.values()] if code_key else list(data.keys())
     names = [_[name_key] for _ in data.values()]
     mapping["name2code"] = dict(zip(names, codes))
     mapping["code2name"] = dict(zip(codes, names))
     async with aopen(swap_file, "w", encoding="utf-8") as fp:
         await fp.write(json.dumps(mapping, ensure_ascii=False))
 
-    return mapping[type_].get(value, None)
+    return mapping[type_].get(value, value)
 
 
 async def character_swap(value: str, type_: str = "name2code") -> str:
     """干员的名字-id互相查询，默认名字查id"""
     swap_file = SWAP_PATH / "character_swap.json"
     source_file = CHARACTER_FILE
     return await _name_code_swap(value, swap_file, source_file, type_)
@@ -131,14 +138,60 @@
             "SUPPORT": "辅助干员",
             "SPECIAL": "特种干员"
         }
     }
     return data[type_][value]
 
 
+async def gacha_rule_swap(value: str, type_: str = "name2code") -> str:
+    """池子类型"""
+    data = {
+        "name2code": {
+            "春节": "ATTAIN",
+            "限定": "LIMITED",
+            "联动": "LINKAGE",
+            "普通": "NORMAL"
+        },
+        "code2name": {
+            "ATTAIN": "春节",
+            "LIMITED": "限定",
+            "LINKAGE": "联动",
+            "NORMAL": "普通"
+        }
+    }
+    return data[type_][value]
+
+
+async def stage_swap(value: str, type_: str = "name2code") -> str:
+    """关卡的名字-id互相查询，默认名字查id"""
+    swap_file = SWAP_PATH / "stage_swap.json"
+    source_file = STAGE_PATH
+    return await _name_code_swap(value, swap_file, source_file, type_, layer=(1, "stages"))
+
+
+async def handbook_stage_swap(value: str, type_: str = "name2code") -> str:
+    """悖论模拟的名字-id互相查询，默认名字查id"""
+    swap_file = SWAP_PATH / "handbook_stage_swap.json"
+    source_file = HANDBOOK_STAGE_PATH
+    return await _name_code_swap(value, swap_file, source_file, type_, layer=(1, "handbookStageData"), code_key="code")
+
+
+async def nickname_swap(value: str) -> str:
+    """干员昵称/外号转换"""
+    swap_file = SWAP_PATH / "nicknames.json"
+    async with aopen(swap_file, "r", encoding="utf-8") as fp:
+        data = json.loads(await fp.read())
+
+    for k, v in data.items():
+        if value == k or value in v:
+            logger.info(f"{value} -> {k}")
+            return k
+    return value
+
+
 async def get_recruitment_available() -> List[str]:
     """获取可以公招获取的干员id们"""
     async with aopen(GACHA_PATH, "r", encoding="utf-8") as fp:
         text = json.loads(await fp.read())["recruitDetail"]
 
     # 处理这堆字
     text = text.replace("\\n", "\n").replace("<@rc.eml>", "\n").replace("</>", "\n").split("\n")
@@ -152,10 +205,15 @@
 __all__ = [
     "character_swap",
     "item_swap",
     "sub_prof_swap",
     "equip_swap",
     "prof_swap",
     "faction_swap",
+    "gacha_rule_swap",
+    "stage_swap",
+    "handbook_stage_swap",
+
+    "nickname_swap",
 
     "get_recruitment_available"
 ]
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/image.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/src/utils/update.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/src/utils/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,50 @@
 from aiofiles import open as aopen, os as aos
 from lxml import etree
 from urllib.parse import quote, unquote
 from nonebot import logger, get_driver
 
 import httpx
 
-from ..configs import PathConfig, ProxyConfig
+from ..configs import PathConfig, ProxyConfig, SchedulerConfig
 
 driver = get_driver()
 pcfg = PathConfig.parse_obj(get_driver().config.dict())
-xcfg = ProxyConfig.parse_obj(get_driver().config.dict())
+data_path = Path(pcfg.arknights_data_path).absolute()
+gamedata_path = Path(pcfg.arknights_gamedata_path).absolute()
+gameimage_path = Path(pcfg.arknights_gameimage_path).absolute()
+font_path = Path(pcfg.arknights_font_path).absolute()
 
+xcfg = ProxyConfig.parse_obj(get_driver().config.dict())
 BASE_URL_RAW = xcfg.github_raw  # 镜像
 BASE_URL_SITE = xcfg.github_site
 
+scfg = SchedulerConfig.parse_obj(get_driver().config.dict())
+
 REPOSITORIES = {
     "gamedata": "/Kengxxiao/ArknightsGameData/master",
     "gameimage_1": "/yuanyan3060/Arknights-Bot-Resource/master",
     "gameimage_2": "/Aceship/Arknight-Images/master",
 }
 
 FILES = {
     "gamedata": [
         "zh_CN/gamedata/excel/building_data.json",          # 基建技能，制造配方
         "zh_CN/gamedata/excel/char_patch_table.json",       # 升变阿米娅
         "zh_CN/gamedata/excel/character_table.json",        # 干员表
         "zh_CN/gamedata/excel/data_version.txt",            # 数据版本
         "zh_CN/gamedata/excel/gamedata_const.json",         # 游戏常数
         "zh_CN/gamedata/excel/gacha_table.json",            # 公招相关
-        "zh_CN/gamedata/excel/item_table.json",   # 物品表
+        "zh_CN/gamedata/excel/item_table.json",             # 物品表
         "zh_CN/gamedata/excel/handbook_info_table.json",    # 档案表
-        "zh_CN/gamedata/excel/skill_table.json",  # 技能表
+        "zh_CN/gamedata/excel/skill_table.json",            # 技能表
         "zh_CN/gamedata/excel/uniequip_table.json",         # 模组表、子职业映射
         "zh_CN/gamedata/excel/handbook_team_table.json",    # 干员阵营
+        "zh_CN/gamedata/excel/skin_table.json",             # 皮肤
+        "zh_CN/gamedata/excel/stage_table.json",            # 关卡
     ]
 }
 
 DIRS = {
     "gamedata": [
         "/zh_CN/gamedata/excel"
     ],
@@ -77,33 +85,33 @@
     def __init__(self, client: httpx.AsyncClient = None):
         self._url = f"{BASE_URL_RAW}{REPOSITORIES['gamedata']}"
         self._client = client or httpx.AsyncClient()
 
     async def get_local_version(self) -> str:
         """获取本地版本"""
         try:
-            async with aopen(pcfg.arknights_gamedata_path / "excel" / "data_version.txt") as fp:
+            async with aopen(gamedata_path / "excel" / "data_version.txt") as fp:
                 data = await fp.read()
         except FileNotFoundError as e:
             return ""
-        return data.split("\n")[-2].split(":")[1]
+        return data.split(":")[-1].strip("\n").strip()
 
     async def get_latest_version(self) -> str:
         """获取最新版本"""
         url = f"{self._url}/zh_CN/gamedata/excel/data_version.txt"
         response = await self._client.get(url)
-        return response.text.split("\n")[-2].split(":")[1]  # eg: "31.4.0"
+        return response.text.split(":")[-1].strip("\n").strip()  # eg: "31.4.0"
 
     async def is_update_needed(self) -> bool:
         """是否要更新"""
         return await self.get_local_version() != await self.get_latest_version()
 
     async def download_files(self):
         """下载gamedata"""
-        tmp = Path(__file__).absolute().parent.parent.parent / "data" / "arknights" / "gamedata" / "excel"
+        tmp = gamedata_path / "excel"
         await aos.makedirs(tmp, exist_ok=True)
         logger.info("##### ARKNIGHTS GAMEDATA DOWNLOAD BEGIN ")
 
         tasks = [
             self.save(self._url, file, tmp)
             for file in FILES['gamedata']
         ]
@@ -122,15 +130,15 @@
     def __init__(self, client: httpx.AsyncClient = None):
         self._client = client or httpx.AsyncClient()
         self._urls: List[str] = []
         self._htmls: Dict[str, str] = {}
 
     async def download_files(self):
         """下载gameimage"""
-        tmp = Path(__file__).absolute().parent.parent.parent / "data" / "arknights" / "gameimage"
+        tmp = gameimage_path
         await aos.makedirs(tmp, exist_ok=True)
         logger.info("##### ARKNIGHTS GAMEIMAGE DOWNLOAD BEGIN ")
 
         logger.info("\t### REQUESTING FILE LISTS ... ")
         tasks = []
         for dir_ in DIRS['gameimage_1']:
             await aos.makedirs(tmp / dir_, exist_ok=True)
@@ -212,64 +220,84 @@
             return
         async with aopen(tmp / unquote(url).split('/master/')[-1], "wb") as fp:
             await fp.write(content)
         logger.info(f"\t- Arknights-Image downloaded: {unquote(url).split('/master/')[-1]}")
 
 
 async def download_extra_files(client: httpx.AsyncClient):
-    """下载字体、猜干员的图片素材"""
+    """下载猜干员的图片素材、干员外号昵称"""
     urls = [
-        f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/fonts/Arknights-en.ttf",
-        f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/fonts/Arknights-zh.otf",
         f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/guess_character/correct.png",
         f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/guess_character/down.png",
         f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/guess_character/up.png",
         f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/guess_character/vague.png",
         f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/guess_character/wrong.png",
+
+        f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/arknights/processed_data/nicknames.json",
     ]
     logger.info("##### EXTRA FILES DOWNLOAD BEGIN")
-    await aos.makedirs(pcfg.arknights_data_path / "fonts", exist_ok=True)
-    await aos.makedirs(pcfg.arknights_data_path / "guess_character", exist_ok=True)
+    await aos.makedirs(data_path / "guess_character", exist_ok=True)
+    await aos.makedirs(data_path / "arknights/processed_data", exist_ok=True)
     for url in urls:
-        path = url.split("data/")[-1]
-        if (pcfg.arknights_data_path / path).exists():
+        path = url.split("/data/")[-1]
+        if (data_path / path).exists():
             continue
         response = await client.get(url)
-        async with aopen(pcfg.arknights_data_path / path, "wb") as fp:
+        async with aopen(data_path / path, "wb") as fp:
             await fp.write(response.content)
             logger.info(f"\t- Extra file downloaded: {path}")
+    await download_fonts(client)
     logger.info("===== EXTRA FILES DOWNLOAD DONE")
 
 
+async def download_fonts(client: httpx.AsyncClient):
+    """下载字体"""
+    urls = [
+        f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/fonts/Arknights-en.ttf",
+        f"{BASE_URL_RAW}/NumberSir/nonebot_plugin_arktools/main/nonebot_plugin_arktools/data/fonts/Arknights-zh.otf",
+    ]
+    await aos.makedirs(font_path, exist_ok=True)
+    for url in urls:
+        path = url.split("/")[-1]
+        if (font_path / path).exists():
+            continue
+        response = await client.get(url)
+        async with aopen(font_path / path, "wb") as fp:
+            await fp.write(response.content)
+            logger.info(f"\t- Font file downloaded: {path}")
+
+
 @driver.on_startup
 async def _init_game_files():
-    async with httpx.AsyncClient(timeout=100) as client:
-        try:
-            await download_extra_files(client)
-        except (httpx.ConnectError, httpx.RemoteProtocolError, httpx.TimeoutException) as e:
-            logger.error("下载方舟额外素材请求出错或连接超时，请修改代理、重试或手动下载：")
-            logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
-
-        logger.info("检查方舟游戏素材版本中 ...")
-        is_latest = False
-        try:
-            if not await ArknightsGameData(client).is_update_needed():
-                logger.info("方舟游戏素材当前为最新！")
-                is_latest = True
-        except (httpx.ConnectError, httpx.RemoteProtocolError, httpx.TimeoutException) as e:
-            logger.error("检查方舟素材版本请求出错或连接超时，请修改代理、重试或手动下载：")
-            logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
-        else:
-            if not is_latest:
-                try:
-                    await ArknightsGameData(client).download_files()
-                    await ArknightsGameImage(client).download_files()
-                except (httpx.ConnectError, httpx.RemoteProtocolError, httpx.TimeoutException) as e:
-                    logger.error("下载方舟素材请求出错或连接超时，请修改代理、重试或手动下载：")
-                    logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
+    if scfg.arknights_update_check_switch:
+        async with httpx.AsyncClient(timeout=100) as client:
+            try:
+                await download_extra_files(client)
+            except (httpx.ConnectError, httpx.RemoteProtocolError, httpx.TimeoutException) as e:
+                logger.error("下载方舟额外素材请求出错或连接超时，请修改代理、重试或手动下载：")
+                logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
+
+            logger.info("检查方舟游戏素材版本中 ...")
+            is_latest = False
+            try:
+                if not await ArknightsGameData(client).is_update_needed():
+                    logger.info("方舟游戏素材当前为最新！")
+                    is_latest = True
+            except (httpx.ConnectError, httpx.RemoteProtocolError, httpx.TimeoutException) as e:
+                logger.error("检查方舟素材版本请求出错或连接超时，请修改代理、重试或手动下载：")
+                logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
+            else:
+                if not is_latest:
+                    logger.info("方舟游戏素材需要更新，开始下载素材...")
+                    try:
+                        await ArknightsGameData(client).download_files()
+                        await ArknightsGameImage(client).download_files()
+                    except (httpx.ConnectError, httpx.RemoteProtocolError, httpx.TimeoutException) as e:
+                        logger.error("下载方舟素材请求出错或连接超时，请修改代理、重试或手动下载：")
+                        logger.error("https://github.com/NumberSir/nonebot_plugin_arktools#%E5%90%AF%E5%8A%A8%E6%B3%A8%E6%84%8F")
 
 
 __all__ = [
     "ArknightsGameImage",
     "ArknightsGameData",
     "_init_game_files"
 ]
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/test_open_recruitment.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/test_open_recruitment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools/test/utils.py` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools/test/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/PKG-INFO` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-arktools
-Version: 1.0.9
+Version: 1.1.0
 Summary: 基于 OneBot 适配器的 NoneBot2 明日方舟小工具箱插件
 Home-page: https://github.com/NumberSir/nonebot_plugin_arktools
 Author: Number_Sir
 Author-email: Number_Sir@126.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
   
 # Nonebot_Plugin_ArkTools
   
 _✨ 基于 OneBot 适配器的 [NoneBot2](https://v2.nonebot.dev/) 明日方舟小工具箱插件 ✨_
   
 </div>
 
-[![OSCS Status](https://www.oscs1024.com/platform/badge/NumberSir/nonebot_plugin_arktools.svg?size=small)](https://www.oscs1024.com/project/NumberSir/nonebot_plugin_arktools?ref=badge_small)
+[![OSCS Status](https://www.oscs1024.com/platform/badge/NumberSir/nonebot_plugin_arktools.svg?size=small)](https://www.oscs1024.com/project/NumberSir/nonebot_plugin_arktools?ref=badge_small)  [![star](https://gitee.com/Number_Sir/nonebot_plugin_arktools/badge/star.svg?theme=white)](https://gitee.com/Number_Sir/nonebot_plugin_arktools/stargazers)
 
 本人python小萌新，插件有不完善和可以改进之处欢迎各位多提pr和issue
 
 - [功能](#功能)
 - [安装](#安装)
 - [使用](#如何使用)
 - [示例](#图片示例)
@@ -42,14 +42,15 @@
 1. [x] 可以查询推荐的公招标签(截图识别/手动输文字)
 2. [x] 可以查询干员的技能升级材料、专精材料、精英化材料、模组升级材料
 3. [x] 可以通过网易云点歌，以卡片形式发送
 4. [x] 猜干员小游戏，玩法与 [wordle](https://github.com/noneplugin/nonebot-plugin-wordle) 相同
 5. [x] 可以查看生日为今天的干员
 6. [x] 可以记录当前理智，等回复满后提醒
 7. [x] 指定群聊自动推送最新游戏公告
+8. [x] 查询、订阅、推送 [MAA 作业站](https://prts.plus)的作业
 
 ## 编写中...
 1. [ ] 可以查询某种资源在哪个关卡期望理智最低
 2. [ ] 根据当前有的资源和需要的资源种类、数量测算最优推图计划
 3. [ ] 查询某干员的基础数据：
    1. [ ] 给定等级、信赖、潜能下的基础面板
    2. [ ] 天赋、特性、技能
@@ -58,67 +59,99 @@
 
 # 安装
 - 使用 pip
 ```
 pip install -U nonebot_plugin_arktools
 ```
 
+- 使用 nb-cli
+```
+nb plugin install nonebot_plugin_arktools
+```
+
 # 如何使用
 ## 启动注意
  - 每次启动并连接到客户端后会从 __[明日方舟常用素材库](https://github.com/yuanyan3060/Arknights-Bot-Resource)__(__[yuanyan3060](https://github.com/yuanyan3060)__), __[《明日方舟》游戏数据库](https://github.com/Kengxxiao/ArknightsGameData)__(__[Kengxxiao](https://github.com/Kengxxiao)__), __[Arknight-Images](https://github.com/Aceship/Arknight-Images)__(__[Aceship](https://github.com/Aceship)__) 下载使用插件必需的文本及图片资源到本地，已经下载过的文件不会重复下载。下载根据网络情况不同可能耗时 5 分钟左右
  - 如需手动更新，请用命令 __“更新方舟素材”__ 进行更新
- - 如果自动下载失败，请手动下载发行版中的 __“`data.zip`”__ 压缩文件，解压到 __“`nonebot_plugin_arktools/data`”__ 文件夹下，正确放置的文件夹结构应为：
+ - 如果自动下载失败，请手动下载发行版中的 __“`data.zip`”/“`data.tar.gz`”__ 压缩文件，解压到 “`机器人根目录`” 文件夹下(即运行 `nb run` 命令的文件夹/ `bot.py` 的文件夹)。正确放置的文件夹结构应为：
 ```txt
-nonebot_plugin_arktools
+举例：
 ├── data
-│   ├── arknights
-│   │   ├── gamedata
-│   │   │   └── excel
-│   │   │       └── ...
-│   │   ├── gameimage
-│   │   │   └── ...
-│   │   └── ...
-│   ├── fonts
-│   │   ├── Arknights-en.ttf
-│   │   └── Arknights-zh.otf
-│   ├── guess_character
-│   │   ├── correct.png
-│   │   ├── down.png
-│   │   ├── up.png
-│   │   ├── vague.png
-│   │   └── wrong.png
-│   └── ...
-├── src
-├── test
-├── ...
+│   └── arktools
+│       ├── arknights
+│       │   ├── gamedata
+│       │   │   └── excel
+│       │   │       └── ...
+│       │   ├── gameimage
+│       │   │   └── ...
+│       │   ├── processed_data
+│       │   │   └── nicknames.json
+│       │   └── ...
+│       ├── fonts
+│       │   ├── Arknights-en.ttf
+│       │   └── Arknights-zh.otf
+│       ├── guess_character
+│       │   ├── correct.png
+│       │   ├── down.png
+│       │   ├── up.png
+│       │   ├── vague.png
+│       │   └── wrong.png
+│       └── ...
+├── plugin
+│   └── nonebot_plugin_arktools
+│       ├── src
+│       └── ...
+├── .env
+├── .env.dev
+├── .env.prod
 ...
 ```
 
 ## .env.env 配置项
 
 ```ini
+# 百度 OCR 配置，公招识别截图用
 # 具体见 https://console.bce.baidu.com/ai/?fromai=1#/ai/ocr/app/list
-arknights_baidu_api_key="xxx"    # 【必填】百度 OCR API KEY
-arknights_baidu_secret_key="xxx"   # 【必填】百度 OCR SECRET KEY
+ARKNIGHTS_BAIDU_API_KEY="xxx"    # 【必填】百度 OCR API KEY
+ARKNIGHTS_BAIDU_SECRET_KEY="xxx"   # 【必填】百度 OCR SECRET KEY
 
-github_raw="https://raw.githubusercontent.com"   # 默认为 https://raw.githubusercontent.com，如有镜像源可以替换
-github_site="https://github.com"  # 默认为 https://github.com，如有镜像源可以替换
+# 代理配置，如部署机器人的服务器在国内大陆地区可能需要修改
+GITHUB_RAW="https://raw.githubusercontent.com"   # 默认为 https://raw.githubusercontent.com，如有镜像源可以替换，如 https://ghproxy.com/https://raw.githubusercontent.com
+GITHUB_SITE="https://github.com"  # 默认为 https://github.com，如有镜像源可以替换，如 https://kgithub.com
+RSS_SITE="https://rsshub.app"  # 默认为 https://rsshub.app，如有镜像源可以替换
+
+# 定时任务配置，默认是关闭的
+ANNOUNCE_PUSH_SWITCH=False  # 是否自动推送舟舟最新公告，默认为 False; True 为开启自动检测
+ANNOUNCE_PUSH_INTERVAL=1  # 自动推送最新公告的检测间隔，上述开关开启时有效，默认为 1 分钟
+SANITY_NOTIFY_SWITCH=False  # 是否自动检测理智提醒，默认为 False; True 为开启自动检测
+SANITY_NOTIFY_INTERVAL=10  # 自动检测理智提醒的检测间隔，上述开关开启时有效，默认为 10 分钟
+MAA_COPILOT_SWITCH=False  # 是否自动推送MAA作业站新作业，默认为 False; True 为开启自动检测
+MAA_COPILOT_INTERVAL=60  # 自动推送MAA作业站新作业的检测间隔，上述开关开启时有效，默认为 60 分钟
+
+# 启动前素材检查配置，默认是开启的
+ARKNIGHTS_UPDATE_CHECK_SWITCH=True  # 是否在启动bot时检查素材版本并下载，默认为True; False 为禁用检查
+
+# 资源路径配置，默认在启动机器人的目录中/运行nb run的目录中/放bot.py的目录中
+ARKNIGHTS_DATA_PATH="data/arktools"                                   # 资源根路径，如果修改了根路径，下方路径都要修改
+ARKNIGHTS_FONT_PATH="data/arktools/fonts"                             # 字体路径
+ARKNIGHTS_GAMEDATA_PATH="data/arktools/arknights/gamedata"            # 游戏数据
+ARKNIGHTS_GAMEIMAGE_PATH="data/arktools/arknights/gameimage"          # 游戏图像
+ARKNIGHTS_DB_URL="data/arktools/databases/arknights_sqlite.sqlite3"   # 数据库
 
-announce_push_switch=False  # 是否自动推送舟舟最新公告，默认为 False; True 为开启自动检测
-announce_push_interval=1  # 自动推送最新公告的检测间隔，上述开关开启时有效，默认为 1 分钟
-
-sanity_notify_switch=False  # 是否自动检测理智提醒，默认为 False; True 为开启自动检测
-sanity_notify_interval=10  # 自动检测理智提醒的检测间隔，上述开关开启时有效，默认为 10 分钟
 ...
 ```
 各配置项的含义如上。
 <div align="left">
   <img src="https://user-images.githubusercontent.com/52584526/219335891-37933d79-1b52-4452-8959-04861087f4e8.png" width="700" />
 </div>
 
+
+## 干员昵称
+位置默认在 `data/arknights/processed_data/nicknames.json` 键为干员中文名称，值为昵称，可自行修改。
+
 ## 指令
 <details>
 <summary>点击展开</summary>
 
 ### 详细指令
 使用以下指令触发，需加上指令前缀
 ```text
@@ -166,14 +199,23 @@
 ```
 公告推送
 ```text
 添加方舟推送群 / ADDGROUP   => 添加自动推送的群号
 删除方舟推送群 / DELGROUP   => 删除自动推送的群号
 查看方舟推送群 / GETGROUP   => 查看自动推送的群号
 ```
+MAA 作业站相关
+```text
+maa添加订阅 / ADDMAA [关键词1 关键词2 ...]  => 添加自动推送的关键词
+maa删除订阅 / DELMAA [关键词1 关键词2 ...]  => 删除自动推送的关键词
+maa查看订阅 / GETMAA                      => 查看本群自动推送的关键词
+
+maa查作业 [关键词1 关键词2 ...]                   => 按关键词组合查作业，默认为最新发布的第一个作业
+maa查作业 [关键词1 关键词2 ...] | [热度/最新/访问]  => 同上，不过可以指定按什么顺序查询
+```
 </details>
 
 # 图片示例
 <details>
 <summary>点击展开</summary>
 
 ## 图片们
@@ -221,20 +263,54 @@
 
 # 感谢
  - __[yuanyan3060](https://github.com/yuanyan3060)__ 的 __[明日方舟常用素材库](https://github.com/yuanyan3060/Arknights-Bot-Resource)__
  - __[Kengxxiao](https://github.com/Kengxxiao)__ 的 __[《明日方舟》游戏数据库](https://github.com/Kengxxiao/ArknightsGameData)__
  - __[Aceship](https://github.com/Aceship)__ 的 __[Arknight-Images](https://github.com/Aceship/Arknight-Images)__
  - __[AmiyaBot](https://github.com/AmiyaBot)__ 的 __[Amiya-bot](https://github.com/AmiyaBot/Amiya-Bot)__
  - __[Strelizia02](https://github.com/Strelizia02)__ 的 __[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__
-
+ - __[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ 的 __[MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights)__
 
 # 更新日志
 <details>
 <summary>点击展开</summary>
 
+> 2023-04-15 v1.1.0
+> - 公招查询、猜干员、理智提醒现在均可以私聊进行 (不推荐，私聊发消息可能导致风控)
+> - 简易修复了与其它同用 Tortoise-ORM 的插件初始化冲突的问题 [@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15)
+> - 添加在群聊查询、订阅、推送 [MAA 作业站](https://prts.plus)作业的功能
+> - 修复了更新数据库中某张表格时会删除所有表格的问题
+> 
+> 2023-04-08 v1.0.20
+> - 修复因素材库更新滞后导致无法查看干员的问题
+> 
+> 2023-04-07 v1.0.19
+> - 修复更新数据库命令不会强制覆盖更新的问题
+> 
+> 2023-04-06 v1.0.18
+> - 修复了舟舟更新数据结构导致的创建表单错误
+>
+> 2023-04-04 v1.0.17
+> - 添加数据库初始化检查，不再每次启动bot时重复创建
+> - 添加每次启动bot时的数据更新检查开关，默认启用 [@issue/39](https://github.com/NumberSir/nonebot_plugin_arktools/issues/39)
+>
+> 2023-03-28 v1.0.15
+> - 猜干员与干员信息功能可以使用干员昵称(可自行增删改查)
+> 
+> 2023-03-24 v1.0.14
+> - 修复阿米娅与近卫阿米娅冲突的问题 [@zx-issue/13](https://github.com/NumberSir/zhenxun_arktools/issues/13)
+> 
+> 2023-03-08 v1.0.12
+> - 添加 rsshub 代理配置项 [@issue/34](https://github.com/NumberSir/nonebot_plugin_arktools/issues/34)
+> - 修复公招命令不处理的问题 [@issue/35](https://github.com/NumberSir/nonebot_plugin_arktools/issues/35)
+> - 添加方舟素材/资源路径配置项，现在默认在机器人根目录下 `data/arktools` 文件夹 [@issue/36](https://github.com/NumberSir/nonebot_plugin_arktools/issues/36)
+> - 修复查询暮落干员信息时会选中空白暮落的问题
+> 
+> 2023-02-20 v1.0.11
+> - 修复最新版本检测出错的问题
+> 
 > 2023-02-19 v1.0.9
 > - 添加定时任务配置项
 > - 修复定时任务导致其它处理器阻塞的问题 [@issue/30](https://github.com/NumberSir/nonebot_plugin_arktools/issues/30) [@zx-issue/9](https://github.com/NumberSir/zhenxun_arktools/issues/9)
 > - 修复猜干员无法判断重复猜的问题 [@zx-issue/10](https://github.com/NumberSir/zhenxun_arktools/issues/10)
 > - 修复猜干员结果图不按顺序绘制的问题
 >
 > 2023-02-16 v1.0.8
```

#### html2text {}

```diff
@@ -1,82 +1,111 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-arktools Version: 1.0.9 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-arktools Version: 1.1.0 Summary:
 åºäº OneBot ééå¨ç NoneBot2 ææ¥æ¹èå°å·¥å·ç®±æä»¶ Home-page:
 https://github.com/NumberSir/nonebot_plugin_arktools Author: Number_Sir Author-
 email: Number_Sir@126.com Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
                                    [nonebot]
  # Nonebot_Plugin_ArkTools _â¨ åºäº OneBot ééå¨ç [NoneBot2](https://
              v2.nonebot.dev/) ææ¥æ¹èå°å·¥å·ç®±æä»¶ â¨_
 [![OSCS Status](https://www.oscs1024.com/platform/badge/NumberSir/
 nonebot_plugin_arktools.svg?size=small)](https://www.oscs1024.com/project/
-NumberSir/nonebot_plugin_arktools?ref=badge_small)
+NumberSir/nonebot_plugin_arktools?ref=badge_small) [![star](https://gitee.com/
+Number_Sir/nonebot_plugin_arktools/badge/star.svg?theme=white)](https://
+gitee.com/Number_Sir/nonebot_plugin_arktools/stargazers)
 æ¬äººpythonå°èæ°ï¼æä»¶æä¸å®ååå¯ä»¥æ¹è¿ä¹å¤æ¬¢è¿åä½å¤æpråissue
 - [åè½](#åè½) - [å®è£](#å®è£) - [ä½¿ç¨](#å¦ä½ä½¿ç¨) - [ç¤ºä¾]
 (#å¾çç¤ºä¾) - [æè°¢](#æè°¢) - [æ´æ°æ¥å¿](#æ´æ°æ¥å¿) # åè½ ##
 å·²å®ç°ï¼ 1. [x] å¯ä»¥æ¥è¯¢æ¨èçå¬ææ ç­¾(æªå¾è¯å«/
 æå¨è¾æå­) 2. [x]
 å¯ä»¥æ¥è¯¢å¹²åçæè½åçº§ææãä¸ç²¾ææãç²¾è±åææãæ¨¡ç»åçº§ææ
 3. [x] å¯ä»¥éè¿ç½æäºç¹æ­ï¼ä»¥å¡çå½¢å¼åé 4. [x]
 çå¹²åå°æ¸¸æï¼ç©æ³ä¸ [wordle](https://github.com/noneplugin/nonebot-
 plugin-wordle) ç¸å 5. [x] å¯ä»¥æ¥ççæ¥ä¸ºä»å¤©çå¹²å 6. [x]
 å¯ä»¥è®°å½å½åçæºï¼ç­åå¤æ»¡åæé 7. [x]
-æå®ç¾¤èèªå¨æ¨éææ°æ¸¸æå¬å ## ç¼åä¸­... 1. [ ]
+æå®ç¾¤èèªå¨æ¨éææ°æ¸¸æå¬å 8. [x] æ¥è¯¢ãè®¢éãæ¨é [MAA
+ä½ä¸ç«](https://prts.plus)çä½ä¸ ## ç¼åä¸­... 1. [ ]
 å¯ä»¥æ¥è¯¢æç§èµæºå¨åªä¸ªå³å¡ææçæºæä½ 2. [ ]
 æ ¹æ®å½åæçèµæºåéè¦çèµæºç§ç±»ãæ°éæµç®æä¼æ¨å¾è®¡å
 3. [ ] æ¥è¯¢æå¹²åçåºç¡æ°æ®ï¼ 1. [ ]
 ç»å®ç­çº§ãä¿¡èµãæ½è½ä¸çåºç¡é¢æ¿ 2. [ ]
 å¤©èµãç¹æ§ãæè½ 3. [ ]
 å¹²åç§æãå¿åãèº«é«ç­åºæ¬ä¸ªäººä¿¡æ¯ 4. [ ] å®æ¶æéå¿ç­ /
 èå»ç«  / åçº¦ç­æ´»å¨è¿æ # å®è£ - ä½¿ç¨ pip ``` pip install -
-U nonebot_plugin_arktools ``` # å¦ä½ä½¿ç¨ ## å¯å¨æ³¨æ -
+U nonebot_plugin_arktools ``` - ä½¿ç¨ nb-cli ``` nb plugin install
+nonebot_plugin_arktools ``` # å¦ä½ä½¿ç¨ ## å¯å¨æ³¨æ -
 æ¯æ¬¡å¯å¨å¹¶è¿æ¥å°å®¢æ·ç«¯åä¼ä» __[ææ¥æ¹èå¸¸ç¨ç´ æåº]
 (https://github.com/yuanyan3060/Arknights-Bot-Resource)__(__[yuanyan3060]
 (https://github.com/yuanyan3060)__), __[ãææ¥æ¹èãæ¸¸ææ°æ®åº]
 (https://github.com/Kengxxiao/ArknightsGameData)__(__[Kengxxiao](https://
 github.com/Kengxxiao)__), __[Arknight-Images](https://github.com/Aceship/
 Arknight-Images)__(__[Aceship](https://github.com/Aceship)__)
 ä¸è½½ä½¿ç¨æä»¶å¿éçææ¬åå¾çèµæºå°æ¬å°ï¼å·²ç»ä¸è½½è¿çæä»¶ä¸ä¼éå¤ä¸è½½ãä¸è½½æ ¹æ®ç½ç»æåµä¸åå¯è½èæ¶
 5 åéå·¦å³ - å¦éæå¨æ´æ°ï¼è¯·ç¨å½ä»¤ __âæ´æ°æ¹èç´ æâ__
 è¿è¡æ´æ° - å¦æèªå¨ä¸è½½å¤±è´¥ï¼è¯·æå¨ä¸è½½åè¡çä¸­ç
-__â`data.zip`â__ åç¼©æä»¶ï¼è§£åå° __â`nonebot_plugin_arktools/
-data`â__ æä»¶å¤¹ä¸ï¼æ­£ç¡®æ¾ç½®çæä»¶å¤¹ç»æåºä¸ºï¼ ```txt
-nonebot_plugin_arktools âââ data â âââ arknights â â
+__â`data.zip`â/â`data.tar.gz`â__ åç¼©æä»¶ï¼è§£åå°
+â`æºå¨äººæ ¹ç®å½`â æä»¶å¤¹ä¸(å³è¿è¡ `nb run` å½ä»¤çæä»¶å¤¹/
+`bot.py` çæä»¶å¤¹)ãæ­£ç¡®æ¾ç½®çæä»¶å¤¹ç»æåºä¸ºï¼ ```txt
+ä¸¾ä¾ï¼ âââ data â âââ arktools â âââ arknights â â
 âââ gamedata â â â âââ excel â â â âââ ... â
-â âââ gameimage â â â âââ ... â â âââ ... â
+â âââ gameimage â â â âââ ... â â âââ
+processed_data â â â âââ nicknames.json â â âââ ... â
 âââ fonts â â âââ Arknights-en.ttf â â âââ Arknights-
 zh.otf â âââ guess_character â â âââ correct.png â â
 âââ down.png â â âââ up.png â â âââ vague.png â â
-âââ wrong.png â âââ ... âââ src âââ test âââ
-... ... ``` ## .env.env éç½®é¡¹ ```ini # å·ä½è§ https://
+âââ wrong.png â âââ ... âââ plugin â âââ
+nonebot_plugin_arktools â âââ src â âââ ... âââ .env
+âââ .env.dev âââ .env.prod ... ``` ## .env.env éç½®é¡¹ ```ini #
+ç¾åº¦ OCR éç½®ï¼å¬æè¯å«æªå¾ç¨ # å·ä½è§ https://
 console.bce.baidu.com/ai/?fromai=1#/ai/ocr/app/list
-arknights_baidu_api_key="xxx" # ãå¿å¡«ãç¾åº¦ OCR API KEY
-arknights_baidu_secret_key="xxx" # ãå¿å¡«ãç¾åº¦ OCR SECRET KEY
-github_raw="https://raw.githubusercontent.com" # é»è®¤ä¸º https://
-raw.githubusercontent.comï¼å¦æéåæºå¯ä»¥æ¿æ¢ github_site="https://
-github.com" # é»è®¤ä¸º https://github.comï¼å¦æéåæºå¯ä»¥æ¿æ¢
-announce_push_switch=False # æ¯å¦èªå¨æ¨éèèææ°å¬åï¼é»è®¤ä¸º
-False; True ä¸ºå¼å¯èªå¨æ£æµ announce_push_interval=1 #
+ARKNIGHTS_BAIDU_API_KEY="xxx" # ãå¿å¡«ãç¾åº¦ OCR API KEY
+ARKNIGHTS_BAIDU_SECRET_KEY="xxx" # ãå¿å¡«ãç¾åº¦ OCR SECRET KEY #
+ä»£çéç½®ï¼å¦é¨ç½²æºå¨äººçæå¡å¨å¨å½åå¤§éå°åºå¯è½éè¦ä¿®æ¹
+GITHUB_RAW="https://raw.githubusercontent.com" # é»è®¤ä¸º https://
+raw.githubusercontent.comï¼å¦æéåæºå¯ä»¥æ¿æ¢ï¼å¦ https://
+ghproxy.com/https://raw.githubusercontent.com GITHUB_SITE="https://github.com"
+# é»è®¤ä¸º https://github.comï¼å¦æéåæºå¯ä»¥æ¿æ¢ï¼å¦ https://
+kgithub.com RSS_SITE="https://rsshub.app" # é»è®¤ä¸º https://
+rsshub.appï¼å¦æéåæºå¯ä»¥æ¿æ¢ #
+å®æ¶ä»»å¡éç½®ï¼é»è®¤æ¯å³é­ç ANNOUNCE_PUSH_SWITCH=False #
+æ¯å¦èªå¨æ¨éèèææ°å¬åï¼é»è®¤ä¸º False; True
+ä¸ºå¼å¯èªå¨æ£æµ ANNOUNCE_PUSH_INTERVAL=1 #
 èªå¨æ¨éææ°å¬åçæ£æµé´éï¼ä¸è¿°å¼å³å¼å¯æ¶ææï¼é»è®¤ä¸º
-1 åé sanity_notify_switch=False #
+1 åé SANITY_NOTIFY_SWITCH=False #
 æ¯å¦èªå¨æ£æµçæºæéï¼é»è®¤ä¸º False; True ä¸ºå¼å¯èªå¨æ£æµ
-sanity_notify_interval=10 #
+SANITY_NOTIFY_INTERVAL=10 #
 èªå¨æ£æµçæºæéçæ£æµé´éï¼ä¸è¿°å¼å³å¼å¯æ¶ææï¼é»è®¤ä¸º
-10 åé ... ``` åéç½®é¡¹çå«ä¹å¦ä¸ã
+10 åé MAA_COPILOT_SWITCH=False #
+æ¯å¦èªå¨æ¨éMAAä½ä¸ç«æ°ä½ä¸ï¼é»è®¤ä¸º False; True
+ä¸ºå¼å¯èªå¨æ£æµ MAA_COPILOT_INTERVAL=60 #
+èªå¨æ¨éMAAä½ä¸ç«æ°ä½ä¸çæ£æµé´éï¼ä¸è¿°å¼å³å¼å¯æ¶ææï¼é»è®¤ä¸º
+60 åé # å¯å¨åç´ ææ£æ¥éç½®ï¼é»è®¤æ¯å¼å¯ç
+ARKNIGHTS_UPDATE_CHECK_SWITCH=True #
+æ¯å¦å¨å¯å¨botæ¶æ£æ¥ç´ æçæ¬å¹¶ä¸è½½ï¼é»è®¤ä¸ºTrue; False
+ä¸ºç¦ç¨æ£æ¥ # èµæºè·¯å¾éç½®ï¼é»è®¤å¨å¯å¨æºå¨äººçç®å½ä¸­/
+è¿è¡nb runçç®å½ä¸­/æ¾bot.pyçç®å½ä¸­ ARKNIGHTS_DATA_PATH="data/
+arktools" #
+èµæºæ ¹è·¯å¾ï¼å¦æä¿®æ¹äºæ ¹è·¯å¾ï¼ä¸æ¹è·¯å¾é½è¦ä¿®æ¹
+ARKNIGHTS_FONT_PATH="data/arktools/fonts" # å­ä½è·¯å¾
+ARKNIGHTS_GAMEDATA_PATH="data/arktools/arknights/gamedata" # æ¸¸ææ°æ®
+ARKNIGHTS_GAMEIMAGE_PATH="data/arktools/arknights/gameimage" # æ¸¸æå¾å
+ARKNIGHTS_DB_URL="data/arktools/databases/arknights_sqlite.sqlite3" # æ°æ®åº
+... ``` åéç½®é¡¹çå«ä¹å¦ä¸ã
 [https://user-images.githubusercontent.com/52584526/219335891-37933d79-1b52-
 4452-8959-04861087f4e8.png]
-## æä»¤  ç¹å»å±å¼ ### è¯¦ç»æä»¤
-ä½¿ç¨ä»¥ä¸æä»¤è§¦åï¼éå ä¸æä»¤åç¼ ```text æ ¼å¼ï¼ æä»¤ =>
-å«ä¹ [] ä»£è¡¨åæ° xxx/yyy ä»£è¡¨ xxx æ yyy ``` æé¡¹ ```text
-æ¹èå¸®å© / arkhelp => æ¥çæä»¤åè¡¨ æ´æ°æ¹èç´ æ =>
-æå¨æ´æ°æ¸¸ææ°æ®(json)ä¸å¾ç æ´æ°æ¹èæ°æ®åº =>
-æå¨æ´æ°æ°æ®åº ``` çå¹²å ```text çå¹²å => å¼å§æ°æ¸¸æ #
-[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
+## å¹²åæµç§° ä½ç½®é»è®¤å¨ `data/arknights/processed_data/nicknames.json`
+é®ä¸ºå¹²åä¸­æåç§°ï¼å¼ä¸ºæµç§°ï¼å¯èªè¡ä¿®æ¹ã ## æä»¤
+ç¹å»å±å¼ ### è¯¦ç»æä»¤ ä½¿ç¨ä»¥ä¸æä»¤è§¦åï¼éå ä¸æä»¤åç¼
+```text æ ¼å¼ï¼ æä»¤ => å«ä¹ [] ä»£è¡¨åæ° xxx/yyy ä»£è¡¨ xxx æ yyy
+``` æé¡¹ ```text æ¹èå¸®å© / arkhelp => æ¥çæä»¤åè¡¨
+æ´æ°æ¹èç´ æ => æå¨æ´æ°æ¸¸ææ°æ®(json)ä¸å¾ç
+æ´æ°æ¹èæ°æ®åº => æå¨æ´æ°æ°æ®åº ``` çå¹²å ```text çå¹²å
+=> å¼å§æ°æ¸¸æ #[å¹²åå] => çå¹²åï¼å¦ï¼#è¾éæ³æ æç¤º =>
 æ¥çç­æ¡å¹²åçä¿¡æ¯ ç»æ => ç»æå½åå±æ¸¸æ ``` ä»æ¥å¹²å
 ```text ä»æ¥å¹²å => æ¥çä»å¤©è¿çæ¥çå¹²å ``` å¡å£¬ç¹æ­ ```text
 å¡å£¬ç¹æ­ [å³é®å­] => ç½æäºç¹æ­ï¼ä»¥å¡çå½¢å¼åå°ç¾¤å ```
 å¹²åä¿¡æ¯ ```text å¹²å [å¹²åå] =>
 æ¥çå¹²åçç²¾è±åãæè½åçº§ãæè½ä¸ç²¾ãæ¨¡ç»è§£ééè¦çææ
 ``` å¬å¼æå ```text å¬æ [å¬æçé¢æªå¾] =>
 æ¥çæ ç­¾ç»ååå¯è½åºç°çå¹²å åå¤æªå¾ï¼å¬æ => åä¸
@@ -84,15 +113,23 @@
 => é»è®¤è®°å½åçæºä¸º0ï¼åæ»¡å°135æ¶æé" çæºæé
 [å½åçæº] [åæ»¡çæº] =>
 åä¸ï¼ä¸è¿æå¨æå®å½åçæºä¸åæ»¡çæº" çæºæ¥ç =>
 æ¥çè·ç¦»çæºåæ»¡è¿æå¤ä¹ï¼ä»¥åå½æçæºä¸ºå¤å°" ```
 å¬åæ¨é ```text æ·»å æ¹èæ¨éç¾¤ / ADDGROUP =>
 æ·»å èªå¨æ¨éçç¾¤å· å é¤æ¹èæ¨éç¾¤ / DELGROUP =>
 å é¤èªå¨æ¨éçç¾¤å· æ¥çæ¹èæ¨éç¾¤ / GETGROUP =>
-æ¥çèªå¨æ¨éçç¾¤å· ```  # å¾çç¤ºä¾  ç¹å»å±å¼ ## å¾çä»¬
+æ¥çèªå¨æ¨éçç¾¤å· ``` MAA ä½ä¸ç«ç¸å³ ```text maaæ·»å è®¢é /
+ADDMAA [å³é®è¯1 å³é®è¯2 ...] => æ·»å èªå¨æ¨éçå³é®è¯
+maaå é¤è®¢é / DELMAA [å³é®è¯1 å³é®è¯2 ...] =>
+å é¤èªå¨æ¨éçå³é®è¯ maaæ¥çè®¢é / GETMAA =>
+æ¥çæ¬ç¾¤èªå¨æ¨éçå³é®è¯ maaæ¥ä½ä¸ [å³é®è¯1 å³é®è¯2 ...]
+=> æå³é®è¯ç»åæ¥ä½ä¸ï¼é»è®¤ä¸ºææ°åå¸çç¬¬ä¸ä¸ªä½ä¸
+maaæ¥ä½ä¸ [å³é®è¯1 å³é®è¯2 ...] | [ç­åº¦/ææ°/è®¿é®] =>
+åä¸ï¼ä¸è¿å¯ä»¥æå®æä»ä¹é¡ºåºæ¥è¯¢ ```  # å¾çç¤ºä¾
+ç¹å»å±å¼ ## å¾çä»¬
 [https://user-images.githubusercontent.com/52584526/218328291-2324ea20-74c4-
 4182-81ed-4b74950c3ef9.png]
 [https://user-images.githubusercontent.com/52584526/218328307-f71e08ff-2370-
 4fb9-8898-c76f7e06a168.png]
 [https://user-images.githubusercontent.com/52584526/218328316-9259d9e6-6c2f-
 40e9-87bd-cee68da240e2.png]
 [https://user-images.githubusercontent.com/52584526/218328320-9ee76c53-dcf2-
@@ -113,16 +150,47 @@
 [ææ¥æ¹èå¸¸ç¨ç´ æåº](https://github.com/yuanyan3060/Arknights-Bot-
 Resource)__ - __[Kengxxiao](https://github.com/Kengxxiao)__ ç __
 [ãææ¥æ¹èãæ¸¸ææ°æ®åº](https://github.com/Kengxxiao/
 ArknightsGameData)__ - __[Aceship](https://github.com/Aceship)__ ç __
 [Arknight-Images](https://github.com/Aceship/Arknight-Images)__ - __[AmiyaBot]
 (https://github.com/AmiyaBot)__ ç __[Amiya-bot](https://github.com/AmiyaBot/
 Amiya-Bot)__ - __[Strelizia02](https://github.com/Strelizia02)__ ç __
-[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__ # æ´æ°æ¥å¿
-ç¹å»å±å¼ > 2023-02-19 v1.0.9 > - æ·»å å®æ¶ä»»å¡éç½®é¡¹ > -
+[AngelinaBot](https://github.com/Strelizia02/AngelinaBot)__ - __
+[MaaAssistantArknights](https://github.com/MaaAssistantArknights)__ ç __[MAA]
+(https://github.com/MaaAssistantArknights/MaaAssistantArknights)__ #
+æ´æ°æ¥å¿  ç¹å»å±å¼ > 2023-04-15 v1.1.0 > -
+å¬ææ¥è¯¢ãçå¹²åãçæºæéç°å¨åå¯ä»¥ç§èè¿è¡
+(ä¸æ¨èï¼ç§èåæ¶æ¯å¯è½å¯¼è´é£æ§) > -
+ç®æä¿®å¤äºä¸å¶å®åç¨ Tortoise-ORM çæä»¶åå§åå²çªçé®é¢
+[@zx-issue/15](https://github.com/NumberSir/zhenxun_arktools/issues/15) > -
+æ·»å å¨ç¾¤èæ¥è¯¢ãè®¢éãæ¨é [MAA ä½ä¸ç«](https://
+prts.plus)ä½ä¸çåè½ > -
+ä¿®å¤äºæ´æ°æ°æ®åºä¸­æå¼ è¡¨æ ¼æ¶ä¼å é¤ææè¡¨æ ¼çé®é¢ > >
+2023-04-08 v1.0.20 > -
+ä¿®å¤å ç´ æåºæ´æ°æ»åå¯¼è´æ æ³æ¥çå¹²åçé®é¢ > > 2023-04-07
+v1.0.19 > - ä¿®å¤æ´æ°æ°æ®åºå½ä»¤ä¸ä¼å¼ºå¶è¦çæ´æ°çé®é¢ > >
+2023-04-06 v1.0.18 > -
+ä¿®å¤äºèèæ´æ°æ°æ®ç»æå¯¼è´çåå»ºè¡¨åéè¯¯ > > 2023-04-04
+v1.0.17 > -
+æ·»å æ°æ®åºåå§åæ£æ¥ï¼ä¸åæ¯æ¬¡å¯å¨botæ¶éå¤åå»º > -
+æ·»å æ¯æ¬¡å¯å¨botæ¶çæ°æ®æ´æ°æ£æ¥å¼å³ï¼é»è®¤å¯ç¨ [@issue/39]
+(https://github.com/NumberSir/nonebot_plugin_arktools/issues/39) > > 2023-03-28
+v1.0.15 > - çå¹²åä¸å¹²åä¿¡æ¯åè½å¯ä»¥ä½¿ç¨å¹²åæµç§°
+(å¯èªè¡å¢å æ¹æ¥) > > 2023-03-24 v1.0.14 > -
+ä¿®å¤é¿ç±³å¨ä¸è¿å«é¿ç±³å¨å²çªçé®é¢ [@zx-issue/13](https://
+github.com/NumberSir/zhenxun_arktools/issues/13) > > 2023-03-08 v1.0.12 > -
+æ·»å  rsshub ä»£çéç½®é¡¹ [@issue/34](https://github.com/NumberSir/
+nonebot_plugin_arktools/issues/34) > - ä¿®å¤å¬æå½ä»¤ä¸å¤ççé®é¢
+[@issue/35](https://github.com/NumberSir/nonebot_plugin_arktools/issues/35) > -
+æ·»å æ¹èç´ æ/èµæºè·¯å¾éç½®é¡¹ï¼ç°å¨é»è®¤å¨æºå¨äººæ ¹ç®å½ä¸
+`data/arktools` æä»¶å¤¹ [@issue/36](https://github.com/NumberSir/
+nonebot_plugin_arktools/issues/36) > -
+ä¿®å¤æ¥è¯¢æ®è½å¹²åä¿¡æ¯æ¶ä¼éä¸­ç©ºç½æ®è½çé®é¢ > > 2023-02-20
+v1.0.11 > - ä¿®å¤ææ°çæ¬æ£æµåºéçé®é¢ > > 2023-02-19 v1.0.9 > -
+æ·»å å®æ¶ä»»å¡éç½®é¡¹ > -
 ä¿®å¤å®æ¶ä»»å¡å¯¼è´å¶å®å¤çå¨é»å¡çé®é¢ [@issue/30](https://
 github.com/NumberSir/nonebot_plugin_arktools/issues/30) [@zx-issue/9](https://
 github.com/NumberSir/zhenxun_arktools/issues/9) > -
 ä¿®å¤çå¹²åæ æ³å¤æ­éå¤ççé®é¢ [@zx-issue/10](https://
 github.com/NumberSir/zhenxun_arktools/issues/10) > -
 ä¿®å¤çå¹²åç»æå¾ä¸æé¡ºåºç»å¶çé®é¢ > > 2023-02-16 v1.0.8 > -
 ç§»é¤ `nb plugin install` å®è£å½ä»¤ï¼æ æ³è¯å«ææ°çæ¬å· [@issue/
```

### Comparing `nonebot_plugin_arktools-1.0.9/nonebot_plugin_arktools.egg-info/SOURCES.txt` & `nonebot_plugin_arktools-1.1.0/nonebot_plugin_arktools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,41 +6,45 @@
 nonebot_plugin_arktools.egg-info/SOURCES.txt
 nonebot_plugin_arktools.egg-info/dependency_links.txt
 nonebot_plugin_arktools.egg-info/requires.txt
 nonebot_plugin_arktools.egg-info/top_level.txt
 nonebot_plugin_arktools/src/__init__.py
 nonebot_plugin_arktools/src/help.py
 nonebot_plugin_arktools/src/configs/__init__.py
+nonebot_plugin_arktools/src/configs/draw_config.py
 nonebot_plugin_arktools/src/configs/ocr_config.py
 nonebot_plugin_arktools/src/configs/path_config.py
 nonebot_plugin_arktools/src/configs/proxy_config.py
 nonebot_plugin_arktools/src/configs/scheduler_config.py
 nonebot_plugin_arktools/src/core/__init__.py
 nonebot_plugin_arktools/src/core/models_v3.py
 nonebot_plugin_arktools/src/core/database/__init__.py
 nonebot_plugin_arktools/src/core/database/game_sqlite.py
 nonebot_plugin_arktools/src/core/database/plugin_sqlite.py
 nonebot_plugin_arktools/src/exceptions/__init__.py
+nonebot_plugin_arktools/src/game_draw_card/__init__.py
 nonebot_plugin_arktools/src/game_guess_operator/__init__.py
 nonebot_plugin_arktools/src/game_guess_operator/data_source.py
 nonebot_plugin_arktools/src/misc_monster_siren/__init__.py
 nonebot_plugin_arktools/src/misc_monster_siren/data_source.py
 nonebot_plugin_arktools/src/misc_operator_birthday/__init__.py
 nonebot_plugin_arktools/src/tool_announce_push/__init__.py
 nonebot_plugin_arktools/src/tool_announce_push/data_source.py
+nonebot_plugin_arktools/src/tool_fetch_maa_copilot/__init__.py
+nonebot_plugin_arktools/src/tool_fetch_maa_copilot/data_source.py
 nonebot_plugin_arktools/src/tool_open_recruitment/__init__.py
 nonebot_plugin_arktools/src/tool_open_recruitment/data_source.py
 nonebot_plugin_arktools/src/tool_operator_info/__init__.py
 nonebot_plugin_arktools/src/tool_operator_info/data_source.py
 nonebot_plugin_arktools/src/tool_sanity_notify/__init__.py
 nonebot_plugin_arktools/src/utils/__init__.py
 nonebot_plugin_arktools/src/utils/database.py
 nonebot_plugin_arktools/src/utils/general.py
 nonebot_plugin_arktools/src/utils/image.py
 nonebot_plugin_arktools/src/utils/update.py
 nonebot_plugin_arktools/test/__init__.py
 nonebot_plugin_arktools/test/test_database_utils.py
-nonebot_plugin_arktools/test/test_models_v3.py
+nonebot_plugin_arktools/test/test_models.py
 nonebot_plugin_arktools/test/test_open_recruitment.py
 nonebot_plugin_arktools/test/test_operator_info.py
 nonebot_plugin_arktools/test/test_update_utils.py
 nonebot_plugin_arktools/test/utils.py
```

### Comparing `nonebot_plugin_arktools-1.0.9/setup.py` & `nonebot_plugin_arktools-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name="nonebot_plugin_arktools",
-    version="1.0.9",
+    version="1.1.0",
     author="Number_Sir",
     author_email="Number_Sir@126.com",
     keywords=["pip", "nonebot2", "nonebot", "nonebot_plugin"],
     description="""基于 OneBot 适配器的 NoneBot2 明日方舟小工具箱插件""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NumberSir/nonebot_plugin_arktools",
@@ -23,18 +23,18 @@
     ],
     include_package_data=True,
     platforms="any",
     install_requires=[
         'nonebot-adapter-onebot>=2.2.0',
         'nonebot2>=2.0.0rc2',
         'nonebot-plugin-apscheduler>=0.2.0',
-        'nonebot-plugin-imageutils>=0.1.14'
+        'nonebot-plugin-imageutils>=0.1.14',
         'nonebot-plugin-htmlrender>=0.2.0.1',
 
         'httpx>=0.23.1',
         'aiofiles>=0.8.0',
         'tortoise-orm>=0.19.3',
-        'lxml>=4.9.2'
+        'lxml>=4.9.2',
         'feedparser>=6.0.10',
     ],
     python_requires=">=3.8"
 )
```

