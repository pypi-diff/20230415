# Comparing `tmp/backend_sqlalchemy-0.1.5.tar.gz` & `tmp/backend_sqlalchemy-0.1.5.dev1681545553.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend_sqlalchemy-0.1.5.tar", max compression
+gzip compressed data, was "backend_sqlalchemy-0.1.5.dev1681545553.tar", max compression
```

## Comparing `backend_sqlalchemy-0.1.5.tar` & `backend_sqlalchemy-0.1.5.dev1681545553.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      355 2023-04-15 08:13:39.995730 backend_sqlalchemy-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-15 08:13:39.995730 backend_sqlalchemy-0.1.5/backend_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      248 2023-04-15 08:13:39.995730 backend_sqlalchemy-0.1.5/backend_sqlalchemy/main.py
--rw-r--r--   0        0        0      463 2023-04-15 08:13:39.995730 backend_sqlalchemy-0.1.5/backend_sqlalchemy/mixins.py
--rw-r--r--   0        0        0     1496 2023-04-15 08:14:03.913378 backend_sqlalchemy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      355 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/backend_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/backend_sqlalchemy/main.py
+-rw-r--r--   0        0        0      463 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/backend_sqlalchemy/mixins.py
+-rw-r--r--   0        0        0     1511 2023-04-15 07:59:13.841840 backend_sqlalchemy-0.1.5.dev1681545553/pyproject.toml
+-rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.5.dev1681545553/PKG-INFO
```

### Comparing `backend_sqlalchemy-0.1.5/pyproject.toml` & `backend_sqlalchemy-0.1.5.dev1681545553/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "backend-sqlalchemy"
 packages = [{include = "backend_sqlalchemy"}]
-version = "0.1.5"
+version = "0.1.5.dev.1681545553"
 description = "Core for SQLAlchemy"
 authors = ["Martin More <martinmore@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sqlalchemy", "python", "backend"]
 
 homepage = "https://example.com/"
```

### Comparing `backend_sqlalchemy-0.1.5/PKG-INFO` & `backend_sqlalchemy-0.1.5.dev1681545553/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend-sqlalchemy
-Version: 0.1.5
+Version: 0.1.5.dev1681545553
 Summary: Core for SQLAlchemy
 Home-page: https://example.com/
 License: MIT
 Keywords: sqlalchemy,python,backend
 Author: Martin More
 Author-email: martinmore@gmail.com
 Requires-Python: >=3.10,<4.0
```

