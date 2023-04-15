# Comparing `tmp/nonebot_plugin_sdgpt-0.2.2.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.2.2.tar` & `nonebot_plugin_sdgpt-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.2/LICENSE
--rw-r--r--   0        0        0     9307 2023-04-14 05:57:29.503439 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     5179 2023-04-14 03:33:23.558251 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     4058 2023-04-14 03:50:34.726392 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/config.py
--rw-r--r--   0        0        0     3670 2023-04-14 05:33:38.768842 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/configspec.ini
--rw-r--r--   0        0        0      196 2023-04-13 02:20:03.916559 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/base.py
--rw-r--r--   0        0        0     2987 2023-04-14 02:02:57.821153 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/check.py
--rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/cons.py
--rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/logger.py
--rw-r--r--   0        0        0     1717 2023-04-14 05:11:14.277310 nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/utils.py
--rw-r--r--   0        0        0     1160 2023-04-14 06:04:08.961530 nonebot_plugin_sdgpt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.2.2/README.md
--rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.3/LICENSE
+-rw-r--r--   0        0        0     9356 2023-04-15 06:17:15.183837 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     6337 2023-04-15 05:43:09.904354 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     6542 2023-04-15 05:42:39.006444 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/config.py
+-rw-r--r--   0        0        0     5386 2023-04-15 06:18:07.002772 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/configspec.ini
+-rw-r--r--   0        0        0      242 2023-04-15 04:34:57.487801 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/base.py
+-rw-r--r--   0        0        0     3028 2023-04-15 05:33:13.203719 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/check.py
+-rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/cons.py
+-rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/logger.py
+-rw-r--r--   0        0        0      125 2023-04-15 05:54:10.530836 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/test.py
+-rw-r--r--   0        0        0     2389 2023-04-15 05:07:08.376886 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/utils.py
+-rw-r--r--   0        0        0     1187 2023-04-15 06:27:43.052562 nonebot_plugin_sdgpt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1066 2023-04-15 04:38:37.455109 nonebot_plugin_sdgpt-0.2.3/README.md
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.2.2/LICENSE` & `nonebot_plugin_sdgpt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import time
 from io import BytesIO
 
 from nonebot import on_command, on_message
 from nonebot.adapters.onebot.v11 import Bot, MessageSegment
 from .bot import bot_start, msg_end, Chat
 from .lib.cons import *
-from .lib.utils import load_preset, rules, getThis
+from .lib.base import *
+from .lib.utils import load_preset, rules, getThis, asBot
 from webuiapi import webuiapi
 
 cfg = asyncio.run(bot_start())
 config = cfg['cfg']
-
-BotUse = config['Chat']['defaultAI']
+BotUse = cfg['BotUse']
 
 
 @event_postprocessor
 async def postprocessor():
     await msg_end()
 
 
@@ -27,118 +27,77 @@
 bing = on_command(config['Command']['bing'][1:], priority=1, block=True)
 switchAI = on_command(config['Command']['switchAI'][1:], priority=1, block=True)
 switch = on_command(config['Command']['switch'][1:], priority=1, block=True)
 switchPreset = on_command(config['Command']['switchPreset'][1:], priority=1, block=True)
 tag = on_command(config['Command']['tag'][1:], priority=1, block=True)
 SD_webui = on_command(config['Command']['SD_webui'][1:], priority=1, block=True)
 MSG = on_message(rule=to_me(), priority=2, block=True)
+poe = on_command(config['Command']['poe'][1:], priority=1, block=True)
+model = on_command(config['Command']['model'][1:], priority=1, block=True)
 
 
 @MSG.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent):
     if not rules('msg', config, event): return
-
-    def asChat():
-        global BotUse
-        if BotUse in cfg:
-            return BotUse
-        else:
-            if 'chatgpt-api' in cfg: return 'chatgpt-api'
-            if 'chatgpt' in cfg: return 'chatgpt'
-            if 'bing' in cfg: return 'bing'
-            error('/chat', '你没有任何chatgpt接入')
-            return False
-
     message = str(event.message)
