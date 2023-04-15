# Comparing `tmp/upathlib-0.7.7.tar.gz` & `tmp/upathlib-0.7.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.7.7.tar", last modified: Sat Apr 15 03:07:43 2023, max compression
+gzip compressed data, was "upathlib-0.7.7b1.tar", last modified: Mon Apr 10 09:15:46 2023, max compression
```

## Comparing `upathlib-0.7.7.tar` & `upathlib-0.7.7b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.7/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.7/README.rst
--rw-r--r--   0        0        0     1726 2023-04-15 03:04:37.334046 upathlib-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     2303 2023-04-15 02:52:53.497373 upathlib-0.7.7/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4438 2023-04-10 08:06:32.336660 upathlib-0.7.7/src/upathlib/_blob.py
--rw-r--r--   0        0        0    11176 2023-04-10 09:03:09.436670 upathlib-0.7.7/src/upathlib/_local.py
--rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.7/src/upathlib/_tests.py
--rw-r--r--   0        0        0    34436 2023-04-14 16:32:49.582758 upathlib-0.7.7/src/upathlib/_upath.py
--rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.7/src/upathlib/azure.py
--rw-r--r--   0        0        0    25298 2023-04-10 08:06:32.346660 upathlib-0.7.7/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.7/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.7/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 upathlib-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.7b1/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.7b1/README.rst
+-rw-r--r--   0        0        0     1696 2023-04-10 08:06:32.336660 upathlib-0.7.7b1/pyproject.toml
+-rw-r--r--   0        0        0     2305 2023-04-10 09:02:39.215528 upathlib-0.7.7b1/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4438 2023-04-10 08:06:32.336660 upathlib-0.7.7b1/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    11176 2023-04-10 09:03:09.436670 upathlib-0.7.7b1/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7852 2023-03-07 05:27:40.006650 upathlib-0.7.7b1/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34266 2023-04-10 09:03:09.506671 upathlib-0.7.7b1/src/upathlib/_upath.py
+-rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/azure.py
+-rw-r--r--   0        0        0    25298 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.7b1/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.7b1/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.7.7b1/PKG-INFO
```

### Comparing `upathlib-0.7.7/LICENSE` & `upathlib-0.7.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/README.rst` & `upathlib-0.7.7b1/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/pyproject.toml` & `upathlib-0.7.7b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -58,18 +58,17 @@
 
 [tool.flit.module]
 name = "upathlib"
 
 
 # See https://beta.ruff.rs/docs/rules/
 [tool.ruff]
-target-version = "py38"
+target-version = "py310"
 select = ["E", "F", "S", "I001"]  # isort
 ignore = ["E501", "S101", "S102", "S103", "S104", "S108", "S301", "S311", "S608"]
-exclude = ["tests/benchmarks"]
 
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 
 
 [tool.pytest.ini_options]
```

### Comparing `upathlib-0.7.7/src/upathlib/__init__.py` & `upathlib-0.7.7b1/src/upathlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.7.7"
+__version__ = "0.7.7b1"
 
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalUpath
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
```

### Comparing `upathlib-0.7.7/src/upathlib/_blob.py` & `upathlib-0.7.7b1/src/upathlib/_blob.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/src/upathlib/_local.py` & `upathlib-0.7.7b1/src/upathlib/_local.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/src/upathlib/_tests.py` & `upathlib-0.7.7b1/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/src/upathlib/_upath.py` & `upathlib-0.7.7b1/src/upathlib/_upath.py`

 * *Files 1% similar despite different names*

```diff
@@ -894,31 +894,28 @@
         Similar to :meth:`iterdir`, if ``self`` is not a dir or does not exist,
         then nothing is yielded, and no exception is raised either.
 
         There is no guarantee on the order of the returned elements.
         """
         raise NotImplementedError
 
-    def rmrf(self, *, quiet: bool = True, concurrent: bool = False) -> int:
+    def rmrf(self, *, quiet: bool = True, concurrent: bool = True) -> int:
         """Remove the current file or dir (i.e. ``self``) recursively.
 
         Analogous to the Linux command ``rm -rf``, hence the name of this method.
 
         Return the number of files removed.
 
         For example, if these blobs are present::
 
             /a/b/c/d/e.txt
             /a/b/c/kk.data
             /a/b/c
 
         then ``Upath('/a/b/c').rmrf()`` would remove all of them.
-
-        ``concurrent`` is ``False`` by default because this method is often used in
-        ``__del__`` of user classes, and thread pool is problematic in ``__del__``.
         """
         if self._path == "/":
             raise UnsupportedOperation("`rmrf` not allowed on root directory")
         try:
             self.remove_file()
         except (FileNotFoundError, IsADirectoryError):
             n = 0
```

### Comparing `upathlib-0.7.7/src/upathlib/azure.py` & `upathlib-0.7.7b1/src/upathlib/azure.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/src/upathlib/gcs.py` & `upathlib-0.7.7b1/src/upathlib/gcs.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/src/upathlib/serializer.py` & `upathlib-0.7.7b1/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.7/PKG-INFO` & `upathlib-0.7.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.7.7
+Version: 0.7.7b1
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

