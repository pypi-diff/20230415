# Comparing `tmp/chatgpt-tool-hub-0.3.7.tar.gz` & `tmp/chatgpt-tool-hub-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-tool-hub-0.3.7.tar", last modified: Sat Apr  8 03:11:07 2023, max compression
+gzip compressed data, was "chatgpt-tool-hub-0.3.9.tar", last modified: Tue Apr 11 18:05:34 2023, max compression
```

## Comparing `chatgpt-tool-hub-0.3.7.tar` & `chatgpt-tool-hub-0.3.9.tar`

### file list

```diff
@@ -1,126 +1,141 @@
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.830018 chatgpt-tool-hub-0.3.7/
--rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.3.7/LICENSE
--rw-r--r--   0 goldfish   (502) staff       (20)    10874 2023-04-08 03:11:07.829847 chatgpt-tool-hub-0.3.7/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)    10079 2023-04-02 13:42:19.000000 chatgpt-tool-hub-0.3.7/README.md
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.808418 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 16:32:46.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.810266 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/
--rw-r--r--   0 goldfish   (502) staff       (20)       52 2023-03-27 18:16:41.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      215 2023-03-27 18:16:41.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/all_app_list.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1546 2023-04-03 00:57:23.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1917 2023-04-02 12:09:49.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/lite_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2072 2023-04-08 03:03:53.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/load_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4400 2023-04-06 14:42:32.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/victorinox.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.811204 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      236 2023-03-27 18:17:19.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/all_bot_list.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12357 2023-04-06 15:03:51.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/bot.py
--rw-r--r--   0 goldfish   (502) staff       (20)    11530 2023-04-08 02:32:23.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/bot_executor.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.811757 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/chat_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/chat_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4880 2023-04-06 13:55:19.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/chat_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      913 2023-04-07 01:31:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/chat_bot/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1935 2023-04-02 11:55:16.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/initialize.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.812213 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/qa_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/qa_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4475 2023-03-27 18:25:42.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/qa_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      635 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/qa_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.813116 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/
--rw-r--r--   0 goldfish   (502) staff       (20)      225 2023-03-27 18:18:03.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.813899 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/api/
--rw-r--r--   0 goldfish   (502) staff       (20)       84 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4250 2023-04-02 15:05:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/api/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1022 2023-03-27 18:20:09.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/api/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)    10688 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7544 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/llm.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.817907 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5094 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/cache.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1647 2023-03-30 15:40:12.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/calculate_token.py
--rw-r--r--   0 goldfish   (502) staff       (20)    25561 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/callbacks.py
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 15:18:58.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/config.py
--rw-r--r--   0 goldfish   (502) staff       (20)      139 2023-03-30 15:20:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/constants.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1262 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/document.py
--rw-r--r--   0 goldfish   (502) staff       (20)      981 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/formatting.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1092 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/input.py
--rw-r--r--   0 goldfish   (502) staff       (20)      510 2023-04-06 15:42:09.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/log.py
--rw-r--r--   0 goldfish   (502) staff       (20)     8579 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/schema.py
--rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/singleton.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6714 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/text_splitter.py
--rw-r--r--   0 goldfish   (502) staff       (20)      689 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.818927 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/
--rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1684 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/chat_memory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2395 2023-04-02 13:29:17.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/token_buffer.py
--rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.819657 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/
--rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    13016 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/base.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.820642 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/chatgpt/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/chatgpt/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5393 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/chatgpt/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15182 2023-04-07 16:11:18.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/chatgpt/chatgpt.py
--rw-r--r--   0 goldfish   (502) staff       (20)    28459 2023-04-02 12:09:49.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/openai.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.821419 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/
--rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6421 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/chat.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      328 2023-04-02 13:23:16.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/run.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.822145 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3779 2023-04-08 01:43:51.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/all_tool_list.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4023 2023-04-02 11:48:52.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/base_tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.822868 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/bing_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      146 2023-04-01 00:56:58.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/bing_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      953 2023-04-01 00:57:31.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/bing_search/bing_search.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3413 2023-04-02 12:41:32.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/bing_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.823456 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/debug/
--rw-r--r--   0 goldfish   (502) staff       (20)       57 2023-04-03 14:50:43.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/debug/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      938 2023-04-03 14:30:20.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/debug/debug.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.824181 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/google_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      174 2023-03-30 14:10:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/google_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1614 2023-04-01 01:48:49.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/google_search/google_search.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3454 2023-04-01 01:48:49.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/google_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2856 2023-04-08 01:43:51.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/load_tools.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.824944 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/meteo/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-27 13:10:30.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/meteo/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3254 2023-04-03 14:23:09.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/meteo/api_docs_prompts.py
--rw-r--r--   0 goldfish   (502) staff       (20)      904 2023-04-06 15:28:50.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/meteo/meteo_weather.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.825630 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/news/
--rw-r--r--   0 goldfish   (502) staff       (20)      121 2023-03-28 16:36:30.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2437 2023-04-03 14:18:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/news/api_docs_prompts.py
--rw-r--r--   0 goldfish   (502) staff       (20)      899 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/news/news.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.825980 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/python/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/python/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1987 2023-04-08 01:44:46.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/python/python_repl.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.826213 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/terminal/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-27 12:40:13.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/terminal/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4069 2023-04-08 03:07:02.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/terminal/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3669 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.828201 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/
--rw-r--r--   0 goldfish   (502) staff       (20)     1830 2023-04-05 01:32:42.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1338 2023-04-05 05:14:36.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/browser.py
--rw-r--r--   0 goldfish   (502) staff       (20)      749 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/delete.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1641 2023-04-05 05:15:36.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/get.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/patch.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2058 2023-03-30 15:44:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/post.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/put.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6093 2023-04-05 05:11:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.828911 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wikipedia/
--rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wikipedia/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      844 2023-04-05 06:37:29.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2151 2023-04-01 01:52:08.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wikipedia/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.829549 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wolfram_alpha/
--rw-r--r--   0 goldfish   (502) staff       (20)      170 2023-03-28 16:36:30.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      914 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1902 2023-03-30 15:40:12.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-04-08 02:15:39.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/version.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-08 03:11:07.808953 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/
--rw-r--r--   0 goldfish   (502) staff       (20)    10874 2023-04-08 03:11:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)     3797 2023-04-08 03:11:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/SOURCES.txt
--rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-04-08 03:11:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/dependency_links.txt
--rw-r--r--   0 goldfish   (502) staff       (20)      202 2023-04-08 03:11:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/requires.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-04-08 03:11:07.000000 chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/top_level.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-04-08 03:11:07.830063 chatgpt-tool-hub-0.3.7/setup.cfg
--rw-r--r--   0 goldfish   (502) staff       (20)     1874 2023-04-03 00:58:37.000000 chatgpt-tool-hub-0.3.7/setup.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.750461 chatgpt-tool-hub-0.3.9/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.3.9/LICENSE
+-rw-r--r--   0 goldfish   (502) staff       (20)    12322 2023-04-11 18:05:34.750254 chatgpt-tool-hub-0.3.9/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)    11527 2023-04-11 17:18:33.000000 chatgpt-tool-hub-0.3.9/README.md
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.723220 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/
+-rw-r--r--   0 goldfish   (502) staff       (20)      287 2023-04-11 14:39:52.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.725372 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/
+-rw-r--r--   0 goldfish   (502) staff       (20)       52 2023-04-08 09:10:31.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      215 2023-03-27 18:16:41.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/all_app_list.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1546 2023-04-03 00:57:23.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1733 2023-04-08 18:43:42.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/app_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1943 2023-04-08 19:02:47.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/lite_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1641 2023-04-08 18:42:45.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/load_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4390 2023-04-09 04:03:14.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/victorinox.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.726482 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      236 2023-03-27 18:17:19.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/all_bot_list.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12507 2023-04-11 16:27:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    11530 2023-04-08 02:32:23.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot_executor.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.727074 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5338 2023-04-11 14:56:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      915 2023-04-11 14:00:29.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1935 2023-04-02 11:55:16.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/initialize.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.727666 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4475 2023-03-27 18:25:42.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      635 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.728514 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/
+-rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.729324 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/
+-rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4243 2023-04-09 16:23:42.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1229 2023-04-09 16:24:47.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    10688 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7544 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/llm.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.733257 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5094 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/cache.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1646 2023-04-10 16:23:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/calculate_token.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    25561 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/callbacks.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      262 2023-04-11 14:28:26.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/constants.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1262 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/document.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      981 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/formatting.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1092 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/input.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      601 2023-04-09 14:00:24.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/log.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     8579 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/schema.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/singleton.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6714 2023-03-27 18:18:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/text_splitter.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      693 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.734155 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/
+-rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1684 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/chat_memory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2395 2023-04-02 13:29:17.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/token_buffer.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.735202 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1381 2023-04-11 15:05:57.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    13016 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/base.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.736057 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5393 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15182 2023-04-07 16:11:18.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/chatgpt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      521 2023-04-08 08:53:56.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/model_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    28454 2023-04-08 08:51:59.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/openai.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.737062 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/
+-rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6421 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/chat.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.738112 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/
+-rw-r--r--   0 goldfish   (502) staff       (20)      535 2023-04-11 17:10:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      737 2023-04-08 18:52:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/all_tool_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.738772 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      143 2023-04-05 16:49:17.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1660 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/arxiv_search.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1672 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4023 2023-04-02 11:48:52.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/base_tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.739452 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      146 2023-04-01 00:56:58.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1219 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/bing_search.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3449 2023-04-09 04:35:45.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.739929 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/
+-rw-r--r--   0 goldfish   (502) staff       (20)       57 2023-04-03 14:50:43.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1101 2023-04-08 19:06:04.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/debug.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.740588 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      174 2023-03-30 14:10:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1804 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/google_search.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3571 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2001 2023-04-09 04:04:32.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/load_tools.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.741300 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/
+-rw-r--r--   0 goldfish   (502) staff       (20)       71 2023-04-08 18:45:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4625 2023-04-11 17:08:37.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/api_docs_prompts.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1679 2023-04-11 17:15:41.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/meteo_weather.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.741933 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       77 2023-04-11 16:16:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2321 2023-04-11 16:12:06.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/morning_news.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/morning_news/summary_prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.742622 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/
+-rw-r--r--   0 goldfish   (502) staff       (20)      121 2023-03-28 16:36:30.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2437 2023-04-03 14:18:25.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/api_docs_prompts.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1664 2023-04-08 18:30:12.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/news.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.743105 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/
+-rw-r--r--   0 goldfish   (502) staff       (20)       68 2023-04-08 18:36:10.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2153 2023-04-08 19:22:38.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/python_repl.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.743780 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      172 2023-04-03 16:21:48.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1887 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/searxng.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15595 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/searxng_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.744309 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/
+-rw-r--r--   0 goldfish   (502) staff       (20)       57 2023-04-08 18:44:31.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4229 2023-04-09 03:07:36.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3673 2023-04-09 15:20:49.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.744754 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/visual_dl/
+-rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/visual_dl/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2229 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/visual_dl/text2image.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.746981 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1919 2023-04-11 15:50:56.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1338 2023-04-05 05:14:36.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/browser.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      749 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/delete.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1821 2023-04-08 19:06:57.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/get.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/patch.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2058 2023-03-30 15:44:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/post.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/put.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6307 2023-04-11 15:03:14.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.748568 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/
+-rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1058 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2370 2023-04-08 17:28:21.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.749389 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/
+-rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1177 2023-04-08 18:14:11.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1902 2023-03-30 15:40:12.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-04-11 18:05:22.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/version.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-11 18:05:34.723811 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/
+-rw-r--r--   0 goldfish   (502) staff       (20)    12322 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)     4358 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)      213 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/requires.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-04-11 18:05:34.000000 chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/top_level.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-04-11 18:05:34.750501 chatgpt-tool-hub-0.3.9/setup.cfg
+-rw-r--r--   0 goldfish   (502) staff       (20)     1897 2023-04-11 17:57:20.000000 chatgpt-tool-hub-0.3.9/setup.py
```

### Comparing `chatgpt-tool-hub-0.3.7/LICENSE` & `chatgpt-tool-hub-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/PKG-INFO` & `chatgpt-tool-hub-0.3.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: chatgpt-tool-hub
-Version: 0.3.7
-Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
-Home-page: https://github.com/goldfishh/chatgpt-tool-hub
-Author: goldfishh
-Author-email: goldfish.buaa@gmail.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h2 align='center'> chatgpt-tool-hub / ChatGPT工具引擎 </h2>
 <p align='center'>给ChatGPT装上手和脚，拿起工具提高你的生产力</p>
 
 <p align="center">
   <a style="text-decoration:none" href="https://aianything.netlify.app" target="_blank">
     <img src="https://img.shields.io/badge/language-python-blue" alt="Language" />
   </a>
