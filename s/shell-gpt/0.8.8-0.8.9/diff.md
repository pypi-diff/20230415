# Comparing `tmp/shell_gpt-0.8.8.tar.gz` & `tmp/shell_gpt-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_gpt-0.8.8.tar", last modified: Mon Apr 10 15:05:44 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `shell_gpt-0.8.8.tar` & `shell_gpt-0.8.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.428330 shell_gpt-0.8.8/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.8/LICENSE
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    16334 2023-04-10 15:05:44.428164 shell_gpt-0.8.8/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    15986 2023-04-10 14:38:44.000000 shell_gpt-0.8.8/README.md
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-10 15:05:44.428375 shell_gpt-0.8.8/setup.cfg
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-10 14:38:44.000000 shell_gpt-0.8.8/setup.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.426005 shell_gpt-0.8.8/sgpt/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      451 2023-04-10 10:35:51.000000 shell_gpt-0.8.8/sgpt/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.8/sgpt/__main__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4674 2023-04-10 13:41:05.000000 shell_gpt-0.8.8/sgpt/app.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.8/sgpt/cache.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3069 2023-04-09 19:35:59.000000 shell_gpt-0.8.8/sgpt/client.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2857 2023-04-10 10:35:51.000000 shell_gpt-0.8.8/sgpt/config.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.427143 shell_gpt-0.8.8/sgpt/handlers/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.8/sgpt/handlers/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.8/sgpt/handlers/chat_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.8/sgpt/handlers/default_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1195 2023-04-10 10:35:51.000000 shell_gpt-0.8.8/sgpt/handlers/handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.8/sgpt/handlers/repl_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.8/sgpt/make_prompt.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1877 2023-04-09 19:35:59.000000 shell_gpt-0.8.8/sgpt/utils.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-10 15:05:44.427982 shell_gpt-0.8.8/shell_gpt.egg-info/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    16334 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/entry_points.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/requires.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-10 15:05:44.000000 shell_gpt-0.8.8/shell_gpt.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/LICENSE
+-rw-r--r--   0        0        0    15996 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/README.md
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/__main__.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/app.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/cache.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/client.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/config.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/make_prompt.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/__init__.py
+-rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/test_integration.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/test_unit.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/LICENSE
+-rw-r--r--   0        0        0    15996 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/README.md
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0    18024 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/PKG-INFO
```

### Comparing `shell_gpt-0.8.8/LICENSE` & `shell_gpt-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.8/PKG-INFO` & `shell_gpt-0.8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: shell_gpt
-Version: 0.8.8
-Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
-Home-page: https://github.com/ther1d/shell_gpt
-Author: Farkhod Sadykov
-Author-email: farkhod@sadykov.dev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shell GPT
 A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
-<div align="center">
-    <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
-</div>
+https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
 pip install shell-gpt==0.8.8
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
@@ -38,15 +26,15 @@
 ```shell
 sgpt "1 hour and 30 minutes to seconds"
 # -> 5,400 seconds
 ```
 ### Summarization and analyzing
 ShellGPT accepts prompt from both stdin and command line argument, you choose the most convenient input method for your preferences. Whether you prefer piping input through the terminal or specifying it directly as arguments, `sgpt` got you covered. This versatile feature is particularly useful when you need to pass file content or pipe output from other commands to the GPT models for summarization or analysis. For example, you can easily generate a git commit message based on a diff:
 ```shell
-git diff | sgpt "Generate git commit message, my changes"
+git diff | sgpt "Generate git commit message, for my changes"
 # -> Commit message: Implement Model enum and get_edited_prompt()
 ```
 You can analyze logs from various sources by passing them using stdin or command line arguments, along with a user-friendly prompt. This enables you to quickly identify errors and get suggestions for possible solutions:
 ```shell
 docker logs -n 20 container_name | sgpt "check logs, find errors, provide possible solutions"
 # ...
 ```
