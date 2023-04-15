# Comparing `tmp/pySigma-backend-opensearch-0.1.5.tar.gz` & `tmp/pysigma_backend_opensearch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySigma-backend-opensearch-0.1.5.tar", max compression
+gzip compressed data, was "pysigma_backend_opensearch-0.1.6.tar", max compression
```

## Comparing `pySigma-backend-opensearch-0.1.5.tar` & `pysigma_backend_opensearch-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     7653 2023-01-18 14:41:33.078559 pySigma-backend-opensearch-0.1.5/LICENSE
--rw-r--r--   0        0        0      633 2023-01-18 14:41:33.078559 pySigma-backend-opensearch-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      161 2023-01-18 14:41:33.078559 pySigma-backend-opensearch-0.1.5/sigma/backends/opensearch/__init__.py
--rw-r--r--   0        0        0     4085 2023-01-18 14:41:33.078559 pySigma-backend-opensearch-0.1.5/sigma/backends/opensearch/opensearch.py
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 pySigma-backend-opensearch-0.1.5/setup.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 pySigma-backend-opensearch-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/LICENSE
+-rw-r--r--   0        0        0      632 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/sigma/backends/opensearch/__init__.py
+-rw-r--r--   0        0        0     4791 2023-04-15 00:36:16.389696 pysigma_backend_opensearch-0.1.6/sigma/backends/opensearch/opensearch.py
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 pysigma_backend_opensearch-0.1.6/PKG-INFO
```

### Comparing `pySigma-backend-opensearch-0.1.5/LICENSE` & `pysigma_backend_opensearch-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pySigma-backend-opensearch-0.1.5/pyproject.toml` & `pysigma_backend_opensearch-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pySigma-backend-opensearch"
-version = "0.1.5"
+version = "0.1.6"
 description = "pySigma OpenSearch backend"
 authors = ["Hendrik Baecker <hendrik.baecker@dcso.de>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-opensearch"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma-backend-elasticsearch = "^0.2.0"
-pysigma = "^0.8.12"
+pysigma-backend-elasticsearch = "^1.0.0"
+pysigma = "^0.9.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 autopep8 = "^1.6.0"
 pytest-cov = "^3.0.0"
 coverage = "^6.4.1"
 requests = "^2.28.1"
```

### Comparing `pySigma-backend-opensearch-0.1.5/sigma/backends/opensearch/opensearch.py` & `pysigma_backend_opensearch-0.1.6/sigma/backends/opensearch/opensearch.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 import sigma
 import json
 from typing import ClassVar, Dict, List, Optional
 from sigma.backends.elasticsearch import LuceneBackend
 
 class OpensearchLuceneBackend(LuceneBackend):
     """OpensearchLuceneBackend backend."""
+    name : ClassVar[str] = "OpenSearch Lucene"            # A descriptive name of the backend
+    formats : ClassVar[Dict[str, str]] = {                # Output formats provided by the backend as name -> description mapping. The name should match to finalize_output_<name>.
+        "default": "Plain OpenSearch Lucene queries",
+        "dashboards_ndjson": "OpenSearch Dashboards NDJSON import file with Lucene queries",
+        "monitor_rule": "OpenSearch monitor rule with embedded Lucene query",
+        "dsl_lucene": "OpenSearch query DSL with embedded Lucene queries",
+    }
+    requires_pipeline : ClassVar[bool] = True             # Does the backend requires that a processing pipeline is provided?
 
     def __init__(self, processing_pipeline: Optional["sigma.processing.pipeline.ProcessingPipeline"] = None,
         collect_errors: bool = False, index_names : List = ["beats-*"], monitor_interval : int = 5,
         monitor_interval_unit : str = "MINUTES", **kwargs):
 
         super().__init__(processing_pipeline, collect_errors, **kwargs)
         self.index_names = index_names or ["beats-*"]
```

### Comparing `pySigma-backend-opensearch-0.1.5/PKG-INFO` & `pysigma_backend_opensearch-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-opensearch
-Version: 0.1.5
+Version: 0.1.6
 Summary: pySigma OpenSearch backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-opensearch
 License: LGPL-3.0-only
 Author: Hendrik Baecker
 Author-email: hendrik.baecker@dcso.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: pysigma (>=0.8.12,<0.9.0)
-Requires-Dist: pysigma-backend-elasticsearch (>=0.2.0,<0.3.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pysigma (>=0.9.5,<0.10.0)
+Requires-Dist: pysigma-backend-elasticsearch (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/SigmaHQ/pySigma-backend-opensearch
```

