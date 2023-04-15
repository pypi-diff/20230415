# Comparing `tmp/anthropic-0.2.6.tar.gz` & `tmp/anthropic-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.2.6.tar", last modified: Mon Apr  3 18:31:14 2023, max compression
+gzip compressed data, was "anthropic-0.2.7.tar", last modified: Sat Apr 15 03:43:38 2023, max compression
```

## Comparing `anthropic-0.2.6.tar` & `anthropic-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:31:14.894661 anthropic-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-03 18:31:00.000000 anthropic-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-03 18:31:14.890660 anthropic-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-03 18:31:00.000000 anthropic-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:31:14.890660 anthropic-0.2.6/anthropic/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-03 18:31:00.000000 anthropic-0.2.6/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-03 18:31:00.000000 anthropic-0.2.6/anthropic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-03 18:31:00.000000 anthropic-0.2.6/anthropic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-03 18:31:00.000000 anthropic-0.2.6/anthropic/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:31:14.890660 anthropic-0.2.6/anthropic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-03 18:31:14.000000 anthropic-0.2.6/anthropic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-03 18:31:14.000000 anthropic-0.2.6/anthropic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 18:31:14.000000 anthropic-0.2.6/anthropic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 18:31:14.000000 anthropic-0.2.6/anthropic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 18:31:14.000000 anthropic-0.2.6/anthropic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-03 18:31:00.000000 anthropic-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 18:31:14.894661 anthropic-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:31:14.890660 anthropic-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-03 18:31:00.000000 anthropic-0.2.6/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.597907 anthropic-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-15 03:43:29.000000 anthropic-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 03:43:38.593907 anthropic-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-15 03:43:29.000000 anthropic-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.593907 anthropic-0.2.7/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-15 03:43:29.000000 anthropic-0.2.7/anthropic/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.593907 anthropic-0.2.7/anthropic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 03:43:38.000000 anthropic-0.2.7/anthropic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-15 03:43:29.000000 anthropic-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:43:38.597907 anthropic-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:43:38.593907 anthropic-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-15 03:43:29.000000 anthropic-0.2.7/tests/test_api.py
```

### Comparing `anthropic-0.2.6/LICENSE` & `anthropic-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.2.6/PKG-INFO` & `anthropic-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.2.6
+Version: 0.2.7
 Summary: Library for accessing the anthropic API
 Author: Anthropic
 License: MIT
 Project-URL: homepage, https://github.com/anthropics/anthropic-sdk-python
 Project-URL: repository, https://github.com/anthropics/anthropic-sdk-python.git
 Keywords: anthropic,anthropicai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anthropic-0.2.6/anthropic/api.py` & `anthropic-0.2.7/anthropic/api.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.2.6/anthropic/tokenizer.py` & `anthropic-0.2.7/anthropic/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     return tokenizer_file
 
 def _get_cached_tokenizer_file_as_str() -> str:
     tokenizer_file = _get_tokenizer_filename()
     if not os.path.exists(tokenizer_file):
         response = httpx.get(CLAUDE_TOKENIZER_REMOTE_FILE)
         response.raise_for_status()
-        with open(tokenizer_file, 'w') as f:
+        with open(tokenizer_file, 'w', encoding="utf-8") as f:
             f.write(response.text)
 
-    with open(tokenizer_file, 'r') as f:
+    with open(tokenizer_file, 'r', encoding="utf-8") as f:
         return f.read()
 
 def get_tokenizer() -> Tokenizer:
     global claude_tokenizer
 
     if not claude_tokenizer:
         try:
```

### Comparing `anthropic-0.2.6/anthropic.egg-info/PKG-INFO` & `anthropic-0.2.7/anthropic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.2.6
+Version: 0.2.7
 Summary: Library for accessing the anthropic API
 Author: Anthropic
 License: MIT
 Project-URL: homepage, https://github.com/anthropics/anthropic-sdk-python
 Project-URL: repository, https://github.com/anthropics/anthropic-sdk-python.git
 Keywords: anthropic,anthropicai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anthropic-0.2.6/pyproject.toml` & `anthropic-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anthropic"
-version = "0.2.6"
+version = "0.2.7"
 description = "Library for accessing the anthropic API"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["anthropic", "anthropicai"]
 license = {text = "MIT"}
 authors = [
     {name = "Anthropic"}
```

### Comparing `anthropic-0.2.6/tests/test_api.py` & `anthropic-0.2.7/tests/test_api.py`

 * *Files identical despite different names*