```

### Comparing `shell_gpt-0.8.8/README.md` & `shell_gpt-0.8.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,55 @@
+Metadata-Version: 2.1
+Name: shell_gpt
+Version: 0.8.9
+Summary: A command-line productivity tool powered by OpenAI GPT models, will help you accomplish your tasks faster and more efficiently.
+Project-URL: homepage, https://github.com/ther1d/shell_gpt
+Project-URL: repository, https://github.com/ther1d/shell_gpt
+Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
+Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: cheet-sheet,cli,gpt,openai,productivity,shell
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Requires-Python: >=3.6
+Requires-Dist: click<9.0.0,>=7.1.1
+Requires-Dist: distro<2.0.0,>=1.8.0
+Requires-Dist: pyreadline3<4.0.0,>=3.4.1; sys_platform == 'win32'
+Requires-Dist: requests<3.0.0,>=2.28.2
+Requires-Dist: rich<13.0.0,>=10.11.0
+Requires-Dist: typer<1.0.0,>=0.7.0
+Provides-Extra: dev
+Requires-Dist: pre-commit<4.0.0,>=3.1.1; extra == 'dev'
+Requires-Dist: ruff==0.0.256; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: black==23.1.0; extra == 'test'
+Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
+Requires-Dist: mypy==1.1.1; extra == 'test'
+Requires-Dist: pytest<8.0.0,>=7.2.2; extra == 'test'
+Requires-Dist: requests-mock[fixture]<2.0.0,>=1.10.0; extra == 'test'
+Requires-Dist: types-requests==2.28.11.17; extra == 'test'
+Description-Content-Type: text/markdown
+
 # Shell GPT
 A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
 
-<div align="center">
-    <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
-</div>
+https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
 pip install shell-gpt==0.8.8
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
@@ -28,15 +70,15 @@
 ```shell
 sgpt "1 hour and 30 minutes to seconds"
 # -> 5,400 seconds
 ```
 ### Summarization and analyzing
 ShellGPT accepts prompt from both stdin and command line argument, you choose the most convenient input method for your preferences. Whether you prefer piping input through the terminal or specifying it directly as arguments, `sgpt` got you covered. This versatile feature is particularly useful when you need to pass file content or pipe output from other commands to the GPT models for summarization or analysis. For example, you can easily generate a git commit message based on a diff:
 ```shell
-git diff | sgpt "Generate git commit message, my changes"
+git diff | sgpt "Generate git commit message, for my changes"
 # -> Commit message: Implement Model enum and get_edited_prompt()
 ```
 You can analyze logs from various sources by passing them using stdin or command line arguments, along with a user-friendly prompt. This enables you to quickly identify errors and get suggestions for possible solutions:
 ```shell
 docker logs -n 20 container_name | sgpt "check logs, find errors, provide possible solutions"
 # ...
 ```
