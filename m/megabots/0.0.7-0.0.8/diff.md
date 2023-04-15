# Comparing `tmp/megabots-0.0.7.tar.gz` & `tmp/megabots-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megabots-0.0.7.tar", last modified: Sat Apr 15 11:30:54 2023, max compression
+gzip compressed data, was "megabots-0.0.8.tar", last modified: Sat Apr 15 15:18:22 2023, max compression
```

## Comparing `megabots-0.0.7.tar` & `megabots-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.525576 megabots-0.0.7/
--rw-r--r--   0 momegas    (501) staff       (20)     1075 2023-04-14 20:57:02.000000 megabots-0.0.7/LICENCE
--rw-r--r--   0 momegas    (501) staff       (20)     4430 2023-04-15 11:30:54.525429 megabots-0.0.7/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)     4044 2023-04-15 11:28:29.000000 megabots-0.0.7/README.md
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.524172 megabots-0.0.7/megabots/
--rw-r--r--   0 momegas    (501) staff       (20)     5290 2023-04-15 11:09:34.000000 megabots-0.0.7/megabots/__init__.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.525231 megabots-0.0.7/megabots/tests/
--rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 megabots-0.0.7/megabots/tests/__init__.py
--rw-r--r--   0 momegas    (501) staff       (20)      593 2023-04-15 11:10:48.000000 megabots-0.0.7/megabots/tests/test_api.py
--rw-r--r--   0 momegas    (501) staff       (20)     1464 2023-04-15 11:11:24.000000 megabots-0.0.7/megabots/tests/test_bots.py
--rw-r--r--   0 momegas    (501) staff       (20)      596 2023-04-15 11:12:44.000000 megabots-0.0.7/megabots/tests/test_ui.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.524775 megabots-0.0.7/megabots.egg-info/
--rw-r--r--   0 momegas    (501) staff       (20)     4430 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)      314 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/SOURCES.txt
--rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/dependency_links.txt
--rw-r--r--   0 momegas    (501) staff       (20)       63 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/requires.txt
--rw-r--r--   0 momegas    (501) staff       (20)        9 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/top_level.txt
--rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-15 11:30:54.525621 megabots-0.0.7/setup.cfg
--rw-r--r--   0 momegas    (501) staff       (20)      767 2023-04-15 11:30:44.000000 megabots-0.0.7/setup.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.451927 megabots-0.0.8/
+-rw-r--r--   0 momegas    (501) staff       (20)     1075 2023-04-14 20:57:02.000000 megabots-0.0.8/LICENCE
+-rw-r--r--   0 momegas    (501) staff       (20)     4784 2023-04-15 15:18:22.451791 megabots-0.0.8/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)     4311 2023-04-15 12:28:59.000000 megabots-0.0.8/README.md
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.449851 megabots-0.0.8/megabots/
+-rw-r--r--   0 momegas    (501) staff       (20)     7219 2023-04-15 15:17:29.000000 megabots-0.0.8/megabots/__init__.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.450607 megabots-0.0.8/megabots.egg-info/
+-rw-r--r--   0 momegas    (501) staff       (20)     4784 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)      278 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/SOURCES.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/dependency_links.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       63 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/requires.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       15 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/top_level.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-15 15:18:22.451969 megabots-0.0.8/setup.cfg
+-rw-r--r--   0 momegas    (501) staff       (20)      854 2023-04-15 15:18:13.000000 megabots-0.0.8/setup.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.451399 megabots-0.0.8/tests/
+-rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 megabots-0.0.8/tests/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)      593 2023-04-15 11:10:48.000000 megabots-0.0.8/tests/test_api.py
+-rw-r--r--   0 momegas    (501) staff       (20)     1423 2023-04-15 14:44:20.000000 megabots-0.0.8/tests/test_bots.py
+-rw-r--r--   0 momegas    (501) staff       (20)      596 2023-04-15 11:12:44.000000 megabots-0.0.8/tests/test_ui.py
```

### Comparing `megabots-0.0.7/LICENCE` & `megabots-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `megabots-0.0.7/PKG-INFO` & `megabots-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1
-Name: megabots
-Version: 0.0.7
-Summary: Create a question answering over docs bot with one line of code.
-Home-page: https://github.com/momegas/megabots
-Author: Megaklis Vasilakis
-Author-email: megaklis.vasilakis@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # 🤖 Megabots
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
 🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
 
+The Megabots library can be used to create bots that:
+
+- ⌚️ are production ready bots in minutes
+- 🗂️ can answer questions over documents
+- 🧑‍⚕️ can act personal assistants and use agents and tools (Coming soon)
+- 🗣️ can accept voice (Coming soon)
+- 👍 validate and correct the outputs of large language models (Coming soon)
+- 💰 semanticly cache LLM Queries and reduce your LLM API Costs by 10x (Coming soon)
+- 🏋️ are mega-easily to train (Coming soon)
+
+🤖 Megabots is backed by some of the most famous tools for productionalising AI. It uses [LangChain](https://docs.langchain.com/docs/) for managing LLM chains, [FastAPI](https://fastapi.tiangolo.com/) to create a production ready API, [Gradio](https://gradio.app/) to create a UI. At the moment it uses [OpenAI](https://openai.com/) to generate answers, but we plan to support other LLMs in the future.
+
 Note: This is a work in progress. The API might change.
 
 ```bash
 pip install megabots
 ```
 
 ```python
