# Comparing `tmp/cairocffi-1.5.0.tar.gz` & `tmp/cairocffi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cairocffi-1.5.0.tar", last modified: Fri Mar 17 16:08:30 2023, max compression
+gzip compressed data, was "cairocffi-1.5.1.tar", last modified: Sat Apr 15 07:25:44 2023, max compression
```

## Comparing `cairocffi-1.5.0.tar` & `cairocffi-1.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-17 16:08:30.838178 cairocffi-1.5.0/
--rw-r--r--   0 lize      (1000) lize      (1000)     1534 2020-10-29 21:18:23.000000 cairocffi-1.5.0/LICENSE
--rw-r--r--   0 lize      (1000) lize      (1000)       22 2023-03-17 15:46:47.000000 cairocffi-1.5.0/MANIFEST.in
--rw-r--r--   0 lize      (1000) lize      (1000)     4610 2023-03-17 16:08:30.838178 cairocffi-1.5.0/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)     1612 2022-09-24 18:06:51.000000 cairocffi-1.5.0/README.rst
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-17 16:08:30.836178 cairocffi-1.5.0/cairocffi/
--rw-r--r--   0 lize      (1000) lize      (1000)     4034 2023-03-17 16:04:05.000000 cairocffi-1.5.0/cairocffi/__init__.py
--rw-r--r--   0 lize      (1000) lize      (1000)    55889 2023-03-11 08:33:29.000000 cairocffi-1.5.0/cairocffi/constants.py
--rw-r--r--   0 lize      (1000) lize      (1000)    84791 2022-10-03 08:01:47.000000 cairocffi-1.5.0/cairocffi/context.py
--rw-r--r--   0 lize      (1000) lize      (1000)     4174 2023-03-17 14:21:58.000000 cairocffi-1.5.0/cairocffi/ffi_build.py
--rw-r--r--   0 lize      (1000) lize      (1000)    19493 2020-10-29 21:18:23.000000 cairocffi-1.5.0/cairocffi/fonts.py
--rw-r--r--   0 lize      (1000) lize      (1000)     8064 2020-10-29 21:18:23.000000 cairocffi-1.5.0/cairocffi/matrix.py
--rw-r--r--   0 lize      (1000) lize      (1000)    12978 2020-10-29 21:18:23.000000 cairocffi-1.5.0/cairocffi/patterns.py
--rw-r--r--   0 lize      (1000) lize      (1000)     7260 2020-10-29 21:18:23.000000 cairocffi-1.5.0/cairocffi/pixbuf.py
--rw-r--r--   0 lize      (1000) lize      (1000)    57999 2023-03-11 21:33:03.000000 cairocffi-1.5.0/cairocffi/surfaces.py
--rw-r--r--   0 lize      (1000) lize      (1000)    46873 2023-03-11 07:55:03.000000 cairocffi-1.5.0/cairocffi/test_cairo.py
--rw-r--r--   0 lize      (1000) lize      (1000)      405 2023-03-11 07:55:03.000000 cairocffi-1.5.0/cairocffi/test_numpy.py
--rw-r--r--   0 lize      (1000) lize      (1000)     2398 2023-03-11 07:55:03.000000 cairocffi-1.5.0/cairocffi/test_pixbuf.py
--rw-r--r--   0 lize      (1000) lize      (1000)     6338 2023-03-11 07:55:03.000000 cairocffi-1.5.0/cairocffi/test_xcb.py
--rw-r--r--   0 lize      (1000) lize      (1000)     2023 2020-10-29 21:18:23.000000 cairocffi-1.5.0/cairocffi/xcb.py
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-17 16:08:30.836178 cairocffi-1.5.0/cairocffi.egg-info/
--rw-r--r--   0 lize      (1000) lize      (1000)     4610 2023-03-17 16:08:30.000000 cairocffi-1.5.0/cairocffi.egg-info/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)      821 2023-03-17 16:08:30.000000 cairocffi-1.5.0/cairocffi.egg-info/SOURCES.txt
--rw-r--r--   0 lize      (1000) lize      (1000)        1 2023-03-17 16:08:30.000000 cairocffi-1.5.0/cairocffi.egg-info/dependency_links.txt
--rw-r--r--   0 lize      (1000) lize      (1000)      106 2023-03-17 16:08:30.000000 cairocffi-1.5.0/cairocffi.egg-info/requires.txt
--rw-r--r--   0 lize      (1000) lize      (1000)       10 2023-03-17 16:08:30.000000 cairocffi-1.5.0/cairocffi.egg-info/top_level.txt
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-17 16:08:30.837178 cairocffi-1.5.0/docs/
--rw-r--r--   0 lize      (1000) lize      (1000)    21215 2020-10-29 21:18:23.000000 cairocffi-1.5.0/docs/api.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     4335 2020-10-29 21:18:23.000000 cairocffi-1.5.0/docs/cffi_api.rst
--rw-r--r--   0 lize      (1000) lize      (1000)       54 2023-03-11 07:55:03.000000 cairocffi-1.5.0/docs/changelog.rst
--rw-r--r--   0 lize      (1000) lize      (1000)      555 2020-10-29 21:18:23.000000 cairocffi-1.5.0/docs/conf.py
--rw-r--r--   0 lize      (1000) lize      (1000)      139 2020-10-29 21:18:23.000000 cairocffi-1.5.0/docs/index.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     5446 2021-10-04 10:06:33.000000 cairocffi-1.5.0/docs/overview.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     1234 2020-10-29 21:18:23.000000 cairocffi-1.5.0/docs/pixbuf.rst
--rw-r--r--   0 lize      (1000) lize      (1000)      273 2020-10-29 21:18:23.000000 cairocffi-1.5.0/docs/xcb.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     1709 2023-03-17 16:01:18.000000 cairocffi-1.5.0/pyproject.toml
--rw-r--r--   0 lize      (1000) lize      (1000)       38 2023-03-17 16:08:30.838178 cairocffi-1.5.0/setup.cfg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-17 16:08:30.838178 cairocffi-1.5.0/utils/
--rw-r--r--   0 lize      (1000) lize      (1000)      740 2023-03-17 16:01:18.000000 cairocffi-1.5.0/utils/build.py
--rw-r--r--   0 lize      (1000) lize      (1000)      777 2020-10-29 21:18:23.000000 cairocffi-1.5.0/utils/cairo_coverage.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1390 2020-10-29 21:18:23.000000 cairocffi-1.5.0/utils/cairocffi_to_pycairo.py
--rw-r--r--   0 lize      (1000) lize      (1000)      756 2020-10-29 21:18:23.000000 cairocffi-1.5.0/utils/compare_pycairo.py
--rw-r--r--   0 lize      (1000) lize      (1000)     3001 2023-03-11 08:03:35.000000 cairocffi-1.5.0/utils/mkconstants.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1853 2020-10-29 21:18:23.000000 cairocffi-1.5.0/utils/pango_example.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1056 2020-10-29 21:18:23.000000 cairocffi-1.5.0/utils/pycairo_to_cairocffi.py
--rw-r--r--   0 lize      (1000) lize      (1000)      999 2023-03-11 07:55:03.000000 cairocffi-1.5.0/utils/tests.py
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.517513 cairocffi-1.5.1/
+-rw-r--r--   0 lize      (1000) lize      (1000)     1534 2020-10-29 21:18:23.000000 cairocffi-1.5.1/LICENSE
+-rw-r--r--   0 lize      (1000) lize      (1000)       22 2023-03-25 08:13:29.000000 cairocffi-1.5.1/MANIFEST.in
+-rw-r--r--   0 lize      (1000) lize      (1000)     4610 2023-04-15 07:25:44.517513 cairocffi-1.5.1/PKG-INFO
+-rw-r--r--   0 lize      (1000) lize      (1000)     1612 2023-03-25 08:13:29.000000 cairocffi-1.5.1/README.rst
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.515513 cairocffi-1.5.1/cairocffi/
+-rw-r--r--   0 lize      (1000) lize      (1000)     4034 2023-04-15 07:22:16.000000 cairocffi-1.5.1/cairocffi/__init__.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    55889 2023-03-25 08:13:29.000000 cairocffi-1.5.1/cairocffi/constants.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    84791 2022-10-03 08:01:47.000000 cairocffi-1.5.1/cairocffi/context.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     4174 2023-04-15 07:12:26.000000 cairocffi-1.5.1/cairocffi/ffi_build.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    19493 2020-10-29 21:18:23.000000 cairocffi-1.5.1/cairocffi/fonts.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     8064 2020-10-29 21:18:23.000000 cairocffi-1.5.1/cairocffi/matrix.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    12978 2020-10-29 21:18:23.000000 cairocffi-1.5.1/cairocffi/patterns.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     7260 2023-04-15 07:08:00.000000 cairocffi-1.5.1/cairocffi/pixbuf.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    57999 2023-03-25 08:13:29.000000 cairocffi-1.5.1/cairocffi/surfaces.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    46873 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_cairo.py
+-rw-r--r--   0 lize      (1000) lize      (1000)      405 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_numpy.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     2398 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_pixbuf.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     6338 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_xcb.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     2023 2023-04-14 22:15:06.000000 cairocffi-1.5.1/cairocffi/xcb.py
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.516513 cairocffi-1.5.1/cairocffi.egg-info/
+-rw-r--r--   0 lize      (1000) lize      (1000)     4610 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/PKG-INFO
+-rw-r--r--   0 lize      (1000) lize      (1000)      821 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/SOURCES.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)        1 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/dependency_links.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)      106 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/requires.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)       10 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/top_level.txt
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.516513 cairocffi-1.5.1/docs/
+-rw-r--r--   0 lize      (1000) lize      (1000)    21215 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/api.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     4335 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/cffi_api.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)       54 2023-03-11 07:55:03.000000 cairocffi-1.5.1/docs/changelog.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)      555 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/conf.py
+-rw-r--r--   0 lize      (1000) lize      (1000)      139 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/index.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     5446 2021-10-04 10:06:33.000000 cairocffi-1.5.1/docs/overview.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     1234 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/pixbuf.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)      273 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/xcb.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     1709 2023-04-15 07:08:00.000000 cairocffi-1.5.1/pyproject.toml
+-rw-r--r--   0 lize      (1000) lize      (1000)       38 2023-04-15 07:25:44.517513 cairocffi-1.5.1/setup.cfg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.517513 cairocffi-1.5.1/utils/
+-rw-r--r--   0 lize      (1000) lize      (1000)      953 2023-04-15 07:17:22.000000 cairocffi-1.5.1/utils/build.py
+-rw-r--r--   0 lize      (1000) lize      (1000)      777 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/cairo_coverage.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     1390 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/cairocffi_to_pycairo.py
+-rw-r--r--   0 lize      (1000) lize      (1000)      756 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/compare_pycairo.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     3001 2023-03-25 08:13:29.000000 cairocffi-1.5.1/utils/mkconstants.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     1853 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/pango_example.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     1056 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/pycairo_to_cairocffi.py
+-rw-r--r--   0 lize      (1000) lize      (1000)      999 2023-03-11 07:55:03.000000 cairocffi-1.5.1/utils/tests.py
```

### Comparing `cairocffi-1.5.0/LICENSE` & `cairocffi-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/PKG-INFO` & `cairocffi-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cairocffi
-Version: 1.5.0
+Version: 1.5.1
 Summary: cffi-based cairo bindings for Python
 Author-email: Simon Sapin <contact@courtbouillon.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2013-2019, Simon Sapin and contributors.
         All rights reserved.
