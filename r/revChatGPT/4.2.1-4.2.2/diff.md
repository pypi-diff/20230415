# Comparing `tmp/revChatGPT-4.2.1.tar.gz` & `tmp/revChatGPT-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.2.1.tar", last modified: Fri Apr 14 00:34:15 2023, max compression
+gzip compressed data, was "revChatGPT-4.2.2.tar", last modified: Sat Apr 15 14:30:15 2023, max compression
```

## Comparing `revChatGPT-4.2.1.tar` & `revChatGPT-4.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    47003 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23144 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-14 00:33:45.000000 revChatGPT-4.2.1/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:34:15.635102 revChatGPT-4.2.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 00:34:15.000000 revChatGPT-4.2.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.692614 revChatGPT-4.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    47274 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.2.1/LICENSE` & `revChatGPT-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.1/PKG-INFO` & `revChatGPT-4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.1
+Version: 4.2.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-4.2.1/README.md` & `revChatGPT-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.1/setup.py` & `revChatGPT-4.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.2.1",
+    version="4.2.2",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.2.1/src/revChatGPT/V1.py` & `revChatGPT-4.2.2/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 import logging
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
-from typing import NoReturn, Generator, AsyncGenerator
+from typing import AsyncGenerator
+from typing import Generator
+from typing import NoReturn
 
-import requests, httpx
+import httpx
+import requests
 from httpx import AsyncClient
 from OpenAIAuth import Authenticator
 from OpenAIAuth import Error as AuthError
 
+from . import __version__
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
 from .utils import get_input
 
 if __name__ == "__main__":
     logging.basicConfig(
@@ -118,24 +122,25 @@
                 Path(user_home, ".config").mkdir()
             if not Path(user_home, ".config", "revChatGPT").exists():
                 Path(user_home, ".config", "revChatGPT").mkdir()
             self.cache_path = Path(user_home, ".config", "revChatGPT", "cache.json")
 
         self.config = config
         self.session = session_client() if session_client else requests.Session()
-        try:
-            cached_access_token = self.__get_cached_access_token(
-                self.config.get("email", None),
-            )
-        except t.Error as error:
-            if error.code == 5:
-                raise
-            cached_access_token = None
-        if cached_access_token is not None:
-            self.config["access_token"] = cached_access_token
+        if "email" in config and "password" in config:
+            try:
+                cached_access_token = self.__get_cached_access_token(
+                    self.config.get("email", None),
+                )
+            except t.Error as error:
+                if error.code == 5:
+                    raise
+                cached_access_token = None
+            if cached_access_token is not None:
+                self.config["access_token"] = cached_access_token
 
         if "proxy" in config:
             if not isinstance(config["proxy"], str):
                 error = TypeError("Proxy must be a string!")
                 raise error
             proxies = {
                 "http": config["proxy"],
@@ -519,15 +524,17 @@
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
         }
 
         yield from self.__send_request(
-            data, timeout=timeout, auto_continue=auto_continue
+            data,
+            timeout=timeout,
+            auto_continue=auto_continue,
         )
 
     @logger(is_timed=True)
     def ask(
         self,
         prompt: str,
         conversation_id: str | None = None,
@@ -651,15 +658,17 @@
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
         }
 
         yield from self.__send_request(
-            data, timeout=timeout, auto_continue=auto_continue
+            data,
+            timeout=timeout,
+            auto_continue=auto_continue,
         )
 
     @logger(is_timed=False)
     def __check_fields(self, data: dict) -> bool:
         try:
             data["message"]["content"]
         except (TypeError, KeyError):
@@ -674,21 +683,21 @@
             response (_type_): _description_
 
         Raises:
             Error: _description_
         """
         try:
             response.raise_for_status()
-        except requests.exceptions.HTTPError:
+        except requests.exceptions.HTTPError as e:
             error = t.Error(
                 source="OpenAI",
                 message=response.text,
                 code=response.status_code,
             )
-            raise error
+            raise error from e
 
     @logger(is_timed=True)
     def get_conversations(
         self,
         offset: int = 0,
         limit: int = 20,
         encoding: str | None = None,
@@ -818,15 +827,18 @@
             conversation_id=conversation_id,
             parent_id=parent_id,
             session_client=AsyncClient,
             base_url=base_url,
         )
 
     async def __send_request(
-        self, data: dict, auto_continue: bool = False, timeout: float = 360
+        self,
+        data: dict,
+        auto_continue: bool = False,
+        timeout: float = 360,
     ) -> AsyncGenerator[dict, None]:
         cid, pid = data["conversation_id"], data["parent_message_id"]
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         message = ""
 
@@ -1157,22 +1169,22 @@
             return False
         return True
 
     async def __check_response(self, response: httpx.Response) -> None:
         # 改成自带的错误处理
         try:
             response.raise_for_status()
-        except httpx.HTTPStatusError:
+        except httpx.HTTPStatusError as e:
             await response.aread()
             error = t.Error(
                 source="OpenAI",
                 message=response.text,
                 code=response.status_code,
             )
-            raise error
+            raise error from e
 
 
 get_input = logger(is_timed=False)(get_input)
 
 
 @logger(is_timed=False)
 def configure() -> dict:
@@ -1298,18 +1310,18 @@
     except Exception as exc:
         error = t.CLIError("command line program unknown error")
         raise error from exc
 
 
 if __name__ == "__main__":
     print(
-        """
+        f"""
         ChatGPT - A command-line interface to OpenAI's ChatGPT (https://chat.openai.com/chat)
         Repo: github.com/acheong08/ChatGPT
-        Version: 4.2.0
+        Version: {__version__}
         """,
     )
     print("Type '!help' to show a full list of commands")
     print(
         f"{bcolors.BOLD}{bcolors.WARNING}Press Esc followed by Enter or Alt+Enter to send a message.{bcolors.ENDC}",
     )
     main(configure())
