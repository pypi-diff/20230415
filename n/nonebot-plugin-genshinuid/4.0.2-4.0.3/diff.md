# Comparing `tmp/nonebot_plugin_genshinuid-4.0.2.tar.gz` & `tmp/nonebot_plugin_genshinuid-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshinuid-4.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshinuid-4.0.3.tar", max compression
```

## Comparing `nonebot_plugin_genshinuid-4.0.2.tar` & `nonebot_plugin_genshinuid-4.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    14037 2023-04-06 16:10:41.216594 nonebot_plugin_genshinuid-4.0.2/GenshinUID/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-06 14:38:25.709357 nonebot_plugin_genshinuid-4.0.2/GenshinUID/auto_install.py
--rw-r--r--   0        0        0    22427 2023-04-07 17:32:00.585344 nonebot_plugin_genshinuid-4.0.2/GenshinUID/client.py
--rw-r--r--   0        0        0     1004 2023-04-02 16:27:11.522237 nonebot_plugin_genshinuid-4.0.2/GenshinUID/models.py
--rw-r--r--   0        0        0      336 2023-04-06 14:38:25.734782 nonebot_plugin_genshinuid-4.0.2/GenshinUID/path.py
--rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.2/LICENSE
--rw-r--r--   0        0        0     1613 2023-04-07 18:29:47.524391 nonebot_plugin_genshinuid-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     3318 2023-03-25 16:39:34.235973 nonebot_plugin_genshinuid-4.0.2/README.md
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0    14731 2023-04-15 16:16:49.431629 nonebot_plugin_genshinuid-4.0.3/GenshinUID/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-14 17:44:32.922572 nonebot_plugin_genshinuid-4.0.3/GenshinUID/auto_install.py
+-rw-r--r--   0        0        0    23262 2023-04-15 16:24:47.352109 nonebot_plugin_genshinuid-4.0.3/GenshinUID/client.py
+-rw-r--r--   0        0        0     1004 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.3/GenshinUID/models.py
+-rw-r--r--   0        0        0      336 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.3/GenshinUID/path.py
+-rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.3/LICENSE
+-rw-r--r--   0        0        0     1652 2023-04-15 16:27:28.995575 nonebot_plugin_genshinuid-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3318 2023-04-14 17:44:32.924573 nonebot_plugin_genshinuid-4.0.3/README.md
+-rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_genshinuid-4.0.2/GenshinUID/__init__.py` & `nonebot_plugin_genshinuid-4.0.3/GenshinUID/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,36 +7,50 @@
 
 import aiofiles
 from nonebot.log import logger
 from nonebot.adapters import Bot
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.internal.adapter import Event
-from nonebot import on_notice, get_driver, on_message, on_fullmatch
+from websockets.exceptions import ConnectionClosed
+from nonebot import require, on_notice, on_message, on_fullmatch
 
-from .client import GsClient
-from .auto_install import start, install
-from .models import Message, MessageReceive
+require('nonebot_plugin_apscheduler')
+
+from nonebot_plugin_apscheduler import scheduler  # noqa:E402
+
+from .client import GsClient, driver  # noqa:E402
+from .auto_install import start, install  # noqa:E402
+from .models import Message, MessageReceive  # noqa:E402
 
 get_message = on_message(priority=999)
 get_notice = on_notice(priority=999)
 install_core = on_fullmatch('gs一键安装', permission=SUPERUSER, block=True)
 start_core = on_fullmatch('启动core', permission=SUPERUSER, block=True)
 connect_core = on_fullmatch(
     ('连接core', '链接core'), permission=SUPERUSER, block=True
 )
-driver = get_driver()
-gsclient: Optional[GsClient] = None
 
+gsclient: Optional[GsClient] = None
 command_start = driver.config.command_start
 
+if hasattr(driver.config, 'gsuid_core_repeat'):
+    is_repeat = True
+else:
+    is_repeat = False
+
 
 @get_notice.handle()
 async def get_notice_message(bot: Bot, ev: Event):
-    if gsclient is None or not gsclient.is_alive:
+    if gsclient is None:
+        return await connect()
+
+    try:
+        await gsclient.ws.ping()
+    except ConnectionClosed:
         return await connect()
 
     raw_data = ev.dict()
     logger.debug(raw_data)
 
     try:
         user_id = str(ev.get_user_id())
@@ -373,19 +387,32 @@
         await connect()
 
 
 async def connect():
     global gsclient
     try:
         gsclient = await GsClient().async_connect()
-        await gsclient.start()
     except ConnectionRefusedError:
         logger.error('Core服务器连接失败...请稍后使用[启动core]命令启动...')
 
 
