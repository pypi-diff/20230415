# Comparing `tmp/nonebot_plugin_gshisbanner-0.4.7.tar.gz` & `tmp/nonebot_plugin_gshisbanner-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-0.4.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-0.4.8.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-0.4.7.tar` & `nonebot_plugin_gshisbanner-0.4.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/LICENSE
--rw-r--r--   0        0        0     4443 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/README.md
--rw-r--r--   0        0        0      241 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0     1030 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      406 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      292 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0     3663 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1182 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     4509 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/main.py
--rw-r--r--   0        0        0     2654 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0      576 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/LICENSE
+-rw-r--r--   0        0        0     4443 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/README.md
+-rw-r--r--   0        0        0      389 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0     1030 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      406 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      292 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0     3663 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1182 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     4509 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/main.py
+-rw-r--r--   0        0        0     2654 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0      576 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     5136 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.4.8/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-0.4.7/LICENSE` & `nonebot_plugin_gshisbanner-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.7/README.md` & `nonebot_plugin_gshisbanner-0.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/forchannot/nonebot-plugin-gshisbanner.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-gshisbanner">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-gshisbanner.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
 本插件用于在机器人上查询原神历史卡池信息
```

### Comparing `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/main.py` & `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/send.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.7/PKG-INFO` & `nonebot_plugin_gshisbanner-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 0.4.7
+Version: 0.4.8
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1,<3.0)
 Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0)
 Description-Content-Type: text/markdown
@@ -30,15 +31,15 @@
 
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/forchannot/nonebot-plugin-gshisbanner.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-gshisbanner">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-gshisbanner.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
 ## 📖 介绍
 
 本插件用于在机器人上查询原神历史卡池信息
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.4.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.4.8 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
-Author-email: yy320206@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
+Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-
-adapter-onebot (>=2.1,<3.0) Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0)
-Description-Content-Type: text/markdown
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.1,<3.0) Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0) Description-Content-
+Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-gshisbanner _â¨
  æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ â¨_ [license]
                                 [pypi] [python]
 ## ð ä»ç» æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ ##
 ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
```

