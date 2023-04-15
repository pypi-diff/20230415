# Comparing `tmp/pentapy-1.1.2.tar.gz` & `tmp/pentapy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pentapy-1.1.2.tar", last modified: Tue Jul  6 08:54:37 2021, max compression
+gzip compressed data, was "pentapy-1.2.0.tar", last modified: Sat Apr 15 18:17:43 2023, max compression
```

## Comparing `pentapy-1.1.2.tar` & `pentapy-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 08:54:37.139055 pentapy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-07-06 08:53:55.000000 pentapy-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-07-06 08:53:55.000000 pentapy-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6682 2021-07-06 08:54:37.139055 pentapy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2021-07-06 08:53:55.000000 pentapy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 08:54:37.139055 pentapy-1.1.2/pentapy/
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-07-06 08:53:55.000000 pentapy-1.1.2/pentapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-07-06 08:54:37.000000 pentapy-1.1.2/pentapy/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2021-07-06 08:53:55.000000 pentapy-1.1.2/pentapy/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-07-06 08:53:55.000000 pentapy-1.1.2/pentapy/solver.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     8874 2021-07-06 08:53:55.000000 pentapy-1.1.2/pentapy/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 08:54:37.139055 pentapy-1.1.2/pentapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-07-06 08:54:37.000000 pentapy-1.1.2/pentapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-07-06 08:53:55.000000 pentapy-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-07-06 08:54:37.139055 pentapy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      748 2021-07-06 08:53:55.000000 pentapy-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 08:54:37.139055 pentapy-1.1.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4988 2021-07-06 08:53:55.000000 pentapy-1.1.2/tests/test_pentapy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-15 18:17:02.000000 pentapy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-15 18:17:43.604335 pentapy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-15 18:17:02.000000 pentapy-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-15 18:17:02.000000 pentapy-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:17:43.604335 pentapy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 18:17:02.000000 pentapy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.600335 pentapy-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/src/pentapy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 18:17:43.000000 pentapy-1.2.0/src/pentapy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/solver.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/solver.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/src/pentapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-15 18:17:43.000000 pentapy-1.2.0/src/pentapy.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-04-15 18:17:02.000000 pentapy-1.2.0/tests/test_pentapy.py
```

### Comparing `pentapy-1.1.2/LICENSE` & `pentapy-1.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 Sebastian Müller
+Copyright (c) 2023 Sebastian Müller
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pentapy-1.1.2/PKG-INFO` & `pentapy-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: pentapy
-Version: 1.1.2
+Version: 1.2.0
 Summary: pentapy: A toolbox for pentadiagonal matrizes.
-Home-page: https://github.com/GeoStat-Framework/pentapy
-Author: Sebastian Müller
-Author-email: info@geostat-framework.org
-Maintainer: Sebastian Müller
-Maintainer-email: info@geostat-framework.org
+Author-email: Sebastian Müller <info@geostat-framework.org>
 License: MIT
