# Comparing `tmp/mls-api-1.0.5.tar.gz` & `tmp/mls-api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.0.5.tar", last modified: Sat Sep 10 15:32:17 2022, max compression
+gzip compressed data, was "dist/mls-api-1.0.6.tar", last modified: Sat Apr 15 21:54:33 2023, max compression
```

## Comparing `mls-api-1.0.5.tar` & `mls-api-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2022-09-10 15:32:17.284324 mls-api-1.0.5/
--rw-r--r--   0 finn       (501) staff       (20)     6904 2022-09-10 15:32:17.284527 mls-api-1.0.5/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     3442 2022-09-10 15:31:13.000000 mls-api-1.0.5/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2022-09-10 15:32:17.281846 mls-api-1.0.5/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      413 2022-09-10 10:52:58.000000 mls-api-1.0.5/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/assists_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1500 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/fixtures_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1510 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/historical_data_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1496 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/latest_news_api.py
--rw-r--r--   0 finn       (501) staff       (20)      655 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/login.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/offence_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/players_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1458 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/real_time_data__live_scores_api.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.5/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)     1508 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/standings_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1476 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/teams_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1512 2022-09-10 10:20:53.000000 mls-api-1.0.5/mls_api/top_scorer_api.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2022-09-10 15:32:01.000000 mls-api-1.0.5/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2022-09-10 15:32:17.284052 mls-api-1.0.5/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     6904 2022-09-10 15:32:17.000000 mls-api-1.0.5/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      549 2022-09-10 15:32:17.000000 mls-api-1.0.5/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2022-09-10 15:32:17.000000 mls-api-1.0.5/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2022-09-10 15:32:14.000000 mls-api-1.0.5/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2022-09-10 15:32:17.000000 mls-api-1.0.5/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2022-09-10 15:32:17.000000 mls-api-1.0.5/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2022-09-10 15:32:17.285050 mls-api-1.0.5/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2022-09-10 15:32:01.000000 mls-api-1.0.5/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-15 21:54:33.860905 mls-api-1.0.6/
+-rw-r--r--   0 finn       (501) staff       (20)     6929 2023-04-15 21:54:33.861118 mls-api-1.0.6/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     3467 2023-04-15 21:50:10.000000 mls-api-1.0.6/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-15 21:54:33.857178 mls-api-1.0.6/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      413 2022-09-10 10:52:58.000000 mls-api-1.0.6/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/assists_api.py
+-rw-r--r--   0 finn       (501) staff       (20)     1500 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/fixtures_api.py
+-rw-r--r--   0 finn       (501) staff       (20)     1510 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/historical_data_api.py
+-rw-r--r--   0 finn       (501) staff       (20)     1496 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/latest_news_api.py
+-rw-r--r--   0 finn       (501) staff       (20)      655 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/login.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/offence_api.py
+-rw-r--r--   0 finn       (501) staff       (20)     1786 2023-04-15 21:48:26.000000 mls-api-1.0.6/mls_api/players_api.py
+-rw-r--r--   0 finn       (501) staff       (20)     1458 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/real_time_data__live_scores_api.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.6/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)     1508 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/standings_api.py
+-rw-r--r--   0 finn       (501) staff       (20)     1476 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/teams_api.py
+-rw-r--r--   0 finn       (501) staff       (20)     1512 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/top_scorer_api.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-15 21:52:31.000000 mls-api-1.0.6/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-15 21:54:33.860380 mls-api-1.0.6/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     6929 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      549 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-15 21:54:16.000000 mls-api-1.0.6/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-15 21:54:33.861641 mls-api-1.0.6/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-15 21:52:31.000000 mls-api-1.0.6/setup.py
```

### Comparing `mls-api-1.0.5/PKG-INFO` & `mls-api-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -75,15 +75,15 @@
             print(mls_historical)
         
             ## Retrieve MLS Historical Data by ID
             mls_historical_id = mls_api.get_historical_data(id='<insert unique id>')
             print(mls_historical_id)
         
             ## Retrieve MLS Players Data
-            mls_players = mls_api.get_players()
+            mls_players = mls_api.get_players(limit=10, offset=0)
             print(mls_players)
         
             ## Retrieve MLS Players Data by ID
             mls_players_id = mls_api.get_players(id='<insert unique id>')
             print(mls_players_id)
         
             ## Retrieve MLS Assist Data
@@ -166,15 +166,15 @@
         
         .. _MIT License: https://moatsystems.com/
         
         
         Copyright
         ----------
         
-        Copyright |copy| 2022 `Moat Systems Limited`_. All Rights Reserved.
+        Copyright |copy| 2021 - 2023 `Moat Systems Limited`_. All Rights Reserved.
         
         .. |copy| unicode:: 0xA9 .. copyright sign
         .. _Moat Systems Limited: https://moatsystems.com/
         
 Keywords: mls,mls api,mls_api,major league soccer,moat,moatsystems,moat systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mls-api-1.0.5/README.md` & `mls-api-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 print(mls_historical)
 
 ## Retrieve MLS Historical Data by ID
 mls_historical_id = mls_api.get_historical_data(id='<insert unique id>')
 print(mls_historical_id)
 
 ## Retrieve MLS Players Data
-mls_players = mls_api.get_players()
+mls_players = mls_api.get_players(limit=10, offset=0)
 print(mls_players)
 
 ## Retrieve MLS Players Data by ID
 mls_players_id = mls_api.get_players(id='<insert unique id>')
 print(mls_players_id)
 
 ## Retrieve MLS Assist Data