-    BOT = asChat()
+    BOT = asBot(['chatgpt-api', 'chatgpt', 'bing'], BotUse, cfg)
     if len(message) == 0: return
     if BOT:
         info(BOT, '对话: ' + message)
         await Chat(event, foo, BOT, message)
 
 
 @chat.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
     if not rules('chat', config, event): return
-
-    def asChatGPT():
-        global BotUse
-        if 'chatgpt' in BotUse:
-            return BotUse
-        else:
-            if 'chatgpt-api' in cfg:
-                return 'chatgpt-api'
-            elif 'chatgpt' in cfg:
-                return 'chatgpt'
-            else:
-                error('/chat', '你没有任何chatgpt接入')
-        return False
-
     message = args.extract_plain_text()
     if len(message) == 0: return
-    BOT = asChatGPT()
+    BOT = asBot('asChat', BotUse, cfg)
     if BOT:
         info(BOT, '对话: ' + message)
         await Chat(event, foo, BOT, message)
 
 
 @bing.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
     if not rules('bing', config, event): return
-
-    def asBing():
-        if 'bing' not in cfg:
-            error('bing', '你没有接入bing')
-            return True
-        return 'bing'
-
-    if asBing():
+    BOT = asBot(['bing'], BotUse, cfg)
+    if BOT:
         message = args.extract_plain_text()
         if len(message) == 0: return
         info('bing', '对话: ' + message)
         await Chat(event, foo, 'bing', message)
 
 
+@poe.handle()
+async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
+    if not rules('poe', config, event): return
+    BOT = asBot(['poe'], BotUse, cfg)
+    if BOT:
+        message = args.extract_plain_text()
+        if len(message) == 0: return
+        info('poe', '对话: ' + message)
+        await Chat(event, foo, 'poe', message)
+
+
 @tag.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
     if not rules('tag', config, event): return
-    def asChat():
-        global BotUse
-        if BotUse in cfg:
-            return BotUse
-        else:
-            if 'chatgpt-api' in cfg: return 'chatgpt-api'
-            if 'chatgpt' in cfg: return 'chatgpt'
-            if 'bing' in cfg: return 'bing'
-            error('/chat', '你没有任何chatgpt接入')
-            return False
-
-    BOT = asChat()
+    BOT = asBot('*', BotUse, cfg)
     message = args.extract_plain_text()
     if len(message) == 0: return
     if BOT:
         info(BOT, '对话: ' + message)
         await Chat(event, foo, BOT, message, noStream=True, p='tag')
 
 
 @SD_webui.handle()
 async def _(foo: Bot, event: GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent, args: Message = CommandArg()):
     if not rules('SD_webui', config, event): return
-    def asChat():
-        global BotUse
-        if BotUse in cfg:
-            return BotUse
-        else:
-            if 'chatgpt-api' in cfg: return 'chatgpt-api'
-            if 'chatgpt' in cfg: return 'chatgpt'
-            if 'bing' in cfg: return 'bing'
-            error('/chat', '你没有任何chatgpt接入')
-            return False
-
-    BOT = asChat()
+    BOT = asBot('*', BotUse, cfg)
     message = args.extract_plain_text()
     if len(message) == 0: return
     if BOT:
         info(BOT, '对话: ' + message)
         prompt = await Chat(event, foo, BOT, message, p='tag', noOut=True)
         sd = config['Stable-Diffusion']
         ip = sd['api_host']
@@ -187,16 +146,16 @@
 
 @switch.handle()
 async def _(event: Event, args: Message = CommandArg()):
     global config
     if not rules('switch', config, event): return
     args = args.extract_plain_text().split(' ')
     if len(args) == 0: return
