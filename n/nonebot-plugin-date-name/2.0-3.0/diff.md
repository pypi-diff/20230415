# Comparing `tmp/nonebot_plugin_date_name-2.0.tar.gz` & `tmp/nonebot_plugin_date_name-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_date_name-2.0.tar", last modified: Wed Jul 27 01:48:53 2022, max compression
+gzip compressed data, was "nonebot_plugin_date_name-3.0.tar", last modified: Sat Apr 15 09:05:52 2023, max compression
```

## Comparing `nonebot_plugin_date_name-2.0.tar` & `nonebot_plugin_date_name-3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-07-27 01:48:53.390184 nonebot_plugin_date_name-2.0/
--rw-rw-rw-   0        0        0      343 2022-07-27 01:48:53.389195 nonebot_plugin_date_name-2.0/PKG-INFO
--rw-rw-rw-   0        0        0      901 2022-07-22 14:24:59.000000 nonebot_plugin_date_name-2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-07-27 01:48:53.373467 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name/
--rw-rw-rw-   0        0        0      834 2022-07-27 01:47:16.000000 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name/__init__.py
--rw-rw-rw-   0        0        0     2145 2022-07-22 14:21:16.000000 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name/config.py
-drwxrwxrwx   0        0        0        0 2022-07-27 01:48:53.385178 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name.egg-info/
--rw-rw-rw-   0        0        0      343 2022-07-27 01:48:53.000000 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2022-07-27 01:48:53.000000 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-27 01:48:53.000000 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2022-07-27 01:48:53.000000 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2022-07-27 01:48:53.000000 nonebot_plugin_date_name-2.0/nonebot_plugin_date_name.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-27 01:48:53.391183 nonebot_plugin_date_name-2.0/setup.cfg
--rw-rw-rw-   0        0        0      612 2022-07-27 01:47:37.000000 nonebot_plugin_date_name-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:05:52.960296 nonebot_plugin_date_name-3.0/
+-rw-rw-rw-   0        0        0      293 2023-04-15 09:05:52.958319 nonebot_plugin_date_name-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-04-15 08:41:47.000000 nonebot_plugin_date_name-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 09:05:52.923320 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name/
+-rw-rw-rw-   0        0        0      688 2023-04-15 08:41:47.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name/__init__.py
+-rw-rw-rw-   0        0        0     1903 2023-04-15 08:56:49.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name/config.py
+-rw-rw-rw-   0        0        0     8192 2023-04-15 08:43:52.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name/name.db
+drwxrwxrwx   0        0        0        0 2023-04-15 09:05:52.951305 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name.egg-info/
+-rw-rw-rw-   0        0        0      293 2023-04-15 09:05:52.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-04-15 09:05:52.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 09:05:52.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-15 09:05:52.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-15 09:05:52.000000 nonebot_plugin_date_name-3.0/nonebot_plugin_date_name.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 09:05:52.961297 nonebot_plugin_date_name-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-04-15 09:05:21.000000 nonebot_plugin_date_name-3.0/setup.py
```

### Comparing `nonebot_plugin_date_name-2.0/README.md` & `nonebot_plugin_date_name-3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
-# NoneBot-Plugin-Date-name
+# NoneBot-Plugin-Date-Name
 _✨ 一个可以群昵称显示现在时间的插件 ✨_
     <br></br>
 </div>
 
 ## 如何安装？如何下载？
 你可以使用 python中的pip
 ```bash
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                                    [nonebot]
-                        # NoneBot-Plugin-Date-name _â¨
+                        # NoneBot-Plugin-Date-Name _â¨
             ä¸ä¸ªå¯ä»¥ç¾¤æµç§°æ¾ç¤ºç°å¨æ¶é´çæä»¶ â¨_
 ## å¦ä½å®è£ï¼å¦ä½ä¸è½½ï¼ ä½ å¯ä»¥ä½¿ç¨ pythonä¸­çpip ```bash pip
 install nonebot-plugin-date-name ``` æènonebotéç ```bash nb plugin
 install nonebot-plugin-date-name ``` --- ## å¦ä½ä½¿ç¨ï¼
 ä»¥ä¸æ¯æä»¤åå®¹ä»¥åæ³¨é `/å³é­æ¶é´åå­
 ##å³é­æä»¶å¯¹ç¨æ·çä½ç¨` `/å¼å¯æ¶é´åå­
 ##å¼å¯æä»¶å¯¹ç¨æ·çä½ç¨` `/datenameæ´æ°ç¼å­
```

### Comparing `nonebot_plugin_date_name-2.0/nonebot_plugin_date_name/__init__.py` & `nonebot_plugin_date_name-3.0/nonebot_plugin_date_name/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-import json
 from nonebot import get_bot
 from nonebot_plugin_apscheduler import scheduler
 from . import config
 from datetime import datetime
 
 @scheduler.scheduled_job('interval', seconds=5)
 async def _():
         try:
             bot = get_bot()
-            for a in config.user:
-                user_id = json.loads(str(a).replace("'",'"'))
-                group_id = user_id[0]
-                user_id_2 = user_id[1]
-                now_time = str(config.id_nickname[user_id_2])+str(" ")+str(datetime.now().strftime("%A %p %Y-%m-%d %H:%M"))
+            for a in config.hashmap:
+                group_id = a[0]
+                user_id_2 = a[1]
+                now_time = f"{a[2]} "+str(datetime.now().strftime("%A %p %Y-%m-%d %H:%M"))
                 await bot.call_api(
                     "set_group_card",**{
                     'group_id':group_id,
                     'user_id':user_id_2,
                     'card':now_time})
         except(ValueError):
             pass
-            
-
```

### Comparing `nonebot_plugin_date_name-2.0/setup.py` & `nonebot_plugin_date_name-3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-
+﻿
  # -*- coding: utf-8 -*-
 import setuptools
 setuptools.setup(
     name = "nonebot_plugin_date_name",
-    version = "2.0",
+    version = "3.0",
     packages = setuptools.find_packages(),
     author="bingyue",
     author_email="hello-yiqiu@qq.com",
     description="""让你的群昵称显示现在时间""",
     url="https://github.com/bingqiu456/nonebot_plugin_date_name",
     install_requires=[
         "nonebot2>=2.0.0b2",
         "Pillow>=9.1.1",
         "nonebot-adapter-onebot>=2.0.0b1",
         "nonebot-plugin-apscheduler>=0.1.3"
     ],
     keywords=["nonebot_plugin_date_name","nonebot","nonebot_plugin"],
-)
+    package_data={
+        'nonebot_plugin_date_name':['name.db'],
+    }
+)
```

