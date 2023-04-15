# Comparing `tmp/pycodeless-0.2.2.tar.gz` & `tmp/pycodeless-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodeless-0.2.2.tar", max compression
+gzip compressed data, was "pycodeless-0.2.3.tar", max compression
```

## Comparing `pycodeless-0.2.2.tar` & `pycodeless-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.2/LICENSE
--rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.2/pycodeless/__init__.py
--rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.2/pycodeless/_api.py
--rw-r--r--   0        0        0     5142 2023-04-14 11:57:05.819090 pycodeless-0.2.2/pycodeless/_generate.py
--rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.2/pycodeless/_llm.py
--rw-r--r--   0        0        0      436 2023-04-13 22:40:30.195789 pycodeless-0.2.2/pycodeless/_load.py
--rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.2/pycodeless/_openai_llm.py
--rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.2/pycodeless/_parse.py
--rw-r--r--   0        0        0      391 2023-04-14 20:08:17.397947 pycodeless-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3855 2023-04-14 20:30:07.129969 pycodeless-0.2.2/README.md
--rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pycodeless-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.3/LICENSE
+-rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.3/pycodeless/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.3/pycodeless/_api.py
+-rw-r--r--   0        0        0     5777 2023-04-15 12:37:15.959582 pycodeless-0.2.3/pycodeless/_generate.py
+-rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.3/pycodeless/_llm.py
+-rw-r--r--   0        0        0      619 2023-04-15 10:07:39.825426 pycodeless-0.2.3/pycodeless/_load.py
+-rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.3/pycodeless/_openai_llm.py
+-rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.3/pycodeless/_parse.py
+-rw-r--r--   0        0        0      680 2023-04-15 12:38:33.060735 pycodeless-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4547 2023-04-15 12:35:52.757655 pycodeless-0.2.3/README.md
+-rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 pycodeless-0.2.3/PKG-INFO
```

### Comparing `pycodeless-0.2.2/LICENSE` & `pycodeless-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.2/pycodeless/_api.py` & `pycodeless-0.2.3/pycodeless/_api.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.2/pycodeless/_generate.py` & `pycodeless-0.2.3/pycodeless/_generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hashlib
 import inspect
 import json
 import platform
+import re
 
 from pathlib import Path
 from typing import Callable
 
 from ._llm import LanguageModel, Message
 from ._parse import Module, parse_module
 
@@ -18,37 +19,54 @@
 
 
 def _checksum(text: str) -> str:
     return hashlib.md5(text.encode()).hexdigest()
 
 
 def _generate_function_source(llm: LanguageModel, template: str) -> str:
+    template = re.sub("^@codeless\n", "", template, flags=re.M)
+
     messages = (
         Message.system(
             "You are a large language model tasked with completing Python"
             " functions given their template with an optional docstring. "
             "When writing code, make sure to follow these rules:\n"
-            " 1. Respond only with a valid Python code including the original"
-            " function definition and imports. Do NOT add any additional "
-            "commentary. Do NOT wrap the code in quotes or backticks.\n"
-            " 2. Always remove the @codeless decorator from the function "
-            "definition. It must not be present in our output!\n"
-            " 3. Preserve the original function definition in your output \n"
-            "including the original docstring."
-            " 4. Make sure the code is compatible with Python version "
+            " 1. Respond with a valid Python code including ONLY the original"
+            " function definition and imports. Do NOT include any classes or "
+            "other definitions. Do NOT add any additional commentary in the "
+            "response! Do NOT wrap the code in quotes or backticks!\n"
+            " 2. Preserve the original function definition in your output "
+            "including the original docstring.\n"
+            " 3. Make sure the code is compatible with Python version "
             f"{platform.python_version()}."
         ),
         Message.user(
             "The following is the function to be completed:\n\n"
             f"{template}"
         )
     )
 
+    #
+    # TODO: The LLMs usually include the user definitions in the response even
+    # thogght they are explicitely asked no to. We should probably also use
+    # the custom parser here to exctract only imports and the completed
+    # function.
+    #
+
     result = llm.prompt(messages).content
 
