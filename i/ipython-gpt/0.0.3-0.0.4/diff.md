# Comparing `tmp/ipython-gpt-0.0.3.tar.gz` & `tmp/ipython-gpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-gpt-0.0.3.tar", last modified: Sat Apr 15 14:12:24 2023, max compression
+gzip compressed data, was "ipython-gpt-0.0.4.tar", last modified: Sat Apr 15 14:29:09 2023, max compression
```

## Comparing `ipython-gpt-0.0.3.tar` & `ipython-gpt-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3502 2023-04-15 09:30:32.494265 ipython-gpt-0.0.3/README.md
--rw-r--r--   0        0        0     5356 2023-04-15 14:11:46.336819 ipython-gpt-0.0.3/ipython_gpt.py
--rw-r--r--   0        0        0      756 2023-04-15 14:12:11.596403 ipython-gpt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4277 2023-04-15 14:12:24.189638 ipython-gpt-0.0.3/setup.py
--rw-r--r--   0        0        0     4251 2023-04-15 14:12:24.190082 ipython-gpt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3922 2023-04-15 14:28:41.986114 ipython-gpt-0.0.4/README.md
+-rw-r--r--   0        0        0     5354 2023-04-15 14:22:53.034120 ipython-gpt-0.0.4/ipython_gpt.py
+-rw-r--r--   0        0        0      756 2023-04-15 14:28:24.646013 ipython-gpt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4703 2023-04-15 14:29:09.825156 ipython-gpt-0.0.4/setup.py
+-rw-r--r--   0        0        0     4671 2023-04-15 14:29:09.825564 ipython-gpt-0.0.4/PKG-INFO
```

### Comparing `ipython-gpt-0.0.3/README.md` & `ipython-gpt-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # IPython ChatGPT extension
 
 This extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell.
 
-**Important!** This is a very early and raw version, I have a lot of things to improve about the code and missing functionality.
+<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">
+
+<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">
+
+**Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality.
 
 ## Installation
 ```python
 !pip install ipython-gpt
 ```
 
 Then in your notebook or ipython shell:
