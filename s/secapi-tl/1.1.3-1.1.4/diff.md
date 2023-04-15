# Comparing `tmp/secapi-tl-1.1.3.tar.gz` & `tmp/secapi-tl-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.3.tar", last modified: Fri Apr 14 17:56:47 2023, max compression
+gzip compressed data, was "secapi-tl-1.1.4.tar", last modified: Sat Apr 15 10:58:59 2023, max compression
```

## Comparing `secapi-tl-1.1.3.tar` & `secapi-tl-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 17:56:47.018238 secapi-tl-1.1.3/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.3/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 17:56:47.018238 secapi-tl-1.1.3/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.3/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-14 17:56:34.000000 secapi-tl-1.1.3/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-14 17:56:47.018238 secapi-tl-1.1.3/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 17:56:47.018238 secapi-tl-1.1.3/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 17:56:47.018238 secapi-tl-1.1.3/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.3/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6025 2023-04-08 12:35:48.000000 secapi-tl-1.1.3/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-08 12:35:48.000000 secapi-tl-1.1.3/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.3/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1125 2023-04-14 17:56:34.000000 secapi-tl-1.1.3/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 17:56:47.018238 secapi-tl-1.1.3/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 17:56:47.000000 secapi-tl-1.1.3/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-14 17:56:47.000000 secapi-tl-1.1.3/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-14 17:56:47.000000 secapi-tl-1.1.3/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-14 17:56:47.000000 secapi-tl-1.1.3/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-14 17:56:47.000000 secapi-tl-1.1.3/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 10:58:59.132494 secapi-tl-1.1.4/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.4/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-15 10:58:59.132494 secapi-tl-1.1.4/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.4/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-15 10:57:37.000000 secapi-tl-1.1.4/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-15 10:58:59.132494 secapi-tl-1.1.4/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 10:58:59.132494 secapi-tl-1.1.4/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 10:58:59.132494 secapi-tl-1.1.4/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.4/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6025 2023-04-08 12:35:48.000000 secapi-tl-1.1.4/src/secapi_tl/filing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-08 12:35:48.000000 secapi-tl-1.1.4/src/secapi_tl/filing_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.4/src/secapi_tl/key_mapper.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1385 2023-04-15 10:41:21.000000 secapi-tl-1.1.4/src/secapi_tl/request.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 10:58:59.132494 secapi-tl-1.1.4/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-15 10:58:59.000000 secapi-tl-1.1.4/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-15 10:58:59.000000 secapi-tl-1.1.4/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-15 10:58:59.000000 secapi-tl-1.1.4/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-15 10:58:59.000000 secapi-tl-1.1.4/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-15 10:58:59.000000 secapi-tl-1.1.4/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.3/LICENSE` & `secapi-tl-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.3/PKG-INFO` & `secapi-tl-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.3
+Version: 1.1.4
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `secapi-tl-1.1.3/README.md` & `secapi-tl-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.3/src/secapi_tl/filing.py` & `secapi-tl-1.1.4/src/secapi_tl/filing.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.3/src/secapi_tl/filing_query.py` & `secapi-tl-1.1.4/src/secapi_tl/filing_query.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.3/src/secapi_tl/key_mapper.py` & `secapi-tl-1.1.4/src/secapi_tl/key_mapper.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.3/src/secapi_tl.egg-info/PKG-INFO` & `secapi-tl-1.1.4/src/secapi_tl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.3
+Version: 1.1.4
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

