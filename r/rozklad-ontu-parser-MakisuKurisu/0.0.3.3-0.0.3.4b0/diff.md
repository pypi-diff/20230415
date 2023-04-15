# Comparing `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.3.tar.gz` & `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.4b0.tar.gz`

## Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3.tar` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/requirements.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/run_lint.bat
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/run_lint.sh
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/example.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/base.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/dataclasses.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/enums.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/parser.py
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/sender.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/LICENSE
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/readme.md
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/run_lint.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/run_lint.sh
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/example.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/base.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/dataclasses.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/enums.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/parser.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/sender.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/readme.md
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/PKG-INFO
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/.github/ISSUE_TEMPLATE/feature_request.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/.github/workflows/pylint.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/.github/workflows/python-publish.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/example.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/example.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/base.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/base.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/dataclasses.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/dataclasses.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/enums.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/enums.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/parser.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/parser.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/ontu_parser/classes/sender.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/sender.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Module for sending operations"""
 import time
 from datetime import datetime
 import requests
 from selenium import webdriver
 from selenium.webdriver import FirefoxOptions
+from selenium.webdriver.common.proxy import Proxy, ProxyType
 
 from .base import BaseClass
 from .enums import RequestsEnum
 
 class TTLValue(BaseClass):
     """Describes value with some time to live (like authorization token)"""
-    _ttl: int = 1800  # Time To Live (in seconds)
+    _ttl: int = 3600  # Time To Live (in seconds)
     _value: object = None
 
     issued_at: datetime = datetime.min
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.issued_at = datetime.now()
@@ -56,43 +57,14 @@
         return cookie
 
     def get_cookie(self):
         """Get's cookie value and notbot (used to verify that request is made by human)"""
         # link = self.sender.link
         notbot = self.sender.notbot.value
 
-        # php_key = 'PHPSESSID'
-
-        # i = 0
-        # phpsessid = notbot.get(php_key, None)
-        # while True:
-        #     if phpsessid:
-        #         break
-
-        #     print("Making request to get PHPSESSID and pow-result")
-        #     response = requests.get(
-        #         link,
-        #         cookies=notbot,
-        #         timeout=30
-        #     )
-        #     phpsessid = response.cookies.get(php_key) or phpsessid
-        #     if not phpsessid:
-        #         if i > 6:
-        #             break
-        #         print(f"Sleeping for {2 ** i} seconds")
-        #         time.sleep(2 ** i)
-        #         i += 1
-        #     else:
-        #         break
-
-        # new_cookies = notbot.copy()
-        # if not new_cookies.get(php_key, None):
-        #     new_cookies.update(
-        #         {php_key: phpsessid}
-        #     )
         return self.set_value(
             notbot
         )
 
 
 class NotBot(TTLValue):
     """Describes NotBot value for requests"""
@@ -144,18 +116,32 @@
                 if cookie['name'] == 'PHPSESSID':
                     phpsesid = cookie['value']
         return (notbot, pow_result, phpsesid)
 
     def get_notbot(self):
         """Gets notbot by making webdriver request (emulates JS)"""
         options = self._browser_kwargs.pop('options', None)
+        desired_capabilities = self._browser_kwargs.pop('desired_capabilities', None)
         if not options:
             options = FirefoxOptions()
             options.add_argument("--headless")
-        driver = webdriver.Firefox(options=options, **self._browser_kwargs)
+        if not desired_capabilities:
+            print("Using local proxy at port 8888 (if available)")
+            proxy = Proxy()
+            proxy.proxy_type = ProxyType.MANUAL
+            proxy.http_proxy = "127.0.0.1:8888"
+            proxy.ssl_proxy = "127.0.0.1:8888"
+            desired_capabilities = webdriver.DesiredCapabilities.FIREFOX
+            proxy.add_to_capabilities(desired_capabilities)
+
+        driver = webdriver.Firefox(
+            options=options,
+            desired_capabilities=desired_capabilities,
+            **self._browser_kwargs
+        )
         i = 0
         while True:
             print("Making request to get cookies")
             notbot, pow_result, phpsesid = self.__make_request(
                 driver=driver
             )
             if all([notbot, pow_result, phpsesid]):
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/LICENSE` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/pyproject.toml` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rozklad_ontu_parser_MakisuKurisu"
-version = "0.0.3.3"
+version = "0.0.3.4b"
 authors = [
   {  name="Pavlo Pohorieltsev", email="667strets@gmail.com"  },
 ]
 description = "Package for parsing data from rozklad.ontu.edu.ua"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/readme.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/readme.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.3/PKG-INFO` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozklad_ontu_parser_MakisuKurisu
-Version: 0.0.3.3
+Version: 0.0.3.4b0
 Summary: Package for parsing data from rozklad.ontu.edu.ua
 Project-URL: Homepage, https://github.com/makisukurisu/rozklad-ontu-parser
 Project-URL: Bug Tracker, https://github.com/makisukurisu/rozklad-ontu-parser/issues
 Author-email: Pavlo Pohorieltsev <667strets@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

