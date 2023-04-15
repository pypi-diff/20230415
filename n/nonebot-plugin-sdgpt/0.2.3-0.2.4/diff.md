# Comparing `tmp/nonebot_plugin_sdgpt-0.2.3.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.2.4.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.2.3.tar` & `nonebot_plugin_sdgpt-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.3/LICENSE
--rw-r--r--   0        0        0     9356 2023-04-15 06:17:15.183837 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     6337 2023-04-15 05:43:09.904354 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     6542 2023-04-15 05:42:39.006444 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/config.py
--rw-r--r--   0        0        0     5386 2023-04-15 06:18:07.002772 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/configspec.ini
--rw-r--r--   0        0        0      242 2023-04-15 04:34:57.487801 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/base.py
--rw-r--r--   0        0        0     3028 2023-04-15 05:33:13.203719 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/check.py
--rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/cons.py
--rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/logger.py
--rw-r--r--   0        0        0      125 2023-04-15 05:54:10.530836 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/test.py
--rw-r--r--   0        0        0     2389 2023-04-15 05:07:08.376886 nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/utils.py
--rw-r--r--   0        0        0     1187 2023-04-15 06:27:43.052562 nonebot_plugin_sdgpt-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1066 2023-04-15 04:38:37.455109 nonebot_plugin_sdgpt-0.2.3/README.md
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.2.4/LICENSE
+-rw-r--r--   0        0        0     9353 2023-04-15 11:12:41.293116 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     6288 2023-04-15 11:16:16.354928 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     6542 2023-04-15 05:42:39.006444 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/config.py
+-rw-r--r--   0        0        0     5386 2023-04-15 06:18:07.002772 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/configspec.ini
+-rw-r--r--   0        0        0      242 2023-04-15 04:34:57.487801 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/base.py
+-rw-r--r--   0        0        0     3028 2023-04-15 05:33:13.203719 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/check.py
+-rw-r--r--   0        0        0      487 2023-04-13 00:23:27.760154 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/cons.py
+-rw-r--r--   0        0        0     2003 2023-04-11 23:52:10.103729 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/logger.py
+-rw-r--r--   0        0        0      125 2023-04-15 05:54:10.530836 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/test.py
+-rw-r--r--   0        0        0     2389 2023-04-15 05:07:08.376886 nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/utils.py
+-rw-r--r--   0        0        0     1187 2023-04-15 11:17:26.147629 nonebot_plugin_sdgpt-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1066 2023-04-15 04:38:37.455109 nonebot_plugin_sdgpt-0.2.4/README.md
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.2.4/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.2.3/LICENSE` & `nonebot_plugin_sdgpt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
 
 @switchAI.handle()
 async def _(foo: Bot, event: Event, args: Message = CommandArg()):
     if not rules('switchAI', config, event): return
     use = args.extract_plain_text()
     if len(args) == 0: return
-    if use in config:
+    if use in cfg:
         global BotUse
         BotUse = use
         await switchAI.send('已切换到 ' + BotUse)
         suc('切换AI', BotUse)
     else:
         await switchAI.send('AI不存在')
         warn("切换AI", f'AI不存在 , {use} is not in: {cfg}')
```

### Comparing `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,16 @@
         if noStream:
             out = re.sub(r".*\.AIP", "", out)
         if noOut:
             return out
         await foo.send(event, out, reply_message=reply)
 
 
-async def ask(bot, message, prompt='', model=''):
+async def ask(bot, message, prompt=''):
     if bot == 'chatgpt':
-        model = config['AI'][bot]['']
         async with L_chatgpt:
             if len(prompt) > 1: message = promptBase.replace("$prompt$", prompt) + message
             info('ASK', message)
             if config['runtime']['chatgpt_model'] and config['runtime']['chatgpt_model'] != '':
                 switchModel(chatgpt, 'chatgpt', config['runtime']['chatgpt_model'])
             async for data in chatgpt.ask(message):
                 out = data['message']
```

### Comparing `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/config.py` & `nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/configspec.ini` & `nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/configspec.ini`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/check.py` & `nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/logger.py` & `nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/logger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.3/nonebot_plugin_SDGPT/lib/utils.py` & `nonebot_plugin_sdgpt-0.2.4/nonebot_plugin_SDGPT/lib/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.3/pyproject.toml` & `nonebot_plugin_sdgpt-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.2.3"
+version = "0.2.4"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
```

### Comparing `nonebot_plugin_sdgpt-0.2.3/README.md` & `nonebot_plugin_sdgpt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.2.3/PKG-INFO` & `nonebot_plugin_sdgpt-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.2.3
+Version: 0.2.4
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Poe / Stable-Diffusion : ChatGPT Bing poe聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
```

