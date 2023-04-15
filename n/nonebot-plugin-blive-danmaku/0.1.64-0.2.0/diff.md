# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.64.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.64.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.64.tar` & `nonebot_plugin_blive_danmaku-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,47 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.64/LICENSE
--rw-r--r--   0        0        0      127 2023-04-12 03:06:27.818661 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       99 2023-04-12 03:06:27.818661 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/__init__.py
--rw-r--r--   0        0        0     1409 2023-04-12 03:06:27.819656 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
--rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
--rw-r--r--   0        0        0     1107 2023-04-12 03:07:40.861965 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
--rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
--rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
--rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
--rw-r--r--   0        0        0     4597 2023-04-12 03:06:27.821658 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
--rw-r--r--   0        0        0     2131 2023-04-12 03:06:27.821658 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/subscribe/live.py
--rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/config.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     3168 2023-04-12 03:06:27.822659 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      969 2023-04-12 03:07:54.046045 nonebot_plugin_blive_danmaku-0.1.64/pyproject.toml
--rw-r--r--   0        0        0     2745 2023-04-12 03:06:27.817658 nonebot_plugin_blive_danmaku-0.1.64/README.md
--rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.64/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.2.0/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-15 08:11:11.487966 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-15 08:11:31.175376 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/__init__.py
+-rw-r--r--   0        0        0      418 2023-04-15 03:50:38.971502 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/config-758143a0.js
+-rw-r--r--   0        0        0   324273 2023-04-15 03:50:38.972505 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-d655f643.css
+-rw-r--r--   0        0        0   166073 2023-04-15 03:50:38.972505 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-f16563b7.js
+-rw-r--r--   0        0        0     3371 2023-04-15 03:50:38.972505 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-123dda7d.js
+-rw-r--r--   0        0        0     2755 2023-04-15 03:50:38.971502 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-8a1cc78a.css
+-rw-r--r--   0        0        0       51 2023-04-15 03:50:38.971502 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-a662ddb2.css
+-rw-r--r--   0        0        0     2798 2023-04-15 03:50:38.971502 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e1716a6f.js
+-rw-r--r--   0        0        0     2230 2023-04-15 03:50:38.971502 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e2ab3243.js
+-rw-r--r--   0        0        0    14578 2023-04-15 03:50:38.972505 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-a70ac895.js
+-rw-r--r--   0        0        0   216097 2023-04-15 03:50:38.972505 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b101ffcd.js
+-rw-r--r--   0        0        0    12014 2023-04-15 02:38:23.791948 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico
+-rw-r--r--   0        0        0      837 2023-04-15 03:50:38.972505 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/index.html
+-rw-r--r--   0        0        0     1497 2023-04-11 07:55:15.290282 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/frontend/vite.svg
+-rw-r--r--   0        0        0      158 2023-04-12 03:47:14.047670 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/models.py
+-rw-r--r--   0        0        0     2570 2023-04-14 18:06:40.658070 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/app/router.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       99 2023-04-15 08:12:24.621824 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1421 2023-04-12 03:47:14.050665 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0     1059 2023-04-15 08:13:53.942309 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     4775 2023-04-14 18:06:07.595964 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2060 2023-04-12 03:47:14.052663 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      328 2023-04-15 08:10:49.614425 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     3222 2023-04-12 03:47:14.052663 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     2033 2023-04-14 18:07:31.232754 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0     1004 2023-04-15 04:09:14.937130 nonebot_plugin_blive_danmaku-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3032 2023-04-15 08:12:54.517429 nonebot_plugin_blive_danmaku-0.2.0/README.md
+-rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/LICENSE` & `nonebot_plugin_blive_danmaku-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_add.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,12 +21,12 @@
     except ResponseCodeError as ex:
         if ex.code == -400 or ex.code == -404:
             await sub_add.finish(f"UID {uid}不存在，请检查后重试")
         elif ex.code == -412:
             await sub_add.finish(f"操作过于频繁，请半小时后再试")
         else:
             await sub_add.finish("发送未知错误")
