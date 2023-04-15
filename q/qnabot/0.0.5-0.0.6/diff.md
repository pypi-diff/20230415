# Comparing `tmp/qnabot-0.0.5.tar.gz` & `tmp/qnabot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnabot-0.0.5.tar", last modified: Thu Apr 13 23:57:45 2023, max compression
+gzip compressed data, was "qnabot-0.0.6.tar", last modified: Sat Apr 15 07:34:04 2023, max compression
```

## Comparing `qnabot-0.0.5.tar` & `qnabot-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.015192 qnabot-0.0.5/
--rw-r--r--   0 momegas    (501) staff       (20)     3521 2023-04-13 23:57:45.015065 qnabot-0.0.5/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)     3161 2023-04-13 23:55:55.000000 qnabot-0.0.5/README.md
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.013900 qnabot-0.0.5/qnabot/
--rw-r--r--   0 momegas    (501) staff       (20)     2997 2023-04-13 23:33:14.000000 qnabot-0.0.5/qnabot/QnABot.py
--rw-r--r--   0 momegas    (501) staff       (20)       55 2023-04-13 23:53:43.000000 qnabot-0.0.5/qnabot/__init__.py
--rw-r--r--   0 momegas    (501) staff       (20)      267 2023-04-13 23:52:46.000000 qnabot-0.0.5/qnabot/api.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.014810 qnabot-0.0.5/qnabot/tests/
--rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 qnabot-0.0.5/qnabot/tests/__init__.py
--rw-r--r--   0 momegas    (501) staff       (20)     1484 2023-04-13 23:17:41.000000 qnabot-0.0.5/qnabot/tests/test_QnABot.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.014618 qnabot-0.0.5/qnabot.egg-info/
--rw-r--r--   0 momegas    (501) staff       (20)     3521 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)      270 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/SOURCES.txt
--rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/dependency_links.txt
--rw-r--r--   0 momegas    (501) staff       (20)       50 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/requires.txt
--rw-r--r--   0 momegas    (501) staff       (20)        7 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/top_level.txt
--rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-13 23:57:45.015232 qnabot-0.0.5/setup.cfg
--rw-r--r--   0 momegas    (501) staff       (20)      739 2023-04-13 23:57:19.000000 qnabot-0.0.5/setup.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 07:34:04.118628 qnabot-0.0.6/
+-rw-r--r--   0 momegas    (501) staff       (20)     1075 2023-04-14 20:57:02.000000 qnabot-0.0.6/LICENCE
+-rw-r--r--   0 momegas    (501) staff       (20)     4126 2023-04-15 07:34:04.118475 qnabot-0.0.6/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)     3744 2023-04-14 17:40:15.000000 qnabot-0.0.6/README.md
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 07:34:04.116567 qnabot-0.0.6/qnabot/
+-rw-r--r--   0 momegas    (501) staff       (20)     3060 2023-04-14 17:27:00.000000 qnabot-0.0.6/qnabot/QnABot.py
+-rw-r--r--   0 momegas    (501) staff       (20)       88 2023-04-14 17:25:24.000000 qnabot-0.0.6/qnabot/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)      260 2023-04-14 17:32:35.000000 qnabot-0.0.6/qnabot/api.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 07:34:04.118126 qnabot-0.0.6/qnabot/tests/
+-rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 qnabot-0.0.6/qnabot/tests/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)     1463 2023-04-14 17:29:48.000000 qnabot-0.0.6/qnabot/tests/test_QnABot.py
+-rw-r--r--   0 momegas    (501) staff       (20)      578 2023-04-14 12:48:59.000000 qnabot-0.0.6/qnabot/tests/test_api.py
+-rw-r--r--   0 momegas    (501) staff       (20)      597 2023-04-14 17:34:04.000000 qnabot-0.0.6/qnabot/tests/test_ui.py
+-rw-r--r--   0 momegas    (501) staff       (20)      407 2023-04-14 20:54:08.000000 qnabot-0.0.6/qnabot/ui.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 07:34:04.117345 qnabot-0.0.6/qnabot.egg-info/
+-rw-r--r--   0 momegas    (501) staff       (20)     4126 2023-04-15 07:34:04.000000 qnabot-0.0.6/qnabot.egg-info/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)      340 2023-04-15 07:34:04.000000 qnabot-0.0.6/qnabot.egg-info/SOURCES.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-15 07:34:04.000000 qnabot-0.0.6/qnabot.egg-info/dependency_links.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       63 2023-04-15 07:34:04.000000 qnabot-0.0.6/qnabot.egg-info/requires.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        7 2023-04-15 07:34:04.000000 qnabot-0.0.6/qnabot.egg-info/top_level.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-15 07:34:04.118672 qnabot-0.0.6/setup.cfg
+-rw-r--r--   0 momegas    (501) staff       (20)      763 2023-04-15 07:33:59.000000 qnabot-0.0.6/setup.py
```

### Comparing `qnabot-0.0.5/PKG-INFO` & `qnabot-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: qnabot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create a question answering over docs bot with one line of code.
 Home-page: https://github.com/momegas/qnabot
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
+License-File: LICENCE
 
 # QnA Bot
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
 Create a question answering over docs bot with one line of code:
 
