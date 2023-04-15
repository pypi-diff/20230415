# Comparing `tmp/coola-0.0.4.tar.gz` & `tmp/coola-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coola-0.0.4.tar", max compression
+gzip compressed data, was "coola-0.0.5.tar", max compression
```

## Comparing `coola-0.0.4.tar` & `coola-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1501 2023-01-13 16:27:20.491742 coola-0.0.4/LICENSE
--rw-r--r--   0        0        0     4178 2023-01-13 16:27:20.491742 coola-0.0.4/README.md
--rw-r--r--   0        0        0     2413 2023-01-13 16:27:20.491742 coola-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      653 2023-01-13 16:27:20.491742 coola-0.0.4/src/coola/__init__.py
--rw-r--r--   0        0        0    18458 2023-01-13 16:27:20.491742 coola-0.0.4/src/coola/allclose.py
--rw-r--r--   0        0        0    13169 2023-01-13 16:27:20.491742 coola-0.0.4/src/coola/equality.py
--rw-r--r--   0        0        0     2444 2023-01-13 16:27:20.491742 coola-0.0.4/src/coola/format.py
--rw-r--r--   0        0        0     1195 2023-01-13 16:27:20.491742 coola-0.0.4/src/coola/import_utils.py
--rw-r--r--   0        0        0     4244 2023-01-13 16:27:20.491742 coola-0.0.4/src/coola/ndarray.py
--rw-r--r--   0        0        0     7489 2023-01-13 16:27:20.491742 coola-0.0.4/src/coola/pytorch.py
--rw-r--r--   0        0        0     5074 1970-01-01 00:00:00.000000 coola-0.0.4/setup.py
--rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 coola-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-04-15 02:23:36.502839 coola-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4491 2023-04-15 02:23:36.502839 coola-0.0.5/README.md
+-rw-r--r--   0        0        0     4067 2023-04-15 02:23:36.502839 coola-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      611 2023-04-15 02:23:36.502839 coola-0.0.5/src/coola/__init__.py
+-rw-r--r--   0        0        0    18460 2023-04-15 02:23:36.502839 coola-0.0.5/src/coola/allclose.py
+-rw-r--r--   0        0        0    13171 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/equality.py
+-rw-r--r--   0        0        0     2444 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/format.py
+-rw-r--r--   0        0        0     1195 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/import_utils.py
+-rw-r--r--   0        0        0     4260 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/ndarray.py
+-rw-r--r--   0        0        0     7521 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/pytorch.py
+-rw-r--r--   0        0        0      297 2023-04-15 02:23:36.506839 coola-0.0.5/src/coola/testing.py
+-rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 coola-0.0.5/PKG-INFO
```

### Comparing `coola-0.0.4/LICENSE` & `coola-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coola-0.0.4/README.md` & `coola-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # coola
 
 <p align="center">
-   <a href="https://github.com/durandtibo/coola/actions">
-      <img alt="CI" src="https://github.com/durandtibo/coola/workflows/CI/badge.svg?event=push&branch=main">
-   </a>
+    <a href="https://github.com/durandtibo/coola/actions">
+        <img alt="CI" src="https://github.com/durandtibo/coola/workflows/CI/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://pypi.org/project/coola/">
+        <img alt="PYPI version" src="https://img.shields.io/pypi/v/coola">
+    </a>
     <a href="https://pypi.org/project/coola/">
-      <img alt="PYPI version" src="https://img.shields.io/pypi/v/coola">
+        <img alt="Python" src="https://img.shields.io/pypi/pyversions/coola.svg">
+    </a>
+    <a href="https://opensource.org/licenses/BSD-3-Clause">
+        <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/coola">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/coola">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://github.com/psf/black">
+        <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+    </a>
+    <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
+        <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
+    </a>
+    <br/>
+    <a href="https://pepy.tech/project/coola">
+        <img  alt="Downloads" src="https://static.pepy.tech/badge/coola">
+    </a>
+    <a href="https://pepy.tech/project/coola">
+        <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/coola/month">
     </a>