```

### Comparing `shell_gpt-0.8.8/sgpt/app.py` & `shell_gpt-0.8.9/sgpt/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 as the command line interface. It supports different modes of output including
 shell commands and code, and allows users to specify the desired OpenAI model
 and length and other options of the output. Additionally, it supports executing
 shell commands directly from the interface.
 
 API Key is stored locally for easy use in future runs.
 """
-import sys
-
 # To allow users to use arrow keys in the REPL.
-import readline  # pylint: disable=unused-import
+import readline  # noqa: F401
+import sys
 
 import typer
 
 # Click is part of typer.
-from click import MissingParameter, BadArgumentUsage
-from sgpt import ChatHandler, DefaultHandler, ReplHandler, OpenAIClient, config
-from sgpt.utils import get_edited_prompt, run_command, ModelOptions
+from click import BadArgumentUsage, MissingParameter
+
+from sgpt import ChatHandler, DefaultHandler, OpenAIClient, ReplHandler, cfg
+from sgpt.utils import ModelOptions, get_edited_prompt, run_command
 
 
-def main(  # pylint: disable=too-many-arguments,too-many-locals
+def main(
     prompt: str = typer.Argument(
         None,
         show_default=False,
         help="The prompt to generate completions for.",
     ),
     model: ModelOptions = typer.Option(
-        ModelOptions(config.get("DEFAULT_MODEL")).value,
+        ModelOptions(cfg.get("DEFAULT_MODEL")).value,
         help="OpenAI GPT model to use.",
     ),
     temperature: float = typer.Option(
         0.1,
         min=0.0,
         max=1.0,
         help="Randomness of generated output.",
@@ -70,21 +70,21 @@
         rich_help_panel="Chat Options",
     ),
     repl: str = typer.Option(
         None,
         help="Start a REPL (Read–eval–print loop) session.",
         rich_help_panel="Chat Options",
     ),
-    show_chat: str = typer.Option(  # pylint: disable=W0613
+    show_chat: str = typer.Option(
         None,
         help="Show all messages from provided chat id.",
         callback=ChatHandler.show_messages_callback,
         rich_help_panel="Chat Options",
     ),
-    list_chat: bool = typer.Option(  # pylint: disable=W0613
+    list_chat: bool = typer.Option(
         False,
         help="List all existing chat ids.",
         callback=ChatHandler.list_ids,
         rich_help_panel="Chat Options",
     ),
 ) -> None:
     stdin_passed = not sys.stdin.isatty()
@@ -103,16 +103,16 @@
 
     if editor and stdin_passed:
         raise BadArgumentUsage("--editor option cannot be used with stdin input.")
 
     if editor:
         prompt = get_edited_prompt()
 
-    api_host = config.get("OPENAI_API_HOST")
-    api_key = config.get("OPENAI_API_KEY")
+    api_host = cfg.get("OPENAI_API_HOST")
+    api_key = cfg.get("OPENAI_API_KEY")
     client = OpenAIClient(api_host, api_key)
 
     if repl:
         # Will be in infinite loop here until user exits with Ctrl+C.
         ReplHandler(client, repl, shell, code).handle(
             prompt,
             model=model.value,
```

### Comparing `shell_gpt-0.8.8/sgpt/cache.py` & `shell_gpt-0.8.9/sgpt/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import json
 from hashlib import md5
 from pathlib import Path
-from typing import Callable
+from typing import Any, Callable, Generator, no_type_check
 
 
-class Cache:  # pylint: disable=too-few-public-methods
+class Cache:
     """
     Decorator class that adds caching functionality to a function.
     """
 
     def __init__(self, length: int, cache_path: Path) -> None:
         """
         Initialize the Cache decorator.
 
         :param length: Integer, maximum number of cache files to keep.
         """
         self.length = length
         self.cache_path = cache_path
         self.cache_path.mkdir(parents=True, exist_ok=True)
 
-    def __call__(self, func: Callable) -> Callable:
+    def __call__(self, func: Callable[..., Any]) -> Callable[..., Any]:
         """
         The Cache decorator.
 
         :param func: The function to cache.
         :return: Wrapped function with caching.
         """
 
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> Generator[str, None, None]:
             # Exclude self instance from hashing.
             cache_key = md5(json.dumps((args[1:], kwargs)).encode("utf-8")).hexdigest()
             cache_file = self.cache_path / cache_key
             # TODO: Fix caching for chat, should hash last user message, (not entire history).
             if kwargs.pop("caching", True) and cache_file.exists():
                 yield cache_file.read_text()
                 return
             result = ""
             for i in func(*args, **kwargs):
                 result += i
                 yield i
             cache_file.write_text(result)
-            self._delete_oldest_files(self.length)
+            self._delete_oldest_files(self.length)  # type: ignore
 
         return wrapper
 
+    @no_type_check
     def _delete_oldest_files(self, max_files: int) -> None:
         """
         Class method to delete the oldest cached files in the CACHE_DIR folder.
 
         :param max_files: Integer, the maximum number of files to keep in the CACHE_DIR folder.
         """
         # Get all files in the folder.
```

### Comparing `shell_gpt-0.8.8/sgpt/client.py` & `shell_gpt-0.8.9/sgpt/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import json
 from pathlib import Path
-from typing import List, Dict, Mapping
+from typing import Dict, Generator, List
 
 import requests
 
-from sgpt import config, Cache
+from sgpt import Cache, cfg
 
-
-# pylint: skip-file
-CACHE_LENGTH = int(config.get("CACHE_LENGTH"))
-CACHE_PATH = Path(config.get("CACHE_PATH"))
-REQUEST_TIMEOUT = int(config.get("REQUEST_TIMEOUT"))
+CACHE_LENGTH = int(cfg.get("CACHE_LENGTH"))
+CACHE_PATH = Path(cfg.get("CACHE_PATH"))
+REQUEST_TIMEOUT = int(cfg.get("REQUEST_TIMEOUT"))
 
 
 class OpenAIClient:
     cache = Cache(CACHE_LENGTH, CACHE_PATH)
 
     def __init__(self, api_host: str, api_key: str) -> None:
         self.api_key = api_key
         self.api_host = api_host
 
     @cache
     def _request(
         self,
-        messages: List[Mapping[str, str]],
+        messages: List[Dict[str, str]],
         model: str = "gpt-3.5-turbo",
         temperature: float = 1,
         top_probability: float = 1,
-    ) -> Dict:
+    ) -> Generator[str, None, None]:
         """
         Make request to OpenAI ChatGPT API, read more:
         https://platform.openai.com/docs/api-reference/chat
 
         :param messages: List of messages {"role": user or assistant, "content": message_string}
         :param model: String gpt-3.5-turbo or gpt-3.5-turbo-0301
         :param temperature: Float in 0.0 - 1.0 range.
