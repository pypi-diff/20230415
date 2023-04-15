# Comparing `tmp/openhasp_config_manager-0.4.6.tar.gz` & `tmp/openhasp_config_manager-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhasp_config_manager-0.4.6.tar", max compression
+gzip compressed data, was "openhasp_config_manager-0.4.7.tar", max compression
```

## Comparing `openhasp_config_manager-0.4.6.tar` & `openhasp_config_manager-0.4.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    34523 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/LICENSE
--rw-r--r--   0        0        0    13491 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/README.md
--rw-r--r--   0        0        0        0 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/__init__.py
--rw-r--r--   0        0        0    11950 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/__init__.py
--rw-r--r--   0        0        0      746 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/cmd.py
--rw-r--r--   0        0        0     3473 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/common.py
--rw-r--r--   0        0        0     1231 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/deploy.py
--rw-r--r--   0        0        0     1044 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/generate.py
--rw-r--r--   0        0        0     1152 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/listen.py
--rw-r--r--   0        0        0      972 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/logs.py
--rw-r--r--   0        0        0     1292 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/screenshot.py
--rw-r--r--   0        0        0     1023 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/shell.py
--rw-r--r--   0        0        0     1056 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/state.py
--rw-r--r--   0        0        0     1072 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/upload.py
--rw-r--r--   0        0        0     1265 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli/vars.py
--rw-r--r--   0        0        0      257 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/cli.py
--rw-r--r--   0        0        0      153 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/const.py
--rw-r--r--   0        0        0    16151 2023-04-15 00:04:00.522458 openhasp_config_manager-0.4.6/openhasp_config_manager/manager.py
--rw-r--r--   0        0        0        0 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/__init__.py
--rw-r--r--   0        0        0     1819 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/image_processor.py
--rw-r--r--   0        0        0        0 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/__init__.py
--rw-r--r--   0        0        0      229 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/component.py
--rw-r--r--   0        0        0      958 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/config.py
--rw-r--r--   0        0        0      164 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/debug_config.py
--rw-r--r--   0        0        0      362 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/device.py
--rw-r--r--   0        0        0      190 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/device_config.py
--rw-r--r--   0        0        0      224 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/gui_config.py
--rw-r--r--   0        0        0      178 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/hasp_config.py
--rw-r--r--   0        0        0      111 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/http_config.py
--rw-r--r--   0        0        0      154 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/mqtt_config.py
--rw-r--r--   0        0        0      193 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
--rw-r--r--   0        0        0       98 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/screen_config.py
--rw-r--r--   0        0        0       97 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/telnet_config.py
--rw-r--r--   0        0        0       85 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/website_config.py
--rw-r--r--   0        0        0       97 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/wifi_config.py
--rw-r--r--   0        0        0     1588 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/mqtt_client.py
--rw-r--r--   0        0        0    11756 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/openhasp.py
--rw-r--r--   0        0        0     4833 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/telnet_client.py
--rw-r--r--   0        0        0     8705 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/webservice_client.py
--rw-r--r--   0        0        0        0 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/device_processor.py
--rw-r--r--   0        0        0      369 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/jsonl/__init__.py
--rw-r--r--   0        0        0     2198 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/jsonl/jsonl.py
--rw-r--r--   0        0        0        0 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/preprocessor/__init__.py
--rw-r--r--   0        0        0     2479 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
--rw-r--r--   0        0        0     5401 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/template_rendering.py
--rw-r--r--   0        0        0     5464 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/processing/variables.py
--rw-r--r--   0        0        0        0 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/ui/__init__.py
--rw-r--r--   0        0        0     1427 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/ui/util.py
--rw-r--r--   0        0        0     6053 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/uploader.py
--rw-r--r--   0        0        0     1798 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/util.py
--rw-r--r--   0        0        0      565 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/validation/__init__.py
--rw-r--r--   0        0        0      649 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/validation/cmd.py
--rw-r--r--   0        0        0     1140 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/validation/device_validator.py
--rw-r--r--   0        0        0     2111 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/openhasp_config_manager/validation/jsonl.py
--rw-r--r--   0        0        0     1300 2023-04-15 00:04:00.526458 openhasp_config_manager-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    14707 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/LICENSE
+-rw-r--r--   0        0        0    13491 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/cmd.py
+-rw-r--r--   0        0        0     3473 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/common.py
+-rw-r--r--   0        0        0     1231 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/deploy.py
+-rw-r--r--   0        0        0     1044 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/generate.py
+-rw-r--r--   0        0        0     1152 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/listen.py
+-rw-r--r--   0        0        0      972 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/logs.py
+-rw-r--r--   0        0        0     1292 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/screenshot.py
+-rw-r--r--   0        0        0     1023 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/shell.py
+-rw-r--r--   0        0        0     1056 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/state.py
+-rw-r--r--   0        0        0     1072 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/upload.py
+-rw-r--r--   0        0        0     1265 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli/vars.py
+-rw-r--r--   0        0        0      257 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/cli.py
+-rw-r--r--   0        0        0      153 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/const.py
+-rw-r--r--   0        0        0    16151 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/manager.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/__init__.py
+-rw-r--r--   0        0        0     1819 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/image_processor.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/__init__.py
+-rw-r--r--   0        0        0      229 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/component.py
+-rw-r--r--   0        0        0      958 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/config.py
+-rw-r--r--   0        0        0      164 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/debug_config.py
+-rw-r--r--   0        0        0      362 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/device.py
+-rw-r--r--   0        0        0      190 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/device_config.py
+-rw-r--r--   0        0        0      224 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/gui_config.py
+-rw-r--r--   0        0        0      178 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/hasp_config.py
+-rw-r--r--   0        0        0      111 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/http_config.py
+-rw-r--r--   0        0        0      154 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/mqtt_config.py
+-rw-r--r--   0        0        0      193 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
+-rw-r--r--   0        0        0       98 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/screen_config.py
+-rw-r--r--   0        0        0       97 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/telnet_config.py
+-rw-r--r--   0        0        0       85 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/website_config.py
+-rw-r--r--   0        0        0       97 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/wifi_config.py
+-rw-r--r--   0        0        0     2817 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/mqtt_client.py
+-rw-r--r--   0        0        0    11756 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/openhasp.py
+-rw-r--r--   0        0        0     4833 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/telnet_client.py
+-rw-r--r--   0        0        0     8705 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/webservice_client.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/device_processor.py
+-rw-r--r--   0        0        0      369 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/jsonl/__init__.py
+-rw-r--r--   0        0        0     2198 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/jsonl/jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/preprocessor/__init__.py
+-rw-r--r--   0        0        0     2479 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
+-rw-r--r--   0        0        0     5401 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/template_rendering.py
+-rw-r--r--   0        0        0     5464 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/processing/variables.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/ui/__init__.py
+-rw-r--r--   0        0        0     1427 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/ui/util.py
+-rw-r--r--   0        0        0     6053 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/uploader.py
+-rw-r--r--   0        0        0     1798 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/util.py
+-rw-r--r--   0        0        0      565 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/__init__.py
+-rw-r--r--   0        0        0      649 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/cmd.py
+-rw-r--r--   0        0        0     1140 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/device_validator.py
+-rw-r--r--   0        0        0     2111 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/openhasp_config_manager/validation/jsonl.py
+-rw-r--r--   0        0        0     1300 2023-04-15 01:02:20.839903 openhasp_config_manager-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    14707 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.7/PKG-INFO
```

### Comparing `openhasp_config_manager-0.4.6/LICENSE` & `openhasp_config_manager-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/README.md` & `openhasp_config_manager-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/__init__.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/cmd.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/common.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/common.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/deploy.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/generate.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/generate.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/listen.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/listen.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/logs.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/logs.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/screenshot.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/screenshot.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/shell.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/shell.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/state.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/state.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/upload.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/upload.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/cli/vars.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/cli/vars.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/manager.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/manager.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/image_processor.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/image_processor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/model/config.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/model/config.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/mqtt_client.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/mqtt_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,76 @@
 import asyncio
 import json
 import uuid
