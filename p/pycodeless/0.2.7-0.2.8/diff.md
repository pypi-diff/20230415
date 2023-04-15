# Comparing `tmp/pycodeless-0.2.7.tar.gz` & `tmp/pycodeless-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodeless-0.2.7.tar", max compression
+gzip compressed data, was "pycodeless-0.2.8.tar", max compression
```

## Comparing `pycodeless-0.2.7.tar` & `pycodeless-0.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.7/LICENSE
--rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.7/pycodeless/__init__.py
--rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.7/pycodeless/_api.py
--rw-r--r--   0        0        0     5790 2023-04-15 14:13:17.163844 pycodeless-0.2.7/pycodeless/_generate.py
--rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.7/pycodeless/_llm.py
--rw-r--r--   0        0        0      619 2023-04-15 10:07:39.825426 pycodeless-0.2.7/pycodeless/_load.py
--rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.7/pycodeless/_openai_llm.py
--rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.7/pycodeless/_parse.py
--rw-r--r--   0        0        0      680 2023-04-15 14:13:36.159327 pycodeless-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4547 2023-04-15 12:35:52.757655 pycodeless-0.2.7/README.md
--rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 pycodeless-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.8/LICENSE
+-rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.8/pycodeless/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.8/pycodeless/_api.py
+-rw-r--r--   0        0        0     5758 2023-04-15 14:59:26.907135 pycodeless-0.2.8/pycodeless/_generate.py
+-rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.8/pycodeless/_llm.py
+-rw-r--r--   0        0        0      619 2023-04-15 10:07:39.825426 pycodeless-0.2.8/pycodeless/_load.py
+-rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.8/pycodeless/_openai_llm.py
+-rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.8/pycodeless/_parse.py
+-rw-r--r--   0        0        0      680 2023-04-15 14:59:37.969572 pycodeless-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4555 2023-04-15 14:21:29.173378 pycodeless-0.2.8/README.md
+-rw-r--r--   0        0        0     5420 1970-01-01 00:00:00.000000 pycodeless-0.2.8/PKG-INFO
```

### Comparing `pycodeless-0.2.7/LICENSE` & `pycodeless-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.7/pycodeless/_api.py` & `pycodeless-0.2.8/pycodeless/_api.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.7/pycodeless/_generate.py` & `pycodeless-0.2.8/pycodeless/_generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,31 +22,29 @@
     return hashlib.md5(text.encode()).hexdigest()
 
 
 def _generate_function_source(llm: LanguageModel, template: str) -> str:
     template = re.sub("^@codeless\n", "", template, flags=re.M)
 
     messages = (
-        Message.system(
+        Message.user(
             "You are a large language model tasked with completing Python"
             " functions given their template with an optional docstring. "
             "When writing code, make sure to follow these rules:\n"
             " 1. Respond with a valid Python code including ONLY the original"
             " function definition and imports. Do NOT include any classes or "
             "other definitions. Do NOT add any additional commentary in the "
             "response! Do NOT wrap the code in quotes or backticks!\n"
             " 2. Preserve the original function definition in your output "
             "including the original docstring.\n"
             " 3. Make sure the code is compatible with Python version "
-            f"{platform.python_version()}."
-        ),
-        Message.user(
+            f"{platform.python_version()}.\n\n"
             "The following is the function to be completed:\n\n"
             f"{template}"
-        )
+        ),
     )
 
     #
     # TODO: The LLMs usually include the user definitions in the response even
     # thogght they are explicitely asked no to. We should probably also use
     # the custom parser here to exctract only imports and the completed
     # function.
```

### Comparing `pycodeless-0.2.7/pycodeless/_llm.py` & `pycodeless-0.2.8/pycodeless/_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.7/pycodeless/_load.py` & `pycodeless-0.2.8/pycodeless/_load.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.7/pycodeless/_openai_llm.py` & `pycodeless-0.2.8/pycodeless/_openai_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.7/pycodeless/_parse.py` & `pycodeless-0.2.8/pycodeless/_parse.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.7/pyproject.toml` & `pycodeless-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycodeless"
-version = "0.2.7"
+version = "0.2.8"
 description = "Build Python code using natural language as a universal interface"
 authors = ["hacksparr0w <hacksparr0w@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hacksparr0w/pycodeless"
 repository = "https://github.com/hacksparr0w/pycodeless"
 documentation = "https://github.com/hacksparr0w/pycodeless"
```

### Comparing `pycodeless-0.2.7/README.md` & `pycodeless-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # You can either specify your OpenAI API key in this way, or you can use the
 # environment variable OPENAI_API_KEY.
 # The same goes for specifying the model name, where the relevant environment
 # variable is OPENAI_MODEL_NAME. If no model name is specified, Pycodeless
 # will default to "gpt-3.5-turbo".
 
 codeless.openai_api_key = "sk-fEaz..."
-codeless.openai_model_name = "gpt-4"
+codeless.openai_model_name = "gpt-3.5-turbo"
 
 
 @codeless
 def greet(name: str) -> str:
     """
     Make greeting for a person with the given name in pirate language
     """
```

### Comparing `pycodeless-0.2.7/PKG-INFO` & `pycodeless-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodeless
-Version: 0.2.7
+Version: 0.2.8
 Summary: Build Python code using natural language as a universal interface
 Home-page: https://github.com/hacksparr0w/pycodeless
 License: MIT
 Keywords: natural,language,codegen,programming,llm,codeless
 Author: hacksparr0w
 Author-email: hacksparr0w@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -63,15 +63,15 @@
 # You can either specify your OpenAI API key in this way, or you can use the
 # environment variable OPENAI_API_KEY.
 # The same goes for specifying the model name, where the relevant environment
 # variable is OPENAI_MODEL_NAME. If no model name is specified, Pycodeless
 # will default to "gpt-3.5-turbo".
 
 codeless.openai_api_key = "sk-fEaz..."
-codeless.openai_model_name = "gpt-4"
+codeless.openai_model_name = "gpt-3.5-turbo"
 
 
 @codeless
 def greet(name: str) -> str:
     """
     Make greeting for a person with the given name in pirate language
     """
```