@@ -54,32 +52,32 @@
             endpoint, headers=headers, json=data, timeout=REQUEST_TIMEOUT, stream=True
         )
         response.raise_for_status()
         # TODO: Optimise.
         # https://github.com/openai/openai-python/blob/237448dc072a2c062698da3f9f512fae38300c1c/openai/api_requestor.py#L98
         for line in response.iter_lines():
             data = line.lstrip(b"data: ").decode("utf-8")
-            if data == "[DONE]":
+            if data == "[DONE]":  # type: ignore
                 break
             if not data:
                 continue
-            data = json.loads(data)
-            delta = data["choices"][0]["delta"]
+            data = json.loads(data)  # type: ignore
+            delta = data["choices"][0]["delta"]  # type: ignore
             if "content" not in delta:
                 continue
             yield delta["content"]
 
     def get_completion(
         self,
-        messages: List[Mapping[str, str]],
+        messages: List[Dict[str, str]],
         model: str = "gpt-3.5-turbo",
         temperature: float = 1,
         top_probability: float = 1,
         caching: bool = True,
-    ) -> str:
+    ) -> Generator[str, None, None]:
         """
         Generates single completion for prompt (message).
 
         :param messages: List of dict with messages and roles.
         :param model: String gpt-3.5-turbo or gpt-3.5-turbo-0301.
         :param temperature: Float in 0.0 - 1.0 range.
         :param top_probability: Float in 0.0 - 1.0 range.
```

### Comparing `shell_gpt-0.8.8/sgpt/config.py` & `shell_gpt-0.8.9/sgpt/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
-from pathlib import Path
 from getpass import getpass
+from pathlib import Path
 from tempfile import gettempdir
-from typing import Any, Optional
+from typing import Any
 
 from click import UsageError
 
 from sgpt.utils import ModelOptions
 
 CONFIG_FOLDER = os.path.expanduser("~/.config")
 CONFIG_PATH = Path(CONFIG_FOLDER) / "shell_gpt" / ".sgptrc"
@@ -26,15 +26,15 @@
     "DEFAULT_MODEL": os.getenv("DEFAULT_MODEL", ModelOptions.GPT3.value),
     "OPENAI_API_HOST": os.getenv("OPENAI_API_HOST", "https://api.openai.com"),
     "DEFAULT_COLOR": os.getenv("DEFAULT_COLOR", "magenta"),
     # New features might add their own config variables here.
 }
 
 
-class Config(dict):
+class Config(dict):  # type: ignore
     def __init__(self, config_path: Path, **defaults: Any):
         self.config_path = config_path
 
         if self._exists:
             self._read()
             has_new_config = False
             for key, value in defaults.items():
@@ -52,29 +52,29 @@
             super().__init__(**defaults)
             self._write()
 
     @property
     def _exists(self) -> bool:
         return self.config_path.exists()
 
-    def _write(self):
+    def _write(self) -> None:
         with open(self.config_path, "w", encoding="utf-8") as file:
             string_config = ""
             for key, value in self.items():
                 string_config += f"{key}={value}\n"
             file.write(string_config)
 
-    def _read(self):
+    def _read(self) -> None:
         with open(self.config_path, "r", encoding="utf-8") as file:
             for line in file:
                 key, value = line.strip().split("=")
                 self[key] = value
 
-    def get(self, key: str) -> Optional[str]:
+    def get(self, key: str) -> str:  # type: ignore
         # Prioritize environment variables over config file.
         value = os.getenv(key) or super().get(key)
         if not value:
             raise UsageError(f"Missing config key: {key}")
         return value
 
 
-config = Config(CONFIG_PATH, **DEFAULT_CONFIG)
+cfg = Config(CONFIG_PATH, **DEFAULT_CONFIG)
```

### Comparing `shell_gpt-0.8.8/sgpt/handlers/chat_handler.py` & `shell_gpt-0.8.9/sgpt/handlers/chat_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 from pathlib import Path
-from typing import List, Dict, Optional, Callable, Generator
+from typing import Any, Callable, Dict, Generator, List, Optional
 
 import typer
 from click import BadArgumentUsage
 
-from sgpt import OpenAIClient, config, make_prompt
-from sgpt.utils import CompletionModes
+from sgpt import OpenAIClient, cfg, make_prompt
 from sgpt.handlers.handler import Handler
+from sgpt.utils import CompletionModes
 
-CHAT_CACHE_LENGTH = int(config.get("CHAT_CACHE_LENGTH"))
-CHAT_CACHE_PATH = Path(config.get("CHAT_CACHE_PATH"))
+CHAT_CACHE_LENGTH = int(cfg.get("CHAT_CACHE_LENGTH"))
+CHAT_CACHE_PATH = Path(cfg.get("CHAT_CACHE_PATH"))
 
 
 class ChatSession:
     """
     This class is used as a decorator for OpenAI chat API requests.
     The ChatSession class caches chat messages and keeps track of the
     conversation history. It is designed to store cached messages
