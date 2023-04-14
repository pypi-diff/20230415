# Comparing `tmp/groundlight-0.7.6.tar.gz` & `tmp/groundlight-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.7.6.tar", max compression
+gzip compressed data, was "groundlight-0.7.7.tar", max compression
```

## Comparing `groundlight-0.7.6.tar` & `groundlight-0.7.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-04-14 23:14:39.436882 groundlight-0.7.6/LICENSE
--rw-r--r--   0        0        0     1604 2023-04-14 23:14:39.436882 groundlight-0.7.6/README.md
--rw-r--r--   0        0        0     3597 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/model.py
--rw-r--r--   0        0        0      721 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14018 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14322 2023-04-14 23:14:39.440882 groundlight-0.7.6/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35591 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      537 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17643 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     4979 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13623 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13486 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11288 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13847 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11330 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12129 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12150 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11438 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79719 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1007 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14005 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/openapi_client/rest.py
--rw-r--r--   0        0        0      955 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/setup.py
--rw-r--r--   0        0        0        0 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-04-14 23:14:39.444882 groundlight-0.7.6/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0     1792 2023-04-14 23:14:39.448882 groundlight-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/__init__.py
--rw-r--r--   0        0        0     1806 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0    10411 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/config.py
--rw-r--r--   0        0        0     2074 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/images.py
--rw-r--r--   0        0        0     5757 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1778 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0      308 2023-04-14 23:14:39.448882 groundlight-0.7.6/src/groundlight/status_codes.py
--rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 groundlight-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-14 23:50:35.066178 groundlight-0.7.7/LICENSE
+-rw-r--r--   0        0        0     1794 2023-04-14 23:50:35.066178 groundlight-0.7.7/README.md
+-rw-r--r--   0        0        0     3597 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/model.py
+-rw-r--r--   0        0        0      721 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14018 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14322 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35591 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      537 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17643 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     4979 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11870 2023-04-14 23:50:35.070179 groundlight-0.7.7/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13623 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13486 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11288 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13847 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11330 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12129 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12150 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11438 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79719 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1007 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14005 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0      955 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-04-14 23:50:35.074179 groundlight-0.7.7/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0     1804 2023-04-14 23:50:35.074179 groundlight-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     1806 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0    10411 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/config.py
+-rw-r--r--   0        0        0     2074 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/images.py
+-rw-r--r--   0        0        0     5757 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1778 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0      308 2023-04-14 23:50:35.078179 groundlight-0.7.7/src/groundlight/status_codes.py
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 groundlight-0.7.7/PKG-INFO
```

### Comparing `groundlight-0.7.6/LICENSE` & `groundlight-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/README.md` & `groundlight-0.7.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 
 ## Computer Vision powered by Natural Language
 
 ```bash
 pip install groundlight
 ```
 
-Build a working computer vision system in just 5 lines of python:
+Build a working computer vision system in just a few lines of python:
 
 ```python
 from groundlight import Groundlight
+from PIL import Image
+import requests
 
 gl = Groundlight()
-d = gl.get_or_create_detector(name="door", query="Is the door open?")
-image_query = gl.submit_image_query(detector=d, image=jpeg_img)
+d = gl.get_or_create_detector(name="doorway", query="Is the doorway open?")
+image_url = "https://images.selfstorage.com/large-compress/2174925f24362c479b2.jpg"
+image = Image.open(requests.get(image_url, stream=True).raw)
+image_query = gl.submit_image_query(detector=d, image=image)
 print(f"The answer is {image_query.result}")
 ```
 
 ### How does it work?
 
 Your images are first analyzed by machine learning (ML) models which are automatically trained on your data. If those models have high enough confidence, that's your answer. But if the models are unsure, then the images are progressively escalated to more resource-intensive analysis methods up to real-time human review. So what you get is a computer vision system that starts working right away without even needing to first gather and label a dataset. At first it will operate with high latency, because people need to review the image queries. But over time, the ML systems will learn and improve so queries come back faster with higher confidence.
