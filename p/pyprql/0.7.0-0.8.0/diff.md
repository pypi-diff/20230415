# Comparing `tmp/pyprql-0.7.0.tar.gz` & `tmp/pyprql-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprql-0.7.0.tar", max compression
+gzip compressed data, was "pyprql-0.8.0.tar", max compression
```

## Comparing `pyprql-0.7.0.tar` & `pyprql-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    10284 2023-04-02 03:10:53.773138 pyprql-0.7.0/LICENSE
--rw-r--r--   0        0        0     2278 2023-04-02 03:10:53.773138 pyprql-0.7.0/README.md
--rw-r--r--   0        0        0     2191 2023-04-02 03:11:27.357478 pyprql-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      140 2023-04-02 03:11:27.321478 pyprql-0.7.0/pyprql/__init__.py
--rw-r--r--   0        0        0     6207 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/magic/README.md
--rw-r--r--   0        0        0      689 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/magic/__init__.py
--rw-r--r--   0        0        0     4303 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/magic/prql.py
--rw-r--r--   0        0        0      246 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/pandas_accessor/__init__.py
--rw-r--r--   0        0        0      878 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/pandas_accessor/prql.py
--rw-r--r--   0        0        0        0 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/py.typed
--rw-r--r--   0        0        0      645 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/tests/__init__.py
--rw-r--r--   0        0        0       30 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/tests/_regtest_outputs/test_magic.test_memory_db.out
--rw-r--r--   0        0        0       33 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/tests/_regtest_outputs/test_magic.test_pass_existing_engine.out
--rw-r--r--   0        0        0     1947 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/tests/conftest.py
--rw-r--r--   0        0        0    14336 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/tests/test_magic.py
--rw-r--r--   0        0        0     3037 2023-04-02 03:10:53.773138 pyprql-0.7.0/pyprql/tests/test_prql_python.py
--rw-r--r--   0        0        0     3405 1970-01-01 00:00:00.000000 pyprql-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10284 2023-04-15 04:20:51.643572 pyprql-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2278 2023-04-15 04:20:51.643572 pyprql-0.8.0/README.md
+-rw-r--r--   0        0        0     2213 2023-04-15 04:21:27.104441 pyprql-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-04-15 04:21:27.068440 pyprql-0.8.0/pyprql/__init__.py
+-rw-r--r--   0        0        0     6502 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/magic/README.md
+-rw-r--r--   0        0        0      689 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/magic/__init__.py
+-rw-r--r--   0        0        0     4440 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/magic/prql.py
+-rw-r--r--   0        0        0      246 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/pandas_accessor/__init__.py
+-rw-r--r--   0        0        0      878 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/pandas_accessor/prql.py
+-rw-r--r--   0        0        0        0 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/py.typed
+-rw-r--r--   0        0        0      645 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/_regtest_outputs/test_magic.test_memory_db.out
+-rw-r--r--   0        0        0       33 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/_regtest_outputs/test_magic.test_pass_existing_engine.out
+-rw-r--r--   0        0        0     1947 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/conftest.py
+-rw-r--r--   0        0        0    14569 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/test_magic.py
+-rw-r--r--   0        0        0     3037 2023-04-15 04:20:51.643572 pyprql-0.8.0/pyprql/tests/test_prql_python.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 pyprql-0.8.0/PKG-INFO
```

### Comparing `pyprql-0.7.0/LICENSE` & `pyprql-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprql-0.7.0/README.md` & `pyprql-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyprql-0.7.0/pyproject.toml` & `pyprql-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 ]
 description = "Python extensions for PRQL"
 homepage = "https://prql-lang.org"
 license = "Apache-2.0"
 name = "pyprql"
 readme = "README.md"
 repository = "https://github.com/prql/pyprql"
-version = "0.7.0"
+version = "0.8.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 duckdb-engine = "^0.7"
 ipython = "^8"
-jupysql = "^0.6"
-pandas = "^1"
-prql-python = "^0.7"
+jupysql = ">=0.7"
+pandas = ">=1.5"
+prql-python = "^0.8"
 traitlets = "^5"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "~4.3"
 black = "^22.1.0"
 commitizen = "^2.21.2"
 coverage = "^6.3.2"
@@ -50,14 +50,15 @@
 pytest-testmon = "*"
 pytest-xdist = "^2.5.0"
 python-semantic-release = "^7.32.2"
 ruff = "^0.0.225"
 safety = "^2"
 sphinx-rtd-theme = "^1.0.0"
 xdoctest = "^0.15.10"
+polars = ">=0.16"
 
 [tool.poetry.scripts]
 pyprql = "pyprql.cli.__init__:main"
 
 [tool.semantic_release]
 branch = "main"
 build_command = "poetry build"
```

### Comparing `pyprql-0.7.0/pyprql/magic/README.md` & `pyprql-0.8.0/pyprql/magic/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -155,14 +155,17 @@
     Current: True
 PrqlMagic.autolimit=<Int>
     Automatically limit the size of the returned result sets
     Current: 0
 PrqlMagic.autopandas=<Bool>
     Return Pandas DataFrames instead of regular result sets
     Current: True
