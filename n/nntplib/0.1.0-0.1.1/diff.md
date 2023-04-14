# Comparing `tmp/nntplib-0.1.0.tar.gz` & `tmp/nntplib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nntplib-0.1.0.tar", last modified: Thu Apr 13 21:12:29 2023, max compression
+gzip compressed data, was "nntplib-0.1.1.tar", last modified: Fri Apr 14 19:49:48 2023, max compression
```

## Comparing `nntplib-0.1.0.tar` & `nntplib-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-13 21:12:29.748476 nntplib-0.1.0/
--rw-r--r--   0 matej     (1000) users      (100)      115 2023-04-13 20:54:11.000000 nntplib-0.1.0/CHANGES
--rw-r--r--   0 matej     (1000) users      (100)     1078 2022-04-11 14:20:29.000000 nntplib-0.1.0/LICENSE
--rw-r--r--   0 matej     (1000) users      (100)      103 2023-04-13 20:50:42.000000 nntplib-0.1.0/MANIFEST.in
--rw-r--r--   0 matej     (1000) users      (100)      835 2023-04-13 21:12:29.748476 nntplib-0.1.0/PKG-INFO
--rw-r--r--   0 matej     (1000) users      (100)      298 2023-04-13 20:32:11.000000 nntplib-0.1.0/README
--rw-r--r--   0 matej     (1000) users      (100)    21764 2022-04-11 07:29:19.000000 nntplib-0.1.0/nntplib.rst
--rw-r--r--   0 matej     (1000) users      (100)      778 2023-04-13 20:41:06.000000 nntplib-0.1.0/pyproject.toml
--rw-r--r--   0 matej     (1000) users      (100)       38 2023-04-13 21:12:29.748476 nntplib-0.1.0/setup.cfg
-drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-13 21:12:29.748476 nntplib-0.1.0/src/
--rw-r--r--   0 matej     (1000) users      (100)        0 2023-04-13 20:45:44.000000 nntplib-0.1.0/src/__init__.py
-drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-13 21:12:29.748476 nntplib-0.1.0/src/nntplib.egg-info/
--rw-r--r--   0 matej     (1000) users      (100)      835 2023-04-13 21:12:29.000000 nntplib-0.1.0/src/nntplib.egg-info/PKG-INFO
--rw-r--r--   0 matej     (1000) users      (100)      325 2023-04-13 21:12:29.000000 nntplib-0.1.0/src/nntplib.egg-info/SOURCES.txt
--rw-r--r--   0 matej     (1000) users      (100)        1 2023-04-13 21:12:29.000000 nntplib-0.1.0/src/nntplib.egg-info/dependency_links.txt
--rw-r--r--   0 matej     (1000) users      (100)       46 2023-04-13 21:12:29.000000 nntplib-0.1.0/src/nntplib.egg-info/requires.txt
--rw-r--r--   0 matej     (1000) users      (100)       17 2023-04-13 21:12:29.000000 nntplib-0.1.0/src/nntplib.egg-info/top_level.txt
--rw-r--r--   0 matej     (1000) users      (100)    41023 2022-04-11 07:29:19.000000 nntplib-0.1.0/src/nntplib.py
-drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-13 21:12:29.748476 nntplib-0.1.0/tests/
--rw-r--r--   0 matej     (1000) users      (100)        0 2023-04-13 20:45:50.000000 nntplib-0.1.0/tests/__init__.py
--rw-r--r--   0 matej     (1000) users      (100)     9448 2022-04-11 07:17:55.000000 nntplib-0.1.0/tests/keycert3.pem
--rw-r--r--   0 matej     (1000) users      (100)    64188 2023-04-13 20:18:57.000000 nntplib-0.1.0/tests/test_nntplib.py
+drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-14 19:49:48.560375 nntplib-0.1.1/
+-rw-r--r--   0 matej     (1000) users      (100)      203 2023-04-14 19:48:29.000000 nntplib-0.1.1/CHANGES
+-rw-r--r--   0 matej     (1000) users      (100)     1078 2022-04-11 14:20:29.000000 nntplib-0.1.1/LICENSE
+-rw-r--r--   0 matej     (1000) users      (100)      103 2023-04-13 21:30:17.000000 nntplib-0.1.1/MANIFEST.in
+-rw-r--r--   0 matej     (1000) users      (100)      987 2023-04-14 19:49:48.560375 nntplib-0.1.1/PKG-INFO
+-rw-r--r--   0 matej     (1000) users      (100)      298 2023-04-13 21:34:20.000000 nntplib-0.1.1/README.md
+-rw-r--r--   0 matej     (1000) users      (100)    21764 2022-04-11 07:29:19.000000 nntplib-0.1.1/nntplib.rst
+-rw-r--r--   0 matej     (1000) users      (100)      893 2023-04-14 19:49:39.000000 nntplib-0.1.1/pyproject.toml
+-rw-r--r--   0 matej     (1000) users      (100)       38 2023-04-14 19:49:48.560375 nntplib-0.1.1/setup.cfg
+drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-14 19:49:48.556375 nntplib-0.1.1/src/
+-rw-r--r--   0 matej     (1000) users      (100)        0 2023-04-13 21:30:17.000000 nntplib-0.1.1/src/__init__.py
+drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-14 19:49:48.560375 nntplib-0.1.1/src/nntplib.egg-info/
+-rw-r--r--   0 matej     (1000) users      (100)      987 2023-04-14 19:49:48.000000 nntplib-0.1.1/src/nntplib.egg-info/PKG-INFO
+-rw-r--r--   0 matej     (1000) users      (100)      328 2023-04-14 19:49:48.000000 nntplib-0.1.1/src/nntplib.egg-info/SOURCES.txt
+-rw-r--r--   0 matej     (1000) users      (100)        1 2023-04-14 19:49:48.000000 nntplib-0.1.1/src/nntplib.egg-info/dependency_links.txt
+-rw-r--r--   0 matej     (1000) users      (100)       46 2023-04-14 19:49:48.000000 nntplib-0.1.1/src/nntplib.egg-info/requires.txt
+-rw-r--r--   0 matej     (1000) users      (100)       17 2023-04-14 19:49:48.000000 nntplib-0.1.1/src/nntplib.egg-info/top_level.txt
+-rw-r--r--   0 matej     (1000) users      (100)    41023 2023-04-13 21:30:17.000000 nntplib-0.1.1/src/nntplib.py
+drwxr-xr-x   0 matej     (1000) users      (100)        0 2023-04-14 19:49:48.560375 nntplib-0.1.1/tests/
+-rw-r--r--   0 matej     (1000) users      (100)        0 2023-04-13 21:30:17.000000 nntplib-0.1.1/tests/__init__.py
+-rw-r--r--   0 matej     (1000) users      (100)     9448 2023-04-13 21:30:17.000000 nntplib-0.1.1/tests/keycert3.pem
+-rw-r--r--   0 matej     (1000) users      (100)    64188 2023-04-13 21:34:23.000000 nntplib-0.1.1/tests/test_nntplib.py
```

### Comparing `nntplib-0.1.0/LICENSE` & `nntplib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nntplib-0.1.0/PKG-INFO` & `nntplib-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: nntplib
-Version: 0.1.0
+Version: 0.1.1
 Summary: nntplib from Python 3 standard library as an independent module
 Author-email: Matěj Cepl <mcepl@cepl.eu>
 License: BSD-3-Clause