```

### Comparing `groundlight-0.7.6/generated/model.py` & `groundlight-0.7.7/generated/model.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/__init__.py` & `groundlight-0.7.7/generated/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/api/detectors_api.py` & `groundlight-0.7.7/generated/openapi_client/api/detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.7.7/generated/openapi_client/api/image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/api_client.py` & `groundlight-0.7.7/generated/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/apis/__init__.py` & `groundlight-0.7.7/generated/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/configuration.py` & `groundlight-0.7.7/generated/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/exceptions.py` & `groundlight-0.7.7/generated/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/classification_result.py` & `groundlight-0.7.7/generated/openapi_client/model/classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/detector.py` & `groundlight-0.7.7/generated/openapi_client/model/detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.7.7/generated/openapi_client/model/detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.7.7/generated/openapi_client/model/detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/image_query.py` & `groundlight-0.7.7/generated/openapi_client/model/image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.7.7/generated/openapi_client/model/image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.7.7/generated/openapi_client/model/paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.7.7/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.7.7/generated/openapi_client/model/result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/model_utils.py` & `groundlight-0.7.7/generated/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/models/__init__.py` & `groundlight-0.7.7/generated/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/openapi_client/rest.py` & `groundlight-0.7.7/generated/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/setup.py` & `groundlight-0.7.7/generated/setup.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_classification_result.py` & `groundlight-0.7.7/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_detector.py` & `groundlight-0.7.7/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_detector_creation_input.py` & `groundlight-0.7.7/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_detector_type_enum.py` & `groundlight-0.7.7/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_detectors_api.py` & `groundlight-0.7.7/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_image_queries_api.py` & `groundlight-0.7.7/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_image_query.py` & `groundlight-0.7.7/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_image_query_type_enum.py` & `groundlight-0.7.7/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_paginated_detector_list.py` & `groundlight-0.7.7/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_paginated_image_query_list.py` & `groundlight-0.7.7/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/generated/test/test_result_type_enum.py` & `groundlight-0.7.7/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/pyproject.toml` & `groundlight-0.7.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 authors = ["Groundlight AI <support@groundlight.ai>"]
 description = "Build computer vision systems from natural language with Groundlight"
-homepage = "https://www.groundlight.ai"
+homepage = "https://code.groundlight.ai/python-sdk"
 license = "MIT"
 name = "groundlight"
 packages = [
     {include = "**/*.py", from = "generated"},
     {include = "**/*.py", from = "src"},
 ]
 readme = "README.md"
-version = "0.7.6"
+version = "0.7.7"
 
 [tool.poetry.dependencies]
 certifi = "^2021.10.8"
 frozendict = "^2.3.2"
 pillow = "^9.0.0" # TODO: We may want to mark pillow (and numpy) as extra (https://python-poetry.org/docs/master/pyproject#extras)
 pydantic = "^1.7.4"
 python = ">=3.7.0,<4.0"
```

### Comparing `groundlight-0.7.6/src/groundlight/__init__.py` & `groundlight-0.7.7/src/groundlight/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/src/groundlight/binary_labels.py` & `groundlight-0.7.7/src/groundlight/binary_labels.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/src/groundlight/client.py` & `groundlight-0.7.7/src/groundlight/client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/src/groundlight/images.py` & `groundlight-0.7.7/src/groundlight/images.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/src/groundlight/internalapi.py` & `groundlight-0.7.7/src/groundlight/internalapi.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/src/groundlight/optional_imports.py` & `groundlight-0.7.7/src/groundlight/optional_imports.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.6/PKG-INFO` & `groundlight-0.7.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: groundlight
-Version: 0.7.6
+Version: 0.7.7
 Summary: Build computer vision systems from natural language with Groundlight
-Home-page: https://www.groundlight.ai
+Home-page: https://code.groundlight.ai/python-sdk
 License: MIT
 Author: Groundlight AI
 Author-email: support@groundlight.ai
 Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -29,22 +29,26 @@
 
 ## Computer Vision powered by Natural Language
 
 ```bash
 pip install groundlight
 ```
 
-Build a working computer vision system in just 5 lines of python:
+Build a working computer vision system in just a few lines of python:
 
 ```python
 from groundlight import Groundlight
+from PIL import Image
+import requests
 
 gl = Groundlight()
-d = gl.get_or_create_detector(name="door", query="Is the door open?")
-image_query = gl.submit_image_query(detector=d, image=jpeg_img)
+d = gl.get_or_create_detector(name="doorway", query="Is the doorway open?")
+image_url = "https://images.selfstorage.com/large-compress/2174925f24362c479b2.jpg"
+image = Image.open(requests.get(image_url, stream=True).raw)
+image_query = gl.submit_image_query(detector=d, image=image)
 print(f"The answer is {image_query.result}")
 ```
 
 ### How does it work?
 
 Your images are first analyzed by machine learning (ML) models which are automatically trained on your data. If those models have high enough confidence, that's your answer. But if the models are unsure, then the images are progressively escalated to more resource-intensive analysis methods up to real-time human review. So what you get is a computer vision system that starts working right away without even needing to first gather and label a dataset. At first it will operate with high latency, because people need to review the image queries. But over time, the ML systems will learn and improve so queries come back faster with higher confidence.
```