-from typing import Callable
+from typing import Callable, List, Dict
 
-from asyncio_mqtt import Client
+from asyncio_mqtt import Client, Message
 
 
 class MqttClient:
 
     def __init__(self, host: str, port: int, mqtt_user: str, mqtt_password: str):
         self._mqtt_client_id = 'openhasp-config-manager'
         self._host = host
         self._port = port
         self._mqtt_user = mqtt_user
         self._mqtt_password = mqtt_password
         self._reconnect_interval_seconds = 5
 
+        self._mqtt_client_task: asyncio.Task = None
+        self._callbacks: Dict[str, List[callable]] = {}
         self.__mqtt_client: Client = None
 
     async def publish(self, topic: str, payload: any):
         async with self._create_mqtt_client() as client:
             if isinstance(payload, dict):
                 payload = json.dumps(payload)
 
             await client.publish(topic, payload=payload)
 
     async def subscribe(self, topic: str, callback: Callable):
-        try:
-            async with self._create_mqtt_client() as client:
-                async with client.messages() as messages:
-                    await client.subscribe(topic)
-                    async for message in messages:
-                        await callback(message.topic, message.payload)
-        except Exception as ex:
-            print(f'Error: {ex}; Reconnecting in {self._reconnect_interval_seconds} seconds ...')
-            await asyncio.sleep(self._reconnect_interval_seconds)
+        if topic not in self._callbacks:
+            self._callbacks[topic] = []
+        if callback not in self._callbacks[topic]:
+            self._callbacks[topic].append(callback)
+
+        if self._callbacks:
+            await self._start_mqtt_client_task()
+        else:
+            await self._stop_mqtt_client_task()
 
     def _create_mqtt_client(self) -> Client:
         return Client(
             hostname=self._host,
             port=self._port,
             username=self._mqtt_user,
             password=self._mqtt_password,
             client_id=f"{self._mqtt_client_id}-{uuid.uuid4()}",
         )