@@ -35,34 +36,47 @@
 # Save the index to save costs (GPT is used to create the index)
 bot.save_index("index.pickle")
 
 # Load the index from a previous run
 bot = QnABot(directory="./mydata", index="index.pickle")
 ```
 
-You can also create a FastAPI app that will expose the bot as an API. You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
+You can also create a FastAPI app that will expose the bot as an API using the create_app function.
+Assuming you file is called `main.py` run `uvicorn main:app --reload` to run the API locally.
+You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
 
 ```python
 from qnabot import QnABot, create_app
 
-app = create_app(QnABot("./examples/files"))
+app = create_app(QnABot("./mydata"))
+```
+
+You can expose a gradio UI for the bot using `create_interface` function.
+Assuming your file is called `ui.py` run `gradio qnabot/ui.py` to run the UI locally.
+You should then be able to visit `http://127.0.0.1:7860` to see the API documentation.
+
+```python
+from qnabot import QnABot, create_interface
+
+demo = create_interface(QnABot("./mydata"))
 ```
 
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
 - [x] FAISS for storing vectors / index
 - [x] Expose bot over API using FastAPI
+- [x] Gradio UI
+- [ ] Integration with [guardrails](https://github.com/ShreyaR/guardrails)
+- [ ] Integration with [GPTCache](https://github.com/zilliztech/GPTCache)
 - [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
 - [ ] Customise prompt
 - [ ] Support for LLaMA model
-- [ ] Support for Anthropic models
-- [ ] CLI / UI
 
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
 
 In simple terms, when you have a question, you first search for relevant documents. Then, you give the documents and the question to the language model to generate an answer. To make this work, you need your documents in a searchable format (an index). This process involves two main steps: (1) preparing your documents for easy querying, and (2) using the retrieval augmented generation method.
```

### Comparing `qnabot-0.0.5/README.md` & `qnabot-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,34 +23,47 @@
 # Save the index to save costs (GPT is used to create the index)
 bot.save_index("index.pickle")
 
 # Load the index from a previous run
 bot = QnABot(directory="./mydata", index="index.pickle")
 ```
 
-You can also create a FastAPI app that will expose the bot as an API. You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
+You can also create a FastAPI app that will expose the bot as an API using the create_app function.
+Assuming you file is called `main.py` run `uvicorn main:app --reload` to run the API locally.
+You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
 
 ```python
 from qnabot import QnABot, create_app
 
-app = create_app(QnABot("./examples/files"))
+app = create_app(QnABot("./mydata"))
+```
+
+You can expose a gradio UI for the bot using `create_interface` function.
+Assuming your file is called `ui.py` run `gradio qnabot/ui.py` to run the UI locally.
+You should then be able to visit `http://127.0.0.1:7860` to see the API documentation.
+
+```python
+from qnabot import QnABot, create_interface
+
+demo = create_interface(QnABot("./mydata"))
 ```
 
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
 - [x] FAISS for storing vectors / index
 - [x] Expose bot over API using FastAPI
+- [x] Gradio UI
+- [ ] Integration with [guardrails](https://github.com/ShreyaR/guardrails)
+- [ ] Integration with [GPTCache](https://github.com/zilliztech/GPTCache)
 - [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
 - [ ] Customise prompt
 - [ ] Support for LLaMA model
-- [ ] Support for Anthropic models
-- [ ] CLI / UI
 
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
 
 In simple terms, when you have a question, you first search for relevant documents. Then, you give the documents and the question to the language model to generate an answer. To make this work, you need your documents in a searchable format (an index). This process involves two main steps: (1) preparing your documents for easy querying, and (2) using the retrieval augmented generation method.
```

### Comparing `qnabot-0.0.5/qnabot/QnABot.py` & `qnabot-0.0.6/qnabot/QnABot.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pickle
 import os
 
 
 class QnABot:
     def __init__(
         self,
-        directory: str,
+        directory: str | None = None,
         index: str | None = None,
         model: str | None = None,
         verbose: bool = False,
         temperature: int = 0,
     ):
         # Initialize the QnABot by selecting a model, creating a loader,
         # and loading or creating an index
@@ -32,15 +32,17 @@
             print("Using model: gpt-3.5-turbo")
             self.llm = ChatOpenAI(temperature=temperature)
 
         if model == "text-davinci-003":
             print("Using model: text-davinci-003")
             self.llm = OpenAI(temperature=temperature)
 
-    def create_loader(self, directory: str):
+    def create_loader(self, directory: str | None):
+        if directory is None:
+            return
         # Create a loader based on the provided directory (either local or S3)
         if directory.startswith("s3://"):
             self.loader = S3DirectoryLoader(directory)
         else:
             self.loader = DirectoryLoader(directory, recursive=True)
 
     def load_or_create_index(self, index_path: str | None):
@@ -62,12 +64,12 @@
 
     def print_answer(self, question: str, k=1):
         # Retrieve and print the answer to the given question
         input_documents = self.search_index.similarity_search(question, k=k)
         a = self.chain.run(input_documents=input_documents, question=question)
         print(a)
 
-    def get_answer(self, question: str, k=1) -> str:
+    def ask(self, question: str, k=1) -> str:
         # Retrieve the answer to the given question and return it
         input_documents = self.search_index.similarity_search(question, k=k)
         answer = self.chain.run(input_documents=input_documents, question=question)
         return answer
```

### Comparing `qnabot-0.0.5/qnabot/tests/test_QnABot.py` & `qnabot-0.0.6/qnabot/tests/test_QnABot.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # Define test data
 test_directory = "./examples/files"
 test_question = "what was the first roster of avengers in comics?"
 correct_answer = "Iron Man, Thor, Hulk, Ant-Man"
 sources = "SOURCES:"
 
 
-def test_get_answer():
+def test_ask():
     bot = QnABot(directory=test_directory)
-    answer = bot.get_answer(test_question)
+    answer = bot.ask(test_question)
 
     # Assert that the answer contains the correct answer
     assert correct_answer in answer
     # Assert that the answer contains the sources
     assert sources in answer
 
 
@@ -37,8 +37,8 @@
         with open(index_path, "rb") as f:
             saved_index = pickle.load(f)
         assert isinstance(saved_index, FAISS)
 
         bot_with_predefined_index = QnABot(directory=test_directory, index=index_path)
 
         # Assert that the bot returns the correct answer to the test question
-        assert correct_answer in bot_with_predefined_index.get_answer(test_question)
+        assert correct_answer in bot_with_predefined_index.ask(test_question)
```

### Comparing `qnabot-0.0.5/qnabot.egg-info/PKG-INFO` & `qnabot-0.0.6/qnabot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: qnabot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create a question answering over docs bot with one line of code.
 Home-page: https://github.com/momegas/qnabot
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
+License-File: LICENCE
 
 # QnA Bot
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
 Create a question answering over docs bot with one line of code:
 
@@ -35,34 +36,47 @@
 # Save the index to save costs (GPT is used to create the index)
 bot.save_index("index.pickle")
 
 # Load the index from a previous run
 bot = QnABot(directory="./mydata", index="index.pickle")
 ```
 
-You can also create a FastAPI app that will expose the bot as an API. You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
+You can also create a FastAPI app that will expose the bot as an API using the create_app function.
+Assuming you file is called `main.py` run `uvicorn main:app --reload` to run the API locally.
+You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
 
 ```python
 from qnabot import QnABot, create_app
 
-app = create_app(QnABot("./examples/files"))
+app = create_app(QnABot("./mydata"))
+```
+
+You can expose a gradio UI for the bot using `create_interface` function.
+Assuming your file is called `ui.py` run `gradio qnabot/ui.py` to run the UI locally.
+You should then be able to visit `http://127.0.0.1:7860` to see the API documentation.
+
+```python
+from qnabot import QnABot, create_interface
+
+demo = create_interface(QnABot("./mydata"))
 ```
 
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
 - [x] FAISS for storing vectors / index
 - [x] Expose bot over API using FastAPI
+- [x] Gradio UI
+- [ ] Integration with [guardrails](https://github.com/ShreyaR/guardrails)
+- [ ] Integration with [GPTCache](https://github.com/zilliztech/GPTCache)
 - [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
 - [ ] Customise prompt
 - [ ] Support for LLaMA model
-- [ ] Support for Anthropic models
-- [ ] CLI / UI
 
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
 
 In simple terms, when you have a question, you first search for relevant documents. Then, you give the documents and the question to the language model to generate an answer. To make this work, you need your documents in a searchable format (an index). This process involves two main steps: (1) preparing your documents for easy querying, and (2) using the retrieval augmented generation method.
```

### Comparing `qnabot-0.0.5/setup.py` & `qnabot-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 setup(
     name="qnabot",
     version=VERSION,
     packages=find_packages(),
     install_requires=[
         "langchain",
         "tiktoken",
         "unstructured",
         "fastapi",
         "faiss-cpu",
+        "pdfminer.six",
     ],
     author="Megaklis Vasilakis",
     author_email="megaklis.vasilakis@gmail.com",
     description="Create a question answering over docs bot with one line of code.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/momegas/qnabot",
```

