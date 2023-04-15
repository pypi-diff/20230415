# Comparing `tmp/nonebot_plugin_bilichat-1.2.2.tar.gz` & `tmp/nonebot_plugin_bilichat-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.2.2.tar", last modified: Tue Apr 11 16:35:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.3.0.tar", last modified: Sat Apr 15 14:07:42 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.2.2.tar` & `nonebot_plugin_bilichat-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-11 16:35:48.299359 nonebot_plugin_bilichat-1.2.2/LICENSE
--rw-r--r--   0        0        0     6750 2023-04-11 16:35:48.299359 nonebot_plugin_bilichat-1.2.2/README.md
--rw-r--r--   0        0        0     7031 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4394 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4408 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3678 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      893 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4067 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2342 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1764 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1344 2023-04-11 16:35:58.791988 nonebot_plugin_bilichat-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-15 14:07:32.127253 nonebot_plugin_bilichat-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7010 2023-04-15 14:07:32.127253 nonebot_plugin_bilichat-1.3.0/README.md
+-rw-r--r--   0        0        0     7031 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4471 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4408 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      893 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-15 14:07:32.135253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-15 14:07:32.139253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-04-15 14:07:32.139253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5422 2023-04-15 14:07:32.139253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-15 14:07:32.139253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2342 2023-04-15 14:07:32.139253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-04-15 14:07:32.139253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1764 2023-04-15 14:07:32.139253 nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1344 2023-04-15 14:07:42.099291 nonebot_plugin_bilichat-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8299 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.2.2/LICENSE` & `nonebot_plugin_bilichat-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/README.md` & `nonebot_plugin_bilichat-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -111,32 +111,32 @@
 | bilichat_enable_private      | bool      | True                 | 是否允许响应私聊 |
 | bilichat_enable_v12_channel  | bool      | True                 | 是否允许响应频道消息(ob12专属) |
 | bilichat_enable_unkown_src   | bool      | False                | 是否允许响应未知来源的消息 |
 | bilichat_whitelist           | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist           | list[str] | []                   | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font        | str       | None                 | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time             | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
+| bilichat_neterror_retry      | int       | 3                    | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr        | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
 | bilichat_word_cloud          | bool      | True                 | 是否开启词云功能 |
 | bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) , 若留空则禁用newbing总结 |
 | bilichat_newbing_token_limit | int       | 0                    | newbing请求的文本量上限, 0为无上限 |
+| bilichat_newbing_preprocess  | bool      | True                 | 是否对newbing的返回值进行预处理, 以去除其中不想要的内容 |
 | bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None                 | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
-
 注:
 
 1. ~~合并转发由于极易受风控影响，因此不推荐使用~~已经把合并转发砍了，没精力适配这玩意了
 2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `openai` 进行总结
 3. 经测试，目前 newbing 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 4. 由于 newbing 限制较大，也不如 openai 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
 
-
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
 
 > 正在开发指令相关，请无视这里的模板