+    if result.startswith("```python"):
+        result = result[9:]
+
+    if result.startswith("```"):
+        result = result[3:]
+
+    if result.endswith("```"):
+        result = result[:-3]
+
     return result
 
 
 def _decode_module_generation_metadata(module: Module) -> dict[str, str]:
     if not module.docstring:
         return {}
 
@@ -87,18 +105,23 @@
             source,
             previous_module.docstring.start_index,
             previous_module.docstring.end_index
         )
 
     source = source.strip()
 
-    if not source:
-        source = f"{docstring}\n{generated_function_source}"
-    else:
-        source = f"{docstring}\n{source}\n\n\n{generated_function_source}"
+    #
+    # This is kinda hacky and could be made way better if we had a proper
+    # import parser.
+    #
+
+    if not "from __stub__ import *" in source:
+        source = f"from __stub__ import *\n\n{source}"
+
+    source = f"{docstring}\n{source}\n\n\n{generated_function_source}"
 
     return source
 
 
 def _generate_module_name(name: str) -> str:
     parts = name.split(".")
 
@@ -139,15 +162,15 @@
     )
 
     if (
         previous_template_function_checksum ==
             current_template_function_checksum and
         function_name in generated_module_parsed.functions
     ):
-        return generated_module_path, generated_module_name
+        return template_module, generated_module_path, generated_module_name
 
     generation_metadata[function_name] = current_template_function_checksum
     generated_function_source = _generate_function_source(
         llm,
         template_function_source
     )
 
@@ -156,8 +179,8 @@
         generated_module_parsed,
         function_name,
         generated_function_source
     )
 
     generated_module_path.write_text(generated_module_source, "utf-8")
 
