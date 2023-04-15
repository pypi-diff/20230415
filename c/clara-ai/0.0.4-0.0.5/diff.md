# Comparing `tmp/clara_ai-0.0.4.tar.gz` & `tmp/clara_ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clara_ai-0.0.4.tar", max compression
+gzip compressed data, was "clara_ai-0.0.5.tar", max compression
```

## Comparing `clara_ai-0.0.4.tar` & `clara_ai-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1534 2023-04-13 21:56:40.455905 clara_ai-0.0.4/LICENSE
--rw-r--r--   0        0        0     2148 2023-04-13 21:56:40.455905 clara_ai-0.0.4/README.md
--rw-r--r--   0        0        0     4458 2023-04-13 21:56:40.455905 clara_ai-0.0.4/clara/cli.py
--rw-r--r--   0        0        0       54 2023-04-13 21:56:40.455905 clara_ai-0.0.4/clara/console.py
--rw-r--r--   0        0        0     3090 2023-04-13 21:56:40.459905 clara_ai-0.0.4/clara/consts.py
--rw-r--r--   0        0        0     5391 2023-04-13 21:56:40.459905 clara_ai-0.0.4/clara/index.py
--rw-r--r--   0        0        0      665 2023-04-13 21:56:40.459905 clara_ai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 clara_ai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1534 2023-04-15 21:29:03.406781 clara_ai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3036 2023-04-15 21:29:03.410781 clara_ai-0.0.5/README.md
+-rw-r--r--   0        0        0     2283 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/chat.py
+-rw-r--r--   0        0        0     6035 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/cli.py
+-rw-r--r--   0        0        0      369 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/config.py
+-rw-r--r--   0        0        0       54 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/console.py
+-rw-r--r--   0        0        0     3593 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/consts.py
+-rw-r--r--   0        0        0     5351 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/index.py
+-rw-r--r--   0        0        0      703 2023-04-15 21:29:03.410781 clara_ai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3808 1970-01-01 00:00:00.000000 clara_ai-0.0.5/PKG-INFO
```

### Comparing `clara_ai-0.0.4/LICENSE` & `clara_ai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.4/README.md` & `clara_ai-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 ## Introduction
 
 Clara is an AI-powered tool designed to assist developers in navigating unfamiliar code repositories, making it highly valuable during the on-boarding process for new projects, or when deciphering legacy code.
 
 In the future, Clara will also provide support for tasks such as documentation, auditing, and developing new features, among others.
 
-## Usage
+## Install
 
-Install:
+With:
 
 ```
 pipx install clara-ai
 ```
 
 Or:
 
@@ -40,32 +40,32 @@
 
 Then, use the command:
 
 ```
 $ clara chat [PATH]
 ```
 
-If the path is omitted, '.' will be used.
+If the path is omitted then '.' will be used.
 
-To exit use `CTRL-C` or `CTRL-D`.
+To exit use `CTRL-C` or `CTRL-D`, or commands `/quit` or `/exit`.
 
 All commands:
 
 ```
-COMMANDS
-    COMMAND is one of the following:
+     ask
+       Ask a question about the code from the command-line.
 
      chat
        Chat about the code.
 
      clean
        Delete vector DB for a given path.
 
      config
-       Get config for a given path.
+       Show config for a given path.
 ```
 
 ## Chat commands
 
 During chat you can also use this commands:
 
 ```
@@ -75,11 +75,37 @@
 
 /quit
 /exit    -- exit (you can use also CTRL-C or CTRL-D)
 
 /help    -- show this message
 ```
 
+## Configuration
+
+Run `poetry run clara config` to know from where the program is going to read the configuration. Usually this path is going to be `/.config/clara/clara.yaml`.
+
+For now, there is only one parameter to change. This is a sample configuration:
+
+```
+llm:
+  model: gpt-3.5-turbo
+```
+
+Change the model for `gpt-4` if you have access to it.
+
+## Cache
+
+Vector DB and chat history are stored in a cache directory, per code directory. Use `poetry run clara config` to know the path to this directory.
+
+You can remove manually this directory, if you want to refresh the data stored, or simply use the command `poetry run clara clean`.
+
+If you want to chat with the code without reading/storing the vector DB (using the DB in memory), use the command `poetry run clara [PATH] --memory-storage`.
+
 ## Roadmap
 
