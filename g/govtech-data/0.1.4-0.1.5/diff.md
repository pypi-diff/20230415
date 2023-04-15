# Comparing `tmp/govtech_data-0.1.4.tar.gz` & `tmp/govtech_data-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.4.tar", max compression
+gzip compressed data, was "govtech_data-0.1.5.tar", max compression
```

## Comparing `govtech_data-0.1.4.tar` & `govtech_data-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.4/README.md
--rw-r--r--   0        0        0      868 2023-04-15 05:49:39.853165 govtech_data-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.4/src/govtech_data/__init__.py
--rw-r--r--   0        0        0     3387 2023-04-15 05:48:04.671607 govtech_data-0.1.4/src/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.4/src/govtech_data/models/__init__.py
--rw-r--r--   0        0        0      418 2023-04-15 04:17:29.700059 govtech_data-0.1.4/src/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.4/src/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.4/src/govtech_data/models/resources/datastore_search.py
--rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.4/src/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.4/src/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.4/src/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.4/src/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 govtech_data-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.5/README.md
+-rw-r--r--   0        0        0      869 2023-04-15 06:50:22.215007 govtech_data-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.5/src/govtech_data/__init__.py
+-rw-r--r--   0        0        0     4793 2023-04-15 06:46:28.641774 govtech_data-0.1.5/src/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.5/src/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0     1046 2023-04-15 06:49:21.541855 govtech_data-0.1.5/src/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.5/src/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.5/src/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.5/src/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.5/src/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.5/src/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.5/src/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0      497 2023-04-15 06:49:21.543747 govtech_data-0.1.5/src/govtech_data/utils/content.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 govtech_data-0.1.5/PKG-INFO
```

### Comparing `govtech_data-0.1.4/pyproject.toml` & `govtech_data-0.1.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "govtech-data"
-version = "0.1.4"
+version = "0.1.5"
 description = "Library to easily access and read data from data.gov.sg"
 authors = ["Khee-Chin Chua <kheechin@gmail.com>"]
 license = "Singapore Open Data License"
 readme = "README.md"
 packages = [{include = "govtech_data", from = "src"}]
 repository = "https://github.com/merlin83/govtech-data"
 
 [tool.poetry.dependencies]
 fuzzywuzzy = "^0.18.0"
 loguru = "^0.7.0"
-pandas = "^2.0.0"
 pydantic = "^1.10.7"
 python = "^3.10"
 python-levenshtein = "^0.20.9"
 requests = "^2.28.2"
+polars = "^0.17.2"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 datamodel-code-generator = "^0.17.2"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
```

### Comparing `govtech_data-0.1.4/src/govtech_data/client.py` & `govtech_data-0.1.5/src/govtech_data/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from functools import lru_cache
 from typing import Type, Union
 
 import requests
 
 from fuzzywuzzy import process
 from loguru import logger
-from pydantic import BaseModel
+from pydantic import BaseModel, validate_arguments
 
+from govtech_data.utils.content import fetch_url, convert_response_to_io
 from src.govtech_data.models.api import (
     DatastoreSearch,
     PackageShow,
     ResourceShow,
     SearchPackage,
+    PackageResourceContent,
+    PackageContent,
 )
 from src.govtech_data.models.resources.datastore_search import DatastoreSearchModel
 from src.govtech_data.models.resources.package_list import PackageListModel
