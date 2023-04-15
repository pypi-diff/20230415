# Comparing `tmp/govtech_data-0.1.7.tar.gz` & `tmp/govtech_data-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.7.tar", max compression
+gzip compressed data, was "govtech_data-0.1.8.tar", max compression
```

## Comparing `govtech_data-0.1.7.tar` & `govtech_data-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.7/README.md
--rw-r--r--   0        0        0      869 2023-04-15 07:18:10.169351 govtech_data-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.7/src/govtech_data/__init__.py
--rw-r--r--   0        0        0     4857 2023-04-15 07:17:18.813435 govtech_data-0.1.7/src/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.7/src/govtech_data/models/__init__.py
--rw-r--r--   0        0        0     1046 2023-04-15 06:49:21.541855 govtech_data-0.1.7/src/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.7/src/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.7/src/govtech_data/models/resources/datastore_search.py
--rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.7/src/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.7/src/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.7/src/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.7/src/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0      497 2023-04-15 06:49:21.543747 govtech_data-0.1.7/src/govtech_data/utils/content.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 govtech_data-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.8/README.md
+-rw-r--r--   0        0        0      869 2023-04-15 07:24:52.383933 govtech_data-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.8/src/govtech_data/__init__.py
+-rw-r--r--   0        0        0     4829 2023-04-15 07:23:31.757518 govtech_data-0.1.8/src/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.8/src/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0     1046 2023-04-15 06:49:21.541855 govtech_data-0.1.8/src/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.8/src/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.8/src/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.8/src/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.8/src/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.8/src/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.8/src/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-15 07:24:29.232006 govtech_data-0.1.8/src/govtech_data/utils/content.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 govtech_data-0.1.8/PKG-INFO
```

### Comparing `govtech_data-0.1.7/pyproject.toml` & `govtech_data-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "govtech-data"
-version = "0.1.7"
+version = "0.1.8"
 description = "Library to easily access and read data from data.gov.sg"
 authors = ["Khee-Chin Chua <kheechin@gmail.com>"]
 license = "Singapore Open Data License"
 readme = "README.md"
 packages = [{include = "govtech_data", from = "src"}]
 repository = "https://github.com/merlin83/govtech-data"
```

### Comparing `govtech_data-0.1.7/src/govtech_data/client.py` & `govtech_data-0.1.8/src/govtech_data/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
             timeout=DEFAULT_TIMEOUT_IN_SECONDS,
         )
         if not resp.ok:
             resp.raise_for_status()
         return model(**resp.json())
 
     @classmethod
-    @lru_cache(maxsize=128)
     @validate_arguments
     def fetch_resources_from_package_result(
         cls, package_result: PackageShowModelResult, limit: int = 0
     ) -> list[PackageResourceContent]:
         r = []
         for resource in package_result.resources:
             if limit != 0 and len(r) >= limit:
```

### Comparing `govtech_data-0.1.7/src/govtech_data/models/api.py` & `govtech_data-0.1.8/src/govtech_data/models/api.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.7/src/govtech_data/models/resources/datastore_search.py` & `govtech_data-0.1.8/src/govtech_data/models/resources/datastore_search.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.7/src/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.8/src/govtech_data/models/resources/package_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.7/src/govtech_data/models/resources/resource_show.py` & `govtech_data-0.1.8/src/govtech_data/models/resources/resource_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.7/PKG-INFO` & `govtech_data-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govtech-data
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to easily access and read data from data.gov.sg
 Home-page: https://github.com/merlin83/govtech-data
 License: Singapore Open Data License
 Author: Khee-Chin Chua
 Author-email: kheechin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

