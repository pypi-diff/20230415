# Comparing `tmp/k-amino.py-1.2.0.tar.gz` & `tmp/k-amino.py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-amino.py-1.2.0.tar", last modified: Sat Apr 15 10:30:51 2023, max compression
+gzip compressed data, was "k-amino.py-1.2.1.tar", last modified: Sat Apr 15 11:16:34 2023, max compression
```

## Comparing `k-amino.py-1.2.0.tar` & `k-amino.py-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.818515 k-amino.py-1.2.0/
--rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2143 2023-04-15 10:30:51.819499 k-amino.py-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.681112 k-amino.py-1.2.0/k_amino/
--rw-rw-rw-   0        0        0      872 2023-04-14 09:14:24.000000 k-amino.py-1.2.0/k_amino/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.726156 k-amino.py-1.2.0/k_amino/k_async/
--rw-rw-rw-   0        0        0      122 2023-04-09 03:38:43.000000 k-amino.py-1.2.0/k_amino/k_async/__init__.py
--rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.2.0/k_amino/k_async/acm.py
--rw-rw-rw-   0        0        0     2392 2023-04-15 05:50:54.000000 k-amino.py-1.2.0/k_amino/k_async/bot.py
--rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.2.0/k_amino/k_async/client.py
--rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.2.0/k_amino/k_async/local.py
--rw-rw-rw-   0        0        0    27516 2023-04-15 09:39:33.000000 k-amino.py-1.2.0/k_amino/k_async/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.772265 k-amino.py-1.2.0/k_amino/k_async/websocket_async/
--rw-rw-rw-   0        0        0      801 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/__init__.py
--rw-rw-rw-   0        0        0    13388 2023-04-14 11:31:01.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_abnf.py
--rw-rw-rw-   0        0        0    20107 2023-04-15 10:19:58.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_app.py
--rw-rw-rw-   0        0        0     2118 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_cookiejar.py
--rw-rw-rw-   0        0        0    20129 2023-04-15 10:09:33.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_core.py
--rw-rw-rw-   0        0        0     2105 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_exceptions.py
--rw-rw-rw-   0        0        0     6073 2023-04-14 11:59:23.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_handshake.py
--rw-rw-rw-   0        0        0    11803 2023-04-14 12:04:01.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_http.py
--rw-rw-rw-   0        0        0     2027 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_logging.py
--rw-rw-rw-   0        0        0     4922 2023-04-14 12:08:35.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_socket.py
--rw-rw-rw-   0        0        0     1122 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_ssl_compat.py
--rw-rw-rw-   0        0        0     4797 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_url.py
--rw-rw-rw-   0        0        0     3516 2023-04-14 11:23:07.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_utils.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 03:38:42.000000 k-amino.py-1.2.0/k_amino/k_async/websocket_async/_wsdump.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.791748 k-amino.py-1.2.0/k_amino/k_sync/
--rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.2.0/k_amino/k_sync/__init__.py
--rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.2.0/k_amino/k_sync/acm.py
--rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.2.0/k_amino/k_sync/bot.py
--rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.2.0/k_amino/k_sync/client.py
--rw-rw-rw-   0        0        0    45202 2023-04-15 06:24:52.000000 k-amino.py-1.2.0/k_amino/k_sync/local.py
--rw-rw-rw-   0        0        0    24349 2023-04-15 06:31:22.000000 k-amino.py-1.2.0/k_amino/k_sync/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.816284 k-amino.py-1.2.0/k_amino/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-04-14 13:36:56.000000 k-amino.py-1.2.0/k_amino/lib/async_sessions.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/exception.py
--rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/headers.py
--rw-rw-rw-   0        0        0   198102 2023-04-15 05:49:07.000000 k-amino.py-1.2.0/k_amino/lib/objects.py
--rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.2.0/k_amino/lib/sessions.py
--rw-rw-rw-   0        0        0     1688 2023-04-09 07:16:48.000000 k-amino.py-1.2.0/k_amino/lib/util.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:51.705657 k-amino.py-1.2.0/k_amino.py.egg-info/
--rw-rw-rw-   0        0        0     2143 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1297 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 10:30:51.000000 k-amino.py-1.2.0/k_amino.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 10:30:51.823500 k-amino.py-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.507357 k-amino.py-1.2.1/
+-rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2143 2023-04-15 11:16:34.508470 k-amino.py-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.384998 k-amino.py-1.2.1/k_amino/
+-rw-rw-rw-   0        0        0      872 2023-04-15 11:11:31.000000 k-amino.py-1.2.1/k_amino/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.427845 k-amino.py-1.2.1/k_amino/k_async/
+-rw-rw-rw-   0        0        0      122 2023-04-09 03:38:43.000000 k-amino.py-1.2.1/k_amino/k_async/__init__.py
+-rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.2.1/k_amino/k_async/acm.py
+-rw-rw-rw-   0        0        0     2392 2023-04-15 05:50:54.000000 k-amino.py-1.2.1/k_amino/k_async/bot.py
+-rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.2.1/k_amino/k_async/client.py
+-rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.2.1/k_amino/k_async/local.py
+-rw-rw-rw-   0        0        0    27434 2023-04-15 11:12:16.000000 k-amino.py-1.2.1/k_amino/k_async/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.466628 k-amino.py-1.2.1/k_amino/k_async/websocket_async/
+-rw-rw-rw-   0        0        0      801 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/__init__.py
+-rw-rw-rw-   0        0        0    13388 2023-04-14 11:31:01.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_abnf.py
+-rw-rw-rw-   0        0        0    20115 2023-04-15 11:13:22.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_app.py
+-rw-rw-rw-   0        0        0     2118 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_cookiejar.py
+-rw-rw-rw-   0        0        0    20129 2023-04-15 10:09:33.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_core.py
+-rw-rw-rw-   0        0        0     2105 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_exceptions.py
+-rw-rw-rw-   0        0        0     6073 2023-04-14 11:59:23.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_handshake.py
+-rw-rw-rw-   0        0        0    11803 2023-04-14 12:04:01.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_http.py
+-rw-rw-rw-   0        0        0     2027 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_logging.py
+-rw-rw-rw-   0        0        0     4922 2023-04-14 12:08:35.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_socket.py
+-rw-rw-rw-   0        0        0     1122 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_ssl_compat.py
+-rw-rw-rw-   0        0        0     4797 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_url.py
+-rw-rw-rw-   0        0        0     3516 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_utils.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 03:38:42.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_wsdump.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.483954 k-amino.py-1.2.1/k_amino/k_sync/
+-rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.2.1/k_amino/k_sync/__init__.py
+-rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.2.1/k_amino/k_sync/acm.py
+-rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.2.1/k_amino/k_sync/bot.py
+-rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.2.1/k_amino/k_sync/client.py
+-rw-rw-rw-   0        0        0    45202 2023-04-15 06:24:52.000000 k-amino.py-1.2.1/k_amino/k_sync/local.py
+-rw-rw-rw-   0        0        0    24349 2023-04-15 06:31:22.000000 k-amino.py-1.2.1/k_amino/k_sync/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.504349 k-amino.py-1.2.1/k_amino/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-04-14 13:36:56.000000 k-amino.py-1.2.1/k_amino/lib/async_sessions.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/exception.py
+-rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/headers.py
+-rw-rw-rw-   0        0        0   198102 2023-04-15 05:49:07.000000 k-amino.py-1.2.1/k_amino/lib/objects.py
+-rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/sessions.py
+-rw-rw-rw-   0        0        0     1688 2023-04-09 07:16:48.000000 k-amino.py-1.2.1/k_amino/lib/util.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.406671 k-amino.py-1.2.1/k_amino.py.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-04-15 11:16:34.000000 k-amino.py-1.2.1/k_amino.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 11:16:34.512576 k-amino.py-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.2.1/setup.py
```

### Comparing `k-amino.py-1.2.0/LICENSE` & `k-amino.py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/PKG-INFO` & `k-amino.py-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.2.0/README.md` & `k-amino.py-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/__init__.py` & `k-amino.py-1.2.1/k_amino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .k_async.acm import AsyncAcm
 from .k_async.client import AsyncClient
 from .k_async.local import AsyncSubClient
 # from .k_async.sockets import *
 from .k_async.bot import AsyncBot
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 __newest__ = loads(get("https://pypi.python.org/pypi/k-amino.py/json").text)["info"]["version"]
 
 if __version__ != __newest__:
     print(f"\033[1;31;38mk_amino New Version!: {__newest__} (You are using {__version__})\033[1;36;33m\nDiscord server: \"https://discord.gg/zd8gyFJquT\"\033[1;0m")
 else:
