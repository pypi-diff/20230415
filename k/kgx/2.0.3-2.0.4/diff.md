# Comparing `tmp/kgx-2.0.3.tar.gz` & `tmp/kgx-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgx-2.0.3.tar", max compression
+gzip compressed data, was "kgx-2.0.4.tar", max compression
```

## Comparing `kgx-2.0.3.tar` & `kgx-2.0.4.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1526 2023-03-29 23:44:20.859840 kgx-2.0.3/LICENSE
--rw-r--r--   0        0        0     6472 2023-03-29 23:44:20.859840 kgx-2.0.3/README.md
--rw-r--r--   0        0        0       42 2023-03-29 23:44:36.627686 kgx-2.0.3/kgx/__init__.py
--rw-r--r--   0        0        0    16105 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/cli/__init__.py
--rw-r--r--   0        0        0    39539 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/cli/cli_utils.py
--rw-r--r--   0        0        0     3900 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/config.py
--rw-r--r--   0        0        0      731 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/config.yml
--rw-r--r--   0        0        0     1942 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/curie_lookup_service.py
--rw-r--r--   0        0        0     5094 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/error_detection.py
--rw-r--r--   0        0        0        0 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph/__init__.py
--rw-r--r--   0        0        0    10649 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph/base_graph.py
--rw-r--r--   0        0        0    13455 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph/nx_graph.py
--rw-r--r--   0        0        0     8498 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph_operations/__init__.py
--rw-r--r--   0        0        0    28863 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph_operations/clique_merge.py
--rw-r--r--   0        0        0     5776 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph_operations/graph_merge.py
--rw-r--r--   0        0        0    36314 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph_operations/meta_knowledge_graph.py
--rw-r--r--   0        0        0    30601 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/graph_operations/summarize_graph.py
--rw-r--r--   0        0        0        0 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/parsers/__init__.py
--rw-r--r--   0        0        0     2156 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/parsers/ntriples_parser.py
--rw-r--r--   0        0        0     6617 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/prefix_manager.py
--rw-r--r--   0        0        0      245 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/sink/__init__.py
--rw-r--r--   0        0        0     1703 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/sink/graph_sink.py
--rw-r--r--   0        0        0     2335 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/sink/json_sink.py
--rw-r--r--   0        0        0     2242 2023-03-29 23:44:20.859840 kgx-2.0.3/kgx/sink/jsonl_sink.py
--rw-r--r--   0        0        0     9073 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/sink/neo_sink.py
--rw-r--r--   0        0        0     1356 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/sink/null_sink.py
--rw-r--r--   0        0        0    20015 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/sink/rdf_sink.py
--rw-r--r--   0        0        0     1436 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/sink/sink.py
--rw-r--r--   0        0        0     8070 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/sink/tsv_sink.py
--rw-r--r--   0        0        0      395 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/__init__.py
--rw-r--r--   0        0        0     2526 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/graph_source.py
--rw-r--r--   0        0        0     2677 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/json_source.py
--rw-r--r--   0        0        0     1821 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/jsonl_source.py
--rw-r--r--   0        0        0    18963 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/neo_source.py
--rw-r--r--   0        0        0    11785 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/obograph_source.py
--rw-r--r--   0        0        0     7503 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/owl_source.py
--rw-r--r--   0        0        0    30464 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/rdf_source.py
--rw-r--r--   0        0        0    12162 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/source.py
--rw-r--r--   0        0        0     8221 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/sssom_source.py
--rw-r--r--   0        0        0     3665 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/trapi_source.py
--rw-r--r--   0        0        0     9206 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/source/tsv_source.py
--rw-r--r--   0        0        0    16628 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/transformer.py
--rw-r--r--   0        0        0        0 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/utils/__init__.py
--rw-r--r--   0        0        0     4575 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/utils/graph_utils.py
--rw-r--r--   0        0        0    18032 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/utils/infores.py
--rw-r--r--   0        0        0    30472 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/utils/kgx_utils.py
--rw-r--r--   0        0        0     8159 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/utils/rdf_utils.py
--rw-r--r--   0        0        0    28313 2023-03-29 23:44:20.863840 kgx-2.0.3/kgx/validator.py
--rw-r--r--   0        0        0     1569 2023-03-29 23:44:36.627686 kgx-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     8488 1970-01-01 00:00:00.000000 kgx-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-04-14 23:05:45.561249 kgx-2.0.4/LICENSE
+-rw-r--r--   0        0        0     6472 2023-04-14 23:05:45.561249 kgx-2.0.4/README.md
+-rw-r--r--   0        0        0       42 2023-04-14 23:06:15.201541 kgx-2.0.4/kgx/__init__.py
+-rw-r--r--   0        0        0    16105 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/cli/__init__.py
+-rw-r--r--   0        0        0    39538 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/cli/cli_utils.py
+-rw-r--r--   0        0        0     3900 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/config.py
+-rw-r--r--   0        0        0      731 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/config.yml
+-rw-r--r--   0        0        0     1942 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/curie_lookup_service.py
+-rw-r--r--   0        0        0     5094 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/error_detection.py
+-rw-r--r--   0        0        0        0 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph/__init__.py
+-rw-r--r--   0        0        0    10649 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph/base_graph.py
+-rw-r--r--   0        0        0    13455 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph/nx_graph.py
+-rw-r--r--   0        0        0     8498 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/__init__.py
+-rw-r--r--   0        0        0    28863 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/clique_merge.py
+-rw-r--r--   0        0        0     5776 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/graph_merge.py
+-rw-r--r--   0        0        0    36314 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/meta_knowledge_graph.py
+-rw-r--r--   0        0        0    30601 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/summarize_graph.py
+-rw-r--r--   0        0        0        0 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/parsers/__init__.py
+-rw-r--r--   0        0        0     2156 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/parsers/ntriples_parser.py
+-rw-r--r--   0        0        0     6617 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/prefix_manager.py
+-rw-r--r--   0        0        0      274 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/__init__.py
+-rw-r--r--   0        0        0     1703 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/graph_sink.py
+-rw-r--r--   0        0        0     2335 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/json_sink.py
+-rw-r--r--   0        0        0     2242 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/jsonl_sink.py
+-rw-r--r--   0        0        0     9073 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/neo_sink.py
+-rw-r--r--   0        0        0     1356 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/null_sink.py
+-rw-r--r--   0        0        0    20014 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/rdf_sink.py
+-rw-r--r--   0        0        0     1436 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/sink.py
+-rw-r--r--   0        0        0    10327 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/sql_sink.py
+-rw-r--r--   0        0        0     8070 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/tsv_sink.py
+-rw-r--r--   0        0        0      395 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/__init__.py
+-rw-r--r--   0        0        0     2526 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/graph_source.py
+-rw-r--r--   0        0        0     2399 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/json_source.py
+-rw-r--r--   0        0        0     1821 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/jsonl_source.py
+-rw-r--r--   0        0        0    18963 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/neo_source.py
+-rw-r--r--   0        0        0    11785 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/obograph_source.py
+-rw-r--r--   0        0        0     7503 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/owl_source.py
+-rw-r--r--   0        0        0    30464 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/rdf_source.py
+-rw-r--r--   0        0        0    12162 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/source.py
+-rw-r--r--   0        0        0     8221 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/sssom_source.py
+-rw-r--r--   0        0        0     3665 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/trapi_source.py
+-rw-r--r--   0        0        0     9150 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/tsv_source.py
+-rw-r--r--   0        0        0    16628 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/utils/__init__.py
+-rw-r--r--   0        0        0     4575 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/utils/graph_utils.py
+-rw-r--r--   0        0        0    18032 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/utils/infores.py
+-rw-r--r--   0        0        0    31762 2023-04-14 23:05:45.569249 kgx-2.0.4/kgx/utils/kgx_utils.py
+-rw-r--r--   0        0        0     8159 2023-04-14 23:05:45.569249 kgx-2.0.4/kgx/utils/rdf_utils.py
+-rw-r--r--   0        0        0    28313 2023-04-14 23:05:45.569249 kgx-2.0.4/kgx/validator.py
+-rw-r--r--   0        0        0     1591 2023-04-14 23:06:15.197540 kgx-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8531 1970-01-01 00:00:00.000000 kgx-2.0.4/PKG-INFO
```

### Comparing `kgx-2.0.3/LICENSE` & `kgx-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/README.md` & `kgx-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/cli/__init__.py` & `kgx-2.0.4/kgx/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/cli/cli_utils.py` & `kgx-2.0.4/kgx/cli/cli_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1070,15 +1070,15 @@
     elif output_format in get_input_file_types():
         output_args["filename"] = output
         output_args["compression"] = output_compression
         if output_format == "nt":
             output_args["reify_all_edges"] = (
                 source["output"]["reify_all_edges"]
                 if "reify_all_edges" in source["output"]
-                else False
+                else True
             )
             output_args["reverse_prefix_map"] = source_reverse_prefix_map
             output_args[
                 "reverse_predicate_mappings"
             ] = source_reverse_predicate_mappings
             output_args["property_types"] = source_property_types
     else:
