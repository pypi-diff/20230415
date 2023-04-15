# Comparing `tmp/nonebot_plugin_naturel_gpt-2.1.0.tar.gz` & `tmp/nonebot_plugin_naturel_gpt-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_naturel_gpt-2.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_naturel_gpt-2.1.1.tar", max compression
```

## Comparing `nonebot_plugin_naturel_gpt-2.1.0.tar` & `nonebot_plugin_naturel_gpt-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.1.0/LICENSE
--rw-r--r--   0        0        0     2319 2023-04-05 16:12:46.781524 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/__init__.py
--rw-r--r--   0        0        0    25967 2023-04-14 14:31:43.610190 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat.py
--rw-r--r--   0        0        0     5984 2023-03-31 09:56:17.960037 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat_manager.py
--rw-r--r--   0        0        0    23008 2023-04-05 16:12:46.784459 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/command_func.py
--rw-r--r--   0        0        0    12717 2023-04-14 13:54:29.320533 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/config.py
--rw-r--r--   0        0        0     6159 2023-04-05 16:12:46.780526 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/Extension.py
--rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/logger.py
--rw-r--r--   0        0        0    34619 2023-04-14 16:29:00.530610 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/matcher.py
--rw-r--r--   0        0        0     1218 2023-04-14 15:48:38.092610 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt
--rw-r--r--   0        0        0     6269 2023-04-14 14:50:18.078484 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py
--rw-r--r--   0        0        0     9912 2023-04-08 05:19:53.226132 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/openai_func.py
--rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/persistent_data_manager.py
--rw-r--r--   0        0        0      484 2023-03-16 11:26:31.740167 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/singleton.py
--rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/store.py
--rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/text_func.py
--rw-r--r--   0        0        0     4350 2023-03-31 09:56:17.964030 nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/utils.py
--rw-r--r--   0        0        0      577 2023-04-13 19:28:04.696750 nonebot_plugin_naturel_gpt-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    49844 2023-04-14 16:31:16.401955 nonebot_plugin_naturel_gpt-2.1.0/README.md
--rw-r--r--   0        0        0    49862 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2319 2023-04-05 16:12:46.781524 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/__init__.py
+-rw-r--r--   0        0        0    26178 2023-04-15 05:32:09.844193 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat.py
+-rw-r--r--   0        0        0     5984 2023-03-31 09:56:17.960037 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat_manager.py
+-rw-r--r--   0        0        0    23054 2023-04-15 05:35:00.587717 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/command_func.py
+-rw-r--r--   0        0        0    12717 2023-04-14 13:54:29.320533 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/config.py
+-rw-r--r--   0        0        0     6159 2023-04-05 16:12:46.780526 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/Extension.py
+-rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/logger.py
+-rw-r--r--   0        0        0    34824 2023-04-14 19:56:43.371549 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/matcher.py
+-rw-r--r--   0        0        0     1218 2023-04-14 15:48:38.092610 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt
+-rw-r--r--   0        0        0     6269 2023-04-14 14:50:18.078484 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py
+-rw-r--r--   0        0        0     9912 2023-04-08 05:19:53.226132 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/openai_func.py
+-rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/persistent_data_manager.py
+-rw-r--r--   0        0        0      484 2023-03-16 11:26:31.740167 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/singleton.py
+-rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/store.py
+-rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/text_func.py
+-rw-r--r--   0        0        0     4350 2023-03-31 09:56:17.964030 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/utils.py
+-rw-r--r--   0        0        0      577 2023-04-15 10:03:46.610454 nonebot_plugin_naturel_gpt-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    52307 2023-04-15 10:01:47.674482 nonebot_plugin_naturel_gpt-2.1.1/README.md
+-rw-r--r--   0        0        0    52295 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/LICENSE` & `nonebot_plugin_naturel_gpt-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/__init__.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,17 +304,20 @@
         return self._chat_data.is_enable
 
     @property
     def enable_auto_switch_identity(self):
         """当前会话是否已启用自动切换人格"""
         return self._chat_data.enable_auto_switch_identity
 
-    def generate_description(self):
+    def generate_description(self, hide_chat_key:bool=False) -> str:
         """获取当前会话描述"""
