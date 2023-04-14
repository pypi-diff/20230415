# Comparing `tmp/bingx_headers_generator-0.0.1.tar.gz` & `tmp/bingx_headers_generator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingx_headers_generator-0.0.1.tar", last modified: Sat Feb  4 00:31:24 2023, max compression
+gzip compressed data, was "bingx_headers_generator-1.0.1.tar", last modified: Fri Apr 14 22:56:49 2023, max compression
```

## Comparing `bingx_headers_generator-0.0.1.tar` & `bingx_headers_generator-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sajmon     (501) staff       (20)        0 2023-02-04 00:31:24.931766 bingx_headers_generator-0.0.1/
--rw-r--r--   0 sajmon     (501) staff       (20)     1069 2023-02-03 23:26:57.000000 bingx_headers_generator-0.0.1/LICENSE
--rw-r--r--   0 sajmon     (501) staff       (20)     2322 2023-02-04 00:31:24.931333 bingx_headers_generator-0.0.1/PKG-INFO
--rw-r--r--   0 sajmon     (501) staff       (20)     1608 2023-02-04 00:14:58.000000 bingx_headers_generator-0.0.1/README.md
-drwxr-xr-x   0 sajmon     (501) staff       (20)        0 2023-02-04 00:31:24.928279 bingx_headers_generator-0.0.1/bingx_headers_generator/
--rw-r--r--   0 sajmon     (501) staff       (20)       45 2023-02-03 23:24:17.000000 bingx_headers_generator-0.0.1/bingx_headers_generator/__init__.py
--rw-r--r--   0 sajmon     (501) staff       (20)      214 2023-02-03 23:15:37.000000 bingx_headers_generator-0.0.1/bingx_headers_generator/__version__.py
--rw-r--r--   0 sajmon     (501) staff       (20)     3744 2023-02-02 21:51:03.000000 bingx_headers_generator-0.0.1/bingx_headers_generator/generator.py
-drwxr-xr-x   0 sajmon     (501) staff       (20)        0 2023-02-04 00:31:24.930705 bingx_headers_generator-0.0.1/bingx_headers_generator.egg-info/
--rw-r--r--   0 sajmon     (501) staff       (20)     2322 2023-02-04 00:31:24.000000 bingx_headers_generator-0.0.1/bingx_headers_generator.egg-info/PKG-INFO
--rw-r--r--   0 sajmon     (501) staff       (20)      326 2023-02-04 00:31:24.000000 bingx_headers_generator-0.0.1/bingx_headers_generator.egg-info/SOURCES.txt
--rw-r--r--   0 sajmon     (501) staff       (20)        1 2023-02-04 00:31:24.000000 bingx_headers_generator-0.0.1/bingx_headers_generator.egg-info/dependency_links.txt
--rw-r--r--   0 sajmon     (501) staff       (20)       24 2023-02-04 00:31:24.000000 bingx_headers_generator-0.0.1/bingx_headers_generator.egg-info/top_level.txt
--rw-r--r--   0 sajmon     (501) staff       (20)       38 2023-02-04 00:31:24.931915 bingx_headers_generator-0.0.1/setup.cfg
--rw-r--r--   0 sajmon     (501) staff       (20)     1133 2023-02-04 00:11:47.000000 bingx_headers_generator-0.0.1/setup.py
+drwxr-xr-x   0 sajmon     (501) staff       (20)        0 2023-04-14 22:56:49.975908 bingx_headers_generator-1.0.1/
+-rw-r--r--   0 sajmon     (501) staff       (20)     1069 2023-04-14 21:39:31.000000 bingx_headers_generator-1.0.1/LICENSE
+-rw-r--r--   0 sajmon     (501) staff       (20)     2570 2023-04-14 22:56:49.975441 bingx_headers_generator-1.0.1/PKG-INFO
+-rw-r--r--   0 sajmon     (501) staff       (20)     1856 2023-04-14 21:39:31.000000 bingx_headers_generator-1.0.1/README.md
+drwxr-xr-x   0 sajmon     (501) staff       (20)        0 2023-04-14 22:56:49.971318 bingx_headers_generator-1.0.1/bingx_headers_generator/
+-rw-r--r--   0 sajmon     (501) staff       (20)       45 2023-04-14 21:39:31.000000 bingx_headers_generator-1.0.1/bingx_headers_generator/__init__.py
+-rw-r--r--   0 sajmon     (501) staff       (20)      214 2023-04-14 22:45:22.000000 bingx_headers_generator-1.0.1/bingx_headers_generator/__version__.py
+-rw-r--r--   0 sajmon     (501) staff       (20)     4293 2023-04-14 22:50:40.000000 bingx_headers_generator-1.0.1/bingx_headers_generator/generator.py
+drwxr-xr-x   0 sajmon     (501) staff       (20)        0 2023-04-14 22:56:49.974369 bingx_headers_generator-1.0.1/bingx_headers_generator.egg-info/
+-rw-r--r--   0 sajmon     (501) staff       (20)     2570 2023-04-14 22:56:49.000000 bingx_headers_generator-1.0.1/bingx_headers_generator.egg-info/PKG-INFO
+-rw-r--r--   0 sajmon     (501) staff       (20)      326 2023-04-14 22:56:49.000000 bingx_headers_generator-1.0.1/bingx_headers_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 sajmon     (501) staff       (20)        1 2023-04-14 22:56:49.000000 bingx_headers_generator-1.0.1/bingx_headers_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 sajmon     (501) staff       (20)       24 2023-04-14 22:56:49.000000 bingx_headers_generator-1.0.1/bingx_headers_generator.egg-info/top_level.txt
+-rw-r--r--   0 sajmon     (501) staff       (20)       38 2023-04-14 22:56:49.976090 bingx_headers_generator-1.0.1/setup.cfg
+-rw-r--r--   0 sajmon     (501) staff       (20)     1133 2023-04-14 21:39:31.000000 bingx_headers_generator-1.0.1/setup.py
```

### Comparing `bingx_headers_generator-0.0.1/LICENSE` & `bingx_headers_generator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bingx_headers_generator-0.0.1/PKG-INFO` & `bingx_headers_generator-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingx_headers_generator
-Version: 0.0.1
+Version: 1.0.1
 Summary: BingX Headers Generator that allows to access most of the BingX API endpoints
 Author: niewiemczego
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -13,17 +13,21 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# THIS PROJECT IS FOR EDUCATIONAL PURPOSES ONLY!
+
+Please keep in mind that I do **NOT** encourage breaking any sort of security on websites. In addition, the project will not be updated in case of security changes by BingX
+
 # bingx-headers-generator
 
