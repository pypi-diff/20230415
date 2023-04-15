# Comparing `tmp/cgpt-1.1.26.tar.gz` & `tmp/cgpt-1.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpt-1.1.26.tar", last modified: Wed Apr 12 19:02:35 2023, max compression
+gzip compressed data, was "cgpt-1.1.29.tar", last modified: Sat Apr 15 17:48:41 2023, max compression
```

## Comparing `cgpt-1.1.26.tar` & `cgpt-1.1.29.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.1.26/LICENSE
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.1.26/MANIFEST.in
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1603 2023-04-12 19:02:35.472151 cgpt-1.1.26/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1684 2023-03-30 12:25:43.000000 cgpt-1.1.26/README.md
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.468151 cgpt-1.1.26/app/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.1.26/app/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2455 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/base.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/app/client/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.26/app/client/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1300 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/client/main.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      499 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/file_service.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      406 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/main.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1319 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/plugin.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/app/server/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.26/app/server/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1186 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/server/main.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/app/utils/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.26/app/utils/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2137 2023-04-12 12:18:25.000000 cgpt-1.1.26/app/utils/constant.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      137 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/utils/verify_env.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/cgpt.egg-info/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1603 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      442 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       34 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/entry_points.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       51 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/requires.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/top_level.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1010 2023-04-12 12:16:38.000000 cgpt-1.1.26/cgpt.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-04-12 19:02:35.472151 cgpt-1.1.26/setup.cfg
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      995 2023-04-12 12:16:38.000000 cgpt-1.1.26/setup.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.886386 cgpt-1.1.29/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.1.29/LICENSE
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.1.29/MANIFEST.in
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1964 2023-04-15 17:48:41.886386 cgpt-1.1.29/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1825 2023-04-15 17:47:31.000000 cgpt-1.1.29/README.md
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.1.29/app/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     3552 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/base.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/client/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.29/app/client/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1419 2023-04-14 13:20:28.000000 cgpt-1.1.29/app/client/main.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/commands/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-14 13:55:23.000000 cgpt-1.1.29/app/commands/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      110 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/commands/main.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      572 2023-04-14 13:20:28.000000 cgpt-1.1.29/app/file_service.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      406 2023-04-12 19:52:50.000000 cgpt-1.1.29/app/main.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1432 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/plugin.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.882386 cgpt-1.1.29/app/server/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.29/app/server/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1282 2023-04-14 13:20:28.000000 cgpt-1.1.29/app/server/main.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.886386 cgpt-1.1.29/app/utils/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.29/app/utils/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2740 2023-04-15 17:02:26.000000 cgpt-1.1.29/app/utils/constant.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      137 2023-04-12 19:52:50.000000 cgpt-1.1.29/app/utils/verify_env.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-15 17:48:41.886386 cgpt-1.1.29/cgpt.egg-info/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1964 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      488 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       77 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/entry_points.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       68 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/requires.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-04-15 17:48:41.000000 cgpt-1.1.29/cgpt.egg-info/top_level.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      984 2023-04-15 17:02:26.000000 cgpt-1.1.29/cgpt.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-04-15 17:48:41.886386 cgpt-1.1.29/setup.cfg
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1133 2023-04-15 17:02:26.000000 cgpt-1.1.29/setup.py
```

### Comparing `cgpt-1.1.26/LICENSE` & `cgpt-1.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpt-1.1.26/PKG-INFO` & `cgpt-1.1.29/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,59 @@
-Metadata-Version: 2.1
-Name: cgpt
-Version: 1.1.26
-Summary: Use openai chat-gpt on your cli
-Home-page: https://github.com/ainayves/cgpt>
-Author: Aina Yves
-Author-email: randrianaina.yves@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+![python](https://img.shields.io/badge/Python-3.7-blue.svg)
+![commit activity](https://img.shields.io/github/commit-activity/m/ainayves/cgpt?color=blue)
+[![Build Status](https://img.shields.io/badge/Build%20status-Passing-green)](https://github.com/ainayves/cgpt/actions)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
 
-## Use openai chat-gpt on your CLI
+<center><h1>🌟 MAKE AI POWERED SEARCH INSIDE YOUR CLI 🌟</h1></center>
+</br>
+
+![cgpt1 1 28 (1)](https://user-images.githubusercontent.com/66997516/232239452-27e5c840-5699-44b8-bb28-da8d2dabc64f.gif)
+
+</br>
+
 `cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
 
-### REQUIREMENTS
+### ❓ REQUIREMENTS
 
 - python >=3.7
 - openai API KEY : 
-
 You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
 
-### SETUP
+### 💻 SETUP
+
+```
+pip install -r requirements.txt
+```
+
+### 🔨 BUILD
+
+- For this part , it is better to use Linux.
+
+If you are on Linux , launch:
 
 ```
-pip install cgpt
+sudo chmod +x build.sh
 ```
-### 😌 VERIFY IF IT IS CORRECTLY INSTALLED
+Then , :
 
 ```
-cgpt hello
+./build.sh
 ```
 
 ### ⏯️ GET VERSION 
 
 ```
-cgpt version
+cgpt-version
 ```
 
 ### 🚀 RUN
 
 ```
-cgpt tellme
+cgpt
 ```
 
 ### 🔗 CGPT INSIDE A LOCAL NETWORK
 
 You can use cgpt inside a LAN. 
 
 - You just need one Host (`connected to internet`) to be the server.
@@ -63,10 +68,10 @@
 ```
 127.0.0.1	localhost
 127.0.1.1	your-hostanme
 ```
 
 - A `client` can also use his own api_key in the next version.
 
-### GITHUB
+### 💚 Feedback
 
-- [cgpt](https://github.com/ainayves/cgpt/)
+Please feel free to leave feedback in issues/PRs.
```

### Comparing `cgpt-1.1.26/app/base.py` & `cgpt-1.1.29/app/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,24 @@
-from typing import Union, List, Dict
+from typing import List, Dict
 import click, socket
 from app.file_service import file_prompt
 from app.plugin import davinci
-from app.utils.constant import init_conversation, ASSISTANT
+from app.utils.constant import (
+    init_conversation,
+    ASSISTANT,
+    MAX_WIDTH,
+    color,
+    top_left,
+    bottom_left,
+    IA,
+    stick,
+    BLANK,
+    assistant_color,
+)
+from termcolor import colored
 
 
 class Base_CGPT:
 
     """
     Baseclass to create a conversational infinite-loop with CGPT module
     """
@@ -61,15 +73,17 @@
             res = davinci(client_input, previous_conv)
 
         return res
 
     def infinite_loop(self) -> None:
         while True:
             self._void_func()
-            client = input(self.input_text)
+            click.echo(BLANK)
+            client = input(colored(self.input_text, assistant_color))
+            click.echo(BLANK)
             if client == self.exit_key:
                 break
 
             elif client == self.modify_api_key:
                 file_prompt()
                 break
 
@@ -79,11 +93,40 @@
                 client_input=client,
                 socket=self.socket_instance,
             )
             init_conversation.append({"role": ASSISTANT, "content": resp})
             if resp is None:
                 break
 
-            click.echo(self.decoration, color=True)
-            click.echo(f"<< {self.icon_ans} >> {resp}")
-            click.echo("\n")
-            click.echo(self.decoration, color=True)
+            result = resp
+            len_res = len(result)
+            emoji_str = IA.encode("utf-8").decode("utf-8") if IA != "IA" else "IA"
+
+            if len(result) > MAX_WIDTH - 4:
+                len_res = MAX_WIDTH - 4
+            else:
+                len_res = len(result)
+
+            wrapped_result = [result]
+
+            box = (
+                colored(top_left, color)
+                + colored("─", color) * (len_res + 2)
+                + " "
+                + emoji_str
+                + "\n"
+            )
+            box += colored(stick, color) + " " * (len_res + 2) + "\n"
+
+            for line in wrapped_result:
+                box += (
+                    colored(stick, color)
+                    + " "
+                    + colored(line)
+                    + " " * (MAX_WIDTH - len(line) - 3)
+                    + "\n"
+                )
+
+            box += colored(stick, color) + " " * (len_res + 2) + "\n"
+            box += colored(bottom_left, color) + colored("─", color) * (len_res + 2)
+
+            click.echo(box)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cgpt-1.1.26/app/client/main.py` & `cgpt-1.1.29/app/client/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 
 import ipaddress
 import socket, click
+from termcolor import colored
 from app.utils.constant import (
     UTF,
     IA,
     SAY_SOMETHING,
     ENTER_SERVER_IP,
     CONNECTION_ERROR,
     CONNECTION_IMPOSSIBLE,
     DASHED,
     PORT,
     ADDRESS_NOT_VALID,
+    error_color,
 )
 
 from app.utils.verify_env import _check_env_file
 from app.base import Base_CGPT
 
 
 def main():
-    adresse_ip = click.prompt(ENTER_SERVER_IP)
+    adresse_ip = click.prompt(colored(ENTER_SERVER_IP, error_color))
 
     try:
         ipaddress.IPv4Address(adresse_ip)
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             s.connect((adresse_ip, int(PORT)))
             Base_CGPT._void_func = _check_env_file
@@ -39,17 +41,17 @@
                 socket_instance=s,
             )
 
             cgpt.infinite_loop()
 
         except OSError as e:
             if e.errno == 113:
-                click.echo(CONNECTION_IMPOSSIBLE)
+                click.echo(colored(CONNECTION_IMPOSSIBLE, error_color))
             else:
-                click.echo(CONNECTION_ERROR, e)
+                click.echo(colored(f"{CONNECTION_ERROR} {e}", error_color))
 
         finally:
             s.close()
 
     except ipaddress.AddressValueError:
         click.echo(ADDRESS_NOT_VALID)
```

### Comparing `cgpt-1.1.26/app/plugin.py` & `cgpt-1.1.29/app/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import os, click
+from termcolor import colored
 from typing import Union, List, Dict
 import openai
 from app.file_service import file_prompt
 from dotenv import load_dotenv
 
 load_dotenv()
 from app.utils.constant import (
@@ -15,14 +16,15 @@
     INCORRECT_API_KEY,
     MESSAGE,
     CONTENT,
     OPENAI_REQUEST_TIMEOUT,
     NOT_CONNECTED,
     TOO_MUCH_REQUEST,
     USER,
+    error_color,
 )
 
 openai.api_key = os.getenv(STR_OPENAI_API_KEY)
 
 
 def davinci(what: str, previous_conv: List[Dict]) -> Union[str, None]:
     try:
@@ -40,19 +42,19 @@
             file_prompt()
             res = None
 
         else:
             res = None
 
     except openai.error.Timeout:
-        click.echo(OPENAI_REQUEST_TIMEOUT)
+        click.echo(colored(OPENAI_REQUEST_TIMEOUT, error_color))
         res = None
 
     except openai.error.APIConnectionError:
-        click.echo(NOT_CONNECTED)
+        click.echo(colored(NOT_CONNECTED, error_color))
         res = None
 
     except openai.error.RateLimitError:
-        click.echo(TOO_MUCH_REQUEST)
+        click.echo(colored(TOO_MUCH_REQUEST, error_color))
         res = None
 
     return res
```

### Comparing `cgpt-1.1.26/app/server/main.py` & `cgpt-1.1.29/app/server/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*-
 
 import socket, click
 from _thread import *
 import threading
+from termcolor import colored
 
 print_lock = threading.Lock()
 from app.plugin import davinci
 from app.utils.constant import (
     PORT,
     SERVER_LIVE,
     UTF,
     LIVE,
     DECONNECTED_HOST,
     init_conversation,
+    error_color,
+    color,
 )
 
 
 def threaded(c):
     init_conversation_client = init_conversation
     while True:
         try:
@@ -28,22 +31,22 @@
             else:
                 continue
 
         except BrokenPipeError:
             continue
 
         except ConnectionResetError:
-            click.echo(DECONNECTED_HOST)
+            click.echo(colored(DECONNECTED_HOST, error_color))
 
 
 def main():
     adresse_ip = socket.gethostbyname(socket.gethostname())
     server_socket = socket.create_server((adresse_ip, int(PORT)), reuse_port=False)
     server_socket.listen()
-    click.echo(f"{SERVER_LIVE} {adresse_ip} ..{LIVE}")
+    click.echo(colored(f"{SERVER_LIVE} {adresse_ip} ..{LIVE}", color))
     while True:
         client, _ = server_socket.accept()
         threading.Thread(target=threaded, args=(client,), daemon=True).start()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cgpt-1.1.26/cgpt.egg-info/PKG-INFO` & `cgpt-1.1.29/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 Metadata-Version: 2.1
 Name: cgpt
-Version: 1.1.26
+Version: 1.1.29
 Summary: Use openai chat-gpt on your cli
 Home-page: https://github.com/ainayves/cgpt>
 Author: Aina Yves
 Author-email: randrianaina.yves@gmail.com
 License: MIT
+Description: ![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
+        
+        ## Use openai chat-gpt on your CLI
+        `cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
+        
+        ### REQUIREMENTS
+        
+        - python >=3.7
+        - openai API KEY : 
+        
+        You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
+        
+        ### SETUP
+        
+        ```
+        pip install cgpt
+        ```
+        
+        ### ⏯️ GET VERSION 
+        
+        ```
+        cgpt-version
+        ```
+        
+        ### 🚀 RUN
+        
+        ```
+        cgpt
+        ```
+        
+        ### 🔗 CGPT INSIDE A LOCAL NETWORK
+        
+        You can use cgpt inside a LAN. 
+        
+        - You just need one Host (`connected to internet`) to be the server.
+        - Other Hosts (`not connected to internet`) can ALWAYS use Chat GPT as `client`. 
+        
+        NOTES : 
+        
+        - For now , a server must be launched inside a `Linux` computer . If the server is inside `Windows` : the address is sometimes wrong (to be fixed in the next version). 
+        
+        - Also , make sure that your `/etc/hosts` is configured correctly like :
+        
+        ```
+        127.0.0.1	localhost
+        127.0.1.1	your-hostanme
+        ```
+        
+        - A `client` can also use his own api_key in the next version.
+        
+        ### GITHUB
+        
+        - [cgpt](https://github.com/ainayves/cgpt/)
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
-
-## Use openai chat-gpt on your CLI
-`cgpt` is a Python module that allows you to use Chat-GPT directly in your favorite Terminal.
-
-### REQUIREMENTS
-
-- python >=3.7
-- openai API KEY : 
-
-You need to register on openai to receive your own api key , here : [api_key](https://platform.openai.com/account/api-keys).
-
-### SETUP
-
-```
-pip install cgpt
-```
-### 😌 VERIFY IF IT IS CORRECTLY INSTALLED
-
-```
-cgpt hello
-```
-
-### ⏯️ GET VERSION 
-
-```
-cgpt version
-```
-
-### 🚀 RUN
-
-```
-cgpt tellme
-```
-
-### 🔗 CGPT INSIDE A LOCAL NETWORK
-
-You can use cgpt inside a LAN. 
-
-- You just need one Host (`connected to internet`) to be the server.
-- Other Hosts (`not connected to internet`) can ALWAYS use Chat GPT as `client`. 
-
-NOTES : 
-
-- For now , a server must be launched inside a `Linux` computer . If the server is inside `Windows` : the address is sometimes wrong (to be fixed in the next version). 
-
-- Also , make sure that your `/etc/hosts` is configured correctly like :
-
-```
-127.0.0.1	localhost
-127.0.1.1	your-hostanme
-```
-
-- A `client` can also use his own api_key in the next version.
-
-### GITHUB
-
-- [cgpt](https://github.com/ainayves/cgpt/)
```

### Comparing `cgpt-1.1.26/setup.py` & `cgpt-1.1.29/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,19 +16,26 @@
     author_email="randrianaina.yves@gmail.com",
     license="MIT",
     description="Use openai chat-gpt on your cli",
     long_description=long_desc,
     url="https://github.com/ainayves/cgpt>",
     long_description_content_type="text/markdown",
     py_modules=["cgpt", "app"],
-    packages=["app", "app.client", "app.server", "app.utils"],
-    install_requires=["setuptools", "twine", "click>=7.1.2", "openai", "python-dotenv"],
+    packages=["app", "app.client", "app.server", "app.utils", "app.commands"],
+    install_requires=[
+        "setuptools",
+        "twine",
+        "click>=7.1.2",
+        "openai",
+        "python-dotenv",
+        "termcolor",
+        "pytest",
+    ],
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
-    entry_points="""
-        [console_scripts]
-        cgpt=cgpt:cli
-    """,
+    entry_points={
+        "console_scripts": ["cgpt=cgpt:cgpt", "cgpt-version=app.commands.main:version"]
+    },
 )
```

