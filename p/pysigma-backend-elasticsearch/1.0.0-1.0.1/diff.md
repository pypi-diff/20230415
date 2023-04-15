# Comparing `tmp/pysigma_backend_elasticsearch-1.0.0.tar.gz` & `tmp/pysigma_backend_elasticsearch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_elasticsearch-1.0.0.tar", max compression
+gzip compressed data, was "pysigma_backend_elasticsearch-1.0.1.tar", max compression
```

## Comparing `pysigma_backend_elasticsearch-1.0.0.tar` & `pysigma_backend_elasticsearch-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7653 2023-04-14 23:51:00.694198 pysigma_backend_elasticsearch-1.0.0/LICENSE
--rw-r--r--   0        0        0      572 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       92 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/backends/elasticsearch/__init__.py
--rw-r--r--   0        0        0    14039 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/backends/elasticsearch/elasticsearch.py
--rw-r--r--   0        0        0      307 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/__init__.py
--rw-r--r--   0        0        0    10111 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/windows.py
--rw-r--r--   0        0        0    61044 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/zeek.py
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-04-15 00:12:32.651280 pysigma_backend_elasticsearch-1.0.1/LICENSE
+-rw-r--r--   0        0        0      572 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/backends/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    14661 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/backends/elasticsearch/elasticsearch.py
+-rw-r--r--   0        0        0      307 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    10111 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/windows.py
+-rw-r--r--   0        0        0    61044 2023-04-15 00:12:32.655280 pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/zeek.py
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.1/PKG-INFO
```

### Comparing `pysigma_backend_elasticsearch-1.0.0/LICENSE` & `pysigma_backend_elasticsearch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.0/pyproject.toml` & `pysigma_backend_elasticsearch-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pySigma-backend-elasticsearch"
-version = "1.0.0"
+version = "1.0.1"
 description = "pySigma Elasticsearch backend"
 authors = ["Thomas Patzke <thomas@patzke.org>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-elasticsearch"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = "^0.9.6"
+pysigma = "^0.9.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 coverage = "^6.4.1"
 requests = "^2.28.1"
```

### Comparing `pysigma_backend_elasticsearch-1.0.0/sigma/backends/elasticsearch/elasticsearch.py` & `pysigma_backend_elasticsearch-1.0.1/sigma/backends/elasticsearch/elasticsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 
 class LuceneBackend(TextQueryBackend):
     """
     Elasticsearch query string backend. Generates query strings described here in the Elasticsearch documentation:
 
     https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-query-string-query.html#query-string-syntax
     """
+    name : ClassVar[str] = "Elasticsearch Lucene"               # A descriptive name of the backend
+    formats : ClassVar[Dict[str, str]] = {                # Output formats provided by the backend as name -> description mapping. The name should match to finalize_output_<name>.
+        "default": "Plain Elasticsearch Lucene queries",
+        "kibana_ndjson": "Kibana NDJSON import file with Lucene queries",
+        "dsl_lucene": "Elasticsearch query DSL with embedded Lucene queries",
+    }
+    requires_pipeline : ClassVar[bool] = True             # Does the backend requires that a processing pipeline is provided?
+
     # Operator precedence: tuple of Condition{AND,OR,NOT} in order of precedence.
     # The backend generates grouping if required
     precedence : ClassVar[Tuple[ConditionItem, ConditionItem, ConditionItem]] = (ConditionNOT, ConditionOR, ConditionAND)
     group_expression : ClassVar[str] = "({expr})"   # Expression for precedence override grouping as format string with {expr} placeholder
     parenthesize: bool = True
 
     # Generated query tokens
```

### Comparing `pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/windows.py` & `pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/windows.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/zeek.py` & `pysigma_backend_elasticsearch-1.0.1/sigma/pipelines/elasticsearch/zeek.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_elasticsearch-1.0.0/PKG-INFO` & `pysigma_backend_elasticsearch-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-elasticsearch
-Version: 1.0.0
+Version: 1.0.1
 Summary: pySigma Elasticsearch backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-elasticsearch
 License: LGPL-3.0-only
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pysigma (>=0.9.6,<0.10.0)
+Requires-Dist: pysigma (>=0.9.5,<0.10.0)
 Project-URL: Repository, https://github.com/SigmaHQ/pySigma-backend-elasticsearch
```