-BingX Headers Generator is an python library which generates for you all required headers to make requests to BingX non-public API endpoints
+BingX Headers Generator is an python library which generates for you all required headers to make requests to BingX API endpoints
 
 # Installation
 
 ```
 pip install bingx-headers-generator
 ```
 
@@ -61,10 +65,9 @@
 
 ```
 
 # How did I find out how to generate headers?
 
 In one of their site files(**https://bin.bb-os.com/_nuxt/1491b29.js**) I found interesting function - `function wt(e)` Go check it and you follow other functions that are called in `wt()` and I'm sure you will start to understand the whole process of generating headers
 
-# THIS PROJECT IS ONLY FOR LEARN PURPOSE!
+<img width="1134" alt="Screenshot 2023-04-04 at 23 12 48" src="https://user-images.githubusercontent.com/50675404/229923789-89571a8b-7372-4c1a-9386-6b9ceecd3fe3.png">
 
-Please keep in mind that I do **NOT** encourage breaking any sort of security on websites
```

### Comparing `bingx_headers_generator-0.0.1/README.md` & `bingx_headers_generator-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+# THIS PROJECT IS FOR EDUCATIONAL PURPOSES ONLY!
+
+Please keep in mind that I do **NOT** encourage breaking any sort of security on websites. In addition, the project will not be updated in case of security changes by BingX
+
 # bingx-headers-generator
 
-BingX Headers Generator is an python library which generates for you all required headers to make requests to BingX non-public API endpoints
+BingX Headers Generator is an python library which generates for you all required headers to make requests to BingX API endpoints
 
 # Installation
 
 ```
 pip install bingx-headers-generator
 ```
 
@@ -42,10 +46,9 @@
 
 ```
 
 # How did I find out how to generate headers?
 
 In one of their site files(**https://bin.bb-os.com/_nuxt/1491b29.js**) I found interesting function - `function wt(e)` Go check it and you follow other functions that are called in `wt()` and I'm sure you will start to understand the whole process of generating headers
 
-# THIS PROJECT IS ONLY FOR LEARN PURPOSE!
+<img width="1134" alt="Screenshot 2023-04-04 at 23 12 48" src="https://user-images.githubusercontent.com/50675404/229923789-89571a8b-7372-4c1a-9386-6b9ceecd3fe3.png">
 
-Please keep in mind that I do **NOT** encourage breaking any sort of security on websites
```

### Comparing `bingx_headers_generator-0.0.1/bingx_headers_generator/generator.py` & `bingx_headers_generator-1.0.1/bingx_headers_generator/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import time, requests, uuid
+import time
+import uuid
 from hashlib import sha256
 from typing import Any
 
+import cloudscraper
+
 
 class BingXHeadersGenerator:
     __DEFAULT_BEGINNING_VALUE = "95d65c73dc5c4370ae9018fb7f2eab69"  # this value can be found in the one of their obfuscated JS files on their website
-    __DEFAULT_PAGE_SIZE = "10"
+    __DEFAULT_PAGE_SIZE = "100"
 
     def __init__(
         self,
         app_version: str,
         user_id: str,
         api_identity: str,
         app_id: str = "30004",
@@ -18,30 +21,37 @@
     ):
         self.__app_version = app_version
         self.__user_id = user_id
         self.__api_identity = api_identity
         self.__app_id = app_id
         self.__main_app_id = main_app_id
         self.__platform_id = platform_id