```

### Comparing `k-amino.py-1.2.0/k_amino/k_async/acm.py` & `k-amino.py-1.2.1/k_amino/k_async/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/bot.py` & `k-amino.py-1.2.1/k_amino/k_async/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/client.py` & `k-amino.py-1.2.1/k_amino/k_async/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/local.py` & `k-amino.py-1.2.1/k_amino/k_async/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/sockets.py` & `k-amino.py-1.2.1/k_amino/k_async/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 class AsyncCallbacks(Bot):
     def __init__(self, is_bot: bool = False, prefix: str = "!"):
         Bot.__init__(self, prefix=prefix)
 
         # if the user want to use the script as a bot
         self.is_bot = is_bot
-        self.lock_command = False
 
         self.handlers = {}
 
         self.methods = {
             10: self._resolve_payload,
             201: self._resolve_channel,
             304: self._resolve_chat_action_start,
@@ -667,27 +666,27 @@
 
         if self.trace:
             print("[LAUNCH] Sockets starting . . . ")
 
         threading.Thread(target=self.run_socket_forever).start()
 
         if first_time:
-            pass
-            # threading.Thread(target=self.reboot_socket).start()
+            loop, th = self.start_async()
+            loop = self.submit_async(self.reboot_socket(), loop)
 
-    def reboot_socket(self):
-        while True:
-            timer.sleep(5)
-            asyncio.run(self.close())
-            self.launch(False)
+    async def reboot_socket(self):
+        self.run_reboot = True
+        while self.run_reboot:
+            await asyncio.sleep(120)
+            await self.close()
+            await self.launch(False)
 
     def start_async(self):
         loop = asyncio.new_event_loop()
         th = threading.Thread(target=loop.run_forever)
-        # th.daemon = True
         th.start()
         return loop, th
 
     def submit_async(self, awaitable, loop):
         return asyncio.run_coroutine_threadsafe(awaitable, loop)
 
     def stop_async(self, loop):
@@ -695,24 +694,21 @@
 
     def run_socket_forever(self, **kwargs):
         loop, th = self.start_async()
         self.wss_loop = self.submit_async(self.socket.run_forever(ping_interval=30), loop)
         self.th = th
 
     async def close(self):
-        # await self.socket.close()
         self.socket._stop_ping_thread()
         self.socket.keep_running = False
 
         if self.socket.sock:
             await self.socket.sock.close()
 
         self.socket.sock = None
-        self.th.join()
-        self.stop_async(self.wss_loop)
 
         if self.trace:
             print("[CLOSE] closing socket . . .")
 
         await asyncio.sleep(1.5)
 
     async def onError(self, *args):
```

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/__init__.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/__init__.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_abnf.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_abnf.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_app.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,15 @@
 
             if not reconnecting:
                 await self._callback(self.on_error, e)
             if isinstance(e, (KeyboardInterrupt, SystemExit)):
                 await teardown()
                 # Propagate further
                 raise
-            if reconnect:
+            if reconnect or True:
                 _logging.info("%s - reconnect" % e)
                 if custom_dispatcher:
                     _logging.debug("Calling custom dispatcher reconnect [%s frames in stack]" % len(inspect.stack()))
                     await dispatcher.reconnect(reconnect, setSock)
             else:
                 _logging.error("%s - goodbye" % e)
                 # print("WEBSOCKET", type(e), e)
```

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_cookiejar.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_core.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_core.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_exceptions.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_exceptions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_handshake.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_handshake.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_http.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_http.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_logging.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_logging.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_socket.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_socket.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_ssl_compat.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_url.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_url.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_utils.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_utils.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_async/websocket_async/_wsdump.py` & `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_wsdump.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_sync/acm.py` & `k-amino.py-1.2.1/k_amino/k_sync/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_sync/bot.py` & `k-amino.py-1.2.1/k_amino/k_sync/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_sync/client.py` & `k-amino.py-1.2.1/k_amino/k_sync/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_sync/local.py` & `k-amino.py-1.2.1/k_amino/k_sync/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/k_sync/sockets.py` & `k-amino.py-1.2.1/k_amino/k_sync/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/lib/async_sessions.py` & `k-amino.py-1.2.1/k_amino/lib/async_sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/lib/exception.py` & `k-amino.py-1.2.1/k_amino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/lib/headers.py` & `k-amino.py-1.2.1/k_amino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/lib/objects.py` & `k-amino.py-1.2.1/k_amino/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/lib/sessions.py` & `k-amino.py-1.2.1/k_amino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino/lib/util.py` & `k-amino.py-1.2.1/k_amino/lib/util.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/k_amino.py.egg-info/PKG-INFO` & `k-amino.py-1.2.1/k_amino.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.2.0/k_amino.py.egg-info/SOURCES.txt` & `k-amino.py-1.2.1/k_amino.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.0/setup.py` & `k-amino.py-1.2.1/setup.py`

 * *Files identical despite different names*

