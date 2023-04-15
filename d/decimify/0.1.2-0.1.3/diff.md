# Comparing `tmp/decimify-0.1.2.tar.gz` & `tmp/decimify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decimify-0.1.2.tar", max compression
+gzip compressed data, was "decimify-0.1.3.tar", max compression
```

## Comparing `decimify-0.1.2.tar` & `decimify-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-15 10:49:52.312021 decimify-0.1.2/LICENSE
--rw-r--r--   0        0        0     6199 2023-04-15 10:49:52.312021 decimify-0.1.2/README.md
--rw-r--r--   0        0        0       51 2023-04-15 10:49:52.312021 decimify-0.1.2/decimify/__init__.py
--rw-r--r--   0        0        0     1243 2023-04-15 10:49:52.312021 decimify-0.1.2/decimify/parser.py
--rw-r--r--   0        0        0     1611 2023-04-15 10:49:52.312021 decimify-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6718 1970-01-01 00:00:00.000000 decimify-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-15 11:24:26.650606 decimify-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6199 2023-04-15 11:24:26.650606 decimify-0.1.3/README.md
+-rw-r--r--   0        0        0       51 2023-04-15 11:24:26.650606 decimify-0.1.3/decimify/__init__.py
+-rw-r--r--   0        0        0     1243 2023-04-15 11:24:26.650606 decimify-0.1.3/decimify/parser.py
+-rw-r--r--   0        0        0        0 2023-04-15 11:24:26.650606 decimify-0.1.3/decimify/py.typed
+-rw-r--r--   0        0        0     1611 2023-04-15 11:24:26.650606 decimify-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6718 1970-01-01 00:00:00.000000 decimify-0.1.3/PKG-INFO
```

### Comparing `decimify-0.1.2/LICENSE` & `decimify-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decimify-0.1.2/README.md` & `decimify-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `decimify-0.1.2/decimify/parser.py` & `decimify-0.1.3/decimify/parser.py`

 * *Files identical despite different names*

### Comparing `decimify-0.1.2/pyproject.toml` & `decimify-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decimify"
-version = "0.1.2"
+version = "0.1.3"
 description = "Parse numbers with different formatting to builtin python Decimal."
 authors = ["Zahid Kizmaz <tech@zahid.rocks>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<=4.0.0"
```

### Comparing `decimify-0.1.2/PKG-INFO` & `decimify-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decimify
-Version: 0.1.2
+Version: 0.1.3
 Summary: Parse numbers with different formatting to builtin python Decimal.
 License: MIT
 Author: Zahid Kizmaz
 Author-email: tech@zahid.rocks
 Requires-Python: >=3.9.0,<=4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

