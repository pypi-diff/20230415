# Comparing `tmp/coola-0.0.5.tar.gz` & `tmp/coola-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coola-0.0.5.tar", max compression
+gzip compressed data, was "coola-0.0.6.tar", max compression
```

## Comparing `coola-0.0.5.tar` & `coola-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1501 2023-04-15 02:23:36.502839 coola-0.0.5/LICENSE
--rw-r--r--   0        0        0     4491 2023-04-15 02:23:36.502839 coola-0.0.5/README.md
--rw-r--r--   0        0        0     4067 2023-04-15 02:23:36.502839 coola-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      611 2023-04-15 02:23:36.502839 coola-0.0.5/src/coola/__init__.py
--rw-r--r--   0        0        0    18460 2023-04-15 02:23:36.502839 coola-0.0.5/src/coola/allclose.py
--rw-r--r--   0        0        0    13171 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/equality.py
--rw-r--r--   0        0        0     2444 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/format.py
--rw-r--r--   0        0        0     1195 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/import_utils.py
--rw-r--r--   0        0        0     4260 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/ndarray.py
--rw-r--r--   0        0        0     7521 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/pytorch.py
--rw-r--r--   0        0        0      297 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/testing.py
--rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 coola-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-04-15 03:00:55.142524 coola-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4491 2023-04-15 03:00:55.142524 coola-0.0.6/README.md
+-rw-r--r--   0        0        0     4113 2023-04-15 03:00:55.146524 coola-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      681 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/__init__.py
+-rw-r--r--   0        0        0    18460 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/allclose.py
+-rw-r--r--   0        0        0    13171 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/equality.py
+-rw-r--r--   0        0        0     2444 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/format.py
+-rw-r--r--   0        0        0     1195 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/import_utils.py
+-rw-r--r--   0        0        0     4260 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/ndarray.py
+-rw-r--r--   0        0        0     7521 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/pytorch.py
+-rw-r--r--   0        0        0      297 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/testing.py
+-rw-r--r--   0        0        0     5791 1970-01-01 00:00:00.000000 coola-0.0.6/PKG-INFO
```

### Comparing `coola-0.0.5/LICENSE` & `coola-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/README.md` & `coola-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/pyproject.toml` & `coola-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coola"
-version = "0.0.5"
+version = "0.0.6"
 description = "A light library to check if two complex/nested objects are equal or not"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/coola"
 repository = "https://github.com/durandtibo/coola"
 keywords = ["equality", "complex/nested objects"]
 license = "BSD-3-Clause"
@@ -14,14 +14,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
 ]
 
 packages = [
     { include = "coola", from = "src" },
 ]
```

### Comparing `coola-0.0.5/src/coola/__init__.py` & `coola-0.0.6/src/coola/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     BaseEqualityTester,
     EqualityTester,
     objects_are_equal,
 )
 from coola.import_utils import is_numpy_available, is_torch_available
 
 if is_numpy_available():
-    pass
+    from coola import ndarray  # noqa: F401
 
 if is_torch_available():
-    pass
+    from coola import pytorch  # noqa: F401
```

### Comparing `coola-0.0.5/src/coola/allclose.py` & `coola-0.0.6/src/coola/allclose.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/src/coola/equality.py` & `coola-0.0.6/src/coola/equality.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/src/coola/format.py` & `coola-0.0.6/src/coola/format.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/src/coola/import_utils.py` & `coola-0.0.6/src/coola/import_utils.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/src/coola/ndarray.py` & `coola-0.0.6/src/coola/ndarray.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/src/coola/pytorch.py` & `coola-0.0.6/src/coola/pytorch.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.5/PKG-INFO` & `coola-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coola
-Version: 0.0.5
+Version: 0.0.6
 Summary: A light library to check if two complex/nested objects are equal or not
 Home-page: https://github.com/durandtibo/coola
 License: BSD-3-Clause
 Keywords: equality,complex/nested objects
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
 Requires-Dist: torch (>=1.10,<3.0) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/coola
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: coola Version: 0.0.5 Summary: A light library to
+Metadata-Version: 2.1 Name: coola Version: 0.0.6 Summary: A light library to
 check if two complex/nested objects are equal or not Home-page: https://
 github.com/durandtibo/coola License: BSD-3-Clause Keywords: equality,complex/
 nested objects Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Software Development :: Libraries Provides-Extra: all Requires-Dist: numpy
-(>=1.20,<2.0) ; extra == "all" Requires-Dist: torch (>=1.10,<3.0) ; extra ==
-"all" Project-URL: Repository, https://github.com/durandtibo/coola Description-
-Content-Type: text/markdown # coola
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
+Libraries Provides-Extra: all Requires-Dist: numpy (>=1.20,<2.0) ; extra ==
+"all" Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Project-URL:
+Repository, https://github.com/durandtibo/coola Description-Content-Type: text/
+markdown # coola
 [CI] [PYPI_version] [Python] [BSD-3-Clause] [Codecov] [Code_style:_black] [Doc
                                 style:_google]
                        [Downloads] [Monthly_downloads]
 ## Overview `coola` is a light Python library that provides simple functions to
 check in a single line if two complex/nested objects are equal or not. `coola`
 was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
 docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
```

