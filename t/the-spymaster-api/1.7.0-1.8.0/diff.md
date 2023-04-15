# Comparing `tmp/the-spymaster-api-1.7.0.tar.gz` & `tmp/the-spymaster-api-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-spymaster-api-1.7.0.tar", last modified: Sat Apr  8 20:45:04 2023, max compression
+gzip compressed data, was "the-spymaster-api-1.8.0.tar", last modified: Sat Apr 15 13:01:38 2023, max compression
```

## Comparing `the-spymaster-api-1.7.0.tar` & `the-spymaster-api-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:45:04.861973 the-spymaster-api-1.7.0/
--rw-rw-r--   0 akali     (1000) akali     (1000)      306 2023-04-08 20:45:04.861973 the-spymaster-api-1.7.0/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 20:45:04.865973 the-spymaster-api-1.7.0/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      559 2023-04-08 20:38:17.000000 the-spymaster-api-1.7.0/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:45:04.861973 the-spymaster-api-1.7.0/the_spymaster_api/
--rw-rw-r--   0 akali     (1000) akali     (1000)       47 2022-09-25 13:05:12.000000 the-spymaster-api-1.7.0/the_spymaster_api/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2227 2023-01-27 15:56:25.000000 the-spymaster-api-1.7.0/the_spymaster_api/client.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:45:04.861973 the-spymaster-api-1.7.0/the_spymaster_api/structs/
--rw-rw-r--   0 akali     (1000) akali     (1000)       63 2022-09-25 13:05:12.000000 the-spymaster-api-1.7.0/the_spymaster_api/structs/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      789 2023-04-08 20:38:47.000000 the-spymaster-api-1.7.0/the_spymaster_api/structs/errors.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      952 2022-09-27 09:51:02.000000 the-spymaster-api-1.7.0/the_spymaster_api/structs/request.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1205 2023-04-08 20:39:36.000000 the-spymaster-api-1.7.0/the_spymaster_api/structs/response.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:45:04.861973 the-spymaster-api-1.7.0/the_spymaster_api.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      306 2023-04-08 20:45:04.000000 the-spymaster-api-1.7.0/the_spymaster_api.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      429 2023-04-08 20:45:04.000000 the-spymaster-api-1.7.0/the_spymaster_api.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 20:45:04.000000 the-spymaster-api-1.7.0/the_spymaster_api.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      104 2023-04-08 20:45:04.000000 the-spymaster-api-1.7.0/the_spymaster_api.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       18 2023-04-08 20:45:04.000000 the-spymaster-api-1.7.0/the_spymaster_api.egg-info/top_level.txt
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 13:01:38.541540 the-spymaster-api-1.8.0/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      306 2023-04-15 13:01:38.541540 the-spymaster-api-1.8.0/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-15 13:01:38.541540 the-spymaster-api-1.8.0/setup.cfg
+-rw-rw-r--   0 akali     (1000) akali     (1000)      557 2023-04-15 12:57:36.000000 the-spymaster-api-1.8.0/setup.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 13:01:38.537539 the-spymaster-api-1.8.0/the_spymaster_api/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       47 2022-09-25 13:05:12.000000 the-spymaster-api-1.8.0/the_spymaster_api/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2227 2023-01-27 15:56:25.000000 the-spymaster-api-1.8.0/the_spymaster_api/client.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 13:01:38.541540 the-spymaster-api-1.8.0/the_spymaster_api/structs/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       63 2022-09-25 13:05:12.000000 the-spymaster-api-1.8.0/the_spymaster_api/structs/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      789 2023-04-08 20:38:47.000000 the-spymaster-api-1.8.0/the_spymaster_api/structs/errors.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      952 2022-09-27 09:51:02.000000 the-spymaster-api-1.8.0/the_spymaster_api/structs/request.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1205 2023-04-08 20:39:36.000000 the-spymaster-api-1.8.0/the_spymaster_api/structs/response.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 13:01:38.541540 the-spymaster-api-1.8.0/the_spymaster_api.egg-info/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      306 2023-04-15 13:01:38.000000 the-spymaster-api-1.8.0/the_spymaster_api.egg-info/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      429 2023-04-15 13:01:38.000000 the-spymaster-api-1.8.0/the_spymaster_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-15 13:01:38.000000 the-spymaster-api-1.8.0/the_spymaster_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      102 2023-04-15 13:01:38.000000 the-spymaster-api-1.8.0/the_spymaster_api.egg-info/requires.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       18 2023-04-15 13:01:38.000000 the-spymaster-api-1.8.0/the_spymaster_api.egg-info/top_level.txt
```

### Comparing `the-spymaster-api-1.7.0/setup.py` & `the-spymaster-api-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name="the-spymaster-api",
-    version="1.7.0",
+    version="1.8.0",
     description="Python client implementation for The Spymaster HTTP backend.",
     author="Asaf Kali",
     author_email="akali93@gmail.com",
     url="https://github.com/asaf-kali/the-spymaster-backend",
     packages=find_packages(),
     install_requires=[
         "codenames~=2.0",
         "the_spymaster_util~=3.0",
-        "the_spymaster_solvers_client>=1.3.1",
+        "the_spymaster_solvers_client~=1.7",
         "pydantic~=1.9",
         "requests~=2.28",
     ],
     include_package_data=True,
 )
```

### Comparing `the-spymaster-api-1.7.0/the_spymaster_api/client.py` & `the-spymaster-api-1.8.0/the_spymaster_api/client.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-api-1.7.0/the_spymaster_api/structs/errors.py` & `the-spymaster-api-1.8.0/the_spymaster_api/structs/errors.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-api-1.7.0/the_spymaster_api/structs/request.py` & `the-spymaster-api-1.8.0/the_spymaster_api/structs/request.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-api-1.7.0/the_spymaster_api/structs/response.py` & `the-spymaster-api-1.8.0/the_spymaster_api/structs/response.py`

 * *Files identical despite different names*

