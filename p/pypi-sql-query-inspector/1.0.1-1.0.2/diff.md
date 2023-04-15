# Comparing `tmp/pypi-sql-query-inspector-1.0.1.tar.gz` & `tmp/pypi-sql-query-inspector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi-sql-query-inspector-1.0.1.tar", last modified: Sat Apr 15 10:23:10 2023, max compression
+gzip compressed data, was "pypi-sql-query-inspector-1.0.2.tar", last modified: Sat Apr 15 10:31:25 2023, max compression
```

## Comparing `pypi-sql-query-inspector-1.0.1.tar` & `pypi-sql-query-inspector-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:23:10.058951 pypi-sql-query-inspector-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:22:58.000000 pypi-sql-query-inspector-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-15 10:23:10.058951 pypi-sql-query-inspector-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-15 10:22:58.000000 pypi-sql-query-inspector-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:23:10.054951 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:22:58.000000 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-15 10:22:58.000000 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:23:10.058951 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-15 10:23:10.000000 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-15 10:23:10.000000 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:23:10.000000 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 10:23:10.000000 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 10:23:10.000000 pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-15 10:22:58.000000 pypi-sql-query-inspector-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:23:10.058951 pypi-sql-query-inspector-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:23:10.058951 pypi-sql-query-inspector-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-15 10:22:58.000000 pypi-sql-query-inspector-1.0.1/tests/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/tests/test_new.py
```

### Comparing `pypi-sql-query-inspector-1.0.1/PKG-INFO` & `pypi-sql-query-inspector-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-sql-query-inspector
-Version: 1.0.1
+Version: 1.0.2
 Summary: A django middleware package to print out connection queries in terminal when DEBUGing
 Author: peacefulseeker
 Project-URL: Homepage, https://pypi.org/project/pypi-sql-query-inspector/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,10 +12,10 @@
 A simple example of django middleware package
 
 ### Usage
 Append middleware to `MIDDLEWARES` list:
 ```
 MIDDLEWARE = [
     ...
-    'pypi_sql_query_inspector.middleware.new_middleware',
+    'pypi_sql_query_inspector.print_sql_queries_to_terminal',
 ]
 ```
```

### Comparing `pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector/middleware.py` & `pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/middleware.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db import connection
 from pygments import highlight
 from pygments.lexers.sql import SqlLexer
 from pygments.formatters import TerminalFormatter
 from sqlparse import format
 
 
-def new_middleware(get_response):
+def print_sql_queries_to_terminal(get_response):
 
     def middleware(request):
         response = get_response(request)
 
         if settings.DEBUG:
             queries = connection.queries
             num_queries = len(queries)
```

### Comparing `pypi-sql-query-inspector-1.0.1/pypi_sql_query_inspector.egg-info/PKG-INFO` & `pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-sql-query-inspector
-Version: 1.0.1
+Version: 1.0.2
 Summary: A django middleware package to print out connection queries in terminal when DEBUGing
 Author: peacefulseeker
 Project-URL: Homepage, https://pypi.org/project/pypi-sql-query-inspector/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,10 +12,10 @@
 A simple example of django middleware package
 
 ### Usage
 Append middleware to `MIDDLEWARES` list:
 ```
 MIDDLEWARE = [
     ...
-    'pypi_sql_query_inspector.middleware.new_middleware',
+    'pypi_sql_query_inspector.print_sql_queries_to_terminal',
 ]
 ```
```

### Comparing `pypi-sql-query-inspector-1.0.1/pyproject.toml` & `pypi-sql-query-inspector-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "wheel"] # packaging into *.whl
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pypi-sql-query-inspector"
-version = "1.0.1"
+version = "1.0.2"
 description = "A django middleware package to print out connection queries in terminal when DEBUGing"
 readme = "README.md"
 license = { file = "MIT"}
 authors = [
     { name = "peacefulseeker" }
 ]
```