@@ -58,37 +39,87 @@
 
 - 支持中文输入输出
 - 支持上下文记忆
 - 支持proxy
 - 支持多种工具： 
   - terminal
   - python
-  - requests
+  - url-get
   - wikipedia
   - meteo-weather
   - news
+  - morning-news
   - bing-search
   - wolfram-alpha
 
 
 ## 快速开始
 
 ---
+### 1.  使用shell运行demo
+
+#### (1). 克隆源代码
+
+```bash
+git clone git@github.com:goldfishh/chatgpt-tool-hub.git
+```
+
+#### (2). `pip install -r requirements.txt`
+
+#### (3). 编辑config.json，填入你的openai_api_key
+
+```json
+{
+  "tools": [],  // 这里填入你想加载的工具名，默认工具无需填入自动加载
+  "kwargs": {
+      "openai_api_key": "",  // 必填
+      "proxy": "",  // 代理配置，国外ip可忽略
+      "debug": false,  // 当你遇到问题提issue前请设置debug为true，提交输出日志
+      "no_default": false,  // 控制是否加载默认工具
+      "model_name": "gpt-3.5-turbo"  // 默认，其他模型暂未测试
+  }
+}
+```
+
+#### (4). `python3 run.py 你的问题1 [你的问题2 ......]`
+
+> chatgpt判断回复是否使用工具，你可要求chatgpt使用工具（更进一步地使用哪个工具）来帮助它更好回答你的问题
+
+#### (5). 给项目点个star & 有能力pr，支持项目作者继续开发...
+
+--- 
+
+### 2. 去[chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat)使用本项目开发的tool插件：[tool README](https://github.com/goldfishh/chatgpt-on-wechat/blob/master/plugins/tool/README.md)
+
+> 你可以在微信用到本项目为chatgpt提供的工具能力
+
+---
+
+### 3. 你是其他项目开发者，想要接入本工具引擎
+
+#### (1). 安装chatgpt-tool-hub包
+
+`pip install -i https://pypi.python.org/simple chatgpt-tool-hub`
+
+#### (2). 示例代码：
 
-`pip install chatgpt-tool-hub`
 ```python
 import os
 from chatgpt_tool_hub.apps import load_app
 os.environ["OPENAI_API_KEY"] = YOUR_OPENAI_API_KEY
 os.environ["PROXY"] = "http://192.168.7.1:7890"
 app = load_app()
 reply = app.ask(YOUR_QUESTION_TO_HERE)
 print(reply)
 ```
-PS: 默认加载：python、requests、terminal、meteo-weather工具
+  
+> 如果有需求，我会更新接入的文档，欢迎提issue
+
+---
+
 ## 工具指南
 
 ---
 
 > 工具名末尾加*表示使用该工具需要额外申请服务key, 超出免费额度需给服务提供商**支付费用** 
 
 #### 1. terminal
@@ -105,15 +136,15 @@
 python解释器，使用它来解释执行python指令，可以配合你想要ChatGPT生成的代码输出结果或执行事务
 
 ```text
 1. 使用python查询今天日期    
 2. eval this expression: hex(123456)-123    
 ```
 
-#### 3. requests
+#### 3. url-get
 
 往往用来获取某个网站具体内容，结果可能会被反爬策略影响
 
 ```
 1. 总结信息 https://github.com/goldfishh/chatgpt-tool-hub    
 2. 可以作为信息入口配合其他工具   
 ```
@@ -167,15 +198,15 @@
 
 工具引擎的实现原理本质是**Chain-of-Thought**：[Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)
   
 我将通过用6个自问自答的问题解释chatgpt-tool-hub的工作原理  
 
 #### 1. 事务型工具（如terminal、python）是在哪运行，以及如何执行的
 
-事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、requests工具分别用到了封装调用subprocess库、python解释器和request库的函数
+事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、url-get工具分别用到了封装调用subprocess库、python解释器和requests库的函数
 
 --- 
 
 #### 2. ChatGPT是如何触发调用这些函数
 
 借助ChatGPT api提供的temperature参数，该参数越低，ChatGPT输出的结果会更集中和确定，当temperature为0时，相同的问题会得到统一回答  
 我在prompt构建时会提供给ChatGPT此时用到的工具列表信息，每个工具信息包含：工具名 和 工具描述：
@@ -183,15 +214,15 @@
 ```text
 TOOLS:  
 ------  
   
 You have access to the following tools:  
 
 > Python REPL: A Python shell. Use this to execute python commands. 
-> requests_get: A portal to the internet. Use this when you need to get specific content from a website. 
+> url-get: A portal to the internet. Use this when you need to get specific content from a website. 
 > Terminal: Executes commands in a terminal. 
 > Bing Search: A wrapper around Bing Search. Useful for when you need to answer questions about current events. 
 ```
 
 有了工具prompt，这时ChatGPT就能理解这些工具名字和使用场景，调用事务函数还需要进一步细化我和ChatGPT之间的通信协议（仍是通过prompt）：
 通信协议限制ChatGPT使用工具时返回内容的格式，只能返回三种前缀的内容：
 
@@ -203,15 +234,15 @@
 
 通信协议完整prompt：  
 ```text
 To use a tool, please use the following format:
 
 
 Thought: Do I need to use a tool? Yes
-Action: the action to take, should be one of [Python REPL, requests_get, Terminal, Bing Search]
+Action: the action to take, should be one of [Python REPL, url-get, Terminal, Bing Search]
 Action Input: the input to the action
 Observation: the result of the action
 ```
 
 此时，工具引擎有专用的文本解析模块负责解析这些内容，当解析成功后，将调度到具体事务函数执行，然后返回固定前缀的结果：
 
 ```text
@@ -299,15 +330,15 @@
 [○] 粒度配置  
 [○] 语音输入  
 [✗] 一个前端demo   
   
 ### tool todolist  
    
 [○] stable-diffusion 中文prompt翻译    
-[○] ImageCaptioning   
+[✓] ImageCaptioning   
 [○] 小米智能家居控制   
 [○] 支持ChatGPT官方插件  
 [○] 支持图片处理工具   
 [○] 支持视频处理工具  
 [✗] Wechat  
 
 ## Q&A
```

### Comparing `chatgpt-tool-hub-0.3.7/README.md` & `chatgpt-tool-hub-0.3.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: chatgpt-tool-hub
+Version: 0.3.9
+Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
+Home-page: https://github.com/goldfishh/chatgpt-tool-hub
+Author: goldfishh
+Author-email: goldfish.buaa@gmail.com
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h2 align='center'> chatgpt-tool-hub / ChatGPT工具引擎 </h2>
 <p align='center'>给ChatGPT装上手和脚，拿起工具提高你的生产力</p>
 
 <p align="center">
   <a style="text-decoration:none" href="https://aianything.netlify.app" target="_blank">
     <img src="https://img.shields.io/badge/language-python-blue" alt="Language" />
   </a>
@@ -39,37 +58,87 @@
 
 - 支持中文输入输出
 - 支持上下文记忆
 - 支持proxy
 - 支持多种工具： 
   - terminal
   - python
-  - requests
+  - url-get
   - wikipedia
   - meteo-weather
   - news
+  - morning-news
   - bing-search
   - wolfram-alpha
 
 
 ## 快速开始
 
 ---
+### 1.  使用shell运行demo
+
+#### (1). 克隆源代码
+
+```bash
+git clone git@github.com:goldfishh/chatgpt-tool-hub.git
+```
+
+#### (2). `pip install -r requirements.txt`
+
+#### (3). 编辑config.json，填入你的openai_api_key
+
+```json
+{
+  "tools": [],  // 这里填入你想加载的工具名，默认工具无需填入自动加载
+  "kwargs": {
+      "openai_api_key": "",  // 必填
+      "proxy": "",  // 代理配置，国外ip可忽略
+      "debug": false,  // 当你遇到问题提issue前请设置debug为true，提交输出日志
+      "no_default": false,  // 控制是否加载默认工具
+      "model_name": "gpt-3.5-turbo"  // 默认，其他模型暂未测试
+  }
+}
+```
+
+#### (4). `python3 run.py 你的问题1 [你的问题2 ......]`
+
+> chatgpt判断回复是否使用工具，你可要求chatgpt使用工具（更进一步地使用哪个工具）来帮助它更好回答你的问题
+
+#### (5). 给项目点个star & 有能力pr，支持项目作者继续开发...
+
+--- 
+
+### 2. 去[chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat)使用本项目开发的tool插件：[tool README](https://github.com/goldfishh/chatgpt-on-wechat/blob/master/plugins/tool/README.md)
+
+> 你可以在微信用到本项目为chatgpt提供的工具能力
+
+---
+
+### 3. 你是其他项目开发者，想要接入本工具引擎
+
+#### (1). 安装chatgpt-tool-hub包
+
+`pip install -i https://pypi.python.org/simple chatgpt-tool-hub`
+
+#### (2). 示例代码：
 
