# Comparing `tmp/write_the-0.0.1.tar.gz` & `tmp/write_the-0.1.0.tar.gz`

## Comparing `write_the-0.0.1.tar` & `write_the-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/__about__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/__main__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/cli/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/cli/utils.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/docs/__init__.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/docs/chain.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/docs/docstring.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 write_the-0.0.1/write_the/docs/write.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 write_the-0.0.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 write_the-0.0.1/README.md
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 write_the-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 write_the-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/__main__.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/cli/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/cli/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/chain.py
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/docstring.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 write_the-0.1.0/write_the/docs/write.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 write_the-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 write_the-0.1.0/README.md
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 write_the-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 write_the-0.1.0/PKG-INFO
```

### Comparing `write_the-0.0.1/write_the/docs/chain.py` & `write_the-0.1.0/write_the/docs/chain.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.llms import OpenAI
 
 llm = OpenAI(temperature=0, max_tokens=2000)
-
-
-docs_template="""
-Write Google style docstrings for the following code, using the multi-line format with a description and examples. The first lines describe the code. Include parameter type definitions where possible, and specify any exceptions raised and side effects of the function. For functions with multiple return values or ambiguous behaviour, provide clear guidelines for documenting the behaviour. Please refer to the Google style guide for more information. Any notes should be include in the `Notes:` section of the docstring. Only return the docstring its self. Return each docstring on a single line with the name of the function/class as the key and the docstring as the value. Separate each result by a newline. If the function is a method return the name in the format Class.method. The class docstring should only contain Description and Attributes. Each result should be separated by multiple newlines. 
----
-EXAMPLE
----
-
-def add(a, b): 
-    return a + b 
-Here are formatted docstrings for only add:
-add:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n
----
-CODE
----
-{code}
-Here are formatted docstrings for only {nodes}:
-"""
-
-docs_prompt = PromptTemplate(
-    input_variables=["code", "nodes"],
-    template=docs_template,
-)
-
+docs_template = "\nWrite Google style docstrings for the following code, using the multi-line format with a description and examples. The first lines describe the code. Include parameter type definitions where possible, and specify any exceptions raised and side effects of the function. For functions with multiple return values or ambiguous behaviour, provide clear guidelines for documenting the behaviour. Please refer to the Google style guide for more information. Any notes should be include in the `Notes:` section of the docstring. Only return the docstring its self. Return each docstring on a single line with the name of the function/class as the key and the docstring as the value. Separate each result by a newline. If the function is a method return the name in the format Class.method. The class docstring should only contain Description and Attributes. Each result should be separated by multiple newlines. \n---\nEXAMPLE\n---\n\ndef add(a, b): \n    return a + b \nHere are formatted docstrings for only add:\nadd:\n  Sums 2 numbers.\n  Args:\n    a (int): The first number to add.\n    b (int): The second number to add.\n  Returns:\n    int: The sum of `a` and `b`.\n  Examples:\n    >>> add(1, 2)\n    3\n\n\n---\nCODE\n---\n{code}\nHere are formatted docstrings for only {nodes}:\n"
+docs_prompt = PromptTemplate(input_variables=["code", "nodes"], template=docs_template)
 docs_chain = LLMChain(llm=llm, prompt=docs_prompt)
 
+
 def run(code, nodes: list) -> str:
+    """
+    Generates docstrings for a given code and list of nodes.
+    Args:
+      code (str): The code to generate docstrings for.
+      nodes (list): A list of nodes to generate docstrings for.
+    Returns:
+      str: The generated docstrings.
+    Examples:
+      >>> run('from langchain.prompts import PromptTemplate', ['PromptTemplate'])
+      'PromptTemplate:
+        A class for generating prompts.
+        Attributes:
+          input_variables (list): A list of input variables for the prompt.
+          template (str): The template for the prompt.'
+    """
     nodes = ",".join(nodes)
     return docs_chain.predict(code=code, nodes=nodes)
```

### Comparing `write_the-0.0.1/write_the/docs/write.py` & `write_the-0.1.0/write_the/docs/write.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,73 @@
 from pathlib import Path
 import ast
 from black import format_str, FileMode
 from .docstring import DocstringAdder, get_node_names, remove_docstrings, process_tree
 from .chain import run
 