```

### Comparing `cairocffi-1.5.0/README.rst` & `cairocffi-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/__init__.py` & `cairocffi-1.5.1/cairocffi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import sys
 from ctypes.util import find_library
 
 from . import constants
 from ._generated.ffi import ffi
 
-VERSION = __version__ = '1.5.0'
+VERSION = __version__ = '1.5.1'
 # supported version of cairo, used to be pycairo version too:
 version = '1.17.2'
 version_info = (1, 17, 2)
 
 
 def dlopen(ffi, library_names, filenames):
     """Try various names for the same library, for different platforms."""
```

### Comparing `cairocffi-1.5.0/cairocffi/constants.py` & `cairocffi-1.5.1/cairocffi/constants.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/context.py` & `cairocffi-1.5.1/cairocffi/context.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/ffi_build.py` & `cairocffi-1.5.1/cairocffi/ffi_build.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/fonts.py` & `cairocffi-1.5.1/cairocffi/fonts.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/matrix.py` & `cairocffi-1.5.1/cairocffi/matrix.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/patterns.py` & `cairocffi-1.5.1/cairocffi/patterns.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/pixbuf.py` & `cairocffi-1.5.1/cairocffi/pixbuf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/surfaces.py` & `cairocffi-1.5.1/cairocffi/surfaces.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/test_cairo.py` & `cairocffi-1.5.1/cairocffi/test_cairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/test_pixbuf.py` & `cairocffi-1.5.1/cairocffi/test_pixbuf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/test_xcb.py` & `cairocffi-1.5.1/cairocffi/test_xcb.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi/xcb.py` & `cairocffi-1.5.1/cairocffi/xcb.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/cairocffi.egg-info/PKG-INFO` & `cairocffi-1.5.1/cairocffi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cairocffi
-Version: 1.5.0
+Version: 1.5.1
 Summary: cffi-based cairo bindings for Python
 Author-email: Simon Sapin <contact@courtbouillon.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2013-2019, Simon Sapin and contributors.
         All rights reserved.