-`pip install chatgpt-tool-hub`
 ```python
 import os
 from chatgpt_tool_hub.apps import load_app
 os.environ["OPENAI_API_KEY"] = YOUR_OPENAI_API_KEY
 os.environ["PROXY"] = "http://192.168.7.1:7890"
 app = load_app()
 reply = app.ask(YOUR_QUESTION_TO_HERE)
 print(reply)
 ```
-PS: 默认加载：python、requests、terminal、meteo-weather工具
+  
+> 如果有需求，我会更新接入的文档，欢迎提issue
+
+---
+
 ## 工具指南
 
 ---
 
 > 工具名末尾加*表示使用该工具需要额外申请服务key, 超出免费额度需给服务提供商**支付费用** 
 
 #### 1. terminal
@@ -86,15 +155,15 @@
 python解释器，使用它来解释执行python指令，可以配合你想要ChatGPT生成的代码输出结果或执行事务
 
 ```text
 1. 使用python查询今天日期    
 2. eval this expression: hex(123456)-123    
 ```
 
-#### 3. requests
+#### 3. url-get
 
 往往用来获取某个网站具体内容，结果可能会被反爬策略影响
 
 ```
 1. 总结信息 https://github.com/goldfishh/chatgpt-tool-hub    
 2. 可以作为信息入口配合其他工具   
 ```
@@ -148,15 +217,15 @@
 
 工具引擎的实现原理本质是**Chain-of-Thought**：[Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)
   
 我将通过用6个自问自答的问题解释chatgpt-tool-hub的工作原理  
 
 #### 1. 事务型工具（如terminal、python）是在哪运行，以及如何执行的
 
-事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、requests工具分别用到了封装调用subprocess库、python解释器和request库的函数
+事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、url-get工具分别用到了封装调用subprocess库、python解释器和requests库的函数
 
 --- 
 
 #### 2. ChatGPT是如何触发调用这些函数
 
 借助ChatGPT api提供的temperature参数，该参数越低，ChatGPT输出的结果会更集中和确定，当temperature为0时，相同的问题会得到统一回答  
 我在prompt构建时会提供给ChatGPT此时用到的工具列表信息，每个工具信息包含：工具名 和 工具描述：
@@ -164,15 +233,15 @@
 ```text
 TOOLS:  
 ------  
   
 You have access to the following tools:  
 
 > Python REPL: A Python shell. Use this to execute python commands. 
-> requests_get: A portal to the internet. Use this when you need to get specific content from a website. 
+> url-get: A portal to the internet. Use this when you need to get specific content from a website. 
 > Terminal: Executes commands in a terminal. 
 > Bing Search: A wrapper around Bing Search. Useful for when you need to answer questions about current events. 
 ```
 
 有了工具prompt，这时ChatGPT就能理解这些工具名字和使用场景，调用事务函数还需要进一步细化我和ChatGPT之间的通信协议（仍是通过prompt）：
 通信协议限制ChatGPT使用工具时返回内容的格式，只能返回三种前缀的内容：
 