+@scheduler.scheduled_job('cron', second='*/10')
+async def repeat_connect():
+    if is_repeat:
+        global gsclient
+        if gsclient is None:
+            await connect()
+        else:
+            try:
+                await gsclient.ws.ensure_open()
+            except ConnectionClosed:
+                return await connect()
+        return
+
+
 def convert_message(_msg: Any, message: List[Message], index: int):
     if _msg.type == 'text':
         data: str = (
             _msg.data['text'] if 'text' in _msg.data else _msg.data['content']
         )
         if index == 0:
             if data.startswith(tuple(command_start)):
```

### Comparing `nonebot_plugin_genshinuid-4.0.2/GenshinUID/auto_install.py` & `nonebot_plugin_genshinuid-4.0.3/GenshinUID/auto_install.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.2/GenshinUID/client.py` & `nonebot_plugin_genshinuid-4.0.3/GenshinUID/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import os
 import json
 import time
+import uuid
 import base64
 import asyncio
 from pathlib import Path
 from typing import Any, Dict, List, Union, Optional
 
 import websockets.client
 from nonebot.log import logger
 from nonebot.adapters import Bot
 from msgspec import json as msgjson
 from nonebot import get_bot, get_bots, get_driver
 from websockets.exceptions import ConnectionClosedError
 
 from .models import MessageSend, MessageReceive
 
-BOT_ID = 'NoneBot2'
 bots: Dict[str, str] = {}
 driver = get_driver()
 
+if hasattr(driver.config, 'gsuid_core_botid'):
+    BOT_ID = str(uuid.uuid4())[:10]
+else:
+    BOT_ID = 'NoneBot2'
+
 if hasattr(driver.config, 'gsuid_core_host'):
     HOST = driver.config.gsuid_core_host
 else:
     HOST = 'localhost'
 
 if hasattr(driver.config, 'gsuid_core_port'):
     PORT = driver.config.gsuid_core_port
@@ -40,27 +45,37 @@
                 break
     bot_real_id = bots[bot_id]
     bot = get_bot(bot_real_id)
     return bot
 
 
 class GsClient:
+    _instance = None
+
     @classmethod
     async def async_connect(cls, IP: str = HOST, PORT: Union[str, int] = PORT):
         self = GsClient()
         cls.is_alive = True
         cls.ws_url = f'ws://{IP}:{PORT}/ws/{BOT_ID}'
         logger.info(f'Bot_ID: {BOT_ID}连接至[gsuid-core]: {self.ws_url}...')
         cls.ws = await websockets.client.connect(
             cls.ws_url, max_size=2**26, open_timeout=60, ping_timeout=60
         )
         logger.success(f'与[gsuid-core]成功连接! Bot_ID: {BOT_ID}')
         cls.msg_list = asyncio.queues.Queue()
+        cls.pending = []
+        await self.start()
         return self
 
+    def __new__(cls, *args, **kwargs):
+        # 判断sv是否已经被初始化
+        if cls._instance is None:
+            cls._instance = super(GsClient, cls).__new__(cls, *args, **kwargs)
+        return cls._instance
+
     async def recv_msg(self):
         try:
             global bots
             await asyncio.sleep(5)
             _bots = get_bots()
             for bot_real_id in _bots:
                 bot = _bots[bot_real_id]
@@ -195,35 +210,42 @@
                                 msg.target_type,
                             )
                 except Exception as e:
                     logger.error(e)
         except RuntimeError as e:
             logger.error(e)
         except ConnectionClosedError:
+            for task in self.pending:
+                task.cancel()
             logger.warning(f'与[gsuid-core]断开连接! Bot_ID: {BOT_ID}')
-            self.is_alive = False
+            for _ in range(30):
+                await asyncio.sleep(5)
+                try:
+                    await self.async_connect()
+                    await self.start()
+                    break
+                except:  # noqa
+                    logger.debug('自动连接core服务器失败...五秒后重新连接...')
 
     async def _input(self, msg: MessageReceive):
         await self.msg_list.put(msg)
 
     async def send_msg(self):
         while True:
             msg: MessageReceive = await self.msg_list.get()
             msg_send = msgjson.encode(msg)
             await self.ws.send(msg_send)
 
     async def start(self):
         recv_task = asyncio.create_task(self.recv_msg())
         send_task = asyncio.create_task(self.send_msg())
-        _, pending = await asyncio.wait(
+        _, self.pending = await asyncio.wait(
             [recv_task, send_task],
             return_when=asyncio.FIRST_COMPLETED,
         )
-        for task in pending:
-            task.cancel()
 
 
 def to_json(msg: str, name: str, uin: int):
     return {
         'type': 'node',
         'data': {'name': name, 'uin': uin, 'content': msg},
     }
@@ -247,20 +269,22 @@
     node: Optional[List[Dict]],
     file: Optional[str],
     at_list: Optional[List[str]],
     target_id: Optional[str],
     target_type: Optional[str],
 ):
     async def _send(content: Optional[str], image: Optional[str]):
