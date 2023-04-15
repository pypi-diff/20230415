# Comparing `tmp/pycodeless-0.2.6.tar.gz` & `tmp/pycodeless-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodeless-0.2.6.tar", max compression
+gzip compressed data, was "pycodeless-0.2.7.tar", max compression
```

## Comparing `pycodeless-0.2.6.tar` & `pycodeless-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.6/LICENSE
--rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.6/pycodeless/__init__.py
--rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.6/pycodeless/_api.py
--rw-r--r--   0        0        0     5783 2023-04-15 14:11:42.907277 pycodeless-0.2.6/pycodeless/_generate.py
--rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.6/pycodeless/_llm.py
--rw-r--r--   0        0        0      619 2023-04-15 10:07:39.825426 pycodeless-0.2.6/pycodeless/_load.py
--rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.6/pycodeless/_openai_llm.py
--rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.6/pycodeless/_parse.py
--rw-r--r--   0        0        0      680 2023-04-15 14:12:04.235838 pycodeless-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4547 2023-04-15 12:35:52.757655 pycodeless-0.2.6/README.md
--rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 pycodeless-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.7/LICENSE
+-rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.7/pycodeless/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.7/pycodeless/_api.py
+-rw-r--r--   0        0        0     5790 2023-04-15 14:13:17.163844 pycodeless-0.2.7/pycodeless/_generate.py
+-rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.7/pycodeless/_llm.py
+-rw-r--r--   0        0        0      619 2023-04-15 10:07:39.825426 pycodeless-0.2.7/pycodeless/_load.py
+-rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.7/pycodeless/_openai_llm.py
+-rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.7/pycodeless/_parse.py
+-rw-r--r--   0        0        0      680 2023-04-15 14:13:36.159327 pycodeless-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4547 2023-04-15 12:35:52.757655 pycodeless-0.2.7/README.md
+-rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 pycodeless-0.2.7/PKG-INFO
```

### Comparing `pycodeless-0.2.6/LICENSE` & `pycodeless-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.6/pycodeless/_api.py` & `pycodeless-0.2.7/pycodeless/_api.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.6/pycodeless/_generate.py` & `pycodeless-0.2.7/pycodeless/_generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hashlib
 import inspect
 import json
 import platform
 import re
 
 from pathlib import Path
-from typing import Callable, Dict
+from typing import Callable, Dict, Tuple
 
 from ._llm import LanguageModel, Message
 from ._parse import Module, parse_module
 
 
 _GENERATED_PACKAGE_NAME = "__pycodeless__"
 
@@ -131,15 +131,15 @@
 def _generate_module_path(path: Path) -> Path:
     return path.parent / _GENERATED_PACKAGE_NAME / path.name
 
 
 def generate(
         llm: LanguageModel,
         template_function: Callable
-) -> tuple[Path, str]:
+) -> Tuple[Path, str]:
     function_name = template_function.__name__
 
     template_module = inspect.getmodule(template_function)
     template_module_name = template_module.__name__
     template_module_path = Path(template_module.__file__)
     template_function_source = inspect.getsource(template_function)
     current_template_function_checksum = _checksum(template_function_source)
```

### Comparing `pycodeless-0.2.6/pycodeless/_llm.py` & `pycodeless-0.2.7/pycodeless/_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.6/pycodeless/_load.py` & `pycodeless-0.2.7/pycodeless/_load.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.6/pycodeless/_openai_llm.py` & `pycodeless-0.2.7/pycodeless/_openai_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.6/pycodeless/_parse.py` & `pycodeless-0.2.7/pycodeless/_parse.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.6/pyproject.toml` & `pycodeless-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycodeless"
-version = "0.2.6"
+version = "0.2.7"
 description = "Build Python code using natural language as a universal interface"
 authors = ["hacksparr0w <hacksparr0w@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hacksparr0w/pycodeless"
 repository = "https://github.com/hacksparr0w/pycodeless"
 documentation = "https://github.com/hacksparr0w/pycodeless"
```

### Comparing `pycodeless-0.2.6/README.md` & `pycodeless-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.6/PKG-INFO` & `pycodeless-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodeless
-Version: 0.2.6
+Version: 0.2.7
 Summary: Build Python code using natural language as a universal interface
 Home-page: https://github.com/hacksparr0w/pycodeless
 License: MIT
 Keywords: natural,language,codegen,programming,llm,codeless
 Author: hacksparr0w
 Author-email: hacksparr0w@protonmail.com
 Requires-Python: >=3.8,<4.0
```

