# Comparing `tmp/selenextra-0.7.tar.gz` & `tmp/selenextra-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.7.tar", last modified: Sun Apr  9 09:30:21 2023, max compression
+gzip compressed data, was "selenextra-0.8.tar", last modified: Sat Apr 15 06:01:36 2023, max compression
```

## Comparing `selenextra-0.7.tar` & `selenextra-0.8.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:30:21.626941 selenextra-0.7/
--rw-rw-rw-   0        0        0    35823 2023-04-09 08:30:10.000000 selenextra-0.7/LICENSE
--rw-rw-rw-   0        0        0   247181 2023-03-28 09:22:26.000000 selenextra-0.7/LICENSE.chromedriver
--rw-rw-rw-   0        0        0      625 2023-04-09 09:30:21.625944 selenextra-0.7/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-04-09 08:30:10.000000 selenextra-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 09:30:21.619958 selenextra-0.7/selenextra/
--rw-rw-rw-   0        0        0     4440 2023-04-09 09:27:39.000000 selenextra-0.7/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-09 08:30:10.000000 selenextra-0.7/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-09 08:30:10.000000 selenextra-0.7/selenextra/patcher.py
--rw-rw-rw-   0        0        0     5149 2023-04-09 08:30:10.000000 selenextra-0.7/selenextra/typer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:30:21.625944 selenextra-0.7/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 09:30:21.626941 selenextra-0.7/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-09 09:27:45.000000 selenextra-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:01:36.560641 selenextra-0.8/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 04:40:09.000000 selenextra-0.8/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-04-15 06:01:36.560641 selenextra-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-15 04:40:09.000000 selenextra-0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 06:01:36.553660 selenextra-0.8/selenextra/
+-rw-rw-rw-   0        0        0     4609 2023-04-15 06:00:14.000000 selenextra-0.8/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-15 04:40:09.000000 selenextra-0.8/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-15 04:40:09.000000 selenextra-0.8/selenextra/patcher.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:01:36.559644 selenextra-0.8/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-15 06:01:36.000000 selenextra-0.8/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 06:01:36.561638 selenextra-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-15 04:48:37.000000 selenextra-0.8/setup.py
```

### Comparing `selenextra-0.7/LICENSE` & `selenextra-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.7/PKG-INFO` & `selenextra-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.7
+Version: 0.8
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.7/selenextra/__init__.py` & `selenextra-0.8/selenextra/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from .typer import Typer
 from undetected_chromedriver import ChromeOptions
 from seleniumwire.undetected_chromedriver import Chrome
 from selenium.common.exceptions import TimeoutException
 from seleniumwire.request import Request, Response
 from typing import Union, Callable, Any, List, Tuple
 from .patcher import CustomPatcher
 from .exceptions import *
 
+import requests
 import re
 import random as rnd
 import time
-import json
 
 
 class ChromeDriver(Chrome):
     CONNECTION_TIMEOUT = 30
 
     def __init__(self, **kwargs) -> None:
         self.custom_patcher = CustomPatcher(
@@ -25,14 +24,21 @@
 
         self.custom_patcher.auto()
 
         release = self.custom_patcher.fetch_release_number()
         version = release.version[0]
 
         kwargs['driver_executable_path'] = self.custom_patcher.executable_path
+        kwargs['seleniumwire_options'] = {
+            'mitm_http2': False,
+            'proxy': {
+                'no_proxy': 'localhost,127.0.0.1'
+            }
+
+        }
 
         super().__init__(
             version_main=version,
             **kwargs
         )
 
     def get_user_agent(self) -> str:
@@ -40,37 +46,14 @@
 
     def get_cookie_string(self) -> str:
         cookies = self.get_cookies()
         cookies = [f'{item["name"]}={item["value"]}' for item in cookies]
 
         return '; '.join(cookies) + ';'
 
-    def get_browser_ip(self) -> str:
-        self.get('https://httpbin.org/ip')
-
-        try:
-            request = self.wait_for_request(
-                pat='/ip',
-                timeout=self.CONNECTION_TIMEOUT
-            )
-
-            if not request.response.status_code == 200:
-                raise RequestException("Request failed with status code: {}".format(
-                    request.response.status_code))
-        except Exception as e:
-            raise RequestException("Failed to retrieve IP: {}".format(str(e)))
-
-        try:
-            body = request.response.body.decode('utf-8')
-            data = json.loads(body)
-        except:
-            return None
-
-        return data['origin']
-
     def callback_with_timeout(self, callback: Callable[[Tuple], Any], params: tuple, timeout: Union[int, float] = 30) -> Any:
         end_time = time.time() + timeout
 
         while time.time() < end_time:
             result = callback(*params)
 
             if not result:
@@ -124,10 +107,35 @@
                 continue
 
             return callback(request) if callback else request
 
     def find_first_matching_request(self, paths: List[Tuple[str, Callable[[Request], Any]]], timeout: Union[int, float] = 30) -> Any:
         return self.callback_with_timeout(self._find_first_matching_request, (paths, ), timeout)
 
+    def add_proxy(self, proxy: str) -> Tuple[bool, str]:
+        proxy_dict = {}
+        proxy_type = proxy.split(':')[0]
+
+        if proxy_type == 'http':
+            proxy_dict['http'] = proxy
+            proxy_dict['https'] = proxy
+        elif proxy_type == 'https':
+            proxy_dict['http'] = f'{proxy.replace("https", "http")}'
+            proxy_dict['https'] = proxy
+
+        result = (False, None)
+
+        try:
+            resp = requests.get('https://httpbin.org/ip', proxies=proxy_dict)
+            if not resp.status_code == 200:
+                return result
+        except:
+            return result
+
+        self.proxy = proxy_dict
+        data = resp.json()
+
+        return True, data['origin']
+
     def quit(self) -> None:
         super().quit()
         self.custom_patcher = None
```

### Comparing `selenextra-0.7/selenextra/patcher.py` & `selenextra-0.8/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.7/selenextra.egg-info/PKG-INFO` & `selenextra-0.8/selenextra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.7
+Version: 0.8
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.7/setup.py` & `selenextra-0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='0.7',
+    version='0.8',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
         'scipy',
```

