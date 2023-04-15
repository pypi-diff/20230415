# Comparing `tmp/govtech_data-0.1.3.tar.gz` & `tmp/govtech_data-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.3.tar", max compression
+gzip compressed data, was "govtech_data-0.1.4.tar", max compression
```

## Comparing `govtech_data-0.1.3.tar` & `govtech_data-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.3/README.md
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.3/govtech_data/__init__.py
--rw-r--r--   0        0        0     3143 2023-04-14 10:06:22.322708 govtech_data-0.1.3/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.3/govtech_data/models/__init__.py
--rw-r--r--   0        0        0      349 2023-04-14 09:18:13.465611 govtech_data-0.1.3/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.3/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0     1541 2023-04-14 09:27:05.352977 govtech_data-0.1.3/govtech_data/models/resources/datastore_search.py
--rw-r--r--   0        0        0      407 2023-04-14 09:27:05.287711 govtech_data-0.1.3/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     4441 2023-04-14 09:27:05.332541 govtech_data-0.1.3/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0     1994 2023-04-14 09:27:05.372624 govtech_data-0.1.3/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.3/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0     1109 2023-04-14 09:37:13.383824 govtech_data-0.1.3/govtech_data/utils/models.py
--rw-r--r--   0        0        0      867 2023-04-14 17:47:39.163246 govtech_data-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 govtech_data-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.4/README.md
+-rw-r--r--   0        0        0      868 2023-04-15 05:49:39.853165 govtech_data-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.4/src/govtech_data/__init__.py
+-rw-r--r--   0        0        0     3387 2023-04-15 05:48:04.671607 govtech_data-0.1.4/src/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.4/src/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0      418 2023-04-15 04:17:29.700059 govtech_data-0.1.4/src/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.4/src/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.4/src/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.4/src/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.4/src/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.4/src/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.4/src/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 govtech_data-0.1.4/PKG-INFO
```

### Comparing `govtech_data-0.1.3/govtech_data/client.py` & `govtech_data-0.1.4/src/govtech_data/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 
 import requests
 
 from fuzzywuzzy import process
 from loguru import logger
 from pydantic import BaseModel
 
-from govtech_data.models.api import DatastoreSearch, PackageShow, ResourceShow
-from govtech_data.models.resources.datastore_search import DatastoreSearchModel
-from govtech_data.models.resources.package_list import PackageListModel
-from govtech_data.models.resources.package_show import PackageShowModel
-from govtech_data.models.resources.resource_show import ResourceShowModel
+from src.govtech_data.models.api import (
+    DatastoreSearch,
+    PackageShow,
+    ResourceShow,
+    SearchPackage,
+)
+from src.govtech_data.models.resources.datastore_search import DatastoreSearchModel
+from src.govtech_data.models.resources.package_list import PackageListModel
+from src.govtech_data.models.resources.package_show import PackageShowModel
+from src.govtech_data.models.resources.resource_show import ResourceShowModel
 
-ENDPOINTS = {
+API_ENDPOINTS = {
     "ckan_datastore_search": "https://data.gov.sg/api/action/datastore_search",
     "ckan_package_show": "https://data.gov.sg/api/action/package_show",
     "ckan_package_list": "https://data.gov.sg/api/action/package_list",
     "ckan_resource_show": "https://data.gov.sg/api/action/resource_show",
 }
 
 COMMON_HEADERS = {"accept": "application/json"}
@@ -38,55 +43,60 @@
 
     @classmethod
     def datastore_search(
         cls, resource_id: str, **kwargs
     ) -> Union[BaseModel, DatastoreSearchModel]:
         kwargs["resource_id"] = resource_id
         return cls.get_model_from_json_response(
-            ENDPOINTS.get("ckan_datastore_search"),
+            API_ENDPOINTS.get("ckan_datastore_search"),
             DatastoreSearch(**kwargs).dict(),
             DatastoreSearchModel,
         )
 
     @classmethod
     def resource_show(cls, resource_id: str) -> Union[BaseModel, ResourceShowModel]:
         return cls.get_model_from_json_response(
-            ENDPOINTS.get("ckan_resource_show"),
+            API_ENDPOINTS.get("ckan_resource_show"),
             ResourceShow(**{"id": resource_id}).dict(),
             ResourceShowModel,
         )
 
     @classmethod
     def package_show(cls, package_id: str) -> Union[BaseModel, PackageShowModel]:
         return cls.get_model_from_json_response(
-            ENDPOINTS.get("ckan_package_show"),
+            API_ENDPOINTS.get("ckan_package_show"),
             PackageShow(**{"id": package_id}).dict(),
             PackageShowModel,
         )
 
     @classmethod
     @lru_cache(maxsize=1)
     def package_list(cls) -> Union[BaseModel, PackageListModel]:
         return cls.get_model_from_json_response(
-            ENDPOINTS.get("ckan_package_list"), {}, PackageListModel
+            API_ENDPOINTS.get("ckan_package_list"), {}, PackageListModel
         )
 
     @classmethod
-    def search_package(cls, name: str, limit: int = 5):
-        return process.extract(name, cls.package_list().result, limit=limit)
+    def search_package(cls, name: str, limit: int = 10) -> list[SearchPackage]:
+        return [
+            SearchPackage(package_id=package_id, score=score)
+            for (package_id, score) in process.extract(
+                name, cls.package_list().result, limit=limit
+            )
+        ]
 
     @classmethod
     def get_model_from_json_response(
         cls, url: str, params: dict, model: Type[BaseModel]
     ):
         if url is None:
             raise Exception("url cannot be None!")
         if model is None:
             raise Exception("model cannot be None!")
-        logger.info(f"endpoint name: {url}")
+        logger.debug(f"endpoint name: {url}")
         resp = requests.get(
             url,
             params=params,
             headers=COMMON_HEADERS,
             timeout=DEFAULT_TIMEOUT_IN_SECONDS,
         )
         if not resp.ok:
```

### Comparing `govtech_data-0.1.3/govtech_data/models/resources/datastore_search.py` & `govtech_data-0.1.4/src/govtech_data/models/resources/datastore_search.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.3/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.4/src/govtech_data/models/resources/package_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.3/govtech_data/models/resources/resource_show.py` & `govtech_data-0.1.4/src/govtech_data/models/resources/resource_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.3/pyproject.toml` & `govtech_data-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "govtech-data"
-version = "0.1.3"
+version = "0.1.4"
 description = "Library to easily access and read data from data.gov.sg"
 authors = ["Khee-Chin Chua <kheechin@gmail.com>"]
 license = "Singapore Open Data License"
 readme = "README.md"
-packages = [{include = "govtech_data"}]
+packages = [{include = "govtech_data", from = "src"}]
 repository = "https://github.com/merlin83/govtech-data"
 
 [tool.poetry.dependencies]
 fuzzywuzzy = "^0.18.0"
 loguru = "^0.7.0"
 pandas = "^2.0.0"
 pydantic = "^1.10.7"
@@ -19,15 +19,15 @@
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 datamodel-code-generator = "^0.17.2"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
-generate-models = "govtech_data.utils.models:generate_models"
+generate-models = "tools.models:generate_models"
 
 [tool.isort]
 profile = 'black'
 lines_between_types = 1
 combine_as_imports = true
 
 [build-system]
```

### Comparing `govtech_data-0.1.3/PKG-INFO` & `govtech_data-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govtech-data
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to easily access and read data from data.gov.sg
 Home-page: https://github.com/merlin83/govtech-data
 License: Singapore Open Data License
 Author: Khee-Chin Chua
 Author-email: kheechin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