@@ -135,8 +135,8 @@
 ## License
 
 This project is licensed under the [MIT License](./LICENSE).
 
 
 ## Copyright
 
-(c) 2022 [Moat Systems Limited](https://moatsystems.com/). All Rights Reserved.
+(c) 2021 - 2023 [Moat Systems Limited](https://moatsystems.com/). All Rights Reserved.
```

### Comparing `mls-api-1.0.5/mls_api/assists_api.py` & `mls-api-1.0.6/mls_api/assists_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/fixtures_api.py` & `mls-api-1.0.6/mls_api/fixtures_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/historical_data_api.py` & `mls-api-1.0.6/mls_api/historical_data_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/latest_news_api.py` & `mls-api-1.0.6/mls_api/latest_news_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/login.py` & `mls-api-1.0.6/mls_api/login.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/offence_api.py` & `mls-api-1.0.6/mls_api/offence_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/players_api.py` & `mls-api-1.0.6/mls_api/top_scorer_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import requests
 import json
 import os
 
-def get_players(id=None):
+def get_top_scorer(id=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/players/'
+    url = 'https://mlssoccerapi.com/topscorer/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     if id != None: 
         url += id
     response = requests.get(url=url, headers=headers)
     return response.json()
 
-def update_players(id, payload):
+def update_top_scorer(id, payload):
     bearerToken = os.getenv('BEARER_TOKEN') 
-    url = f'https://mlssoccerapi.com/players/{id}'
+    url = f'https://mlssoccerapi.com/topscorer/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.put(url=url, headers=headers, data=payload)
     return response.json()
 
-def delete_players(id): 
+def delete_top_scorer(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f'https://mlssoccerapi.com/players/{id}'
+    url = f'https://mlssoccerapi.com/topscorer/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     payload = json.dumps({
         'id': id
     })
     response = requests.delete(url=url, headers=headers, data=payload)
     return response.json()
 
-def add_players(payload):
+def add_top_scorer(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/players/'
+    url = 'https://mlssoccerapi.com/topscorer/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.post(url=url, headers=headers, data=payload)
     return response.json()
```

### Comparing `mls-api-1.0.5/mls_api/real_time_data__live_scores_api.py` & `mls-api-1.0.6/mls_api/real_time_data__live_scores_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/six.py` & `mls-api-1.0.6/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/standings_api.py` & `mls-api-1.0.6/mls_api/standings_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/teams_api.py` & `mls-api-1.0.6/mls_api/teams_api.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/mls_api/top_scorer_api.py` & `mls-api-1.0.6/mls_api/players_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import requests
 import json
 import os
 
-def get_top_scorer(id=None):
+def get_players(id=None, limit=None, offset=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/topscorer/'
+    url = 'https://mlssoccerapi.com/players/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     if id != None: 
         url += id
+    else:
+        params = {}
+        if limit is not None:
+            params['limit'] = limit
+        if offset is not None:
+            params['offset'] = offset
+        if params:
+            url += '?' + '&'.join([f'{k}={v}' for k, v in params.items()])
+
     response = requests.get(url=url, headers=headers)
     return response.json()
 
-def update_top_scorer(id, payload):
+def update_players(id, payload):
     bearerToken = os.getenv('BEARER_TOKEN') 
-    url = f'https://mlssoccerapi.com/topscorer/{id}'
+    url = f'https://mlssoccerapi.com/players/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.put(url=url, headers=headers, data=payload)
     return response.json()
 
-def delete_top_scorer(id): 
+def delete_players(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f'https://mlssoccerapi.com/topscorer/{id}'
+    url = f'https://mlssoccerapi.com/players/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     payload = json.dumps({
         'id': id
     })
     response = requests.delete(url=url, headers=headers, data=payload)
     return response.json()
 
-def add_top_scorer(payload):
+def add_players(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/topscorer/'
+    url = 'https://mlssoccerapi.com/players/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.post(url=url, headers=headers, data=payload)
     return response.json()
```

### Comparing `mls-api-1.0.5/mls_api.egg-info/PKG-INFO` & `mls-api-1.0.6/mls_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -75,15 +75,15 @@
             print(mls_historical)
         
             ## Retrieve MLS Historical Data by ID
             mls_historical_id = mls_api.get_historical_data(id='<insert unique id>')
             print(mls_historical_id)
         
             ## Retrieve MLS Players Data
-            mls_players = mls_api.get_players()
+            mls_players = mls_api.get_players(limit=10, offset=0)
             print(mls_players)
         
             ## Retrieve MLS Players Data by ID
             mls_players_id = mls_api.get_players(id='<insert unique id>')
             print(mls_players_id)
         
             ## Retrieve MLS Assist Data
@@ -166,15 +166,15 @@
         
         .. _MIT License: https://moatsystems.com/
         
         
         Copyright
         ----------
         
-        Copyright |copy| 2022 `Moat Systems Limited`_. All Rights Reserved.
+        Copyright |copy| 2021 - 2023 `Moat Systems Limited`_. All Rights Reserved.
         
         .. |copy| unicode:: 0xA9 .. copyright sign
         .. _Moat Systems Limited: https://moatsystems.com/
         
 Keywords: mls,mls api,mls_api,major league soccer,moat,moatsystems,moat systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mls-api-1.0.5/mls_api.egg-info/SOURCES.txt` & `mls-api-1.0.6/mls_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.5/setup.py` & `mls-api-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