-- [ ] Improve chat: short-term history, context, personality,...
-- [ ] Tools: document code, audit, refactoring, test creation,...
+- [x] Short-term history
+- [x] Configurable LLM
+- [ ] Tools
+  - [ ] Document code with docstrings
+  - [ ] Test creation
+  - [ ] Audit code
+  - [ ] Refactoring
```

### Comparing `clara_ai-0.0.4/clara/cli.py` & `clara_ai-0.0.5/clara/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,59 +6,104 @@
 from rich.prompt import Confirm
 from rich.markdown import Markdown
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 import click
 from openai.error import InvalidRequestError
 
-from .consts import HELP_MESSAGE
+from .consts import HELP_MESSAGE, CONFIG_PATH
 from .console import console
 from .index import RepositoryIndex
 
 
 # Disable warnings
-logging.getLogger("chromadb").setLevel(logging.ERROR)
 logging.getLogger().setLevel(logging.ERROR)
 
 
+def setup(path: str, memory_storage: bool) -> RepositoryIndex:
+    index = RepositoryIndex(path, in_memory=memory_storage)
+
+    with console.status(
+        f"Ingesting code repository from path: [blue underline]{path} …",
+        spinner="weather",
+    ):
+        index.ingest()
+
+    with console.status(
+        "Storing vector database in path: " "[blue underline]{index.persist_path} …",
+        spinner="weather",
+    ):
+        index.persist()
+
+    return index
+
+
 class Clara:
     """CLARA: Code Language Assistant & Repository Analyzer"""
 
     def config(self, path: str = "."):
         """Show config for a given path."""
         index = RepositoryIndex(path)
-        console.print(f"Vector DB persist path = [blue underline]{index.persist_path}")
+        console.print(f"Configuration path (global) = [blue underline]{CONFIG_PATH}")
+        console.print(
+            "Data persistence path (for this project) = "
+            f"[blue underline]{index.persist_path}"
+        )
 
     def clean(self, path: str = "."):
         """Delete vector DB for a given path."""
         index = RepositoryIndex(path)
         if Confirm.ask(
             "Are you sure you want to remove "
-            f"[blue underline]{index.persist_path}[/blue underline]?",
+            f"[blue underline]{index.persist_path}[/blue underline]? "
+            "This will remove the vector DB and the chat history for this code.",
             default=False,
         ):
             index.clean()
 
-    def chat(self, path: str = ".", memory_storage: bool = False):
-        """Chat about the code."""
-
-        index = RepositoryIndex(path, in_memory=memory_storage)
+    def ask(
+        self,
+        question,
+        path: str = ".",
+        memory_storage: bool = False,
+        markdown_render: bool = True,
+        sources: bool = True,
+        full_sources: bool = False,
+    ):
+        """Ask a question about the code from the command-line."""
+        index = setup(path, memory_storage)
 
-        with console.status(
-            f"Ingesting code repository from path: [blue underline]{path} …",
-            spinner="weather",
-        ):
-            index.ingest()
+        try:
+            with console.status("Querying…", spinner="weather"):
+                result = index.query_with_sources(question)
+            if markdown_render:
+                console.print(Markdown(result.answer))
+            else:
+                console.print(result.answer)
+            console.print()
+            console.print("[yellow]SOURCES[/yellow]")
+            if sources:
+                if full_sources:
+                    for source in result.sources:
+                        console.print()
+                        console.print(source.page_content)
+                        console.print(f"- [blue underline]{source.metadata['source']}")
+                else:
+                    for source in result.sources:
+                        console.print(f"- [blue underline]{source.metadata['source']}")
+        except InvalidRequestError:
+            console.print(
+                ":no_entry: " "[bold red]Ups, the request was invalid for some reason."
+            )
+        finally:
+            pass
 
