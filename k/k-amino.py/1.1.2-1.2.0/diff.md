# Comparing `tmp/k-amino.py-1.1.2.tar.gz` & `tmp/k-amino.py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-amino.py-1.1.2.tar", last modified: Sun Apr  9 11:22:10 2023, max compression
+gzip compressed data, was "k-amino.py-1.2.0.tar", last modified: Sat Apr 15 10:30:51 2023, max compression
```

## Comparing `k-amino.py-1.1.2.tar` & `k-amino.py-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.468340 k-amino.py-1.1.2/
--rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2143 2023-04-09 11:22:10.468340 k-amino.py-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.347353 k-amino.py-1.1.2/k_amino/
--rw-rw-rw-   0        0        0      872 2023-04-09 11:22:00.000000 k-amino.py-1.1.2/k_amino/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.390340 k-amino.py-1.1.2/k_amino/k_async/
--rw-rw-rw-   0        0        0      122 2023-04-09 03:38:43.000000 k-amino.py-1.1.2/k_amino/k_async/__init__.py
--rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.1.2/k_amino/k_async/acm.py
--rw-rw-rw-   0        0        0     1950 2023-04-07 03:16:23.000000 k-amino.py-1.1.2/k_amino/k_async/bot.py
--rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.1.2/k_amino/k_async/client.py
--rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.1.2/k_amino/k_async/local.py
--rw-rw-rw-   0        0        0    24690 2023-04-09 11:21:26.000000 k-amino.py-1.1.2/k_amino/k_async/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.409341 k-amino.py-1.1.2/k_amino/k_sync/
--rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.1.2/k_amino/k_sync/__init__.py
--rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.1.2/k_amino/k_sync/acm.py
--rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.1.2/k_amino/k_sync/bot.py
--rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.1.2/k_amino/k_sync/client.py
--rw-rw-rw-   0        0        0    45202 2023-04-09 02:51:09.000000 k-amino.py-1.1.2/k_amino/k_sync/local.py
--rw-rw-rw-   0        0        0    23210 2023-04-09 01:13:33.000000 k-amino.py-1.1.2/k_amino/k_sync/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.431340 k-amino.py-1.1.2/k_amino/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/__init__.py
--rw-rw-rw-   0        0        0     2803 2023-04-07 05:28:51.000000 k-amino.py-1.1.2/k_amino/lib/async_sessions.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/exception.py
--rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/headers.py
--rw-rw-rw-   0        0        0   198102 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/objects.py
--rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/sessions.py
--rw-rw-rw-   0        0        0     1688 2023-04-09 07:16:48.000000 k-amino.py-1.1.2/k_amino/lib/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.370341 k-amino.py-1.1.2/k_amino.py.egg-info/
--rw-rw-rw-   0        0        0     2143 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-04-09 11:22:10.000000 k-amino.py-1.1.2/k_amino.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.447341 k-amino.py-1.1.2/k_asyncOld/
--rw-rw-rw-   0        0        0       79 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/__init__.py
--rw-rw-rw-   0        0        0     5940 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/acm.py
--rw-rw-rw-   0        0        0    40417 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/client.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.465344 k-amino.py-1.1.2/k_asyncOld/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/__init__.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/exception.py
--rw-rw-rw-   0        0        0     1631 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/headers.py
--rw-rw-rw-   0        0        0   198118 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/objects.py
--rw-rw-rw-   0        0        0      768 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/util.py
--rw-rw-rw-   0        0        0    55364 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/local.py
--rw-rw-rw-   0        0        0    24930 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/sockets.py
--rw-rw-rw-   0        0        0       42 2023-04-09 11:22:10.473342 k-amino.py-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.818515 k-amino.py-1.2.0/
+-rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2143 2023-04-15 10:30:51.819499 k-amino.py-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.681112 k-amino.py-1.2.0/k_amino/
+-rw-rw-rw-   0        0        0      872 2023-04-14 09:14:24.000000 k-amino.py-1.2.0/k_amino/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.726156 k-amino.py-1.2.0/k_amino/k_async/
+-rw-rw-rw-   0        0        0      122 2023-04-09 03:38:43.000000 k-amino.py-1.2.0/k_amino/k_async/__init__.py
+-rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.2.0/k_amino/k_async/acm.py
+-rw-rw-rw-   0        0        0     2392 2023-04-15 05:50:54.000000 k-amino.py-1.2.0/k_amino/k_async/bot.py
+-rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.2.0/k_amino/k_async/client.py
+-rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.2.0/k_amino/k_async/local.py
+-rw-rw-rw-   0        0        0    27516 2023-04-15 09:39:33.000000 k-amino.py-1.2.0/k_amino/k_async/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.772265 k-amino.py-1.2.0/k_amino/k_async/websocket_async/
+-rw-rw-rw-   0        0        0      801 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/__init__.py
+-rw-rw-rw-   0        0        0    13388 2023-04-14 11:31:01.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_abnf.py
+-rw-rw-rw-   0        0        0    20107 2023-04-15 10:19:58.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_app.py
+-rw-rw-rw-   0        0        0     2118 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_cookiejar.py
+-rw-rw-rw-   0        0        0    20129 2023-04-15 10:09:33.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_core.py
+-rw-rw-rw-   0        0        0     2105 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_exceptions.py
+-rw-rw-rw-   0        0        0     6073 2023-04-14 11:59:23.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_handshake.py
+-rw-rw-rw-   0        0        0    11803 2023-04-14 12:04:01.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_http.py
+-rw-rw-rw-   0        0        0     2027 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_logging.py
+-rw-rw-rw-   0        0        0     4922 2023-04-14 12:08:35.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_socket.py
+-rw-rw-rw-   0        0        0     1122 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_ssl_compat.py
+-rw-rw-rw-   0        0        0     4797 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_url.py
+-rw-rw-rw-   0        0        0     3516 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_utils.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 03:38:42.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_wsdump.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.791748 k-amino.py-1.2.0/k_amino/k_sync/
+-rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.2.0/k_amino/k_sync/__init__.py
+-rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.2.0/k_amino/k_sync/acm.py
+-rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.2.0/k_amino/k_sync/bot.py
+-rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.2.0/k_amino/k_sync/client.py
+-rw-rw-rw-   0        0        0    45202 2023-04-15 06:24:52.000000 k-amino.py-1.2.0/k_amino/k_sync/local.py
+-rw-rw-rw-   0        0        0    24349 2023-04-15 06:31:22.000000 k-amino.py-1.2.0/k_amino/k_sync/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.816284 k-amino.py-1.2.0/k_amino/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-04-14 13:36:56.000000 k-amino.py-1.2.0/k_amino/lib/async_sessions.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/exception.py
+-rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/headers.py
+-rw-rw-rw-   0        0        0   198102 2023-04-15 05:49:07.000000 k-amino.py-1.2.0/k_amino/lib/objects.py
+-rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/sessions.py
+-rw-rw-rw-   0        0        0     1688 2023-04-09 07:16:48.000000 k-amino.py-1.2.0/k_amino/lib/util.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.705657 k-amino.py-1.2.0/k_amino.py.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 10:30:51.823500 k-amino.py-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.2.0/setup.py
```

### Comparing `k-amino.py-1.1.2/LICENSE` & `k-amino.py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/PKG-INFO` & `k-amino.py-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.1.2
+Version: 1.2.0
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.1.2/README.md` & `k-amino.py-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/__init__.py` & `k-amino.py-1.2.0/k_amino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .k_async.acm import AsyncAcm
 from .k_async.client import AsyncClient
 from .k_async.local import AsyncSubClient
 # from .k_async.sockets import *
 from .k_async.bot import AsyncBot
 
 
