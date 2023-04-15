# Comparing `tmp/megabots-0.0.6.tar.gz` & `tmp/megabots-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megabots-0.0.6.tar", last modified: Sat Apr 15 08:53:46 2023, max compression
+gzip compressed data, was "megabots-0.0.7.tar", last modified: Sat Apr 15 11:30:54 2023, max compression
```

## Comparing `megabots-0.0.6.tar` & `megabots-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 08:53:46.811348 megabots-0.0.6/
--rw-r--r--   0 momegas    (501) staff       (20)     1075 2023-04-14 20:57:02.000000 megabots-0.0.6/LICENCE
--rw-r--r--   0 momegas    (501) staff       (20)     4243 2023-04-15 08:53:46.810710 megabots-0.0.6/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)     3857 2023-04-15 08:35:06.000000 megabots-0.0.6/README.md
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 08:53:46.799628 megabots-0.0.6/megabots.egg-info/
--rw-r--r--   0 momegas    (501) staff       (20)     4243 2023-04-15 08:53:46.000000 megabots-0.0.6/megabots.egg-info/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)      350 2023-04-15 08:53:46.000000 megabots-0.0.6/megabots.egg-info/SOURCES.txt
--rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-15 08:53:46.000000 megabots-0.0.6/megabots.egg-info/dependency_links.txt
--rw-r--r--   0 momegas    (501) staff       (20)       63 2023-04-15 08:53:46.000000 megabots-0.0.6/megabots.egg-info/requires.txt
--rw-r--r--   0 momegas    (501) staff       (20)        7 2023-04-15 08:53:46.000000 megabots-0.0.6/megabots.egg-info/top_level.txt
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 08:53:46.804983 megabots-0.0.6/qnabot/
--rw-r--r--   0 momegas    (501) staff       (20)     3060 2023-04-14 17:27:00.000000 megabots-0.0.6/qnabot/QnABot.py
--rw-r--r--   0 momegas    (501) staff       (20)       88 2023-04-14 17:25:24.000000 megabots-0.0.6/qnabot/__init__.py
--rw-r--r--   0 momegas    (501) staff       (20)      260 2023-04-14 17:32:35.000000 megabots-0.0.6/qnabot/api.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 08:53:46.808823 megabots-0.0.6/qnabot/tests/
--rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 megabots-0.0.6/qnabot/tests/__init__.py
--rw-r--r--   0 momegas    (501) staff       (20)     1463 2023-04-14 17:29:48.000000 megabots-0.0.6/qnabot/tests/test_QnABot.py
--rw-r--r--   0 momegas    (501) staff       (20)      578 2023-04-14 12:48:59.000000 megabots-0.0.6/qnabot/tests/test_api.py
--rw-r--r--   0 momegas    (501) staff       (20)      597 2023-04-14 17:34:04.000000 megabots-0.0.6/qnabot/tests/test_ui.py
--rw-r--r--   0 momegas    (501) staff       (20)      407 2023-04-14 20:54:08.000000 megabots-0.0.6/qnabot/ui.py
--rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-15 08:53:46.811423 megabots-0.0.6/setup.cfg
--rw-r--r--   0 momegas    (501) staff       (20)      767 2023-04-15 08:53:39.000000 megabots-0.0.6/setup.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.525576 megabots-0.0.7/
+-rw-r--r--   0 momegas    (501) staff       (20)     1075 2023-04-14 20:57:02.000000 megabots-0.0.7/LICENCE
+-rw-r--r--   0 momegas    (501) staff       (20)     4430 2023-04-15 11:30:54.525429 megabots-0.0.7/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)     4044 2023-04-15 11:28:29.000000 megabots-0.0.7/README.md
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.524172 megabots-0.0.7/megabots/
+-rw-r--r--   0 momegas    (501) staff       (20)     5290 2023-04-15 11:09:34.000000 megabots-0.0.7/megabots/__init__.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.525231 megabots-0.0.7/megabots/tests/
+-rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 megabots-0.0.7/megabots/tests/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)      593 2023-04-15 11:10:48.000000 megabots-0.0.7/megabots/tests/test_api.py
+-rw-r--r--   0 momegas    (501) staff       (20)     1464 2023-04-15 11:11:24.000000 megabots-0.0.7/megabots/tests/test_bots.py
+-rw-r--r--   0 momegas    (501) staff       (20)      596 2023-04-15 11:12:44.000000 megabots-0.0.7/megabots/tests/test_ui.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 11:30:54.524775 megabots-0.0.7/megabots.egg-info/
+-rw-r--r--   0 momegas    (501) staff       (20)     4430 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)      314 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/SOURCES.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/dependency_links.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       63 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/requires.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        9 2023-04-15 11:30:54.000000 megabots-0.0.7/megabots.egg-info/top_level.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-15 11:30:54.525621 megabots-0.0.7/setup.cfg
+-rw-r--r--   0 momegas    (501) staff       (20)      767 2023-04-15 11:30:44.000000 megabots-0.0.7/setup.py
```

### Comparing `megabots-0.0.6/LICENCE` & `megabots-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `megabots-0.0.6/PKG-INFO` & `megabots-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 Metadata-Version: 2.1
 Name: megabots
-Version: 0.0.6
+Version: 0.0.7
 Summary: Create a question answering over docs bot with one line of code.
 Home-page: https://github.com/momegas/megabots
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# QnA Bot
+# 🤖 Megabots
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
-Here is an example of what you build with this library: [Demo](https://huggingface.co/spaces/momegas/megas-bot)
+🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
 
-Create a question answering over docs bot with one line of code:
+Note: This is a work in progress. The API might change.
 
 ```bash
