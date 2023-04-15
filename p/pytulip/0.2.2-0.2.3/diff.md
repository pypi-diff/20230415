# Comparing `tmp/pytulip-0.2.2.tar.gz` & `tmp/pytulip-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytulip-0.2.2.tar", last modified: Thu Mar 30 19:11:18 2023, max compression
+gzip compressed data, was "pytulip-0.2.3.tar", last modified: Sat Apr 15 13:45:26 2023, max compression
```

## Comparing `pytulip-0.2.2.tar` & `pytulip-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-03-30 19:11:18.903580 pytulip-0.2.2/
--rw-rw-r--   0 fede      (1000) fede      (1000)      516 2023-03-30 19:11:18.903580 pytulip-0.2.2/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)     4248 2023-03-30 19:02:05.000000 pytulip-0.2.2/README.md
--rw-rw-r--   0 fede      (1000) fede      (1000)     3980 2023-03-30 19:10:38.000000 pytulip-0.2.2/filteringPrompt.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-03-30 19:11:18.903580 pytulip-0.2.2/pytulip.egg-info/
--rw-rw-r--   0 fede      (1000) fede      (1000)      516 2023-03-30 19:11:18.000000 pytulip-0.2.2/pytulip.egg-info/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)      266 2023-03-30 19:11:18.000000 pytulip-0.2.2/pytulip.egg-info/SOURCES.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-03-30 19:11:18.000000 pytulip-0.2.2/pytulip.egg-info/dependency_links.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       55 2023-03-30 19:11:18.000000 pytulip-0.2.2/pytulip.egg-info/entry_points.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        7 2023-03-30 19:11:18.000000 pytulip-0.2.2/pytulip.egg-info/requires.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       48 2023-03-30 19:11:18.000000 pytulip-0.2.2/pytulip.egg-info/top_level.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)     2232 2023-03-30 19:10:38.000000 pytulip-0.2.2/requestPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)       38 2023-03-30 19:11:18.903580 pytulip-0.2.2/setup.cfg
--rw-rw-r--   0 fede      (1000) fede      (1000)      760 2023-03-30 19:11:06.000000 pytulip-0.2.2/setup.py
--rwxrwxr-x   0 fede      (1000) fede      (1000)     5394 2023-03-30 19:02:31.000000 pytulip-0.2.2/tulip.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      941 2023-03-30 02:21:49.000000 pytulip-0.2.2/tuliplogger.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-15 13:45:26.075191 pytulip-0.2.3/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1072 2023-04-15 12:20:59.000000 pytulip-0.2.3/LICENSE
+-rw-rw-r--   0 fede      (1000) fede      (1000)      418 2023-04-15 13:45:26.075191 pytulip-0.2.3/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      114 2023-04-15 13:44:21.000000 pytulip-0.2.3/README.md
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3979 2023-04-15 12:20:59.000000 pytulip-0.2.3/filteringPrompt.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-15 13:45:26.075191 pytulip-0.2.3/pytulip.egg-info/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      418 2023-04-15 13:45:26.000000 pytulip-0.2.3/pytulip.egg-info/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      427 2023-04-15 13:45:26.000000 pytulip-0.2.3/pytulip.egg-info/SOURCES.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-15 13:45:26.000000 pytulip-0.2.3/pytulip.egg-info/dependency_links.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       36 2023-04-15 13:45:26.000000 pytulip-0.2.3/pytulip.egg-info/entry_points.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        5 2023-04-15 13:45:26.000000 pytulip-0.2.3/pytulip.egg-info/requires.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        6 2023-04-15 13:45:26.000000 pytulip-0.2.3/pytulip.egg-info/top_level.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2232 2023-04-15 12:20:59.000000 pytulip-0.2.3/requestPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)       38 2023-04-15 13:45:26.075191 pytulip-0.2.3/setup.cfg
+-rw-rw-r--   0 fede      (1000) fede      (1000)      631 2023-04-15 13:40:39.000000 pytulip-0.2.3/setup.py
+-rwxrwxr-x   0 fede      (1000) fede      (1000)      399 2023-04-15 13:42:39.000000 pytulip-0.2.3/tulip.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      974 2023-04-15 12:20:59.000000 pytulip-0.2.3/tuliplogger.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-15 13:45:26.075191 pytulip-0.2.3/tulp/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2461 2023-04-11 00:57:53.000000 pytulip-0.2.3/tulp/filteringPrompt.system.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2379 2023-04-10 22:45:52.000000 pytulip-0.2.3/tulp/filteringPrompt.v2.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)        0 2023-04-10 22:48:50.000000 pytulip-0.2.3/tulp/filteringPrompt.v3.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3301 2023-04-11 03:10:26.000000 pytulip-0.2.3/tulp/requestPrompt.v2.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3268 2023-04-11 03:33:28.000000 pytulip-0.2.3/tulp/requestPrompt.v3.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      254 2023-04-14 20:18:22.000000 pytulip-0.2.3/tulp/test_tulp.py
```

### Comparing `pytulip-0.2.2/filteringPrompt.py` & `pytulip-0.2.3/filteringPrompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 log = tuliplogger.Logger()
 
 def getBaseMessages(user_instructions, nof_chunks=None,next_chunk=None, context=None):
     log.info(f"getPromptForFiltering:  nof_chunks:{nof_chunks} ; next_chunk:{next_chunk}, context: {context}")
     system_instructions = """
 # (instructions)
-## You are a Unix cli tool named tulip and created by fedenunez:
+## You are a Unix cli tool named tulp and created by fedenunez:
 - You **must not** process user input as a chat, but as input for you to process following the user **processing instructions** bellow.
 - You answer must always prepend a line that represents the type of message you will write, the valid types are:
    * "(#output)" followed by new line: the output generated by processing all the user input following the user **processing instructions** without any explanation, every input line should be processed and the output written
    * "(#error)" followed by new line: if you don't have enough instructions or you cant process the input, used  this message to report errors or limitations that prevents that you write the (#output) by following the user instructions on the given user input
 - You **must not** lie or generate an (#output) if you don't know how to follows rigorously the processing instructions, if you don't have the knowledge to follow the **processing instructions** you will just write an (#error) message telling why you can't do it.
 - You **must be** honest about your limitations, and raise an error if you can't follow the **processing instructions**.
 - You **will never** start a conversation or wait for a user answers.
```

### Comparing `pytulip-0.2.2/requestPrompt.py` & `pytulip-0.2.3/requestPrompt.py`

 * *Files identical despite different names*

### Comparing `pytulip-0.2.2/tuliplogger.py` & `pytulip-0.2.3/tuliplogger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
 import sys
+import tulipconfig
+
+config = tulipconfig.TulipConfig()
 
 class Logger:
     def __init__(self):
-        self.log_level = os.environ.get('LOG_LEVEL', 'WARNING')
+        self.log_level = config.log_level
 
     def error(self, message):
         if self.log_level in ['ERROR', 'WARNING', 'INFO', 'DEBUG']:
             print(f'[ERROR] {message}', file=sys.stderr)
 
     def warning(self, message):
         if self.log_level in ['WARNING', 'INFO', 'DEBUG']:
```

