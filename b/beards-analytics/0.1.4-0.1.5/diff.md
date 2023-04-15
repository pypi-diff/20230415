# Comparing `tmp/beards_analytics-0.1.4-py3-none-any.whl.zip` & `tmp/beards_analytics-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,22 @@
-Zip file size: 4880 bytes, number of entries: 11
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-14 15:50 beards_analytics/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:10 beards_analytics/cloud_functions/__init__.py
--rw-r--r--  2.0 unx     3049 b- defN 23-Apr-11 14:20 beards_analytics/cloud_functions/http.py
+Zip file size: 10171 bytes, number of entries: 20
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-15 14:49 beards_analytics/__init__.py
+-rw-r--r--  2.0 unx       19 b- defN 23-Apr-15 14:34 beards_analytics/cloud_functions/__init__.py
+-rw-r--r--  2.0 unx     3087 b- defN 23-Apr-15 14:45 beards_analytics/cloud_functions/http.py
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-15 14:30 beards_analytics/common/__init__.py
+-rw-r--r--  2.0 unx      847 b- defN 23-Apr-11 15:43 beards_analytics/common/date.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-Apr-15 14:29 beards_analytics/common/logger.py
+-rw-r--r--  2.0 unx     1342 b- defN 23-Apr-15 14:43 beards_analytics/common/tasks.py
+-rw-r--r--  2.0 unx       82 b- defN 23-Apr-14 14:04 beards_analytics/common/types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 11:18 beards_analytics/data/__init__.py
 -rw-r--r--  2.0 unx      514 b- defN 23-Apr-11 13:34 beards_analytics/data/models.py
--rw-r--r--  2.0 unx      782 b- defN 23-Apr-11 14:50 beards_analytics/data/operations.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Apr-14 15:50 beards_analytics-0.1.4.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      680 b- defN 23-Apr-14 15:50 beards_analytics-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 15:50 beards_analytics-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-14 15:50 beards_analytics-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      977 b- defN 23-Apr-14 15:50 beards_analytics-0.1.4.dist-info/RECORD
-11 files, 7193 bytes uncompressed, 3184 bytes compressed:  55.7%
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-14 21:27 beards_analytics/data/operations.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 21:32 beards_analytics/public_api/__init__.py
+-rw-r--r--  2.0 unx     2846 b- defN 23-Apr-15 14:17 beards_analytics/public_api/_metadata.py
+-rw-r--r--  2.0 unx     2162 b- defN 23-Apr-15 14:38 beards_analytics/public_api/client.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Apr-14 20:48 beards_analytics/public_api/models.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Apr-15 14:50 beards_analytics-0.1.5.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      731 b- defN 23-Apr-15 14:50 beards_analytics-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 14:50 beards_analytics-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-15 14:50 beards_analytics-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1798 b- defN 23-Apr-15 14:50 beards_analytics-0.1.5.dist-info/RECORD
+20 files, 18662 bytes uncompressed, 7159 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -3,32 +3,59 @@
 
 Filename: beards_analytics/cloud_functions/__init__.py
 Comment: 
 
 Filename: beards_analytics/cloud_functions/http.py
 Comment: 
 
+Filename: beards_analytics/common/__init__.py
+Comment: 
+
+Filename: beards_analytics/common/date.py
+Comment: 
+
+Filename: beards_analytics/common/logger.py
+Comment: 
+
+Filename: beards_analytics/common/tasks.py
+Comment: 
+
+Filename: beards_analytics/common/types.py
+Comment: 
+
 Filename: beards_analytics/data/__init__.py
 Comment: 
 
 Filename: beards_analytics/data/models.py
 Comment: 
 
 Filename: beards_analytics/data/operations.py
 Comment: 
 
-Filename: beards_analytics-0.1.4.dist-info/LICENCE.txt
+Filename: beards_analytics/public_api/__init__.py
+Comment: 
+
+Filename: beards_analytics/public_api/_metadata.py
+Comment: 
+
+Filename: beards_analytics/public_api/client.py
+Comment: 
+
+Filename: beards_analytics/public_api/models.py
+Comment: 
+
+Filename: beards_analytics-0.1.5.dist-info/LICENCE.txt
 Comment: 
 
-Filename: beards_analytics-0.1.4.dist-info/METADATA
+Filename: beards_analytics-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: beards_analytics-0.1.4.dist-info/WHEEL
+Filename: beards_analytics-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: beards_analytics-0.1.4.dist-info/top_level.txt
+Filename: beards_analytics-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: beards_analytics-0.1.4.dist-info/RECORD
+Filename: beards_analytics-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beards_analytics/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
```

## beards_analytics/cloud_functions/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 2069 6d70 6f72 7420 6874  from . import ht
+00000010: 7470 0a                                  tp.
```

## beards_analytics/cloud_functions/http.py

```diff
@@ -75,14 +75,15 @@
     func = functions_framework.http(func)
     func = safe_return(func)
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         _update_flask_request()
         
+        # TODO: Add exception handler
         try:
             return func(*args, **kwargs)
         except pydantic.ValidationError as e:
             if hasattr(e, _INPUT_SOURCE):
                 input_source: str = getattr(e, _INPUT_SOURCE)
                 return error_response(message=f'Invalid {input_source}', errors=e.errors(), status_code=400)
             raise
```

## Comparing `beards_analytics-0.1.4.dist-info/LICENCE.txt` & `beards_analytics-0.1.5.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `beards_analytics-0.1.4.dist-info/METADATA` & `beards_analytics-0.1.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beards-analytics
-Version: 0.1.4
+Version: 0.1.5
 Summary: Beards Analytics packages
 Home-page: https://beardsanalytics.com
 Author: Beards Analytics
 Author-email: tz@or.com.ua
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,11 +13,13 @@
 License-File: LICENCE.txt
 Requires-Dist: python-slugify
 Requires-Dist: flask
 Requires-Dist: pydantic
 Requires-Dist: functions-framework
 Requires-Dist: ujson
 Requires-Dist: pendulum
+Requires-Dist: google-auth
+Requires-Dist: requests
 
 # Beards Analytics Python Packages
 
 A useful set of functions to build Google Cloud Functions and more
```