-   <a href="https://pypi.org/project/coola/">
-      <img alt="Python" src="https://img.shields.io/pypi/pyversions/coola.svg">
-   </a>
-   <a href="https://opensource.org/licenses/BSD-3-Clause">
-      <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/coola">
-   </a>
-   <a href="https://codecov.io/gh/durandtibo/coola">
-      <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">
-   </a>
-   <a href="https://github.com/psf/black">
-     <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
-   </a>
-   <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
-     <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
-   </a>
-   <br/>
+    <br/>
 </p>
 
 ## Overview
 
 `coola` is a light Python library that provides simple functions to check in a single line if two
 complex/nested objects are equal or not.
 `coola` was initially designed to work
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 # coola
 [CI] [PYPI_version] [Python] [BSD-3-Clause] [Codecov] [Code_style:_black] [Doc
                                 style:_google]
+                       [Downloads] [Monthly_downloads]
 ## Overview `coola` is a light Python library that provides simple functions to
 check in a single line if two complex/nested objects are equal or not. `coola`
 was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
 docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
 reference/generated/numpy.ndarray.html), but it is possible to extend it to
 [support other data structures](https://durandtibo.github.io/coola/
 customization). - [Motivation](#motivation) - [Documentation](https://
```

### Comparing `coola-0.0.4/src/coola/__init__.py` & `coola-0.0.5/src/coola/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     BaseEqualityTester,
     EqualityTester,
     objects_are_equal,
 )
 from coola.import_utils import is_numpy_available, is_torch_available
 
 if is_numpy_available():
-    from coola import ndarray
+    pass
 
 if is_torch_available():
-    from coola import pytorch
+    pass
```

### Comparing `coola-0.0.4/src/coola/allclose.py` & `coola-0.0.5/src/coola/allclose.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         object1: Any,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
-        if not type(object1) is type(object2):
+        if type(object1) is not type(object2):
             if show_difference:
                 logger.info(f"Objects have different types: {type(object1)} vs {type(object2)}")
             return False
         object_equal = object1 == object2
         if show_difference and not object_equal:
             logger.info(f"Objects are different:\nobject1={object1}\nobject2={object2}")
         return object_equal
@@ -220,15 +220,15 @@
         object1: Mapping,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
-        if not type(object1) is type(object2):
+        if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The mappings have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
             if show_difference:
@@ -265,15 +265,15 @@
         object1: Union[bool, int, float],
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
-        if not type(object1) is type(object2):
+        if type(object1) is not type(object2):
             if show_difference:
                 logger.info(f"Objects have different types: {type(object1)} vs {type(object2)}")
             return False
         number_equal = math.isclose(object1, object2, rel_tol=rtol, abs_tol=atol)
         if show_difference and not number_equal:
             logger.info(f"The numbers are different: {object1} vs {object2}")
         return number_equal
@@ -288,15 +288,15 @@
         object1: Sequence,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
-        if not type(object1) is type(object2):
+        if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The sequences have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
             if show_difference:
@@ -394,15 +394,15 @@
             ...     ) -> bool:
             ...         ...  # Custom implementation to test strings
             >>> AllCloseTester.add_allclose_operator(str, MyStringAllCloseOperator())
             # To overwrite an existing operato
             >>> AllCloseTester.add_allclose_operator(str, MyStringAllCloseOperator(), exist_ok=True)
         """
         if data_type in cls.registry and not exist_ok:
-            raise ValueError(
+            raise RuntimeError(
                 f"An operator ({cls.registry[data_type]}) is already registered for the data "
                 f"type {data_type}.Please use `exist_ok=True` if you want to overwrite the "
                 "operator for this type"
             )
         cls.registry[data_type] = operator
 
     def allclose(
```

### Comparing `coola-0.0.4/src/coola/equality.py` & `coola-0.0.5/src/coola/equality.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Any,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
-        if not type(object1) is type(object2):
+        if type(object1) is not type(object2):
             if show_difference:
                 logger.info(f"Objects have different types: {type(object1)} vs {type(object2)}")
             return False
         object_equal = object1 == object2
         if show_difference and not object_equal:
             logger.info(f"Objects are different:\nobject1={object1}\nobject2={object2}")
         return object_equal
@@ -155,15 +155,15 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Mapping,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
-        if not type(object1) is type(object2):
+        if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The mappings have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
             if show_difference:
@@ -195,15 +195,15 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Sequence,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
-        if not type(object1) is type(object2):
+        if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The sequences have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
             if show_difference:
@@ -275,15 +275,15 @@
             ...     ) -> bool:
             ...         ...  # Custom implementation to test strings
             >>> EqualityTester.add_equality_operator(str, MyStringEqualityOperator())
             # To overwrite an existing operato
             >>> EqualityTester.add_equality_operator(str, MyStringEqualityOperator(), exist_ok=True)
         """
         if data_type in cls.registry and not exist_ok:
-            raise ValueError(
+            raise RuntimeError(
                 f"An operator ({cls.registry[data_type]}) is already registered for the data "
                 f"type {data_type}. Please use `exist_ok=True` if you want to overwrite the "
                 "operator for this type"
             )
         cls.registry[data_type] = operator
 
     def equal(self, object1: Any, object2: Any, show_difference: bool = False) -> bool:
```

### Comparing `coola-0.0.4/src/coola/format.py` & `coola-0.0.5/src/coola/format.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.4/src/coola/import_utils.py` & `coola-0.0.5/src/coola/import_utils.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.4/src/coola/ndarray.py` & `coola-0.0.5/src/coola/ndarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     Args:
         check_dtype (bool, optional): If ``True``, the data type of
             the arrays are checked, otherwise the data types are
             ignored. Default: ``True``
     """
 
-    def __init__(self, check_dtype: bool = True):
+    def __init__(self, check_dtype: bool = True) -> None:
         check_numpy()
         self._check_dtype = bool(check_dtype)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(check_dtype={self._check_dtype})"
 
     def allclose(
@@ -68,15 +68,15 @@
 
     Args:
         check_dtype (bool, optional): If ``True``, the data type of
             the arrays are checked, otherwise the data types are
             ignored. Default: ``True``
     """
 
-    def __init__(self, check_dtype: bool = True):
+    def __init__(self, check_dtype: bool = True) -> None:
         check_numpy()
         self._check_dtype = bool(check_dtype)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(check_dtype={self._check_dtype})"
 
     def equal(
```

### Comparing `coola-0.0.4/src/coola/pytorch.py` & `coola-0.0.5/src/coola/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 logger = logging.getLogger(__name__)
 
 
 class PackedSequenceAllCloseOperator(BaseAllCloseOperator[PackedSequence]):
     r"""Implements an allclose operator for
     ``torch.nn.utils.rnn.PackedSequence``."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         check_torch()
 
     def allclose(
         self,
         tester: BaseAllCloseTester,
         object1: PackedSequence,
         object2: Any,
@@ -86,15 +86,15 @@
         return object_equal
 
 
 class PackedSequenceEqualityOperator(BaseEqualityOperator[PackedSequence]):
     r"""Implements an equality operator for
     ``torch.nn.utils.rnn.PackedSequence``."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         check_torch()
 
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: PackedSequence,
         object2: Any,
@@ -119,15 +119,15 @@
             )
         return object_equal
 
 
 class TensorAllCloseOperator(BaseAllCloseOperator[Tensor]):
     r"""Implements an allclose operator for ``torch.Tensor``."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         check_torch()
 
     def allclose(
         self,
         tester: BaseAllCloseTester,
         object1: Tensor,
         object2: Any,
@@ -163,15 +163,15 @@
             logger.info(f"torch.Tensors are different\nobject1=\n{object1}\nobject2=\n{object2}")
         return object_equal
 
 
 class TensorEqualityOperator(BaseEqualityOperator[Tensor]):
     r"""Implements an equality operator for ``torch.Tensor``."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         check_torch()
 
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Tensor,
         object2: Any,
```

### Comparing `coola-0.0.4/setup.py` & `coola-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,153 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: coola
+Version: 0.0.5
+Summary: A light library to check if two complex/nested objects are equal or not
+Home-page: https://github.com/durandtibo/coola
+License: BSD-3-Clause
+Keywords: equality,complex/nested objects
+Author: Thibaut Durand
+Author-email: durand.tibo+gh@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: all
+Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
+Requires-Dist: torch (>=1.10,<3.0) ; extra == "all"
+Project-URL: Repository, https://github.com/durandtibo/coola
+Description-Content-Type: text/markdown
+
+# coola
+
+<p align="center">
+    <a href="https://github.com/durandtibo/coola/actions">
+        <img alt="CI" src="https://github.com/durandtibo/coola/workflows/CI/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://pypi.org/project/coola/">
+        <img alt="PYPI version" src="https://img.shields.io/pypi/v/coola">
+    </a>
+    <a href="https://pypi.org/project/coola/">
+        <img alt="Python" src="https://img.shields.io/pypi/pyversions/coola.svg">
+    </a>
+    <a href="https://opensource.org/licenses/BSD-3-Clause">
+        <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/coola">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/coola">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://github.com/psf/black">
+        <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+    </a>
+    <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
+        <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
+    </a>
+    <br/>
+    <a href="https://pepy.tech/project/coola">
+        <img  alt="Downloads" src="https://static.pepy.tech/badge/coola">
+    </a>
+    <a href="https://pepy.tech/project/coola">
+        <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/coola/month">
+    </a>
+    <br/>
+</p>
+
+## Overview
+
+`coola` is a light Python library that provides simple functions to check in a single line if two
+complex/nested objects are equal or not.
+`coola` was initially designed to work
+with [PyTorch `Tensor`s](https://pytorch.org/docs/stable/tensors.html)
+and [NumPy `ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
+is possible to extend it
+to [support other data structures](https://durandtibo.github.io/coola/customization).
+
+- [Motivation](#motivation)
+- [Documentation](https://durandtibo.github.io/coola/)
+- [Installation](#installation)
+- [Contributing](#contributing)
+- [API stability](#api-stability)
+- [License](#license)
+
+## Motivation
+
+Let's imagine you have the following dictionaries that contain both a PyTorch `Tensor` and a
+NumPy `ndarray`.
+You want to check if the two dictionaries are equal or not.
+By default, Python does not provide an easy way to check if the two dictionaries are equal or not.
+It is not possible to use the default equality operator `==` because it will raise an error.
+The `coola` library was developed to fill this gap. `coola` provides a function `objects_are_equal`
+that can indicate if two complex/nested objects are equal or not.
+
+```python
+import numpy
+import torch
+
+from coola import objects_are_equal
+
+data1 = {'torch': torch.ones(2, 3), 'numpy': numpy.zeros((2, 3))}
+data2 = {'torch': torch.zeros(2, 3), 'numpy': numpy.ones((2, 3))}
+
+objects_are_equal(data1, data2)
+```
+
+`coola` also provides a function `objects_are_allclose` that can indicate if two complex/nested
+objects are equal within a tolerance or not.
+
+```python
+from coola import objects_are_allclose
+
+objects_are_allclose(data1, data2, atol=1e-6)
+```
+
+Please check the [quickstart page](https://durandtibo.github.io/coola/quickstart) to learn more on
+how to use `coola`.
+
+## Installation
+
+We highly recommend installing
+a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
+`coola` can be installed from pip using the following command:
+
+```shell
+pip install coola
+```
+
+To make the package as slim as possible, only the minimal packages required to use `coola` are
+installed.
+To include all the packages, you can use the following command:
+
+```shell
+pip install coola[all]
+```
+
+Please check the [get started page](https://durandtibo.github.io/coola/get_started) to see how to
+install only some specific packages or other alternatives to install the library.
+
+## Contributing
+
+Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
+
+## API stability
+
+:warning: While `coola` is in development stage, no API is guaranteed to be stable from one
+release to the next.
+In fact, it is very likely that the API will change multiple times before a stable 1.0.0 release.
+In practice, this means that upgrading `coola` to a new version will possibly break any code that
+was using the old version of `coola`.
 
-package_dir = \
-{'': 'src'}
+## License
 
-packages = \
-['coola']
+`coola` is licensed under BSD 3-Clause "New" or "Revised" license available in [LICENSE](LICENSE)
+file.
 
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'all': ['numpy>=1.20,<2.0', 'torch>=1.10,<2.0']}
-
-setup_kwargs = {
-    'name': 'coola',
-    'version': '0.0.4',
-    'description': 'A light library to check if two complex/nested objects are equal or not',
-    'long_description': '# coola\n\n<p align="center">\n   <a href="https://github.com/durandtibo/coola/actions">\n      <img alt="CI" src="https://github.com/durandtibo/coola/workflows/CI/badge.svg?event=push&branch=main">\n   </a>\n    <a href="https://pypi.org/project/coola/">\n      <img alt="PYPI version" src="https://img.shields.io/pypi/v/coola">\n    </a>\n   <a href="https://pypi.org/project/coola/">\n      <img alt="Python" src="https://img.shields.io/pypi/pyversions/coola.svg">\n   </a>\n   <a href="https://opensource.org/licenses/BSD-3-Clause">\n      <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/coola">\n   </a>\n   <a href="https://codecov.io/gh/durandtibo/coola">\n      <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">\n   </a>\n   <a href="https://github.com/psf/black">\n     <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">\n   </a>\n   <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">\n     <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">\n   </a>\n   <br/>\n</p>\n\n## Overview\n\n`coola` is a light Python library that provides simple functions to check in a single line if two\ncomplex/nested objects are equal or not.\n`coola` was initially designed to work\nwith [PyTorch `Tensor`s](https://pytorch.org/docs/stable/tensors.html)\nand [NumPy `ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it\nis possible to extend it\nto [support other data structures](https://durandtibo.github.io/coola/customization).\n\n- [Motivation](#motivation)\n- [Documentation](https://durandtibo.github.io/coola/)\n- [Installation](#installation)\n- [Contributing](#contributing)\n- [API stability](#api-stability)\n- [License](#license)\n\n## Motivation\n\nLet\'s imagine you have the following dictionaries that contain both a PyTorch `Tensor` and a\nNumPy `ndarray`.\nYou want to check if the two dictionaries are equal or not.\nBy default, Python does not provide an easy way to check if the two dictionaries are equal or not.\nIt is not possible to use the default equality operator `==` because it will raise an error.\nThe `coola` library was developed to fill this gap. `coola` provides a function `objects_are_equal`\nthat can indicate if two complex/nested objects are equal or not.\n\n```python\nimport numpy\nimport torch\n\nfrom coola import objects_are_equal\n\ndata1 = {\'torch\': torch.ones(2, 3), \'numpy\': numpy.zeros((2, 3))}\ndata2 = {\'torch\': torch.zeros(2, 3), \'numpy\': numpy.ones((2, 3))}\n\nobjects_are_equal(data1, data2)\n```\n\n`coola` also provides a function `objects_are_allclose` that can indicate if two complex/nested\nobjects are equal within a tolerance or not.\n\n```python\nfrom coola import objects_are_allclose\n\nobjects_are_allclose(data1, data2, atol=1e-6)\n```\n\nPlease check the [quickstart page](https://durandtibo.github.io/coola/quickstart) to learn more on\nhow to use `coola`.\n\n## Installation\n\nWe highly recommend installing\na [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).\n`coola` can be installed from pip using the following command:\n\n```shell\npip install coola\n```\n\nTo make the package as slim as possible, only the minimal packages required to use `coola` are\ninstalled.\nTo include all the packages, you can use the following command:\n\n```shell\npip install coola[all]\n```\n\nPlease check the [get started page](https://durandtibo.github.io/coola/get_started) to see how to\ninstall only some specific packages or other alternatives to install the library.\n\n## Contributing\n\nPlease check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).\n\n## API stability\n\n:warning: While `coola` is in development stage, no API is guaranteed to be stable from one\nrelease to the next.\nIn fact, it is very likely that the API will change multiple times before a stable 1.0.0 release.\nIn practice, this means that upgrading `coola` to a new version will possibly break any code that\nwas using the old version of `coola`.\n\n## License\n\n`coola` is licensed under BSD 3-Clause "New" or "Revised" license available in [LICENSE](LICENSE)\nfile.\n',
-    'author': 'Thibaut Durand',
-    'author_email': 'durand.tibo+gh@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/durandtibo/coola',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,56 +1,60 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['coola'] package_data = \ {'': ['*']} extras_require = \
-{'all': ['numpy>=1.20,<2.0', 'torch>=1.10,<2.0']} setup_kwargs = { 'name':
-'coola', 'version': '0.0.4', 'description': 'A light library to check if two
-complex/nested objects are equal or not', 'long_description': '# coola\n\n
-\n \n_[CI]\n\n \n_[PYPI_version]\n\n \n_[Python]\n\n \n_[BSD-3-Clause]\n\n \n_
-     [Codecov]\n\n \n_[Code_style:_black]\n\n \n_[Doc_style:_google]\n\n
-                                      \n
-\n\n## Overview\n\n`coola` is a light Python library that provides simple
-functions to check in a single line if two\ncomplex/nested objects are equal or
-not.\n`coola` was initially designed to work\nwith [PyTorch `Tensor`s](https://
-pytorch.org/docs/stable/tensors.html)\nand [NumPy `ndarray`](https://numpy.org/
-doc/stable/reference/generated/numpy.ndarray.html), but it\nis possible to
-extend it\nto [support other data structures](https://durandtibo.github.io/
-coola/customization).\n\n- [Motivation](#motivation)\n- [Documentation](https:/
-/durandtibo.github.io/coola/)\n- [Installation](#installation)\n-
-[Contributing](#contributing)\n- [API stability](#api-stability)\n- [License]
-(#license)\n\n## Motivation\n\nLet\'s imagine you have the following
-dictionaries that contain both a PyTorch `Tensor` and a\nNumPy `ndarray`.\nYou
-want to check if the two dictionaries are equal or not.\nBy default, Python
-does not provide an easy way to check if the two dictionaries are equal or
-not.\nIt is not possible to use the default equality operator `==` because it
-will raise an error.\nThe `coola` library was developed to fill this gap.
-`coola` provides a function `objects_are_equal`\nthat can indicate if two
-complex/nested objects are equal or not.\n\n```python\nimport numpy\nimport
-torch\n\nfrom coola import objects_are_equal\n\ndata1 = {\'torch\': torch.ones
-(2, 3), \'numpy\': numpy.zeros((2, 3))}\ndata2 = {\'torch\': torch.zeros(2, 3),
-\'numpy\': numpy.ones((2, 3))}\n\nobjects_are_equal(data1,
-data2)\n```\n\n`coola` also provides a function `objects_are_allclose` that can
-indicate if two complex/nested\nobjects are equal within a tolerance or
-not.\n\n```python\nfrom coola import
-objects_are_allclose\n\nobjects_are_allclose(data1, data2, atol=1e-
-6)\n```\n\nPlease check the [quickstart page](https://durandtibo.github.io/
-coola/quickstart) to learn more on\nhow to use `coola`.\n\n##
-Installation\n\nWe highly recommend installing\na [virtual environment](https:/
-/packaging.python.org/guides/installing-using-pip-and-virtual-environments/
-).\n`coola` can be installed from pip using the following command:
-\n\n```shell\npip install coola\n```\n\nTo make the package as slim as
-possible, only the minimal packages required to use `coola` are\ninstalled.\nTo
-include all the packages, you can use the following command:\n\n```shell\npip
-install coola[all]\n```\n\nPlease check the [get started page](https://
-durandtibo.github.io/coola/get_started) to see how to\ninstall only some
-specific packages or other alternatives to install the library.\n\n##
-Contributing\n\nPlease check the instructions in [CONTRIBUTING.md](.github/
-CONTRIBUTING.md).\n\n## API stability\n\n:warning: While `coola` is in
-development stage, no API is guaranteed to be stable from one\nrelease to the
-next.\nIn fact, it is very likely that the API will change multiple times
-before a stable 1.0.0 release.\nIn practice, this means that upgrading `coola`
-to a new version will possibly break any code that\nwas using the old version
-of `coola`.\n\n## License\n\n`coola` is licensed under BSD 3-Clause "New" or
-"Revised" license available in [LICENSE](LICENSE)\nfile.\n', 'author': 'Thibaut
-Durand', 'author_email': 'durand.tibo+gh@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/durandtibo/coola',
-'package_dir': package_dir, 'packages': packages, 'package_data': package_data,
-'extras_require': extras_require, 'python_requires': '>=3.9,<4.0', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: coola Version: 0.0.5 Summary: A light library to
+check if two complex/nested objects are equal or not Home-page: https://
+github.com/durandtibo/coola License: BSD-3-Clause Keywords: equality,complex/
+nested objects Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com
+Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Information Technology Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Software Development :: Libraries Provides-Extra: all Requires-Dist: numpy
+(>=1.20,<2.0) ; extra == "all" Requires-Dist: torch (>=1.10,<3.0) ; extra ==
+"all" Project-URL: Repository, https://github.com/durandtibo/coola Description-
+Content-Type: text/markdown # coola
+[CI] [PYPI_version] [Python] [BSD-3-Clause] [Codecov] [Code_style:_black] [Doc
+                                style:_google]
+                       [Downloads] [Monthly_downloads]
+## Overview `coola` is a light Python library that provides simple functions to
+check in a single line if two complex/nested objects are equal or not. `coola`
+was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
+docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
+reference/generated/numpy.ndarray.html), but it is possible to extend it to
+[support other data structures](https://durandtibo.github.io/coola/
+customization). - [Motivation](#motivation) - [Documentation](https://
+durandtibo.github.io/coola/) - [Installation](#installation) - [Contributing]
+(#contributing) - [API stability](#api-stability) - [License](#license) ##
+Motivation Let's imagine you have the following dictionaries that contain both
+a PyTorch `Tensor` and a NumPy `ndarray`. You want to check if the two
+dictionaries are equal or not. By default, Python does not provide an easy way
+to check if the two dictionaries are equal or not. It is not possible to use
+the default equality operator `==` because it will raise an error. The `coola`
+library was developed to fill this gap. `coola` provides a function
+`objects_are_equal` that can indicate if two complex/nested objects are equal
+or not. ```python import numpy import torch from coola import objects_are_equal
+data1 = {'torch': torch.ones(2, 3), 'numpy': numpy.zeros((2, 3))} data2 =
+{'torch': torch.zeros(2, 3), 'numpy': numpy.ones((2, 3))} objects_are_equal
+(data1, data2) ``` `coola` also provides a function `objects_are_allclose` that
+can indicate if two complex/nested objects are equal within a tolerance or not.
+```python from coola import objects_are_allclose objects_are_allclose(data1,
+data2, atol=1e-6) ``` Please check the [quickstart page](https://
+durandtibo.github.io/coola/quickstart) to learn more on how to use `coola`. ##
+Installation We highly recommend installing a [virtual environment](https://
+packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
+`coola` can be installed from pip using the following command: ```shell pip
+install coola ``` To make the package as slim as possible, only the minimal
+packages required to use `coola` are installed. To include all the packages,
+you can use the following command: ```shell pip install coola[all] ``` Please
+check the [get started page](https://durandtibo.github.io/coola/get_started) to
+see how to install only some specific packages or other alternatives to install
+the library. ## Contributing Please check the instructions in [CONTRIBUTING.md]
+(.github/CONTRIBUTING.md). ## API stability :warning: While `coola` is in
+development stage, no API is guaranteed to be stable from one release to the
+next. In fact, it is very likely that the API will change multiple times before
+a stable 1.0.0 release. In practice, this means that upgrading `coola` to a new
+version will possibly break any code that was using the old version of `coola`.
+## License `coola` is licensed under BSD 3-Clause "New" or "Revised" license
+available in [LICENSE](LICENSE) file.
```