-    res = await db.add_sub(uid=uid, type=event.message_type, type_id=type_id, street_lamp=True, bot_id=event.self_id)
+    res = await db.add_sub(uid=uid, type=event.message_type, type_id=type_id, street_lamp=True, live=False, bot_id=event.self_id)
     name = user["name"]
     if res:
         await sub_add.finish(f"添加订阅 {name}({uid}) 成功")
     await sub_add.finish(f"{name}({uid}) 已经订阅")
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_list.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot import on_command, get_driver
 from ...utils import get_type_id,permission_check
 from bilireq.user import get_user_info
 from ...database import Db as db
-from ...config import Config
+from ...config import danmaku_config
 
 
 sub_list = on_command("订阅列表", priority=5)
 sub_list.__doc__ = """订阅列表"""
 sub_list.handle()(permission_check)
 
 @sub_list.handle()
 async def _(event: MessageEvent, bot: Bot):
     """查看订阅列表"""
     type_id = await get_type_id(event)
     subs = await db.get_subs(type=event.message_type, type_id=type_id)
     msg = "订阅列表：\n\n"
-    plugin_config = Config.parse_obj(get_driver().config)
     for sub in subs:
         user = await get_user_info(sub.uid, reqtype="web", proxies=None)
         name = user["name"]
         msg += (
-            f"{name}({sub.uid})"
-            f"路灯：{'开' if sub.street_lamp else '关'}"
-            f"开播提醒：{'开' if plugin_config.danmaku_group_notice else '关'}"
+            f"{name}({sub.uid}) "
+            f"路灯：{'开' if sub.street_lamp else '关'} "
+            f"开播提醒：{'开' if danmaku_config.danmaku_group_notice else '关'}"
         )
     await sub_list.finish(msg)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_off.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/sub/sub_on.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,34 +45,33 @@
                 model.client.add_handler(handler)
                 model.client.start()
                 model.uid=uid
                 model.name=info["uname"]
                 model.live_time=get_timespan(room_info["live_time"])
                 clients.append(model)
 
-                start_timespan = get_timespan(room_info["live_time"])
                 cover = (
                     info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
                 )
-                room = db.get_room(room_id=room_id, uid=uid, start_time=start_timespan)
+                start_timespan = get_timespan(room_info["live_time"])
+                room = await db.get_room(room_id=room_id, uid=uid, start_time=start_timespan)
                 if not room:
                     await db.add_room(room_id=room_id, uid=uid, cover=cover, title=info["title"], name=info["uname"], start_time=start_timespan, end_time=0)
         else:
             if new_status == 0:
                 model = index[0]
                 client = model.client
+                room_id = info["short_id"] if info["short_id"] else info["room_id"]
                 try:
                     asyncio.gather(client.join())
                 finally:
                     await asyncio.gather(client.stop_and_close())
                     clients.remove(model)
                     logger.info(f'{info["uname"]}下播了，断开直播间连接')
-                
                 now = int(time.time())
-                room_id = info["short_id"] if info["short_id"] else info["room_id"]
                 room_list = await db.get_rooms(room_id=room_id, uid=uid)
                 room_list.sort(key=lambda x:x.start_time, reverse=True)
                 room = room_list[0]
                 await db.update_room("end_time", now, room_id=room_id, uid=uid, start_time=room.start_time)
 
     
 
@@ -92,15 +91,19 @@
                     await disconnect_room(model)
                     continue
                 dt = get_time_difference(model.live_time)
                 datetime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
                 blive_danmaku = message.msg.replace("#路灯","", 1).strip()
                 msg = f'【{model.name}】 在 {datetime}({dt}) 收到了 {message.uname} 发来的路灯【{blive_danmaku}】'
                 await send_msg(bot_id=sub.bot_id,send_type=sub.type,type_id=sub.type_id,message=msg)
