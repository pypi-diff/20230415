# Comparing `tmp/Monzo API-0.2.1.tar.gz` & `tmp/Monzo API-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Monzo API-0.2.1.tar", last modified: Fri Oct 14 17:25:14 2022, max compression
+gzip compressed data, was "Monzo API-0.3.0.tar", last modified: Sat Apr 15 12:35:05 2023, max compression
```

## Comparing `Monzo API-0.2.1.tar` & `Monzo API-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.676074 Monzo API-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-10-14 17:24:56.000000 Monzo API-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.672074 Monzo API-0.2.1/Monzo_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-10-14 17:25:14.000000 Monzo API-0.2.1/Monzo_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-10-14 17:25:14.000000 Monzo API-0.2.1/Monzo_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 17:25:14.000000 Monzo API-0.2.1/Monzo_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-14 17:25:14.000000 Monzo API-0.2.1/Monzo_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-14 17:25:14.000000 Monzo API-0.2.1/Monzo_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-10-14 17:25:14.676074 Monzo API-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-10-14 17:24:56.000000 Monzo API-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.672074 Monzo API-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 17:24:56.000000 Monzo API-0.2.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-10-14 17:24:56.000000 Monzo API-0.2.1/examples/auth_step_01.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-10-14 17:24:56.000000 Monzo API-0.2.1/examples/auth_step_02.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-14 17:24:56.000000 Monzo API-0.2.1/examples/create_feed_item.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-10-14 17:24:56.000000 Monzo API-0.2.1/examples/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-10-14 17:24:56.000000 Monzo API-0.2.1/examples/get_whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.676074 Monzo API-0.2.1/monzo/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10071 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.676074 Monzo API-0.2.1/monzo/endpoints/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     5665 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/balance.py
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/feed_item.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/monzo.py
--rw-r--r--   0 runner    (1001) docker     (121)     7729 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/pot.py
--rw-r--r--   0 runner    (1001) docker     (121)    12275 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/receipt.py
--rw-r--r--   0 runner    (1001) docker     (121)    15476 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3450 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/endpoints/whoami.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.676074 Monzo API-0.2.1/monzo/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/handlers/echo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/handlers/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/handlers/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6669 2022-10-14 17:24:56.000000 Monzo API-0.2.1/monzo/httpio.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-14 17:24:56.000000 Monzo API-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-10-14 17:25:14.676074 Monzo API-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.676074 Monzo API-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 17:24:56.000000 Monzo API-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-10-14 17:24:56.000000 Monzo API-0.2.1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.676074 Monzo API-0.2.1/tests/mock_payloads/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 17:24:56.000000 Monzo API-0.2.1/tests/mock_payloads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 17:25:14.676074 Monzo API-0.2.1/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 17:24:56.000000 Monzo API-0.2.1/tests/mock_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-10-14 17:24:56.000000 Monzo API-0.2.1/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)    19621 2022-10-14 17:24:56.000000 Monzo API-0.2.1/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)    11779 2022-10-14 17:24:56.000000 Monzo API-0.2.1/tests/test_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.324282 Monzo API-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-15 12:34:50.000000 Monzo API-0.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.320282 Monzo API-0.3.0/Monzo_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-15 12:35:05.000000 Monzo API-0.3.0/Monzo_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-15 12:35:05.000000 Monzo API-0.3.0/Monzo_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 12:35:05.000000 Monzo API-0.3.0/Monzo_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 12:35:05.000000 Monzo API-0.3.0/Monzo_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 12:35:05.000000 Monzo API-0.3.0/Monzo_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-15 12:35:05.324282 Monzo API-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 12:34:50.000000 Monzo API-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.320282 Monzo API-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:34:50.000000 Monzo API-0.3.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-15 12:34:50.000000 Monzo API-0.3.0/examples/auth_step_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 12:34:50.000000 Monzo API-0.3.0/examples/auth_step_02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-15 12:34:50.000000 Monzo API-0.3.0/examples/create_feed_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-15 12:34:50.000000 Monzo API-0.3.0/examples/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-15 12:34:50.000000 Monzo API-0.3.0/examples/get_whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.324282 Monzo API-0.3.0/monzo/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.324282 Monzo API-0.3.0/monzo/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/feed_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/monzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/endpoints/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.324282 Monzo API-0.3.0/monzo/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/handlers/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/handlers/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/handlers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-15 12:34:50.000000 Monzo API-0.3.0/monzo/httpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 12:34:50.000000 Monzo API-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-15 12:35:05.324282 Monzo API-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.324282 Monzo API-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:34:50.000000 Monzo API-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-15 12:34:50.000000 Monzo API-0.3.0/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.324282 Monzo API-0.3.0/tests/mock_payloads/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:34:50.000000 Monzo API-0.3.0/tests/mock_payloads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:35:05.324282 Monzo API-0.3.0/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:34:50.000000 Monzo API-0.3.0/tests/mock_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-15 12:34:50.000000 Monzo API-0.3.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-15 12:34:50.000000 Monzo API-0.3.0/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-15 12:34:50.000000 Monzo API-0.3.0/tests/test_payload.py
```

### Comparing `Monzo API-0.2.1/LICENSE` & `Monzo API-0.3.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017 AlexaBible.com (Peter McDonald)
+Copyright (c) 2023 (Peter McDonald)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `Monzo API-0.2.1/Monzo_API.egg-info/PKG-INFO` & `Monzo API-0.3.0/Monzo_API.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: Monzo-API
-Version: 0.2.1
+Version: 0.3.0
 Summary: Package to interact with the API provided by Monzo bank
 Home-page: https://github.com/petermcd/monzo-api
 Author: Peter McDonald
 Author-email: git@petermcdonald.co.uk
 Project-URL: Bug Tracker, https://github.com/petermcd/monzo-api/issues
 Project-URL: Documentation, https://monzo-api.readthedocs.io
 Project-URL: Source, https://github.com/petermcd/monzo-api
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: viewer
 License-File: LICENSE
```

