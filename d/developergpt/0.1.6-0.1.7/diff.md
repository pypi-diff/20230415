# Comparing `tmp/developergpt-0.1.6.tar.gz` & `tmp/developergpt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.1.6.tar", last modified: Wed Apr 12 19:21:34 2023, max compression
+gzip compressed data, was "developergpt-0.1.7.tar", last modified: Sat Apr 15 19:20:48 2023, max compression
```

## Comparing `developergpt-0.1.6.tar` & `developergpt-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 19:21:25.000000 developergpt-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 19:21:25.000000 developergpt-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 19:21:34.556047 developergpt-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 19:21:25.000000 developergpt-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:21:34.556047 developergpt-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 19:21:25.000000 developergpt-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:25.000000 developergpt-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 19:21:25.000000 developergpt-0.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 19:21:25.000000 developergpt-0.1.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.444974 developergpt-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-15 19:20:35.000000 developergpt-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 19:20:35.000000 developergpt-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-15 19:20:48.440973 developergpt-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-15 19:20:35.000000 developergpt-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.440973 developergpt-0.1.7/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.440973 developergpt-0.1.7/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:20:48.444974 developergpt-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-15 19:20:35.000000 developergpt-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.440973 developergpt-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:35.000000 developergpt-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-15 19:20:35.000000 developergpt-0.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 19:20:35.000000 developergpt-0.1.7/tests/test_cli.py
```

### Comparing `developergpt-0.1.6/LICENSE` & `developergpt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.6/PKG-INFO` & `developergpt-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.1.6
+Version: 0.1.7
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -65,14 +65,17 @@
 $ developergpt chat
 
 # natural language to terminal commands using GPT-3.5 (default)
 $ developergpt cmd
 
 # natural langauge to terminal commands using BLOOM
 $ developergpt --model bloom cmd
+
+# give feedback
+$ developergpt feedback
 ```
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
@@ -80,13 +83,13 @@
 Currently, using the BLOOM model does not require a [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index) token and is free (but rate limited). 
 
 ## Contributing
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
-- Add support for more open-source models (Vicuna-13B?)
+- Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
 - This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.1.6/README.md` & `developergpt-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,17 @@
 $ developergpt chat
 
 # natural language to terminal commands using GPT-3.5 (default)
 $ developergpt cmd
 
 # natural langauge to terminal commands using BLOOM
 $ developergpt --model bloom cmd
+
+# give feedback
+$ developergpt feedback
 ```
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
@@ -69,13 +72,13 @@
 Currently, using the BLOOM model does not require a [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index) token and is free (but rate limited). 
 
 ## Contributing
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
-- Add support for more open-source models (Vicuna-13B?)
+- Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
 - This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.1.6/developergpt/cli.py` & `developergpt-0.1.7/developergpt/cli.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.6/developergpt/config.py` & `developergpt-0.1.7/developergpt/config.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.6/developergpt/huggingface_adapter.py` & `developergpt-0.1.7/developergpt/huggingface_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.6/developergpt/openai_adapter.py` & `developergpt-0.1.7/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.6/developergpt/utils.py` & `developergpt-0.1.7/developergpt/utils.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.6/developergpt.egg-info/PKG-INFO` & `developergpt-0.1.7/developergpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.1.6
+Version: 0.1.7
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -65,14 +65,17 @@
 $ developergpt chat
 
 # natural language to terminal commands using GPT-3.5 (default)
 $ developergpt cmd
 
 # natural langauge to terminal commands using BLOOM
 $ developergpt --model bloom cmd
+
+# give feedback
+$ developergpt feedback
 ```
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
@@ -80,13 +83,13 @@
 Currently, using the BLOOM model does not require a [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index) token and is free (but rate limited). 
 
 ## Contributing
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
-- Add support for more open-source models (Vicuna-13B?)
+- Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
 - Thanks to Hugging Face and the NLP community for open-source models! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
 - This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.1.6/developergpt.egg-info/SOURCES.txt` & `developergpt-0.1.7/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.6/setup.py` & `developergpt-0.1.7/setup.py`

 * *Files identical despite different names*

