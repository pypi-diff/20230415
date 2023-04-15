# Comparing `tmp/fernetcrypt-0.9.4.tar.gz` & `tmp/fernetcrypt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fernetcrypt-0.9.4.tar", last modified: Sat Apr 15 15:41:02 2023, max compression
+gzip compressed data, was "fernetcrypt-1.0.0.tar", last modified: Sat Apr 15 15:46:13 2023, max compression
```

## Comparing `fernetcrypt-0.9.4.tar` & `fernetcrypt-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:41:02.663959 fernetcrypt-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-15 15:40:47.000000 fernetcrypt-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-15 15:41:02.663959 fernetcrypt-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-15 15:40:47.000000 fernetcrypt-0.9.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     4161 2023-04-15 15:40:47.000000 fernetcrypt-0.9.4/fernetcrypt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:41:02.659959 fernetcrypt-0.9.4/fernetcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-15 15:41:02.000000 fernetcrypt-0.9.4/fernetcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-15 15:41:02.000000 fernetcrypt-0.9.4/fernetcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:41:02.000000 fernetcrypt-0.9.4/fernetcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 15:41:02.000000 fernetcrypt-0.9.4/fernetcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:41:02.000000 fernetcrypt-0.9.4/fernetcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:41:02.663959 fernetcrypt-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-15 15:40:53.000000 fernetcrypt-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:46:13.024688 fernetcrypt-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-15 15:46:01.000000 fernetcrypt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-15 15:46:13.024688 fernetcrypt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-15 15:46:01.000000 fernetcrypt-1.0.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4161 2023-04-15 15:46:01.000000 fernetcrypt-1.0.0/fernetcrypt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:46:13.024688 fernetcrypt-1.0.0/fernetcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-15 15:46:13.000000 fernetcrypt-1.0.0/fernetcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-15 15:46:13.000000 fernetcrypt-1.0.0/fernetcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:46:13.000000 fernetcrypt-1.0.0/fernetcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 15:46:13.000000 fernetcrypt-1.0.0/fernetcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:46:13.000000 fernetcrypt-1.0.0/fernetcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:46:13.024688 fernetcrypt-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-15 15:46:06.000000 fernetcrypt-1.0.0/setup.py
```

### Comparing `fernetcrypt-0.9.4/LICENSE` & `fernetcrypt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fernetcrypt-0.9.4/PKG-INFO` & `fernetcrypt-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fernetcrypt
-Version: 0.9.4
+Version: 1.0.0
 Summary: FernetCrypt CLI Encrypt and decrypt files using a password.
 Home-page: https://github.com/linsomniac/fernetcrypt
 Author: Sean Reifschneider
 Author-email: jafo00@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fernetcrypt-0.9.4/README.md` & `fernetcrypt-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fernetcrypt-0.9.4/fernetcrypt` & `fernetcrypt-1.0.0/fernetcrypt`

 * *Files identical despite different names*

### Comparing `fernetcrypt-0.9.4/fernetcrypt.egg-info/PKG-INFO` & `fernetcrypt-1.0.0/fernetcrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fernetcrypt
-Version: 0.9.4
+Version: 1.0.0
 Summary: FernetCrypt CLI Encrypt and decrypt files using a password.
 Home-page: https://github.com/linsomniac/fernetcrypt
 Author: Sean Reifschneider
 Author-email: jafo00@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fernetcrypt-0.9.4/setup.py` & `fernetcrypt-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 readme = open('README.md', 'r').read()
 
 setup(
     name="fernetcrypt",
-    version="0.9.4",
+    version="1.0.0",
     description="FernetCrypt CLI Encrypt and decrypt files using a password.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Sean Reifschneider",
     author_email="jafo00@gmail.com",
     url="https://github.com/linsomniac/fernetcrypt",
     scripts=["fernetcrypt"],
```