+        self.session = cloudscraper.create_scraper()
 
     def generate_encryption_content(self) -> str:
         """
         It generates the encryption content for the request which is used to generate the sign.\n
         The encryption content is created by concatenating specific values in a specific order.
         """
         self.__timestamp = str(int(time.time() * 1000))
         self.__trace_id = str(uuid.uuid4())
         self.__device_id = str(uuid.uuid4())
-        payload = (
-            '{"apiIdentity":"api_identity","pageId":"0","pageSize":"__DEFAULT_PAGE_SIZE","uid":"user_id"}'.replace(
-                "api_identity", self.__api_identity
+        if self.__api_identity != "0":
+            payload = (
+                '{"apiIdentity":"api_identity","pageId":"0","pageSize":"__DEFAULT_PAGE_SIZE","uid":"user_id"}'
+                .replace("api_identity", self.__api_identity)
+                .replace("user_id", self.__user_id)
+                .replace("__DEFAULT_PAGE_SIZE", self.__DEFAULT_PAGE_SIZE)
+            )
+        else:
+            payload = (
+                '{"pageId":"0","pageSize":"__DEFAULT_PAGE_SIZE","trader":"user_id"}'
+                .replace("user_id", self.__user_id)
+                .replace("__DEFAULT_PAGE_SIZE", self.__DEFAULT_PAGE_SIZE)
             )
-            .replace("user_id", self.__user_id)
-            .replace("__DEFAULT_PAGE_SIZE", self.__DEFAULT_PAGE_SIZE)
-        )
         encryption_content = "".join(
             [
                 self.__DEFAULT_BEGINNING_VALUE,
                 self.__timestamp,
                 self.__trace_id,
                 self.__device_id,
                 self.__platform_id,
@@ -77,21 +87,21 @@
             "sign": sign,
             "timestamp": self.__timestamp,
             "timezone": "1",
             "traceid": self.__trace_id,
         }
         return headers | custom_headers
 
-    def make_request(
-        self, type: str, base_url: str, custom_headers: dict[str, Any] = {}
-    ) -> requests.Response:
+    def make_request(self, type: str, base_url: str, custom_headers: dict[str, Any] = {}) -> cloudscraper.requests.Response:
         """
         This function makes a request to the API using the given type (GET, POST, etc.) and base URL
 
         :param type: str - The type of request you want to make i.e. GET or POST
         :param base_url: The base url for the request i.e. https://api-app.we-api.com/api/copytrade/v1/real/trader/positions
         """
         headers = self.generate_headers(custom_headers)
-
-        complete_url = f"{base_url}?uid={self.__user_id}&apiIdentity={self.__api_identity}&pageId=0&pageSize={self.__DEFAULT_PAGE_SIZE}"
-        res = requests.request(type.upper(), complete_url, headers=headers)
+        if self.__api_identity != "0":
+            complete_url = f"{base_url}?uid={self.__user_id}&apiIdentity={self.__api_identity}&pageId=0&pageSize={self.__DEFAULT_PAGE_SIZE}"
+        else:
+            complete_url = f"{base_url}?trader={self.__user_id}&pageId=0&pageSize={self.__DEFAULT_PAGE_SIZE}"
+        res = self.session.request(type.upper(), complete_url, headers=headers)
         return res
```

### Comparing `bingx_headers_generator-0.0.1/bingx_headers_generator.egg-info/PKG-INFO` & `bingx_headers_generator-1.0.1/bingx_headers_generator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingx-headers-generator
-Version: 0.0.1
+Version: 1.0.1
 Summary: BingX Headers Generator that allows to access most of the BingX API endpoints
 Author: niewiemczego
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -13,17 +13,21 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# THIS PROJECT IS FOR EDUCATIONAL PURPOSES ONLY!
+
+Please keep in mind that I do **NOT** encourage breaking any sort of security on websites. In addition, the project will not be updated in case of security changes by BingX
+
 # bingx-headers-generator
 
-BingX Headers Generator is an python library which generates for you all required headers to make requests to BingX non-public API endpoints
+BingX Headers Generator is an python library which generates for you all required headers to make requests to BingX API endpoints
 
 # Installation
 
 ```
 pip install bingx-headers-generator
 ```
 
@@ -61,10 +65,9 @@
 
 ```
 
 # How did I find out how to generate headers?
 
 In one of their site files(**https://bin.bb-os.com/_nuxt/1491b29.js**) I found interesting function - `function wt(e)` Go check it and you follow other functions that are called in `wt()` and I'm sure you will start to understand the whole process of generating headers
 
-# THIS PROJECT IS ONLY FOR LEARN PURPOSE!
+<img width="1134" alt="Screenshot 2023-04-04 at 23 12 48" src="https://user-images.githubusercontent.com/50675404/229923789-89571a8b-7372-4c1a-9386-6b9ceecd3fe3.png">
 
-Please keep in mind that I do **NOT** encourage breaking any sort of security on websites
```

### Comparing `bingx_headers_generator-0.0.1/setup.py` & `bingx_headers_generator-1.0.1/setup.py`

 * *Files identical despite different names*

