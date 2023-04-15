# Comparing `tmp/webp_support-0.2.2.tar.gz` & `tmp/webp_support-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webp_support-0.2.2.tar", last modified: Sat Apr 15 04:07:58 2023, max compression
+gzip compressed data, was "webp_support-0.2.3.tar", last modified: Sat Apr 15 04:08:55 2023, max compression
```

## Comparing `webp_support-0.2.2.tar` & `webp_support-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:07:58.839226 webp_support-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 04:07:20.000000 webp_support-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-15 04:07:20.000000 webp_support-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 04:07:58.839226 webp_support-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 04:07:20.000000 webp_support-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-15 04:07:20.000000 webp_support-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:07:58.839226 webp_support-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-15 04:07:20.000000 webp_support-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)   113081 2023-04-15 04:07:44.000000 webp_support-0.2.2/webp_support.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:07:58.839226 webp_support-0.2.2/webp_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 04:07:58.000000 webp_support-0.2.2/webp_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-15 04:07:58.000000 webp_support-0.2.2/webp_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:07:58.000000 webp_support-0.2.2/webp_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 04:07:58.000000 webp_support-0.2.2/webp_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 04:07:20.000000 webp_support-0.2.2/webp_support.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 04:07:20.000000 webp_support-0.2.2/webp_support.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 04:07:20.000000 webp_support-0.2.2/webp_support_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 04:07:20.000000 webp_support-0.2.2/webp_support_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:08:55.770403 webp_support-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 04:08:38.000000 webp_support-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-15 04:08:38.000000 webp_support-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 04:08:55.770403 webp_support-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 04:08:38.000000 webp_support-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-15 04:08:38.000000 webp_support-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:08:55.770403 webp_support-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-15 04:08:38.000000 webp_support-0.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113081 2023-04-15 04:08:48.000000 webp_support-0.2.3/webp_support.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:08:55.770403 webp_support-0.2.3/webp_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 04:08:55.000000 webp_support-0.2.3/webp_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-15 04:08:55.000000 webp_support-0.2.3/webp_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:08:55.000000 webp_support-0.2.3/webp_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 04:08:55.000000 webp_support-0.2.3/webp_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 04:08:38.000000 webp_support-0.2.3/webp_support.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 04:08:38.000000 webp_support-0.2.3/webp_support.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 04:08:38.000000 webp_support-0.2.3/webp_support_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 04:08:38.000000 webp_support-0.2.3/webp_support_c.h
```

### Comparing `webp_support-0.2.2/LICENSE` & `webp_support-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.2/PKG-INFO` & `webp_support-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp_support
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `webp_support-0.2.2/README.md` & `webp_support-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.2/setup.py` & `webp_support-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         language_level=3,
         compiler_directives={
             "language_level": 3,
             "boundscheck": False,
             "wraparound": False,
         },
     ),
-    package_data={'webp_support': ['*.pyi', "*.pyx"]},
+    package_data={'webp_support': ['*.pyi', "*.pyx","*.c","*.h"]},
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.2.2",
+    version="0.2.3",
     url="https://github.com/bymoye/webp_support",
     description="A Quickly determine whether Webp is supported from UserAgent.",
     long_description="A Quickly determine whether Webp is supported from UserAgent.",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `webp_support-0.2.2/webp_support.c` & `webp_support-0.2.3/webp_support.c`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.2/webp_support.egg-info/PKG-INFO` & `webp_support-0.2.3/webp_support.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp-support
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `webp_support-0.2.2/webp_support_c.c` & `webp_support-0.2.3/webp_support_c.c`

 * *Files identical despite different names*