-    if args[0] == '群聊': args = ['Function','Group','groups',args[-1]]
-    if args[0] == '私聊': args = ['Function','Private','member',args[-1]]
+    if args[0] == '群聊': args = ['Function', 'Group', 'groups', args[-1]]
+    if args[0] == '私聊': args = ['Function', 'Private', 'member', args[-1]]
     if args[0] == '频道': args = ['Function', 'Guild', 'guilds', args[-1]]
     path = args[:-2]
     isOwner = (config['Bot']['owner'] == event.get_user_id())
     if config['Bot']['switchConfigEval'] is False and not isOwner:
         return warn('/switch', '无权限更改')
     if args[0] == 'Bot' and not isOwner:
         return warn('/switch', '无权限更改 Bot')
@@ -224,15 +183,15 @@
         data = now[args[-2]]
     else:
         data = args[-1]
     if not isinstance(now[args[-2]], (int, float, str, bool, list)):
         rep = {"'(access_token)': '[^’]*'": r"[$1]",
                "'(api_key)': '[^']*'": r"[$2]",
                "'(api_host)': '[^']*'": r"[$3]",
-        }
+               }
         result = re.sub("|".join(rep.keys()), '[隐藏]', str(now[args[-2]]))
         return await switch.send(result)
     now[args[-2]] = data
     config.write()
     print(config['Chat'])
     await switch.send('.'.join(args[:-1]) + '已改为' + str(data))
 
@@ -254,7 +213,36 @@
         config.write()
     elif args in ['None', 'none', '0', 'false', 'False', 'default']:
         config['runtime']['preset'] = ''
         config.write()
     else:
         await switchPreset.send('预设不存在，请在配置中注册')
         return error('/switchPreset', '预设不存在，请在配置中注册')
+
+
+@model.handle()
+async def _(event: Event, args: Message = CommandArg()):
+    global config
+    if not rules('switchPreset', config, event): return
+    args = args.extract_plain_text()
+    if len(args) == 0: return
+    args = args.split(' ')
+    if len(args) == 1:
+        bot_ = BotUse
+        arg = args[0]
+    elif len(args) == 2:
+        bot_ = args[0]
+        arg = args[1]
+    else:
+        return
+    modelDIR = {i.split(':')[1]: i.split(':')[0] for i in config['AI'][bot_]['models']}
+    modelLIST = list(modelDIR.values())
+    if arg in modelDIR:
+        model_ = modelDIR[arg]
+    elif arg in modelLIST:
+        model_ = arg
+    else:
+        warn('/model', '模型不存在')
+        return await model.send('模型不存在')
+    config['runtime'][bot_.replace('-', '_') + '_model'] = model_
+    config.write()
+    return await model.send(f'{bot_} 的模型更改为 {model_}')
```

### Comparing `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 import asyncio
-import os
 import re
 import time
 
-from celery import Celery
-
 from .lib.cons import *
 from .lib.base import *
-from .lib.utils import load_preset
+from .lib.utils import load_preset, switchModel
 from .config import load as cfg_load
-from nonebot.adapters.onebot.v11.adapter import Message
 
 global dotenv_file
 global chatgpt
 global chatgpt_api
 global bing
 global config
-global defaultAI
+global L_chatgpt
+global L_chatgpt_api
+global L_bing
+global L_poe
+global poe
 
 
 async def bot_start():
     global L_chatgpt
     global L_chatgpt_api
     global L_bing
+    global L_poe
     global chatgpt
     global chatgpt_api
     global bing
+    global poe
     global config
-    global defaultAI
     cfg = await cfg_load()
     if 'chatgpt' in cfg: chatgpt = cfg['chatgpt']
     if 'chatgpt-api' in cfg: chatgpt_api = cfg['chatgpt-api']
     if 'bing' in cfg: bing = cfg['bing']
+    if 'poe' in cfg: poe = cfg['poe']
+
     config = cfg['cfg']
     if config['Chat']['reload_presets']:
         config['runtime']['preset'] = ''
         config.write()
-    defaultAI = config['Chat']['defaultAI']
 
     L_chatgpt = asyncio.Lock()