-                await db.add_danmaku(room_id=client.room_id, uname=message.uname, message=blive_danmaku, create_time=datetime, live_duration=dt)
+
+                room_list = await db.get_rooms(room_id=client.room_id, uid=sub.uid)
+                room_list.sort(key=lambda x:x.start_time, reverse=True)
+                room = room_list[0]
+                await db.add_danmaku(room_id=room.id, uname=message.uname, message=blive_danmaku, create_time=datetime, live_duration=dt)
 
 
 async def disconnect_room(model):
     client = model.client
     try:
         asyncio.gather(client.join())
     finally:
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/command/subscribe/live.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/command/subscribe/live.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,25 +25,24 @@
         return
     
     res = await get_rooms_info_by_uids(uids, reqtype="web", proxies=None)
     if not res:
         return
     for uid, info in res.items():
         live_status = 0 if info["live_status"] == 2 else info["live_status"]
+        name = info["uname"]
+        room_id = info["short_id"] if info["short_id"] else info["room_id"]
         if uid not in live_uids:
             live_uids[uid] = live_status
             continue
         status = live_uids[uid]
         if live_status == status:
             continue
         live_uids[uid] = live_status
 
-        name = info["uname"]
-        room_id = info["short_id"] if info["short_id"] else info["room_id"]
-        room_info = await get_room_info_by_id(room_id, reqtype="web")
         if live_status:
             logger.info(f"{name} 开播了")
             url = f"https://live.bilibili.com/{room_id}"
             cover = (
                 info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
             )
             title = info["title"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from nonebot import get_driver
-from nonebot.log import logger
 from tortoise import Tortoise
 from tortoise.connection import connections
 
 from ..utils import get_path
 from .model import Sub, LiveRoom, Danmaku
 from aerich import Command
+from nonebot.log import logger
 
 sub_dict = {"street_lamp": [], "live": []}
 
 class Db:
     @classmethod
     async def init(cls):
         config={
             "connections":{"danmaku_bot":f"sqlite://{get_path('danmakuBot.sqlite3')}"},
             "apps":{
                 "danmaku_bot_app":{
-                    "models":["nonebot_plugin_blive_danmaku.database.model"],
+                    "models":["aerich.models","nonebot_plugin_blive_danmaku.database.model"],
                     "default_connection":"danmaku_bot"
                 }
             }
         }
         try:
             command = Command(tortoise_config=config)
             await command.init()
             await command.migrate("danmakuBot")
         except:
             logger.debug("migrate error")
         await Tortoise.init(config=config)
         await Tortoise.generate_schemas()
         await cls.update_sub_list()
+        logger.info("load db")
+        
     
     @classmethod
     async def add_sub(cls, **kwargs) -> bool:
         if not await Sub.add(**kwargs):
             return False
         await cls.update_sub_list()
         return True
@@ -66,15 +68,15 @@
     def get_sub_list(cls, key):
         return sub_dict[key]
  
     @classmethod
     async def update_sub_list(cls):
         subs = Sub.all()
         sub_dict["street_lamp"] = list(set([sub.uid async for sub in subs if sub.street_lamp]))
-        sub_dict["live"] = list(set([sub.uid async for sub in subs]))
+        sub_dict["live"] = list(set([x.uid async for x in subs]))
     
     @classmethod
     async def get_rooms(cls, **kwargs):
         res = await LiveRoom.get(**kwargs)
         return res
     
     @classmethod
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     type=fields.CharField(max_length=10)
     uid=fields.BigIntField()
     street_lamp=fields.BooleanField()
     bot_id=fields.BigIntField()
 
 
 class LiveRoom(BaseModel):
+    id=fields.IntField(pk=True, generated=True)
     room_id=fields.BigIntField()
     cover=fields.CharField(max_length=500)
     title=fields.CharField(max_length=50)
     uid=fields.BigIntField()
     name=fields.CharField(max_length=50)
     start_time=fields.BigIntField()
     end_time=fields.BigIntField()
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.2.0/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.64"
+version = "0.2.0"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
@@ -21,12 +21,13 @@
 bilireq = "^0.2.4"
 nonebot_plugin_apscheduler = "^0.2.0"
 tortoise = "^0.1.1"
 tortoise-orm = "^0.19.3"
 aiohttp = "3.7.4"
 Brotli = "1.0.9"
 aerich = "0.7.1"
-
+Pillow = "^9.5.0"
+Jinja2 = "^3.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/README.md` & `nonebot_plugin_blive_danmaku-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -36,30 +36,40 @@
 ```
 nb plugin install nonebot-plugin-blive-danmaku
 ```
 - 方式二：使用`pip`安装
 ```
 python -m pip install nonebot-plugin-blive-danmaku
 ```  
+## 配置  
+
+|名称|类型|默认值|描述|
+|-----|-----|-----|-----|
+|danmaku_group_notice|bool|False|全局群开播提醒|  
 
 ## 指令
 
 |指令|说明|
 |------|------|
 |/添加订阅 UID|UID为B站用户的uid，不是直播间id，以下同理|
 |/取消订阅 UID|删除订阅|
 |/开启路灯 UID|开启直播间弹幕监听|
 |/关闭路灯 UID|关闭直播间弹幕监听|
 |/订阅列表|| 
+|/查看面板|打开网页版查询|
 
 ## 效果预览 
 
 ![](/doc/screenshot.png)
 
-## 更新日志  
+## 更新日志 
+
+- v0.2.0
+    - 修复历史bug  
+    - 添加网页面板，外部访问请自行配置反向代理服务器
 - v0.1.4
     - 添加开播提醒，`.env`新增全局配置项`danmaku_group_notice`开关 [#3](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/3)  
     - 调整日志级别 [#5](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/5)
 - v0.1.3
     - bot提醒在时间后面加上直播时长显示，避免直播画面没有当前时间的场景
 - v0.1.2
     - fix局部变量无法正常更新的bug
```

#### html2text {}

```diff
@@ -14,21 +14,25 @@
 ![](/doc/screenshot1.png) -
 è·¯ç¯ï¼ææç´æ­è¿ç¨ä¸­æè¶£çç¹è®°å½ä¸æ¥ï¼ç»åªè¾æ ¹æ®è®°å½çæ¶é´ç¹ååå®¹ååºå¯¹åºçè§é¢ã
 ## åè½ - ç¨å¼¹å¹çå½¢å¼è®°å½ç´æ­é«è½ç¹ -
 å¼¹å¹æä»¤ä¸º`#è·¯ç¯`å ä¸è®°å½çåå®¹ -
 ä»å¨å¼æ­æ¶å¼¹å¹æä»¤æä¼çæ ## ä¾èµ - Python >= 3.10 - OneBot V11
 ## å®è£ - æ¹å¼ä¸ï¼ä½¿ç¨`nb-cli`å®è£æä»¶ ``` nb plugin install
 nonebot-plugin-blive-danmaku ``` - æ¹å¼äºï¼ä½¿ç¨`pip`å®è£ ``` python -
-m pip install nonebot-plugin-blive-danmaku ``` ## æä»¤ |æä»¤|è¯´æ| |-----
--|------| |/æ·»å è®¢é
+m pip install nonebot-plugin-blive-danmaku ``` ## éç½®
+|åç§°|ç±»å|é»è®¤å¼|æè¿°| |-----|-----|-----|-----
+| |danmaku_group_notice|bool|False|å¨å±ç¾¤å¼æ­æé| ## æä»¤
+|æä»¤|è¯´æ| |------|------| |/æ·»å è®¢é
 UID|UIDä¸ºBç«ç¨æ·çuidï¼ä¸æ¯ç´æ­é´idï¼ä»¥ä¸åç| |/åæ¶è®¢é
 UID|å é¤è®¢é| |/å¼å¯è·¯ç¯ UID|å¼å¯ç´æ­é´å¼¹å¹çå¬| |/
-å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/è®¢éåè¡¨|| ## ææé¢è§
-![](/doc/screenshot.png) ## æ´æ°æ¥å¿ - v0.1.4 -
-æ·»å å¼æ­æéï¼`.env`æ°å¢å¨å±éç½®é¡¹`danmaku_group_notice`å¼å³
+å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/è®¢éåè¡¨|| |/
+æ¥çé¢æ¿|æå¼ç½é¡µçæ¥è¯¢| ## ææé¢è§ ![](/doc/screenshot.png) ##
+æ´æ°æ¥å¿ - v0.2.0 - ä¿®å¤åå²bug -
+æ·»å ç½é¡µé¢æ¿ï¼å¤é¨è®¿é®è¯·èªè¡éç½®ååä»£çæå¡å¨ - v0.1.4
+- æ·»å å¼æ­æéï¼`.env`æ°å¢å¨å±éç½®é¡¹`danmaku_group_notice`å¼å³
 [#3](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/3) -
 è°æ´æ¥å¿çº§å« [#5](https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku/issues/5) - v0.1.3 -
 botæéå¨æ¶é´åé¢å ä¸ç´æ­æ¶é¿æ¾ç¤ºï¼é¿åç´æ­ç»é¢æ²¡æå½åæ¶é´çåºæ¯
 - v0.1.2 - fixå±é¨åéæ æ³æ­£å¸¸æ´æ°çbug - v0.1.0 -
 åºäºnonebot2ï¼å®ç°åæ­¥è·¯ç¯å¼¹å¹å°qqç¾¤ ## æè°¢ - [HarukaBot]
 (https://github.com/SK-415/HarukaBot) - [blivechat](https://github.com/
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.64/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.1.64
+Version: 0.2.0
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Brotli (==1.0.9)
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: Pillow (>=9.5.0,<10.0.0)
 Requires-Dist: aerich (==0.7.1)
 Requires-Dist: aiohttp (==3.7.4)
 Requires-Dist: bilireq (>=0.2.4,<0.3.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: tortoise (>=0.1.1,<0.2.0)
@@ -64,30 +66,40 @@
 ```
 nb plugin install nonebot-plugin-blive-danmaku
 ```
 - 方式二：使用`pip`安装
 ```
 python -m pip install nonebot-plugin-blive-danmaku
 ```  
+## 配置  
+
+|名称|类型|默认值|描述|
+|-----|-----|-----|-----|
+|danmaku_group_notice|bool|False|全局群开播提醒|  
 
 ## 指令
 
 |指令|说明|
 |------|------|
 |/添加订阅 UID|UID为B站用户的uid，不是直播间id，以下同理|
 |/取消订阅 UID|删除订阅|
 |/开启路灯 UID|开启直播间弹幕监听|
 |/关闭路灯 UID|关闭直播间弹幕监听|
 |/订阅列表|| 
+|/查看面板|打开网页版查询|
 
 ## 效果预览 
 
 ![](/doc/screenshot.png)
 
-## 更新日志  
+## 更新日志 
+
+- v0.2.0
+    - 修复历史bug  
+    - 添加网页面板，外部访问请自行配置反向代理服务器
 - v0.1.4
     - 添加开播提醒，`.env`新增全局配置项`danmaku_group_notice`开关 [#3](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/3)  
     - 调整日志级别 [#5](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/5)
 - v0.1.3
     - bot提醒在时间后面加上直播时长显示，避免直播画面没有当前时间的场景
 - v0.1.2
     - fix局部变量无法正常更新的bug
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.1.64
+Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.2.0
 Summary: A danmaku plugin for Nonebot2 Home-page: https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku License: MIT Keywords:
 nonebot,nonebot2,bilibili,danmaku Author: ricardo Author-email:
 thespirit@vip.qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Brotli
-(==1.0.9) Requires-Dist: aerich (==0.7.1) Requires-Dist: aiohttp (==3.7.4)
-Requires-Dist: bilireq (>=0.2.4,<0.3.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.2,<3.0.0) Requires-Dist: nonebot2[fastapi] (>=2.0.0rc4,<3.0.0) Requires-
-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: tortoise
-(>=0.1.1,<0.2.0) Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0) Project-URL:
-Documentation, https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme
-Description-Content-Type: text/markdown
+(==1.0.9) Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: Pillow
+(>=9.5.0,<10.0.0) Requires-Dist: aerich (==0.7.1) Requires-Dist: aiohttp
+(==3.7.4) Requires-Dist: bilireq (>=0.2.4,<0.3.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot2[fastapi]
+(>=2.0.0rc4,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: tortoise (>=0.1.1,<0.2.0) Requires-Dist: tortoise-orm
+(>=0.19.3,<0.20.0) Project-URL: Documentation, https://github.com/zangxx66/
+nonebot_plugin_blive_danmaku#readme Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_blive_danmaku _ð« Bç«ç´æ­é´è·¯ç¯æä»¶ ð«_ [![pypi]
   (https://img.shields.io/pypi/v/nonebot-plugin-blive-danmaku.svg)](https://
       pypi.org/project/nonebot-plugin-blive-danmaku/) ![python](https://
 img.shields.io/pypi/pyversions/nonebot-plugin-blive-danmaku) [![license](https:
   //img.shields.io/github/license/zangxx66/nonebot_plugin_blive_danmaku.svg)]
@@ -30,21 +31,25 @@
 ![](/doc/screenshot1.png) -
 è·¯ç¯ï¼ææç´æ­è¿ç¨ä¸­æè¶£çç¹è®°å½ä¸æ¥ï¼ç»åªè¾æ ¹æ®è®°å½çæ¶é´ç¹ååå®¹ååºå¯¹åºçè§é¢ã
 ## åè½ - ç¨å¼¹å¹çå½¢å¼è®°å½ç´æ­é«è½ç¹ -
 å¼¹å¹æä»¤ä¸º`#è·¯ç¯`å ä¸è®°å½çåå®¹ -
 ä»å¨å¼æ­æ¶å¼¹å¹æä»¤æä¼çæ ## ä¾èµ - Python >= 3.10 - OneBot V11
 ## å®è£ - æ¹å¼ä¸ï¼ä½¿ç¨`nb-cli`å®è£æä»¶ ``` nb plugin install
 nonebot-plugin-blive-danmaku ``` - æ¹å¼äºï¼ä½¿ç¨`pip`å®è£ ``` python -
-m pip install nonebot-plugin-blive-danmaku ``` ## æä»¤ |æä»¤|è¯´æ| |-----
--|------| |/æ·»å è®¢é
+m pip install nonebot-plugin-blive-danmaku ``` ## éç½®
+|åç§°|ç±»å|é»è®¤å¼|æè¿°| |-----|-----|-----|-----
+| |danmaku_group_notice|bool|False|å¨å±ç¾¤å¼æ­æé| ## æä»¤
+|æä»¤|è¯´æ| |------|------| |/æ·»å è®¢é
 UID|UIDä¸ºBç«ç¨æ·çuidï¼ä¸æ¯ç´æ­é´idï¼ä»¥ä¸åç| |/åæ¶è®¢é
 UID|å é¤è®¢é| |/å¼å¯è·¯ç¯ UID|å¼å¯ç´æ­é´å¼¹å¹çå¬| |/
-å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/è®¢éåè¡¨|| ## ææé¢è§
-![](/doc/screenshot.png) ## æ´æ°æ¥å¿ - v0.1.4 -
-æ·»å å¼æ­æéï¼`.env`æ°å¢å¨å±éç½®é¡¹`danmaku_group_notice`å¼å³
+å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/è®¢éåè¡¨|| |/
+æ¥çé¢æ¿|æå¼ç½é¡µçæ¥è¯¢| ## ææé¢è§ ![](/doc/screenshot.png) ##
+æ´æ°æ¥å¿ - v0.2.0 - ä¿®å¤åå²bug -
+æ·»å ç½é¡µé¢æ¿ï¼å¤é¨è®¿é®è¯·èªè¡éç½®ååä»£çæå¡å¨ - v0.1.4
+- æ·»å å¼æ­æéï¼`.env`æ°å¢å¨å±éç½®é¡¹`danmaku_group_notice`å¼å³
 [#3](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/3) -
 è°æ´æ¥å¿çº§å« [#5](https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku/issues/5) - v0.1.3 -
 botæéå¨æ¶é´åé¢å ä¸ç´æ­æ¶é¿æ¾ç¤ºï¼é¿åç´æ­ç»é¢æ²¡æå½åæ¶é´çåºæ¯
 - v0.1.2 - fixå±é¨åéæ æ³æ­£å¸¸æ´æ°çbug - v0.1.0 -
 åºäºnonebot2ï¼å®ç°åæ­¥è·¯ç¯å¼¹å¹å°qqç¾¤ ## æè°¢ - [HarukaBot]
 (https://github.com/SK-415/HarukaBot) - [blivechat](https://github.com/
```

