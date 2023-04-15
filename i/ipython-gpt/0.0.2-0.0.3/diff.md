# Comparing `tmp/ipython-gpt-0.0.2.tar.gz` & `tmp/ipython-gpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-gpt-0.0.2.tar", last modified: Sat Apr 15 09:59:31 2023, max compression
+gzip compressed data, was "ipython-gpt-0.0.3.tar", last modified: Sat Apr 15 14:12:24 2023, max compression
```

## Comparing `ipython-gpt-0.0.2.tar` & `ipython-gpt-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3502 2023-04-15 09:30:32.494265 ipython-gpt-0.0.2/README.md
--rw-r--r--   0        0        0     5265 2023-04-15 09:40:59.930200 ipython-gpt-0.0.2/ipython_gpt.py
--rw-r--r--   0        0        0      756 2023-04-15 09:59:27.195085 ipython-gpt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4277 2023-04-15 09:59:31.988748 ipython-gpt-0.0.2/setup.py
--rw-r--r--   0        0        0     4251 2023-04-15 09:59:31.989167 ipython-gpt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3502 2023-04-15 09:30:32.494265 ipython-gpt-0.0.3/README.md
+-rw-r--r--   0        0        0     5356 2023-04-15 14:11:46.336819 ipython-gpt-0.0.3/ipython_gpt.py
+-rw-r--r--   0        0        0      756 2023-04-15 14:12:11.596403 ipython-gpt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4277 2023-04-15 14:12:24.189638 ipython-gpt-0.0.3/setup.py
+-rw-r--r--   0        0        0     4251 2023-04-15 14:12:24.190082 ipython-gpt-0.0.3/PKG-INFO
```

### Comparing `ipython-gpt-0.0.2/README.md` & `ipython-gpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ipython-gpt-0.0.2/ipython_gpt.py` & `ipython-gpt-0.0.3/ipython_gpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         self.default_model = "gpt-3.5-turbo"
         self.default_system_message = "You're a python data science coding assistant"
 
         self.message_history = []
 
     def display_notebook(self, message):
-        display(Markdown(message))
+        display(Markdown(f"<div style='width:60%;margin-left:5%;overflow: scroll;max-height:500px'>\n\n{message}\n\n</div>"))
 
     def display_shell(self, message):
         display(message)
 
     def display(self, message):
         method_name = DISPLAY_METHODS.get(
             ipy.get_ipython().__class__.__name__, "display_shell")
```

### Comparing `ipython-gpt-0.0.2/pyproject.toml` & `ipython-gpt-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipython-gpt"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Jupyter/IPython extension to use ChatGPT"
 authors = ["Santiago Basulto <santiago.basulto@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/santiagobasulto/ipython-gpt"
 repository = "https://github.com/santiagobasulto/ipython-gpt"
 keywords = ["ipython", "jupyter", "chatgpt", "openai"]
 classifiers = [
```

### Comparing `ipython-gpt-0.0.2/setup.py` & `ipython-gpt-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['ipython_gpt']
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'ipython-gpt',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'A Jupyter/IPython extension to use ChatGPT',
     'long_description': '# IPython ChatGPT extension\n\nThis extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell.\n\n**Important!** This is a very early and raw version, I have a lot of things to improve about the code and missing functionality.\n\n## Installation\n```python\n!pip install ipython-gpt\n```\n\nThen in your notebook or ipython shell:\n\n```ipython\n%load_ext ipython_gpt\n```\n\n## Setup\n\nYou must first generate an API key at OpenAI (https://platform.openai.com/account/api-keys) and set is an environment variable `OPENAI_API_KEY`. You can do it by modifying your `.bashrc/.zshrc` or starting jupyter with it:\n\n```bash\n$ OPENAI_API_KEY=[YOUR-KEY] jupyter lab\n```\n\nThere are a few other ways to set the API KEY, but the envvar is the recommended one.\n\n## ChatGPT API\n\nThe command `%%chat` interfaces with ChatGPT. It accepts multiple parameters (see Usage). Here\'s an example:\n\n\n```python\n%%chat --max-tokens=25\n\nWhat\'s the purpose of life?\n...\n\n>>> CHAT RESPONSE\n```\n\n**Important** by default, the `%%chat` command preserves the conversation to give the Agent some context, in the same way that ChatGPT works. You can "reset" its status passing the flag `--reset-conversation`.\n\n\n```python\n%%chat --reset-conversation\n\nHow can I avoid pandas using scientific notation in outputs, and do it globally?\n...\n...\n>>> CHAT RESPONSE\n```\n\n## Agent\'s role (system message) and other chat parameters\n\nBy default, the Chat is started with the role: *"You\'re a python data science coding assistant"*. You can change that by passing something different in your first `%%chat`:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant"\n\nYour message...\n```\n\nOnce the conversation has started, you can\'t change the original message, as the context is preserved. To do so, you must reset the conversation:\n\n```ipython\n%%chat --system-message="You\'re a R Data Science assistant" --reset-conversation\n\nYour message...\n```\n\n## Setting global config\n\nYou can change the defaults using the `%chat_config` line magic:\n\n```ipython\n%chat_config --system-message="You\'re an R data scientist coding assistant specialized in visualizations" --model "other model" --reset-conversation\n```\n\nInvoke it without parameters to see the defaults set:\n\n\n```python\n%chat_config\n...\n\n>>>\n##### Conf set:\n\n* **Default model**: gpt-3.5-turbo\n* **Default system message**: You\'re a python data science coding assistant\n* **Chat history length**: 0\n```\n\n\n## Other methods\n\n#### Display available models\n\nUsage:\n```bash\n%chat_models [--all-models]\n```\n\n\n```python\n%chat_models\n```\n\n\n##### Available models:\n\n\t- gpt-3.5-turbo-0301\n\t- gpt-3.5-turbo\n\n\n#### Display usage and accepted parameters\n\n\n```python\n%reload_ext ipython_gpt\n%chat_help\n...\n\n\n    usage: ipykernel_launcher.py [-h] [--openai-api-key OPENAI_API_KEY]\n                                 [--reset-conversation]\n                                 [--system-message SYSTEM_MESSAGE]\n                                 [--no-system-message] [--model MODEL]\n                                 [--temperature TEMPERATURE]\n                                 [--max-tokens MAX_TOKENS] [--all-models]\n\n```\n\n## Alternative authentication\n\nAside from setting the environment variable, you can also set `OPENAI_API_KEY` as a global variable in your notebook, or pass it directly as a parameter in any method ``--openai-api-key=YOUR-KEY`.\n\nThese alternative methods are NOT recommended, as you might leak your API Key in the notebooks\' history, stored in `.ipynb_checkpoints`.\n',
     'author': 'Santiago Basulto',
     'author_email': 'santiago.basulto@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/santiagobasulto/ipython-gpt',
```

### Comparing `ipython-gpt-0.0.2/PKG-INFO` & `ipython-gpt-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-gpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Jupyter/IPython extension to use ChatGPT
 Home-page: https://github.com/santiagobasulto/ipython-gpt
 Keywords: ipython,jupyter,chatgpt,openai
 Author: Santiago Basulto
 Author-email: santiago.basulto@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

