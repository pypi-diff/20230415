# Comparing `tmp/openhasp_config_manager-0.4.7.tar.gz` & `tmp/openhasp_config_manager-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhasp_config_manager-0.4.7.tar", max compression
+gzip compressed data, was "openhasp_config_manager-0.4.8.tar", max compression
```

## Comparing `openhasp_config_manager-0.4.7.tar` & `openhasp_config_manager-0.4.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    34523 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/LICENSE
--rw-r--r--   0        0        0    13491 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/README.md
--rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/__init__.py
--rw-r--r--   0        0        0    11950 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/__init__.py
--rw-r--r--   0        0        0      746 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/cmd.py
--rw-r--r--   0        0        0     3473 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/common.py
--rw-r--r--   0        0        0     1231 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/deploy.py
--rw-r--r--   0        0        0     1044 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/generate.py
--rw-r--r--   0        0        0     1152 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/listen.py
--rw-r--r--   0        0        0      972 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/logs.py
--rw-r--r--   0        0        0     1292 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/screenshot.py
--rw-r--r--   0        0        0     1023 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/shell.py
--rw-r--r--   0        0        0     1056 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/state.py
--rw-r--r--   0        0        0     1072 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/upload.py
--rw-r--r--   0        0        0     1265 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/vars.py
--rw-r--r--   0        0        0      257 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli.py
--rw-r--r--   0        0        0      153 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/const.py
--rw-r--r--   0        0        0    16151 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/manager.py
--rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/__init__.py
--rw-r--r--   0        0        0     1819 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/image_processor.py
--rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/__init__.py
--rw-r--r--   0        0        0      229 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/component.py
--rw-r--r--   0        0        0      958 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/config.py
--rw-r--r--   0        0        0      164 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/debug_config.py
--rw-r--r--   0        0        0      362 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/device.py
--rw-r--r--   0        0        0      190 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/device_config.py
--rw-r--r--   0        0        0      224 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/gui_config.py
--rw-r--r--   0        0        0      178 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/hasp_config.py
--rw-r--r--   0        0        0      111 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/http_config.py
--rw-r--r--   0        0        0      154 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/mqtt_config.py
--rw-r--r--   0        0        0      193 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
--rw-r--r--   0        0        0       98 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/screen_config.py
--rw-r--r--   0        0        0       97 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/telnet_config.py
--rw-r--r--   0        0        0       85 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/website_config.py
--rw-r--r--   0        0        0       97 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/wifi_config.py
--rw-r--r--   0        0        0     2817 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/mqtt_client.py
--rw-r--r--   0        0        0    11756 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/openhasp.py
--rw-r--r--   0        0        0     4833 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/telnet_client.py
--rw-r--r--   0        0        0     8705 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/webservice_client.py
--rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/device_processor.py
--rw-r--r--   0        0        0      369 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/jsonl/__init__.py
--rw-r--r--   0        0        0     2198 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/jsonl/jsonl.py
--rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/preprocessor/__init__.py
--rw-r--r--   0        0        0     2479 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
--rw-r--r--   0        0        0     5401 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/template_rendering.py
--rw-r--r--   0        0        0     5464 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/variables.py
--rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/ui/__init__.py
--rw-r--r--   0        0        0     1427 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/ui/util.py
--rw-r--r--   0        0        0     6053 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/uploader.py
--rw-r--r--   0        0        0     1798 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/util.py
--rw-r--r--   0        0        0      565 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/__init__.py
--rw-r--r--   0        0        0      649 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/cmd.py
--rw-r--r--   0        0        0     1140 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/device_validator.py
--rw-r--r--   0        0        0     2111 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/jsonl.py
--rw-r--r--   0        0        0     1300 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    14707 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/LICENSE
+-rw-r--r--   0        0        0    13491 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/cmd.py
+-rw-r--r--   0        0        0     3473 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/common.py
+-rw-r--r--   0        0        0     1231 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/deploy.py
+-rw-r--r--   0        0        0     1044 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/generate.py
+-rw-r--r--   0        0        0     1152 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/listen.py
+-rw-r--r--   0        0        0      972 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/logs.py
+-rw-r--r--   0        0        0     1292 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/screenshot.py
+-rw-r--r--   0        0        0     1023 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/shell.py
+-rw-r--r--   0        0        0     1056 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/state.py
+-rw-r--r--   0        0        0     1072 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/upload.py
+-rw-r--r--   0        0        0     1265 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/vars.py
+-rw-r--r--   0        0        0      257 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli.py
+-rw-r--r--   0        0        0      153 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/const.py
+-rw-r--r--   0        0        0    16151 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/manager.py
+-rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/__init__.py
+-rw-r--r--   0        0        0     1819 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/image_processor.py
+-rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/__init__.py
+-rw-r--r--   0        0        0      229 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/component.py
+-rw-r--r--   0        0        0      958 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/config.py
+-rw-r--r--   0        0        0      164 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/debug_config.py
+-rw-r--r--   0        0        0      362 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/device.py
+-rw-r--r--   0        0        0      190 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/device_config.py
+-rw-r--r--   0        0        0      224 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/gui_config.py
+-rw-r--r--   0        0        0      178 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/hasp_config.py
+-rw-r--r--   0        0        0      111 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/http_config.py
+-rw-r--r--   0        0        0      154 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/mqtt_config.py
+-rw-r--r--   0        0        0      193 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
+-rw-r--r--   0        0        0       98 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/screen_config.py
+-rw-r--r--   0        0        0       97 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/telnet_config.py
+-rw-r--r--   0        0        0       85 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/website_config.py
+-rw-r--r--   0        0        0       97 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/wifi_config.py
+-rw-r--r--   0        0        0     4033 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/mqtt_client.py
+-rw-r--r--   0        0        0    12037 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/openhasp.py
+-rw-r--r--   0        0        0     4833 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/telnet_client.py
+-rw-r--r--   0        0        0     8705 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/webservice_client.py
+-rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/device_processor.py
+-rw-r--r--   0        0        0      369 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/jsonl/__init__.py
+-rw-r--r--   0        0        0     2198 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/jsonl/jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/preprocessor/__init__.py
+-rw-r--r--   0        0        0     2479 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
+-rw-r--r--   0        0        0     5401 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/template_rendering.py
+-rw-r--r--   0        0        0     5464 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/variables.py
+-rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/ui/__init__.py
+-rw-r--r--   0        0        0     1427 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/ui/util.py
+-rw-r--r--   0        0        0     6053 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/uploader.py
+-rw-r--r--   0        0        0     1798 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/util.py
+-rw-r--r--   0        0        0      565 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/__init__.py
+-rw-r--r--   0        0        0      649 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/cmd.py
+-rw-r--r--   0        0        0     1140 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/device_validator.py
+-rw-r--r--   0        0        0     2111 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/jsonl.py
+-rw-r--r--   0        0        0     1300 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0    14707 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.8/PKG-INFO
```

### Comparing `openhasp_config_manager-0.4.7/LICENSE` & `openhasp_config_manager-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/README.md` & `openhasp_config_manager-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/__init__.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/cmd.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/common.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/common.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/deploy.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/generate.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/generate.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/listen.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/listen.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/logs.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/logs.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/screenshot.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/screenshot.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/shell.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/shell.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/state.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/state.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/upload.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/upload.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/vars.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/vars.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/manager.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/manager.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/image_processor.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/image_processor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/config.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/config.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/openhasp.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/openhasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,22 @@
         Set the text of an object
         :param obj: the object to set the text for
         :param text: the text to set
         """
         await self.set_object_properties(obj, {"text": text})
 
     async def set_image(
-            self,
-            obj: str,
-            image,
-            access_host: str,
-            listen_host: str = "0.0.0.0",
-            timeout: int = 10,
-            size: Tuple[int or None, int or None] = (None, None),
-            fitscreen: bool = False,
+        self,
+        obj: str,
+        image,
+        access_host: str,
+        listen_host: str = "0.0.0.0",
+        timeout: int = 10,
+        size: Tuple[int or None, int or None] = (None, None),
+        fitscreen: bool = False,
     ):
         """
         Sets the image of an object.
         If the image is a URL, it will be fetched first.
         The image will then be converted to RGB565 and
         served by a temporary webserver for the plate to fetch it.
 