+Project-URL: Homepage, https://github.com/GeoStat-Framework/pentapy
 Project-URL: Documentation, https://pentapy.readthedocs.io
 Project-URL: Source, https://github.com/GeoStat-Framework/pentapy
 Project-URL: Tracker, https://github.com/GeoStat-Framework/pentapy/issues
 Project-URL: Changelog, https://github.com/GeoStat-Framework/pentapy/blob/main/CHANGELOG.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/pentapy
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
@@ -26,21 +22,22 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: scipy
 Provides-Extra: umfpack
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: test
+Provides-Extra: check
 License-File: LICENSE
 
 # Welcome to pentapy
 
 [![status](https://joss.theoj.org/papers/57c3bbdd7b7f3068dd1e669ccbcf107c/status.svg)](https://joss.theoj.org/papers/57c3bbdd7b7f3068dd1e669ccbcf107c)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2587158.svg)](https://doi.org/10.5281/zenodo.2587158)
 [![PyPI version](https://badge.fury.io/py/pentapy.svg)](https://badge.fury.io/py/pentapy)
@@ -65,21 +62,15 @@
 ## Installation
 
 The package can be installed via [pip][pip_link].
 On Windows you can install [WinPython][winpy_link] to get Python and pip running.
 
     pip install pentapy
 
-There are pre-built wheels for Linux, MacOS and Windows for most Python versions (2.7, 3.4-3.7).
-
-If your system is not supported and you want to have the Cython routines of
-pentapy installed, you have to provide a c-compiler and run:
-
-    pip install numpy cython
-    pip install pentapy
+There are pre-built wheels for Linux, MacOS and Windows for most Python versions.
 
 To get the scipy solvers running, you have to install scipy or you can use the
 following extra argument:
 
     pip install pentapy[all]
 
 Instead of "all" you can also typ "scipy" or "umfpack" to get one of these specific packages.
@@ -164,15 +155,14 @@
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[MIT][licence_link] © 2019 - 2021
+[MIT][licence_link] © 2019 - 2023
 
 [ref_link]: http://dx.doi.org/10.1155/2015/232456
 [pip_link]: https://pypi.org/project/pentapy
 [winpy_link]: https://winpython.github.io/
 [licence_link]: https://github.com/GeoStat-Framework/pentapy/blob/main/LICENSE
 [doc_link]: https://pentapy.readthedocs.org
-
```

### Comparing `pentapy-1.1.2/README.md` & `pentapy-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,21 +24,15 @@
 ## Installation
 
 The package can be installed via [pip][pip_link].
 On Windows you can install [WinPython][winpy_link] to get Python and pip running.
 
     pip install pentapy
 
-There are pre-built wheels for Linux, MacOS and Windows for most Python versions (2.7, 3.4-3.7).
-
-If your system is not supported and you want to have the Cython routines of
-pentapy installed, you have to provide a c-compiler and run:
-
-    pip install numpy cython
-    pip install pentapy
+There are pre-built wheels for Linux, MacOS and Windows for most Python versions.
 
 To get the scipy solvers running, you have to install scipy or you can use the
 following extra argument:
 
     pip install pentapy[all]
 
 Instead of "all" you can also typ "scipy" or "umfpack" to get one of these specific packages.
@@ -123,14 +117,14 @@
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[MIT][licence_link] © 2019 - 2021
+[MIT][licence_link] © 2019 - 2023
 
 [ref_link]: http://dx.doi.org/10.1155/2015/232456
 [pip_link]: https://pypi.org/project/pentapy
 [winpy_link]: https://winpython.github.io/
 [licence_link]: https://github.com/GeoStat-Framework/pentapy/blob/main/LICENSE
 [doc_link]: https://pentapy.readthedocs.org
```

### Comparing `pentapy-1.1.2/pentapy/__init__.py` & `pentapy-1.2.0/src/pentapy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-# -*- coding: utf-8 -*-
 """
 Purpose
 =======
 
 pentapy is a toolbox to deal with pentadiagonal matrizes in Python.
 
+
+Subpackages
+^^^^^^^^^^^
+
+.. autosummary::
+   :toctree: api
+
+   tools
+
+
 Solver
 ^^^^^^
 
-.. currentmodule:: pentapy.core
-
 Solver for a pentadiagonal equations system.
 
 .. autosummary::
+   :toctree: api
+
    solve
 
 
 Tools
 ^^^^^
 
 .. currentmodule:: pentapy.tools
@@ -29,16 +38,16 @@
    create_banded
    create_full
 """
 from pentapy.core import solve
 from pentapy.tools import (
     create_banded,
     create_full,
-    shift_banded,
     diag_indices,
+    shift_banded,
 )
 
 try:
     from pentapy._version import __version__
 except ImportError:  # pragma: nocover
     # package is not installed
     __version__ = "0.0.0.dev0"
```

### Comparing `pentapy-1.1.2/pentapy/core.py` & `pentapy-1.2.0/src/pentapy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-# -*- coding: utf-8 -*-
-"""
-The core module of pentapy.
-
-The following functions are provided
-
-.. currentmodule:: pentapy.core
-
-.. autosummary::
-   solve
-"""
+"""The core module of pentapy."""
 # pylint: disable=C0103, C0415, R0911, E0611
 import warnings
+
 import numpy as np
-from pentapy.tools import shift_banded, create_banded, _check_penta
+
 from pentapy.solver import penta_solver1, penta_solver2
+from pentapy.tools import _check_penta, create_banded, shift_banded
 
 
 def solve(mat, rhs, is_flat=False, index_row_wise=True, solver=1):
     """
     Solver for a pentadiagonal system.
 
     The matrix can be given as a full n x n matrix or as a flattend one.
```

### Comparing `pentapy-1.1.2/pentapy/solver.pyx` & `pentapy-1.2.0/src/pentapy/solver.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 #cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
-# -*- coding: utf-8 -*-
 """
 This is a solver linear equation systems with a penta-diagonal matrix,
 implemented in cython.
 """
 import numpy as np
 
 cimport cython
 cimport numpy as np
 
 
 def penta_solver1(double[:,:] mat_flat, double[:] rhs):
+    return np.asarray(c_penta_solver1(mat_flat, rhs))
+
+
+def penta_solver2(double[:,:] mat_flat, double[:] rhs):
+    return np.asarray(c_penta_solver2(mat_flat, rhs))
+
+
+cdef double[:] c_penta_solver1(double[:,:] mat_flat, double[:] rhs):
 
     cdef int mat_j = mat_flat.shape[1]
 
     cdef double[:] result = np.zeros(mat_j)
 
     cdef double[:] al = np.zeros(mat_j)
     cdef double[:] be = np.zeros(mat_j)
@@ -55,18 +62,18 @@
     # Backward substitution
     result[mat_j-1] = ze[mat_j-1]
     result[mat_j-2] = ze[mat_j-2] - al[mat_j-2] * result[mat_j-1]
 
     for i in range(mat_j-3, -1, -1):
         result[i] = ze[i] - al[i] * result[i+1] - be[i] * result[i+2]
 
-    return np.asarray(result)
+    return result
 
 
-def penta_solver2(double[:,:] mat_flat, double[:] rhs):
+cdef double[:] c_penta_solver2(double[:,:] mat_flat, double[:] rhs):
 
     cdef int mat_j = mat_flat.shape[1]
 
     cdef double[:] result = np.zeros(mat_j)
 
     cdef double[:] ps = np.zeros(mat_j)  # psi
     cdef double[:] si = np.zeros(mat_j)  # sigma
@@ -107,8 +114,8 @@
     # Foreward substitution
     result[0] = we[0]
     result[1] = we[1] - si[1] * result[0]
 
     for i in range(2, mat_j):
         result[i] = we[i] - si[i] * result[i-1] - ph[i] * result[i-2]
 
-    return np.asarray(result)
+    return result
```

### Comparing `pentapy-1.1.2/pentapy/tools.py` & `pentapy-1.2.0/src/pentapy/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# -*- coding: utf-8 -*-
 """
 The tools module of pentapy.
 
 The following functions are provided
 
 .. currentmodule:: pentapy.tools
 
 .. autosummary::
+   :toctree:
+
    diag_indices
    shift_banded
    create_banded
    create_full
 """
 # pylint: disable=C0103
 import numpy as np
```

### Comparing `pentapy-1.1.2/tests/test_pentapy.py` & `pentapy-1.2.0/tests/test_pentapy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest for pentapy.
 """
-from __future__ import division, absolute_import, print_function
+import unittest
 
 # import platform
 import warnings
-import unittest
+
 import numpy as np
-import pentapy as pp
 
+import pentapy as pp
 
 warnings.simplefilter("always")
 
 
 class TestPentapy(unittest.TestCase):
     def setUp(self):
         self.seed = 19031977
```