-from src.govtech_data.models.resources.package_show import PackageShowModel
+from src.govtech_data.models.resources.package_show import (
+    PackageShowModel,
+    Result as PackageShowModelResult,
+)
 from src.govtech_data.models.resources.resource_show import ResourceShowModel
 
 API_ENDPOINTS = {
     "ckan_datastore_search": "https://data.gov.sg/api/action/datastore_search",
     "ckan_package_show": "https://data.gov.sg/api/action/package_show",
     "ckan_package_list": "https://data.gov.sg/api/action/package_list",
     "ckan_resource_show": "https://data.gov.sg/api/action/resource_show",
@@ -38,57 +44,63 @@
             cls._instance = super(GovTechClient, cls).__new__(cls, *args, **kwargs)
         return cls._instance
 
     def __init__(self):
         pass
 
     @classmethod
+    @validate_arguments
     def datastore_search(
         cls, resource_id: str, **kwargs
     ) -> Union[BaseModel, DatastoreSearchModel]:
         kwargs["resource_id"] = resource_id
         return cls.get_model_from_json_response(
             API_ENDPOINTS.get("ckan_datastore_search"),
             DatastoreSearch(**kwargs).dict(),
             DatastoreSearchModel,
         )
 
     @classmethod
+    @validate_arguments
     def resource_show(cls, resource_id: str) -> Union[BaseModel, ResourceShowModel]:
         return cls.get_model_from_json_response(
             API_ENDPOINTS.get("ckan_resource_show"),
             ResourceShow(**{"id": resource_id}).dict(),
             ResourceShowModel,
         )
 
     @classmethod
+    @validate_arguments
     def package_show(cls, package_id: str) -> Union[BaseModel, PackageShowModel]:
         return cls.get_model_from_json_response(
             API_ENDPOINTS.get("ckan_package_show"),
             PackageShow(**{"id": package_id}).dict(),
             PackageShowModel,
         )
 
     @classmethod
     @lru_cache(maxsize=1)
+    @validate_arguments
     def package_list(cls) -> Union[BaseModel, PackageListModel]:
         return cls.get_model_from_json_response(
             API_ENDPOINTS.get("ckan_package_list"), {}, PackageListModel
         )
 
     @classmethod
+    @validate_arguments
     def search_package(cls, name: str, limit: int = 10) -> list[SearchPackage]:
         return [
             SearchPackage(package_id=package_id, score=score)
             for (package_id, score) in process.extract(
                 name, cls.package_list().result, limit=limit
             )
         ]
 
     @classmethod
+    @validate_arguments
     def get_model_from_json_response(
         cls, url: str, params: dict, model: Type[BaseModel]
     ):
         if url is None:
             raise Exception("url cannot be None!")
         if model is None:
             raise Exception("model cannot be None!")
@@ -98,7 +110,39 @@
             params=params,
             headers=COMMON_HEADERS,
             timeout=DEFAULT_TIMEOUT_IN_SECONDS,
         )
         if not resp.ok:
             resp.raise_for_status()
         return model(**resp.json())
+
+    @classmethod
+    @validate_arguments
+    def fetch_resources_from_package_result(
+        cls, package_result: PackageShowModelResult, limit: int = 0
+    ) -> list[PackageResourceContent]:
+        r = []
+        for resource in package_result.resources:
+            if limit != 0 and len(r) >= limit:
+                break
+            resp = fetch_url(resource.url)
+            r.append(
+                PackageResourceContent(
+                    resource=resource, content=convert_response_to_io(resp)
+                )
+            )
+        return r
+
+    @classmethod
+    @validate_arguments
+    def fetch_content_from_package(cls, package_name: str, limit: int = 0):
+        package_show_model: Union[PackageShowModel, None] = cls.package_show(
+            package_name
+        )
+        if package_show_model.result is None:
+            return None
+        return PackageContent(
+            package=package_show_model.result,
+            resources=cls.fetch_resources_from_package_result(
+                package_show_model.result, limit
+            ),
+        )
```

### Comparing `govtech_data-0.1.4/src/govtech_data/models/resources/datastore_search.py` & `govtech_data-0.1.5/src/govtech_data/models/resources/datastore_search.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.4/src/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.5/src/govtech_data/models/resources/package_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.4/src/govtech_data/models/resources/resource_show.py` & `govtech_data-0.1.5/src/govtech_data/models/resources/resource_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.4/PKG-INFO` & `govtech_data-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: govtech-data
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to easily access and read data from data.gov.sg
 Home-page: https://github.com/merlin83/govtech-data
 License: Singapore Open Data License
 Author: Khee-Chin Chua
 Author-email: kheechin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: polars (>=0.17.2,<0.18.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-levenshtein (>=0.20.9,<0.21.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/merlin83/govtech-data
 Description-Content-Type: text/markdown
```

