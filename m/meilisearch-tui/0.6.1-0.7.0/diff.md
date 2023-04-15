# Comparing `tmp/meilisearch_tui-0.6.1.tar.gz` & `tmp/meilisearch_tui-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_tui-0.6.1.tar", max compression
+gzip compressed data, was "meilisearch_tui-0.7.0.tar", max compression
```

## Comparing `meilisearch_tui-0.6.1.tar` & `meilisearch_tui-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/LICENSE
--rw-r--r--   0        0        0     2045 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/__init__.py
--rw-r--r--   0        0        0     2776 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/__main__.py
--rw-r--r--   0        0        0      608 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/client.py
--rw-r--r--   0        0        0     3226 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/config.py
--rw-r--r--   0        0        0       86 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/errors.py
--rw-r--r--   0        0        0     1909 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/meilisearch.css
--rw-r--r--   0        0        0        0 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/py.typed
--rw-r--r--   0        0        0        0 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/screens/__init__.py
--rw-r--r--   0        0        0     4548 2023-04-12 20:46:48.091206 meilisearch_tui-0.6.1/meilisearch_tui/screens/configuration.py
--rw-r--r--   0        0        0    29002 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/screens/indexes.py
--rw-r--r--   0        0        0     3173 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/screens/meilisearch_settings.py
--rw-r--r--   0        0        0     6208 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/screens/search.py
--rw-r--r--   0        0        0      897 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/utils.py
--rw-r--r--   0        0        0        0 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/__init__.py
--rw-r--r--   0        0        0      844 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/index.py
--rw-r--r--   0        0        0     1543 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/index_sidebar.py
--rw-r--r--   0        0        0     1730 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/input.py
--rw-r--r--   0        0        0      709 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/meilisearch_tui/widgets/messages.py
--rw-r--r--   0        0        0     1985 2023-04-12 20:46:48.095207 meilisearch_tui-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 meilisearch_tui-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2045 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/__main__.py
+-rw-r--r--   0        0        0      608 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/client.py
+-rw-r--r--   0        0        0     3226 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/config.py
+-rw-r--r--   0        0        0       86 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/errors.py
+-rw-r--r--   0        0        0     2776 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/main.py
+-rw-r--r--   0        0        0     1909 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/meilisearch.css
+-rw-r--r--   0        0        0        0 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/py.typed
+-rw-r--r--   0        0        0        0 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/screens/__init__.py
+-rw-r--r--   0        0        0     4548 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/screens/configuration.py
+-rw-r--r--   0        0        0    29002 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/screens/indexes.py
+-rw-r--r--   0        0        0     6241 2023-04-15 14:59:36.851476 meilisearch_tui-0.7.0/meilisearch_tui/screens/search.py
+-rw-r--r--   0        0        0      897 2023-04-15 14:59:36.855476 meilisearch_tui-0.7.0/meilisearch_tui/utils.py
+-rw-r--r--   0        0        0        0 2023-04-15 14:59:36.855476 meilisearch_tui-0.7.0/meilisearch_tui/widgets/__init__.py
+-rw-r--r--   0        0        0      844 2023-04-15 14:59:36.855476 meilisearch_tui-0.7.0/meilisearch_tui/widgets/index.py
+-rw-r--r--   0        0        0     1543 2023-04-15 14:59:36.855476 meilisearch_tui-0.7.0/meilisearch_tui/widgets/index_sidebar.py
+-rw-r--r--   0        0        0     1730 2023-04-15 14:59:36.855476 meilisearch_tui-0.7.0/meilisearch_tui/widgets/input.py
+-rw-r--r--   0        0        0      709 2023-04-15 14:59:36.855476 meilisearch_tui-0.7.0/meilisearch_tui/widgets/messages.py
+-rw-r--r--   0        0        0     2005 2023-04-15 14:59:36.855476 meilisearch_tui-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 meilisearch_tui-0.7.0/PKG-INFO
```

### Comparing `meilisearch_tui-0.6.1/LICENSE` & `meilisearch_tui-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/README.md` & `meilisearch_tui-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/__main__.py` & `meilisearch_tui-0.7.0/meilisearch_tui/main.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/client.py` & `meilisearch_tui-0.7.0/meilisearch_tui/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/config.py` & `meilisearch_tui-0.7.0/meilisearch_tui/config.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/meilisearch.css` & `meilisearch_tui-0.7.0/meilisearch_tui/meilisearch.css`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/screens/configuration.py` & `meilisearch_tui-0.7.0/meilisearch_tui/screens/configuration.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/screens/indexes.py` & `meilisearch_tui-0.7.0/meilisearch_tui/screens/indexes.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/screens/search.py` & `meilisearch_tui-0.7.0/meilisearch_tui/screens/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 from functools import cached_property
 
+from aiocache import cached
 from meilisearch_python_async.errors import MeilisearchCommunicationError
 from meilisearch_python_async.models.search import SearchResults
 from textual import events
 from textual.app import ComposeResult
 from textual.containers import Center, Container, Content
 from textual.screen import Screen
 from textual.widgets import Button, Footer, Input, Markdown, Static
@@ -101,27 +102,28 @@
         self.index_name.update(f"Searching index: {self.selected_index}")
         self.search_input.value = ""
         self.results.update("")
 
     async def on_input_changed(self, message: Input.Changed) -> None:
         self.limit = 20
         if message.value:
-            asyncio.create_task(self.lookup_word(message.value))
+            asyncio.create_task(self.search(message.value))
         else:
             self.results.update("")
             self.load_more_button.visible = False
 
     async def on_button_pressed(self, event: Button.Pressed) -> None:
         button_id = event.button.id
 
         if button_id == "load-more-button":
             self.limit += 20
-            asyncio.create_task(self.lookup_word(self.search_input.value))
+            asyncio.create_task(self.search(self.search_input.value))
 
-    async def lookup_word(self, search: str) -> None:
+    @cached(ttl=10)
+    async def search(self, search: str) -> None:
         if not self.selected_index and search == self.search_input.value:
             self.results.update("Error: No index provided")
             return
 
         if not self.selected_index:
             self.results.update("No index selected")
             return
```

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/utils.py` & `meilisearch_tui-0.7.0/meilisearch_tui/utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/widgets/index.py` & `meilisearch_tui-0.7.0/meilisearch_tui/widgets/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/widgets/index_sidebar.py` & `meilisearch_tui-0.7.0/meilisearch_tui/widgets/index_sidebar.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/widgets/input.py` & `meilisearch_tui-0.7.0/meilisearch_tui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/meilisearch_tui/widgets/messages.py` & `meilisearch_tui-0.7.0/meilisearch_tui/widgets/messages.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.6.1/pyproject.toml` & `meilisearch_tui-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-tui"
-version = "0.6.1"
+version = "0.7.0"
 description = "A TUI for Managing and Searching with Meilisearch"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-tui"
 homepage = "https://github.com/sanders41/meilisearch-tui"
 documentation = "https://github.com/sanders41/meilisearch-tui"
@@ -20,14 +20,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 meilisearch-python-async = "1.1.1"
 textual = "0.19.1"
 uvloop = {version = "0.17.0", markers = "sys_platform != 'win32'"}
+aiocache = "0.12.0"
 
 [tool.poetry.group.dev.dependencies]
 aiohttp = "3.8.4"
 black = "23.3.0"
 click = "8.1.3"
 msgpack = "1.0.5"
 mypy = "1.2.0"
```

### Comparing `meilisearch_tui-0.6.1/PKG-INFO` & `meilisearch_tui-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-tui
-Version: 0.6.1
+Version: 0.7.0
 Summary: A TUI for Managing and Searching with Meilisearch
 Home-page: https://github.com/sanders41/meilisearch-tui
 License: MIT
 Keywords: meilisearch,tui
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: aiocache (==0.12.0)
 Requires-Dist: meilisearch-python-async (==1.1.1)
 Requires-Dist: textual (==0.19.1)
 Requires-Dist: uvloop (==0.17.0) ; sys_platform != "win32"
 Project-URL: Documentation, https://github.com/sanders41/meilisearch-tui
 Project-URL: Repository, https://github.com/sanders41/meilisearch-tui
 Description-Content-Type: text/markdown
```