-    #L_chatgpt_api = asyncio.Lock()
+    # L_chatgpt_api = asyncio.Lock()
     L_bing = asyncio.Lock()
+    L_poe = asyncio.Lock()
 
     return cfg
 
 
 async def msg_end():
     return
 
@@ -76,32 +79,43 @@
         if noStream:
             out = re.sub(r".*\.AIP", "", out)
         if noOut:
             return out
         await foo.send(event, out, reply_message=reply)
 
 
-async def ask(bot, message, prompt=''):
+async def ask(bot, message, prompt='', model=''):
     if bot == 'chatgpt':
+        model = config['AI'][bot]['']
         async with L_chatgpt:
             if len(prompt) > 1: message = promptBase.replace("$prompt$", prompt) + message
             info('ASK', message)
+            if config['runtime']['chatgpt_model'] and config['runtime']['chatgpt_model'] != '':
+                switchModel(chatgpt, 'chatgpt', config['runtime']['chatgpt_model'])
             async for data in chatgpt.ask(message):
                 out = data['message']
             return out
     if bot == 'chatgpt-api':
         chatgpt_api.system_prompt = prompt
+        switchModel(chatgpt, 'chatgpt-api', config['runtime']['chatgpt_api_model'])
         out = await chatgpt_api.ask_async(message)
         return out
     if bot == 'bing':
         async with L_bing:
             if len(prompt) > 1: message = promptBase + message
-            out = await bing.ask(message)
+            out = await bing.ask(message, conversation_style=config['runtime']['bing_model'])
             out = out['item']['messages'][-1]['text']
             return out
+    if bot == 'poe':
+        async with L_poe:
+            if len(prompt) > 1: message = promptBase + message
+            for chunk in poe.send_message(config['runtime']['poe_models'][config['runtime']['poe_model']], message):
+                pass
+            out = chunk["text"]
+            return out
 
 
 async def ask_stream(event, func, bot, message, prompt=''):
     text = ''
     timeNow = time.time()
     wait_time = config['Chat']['stream_wait_time']
     end_str = tuple(config['Chat']['stream_endStr'])
@@ -151,7 +165,15 @@
             async for data in bing.ask_stream(message):
                 isTrue, textdata = data
                 if type(textdata) == str:
                     text = textdata
                     await stream_process('Bing')
                 else:
                     await stream_process('bing', text)
+    if bot == 'poe':
+        async with L_poe:
+            if len(prompt) > 1: message = promptBase + message
+            for chunk in poe.send_message(config['runtime']['poe_models'][config['runtime']['poe_model']], message):
+                text += chunk["text_new"]
+                isEnd = await stream_process('poe')
+                if isEnd and len(text.replace(before, '').replace(' ', '')) > 1:
+                    await stream_process('poe', text)
```

### Comparing `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/check.py` & `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,25 +110,27 @@
 def check_token(value):
     if len(value) > 20: return value
     if value == '':
         return value
     es(value, 'access_token不合法')
     raise ValueError
 
+def check_poetoken(value):
+    return value
 
 def ip_test_switch(value):
     global switch
     if value == 'True':
         switch = True
     else:
         switch = False
     return value
 
 
-def check_model(value: str):
+def check_model(value):
     return value
 
 
 def check_id(value):
     return value
 
 def check_any(value):
```

### Comparing `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/logger.py` & `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/logger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.2/nonebot_plugin_SDGPT/lib/utils.py` & `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import aiofiles
 from .logger import err
 from .cons import *
+from .base import *
 
 
 async def load_preset(dir, filename):
     try:
         async with aiofiles.open(dir + "/" + filename, mode="r", encoding='utf-8') as f:
             text = await f.read()
         return text
@@ -29,14 +30,37 @@
         if cmdName not in private['function'] and ('*' not in private['function']): return
     if isinstance(event, GuildMessageEvent):
         if not guild['switch']: return
         if event.guild_id not in guild['guilds'] and ('*' not in guild['guilds']): return
         if cmdName not in guild['function'] and ('*' not in guild['function']): return
     return True
 
