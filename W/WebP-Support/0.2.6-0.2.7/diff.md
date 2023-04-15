# Comparing `tmp/webp_support-0.2.6.tar.gz` & `tmp/webp_support-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webp_support-0.2.6.tar", last modified: Sat Apr 15 07:41:56 2023, max compression
+gzip compressed data, was "webp_support-0.2.7.tar", last modified: Sat Apr 15 07:53:00 2023, max compression
```

## Comparing `webp_support-0.2.6.tar` & `webp_support-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:41:56.612640 webp_support-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 07:41:37.000000 webp_support-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 07:41:37.000000 webp_support-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:41:56.612640 webp_support-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 07:41:37.000000 webp_support-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 07:41:37.000000 webp_support-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:41:56.612640 webp_support-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-15 07:41:37.000000 webp_support-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:41:56.612640 webp_support-0.2.6/webp_support/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115007 2023-04-15 07:41:48.000000 webp_support-0.2.6/webp_support/webp_support.c
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:41:56.612640 webp_support-0.2.6/webp_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:53:00.127435 webp_support-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 07:52:41.000000 webp_support-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-15 07:52:41.000000 webp_support-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:53:00.127435 webp_support-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 07:52:41.000000 webp_support-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 07:52:41.000000 webp_support-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:53:00.127435 webp_support-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-15 07:52:41.000000 webp_support-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:53:00.127435 webp_support-0.2.7/webp_support/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-15 07:52:41.000000 webp_support-0.2.7/webp_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115007 2023-04-15 07:52:51.000000 webp_support-0.2.7/webp_support/webp_support.c
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 07:52:41.000000 webp_support-0.2.7/webp_support/webp_support.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 07:52:41.000000 webp_support-0.2.7/webp_support/webp_support.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 07:52:41.000000 webp_support-0.2.7/webp_support/webp_support.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 07:52:41.000000 webp_support-0.2.7/webp_support/webp_support_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 07:52:41.000000 webp_support-0.2.7/webp_support/webp_support_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:53:00.127435 webp_support-0.2.7/webp_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:53:00.000000 webp_support-0.2.7/webp_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-15 07:53:00.000000 webp_support-0.2.7/webp_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:53:00.000000 webp_support-0.2.7/webp_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 07:53:00.000000 webp_support-0.2.7/webp_support.egg-info/top_level.txt
```

### Comparing `webp_support-0.2.6/LICENSE` & `webp_support-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.6/PKG-INFO` & `webp_support-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp_support
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `webp_support-0.2.6/README.md` & `webp_support-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.6/setup.py` & `webp_support-0.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             "webp_support/webp_support_c.h",
             "webp_support/webp_support.pxd",
         ]
     },
     include_package_data=True,
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.2.6",
+    version="0.2.7",
     url="https://github.com/bymoye/webp_support",
     description="A Quickly determine whether Webp is supported from UserAgent.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

### Comparing `webp_support-0.2.6/webp_support/webp_support.c` & `webp_support-0.2.7/webp_support/webp_support.c`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.6/webp_support/webp_support_c.c` & `webp_support-0.2.7/webp_support/webp_support_c.c`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.6/webp_support.egg-info/PKG-INFO` & `webp_support-0.2.7/webp_support.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp-support
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