-pip install qnabot
+pip install megabots
 ```
 
 ```python
-from qnabot import QnABot
+from megabots import bot
 import os
 
 os.environ["OPENAI_API_KEY"] = "my key"
 
-# Create a bot 👉 with one line of code
-bot = QnABot(directory="./mydata")
+# Create a bot 👉 with one line of code. Automatically loads your data from ./index or index.pkl.
+qnabot = bot("qna-over-docs")
 
 # Ask a question
 answer = bot.ask("How do I use this bot?")
 
 # Save the index to save costs (GPT is used to create the index)
-bot.save_index("index.pickle")
+bot.save_index("index.pkl")
 
 # Load the index from a previous run
-bot = QnABot(directory="./mydata", index="index.pickle")
+qnabot = bot("qna-over-docs", index="./index.pkl")
+
+# Or create the index from a directory of documents
+qnabot = bot("qna-over-docs", index="./index")
 ```
 
 You can also create a FastAPI app that will expose the bot as an API using the create_app function.
 Assuming you file is called `main.py` run `uvicorn main:app --reload` to run the API locally.
 You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
 
 ```python
-from qnabot import QnABot, create_app
+from megabots import bot, create_api
 
-app = create_app(QnABot("./mydata"))
+app = create_app(bot("qna-over-docs"))
 ```
 
 You can expose a gradio UI for the bot using `create_interface` function.
 Assuming your file is called `ui.py` run `gradio qnabot/ui.py` to run the UI locally.
 You should then be able to visit `http://127.0.0.1:7860` to see the API documentation.
 
 ```python
-from qnabot import QnABot, create_interface
+from megabots import bot, create_interface
 
-demo = create_interface(QnABot("./mydata"))
+demo = create_interface(QnABot("qna-over-docs"))
 ```
 
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
```

### Comparing `megabots-0.0.6/README.md` & `megabots-0.0.7/megabots.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,72 @@
-# QnA Bot
+Metadata-Version: 2.1
+Name: megabots
+Version: 0.0.7
+Summary: Create a question answering over docs bot with one line of code.
+Home-page: https://github.com/momegas/megabots
+Author: Megaklis Vasilakis
+Author-email: megaklis.vasilakis@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# 🤖 Megabots
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
-Here is an example of what you build with this library: [Demo](https://huggingface.co/spaces/momegas/megas-bot)
+🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
 
-Create a question answering over docs bot with one line of code:
+Note: This is a work in progress. The API might change.
 
 ```bash
-pip install qnabot
+pip install megabots
 ```
 
 ```python
-from qnabot import QnABot
+from megabots import bot
 import os
 
 os.environ["OPENAI_API_KEY"] = "my key"
 
-# Create a bot 👉 with one line of code
-bot = QnABot(directory="./mydata")
+# Create a bot 👉 with one line of code. Automatically loads your data from ./index or index.pkl.
+qnabot = bot("qna-over-docs")
 
 # Ask a question
 answer = bot.ask("How do I use this bot?")
 
 # Save the index to save costs (GPT is used to create the index)
-bot.save_index("index.pickle")
+bot.save_index("index.pkl")
 
 # Load the index from a previous run
-bot = QnABot(directory="./mydata", index="index.pickle")
+qnabot = bot("qna-over-docs", index="./index.pkl")
+
+# Or create the index from a directory of documents
+qnabot = bot("qna-over-docs", index="./index")
 ```
 
 You can also create a FastAPI app that will expose the bot as an API using the create_app function.
 Assuming you file is called `main.py` run `uvicorn main:app --reload` to run the API locally.
 You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
 
 ```python
-from qnabot import QnABot, create_app
+from megabots import bot, create_api
 
-app = create_app(QnABot("./mydata"))
+app = create_app(bot("qna-over-docs"))
 ```
 
 You can expose a gradio UI for the bot using `create_interface` function.
 Assuming your file is called `ui.py` run `gradio qnabot/ui.py` to run the UI locally.
 You should then be able to visit `http://127.0.0.1:7860` to see the API documentation.
 
 ```python
-from qnabot import QnABot, create_interface
+from megabots import bot, create_interface
 
-demo = create_interface(QnABot("./mydata"))
+demo = create_interface(QnABot("qna-over-docs"))
 ```
 
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
@@ -95,7 +111,9 @@
     API ->> Vectorstore: Lookup documents in the index relevant to the question
     API ->> API: Construct a prompt from the question and any relevant documents
     API ->> LLM: Pass the prompt to the model
     LLM -->> API: Get response from model
     API -->> User: Return response
 
 ```
+
+
```

### Comparing `megabots-0.0.6/megabots.egg-info/PKG-INFO` & `megabots-0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,59 @@
-Metadata-Version: 2.1
-Name: megabots
-Version: 0.0.6
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
-# QnA Bot
+# 🤖 Megabots
 
 [![Tests](https://github.com/momegas/qnabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/momegas/qnabot/actions/workflows/python-package.yml)
 
-Here is an example of what you build with this library: [Demo](https://huggingface.co/spaces/momegas/megas-bot)
+🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵
 
-Create a question answering over docs bot with one line of code:
+Note: This is a work in progress. The API might change.
 
 ```bash
-pip install qnabot
+pip install megabots
 ```
 
 ```python
-from qnabot import QnABot
+from megabots import bot
 import os
 
 os.environ["OPENAI_API_KEY"] = "my key"
 
-# Create a bot 👉 with one line of code
-bot = QnABot(directory="./mydata")
+# Create a bot 👉 with one line of code. Automatically loads your data from ./index or index.pkl.
+qnabot = bot("qna-over-docs")
 
 # Ask a question
 answer = bot.ask("How do I use this bot?")
 
 # Save the index to save costs (GPT is used to create the index)
-bot.save_index("index.pickle")
+bot.save_index("index.pkl")
 
 # Load the index from a previous run
-bot = QnABot(directory="./mydata", index="index.pickle")
+qnabot = bot("qna-over-docs", index="./index.pkl")
+
+# Or create the index from a directory of documents
+qnabot = bot("qna-over-docs", index="./index")
 ```
 
 You can also create a FastAPI app that will expose the bot as an API using the create_app function.
 Assuming you file is called `main.py` run `uvicorn main:app --reload` to run the API locally.
 You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
 
 ```python
-from qnabot import QnABot, create_app
+from megabots import bot, create_api
 
-app = create_app(QnABot("./mydata"))
+app = create_app(bot("qna-over-docs"))
 ```
 
 You can expose a gradio UI for the bot using `create_interface` function.
 Assuming your file is called `ui.py` run `gradio qnabot/ui.py` to run the UI locally.
 You should then be able to visit `http://127.0.0.1:7860` to see the API documentation.
 
 ```python
-from qnabot import QnABot, create_interface
+from megabots import bot, create_interface
 
-demo = create_interface(QnABot("./mydata"))
+demo = create_interface(QnABot("qna-over-docs"))
 ```
 
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
@@ -108,9 +98,7 @@
     API ->> Vectorstore: Lookup documents in the index relevant to the question
     API ->> API: Construct a prompt from the question and any relevant documents
     API ->> LLM: Pass the prompt to the model
     LLM -->> API: Get response from model
     API -->> User: Return response
 
 ```
-
-
```

### Comparing `megabots-0.0.6/qnabot/tests/test_QnABot.py` & `megabots-0.0.7/megabots/tests/test_bots.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import os
 import tempfile
-from qnabot import QnABot
+from megabots import bot
 import pickle
 from langchain.vectorstores.faiss import FAISS
 from dotenv import load_dotenv
 
 load_dotenv()
 
 # Define test data
 test_directory = "./examples/files"
 test_question = "what was the first roster of avengers in comics?"
 correct_answer = "Iron Man, Thor, Hulk, Ant-Man"
 sources = "SOURCES:"
 
 
 def test_ask():
-    bot = QnABot(directory=test_directory)
-    answer = bot.ask(test_question)
+    qnabot = bot("qna-over-docs", index=test_directory)
+    answer = qnabot.ask(test_question)
 
     # Assert that the answer contains the correct answer
     assert correct_answer in answer
     # Assert that the answer contains the sources
     assert sources in answer
 
 
 def test_save_load_index():
     # Create a temporary directory and file path for the test index
     with tempfile.TemporaryDirectory() as temp_dir:
         index_path = os.path.join(temp_dir, "test_index.pkl")
 
         # Create a bot and save the index to the temporary file path
-        bot = QnABot(directory=test_directory, index=index_path)
-        bot.save_index(index_path)
+        qnabot = bot("qna-over-docs", index=test_directory)
+        qnabot.save_index(index_path)
 
         # Load the saved index and assert that it is the same as the original index
         with open(index_path, "rb") as f:
             saved_index = pickle.load(f)
         assert isinstance(saved_index, FAISS)
 
-        bot_with_predefined_index = QnABot(directory=test_directory, index=index_path)
+        bot_with_predefined_index = bot("qna-over-docs", index=index_path)
 
         # Assert that the bot returns the correct answer to the test question
         assert correct_answer in bot_with_predefined_index.ask(test_question)
```

### Comparing `megabots-0.0.6/qnabot/tests/test_ui.py` & `megabots-0.0.7/megabots/tests/test_ui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gradio as gr
-from qnabot import create_interface
+from megabots import create_interface
 
 
 def test_create_interface():
-    # create a mock QnABot object
+    # create a mock Bot object
     class MockBot:
         def ask(self, question: str):
             return "Answer"
 
     # create a mock example
     example = [["What is your name?"], ["My name is Bot."]]
```

