# Comparing `tmp/pypi-sql-query-inspector-1.0.2.tar.gz` & `tmp/pypi-sql-query-inspector-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi-sql-query-inspector-1.0.2.tar", last modified: Sat Apr 15 10:31:25 2023, max compression
+gzip compressed data, was "pypi-sql-query-inspector-1.0.3.tar", last modified: Sat Apr 15 10:35:12 2023, max compression
```

## Comparing `pypi-sql-query-inspector-1.0.2.tar` & `pypi-sql-query-inspector-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 10:31:25.000000 pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:31:25.204825 pypi-sql-query-inspector-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-15 10:31:16.000000 pypi-sql-query-inspector-1.0.2/tests/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:35:12.259114 pypi-sql-query-inspector-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:35:03.000000 pypi-sql-query-inspector-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 10:35:12.259114 pypi-sql-query-inspector-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 10:35:03.000000 pypi-sql-query-inspector-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:35:12.259114 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 10:35:03.000000 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-15 10:35:03.000000 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:35:12.259114 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 10:35:12.000000 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-15 10:35:12.000000 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:35:12.000000 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 10:35:12.000000 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 10:35:12.000000 pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-15 10:35:03.000000 pypi-sql-query-inspector-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:35:12.259114 pypi-sql-query-inspector-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:35:12.259114 pypi-sql-query-inspector-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-15 10:35:03.000000 pypi-sql-query-inspector-1.0.3/tests/test_new.py
```

### Comparing `pypi-sql-query-inspector-1.0.2/PKG-INFO` & `pypi-sql-query-inspector-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-sql-query-inspector
-Version: 1.0.2
+Version: 1.0.3
 Summary: A django middleware package to print out connection queries in terminal when DEBUGing
 Author: peacefulseeker
 Project-URL: Homepage, https://pypi.org/project/pypi-sql-query-inspector/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector/middleware.py` & `pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector/middleware.py`

 * *Files identical despite different names*

### Comparing `pypi-sql-query-inspector-1.0.2/pypi_sql_query_inspector.egg-info/PKG-INFO` & `pypi-sql-query-inspector-1.0.3/pypi_sql_query_inspector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-sql-query-inspector
-Version: 1.0.2
+Version: 1.0.3
 Summary: A django middleware package to print out connection queries in terminal when DEBUGing
 Author: peacefulseeker
 Project-URL: Homepage, https://pypi.org/project/pypi-sql-query-inspector/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pypi-sql-query-inspector-1.0.2/pyproject.toml` & `pypi-sql-query-inspector-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "wheel"] # packaging into *.whl
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pypi-sql-query-inspector"
-version = "1.0.2"
+version = "1.0.3"
 description = "A django middleware package to print out connection queries in terminal when DEBUGing"
 readme = "README.md"
 license = { file = "MIT"}
 authors = [
     { name = "peacefulseeker" }
 ]
```