@@ -247,14 +247,21 @@
         Listen to OpenHASP events related to this device
         :param path: MQTT subpath to listen to
         :param callback: callback to call when a matching event is received
         """
         topic = f"hasp/{self._device.config.mqtt.name}/{path}"
         await self._mqtt_client.subscribe(topic, callback)
 
+    async def cancel_callback(self, callback: Callable = None):
+        """
+        Cancel a callback which was previously registered, f.ex. via listen_event (or listen_state)
+        :param callback: the specific callback to cancel
+        """
+        await self._mqtt_client.cancel_callback(callback=callback)
+
     async def command(self, name: str, params: any):
         """
         Execute a command on a device
         :param name: the name of the command
         :param params: parameters for the command
         """
         topic = f"hasp/{self._device.config.mqtt.name}/command/{name}"
```

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/telnet_client.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/telnet_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/webservice_client.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/webservice_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/device_processor.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/device_processor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/jsonl/jsonl.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/jsonl/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/template_rendering.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/template_rendering.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/variables.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/variables.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/ui/util.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/ui/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/uploader.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/uploader.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/util.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/__init__.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/cmd.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/device_validator.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/device_validator.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/jsonl.py` & `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.7/pyproject.toml` & `openhasp_config_manager-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openhasp-config-manager"
-version = "0.4.7"
+version = "0.4.8"
 description = "A tool to manage all of your openHASP device configs in a centralized place."
 
 license = "AGPL-3.0-or-later"
 
 authors = [
     "Markus Ressel <mail@markusressel.de>",
 ]
```

### Comparing `openhasp_config_manager-0.4.7/PKG-INFO` & `openhasp_config_manager-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhasp-config-manager
-Version: 0.4.7
+Version: 0.4.8
 Summary: A tool to manage all of your openHASP device configs in a centralized place.
 Home-page: https://github.com/markusressel/openhasp-config-manager
 License: AGPL-3.0-or-later
 Keywords: openhasp,config,management
 Author: Markus Ressel
 Author-email: mail@markusressel.de
 Requires-Python: >=3.10,<4.0
```