+Project-URL: Homepage, https://sr.ht/~mcepl/nntplib/
+Project-URL: Bug Tracker, https://lists.sr.ht/~mcepl/devel
 Keywords: nntp
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications :: Usenet News
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 nntplib library from Python 3 standard library as an independent module.
 
 All issues, questions, complaints, or (even better!) patches
 should be send via email to
 [~mcepl/devel@lists.sr.ht](mailto:~mcepl/devel@lists.sr.ht) email
```

### Comparing `nntplib-0.1.0/nntplib.rst` & `nntplib-0.1.1/nntplib.rst`

 * *Files identical despite different names*

### Comparing `nntplib-0.1.0/pyproject.toml` & `nntplib-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [project]
 name = "nntplib"
-version = "0.1.0"
+version = "0.1.1"
 description = "nntplib from Python 3 standard library as an independent module"
 keywords = ["nntp"]
 authors = [
     { name = "Matěj Cepl", email = "mcepl@cepl.eu" }
 ]
 dependencies = [
     'importlib-metadata; python_version<"3.8"',
 ]
-readme = "README"
+readme = "README.md"
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Framework :: Django",
     "License :: OSI Approved :: BSD License",
     "Topic :: Internet",
     "Topic :: Communications :: Usenet News",
     "Topic :: Software Development :: Libraries",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
 ]
 
+[project.urls]
+"Homepage" = "https://sr.ht/~mcepl/nntplib/"
+"Bug Tracker" = "https://lists.sr.ht/~mcepl/devel"
+
 # [project.scripts]
 # my-script = "my_package.module:function"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `nntplib-0.1.0/src/nntplib.egg-info/PKG-INFO` & `nntplib-0.1.1/src/nntplib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: nntplib
-Version: 0.1.0
+Version: 0.1.1
 Summary: nntplib from Python 3 standard library as an independent module
 Author-email: Matěj Cepl <mcepl@cepl.eu>
 License: BSD-3-Clause
+Project-URL: Homepage, https://sr.ht/~mcepl/nntplib/
+Project-URL: Bug Tracker, https://lists.sr.ht/~mcepl/devel
 Keywords: nntp
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications :: Usenet News
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 nntplib library from Python 3 standard library as an independent module.
 
 All issues, questions, complaints, or (even better!) patches
 should be send via email to
 [~mcepl/devel@lists.sr.ht](mailto:~mcepl/devel@lists.sr.ht) email
```

### Comparing `nntplib-0.1.0/src/nntplib.py` & `nntplib-0.1.1/src/nntplib.py`

 * *Files identical despite different names*

### Comparing `nntplib-0.1.0/tests/keycert3.pem` & `nntplib-0.1.1/tests/keycert3.pem`

 * *Files identical despite different names*

### Comparing `nntplib-0.1.0/tests/test_nntplib.py` & `nntplib-0.1.1/tests/test_nntplib.py`

 * *Files identical despite different names*