-    return generated_module_path, generated_module_name
+    return template_module, generated_module_path, generated_module_name
```

### Comparing `pycodeless-0.2.2/pycodeless/_llm.py` & `pycodeless-0.2.3/pycodeless/_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.2/pycodeless/_openai_llm.py` & `pycodeless-0.2.3/pycodeless/_openai_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.2/pycodeless/_parse.py` & `pycodeless-0.2.3/pycodeless/_parse.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.2/README.md` & `pycodeless-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-# pycodeless
+# Pycodeless
 
 > **Warning**
 > This project is in a very early stage of development and may not always
 > produce desired results. See the [limitations](#limitations) section for
 > more information.
 
 Pycodeless integrates the power of LLMs into the Python programming language
 and allows you to use natural language as a universal interface for code
 generation.
 
 ## Features
 
- - [x] The `@codeless` decorator allows you to define your functions using
- natural language. All generated code is stored and can be edited or committed
- to your version control system.
+ - [x] The `@codeless` decorator generates your function code from their type
+ annotations and docstrings. All generated code is cached in a local
+ `__pycodeless__` package and can be edited or committed to your version
+ control system.
  - [ ] Support for different language models to allow for better customization
  and offline usage.
  - [ ] Custom docstring formatting to allow for referencing objects across the
  whole codebase.
 
 ## Installation
 
-You can install pycodeless using pip:
+You can install Pycodeless using pip:
 
 ```
 pip install pycodeless
 ```
 
+Since Pycodeless currently only works with the OpenAI API, you'll also need an
+[OpenAI API key][openai-api-keys].
+
 ## Usage
 
-Following is a sample code using pycodeless.
+Following is a sample code using Pycodeless.
 
 ```python
 from pycodeless import codeless
 
 
 # You can either specify your OpenAI API key in this way, or you can use the
 # environment variable OPENAI_API_KEY.
@@ -44,15 +48,15 @@
 codeless.openai_api_key = "sk-fEaz..."
 codeless.openai_model_name = "gpt-4"
 
 
 @codeless
 def greet(name: str) -> str:
     """
-    Make greeting for a person with the given name
+    Make greeting for a person with the given name in pirate language
     """
 
 
 @codeless
 def spongebob_case(text: str) -> str:
     """
     Convert the passed text into spongebob case
@@ -64,14 +68,38 @@
 
 
 if __name__ == "__main__":
     main()
 
 ```
 
+## Limitations
+
+At this point, Pycodeless works *reasonably* well with native Python type
+hints or type annotations from popular third-party libraries that the LLMs
+are familiar with and know how to import. Unless you are able to come up with
+a very elaborate docstring prompt, custom type annotations will not work. More
+exploration work is needed to figure out how to make this work in all cases.
+
+Following is an non-exhaustive list of known limitations:
+
+ - The current code generation and parsing features might be buggy, as there's
+ currently no mechanism for telling whether an output from an LLM is actually
+ runnable Python code.
+ - The `@codeless` decorator may not work in all contexts (REPL, classes,
+ methods, etc.).
+ - There's currently no dependency management in place. This means that we
+ can't track changes across the whole codebase and regenerate functions when
+ their dependencies change. This also means that we can't remove any generated
+ imports when removing a generated function inside a generated module, because
+ there's no way of telling whether or not the import in question is used by
+ any other function. Another problem with this is that if there's a custom
+ type annotation in the function definition, we have no way of referencing it
+ in the generated module.
+
 ## FAQ
 
  - **How is this different from GitHub Copilot?**
  Pycodeless has indeed very similar functionality to GitHub Copilot, but
  the goal of this project is very different. Firstly, Copilot autocompletes
  your code in place and does not differentiate between the generated part of
  the code and the original prompt. One of the main points of this project is
@@ -84,27 +112,13 @@
  which means we can leverage the whole Python infrastructure to enhance the
  prompt specification process (think dynamic docstrings with custom tags to 
  reference various objects from the codebase and aid the LLMs, walking through
  the dependency graphs of type annotations to provide additional context, etc.).
  Also, I like the idea of not being dependent on any particular language model
  or text editor.
 
-## Limitations
-
- - The current code generation and parsing features might be buggy, as there's
- currently no mechanism for telling whether an output from an LLM is actually
- runnable Python code.
- - The `@codeless` decorator may not work in all contexts (REPL, classes,
- methods, etc.).
- - There's currently no dependency management in place. This means that we
- can't track changes across the whole codebase and regenerate functions when
- their dependencies change. This also means that we can't remove any generated
- imports when removing a generated function inside a generated module, because
- there's no way of telling whether or not the import in question is used by
- any other function. Another problem with this is that if there's a custom
- type annotation in the function definition, we have no way of referencing it
- in the generated module.
-
 ## Contribution
 
 If you'd like to report a bug or have an idea for a cool feature, issues and
 pull requests are highly appreciated.
+
+[openai-api-keys]: https://platform.openai.com/account/api-keys
```

### Comparing `pycodeless-0.2.2/PKG-INFO` & `pycodeless-0.2.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 Metadata-Version: 2.1
 Name: pycodeless
-Version: 0.2.2
+Version: 0.2.3
 Summary: Build Python code using natural language as a universal interface
+Home-page: https://github.com/hacksparr0w/pycodeless
 License: MIT
+Keywords: natural,language,codegen,programming,llm,codeless
 Author: hacksparr0w
 Author-email: hacksparr0w@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.4,<0.28.0)
+Project-URL: Documentation, https://github.com/hacksparr0w/pycodeless
+Project-URL: Repository, https://github.com/hacksparr0w/pycodeless
 Description-Content-Type: text/markdown
 