-__version__ = "1.1.2"
+__version__ = "1.2.0"
 
 
 __newest__ = loads(get("https://pypi.python.org/pypi/k-amino.py/json").text)["info"]["version"]
 
 if __version__ != __newest__:
     print(f"\033[1;31;38mk_amino New Version!: {__newest__} (You are using {__version__})\033[1;36;33m\nDiscord server: \"https://discord.gg/zd8gyFJquT\"\033[1;0m")
 else:
```

### Comparing `k-amino.py-1.1.2/k_amino/k_async/acm.py` & `k-amino.py-1.2.0/k_amino/k_async/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/k_async/bot.py` & `k-amino.py-1.2.0/k_amino/k_sync/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from easy_events import AsyncEvents, Parameters
+from easy_events import Events, Parameters
 
-from .local import AsyncSubClient as SubClient
+from .local import SubClient
 
 
-class AsyncBot(AsyncEvents):
+class Bot(Events):
     def __init__(self, prefix: str = "!"):
-        AsyncEvents.__init__(self, prefix=prefix, str_only=True, first_parameter_object=True, default_event=False)
+        Events.__init__(self, prefix=prefix, str_only=True, first_parameter_object=True, default_event=False)
 
         # to make @client.command()
         self.command = self.add_event
 
     def build_parameters(self, obj_data):
         data = Parameters(data=obj_data.message.content, prefix=self.prefix, str_only=True)
```

### Comparing `k-amino.py-1.1.2/k_amino/k_async/client.py` & `k-amino.py-1.2.0/k_amino/k_async/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/k_async/local.py` & `k-amino.py-1.2.0/k_amino/k_async/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/k_async/sockets.py` & `k-amino.py-1.2.0/k_amino/k_sync/sockets.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,38 +3,34 @@
 import threading
 import time as timer
 from sys import _getframe as getframe
 from typing import Union
 
 import ujson as json
 import websocket
-import asyncio
 
 from ..lib import *
 from ..lib.objects import *
-from .bot import AsyncBot as Bot
-from easy_events import AsyncEvents
+from .bot import Bot
 
-try:
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-except Exception:
-    pass
 
-
-class AsyncCallbacks(Bot):
+class Callbacks(Bot):
     def __init__(self, is_bot: bool = False, prefix: str = "!"):
         Bot.__init__(self, prefix=prefix)
 
         # if the user want to use the script as a bot
         self.is_bot = is_bot
 
         self.handlers = {}
 
         self.methods = {
             10: self._resolve_payload,
+            201: self._resolve_channel,
+            304: self._resolve_chat_action_start,
+            306: self._resolve_chat_action_end,
             400: self._resolve_topics,
             1000: self._resolve_chat_message,
         }
 
         self.chat_methods = {
             "0:0": self.on_text_message,
             "0:100": self.on_image_message,
@@ -85,129 +81,151 @@
             "129:0": self.on_chat_tipping_disabled,
             "65281:0": self.on_timestamp_message,
             "65282:0": self.on_welcome_message,
             "65283:0": self.on_invite_message,
         }
 
         self.notif_methods = {
+            "18": self.on_alert,
             "53": self.on_member_set_you_host,
             "67": self.on_member_set_you_cohost,
             "68": self.on_member_remove_you_cohost,
         }
 
+        self.chat_action_methods = {
+            "fetch-channel": self.on_fetch_channel,
+            "Typing-start": self.on_user_typing_start,
+            "Typing-end": self.on_user_typing_end,
+        }
+
         self.topics = {
             "online-members": self.on_online_users_update,
             "users-start-typing-at": self.on_user_typing_start,
             "users-end-typing-at": self.on_user_typing_end,
             "users-start-recording-at": self.on_voice_chat_start,
             "users-end-recording-at": self.on_voice_chat_end,
         }
 
-    async def _resolve_payload(self, data):
+    def _resolve_chat_action_start(self, data):
+        key = data['o'].get('actions', 0)+"-start"
+        return self.chat_action_methods.get(key, self.default)(data)
+
+    def _resolve_chat_action_end(self, data):
+        key = data['o'].get('actions', 0)+"-end"
+        return self.chat_action_methods.get(key, self.default)(data)
+
+    def _resolve_channel(self, data):
+            if data['t'] == 201:
+                return self.chat_action_methods.get("fetch-channel")(data)
+
+    def _resolve_payload(self, data):
         key = f"{data['o']['payload']['notifType']}"
-        return await self.notif_methods.get(key)(data)
+        return self.notif_methods.get(key)(data)
 
-    async def _resolve_chat_message(self, data):
+    def _resolve_chat_message(self, data):
         key = f"{data['o']['chatMessage']['type']}:{data['o']['chatMessage'].get('mediaType', 0)}"
-        return await self.chat_methods.get(key)(data)
+        return self.chat_methods.get(key)(data)
 
-    async def _resolve_topics(self, data):
+    def _resolve_topics(self, data):
         key = str(data["o"].get("topic", 0)).split(":")[2]
-        return await self.topics.get(key)(data)
+        return self.topics.get(key)(data)
 
-    async def resolve(self, data):
+    def resolve(self, data):
         data = json.loads(data)
-        return await self.methods.get(data.get("t"))(data)
+        return self.methods.get(data["t"])(data)
 
-    async def call(self, callType, data):
+    def call(self, callType, data):
         if self.handlers.get(callType):
             for handler in self.handlers[callType]:
-                await handler(data)
+                handler(data)
 
     def event(self, eventType):
         def registerHandler(handler):
             if self.handlers.get(eventType):
                 self.handlers[eventType].append(handler)
             else:
                 self.handlers[eventType] = [handler]
             return handler
 
         return registerHandler
 
-    async def setCall(self, name, data):
-        await self.call(name, Event(data["o"]).Event)
+    def setCall(self, name, data):
+        self.call(name, Event(data["o"]).Event)
 
-    async def on_text_message(self, data):
+    def on_text_message(self, data):
         if self.is_bot:
             new_data = Event(data["o"]).Event
             new_data = self.build_parameters(new_data)
-            await self.trigger(new_data, str_only=True)
+            self.trigger(new_data, str_only=True)
+
+        self.setCall(getframe(0).f_code.co_name, data)
 
