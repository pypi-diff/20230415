# Comparing `tmp/s3tethys-0.0.7.tar.gz` & `tmp/s3tethys-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3tethys-0.0.7.tar", last modified: Sat Apr 15 00:19:26 2023, max compression
+gzip compressed data, was "s3tethys-0.0.8.tar", last modified: Sat Apr 15 00:21:00 2023, max compression
```

## Comparing `s3tethys-0.0.7.tar` & `s3tethys-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:19:26.057992 s3tethys-0.0.7/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-11-04 04:20:46.000000 s3tethys-0.0.7/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      579 2023-04-15 00:19:26.057992 s3tethys-0.0.7/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      131 2022-11-04 04:20:46.000000 s3tethys-0.0.7/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2022-11-04 04:20:46.000000 s3tethys-0.0.7/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:19:26.057992 s3tethys-0.0.7/s3tethys/
--rw-rw-r--   0 mike      (1000) mike      (1000)      379 2022-11-04 04:20:46.000000 s3tethys-0.0.7/s3tethys/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:19:26.057992 s3tethys-0.0.7/s3tethys/datasets/
--rw-rw-r--   0 mike      (1000) mike      (1000)      906 2022-11-04 04:20:46.000000 s3tethys-0.0.7/s3tethys/datasets/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    23325 2023-04-14 23:56:13.000000 s3tethys-0.0.7/s3tethys/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:19:26.057992 s3tethys-0.0.7/s3tethys/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2022-11-04 04:20:46.000000 s3tethys-0.0.7/s3tethys/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1433 2023-04-14 23:27:57.000000 s3tethys-0.0.7/s3tethys/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:19:26.057992 s3tethys-0.0.7/s3tethys.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      579 2023-04-15 00:19:26.000000 s3tethys-0.0.7/s3tethys.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      324 2023-04-15 00:19:26.000000 s3tethys-0.0.7/s3tethys.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-04-15 00:19:26.000000 s3tethys-0.0.7/s3tethys.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       43 2023-04-15 00:19:26.000000 s3tethys-0.0.7/s3tethys.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        9 2023-04-15 00:19:26.000000 s3tethys-0.0.7/s3tethys.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-04-15 00:19:26.057992 s3tethys-0.0.7/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7230 2023-04-15 00:19:19.000000 s3tethys-0.0.7/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:21:00.822527 s3tethys-0.0.8/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-11-04 04:20:46.000000 s3tethys-0.0.8/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      579 2023-04-15 00:21:00.822527 s3tethys-0.0.8/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      131 2022-11-04 04:20:46.000000 s3tethys-0.0.8/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2022-11-04 04:20:46.000000 s3tethys-0.0.8/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:21:00.818527 s3tethys-0.0.8/s3tethys/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      379 2022-11-04 04:20:46.000000 s3tethys-0.0.8/s3tethys/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:21:00.822527 s3tethys-0.0.8/s3tethys/datasets/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      906 2022-11-04 04:20:46.000000 s3tethys-0.0.8/s3tethys/datasets/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    23325 2023-04-14 23:56:13.000000 s3tethys-0.0.8/s3tethys/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:21:00.822527 s3tethys-0.0.8/s3tethys/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2022-11-04 04:20:46.000000 s3tethys-0.0.8/s3tethys/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1433 2023-04-14 23:27:57.000000 s3tethys-0.0.8/s3tethys/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:21:00.822527 s3tethys-0.0.8/s3tethys.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      579 2023-04-15 00:21:00.000000 s3tethys-0.0.8/s3tethys.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      324 2023-04-15 00:21:00.000000 s3tethys-0.0.8/s3tethys.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-04-15 00:21:00.000000 s3tethys-0.0.8/s3tethys.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       52 2023-04-15 00:21:00.000000 s3tethys-0.0.8/s3tethys.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        9 2023-04-15 00:21:00.000000 s3tethys-0.0.8/s3tethys.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-04-15 00:21:00.822527 s3tethys-0.0.8/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7242 2023-04-15 00:20:05.000000 s3tethys-0.0.8/setup.py
```

### Comparing `s3tethys-0.0.7/LICENSE` & `s3tethys-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `s3tethys-0.0.7/PKG-INFO` & `s3tethys-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3tethys
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python S3 tools for tethys using smart_open
 Home-page: https://github.com/tethys-ts/s3tethys
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3tethys-0.0.7/s3tethys/datasets/__init__.py` & `s3tethys-0.0.8/s3tethys/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `s3tethys-0.0.7/s3tethys/main.py` & `s3tethys-0.0.8/s3tethys/main.py`

 * *Files identical despite different names*

### Comparing `s3tethys-0.0.7/s3tethys/utils.py` & `s3tethys-0.0.8/s3tethys/utils.py`

 * *Files identical despite different names*

### Comparing `s3tethys-0.0.7/s3tethys.egg-info/PKG-INFO` & `s3tethys-0.0.8/s3tethys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3tethys
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python S3 tools for tethys using smart_open
 Home-page: https://github.com/tethys-ts/s3tethys
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3tethys-0.0.7/setup.py` & `s3tethys-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3tethys'
 main_package = 's3tethys'
 datasets = 'datasets'
-version = '0.0.7'
+version = '0.0.8'
 descrip = 'Python S3 tools for tethys using smart_open'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
 else:
-    INSTALL_REQUIRES = ['smart_open', 'boto3', 'pandas', 'zstandard', 'requests']
+    INSTALL_REQUIRES = ['smart_open', 'boto3', 'pandas', 'zstandard', 'requests', 'pydantic']
 
 # Get the long description from the README file
 with open(os.path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 # get all data dirs in the datasets module
 # data_files = []
```