-# pycodeless
+# Pycodeless
 
 > **Warning**
 > This project is in a very early stage of development and may not always
 > produce desired results. See the [limitations](#limitations) section for
 > more information.
 
 Pycodeless integrates the power of LLMs into the Python programming language
 and allows you to use natural language as a universal interface for code
 generation.
 
 ## Features
 
- - [x] The `@codeless` decorator allows you to define your functions using
- natural language. All generated code is stored and can be edited or committed
- to your version control system.
+ - [x] The `@codeless` decorator generates your function code from their type
+ annotations and docstrings. All generated code is cached in a local
+ `__pycodeless__` package and can be edited or committed to your version
+ control system.
  - [ ] Support for different language models to allow for better customization
  and offline usage.
  - [ ] Custom docstring formatting to allow for referencing objects across the
  whole codebase.
 
 ## Installation
 
-You can install pycodeless using pip:
+You can install Pycodeless using pip:
 
 ```
 pip install pycodeless
 ```
 
+Since Pycodeless currently only works with the OpenAI API, you'll also need an
+[OpenAI API key][openai-api-keys].
+
 ## Usage
 
-Following is a sample code using pycodeless.
+Following is a sample code using Pycodeless.
 
 ```python
 from pycodeless import codeless
 
 
 # You can either specify your OpenAI API key in this way, or you can use the
 # environment variable OPENAI_API_KEY.
@@ -60,15 +68,15 @@
 codeless.openai_api_key = "sk-fEaz..."
 codeless.openai_model_name = "gpt-4"
 
 
 @codeless
 def greet(name: str) -> str:
     """
-    Make greeting for a person with the given name
+    Make greeting for a person with the given name in pirate language
     """
 
 
 @codeless
 def spongebob_case(text: str) -> str:
     """
     Convert the passed text into spongebob case
@@ -80,14 +88,38 @@
 
 
 if __name__ == "__main__":
     main()
 
 ```
 
+## Limitations
+
+At this point, Pycodeless works *reasonably* well with native Python type
+hints or type annotations from popular third-party libraries that the LLMs
+are familiar with and know how to import. Unless you are able to come up with
+a very elaborate docstring prompt, custom type annotations will not work. More
+exploration work is needed to figure out how to make this work in all cases.
+
+Following is an non-exhaustive list of known limitations:
+
+ - The current code generation and parsing features might be buggy, as there's
+ currently no mechanism for telling whether an output from an LLM is actually
+ runnable Python code.
+ - The `@codeless` decorator may not work in all contexts (REPL, classes,
+ methods, etc.).
+ - There's currently no dependency management in place. This means that we
+ can't track changes across the whole codebase and regenerate functions when
+ their dependencies change. This also means that we can't remove any generated
+ imports when removing a generated function inside a generated module, because
+ there's no way of telling whether or not the import in question is used by
+ any other function. Another problem with this is that if there's a custom
+ type annotation in the function definition, we have no way of referencing it
+ in the generated module.
+
 ## FAQ
 
  - **How is this different from GitHub Copilot?**
  Pycodeless has indeed very similar functionality to GitHub Copilot, but
  the goal of this project is very different. Firstly, Copilot autocompletes
  your code in place and does not differentiate between the generated part of
  the code and the original prompt. One of the main points of this project is
@@ -100,28 +132,14 @@
  which means we can leverage the whole Python infrastructure to enhance the
  prompt specification process (think dynamic docstrings with custom tags to 
  reference various objects from the codebase and aid the LLMs, walking through
  the dependency graphs of type annotations to provide additional context, etc.).
  Also, I like the idea of not being dependent on any particular language model
  or text editor.
 
-## Limitations
-
- - The current code generation and parsing features might be buggy, as there's
- currently no mechanism for telling whether an output from an LLM is actually
- runnable Python code.
- - The `@codeless` decorator may not work in all contexts (REPL, classes,
- methods, etc.).
- - There's currently no dependency management in place. This means that we
- can't track changes across the whole codebase and regenerate functions when
- their dependencies change. This also means that we can't remove any generated
- imports when removing a generated function inside a generated module, because
- there's no way of telling whether or not the import in question is used by
- any other function. Another problem with this is that if there's a custom
- type annotation in the function definition, we have no way of referencing it
- in the generated module.
-
 ## Contribution
 
 If you'd like to report a bug or have an idea for a cool feature, issues and
 pull requests are highly appreciated.
 
+[openai-api-keys]: https://platform.openai.com/account/api-keys
+
```

