# Comparing `tmp/tastytrade-api-0.1.1.tar.gz` & `tmp/tastytrade-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-api-0.1.1.tar", last modified: Fri Apr 14 19:30:34 2023, max compression
+gzip compressed data, was "tastytrade-api-0.2.1.tar", last modified: Sat Apr 15 08:23:06 2023, max compression
```

## Comparing `tastytrade-api-0.1.1.tar` & `tastytrade-api-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 peteroroszvari   (501) staff       (20)        0 2023-04-14 19:30:34.917638 tastytrade-api-0.1.1/
--rw-r--r--   0 peteroroszvari   (501) staff       (20)        0 2023-04-14 18:57:56.000000 tastytrade-api-0.1.1/LICENSE
--rw-r--r--   0 peteroroszvari   (501) staff       (20)     2003 2023-04-14 19:30:34.916946 tastytrade-api-0.1.1/PKG-INFO
--rw-r--r--   0 peteroroszvari   (501) staff       (20)     1255 2023-04-14 19:03:18.000000 tastytrade-api-0.1.1/README.md
--rw-r--r--   0 peteroroszvari   (501) staff       (20)       38 2023-04-14 19:30:34.917866 tastytrade-api-0.1.1/setup.cfg
--rw-r--r--   0 peteroroszvari   (501) staff       (20)     1031 2023-04-14 19:27:32.000000 tastytrade-api-0.1.1/setup.py
-drwxr-xr-x   0 peteroroszvari   (501) staff       (20)        0 2023-04-14 19:30:34.912383 tastytrade-api-0.1.1/tastytrade_api/
--rw-r--r--   0 peteroroszvari   (501) staff       (20)        1 2023-04-14 16:45:21.000000 tastytrade-api-0.1.1/tastytrade_api/__init__.py
--rw-r--r--   0 peteroroszvari   (501) staff       (20)     2854 2023-04-14 19:24:40.000000 tastytrade-api-0.1.1/tastytrade_api/authentication.py
-drwxr-xr-x   0 peteroroszvari   (501) staff       (20)        0 2023-04-14 19:30:34.914912 tastytrade-api-0.1.1/tastytrade_api.egg-info/
--rw-r--r--   0 peteroroszvari   (501) staff       (20)     2003 2023-04-14 19:30:34.000000 tastytrade-api-0.1.1/tastytrade_api.egg-info/PKG-INFO
--rw-r--r--   0 peteroroszvari   (501) staff       (20)      322 2023-04-14 19:30:34.000000 tastytrade-api-0.1.1/tastytrade_api.egg-info/SOURCES.txt
--rw-r--r--   0 peteroroszvari   (501) staff       (20)        1 2023-04-14 19:30:34.000000 tastytrade-api-0.1.1/tastytrade_api.egg-info/dependency_links.txt
--rw-r--r--   0 peteroroszvari   (501) staff       (20)        9 2023-04-14 19:30:34.000000 tastytrade-api-0.1.1/tastytrade_api.egg-info/requires.txt
--rw-r--r--   0 peteroroszvari   (501) staff       (20)       21 2023-04-14 19:30:34.000000 tastytrade-api-0.1.1/tastytrade_api.egg-info/top_level.txt
-drwxr-xr-x   0 peteroroszvari   (501) staff       (20)        0 2023-04-14 19:30:34.915562 tastytrade-api-0.1.1/tests/
--rw-r--r--   0 peteroroszvari   (501) staff       (20)        0 2023-04-14 16:46:06.000000 tastytrade-api-0.1.1/tests/__init__.py
--rw-r--r--   0 peteroroszvari   (501) staff       (20)     4382 2023-04-14 18:20:58.000000 tastytrade-api-0.1.1/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.830801 tastytrade-api-0.2.1/tastytrade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.830801 tastytrade-api-0.2.1/tastytrade_api/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/streamer/streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.830801 tastytrade-api-0.2.1/tastytrade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tests/test_authentication.py
```

### Comparing `tastytrade-api-0.1.1/PKG-INFO` & `tastytrade-api-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.1.1
+Version: 0.2.1
 Summary: A Python client for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tastytrade API
 
+_The Tastytrade API, which my Python module relies on, is currently in beta and not yet publicly accessible. As a result, you may not be able to test the functionality of this module until the API becomes available for public use._
+
 A Python client for the Tastytrade API, providing convenient access to Tastytrade's REST API for trading, account management, and more.
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
```

### Comparing `tastytrade-api-0.1.1/setup.py` & `tastytrade-api-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tastytrade-api",
-    version="0.1.1",
+    version="0.2.1",
     author="Peter Oroszvari",
     author_email="peter@oroszvari.hu",
     description="A Python client for the Tastytrade API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peter-oroszvari/tastytrade-api",
     packages=find_packages(),
```

### Comparing `tastytrade-api-0.1.1/tastytrade_api/authentication.py` & `tastytrade-api-0.2.1/tastytrade_api/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         response = requests.post(url, headers=headers)
 
         if response.status_code == 200:
             data = response.json()
             return data
         else:
             print(f"Error: {response.status_code}")
+            print("Response text:", response.text)
+
             return None
 
     def destroy_session(self) -> bool:
         """
         Destroys the current session, logging the user out.
 
         Returns:
```

### Comparing `tastytrade-api-0.1.1/tastytrade_api.egg-info/PKG-INFO` & `tastytrade-api-0.2.1/tastytrade_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.1.1
+Version: 0.2.1
 Summary: A Python client for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tastytrade API
 
+_The Tastytrade API, which my Python module relies on, is currently in beta and not yet publicly accessible. As a result, you may not be able to test the functionality of this module until the API becomes available for public use._
+
 A Python client for the Tastytrade API, providing convenient access to Tastytrade's REST API for trading, account management, and more.
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
```

### Comparing `tastytrade-api-0.1.1/tests/test_authentication.py` & `tastytrade-api-0.2.1/tests/test_authentication.py`

 * *Files identical despite different names*