-        with console.status(
-            "Storing vector database in path: "
-            "[blue underline]{index.persist_path} …",
-            spinner="weather",
-        ):
-            index.persist()
+    def chat(self, path: str = ".", memory_storage: bool = False):
+        """Chat about the code."""
+        index = setup(path, memory_storage)
 
         console.rule("[bold blue]CHAT")
         console.print("Hi, I'm Clara!", ":scroll::mag::robot:")
         console.print("How can I help you?")
         console.print()
 
         last_sources = []
@@ -92,18 +137,15 @@
                         query = query.strip()
                         session.history.append_string(query)
                         console.print(">>>", query)
                     elif query == "/help":
                         console.print(HELP_MESSAGE)
                         continue
                     else:
-                        console.print(
-                            ":no_entry: "
-                            "[bold red]Unknown command."
-                        )
+                        console.print(":no_entry: " "[bold red]Unknown command.")
                         continue
 
                 try:
                     with console.status("Querying…", spinner="weather"):
                         result = index.query_with_sources(query)
                     console.print()
                     console.print(Markdown(result.answer))
@@ -113,14 +155,16 @@
                         console.print(f"- [blue underline]{source.metadata['source']}")
                     last_sources = result.sources
                 except InvalidRequestError:
                     console.print(
                         ":no_entry: "
                         "[bold red]Ups, the request was invalid for some reason."
                     )
+                finally:
+                    pass
                 console.rule()
         except (KeyboardInterrupt, EOFError):
             console.print()
         finally:
             console.rule("[bold blue]END")
             console.print()
             console.print("Bye!", ":wave:")
```

### Comparing `clara_ai-0.0.4/clara/index.py` & `clara_ai-0.0.5/clara/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,40 @@
 import pathlib
 import hashlib
 import shutil
 from typing import List, Tuple, Iterable, Optional
 from dataclasses import dataclass
 import glob
 
-from langchain.chat_models import ChatOpenAI
-from langchain.chains import ConversationalRetrievalChain
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.indexes.vectorstore import VectorStoreIndexWrapper
 from langchain.vectorstores import Chroma
 from langchain.document_loaders import TextLoader
 from langchain.text_splitter import CharacterTextSplitter
 from langchain.schema import Document
 
-from .consts import WILDCARDS, BASE_PERSIST_PATH, PROMPT_PREFIX, CONDENSE_QUESTION_PROMPT
+from .consts import (
+    WILDCARDS,
+    BASE_PERSIST_PATH,
+    PROMPT_PREFIX,
+)
+from .chat import create_chat
 from .console import console
 
 
 @dataclass
 class QueryResult:
     question: str
     answer: str
     sources: List[Document]
 
 
 class ChatHistory:
     def __init__(
-        self, prompt_prefix: Optional[Tuple[str, str]] = None, length_limit: int = 4096
+        self, prompt_prefix: Optional[Tuple[str, str]] = None, length_limit: int = 3500
     ):
         self.prompt_prefix = prompt_prefix
         self.history = [prompt_prefix] if prompt_prefix else []
         self.length_limit = length_limit
 
     def append(self, messages: Tuple[str, str]):
         def get_total_length(messages: Iterable[str]) -> int:
@@ -129,21 +132,23 @@
             self.index.vectorstore.persist()
 
     def clean(self):
         if not self.in_memory:
             shutil.rmtree(self.persist_path)
 
     def init_chat(self):