```

### Comparing `cairocffi-1.5.0/cairocffi.egg-info/SOURCES.txt` & `cairocffi-1.5.1/cairocffi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/docs/api.rst` & `cairocffi-1.5.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/docs/cffi_api.rst` & `cairocffi-1.5.1/docs/cffi_api.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/docs/conf.py` & `cairocffi-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/docs/overview.rst` & `cairocffi-1.5.1/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/docs/pixbuf.rst` & `cairocffi-1.5.1/docs/pixbuf.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/pyproject.toml` & `cairocffi-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/utils/build.py` & `cairocffi-1.5.1/utils/build.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib.util
+import subprocess
 import sys
 from pathlib import Path
 
 from setuptools import build_meta
 from setuptools.build_meta import *  # noqa
 
 folder = Path(__file__).parent.parent / 'cairocffi'
@@ -11,14 +12,21 @@
 def build_sdist(*args, **kwargs):
     (folder / '_generated' / 'ffi.py').unlink(missing_ok=True)
     (folder / '_generated' / 'ffi_pixbuf.py').unlink(missing_ok=True)
     return build_meta.build_sdist(*args, **kwargs)
 
 
 def build_wheel(*args, **kwargs):
+    # Try to install xcffib for XCB support
+    try:
+        pip = Path(sys.executable).parent / 'pip'
+        subprocess.run([str(pip), 'install', 'xcffib'])
+    except Exception:
+        pass
+
     spec = importlib.util.spec_from_file_location(
         'ffi_build', folder / 'ffi_build.py')
     module = importlib.util.module_from_spec(spec)
     sys.modules['ffi_build'] = module
     spec.loader.exec_module(module)
     module.compile()
     return build_meta.build_wheel(*args, **kwargs)
```

### Comparing `cairocffi-1.5.0/utils/cairo_coverage.py` & `cairocffi-1.5.1/utils/cairo_coverage.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/utils/cairocffi_to_pycairo.py` & `cairocffi-1.5.1/utils/cairocffi_to_pycairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/utils/compare_pycairo.py` & `cairocffi-1.5.1/utils/compare_pycairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/utils/mkconstants.py` & `cairocffi-1.5.1/utils/mkconstants.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/utils/pango_example.py` & `cairocffi-1.5.1/utils/pango_example.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/utils/pycairo_to_cairocffi.py` & `cairocffi-1.5.1/utils/pycairo_to_cairocffi.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.0/utils/tests.py` & `cairocffi-1.5.1/utils/tests.py`

 * *Files identical despite different names*