```

### Comparing `kgx-2.0.3/kgx/config.py` & `kgx-2.0.4/kgx/config.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/config.yml` & `kgx-2.0.4/kgx/config.yml`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/curie_lookup_service.py` & `kgx-2.0.4/kgx/curie_lookup_service.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/error_detection.py` & `kgx-2.0.4/kgx/error_detection.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/graph/base_graph.py` & `kgx-2.0.4/kgx/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/graph/nx_graph.py` & `kgx-2.0.4/kgx/graph/nx_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/graph_operations/__init__.py` & `kgx-2.0.4/kgx/graph_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/graph_operations/clique_merge.py` & `kgx-2.0.4/kgx/graph_operations/clique_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/graph_operations/graph_merge.py` & `kgx-2.0.4/kgx/graph_operations/graph_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/graph_operations/meta_knowledge_graph.py` & `kgx-2.0.4/kgx/graph_operations/meta_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/graph_operations/summarize_graph.py` & `kgx-2.0.4/kgx/graph_operations/summarize_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/parsers/ntriples_parser.py` & `kgx-2.0.4/kgx/parsers/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/prefix_manager.py` & `kgx-2.0.4/kgx/prefix_manager.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/sink/graph_sink.py` & `kgx-2.0.4/kgx/sink/graph_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/sink/json_sink.py` & `kgx-2.0.4/kgx/sink/json_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/sink/jsonl_sink.py` & `kgx-2.0.4/kgx/sink/jsonl_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/sink/neo_sink.py` & `kgx-2.0.4/kgx/sink/neo_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/sink/null_sink.py` & `kgx-2.0.4/kgx/sink/null_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/sink/rdf_sink.py` & `kgx-2.0.4/kgx/sink/rdf_sink.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def __init__(
         self,
         owner,
         filename: str,
         format: str = "nt",
         compression: Optional[bool] = None,
-        reify_all_edges: bool = False,
+        reify_all_edges: bool = True,
         **kwargs: Any,
     ):
         super().__init__(owner)
         if format not in {"nt"}:
             raise ValueError(f"Only RDF N-Triples ('nt') serialization supported.")
         self.DEFAULT = Namespace(self.prefix_manager.prefix_map[""])
         # self.OBO = Namespace('http://purl.obolibrary.org/obo/')
```

