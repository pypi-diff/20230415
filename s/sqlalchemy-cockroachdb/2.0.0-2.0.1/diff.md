# Comparing `tmp/sqlalchemy-cockroachdb-2.0.0.tar.gz` & `tmp/sqlalchemy-cockroachdb-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-cockroachdb-2.0.0.tar", last modified: Tue Feb 21 14:56:41 2023, max compression
+gzip compressed data, was "sqlalchemy-cockroachdb-2.0.1.tar", last modified: Fri Apr 14 23:09:21 2023, max compression
```

## Comparing `sqlalchemy-cockroachdb-2.0.0.tar` & `sqlalchemy-cockroachdb-2.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-02-21 14:56:41.347212 sqlalchemy-cockroachdb-2.0.0/
--rw-r--r--   0 rafiss     (503) staff       (20)    11325 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/LICENSE
--rw-r--r--   0 rafiss     (503) staff       (20)     2633 2023-02-21 14:56:41.347281 sqlalchemy-cockroachdb-2.0.0/PKG-INFO
--rw-r--r--   0 rafiss     (503) staff       (20)     1629 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/README.md
--rw-r--r--   0 rafiss     (503) staff       (20)      212 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/pyproject.toml
--rw-r--r--   0 rafiss     (503) staff       (20)      353 2023-02-21 14:56:41.347553 sqlalchemy-cockroachdb-2.0.0/setup.cfg
--rw-r--r--   0 rafiss     (503) staff       (20)     1944 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/setup.py
-drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-02-21 14:56:41.342998 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/
--rw-r--r--   0 rafiss     (503) staff       (20)      372 2023-02-21 14:55:00.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/__init__.py
--rw-r--r--   0 rafiss     (503) staff       (20)      250 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/_psycopg_common.py
--rw-r--r--   0 rafiss     (503) staff       (20)      769 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/asyncpg.py
--rw-r--r--   0 rafiss     (503) staff       (20)    23447 2023-02-21 14:47:04.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/base.py
--rw-r--r--   0 rafiss     (503) staff       (20)      611 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/ddl_compiler.py
--rw-r--r--   0 rafiss     (503) staff       (20)      205 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/provision.py
--rw-r--r--   0 rafiss     (503) staff       (20)      577 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/psycopg2.py
--rw-r--r--   0 rafiss     (503) staff       (20)     7444 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/requirements.py
--rw-r--r--   0 rafiss     (503) staff       (20)     1540 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/stmt_compiler.py
--rw-r--r--   0 rafiss     (503) staff       (20)     4348 2023-02-10 16:14:33.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/transaction.py
-drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-02-21 14:56:41.344186 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/
--rw-r--r--   0 rafiss     (503) staff       (20)     2633 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/PKG-INFO
--rw-r--r--   0 rafiss     (503) staff       (20)      994 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/SOURCES.txt
--rw-r--r--   0 rafiss     (503) staff       (20)        1 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/dependency_links.txt
--rw-r--r--   0 rafiss     (503) staff       (20)      259 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/entry_points.txt
--rw-r--r--   0 rafiss     (503) staff       (20)        1 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/not-zip-safe
--rw-r--r--   0 rafiss     (503) staff       (20)       11 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/requires.txt
--rw-r--r--   0 rafiss     (503) staff       (20)       23 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/top_level.txt
-drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-02-21 14:56:41.347068 sqlalchemy-cockroachdb-2.0.0/test/
--rw-r--r--   0 rafiss     (503) staff       (20)     2121 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/test/test_across_schema.py
--rw-r--r--   0 rafiss     (503) staff       (20)     2599 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/test/test_column_reflect.py
--rw-r--r--   0 rafiss     (503) staff       (20)     5298 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/test/test_introspection.py
--rw-r--r--   0 rafiss     (503) staff       (20)     2982 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/test/test_json.py
--rw-r--r--   0 rafiss     (503) staff       (20)     4552 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.0/test/test_run_transaction_core.py
--rw-r--r--   0 rafiss     (503) staff       (20)     4106 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/test/test_run_transaction_session.py
--rw-r--r--   0 rafiss     (503) staff       (20)     3481 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/test/test_suite_alembic.py
--rw-r--r--   0 rafiss     (503) staff       (20)     7372 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/test/test_suite_sqlalchemy.py
--rw-r--r--   0 rafiss     (503) staff       (20)     1115 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.0/test/test_with_hint.py
+drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-04-14 23:09:21.546207 sqlalchemy-cockroachdb-2.0.1/
+-rw-r--r--   0 rafiss     (503) staff       (20)    11325 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/LICENSE
+-rw-r--r--   0 rafiss     (503) staff       (20)     2633 2023-04-14 23:09:21.546284 sqlalchemy-cockroachdb-2.0.1/PKG-INFO
+-rw-r--r--   0 rafiss     (503) staff       (20)     1629 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/README.md
+-rw-r--r--   0 rafiss     (503) staff       (20)      212 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/pyproject.toml
+-rw-r--r--   0 rafiss     (503) staff       (20)      353 2023-04-14 23:09:21.546605 sqlalchemy-cockroachdb-2.0.1/setup.cfg
+-rw-r--r--   0 rafiss     (503) staff       (20)     1980 2023-04-14 23:04:13.000000 sqlalchemy-cockroachdb-2.0.1/setup.py
+drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-04-14 23:09:21.542859 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/
+-rw-r--r--   0 rafiss     (503) staff       (20)      372 2023-04-14 23:08:15.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/__init__.py
+-rw-r--r--   0 rafiss     (503) staff       (20)      263 2023-04-14 23:04:13.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/_psycopg_common.py
+-rw-r--r--   0 rafiss     (503) staff       (20)      782 2023-04-14 23:04:13.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/asyncpg.py
+-rw-r--r--   0 rafiss     (503) staff       (20)    23447 2023-02-21 14:47:04.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/base.py
+-rw-r--r--   0 rafiss     (503) staff       (20)      611 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/ddl_compiler.py
+-rw-r--r--   0 rafiss     (503) staff       (20)      205 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/provision.py
+-rw-r--r--   0 rafiss     (503) staff       (20)      577 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/psycopg2.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     7640 2023-04-14 23:04:13.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/requirements.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     1540 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/stmt_compiler.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     4348 2023-02-10 16:14:33.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/transaction.py
+drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-04-14 23:09:21.544213 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/
+-rw-r--r--   0 rafiss     (503) staff       (20)     2633 2023-04-14 23:09:21.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/PKG-INFO
+-rw-r--r--   0 rafiss     (503) staff       (20)      994 2023-04-14 23:09:21.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/SOURCES.txt
+-rw-r--r--   0 rafiss     (503) staff       (20)        1 2023-04-14 23:09:21.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/dependency_links.txt
+-rw-r--r--   0 rafiss     (503) staff       (20)      259 2023-04-14 23:09:21.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/entry_points.txt
+-rw-r--r--   0 rafiss     (503) staff       (20)        1 2023-02-21 14:56:41.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/not-zip-safe
+-rw-r--r--   0 rafiss     (503) staff       (20)       11 2023-04-14 23:09:21.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/requires.txt
+-rw-r--r--   0 rafiss     (503) staff       (20)       23 2023-04-14 23:09:21.000000 sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/top_level.txt
+drwxr-xr-x   0 rafiss     (503) staff       (20)        0 2023-04-14 23:09:21.546053 sqlalchemy-cockroachdb-2.0.1/test/
+-rw-r--r--   0 rafiss     (503) staff       (20)     2121 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/test/test_across_schema.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     2599 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/test/test_column_reflect.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     5298 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/test/test_introspection.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     2982 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/test/test_json.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     4552 2023-01-05 19:13:56.000000 sqlalchemy-cockroachdb-2.0.1/test/test_run_transaction_core.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     4106 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/test/test_run_transaction_session.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     3481 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/test/test_suite_alembic.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     7372 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/test/test_suite_sqlalchemy.py
+-rw-r--r--   0 rafiss     (503) staff       (20)     1115 2023-02-09 19:07:52.000000 sqlalchemy-cockroachdb-2.0.1/test/test_with_hint.py
```

### Comparing `sqlalchemy-cockroachdb-2.0.0/LICENSE` & `sqlalchemy-cockroachdb-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/PKG-INFO` & `sqlalchemy-cockroachdb-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-cockroachdb
-Version: 2.0.0
+Version: 2.0.1
 Summary: CockroachDB dialect for SQLAlchemy
 Home-page: https://github.com/cockroachdb/sqlalchemy-cockroachdb
 Author: Cockroach Labs
 Author-email: cockroach-db@googlegroups.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/cockroachdb/sqlalchemy-cockroachdb/wiki
 Project-URL: Source, https://github.com/cockroachdb/sqlalchemy-cockroachdb