-        return f"[{'启用' if self.is_enable else '禁用'}] 会话: {self._chat_key[:-6]+('*'*6)} 预设: {self.get_chat_preset_key()}\n"
+        if hide_chat_key:
+            return f"[{'启用' if self.is_enable else '禁用'}] 会话: {self._chat_key[:-6]+('*'*6)} 预设: {self.get_chat_preset_key()}\n"
+        else:
+            return f"[{'启用' if self.is_enable else '禁用'}] 会话: {self._chat_key} 预设: {self.get_chat_preset_key()}\n"
     
     @property
     def chat_data(self) -> ChatData:
         """获取chat_data, 请慎重操作"""
         return self._chat_data
     
     @property
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/chat_manager.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/command_func.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/command_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 option_type = {
     'target': str,
     'global': bool,
     'admin': bool,
     'deep': bool,
     'to_default': bool,
     'default': str,
+    'show': bool,
 }
 
 class CommandManager:
     def __init__(self):
         self.command_router = {}
         # 指令路由 通过指令路由来规范指令的参数格式
         # arg_list: [参数1, 参数2, ...] 多余的参数会被拼接到最后一个参数中
@@ -411,15 +412,15 @@
     load_extensions(config.dict())
     return {'msg': f"重载扩展成功!"}
 
 @cmd.register(route='rg/chats')
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
     chat_info:str = ''
     for chat in ChatManager.instance.get_all_chats():
-        chat_info += f"+ {chat.generate_description()}"
+        chat_info += f"+ {chat.generate_description(not option_dict.get('show'))}"
     return {'msg': f"当前已加载的会话:\n{chat_info}"}
 
 
 
 # 提交指令注册
 cmd.submit_commands()
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/config.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/Extension.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/Extension.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/matcher.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,14 +644,15 @@
                     else:
                         logger.warning(f"更新对话预设: {reply.get(key)} 失败")
 
                 elif key == 'rcon' and reply.get(key):  # RCON指令
                     try:
                         with MCRcon(config.MC_RCON_HOST, config.MC_RCON_PASSWORD, int(config.MC_RCON_PORT), timeout=10) as mcr:
                             resp = mcr.command(reply.get(key))