@@ -27,23 +27,23 @@
 
         :param length: Integer, maximum number of cached messages to keep.
         """
         self.length = length
         self.storage_path = storage_path
         self.storage_path.mkdir(parents=True, exist_ok=True)
 
-    def __call__(self, func: Callable) -> Callable:
+    def __call__(self, func: Callable[..., Any]) -> Callable[..., Any]:
         """
         The Cache decorator.
 
         :param func: The chat function to cache.
         :return: Wrapped function with chat caching.
         """
 
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> Generator[str, None, None]:
             chat_id = kwargs.pop("chat_id", None)
             messages = kwargs["messages"]
             if not chat_id:
                 yield from func(*args, **kwargs)
                 return
             old_messages = self._read(chat_id)
             for message in messages:
@@ -54,47 +54,47 @@
                 response_text += word
                 yield word
             old_messages.append({"role": "assistant", "content": response_text})
             self._write(kwargs["messages"], chat_id)
 
         return wrapper
 
-    def _read(self, chat_id: str) -> List[Dict]:
+    def _read(self, chat_id: str) -> List[Dict[str, str]]:
         file_path = self.storage_path / chat_id
         if not file_path.exists():
             return []
         parsed_cache = json.loads(file_path.read_text())
         return parsed_cache if isinstance(parsed_cache, list) else []
 
-    def _write(self, messages: List[Dict], chat_id: str):
+    def _write(self, messages: List[Dict[str, str]], chat_id: str) -> None:
         file_path = self.storage_path / chat_id
         json.dump(messages[-self.length :], file_path.open("w"))
 
-    def invalidate(self, chat_id: str):
+    def invalidate(self, chat_id: str) -> None:
         file_path = self.storage_path / chat_id
         file_path.unlink(missing_ok=True)
 
-    def get_messages(self, chat_id):
+    def get_messages(self, chat_id: str) -> List[str]:
         messages = self._read(chat_id)
         return [f"{message['role']}: {message['content']}" for message in messages]
 
     def exists(self, chat_id: Optional[str]) -> bool:
-        return chat_id and bool(self._read(chat_id))
+        return bool(chat_id and bool(self._read(chat_id)))
 
-    def list(self):
+    def list(self) -> List[Path]:
         # Get all files in the folder.
         files = self.storage_path.glob("*")
         # Sort files by last modification time in ascending order.
         return sorted(files, key=lambda f: f.stat().st_mtime)
 
 
 class ChatHandler(Handler):
     chat_session = ChatSession(CHAT_CACHE_LENGTH, CHAT_CACHE_PATH)
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         client: OpenAIClient,
         chat_id: str,
         shell: bool = False,
         code: bool = False,
         model: str = "gpt-3.5-turbo",
     ) -> None:
@@ -107,15 +107,15 @@
         if chat_id == "temp":
             # If the chat id is "temp", we don't want to save the chat session.
             self.chat_session.invalidate(chat_id)
 
         self.validate()
 
     @classmethod
-    def list_ids(cls, value) -> None:
+    def list_ids(cls, value: str) -> None:
         if not value:
             return
         # Prints all existing chat IDs to the console.
         for chat_id in cls.chat_session.list():
             typer.echo(chat_id)
         raise typer.Exit()
 
@@ -123,28 +123,28 @@
     def initiated(self) -> bool:
         return self.chat_session.exists(self.chat_id)
 
     @property
     def is_shell_chat(self) -> bool:
         # TODO: Should be optimized for REPL mode.
         chat_history = self.chat_session.get_messages(self.chat_id)
-        return chat_history and chat_history[0].endswith("###\nCommand:")
+        return bool(chat_history and chat_history[0].endswith("###\nCommand:"))
 
     @property
     def is_code_chat(self) -> bool:
         chat_history = self.chat_session.get_messages(self.chat_id)
-        return chat_history and chat_history[0].endswith("###\nCode:")
+        return bool(chat_history and chat_history[0].endswith("###\nCode:"))
 
     @property
     def is_default_chat(self) -> bool:
         chat_history = self.chat_session.get_messages(self.chat_id)
-        return chat_history and chat_history[0].endswith("###")
+        return bool(chat_history and chat_history[0].endswith("###"))
 
     @classmethod
-    def show_messages_callback(cls, chat_id) -> None:
+    def show_messages_callback(cls, chat_id: str) -> None:
         if not chat_id:
             return
         cls.show_messages(chat_id)
         raise typer.Exit()
 
     @classmethod
     def show_messages(cls, chat_id: str) -> None:
@@ -189,12 +189,12 @@
         return make_prompt.initial(
             prompt,
             self.mode == CompletionModes.SHELL,
             self.mode == CompletionModes.CODE,
         )
 
     @chat_session
-    def get_completion(  # pylint: disable=arguments-differ
+    def get_completion(
         self,
-        **kwargs,
-    ) -> Generator:
+        **kwargs: Any,
+    ) -> Generator[str, None, None]:
         yield from super().get_completion(**kwargs)
```

### Comparing `shell_gpt-0.8.8/sgpt/handlers/default_handler.py` & `shell_gpt-0.8.9/sgpt/handlers/default_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
-from sgpt import OpenAIClient, config, make_prompt
+from sgpt import OpenAIClient, cfg, make_prompt
 from sgpt.utils import CompletionModes
+
 from .handler import Handler
 
-CHAT_CACHE_LENGTH = int(config.get("CHAT_CACHE_LENGTH"))
-CHAT_CACHE_PATH = Path(config.get("CHAT_CACHE_PATH"))
+CHAT_CACHE_LENGTH = int(cfg.get("CHAT_CACHE_LENGTH"))
+CHAT_CACHE_PATH = Path(cfg.get("CHAT_CACHE_PATH"))
 
 
 class DefaultHandler(Handler):
     def __init__(
         self,
         client: OpenAIClient,
         shell: bool = False,
@@ -17,14 +18,14 @@
         model: str = "gpt-3.5-turbo",
     ) -> None:
         super().__init__(client)
         self.client = client
         self.mode = CompletionModes.get_mode(shell, code)
         self.model = model
 
-    def make_prompt(self, prompt) -> str:
+    def make_prompt(self, prompt: str) -> str:
         prompt = prompt.strip()
         return make_prompt.initial(
             prompt,
             self.mode == CompletionModes.SHELL,
             self.mode == CompletionModes.CODE,
         )
```

### Comparing `shell_gpt-0.8.8/sgpt/handlers/handler.py` & `shell_gpt-0.8.9/sgpt/handlers/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from typing import List, Dict, Generator
+from typing import Any, Dict, Generator, List
 
 import typer
 
-from sgpt import OpenAIClient
-from sgpt import config
+from sgpt import OpenAIClient, cfg
 
 
 class Handler:
     def __init__(self, client: OpenAIClient) -> None:
         self.client = client
-        self.color = config.get("DEFAULT_COLOR")
+        self.color = cfg.get("DEFAULT_COLOR")
 
-    def make_prompt(self, prompt) -> str:
+    def make_prompt(self, prompt: str) -> str:
         raise NotImplementedError
 
-    def get_completion(  # pylint: disable=too-many-arguments
+    def get_completion(
         self,
         messages: List[Dict[str, str]],
         model: str = "gpt-3.5-turbo",
         temperature: float = 1,
         top_probability: float = 1,
         caching: bool = True,
-    ) -> Generator:
+    ) -> Generator[str, None, None]:
         yield from self.client.get_completion(
             messages,
             model,
             temperature,
             top_probability,
             caching=caching,
         )
 
-    def handle(self, prompt: str, **kwargs) -> str:
+    def handle(self, prompt: str, **kwargs: Any) -> str:
         prompt = self.make_prompt(prompt)
         messages = [{"role": "user", "content": prompt}]
         full_completion = ""
         for word in self.get_completion(messages=messages, **kwargs):
             typer.secho(word, fg=self.color, bold=True, nl=False)
             full_completion += word
         typer.echo()
```

### Comparing `shell_gpt-0.8.8/sgpt/handlers/repl_handler.py` & `shell_gpt-0.8.9/sgpt/handlers/repl_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-import typer
+from typing import Any
 
+import typer
 from rich import print as rich_print
 from rich.rule import Rule
 
-from sgpt.handlers.chat_handler import ChatHandler
 from sgpt.client import OpenAIClient
+from sgpt.handlers.chat_handler import ChatHandler
 from sgpt.utils import CompletionModes, run_command
 
 
 class ReplHandler(ChatHandler):
-    def __init__(  # pylint: disable=useless-parent-delegation,too-many-arguments
+    def __init__(
         self,
         client: OpenAIClient,
         chat_id: str,
         shell: bool = False,
         code: bool = False,
         model: str = "gpt-3.5-turbo",
     ):
         super().__init__(client, chat_id, shell, code, model)
 
-    def handle(self, prompt: str, **kwargs) -> None:
+    def handle(self, prompt: str, **kwargs: Any) -> None:  # type: ignore
         if self.initiated:
             rich_print(Rule(title="Chat History", style="bold magenta"))
             self.show_messages(self.chat_id)
             rich_print(Rule(style="bold magenta"))
 
         info_message = (
             "Entering REPL mode, press Ctrl+C to exit."
```

### Comparing `shell_gpt-0.8.8/sgpt/make_prompt.py` & `shell_gpt-0.8.9/sgpt/make_prompt.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 from os import getenv, pathsep
 from os.path import basename
-from distro import name as distro_name
 
+from distro import name as distro_name
 
 SHELL_PROMPT = """###
 Provide only {shell} commands for {os} without any description.
 If there is a lack of details, provide most logical solution.
 Ensure the output is a valid shell command.
 If multiple steps required try to combine them together.
 Prompt: {prompt}
```

### Comparing `shell_gpt-0.8.8/sgpt/utils.py` & `shell_gpt-0.8.9/sgpt/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
+import platform
 import shlex
-
 from enum import Enum
 from tempfile import NamedTemporaryFile
 
-import platform
-
 from click import BadParameter
 
 
 class ModelOptions(str, Enum):
     GPT3 = "gpt-3.5-turbo"
     GPT4 = "gpt-4"
     GPT4_32K = "gpt-4-32k"
@@ -17,15 +15,15 @@
 
 class CompletionModes(Enum):
     NORMAL = "normal"
     SHELL = "shell"
     CODE = "code"
 
     @classmethod
-    def get_mode(cls, shell, code) -> "CompletionModes":
+    def get_mode(cls, shell: bool, code: bool) -> "CompletionModes":
         if shell:
             return CompletionModes.SHELL
         if code:
             return CompletionModes.CODE
         return CompletionModes.NORMAL
```

