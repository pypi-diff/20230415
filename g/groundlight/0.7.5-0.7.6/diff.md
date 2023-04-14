# Comparing `tmp/groundlight-0.7.5.tar.gz` & `tmp/groundlight-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.7.5.tar", max compression
+gzip compressed data, was "groundlight-0.7.6.tar", max compression
```

## Comparing `groundlight-0.7.5.tar` & `groundlight-0.7.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-04-14 22:37:58.397035 groundlight-0.7.5/LICENSE
--rw-r--r--   0        0        0     1604 2023-04-14 22:37:58.397035 groundlight-0.7.5/README.md
--rw-r--r--   0        0        0     3597 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/model.py
--rw-r--r--   0        0        0      721 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14018 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14322 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35591 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      537 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17643 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     4979 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13623 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13486 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11288 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13847 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11330 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12129 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12150 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11438 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79719 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1007 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14005 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/rest.py
--rw-r--r--   0        0        0      955 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/setup.py
--rw-r--r--   0        0        0        0 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0     1792 2023-04-14 22:37:58.409036 groundlight-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/__init__.py
--rw-r--r--   0        0        0     1806 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0    10411 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/config.py
--rw-r--r--   0        0        0     2074 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/images.py
--rw-r--r--   0        0        0     5757 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1778 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0      308 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/status_codes.py
--rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 groundlight-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-14 23:14:39.436882 groundlight-0.7.6/LICENSE
+-rw-r--r--   0        0        0     1604 2023-04-14 23:14:39.436882 groundlight-0.7.6/README.md
+-rw-r--r--   0        0        0     3597 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/model.py
+-rw-r--r--   0        0        0      721 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14018 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14322 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35591 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      537 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17643 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     4979 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11870 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13623 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13486 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11288 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13847 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11330 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12129 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12150 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11438 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79719 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1007 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14005 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0      955 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0     1792 2023-04-14 23:14:39.448882 groundlight-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     1806 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0    10411 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/config.py
+-rw-r--r--   0        0        0     2074 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/images.py
+-rw-r--r--   0        0        0     5757 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1778 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0      308 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/status_codes.py
+-rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 groundlight-0.7.6/PKG-INFO
```

### Comparing `groundlight-0.7.5/LICENSE` & `groundlight-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/README.md` & `groundlight-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/model.py` & `groundlight-0.7.6/generated/model.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/__init__.py` & `groundlight-0.7.6/generated/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/api/detectors_api.py` & `groundlight-0.7.6/generated/openapi_client/api/detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.7.6/generated/openapi_client/api/image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/api_client.py` & `groundlight-0.7.6/generated/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/apis/__init__.py` & `groundlight-0.7.6/generated/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/configuration.py` & `groundlight-0.7.6/generated/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/exceptions.py` & `groundlight-0.7.6/generated/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/classification_result.py` & `groundlight-0.7.6/generated/openapi_client/model/classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/detector.py` & `groundlight-0.7.6/generated/openapi_client/model/detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.7.6/generated/openapi_client/model/detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.7.6/generated/openapi_client/model/detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/image_query.py` & `groundlight-0.7.6/generated/openapi_client/model/image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.7.6/generated/openapi_client/model/image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.7.6/generated/openapi_client/model/paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.7.6/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.7.6/generated/openapi_client/model/result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/model_utils.py` & `groundlight-0.7.6/generated/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/models/__init__.py` & `groundlight-0.7.6/generated/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/openapi_client/rest.py` & `groundlight-0.7.6/generated/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/setup.py` & `groundlight-0.7.6/generated/setup.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_classification_result.py` & `groundlight-0.7.6/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_detector.py` & `groundlight-0.7.6/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_detector_creation_input.py` & `groundlight-0.7.6/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_detector_type_enum.py` & `groundlight-0.7.6/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_detectors_api.py` & `groundlight-0.7.6/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_image_queries_api.py` & `groundlight-0.7.6/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_image_query.py` & `groundlight-0.7.6/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_image_query_type_enum.py` & `groundlight-0.7.6/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_paginated_detector_list.py` & `groundlight-0.7.6/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_paginated_image_query_list.py` & `groundlight-0.7.6/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/generated/test/test_result_type_enum.py` & `groundlight-0.7.6/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/pyproject.toml` & `groundlight-0.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = "MIT"
 name = "groundlight"
 packages = [
     {include = "**/*.py", from = "generated"},
     {include = "**/*.py", from = "src"},
 ]
 readme = "README.md"
-version = "0.7.5"
+version = "0.7.6"
 
 [tool.poetry.dependencies]
 certifi = "^2021.10.8"
 frozendict = "^2.3.2"
 pillow = "^9.0.0" # TODO: We may want to mark pillow (and numpy) as extra (https://python-poetry.org/docs/master/pyproject#extras)
 pydantic = "^1.7.4"
 python = ">=3.7.0,<4.0"
```

### Comparing `groundlight-0.7.5/src/groundlight/__init__.py` & `groundlight-0.7.6/src/groundlight/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/src/groundlight/binary_labels.py` & `groundlight-0.7.6/src/groundlight/binary_labels.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/src/groundlight/client.py` & `groundlight-0.7.6/src/groundlight/client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/src/groundlight/images.py` & `groundlight-0.7.6/src/groundlight/images.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/src/groundlight/internalapi.py` & `groundlight-0.7.6/src/groundlight/internalapi.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/src/groundlight/optional_imports.py` & `groundlight-0.7.6/src/groundlight/optional_imports.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.5/PKG-INFO` & `groundlight-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groundlight
-Version: 0.7.5
+Version: 0.7.6
 Summary: Build computer vision systems from natural language with Groundlight
 Home-page: https://www.groundlight.ai
 License: MIT
 Author: Groundlight AI
 Author-email: support@groundlight.ai
 Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