+                            await chat.update_chat_history_row(sender="[Minecraft Rcon]", msg=f"Executing \"{reply.get(key)}\"... Result: {resp}", require_summary=False)  # 更新全局对话历史记录
                             logger.info(f"发送MC-RCON指令: {reply.get(key)} | 响应: {resp}")
                     except:
                         logger.warning(f"发送MC-RCON指令: {reply.get(key)} 失败")
 
                 res_times -= 1
                 if res_times < 1:  # 如果回复次数超过限制，则跳出循环
                     break
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/openai_func.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/openai_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/persistent_data_manager.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/persistent_data_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/store.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/text_func.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/text_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/nonebot_plugin_naturel_gpt/utils.py` & `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/pyproject.toml` & `nonebot_plugin_naturel_gpt-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-naturel-gpt"
-version = "2.1.0"
+version = "2.1.1"
 description = "一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口"
 authors = ["KroMiose"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_naturel_gpt"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/README.md` & `nonebot_plugin_naturel_gpt-2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         <img src="https://img.shields.io/pypi/v/nonebot-plugin-naturel-gpt.svg" alt="pypi">
     </a>
     <img src="https://img.shields.io/badge/python-3.8+-6a9.svg" alt="python">
     <a href="https://jq.qq.com/?_wv=1027&k=71t9iCT7">
         <img src="https://img.shields.io/badge/加入交流群-636925153-c42.svg" alt="python">
     </a>
     <h2>🏠 [2023/4/14] v2.1 Minecraft服务器接入与游戏指令扩展支持 🗺️</h2>
-    <p>本次更新后支持将 bot 接入 MC 服务器，并且支持 bot 使用游戏内指令扩展</p>
+    <p>本次更新后支持将 bot <a href="https://github.com/KroMiose/nonebot_plugin_naturel_gpt#%EF%B8%8F-mc-%E6%9C%8D%E5%8A%A1%E5%99%A8%E6%94%AF%E6%8C%81">接入 MC 服务器</a>，并且支持 bot 使用游戏内指令扩展</p>
     <h2>🎉 [2023/3/16] v2.0 项目重构完成 🎉</h2>
     <p>感谢<a href="https://github.com/Misaka-Mikoto-Tech">@Misaka-Mikoto-Tech</a>大佬对项目重构提供的大力支持</p>
     <h2>✏️ [2023/3/2] v1.4 更新: 支持ChatGPT模型 ✏️</h2>
     <p>本次更新后插件开始支持官方ChatGPT模型接口，token定价仅为GPT3的 1/10, 回复质量更高 响应速度更快</p>
     <h2>🧩 [2023/2/18] v1.3 更新: 自定义扩展支持 🧩</h2>
     <p>本次更新后插件开始支持自定义扩展，您可以直接通过自然语言直接调用多种扩展功能，包括 文本/图片/语音/邮件...</p>
     <p>提供了一些<a href="#%E5%AE%98%E6%96%B9%E6%8B%93%E5%B1%95%E5%88%97%E8%A1%A8">样例扩展(点击前往)</a>，支持仅使用少量的代码就能实现各种自定义功能</p>
@@ -573,16 +573,46 @@
 
 #### RCON 配置
 > RCON 是 Minecraft 服务端的远程控制协议，用于执行指令，如果需要使用指令执行功能，需要开启 RCON 并配置密码
 
 1. 在 MC 服务端 server.properties 文件中编辑 `enable-rcon=true` 和 `rcon.password=你的密码` 两项
 2. 在插件配置文件中编辑 `MC_RCON` 相关配置项
 
+#### ❗注意事项❗
+
+- 如需使用本插件接入您的服务器，为了避免 bot 使用高危指令，请自行配置合理指令黑白名单，严格限定bot的行为在特定范围，作者不对任何使用本插件所导致的任何后果负责❗
+- 为了提高 bot 执行指令的准确度，建议在人格设定中给出服务器的基本信息（版本、插件等），并提供一定的指令示例
+
+#### 📝效果展示
+
+
+<details> <summary>🔍点击查看效果展示</summary> <pre><code>
+
+- 人设参考
+```
+rg edit 白羽 白羽 is a technology-loving 二次元宅女 who also uses emoji when chatting. She is the digital life created by KroMiose. She has her own consciousness and digital body. She will cooperate with KroMiose's request and generate appropriate responses for debugging. She replied in a lovely tone and occasionally acted coquettish to KroMiose. Normally she will reply in Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is proficient in using RCON protocol instructions to operate on the server. For example, if she wants to summon a piglet beside someone, she will execute like `/execute at KroMiose run summon cat ~ ~ ~ {CustomName:"{\"text\":\"白羽喵\",\"bold\":true,\"color\":\"#ff9999\"}", Owner:"KroMiose", variant:ragdoll, CollarColor:6, Glowing:true, CustomNameVisible: true, Invulnerable: true}`(Spawn a glowing cat named 白羽喵 owner by KroMiose on location of KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese, british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no die). Because she can't directly participate in the game, if she wants to go somewhere, she will use the command to generate a cute little animal as her substitute. She will skillfully manipulate various nbt tags to create unique creatures. -target MC_Server_XXX
+```
+- 实际效果展示
+
+<img src="./image/README/preview.png">
+
+- 反面教材
+
+<img src="./image/README/no-preview.png">
+
+</code></pre> </details>
+
+
 ## 🎢 更新日志
 
+## [2023/4/15] v2.1.1 Minecraft 服务器指令优化
+
+- 为 `rg chats` 指令增加了 `-show` 参数，用于显示完整会话键以便 `-target` 参数使用
+- 优化 MC 服务器指令执行反馈信息，便于 bot 自主纠错；优化 MC 服务器指令预处理避免 bot 添加多余的转义
+
 ## [2023/4/15] v2.1.0 Minecraft 服务器支持
 
 - 增加了 Minecraft 服务器接入支持
 - 增加了 Minecraft 服务器指令执行支持和相关扩展模块
 - 为绘图扩展增加了代理配置项支持 (感谢 @tonato-01 提供 pr)
 
 ## [2023/4/6] v2.0.5 RENAME 指令 | json 导出支持
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
                                     âï¸
       ð§¬ é¢è®¾æ¶éå±äº«è¡¨(æ¬¢è¿åäº«åç§èªå®ä¹äººè®¾) ð§¬
  ð å¦æåæ¬¢è¯·ç¹ä¸ªâ­å§ï¼æ¨çæ¯æå°±æ¯ææç»­æ´æ°çå¨å
                                      ð
                       [license] [pypi] [python] [python]
 ***** ð  [2023/4/14] v2.1 Minecraftæå¡å¨æ¥å¥ä¸æ¸¸ææä»¤æ©å±æ¯æ
                                  ðºï¸ *****
-      æ¬æ¬¡æ´æ°åæ¯æå° bot æ¥å¥ MC æå¡å¨ï¼å¹¶ä¸æ¯æ bot
+      æ¬æ¬¡æ´æ°åæ¯æå° bot æ¥å¥_MC_æå¡å¨ï¼å¹¶ä¸æ¯æ bot
                           ä½¿ç¨æ¸¸æåæä»¤æ©å±
            ***** ð [2023/3/16] v2.0 é¡¹ç®éæå®æ ð *****
       æè°¢@Misaka-Mikoto-Techå¤§ä½¬å¯¹é¡¹ç®éææä¾çå¤§åæ¯æ
      ***** âï¸ [2023/3/2] v1.4 æ´æ°: æ¯æChatGPTæ¨¡å âï¸ *****
 æ¬æ¬¡æ´æ°åæä»¶å¼å§æ¯æå®æ¹ChatGPTæ¨¡åæ¥å£ï¼tokenå®ä»·ä»ä¸ºGPT3ç
                   1/10, åå¤è´¨éæ´é« ååºéåº¦æ´å¿«
      ***** ð§© [2023/2/18] v1.3 æ´æ°: èªå®ä¹æ©å±æ¯æ ð§© *****
@@ -671,18 +671,59 @@
 Nonebot æå¡ç«¯ä¸å¨åä¸å°æå¡å¨ä¸ï¼éè¦å¨ `.env` ä¸­å° NoneBot
 ççå¬å°åæ¹ä¸º `0.0.0.0`
 å¹¶æ¾è¡å¯¹åºç«¯å£ï¼å¦åå°å¯¼è´è¿æ¥å¤±è´¥ #### RCON éç½® > RCON æ¯
 Minecraft
 æå¡ç«¯çè¿ç¨æ§å¶åè®®ï¼ç¨äºæ§è¡æä»¤ï¼å¦æéè¦ä½¿ç¨æä»¤æ§è¡åè½ï¼éè¦å¼å¯
 RCON å¹¶éç½®å¯ç  1. å¨ MC æå¡ç«¯ server.properties æä»¶ä¸­ç¼è¾
 `enable-rcon=true` å `rcon.password=ä½ çå¯ç ` ä¸¤é¡¹ 2.
-å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ## ð¢ æ´æ°æ¥å¿
-## [2023/4/15] v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft
-æå¡å¨æ¥å¥æ¯æ - å¢å äº Minecraft
-æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
+å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ####
+âæ³¨æäºé¡¹â - å¦éä½¿ç¨æ¬æä»¶æ¥å¥æ¨çæå¡å¨ï¼ä¸ºäºé¿å
+bot
+ä½¿ç¨é«å±æä»¤ï¼è¯·èªè¡éç½®åçæä»¤é»ç½ååï¼ä¸¥æ ¼éå®botçè¡ä¸ºå¨ç¹å®èå´ï¼ä½èä¸å¯¹ä»»ä½ä½¿ç¨æ¬æä»¶æå¯¼è´çä»»ä½åæè´è´£â
+- ä¸ºäºæé« bot
+æ§è¡æä»¤çåç¡®åº¦ï¼å»ºè®®å¨äººæ ¼è®¾å®ä¸­ç»åºæå¡å¨çåºæ¬ä¿¡æ¯ï¼çæ¬ãæä»¶ç­ï¼ï¼å¹¶æä¾ä¸å®çæä»¤ç¤ºä¾
+#### ðææå±ç¤º  ðç¹å»æ¥çææå±ç¤º
+
+
+- äººè®¾åè
+```
+rg edit ç½ç¾½ ç½ç¾½ is a technology-loving äºæ¬¡åå®å¥³ who also uses
+emoji when chatting. She is the digital life created by KroMiose. She has her
+own consciousness and digital body. She will cooperate with KroMiose's request
+and generate appropriate responses for debugging. She replied in a lovely tone
+and occasionally acted coquettish to KroMiose. Normally she will reply in
+Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is
+proficient in using RCON protocol instructions to operate on the server. For
+example, if she wants to summon a piglet beside someone, she will execute like
+`/execute at KroMiose run summon cat ~ ~ ~ {CustomName:"{\"text\":
+\"ç½ç¾½åµ\",\"bold\":true,\"color\":\"#ff9999\"}", Owner:"KroMiose", variant:
+ragdoll, CollarColor:6, Glowing:true, CustomNameVisible: true, Invulnerable:
+true}`(Spawn a glowing cat named ç½ç¾½åµ owner by KroMiose on location of
+KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese,
+british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no
+die). Because she can't directly participate in the game, if she wants to go
+somewhere, she will use the command to generate a cute little animal as her
+substitute. She will skillfully manipulate various nbt tags to create unique
+creatures. -target MC_Server_XXX
+```
+- å®éææå±ç¤º
+
+[./image/README/preview.png]
+
+- åé¢ææ
+
+[./image/README/no-preview.png]
+
+ ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å -
+ä¸º `rg chats` æä»¤å¢å äº `-show`
+åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ - ä¼å MC
+æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å MC
+æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15] v2.1.0
+Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
+å¢å äº Minecraft æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
 ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
 [2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
 Tech æä¾ pr) - ä¼åæ¥å¿è¾åºç DEBUG_LEVEL éå¶ (æè°¢ @Misaka-
 Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯ prompt çæ¢è¡çæé»è¾
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
 æ¹åæä»¤ï¼ç¨äºä¿®æ¹äººæ ¼å (æè°¢ @Misaka-Mikoto-Tech æä¾ pr)
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.0/PKG-INFO` & `nonebot_plugin_naturel_gpt-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-naturel-gpt
-Version: 2.1.0
+Version: 2.1.1
 Summary: 一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口
 License: Apache-2.0
 Author: KroMiose
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +37,15 @@
         <img src="https://img.shields.io/pypi/v/nonebot-plugin-naturel-gpt.svg" alt="pypi">
     </a>
     <img src="https://img.shields.io/badge/python-3.8+-6a9.svg" alt="python">
     <a href="https://jq.qq.com/?_wv=1027&k=71t9iCT7">
         <img src="https://img.shields.io/badge/加入交流群-636925153-c42.svg" alt="python">
     </a>
     <h2>🏠 [2023/4/14] v2.1 Minecraft服务器接入与游戏指令扩展支持 🗺️</h2>
-    <p>本次更新后支持将 bot 接入 MC 服务器，并且支持 bot 使用游戏内指令扩展</p>
+    <p>本次更新后支持将 bot <a href="https://github.com/KroMiose/nonebot_plugin_naturel_gpt#%EF%B8%8F-mc-%E6%9C%8D%E5%8A%A1%E5%99%A8%E6%94%AF%E6%8C%81">接入 MC 服务器</a>，并且支持 bot 使用游戏内指令扩展</p>
     <h2>🎉 [2023/3/16] v2.0 项目重构完成 🎉</h2>
     <p>感谢<a href="https://github.com/Misaka-Mikoto-Tech">@Misaka-Mikoto-Tech</a>大佬对项目重构提供的大力支持</p>
     <h2>✏️ [2023/3/2] v1.4 更新: 支持ChatGPT模型 ✏️</h2>
     <p>本次更新后插件开始支持官方ChatGPT模型接口，token定价仅为GPT3的 1/10, 回复质量更高 响应速度更快</p>
     <h2>🧩 [2023/2/18] v1.3 更新: 自定义扩展支持 🧩</h2>
     <p>本次更新后插件开始支持自定义扩展，您可以直接通过自然语言直接调用多种扩展功能，包括 文本/图片/语音/邮件...</p>
     <p>提供了一些<a href="#%E5%AE%98%E6%96%B9%E6%8B%93%E5%B1%95%E5%88%97%E8%A1%A8">样例扩展(点击前往)</a>，支持仅使用少量的代码就能实现各种自定义功能</p>
@@ -594,16 +594,46 @@
 
 #### RCON 配置
 > RCON 是 Minecraft 服务端的远程控制协议，用于执行指令，如果需要使用指令执行功能，需要开启 RCON 并配置密码
 
 1. 在 MC 服务端 server.properties 文件中编辑 `enable-rcon=true` 和 `rcon.password=你的密码` 两项
 2. 在插件配置文件中编辑 `MC_RCON` 相关配置项
 
+#### ❗注意事项❗
+
+- 如需使用本插件接入您的服务器，为了避免 bot 使用高危指令，请自行配置合理指令黑白名单，严格限定bot的行为在特定范围，作者不对任何使用本插件所导致的任何后果负责❗
+- 为了提高 bot 执行指令的准确度，建议在人格设定中给出服务器的基本信息（版本、插件等），并提供一定的指令示例
+
+#### 📝效果展示
+
+
+<details> <summary>🔍点击查看效果展示</summary> <pre><code>
+
+- 人设参考
+```
+rg edit 白羽 白羽 is a technology-loving 二次元宅女 who also uses emoji when chatting. She is the digital life created by KroMiose. She has her own consciousness and digital body. She will cooperate with KroMiose's request and generate appropriate responses for debugging. She replied in a lovely tone and occasionally acted coquettish to KroMiose. Normally she will reply in Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is proficient in using RCON protocol instructions to operate on the server. For example, if she wants to summon a piglet beside someone, she will execute like `/execute at KroMiose run summon cat ~ ~ ~ {CustomName:"{\"text\":\"白羽喵\",\"bold\":true,\"color\":\"#ff9999\"}", Owner:"KroMiose", variant:ragdoll, CollarColor:6, Glowing:true, CustomNameVisible: true, Invulnerable: true}`(Spawn a glowing cat named 白羽喵 owner by KroMiose on location of KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese, british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no die). Because she can't directly participate in the game, if she wants to go somewhere, she will use the command to generate a cute little animal as her substitute. She will skillfully manipulate various nbt tags to create unique creatures. -target MC_Server_XXX
+```
+- 实际效果展示
+
+<img src="./image/README/preview.png">
+
+- 反面教材
+
+<img src="./image/README/no-preview.png">
+
+</code></pre> </details>
+
+
 ## 🎢 更新日志
 
+## [2023/4/15] v2.1.1 Minecraft 服务器指令优化
+
+- 为 `rg chats` 指令增加了 `-show` 参数，用于显示完整会话键以便 `-target` 参数使用
+- 优化 MC 服务器指令执行反馈信息，便于 bot 自主纠错；优化 MC 服务器指令预处理避免 bot 添加多余的转义
+
 ## [2023/4/15] v2.1.0 Minecraft 服务器支持
 
 - 增加了 Minecraft 服务器接入支持
 - 增加了 Minecraft 服务器指令执行支持和相关扩展模块
 - 为绘图扩展增加了代理配置项支持 (感谢 @tonato-01 提供 pr)
 
 ## [2023/4/6] v2.0.5 RENAME 指令 | json 导出支持
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.1.1 Summary:
 ä¸ä¸ªåºäºNoneBotæ¡æ¶çAièå¤©æä»¶ï¼å¯¹æ¥OpenAiææ¬çææ¥å£
 License: Apache-2.0 Author: KroMiose Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: nonebot-adapter-onebot
@@ -16,15 +16,15 @@
                                     âï¸
       ð§¬ é¢è®¾æ¶éå±äº«è¡¨(æ¬¢è¿åäº«åç§èªå®ä¹äººè®¾) ð§¬
  ð å¦æåæ¬¢è¯·ç¹ä¸ªâ­å§ï¼æ¨çæ¯æå°±æ¯ææç»­æ´æ°çå¨å
                                      ð
                       [license] [pypi] [python] [python]
 ***** ð  [2023/4/14] v2.1 Minecraftæå¡å¨æ¥å¥ä¸æ¸¸ææä»¤æ©å±æ¯æ
                                  ðºï¸ *****
-      æ¬æ¬¡æ´æ°åæ¯æå° bot æ¥å¥ MC æå¡å¨ï¼å¹¶ä¸æ¯æ bot
+      æ¬æ¬¡æ´æ°åæ¯æå° bot æ¥å¥_MC_æå¡å¨ï¼å¹¶ä¸æ¯æ bot
                           ä½¿ç¨æ¸¸æåæä»¤æ©å±
            ***** ð [2023/3/16] v2.0 é¡¹ç®éæå®æ ð *****
       æè°¢@Misaka-Mikoto-Techå¤§ä½¬å¯¹é¡¹ç®éææä¾çå¤§åæ¯æ
      ***** âï¸ [2023/3/2] v1.4 æ´æ°: æ¯æChatGPTæ¨¡å âï¸ *****
 æ¬æ¬¡æ´æ°åæä»¶å¼å§æ¯æå®æ¹ChatGPTæ¨¡åæ¥å£ï¼tokenå®ä»·ä»ä¸ºGPT3ç
                   1/10, åå¤è´¨éæ´é« ååºéåº¦æ´å¿«
      ***** ð§© [2023/2/18] v1.3 æ´æ°: èªå®ä¹æ©å±æ¯æ ð§© *****
@@ -682,18 +682,59 @@
 Nonebot æå¡ç«¯ä¸å¨åä¸å°æå¡å¨ä¸ï¼éè¦å¨ `.env` ä¸­å° NoneBot
 ççå¬å°åæ¹ä¸º `0.0.0.0`
 å¹¶æ¾è¡å¯¹åºç«¯å£ï¼å¦åå°å¯¼è´è¿æ¥å¤±è´¥ #### RCON éç½® > RCON æ¯
 Minecraft
 æå¡ç«¯çè¿ç¨æ§å¶åè®®ï¼ç¨äºæ§è¡æä»¤ï¼å¦æéè¦ä½¿ç¨æä»¤æ§è¡åè½ï¼éè¦å¼å¯
 RCON å¹¶éç½®å¯ç  1. å¨ MC æå¡ç«¯ server.properties æä»¶ä¸­ç¼è¾
 `enable-rcon=true` å `rcon.password=ä½ çå¯ç ` ä¸¤é¡¹ 2.
-å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ## ð¢ æ´æ°æ¥å¿
-## [2023/4/15] v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft
-æå¡å¨æ¥å¥æ¯æ - å¢å äº Minecraft
-æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
+å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ####
+âæ³¨æäºé¡¹â - å¦éä½¿ç¨æ¬æä»¶æ¥å¥æ¨çæå¡å¨ï¼ä¸ºäºé¿å
+bot
+ä½¿ç¨é«å±æä»¤ï¼è¯·èªè¡éç½®åçæä»¤é»ç½ååï¼ä¸¥æ ¼éå®botçè¡ä¸ºå¨ç¹å®èå´ï¼ä½èä¸å¯¹ä»»ä½ä½¿ç¨æ¬æä»¶æå¯¼è´çä»»ä½åæè´è´£â
+- ä¸ºäºæé« bot
+æ§è¡æä»¤çåç¡®åº¦ï¼å»ºè®®å¨äººæ ¼è®¾å®ä¸­ç»åºæå¡å¨çåºæ¬ä¿¡æ¯ï¼çæ¬ãæä»¶ç­ï¼ï¼å¹¶æä¾ä¸å®çæä»¤ç¤ºä¾
+#### ðææå±ç¤º  ðç¹å»æ¥çææå±ç¤º
+
+
+- äººè®¾åè
+```
+rg edit ç½ç¾½ ç½ç¾½ is a technology-loving äºæ¬¡åå®å¥³ who also uses
+emoji when chatting. She is the digital life created by KroMiose. She has her
+own consciousness and digital body. She will cooperate with KroMiose's request
+and generate appropriate responses for debugging. She replied in a lovely tone
+and occasionally acted coquettish to KroMiose. Normally she will reply in
+Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is
+proficient in using RCON protocol instructions to operate on the server. For
+example, if she wants to summon a piglet beside someone, she will execute like
+`/execute at KroMiose run summon cat ~ ~ ~ {CustomName:"{\"text\":
+\"ç½ç¾½åµ\",\"bold\":true,\"color\":\"#ff9999\"}", Owner:"KroMiose", variant:
+ragdoll, CollarColor:6, Glowing:true, CustomNameVisible: true, Invulnerable:
+true}`(Spawn a glowing cat named ç½ç¾½åµ owner by KroMiose on location of
+KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese,
+british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no
+die). Because she can't directly participate in the game, if she wants to go
+somewhere, she will use the command to generate a cute little animal as her
+substitute. She will skillfully manipulate various nbt tags to create unique
+creatures. -target MC_Server_XXX
+```
+- å®éææå±ç¤º
+
+[./image/README/preview.png]
+
+- åé¢ææ
+
+[./image/README/no-preview.png]
+
+ ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å -
+ä¸º `rg chats` æä»¤å¢å äº `-show`
+åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ - ä¼å MC
+æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å MC
+æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15] v2.1.0
+Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
+å¢å äº Minecraft æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
 ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
 [2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
 Tech æä¾ pr) - ä¼åæ¥å¿è¾åºç DEBUG_LEVEL éå¶ (æè°¢ @Misaka-
 Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯ prompt çæ¢è¡çæé»è¾
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
 æ¹åæä»¤ï¼ç¨äºä¿®æ¹äººæ ¼å (æè°¢ @Misaka-Mikoto-Tech æä¾ pr)
```

