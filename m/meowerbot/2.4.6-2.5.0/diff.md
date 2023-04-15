# Comparing `tmp/meowerbot-2.4.6.tar.gz` & `tmp/meowerbot-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.4.6.tar", max compression
+gzip compressed data, was "meowerbot-2.5.0.tar", max compression
```

## Comparing `meowerbot-2.4.6.tar` & `meowerbot-2.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.4.6/LICENSE
--rw-r--r--   0        0        0      154 2023-03-25 06:29:26.519423 meowerbot-2.4.6/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-03-25 06:14:31.584953 meowerbot-2.4.6/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1321 2023-03-25 06:14:31.578955 meowerbot-2.4.6/MeowerBot/API.py
--rw-r--r--   0        0        0    12319 2023-03-25 06:28:28.818441 meowerbot-2.4.6/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.4.6/MeowerBot/cloudlink/__init__.py
--rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.4.6/MeowerBot/cloudlink/cloudlink.py
--rw-r--r--   0        0        0      738 2023-03-25 06:14:31.585951 meowerbot-2.4.6/MeowerBot/cog.py
--rw-r--r--   0        0        0     1510 2023-03-25 06:14:31.586953 meowerbot-2.4.6/MeowerBot/command.py
--rw-r--r--   0        0        0     2087 2023-03-25 06:16:14.726304 meowerbot-2.4.6/MeowerBot/context.py
--rw-r--r--   0        0        0      566 2023-03-25 06:29:31.002992 meowerbot-2.4.6/pyproject.toml
--rw-r--r--   0        0        0      244 2023-02-15 00:38:57.660810 meowerbot-2.4.6/README.md
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.4.6/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.0/LICENSE
+-rw-r--r--   0        0        0      154 2023-04-15 02:29:06.934850 meowerbot-2.5.0/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.0/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1384 2023-04-15 02:05:09.867583 meowerbot-2.5.0/MeowerBot/API.py
+-rw-r--r--   0        0        0    13566 2023-04-15 01:49:29.377831 meowerbot-2.5.0/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.0/MeowerBot/cloudlink/__init__.py
+-rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.0/MeowerBot/cloudlink/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.0/MeowerBot/cog.py
+-rw-r--r--   0        0        0     2084 2023-04-15 02:19:55.402707 meowerbot-2.5.0/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.0/MeowerBot/context.py
+-rw-r--r--   0        0        0      566 2023-04-15 02:29:17.590678 meowerbot-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.0/README.md
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.0/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.0/PKG-INFO
```

### Comparing `meowerbot-2.4.6/LICENSE` & `meowerbot-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.4.6/MeowerBot/API.py` & `meowerbot-2.5.0/MeowerBot/API.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import requests
 from urllib.parse import urljoin
 
 
 class MeowerAPI:
     base_uri = "https://api.meower.org/"
 
-    def __init__(self, token, username):
+    def __init__(self, username):
 
         self.session = requests.session()
-        self.session.headers.update({"token": token, "usename": username})
+        self.session.headers.update({"usename": username})
+
+    def login(self, token):
+        self.session.headers.update({"token": token})
 
     def get_page(self, page=1, chatid="home"):
         if chatid == "home":
             return self.session.get(
                 urljoin(self.base_uri, "/home?autoget&page={0}".format(page))
             ).json()
         else:
```

### Comparing `meowerbot-2.4.6/MeowerBot/Bot.py` & `meowerbot-2.5.0/MeowerBot/Bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 from .command import AppCommand
 from .context import CTX
 
 import time
 import logging
 
-from websocket._exceptions import WebSocketConnectionClosedException
+from .API import MeowerAPI
+
+from websocket._exceptions import WebSocketConnectionClosedException, WebSocketException
 
 
 class Bot:
     """
     A class that holds all of the networking for a meower bot to function and run
 
     """
@@ -49,14 +51,15 @@
             time.sleep(60)
 
             self.wss.sendPacket({"cmd": "ping", "val": ""})
 
     def __init__(self, prefix=None, autoreload: int or None = None): #type: ignore
         self.wss = CloudLink()
         self.callbacks = {}
