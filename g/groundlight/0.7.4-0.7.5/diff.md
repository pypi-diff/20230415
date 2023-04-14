# Comparing `tmp/groundlight-0.7.4.tar.gz` & `tmp/groundlight-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.7.4.tar", max compression
+gzip compressed data, was "groundlight-0.7.5.tar", max compression
```

## Comparing `groundlight-0.7.4.tar` & `groundlight-0.7.5.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-04-12 20:20:27.404784 groundlight-0.7.4/LICENSE
--rw-r--r--   0        0        0     1606 2023-04-12 20:20:27.404784 groundlight-0.7.4/README.md
--rw-r--r--   0        0        0     3597 2023-04-12 20:20:27.408784 groundlight-0.7.4/generated/model.py
--rw-r--r--   0        0        0      723 2023-04-12 20:20:27.408784 groundlight-0.7.4/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-04-12 20:20:27.408784 groundlight-0.7.4/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14018 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14322 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35591 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      539 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17643 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     4979 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13623 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13486 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11288 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13847 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11330 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12129 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12150 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11438 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79719 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1009 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14005 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/openapi_client/rest.py
--rw-r--r--   0        0        0      955 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/setup.py
--rw-r--r--   0        0        0        0 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-04-12 20:20:27.412784 groundlight-0.7.4/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0      978 2023-04-12 20:20:27.412784 groundlight-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      537 2023-04-12 20:20:27.412784 groundlight-0.7.4/src/groundlight/__init__.py
--rw-r--r--   0        0        0     1685 2023-04-12 20:20:27.412784 groundlight-0.7.4/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0     9506 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/config.py
--rw-r--r--   0        0        0     2115 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/images.py
--rw-r--r--   0        0        0     4671 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1564 2023-04-12 20:20:27.416784 groundlight-0.7.4/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0     2575 1970-01-01 00:00:00.000000 groundlight-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-14 22:37:58.397035 groundlight-0.7.5/LICENSE
+-rw-r--r--   0        0        0     1604 2023-04-14 22:37:58.397035 groundlight-0.7.5/README.md
+-rw-r--r--   0        0        0     3597 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/model.py
+-rw-r--r--   0        0        0      721 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14018 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14322 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35591 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      537 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17643 2023-04-14 22:37:58.401036 groundlight-0.7.5/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     4979 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11870 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13623 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13486 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11288 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13847 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11330 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12129 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12150 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11438 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79719 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1007 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14005 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0      955 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-04-14 22:37:58.405036 groundlight-0.7.5/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0     1792 2023-04-14 22:37:58.409036 groundlight-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     1806 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0    10411 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/config.py
+-rw-r--r--   0        0        0     2074 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/images.py
+-rw-r--r--   0        0        0     5757 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1778 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0      308 2023-04-14 22:37:58.409036 groundlight-0.7.5/src/groundlight/status_codes.py
+-rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 groundlight-0.7.5/PKG-INFO
```

### Comparing `groundlight-0.7.4/LICENSE` & `groundlight-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/README.md` & `groundlight-0.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Groundlight Python SDK
 