-        await self.setCall(getframe(0).f_code.co_name, data)
+    def on_alert(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+    def on_member_set_you_host(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+    def on_member_remove_you_cohost(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+    def on_member_set_you_cohost(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+
+    def on_image_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_youtube_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_strike_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_sticker_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def TYPE_USER_SHARE_EXURL(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def TYPE_USER_SHARE_USER(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_not_answered(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_not_cancelled(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_not_declined(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_video_chat_not_answered(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_video_chat_not_cancelled(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_video_chat_not_declined(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_avatar_chat_not_answered(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_avatar_chat_not_cancelled(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_avatar_chat_not_declined(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_delete_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_group_member_join(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_group_member_leave(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_invite(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_background_changed(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_title_changed(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_icon_changed(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_start(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_video_chat_start(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_avatar_chat_start(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_end(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_video_chat_end(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_avatar_chat_end(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_content_changed(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_screen_room_start(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_screen_room_end(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_host_transfered(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_text_message_force_removed(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_removed_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_text_message_removed_by_admin(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_tip(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_pin_announcement(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_permission_open_to_everyone(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_permission_invited_and_requested(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_voice_chat_permission_invite_only(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_view_only_enabled(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_view_only_disabled(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_unpin_announcement(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_tipping_enabled(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_chat_tipping_disabled(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_timestamp_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+
+    def on_welcome_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+    def on_invite_message(self, data): self.setCall(getframe(0).f_code.co_name, data)
+
+    def on_user_typing_start(self, data): self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
+    def on_user_typing_end(self, data): self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
+    def on_online_users_update(self, data): self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
 
-    async def on_member_set_you_host(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
-    async def on_member_remove_you_cohost(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
-    async def on_member_set_you_cohost(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
-
-    async def on_image_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_youtube_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_strike_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_sticker_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def TYPE_USER_SHARE_EXURL(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def TYPE_USER_SHARE_USER(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_not_answered(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_not_cancelled(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_not_declined(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_video_chat_not_answered(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_video_chat_not_cancelled(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_video_chat_not_declined(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_avatar_chat_not_answered(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_avatar_chat_not_cancelled(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_avatar_chat_not_declined(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_delete_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_group_member_join(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_group_member_leave(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_invite(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_background_changed(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_title_changed(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_icon_changed(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_start(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_video_chat_start(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_avatar_chat_start(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_end(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_video_chat_end(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_avatar_chat_end(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_content_changed(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_screen_room_start(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_screen_room_end(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_host_transfered(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_text_message_force_removed(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_removed_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_text_message_removed_by_admin(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_tip(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_pin_announcement(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_permission_open_to_everyone(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_permission_invited_and_requested(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_voice_chat_permission_invite_only(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_view_only_enabled(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_view_only_disabled(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_unpin_announcement(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_tipping_enabled(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_chat_tipping_disabled(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_timestamp_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-
-    async def on_welcome_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-    async def on_invite_message(self, data): await self.setCall(getframe(0).f_code.co_name, data)
-
-    async def on_user_typing_start(self, data): await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
-    async def on_user_typing_end(self, data): await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
-    async def on_online_users_update(self, data): await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
+    def on_fetch_channel(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
 
-    async def default(self, data): await self.call(getframe(0).f_code.co_name, data)
+    def default(self, data): self.call(getframe(0).f_code.co_name, data)
 
 
 class SetAction:
     def __init__(self, wss, data):
         self.action = data
         self.wss = wss
 
@@ -374,29 +392,29 @@
         return SetAction(self.socket, data)
 
 
 class WssClient:
     def __init__(self, wss):
         self.wss = wss
 
-    async def joinVoiceChat(self, comId: str, chatId: str, joinType: int = 1):
+    def joinVoiceChat(self, comId: str, chatId: str, joinType: int = 1):
 
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
                 "id": "37549515",
             },
             "t": 112,
         }
-        asyncio.sleep(2.2)
-        await self.wss.send(data)
+        timer.sleep(2.2)
+        self.wss.send(data)
 
-    async def joinVideoChat(self, comId: str, chatId: str, joinType: int = 1):
+    def joinVideoChat(self, comId: str, chatId: str, joinType: int = 1):
         """
         Join The Video Chat
 
         **Parameters**
             - **comId**: ID of the Community (str)
             - **chatId**: ID of the Chat (str)
             - **joinType**: Join type to Join Video as.. (int)
@@ -407,18 +425,18 @@
                 "threadId": chatId,
                 "joinRole": joinType,
                 "channelType": 5,
                 "id": "2154531",
             },
             "t": 108,
         }
-        asyncio.sleep(2.2)
-        await self.wss.send(data)
+        timer.sleep(2.2)
+        self.wss.send(data)
 
-    async def startVoiceChat(self, comId, chatId: str, joinType: int = 1):
+    def startVoiceChat(self, comId, chatId: str, joinType: int = 1):
         """
         Start The Voice Chat
 
         **Parameters**
             - **comId**: ID of the Community (str)
             - **chatId**: ID of the Chat (str)
             - **joinType**: Join type to Start voice as.. (int)
@@ -428,29 +446,29 @@
                 "ndcId": comId,
                 "threadId": chatId,
                 "joinRole": joinType,
                 "id": "2154531",
             },
             "t": 112,
         }
-        asyncio.sleep(2.2)
-        await self.wss.send(data)
+        timer.sleep(2.2)
+        self.wss.send(data)
         data = {
             "o": {
                 "ndcId": comId,
                 "threadId": chatId,
                 "channelType": 1,
                 "id": "2154531",
             },
             "t": 108,
         }
-        asyncio.sleep(2.2)
-        await self.wss.send(data)
+        timer.sleep(2.2)
+        self.wss.send(data)
 
-    async def endVoiceChat(self, comId: str, chatId: str, leaveType: int = 2):
+    def endVoiceChat(self, comId: str, chatId: str, leaveType: int = 2):
         """
         End The Voice Chat
 
         **Parameters**
             - **comId**: ID of the Community (str)
             - **chatId**: ID of the Chat (str)
             - **leaveType**: Leave type to end voice as.. (int)
@@ -460,18 +478,18 @@
                 "ndcId": comId,
                 "threadId": chatId,
                 "joinRole": leaveType,
                 "id": "2154531",
             },
             "t": 112,
         }
-        asyncio.sleep(2.2)
-        await self.wss.send(data)
+        timer.sleep(2.2)
+        self.wss.send(data)
 
-    async def joinVideoChatAsSpectator(self, comId: str, chatId: str):
+    def joinVideoChatAsSpectator(self, comId: str, chatId: str):
         """
         Join Video Chat As Spectator
 
         **Parameters**
             - **comId**: ID of the Community (str)
             - **chatId**: ID of the Chat (str)
         """
@@ -480,42 +498,42 @@
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": 2,
                 "id": "72446",
             },
             "t": 112,
         }
-        asyncio.sleep(2.2)
-        await self.wss.send(data)
+        timer.sleep(2.2)
+        self.wss.send(data)
 
-    async def threadJoin(self, comId: str, chatId: str):
+    def threadJoin(self, comId: str, chatId: str):
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": 1,
                 "id": "10335106",
             },
             "t": 112,
         }
-        await self.wss.send(data)
+        self.wss.send(data)
 
-    async def channelJoin(self, comId: str, chatId: str):
+    def channelJoin(self, comId: str, chatId: str):
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "channelType": 5,
                 "id": "10335436",
             },
             "t": 108,
         }
-        await self.wss.send(data)
+        self.wss.send(data)
 
-    async def GetUsersActions(self, comId: str = None, path: int = 0, chatId: str = None):
+    def GetUsersActions(self, comId: str = None, path: int = 0, chatId: str = None):
         """
         Get users actions:
         This functions gets certain socket actions happening
         such as online users and users chatting
 
         Parameters
             ----------
@@ -553,43 +571,40 @@
                 "ndcId": int(comId) if comId else 0,
                 "topic": f"ndtopic:x{comId}:{topic}",
                 "id": "4538416",
             },
             "t": 300,
         }
 
-        asyncio.sleep(2.2)
-        await self.wss.send(data)
+        timer.sleep(2.2)
+        self.wss.send(data)
 
         for i in range(3):
-            data = await self.wss.receive()
-            if data:
-                return UsersActions(data=data).UsersActions
+            if self.wss.receive():
+                return UsersActions(data=self.wss.receive()).UsersActions
             else:
                 continue
 
         return UsersActions(data={}).UsersActions
 
     def actions(self, comId: str, chatId: str):
         return Actions(self.wss, comId, chatId)
 
 
-class Wss(AsyncCallbacks, WssClient, Headers):
+class Wss(Callbacks, WssClient, Headers):
     def __init__(self, client, trace: bool = False, is_bot: bool = False):
-        self.ev = AsyncEvents(str_only=False, first_parameter_object=False, default_event=False)
-        self.ev.add_event(callback=self.res, aliases=["res"], event_type="wss")
 
         self.trace = trace
         self.socket = None
         self.headers = None
         self.client = client
         self.isOpened = False
 
         Headers.__init__(self)
-        AsyncCallbacks.__init__(self, is_bot=is_bot)
+        Callbacks.__init__(self, is_bot=is_bot)
         WssClient.__init__(self, self)
 
         self.narvi = "https://service.narvii.com/api/v1/"
         self.socket_url = "wss://ws1.narvii.com"
         self.lastMessage = {}
         websocket.enableTrace(trace)
 
@@ -599,34 +614,29 @@
             print("[ON-OPEN] Sockets are open")
 
     def onClose(self, *args):
         self.isOpened = False
         if self.trace:
             print("[ON-CLOSE] Sockets are closed")
 
-    async def send(self, data):
-        await self.socket.send(json.dumps(data))
+    def send(self, data):
+        self.socket.send(json.dumps(data))
 
-    async def receive(self):
+    def receive(self):
         if self.trace:
             print("[RECEIVE] returning last message")
         return self.lastMessage
 
     def on_message(self, ws, data):
         self.lastMessage = json.loads(data)
-        self.ev.add_task(data={"event": "res", "parameters": {"data": data}}, event_type="wss", str_only=False)
-        self.ev.run_task_sync()
-
+        self.resolve(data)
         if self.trace:
             print("[ON-MESSAGE] Received a message . . .")
 
-    async def res(self, data):
-        await self.resolve(data)
-
-    async def launch(self):
+    def launch(self):
         final = f"{self.client.deviceId}|{int(timer.time() * 1000)}"
         self.headers = {
             "NDCDEVICEID": self.client.deviceId,
             "NDCAUTH": self.client.sid,
             "NDC-MSG-SIG": util.generateSig(data=final),
         }
 
@@ -636,24 +646,21 @@
             on_close=self.onClose,
             on_open=self.onOpen,
             header=self.headers,
         )
 
         if self.trace:
             print("[LAUNCH] Sockets starting . . . ")
-
         threading.Thread(
             target=self.socket.run_forever, kwargs={"ping_interval": 60}
         ).start()
 
-    async def close(self):
+    def close(self):
         self.socket.close()
-
         if self.trace:
             print("[CLOSE] closing socket . . .")
-
-        asyncio.sleep(1.5)
+        timer.sleep(1.5)
 
     def socket_status(self):
         print("\nSockets are OPEN\n") if self.isOpened else print(
             "\nSockets are CLOSED\n"
         )
```

### Comparing `k-amino.py-1.1.2/k_amino/k_sync/acm.py` & `k-amino.py-1.2.0/k_amino/k_sync/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/k_sync/bot.py` & `k-amino.py-1.2.0/k_amino/k_async/bot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,33 @@
-from easy_events import Events, Parameters
+from easy_events import AsyncEvents, Parameters
 
-from .local import SubClient
+from .local import AsyncSubClient as SubClient
 
 
-class Bot(Events):
+class AsyncBot(AsyncEvents):
     def __init__(self, prefix: str = "!"):
-        Events.__init__(self, prefix=prefix, str_only=True, first_parameter_object=True, default_event=False)
+        AsyncEvents.__init__(self, prefix=prefix, str_only=True, first_parameter_object=True, default_event=False)
 
         # to make @client.command()
         self.command = self.add_event
 
+    def build_alert_parameters(self, obj_data):
+        message = obj_data.alert.split(": ", 1)
+
+        data = Parameters(data=message[-1], prefix=self.prefix, str_only=True)
+
+        for k, v in obj_data.__dict__.items():
+            setattr(data, k, v)
+
+        data.authorName = message[0]
+        data.comId = obj_data.ndcId
+        data.subClient = data.local = SubClient(comId=data.comId, acm=True)
+
+        return data
+
     def build_parameters(self, obj_data):
         data = Parameters(data=obj_data.message.content, prefix=self.prefix, str_only=True)
 
         for k, v in obj_data.__dict__.items():
             setattr(data, k, v)
 
         for k, v in obj_data.message.__dict__.items():
```

### Comparing `k-amino.py-1.1.2/k_amino/k_sync/client.py` & `k-amino.py-1.2.0/k_amino/k_sync/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/k_sync/local.py` & `k-amino.py-1.2.0/k_amino/k_sync/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/lib/async_sessions.py` & `k-amino.py-1.2.0/k_amino/lib/async_sessions.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.staticDevice = staticDevice
 
         self.sid = user_settings["sid"]
         self.uid = user_settings["userId"]
         self.secret = user_settings["secret"]
 
         Headers.__init__(self, header_device=self.staticDevice)
-        self.session = AC(proxies=self.proxy, timeout = 20)
+        # self.session = AC(proxies=self.proxy, timeout = 20)
 
         self.deviceId = self.header_device
         self.sidInit()
 
     def sidInit(self):
         if self.sid: self.updateHeaders(sid = self.sid)
 
@@ -48,36 +48,36 @@
     async def postRequest(self, url: str, data: Union[str, dict, BinaryIO] = None, newHeaders: dict = None, webRequest: bool = False, minify: bool = False):
         if newHeaders: self.app_headers.update(newHeaders)
 
         if not isinstance(data, (str, BinaryIO)):
             data = json_minify(dumps(data)) if minify else dumps(data)
 
         try:
-            req = await self.session.post(
-                url=webApi(url) if webRequest else api(url),
-                data=data if isinstance(data, str) else None,
-                files={"file": data} if isinstance(data, BinaryIO) else None,
-                headers=self.web_headers if webRequest else self.updateHeaders(data=data, sid=self.sid)
-                )
-            await self.session.aclose()
+            async with AC(proxies=self.proxy, timeout = 20) as session:
+                req = await session.post(
+                    url=webApi(url) if webRequest else api(url),
+                    data=data if isinstance(data, str) else None,
+                    files={"file": data} if isinstance(data, BinaryIO) else None,
+                    headers=self.web_headers if webRequest else self.updateHeaders(data=data, sid=self.sid)
+                    )
         except Exception:
-            return
+            pass
 
         return CheckExceptions(req.json()) if req.status_code != 200 else req.json()
 
     async def getRequest(self, url: str):
         try:
-            req = await self.session.get(url=api(url), headers=self.updateHeaders())
-            await self.session.aclose()
+            async with AC(proxies=self.proxy, timeout = 20) as session:
+                req = await session.get(url=api(url), headers=self.updateHeaders())
         except Exception:
-            return
+            pass
 
         return CheckExceptions(req.json()) if req.status_code != 200 else req.json()
 
     async def deleteRequest(self, url: str):
         try:
-            req = await self.session.delete(url=api(url), headers=self.updateHeaders())
-            await self.session.aclose()
+            async with AC(proxies=self.proxy, timeout = 20) as session:
+                req = await session.delete(url=api(url), headers=self.updateHeaders())
         except Exception:
-            return
+            pass
 
         return CheckExceptions(req.json()) if req.status_code != 200 else req.json()
```

### Comparing `k-amino.py-1.1.2/k_amino/lib/exception.py` & `k-amino.py-1.2.0/k_amino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/lib/headers.py` & `k-amino.py-1.2.0/k_amino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/lib/objects.py` & `k-amino.py-1.2.0/k_amino/lib/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -3404,19 +3404,18 @@
         self.chatId = None
         self.alert = None
 
     @property
     def Payload(self):
         try: self.ndcId = self.json["ndcId"]
         except (KeyError, TypeError): pass
-        try: self.ndcId = self.json["tid"]
+        try: self.chatId = self.json["tid"]
         except (KeyError, TypeError): pass
         try: self.alert = self.json["aps"]["alert"]
         except (KeyError, TypeError): pass
-
         return self
 
 class Event:
     def __init__(self, data):
         self.json = data
         self.comId = None
         self.alertOption = None
```

### Comparing `k-amino.py-1.1.2/k_amino/lib/sessions.py` & `k-amino.py-1.2.0/k_amino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino/lib/util.py` & `k-amino.py-1.2.0/k_amino/lib/util.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.2/k_amino.py.egg-info/PKG-INFO` & `k-amino.py-1.2.0/k_amino.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.1.2
+Version: 1.2.0
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.1.2/k_asyncOld/sockets.py` & `k-amino.py-1.2.0/k_amino/k_async/sockets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,46 @@
-# those sockets are based on: Amino-Sockets / Amino.py
-# Modified by SirLez, zett.0, Bovonos
+# those sockets are based on: Amino-Sockets & Amino.py
 
-import asyncio
 import threading
-import time
+import time as timer
 from sys import _getframe as getframe
-from typing import Union, BinaryIO
+from typing import Union
 
 import ujson as json
-import websockets
+import asyncio
+
+from .websocket_async import WebSocketApp
 
 from ..lib import *
+from ..lib.objects import *
+from .bot import AsyncBot as Bot
 
+try:
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+except Exception:
+    pass
+
+
+class AsyncCallbacks(Bot):
+    def __init__(self, is_bot: bool = False, prefix: str = "!"):
+        Bot.__init__(self, prefix=prefix)
+
+        # if the user want to use the script as a bot
+        self.is_bot = is_bot
+        self.lock_command = False
 
-class Callbacks:
-    def __init__(self):
         self.handlers = {}
 
         self.methods = {
             10: self._resolve_payload,
+            201: self._resolve_channel,
+            304: self._resolve_chat_action_start,
+            306: self._resolve_chat_action_end,
             400: self._resolve_topics,
-            1000: self._resolve_chat_message
+            1000: self._resolve_chat_message,
         }
 
         self.chat_methods = {
             "0:0": self.on_text_message,
             "0:100": self.on_image_message,
             "0:103": self.on_youtube_message,
             "1:0": self.on_strike_message,
@@ -69,520 +85,641 @@
             "125:0": self.on_chat_view_only_enabled,
             "126:0": self.on_chat_view_only_disabled,
             "127:0": self.on_chat_unpin_announcement,
             "128:0": self.on_chat_tipping_enabled,
             "129:0": self.on_chat_tipping_disabled,
             "65281:0": self.on_timestamp_message,
             "65282:0": self.on_welcome_message,
-            "65283:0": self.on_invite_message
+            "65283:0": self.on_invite_message,
         }
 
         self.notif_methods = {
+            "18": self.on_alert,
             "53": self.on_member_set_you_host,
             "67": self.on_member_set_you_cohost,
-            "68": self.on_member_remove_you_cohost
+            "68": self.on_member_remove_you_cohost,
+        }
+
+        self.chat_action_methods = {
+            "fetch-channel": self.on_fetch_channel,
+            "Typing-start": self.on_user_typing_start,
+            "Typing-end": self.on_user_typing_end,
         }
 
         self.topics = {
             "online-members": self.on_online_users_update,
             "users-start-typing-at": self.on_user_typing_start,
             "users-end-typing-at": self.on_user_typing_end,
             "users-start-recording-at": self.on_voice_chat_start,
-            "users-end-recording-at": self.on_voice_chat_end
+            "users-end-recording-at": self.on_voice_chat_end,
         }
 
+    async def _resolve_chat_action_start(self, data):
+        key = data['o'].get('actions', 0)+"-start"
+        return await self.chat_action_methods.get(key, self.default)(data)
+
+    async def _resolve_chat_action_end(self, data):
+        key = data['o'].get('actions', 0)+"-end"
+        return await self.chat_action_methods.get(key, self.default)(data)
+
+    async def _resolve_channel(self, data):
+            if data['t'] == 201:
+                return await self.chat_action_methods.get("fetch-channel")(data)
+
     async def _resolve_payload(self, data):
         key = f"{data['o']['payload']['notifType']}"
-        return await self.notif_methods.get(key, self.default)(data)
+        return await self.notif_methods.get(key)(data)
 
     async def _resolve_chat_message(self, data):
         key = f"{data['o']['chatMessage']['type']}:{data['o']['chatMessage'].get('mediaType', 0)}"
-        return await self.chat_methods.get(key, self.default)(data)
+        return await self.chat_methods.get(key)(data)
 
     async def _resolve_topics(self, data):
-        key = str(data['o'].get('topic', 0)).split(":")[2]
-        return await self.topics.get(key, self.default)(data)
+        key = str(data["o"].get("topic", 0)).split(":")[2]
+        return await self.topics.get(key)(data)
 
-    def resolve(self, data):
+    async def resolve(self, data):
         data = json.loads(data)
-        return asyncio.create_task(self.methods.get(data["t"], self.default)(data))
+        return await self.methods.get(data.get("t"))(data)
 
-    async def call(self, type, data):
-        if type in self.handlers:
-            for handler in self.handlers[type]:
+    async def call(self, callType, data):
+        if self.handlers.get(callType):
+            for handler in self.handlers[callType]:
                 await handler(data)
 
-    def event(self, type):
+    def event(self, eventType):
         def registerHandler(handler):
-            if type in self.handlers:
-                self.handlers[type].append(handler)
+            if self.handlers.get(eventType):
+                self.handlers[eventType].append(handler)
             else:
-                self.handlers[type] = [handler]
+                self.handlers[eventType] = [handler]
             return handler
 
         return registerHandler
 
-    async def on_member_set_you_host(self, data): await self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
-    async def on_member_remove_you_cohost(self, data): await self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
-    async def on_member_set_you_cohost(self, data): await self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
-
-    async def on_text_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_image_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_youtube_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_strike_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_sticker_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def TYPE_USER_SHARE_EXURL(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def TYPE_USER_SHARE_USER(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_not_answered(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_not_cancelled(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_not_declined(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_video_chat_not_answered(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_video_chat_not_cancelled(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_video_chat_not_declined(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_avatar_chat_not_answered(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_avatar_chat_not_cancelled(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_avatar_chat_not_declined(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_delete_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_group_member_join(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_group_member_leave(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_invite(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_background_changed(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_title_changed(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_icon_changed(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_start(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_video_chat_start(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_avatar_chat_start(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_end(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_video_chat_end(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_avatar_chat_end(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_content_changed(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_screen_room_start(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_screen_room_end(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_host_transfered(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_text_message_force_removed(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_removed_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_text_message_removed_by_admin(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_tip(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_pin_announcement(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_permission_open_to_everyone(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_permission_invited_and_requested(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_voice_chat_permission_invite_only(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_view_only_enabled(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_view_only_disabled(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_unpin_announcement(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_tipping_enabled(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_chat_tipping_disabled(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_timestamp_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_welcome_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-    async def on_invite_message(self, data): await self.call(getframe(0).f_code.co_name, Event(data["o"]).Event)
-
-    async def on_user_typing_start(self, data): await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
-    async def on_user_typing_end(self, data): await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
-    async def on_online_users_update(self, data): await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
+    async def setCall(self, name, data):
+        return await self.call(name, Event(data["o"]).Event)
+
+    async def on_text_message(self, data):
+        if self.is_bot:
+            new_data = Event(data["o"]).Event
+            new_data = self.build_parameters(new_data)
+            await self.trigger(new_data, str_only=True)
+
+        return await self.setCall(getframe(0).f_code.co_name, data)
+
+    async def on_alert(self, data):
+        if self.is_bot and False:
+            new_data = Payload(data["o"]["payload"]).Payload
+            new_data = self.build_alert_parameters(new_data)
+            await self.trigger(new_data, str_only=True)
+
+        return await self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+
+
+    async def on_member_set_you_host(self, data): return await self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+    async def on_member_remove_you_cohost(self, data): return await self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+    async def on_member_set_you_cohost(self, data): return await self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+    async def on_fetch_channel(self, data): return await self.call(getframe(0).f_code.co_name, Payload(data["o"]["payload"]).Payload)
+
+    async def on_image_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_youtube_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_strike_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_sticker_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def TYPE_USER_SHARE_EXURL(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def TYPE_USER_SHARE_USER(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_not_answered(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_not_cancelled(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_not_declined(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_video_chat_not_answered(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_video_chat_not_cancelled(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_video_chat_not_declined(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_avatar_chat_not_answered(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_avatar_chat_not_cancelled(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_avatar_chat_not_declined(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_delete_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_group_member_join(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_group_member_leave(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_invite(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_background_changed(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_title_changed(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_icon_changed(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_start(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_video_chat_start(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_avatar_chat_start(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_end(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_video_chat_end(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_avatar_chat_end(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_content_changed(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_screen_room_start(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_screen_room_end(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_host_transfered(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_text_message_force_removed(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_removed_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_text_message_removed_by_admin(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_tip(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_pin_announcement(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_permission_open_to_everyone(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_permission_invited_and_requested(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_voice_chat_permission_invite_only(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_view_only_enabled(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_view_only_disabled(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_unpin_announcement(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_tipping_enabled(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_chat_tipping_disabled(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_timestamp_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+
+    async def on_welcome_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+    async def on_invite_message(self, data): return await self.setCall(getframe(0).f_code.co_name, data)
+
+    async def on_user_typing_start(self, data): return await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
+    async def on_user_typing_end(self, data): return await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
+    async def on_online_users_update(self, data): return await self.call(getframe(0).f_code.co_name, UsersActions(data).UsersActions)
 
-    async def default(self, data): await self.call(getframe(0).f_code.co_name, data)
+    async def default(self, data): return await self.call(getframe(0).f_code.co_name, data)
 
 
 class SetAction:
     def __init__(self, wss, data):
         self.action = data
         self.wss = wss
 
     def start(self):
         """
         Start the Action
         """
         self.wss.send(self.action)
 
-    async def stop(self):
+    def stop(self):
         """
         Get back to the last board
         """
         act = self.action
         act["t"] = 303
-        await self.wss.send(self.action)
+        self.wss.send(self.action)
 
 
 class Actions:
     def __init__(self, socket, comId, chatId):
         self.socket = socket
         self.chatId = chatId
         self.comId = comId
 
-    def sendDefaultAction(self):
-        SetAction(self.socket, {
-            "o": {"actions": ["Browsing"], "target": f"ndc://x{self.comId}/", "ndcId": int(self.comId),
-                  "params": {"duration": 27605}, "id": "363483"}, "t": 306}).start()
+    def setDefaultAction(self):
+        """
+        Default Browsing
+        """
+        SetAction(
+            self.socket,
+            {
+                "o": {
+                    "actions": ["Browsing"],
+                    "target": f"ndc://x{self.comId}/",
+                    "ndcId": int(self.comId),
+                    "params": {"duration": 27605},
+                    "id": "363483",
+                },
+                "t": 306,
+            },
+        ).start()
 
     def Browsing(self, blogId: str = None, blogType: int = 0):
+        """
+        Send Browsing Action
+
+        **Parameters**
+            - **blogId**: target blogId (str)
+            - **blogType**: Type Of the Blog *poll & blog & wiki* (int)
+
+        **Return**
+            - **SetAction**:  (Class)
+        """
+        target = f"ndc://x{self.comId}/featured"
 
         if blogId and blogType:
             target = f"ndc://x{self.comId}/blog/"
-        else:
-            target = f"ndc://x{self.comId}/featured"
 
         data = {
             "o": {
                 "actions": ["Browsing"],
                 "target": target,
                 "ndcId": int(self.comId),
                 "params": {"blogType": blogType},
-                "id": "363483"
+                "id": "363483",
             },
-            "t": 306
+            "t": 306,
         }
-        self.sendDefaultAction()
+        self.setDefaultAction()
         return SetAction(self.socket, data)
 
-    def Chatting(self, threadType: int = 2):
+    def Chatting(self, threadId: str = None, threadType: int = 2):
+        """
+        Send Chatting Action
+
+        **Paramaters**
+            - **threadType**: 2 For Public 1 & 0 For Private (int)
+
+        **Return**
+            - **SetAction**:  (Class)
+        """
 
         data = {
             "o": {
                 "actions": ["Chatting"],
                 "target": f"ndc://x{self.comId}/chat-thread/{self.chatId}",
                 "ndcId": int(self.comId),
                 "params": {
                     "duration": 12800,
                     "membershipStatus": 1,
-                    "threadType": threadType
+                    "threadType": threadType,
+                    "threadId": threadId,
                 },
-                "id": "1715976"
+                "id": "1715976",
             },
-            "t": 306
+            "t": 306,
         }
-        self.sendDefaultAction()
+        # self.defaultData()
         return SetAction(self.socket, data)
 
     def PublicChats(self):
+        """
+        Send PublicChats Action
 
+        **Return**
+            - **SetAction**:  (Class)
+        """
         data = {
             "o": {
                 "actions": ["Browsing"],
                 "target": f"ndc://x{self.comId}/public-chats",
                 "ndcId": int(self.comId),
                 "params": {"duration": 859},
-                "id": "363483"
+                "id": "363483",
             },
-            "t": 306
+            "t": 306,
         }
-        self.sendDefaultAction()
+        self.setDefaultAction()
         return SetAction(self.socket, data)
 
     def LeaderBoards(self):
+        """
+        Send LeaderBoard Action
 
+        **Return**
+            - **SetAction**:  (Class)
+        """
         data = {
             "o": {
                 "actions": ["Browsing"],
                 "target": f"ndc://x{self.comId}/leaderboards",
                 "ndcId": int(self.comId),
                 "params": {"duration": 859},
-                "id": "363483"
+                "id": "363483",
             },
-            "t": 306
+            "t": 306,
         }
-        self.sendDefaultAction()
+        self.setDefaultAction()
         return SetAction(self.socket, data)
 
     def Custom(self, actions: Union[str, list], target: str, params: dict):
+        """
+        Send Custom Action
+
+        **Parameters**
+            - **actions**: List of action Types (list[str])
+            - **target**: Example | ndc://x000000/leaderboards (str)
+            - **params**: Set the blogType and more with params (dict)
 
+        **Return**
+            - **SetAction**:  (Class)
+        """
         data = {
             "o": {
                 "actions": actions,
                 "target": target,
                 "ndcId": int(self.comId),
                 "params": params,
-                "id": "363483"
+                "id": "363483",
             },
-            "t": 306
+            "t": 306,
         }
-        self.sendDefaultAction()
+        self.setDefaultAction()
         return SetAction(self.socket, data)
 
 
 class WssClient:
     def __init__(self, wss):
         self.wss = wss
 
     async def joinVoiceChat(self, comId: str, chatId: str, joinType: int = 1):
 
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
-                "id": "37549515"
+                "id": "37549515",
             },
-            "t": 112
+            "t": 112,
         }
-        await asyncio.sleep(2)
+        await asyncio.sleep(2.2)
         await self.wss.send(data)
 
     async def joinVideoChat(self, comId: str, chatId: str, joinType: int = 1):
+        """
+        Join The Video Chat
 
+        **Parameters**
+            - **comId**: ID of the Community (str)
+            - **chatId**: ID of the Chat (str)
+            - **joinType**: Join type to Join Video as.. (int)
+        """
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
                 "channelType": 5,
-                "id": "2154531"
+                "id": "2154531",
             },
-            "t": 108
+            "t": 108,
         }
-        await asyncio.sleep(2)
+        await asyncio.sleep(2.2)
         await self.wss.send(data)
 
     async def startVoiceChat(self, comId, chatId: str, joinType: int = 1):
+        """
+        Start The Voice Chat
 
+        **Parameters**
+            - **comId**: ID of the Community (str)
+            - **chatId**: ID of the Chat (str)
+            - **joinType**: Join type to Start voice as.. (int)
+        """
         data = {
             "o": {
                 "ndcId": comId,
                 "threadId": chatId,
                 "joinRole": joinType,
-                "id": "2154531"
+                "id": "2154531",
             },
-            "t": 112
+            "t": 112,
         }
-        await asyncio.sleep(2)
+        await asyncio.sleep(2.2)
         await self.wss.send(data)
         data = {
             "o": {
                 "ndcId": comId,
                 "threadId": chatId,
                 "channelType": 1,
-                "id": "2154531"
+                "id": "2154531",
             },
-            "t": 108
+            "t": 108,
         }
-        await asyncio.sleep(2)
+        await asyncio.sleep(2.2)
         await self.wss.send(data)
 
     async def endVoiceChat(self, comId: str, chatId: str, leaveType: int = 2):
+        """
+        End The Voice Chat
 
+        **Parameters**
+            - **comId**: ID of the Community (str)
+            - **chatId**: ID of the Chat (str)
+            - **leaveType**: Leave type to end voice as.. (int)
+        """
         data = {
             "o": {
                 "ndcId": comId,
                 "threadId": chatId,
                 "joinRole": leaveType,
-                "id": "2154531"
+                "id": "2154531",
             },
-            "t": 112
+            "t": 112,
         }
-        await asyncio.sleep(2)
+        await asyncio.sleep(2.2)
         await self.wss.send(data)
 
     async def joinVideoChatAsSpectator(self, comId: str, chatId: str):
+        """
+        Join Video Chat As Spectator
 
+        **Parameters**
+            - **comId**: ID of the Community (str)
+            - **chatId**: ID of the Chat (str)
+        """
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": 2,
-                "id": "72446"
+                "id": "72446",
             },
-            "t": 112
+            "t": 112,
         }
-        await asyncio.sleep(2)
+        await asyncio.sleep(2.2)
         await self.wss.send(data)
 
     async def threadJoin(self, comId: str, chatId: str):
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": 1,
-                "id": "10335106"
+                "id": "10335106",
             },
-            "t": 112
+            "t": 112,
         }
         await self.wss.send(data)
 
     async def channelJoin(self, comId: str, chatId: str):
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "channelType": 5,
-                "id": "10335436"
-            },
-            "t": 108
-        }
-        await self.wss.send(data)
-
-    async def videoPlayer(self, comId: str, chatId: str, path: str, title: str, background: str, duration: int):
-        await self.actions(comId, chatId).Chatting().start()
-        await self.threadJoin(comId, chatId)
-        await self.channelJoin(comId, chatId)
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "playlist": {
-                    "currentItemIndex": 0,
-                    "currentItemStatus": 1,
-                    "items": [{
-                        "author": None,
-                        "duration": duration,
-                        "isDone": False,
-                        "mediaList": [[100, background, None]],
-                        "title": title,
-                        "type": 1,
-                        "url": f"file://{path}"
-                    }]
-                },
-                "id": "3423239"
+                "id": "10335436",
             },
-            "t": 120
+            "t": 108,
         }
         await self.wss.send(data)
-        await asyncio.sleep(2)
-        data["o"]["playlist"]["currentItemStatus"] = 2
-        data["o"]["playlist"]["items"][0]["isDone"] = True
-        await self.wss.send(data)
-
-    async def playVideo(self, comId: str, chatId: str, path: str, title: str, background: BinaryIO, duration: int):
-
-        threading.Thread(target=self.videoPlayer, args=(comId, chatId, path, title, await self.wss.uploadMedia(background, "image"), duration)).start()
 
-    async def GetUsersActions(self, comId: str, path: int = 0, chatId: str = None):
+    async def GetUsersActions(self, comId: str = None, path: int = 0, chatId: str = None):
         """
-            Get users actions:
-            This functions gets certain socket actions happening
-            such as online users and users chatting
+        Get users actions:
+        This functions gets certain socket actions happening
+        such as online users and users chatting
 
-            Parameters
+        Parameters
             ----------
             comId : int
                 the community id -required
+
             path : int
                 takes an intger >= 0 and <= 5 each one sends a certain action
                 not required -set by default to 0 // users-chatting
+
             chatId : str
                 the chatId used in certain actions such as 'users-start-typing-at -Optional
-                
+
             Returns
             ----------
-            A Class property if there is a new message it will contain a userProfileList
-            you can explore 'UsersActions' in objects file  
+        A Class property if there is a new message it will contain a userProfileList
+        you can explore 'UsersActions' in objects file
         """
         acts = {
             0: "users-chatting",
             1: "online-members",
             2: "users-start-typing-at",
             3: "users-end-typing-at",
             4: "users-start-recording-at",
-            5: "users-start-recording-at"
+            5: "users-start-recording-at",
         }
 
-        if chatId: topic = f'{acts.get(path, "users-chatting")}:{chatId}'
-        else: topic = acts.get(path, "users-chatting")
+        if chatId:
+            topic = f'{acts.get(path, "users-chatting")}:{chatId}'
+        else:
+            topic = acts.get(path, "users-chatting")
 
         data = {
             "o": {
-                "ndcId": int(comId),
+                "ndcId": int(comId) if comId else 0,
                 "topic": f"ndtopic:x{comId}:{topic}",
-                "id": "4538416"
+                "id": "4538416",
             },
-            "t": 300
+            "t": 300,
         }
 
-        asyncio.sleep(2.2)
+        await asyncio.sleep(2.2)
         await self.wss.send(data)
-        if (await self.wss.receive()): return UsersActions((await self.wss.receive())).UsersActions
-        else: print('\nWaiting for messages . . .\n')
 
-    async def actions(self, comId: str, chatId: str):
-        threading.Thread(target=await self.wss.sendWebActive, args=(comId, )).start()
+        for i in range(3):
+            data = await self.wss.receive()
+            if data:
+                return UsersActions(data=data).UsersActions
+            else:
+                continue
+
+        return UsersActions(data={}).UsersActions
+
+    def actions(self, comId: str, chatId: str):
         return Actions(self.wss, comId, chatId)
 
-class Wss(Callbacks, WssClient, Headers):
-    def __init__(self, client, Session, Trace):
+
+class Wss(AsyncCallbacks, WssClient, Headers):
+    def __init__(self, client, trace: bool = False, is_bot: bool = False):
+        self.trace = trace
+        self.socket = None
+        self.headers = None
         self.client = client
-        self.ses = Session
+        self.isOpened = False
 
         Headers.__init__(self)
-        Callbacks.__init__(self)
+        AsyncCallbacks.__init__(self, is_bot=is_bot)
         WssClient.__init__(self, self)
 
         self.narvi = "https://service.narvii.com/api/v1/"
         self.socket_url = "wss://ws1.narvii.com"
         self.lastMessage = {}
+        # websocket.enableTrace(trace)
+
+    async def onOpen(self, *args):
+        self.isOpened = True
+        if self.trace:
+            print("[ON-OPEN] Sockets are open")
+
+    async def onClose(self, *args):
         self.isOpened = False
-        self.Trace = Trace
-        self.Ran = False
-        self.socket: websockets = None
+        if self.trace:
+            print("[ON-CLOSE] Sockets are closed")
 
-        self.web_headers = self.web_headers
-        self.headers = self.headers
+    async def send(self, data):
+        await self.socket.send(json.dumps(data))
 
-    def receive(self):
+    async def receive(self):
+        if self.trace:
+            print("[RECEIVE] returning last message")
         return self.lastMessage
 
-    async def send(self, data):
-        if self.Trace:print("Sending Data")
-        data = json.dumps(data)
-        await self.socket.send(data)
+    async def on_message(self, ws, data):
+        self.lastMessage = json.loads(data)
+        await self.resolve(data)
 
-    async def on_message(self, data):
-        self.resolve(data)
+        if self.trace:
+            print("[ON-MESSAGE] Received a message . . .")
 
-    async def Runner(self):
-        final = f"{self.client.deviceId}|{int(time.time() * 1000)}"
+    async def launch(self, first_time: bool = True):
+        final = f"{self.client.deviceId}|{int(timer.time() * 1000)}"
         self.headers = {
             "NDCDEVICEID": self.client.deviceId,
             "NDCAUTH": self.client.sid,
-            "NDC-MSG-SIG": util.generateSig(data=final)}
-        try:
-            async with websockets.connect(f"{self.socket_url}/?signbody={final.replace('|', '%7C')}", extra_headers=self.headers) as webs:
-                self.socket = webs
-                self.Ran = True
-                if self.Trace: print("[Starting][Runner] Socket Started")
-                while self.Ran:
-                    try: message = await webs.recv()
-                    except websockets.exceptions.ConnectionClosedOK: continue
-                    await self.on_message(message)
-        except RuntimeError: pass
-
-    async def Launch(self):
-        if self.Trace: print("[Starting][Launch] Running Amino Sockets")
-        asyncio.create_task(self.Runner())
+            "NDC-MSG-SIG": util.generateSig(data=final),
+        }
+
+        self.socket = WebSocketApp(
+            f"{self.socket_url}/?signbody={final.replace('|', '%7C')}",
+            on_message=self.on_message,
+            on_close=self.onClose,
+            on_open=self.onOpen,
+            on_error=self.onError,
+            header=self.headers
+        )
+
+        if self.trace:
+            print("[LAUNCH] Sockets starting . . . ")
+
+        threading.Thread(target=self.run_socket_forever).start()
+
+        if first_time:
+            pass
+            # threading.Thread(target=self.reboot_socket).start()
+
+    def reboot_socket(self):
         while True:
-            await asyncio.sleep(360)
-            if self.socket.closed: return
-            await self.close()
-            asyncio.create_task(self.Runner())
-
-    async def Start(self):
-        if self.Trace:print("[Starting][Start] Starting Socket")
-        threading.Thread(target = asyncio.run, args = (self.Launch(), )).start()
+            timer.sleep(5)
+            asyncio.run(self.close())
+            self.launch(False)
+
+    def start_async(self):
+        loop = asyncio.new_event_loop()
+        th = threading.Thread(target=loop.run_forever)
+        # th.daemon = True
+        th.start()
+        return loop, th
+
+    def submit_async(self, awaitable, loop):
+        return asyncio.run_coroutine_threadsafe(awaitable, loop)
+
+    def stop_async(self, loop):
+        loop.call_soon_threadsafe(loop.stop)
+
+    def run_socket_forever(self, **kwargs):
+        loop, th = self.start_async()
+        self.wss_loop = self.submit_async(self.socket.run_forever(ping_interval=30), loop)
+        self.th = th
 
     async def close(self):
-        if self.Trace:print("[Closing][close] Closing Socket")
-
-        self.Ran = False
-        try:
-            if self.socket is not None:await self.socket.close()
-            else:
-                await asyncio.sleep(2.2)
-                await self.socket.close()
-        except Exception as e:
-            if self.Trace: print(f"[Closing][close] Error occured {e}")
-
-    async def uploadMedia(self, file: BinaryIO, fileType: str):
-        if fileType == "audio":typee = "audio/aac"
-        elif fileType == "image":typee = "image/jpg"
-        else:raise TypeError("Wrong fileType")
-
-        data = file.read()
-        self.headers["content-type"] = typee
-        self.headers["content-length"] = str(len(data))
-
-        async with self.ses.post(f"{self.narvi}/g/s/media/upload", data=data, headers=headers) as response:
-            if await response.json()["api:statuscode"] != 0: return CheckExceptions(await response.json())
-            return await response.json()["mediaValue"]
-
-    async def sendWebActive(self, comId: str):
-        data = {"ndcId": comId}
-        async with self.ses.post(webApi("/community/stats/web-user-active-time"), json=data, headers=self.web_headers) as response:
-            if await response.json()["code"] != 200: return CheckExceptions(await response.json())
-            return await response
+        # await self.socket.close()
+        self.socket._stop_ping_thread()
+        self.socket.keep_running = False
+
+        if self.socket.sock:
+            await self.socket.sock.close()
+
+        self.socket.sock = None
+        self.th.join()
+        self.stop_async(self.wss_loop)
+
+        if self.trace:
+            print("[CLOSE] closing socket . . .")
+
+        await asyncio.sleep(1.5)
+
+    async def onError(self, *args):
+        if self.trace:
+            print(f"[ERROR] Error! {args}")
+
+    def socket_status(self):
+        print("\nSockets are OPEN\n") if self.isOpened else print(
+            "\nSockets are CLOSED\n"
+        )
```

### Comparing `k-amino.py-1.1.2/setup.py` & `k-amino.py-1.2.0/setup.py`

 * *Files identical despite different names*

