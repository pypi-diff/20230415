# Comparing `tmp/backend_sqlalchemy-0.1.4.dev1681023002.tar.gz` & `tmp/backend_sqlalchemy-0.1.5.dev1681545553.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend_sqlalchemy-0.1.4.dev1681023002.tar", max compression
+gzip compressed data, was "backend_sqlalchemy-0.1.5.dev1681545553.tar", max compression
```

## Comparing `backend_sqlalchemy-0.1.4.dev1681023002.tar` & `backend_sqlalchemy-0.1.5.dev1681545553.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      291 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/README.md
--rw-r--r--   0        0        0        0 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/backend_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      248 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/backend_sqlalchemy/main.py
--rw-r--r--   0        0        0     1415 2023-04-09 06:50:03.518454 backend_sqlalchemy-0.1.4.dev1681023002/pyproject.toml
--rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.4.dev1681023002/PKG-INFO
+-rw-r--r--   0        0        0      355 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/backend_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/backend_sqlalchemy/main.py
+-rw-r--r--   0        0        0      463 2023-04-15 07:58:53.144765 backend_sqlalchemy-0.1.5.dev1681545553/backend_sqlalchemy/mixins.py
+-rw-r--r--   0        0        0     1511 2023-04-15 07:59:13.841840 backend_sqlalchemy-0.1.5.dev1681545553/pyproject.toml
+-rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.5.dev1681545553/PKG-INFO
```

### Comparing `backend_sqlalchemy-0.1.4.dev1681023002/pyproject.toml` & `backend_sqlalchemy-0.1.5.dev1681545553/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "backend-sqlalchemy"
 packages = [{include = "backend_sqlalchemy"}]
-version = "0.1.4.dev.1681023002"
+version = "0.1.5.dev.1681545553"
 description = "Core for SQLAlchemy"
 authors = ["Martin More <martinmore@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sqlalchemy", "python", "backend"]
 
 homepage = "https://example.com/"
@@ -31,14 +31,19 @@
 python = "^3.10"
 sqlalchemy = "^1.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 
+[tool.poetry.group.dev.dependencies]
+isort = "^5.12.0"
+black = "^23.3.0"
+pre-commit = "^3.2.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.autopub]
 git-username = "martin-more"
 git-email = "martinmore@gmail.com"
```

### Comparing `backend_sqlalchemy-0.1.4.dev1681023002/PKG-INFO` & `backend_sqlalchemy-0.1.5.dev1681545553/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend-sqlalchemy
-Version: 0.1.4.dev1681023002
+Version: 0.1.5.dev1681545553
 Summary: Core for SQLAlchemy
 Home-page: https://example.com/
 License: MIT
 Keywords: sqlalchemy,python,backend
 Author: Martin More
 Author-email: martinmore@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -30,10 +30,14 @@
 
 
 [![codecov](https://codecov.io/gh/martinmore-team/backend-sqlalchemy/branch/main/graph/badge.svg?token=XJER9LZAZV)](https://codecov.io/gh/martinmore-team/backend-sqlalchemy)
 
 
 ## Tests
 
-- poetry run coverage run -m pytest --showlocals -vv
-- poetry run coverage xml -i
+- `poetry run coverage run -m pytest --showlocals -vv`
+- `poetry run coverage xml -i`
+
+## Linter
+- `pre-commit autoupdate`
+- `pre-commit install`
```

