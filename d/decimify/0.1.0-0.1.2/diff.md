# Comparing `tmp/decimify-0.1.0.tar.gz` & `tmp/decimify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decimify-0.1.0.tar", max compression
+gzip compressed data, was "decimify-0.1.2.tar", max compression
```

## Comparing `decimify-0.1.0.tar` & `decimify-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-04-15 07:37:42.091704 decimify-0.1.0/LICENSE
--rw-r--r--   0        0        0     1088 2023-04-15 07:37:42.091704 decimify-0.1.0/README.md
--rw-r--r--   0        0        0       51 2023-04-15 07:37:42.091704 decimify-0.1.0/decimify/__init__.py
--rw-r--r--   0        0        0     1243 2023-04-15 07:37:42.091704 decimify-0.1.0/decimify/parser.py
--rw-r--r--   0        0        0     1552 2023-04-15 07:37:42.091704 decimify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 decimify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-15 10:49:52.312021 decimify-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6199 2023-04-15 10:49:52.312021 decimify-0.1.2/README.md
+-rw-r--r--   0        0        0       51 2023-04-15 10:49:52.312021 decimify-0.1.2/decimify/__init__.py
+-rw-r--r--   0        0        0     1243 2023-04-15 10:49:52.312021 decimify-0.1.2/decimify/parser.py
+-rw-r--r--   0        0        0     1611 2023-04-15 10:49:52.312021 decimify-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6718 1970-01-01 00:00:00.000000 decimify-0.1.2/PKG-INFO
```

### Comparing `decimify-0.1.0/LICENSE` & `decimify-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decimify-0.1.0/decimify/parser.py` & `decimify-0.1.2/decimify/parser.py`

 * *Files identical despite different names*

### Comparing `decimify-0.1.0/pyproject.toml` & `decimify-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "decimify"
-version = "0.1.0"
-description = "Parse numbers to Decimal"
+version = "0.1.2"
+description = "Parse numbers with different formatting to builtin python Decimal."
 authors = ["Zahid Kizmaz <tech@zahid.rocks>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<=4.0.0"
 
@@ -13,14 +13,15 @@
 mypy = "*"
 black = "*"
 pytest = "*"
 ruff = "*"
 isort = "*"
 pre-commit = "*"
 exceptiongroup = "*"
+pytest-cov = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.ruff]
```