@@ -61,28 +60,14 @@
 
 ```python
 from megabots import bot, create_interface
 
 demo = create_interface(QnABot("qna-over-docs"))
 ```
 
-### Features
-
-- [x] Create a question answering bot over your documents with one line of code using GPT
-- [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
-- [x] Local data source (directory of documents) or S3 data source
-- [x] FAISS for storing vectors / index
-- [x] Expose bot over API using FastAPI
-- [x] Gradio UI
-- [ ] Integration with [guardrails](https://github.com/ShreyaR/guardrails)
-- [ ] Integration with [GPTCache](https://github.com/zilliztech/GPTCache)
-- [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
-- [ ] Customise prompt
-- [ ] Support for LLaMA model
-
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
 
 In simple terms, when you have a question, you first search for relevant documents. Then, you give the documents and the question to the language model to generate an answer. To make this work, you need your documents in a searchable format (an index). This process involves two main steps: (1) preparing your documents for easy querying, and (2) using the retrieval augmented generation method.
 
 `QnABot` uses FAISS to create an index of documents and GPT to generate answers.
@@ -111,9 +96,7 @@
     API ->> Vectorstore: Lookup documents in the index relevant to the question
     API ->> API: Construct a prompt from the question and any relevant documents
     API ->> LLM: Pass the prompt to the model
     LLM -->> API: Get response from model
     API -->> User: Return response
 
 ```
-
-
```

### Comparing `megabots-0.0.7/README.md` & `megabots-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,38 @@
+Metadata-Version: 2.1
+Name: megabots
+Version: 0.0.8
+Summary: 🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
+Home-page: https://github.com/momegas/megabots
+Author: Megaklis Vasilakis
+Author-email: megaklis.vasilakis@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # 🤖 Megabots
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
 🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
 
+The Megabots library can be used to create bots that:
+
+- ⌚️ are production ready bots in minutes
+- 🗂️ can answer questions over documents
+- 🧑‍⚕️ can act personal assistants and use agents and tools (Coming soon)
+- 🗣️ can accept voice (Coming soon)
+- 👍 validate and correct the outputs of large language models (Coming soon)
+- 💰 semanticly cache LLM Queries and reduce your LLM API Costs by 10x (Coming soon)
+- 🏋️ are mega-easily to train (Coming soon)
+
+🤖 Megabots is backed by some of the most famous tools for productionalising AI. It uses [LangChain](https://docs.langchain.com/docs/) for managing LLM chains, [FastAPI](https://fastapi.tiangolo.com/) to create a production ready API, [Gradio](https://gradio.app/) to create a UI. At the moment it uses [OpenAI](https://openai.com/) to generate answers, but we plan to support other LLMs in the future.
+
 Note: This is a work in progress. The API might change.
 
 ```bash
 pip install megabots
 ```
 
 ```python
@@ -48,28 +73,14 @@
 
 ```python
 from megabots import bot, create_interface
 
 demo = create_interface(QnABot("qna-over-docs"))
 ```
 
-### Features
-
-- [x] Create a question answering bot over your documents with one line of code using GPT
-- [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
-- [x] Local data source (directory of documents) or S3 data source
-- [x] FAISS for storing vectors / index
-- [x] Expose bot over API using FastAPI
-- [x] Gradio UI
-- [ ] Integration with [guardrails](https://github.com/ShreyaR/guardrails)
-- [ ] Integration with [GPTCache](https://github.com/zilliztech/GPTCache)
-- [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
-- [ ] Customise prompt
-- [ ] Support for LLaMA model
-
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
 
 In simple terms, when you have a question, you first search for relevant documents. Then, you give the documents and the question to the language model to generate an answer. To make this work, you need your documents in a searchable format (an index). This process involves two main steps: (1) preparing your documents for easy querying, and (2) using the retrieval augmented generation method.
 
 `QnABot` uses FAISS to create an index of documents and GPT to generate answers.
@@ -98,7 +109,9 @@
     API ->> Vectorstore: Lookup documents in the index relevant to the question
     API ->> API: Construct a prompt from the question and any relevant documents
     API ->> LLM: Pass the prompt to the model
     LLM -->> API: Get response from model
     API -->> User: Return response
 
 ```
+
+
```

### Comparing `megabots-0.0.7/megabots/tests/test_api.py` & `megabots-0.0.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `megabots-0.0.7/megabots/tests/test_bots.py` & `megabots-0.0.8/tests/test_bots.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 import tempfile
 from megabots import bot
 import pickle
 from langchain.vectorstores.faiss import FAISS
-from dotenv import load_dotenv
 
-load_dotenv()
 
 # Define test data
 test_directory = "./examples/files"
 test_question = "what was the first roster of avengers in comics?"
 correct_answer = "Iron Man, Thor, Hulk, Ant-Man"
 sources = "SOURCES:"
 
@@ -17,15 +15,15 @@
 def test_ask():
     qnabot = bot("qna-over-docs", index=test_directory)
     answer = qnabot.ask(test_question)
 
     # Assert that the answer contains the correct answer
     assert correct_answer in answer
     # Assert that the answer contains the sources
-    assert sources in answer
+    assert sources not in answer
 
 
 def test_save_load_index():
     # Create a temporary directory and file path for the test index
     with tempfile.TemporaryDirectory() as temp_dir:
         index_path = os.path.join(temp_dir, "test_index.pkl")
```

### Comparing `megabots-0.0.7/megabots/tests/test_ui.py` & `megabots-0.0.8/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `megabots-0.0.7/megabots.egg-info/PKG-INFO` & `megabots-0.0.8/megabots.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: megabots
-Version: 0.0.7
-Summary: Create a question answering over docs bot with one line of code.
+Version: 0.0.8
+Summary: 🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
 Home-page: https://github.com/momegas/megabots
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
@@ -13,14 +13,26 @@
 
 # 🤖 Megabots
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
 🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
 
+The Megabots library can be used to create bots that:
+
+- ⌚️ are production ready bots in minutes
+- 🗂️ can answer questions over documents
+- 🧑‍⚕️ can act personal assistants and use agents and tools (Coming soon)
+- 🗣️ can accept voice (Coming soon)
+- 👍 validate and correct the outputs of large language models (Coming soon)
+- 💰 semanticly cache LLM Queries and reduce your LLM API Costs by 10x (Coming soon)
+- 🏋️ are mega-easily to train (Coming soon)
+
+🤖 Megabots is backed by some of the most famous tools for productionalising AI. It uses [LangChain](https://docs.langchain.com/docs/) for managing LLM chains, [FastAPI](https://fastapi.tiangolo.com/) to create a production ready API, [Gradio](https://gradio.app/) to create a UI. At the moment it uses [OpenAI](https://openai.com/) to generate answers, but we plan to support other LLMs in the future.
+
 Note: This is a work in progress. The API might change.
 
 ```bash
 pip install megabots
 ```
 
 ```python
@@ -61,28 +73,14 @@
 
 ```python
 from megabots import bot, create_interface
 
 demo = create_interface(QnABot("qna-over-docs"))
 ```
 
-### Features
-
-- [x] Create a question answering bot over your documents with one line of code using GPT
-- [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
-- [x] Local data source (directory of documents) or S3 data source
-- [x] FAISS for storing vectors / index
-- [x] Expose bot over API using FastAPI
-- [x] Gradio UI
-- [ ] Integration with [guardrails](https://github.com/ShreyaR/guardrails)
-- [ ] Integration with [GPTCache](https://github.com/zilliztech/GPTCache)
-- [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
-- [ ] Customise prompt
-- [ ] Support for LLaMA model
-
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
 
 In simple terms, when you have a question, you first search for relevant documents. Then, you give the documents and the question to the language model to generate an answer. To make this work, you need your documents in a searchable format (an index). This process involves two main steps: (1) preparing your documents for easy querying, and (2) using the retrieval augmented generation method.
 
 `QnABot` uses FAISS to create an index of documents and GPT to generate answers.
```

### Comparing `megabots-0.0.7/setup.py` & `megabots-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 setup(
     name="megabots",
     version=VERSION,
     packages=find_packages(),
     install_requires=[
         "langchain",
@@ -12,15 +12,15 @@
         "unstructured",
         "fastapi",
         "faiss-cpu",
         "pdfminer.six",
     ],
     author="Megaklis Vasilakis",
     author_email="megaklis.vasilakis@gmail.com",
-    description="Create a question answering over docs bot with one line of code.",
+    description="🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/momegas/megabots",
     classifiers=[
         # Choose appropriate classifiers from
         # https://pypi.org/classifiers/
         "Development Status :: 4 - Beta"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