```

#### html2text {}

```diff
@@ -33,27 +33,29 @@
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_v12_channel | bool | True |
 æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±) | | bilichat_enable_unkown_src |
 bool | False | æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist |
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
-(é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
-æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
+(é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
+å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
+True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
 bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾
 (è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
 authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
 plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) ,
 è¥çç©ºåç¦ç¨newbingæ»ç» | | bilichat_newbing_token_limit | int | 0 |
-newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_openai_token | str
-| None | openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | |
-bilichat_openai_proxy | str | None |
-è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
-gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess
+| bool | True | æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç,
+ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹ | | bilichat_openai_token | str | None |
+openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str
+| None | è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model
+| str | gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
 bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
 è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | æ³¨: 1.
 ~~åå¹¶è½¬åç±äºææåé£æ§å½±åï¼å æ­¤ä¸æ¨èä½¿ç¨~~å·²ç»æåå¹¶è½¬åç äºï¼æ²¡ç²¾åééè¿ç©æäº
 2. å¦æåæ¶å¡«åäº `bilichat_openai_token` å
 `bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `openai` è¿è¡æ»ç» 3.
 ç»æµè¯ï¼ç®å newbing è³å°è½æ»ç» 12000 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ
 token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
```

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,27 @@
     bilichat_enable_private: bool = True
     bilichat_enable_v12_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
+    bilichat_neterror_retry = 3
     nickname: List[str] = ["awesome-nonebot"]
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = True
 
     # AI Summary
     bilichat_newbing_cookie: Optional[str]
     bilichat_newbing_token_limit: int = 0
+    bilichat_newbing_preprocess: bool = True
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
     bilichat_openai_model: Literal["gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
 
     @validator("nickname")
     def check_nickname(cls, v):
```

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,21 +65,28 @@
             audio_resp = await client.get(
                 playview.video_info.dash_audio[-1].backup_url[0]
                 if playview.video_info.dash_audio[-1].backup_url
                 else playview.video_info.dash_audio[-1].baseUrl,
             )
         audio_resp.raise_for_status()
         audio = audio_resp.content
-        try:
-            asr = await get_bcut_asr(audio)
-        except Exception as e:
-            logger.exception(f"BCut-ASR conversion failed: {e}")
-            capture_exception()
-            raise AbortError("BCut-ASR conversion failed") from e
-        return [x.transcript for x in asr]
+        for count in range(plugin_config.bilichat_neterror_retry):
+            try:
+                asr = await get_bcut_asr(audio)
+                return [x.transcript for x in asr]
+            except httpx.ReadTimeout as e:
+                logger.error(
+                    f"except httpx.ReadTimeout, retry count remaining {plugin_config.bilichat_neterror_retry-count-1}"
+                )
+                await asyncio.sleep(5)
+            except Exception as e:
+                logger.exception(f"BCut-ASR conversion failed: {e}")
+                capture_exception()
+                raise AbortError("BCut-ASR conversion failed") from e
+        raise AbortError("BCut-ASR conversion failed due to network error")
     else:
         raise AbortError("Subtitles not found and BCut-ASR is disabled in env")
     return [x["content"] for x in subtitle.json()["body"]]
 
 
 async def get_bcut_asr(file_bytes: bytes):
     bcut = BcutASR()
```

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import random
 import re
 from collections import OrderedDict
 from pathlib import Path
-from typing import List
+from typing import List, Dict
 
 from EdgeGPT import Chatbot, ConversationStyle
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..lib.store import BING_APOLOGY
 from ..model.cache import Cache
@@ -23,37 +23,63 @@
         logger.success("Bing chatbot init success")
         break
     except Exception:
         logger.error(f"Bing chatbot init failed, retrying {count+1}/5")
 
 
 def get_small_size_transcripts(title: str, text_data: List[str]):
-    prompt = f"请为视频“{title}”总结文案,开头用一整段文字简述视频的要点(大于40字符),\
-随后总结2-6条视频的Bulletpoint(每条大于15字符),\
-然后使用以下格式输出总结内容 ## 总结 \n ## 要点 \n - [Emoji] Bulletpoint\n\n,\
-如果你无法找到相关的信息可以尝试自己总结,\
-但请一定不要输出任何其他内容。视频文案的内容如下: "
+    prompt = (
+        "使用以下Markdown模板为我总结视频字幕数据，除非字幕中的内容无意义，或者内容较少无法总结，或者未提供字幕数据，或者无有效内容，你就不使用模板回复，只回复“无意义”：\
+        ## 概述\
+        {内容，尽可能精简总结内容不要太详细}\
+        ## 要点\
+        - {使用不重复并合适的emoji，仅限一个，禁止重复} {内容不换行大于15字，可多项，条数与有效内容数量呈正比}\
+        不要随意翻译任何内容。仅使用中文总结。\
+        不说与总结无关的其他内容，你的回复仅限固定格式提供的“概述”和“要点”两项。"
+        + f"视频标题为“{title}”，视频字幕数据如下，立刻开始总结："
+    )
     unique_texts = list(OrderedDict.fromkeys(text_data))
     if plugin_config.bilichat_newbing_token_limit > 0:
         while len(",".join(unique_texts)) + len(prompt) > plugin_config.bilichat_newbing_token_limit:
             unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return prompt + ",".join(unique_texts)
 
 
+def newbing_summary_preprocess(ai_summary: str):
+    # https://github.com/djkcyl/nonebot-plugin-bilichat/pull/18
+    """预处理（清洗）newbing输出的总结内容"""
+    if search_obj := re.search(r"##\s+概述\s+(.*)##\s+要点\s+(.*)", ai_summary, re.S):
+        summary = search_obj[1].strip()
+        bulletpoint = search_obj[2].strip()
+        bulletpoint = re.sub(r"\[\^\d+\^\]\s*", "", bulletpoint)  # 去除引用标记 eg. [^1^]
+        bulletpoint = re.sub(r"-\s*\[(.+?)\]\s*", r"\n● \g<1> ", bulletpoint)
+        bulletpoint = re.sub(r"\n+", r"\n", bulletpoint).strip()
+        bing_summary = f"## 总结\n{summary}\n\n## 要点\n{bulletpoint}"
+        logger.info(f"Newbing summary: \n{bing_summary}")
+        return bing_summary
+    else:
+        logger.debug(f"Newbing output is meaningless: \n{ai_summary}")
+        return None
+
+
 async def newbing_req(prompt: str):
     logger.debug(f"prompt have {len(prompt)} chars")
     ans = await bot.ask(
         prompt=prompt,
         conversation_style=ConversationStyle.creative,
         wss_link="wss://sydney.bing.com/sydney/ChatHub",
     )
     await bot.reset()
     logger.debug(ans)
-    bing_resp = ans["item"]["messages"][1]
-    return None if bing_resp["contentOrigin"] == "Apology" else bing_resp["text"]
+    bing_resp: Dict = ans["item"]["messages"][1]
+    return (
+        newbing_summary_preprocess(bing_resp.get("text", ""))
+        if plugin_config.bilichat_newbing_preprocess
+        else bing_resp.get("text", None)
+    )
 
 
 async def newbing_summarization(cache: Cache, cid: str = "0"):
     meaning = False
     try:
         if not cache.episodes[cid].newbing:
             if cache.id[:2].lower() in ["bv", "av"]:
```

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.2/pyproject.toml` & `nonebot_plugin_bilichat-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.2.2"
+version = "1.3.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.2.2/PKG-INFO` & `nonebot_plugin_bilichat-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.2.2
+Version: 1.3.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -144,32 +144,32 @@
 | bilichat_enable_private      | bool      | True                 | 是否允许响应私聊 |
 | bilichat_enable_v12_channel  | bool      | True                 | 是否允许响应频道消息(ob12专属) |
 | bilichat_enable_unkown_src   | bool      | False                | 是否允许响应未知来源的消息 |
 | bilichat_whitelist           | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist           | list[str] | []                   | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font        | str       | None                 | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time             | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
+| bilichat_neterror_retry      | int       | 3                    | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr        | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
 | bilichat_word_cloud          | bool      | True                 | 是否开启词云功能 |
 | bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) , 若留空则禁用newbing总结 |
 | bilichat_newbing_token_limit | int       | 0                    | newbing请求的文本量上限, 0为无上限 |
+| bilichat_newbing_preprocess  | bool      | True                 | 是否对newbing的返回值进行预处理, 以去除其中不想要的内容 |
 | bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None                 | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
-
 注:
 
 1. ~~合并转发由于极易受风控影响，因此不推荐使用~~已经把合并转发砍了，没精力适配这玩意了
 2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `openai` 进行总结
 3. 经测试，目前 newbing 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 4. 由于 newbing 限制较大，也不如 openai 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
 
-
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
 
 > 正在开发指令相关，请无视这里的模板
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.3.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
@@ -51,27 +51,29 @@
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_v12_channel | bool | True |
 æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±) | | bilichat_enable_unkown_src |
 bool | False | æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist |
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
-(é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
-æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
+(é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
+å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
+True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
 bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾
 (è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
 authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
 plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) ,
 è¥çç©ºåç¦ç¨newbingæ»ç» | | bilichat_newbing_token_limit | int | 0 |
-newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_openai_token | str
-| None | openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | |
-bilichat_openai_proxy | str | None |
-è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
-gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess
+| bool | True | æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç,
+ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹ | | bilichat_openai_token | str | None |
+openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str
+| None | è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model
+| str | gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
 bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
 è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | æ³¨: 1.
 ~~åå¹¶è½¬åç±äºææåé£æ§å½±åï¼å æ­¤ä¸æ¨èä½¿ç¨~~å·²ç»æåå¹¶è½¬åç äºï¼æ²¡ç²¾åééè¿ç©æäº
 2. å¦æåæ¶å¡«åäº `bilichat_openai_token` å
 `bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `openai` è¿è¡æ»ç» 3.
 ç»æµè¯ï¼ç®å newbing è³å°è½æ»ç» 12000 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ
 token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
```