```

### Comparing `revChatGPT-4.2.1/src/revChatGPT/V3.py` & `revChatGPT-4.2.2/src/revChatGPT/V3.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import AsyncGenerator
 from typing import NoReturn
 
 import httpx
 import requests
 import tiktoken
 
+from . import __version__
 from . import typings as t
 from .utils import create_completer
 from .utils import create_keybindings
 from .utils import create_session
 from .utils import get_filtered_keys_from_object
 from .utils import get_input
 
@@ -508,17 +509,18 @@
 
 
 def main() -> NoReturn:
     """
     Main function
     """
     print(
-        """
+        f"""
     ChatGPT - Official ChatGPT API
     Repo: github.com/acheong08/ChatGPT
+    Version: {__version__}
     """,
     )
     print("Type '!help' to show a full list of commands")
     print("Press Esc followed by Enter or Alt+Enter to send a message.\n")
 
     # Get API key from command line
     parser = argparse.ArgumentParser()
```

### Comparing `revChatGPT-4.2.1/src/revChatGPT/__init__.py` & `revChatGPT-4.2.2/src/revChatGPT/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The __init__ file does not a main file
 
 You can import the following module to use:
 revChatGPT.V0
 revChatGPT.V1
 revChatGPT.V3
 """
+__version__ = "4.2.1"
 __all__ = ()
 
 # Available Python Version Verify
 from . import typings as t
 from platform import python_version_tuple
 from platform import python_version
 from warnings import warn
```

### Comparing `revChatGPT-4.2.1/src/revChatGPT/__main__.py` & `revChatGPT-4.2.2/src/revChatGPT/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Main CLI
 """
 import argparse
 import sys
 
+from . import __version__
 from . import typings as t
 from . import V1
 from . import V3
 
 __all__ = ()
 
 
@@ -31,17 +32,18 @@
         help="Use the API version of ChatGPT",
     )
     args, _ = parser.parse_known_args()
     mode = "V1" if args.V1 else "V3" if args.V3 else input("Version (V1/V3):")
 
     if mode == "V1":
         print(
-            """
+            f"""
         ChatGPT - A command-line interface to OpenAI's ChatGPT (https://chat.openai.com/chat)
         Repo: github.com/acheong08/ChatGPT
+        Version: {__version__}
         """,
         )
         print("Type '!help' to show a full list of commands")
         print(
             f"{V1.bcolors.BOLD}{V1.bcolors.WARNING}Press Esc followed by Enter or Alt+Enter to send a message.{V1.bcolors.ENDC}",
         )
         V1.main(V1.configure())
```

### Comparing `revChatGPT-4.2.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.2.2/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.1/src/revChatGPT/typings.py` & `revChatGPT-4.2.2/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.1/src/revChatGPT/utils.py` & `revChatGPT-4.2.2/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.2.2/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.1
+Version: 4.2.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