+
 def getThis(event):
     if isinstance(event, GroupMessageEvent):
         return event.group_id
     if isinstance(event, PrivateMessageEvent):
         return event.user_id
     if isinstance(event, GuildMessageEvent):
-        return event.guild_id
+        return event.guild_id
+
+
+def asBot(botList, botUse, cfg):
+    if botUse != 'None': return botUse
+    if botList == '*': botList = AI_list
+    if botList == 'chat': botList = asChat
+    for bot in botList:
+        if bot in cfg:
+            return bot
+    err('无可用ai', '此功能可用ai列表中无已加载的ai' + ', '.join(botList))
+    return False
+
+
+def switchModel(bot, botName, model):
+    if botName == 'chatgpt':
+        bot.config['model'] = model
+    if botName == 'chatgpt-api':
+        bot.engine = model
+    if botName == 'bing':
+        error('switchModel', 'bing')
+    if botName == 'poe':
+        error('switchModel', 'poe')
```

### Comparing `nonebot_plugin_sdgpt-0.2.2/pyproject.toml` & `nonebot_plugin_sdgpt-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.2.2"
-description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像"
+version = "0.2.3"
+description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
 keywords = ["nonebot", "nonebot2", "chatgpt", "new bing","Stable-Diffusion"]
@@ -24,14 +24,16 @@
 EdgeGPT = "*"
 webuiapi = "*"
 nonebot-plugin-guild-patch ="*"
 nonebot-adapter-onebot = { version = "^2.0.0-beta.1", optional = true }
 websockets = "^10.0"
 aiofiles = "*"
 configobj = "*"
+poe-api = "*"
+
 
 [tool.poetry.extras]
 onebot = ["nonebot-adapter-onebot"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_sdgpt-0.2.2/README.md` & `nonebot_plugin_sdgpt-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SDGPT 
 基于 **[NoneBot2](https://v2.nonebot.dev/)** 
   
  
-## 功能
+## 功能[pyproject.toml](pyproject.toml)
 链接 ChatGPT / Bing / Stable-Diffusion  :   
 - [x] ChatGPT对话 
 - [x] Bing对话
 - [x] Stable-Diffusion 文生图  
   > 基于 chatGPT 或 bing 解析自然语言转 Stable-Diffusion 生成图像
 - [x] qq 频道支持 
   > qq 频道下 chatGPT bing 的对话会分段发送
```

### Comparing `nonebot_plugin_sdgpt-0.2.2/PKG-INFO` & `nonebot_plugin_sdgpt-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.2.2
-Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像
+Version: 0.2.3
+Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,27 +17,28 @@
 Provides-Extra: onebot
 Requires-Dist: EdgeGPT
 Requires-Dist: aiofiles
 Requires-Dist: configobj
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0) ; extra == "onebot"
 Requires-Dist: nonebot-plugin-guild-patch
 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: poe-api
 Requires-Dist: python-dotenv
 Requires-Dist: revChatGPT
 Requires-Dist: websockets (>=10.0,<11.0)
 Requires-Dist: webuiapi
 Project-URL: Documentation, https://github.com/thx114/SDGPTreadme
 Project-URL: Repository, https://github.com/thx114/SDGPT
 Description-Content-Type: text/markdown
 
 # SDGPT 
 基于 **[NoneBot2](https://v2.nonebot.dev/)** 
   
  
-## 功能
+## 功能[pyproject.toml](pyproject.toml)
 链接 ChatGPT / Bing / Stable-Diffusion  :   
 - [x] ChatGPT对话 
 - [x] Bing对话
 - [x] Stable-Diffusion 文生图  
   > 基于 chatGPT 或 bing 解析自然语言转 Stable-Diffusion 生成图像
 - [x] qq 频道支持 
   > qq 频道下 chatGPT bing 的对话会分段发送
```