+
+    async def _start_mqtt_client_task(self):
+        if self._mqtt_client_task is None:
+            self._mqtt_client_task = asyncio.create_task(self._mqtt_client_task_function())
+
+    async def _stop_mqtt_client_task(self):
+        if self._mqtt_client_task is not None:
+            self._mqtt_client_task.cancel()
+            self._mqtt_client_task = None
+
+    async def _mqtt_client_task_function(self):
+        while True:
+            try:
+                async with self._create_mqtt_client() as client:
+                    async with client.messages() as messages:
+                        await client.subscribe("hasp/#")
+                        async for message in messages:
+                            await self._handle_message(message)
+            except Exception as ex:
+                # TODO: use logger instead of print
+                print(f'Error: {ex}; Reconnecting in {self._reconnect_interval_seconds} seconds ...')
+                await asyncio.sleep(self._reconnect_interval_seconds)
+
+    async def _handle_message(self, message: Message):
+        for topic, callbacks in self._callbacks.items():
+            if message.topic.matches(topic):
+                for callback in callbacks:
+                    await callback(message.topic, message.payload)
```

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/openhasp.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/openhasp.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/telnet_client.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/telnet_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/openhasp_client/webservice_client.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/openhasp_client/webservice_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/processing/device_processor.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/device_processor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/processing/jsonl/jsonl.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/jsonl/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/processing/template_rendering.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/template_rendering.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/processing/variables.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/processing/variables.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/ui/util.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/ui/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/uploader.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/uploader.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/util.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/validation/__init__.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/validation/cmd.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/validation/device_validator.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/device_validator.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/openhasp_config_manager/validation/jsonl.py` & `openhasp_config_manager-0.4.7/openhasp_config_manager/validation/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.6/pyproject.toml` & `openhasp_config_manager-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openhasp-config-manager"
-version = "0.4.6"
+version = "0.4.7"
 description = "A tool to manage all of your openHASP device configs in a centralized place."
 
 license = "AGPL-3.0-or-later"
 
 authors = [
     "Markus Ressel <mail@markusressel.de>",
 ]
```

### Comparing `openhasp_config_manager-0.4.6/PKG-INFO` & `openhasp_config_manager-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhasp-config-manager
-Version: 0.4.6
+Version: 0.4.7
 Summary: A tool to manage all of your openHASP device configs in a centralized place.
 Home-page: https://github.com/markusressel/openhasp-config-manager
 License: AGPL-3.0-or-later
 Keywords: openhasp,config,management
 Author: Markus Ressel
 Author-email: mail@markusressel.de
 Requires-Python: >=3.10,<4.0
```