### Comparing `kgx-2.0.3/kgx/sink/sink.py` & `kgx-2.0.4/kgx/sink/sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/sink/tsv_sink.py` & `kgx-2.0.4/kgx/sink/tsv_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/graph_source.py` & `kgx-2.0.4/kgx/source/graph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/json_source.py` & `kgx-2.0.4/kgx/source/json_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 import gzip
 import typing
-from typing import Optional, Generator, Any
 import ijson
 from itertools import chain
 from typing import Dict, Tuple, Any, Generator, Optional, List
 from kgx.config import get_logger
-from kgx.error_detection import ErrorType, MessageLevel
-from kgx.source.source import Source
-from kgx.utils.kgx_utils import (
-    generate_uuid,
-    generate_edge_key,
-    extension_types,
-    archive_read_mode,
-    sanitize_import
-)
+
 from kgx.source.tsv_source import TsvSource
 log = get_logger()
 
 
 class JsonSource(TsvSource):
     """
     JsonSource is responsible for reading data as records
```

### Comparing `kgx-2.0.3/kgx/source/jsonl_source.py` & `kgx-2.0.4/kgx/source/jsonl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/neo_source.py` & `kgx-2.0.4/kgx/source/neo_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/obograph_source.py` & `kgx-2.0.4/kgx/source/obograph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/owl_source.py` & `kgx-2.0.4/kgx/source/owl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/rdf_source.py` & `kgx-2.0.4/kgx/source/rdf_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/source.py` & `kgx-2.0.4/kgx/source/source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/sssom_source.py` & `kgx-2.0.4/kgx/source/sssom_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/trapi_source.py` & `kgx-2.0.4/kgx/source/trapi_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/source/tsv_source.py` & `kgx-2.0.4/kgx/source/tsv_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 import tarfile
 import typing
 from typing import Dict, Tuple, Any, Generator, Optional, List
 import pandas as pd
 
 from kgx.config import get_logger
-from kgx.error_detection import ErrorType, MessageLevel
 from kgx.source.source import Source
 from kgx.utils.kgx_utils import (
     generate_uuid,
     generate_edge_key,
     extension_types,
     archive_read_mode,
     sanitize_import
```

### Comparing `kgx-2.0.3/kgx/transformer.py` & `kgx-2.0.4/kgx/transformer.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/utils/graph_utils.py` & `kgx-2.0.4/kgx/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/utils/infores.py` & `kgx-2.0.4/kgx/utils/infores.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/utils/kgx_utils.py` & `kgx-2.0.4/kgx/utils/kgx_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import re
 import time
 import uuid
+import sqlite3
 from enum import Enum
 from typing import List, Dict, Set, Optional, Any, Union
 import stringcase
 from inflection import camelize
 from linkml_runtime.linkml_model.meta import (
     TypeDefinitionName,
     EnumDefinition,
@@ -64,15 +65,15 @@
     "negated": bool,
     "xrefs": list,
 }
 column_types.update(provenance_slot_types)
 
 knowledge_provenance_properties = set(provenance_slot_types.keys())
 
-extension_types = {"csv": ",", "tsv": "\t", "csv:neo4j": ",", "tsv:neo4j": "\t"}
+extension_types = {"csv": ",", "tsv": "\t", "csv:neo4j": ",", "tsv:neo4j": "\t", "sql": "|"}
 
 archive_read_mode = {"tar": "r", "tar.gz": "r:gz", "tar.bz2": "r:bz2"}
 archive_write_mode = {"tar": "w", "tar.gz": "w:gz", "tar.bz2": "w:bz2"}
 
 archive_format = {
     "r": "tar",
     "r:gz": "tar.gz",
@@ -1064,7 +1065,58 @@
     for operation in operations:
         op_name = operation["name"]
         op_args = operation["args"]
         module_name = ".".join(op_name.split(".")[0:-1])
         function_name = op_name.split(".")[-1]
         f = getattr(importlib.import_module(module_name), function_name)
         f(graph, **op_args)
+
+
+def create_connection(db_file):
+    """ create a database connection to the SQLite database
+        specified by db_file
+    :param db_file: database file
+    :return: Connection object or None
+    """
+    conn = None
+    try:
+        conn = sqlite3.connect(db_file)
+    except ConnectionError as e:
+        print(e)
+
+    return conn
+
+
+def close_connection(conn):
+    """ close a database connection to the SQLite database
+    :return: None
+    """
+
+    try:
+        if conn:
+            conn.close()
+    except ConnectionError as e:
+        print(e)
+
+    return conn
+
+
+def drop_existing_tables(conn):
+    try:
+        # Get a cursor object
+        c = conn.cursor()
+
+        # Get a list of all tables in the database
+        c.execute("SELECT name FROM sqlite_master WHERE type='table';")
+        table_names = [row[0] for row in c.fetchall()]
+
+        # Loop through the table names and drop each table
+        for table_name in table_names:
+            drop_table_sql = f"DROP TABLE IF EXISTS {table_name};"
+            c.execute(drop_table_sql)
+
+        # Commit the changes and close the connection
+        conn.commit()
+
+    except sqlite3.Error as e:
+        print(f"An error occurred while removing all tables and data from the SQLite database: {e}")
+
```

### Comparing `kgx-2.0.3/kgx/utils/rdf_utils.py` & `kgx-2.0.4/kgx/utils/rdf_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/kgx/validator.py` & `kgx-2.0.4/kgx/validator.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.3/pyproject.toml` & `kgx-2.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kgx"
-version = "2.0.3"
+version = "2.0.4"
 description = "A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model."
 authors = ["Deepak Unni <deepak.unni3@gmail.com>", "Richard Bruskiewich <richard.bruskiewich@delphinai.com>", "Sierra Moxon <smoxon@lbl.gov>"]
 
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -48,14 +48,15 @@
 jsonstreams = "^0.6.0"
 ijson = "^3.1.3"
 deprecation = "^2.1.0"
 recommonmark = "*"
 tox = "^3.0"
 bmt = "^1.0.5"
 inflection = "^0.5.1"
+closurizer = "^0.1.7"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
 [build-system]
```

### Comparing `kgx-2.0.3/PKG-INFO` & `kgx-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgx
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model.
 License: BSD
 Author: Deepak Unni
 Author-email: deepak.unni3@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: Click
 Requires-Dist: SPARQLWrapper (>=1.8.2,<2.0.0)
 Requires-Dist: Sphinx
 Requires-Dist: bmt (>=1.0.5,<2.0.0)
 Requires-Dist: cachetools (>=5.0.0,<6.0.0)
+Requires-Dist: closurizer (>=0.1.7,<0.2.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: docutils (>=0.18.1,<0.19.0)
 Requires-Dist: ijson (>=3.1.3,<4.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: jsonstreams (>=0.6.0,<0.7.0)
```

