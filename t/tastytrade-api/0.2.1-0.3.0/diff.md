# Comparing `tmp/tastytrade-api-0.2.1.tar.gz` & `tmp/tastytrade-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-api-0.2.1.tar", last modified: Sat Apr 15 08:23:06 2023, max compression
+gzip compressed data, was "tastytrade-api-0.3.0.tar", last modified: Sat Apr 15 14:07:49 2023, max compression
```

## Comparing `tastytrade-api-0.2.1.tar` & `tastytrade-api-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.830801 tastytrade-api-0.2.1/tastytrade_api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.830801 tastytrade-api-0.2.1/tastytrade_api/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tastytrade_api/streamer/streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.830801 tastytrade-api-0.2.1/tastytrade_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 08:23:06.000000 tastytrade-api-0.2.1/tastytrade_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:23:06.834801 tastytrade-api-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-15 08:22:46.000000 tastytrade-api-0.2.1/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:49.150472 tastytrade-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 14:07:49.150472 tastytrade-api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 14:07:49.150472 tastytrade-api-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:49.146473 tastytrade-api-0.3.0/tastytrade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/tastytrade_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/tastytrade_api/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:49.150472 tastytrade-api-0.3.0/tastytrade_api/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/tastytrade_api/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/tastytrade_api/streamer/streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:49.150472 tastytrade-api-0.3.0/tastytrade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 14:07:49.000000 tastytrade-api-0.3.0/tastytrade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-15 14:07:49.000000 tastytrade-api-0.3.0/tastytrade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:07:49.000000 tastytrade-api-0.3.0/tastytrade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 14:07:49.000000 tastytrade-api-0.3.0/tastytrade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 14:07:49.000000 tastytrade-api-0.3.0/tastytrade_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:49.150472 tastytrade-api-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-15 14:07:27.000000 tastytrade-api-0.3.0/tests/test_authentication.py
```

### Comparing `tastytrade-api-0.2.1/PKG-INFO` & `tastytrade-api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python client for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.2.1/README.md` & `tastytrade-api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.2.1/setup.py` & `tastytrade-api-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tastytrade-api",
-    version="0.2.1",
+    version="0.3.0",
     author="Peter Oroszvari",
     author_email="peter@oroszvari.hu",
     description="A Python client for the Tastytrade API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peter-oroszvari/tastytrade-api",
     packages=find_packages(),
```

### Comparing `tastytrade-api-0.2.1/tastytrade_api/authentication.py` & `tastytrade-api-0.3.0/tastytrade_api/authentication.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-0.2.1/tastytrade_api/streamer/streamer.py` & `tastytrade-api-0.3.0/tastytrade_api/streamer/streamer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,8 +151,8 @@
 
 if streamer.wait_for_connection():
     streamer.start_heartbeat()
     streamer.public_watchlists_subscribe()
     streamer.quote_alerts_subscribe()
     while streamer.ws.sock and streamer.ws.sock.connected:
         time.sleep(1)
-'''
+'''
```

### Comparing `tastytrade-api-0.2.1/tastytrade_api.egg-info/PKG-INFO` & `tastytrade-api-0.3.0/tastytrade_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python client for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-0.2.1/tests/test_authentication.py` & `tastytrade-api-0.3.0/tests/test_authentication.py`

 * *Files identical despite different names*