+        self._last_to = "Home"
 
         self.wss.callback(
             "on_packet", self._debug_fix
         )  # self._debug_fix catches all errors
         self.wss.callback("on_error", self.__handle_error__)  # handle uncought errors
         self.wss.callback("on_close", self.__handle_close__)  # Websocket disconnected
         self.wss.callback(
@@ -66,16 +69,16 @@
         # to be used in start
         self.username = None
         self.password = None
         self.logger_in = False
 
         if autoreload:
             self.autoreload = True
-            self.autoreload_time = autoreload + 1
-            self.autoreload_original = autoreload + 1
+            self.autoreload_time = min(autoreload, 1)
+            self.autoreload_original = min(autoreload, 1)
         else:
             self.autoreload = False
             self.autoreload_time = 0
             self.autoreload_original = 0
 
         self.commands = {}
         self.prefix = prefix
@@ -205,15 +208,15 @@
 
         elif listener == "__meowerbot__login":
             if status == "E:104 | Internal":
                 requests.post(
                     "https://webhooks.meower.org/post/home",
                     json={
                         "post": "ERROR: MeowerBot.py Webhooks Logging\n\n Account Softlocked.",
-                        "username": self.username,
+                         "username": self.username,
                     },
                 )
                 print("CRITICAL ERROR! ACCOUNT SOFTLOCKED!!!!.", file=sys.__stdout__)
                 self.bad_exit = True
                 self.wss.stop()
                 return
 
@@ -221,36 +224,36 @@
                 raise RuntimeError("Password Or Username Is Incorrect")
 
             time.sleep(0.5)
             self.run_cb("login", args=(), kwargs={})
 
         elif listener == "__meowerbot__send_message":
             if status == "I:100 | OK":
+                self.autoreload_time = self.autoreload_original
                 return  # This is just checking if a post went OK
-            
-            self.autoreload_time = self.autoreload_original #autoreload time should reset if 
+            #autoreload time should reset if 
+
+
             raise RuntimeError("Post Failed to send")
+        
 
     def callback(self, callback, cbid=None):
         """Connects a callback ID to a callback"""
         if cbid is None:
             cbid = callback.__name__
 
         if cbid not in self.callbacks:
             self.callbacks[cbid] = []
         self.callbacks[cbid].append(callback)
 
     def __handle_close__(self, *args, **kwargs):
         if self.autoreload:
             self.autoreload = False #to stop race condisons 
             self.logger_in = True
-            if not self.autoreload_time >= 100: self.autoreload_time *= 1.2 
-            
-            else:
-                 self.autoreload_time = 100
+            self.autoreload_time *= 1.2 
             
             
             time.sleep(self.autoreload_time)
             self.autoreload = True #reset this, as i set it to false above.
 
             self.wss.state = 0 #type: ignore
             self.wss.client(self.server) #type: ignore
@@ -290,16 +293,23 @@
 
                 self.run_command(ctx.message)
 
             self.run_cb("raw_message", args=(packet["val"],))
 
         elif packet["cmd"] == "direct":
             listener = packet.get("listener")
+
+            if listener == "mb_get_chat_list":
+                self.run_cb("chat_list", args=(packet["val"]["payload"], listener))
+            elif listener == "__meowerbot__login":
+                self.api.login(packet['val']['payload']['token'])
             self.run_cb("direct", args=(packet["val"], listener))
 
+        
+
         else:
             listener = packet.get("listener")
             self.run_cb(packet["cmd"], args=(packet["val"], listener))
 
         
         if (packet["cmd"] == "pmsg") and  (packet["val"] not in self.BOT_NO_PMSG_RESPONSE):
             self.wss.sendPacket({
@@ -313,30 +323,37 @@
 
         try:
             self.commands[args[0]]["command"].run_cmd(message.ctx, *args[1:])
         except KeyError as e:
             self.run_cb("error", args=(e,))
 
     def send_msg(self, msg, to="home"):
-        if to == "home":
-            self.wss.sendPacket(
-                {
-                    "cmd": "direct",
-                    "val": {"cmd": "post_home", "val": msg},
-                    "listener": "__meowerbot__send_message",
-                }
-            )
-        else:
-            self.wss.sendPacket(
-                {
-                    "cmd": "direct",
-                    "val": {"cmd": "post_chat", "val": {"chatid": to, "p": msg}},
-                    "listener": "__meowerbot__send_message",
-                }
-            )
+        self._last_to = to
+        self._last_sent = msg
+        try:
+            if to == "home":
+                self.wss.sendPacket(
+                    {
+                        "cmd": "direct",
+                        "val": {"cmd": "post_home", "val": msg},
+                        "listener": "__meowerbot__send_message",
+                    }
+                )
+            else:
+                self.wss.sendPacket(
+                    {
+                        "cmd": "direct",
+                        "val": {"cmd": "post_chat", "val": {"chatid": to, "p": msg}},
+                        "listener": "__meowerbot__send_message",
+                    }
+                )
+        #socket is closed, use webhooks
+        except WebSocketException as e:
+            self.run_cb(cbid="error", args=(e,))
+            
 
     def send_typing(self, to="home"):
         if  to == "home":
             self.wss.sendPacket(
                 {
                     "cmd": "direct",
                     "val": {
@@ -357,29 +374,57 @@
                     "val": {
                         "chatid": to,
                         "state": 100,
                     },
                 },
             }
           )
-       
+        
     def enter_chat(self, chatid="livechat"):
         self.wss.sendPacket(
             {
                 "cmd": "direct",
                 "val": {
                     "cmd": "set_chat_state",
                     "val": {
                         "chatid": chatid,
                         "state": 1,
                     },
                 },
             }
         )
 
+    def create_chat(self, name):
+        """
+        Unstable, use at your own risk
+
+        comes with callbacks: chat_list 
+        """
+        self.wss.sendPacket({
+            "cmd": "direct",
+            "val": {
+                "cmd": "create_chat",
+                "val": name
+            },
+            "listener": "mb_create_chat"
+        })
+
+        time.sleep(secs=0.5)
+
+        self.wss.sendPacket({
+            "cmd": "direct",
+            "val": {
+                "cmd": "get_chat_list",
+                "val": {
+                    "page": 1
+                }
+            },
+            "listener": "mb_get_chat_list"
+        })
+
 
     def run(self, username, password, server="wss://server.meower.org"):
         """
         Runs The bot (Blocking)
         """
         self.username = username
         self._password = password
@@ -387,10 +432,11 @@
 
         self._t_ping_thread.start()
         if self.prefix is None:
             self.prefix = "@" + self.username
         self.logger = logging.getLogger(f"MeowerBot {self.username}")
         self.server = server
         self.wss.client(server)
+        self.api = API(self)
 
         if self.bad_exit:
             raise BaseException("Bot Account Softlocked")
```

### Comparing `meowerbot-2.4.6/MeowerBot/cloudlink/cloudlink.py` & `meowerbot-2.5.0/MeowerBot/cloudlink/cloudlink.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.4.6/MeowerBot/cog.py` & `meowerbot-2.5.0/MeowerBot/cog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .command import AppCommand
+from .command import AppCommand, command
 import weakref
 
 
 class Cog:
     __commands__ = None
     __instence__ = None
```

### Comparing `meowerbot-2.4.6/MeowerBot/command.py` & `meowerbot-2.5.0/MeowerBot/command.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,22 +11,41 @@
 
         self.name = name
         self.func = func
         self.args = args
 
         self.arg_names = inspect.getfullargspec(func)[0]
         self.arg_types = func.__annotations__
+        self.subcommands = {}
 
     def __call__(self, *args):
         raise RuntimeError("AppCommand is not callable")
 
     def register_class(self, con):
         self.connected = con
 
+    def subcommand(self, name=None, args=0):
+        def inner(func):
+
+            cmd = AppCommand(func, name=name, args=args)
+            cmd.register_class(self.connected)
+
+            self.subcommands[name] = cmd.info()
+
+
+            return func #dont want mb to register this as a root command
+
+        return inner
+
     def run_cmd(self, ctx, *args):
+        
+        if self.subcommands and (args[0] if len(args) >= 1 else None) in self.subcommands:
+            self.subcommands[args[0]]["command"].run_cmd(ctx, *args[1:])
+            return
+        
         if not self.args == 0:
             args = args[: self.args]
 
         if self.connected is None:
             self.func(ctx, *args)
         else:
             self.func(self.connected, ctx, *args)
@@ -35,14 +54,15 @@
         return {
             self.name: {
                 "args": self.args,
                 "arg_names": self.arg_names,
                 "arg_types": self.arg_types,
                 "command": self,
                 "func": self.func,
+
             }
         }
 
 
 class _Command(AppCommand):
     def __init__(self, func, *args, name=None, **kwargs):
         super().__init__(func, *args, name=name, **kwargs)
```

### Comparing `meowerbot-2.4.6/MeowerBot/context.py` & `meowerbot-2.5.0/MeowerBot/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,48 +3,30 @@
 import typing
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .Bot import Bot
 
 import weakref
+import requests
 
 
 class User:
     def __init__(self, bot, username):
         self.username = username
-        self._raw = None
-
+        
         self.bot = bot
-        self.bot.wss.sendPacket(
-            {
-                "cmd": "direct",
-                "val": {"cmd": "get_profile", "val": self.username},
-                "listener": f"get_user_{self.username}",
-            }
-        )
-
-        self.level = 0
-        self.pfp = 0
-        self.quote = ""
-
-    def _handle_usr_data(self, val, listener):
-        if listener is None:
-            return
-        if listener is not f"get_user_{self.username}":
-            return
-        if "mode" not in val or not val["mode"] == "profile":
-            return
+        self._raw = self.bot.api.get_user(self.username)
 
-        # checks are finaly over lmao
-        self._raw = val["payload"]
         self.level = self._raw["lvl"]
         self.pfp = self._raw["pfp_data"]
         self.quote = self._raw["quote"]
 
+    
+
     def ping(self, msg, to="home"):
         self.bot.send_msg(f"@{self.username} {msg}", to=to)
 
     def __str__(self):
         return str(self.__dict__)
```

### Comparing `meowerbot-2.4.6/pyproject.toml` & `meowerbot-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.4.6"
+version = "2.5.0"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
```

### Comparing `meowerbot-2.4.6/setup.py` & `meowerbot-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.4.6',
+    'version': '2.5.0',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
```

### Comparing `meowerbot-2.4.6/PKG-INFO` & `meowerbot-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.4.6
+Version: 2.5.0
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

