# Comparing `tmp/async_etcd3gw-0.1.tar.gz` & `tmp/async_etcd3gw-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_etcd3gw-0.1.tar", last modified: Fri Apr 14 22:07:12 2023, max compression
+gzip compressed data, was "async_etcd3gw-0.2.tar", last modified: Fri Apr 14 23:00:22 2023, max compression
```

## Comparing `async_etcd3gw-0.1.tar` & `async_etcd3gw-0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 andreax   (1000) andreax   (1000)        0 2023-04-14 22:07:12.411753 async_etcd3gw-0.1/
--rw-rw-r--   0 andreax   (1000) andreax   (1000)    11357 2023-04-14 21:46:18.000000 async_etcd3gw-0.1/LICENSE
--rw-rw-r--   0 andreax   (1000) andreax   (1000)     1000 2023-04-14 22:07:12.411753 async_etcd3gw-0.1/PKG-INFO
--rw-rw-r--   0 andreax   (1000) andreax   (1000)     1214 2023-04-14 21:49:45.000000 async_etcd3gw-0.1/README.md
-drwxrwxr-x   0 andreax   (1000) andreax   (1000)        0 2023-04-14 22:07:12.411753 async_etcd3gw-0.1/async_etcd3gw/
--rw-rw-r--   0 andreax   (1000) andreax   (1000)      946 2023-04-14 21:35:23.000000 async_etcd3gw-0.1/async_etcd3gw/__init__.py
--rw-r--r--   0 andreax   (1000) andreax   (1000)    15539 2023-04-14 21:34:19.000000 async_etcd3gw-0.1/async_etcd3gw/async_client.py
--rw-r--r--   0 andreax   (1000) andreax   (1000)     3034 2023-04-14 21:34:08.000000 async_etcd3gw-0.1/async_etcd3gw/async_lease.py
--rw-r--r--   0 andreax   (1000) andreax   (1000)     3460 2023-04-14 21:33:55.000000 async_etcd3gw-0.1/async_etcd3gw/async_lock.py
--rw-rw-r--   0 andreax   (1000) andreax   (1000)     2744 2023-04-14 21:33:45.000000 async_etcd3gw-0.1/async_etcd3gw/async_watch.py
--rw-r--r--   0 andreax   (1000) andreax   (1000)     1527 2023-04-14 21:33:27.000000 async_etcd3gw-0.1/async_etcd3gw/exceptions.py
--rw-r--r--   0 andreax   (1000) andreax   (1000)     1765 2023-04-14 21:35:59.000000 async_etcd3gw-0.1/async_etcd3gw/utils.py
-drwxrwxr-x   0 andreax   (1000) andreax   (1000)        0 2023-04-14 22:07:12.411753 async_etcd3gw-0.1/async_etcd3gw.egg-info/
--rw-rw-r--   0 andreax   (1000) andreax   (1000)     1000 2023-04-14 22:07:12.000000 async_etcd3gw-0.1/async_etcd3gw.egg-info/PKG-INFO
--rw-rw-r--   0 andreax   (1000) andreax   (1000)      509 2023-04-14 22:07:12.000000 async_etcd3gw-0.1/async_etcd3gw.egg-info/SOURCES.txt
--rw-rw-r--   0 andreax   (1000) andreax   (1000)        1 2023-04-14 22:07:12.000000 async_etcd3gw-0.1/async_etcd3gw.egg-info/dependency_links.txt
--rw-rw-r--   0 andreax   (1000) andreax   (1000)       15 2023-04-14 22:07:12.000000 async_etcd3gw-0.1/async_etcd3gw.egg-info/requires.txt
--rw-rw-r--   0 andreax   (1000) andreax   (1000)       14 2023-04-14 22:07:12.000000 async_etcd3gw-0.1/async_etcd3gw.egg-info/top_level.txt
--rw-rw-r--   0 andreax   (1000) andreax   (1000)        1 2023-04-14 22:07:12.000000 async_etcd3gw-0.1/async_etcd3gw.egg-info/zip-safe
--rw-rw-r--   0 andreax   (1000) andreax   (1000)      384 2023-04-14 21:59:00.000000 async_etcd3gw-0.1/pyproject.toml
--rw-rw-r--   0 andreax   (1000) andreax   (1000)     1289 2023-04-14 22:07:12.415753 async_etcd3gw-0.1/setup.cfg
--rw-rw-r--   0 andreax   (1000) andreax   (1000)       91 2023-04-14 14:22:15.000000 async_etcd3gw-0.1/setup.py
-drwxrwxr-x   0 andreax   (1000) andreax   (1000)        0 2023-04-14 22:07:12.411753 async_etcd3gw-0.1/tests/
--rw-rw-r--   0 andreax   (1000) andreax   (1000)    13000 2023-04-14 22:00:52.000000 async_etcd3gw-0.1/tests/test_async_etcd3gw.py
--rw-rw-r--   0 andreax   (1000) andreax   (1000)     1390 2023-04-14 14:40:39.000000 async_etcd3gw-0.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/async_etcd3gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/async_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/async_etcd3gw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/async_etcd3gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:00:22.000000 async_etcd3gw-0.2/async_etcd3gw.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:00:22.238322 async_etcd3gw-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/tests/test_async_etcd3gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-14 22:59:59.000000 async_etcd3gw-0.2/tests/test_client.py
```

### Comparing `async_etcd3gw-0.1/LICENSE` & `async_etcd3gw-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/README.md` & `async_etcd3gw-0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-# async_etcd3gw
+# async-etcd3gw
 An async etcd3 grpc-gateway v3 API Python client, derived from [etcd3gw](https://opendev.org/openstack/etcd3gw).
 
+[![Build Status](https://github.com//DLBD-Department/async_etcd3gw/workflows/Tests/badge.svg)](https://github.com//DLBD-Department/async_etcd3gw/actions)
+[![PyPI version](https://badge.fury.io/py/async-etcd3gw.svg)](https://badge.fury.io/py/async-etcd3gw)
+[![PyPI](https://img.shields.io/pypi/pyversions/async-etcd3gw.svg)](https://pypi.org/project/async-etcd3gw)
+[![License: Apache 2](https://img.shields.io/pypi/l/async-etcd3gw)](https://www.apache.org/licenses/LICENSE-2.0.html)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 ### Library Installation
 
 ```
-$ pip install async_etcd3gw
+$ pip install async-etcd3gw
 ```
 
 ### Usage
 
 You can find examples in examples folder.
 
 Basic usage example:
 
 ```python
 import asyncio
-from async_etcd3gw.async_client import AsyncEtcd3Client
+from async_etcd3gw import AsyncEtcd3Client
 
 async def main():
     client = AsyncEtcd3Client(host='etcd', port=2379)
 
     # Put key
     await client.put(key='foo', value='bar')
```

### Comparing `async_etcd3gw-0.1/async_etcd3gw/__init__.py` & `async_etcd3gw-0.2/async_etcd3gw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/__init__.py
 
 from . import utils
 from .async_client import AsyncEtcd3Client, async_client
 from .async_lease import AsyncLease
 from .async_lock import AsyncLock
 
-__version__ = "0.1"
+__version__ = "0.2"
 
 __all__ = (
     "AsyncEtcd3Client",
     "AsyncLease",
     "AsyncLock",
     "async_client",
     "utils",
```

### Comparing `async_etcd3gw-0.1/async_etcd3gw/async_client.py` & `async_etcd3gw-0.2/async_etcd3gw/async_client.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/async_etcd3gw/async_lease.py` & `async_etcd3gw-0.2/async_etcd3gw/async_lease.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/async_etcd3gw/async_lock.py` & `async_etcd3gw-0.2/async_etcd3gw/async_lock.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/async_etcd3gw/async_watch.py` & `async_etcd3gw-0.2/async_etcd3gw/async_watch.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/async_etcd3gw/exceptions.py` & `async_etcd3gw-0.2/async_etcd3gw/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/async_etcd3gw/utils.py` & `async_etcd3gw-0.2/async_etcd3gw/utils.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/setup.cfg` & `async_etcd3gw-0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [metadata]
 name = async_etcd3gw
 version = attr: async_etcd3gw.__version__
 summary = An async Python client for etcd3 grpc-gateway v3 API
-description_file = 
-	README.md
+keywords = etcd, asyncio, aiohttp
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = Alkemy spa
 author_email = DLBDDepartment@alkemy.com
 home_page = https://github.com/DLBD-Department/async_etcd3gw
 python_requires = >=3.9
+license = Apache License 2.0
+license_files = LICENSE
+platforms = any
 classifier = 
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
@@ -25,14 +29,16 @@
 	Source Code = https://github.com/DLBD-Department/async_etcd3gw
 
 [options]
 zip_safe = True
 include_package_data = True
 python_requires = >=3.9
 packages = find:
+install_requires = 
+	aiohttp
 
 [options.packages.find]
 include = async_etcd3gw*
 exclude = 
 	ez_setup
 	examples
 	tests
```

### Comparing `async_etcd3gw-0.1/tests/test_async_etcd3gw.py` & `async_etcd3gw-0.2/tests/test_async_etcd3gw.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.1/tests/test_client.py` & `async_etcd3gw-0.2/tests/test_client.py`

 * *Files identical despite different names*