@@ -184,15 +253,15 @@
 
 通信协议完整prompt：  
 ```text
 To use a tool, please use the following format:
 
 
 Thought: Do I need to use a tool? Yes
-Action: the action to take, should be one of [Python REPL, requests_get, Terminal, Bing Search]
+Action: the action to take, should be one of [Python REPL, url-get, Terminal, Bing Search]
 Action Input: the input to the action
 Observation: the result of the action
 ```
 
 此时，工具引擎有专用的文本解析模块负责解析这些内容，当解析成功后，将调度到具体事务函数执行，然后返回固定前缀的结果：
 
 ```text
@@ -280,15 +349,15 @@
 [○] 粒度配置  
 [○] 语音输入  
 [✗] 一个前端demo   
   
 ### tool todolist  
    
 [○] stable-diffusion 中文prompt翻译    
-[○] ImageCaptioning   
+[✓] ImageCaptioning   
 [○] 小米智能家居控制   
 [○] 支持ChatGPT官方插件  
 [○] 支持图片处理工具   
 [○] 支持视频处理工具  
 [✗] Wechat  
 
 ## Q&A
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/app.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/lite_app.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/lite_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from chatgpt_tool_hub.apps.app import App
 from chatgpt_tool_hub.apps.load_app import load_app
 from chatgpt_tool_hub.chains import LLMChain
 from chatgpt_tool_hub.common.log import LOG
-from chatgpt_tool_hub.models.chatgpt import ChatOpenAI
+from chatgpt_tool_hub.models.model_factory import ModelFactory
 from chatgpt_tool_hub.prompts import PromptTemplate
 
 
 class LiteApp(App):
 
     def __init__(self, **app_kwargs):
         super().__init__()
         if not self.init_flag:
-
-            self.llm = ChatOpenAI(temperature=0.9, **app_kwargs)
+            self.llm = ModelFactory.create_llm_model(temperature=0.9, **app_kwargs)
 
             self.prompt = PromptTemplate(
                 input_variables=["question"],
                 template="{question}?",
             )
 
             self.init_flag = True
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/load_app.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/load_app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from chatgpt_tool_hub.apps.app import App
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.models import build_model_params
 
 
 def init_env(**kwargs):
     """ 环境初始化 """
     # debug mode
     debug_flag = get_from_dict_or_env(kwargs, "debug", "DEBUG", "")
     if debug_flag:
@@ -16,49 +17,37 @@
 
     # default tools
     no_default_flag = get_from_dict_or_env(kwargs, "no_default", "NO_DEFAULT", "")
     global default_tools_list
     if no_default_flag:
         default_tools_list = []
     else:
-        default_tools_list = ["python", "requests", "terminal", "meteo-weather"]
-
-
-def get_app_kwargs(kwargs: dict) -> dict:
-    return {
-        "openai_api_key": get_from_dict_or_env(kwargs, "openai_api_key", "OPENAI_API_KEY"),
-        "proxy": get_from_dict_or_env(kwargs, "proxy", "PROXY", ""),
-        "model_name": get_from_dict_or_env(kwargs, "model_name", "MODEL_NAME", "gpt-3.5-turbo"),  # 对话模型的名称
-        "top_p": 1,
-        "frequency_penalty": 0.0,  # [-2,2]之间，该值越大则更倾向于产生不同的内容
-        "presence_penalty": 0.0,  # [-2,2]之间，该值越大则更倾向于产生不同的内容
-        "request_timeout": 60,
-        "max_retries": 2
-    }
+        default_tools_list = ["python", "url-get", "terminal", "meteo-weather"]
 
 
 def load_app(app_type: str = 'victorinox', tools_list: list = None, **kwargs) -> App:
+    LOG.warning("[deprecated]: load_app will be replaced by chatgpt_tool_hub.apps.AppFactory.create_app")
     tools_list = [] if not tools_list else tools_list
 
     init_env(**kwargs)
 
     if app_type == 'lite':
         from chatgpt_tool_hub.apps.lite_app import LiteApp
-        app = LiteApp(**get_app_kwargs(kwargs))
+        app = LiteApp(**build_model_params(kwargs))
         app.create(tools_list, **kwargs)
         return app
 
     elif app_type == 'victorinox':
         from chatgpt_tool_hub.apps.victorinox import Victorinox
 
-        for tool in default_tools_list:
-            if tool not in tools_list:
-                tools_list.append(tool)
+        for default_tool in default_tools_list:
+            if default_tool not in tools_list:
+                tools_list.append(default_tool)
 
-        app = Victorinox(**get_app_kwargs(kwargs))
+        app = Victorinox(**build_model_params(kwargs))
         app.create(tools_list, **kwargs)
         return app
 
     else:
         raise NotImplementedError
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/apps/victorinox.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/apps/victorinox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 from chatgpt_tool_hub.apps.app import App
 from chatgpt_tool_hub.apps.load_app import load_app
 from chatgpt_tool_hub.bots.initialize import initialize_bot
 from chatgpt_tool_hub.common.constants import MEMORY_MAX_TOKENS_NUM
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.database import ConversationTokenBufferMemory
-from chatgpt_tool_hub.models.chatgpt import ChatOpenAI
+from chatgpt_tool_hub.models.model_factory import ModelFactory
 from chatgpt_tool_hub.tools.load_tools import load_tools
 
 
 class Victorinox(App):
     def __init__(self, **app_kwargs):
         super().__init__()
         if not self.init_flag:
-
-            self.llm = ChatOpenAI(temperature=0, **app_kwargs)
+            self.llm = ModelFactory().create_llm_model(**app_kwargs)
 
             self.memory = ConversationTokenBufferMemory(llm=self.llm, memory_key="chat_history",
                                                         output_key='output', max_token_limit=MEMORY_MAX_TOKENS_NUM)
             self.init_flag = True
 
     def create(self, tools_list: list, **tools_kwargs):
         if tools_list is None:
             tools_list = []
         if not self._check_mandatory_tools(tools_list):
             raise ValueError("check mandatory tools failed")
         if self.tools or self.tools_kwargs:
             LOG.warning("refresh the config of tools")
 
-        [self.tools.add(tool) for tool in tools_list]
+        map(self.tools.add, tools_list)
         self.tools_kwargs = tools_kwargs
 
         try:
-            tools = load_tools(tools_list, llm=self.llm, **tools_kwargs)
+            tools = load_tools(tools_list, **tools_kwargs)
         except ValueError as e:
             LOG.error(str(e))
-            return "load_tools failed"
+            raise RuntimeError("tool初始化失败")
 
         # loading tools from config.
         LOG.info(f"Initializing {self.get_class_name()} success, "
                  f"use_tools={tools_list}, params: {str(tools_kwargs)}")
 
         # create bots
         self.bot = initialize_bot(tools, self.llm, bot="chat-bot", verbose=True,
@@ -46,36 +45,36 @@
 
     def add_tool(self, tools_list: list, **tools_kwargs):
         """todo: I think there have better way to implement"""
         if not tools_list:
             LOG.info("no tool to add")
             return
 
-        [self.tools.add(tool) for tool in tools_list]
+        map(self.tools.add, tools_list)
         for tool_key in tools_kwargs:
             self.tools_kwargs[tool_key] = tools_kwargs[tool_key]
 
         try:
-            new_tools_list = load_tools(list(self.tools), llm=self.llm, **self.tools_kwargs)
+            new_tools_list = load_tools(list(self.tools), **self.tools_kwargs)
         except ValueError as e:
             LOG.error(str(e))
-            return "load_tools failed"
+            raise RuntimeError("tool初始化失败")
 
         # loading tools from config.
         LOG.info(f"add_tool {self.get_class_name()} success, "
                  f"use_tools={new_tools_list}, params: {str(self.tools_kwargs)}")
 
         # create bots
         self.bot = initialize_bot(new_tools_list, self.llm, bot="chat-bot", verbose=True,
                                   memory=self.memory, max_iterations=2, early_stopping_method="generate")
 
     def ask(self, query: str, chat_history: list = None, retry_num: int = 0) -> str:
         if self.bot is None:
             LOG.error("before calling the ask method, you should use create bot firstly")
-            raise RuntimeError("初始化失败")
+            raise RuntimeError("app初始化失败")
 
         if not query:
             LOG.warning("[APP]: query is zero value")
             raise ValueError("请求为空")
 
         # 更新session
         if chat_history is not None:
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/bot.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,16 +90,17 @@
             retry_num += 1
             if retry_num > self.max_parse_retry_num:
                 raise ValueError(f"Could not parse LLM output: `{parsed_output}`")
 
             full_output = self._fix_text(full_output)
             full_inputs["bot_scratchpad"] += full_output
             output = self.llm_chain.predict(**full_inputs)
-            full_output += output
-            parsed_output = self._extract_tool_and_input(full_output)
+            LOG.debug("(fix_text): retry response: " + str(output))
+            # full_output += output
+            parsed_output = self._extract_tool_and_input(output)
         return BotAction(
             tool=parsed_output[0], tool_input=parsed_output[1], log=full_output
         )
 
     def plan(
         self, intermediate_steps: List[Tuple[BotAction, str]], **kwargs: Any
     ) -> Union[BotAction, BotFinish]:
@@ -216,15 +217,16 @@
             for action, observation in intermediate_steps:
                 thoughts += action.log
                 thoughts += (
                     f"\n{self.observation_prefix}{observation}\n{self.llm_prefix}"
                 )
             # Adding to the previous steps, we now tell the LLM to make a final pred
             thoughts += (
-                "\n\nI now need to return a final answer based on the previous steps:"
+                "\n\nI have exceeded the limit of tool usage and "
+                "now need to summarize all the information collected so far to generate a final answer:"
             )
             new_inputs = {"bot_scratchpad": thoughts, "stop": self._stop}
             full_inputs = {**kwargs, **new_inputs}
             full_output = self.llm_chain.predict(**full_inputs)
             # We try to extract a final answer
             parsed_output = self._extract_tool_and_input(full_output)
             if parsed_output is None:
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/bot_executor.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/bot_executor.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/chat_bot/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,45 +15,54 @@
 
 
 class ChatBot(Bot):
     """An bot designed to hold a conversation in addition to using tools."""
 
     ai_prefix: str = "AI"
 
-    instruction_text: str = f"{ai_prefix}: the response to the original input question in chinese"
-
     @property
     def _bot_type(self) -> str:
         """Return Identifier of bot type."""
         return "chat-bot"
 
     @property
     def observation_prefix(self) -> str:
         """Prefix to append the observation with."""
         return "Observation: "
 
     def _fix_text(self, text: str) -> str:
-        return (f"Observation: You told me: {text}, but it doesn't meet the format I mentioned to you. "
-                f"Please try again: {self.instruction_text}")
+        if not self.allowed_tools:
+            tool_names = ""
+        else:
+            tool_names = ", ".join([tool for tool in self.allowed_tools])
+        instruction_text = FORMAT_INSTRUCTIONS.format(
+            tool_names=tool_names, ai_prefix=self.ai_prefix
+        )
+        _text = ("\n\n"
+                 f"You just told me: {text}, but it doesn't meet the format I mentioned to you. \n\n"
+                 f"format: {instruction_text}. \n\n"
+                 "You should understand why you did not input the correct format, correct it and try again. \n\n")
+        LOG.debug("(fix_text): fix_text: " + repr(_text))
+        return _text
 
     @property
     def llm_prefix(self) -> str:
         """Prefix to append the llm call with."""
         return "Thought:"
 
     @classmethod
     def create_prompt(
-        cls,
-        tools: Sequence[BaseTool],
-        prefix: str = PREFIX,
-        suffix: str = SUFFIX,
-        format_instructions: str = FORMAT_INSTRUCTIONS,
-        ai_prefix: str = "AI",
-        human_prefix: str = "Human",
-        input_variables: Optional[List[str]] = None,
+            cls,
+            tools: Sequence[BaseTool],
+            prefix: str = PREFIX,
+            suffix: str = SUFFIX,
+            format_instructions: str = FORMAT_INSTRUCTIONS,
+            ai_prefix: str = "AI",
+            human_prefix: str = "Human",
+            input_variables: Optional[List[str]] = None,
     ) -> PromptTemplate:
         """Create prompt in the style of the zero shot bot.
 
         Args:
             tools: List of tools the bot will have access to, used to format the
                 prompt.
             prefix: String to put before the list of tools.
@@ -66,56 +75,57 @@
             A PromptTemplate with the template assembled from the pieces here.
         """
         tool_strings = "\n".join(
             [f"> {tool.name}: {tool.description}" for tool in tools]
         )
         tool_names = ", ".join([tool.name for tool in tools])
 
-        cls.instruction_text = format_instructions.format(
-            tool_names=tool_names, ai_prefix=ai_prefix, human_prefix=human_prefix
+        instruction_text = format_instructions.format(
+            tool_names=tool_names, ai_prefix=ai_prefix
         )
-        template = "\n\n".join([prefix, tool_strings, cls.instruction_text, suffix])
+        template = "\n\n".join([prefix, tool_strings, instruction_text, suffix])
         if input_variables is None:
             input_variables = ["input", "chat_history", "bot_scratchpad"]
         prompt = PromptTemplate(template=template, input_variables=input_variables)
 
         LOG.debug("\nprompt: " + str(prompt) + "\n")
         return prompt
 
     @property
     def finish_tool_name(self) -> str:
         """Name of the tool to use to finish the chain."""
         return self.ai_prefix
 
     def _extract_tool_and_input(self, llm_output: str) -> Optional[Tuple[str, str]]:
+        # this is bad parsing rule
         if f"{self.ai_prefix}:" in llm_output:
             return self.ai_prefix, llm_output.split(f"{self.ai_prefix}:")[-1].strip()
         regex = r"Action: (.*?)[\n]*Action Input: (.*)"
         match = re.search(regex, llm_output, re.DOTALL)
         if not match:
             return None
 
         action = match.group(1)
         action_input = match.group(2)
         LOG.info(f"执行Tool: {action}中...")
         return action.strip(), action_input.strip(" ").strip('"')
 
     @classmethod
     def from_llm_and_tools(
-        cls,
-        llm: BaseLLM,
-        tools: Sequence[BaseTool],
-        callback_manager: Optional[BaseCallbackManager] = None,
-        prefix: str = PREFIX,
-        suffix: str = SUFFIX,
-        format_instructions: str = FORMAT_INSTRUCTIONS,
-        ai_prefix: str = "AI",
-        human_prefix: str = "Human",
-        input_variables: Optional[List[str]] = None,
-        **kwargs: Any,
+            cls,
+            llm: BaseLLM,
+            tools: Sequence[BaseTool],
+            callback_manager: Optional[BaseCallbackManager] = None,
+            prefix: str = PREFIX,
+            suffix: str = SUFFIX,
+            format_instructions: str = FORMAT_INSTRUCTIONS,
+            ai_prefix: str = "AI",
+            human_prefix: str = "Human",
+            input_variables: Optional[List[str]] = None,
+            **kwargs: Any,
     ) -> Bot:
         """Construct an bot from an LLM and tools."""
         prompt = cls.create_prompt(
             tools,
             ai_prefix=ai_prefix,
             human_prefix=human_prefix,
             prefix=prefix,
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/chat_bot/prompt.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/chat_bot/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 PREFIX = """You are a helpful assistant.
 
-TOOLS:
-------
+Assistant has access to the following tools:
 
-Assistant has access to the following tools:"""
+TOOLS:
+------"""
 
-FORMAT_INSTRUCTIONS = """To use a tool, please use the following format:
+FORMAT_INSTRUCTIONS = """To use a tool, you MUST use the following format:
 ```
 Thought: Do I need to use a tool? Yes
 Action: the action to take, should be one of [{tool_names}]
 Action Input: the input to the action
 Observation: the result of the action
 ```
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/initialize.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/initialize.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/qa_bot/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/bots/qa_bot/prompt.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/bots/qa_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/api/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pydantic import BaseModel, Field, root_validator
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.chains.api.prompt import API_RESPONSE_PROMPT, API_URL_PROMPT
 from chatgpt_tool_hub.chains.base import Chain
 from chatgpt_tool_hub.chains.llm import LLMChain
 from chatgpt_tool_hub.common.schema import BaseLanguageModel
 from chatgpt_tool_hub.prompts import BasePromptTemplate
-from chatgpt_tool_hub.tools.web_requests.wrapper import RequestsWrapper
+from chatgpt_tool_hub.tools.web_requests import RequestsWrapper
 
 
 class APIChain(Chain, BaseModel):
     """Chain that makes API calls and summarizes the responses to answer a question."""
 
     api_request_chain: LLMChain
     api_answer_chain: LLMChain
@@ -73,14 +73,15 @@
         api_response = self.requests_wrapper.get(api_url)
         LOG.debug("[API] response: " + str(api_response))
         self.callback_manager.on_text(
             api_response, color="yellow", end="\n", verbose=self.verbose
         )
         # api_docs chunking
         self.api_docs = "Here represents the API documentation that you previously used to generate API url."
+
         answer = self.api_answer_chain.predict(
             question=question,
             api_docs=self.api_docs,
             api_url=api_url,
             api_response=api_response,
         )
         return {self.output_key: answer}
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/api/prompt.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/api/prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from chatgpt_tool_hub.prompts.prompt import PromptTemplate
 
-API_URL_PROMPT_TEMPLATE = """You are given the below API Documentation: {api_docs} Using this documentation, 
-generate the full API url to call for answering the user question. You should build the API url in order to get a 
-response that is as short as possible, while still getting the necessary information to answer the question. Pay 
-attention to deliberately exclude any unnecessary pieces of data in the API call.
+API_URL_PROMPT_TEMPLATE = """You are given the below API Documentation: {api_docs} 
+Using this documentation, generate the full API url to call for answering the user question. 
+You should build the API url in order to get a response that is as short as possible, 
+while still getting the necessary information to answer the question. 
+Pay attention to deliberately exclude any unnecessary pieces of data in the API call.
 
 Question:{question}
 API url:"""
 
 API_URL_PROMPT = PromptTemplate(
     input_variables=[
         "api_docs",
@@ -21,16 +22,20 @@
     API_URL_PROMPT_TEMPLATE
     + """ {api_url}
 
 Here is the response from the API:
 
 {api_response}
 
-Summarize this response to answer the original question.
+You can answer my question step by step according to api response.
 
-Summary:"""
+You should provide feedback on whether the question can be answered, 
+explain what you have done, what you have seen and what the outcome was to the Human. 
+Don't make up you response!
+
+Your final answer:"""
 )
 
 API_RESPONSE_PROMPT = PromptTemplate(
     input_variables=["api_docs", "question", "api_url", "api_response"],
     template=API_RESPONSE_PROMPT_TEMPLATE,
 )
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/chains/llm.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/chains/llm.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/cache.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/cache.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/calculate_token.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/calculate_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from chatgpt_tool_hub.common.log import LOG
 
 
 # refer to https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
 def num_tokens_from_messages(messages, model: str = "gpt-3.5-turbo"):
     """Returns the number of tokens used by a list of messages."""
     import tiktoken
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/callbacks.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/document.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/document.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/formatting.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/formatting.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/input.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/input.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/schema.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/schema.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/singleton.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/singleton.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/text_splitter.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/common/utils.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/common/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Generic utility functions."""
 import os
 from typing import Any, Dict, Optional
 
 
 def get_from_dict_or_env(
-    data: Dict[str, Any], key: str, env_key: str, default: Optional[str] = None
-) -> str:
+        data: Dict[str, Any], key: str, env_key: str, default: Optional[Any] = None
+) -> Any:
     """Get a value from a dictionary or an environment variable."""
     if key in data and data[key]:
         return data[key]
     elif env_key in os.environ and os.environ[env_key]:
         return os.environ[env_key]
     elif default is not None:
         return default
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/chat_memory.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/chat_memory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/token_buffer.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/token_buffer.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/database/utils.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/database/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/chatgpt/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/chatgpt/chatgpt.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/models/openai.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/models/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
 from chatgpt_tool_hub.common.schema import Generation, LLMResult
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
-from chatgpt_tool_hub.models.base import BaseLLM
+from chatgpt_tool_hub.models import BaseLLM
 from chatgpt_tool_hub.common.log import LOG
 
 
 def update_token_usage(
     keys: Set[str], response: Dict[str, Any], token_usage: Dict[str, Any]
 ) -> None:
     """Update token usage."""
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/__init__.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/chat.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/prompts/prompt.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/base_tool.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/bing_search/wrapper.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Util that calls Bing Search."""
+import json
 from typing import Dict, List
 
-import json
-import requests
 from pydantic import BaseModel, Extra, root_validator
-from chatgpt_tool_hub.tools.web_requests.wrapper import RequestsWrapper
+
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.tools.web_requests import filter_text
+from chatgpt_tool_hub.tools.web_requests.wrapper import RequestsWrapper
 
 
 class BingSearchAPIWrapper(BaseModel):
     """Wrapper for Bing Search API."""
 
     bing_subscription_key: str
     bing_search_url: str
-    k: int = 2
+    top_k_results: int = 2
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
 
     def _bing_search_results(self, search_term: str, count: int) -> List[dict]:
@@ -40,34 +40,36 @@
             result = []
             LOG.error("[bing_search] " + repr(e))
         return result
 
     @root_validator(pre=True)
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and endpoint exists in environment."""
-        bing_subscription_key = get_from_dict_or_env(
+
+        values["bing_subscription_key"] = get_from_dict_or_env(
             values, "bing_subscription_key", "BING_SUBSCRIPTION_KEY"
         )
-        values["bing_subscription_key"] = bing_subscription_key
 
-        bing_search_url = get_from_dict_or_env(
+        values["bing_search_url"] = get_from_dict_or_env(
             values,
             "bing_search_url",
             "BING_SEARCH_URL",
             default="https://api.bing.microsoft.com/v7.0/search",
         )
 
-        values["bing_search_url"] = bing_search_url
+        values["top_k_results"] = get_from_dict_or_env(
+            values, 'top_k_results', "TOP_K_RESULTS", 2
+        )
 
         return values
 
     def run(self, query: str) -> str:
         """Run query through BingSearch and parse result."""
         snippets = []
-        results = self._bing_search_results(query, count=self.k)
+        results = self._bing_search_results(query, count=self.top_k_results)
         if len(results) == 0:
             return "No good Bing Search Result was found"
 
         for result in results:
             snippets.append(filter_text(result["snippet"]))
 
         return " ".join(snippets)
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/debug/debug.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/debug/debug.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import Callable
 
 from pydantic import Field
 
+from chatgpt_tool_hub.tools.all_tool_list import register_tool
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
+default_tool_name = "debug"
+
 
 def _print_func(text: str) -> None:
     print("\n")
     print(text)
 
 
 class DebugTool(BaseTool):
     """Tool for asking for help."""
 
-    name = "Helper"
+    name = default_tool_name
     description = (
         "You can ask a helper for guidance when you think you "
         "got stuck or you are not sure what to do next. "
         "The input should be a question for the human in chinese."
     )
     prompt_func: Callable[[str], None] = Field(default_factory=lambda: _print_func)
     input_func: Callable = Field(default_factory=lambda: input)
@@ -26,7 +29,10 @@
         """Use the DebugTool tool."""
         self.prompt_func(query)
         return self.input_func()
 
     async def _arun(self, query: str) -> str:
         """Use the DebugTool asynchronously."""
         raise NotImplementedError("DebugTool does not support async")
+
+
+register_tool(default_tool_name, lambda _: DebugTool(), [])
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/google_search/google_search.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/bing_search/bing_search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,36 @@
-"""Tool for the Google search API."""
+"""Tool for the Bing search API."""
 
 from chatgpt_tool_hub.tools.base_tool import BaseTool
-from chatgpt_tool_hub.tools.google_search.wrapper import GoogleSearchAPIWrapper
+from chatgpt_tool_hub.tools.bing_search.wrapper import BingSearchAPIWrapper
+from chatgpt_tool_hub.tools.all_tool_list import register_tool
 
 
-class GoogleSearch(BaseTool):
-    """Tool that adds the capability to query the Google search API."""
+default_tool_name = "bing-search"
 
-    name = "Google Search"
+
+class BingSearch(BaseTool):
+    """Tool that adds the capability to query the Bing search API.
+
+    In order to set this up, follow instructions at:
+    https://levelup.gitconnected.com/api-tutorial-how-to-use-bing-web-search-api-in-python-4165d5592a7e
+    """
+
+    name = default_tool_name
     description = (
-        "A wrapper around Google Search. "
+        "A wrapper around Bing Search. "
         "Useful for when you need to answer questions about current events. "
         "Input should be a search query."
     )
-    api_wrapper: GoogleSearchAPIWrapper
+    api_wrapper: BingSearchAPIWrapper
 
     def _run(self, query: str) -> str:
         """Use the tool."""
         return self.api_wrapper.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
-        raise NotImplementedError("GoogleSearchRun does not support async")
-
+        raise NotImplementedError("BingSearch does not support async")
 
-class GoogleSearchJson(BaseTool):
-    """Tool that has capability to query the Google Search API and get back json."""
 
-    name = "Google Search Results JSON"
-    description = (
-        "A wrapper around Google Search. "
-        "Useful for when you need to answer questions about current events. "
-        "Input should be a search query. Output is a JSON array of the query results"
-    )
-    num_results: int = 2  # the search api return top-2 results
-    api_wrapper: GoogleSearchAPIWrapper
-
-    def _run(self, query: str) -> str:
-        """Use the tool."""
-        return str(self.api_wrapper.results(query, self.num_results))
-
-    async def _arun(self, query: str) -> str:
-        """Use the tool asynchronously."""
-        raise NotImplementedError("GoogleSearchRun does not support async")
+register_tool(default_tool_name, lambda kwargs: BingSearch(api_wrapper=BingSearchAPIWrapper(**kwargs)),
+              tool_input_keys=["bing_subscription_key"])
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/google_search/wrapper.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/google_search/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.tools.web_requests import filter_text
 
 class GoogleSearchAPIWrapper(BaseModel):
     """Wrapper for Google Search API."""
 
-    search_engine: Any  #: :meta private:
+    search_engine: Any
     google_api_key: Optional[str] = None
     google_cse_id: Optional[str] = None
-    k: int = 2
+    top_k_results: int = 2
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
 
     def _google_search_results(self, search_term: str, **kwargs: Any) -> List[dict]:
@@ -47,44 +47,48 @@
                 "google-api-python-client is not installed. "
                 "Please install it with `pip install google-api-python-client`"
             )
 
         service = build("customsearch", "v1", developerKey=google_api_key)
         values["search_engine"] = service
 
+        values["top_k_results"] = get_from_dict_or_env(
+            values, 'top_k_results', "TOP_K_RESULTS", 2
+        )
+
         return values
 
     def run(self, query: str) -> str:
         """(for normal result): Run query through GoogleSearch and parse result."""
         snippets = []
-        results = self._google_search_results(query, num=self.k)
+        results = self._google_search_results(query, num=self.top_k_results)
         if len(results) == 0:
             return "No good Google Search Result was found"
 
         for result in results:
             if "snippet" in result:
                 snippets.append(filter_text(result["snippet"]))
         LOG.debug("[GoogleSearch] output: " + str(snippets))
         return " ".join(snippets)
 
-    def results(self, query: str, num_results: int) -> List[Dict]:
+    def results(self, query: str) -> List[Dict]:
         """(for json result): Run query through GoogleSearch and return metadata.
 
         Args:
             query: The query to search for.
             num_results: The number of results to return.
 
         Returns:
             A list of dictionaries with the following keys:
                 snippet - The description of the result.
                 title - The title of the result.
                 link - The link to the result.
         """
         metadata_results = []
-        results = self._google_search_results(query, num=num_results)
+        results = self._google_search_results(query, num=self.top_k_results)
         if len(results) == 0:
             return [{"Result": "No good Google Search Result was found"}]
 
         for result in results:
             metadata_result = {
                 "title": result["title"],
                 "link": result["link"],
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/load_tools.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/load_tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,59 @@
 """Load tools."""
+from typing import Any, List
 from typing import Optional
 
 from chatgpt_tool_hub.common.callbacks import BaseCallbackManager
-from chatgpt_tool_hub.common.schema import BaseLanguageModel
-from chatgpt_tool_hub.tools.all_tool_list import *
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.tools.all_tool_list import get_all_tool_dict
+from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 
 def load_tools(
     tool_names: List[str],
-    llm: Optional[BaseLanguageModel] = None,
     callback_manager: Optional[BaseCallbackManager] = None,
     **kwargs: Any,
 ) -> List[BaseTool]:
     """Load tools based on their name.
 
     Args:
         tool_names: name of tools to load.
-        llm: Optional language model, may be needed to initialize certain tools.
         callback_manager: Optional callback manager. If not provided, default global callback manager will be used.
-
     Returns:
         List of tools.
     """
     tools = []
+    all_tool_dict = get_all_tool_dict()
     for name in tool_names:
-        if name in BASE_TOOLS:
-            tools.append(BASE_TOOLS[name]())
-        elif name in BOT_TOOLS:
-            if llm is None:
-                raise ValueError(f"Tool {name} requires an LLM to be provided")
-            tool = BOT_TOOLS[name](llm)
-            if callback_manager is not None:
-                tool.callback_manager = callback_manager
-            tools.append(tool)
-        elif name in BOT_WITH_KEY_TOOLS:
-            if llm is None:
-                raise ValueError(f"Tool {name} requires an LLM to be provided")
-            _get_llm_tool_func, extra_keys = BOT_WITH_KEY_TOOLS[name]
+        if name in all_tool_dict:
+            _get_tool_func, extra_keys = all_tool_dict[name]
+
+            # consistency validation between input and required params
             missing_keys = set(extra_keys).difference(kwargs)
             if missing_keys:
                 raise ValueError(
                     f"Tool {name} requires some parameters that were not "
                     f"provided: {missing_keys}"
                 )
-            sub_kwargs = {k: kwargs[k] for k in extra_keys}
-            tool = _get_llm_tool_func(llm=llm, **sub_kwargs)
 
-            if callback_manager is not None:
-                tool.callback_manager = callback_manager
-
-            tools.append(tool)
-        elif name in OPTIONAL_ADVANCED_TOOLS:
-            _get_tool_func, extra_keys = OPTIONAL_ADVANCED_TOOLS[name]
             sub_kwargs = {k: kwargs[k] for k in extra_keys if k in kwargs}
-            tool = _get_tool_func(**sub_kwargs)
-            if callback_manager is not None:
-                tool.callback_manager = callback_manager
-            tools.append(tool)
-        elif name in CUSTOM_TOOL:
-            _get_tool_func, extra_keys = CUSTOM_TOOL[name]
-            sub_kwargs = {k: kwargs[k] for k in extra_keys if k in kwargs}
-            tool = _get_tool_func(**sub_kwargs)
+            tool = _get_tool_func(sub_kwargs)
+
             if callback_manager is not None:
                 tool.callback_manager = callback_manager
+
             tools.append(tool)
         else:
-            LOG.error("现在支持的工具有："+str(get_all_tool_names()))
-            raise ValueError(f"Got unknown tool {name}")
+            LOG.error("All the tools currently supported are："+str(list(all_tool_dict)))
+            raise ValueError(f"Got unknown tool: {name}")
+    filter_tools = crop_tools(tools)
+    return filter_tools
+
+
+def crop_tools(tools: List[BaseTool]) -> List[BaseTool]:
+    if len(tools) > 8:
+        LOG.warning(f"get too many tools, tools after {tools[8].name} will be ignored...")
+        return tools[:8]
+    # todo: 检查description是否超出限制
+    for tool in tools:
+        pass
     return tools
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/meteo/api_docs_prompts.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/meteo/api_docs_prompts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 OPEN_METEO_DOCS = """BASE URL: https://api.open-meteo.com/
 
 API Documentation
 The API endpoint /v1/forecast accepts a geographical coordinate, a list of weather variables and responds with a JSON hourly weather forecast for 7 days. Time always starts at 0:00 today and contains 168 hours. All URL parameters are listed below:
 
 Parameter	Format	Required	Default	Description
 latitude, longitude	Floating point	Yes		Geographical WGS84 coordinate of the location
@@ -13,22 +12,51 @@
 windspeed_unit	String	No	kmh	Other wind speed speed units: ms, mph and kn
 precipitation_unit	String	No	mm	Other precipitation amount units: inch
 timeformat	String	No	iso8601	If format unixtime is selected, all time values are returned in UNIX epoch time in seconds. Please note that all timestamp are in GMT+0! For daily values with unix timestamps, please apply utc_offset_seconds again to get the correct date.
 timezone	String	No	GMT	If timezone is set, all timestamps are returned as local-time and data is returned starting at 00:00 local-time. Any time zone name from the time zone database is supported. If auto is set as a time zone, the coordinates will be automatically resolved to the local time zone.
 past_days	Integer (0-2)	No	0	If past_days is set, yesterday or the day before yesterday data are also returned.
 start_date & end_date	String (yyyy-mm-dd)	No		The time interval to get weather data. A day must be specified as an ISO8601 date (e.g. 2022-06-30).
 
-Hourly Parameter Definition
-The parameter &hourly= accepts the following values. Most weather variables are given as an instantaneous value for the indicated hour. Some variables like precipitation are calculated from the preceding hour as an average or sum.
+Hourly Parameter Definition:
+The parameter &hourly= accepts the following values; note that you cannot use Daily Parameter in &hourly=.
+Most weather variables are given as an instantaneous value for the indicated hour. 
+Some variables like precipitation are calculated from the preceding hour as an average or sum.
 
 Variable	Valid time	Unit	Description
 temperature_2m	Instant	°C (°F)	Air temperature at 2 meters above ground
+cloudcover	Instant	%	Total cloud cover as an area fraction
+precipitation	Preceding hour sum	mm (inch)	Total precipitation (rain, showers, snow) sum of the preceding hour
 snowfall	Preceding hour sum	cm (inch)	Snowfall amount of the preceding hour in centimeters. For the water equivalent in millimeter, divide by 7. E.g. 7 cm snow = 10 mm precipitation water equivalent
 rain	Preceding hour sum	mm (inch)	Rain from large scale weather systems of the preceding hour in millimeter
-showers	Preceding hour sum	mm (inch)	Showers from convective precipitation in millimeters from the preceding hour
-weathercode	Instant	WMO code	Weather condition as a numeric code. Follow WMO weather interpretation codes. See table below for details.
+weathercode	Instant	WMO code	Weather condition as a numeric code. Follow WMO weather interpretation codes.   
+windspeed_10m & windspeed_80m & windspeed_120m & windspeed_180m	Instant	km/h (mph, m/s, knots)	Wind speed at 10, 80, 120 or 180 meters above ground. Wind speed on 10 meters is the standard level.
 snow_depth	Instant	meters	Snow depth on the ground
-freezinglevel_height	Instant	meters	Altitude above sea level of the 0°C level
 visibility	Instant	meters	Viewing distance in meters. Influenced by low clouds, humidity and aerosols. Maximum visibility is approximately 24 km.
 
+Daily Parameter Definition:
+The parameter &daily= accepts the following values:
+Aggregations are a simple 24 hour aggregation from hourly values.  
+note that you cannot use Hourly Parameter in &daily=.
+
+Variable	Unit	Description
+temperature_2m_max & temperature_2m_min	°C (°F)	Maximum and minimum daily air temperature at 2 meters above ground
+precipitation_sum	mm	Sum of daily precipitation (including rain, showers and snowfall)
+rain_sum	mm	Sum of daily rain
+weathercode	WMO code	The most severe weather condition on a given day. Follow WMO weather interpretation codes. 
+sunrise & sunset	iso8601	Sun rise and set times
+windspeed_10m_max & windgusts_10m_max	km/h (mph, m/s, knots)	Maximum wind speed and gusts on a day
+winddirection_10m_dominant	°	Dominant wind direction
+
+
+WMO Weather interpretation codes (WW)
+Code	Description
+0	Clear sky
+1, 2, 3	Mainly clear, partly cloudy, and overcast
+45, 48	Fog and depositing rime fog
+51, 53, 55	Drizzle: Light, moderate, and dense intensity
+56, 57	Freezing Drizzle: Light and dense intensity
+
 If daily weather variables are specified, parameter timezone is required.
+Parameter past_days is mutually exclusive with start_date and end_date.
+
+Your output can only be a URL, no need for explanation.
 """
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/news/api_docs_prompts.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/news/api_docs_prompts.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/python/python_repl.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/python/python_repl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """A tool for running python code in a REPL."""
 
 import sys
 from io import StringIO
 from typing import Dict, Optional
 
 from pydantic import Field, BaseModel
+
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.tools.all_tool_list import register_tool
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 
 
+default_tool_name = "python"
+
+
 class PythonREPL(BaseModel):
     """Simulates a standalone Python REPL."""
 
     globals: Optional[Dict] = Field(default_factory=dict, alias="_globals")
     locals: Optional[Dict] = Field(default_factory=dict, alias="_locals")
 
     def run(self, command: str) -> str:
@@ -38,22 +43,25 @@
 def _get_default_python_repl() -> PythonREPL:
     return PythonREPL(_globals=globals(), _locals=None)
 
 
 class PythonREPLTool(BaseTool):
     """A tool for running python code in a REPL."""
 
-    name = "Python REPL"
+    name = default_tool_name
     description = (
         "A Python shell. Use this to execute python commands. "
         "Input should be a valid python command. "
         "If you want to see the output of a value, you should print it out with `print(...)`."
     )
     python_repl: PythonREPL = Field(default_factory=_get_default_python_repl)
 
     def _run(self, query: str) -> str:
         """Use the tool."""
         return self.python_repl.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("PythonReplTool does not support async")
+
+
+register_tool(default_tool_name, lambda _: PythonREPLTool(), [])
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/terminal/base.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/terminal/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import subprocess
 from typing import List, Union
 
 from pydantic import Field
 
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.tools.all_tool_list import register_tool
+
+
+default_tool_name = "terminal"
 
 
 class BashProcess:
     """Executes bash commands and returns the output."""
 
     def __init__(self, use_nsfc_filter: bool = True, return_err_output: bool = True, timeout: float = 20):
         # 是否过滤命令
@@ -26,19 +30,19 @@
         _commands = " ".join(commands)
 
         # filter punctuation
         for i in string.punctuation:
             _commands = _commands.replace(i, ' ')
 
         command_ban_set = {"halt", "poweroff", "shutdown", "reboot", "rm", "kill",
-                             "exit", "sudo", "su", "userdel", "groupdel", "logout", "alias"}
+                           "exit", "sudo", "su", "userdel", "groupdel", "logout", "alias"}
         _both_have = command_ban_set.intersection(set(_commands.split()))
         if len(_both_have) > 0:
             LOG.info("[terminal] nsfc_filter: unsupported command: " + repr(_both_have))
-            return False, "this command: " + repr(_both_have) + " is dangerous for you, you are not allow to use it"
+            return False, "this command: " + repr(_both_have) + " is dangerous for you, you are not allowed to use it"
         else:
             return True, "success"
 
     def reprocess(self, commands: str) -> str:
         # ```xxx
         # real commands is here
         # ```
