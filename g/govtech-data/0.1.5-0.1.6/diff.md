# Comparing `tmp/govtech_data-0.1.5.tar.gz` & `tmp/govtech_data-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.5.tar", max compression
+gzip compressed data, was "govtech_data-0.1.6.tar", max compression
```

## Comparing `govtech_data-0.1.5.tar` & `govtech_data-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.5/README.md
--rw-r--r--   0        0        0      869 2023-04-15 06:50:22.215007 govtech_data-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.5/src/govtech_data/__init__.py
--rw-r--r--   0        0        0     4793 2023-04-15 06:46:28.641774 govtech_data-0.1.5/src/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.5/src/govtech_data/models/__init__.py
--rw-r--r--   0        0        0     1046 2023-04-15 06:49:21.541855 govtech_data-0.1.5/src/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.5/src/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.5/src/govtech_data/models/resources/datastore_search.py
--rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.5/src/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.5/src/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.5/src/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.5/src/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0      497 2023-04-15 06:49:21.543747 govtech_data-0.1.5/src/govtech_data/utils/content.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 govtech_data-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.6/README.md
+-rw-r--r--   0        0        0      869 2023-04-15 06:56:03.648118 govtech_data-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.6/src/govtech_data/__init__.py
+-rw-r--r--   0        0        0     4773 2023-04-15 06:55:43.227701 govtech_data-0.1.6/src/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.6/src/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0     1046 2023-04-15 06:49:21.541855 govtech_data-0.1.6/src/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.6/src/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.6/src/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.6/src/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.6/src/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.6/src/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.6/src/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0      497 2023-04-15 06:49:21.543747 govtech_data-0.1.6/src/govtech_data/utils/content.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 govtech_data-0.1.6/PKG-INFO
```

### Comparing `govtech_data-0.1.5/pyproject.toml` & `govtech_data-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "govtech-data"
-version = "0.1.5"
+version = "0.1.6"
 description = "Library to easily access and read data from data.gov.sg"
 authors = ["Khee-Chin Chua <kheechin@gmail.com>"]
 license = "Singapore Open Data License"
 readme = "README.md"
 packages = [{include = "govtech_data", from = "src"}]
 repository = "https://github.com/merlin83/govtech-data"
```

### Comparing `govtech_data-0.1.5/src/govtech_data/client.py` & `govtech_data-0.1.6/src/govtech_data/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 import requests
 
 from fuzzywuzzy import process
 from loguru import logger
 from pydantic import BaseModel, validate_arguments
 
 from govtech_data.utils.content import fetch_url, convert_response_to_io
-from src.govtech_data.models.api import (
+from govtech_data.models.api import (
     DatastoreSearch,
     PackageShow,
     ResourceShow,
     SearchPackage,
     PackageResourceContent,
     PackageContent,
 )
-from src.govtech_data.models.resources.datastore_search import DatastoreSearchModel
-from src.govtech_data.models.resources.package_list import PackageListModel
-from src.govtech_data.models.resources.package_show import (
+from govtech_data.models.resources.datastore_search import DatastoreSearchModel
+from govtech_data.models.resources.package_list import PackageListModel
+from govtech_data.models.resources.package_show import (
     PackageShowModel,
     Result as PackageShowModelResult,
 )
-from src.govtech_data.models.resources.resource_show import ResourceShowModel
+from govtech_data.models.resources.resource_show import ResourceShowModel
 
 API_ENDPOINTS = {
     "ckan_datastore_search": "https://data.gov.sg/api/action/datastore_search",
     "ckan_package_show": "https://data.gov.sg/api/action/package_show",
     "ckan_package_list": "https://data.gov.sg/api/action/package_list",
     "ckan_resource_show": "https://data.gov.sg/api/action/resource_show",
 }
```

### Comparing `govtech_data-0.1.5/src/govtech_data/models/api.py` & `govtech_data-0.1.6/src/govtech_data/models/api.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.5/src/govtech_data/models/resources/datastore_search.py` & `govtech_data-0.1.6/src/govtech_data/models/resources/datastore_search.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.5/src/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.6/src/govtech_data/models/resources/package_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.5/src/govtech_data/models/resources/resource_show.py` & `govtech_data-0.1.6/src/govtech_data/models/resources/resource_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.5/PKG-INFO` & `govtech_data-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govtech-data
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library to easily access and read data from data.gov.sg
 Home-page: https://github.com/merlin83/govtech-data
 License: Singapore Open Data License
 Author: Khee-Chin Chua
 Author-email: kheechin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

