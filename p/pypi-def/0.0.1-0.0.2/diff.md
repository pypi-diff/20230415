# Comparing `tmp/pypi_def-0.0.1.tar.gz` & `tmp/pypi_def-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_def-0.0.1.tar", last modified: Fri Apr 14 22:16:18 2023, max compression
+gzip compressed data, was "pypi_def-0.0.2.tar", last modified: Fri Apr 14 22:26:47 2023, max compression
```

## Comparing `pypi_def-0.0.1.tar` & `pypi_def-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:16:18.605877 pypi_def-0.0.1/
--rw-r--r--   0 novay      (501) staff       (20)     1072 2023-04-14 22:09:39.000000 pypi_def-0.0.1/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)     2344 2023-04-14 22:16:18.605704 pypi_def-0.0.1/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     1639 2023-04-14 22:14:58.000000 pypi_def-0.0.1/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:16:18.604622 pypi_def-0.0.1/pypi_def/
--rw-r--r--   0 novay      (501) staff       (20)       41 2023-04-14 21:21:01.000000 pypi_def-0.0.1/pypi_def/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)       44 2023-04-14 21:21:15.000000 pypi_def-0.0.1/pypi_def/module1.py
--rw-r--r--   0 novay      (501) staff       (20)       62 2023-04-14 21:21:25.000000 pypi_def-0.0.1/pypi_def/module2.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:16:18.605416 pypi_def-0.0.1/pypi_def.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     2344 2023-04-14 22:16:18.000000 pypi_def-0.0.1/pypi_def.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)      215 2023-04-14 22:16:18.000000 pypi_def-0.0.1/pypi_def.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-14 22:16:18.000000 pypi_def-0.0.1/pypi_def.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)        9 2023-04-14 22:16:18.000000 pypi_def-0.0.1/pypi_def.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-14 22:16:18.605937 pypi_def-0.0.1/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1019 2023-04-14 22:11:33.000000 pypi_def-0.0.1/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:26:47.647945 pypi_def-0.0.2/
+-rw-r--r--   0 novay      (501) staff       (20)     1072 2023-04-14 22:09:39.000000 pypi_def-0.0.2/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)     2344 2023-04-14 22:26:47.647793 pypi_def-0.0.2/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     1639 2023-04-14 22:14:58.000000 pypi_def-0.0.2/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:26:47.645249 pypi_def-0.0.2/pypi_def/
+-rw-r--r--   0 novay      (501) staff       (20)       41 2023-04-14 21:21:01.000000 pypi_def-0.0.2/pypi_def/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)       44 2023-04-14 21:21:15.000000 pypi_def-0.0.2/pypi_def/module1.py
+-rw-r--r--   0 novay      (501) staff       (20)       62 2023-04-14 21:21:25.000000 pypi_def-0.0.2/pypi_def/module2.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:26:47.646908 pypi_def-0.0.2/pypi_def/subpackage1/
+-rw-r--r--   0 novay      (501) staff       (20)       46 2023-04-14 21:21:34.000000 pypi_def-0.0.2/pypi_def/subpackage1/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)       44 2023-04-14 21:21:41.000000 pypi_def-0.0.2/pypi_def/subpackage1/module3.py
+-rw-r--r--   0 novay      (501) staff       (20)       62 2023-04-14 21:21:47.000000 pypi_def-0.0.2/pypi_def/subpackage1/module4.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:26:47.647447 pypi_def-0.0.2/pypi_def/subpackage2/
+-rw-r--r--   0 novay      (501) staff       (20)       46 2023-04-14 21:21:54.000000 pypi_def-0.0.2/pypi_def/subpackage2/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)       44 2023-04-14 21:24:59.000000 pypi_def-0.0.2/pypi_def/subpackage2/module5.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:26:47.646145 pypi_def-0.0.2/pypi_def.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     2344 2023-04-14 22:26:47.000000 pypi_def-0.0.2/pypi_def.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-14 22:26:47.000000 pypi_def-0.0.2/pypi_def.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-14 22:26:47.000000 pypi_def-0.0.2/pypi_def.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)        9 2023-04-14 22:26:47.000000 pypi_def-0.0.2/pypi_def.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-14 22:26:47.647999 pypi_def-0.0.2/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1037 2023-04-14 22:26:34.000000 pypi_def-0.0.2/setup.py
```

### Comparing `pypi_def-0.0.1/LICENSE` & `pypi_def-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_def-0.0.1/PKG-INFO` & `pypi_def-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi_def
-Version: 0.0.1
+Version: 0.0.2
 Summary: Contoh Library Python dengan Def.
 Home-page: https://github.com/novay/pypi-def
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypi_def-0.0.1/README.md` & `pypi_def-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pypi_def-0.0.1/pypi_def.egg-info/PKG-INFO` & `pypi_def-0.0.2/pypi_def.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-def
-Version: 0.0.1
+Version: 0.0.2
 Summary: Contoh Library Python dengan Def.
 Home-page: https://github.com/novay/pypi-def
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypi_def-0.0.1/setup.py` & `pypi_def-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 from codecs import open
 from os import path
 
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="pypi_def",
-    version="0.0.1",
+    version="0.0.2",
     description="Contoh Library Python dengan Def.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/pypi-def",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
@@ -25,9 +25,9 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
-    packages=["pypi_def"]
+    packages=find_packages()
 )
```