-        model = ChatOpenAI(model="gpt-3.5-turbo", temperature=0)  # 'gpt-4',
-        self.chat = ConversationalRetrievalChain.from_llm(
-            model,
-            retriever=self.index.vectorstore.as_retriever(),
-            return_source_documents=True,
-            condense_question_prompt=CONDENSE_QUESTION_PROMPT,
-        )
+        # model = self.get_model()
+        # self.chat = ConversationalRetrievalChain.from_llm(
+        #     model,
+        #     retriever=self.index.vectorstore.as_retriever(),
+        #     return_source_documents=True,
+        #     condense_question_prompt=CONDENSE_QUESTION_PROMPT,
+        # )
+
+        self.chat = create_chat(self.index.vectorstore.as_retriever())
 
     def query_with_sources(self, query: str) -> QueryResult:
         # return QueryResult(**self.index.query_with_sources(query))
         if self.chat is None:
             self.init_chat()
         response = self.chat(
             {"question": query, "chat_history": self.chat_history.history}
```

### Comparing `clara_ai-0.0.4/pyproject.toml` & `clara_ai-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "clara-ai"
-version = "0.0.4"
+version = "0.0.5"
 description = "CLARA: Code Language Assistant & Repository Analyzer"
 authors = ["Cristóbal Carnero Liñán <cristobal@seednapse.ai>"]
 readme = "README.md"
 packages = [{include = "clara"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-langchain = {extras = ["llms"], version = "^0.0.136"}
+langchain = {version = ">=0.0.139", extras = ["llms"]}
 fire = "^0.5.0"
 chromadb = "^0.3.21"
 rich = "^13.3.3"
 tiktoken = "^0.3.3"
 prompt-toolkit = "^3.0.38"
 click = "^8.1.3"
+pyyaml = "^6.0"
+mergedeep = "^1.3.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 icecream = "^2.1.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `clara_ai-0.0.4/PKG-INFO` & `clara_ai-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: clara-ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLARA: Code Language Assistant & Repository Analyzer
 Author: Cristóbal Carnero Liñán
 Author-email: cristobal@seednapse.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.3.21,<0.4.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: langchain[llms] (>=0.0.136,<0.0.137)
+Requires-Dist: langchain[llms] (>=0.0.139)
+Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Description-Content-Type: text/markdown
 
 CLARA: Code Language Assistant & Repository Analyzer 📜🔍🤖
 ========================================================
 
@@ -31,17 +33,17 @@
 
 ## Introduction
 
 Clara is an AI-powered tool designed to assist developers in navigating unfamiliar code repositories, making it highly valuable during the on-boarding process for new projects, or when deciphering legacy code.
 
 In the future, Clara will also provide support for tasks such as documentation, auditing, and developing new features, among others.
 
-## Usage
+## Install
 
-Install:
+With:
 
 ```
 pipx install clara-ai
 ```
 
 Or:
 
@@ -59,32 +61,32 @@
 
 Then, use the command:
 
 ```
 $ clara chat [PATH]
 ```
 
-If the path is omitted, '.' will be used.
+If the path is omitted then '.' will be used.
 
-To exit use `CTRL-C` or `CTRL-D`.
+To exit use `CTRL-C` or `CTRL-D`, or commands `/quit` or `/exit`.
 
 All commands:
 
 ```
-COMMANDS
-    COMMAND is one of the following:
+     ask
+       Ask a question about the code from the command-line.
 
      chat
        Chat about the code.
 
      clean
        Delete vector DB for a given path.
 
      config
-       Get config for a given path.
+       Show config for a given path.
 ```
 
 ## Chat commands
 
 During chat you can also use this commands:
 
 ```
@@ -94,12 +96,38 @@
 
 /quit
 /exit    -- exit (you can use also CTRL-C or CTRL-D)
 
 /help    -- show this message
 ```
 
+## Configuration
+
+Run `poetry run clara config` to know from where the program is going to read the configuration. Usually this path is going to be `/.config/clara/clara.yaml`.
+
+For now, there is only one parameter to change. This is a sample configuration:
+
+```
+llm:
+  model: gpt-3.5-turbo
+```
+
+Change the model for `gpt-4` if you have access to it.
+
+## Cache
+
+Vector DB and chat history are stored in a cache directory, per code directory. Use `poetry run clara config` to know the path to this directory.
+
+You can remove manually this directory, if you want to refresh the data stored, or simply use the command `poetry run clara clean`.
+
+If you want to chat with the code without reading/storing the vector DB (using the DB in memory), use the command `poetry run clara [PATH] --memory-storage`.
+
 ## Roadmap
 
-- [ ] Improve chat: short-term history, context, personality,...
-- [ ] Tools: document code, audit, refactoring, test creation,...
+- [x] Short-term history
+- [x] Configurable LLM
+- [ ] Tools
+  - [ ] Document code with docstrings
+  - [ ] Test creation
+  - [ ] Audit code
+  - [ ] Refactoring
```