@@ -69,15 +73,15 @@
                 commands,
                 shell=True,
                 check=True,  # raises a CalledProcessError when exit code is non-zero
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 timeout=self.timeout  # raises TimeoutExpired after running 20s
             ).stdout.decode()
-        except (subprocess.CalledProcessError, ) as error:
+        except subprocess.CalledProcessError as error:
             LOG.error("[Terminal] " + str(error))
             if self.return_err_output:
                 return error.stdout.decode()
             return "this tool can't run there commands"
         except subprocess.TimeoutExpired as error:
             LOG.error("[Terminal] " + str(error))
             return f"you input commands exceeds the time limit: `{self.timeout} seconds` " \
@@ -87,15 +91,15 @@
 
 
 def _get_default_bash_process() -> BashProcess:
     return BashProcess()
 
 
 class Terminal(BaseTool):
-    name = "Terminal"
+    name = default_tool_name
     description = (
         f"Executes commands in a terminal. Input should be valid commands in {sys.platform} platform, "
         "and the output will be any output from running that command."
         "Don't input any backquote to this tool."
     )
 
     bash_process: BashProcess = Field(default_factory=_get_default_bash_process)
@@ -105,11 +109,14 @@
         return self.bash_process.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the tool asynchronously."""
         raise NotImplementedError("[Terminal] does not support async")
 
 
+register_tool(default_tool_name, lambda _: Terminal(), [])
+
+
 if __name__ == "__main__":
     bash = BashProcess()
     content = bash.run("`poweroff; sudo ls -l; pwd`")
     print(content)
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/tool.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,19 @@
     """Tool that is run when invalid tool name is encountered by bot."""
 
     name = "invalid_tool"
     description = "Called when tool name is invalid."
 
     def _run(self, tool_name: str) -> str:
         """Use the tool."""
-        return f"{tool_name} is not a valid tool, try another one."
+        return f"`{tool_name}` is not a valid tool, try another one."
 
     async def _arun(self, tool_name: str) -> str:
         """Use the tool asynchronously."""
-        return f"{tool_name} is not a valid tool, try another one."
+        return f"`{tool_name}` is not a valid tool, try another one."
 
 
 def tool(*args: Union[str, Callable], return_direct: bool = False, **kwargs) -> Callable:
     """tool decorator
 
     Requires:
         - Function must be of type (str) -> str
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/__init__.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     # break into lines and remove leading and trailing space on each
     lines = (line.strip() for line in text.splitlines())
     # break multi-headlines into a line each
     chunks = (phrase.strip() for line in lines for phrase in line.split("  "))
     # drop blank lines
     text = '\n'.join(chunk for chunk in chunks if chunk)
     # compress text size