-def write_the_docs(filename: Path, nodes=[], force=False, inplace=False, context=True) -> str:   
+
+def write_the_docs(
+    filename: Path, nodes=[], force=False, inplace=False, context=True
+) -> str:
+    '''
+    Writes docstrings to a given file.
+    Args:
+      filename (Path): The path to the file to write the docstrings to.
+      nodes (list): A list of nodes to write docstrings for.
+      force (bool): If True, overwrite existing docstrings.
+      inplace (bool): If True, write docstrings to the same file.
+      context (bool): If True, write docstrings for all nodes in the file.
+    Returns:
+      str: The modified source code with the docstrings added.
+    Notes:
+      If `nodes` is empty, docstrings will be written for all nodes in the file.
+      If `context` is False, docstrings will only be written for the nodes in `nodes`.
+    Examples:
+      >>> write_the_docs('example.py', nodes=['add', 'subtract'], force=True, inplace=True, context=False)
+      'def add(a, b):
+          """Adds two numbers.
+          Args:
+              a (int): The first number to add.
+              b (int): The second number to add.
+          Returns:
+              int: The sum of `a` and `b`.
+          """
+          return a + b
+      def subtract(a, b):
+          """Subtracts two numbers.
+          Args:
+              a (int): The first number to subtract.
+              b (int): The second number to subtract.
+          Returns:
+              int: The difference of `a` and `b`.
+          """
+          return a - b'
+    '''
     with open(filename, "r") as file:
         source_code = file.read()
     source_code = format_str(source_code, mode=FileMode())
     tree = ast.parse(source_code)
     extract_specific_nodes = False
     if nodes:
         extract_specific_nodes = True
     else:
         nodes = get_node_names(tree, force)
-    
-    processed_tree = remove_docstrings(tree, nodes) # giving nodes is equal to force 
-
+    processed_tree = remove_docstrings(tree, nodes)
     if not context:
         if extract_specific_nodes:
             processed_tree = process_tree(processed_tree, nodes, False)
         else:
-            # remove any nodes that aren't in the nodes list
             all_nodes = get_node_names(tree, False)
             nodes_to_remove = [n for n in all_nodes if n not in nodes]
             processed_tree = process_tree(processed_tree, nodes_to_remove, True)
-        
     code = ast.unparse(processed_tree)
     result = run(code=code, nodes=nodes)
-
     docstring_dict = {}
     for line in result.split("\n\n"):
-        node_name, docsting = line.split(':', 1)
+        (node_name, docsting) = line.split(":", 1)
         docstring_dict[node_name] = docsting + "\n\n"
-    
     modified_tree = DocstringAdder(docstring_dict, force).visit(tree)
     if not inplace and extract_specific_nodes:
         modified_tree = process_tree(tree, nodes, False)
     modified_tree = ast.fix_missing_locations(modified_tree)
     modified_code = ast.unparse(modified_tree)
     return format_str(modified_code, mode=FileMode())
```

### Comparing `write_the-0.0.1/LICENSE.txt` & `write_the-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.0.1/README.md` & `write_the-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 Write-The offers the following AI-driven features:
 
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs.
 
 ## Requirements
-Python 3.7 or higher
-OpenAI api key
+- Python 3.9 or higher  
+- OpenAI api key
 
 ## Usage
 To use Write-The, run the following commands:
 
 Write-the Docs:
 ```bash
 write-the docs [OPTIONS] [PATH_TO_SOURCE_CODE]
```

### Comparing `write_the-0.0.1/pyproject.toml` & `write_the-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,17 @@
   "typer[all]",
   "langchain",
   "black"
 ]
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://github.com/unknown/write-the#readme"
-Issues = "https://github.com/unknown/write-the/issues"
-Source = "https://github.com/unknown/write-the"
+Documentation = "https://github.com/wytamma/write-the#readme"
+Issues = "https://github.com/wytamma/write-the/issues"
+Source = "https://github.com/wytamma/write-the"
 
 [project.scripts]
 write-the = "write_the.cli:app"
 
 [tool.hatch.version]
 path = "write_the/__about__.py"
```

### Comparing `write_the-0.0.1/PKG-INFO` & `write_the-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.0.1
+Version: 0.1.0
 Summary: AI-powered Code Generation and Refactoring Tool
-Project-URL: Documentation, https://github.com/unknown/write-the#readme
-Project-URL: Issues, https://github.com/unknown/write-the/issues
-Project-URL: Source, https://github.com/unknown/write-the
+Project-URL: Documentation, https://github.com/wytamma/write-the#readme
+Project-URL: Issues, https://github.com/wytamma/write-the/issues
+Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -51,16 +51,16 @@
 Write-The offers the following AI-driven features:
 
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs.
 
 ## Requirements
-Python 3.7 or higher
-OpenAI api key
+- Python 3.9 or higher  
+- OpenAI api key
 
 ## Usage
 To use Write-The, run the following commands:
 
 Write-the Docs:
 ```bash
 write-the docs [OPTIONS] [PATH_TO_SOURCE_CODE]
```