@@ -17,14 +21,16 @@
 
 ## Setup
 
 You must first generate an API key at OpenAI (https://platform.openai.com/account/api-keys) and set is an environment variable `OPENAI_API_KEY`. You can do it by modifying your `.bashrc/.zshrc` or starting jupyter with it:
 
 ```bash
 $ OPENAI_API_KEY=[YOUR-KEY] jupyter lab
+# ...
+$ OPENAI_API_KEY=[YOUR-KEY] ipython
 ```
 
 There are a few other ways to set the API KEY, but the envvar is the recommended one.
 
 ## ChatGPT API
 
 The command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here's an example:
```

### Comparing `ipython-gpt-0.0.3/ipython_gpt.py` & `ipython-gpt-0.0.4/ipython_gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         self.message_history = []
 
     def display_notebook(self, message):
         display(Markdown(f"<div style='width:60%;margin-left:5%;overflow: scroll;max-height:500px'>\n\n{message}\n\n</div>"))
 
     def display_shell(self, message):
-        display(message)
+        print(message)
 
     def display(self, message):
         method_name = DISPLAY_METHODS.get(
             ipy.get_ipython().__class__.__name__, "display_shell")
         getattr(self, method_name)(message)
 
     @cell_magic
```

### Comparing `ipython-gpt-0.0.3/pyproject.toml` & `ipython-gpt-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipython-gpt"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Jupyter/IPython extension to use ChatGPT"
 authors = ["Santiago Basulto <santiago.basulto@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/santiagobasulto/ipython-gpt"
 repository = "https://github.com/santiagobasulto/ipython-gpt"
 keywords = ["ipython", "jupyter", "chatgpt", "openai"]
 classifiers = [
```

### Comparing `ipython-gpt-0.0.3/setup.py` & `ipython-gpt-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 modules = \
 ['ipython_gpt']
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'ipython-gpt',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'A Jupyter/IPython extension to use ChatGPT',
-    'long_description': '# IPython ChatGPT extension\n\nThis extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell.\n\n**Important!** This is a very early and raw version, I have a lot of things to improve about the code and missing functionality.\n\n## Installation\n```python\n!pip install ipython-gpt\n```\n\nThen in your notebook or ipython shell:\n\n```ipython\n%load_ext ipython_gpt\n```\n\n## Setup\n\nYou must first generate an API key at OpenAI (https://platform.openai.com/account/api-keys) and set is an environment variable `OPENAI_API_KEY`. You can do it by modifying your `.bashrc/.zshrc` or starting jupyter with it:\n\n```bash\n$ OPENAI_API_KEY=[YOUR-KEY] jupyter lab\n```\n\nThere are a few other ways to set the API KEY, but the envvar is the recommended one.\n\n## ChatGPT API\n\nThe command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here\'s an example:\n\n\n```python\n%%chat --max-tokens=25\n\nWhat\'s the purpose of life?\n...\n\n>>> CHAT RESPONSE\n```\n\n**Important** by default, the `%%chat` command preserves the conversation to give the Agent some context, in the same way that ChatGPT works. You can "reset" its status passing the flag `--reset-conversation`.\n\n\n```python\n%%chat --reset-conversation\n\nHow can I avoid pandas using scientific notation in outputs, and do it globally?\n...\n...\n>>> CHAT RESPONSE\n```\n\n## Agent\'s role (system message) and other chat parameters\n\nBy default, the Chat is started with the role: *"You\'re a python data science coding assistant"*. You can change that by passing something different in your first `%%chat`:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant"\n\nYour message...\n```\n\nOnce the conversation has started, you can\'t change the original message, as the context is preserved. To do so, you must reset the conversation:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant" --reset-conversation\n\nYour message...\n```\n\n## Setting global config\n\nYou can change the defaults using the `%chat_config` line magic:\n\n```ipython\n%chat_config --system-message="You\'re an R data scientist coding assistant specialized in visualizations" --model "other model" --reset-conversation\n```\n\nInvoke it without parameters to see the defaults set:\n\n\n```python\n%chat_config\n...\n\n>>>\n##### Conf set:\n\n* **Default model**: gpt-3.5-turbo\n* **Default system message**: You\'re a python data science coding assistant\n* **Chat history length**: 0\n```\n\n\n## Other methods\n\n#### Display available models\n\nUsage:\n```bash\n%chat_models [--all-models]\n```\n\n\n```python\n%chat_models\n```\n\n\n##### Available models:\n\n\t- gpt-3.5-turbo-0301\n\t- gpt-3.5-turbo\n\n\n#### Display usage and accepted parameters\n\n\n```python\n%reload_ext ipython_gpt\n%chat_help\n...\n\n\n    usage: ipykernel_launcher.py [-h] [--openai-api-key OPENAI_API_KEY]\n                                 [--reset-conversation]\n                                 [--system-message SYSTEM_MESSAGE]\n                                 [--no-system-message] [--model MODEL]\n                                 [--temperature TEMPERATURE]\n                                 [--max-tokens MAX_TOKENS] [--all-models]\n\n```\n\n## Alternative authentication\n\nAside from setting the environment variable, you can also set `OPENAI_API_KEY` as a global variable in your notebook, or pass it directly as a parameter in any method ``--openai-api-key=YOUR-KEY`.\n\nThese alternative methods are NOT recommended, as you might leak your API Key in the notebooks\' history, stored in `.ipynb_checkpoints`.\n',
+    'long_description': '# IPython ChatGPT extension\n\nThis extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell.\n\n<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">\n\n<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">\n\n**Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality.\n\n## Installation\n```python\n!pip install ipython-gpt\n```\n\nThen in your notebook or ipython shell:\n\n```ipython\n%load_ext ipython_gpt\n```\n\n## Setup\n\nYou must first generate an API key at OpenAI (https://platform.openai.com/account/api-keys) and set is an environment variable `OPENAI_API_KEY`. You can do it by modifying your `.bashrc/.zshrc` or starting jupyter with it:\n\n```bash\n$ OPENAI_API_KEY=[YOUR-KEY] jupyter lab\n# ...\n$ OPENAI_API_KEY=[YOUR-KEY] ipython\n```\n\nThere are a few other ways to set the API KEY, but the envvar is the recommended one.\n\n## ChatGPT API\n\nThe command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here\'s an example:\n\n\n```python\n%%chat --max-tokens=25\n\nWhat\'s the purpose of life?\n...\n\n>>> CHAT RESPONSE\n```\n\n**Important** by default, the `%%chat` command preserves the conversation to give the Agent some context, in the same way that ChatGPT works. You can "reset" its status passing the flag `--reset-conversation`.\n\n\n```python\n%%chat --reset-conversation\n\nHow can I avoid pandas using scientific notation in outputs, and do it globally?\n...\n...\n>>> CHAT RESPONSE\n```\n\n## Agent\'s role (system message) and other chat parameters\n\nBy default, the Chat is started with the role: *"You\'re a python data science coding assistant"*. You can change that by passing something different in your first `%%chat`:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant"\n\nYour message...\n```\n\nOnce the conversation has started, you can\'t change the original message, as the context is preserved. To do so, you must reset the conversation:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant" --reset-conversation\n\nYour message...\n```\n\n## Setting global config\n\nYou can change the defaults using the `%chat_config` line magic:\n\n```ipython\n%chat_config --system-message="You\'re an R data scientist coding assistant specialized in visualizations" --model "other model" --reset-conversation\n```\n\nInvoke it without parameters to see the defaults set:\n\n\n```python\n%chat_config\n...\n\n>>>\n##### Conf set:\n\n* **Default model**: gpt-3.5-turbo\n* **Default system message**: You\'re a python data science coding assistant\n* **Chat history length**: 0\n```\n\n\n## Other methods\n\n#### Display available models\n\nUsage:\n```bash\n%chat_models [--all-models]\n```\n\n\n```python\n%chat_models\n```\n\n\n##### Available models:\n\n\t- gpt-3.5-turbo-0301\n\t- gpt-3.5-turbo\n\n\n#### Display usage and accepted parameters\n\n\n```python\n%reload_ext ipython_gpt\n%chat_help\n...\n\n\n    usage: ipykernel_launcher.py [-h] [--openai-api-key OPENAI_API_KEY]\n                                 [--reset-conversation]\n                                 [--system-message SYSTEM_MESSAGE]\n                                 [--no-system-message] [--model MODEL]\n                                 [--temperature TEMPERATURE]\n                                 [--max-tokens MAX_TOKENS] [--all-models]\n\n```\n\n## Alternative authentication\n\nAside from setting the environment variable, you can also set `OPENAI_API_KEY` as a global variable in your notebook, or pass it directly as a parameter in any method ``--openai-api-key=YOUR-KEY`.\n\nThese alternative methods are NOT recommended, as you might leak your API Key in the notebooks\' history, stored in `.ipynb_checkpoints`.\n',
     'author': 'Santiago Basulto',
     'author_email': 'santiago.basulto@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/santiagobasulto/ipython-gpt',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `ipython-gpt-0.0.3/PKG-INFO` & `ipython-gpt-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-gpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Jupyter/IPython extension to use ChatGPT
 Home-page: https://github.com/santiagobasulto/ipython-gpt
 Keywords: ipython,jupyter,chatgpt,openai
 Author: Santiago Basulto
 Author-email: santiago.basulto@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,19 @@
 Project-URL: Repository, https://github.com/santiagobasulto/ipython-gpt
 Description-Content-Type: text/markdown
 
 # IPython ChatGPT extension
 
 This extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell.
 
-**Important!** This is a very early and raw version, I have a lot of things to improve about the code and missing functionality.
+<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">
+
+<img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">
+
+**Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality.
 
 ## Installation
 ```python
 !pip install ipython-gpt
 ```
 
 Then in your notebook or ipython shell:
@@ -37,14 +41,16 @@
 
 ## Setup
 
 You must first generate an API key at OpenAI (https://platform.openai.com/account/api-keys) and set is an environment variable `OPENAI_API_KEY`. You can do it by modifying your `.bashrc/.zshrc` or starting jupyter with it:
 
 ```bash
 $ OPENAI_API_KEY=[YOUR-KEY] jupyter lab
+# ...
+$ OPENAI_API_KEY=[YOUR-KEY] ipython
 ```
 
 There are a few other ways to set the API KEY, but the envvar is the recommended one.
 
 ## ChatGPT API
 
 The command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here's an example:
```

