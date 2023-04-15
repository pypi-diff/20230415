# Comparing `tmp/typing_result-0.1.0.tar.gz` & `tmp/typing_result-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_result-0.1.0.tar", max compression
+gzip compressed data, was "typing_result-0.1.1.tar", max compression
```

## Comparing `typing_result-0.1.0.tar` & `typing_result-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1091 2023-04-15 18:18:10.898300 typing_result-0.1.0/LICENSE
--rw-r--r--   0        0        0      435 2023-04-15 18:26:24.076727 typing_result-0.1.0/README.md
--rw-r--r--   0        0        0     1049 2023-04-15 18:38:50.773113 typing_result-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-04-15 02:44:37.989551 typing_result-0.1.0/src/result/__init__.py
--rw-r--r--   0        0        0       45 2023-04-15 02:34:59.692320 typing_result-0.1.0/src/result/errors.py
--rw-r--r--   0        0        0     2712 2023-04-15 18:36:57.470371 typing_result-0.1.0/src/result/result.py
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 typing_result-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-15 18:18:10.898300 typing_result-0.1.1/LICENSE
+-rw-r--r--   0        0        0      443 2023-04-15 18:39:38.642861 typing_result-0.1.1/README.md
+-rw-r--r--   0        0        0     1049 2023-04-15 18:49:44.182915 typing_result-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-04-15 02:44:37.989551 typing_result-0.1.1/src/result/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-15 02:34:59.692320 typing_result-0.1.1/src/result/errors.py
+-rw-r--r--   0        0        0     2712 2023-04-15 18:36:57.470371 typing_result-0.1.1/src/result/result.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 typing_result-0.1.1/PKG-INFO
```

### Comparing `typing_result-0.1.0/LICENSE` & `typing_result-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_result-0.1.0/pyproject.toml` & `typing_result-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   "Programming Language :: Python :: 3.10",
 ]
 description = "A python implementation of the Result type, based on the rust language"
 license = "MIT License"
 name = "typing-result"
 packages = [{include = "result", from = "src"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.urls]
 github = "https://github.com/wosteimer/py-result"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
```

### Comparing `typing_result-0.1.0/src/result/result.py` & `typing_result-0.1.1/src/result/result.py`

 * *Files identical despite different names*

### Comparing `typing_result-0.1.0/PKG-INFO` & `typing_result-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing-result
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python implementation of the Result type, based on the rust language
 License: MIT
 Author: William Osteimer Cardoso dos Anjos
 Author-email: wosteimer1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -16,19 +16,19 @@
 Description-Content-Type: text/markdown
 
 A python implementation of the Result type, based on the rust language
 
 ## Installation
 
 ```bash
-pip install py-result
+pip install typing-result
 ```
 or
 ```bash
-poetry install py-result
+poetry install typing-result
 ```
 
 ## Usage Example
 
 ```python
 def div(x: float, y: float) -> Result[float, ZeroDivisionError]:
 	if y == 0:
```

