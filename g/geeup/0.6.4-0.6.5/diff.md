# Comparing `tmp/geeup-0.6.4.tar.gz` & `tmp/geeup-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\geeup-0.6.4.tar", last modified: Thu Apr 13 02:38:19 2023, max compression
+gzip compressed data, was "dist\geeup-0.6.5.tar", last modified: Sat Apr 15 05:31:16 2023, max compression
```

## Comparing `geeup-0.6.4.tar` & `geeup-0.6.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:38:19.607045 geeup-0.6.4/
--rw-rw-rw-   0        0        0    31128 2023-04-13 02:38:19.589545 geeup-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0    25398 2023-04-13 02:37:01.000000 geeup-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:38:19.522635 geeup-0.6.4/geeup/
--rw-rw-rw-   0        0        0      119 2023-04-13 02:33:00.000000 geeup-0.6.4/geeup/__init__.py
--rw-rw-rw-   0        0        0       69 2020-06-18 02:06:06.000000 geeup-0.6.4/geeup/__main__.py
--rw-rw-rw-   0        0        0    17773 2023-04-13 02:23:25.000000 geeup-0.6.4/geeup/batch_uploader.py
--rw-rw-rw-   0        0        0    22030 2023-04-13 02:22:21.000000 geeup-0.6.4/geeup/geeup.py
--rw-rw-rw-   0        0        0     1504 2022-09-03 22:53:54.000000 geeup-0.6.4/geeup/getmeta.py
--rw-rw-rw-   0        0        0     3707 2021-04-16 00:02:09.000000 geeup-0.6.4/geeup/metadata_loader.py
--rw-rw-rw-   0        0        0    15888 2023-02-04 18:45:53.000000 geeup-0.6.4/geeup/tuploader.py
--rw-rw-rw-   0        0        0     2074 2022-05-26 04:04:00.000000 geeup-0.6.4/geeup/zipfiles.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:38:19.582545 geeup-0.6.4/geeup.egg-info/
--rw-rw-rw-   0        0        0    31128 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      253 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 02:38:19.607878 geeup-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1884 2023-04-13 02:33:22.000000 geeup-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:31:16.838020 geeup-0.6.5/
+-rw-rw-rw-   0        0        0    31342 2023-04-15 05:31:16.823903 geeup-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0    25572 2023-04-15 05:30:50.000000 geeup-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 05:31:16.761566 geeup-0.6.5/geeup/
+-rw-rw-rw-   0        0        0      119 2023-04-15 05:28:39.000000 geeup-0.6.5/geeup/__init__.py
+-rw-rw-rw-   0        0        0       69 2020-06-18 02:06:06.000000 geeup-0.6.5/geeup/__main__.py
+-rw-rw-rw-   0        0        0    17093 2023-04-15 05:28:02.000000 geeup-0.6.5/geeup/batch_uploader.py
+-rw-rw-rw-   0        0        0    22076 2023-04-15 05:27:21.000000 geeup-0.6.5/geeup/geeup.py
+-rw-rw-rw-   0        0        0     1504 2022-09-03 22:53:54.000000 geeup-0.6.5/geeup/getmeta.py
+-rw-rw-rw-   0        0        0     3707 2021-04-16 00:02:09.000000 geeup-0.6.5/geeup/metadata_loader.py
+-rw-rw-rw-   0        0        0    15888 2023-02-04 18:45:53.000000 geeup-0.6.5/geeup/tuploader.py
+-rw-rw-rw-   0        0        0     2074 2022-05-26 04:04:00.000000 geeup-0.6.5/geeup/zipfiles.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:31:16.819905 geeup-0.6.5/geeup.egg-info/
+-rw-rw-rw-   0        0        0    31342 2023-04-15 05:31:15.000000 geeup-0.6.5/geeup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-15 05:31:15.000000 geeup-0.6.5/geeup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 05:31:15.000000 geeup-0.6.5/geeup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-15 05:31:15.000000 geeup-0.6.5/geeup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      253 2023-04-15 05:31:15.000000 geeup-0.6.5/geeup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 05:31:15.000000 geeup-0.6.5/geeup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 05:31:16.839018 geeup-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1884 2023-04-15 05:28:50.000000 geeup-0.6.5/setup.py
```

### Comparing `geeup-0.6.4/PKG-INFO` & `geeup-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeup
-Version: 0.6.4
+Version: 0.6.5
 Summary: Simple Client for Earth Engine Uploads
 Home-page: https://github.com/samapriya/geeup
 Author: Samapriya Roy
 Author-email: samapriya.roy@gmail.com
 License: Apache 2.0
 Description: # geeup: Simple CLI for Earth Engine Uploads
         
@@ -344,14 +344,19 @@
         
         optional arguments:
           -h, --help  show this help message and exit
         ```
         
         # Changelog
         
+        ### 0.6.5
+        - Fixed issue with iteritems for pandas >2.0.0
+        - Updated task running check and updated function
+        - Updated handling boolean for using last band as alpha mask
+        
         ### 0.6.4
         - Added masking option to use last band as mask
         
         ### 0.6.2
         - Removed call to shell
         - Now prints status of task at task creation
         - Overwrite option for both images and tables
```

### Comparing `geeup-0.6.4/README.md` & `geeup-0.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -336,14 +336,19 @@
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 
 # Changelog
 
+### 0.6.5
+- Fixed issue with iteritems for pandas >2.0.0
+- Updated task running check and updated function
+- Updated handling boolean for using last band as alpha mask
+
 ### 0.6.4
 - Added masking option to use last band as mask
 
 ### 0.6.2
 - Removed call to shell
 - Now prints status of task at task creation
 - Overwrite option for both images and tables