+PrqlMagic.autopolars=<Bool>
+    Return Polars DataFrames instead of regular result sets
+    Current: False
 PrqlMagic.autoview=<Bool>
     Display results
     Current: True
 PrqlMagic.column_local_vars=<Bool>
     Return data into local variables from column names
     Current: False
 PrqlMagic.displaycon=<Bool>
@@ -179,14 +182,18 @@
     Path to DSN file. When the first argument is of the form [section], a
     sqlalchemy connection string is formed from the matching section in the DSN
     file.
     Current: 'odbc.ini'
 PrqlMagic.feedback=<Bool>
     Print number of rows affected by DML
     Current: False
+PrqlMagic.polars_dataframe_kwargs=<key-1>=<value-1>...
+    Polars DataFrame constructor keyword arguments(e.g. infer_schema_length,
+    nan_to_null, schema_overrides, etc)
+    Current: {}
 PrqlMagic.short_errors=<Bool>
     Don't display the full traceback on SQL Programming Error
     Current: True
 PrqlMagic.style=<Unicode>
     Set the table printing style to any of prettytable's defined styles
     (currently DEFAULT, MSWORD_FRIENDLY, PLAIN_COLUMNS, RANDOM)
     Current: 'DEFAULT'
```

### Comparing `pyprql-0.7.0/pyprql/magic/__init__.py` & `pyprql-0.8.0/pyprql/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.7.0/pyprql/magic/prql.py` & `pyprql-0.8.0/pyprql/magic/prql.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 
     displaycon = Bool(False, config=True, help="Show connection string after execute")
     autopandas = Bool(
         True,
         config=True,
         help="Return Pandas DataFrames instead of regular result sets",
     )
+    autopolars = Bool(
+        False,
+        config=True,
+        help="Return Polars DataFrames instead of regular result sets",
+    )
     autoview = Bool(True, config=True, help="Display results")
     feedback = Bool(False, config=True, help="Print number of rows affected by DML")
     target = Unicode("sql.any", config=True, help="Compile target of prql-compiler")
     dryrun = Bool(False, config=True, help="Only print the compiled SQL")
 
     @needs_local_scope
     @line_magic("prql")
```

### Comparing `pyprql-0.7.0/pyprql/pandas_accessor/prql.py` & `pyprql-0.8.0/pyprql/pandas_accessor/prql.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.7.0/pyprql/tests/__init__.py` & `pyprql-0.8.0/pyprql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.7.0/pyprql/tests/conftest.py` & `pyprql-0.8.0/pyprql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.7.0/pyprql/tests/test_magic.py` & `pyprql-0.8.0/pyprql/tests/test_magic.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 import os.path
 import re
 import tempfile
 from textwrap import dedent
 
+import polars as pl
 import pytest
 from sqlalchemy import create_engine
 
 from pyprql.tests import run_sql
 
 from . import run_prql
 
@@ -258,21 +259,30 @@
 def test_bind_vars(ip):
     ip.user_global_ns["x"] = 22
     result = run_prql(ip, "SELECT :x")
     assert result[0][0] == 22
 
 
 def test_autopandas(ip):
-    ip.run_line_magic("config", "SqlMagic.autopandas = True")
     dframe = run_prql(ip, "from test")
     assert not dframe.empty
     assert dframe.ndim == 2
     assert dframe.name[0] == "foo"
 
 
+def test_autopolars(ip):
+    ip.run_line_magic("config", "PrqlMagic.autopolars = True")
+    dframe = run_prql(ip, "from test")
+
+    assert type(dframe) == pl.DataFrame
+    assert not dframe.is_empty()
+    assert len(dframe.shape) == 2
+    assert dframe["name"][0] == "foo"
+
+
 def test_target_dialect(ip):
     ip.run_line_magic("config", 'PrqlMagic.target = "sql.sqlite"')
     dframe = run_prql(
         ip, 'from author | select foo = f"{first_name}-{last_name}" | take 1'
     )
     assert dframe.foo[0] == "William-Shakespeare"
```

### Comparing `pyprql-0.7.0/pyprql/tests/test_prql_python.py` & `pyprql-0.8.0/pyprql/tests/test_prql_python.py`

 * *Files identical despite different names*

### Comparing `pyprql-0.7.0/PKG-INFO` & `pyprql-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprql
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python extensions for PRQL
 Home-page: https://prql-lang.org
 License: Apache-2.0
 Author: Charlie Sanders
 Author-email: charlie.fats@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,17 +17,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: duckdb-engine (>=0.7,<0.8)
 Requires-Dist: ipython (>=8,<9)
-Requires-Dist: jupysql (>=0.6,<0.7)
-Requires-Dist: pandas (>=1,<2)
-Requires-Dist: prql-python (>=0.7,<0.8)
+Requires-Dist: jupysql (>=0.7)
+Requires-Dist: pandas (>=1.5)
+Requires-Dist: prql-python (>=0.8,<0.9)
 Requires-Dist: traitlets (>=5,<6)
 Project-URL: Repository, https://github.com/prql/pyprql
 Description-Content-Type: text/markdown
 
 # pyprql
 
 [![CI/CD](https://github.com/prql/pyprql/actions/workflows/pull-request.yaml/badge.svg?branch=main)](https://github.com/prql/pyprql/actions/workflows/pull-request.yaml)
```

