# Comparing `tmp/pySigma-backend-elasticsearch-0.2.0.tar.gz` & `tmp/pysigma_backend_elasticsearch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySigma-backend-elasticsearch-0.2.0.tar", max compression
+gzip compressed data, was "pysigma_backend_elasticsearch-1.0.0.tar", max compression
```

## Comparing `pySigma-backend-elasticsearch-0.2.0.tar` & `pysigma_backend_elasticsearch-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     7653 2023-01-18 14:15:16.608780 pySigma-backend-elasticsearch-0.2.0/LICENSE
--rw-r--r--   0        0        0      573 2023-01-18 14:15:16.608780 pySigma-backend-elasticsearch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       40 2023-01-18 14:15:16.608780 pySigma-backend-elasticsearch-0.2.0/sigma/backends/elasticsearch/__init__.py
--rw-r--r--   0        0        0    14039 2023-01-18 14:15:16.608780 pySigma-backend-elasticsearch-0.2.0/sigma/backends/elasticsearch/elasticsearch.py
--rw-r--r--   0        0        0        0 2023-01-18 14:15:16.608780 pySigma-backend-elasticsearch-0.2.0/sigma/pipelines/elasticsearch/__init__.py
--rw-r--r--   0        0        0    10561 2023-01-18 14:15:16.608780 pySigma-backend-elasticsearch-0.2.0/sigma/pipelines/elasticsearch/windows.py
--rw-r--r--   0        0        0    60870 2023-01-18 14:15:16.608780 pySigma-backend-elasticsearch-0.2.0/sigma/pipelines/elasticsearch/zeek.py
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 pySigma-backend-elasticsearch-0.2.0/setup.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 pySigma-backend-elasticsearch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-04-14 23:51:00.694198 pysigma_backend_elasticsearch-1.0.0/LICENSE
+-rw-r--r--   0        0        0      572 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/backends/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    14039 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/backends/elasticsearch/elasticsearch.py
+-rw-r--r--   0        0        0      307 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    10111 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/windows.py
+-rw-r--r--   0        0        0    61044 2023-04-14 23:51:00.698198 pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/zeek.py
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pysigma_backend_elasticsearch-1.0.0/PKG-INFO
```

### Comparing `pySigma-backend-elasticsearch-0.2.0/LICENSE` & `pysigma_backend_elasticsearch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pySigma-backend-elasticsearch-0.2.0/pyproject.toml` & `pysigma_backend_elasticsearch-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pySigma-backend-elasticsearch"
-version = "0.2.0"
+version = "1.0.0"
 description = "pySigma Elasticsearch backend"
 authors = ["Thomas Patzke <thomas@patzke.org>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-elasticsearch"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = "^0.8.12"
+pysigma = "^0.9.6"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 coverage = "^6.4.1"
 requests = "^2.28.1"
```

### Comparing `pySigma-backend-elasticsearch-0.2.0/sigma/backends/elasticsearch/elasticsearch.py` & `pysigma_backend_elasticsearch-1.0.0/sigma/backends/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pySigma-backend-elasticsearch-0.2.0/sigma/pipelines/elasticsearch/windows.py` & `pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/windows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sigma.pipelines.common import logsource_windows, windows_logsource_mapping
+from sigma.pipelines.common import logsource_windows, windows_logsource_mapping, generate_windows_logsource_items
 from sigma.processing.transformations import FieldMappingTransformation, AddFieldnamePrefixTransformation, AddConditionTransformation
 from sigma.processing.conditions import LogsourceCondition, IncludeFieldCondition, FieldNameProcessingItemAppliedCondition
 from sigma.processing.pipeline import ProcessingItem, ProcessingPipeline
 
 ecs_windows_variable_mappings = {
     "FileVersion": (
         ("category", "process_creation", "process.pe.file_version"),
@@ -66,22 +66,16 @@
     ),
 }
 
 def ecs_windows():
     return ProcessingPipeline(
         name="Elastic Common Schema (ECS) Windows log mappings from Winlogbeat from version 7",
         priority=20,
-        items=[
-            ProcessingItem(     # Windows log channels
-                identifier=f"elasticsearch_windows_{service}",
-                transformation=AddConditionTransformation({ "winlog.channel": source}),
-                rule_conditions=[logsource_windows(service)],
-            )
-            for service, source in windows_logsource_mapping.items()
-        ] + [                   # Variable field mappinga depending on category/service
+        allowed_backends=("elasticsearch", "opensearch"),
+        items=generate_windows_logsource_items("winlog.channel", "{source}") + [                   # Variable field mappinga depending on category/service
            ProcessingItem(
                 identifier=f"elasticsearch_windows-{field}-{logsrc_field}-{logsrc}",
                 transformation=FieldMappingTransformation({
                     field: mapped
                 }),
                 rule_conditions=[
                     LogsourceCondition(**{
@@ -187,22 +181,16 @@
         ],
     )
 
 def ecs_windows_old():
     return ProcessingPipeline(
         name="Elastic Common Schema (ECS) Windows log mappings from Winlogbeat up to version 6",
         priority=20,
-        items=[
-            ProcessingItem(     # Windows log channels
-                identifier=f"elasticsearch_windows_{service}",
-                transformation=AddConditionTransformation({ "winlog.channel": source}),
-                rule_conditions=[logsource_windows(service)],
-            )
-            for service, source in windows_logsource_mapping.items()
-        ] + [
+        allowed_backends=("elasticsearch", "opensearch"),
+        items=generate_windows_logsource_items("winlog.channel", "{source}") + [
             ProcessingItem(     # Field mappings
                 identifier="ecs_windows_field_mapping",
                 transformation=FieldMappingTransformation({
                     "EventID": "event_id",
                     "Channel": "winlog.channel",
                 }),
                 rule_conditions=[
```

### Comparing `pySigma-backend-elasticsearch-0.2.0/sigma/pipelines/elasticsearch/zeek.py` & `pysigma_backend_elasticsearch-1.0.0/sigma/pipelines/elasticsearch/zeek.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "webserver": "http",
 }
 
 def ecs_zeek_beats():
     return ProcessingPipeline(
         name="Elastic Common Schema (ECS) for Zeek using filebeat >= 7.6.1",
         priority=20,
+        allowed_backends=("elasticsearch", "opensearch"),
         items=[
             ProcessingItem(
                 identifier=f"zeek_mapping_category_{ category }_to_service_{ service }",
                 transformation=ChangeLogsourceTransformation(product="zeek", service=service),
                 rule_conditions=[
                     LogsourceCondition(category=category),
                 ],
@@ -478,14 +479,15 @@
         ],
     )
 
 def ecs_zeek_corelight():
     return ProcessingPipeline(
         name="Elastic Common Schema (ECS) mapping from Corelight",
         priority=20,
+        allowed_backends=("elasticsearch", "opensearch"),
         items=[
             ProcessingItem(
                 identifier=f"zeek_mapping_category_{ category }_to_service_{ service }",
                 transformation=ChangeLogsourceTransformation(product="zeek", service=service),
                 rule_conditions=[
                     LogsourceCondition(category=category),
                 ],
@@ -946,14 +948,15 @@
     ],
 )
 
 def zeek_raw():
     return ProcessingPipeline(
         name="Zeek raw JSON field naming",
         priority=20,
+        allowed_backends=("elasticsearch", "opensearch"),
         items=[
             ProcessingItem(
                 identifier=f"zeek_mapping_category_{ category }_to_service_{ service }",
                 transformation=ChangeLogsourceTransformation(product="zeek", service=service),
                 rule_conditions=[
                     LogsourceCondition(category=category),
                 ],
```

### Comparing `pySigma-backend-elasticsearch-0.2.0/PKG-INFO` & `pysigma_backend_elasticsearch-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-elasticsearch
-Version: 0.2.0
+Version: 1.0.0
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
-Requires-Dist: pysigma (>=0.8.12,<0.9.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pysigma (>=0.9.6,<0.10.0)
 Project-URL: Repository, https://github.com/SigmaHQ/pySigma-backend-elasticsearch
```