### Comparing `Monzo API-0.2.1/Monzo_API.egg-info/SOURCES.txt` & `Monzo API-0.3.0/Monzo_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/PKG-INFO` & `Monzo API-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: Monzo API
-Version: 0.2.1
+Version: 0.3.0
 Summary: Package to interact with the API provided by Monzo bank
 Home-page: https://github.com/petermcd/monzo-api
 Author: Peter McDonald
 Author-email: git@petermcdonald.co.uk
 Project-URL: Bug Tracker, https://github.com/petermcd/monzo-api/issues
 Project-URL: Documentation, https://monzo-api.readthedocs.io
 Project-URL: Source, https://github.com/petermcd/monzo-api
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: viewer
 License-File: LICENSE
```

### Comparing `Monzo API-0.2.1/README.rst` & `Monzo API-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/examples/auth_step_02.py` & `Monzo API-0.3.0/examples/auth_step_02.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/examples/create_feed_item.py` & `Monzo API-0.3.0/examples/create_feed_item.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/examples/get_accounts.py` & `Monzo API-0.3.0/examples/get_accounts.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/examples/get_whoami.py` & `Monzo API-0.3.0/examples/get_whoami.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/authentication.py` & `Monzo API-0.3.0/monzo/authentication.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/attachment.py` & `Monzo API-0.3.0/monzo/endpoints/attachment.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/balance.py` & `Monzo API-0.3.0/monzo/endpoints/balance.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/feed_item.py` & `Monzo API-0.3.0/monzo/endpoints/feed_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def __init__(
         self,
         auth: Authentication,
         account_id: str,
         feed_type: str,
         params: Dict[str, str],
-        url: str = None,
+        url: str = '',
     ):
         """
         Initialize FeedItem.
 
         Args:
             auth: Monzo authentication object
             account_id: ID for the account to create the feed item for
@@ -108,15 +108,15 @@
     @classmethod
     def create(
         cls,
         auth: Authentication,
         account_id: str,
         feed_type: str,
         params: Dict[str, str],
-        url: str = None
+        url: str = ''
     ) -> FeedItem:
         """
         Create a new feed item.
 
         Args:
             auth: Monzo authentication object
             account_id: ID for the account to create the feed item for
```

### Comparing `Monzo API-0.2.1/monzo/endpoints/monzo.py` & `Monzo API-0.3.0/monzo/endpoints/monzo.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/pot.py` & `Monzo API-0.3.0/monzo/endpoints/pot.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/receipt.py` & `Monzo API-0.3.0/monzo/endpoints/receipt.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/transaction.py` & `Monzo API-0.3.0/monzo/endpoints/transaction.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/webhooks.py` & `Monzo API-0.3.0/monzo/endpoints/webhooks.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/endpoints/whoami.py` & `Monzo API-0.3.0/monzo/endpoints/whoami.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/exceptions.py` & `Monzo API-0.3.0/monzo/exceptions.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/handlers/echo.py` & `Monzo API-0.3.0/monzo/handlers/echo.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/handlers/filesystem.py` & `Monzo API-0.3.0/monzo/handlers/filesystem.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/handlers/storage.py` & `Monzo API-0.3.0/monzo/handlers/storage.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/helpers.py` & `Monzo API-0.3.0/monzo/helpers.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/monzo/httpio.py` & `Monzo API-0.3.0/monzo/httpio.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/setup.cfg` & `Monzo API-0.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [metadata]
 name = Monzo API
-version = 0.2.1
+version = 0.3.0
 author = Peter McDonald
 author_email = git@petermcdonald.co.uk
 description = Package to interact with the API provided by Monzo bank
 long_description = file: README.rst
 long_description_content_type = text/markdown
 url = https://github.com/petermcd/monzo-api
 project_urls = 
 	Bug Tracker = https://github.com/petermcd/monzo-api/issues
 	Documentation = https://monzo-api.readthedocs.io
 	Source = https://github.com/petermcd/monzo-api
 classifiers = 
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Intended Audience :: Developers
 	Topic :: Office/Business :: Financial
 
 [options]
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.extras_require]
-test = flake8; isort; mypy;
+test = flake8; isort; mypy; pytest;
 build = wheel; build;
 docs = sphinx; sphinx_rtd_theme;
 viewer = jinja2;
 
 [options.package_data]
 monzo.viewer.html = *.html
```

### Comparing `Monzo API-0.2.1/tests/helpers.py` & `Monzo API-0.3.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/tests/test_authentication.py` & `Monzo API-0.3.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/tests/test_endpoints.py` & `Monzo API-0.3.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `Monzo API-0.2.1/tests/test_payload.py` & `Monzo API-0.3.0/tests/test_payload.py`

 * *Files identical despite different names*