```

### Comparing `geeup-0.6.4/geeup/batch_uploader.py` & `geeup-0.6.5/geeup/batch_uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import print_function
 
 __copyright__ = """
 
-    Copyright 2016 Lukasz Tracewski
+    Copyright 2023 Samapriya Roy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
@@ -15,40 +15,14 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 """
 __license__ = "Apache 2.0"
 
-__Modifications_copyright__ = """
-
-    Copyright 2022 Samapriya Roy
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-
-"""
-__license__ = "Apache 2.0"
-
-"""
-Modifications to file:
-- Uses cookie based upload
-- Removed multipart upload
-- Uses polling
-"""
-
 import ast
 import csv
 import glob
 import json
 import logging
 import os
 import platform
@@ -80,14 +54,27 @@
         self.custom_defined_schema = schema
 
     def _format_message(self, field, error):
         print("")
         return "GEE file name & path cannot have spaces & can only have letters, numbers, hyphens and underscores"
 
 
+def task_counter():
+    ee.Initialize()
+    status = ["RUNNING", "PENDING"]
+    task_count = len(
+        [
+            task
+            for task in ee.data.listOperations()
+            if task["metadata"]["state"] in status
+        ]
+    )
+    return task_count
+
+
 def upload(
     user,
     source_path,
     pyramiding,
     mask,
     destination_path,
     metadata_path=None,
@@ -129,27 +116,21 @@
         print("No images found that match %s. Exiting...", path)
         sys.exit(1)
     file_count = len(images_for_upload_path)
     for current_image_no, image_path in enumerate(natsorted(images_for_upload_path)):
         # logging.info(
         #     f"Processing image {current_image_no + 1} out of {no_images} : {image_path}"
         # )
-        status = ["RUNNING", "PENDING"]
-        task_count = len(
-            [
-                task
-                for task in ee.data.listOperations()
-                if task["metadata"]["state"] in status
-            ]
-        )
-        while task_count >= 2500:
+        task_count = task_counter()
+        while task_count >= 2800:
             logging.info(
                 f"Total tasks running or submitted {task_count}: waiting for 5 minutes"
             )
             time.sleep(300)
+            task_count = task_counter()
         filename = __get_filename_from_path(path=image_path)
 
         destination_path = ee.data.getAsset(destination_path + "/")["name"]
         asset_full_path = destination_path + "/" + filename
 
         if metadata and not filename in metadata:
             print(
@@ -161,15 +142,15 @@
         try:
             if user is not None:
                 gsid = __upload_file_gee(
                     session=google_session, file_path=image_path)
 
             df = pd.read_csv(metadata_path)
             dd = (df.applymap(type) == str).all(0)
-            for ind, val in dd.iteritems():
+            for ind, val in dd.items():
                 if val == True:
                     slist.append(ind)
             intcol = list(df.select_dtypes(include=["int64"]).columns)
             floatcol = list(df.select_dtypes(include=["float64"]).columns)
             with open(metadata_path, "r") as f:
                 reader = csv.DictReader(f, delimiter=",")
                 for i, line in enumerate(reader):
```

### Comparing `geeup-0.6.4/geeup/geeup.py` & `geeup-0.6.5/geeup/geeup.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,14 +562,15 @@
         "--nodata",
         type=int,
         help="The value to burn into the raster as NoData (missing data)",
     )
     optional_named.add_argument(
         "--mask",
         default=False,
+        choices=('True', 'False', 't', 'f'),
         help="Binary to use last band for mask True or False",
     )
     optional_named.add_argument(
         "--pyramids",
         help="Pyramiding Policy, MEAN, MODE, MIN, MAX, SAMPLE",
     )
     optional_named.add_argument(
```

### Comparing `geeup-0.6.4/geeup/getmeta.py` & `geeup-0.6.5/geeup/getmeta.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.4/geeup/metadata_loader.py` & `geeup-0.6.5/geeup/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.4/geeup/tuploader.py` & `geeup-0.6.5/geeup/tuploader.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.4/geeup/zipfiles.py` & `geeup-0.6.5/geeup/zipfiles.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.4/geeup.egg-info/PKG-INFO` & `geeup-0.6.5/geeup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeup
-Version: 0.6.4
+Version: 0.6.5
 Summary: Simple Client for Earth Engine Uploads
 Home-page: https://github.com/samapriya/geeup
 Author: Samapriya Roy
 Author-email: samapriya.roy@gmail.com
 License: Apache 2.0
 Description: # geeup: Simple CLI for Earth Engine Uploads
         
@@ -344,14 +344,19 @@
         
         optional arguments:
           -h, --help  show this help message and exit
         ```
         
         # Changelog
         
+        ### 0.6.5
+        - Fixed issue with iteritems for pandas >2.0.0
+        - Updated task running check and updated function
+        - Updated handling boolean for using last band as alpha mask
+        
         ### 0.6.4
         - Added masking option to use last band as mask
         
         ### 0.6.2
         - Removed call to shell
         - Now prints status of task at task creation
         - Overwrite option for both images and tables
```

### Comparing `geeup-0.6.4/setup.py` & `geeup-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setuptools.setup(
     name="geeup",
-    version="0.6.4",
+    version="0.6.5",
     packages=find_packages(),
     url="https://github.com/samapriya/geeup",
     install_requires=[
         "wheel",
         "earthengine_api>=0.1.274",
         "logzero>=1.5.0",
         "requests >= 2.10.0",
```