```

### Comparing `sqlalchemy-cockroachdb-2.0.0/README.md` & `sqlalchemy-cockroachdb-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/setup.py` & `sqlalchemy-cockroachdb-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import re
 
 from setuptools import setup, find_packages
 
-with open(os.path.join(os.path.dirname(__file__), "sqlalchemy_cockroachdb", "__init__.py")) as v:
+with open(os.path.join(os.path.dirname(__file__), "sqlalchemy_cockroachdb", "__init__.py"), encoding='UTF-8') as v:
     VERSION = re.compile(r'.*__version__ = "(.*?)"', re.S).match(v.read()).group(1)
 
-with open(os.path.join(os.path.dirname(__file__), "README.md")) as f:
+with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding='UTF-8') as f:
     README = f.read()
 
 setup(
     name="sqlalchemy-cockroachdb",
     version=VERSION,
     author="Cockroach Labs",
     author_email="cockroach-db@googlegroups.com",
```

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/asyncpg.py` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/asyncpg.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     supports_statement_cache = True
 
     async def setup_asyncpg_json_codec(self, conn):
         # https://github.com/cockroachdb/cockroach/issues/9990#issuecomment-579202144
         pass
 
     def get_isolation_level_values(self, dbapi_conn):
-        return ("SERIALIZABLE",)
+        return ("SERIALIZABLE", "AUTOCOMMIT")
```

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/base.py` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/ddl_compiler.py` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/ddl_compiler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/psycopg2.py` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/psycopg2.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/requirements.py` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/requirements.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,14 +171,20 @@
         return exclusions.closed()
 
     @property
     def uuid_data_type(self):
         return exclusions.open()
 
     def get_isolation_levels(self, config):
-        return {"default": "SERIALIZABLE", "supported": ["SERIALIZABLE"]}
+        return {"default": "SERIALIZABLE", "supported": ["SERIALIZABLE", "AUTOCOMMIT"]}
 
+    @property
+    def autocommit(self):
+        return exclusions.open()
+
+    # -----------------------------------------------
     # non-default requirements for Alembic test suite
+    # -----------------------------------------------
 
     @property
     def autoincrement_on_composite_pk(self):
         return exclusions.open()
```

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/stmt_compiler.py` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/stmt_compiler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb/transaction.py` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb/transaction.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/PKG-INFO` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-cockroachdb
-Version: 2.0.0
+Version: 2.0.1
 Summary: CockroachDB dialect for SQLAlchemy
 Home-page: https://github.com/cockroachdb/sqlalchemy-cockroachdb
 Author: Cockroach Labs
 Author-email: cockroach-db@googlegroups.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/cockroachdb/sqlalchemy-cockroachdb/wiki
 Project-URL: Source, https://github.com/cockroachdb/sqlalchemy-cockroachdb
```

### Comparing `sqlalchemy-cockroachdb-2.0.0/sqlalchemy_cockroachdb.egg-info/SOURCES.txt` & `sqlalchemy-cockroachdb-2.0.1/sqlalchemy_cockroachdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_across_schema.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_across_schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_column_reflect.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_column_reflect.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_introspection.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_introspection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_json.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_json.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_run_transaction_core.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_run_transaction_core.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_run_transaction_session.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_run_transaction_session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_suite_alembic.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_suite_alembic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_suite_sqlalchemy.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_suite_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-cockroachdb-2.0.0/test/test_with_hint.py` & `sqlalchemy-cockroachdb-2.0.1/test/test_with_hint.py`

 * *Files identical despite different names*