+    # todo gpt-index
     text = text[:500]
 
     return text.encode('utf-8').decode()
 
 
 def _parse_input(text: str) -> Dict[str, Any]:
     """Parse the json string into a dict."""
@@ -42,14 +43,15 @@
 
 class BaseRequestsTool(BaseModel):
     """Base class for requests tools."""
 
     requests_wrapper: RequestsWrapper
 
 
+from chatgpt_tool_hub.tools.web_requests.browser import BrowserTool
 from chatgpt_tool_hub.tools.web_requests.delete import RequestsDeleteTool
 from chatgpt_tool_hub.tools.web_requests.get import RequestsGetTool
 from chatgpt_tool_hub.tools.web_requests.patch import RequestsPatchTool
 from chatgpt_tool_hub.tools.web_requests.post import RequestsPostTool
 from chatgpt_tool_hub.tools.web_requests.put import RequestsPutTool
 
 __all__ = (
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/browser.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/browser.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/delete.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/delete.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/patch.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/patch.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/post.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/post.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/put.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/put.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/web_requests/wrapper.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/web_requests/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Lightweight wrapper around requests library, with async support."""
+import logging
 from typing import Any, Dict, Optional
 
 import aiohttp
 import requests
 from pydantic import BaseModel, Extra, root_validator
+from chatgpt_tool_hub.common.log import LOG
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
-
 from chatgpt_tool_hub.tools.web_requests import DEFAULT_HEADER
 
 
 class RequestsWrapper(BaseModel):
     """Lightweight wrapper around requests library."""
 
     headers: Optional[Dict[str, str]] = dict()
     aiosession: Optional[aiohttp.ClientSession] = None
 
-    browser: Any  # PhantomJSWebDriver or None
+    browser: Any = None  # PhantomJSWebDriver or None
     phantomjs_exec_path: Optional[str]  # download link: https://phantomjs.org/download.html
 
     proxy: Optional[str]
 
     class Config:
         """Configuration for this pydantic object."""
 
@@ -28,39 +29,38 @@
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that browser param exists in environment."""
         phantomjs_exec_path = get_from_dict_or_env(
             values, "phantomjs_exec_path", "PHANTOMJS_EXEC_PATH", ""
         )
-        if not phantomjs_exec_path:
-            values["browser"] = None
-            return values
         proxy = get_from_dict_or_env(
             values, 'proxy', "PROXY", ""
         )
+
+        if not phantomjs_exec_path:
+            values["browser"] = None
+            return values
+
         try:
             from selenium import webdriver
 
             values["browser"] = cls._build_browser_option(phantomjs_exec_path, proxy)
         except ImportError:
             raise ImportError(
                 "selenium is not installed. "
                 "Please install it with `pip install selenium==2.48.0`"
             )
-
-
         return values
 
     @classmethod
     def _build_browser_option(self, exec_path: str, proxy: str = ""):
         from selenium import webdriver
 
         from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
-        from selenium.webdriver.common.proxy import ProxyType
 
         dcap = dict(DesiredCapabilities.PHANTOMJS)
 
         # 设置user-agent请求头
         dcap["phantomjs.page.settings.userAgent"] = DEFAULT_HEADER.get('User-Agent', '')
         # 禁止加载图片
         dcap["phantomjs.page.settings.loadImages"] = False
@@ -76,26 +76,31 @@
             # 将代理设置添加到webdriver.DesiredCapabilities.PHANTOMJS中
             _proxy.add_to_capabilities(webdriver.DesiredCapabilities.PHANTOMJS)
 
         browser.start_session(webdriver.DesiredCapabilities.PHANTOMJS)
 
         return browser
 
-    def get(self, url: str, params: Dict[str, Any] = None, raise_for_status: bool = False) -> str:
+    def get(self, url: str, params: Dict[str, Any] = None, raise_for_status: bool = False, **kwargs) -> str:
         """GET the URL and return the text."""
         if self.browser:
             self.browser.get(url)
             _content = self.browser.page_source
+            # todo raise_for_status?
             self.browser.close()  # 退出当前页面, 节省内存
             return _content
         else:
             self.headers.update(DEFAULT_HEADER)
-            response = requests.get(url, headers=self.headers, params=params)
+            response = requests.get(url, headers=self.headers, params=params, **kwargs)
             if raise_for_status:
-                response.raise_for_status()
+                try:
+                    response.raise_for_status()
+                except Exception as e:
+                    LOG.error("RequestsWrapper.get status_code is not good: " + repr(e))
+
             return response.text
 
     def post(self, url: str, data: Dict[str, Any]) -> str:
         """POST to the URL and return the text."""
         self.headers = dict().update(DEFAULT_HEADER) if not self.headers else self.headers.update(DEFAULT_HEADER)
         return requests.post(url, data=data, headers=self.headers).text
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wikipedia/wikipedia.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wikipedia.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """Tool for the Wikipedia API."""
 
 from chatgpt_tool_hub.tools.base_tool import BaseTool
 from chatgpt_tool_hub.tools.wikipedia.wrapper import WikipediaAPIWrapper
+from chatgpt_tool_hub.tools.all_tool_list import register_tool
 
 
+default_tool_name = "wikipedia"
+
 class WikipediaTool(BaseTool):
     """Tool that adds the capability to search using the Wikipedia API."""
 
-    name = "Wikipedia"
+    name = default_tool_name
     description = (
         "Useful for when you need to answer general questions about "
         "people, places, companies, historical events, or other subjects. "
         "Input should be a search query."
     )
     api_wrapper: WikipediaAPIWrapper
 
     def _run(self, query: str) -> str:
         """Use the Wikipedia tool."""
         return self.api_wrapper.run(query)
 
     async def _arun(self, query: str) -> str:
         """Use the Wikipedia tool asynchronously."""
         raise NotImplementedError("WikipediaQueryRun does not support async")
+
+
+register_tool(default_tool_name, lambda kwargs: WikipediaTool(api_wrapper=WikipediaAPIWrapper(**kwargs)), [])
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wikipedia/wrapper.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wikipedia/wrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Util that calls Wikipedia."""
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, Extra, root_validator
 
 from chatgpt_tool_hub.common.log import LOG
+from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 
 
 class WikipediaAPIWrapper(BaseModel):
     """Wrapper around WikipediaAPI.
 
     To use, you should have the ``wikipedia`` python package installed.
     This wrapper will use the Wikipedia API to conduct searches and
@@ -16,25 +17,27 @@
     """
 
     wiki_client: Any  #: :meta private:
     top_k_results: int = 2
 
     class Config:
         """Configuration for this pydantic object."""
-
         extra = Extra.forbid
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that the python package exists in environment."""
         try:
             import wikipedia
-
+            # 本土化
             wikipedia.set_lang("zh")
 
+            values["top_k_results"] = get_from_dict_or_env(
+                values, 'top_k_results', "TOP_K_RESULTS", 2
+            )
             values["wiki_client"] = wikipedia
         except ImportError:
             raise ValueError(
                 "Could not import wikipedia python package. "
                 "Please it install it with `pip install wikipedia`."
             )
         return values
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/PKG-INFO` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.3.7
+Version: 0.3.9
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -58,37 +58,87 @@
 
 - 支持中文输入输出
 - 支持上下文记忆
 - 支持proxy
 - 支持多种工具： 
   - terminal
   - python
-  - requests
+  - url-get
   - wikipedia
   - meteo-weather
   - news
+  - morning-news
   - bing-search
   - wolfram-alpha
 
 
 ## 快速开始
 
 ---
+### 1.  使用shell运行demo
+
+#### (1). 克隆源代码
+
+```bash
+git clone git@github.com:goldfishh/chatgpt-tool-hub.git
+```
+
+#### (2). `pip install -r requirements.txt`
+
+#### (3). 编辑config.json，填入你的openai_api_key
+
+```json
+{
+  "tools": [],  // 这里填入你想加载的工具名，默认工具无需填入自动加载
+  "kwargs": {
+      "openai_api_key": "",  // 必填
+      "proxy": "",  // 代理配置，国外ip可忽略
+      "debug": false,  // 当你遇到问题提issue前请设置debug为true，提交输出日志
+      "no_default": false,  // 控制是否加载默认工具
+      "model_name": "gpt-3.5-turbo"  // 默认，其他模型暂未测试
+  }
+}
+```
+
+#### (4). `python3 run.py 你的问题1 [你的问题2 ......]`
+
+> chatgpt判断回复是否使用工具，你可要求chatgpt使用工具（更进一步地使用哪个工具）来帮助它更好回答你的问题
+
+#### (5). 给项目点个star & 有能力pr，支持项目作者继续开发...
+
+--- 
+
+### 2. 去[chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat)使用本项目开发的tool插件：[tool README](https://github.com/goldfishh/chatgpt-on-wechat/blob/master/plugins/tool/README.md)
+
+> 你可以在微信用到本项目为chatgpt提供的工具能力
+
+---
+
+### 3. 你是其他项目开发者，想要接入本工具引擎
+
+#### (1). 安装chatgpt-tool-hub包
+
+`pip install -i https://pypi.python.org/simple chatgpt-tool-hub`
+
+#### (2). 示例代码：
 
-`pip install chatgpt-tool-hub`
 ```python
 import os
 from chatgpt_tool_hub.apps import load_app
 os.environ["OPENAI_API_KEY"] = YOUR_OPENAI_API_KEY
 os.environ["PROXY"] = "http://192.168.7.1:7890"
 app = load_app()
 reply = app.ask(YOUR_QUESTION_TO_HERE)
 print(reply)
 ```
-PS: 默认加载：python、requests、terminal、meteo-weather工具
+  
+> 如果有需求，我会更新接入的文档，欢迎提issue
+
+---
+
 ## 工具指南
 
 ---
 
 > 工具名末尾加*表示使用该工具需要额外申请服务key, 超出免费额度需给服务提供商**支付费用** 
 
 #### 1. terminal
@@ -105,15 +155,15 @@
 python解释器，使用它来解释执行python指令，可以配合你想要ChatGPT生成的代码输出结果或执行事务
 
 ```text
 1. 使用python查询今天日期    
 2. eval this expression: hex(123456)-123    
 ```
 
-#### 3. requests
+#### 3. url-get
 
 往往用来获取某个网站具体内容，结果可能会被反爬策略影响
 
 ```
 1. 总结信息 https://github.com/goldfishh/chatgpt-tool-hub    
 2. 可以作为信息入口配合其他工具   
 ```
@@ -167,15 +217,15 @@
 
 工具引擎的实现原理本质是**Chain-of-Thought**：[Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)
   
 我将通过用6个自问自答的问题解释chatgpt-tool-hub的工作原理  
 
 #### 1. 事务型工具（如terminal、python）是在哪运行，以及如何执行的
 
-事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、requests工具分别用到了封装调用subprocess库、python解释器和request库的函数
+事务型工具是在你本地运行的，事务型工具本质是一个python编写的函数，terminal、python、url-get工具分别用到了封装调用subprocess库、python解释器和requests库的函数
 
 --- 
 
 #### 2. ChatGPT是如何触发调用这些函数
 
 借助ChatGPT api提供的temperature参数，该参数越低，ChatGPT输出的结果会更集中和确定，当temperature为0时，相同的问题会得到统一回答  
 我在prompt构建时会提供给ChatGPT此时用到的工具列表信息，每个工具信息包含：工具名 和 工具描述：
@@ -183,15 +233,15 @@
 ```text
 TOOLS:  
 ------  
   
 You have access to the following tools:  
 
 > Python REPL: A Python shell. Use this to execute python commands. 
-> requests_get: A portal to the internet. Use this when you need to get specific content from a website. 
+> url-get: A portal to the internet. Use this when you need to get specific content from a website. 
 > Terminal: Executes commands in a terminal. 
 > Bing Search: A wrapper around Bing Search. Useful for when you need to answer questions about current events. 
 ```
 
 有了工具prompt，这时ChatGPT就能理解这些工具名字和使用场景，调用事务函数还需要进一步细化我和ChatGPT之间的通信协议（仍是通过prompt）：
 通信协议限制ChatGPT使用工具时返回内容的格式，只能返回三种前缀的内容：
 
@@ -203,15 +253,15 @@
 
 通信协议完整prompt：  
 ```text
 To use a tool, please use the following format:
 
 
 Thought: Do I need to use a tool? Yes
-Action: the action to take, should be one of [Python REPL, requests_get, Terminal, Bing Search]
+Action: the action to take, should be one of [Python REPL, url-get, Terminal, Bing Search]
 Action Input: the input to the action
 Observation: the result of the action
 ```
 
 此时，工具引擎有专用的文本解析模块负责解析这些内容，当解析成功后，将调度到具体事务函数执行，然后返回固定前缀的结果：
 
 ```text
@@ -299,15 +349,15 @@
 [○] 粒度配置  
 [○] 语音输入  
 [✗] 一个前端demo   
   
 ### tool todolist  
    
 [○] stable-diffusion 中文prompt翻译    
-[○] ImageCaptioning   
+[✓] ImageCaptioning   
 [○] 小米智能家居控制   
 [○] 支持ChatGPT官方插件  
 [○] 支持图片处理工具   
 [○] 支持视频处理工具  
 [✗] Wechat  
 
 ## Q&A
```

### Comparing `chatgpt-tool-hub-0.3.7/chatgpt_tool_hub.egg-info/SOURCES.txt` & `chatgpt-tool-hub-0.3.9/chatgpt_tool_hub.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 README.md
 setup.py
 chatgpt_tool_hub/__init__.py
-chatgpt_tool_hub/run.py
 chatgpt_tool_hub/version.py
 chatgpt_tool_hub.egg-info/PKG-INFO
 chatgpt_tool_hub.egg-info/SOURCES.txt
 chatgpt_tool_hub.egg-info/dependency_links.txt
 chatgpt_tool_hub.egg-info/requires.txt
 chatgpt_tool_hub.egg-info/top_level.txt
 chatgpt_tool_hub/apps/__init__.py
 chatgpt_tool_hub/apps/all_app_list.py
 chatgpt_tool_hub/apps/app.py
+chatgpt_tool_hub/apps/app_factory.py
 chatgpt_tool_hub/apps/lite_app.py
 chatgpt_tool_hub/apps/load_app.py
 chatgpt_tool_hub/apps/victorinox.py
 chatgpt_tool_hub/bots/__init__.py
 chatgpt_tool_hub/bots/all_bot_list.py
 chatgpt_tool_hub/bots/bot.py
 chatgpt_tool_hub/bots/bot_executor.py
@@ -32,15 +32,14 @@
 chatgpt_tool_hub/chains/api/__init__.py
 chatgpt_tool_hub/chains/api/base.py
 chatgpt_tool_hub/chains/api/prompt.py
 chatgpt_tool_hub/common/__init__.py
 chatgpt_tool_hub/common/cache.py
 chatgpt_tool_hub/common/calculate_token.py
 chatgpt_tool_hub/common/callbacks.py
-chatgpt_tool_hub/common/config.py
 chatgpt_tool_hub/common/constants.py
 chatgpt_tool_hub/common/document.py
 chatgpt_tool_hub/common/formatting.py
 chatgpt_tool_hub/common/input.py
 chatgpt_tool_hub/common/log.py
 chatgpt_tool_hub/common/schema.py
 chatgpt_tool_hub/common/singleton.py
@@ -48,45 +47,57 @@
 chatgpt_tool_hub/common/utils.py
 chatgpt_tool_hub/database/__init__.py
 chatgpt_tool_hub/database/chat_memory.py
 chatgpt_tool_hub/database/token_buffer.py
 chatgpt_tool_hub/database/utils.py
 chatgpt_tool_hub/models/__init__.py
 chatgpt_tool_hub/models/base.py
+chatgpt_tool_hub/models/model_factory.py
 chatgpt_tool_hub/models/openai.py
 chatgpt_tool_hub/models/chatgpt/__init__.py
 chatgpt_tool_hub/models/chatgpt/base.py
 chatgpt_tool_hub/models/chatgpt/chatgpt.py
 chatgpt_tool_hub/prompts/__init__.py
 chatgpt_tool_hub/prompts/base.py
 chatgpt_tool_hub/prompts/chat.py
 chatgpt_tool_hub/prompts/prompt.py
 chatgpt_tool_hub/tools/__init__.py
 chatgpt_tool_hub/tools/all_tool_list.py
 chatgpt_tool_hub/tools/base_tool.py
 chatgpt_tool_hub/tools/load_tools.py
 chatgpt_tool_hub/tools/tool.py
+chatgpt_tool_hub/tools/arxiv_search/__init__.py
+chatgpt_tool_hub/tools/arxiv_search/arxiv_search.py
+chatgpt_tool_hub/tools/arxiv_search/wrapper.py
 chatgpt_tool_hub/tools/bing_search/__init__.py
 chatgpt_tool_hub/tools/bing_search/bing_search.py
 chatgpt_tool_hub/tools/bing_search/wrapper.py
 chatgpt_tool_hub/tools/debug/__init__.py
 chatgpt_tool_hub/tools/debug/debug.py
 chatgpt_tool_hub/tools/google_search/__init__.py
 chatgpt_tool_hub/tools/google_search/google_search.py
 chatgpt_tool_hub/tools/google_search/wrapper.py
 chatgpt_tool_hub/tools/meteo/__init__.py
 chatgpt_tool_hub/tools/meteo/api_docs_prompts.py
 chatgpt_tool_hub/tools/meteo/meteo_weather.py
+chatgpt_tool_hub/tools/morning_news/__init__.py
+chatgpt_tool_hub/tools/morning_news/morning_news.py
+chatgpt_tool_hub/tools/morning_news/summary_prompt.py
 chatgpt_tool_hub/tools/news/__init__.py
 chatgpt_tool_hub/tools/news/api_docs_prompts.py
 chatgpt_tool_hub/tools/news/news.py
 chatgpt_tool_hub/tools/python/__init__.py
 chatgpt_tool_hub/tools/python/python_repl.py
+chatgpt_tool_hub/tools/searxng_search/__init__.py
+chatgpt_tool_hub/tools/searxng_search/searxng.py
+chatgpt_tool_hub/tools/searxng_search/wrapper.py
 chatgpt_tool_hub/tools/terminal/__init__.py
 chatgpt_tool_hub/tools/terminal/base.py
+chatgpt_tool_hub/tools/visual_dl/__init__.py
+chatgpt_tool_hub/tools/visual_dl/text2image.py
 chatgpt_tool_hub/tools/web_requests/__init__.py
 chatgpt_tool_hub/tools/web_requests/browser.py
 chatgpt_tool_hub/tools/web_requests/delete.py
 chatgpt_tool_hub/tools/web_requests/get.py
 chatgpt_tool_hub/tools/web_requests/patch.py
 chatgpt_tool_hub/tools/web_requests/post.py
 chatgpt_tool_hub/tools/web_requests/put.py
```

### Comparing `chatgpt-tool-hub-0.3.7/setup.py` & `chatgpt-tool-hub-0.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,26 +27,27 @@
     author="goldfishh",
     author_email="goldfish.buaa@gmail.com",
     license="MIT",
     packages=setuptools.find_packages(exclude=["*.dev", "*.dev.*", "dev.*", "*.custom_tools", "*.custom_tools.*", "custom_tools.*"]),
     include_package_data=True,
     install_requires=[
         'pydantic~=1.10.7',
-        'aiohttp~=3.8.4',
-        'requests~=2.28.2',
-        'pyyaml',
+        'pyopenssl',
+        'pyyaml~=6.0',
         'beautifulsoup4~=4.12.0',
         "tenacity~=8.2.2",
         "openai~=0.27.2",
-        "SQLAlchemy~=2.0.7",
         "tiktoken~=0.3.2",
-        "google-api-python-client",
-        'pyopenssl',
+        "arxiv",
         "wikipedia",
-        "wolframalpha"
+        "wolframalpha",
+        'aiohttp~=3.8.4',
+        'requests~=2.28.2',
+        "google-api-python-client",
+        "SQLAlchemy~=2.0.7",
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