-        result_image = f'[CQ:image,file={image}]' if image else ''
-        content = content if content else ''
-        result_msg = content + result_image
+        from nonebot.adapters.onebot.v11 import MessageSegment
+
+        result_image = MessageSegment.image(image) if image else ''
+        _content = MessageSegment.text(content) if content else ''
+        result_msg = _content + result_image
         if at_list and target_type == 'group':
             for at in at_list:
-                result_msg += f'[CQ:at,qq={at}]'
+                result_msg += MessageSegment.at(at)
 
         if file:
             file_name, file_content = file.split('|')
             path = Path(__file__).resolve().parent / file_name
             store_file(path, file_content)
             if target_type == 'group':
                 await bot.call_api(
```

### Comparing `nonebot_plugin_genshinuid-4.0.2/GenshinUID/models.py` & `nonebot_plugin_genshinuid-4.0.3/GenshinUID/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.2/LICENSE` & `nonebot_plugin_genshinuid-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.2/pyproject.toml` & `nonebot_plugin_genshinuid-4.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nonebot-plugin-genshinuid"
-version = "4.0.2"
+version = "4.0.3"
 description = "支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件"
 authors = ["KimigaiiWuyi <444835641@qq.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2"
 repository = "https://github.com/KimigaiiWuyi/GenshinUID"
 documentation = "https://docs.gsuid.gbots.work/#/"
@@ -43,14 +43,15 @@
 python = "^3.8.1"
 nonebot2 = ">=2.0.0b4"
 pillow = ">=9.2.0"
 gitpython = ">=3.1.27"
 msgspec = ">=0.13.1"
 aiofiles = ">=23.1.0"
 websockets = ">=11.0.1"
+nonebot-plugin-apscheduler = "^0.2.0"
 
 [[tool.poetry.source]]
 name = "USTC"
 url = "https://pypi.mirrors.ustc.edu.cn/simple"
 default = false
 secondary = true
```

### Comparing `nonebot_plugin_genshinuid-4.0.2/README.md` & `nonebot_plugin_genshinuid-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.2/PKG-INFO` & `nonebot_plugin_genshinuid-4.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshinuid
-Version: 4.0.2
+Version: 4.0.3
 Summary: 支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later
 Author: KimigaiiWuyi
 Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0)
 Requires-Dist: gitpython (>=3.1.27)
 Requires-Dist: msgspec (>=0.13.1)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0b4)
 Requires-Dist: pillow (>=9.2.0)
 Requires-Dist: websockets (>=11.0.1)
 Project-URL: Bug Tracker, https://github.com/KimigaiiWuyi/GenshinUID/issues
 Project-URL: Documentation, https://docs.gsuid.gbots.work/#/
 Project-URL: Repository, https://github.com/KimigaiiWuyi/GenshinUID
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.3 Summary:
 æ¯æOneBot
 (QQ)ãOneBotV12ãQQé¢éãå¾®ä¿¡ãKOOKï¼å¼é»å¦ï¼ãTelegramï¼çµæ¥ï¼ãFeiShuï¼é£ä¹¦ï¼çå¨åè½NoneBot2åç¥æä»¶
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later Author: KimigaiiWuyi Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: GNU
 General Public License v3 or later (GPLv3+) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0) Requires-Dist: gitpython
-(>=3.1.27) Requires-Dist: msgspec (>=0.13.1) Requires-Dist: nonebot2
-(>=2.0.0b4) Requires-Dist: pillow (>=9.2.0) Requires-Dist: websockets
-(>=11.0.1) Project-URL: Bug Tracker, https://github.com/KimigaiiWuyi/
-GenshinUID/issues Project-URL: Documentation, https://docs.gsuid.gbots.work/#/
-Project-URL: Repository, https://github.com/KimigaiiWuyi/GenshinUID
-Description-Content-Type: text/markdown
+(>=3.1.27) Requires-Dist: msgspec (>=0.13.1) Requires-Dist: nonebot-plugin-
+apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0b4) Requires-Dist:
+pillow (>=9.2.0) Requires-Dist: websockets (>=11.0.1) Project-URL: Bug Tracker,
+https://github.com/KimigaiiWuyi/GenshinUID/issues Project-URL: Documentation,
+https://docs.gsuid.gbots.work/#/ Project-URL: Repository, https://github.com/
+KimigaiiWuyi/GenshinUID Description-Content-Type: text/markdown
                                  [GenshinUID]
                          ****** GenshinUID 4.0 ******
                               *** â¨æ¯æOneBot
  (QQ)ãQQé¢éãå¾®ä¿¡ãå¼é»å¦ãTelegramçå¨åè½åç¥Botæä»¶â¨
                                       ***
              å®è£ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
              [https://s2.loli.net/2023/03/26/76oWuYJwg18aXL2.jpg]
```