-Groundlight makes it simple to build reliable visual applications.  Read the [full documentation here](https://code.groundlight.ai/python-sdk/).
+Groundlight makes it simple to build reliable visual applications. Read the [full documentation here](https://code.groundlight.ai/python-sdk/).
 
 ## Computer Vision powered by Natural Language
 
 ```bash
 pip install groundlight
 ```
 
@@ -25,12 +25,11 @@
 
 _Note: The SDK is currently in "beta" phase. Interfaces are subject to change in future versions._
 
 ## Learn more
 
 Some more resources you might like:
 
-* [Code Documentation](https://code.groundlight.ai/)
-* [Python SDK](https://pypi.org/project/groundlight/)
-* [Company](https://www.groundlight.ai/)
-* [Login to Groundlight](https://app.groundlight.ai/)
-
+- [Code Documentation](https://code.groundlight.ai/)
+- [Python SDK](https://pypi.org/project/groundlight/)
+- [Company](https://www.groundlight.ai/)
+- [Login to Groundlight](https://app.groundlight.ai/)
```

### Comparing `groundlight-0.7.4/generated/model.py` & `groundlight-0.7.5/generated/model.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/__init__.py` & `groundlight-0.7.5/generated/openapi_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# flake8: noqa
+# ruff: noqa
 
 """
     Groundlight API
 
     Ask visual queries.  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
```

### Comparing `groundlight-0.7.4/generated/openapi_client/api/detectors_api.py` & `groundlight-0.7.5/generated/openapi_client/api/detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.7.5/generated/openapi_client/api/image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/api_client.py` & `groundlight-0.7.5/generated/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/apis/__init__.py` & `groundlight-0.7.5/generated/openapi_client/apis/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# flake8: noqa
+# ruff: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
 #   from .api.detectors_api import DetectorsApi
```

### Comparing `groundlight-0.7.4/generated/openapi_client/configuration.py` & `groundlight-0.7.5/generated/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/exceptions.py` & `groundlight-0.7.5/generated/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/classification_result.py` & `groundlight-0.7.5/generated/openapi_client/model/classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/detector.py` & `groundlight-0.7.5/generated/openapi_client/model/detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.7.5/generated/openapi_client/model/detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.7.5/generated/openapi_client/model/detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/image_query.py` & `groundlight-0.7.5/generated/openapi_client/model/image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.7.5/generated/openapi_client/model/image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.7.5/generated/openapi_client/model/paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.7.5/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.7.5/generated/openapi_client/model/result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/model_utils.py` & `groundlight-0.7.5/generated/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/openapi_client/models/__init__.py` & `groundlight-0.7.5/generated/openapi_client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# flake8: noqa
+# ruff: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from openapi_client.model.pet import Pet
 # or import this package, but before doing it, use:
```

### Comparing `groundlight-0.7.4/generated/openapi_client/rest.py` & `groundlight-0.7.5/generated/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/setup.py` & `groundlight-0.7.5/generated/setup.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_classification_result.py` & `groundlight-0.7.5/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_detector.py` & `groundlight-0.7.5/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_detector_creation_input.py` & `groundlight-0.7.5/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_detector_type_enum.py` & `groundlight-0.7.5/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_detectors_api.py` & `groundlight-0.7.5/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_image_queries_api.py` & `groundlight-0.7.5/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_image_query.py` & `groundlight-0.7.5/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_image_query_type_enum.py` & `groundlight-0.7.5/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_paginated_detector_list.py` & `groundlight-0.7.5/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_paginated_image_query_list.py` & `groundlight-0.7.5/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/generated/test/test_result_type_enum.py` & `groundlight-0.7.5/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.7.4/src/groundlight/__init__.py` & `groundlight-0.7.5/src/groundlight/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# flake8: noqa
+# ruff: noqa
 # Add useful imports from the generated code here at the top level, as a convenience.
 from openapi_client import ApiException
 
 # Imports from our code
 from .client import Groundlight
 
 try:
```

### Comparing `groundlight-0.7.4/src/groundlight/binary_labels.py` & `groundlight-0.7.5/src/groundlight/binary_labels.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,36 +7,45 @@
 from typing import List, Union
 
 from model import Detector, ImageQuery
 
 logger = logging.getLogger("groundlight.sdk")
 
 
-def internal_labels_for_detector(context: Union[ImageQuery, Detector, str]) -> List[str]:
+def internal_labels_for_detector(
+    context: Union[ImageQuery, Detector, str],  # pylint: disable=unused-argument
+) -> List[str]:
     """Returns an ordered list of class labels as strings.
     These are the versions of labels that the API demands.
-    :param context: Can be an ImageQuery, a Detector, or a string-id for one of them."""
+    :param context: Can be an ImageQuery, a Detector, or a string-id for one of them.
+    """
     # NOTE: At some point this will need to be an API call, because these will be defined per-detector
     return ["PASS", "FAIL"]
 
 
-def convert_internal_label_to_display(context: Union[ImageQuery, Detector, str], label: str) -> str:
+def convert_internal_label_to_display(
+    context: Union[ImageQuery, Detector, str],  # pylint: disable=unused-argument
+    label: str,
+) -> str:
     # NOTE: Someday we will do nothing here, when the server provides properly named classes.
     upper = label.upper()
     if upper == "PASS":
         return "YES"
     if upper == "FAIL":
         return "NO"
     if upper in ["YES", "NO"]:
         return label
     logger.warning(f"Unrecognized internal label {label} - leaving alone.")
     return label
 
 
-def convert_display_label_to_internal(context: Union[ImageQuery, Detector, str], label: str) -> str:
+def convert_display_label_to_internal(
+    context: Union[ImageQuery, Detector, str],  # pylint: disable=unused-argument
+    label: str,
+) -> str:
     # NOTE: In the future we should validate against actually supported labels for the detector
     upper = label.upper()
-    if upper == "PASS" or upper == "YES":
+    if upper in {"PASS", "YES"}:
         return "PASS"
-    if upper == "FAIL" or upper == "NO":
+    if upper in {"FAIL", "NO"}:
         return "FAIL"
     raise ValueError(f'Invalid label string "{label}".  Must be one of YES,NO,PASS,FAIL')
```

### Comparing `groundlight-0.7.4/src/groundlight/client.py` & `groundlight-0.7.5/src/groundlight/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,139 @@
 import logging
 import os
 import time
 from io import BufferedReader, BytesIO
 from typing import Optional, Union
 
-from groundlight.optional_imports import Image
 from model import Detector, ImageQuery, PaginatedDetectorList, PaginatedImageQueryList
-from openapi_client import ApiClient, Configuration
+from openapi_client import Configuration
 from openapi_client.api.detectors_api import DetectorsApi
 from openapi_client.api.image_queries_api import ImageQueriesApi
 from openapi_client.model.detector_creation_input import DetectorCreationInput
 
-from groundlight.binary_labels import convert_display_label_to_internal, convert_internal_label_to_display
-from groundlight.config import API_TOKEN_VARIABLE_NAME, API_TOKEN_WEB_URL, DEFAULT_ENDPOINT
-from groundlight.images import buffer_from_jpeg_file, jpeg_from_numpy, parse_supported_image_types
+from groundlight.binary_labels import convert_display_label_to_internal
+from groundlight.config import API_TOKEN_VARIABLE_NAME, API_TOKEN_WEB_URL
+from groundlight.images import parse_supported_image_types
 from groundlight.internalapi import GroundlightApiClient, sanitize_endpoint_url
-from groundlight.optional_imports import np
+from groundlight.optional_imports import Image, np
 
 logger = logging.getLogger("groundlight.sdk")
 
 
 class ApiTokenError(Exception):
     pass
 
 
 class Groundlight:
-    """
-    Client for accessing the Groundlight cloud service.
+    """Client for accessing the Groundlight cloud service.
 
     The API token (auth) is specified through the GROUNDLIGHT_API_TOKEN environment variable by default.
 
     Example usage:
     ```
     gl = Groundlight()
     d = gl.get_or_create_detector("door", "Is the door locked?")
     iq = gl.submit_image_query(d, image)
     print(iq.result)
     ```
     """
 
-    DEFAULT_WAIT = 30
+    DEFAULT_WAIT: float = 30.0
 
     BEFORE_POLLING_DELAY = 3.0  # Expected minimum time for a label to post
     POLLING_INITIAL_DELAY = 0.5
     POLLING_EXPONENTIAL_BACKOFF = 1.3  # This still has the nice backoff property that the max number of requests
     # is O(log(time)), but with 1.3 the guarantee is that the call will return no more than 30% late
 
-    def __init__(self, endpoint: Optional[str] = None, api_token: str = None):
-        """
-        :param endpoint: optionally specify a different endpoint
+    def __init__(self, endpoint: Optional[str] = None, api_token: Optional[str] = None) -> None:
+        """:param endpoint: optionally specify a different endpoint
         :param api_token: use this API token for your API calls. If unset, fallback to the
             environment variable "GROUNDLIGHT_API_TOKEN".
         """
         # Specify the endpoint
         self.endpoint = sanitize_endpoint_url(endpoint)
         configuration = Configuration(host=self.endpoint)
 
         if api_token is None:
             try:
                 # Retrieve the API token from environment variable
                 api_token = os.environ[API_TOKEN_VARIABLE_NAME]
             except KeyError as e:
                 raise ApiTokenError(
-                    "No API token found. Please put your token in an environment variable "
-                    f'named "{API_TOKEN_VARIABLE_NAME}". If you don\'t have a token, you can '
-                    f"create one at {API_TOKEN_WEB_URL}"
+                    (
+                        "No API token found. Please put your token in an environment variable "
+                        f'named "{API_TOKEN_VARIABLE_NAME}". If you don\'t have a token, you can '
+                        f"create one at {API_TOKEN_WEB_URL}"
+                    ),
                 ) from e
 
         configuration.api_key["ApiToken"] = api_token
 
         self.api_client = GroundlightApiClient(configuration)
         self.detectors_api = DetectorsApi(self.api_client)
         self.image_queries_api = ImageQueriesApi(self.api_client)
 
-    def get_detector(self, id: Union[str, Detector]) -> Detector:
+    def get_detector(self, id: Union[str, Detector]) -> Detector:  # pylint: disable=redefined-builtin
         if isinstance(id, Detector):
             # Short-circuit
             return id
         obj = self.detectors_api.get_detector(id=id)
         return Detector.parse_obj(obj.to_dict())
 
-    def get_detector_by_name(self, name: str) -> Optional[Detector]:
-        # TODO: Do this on server.
-        detector_list = self.list_detectors(page_size=250)
-        for d in detector_list.results:
-            if d.name == name:
-                return d
-        if detector_list.next:
-            # TODO: paginate
-            raise RuntimeError("You have too many detectors to use get_detector_by_name")
-        return None
+    def get_detector_by_name(self, name: str) -> Detector:
+        return self.api_client._get_detector_by_name(name)  # pylint: disable=protected-access
 
     def list_detectors(self, page: int = 1, page_size: int = 10) -> PaginatedDetectorList:
         obj = self.detectors_api.list_detectors(page=page, page_size=page_size)
         return PaginatedDetectorList.parse_obj(obj.to_dict())
 
-    def create_detector(self, name: str, query: str, config_name: str = None) -> Detector:
-        obj = self.detectors_api.create_detector(DetectorCreationInput(name=name, query=query, config_name=config_name))
+    def create_detector(
+        self,
+        name: str,
+        query: str,
+        *,
+        confidence_threshold: Optional[float] = None,
+        config_name: Optional[str] = None,
+    ) -> Detector:
+        detector_creation_input = DetectorCreationInput(name=name, query=query)
+        if confidence_threshold is not None:
+            detector_creation_input.confidence_threshold = confidence_threshold
+        if config_name is not None:
+            detector_creation_input.config_name = config_name
+        obj = self.detectors_api.create_detector(detector_creation_input)
         return Detector.parse_obj(obj.to_dict())
 
-    def get_or_create_detector(self, name: str, query: str, config_name: str = None) -> Detector:
-        """Tries to look up the detector by name.  If a detector with that name and query exists, return it.
-        Otherwise, create a detector with the specified query and config.
+    def get_or_create_detector(
+        self, name: str, query: str, *, confidence_threshold: Optional[float] = None, config_name: Optional[str] = None
+    ) -> Detector:
+        """Tries to look up the detector by name.  If a detector with that name, query, and
+        confidence exists, return it. Otherwise, create a detector with the specified query and
+        config.
         """
         existing_detector = self.get_detector_by_name(name)
         if existing_detector:
-            if existing_detector.query == query:
-                return existing_detector
-            else:
+            # TODO: We may soon allow users to update the retrieved detector's fields.
+            if existing_detector.query != query:
+                raise ValueError(
+                    f"Found existing detector with name={name} (id={existing_detector.id}) but the queries don't match."
+                    f" The existing query is '{existing_detector.query}'."
+                )
+            if confidence_threshold is not None and existing_detector.confidence_threshold != confidence_threshold:
                 raise ValueError(
-                    f"Found existing detector with name={name} (id={existing_detector.id}) but the queries don't match"
+                    f"Found existing detector with name={name} (id={existing_detector.id}) but the confidence"
+                    " thresholds don't match. The existing confidence threshold is"
+                    f" {existing_detector.confidence_threshold}."
                 )
+            return existing_detector
 
-        return self.create_detector(name, query, config_name)
+        return self.create_detector(
+            name=name, query=query, confidence_threshold=confidence_threshold, config_name=config_name
+        )
 
-    def get_image_query(self, id: str) -> ImageQuery:
+    def get_image_query(self, id: str) -> ImageQuery:  # pylint: disable=redefined-builtin
         obj = self.image_queries_api.get_image_query(id=id)
         return ImageQuery.parse_obj(obj.to_dict())
 
     def list_image_queries(self, page: int = 1, page_size: int = 10) -> PaginatedImageQueryList:
         obj = self.image_queries_api.list_image_queries(page=page, page_size=page_size)
         return PaginatedImageQueryList.parse_obj(obj.to_dict())
 
@@ -134,69 +149,73 @@
           - filename (string) of a jpeg file
           - byte array or BytesIO or BufferedReader with jpeg bytes
           - numpy array with values 0-255 and dimensions (H,W,3) in RGB order
             (Note OpenCV uses BGR not RGB. `img[:, :, ::-1]` will reverse the channels)
           - PIL Image
           Any binary format must be JPEG-encoded already.  Any pixel format will get
           converted to JPEG at high quality before sending to service.
-        :param wait: How long to wait (in seconds) for a confident answer
+        :param wait: How long to wait (in seconds) for a confident answer.
         """
         if wait is None:
             wait = self.DEFAULT_WAIT
-        if isinstance(detector, Detector):
-            detector_id = detector.id
-        else:
-            detector_id = detector
+        detector_id = detector.id if isinstance(detector, Detector) else detector
         image_bytesio: Union[BytesIO, BufferedReader] = parse_supported_image_types(image)
 
         raw_image_query = self.image_queries_api.submit_image_query(detector_id=detector_id, body=image_bytesio)
         image_query = ImageQuery.parse_obj(raw_image_query.to_dict())
         if wait:
             threshold = self.get_detector(detector).confidence_threshold
             image_query = self.wait_for_confident_result(image_query, confidence_threshold=threshold, timeout_sec=wait)
         return image_query
 
     def wait_for_confident_result(
-        self, image_query: ImageQuery, confidence_threshold: float, timeout_sec: float = 30.0
+        self,
+        image_query: ImageQuery,
+        confidence_threshold: float,
+        timeout_sec: float = 30.0,
     ) -> ImageQuery:
         """Waits for an image query result's confidence level to reach the specified value.
         Currently this is done by polling with an exponential back-off.
         :param image_query: An ImageQuery object to poll
         :param confidence_threshold: The minimum confidence level required to return before the timeout.
-        :param timeout_sec: The maximum number of seconds to wait."""
+        :param timeout_sec: The maximum number of seconds to wait.
+        """
         # TODO: Add support for ImageQuery id instead of object.
         timeout_time = time.time() + timeout_sec
         time.sleep(self.BEFORE_POLLING_DELAY)
         delay = self.POLLING_INITIAL_DELAY
         while time.time() < timeout_time:
             current_confidence = image_query.result.confidence
             if current_confidence is None:
-                logging.debug(f"Image query with None confidence implies human label (for now)")
+                logging.debug("Image query with None confidence implies human label (for now)")
                 break
             if current_confidence >= confidence_threshold:
                 logging.debug(f"Image query confidence {current_confidence:.3f} above {confidence_threshold:.3f}")
                 break
             logger.debug(
-                f"Polling for updated image_query because confidence {current_confidence:.3f} < {confidence_threshold:.3f}"
+                (
+                    f"Polling for updated image_query because confidence {current_confidence:.3f} <"
+                    f" {confidence_threshold:.3f}"
+                ),
             )
             time_left = max(0, time.time() - timeout_time)
             time.sleep(min(delay, time_left))
             delay *= self.POLLING_EXPONENTIAL_BACKOFF
             image_query = self.get_image_query(image_query.id)
         return image_query
 
     def add_label(self, image_query: Union[ImageQuery, str], label: str):
-        """a new label to an image query.  This answers the detector's question.
+        """A new label to an image query.  This answers the detector's question.
         :param image_query: Either an ImageQuery object (returned from `submit_image_query`) or
         an image_query id as a string.
         :param label: The string "Yes" or the string "No" in answer to the query.
         """
         if isinstance(image_query, ImageQuery):
             image_query_id = image_query.id
         else:
             image_query_id = str(image_query)
             # Some old imagequery id's started with "chk_"
-            if not (image_query_id.startswith("chk_") or image_query_id.startswith("iq_")):
+            if not image_query_id.startswith(("chk_", "iq_")):
                 raise ValueError(f"Invalid image query id {image_query_id}")
         api_label = convert_display_label_to_internal(image_query_id, label)
 
-        return self.api_client._add_label(image_query_id, api_label)
+        return self.api_client._add_label(image_query_id, api_label)  # pylint: disable=protected-access
```

### Comparing `groundlight-0.7.4/src/groundlight/images.py` & `groundlight-0.7.5/src/groundlight/images.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,56 +2,57 @@
 from io import BufferedReader, BytesIO
 from typing import Union
 
 from groundlight.optional_imports import Image, np
 
 
 def buffer_from_jpeg_file(image_filename: str) -> BufferedReader:
-    """
-    Get a buffer from an jpeg image file.
+    """Get a buffer from an jpeg image file.
 
     For now, we only support JPEG files, and raise an ValueError otherwise.
     """
     if imghdr.what(image_filename) == "jpeg":
         # Note this will get fooled by truncated binaries since it only reads the header.
         # That's okay - the server will catch it.
         return open(image_filename, "rb")
-    else:
-        raise ValueError("We only support JPEG files, for now.")
+    raise ValueError("We only support JPEG files, for now.")
 
 
 def jpeg_from_numpy(img: np.ndarray, jpeg_quality: int = 95) -> bytes:
-    """Converts a numpy array to BytesIO"""
+    """Converts a numpy array to BytesIO."""
     pilim = Image.fromarray(img.astype("uint8"), "RGB")
     with BytesIO() as buf:
-        buf = BytesIO()
         pilim.save(buf, "jpeg", quality=jpeg_quality)
         out = buf.getvalue()
         return out
 
 
 def parse_supported_image_types(
-    image: Union[str, bytes, Image.Image, BytesIO, BufferedReader, np.ndarray], jpeg_quality: int = 95
+    image: Union[str, bytes, Image.Image, BytesIO, BufferedReader, np.ndarray],
+    jpeg_quality: int = 95,
 ) -> Union[BytesIO, BufferedReader]:
     """Parse the many supported image types into a bytes-stream objects.
-    In some cases we have to JPEG compress."""
+    In some cases we have to JPEG compress.
+    """
     if isinstance(image, str):
         # Assume it is a filename
         return buffer_from_jpeg_file(image)
-    elif isinstance(image, bytes):
+    if isinstance(image, bytes):
         # Create a BytesIO object
         return BytesIO(image)
-    elif isinstance(image, Image.Image):
+    if isinstance(image, Image.Image):
         # Save PIL image as jpeg in BytesIO
         bytesio = BytesIO()
         image.save(bytesio, "jpeg", quality=jpeg_quality)
         bytesio.seek(0)
         return bytesio
-    elif isinstance(image, BytesIO) or isinstance(image, BufferedReader):
+    if isinstance(image, (BytesIO, BufferedReader)):
         # Already in the right format
         return image
-    elif isinstance(image, np.ndarray):
+    if isinstance(image, np.ndarray):
         return BytesIO(jpeg_from_numpy(image, jpeg_quality=jpeg_quality))
-    else:
-        raise TypeError(
-            "Unsupported type for image. Must be PIL, numpy (H,W,3) RGB, or a JPEG as a filename (str), bytes, BytesIO, or BufferedReader."
-        )
+    raise TypeError(
+        (
+            "Unsupported type for image. Must be PIL, numpy (H,W,3) RGB, or a JPEG as a filename (str), bytes,"
+            " BytesIO, or BufferedReader."
+        ),
+    )
```

### Comparing `groundlight-0.7.4/src/groundlight/internalapi.py` & `groundlight-0.7.5/src/groundlight/internalapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import logging
 import os
 import time
-from typing import Dict
-from urllib.parse import urlsplit, urlunsplit
 import uuid
+from typing import Optional
+from urllib.parse import urlsplit, urlunsplit
 
-from groundlight.config import DEFAULT_ENDPOINT
-
-import model
 import requests
+from model import Detector
 from openapi_client.api_client import ApiClient
 
+from groundlight.status_codes import is_ok
+
 logger = logging.getLogger("groundlight.sdk")
 
 
-def sanitize_endpoint_url(endpoint: str) -> str:
+class NotFoundError(Exception):
+    pass
+
+
+def sanitize_endpoint_url(endpoint: Optional[str] = None) -> str:
     """Takes a URL for an endpoint, and returns a "sanitized" version of it.
     Currently the production API path must be exactly "/device-api".
     This allows people to leave that off entirely, or add a trailing slash.
     Also some future-proofing by allowing "v1" or "v2" or "v3" paths.
     """
     if not endpoint:
         endpoint = os.environ.get("GROUNDLIGHT_ENDPOINT", "")
         if not endpoint:
             # Because sometimes people set an environment variable to a blank string by mistake
             endpoint = "https://api.groundlight.ai/"
     parts = urlsplit(endpoint)
     if (parts.scheme not in ("http", "https")) or (not parts.netloc):
         raise ValueError(
-            f"Invalid API endpoint {endpoint}.  Unsupported scheme: {parts.scheme}.  Must be http or https, e.g. https://api.groundlight.ai/"
+            (
+                f"Invalid API endpoint {endpoint}.  Unsupported scheme: {parts.scheme}.  Must be http or https, e.g."
+                " https://api.groundlight.ai/"
+            ),
         )
     if parts.query or parts.fragment:
         raise ValueError(f"Invalid API endpoint {endpoint}.  Cannot have query or fragment.")
     if not parts.path:
         parts = parts._replace(path="/")
     if not parts.path.endswith("/"):
         parts = parts._replace(path=parts.path + "/")
@@ -47,15 +54,15 @@
 
 def _generate_request_id():
     # TODO: use a ksuid instead of a uuid.  Most of our API uses ksuids for lots of reasons.
     # But we don't want to just import ksuid because we want to avoid dependency bloat
     return "req_uu" + uuid.uuid4().hex
 
 
-class InternalApiException(RuntimeError):
+class InternalApiError(RuntimeError):
     # TODO: We need a better exception hierarchy
     pass
 
 
 class GroundlightApiClient(ApiClient):
     """Subclassing the OpenAPI-generated ApiClient to add a bit of custom functionality.
     Not crazy about using polymorphism, but this is simpler than modifying the moustache
@@ -66,20 +73,19 @@
 
     def call_api(self, *args, **kwargs):
         """Adds a request-id header to each API call."""
         # Note we don't look for header_param in kwargs here, because this method is only called in one place
         # in the generated code, so we can afford to make this brittle.
         header_param = args[4]  # that's the number in the list
         if not header_param:
-            # This will never happen in normal useage.
+            # This will never happen in normal usage.
             logger.warning("Can't set request-id because headers not set")
-        else:
-            if not header_param.get(self.REQUEST_ID_HEADER, None):
-                header_param[self.REQUEST_ID_HEADER] = _generate_request_id()
-                # Note that we have updated the actual dict in args, so we don't have to put it back in
+        elif not header_param.get(self.REQUEST_ID_HEADER, None):
+            header_param[self.REQUEST_ID_HEADER] = _generate_request_id()
+            # Note that we have updated the actual dict in args, so we don't have to put it back in
         return super().call_api(*args, **kwargs)
 
     #
     # The methods below will eventually go away when we move to properly model
     # these methods with OpenAPI
     #
 
@@ -105,13 +111,37 @@
         headers = self._headers()
 
         logger.info(f"Posting label={label} to image_query {image_query_id} ...")
         response = requests.request("POST", url, json=data, headers=headers)
         elapsed = 1000 * (time.time() - start_time)
         logger.debug(f"Call to ImageQuery.add_label took {elapsed:.1f}ms response={response.text}")
 
-        if response.status_code != 200:
-            raise InternalApiException(
-                f"Error adding label to image query {image_query_id} status={response.status_code} {response.text}"
+        if not is_ok(response.status_code):
+            raise InternalApiError(
+                f"Error adding label to image query {image_query_id} status={response.status_code} {response.text}",
             )
 
         return response.json()
+
+    def _get_detector_by_name(self, name: str) -> Detector:
+        """Get a detector by name. For now, we use the list detectors API directly.
+
+        TODO: Properly model this in the API, and generate SDK code for it.
+        """
+        url = f"{self.configuration.host}/v1/detectors?name={name}"
+        headers = self._headers()
+        response = requests.request("GET", url, headers=headers)
+
+        if not is_ok(response.status_code):
+            raise InternalApiError(
+                f"Error getting detector by name '{name}' (status={response.status_code}): {response.text}"
+            )
+
+        parsed = response.json()
+
+        if parsed["count"] == 0:
+            raise NotFoundError(f"Detector with name={name} not found.")
+        if parsed["count"] > 1:
+            raise RuntimeError(
+                f"We found multiple ({parsed['count']}) detectors with the same name. This shouldn't happen."
+            )
+        return Detector.parse_obj(parsed["results"][0])
```

### Comparing `groundlight-0.7.4/src/groundlight/optional_imports.py` & `groundlight-0.7.5/src/groundlight/optional_imports.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# ruff: noqa: N804
 """We use a trick to check if libraries like numpy are installed or not.
 If they are, we make it available as normal.
 If not, we set it up as a shim object which still lets type-hinting work properly,
 but will fail at runtime if you try to use it.
 
-This can be confusing, but hopefully the errors are explicit enough to be 
+This can be confusing, but hopefully the errors are explicit enough to be
 clear about what's happening, and it makes the code which hopes numpy is installed
 look readable.
 """
 
 
 class UnavailableModule(type):
     """Represents a module that is not installed or otherwise unavailable at runtime.
@@ -18,35 +19,35 @@
     """
 
     def __new__(cls, exc):
         out = type("UnavailableModule", (), {})
         out.exc = exc
         return out
 
-    def __getattr__(self, key):
+    def __getattr__(self, key):  # pylint: disable=bad-mcs-method-argument
         # TODO: This isn't getting called for some reason.
-        raise RuntimeError("attempt to use module that failed to load") from self.exc
+        raise RuntimeError("attempt to use module that failed to load") from self.exc  # type: ignore
 
 
 try:
-    import numpy as np
+    import numpy as np  # pyright: reportMissingImports=false
 
     MISSING_NUMPY = False
 except ImportError as e:
     np = UnavailableModule(e)
     # Expose np.ndarray so type-hinting looks normal
-    np.ndarray = np
+    np.ndarray = np  # pylint: disable=attribute-defined-outside-init
     MISSING_NUMPY = True
 
 try:
     import PIL
     from PIL import Image
 
     MISSING_PIL = False
 except ImportError as e:
     PIL = UnavailableModule(e)
     Image = PIL
-    Image.Image = PIL  # for type-hinting
+    Image.Image = PIL  # for type-hinting; pylint: disable=attribute-defined-outside-init
     MISSING_PIL = True
 
 
 __all__ = ["np", "PIL", "Image", "MISSING_NUMPY", "MISSING_PIL"]
```

### Comparing `groundlight-0.7.4/PKG-INFO` & `groundlight-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groundlight
-Version: 0.7.4
+Version: 0.7.5
 Summary: Build computer vision systems from natural language with Groundlight
 Home-page: https://www.groundlight.ai
 License: MIT
 Author: Groundlight AI
 Author-email: support@groundlight.ai
 Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Groundlight Python SDK
 
-Groundlight makes it simple to build reliable visual applications.  Read the [full documentation here](https://code.groundlight.ai/python-sdk/).
+Groundlight makes it simple to build reliable visual applications. Read the [full documentation here](https://code.groundlight.ai/python-sdk/).
 
 ## Computer Vision powered by Natural Language
 
 ```bash
 pip install groundlight
 ```
 
@@ -50,13 +50,12 @@
 
 _Note: The SDK is currently in "beta" phase. Interfaces are subject to change in future versions._
 
 ## Learn more
 
 Some more resources you might like:
 
-* [Code Documentation](https://code.groundlight.ai/)
-* [Python SDK](https://pypi.org/project/groundlight/)
-* [Company](https://www.groundlight.ai/)
-* [Login to Groundlight](https://app.groundlight.ai/)
-
+- [Code Documentation](https://code.groundlight.ai/)
+- [Python SDK](https://pypi.org/project/groundlight/)
+- [Company](https://www.groundlight.ai/)
+- [Login to Groundlight](https://app.groundlight.ai/)
```

