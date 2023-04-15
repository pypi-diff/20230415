# Comparing `tmp/twitter-api-client-0.6.3.tar.gz` & `tmp/twitter-api-client-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.6.3.tar", last modified: Sat Apr 15 18:33:09 2023, max compression
+gzip compressed data, was "twitter-api-client-0.6.4.tar", last modified: Sat Apr 15 20:46:50 2023, max compression
```

## Comparing `twitter-api-client-0.6.3.tar` & `twitter-api-client-0.6.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 18:33:09.814455 twitter-api-client-0.6.3/
--rw-rw-r--   0 x         (1000) x         (1000)     1075 2023-04-14 02:53:18.000000 twitter-api-client-0.6.3/LICENSE
--rw-rw-r--   0 x         (1000) x         (1000)     6274 2023-04-15 18:33:09.814455 twitter-api-client-0.6.3/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)       38 2023-04-15 18:33:09.814455 twitter-api-client-0.6.3/setup.cfg
--rw-rw-r--   0 x         (1000) x         (1000)     7259 2023-04-15 18:33:03.000000 twitter-api-client-0.6.3/setup.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 18:33:09.806455 twitter-api-client-0.6.3/twitter/
--rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.3/twitter/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)    26558 2023-04-15 00:35:53.000000 twitter-api-client-0.6.3/twitter/account.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 18:33:09.814455 twitter-api-client-0.6.3/twitter/config/
--rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.3/twitter/config/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)      909 2023-04-14 02:53:18.000000 twitter-api-client-0.6.3/twitter/config/log.py
--rw-rw-r--   0 x         (1000) x         (1000)   147862 2023-04-14 21:16:39.000000 twitter-api-client-0.6.3/twitter/config/operations.py
--rw-rw-r--   0 x         (1000) x         (1000)     5859 2023-04-15 18:04:24.000000 twitter-api-client-0.6.3/twitter/config/settings.py
--rw-rw-r--   0 x         (1000) x         (1000)     2539 2023-04-14 21:53:11.000000 twitter-api-client-0.6.3/twitter/constants.py
--rw-rw-r--   0 x         (1000) x         (1000)     5242 2023-04-14 02:53:18.000000 twitter-api-client-0.6.3/twitter/login.py
--rw-rw-r--   0 x         (1000) x         (1000)    12761 2023-04-14 02:53:18.000000 twitter-api-client-0.6.3/twitter/scraper.py
--rw-rw-r--   0 x         (1000) x         (1000)     5478 2023-04-15 18:23:12.000000 twitter-api-client-0.6.3/twitter/search.py
--rw-rw-r--   0 x         (1000) x         (1000)     2235 2023-04-14 02:53:18.000000 twitter-api-client-0.6.3/twitter/utils.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 18:33:09.814455 twitter-api-client-0.6.3/twitter_api_client.egg-info/
--rw-rw-r--   0 x         (1000) x         (1000)     6274 2023-04-15 18:33:09.000000 twitter-api-client-0.6.3/twitter_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)      461 2023-04-15 18:33:09.000000 twitter-api-client-0.6.3/twitter_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 x         (1000) x         (1000)        1 2023-04-15 18:33:09.000000 twitter-api-client-0.6.3/twitter_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 x         (1000) x         (1000)       82 2023-04-15 18:33:09.000000 twitter-api-client-0.6.3/twitter_api_client.egg-info/requires.txt
--rw-rw-r--   0 x         (1000) x         (1000)        8 2023-04-15 18:33:09.000000 twitter-api-client-0.6.3/twitter_api_client.egg-info/top_level.txt
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/
+-rw-rw-r--   0 x         (1000) x         (1000)     1075 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/LICENSE
+-rw-rw-r--   0 x         (1000) x         (1000)     6274 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)       38 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/setup.cfg
+-rw-rw-r--   0 x         (1000) x         (1000)     7259 2023-04-15 20:45:23.000000 twitter-api-client-0.6.4/setup.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.846656 twitter-api-client-0.6.4/twitter/
+-rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)    26564 2023-04-15 20:45:23.000000 twitter-api-client-0.6.4/twitter/account.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/twitter/config/
+-rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/config/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)      909 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/config/log.py
+-rw-rw-r--   0 x         (1000) x         (1000)   147862 2023-04-14 21:16:39.000000 twitter-api-client-0.6.4/twitter/config/operations.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5859 2023-04-15 18:04:24.000000 twitter-api-client-0.6.4/twitter/config/settings.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2539 2023-04-14 21:53:11.000000 twitter-api-client-0.6.4/twitter/constants.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5242 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/login.py
+-rw-rw-r--   0 x         (1000) x         (1000)    12761 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/scraper.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5478 2023-04-15 18:23:12.000000 twitter-api-client-0.6.4/twitter/search.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2235 2023-04-14 02:53:18.000000 twitter-api-client-0.6.4/twitter/utils.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 20:46:50.850656 twitter-api-client-0.6.4/twitter_api_client.egg-info/
+-rw-rw-r--   0 x         (1000) x         (1000)     6274 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)      461 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        1 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 x         (1000) x         (1000)       82 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/requires.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        8 2023-04-15 20:46:50.000000 twitter-api-client-0.6.4/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.6.3/LICENSE` & `twitter-api-client-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/PKG-INFO` & `twitter-api-client-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.3
+Version: 0.6.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.6.3/setup.py` & `twitter-api-client-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.6.3",
+    version="0.6.4",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
```

### Comparing `twitter-api-client-0.6.3/twitter/account.py` & `twitter-api-client-0.6.4/twitter/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
     @log(info=['json'])
     def home_timeline(self):
         return self.gql(Operation.Account.HomeTimeline, {})
 
     def home_latest_timeline(self, limit: int = 100):
         r = self.gql(Operation.Account.HomeLatestTimeline, {})
         data = r.json() | {ID: self.session.cookies.get('username')}
-        return self.paginate(self.session, data, Operation.Account.HomeTimeline, limit)
+        return self.paginate(self.session, data, Operation.Account.HomeLatestTimeline, limit)
 
     # todo: a lot of duplicated code here, will need to refactor
     def paginate(self, session: Session, data: dict, operation: tuple, limit: int):
 
         def get_cursor(data):
             # inefficient, but need to deal with arbitrary schema
             entries = find_key(data, 'entries')
```

### Comparing `twitter-api-client-0.6.3/twitter/config/log.py` & `twitter-api-client-0.6.4/twitter/config/log.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter/config/operations.py` & `twitter-api-client-0.6.4/twitter/config/operations.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter/config/settings.py` & `twitter-api-client-0.6.4/twitter/config/settings.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter/constants.py` & `twitter-api-client-0.6.4/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter/login.py` & `twitter-api-client-0.6.4/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter/scraper.py` & `twitter-api-client-0.6.4/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter/search.py` & `twitter-api-client-0.6.4/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter/utils.py` & `twitter-api-client-0.6.4/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.3/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.6.4/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.3
+Version: 0.6.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

