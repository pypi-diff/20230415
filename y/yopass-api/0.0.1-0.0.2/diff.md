# Comparing `tmp/yopass_api-0.0.1.tar.gz` & `tmp/yopass-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopass_api-0.0.1.tar", last modified: Sat Apr 15 19:30:23 2023, max compression
+gzip compressed data, was "yopass-api-0.0.2.tar", last modified: Sat Apr 15 19:48:50 2023, max compression
```

## Comparing `yopass_api-0.0.1.tar` & `yopass-api-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-15 19:30:23.643561 yopass_api-0.0.1/
--rw-rw-r--   0 xstl      (1000) xstl      (1000)     1075 2023-04-15 17:52:02.000000 yopass_api-0.0.1/LICENSE
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      834 2023-04-15 19:30:23.643561 yopass_api-0.0.1/PKG-INFO
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      356 2023-04-15 18:02:41.000000 yopass_api-0.0.1/README.md
-drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-15 19:30:23.631561 yopass_api-0.0.1/package/
--rw-rw-r--   0 xstl      (1000) xstl      (1000)        0 2023-04-10 06:50:19.000000 yopass_api-0.0.1/package/__init__.py
--rw-rw-r--   0 xstl      (1000) xstl      (1000)     5011 2023-04-15 19:26:48.000000 yopass_api-0.0.1/package/main.py
--rw-rw-r--   0 xstl      (1000) xstl      (1000)       38 2023-04-15 19:30:23.647561 yopass_api-0.0.1/setup.cfg
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      888 2023-04-15 19:14:43.000000 yopass_api-0.0.1/setup.py
-drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-15 19:30:23.643561 yopass_api-0.0.1/yopass_api.egg-info/
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      834 2023-04-15 19:30:23.000000 yopass_api-0.0.1/yopass_api.egg-info/PKG-INFO
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      241 2023-04-15 19:30:23.000000 yopass_api-0.0.1/yopass_api.egg-info/SOURCES.txt
--rw-rw-r--   0 xstl      (1000) xstl      (1000)        1 2023-04-15 19:30:23.000000 yopass_api-0.0.1/yopass_api.egg-info/dependency_links.txt
--rw-rw-r--   0 xstl      (1000) xstl      (1000)       72 2023-04-15 19:30:23.000000 yopass_api-0.0.1/yopass_api.egg-info/requires.txt
--rw-rw-r--   0 xstl      (1000) xstl      (1000)        8 2023-04-15 19:30:23.000000 yopass_api-0.0.1/yopass_api.egg-info/top_level.txt
+drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-15 19:48:50.179174 yopass-api-0.0.2/
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)     1075 2023-04-15 19:39:08.000000 yopass-api-0.0.2/LICENSE
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)      844 2023-04-15 19:48:50.183174 yopass-api-0.0.2/PKG-INFO
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)      329 2023-04-15 19:41:03.000000 yopass-api-0.0.2/README.md
+drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-15 19:48:50.171174 yopass-api-0.0.2/package/
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)        0 2023-04-15 19:39:08.000000 yopass-api-0.0.2/package/__init__.py
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)     5011 2023-04-15 19:40:32.000000 yopass-api-0.0.2/package/main.py
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)       38 2023-04-15 19:48:50.191174 yopass-api-0.0.2/setup.cfg
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)      888 2023-04-15 19:48:43.000000 yopass-api-0.0.2/setup.py
+drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-15 19:48:50.179174 yopass-api-0.0.2/yopass_api.egg-info/
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)      844 2023-04-15 19:48:49.000000 yopass-api-0.0.2/yopass_api.egg-info/PKG-INFO
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)      241 2023-04-15 19:48:49.000000 yopass-api-0.0.2/yopass_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)        1 2023-04-15 19:48:49.000000 yopass-api-0.0.2/yopass_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)       72 2023-04-15 19:48:49.000000 yopass-api-0.0.2/yopass_api.egg-info/requires.txt
+-rw-rw-r--   0 xstl      (1000) xstl      (1000)        8 2023-04-15 19:48:49.000000 yopass-api-0.0.2/yopass_api.egg-info/top_level.txt
```

### Comparing `yopass_api-0.0.1/LICENSE` & `yopass-api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yopass_api-0.0.1/PKG-INFO` & `yopass-api-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
-Name: yopass_api
-Version: 0.0.1
+Name: yopass-api
+Version: 0.0.2
 Summary: Module for interacting with Yopass backend
 Home-page: https://github.com/silyashevich/yopass_api
 Author: silyashevich
 Author-email: silyashevich@gmail.com
+License: UNKNOWN
 Keywords: example python
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a module to work with a (the) [Yopass](https://github.com/jhaals/yopass) backend created by [Johan Haals](https://github.com/jhaals).
 The module will allow you to use Yopass in automation projects.
 
 ### Installation
 
-yopass_api requires [python3](https://www.python.org/downloads/) to run.
+yopass-api requires [python3](https://www.python.org/downloads/) to run.
 
-    $ pip install --user yopass_api
+    $ pip install yopass-api
 
 
-License
-----
-
-MIT
```

### Comparing `yopass_api-0.0.1/package/main.py` & `yopass-api-0.0.2/package/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-yopass_api :: store and fetch secrets in Yopass
+yopass-api :: store and fetch secrets in Yopass
 """
 import json
 import re
 import warnings
 from random import SystemRandom
 from string import ascii_letters, digits
 from urllib.parse import urljoin
```

### Comparing `yopass_api-0.0.1/setup.py` & `yopass-api-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(
-    name="yopass_api",
-    version="0.0.1",
+    name="yopass-api",
+    version="0.0.2",
     author="silyashevich",
     author_email="silyashevich@gmail.com",
     description="Module for interacting with Yopass backend",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/silyashevich/yopass_api",
     packages=find_packages(),
```

### Comparing `yopass_api-0.0.1/yopass_api.egg-info/PKG-INFO` & `yopass-api-0.0.2/yopass_api.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: yopass-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Module for interacting with Yopass backend
 Home-page: https://github.com/silyashevich/yopass_api
 Author: silyashevich
 Author-email: silyashevich@gmail.com
+License: UNKNOWN
 Keywords: example python
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a module to work with a (the) [Yopass](https://github.com/jhaals/yopass) backend created by [Johan Haals](https://github.com/jhaals).
 The module will allow you to use Yopass in automation projects.
 
 ### Installation
 
-yopass_api requires [python3](https://www.python.org/downloads/) to run.
+yopass-api requires [python3](https://www.python.org/downloads/) to run.
 
-    $ pip install --user yopass_api
+    $ pip install yopass-api
 
 
-License
-----
-
-MIT
```

