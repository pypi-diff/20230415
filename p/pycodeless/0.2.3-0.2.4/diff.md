# Comparing `tmp/pycodeless-0.2.3.tar.gz` & `tmp/pycodeless-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodeless-0.2.3.tar", max compression
+gzip compressed data, was "pycodeless-0.2.4.tar", max compression
```

## Comparing `pycodeless-0.2.3.tar` & `pycodeless-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.3/LICENSE
--rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.3/pycodeless/__init__.py
--rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.3/pycodeless/_api.py
--rw-r--r--   0        0        0     5777 2023-04-15 12:37:15.959582 pycodeless-0.2.3/pycodeless/_generate.py
--rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.3/pycodeless/_llm.py
--rw-r--r--   0        0        0      619 2023-04-15 10:07:39.825426 pycodeless-0.2.3/pycodeless/_load.py
--rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.3/pycodeless/_openai_llm.py
--rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.3/pycodeless/_parse.py
--rw-r--r--   0        0        0      680 2023-04-15 12:38:33.060735 pycodeless-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4547 2023-04-15 12:35:52.757655 pycodeless-0.2.3/README.md
--rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 pycodeless-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.4/LICENSE
+-rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.4/pycodeless/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.4/pycodeless/_api.py
+-rw-r--r--   0        0        0     5777 2023-04-15 12:37:15.959582 pycodeless-0.2.4/pycodeless/_generate.py
+-rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.4/pycodeless/_llm.py
+-rw-r--r--   0        0        0      619 2023-04-15 10:07:39.825426 pycodeless-0.2.4/pycodeless/_load.py
+-rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.4/pycodeless/_openai_llm.py
+-rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.4/pycodeless/_parse.py
+-rw-r--r--   0        0        0      680 2023-04-15 14:05:10.647344 pycodeless-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4547 2023-04-15 12:35:52.757655 pycodeless-0.2.4/README.md
+-rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 pycodeless-0.2.4/PKG-INFO
```

### Comparing `pycodeless-0.2.3/LICENSE` & `pycodeless-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/pycodeless/_api.py` & `pycodeless-0.2.4/pycodeless/_api.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/pycodeless/_generate.py` & `pycodeless-0.2.4/pycodeless/_generate.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/pycodeless/_llm.py` & `pycodeless-0.2.4/pycodeless/_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/pycodeless/_load.py` & `pycodeless-0.2.4/pycodeless/_load.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/pycodeless/_openai_llm.py` & `pycodeless-0.2.4/pycodeless/_openai_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/pycodeless/_parse.py` & `pycodeless-0.2.4/pycodeless/_parse.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/pyproject.toml` & `pycodeless-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycodeless"
-version = "0.2.3"
+version = "0.2.4"
 description = "Build Python code using natural language as a universal interface"
 authors = ["hacksparr0w <hacksparr0w@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hacksparr0w/pycodeless"
 repository = "https://github.com/hacksparr0w/pycodeless"
 documentation = "https://github.com/hacksparr0w/pycodeless"
@@ -14,14 +14,14 @@
     "codegen",
     "programming",
     "llm",
     "codeless"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 openai = "^0.27.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pycodeless-0.2.3/README.md` & `pycodeless-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.3/PKG-INFO` & `pycodeless-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pycodeless
-Version: 0.2.3
+Version: 0.2.4
 Summary: Build Python code using natural language as a universal interface
 Home-page: https://github.com/hacksparr0w/pycodeless
 License: MIT
 Keywords: natural,language,codegen,programming,llm,codeless
 Author: hacksparr0w
 Author-email: hacksparr0w@protonmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Project-URL: Documentation, https://github.com/hacksparr0w/pycodeless
 Project-URL: Repository, https://github.com/hacksparr0w/pycodeless
 Description-Content-Type: text/markdown
```

