# Comparing `tmp/pipe-utils-0.2.2.tar.gz` & `tmp/pipe-utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipe-utils-0.2.2.tar", last modified: Sat Apr  1 00:19:13 2023, max compression
+gzip compressed data, was "pipe-utils-0.3.0.tar", last modified: Sat Apr 15 08:01:21 2023, max compression
```

## Comparing `pipe-utils-0.2.2.tar` & `pipe-utils-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2023-04-01 00:19:13.144224 pipe-utils-0.2.2/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     1076 2023-02-19 11:27:38.000000 pipe-utils-0.2.2/LICENSE
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2576 2023-04-01 00:19:13.144101 pipe-utils-0.2.2/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002      821 2023-03-18 08:54:22.000000 pipe-utils-0.2.2/README.md
--rw-r--r--   0 jfin305  (1356368322) 1403514002      725 2023-03-31 06:45:27.000000 pipe-utils-0.2.2/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) 1403514002       19 2023-03-15 06:03:58.000000 pipe-utils-0.2.2/requirements.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2023-04-01 00:19:13.144262 pipe-utils-0.2.2/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2023-04-01 00:19:13.140507 pipe-utils-0.2.2/src/
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2023-04-01 00:19:13.142009 pipe-utils-0.2.2/src/pipe_utils/
--rw-r--r--   0 jfin305  (1356368322) 1403514002      147 2023-03-17 02:53:06.000000 pipe-utils-0.2.2/src/pipe_utils/__init__.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     1371 2023-04-01 00:17:51.000000 pipe-utils-0.2.2/src/pipe_utils/_types.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002    22391 2023-03-31 20:33:53.000000 pipe-utils-0.2.2/src/pipe_utils/iterables.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3561 2023-03-15 02:22:25.000000 pipe-utils-0.2.2/src/pipe_utils/mappings.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002      939 2023-04-01 00:00:18.000000 pipe-utils-0.2.2/src/pipe_utils/override.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002    14069 2023-04-01 00:18:34.000000 pipe-utils-0.2.2/src/pipe_utils/pipe.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002      472 2023-03-15 06:42:50.000000 pipe-utils-0.2.2/src/pipe_utils/utils.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     8928 2023-04-01 00:03:08.000000 pipe-utils-0.2.2/src/pipe_utils/values.py
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2023-04-01 00:19:13.142636 pipe-utils-0.2.2/src/pipe_utils.egg-info/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2576 2023-04-01 00:19:13.000000 pipe-utils-0.2.2/src/pipe_utils.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002      571 2023-04-01 00:19:13.000000 pipe-utils-0.2.2/src/pipe_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2023-04-01 00:19:13.000000 pipe-utils-0.2.2/src/pipe_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002       19 2023-04-01 00:19:13.000000 pipe-utils-0.2.2/src/pipe_utils.egg-info/requires.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002       11 2023-04-01 00:19:13.000000 pipe-utils-0.2.2/src/pipe_utils.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2023-04-01 00:19:13.143923 pipe-utils-0.2.2/tests/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     6511 2023-03-17 02:15:34.000000 pipe-utils-0.2.2/tests/test_it.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002    22888 2023-03-31 20:31:39.000000 pipe-utils-0.2.2/tests/test_iterables.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3213 2023-03-15 05:39:19.000000 pipe-utils-0.2.2/tests/test_mappings.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2475 2023-03-31 23:56:58.000000 pipe-utils-0.2.2/tests/test_override.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3762 2023-03-31 21:21:37.000000 pipe-utils-0.2.2/tests/test_pipe.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     8432 2023-03-31 23:57:08.000000 pipe-utils-0.2.2/tests/test_values.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-15 08:01:21.723412 pipe-utils-0.3.0/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2023-02-19 11:27:38.000000 pipe-utils-0.3.0/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2606 2023-04-15 08:01:21.723267 pipe-utils-0.3.0/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      851 2023-04-15 07:42:41.000000 pipe-utils-0.3.0/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      725 2023-04-15 08:01:13.000000 pipe-utils-0.3.0/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       19 2023-04-02 23:35:59.000000 pipe-utils-0.3.0/requirements.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-04-15 08:01:21.723456 pipe-utils-0.3.0/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-15 08:01:21.717620 pipe-utils-0.3.0/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-15 08:01:21.720517 pipe-utils-0.3.0/src/pipe_utils/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      147 2023-03-17 02:53:06.000000 pipe-utils-0.3.0/src/pipe_utils/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1515 2023-04-08 06:45:53.000000 pipe-utils-0.3.0/src/pipe_utils/_types.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)    26573 2023-04-15 07:09:17.000000 pipe-utils-0.3.0/src/pipe_utils/iterables.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3561 2023-03-15 02:22:25.000000 pipe-utils-0.3.0/src/pipe_utils/mappings.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      959 2023-04-02 08:33:16.000000 pipe-utils-0.3.0/src/pipe_utils/override.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)    14582 2023-04-15 06:35:10.000000 pipe-utils-0.3.0/src/pipe_utils/pipe.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3323 2023-04-02 09:19:57.000000 pipe-utils-0.3.0/src/pipe_utils/values.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-15 08:01:21.721277 pipe-utils-0.3.0/src/pipe_utils.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2606 2023-04-15 08:01:21.000000 pipe-utils-0.3.0/src/pipe_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      547 2023-04-15 08:01:21.000000 pipe-utils-0.3.0/src/pipe_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-04-15 08:01:21.000000 pipe-utils-0.3.0/src/pipe_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       19 2023-04-15 08:01:21.000000 pipe-utils-0.3.0/src/pipe_utils.egg-info/requires.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       11 2023-04-15 08:01:21.000000 pipe-utils-0.3.0/src/pipe_utils.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-15 08:01:21.722935 pipe-utils-0.3.0/tests/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6511 2023-03-17 02:15:34.000000 pipe-utils-0.3.0/tests/test_it.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)    27797 2023-04-15 06:54:12.000000 pipe-utils-0.3.0/tests/test_iterables.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3213 2023-03-15 05:39:19.000000 pipe-utils-0.3.0/tests/test_mappings.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2830 2023-04-02 05:29:01.000000 pipe-utils-0.3.0/tests/test_override.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4528 2023-04-02 05:32:42.000000 pipe-utils-0.3.0/tests/test_pipe.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3678 2023-04-02 09:20:53.000000 pipe-utils-0.3.0/tests/test_values.py
```

### Comparing `pipe-utils-0.2.2/LICENSE` & `pipe-utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipe-utils-0.2.2/PKG-INFO` & `pipe-utils-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipe-utils
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python with pipes, utils, and pipe utils
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -26,15 +26,15 @@
         
 Project-URL: repository, https://github.com/James-Ansley/pipe-utils
 Project-URL: documentation, https://pipe-utils.rtfd.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pipe Utils
 
 Python with pipes, utils, and pipe utils.
 
@@ -42,15 +42,15 @@
 
 ```
 pip install pipe-utils
 ```
 
 ## Docs
 
-https://pipe-utils.rtfd.io
+[https://pipe-utils.rtfd.io](https://pipe-utils.rtfd.io)
 
 ## Example
 
 ```python
 from pipe_utils import *
 
 words = "I just think pipes are neat"
@@ -64,15 +64,15 @@
 ).get()
 
 print(result)
 #  {1: ['i'], 3: ['are'], 4: ['just', 'neat'], 5: ['think', 'pipes']}
 ```
 
 And, if you're feeling dangerous, override builtin functions
-like `filter`, `map`, and `all` by importing from `pipe-utils.override`:
+like `filter`, `map`, and `all` by importing from `pipe_utils.override`:
 
 ```python
 from pipe_utils.override import *
 
 data = [[1, -3, 4], [1, 2, 3], [2, 3, 4], [5, -1, 4]]
 
 result = (
```

### Comparing `pipe-utils-0.2.2/README.md` & `pipe-utils-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ```
 pip install pipe-utils
 ```
 
 ## Docs
 
-https://pipe-utils.rtfd.io
+[https://pipe-utils.rtfd.io](https://pipe-utils.rtfd.io)
 
 ## Example
 
 ```python
 from pipe_utils import *
 
 words = "I just think pipes are neat"
@@ -28,15 +28,15 @@
 ).get()
 
 print(result)
 #  {1: ['i'], 3: ['are'], 4: ['just', 'neat'], 5: ['think', 'pipes']}
 ```
 
 And, if you're feeling dangerous, override builtin functions
-like `filter`, `map`, and `all` by importing from `pipe-utils.override`:
+like `filter`, `map`, and `all` by importing from `pipe_utils.override`:
 
 ```python
 from pipe_utils.override import *
 
 data = [[1, -3, 4], [1, 2, 3], [2, 3, 4], [5, -1, 4]]
 
 result = (
```

### Comparing `pipe-utils-0.2.2/pyproject.toml` & `pipe-utils-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pipe-utils"
-version = "0.2.2"
+version = "0.3.0"
 description = "Python with pipes, utils, and pipe utils"
 
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Utilities",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `pipe-utils-0.2.2/src/pipe_utils/_types.py` & `pipe-utils-0.3.0/src/pipe_utils/_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections.abc import Callable, Hashable, Iterable, Mapping
-from typing import Type, TypeVar
+from typing import Any, Type, TypeVar
 
 __all__ = [
     # Singleton
     "nothing",
 
     # Generic Types
     "T",
     "V",
+    "R",
     "K",
     "H",
     "E",
     "EType",
     "ExceptionHandler",
     "NestedIter",
 
@@ -28,15 +29,17 @@
     "Reducer",
     "OptionalReducer",
     "Consumer",
 
     # FuncUtils
     "Action",
     "Function",
+    "IndexedFunction",
     "Predicate",
+    "IndexedPredicate",
 ]
 
 nothing = object()
 
 T = TypeVar("T")
 V = TypeVar("V")
 R = TypeVar("R")
@@ -57,10 +60,12 @@
 Reducer = Callable[[Iterable[T]], T]
 OptionalReducer = Callable[[Iterable[T]], T | None]
 BoolReducer = Callable[[Iterable[T]], bool]
 IntReducer = Callable[[Iterable[T]], int]
 StrReducer = Callable[[Iterable[T]], str]
 Consumer = Callable[[Iterable[T]], None]
 
-Action = Callable[[T], None]
+Action = Callable[[T], Any]
 Function = Callable[[T], V]
+IndexedFunction = Callable[[int, T], V]
 Predicate = Callable[[T], bool]
+IndexedPredicate = Callable[[int, T], bool]
```

### Comparing `pipe-utils-0.2.2/src/pipe_utils/iterables.py` & `pipe-utils-0.3.0/src/pipe_utils/iterables.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Contains several utility functions to support processing iterables
 """
 
 import functools
 import itertools
 from collections import defaultdict, deque
-from collections.abc import Callable, Iterable, Mapping, Sequence
+from collections.abc import Callable, Iterable, Mapping, Reversible, Sequence
 from typing import overload
 
+from deprecated.sphinx import deprecated
+
 from ._types import *
 
 __all__ = [
     "all_",
     "any_",
     "associate",
     "associate_with",
@@ -23,16 +25,19 @@
     "count",
     "distinct",
     "distinct_by",
     "drop",
     "drop_last",
     "drop_last_while",
     "drop_while",
+    "extend",
+    "extend_left",
     "filter_",
     "filter_false",
+    "filter_indexed",
     "find",
     "find_last",
     "first",
     "flatten",
     "flat_map",
     "fold",
     "for_each",
@@ -41,42 +46,49 @@
     "get_or_default",
     "is_empty",
     "is_not_empty",
     "index_of",
     "index_of_last",
     "join_to_str",
     "last",
+    "lstrip",
     "map_",
+    "map_indexed",
     "max_by",
     "min_by",
     "none",
     "not_contains",
     "pad_with",
     "partition",
     "peek",
     "reduce",
     "remove",
     "remove_last",
+    "replace",
+    "rstrip",
     "scan",
     "slice_",
     "sorted_by",
     "sorted_desc",
     "sorted_desc_by",
     "split_by",
     "starmap",
     "starred",
+    "strip",
+    "strip_while",
     "sum_by",
     "take",
     "take_last",
     "take_last_while",
     "take_while",
     "to_each",
     "transpose",
     "try_map",
     "windowed",
+    "wrap",
     "unzip",
 ]
 
 
 def all_(func: Predicate) -> BoolReducer:
     """
     Returns a callable that returns True iff all items in an iterable satisfy
@@ -111,34 +123,56 @@
     func(t) -> v
 
     Duplicate key items are ignored.
     """
     return lambda data: {k: func(k) for k in data}
 
 
-def chunked(n: int) -> NestedIterCurry:
-    """Returns a callable that yields items split into chunks of size n"""
+def chunked(
+        n: int, *, strict: bool = True, partial: bool = False,
+) -> NestedIterCurry:
+    """
+    Returns a callable that yields items split into chunks of size n. If
+    partial is True, also yields trailing chunk even if it has fewer than n
+    items. If strict is True (and partial is False), will raise a value error
+    if there are fewer than n trailing items at the end of the chunk sequence.
+    """
     if n <= 0:
         raise ValueError("Cannot yield non-positive chunk sizes")
 
     def _func(data):
         data = iter(data)
         while chunk := tuple(itertools.islice(data, n)):
-            yield chunk
+            if len(chunk) == n:
+                yield chunk
+            elif partial:
+                yield chunk
+            elif strict:
+                raise ValueError(
+                    "Chunked iterator has trailing items in strict mode"
+                )
 
     return _func
 
 
+@deprecated(
+    version="0.3.0",
+    reason="Use `extend` instead for consistency with Python naming"
+)
 def concat(other: Iterable[T]) -> IterCurry:
-    """Returns a callable that yield [\\*data, \\*other]"""
+    """Returns a callable that yields [\\*data, \\*other]"""
     return lambda data: itertools.chain(data, other)
 
 
+@deprecated(
+    version="0.3.0",
+    reason="Use `extend_left` instead for consistency with Python naming"
+)
 def concat_after(other: Iterable[T]) -> IterCurry:
-    """Returns a callable that yield [\\*other, \\*data]"""
+    """Returns a callable that yields [\\*other, \\*data]"""
     return lambda data: itertools.chain(other, data)
 
 
 def contains(value: T) -> BoolReducer:
     """
     Returns a callable that returns True if the given iterable contains the
     value
@@ -250,14 +284,34 @@
     """
     Returns a callable that drops the items of an iterable while the
     predicate is True
     """
     return lambda data: itertools.dropwhile(func, data)
 
 
+def extend(other: Iterable[T]) -> IterCurry:
+    """Returns a callable that yields ≈ [\\*data, \\*other]"""
+    return lambda data: itertools.chain(data, other)
+
+
+def extend_left(other: Iterable[T], *, reverse: bool = False) -> IterCurry:
+    """
+    Returns a callable that yields ≈ [\\*other, \\*data]. This does *not*
+    reverse the ``other`` iterable as other similar function do in Python by
+    default. However, calling with reverse = True will yield the equivalent
+    of [ \\*reversed(other), \\*data] even if ``other`` has no default
+    reverse iterator.
+    """
+    if reverse and isinstance(other, Reversible):
+        other = reversed(other)
+    elif reverse:
+        other = reversed(tuple(other))
+    return lambda data: itertools.chain(other, data)
+
+
 def filter_(func: Predicate) -> IterCurry:
     """
     Returns a callable that returns an iterator yielding those items of
     the iterable for which func(item) is true.
     """
     return lambda data: filter(func, data)
 
@@ -266,14 +320,30 @@
     """
     Returns a callable that returns an iterator yielding those items of
     the iterable for which func(item) is false.
     """
     return lambda data: itertools.filterfalse(func, data)
 
 
+def filter_indexed(func: IndexedPredicate, *, start: int = 0) -> IterCurry:
+    """
+    Returns a callable that returns an iterator yielding those items of the
+    iterable for which func(i, item) is true where i is the position of the
+    current item offset by the given start value.
+    """
+
+    def _func(data):
+        data = enumerate(data, start=start)
+        for i, e in data:
+            if func(i, e):
+                yield e
+
+    return _func
+
+
 def find(func: Predicate) -> OptionalReducer:
     """
     Returns a callable that returns the first item that satisfies the given
     predicate or None
     """
     return lambda data: next((e for e in data if func(e)), None)
 
@@ -331,15 +401,15 @@
     return lambda data: functools.reduce(
         func, itertools.chain((initial,), data)
     )
 
 
 def for_each(func: Callable[[T], None]) -> Consumer:
     """
-    Returns a callable that eagerly applies func to each item in a given
+    Returns a callable that eagerly calls func for each item in a given
     iterable
     """
 
     def _func(data):
         for e in data:
             func(e)
 
@@ -474,22 +544,38 @@
         for e in it:
             window.append(e)
         return window
 
     return _func
 
 
+def lstrip(value: T) -> IterCurry:
+    """
+    returns a callable that strips all leading values equal to the given value
+    """
+    return drop_while(lambda e: e == value)
+
+
 def map_(func: Function) -> IterMapCurry:
     """
     Returns a callable that returns an iterator yielding those items of
     the iterable mapped with the function func(item)
     """
     return lambda data: map(func, data)
 
 
+def map_indexed(func: IndexedFunction, *, start: int = 0) -> IterMapCurry:
+    """
+    Returns a callable that returns an iterator yielding those items of the
+    iterable mapped with the function func(i, item) where i in the position
+    of the current item in the iterable offset with the given start value.
+    """
+    return lambda data: itertools.starmap(func, enumerate(data, start=start))
+
+
 def max_by(func: Function) -> Reducer:
     """
     Returns a callable that returns the item with the max value using the key
     function
     """
     return lambda data: max(data, key=func)
 
@@ -607,14 +693,35 @@
         if queue:
             queue.popleft()
         yield from queue
 
     return _func
 
 
+def replace(old: T, new: V) -> Callable[[Iterable[T]], Iterable[T | V]]:
+    """Returns a callable that replaces all occurrences of *old* with *new*"""
+
+    def func(data):
+        for e in data:
+            if e != old:
+                yield e
+            else:
+                yield new
+
+    return func
+
+
+def rstrip(value: T):
+    """
+    returns a callable that strips all trailing values in an iterable which are
+    equal to the given value
+    """
+    return drop_last_while(lambda e: e == value)
+
+
 def scan(func: Callable[[T, T], T], initial=None) -> IterCurry:
     """Returns a callable that yields accumulated values"""
     return lambda data: itertools.accumulate(data, func, initial=initial)
 
 
 @overload
 def slice_(stop: int) -> IterCurry:
@@ -690,14 +797,33 @@
     """
     Returns a callable that takes in data and calls func with the data starred.
     Kwargs are passed to the function.
     """
     return lambda data: func(*data, **kwargs)
 
 
+def strip(value: T) -> IterCurry:
+    """
+    returns a callable that strips all leading and trailing values equal to
+    the given value
+    """
+    return strip_while(lambda e: e == value)
+
+
+def strip_while(func: Predicate) -> IterCurry:
+    """
+    returns a callable that strips all leading and trailing values that
+    satisfy the given predicate.
+
+    Use :func:`drop_while` and :func:`drop_last_while` for the equivalent
+    left and right counterparts
+    """
+    return lambda data: drop_last_while(func)(drop_while(func)(data))
+
+
 def sum_by(func: Callable[[T], V], start: V = 0) -> Callable[[Iterable[T]], V]:
     """Returns a callable that sums an iterable by the given function"""
     return lambda data: sum((func(e) for e in data), start=start)
 
 
 def take(n: int = 1) -> IterCurry:
     """
@@ -768,35 +894,33 @@
 def transpose(data: NestedIter) -> NestedIter:
     """Returns the data transposed. e.g. [[1, 2], [3, 4]] -> [[1, 3], [2, 4]]"""
     return zip(*data)
 
 
 def try_map(
         func: Function,
-        err: EType = Exception,
-        default: V = None,
+        catch: EType = Exception,
         *,
-        ignore_errors: bool = False
+        default: V = nothing,
 ) -> IterMapCurry:
     """
     Returns a callable that attempts to map each item in an iterable.
 
     :param func: The mapping function
-    :param err: The error type(s) that will be excepted
+    :param catch: The error type(s) that will be excepted
     :param default: The value that will be used if the error type err is raised
-    :param ignore_errors: If False, the default value will replace values that
-        error, otherwise values that error are skipped
+        – if not provided the error is simply ignored and no value is yielded
     """
 
     def _func(data):
         for e in data:
             try:
                 yield func(e)
-            except err:
-                if not ignore_errors:
+            except catch:
+                if default is not nothing:
                     yield default
 
     return _func
 
 
 def windowed(
         n: int, *, strict: bool = True, partial: bool = False
@@ -847,7 +971,19 @@
     the given data, the second iterable contains the second element form the
     given data
     """
     if isinstance(data, Mapping):
         return data.keys(), data.values()
     thing1, thing2 = itertools.tee(data, 2)
     return (e[0] for e in thing1), (e[1] for e in thing2)
+
+
+def wrap(other: Iterable[T], *, reverse_left: bool = False) -> IterCurry:
+    """
+    Returns a callable that yields ≈ [\\*other, \\*data, \\*other]
+    if ``reverse_left`` is True, yields the equivalent of
+    [\\*reversed(other), \\*data, \\*other]
+    """
+    other1, other2 = itertools.tee(other, 2)
+    if reverse_left:
+        other1 = reversed(tuple(other1))
+    return lambda data: itertools.chain(other1, data, other2)
```

### Comparing `pipe-utils-0.2.2/src/pipe_utils/mappings.py` & `pipe-utils-0.3.0/src/pipe_utils/mappings.py`

 * *Files identical despite different names*

### Comparing `pipe-utils-0.2.2/src/pipe_utils/override.py` & `pipe-utils-0.3.0/src/pipe_utils/override.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # noinspection PyUnresolvedReferences
 from .iterables import *
 # noinspection PyUnresolvedReferences
 from .mappings import *
 # noinspection PyUnresolvedReferences
 from .values import *
 
-# noinspection PyUnresolvedReferences
+# noinspection PyUnresolvedReferences,PyShadowingBuiltins
 from .iterables import (
     filter_ as filter,
     map_ as map,
     all_ as all,
     any_ as any,
     slice_ as slice,
 )
```

### Comparing `pipe-utils-0.2.2/src/pipe_utils/pipe.py` & `pipe-utils-0.3.0/src/pipe_utils/pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """
 
     def __init__(self, exception: EType, handler: ExceptionHandler):
         self.exception = exception
         self.handler = handler
 
 
-class Pipe(Generic[T, R]):
+class Pipe(Generic[T]):
     """
     Pipe class that supports chained operations on the given data. If an
     error occurs during the chaining process, the pipe goes into error
     state. The error must either be caught by calling ``.catch`` or ignored
     when yielding data with ``get_or_default`` or ``get_or_raise``
     """
 
@@ -83,37 +83,40 @@
             return self.then(other)
         elif isinstance(other, Iterable):
             return self.then(*other)
         elif isinstance(other, Then):
             return self.then(other.func, *other.args, **other.kwargs)
         elif isinstance(other, Catch):
             return self.catch(other.exception, other.handler)
-        raise ValueError(f"cannot perform pipe with type {type(other)}")
+        else:
+            raise ValueError(f"cannot perform pipe with type {type(other)}")
 
     def catch(
             self,
             exception: EType,
             handler: ExceptionHandler,
     ) -> "Pipe[T | R]":
         """
         Catches the given exception if it has been raised and returns a new
         Pipe containing the result of the handler
         """
         if isinstance(self._err, exception):
             return Pipe(handler(self._err))
-        return self
+        else:
+            return self
 
     def get(self):
         """
         Returns the result of the pipe or raises the first error encountered
         when chaining functions
         """
         if self._err is not None:
             raise self._err
-        return self._data
+        else:
+            return self._data
 
     def get_or_default(
             self, default: V = None, *, catch: EType = Exception
     ) -> T | V:
         """
         Returns the result of the pipe or the default value if the pipe is in
         error state and the error is of type :code:`catch`. If the error is
@@ -123,25 +126,37 @@
             return self._data
         elif isinstance(self._err, catch):
             return default
         else:
             raise self._err
 
     def get_or_raise(
-            self, exception: E | Type[E], *, catch: EType = Exception,
+            self,
+            exception: E | Type[E],
+            *,
+            catch: EType = Exception,
+            chained: bool = True,
     ) -> T:
         """
         Returns the result of the pipe or raises the given exception if the
         pipe is in error state and the error is of type :code:`catch`. If the
-        error is not of type :code:`catch`, the error itself is raised instead.
+        error is not of type :code:`catch`, the error itself is raised
+        instead.
+
+        If ``chained`` is ``True``, the given exception will be
+        raised from the exception currently in the ``Pipe`` object.
+        Otherwise, the given exception is raised as is – but may still be
+        chained if this is raised during the handling of another exception.
         """
         if self._err is None:
             return self._data
-        elif isinstance(self._err, catch):
+        elif isinstance(self._err, catch) and chained:
             raise exception from self._err
+        elif isinstance(self._err, catch) and not chained:
+            raise exception
         else:
             raise self._err
 
 
 class _It:
     def __init__(self, call=None):
         if call is None:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pipe-utils-0.2.2/src/pipe_utils.egg-info/PKG-INFO` & `pipe-utils-0.3.0/src/pipe_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipe-utils
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python with pipes, utils, and pipe utils
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -26,15 +26,15 @@
         
 Project-URL: repository, https://github.com/James-Ansley/pipe-utils
 Project-URL: documentation, https://pipe-utils.rtfd.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pipe Utils
 
 Python with pipes, utils, and pipe utils.
 
@@ -42,15 +42,15 @@
 
 ```
 pip install pipe-utils
 ```
 
 ## Docs
 
-https://pipe-utils.rtfd.io
+[https://pipe-utils.rtfd.io](https://pipe-utils.rtfd.io)
 
 ## Example
 
 ```python
 from pipe_utils import *
 
 words = "I just think pipes are neat"
@@ -64,15 +64,15 @@
 ).get()
 
 print(result)
 #  {1: ['i'], 3: ['are'], 4: ['just', 'neat'], 5: ['think', 'pipes']}
 ```
 
 And, if you're feeling dangerous, override builtin functions
-like `filter`, `map`, and `all` by importing from `pipe-utils.override`:
+like `filter`, `map`, and `all` by importing from `pipe_utils.override`:
 
 ```python
 from pipe_utils.override import *
 
 data = [[1, -3, 4], [1, 2, 3], [2, 3, 4], [5, -1, 4]]
 
 result = (
```

### Comparing `pipe-utils-0.2.2/src/pipe_utils.egg-info/SOURCES.txt` & `pipe-utils-0.3.0/src/pipe_utils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 requirements.txt
 src/pipe_utils/__init__.py
 src/pipe_utils/_types.py
 src/pipe_utils/iterables.py
 src/pipe_utils/mappings.py
 src/pipe_utils/override.py
 src/pipe_utils/pipe.py
-src/pipe_utils/utils.py
 src/pipe_utils/values.py
 src/pipe_utils.egg-info/PKG-INFO
 src/pipe_utils.egg-info/SOURCES.txt
 src/pipe_utils.egg-info/dependency_links.txt
 src/pipe_utils.egg-info/requires.txt
 src/pipe_utils.egg-info/top_level.txt
 tests/test_it.py
```

### Comparing `pipe-utils-0.2.2/tests/test_it.py` & `pipe-utils-0.3.0/tests/test_it.py`

 * *Files identical despite different names*

### Comparing `pipe-utils-0.2.2/tests/test_iterables.py` & `pipe-utils-0.3.0/tests/test_iterables.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 from fractions import Fraction
 from io import StringIO
 from operator import add
 
+import pytest
 from pytest import raises
 
 from pipe_utils import Pipe, it
 from pipe_utils.iterables import *
 
 
 def is_even(e):
@@ -52,55 +53,80 @@
     pipe = (
             Pipe(range(9))
             | chunked(3)
             | map_(list)
             | list
     )
     assert pipe.get() == [[0, 1, 2], [3, 4, 5], [6, 7, 8]]
+    pipe = (
+            Pipe(range(10))
+            | chunked(3, partial=True)
+            | map_(list)
+            | list
+    )
+    assert pipe.get() == [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]]
+    pipe = (
+            Pipe(range(10))
+            | chunked(3, strict=False)
+            | map_(list)
+            | list
+    )
+    assert pipe.get() == [[0, 1, 2], [3, 4, 5], [6, 7, 8]]
+    pipe = (
+            Pipe(range(10))
+            | chunked(3, strict=False, partial=True)
+            | map_(list)
+            | list
+    )
+    assert pipe.get() == [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]]
 
     with raises(ValueError):
         Pipe([]) | chunked(0)
     with raises(ValueError):
         Pipe([]) | chunked(-1)
+    with raises(ValueError):
+        (Pipe(range(10)) | chunked(3) | map_(list) | list).get()
 
 
 def test_concat():
-    assert (Pipe([]) | concat([]) | list).get() == []
-    assert (Pipe(["a"]) | concat([]) | list).get() == ["a"]
-    assert (Pipe([]) | concat(["b"]) | list).get() == ["b"]
-    assert (Pipe(["a"]) | concat(["b"]) | list).get() == ["a", "b"]
-    pipe = (Pipe(["a", "b", "c"])
-            | concat(["d", "e", "f"])
-            | list)
-    assert pipe.get() == list("abcdef")
+    with pytest.deprecated_call():
+        assert (Pipe([]) | concat([]) | list).get() == []
+        assert (Pipe(["a"]) | concat([]) | list).get() == ["a"]
+        assert (Pipe([]) | concat(["b"]) | list).get() == ["b"]
+        assert (Pipe(["a"]) | concat(["b"]) | list).get() == ["a", "b"]
+        pipe = (Pipe(["a", "b", "c"])
+                | concat(["d", "e", "f"])
+                | list)
+        assert pipe.get() == list("abcdef")
 
 
 def test_concat_after():
-    assert (Pipe([]) | concat_after([]) | list).get() == []
-    assert (Pipe(["a"]) | concat_after([]) | list).get() == ["a"]
-    assert (Pipe([]) | concat_after(["b"]) | list).get() == ["b"]
-    assert (Pipe(["a"]) | concat_after(["b"]) | list).get() == ["b", "a"]
-    pipe = (Pipe(["a", "b", "c"])
-            | concat_after(["d", "e", "f"])
-            | list)
-    assert pipe.get() == list("defabc")
+    with pytest.deprecated_call():
+        assert (Pipe([]) | concat_after([]) | list).get() == []
+        assert (Pipe(["a"]) | concat_after([]) | list).get() == ["a"]
+        assert (Pipe([]) | concat_after(["b"]) | list).get() == ["b"]
+        assert (Pipe(["a"]) | concat_after(["b"]) | list).get() == ["b", "a"]
+        pipe = (Pipe(["a", "b", "c"])
+                | concat_after(["d", "e", "f"])
+                | list)
+        assert pipe.get() == list("defabc")
 
 
 def test_contains():
     assert (Pipe([]) | contains(0)).get() is False
     assert (Pipe([-1, 1]) | contains(0)).get() is False
     assert (Pipe([-1, 0, 1]) | contains(0)).get() is True
-    assert (Pipe([-1]) | concat([0]) | contains(0)).get() is True
+    assert (Pipe([-1]) | extend([0]) | contains(0)).get() is True
 
 
 def test_contains_all():
     assert (Pipe([]) | contains_all([0])).get() is False
     assert (Pipe([-1, 1]) | contains_all([0, 1])).get() is False
     assert (Pipe([-1, 0, 1]) | contains_all([0, -1])).get() is True
-    assert (Pipe([-1]) | concat([0]) | contains_all([-1, 0])).get() is True
+    assert (Pipe([-1]) | extend([0]) | contains_all([-1, 0])).get() is True
 
 
 def test_count():
     assert (Pipe([]) | count(0)).get() == 0
     assert (Pipe([-1, 1]) | count(0)).get() == 0
     assert (Pipe([-1, 0, 1]) | count(0)).get() == 1
     assert (Pipe([-1, 0, 1, 0, 0]) | count(0)).get() == 3
@@ -166,27 +192,65 @@
 def test_drop_while():
     assert (Pipe([]) | drop_while(is_even) | list).get() == []
     assert (Pipe([0, 1, 2]) | drop_while(is_even) | list).get() == [1, 2]
     assert (Pipe([1, 2, 3]) | drop_while(is_even) | list).get() == [1, 2, 3]
     assert (Pipe([0, 0, 0]) | drop_while(is_even) | list).get() == []
 
 
+def test_extend():
+    assert (Pipe([]) | extend([]) | list).get() == []
+    assert (Pipe(["a"]) | extend([]) | list).get() == ["a"]
+    assert (Pipe([]) | extend(["b"]) | list).get() == ["b"]
+    assert (Pipe(["a"]) | extend(["b"]) | list).get() == ["a", "b"]
+    pipe = (Pipe(["a", "b", "c"])
+            | extend(["d", "e", "f"])
+            | list)
+    assert pipe.get() == list("abcdef")
+
+
+def test_extend_left():
+    assert (Pipe([]) | extend_left([]) | list).get() == []
+    assert (Pipe(["a"]) | extend_left([]) | list).get() == ["a"]
+    assert (Pipe([]) | extend_left(["b"]) | list).get() == ["b"]
+    assert (Pipe(["a"]) | extend_left(["b"]) | list).get() == ["b", "a"]
+    pipe = (Pipe(["a", "b", "c"])
+            | extend_left(["d", "e", "f"])
+            | list)
+    assert pipe.get() == list("defabc")
+    pipe = (Pipe(["a", "b", "c"])
+            | extend_left(["d", "e", "f"], reverse=True)
+            | list)
+    assert pipe.get() == list("fedabc")
+    pipe = (Pipe(["a", "b", "c"])
+            | extend_left(iter(["d", "e", "f"]), reverse=True)
+            | list)
+    assert pipe.get() == list("fedabc")
+
+
 def test_filter():
     assert (Pipe([]) | filter_(is_even) | list).get() == []
     pipe = Pipe(range(11)) | filter_(is_even) | list
     assert pipe.get() == [0, 2, 4, 6, 8, 10]
 
 
 def test_filter_false():
     assert (Pipe([]) | filter_false(is_even) | list).get() == []
     assert (Pipe([-1, 0, 1]) | filter_false(is_even) | list).get() == [-1, 1]
     pipe = (Pipe(range(11)) | filter_false(is_even) | list)
     assert pipe.get() == [1, 3, 5, 7, 9]
 
 
+def test_filter_indexed():
+    data = [-4, 2, 6, -2, 8, 3, 0]
+    assert [*filter_indexed(lambda i, e: i % 2 == 0 and e > 0)(data)] == [6, 8]
+    assert [*filter_indexed(lambda i, e: i % 2 == 0 and e > 0)([])] == []
+    assert [*filter_indexed(lambda i, e: i % 2 == 0 and e > 0, start=1)(data)] \
+           == [2, 3]
+
+
 def test_find():
     assert (Pipe([]) | find(is_even)).get() is None
     assert (Pipe([1, 2, 3, 4]) | find(is_even)).get() == 2
     assert (Pipe([1, 3, 5, 7]) | find(is_even)).get() is None
 
 
 def test_find_last():
@@ -223,24 +287,25 @@
 
 def test_fold():
     assert (Pipe([]) | fold(1, add)).get() == 1
     assert (Pipe([1]) | fold(1, add)).get() == 2
     assert (Pipe([1, 2, 3]) | fold(1, add)).get() == 7
 
 
-# noinspection PyShadowingNames,PyDefaultArgument
+# noinspection PyDefaultArgument
 def test_for_each():
     res = []
-    Pipe([]) | for_each(lambda e, res=res: res.append(e))
+    Pipe([]) | for_each(lambda e, r=res: r.append(e))
     assert res == []
     res = []
-    Pipe([1, 2, 3]) | for_each(lambda e, res=res: res.append(e))
+    Pipe([1, 2, 3]) | for_each(lambda e, r=res: r.append(e))
     assert res == [1, 2, 3]
 
 
+# noinspection PyShadowingNames,PyDefaultArgument
 def test_group_by():
     assert (Pipe([]) | group_by(len) | dict).get() == {}
     assert (Pipe(["a"]) | group_by(len) | dict).get() == {1: ["a"]}
     pipe = (Pipe(["a", "b", "ab"]) | group_by(len) | dict)
     assert pipe.get() == {1: ["a", "b"], 2: ["ab"]}
 
 
@@ -314,21 +379,38 @@
     assert (Pipe([1, 2, 3]) | last(3) | list).get() == [1, 2, 3]
     assert (Pipe([1, 2, 3]) | last(4) | list).get() == [1, 2, 3]
 
     with raises(ValueError):
         Pipe([]) | last(-1)
 
 
+def test_lstrip():
+    assert [*lstrip(0)([0, 0, 3, 5, 0, 0])] == [3, 5, 0, 0]
+    assert [*lstrip(0)([3, 5, 0, 0])] == [3, 5, 0, 0]
+    assert [*lstrip(0)([0, 0, 3, 5])] == [3, 5]
+    assert [*lstrip(0)([3, 5])] == [3, 5]
+    assert [*lstrip(0)([])] == []
+
+
 def test_map():
     pipe = Pipe(range(11)) | filter_(is_even) | map_(lambda e: e * 2) | list
     assert pipe.get() == [0, 4, 8, 12, 16, 20]
     pipe = Pipe([[3, 2, 1], [6, 5, 4]]) | map_(sorted) | list
     assert pipe.get() == [[1, 2, 3], [4, 5, 6]]
 
 
+def test_map_indexed():
+    assert [*map_indexed(lambda i, e: str(i) + e)("abc")] == ["0a", "1b", "2c"]
+    assert [*map_indexed(lambda i, e: e)("")] == []
+    assert [*map_indexed(lambda i, e: str(i) + e, start=1)("abc")] \
+           == ["1a", "2b", "3c"]
+    assert [*map_indexed(lambda i, e: str(i) + e, start=-1)("abc")] \
+           == ["-1a", "0b", "1c"]
+
+
 def test_max_by():
     assert (Pipe(["a"]) | max_by(len)).get() == "a"
     assert (Pipe(["a", "b"]) | max_by(len)).get() == "a"
     assert (Pipe(["a", "b", "ab"]) | max_by(len)).get() == "ab"
     assert (Pipe(["a", "b", "ab", "cd"]) | max_by(len)).get() == "ab"
 
 
@@ -345,15 +427,15 @@
     assert (Pipe([-1, 0, 1]) | none(lambda x: x == 0)).get() is False
 
 
 def test_not_contains():
     assert (Pipe([]) | not_contains(0)).get() is True
     assert (Pipe([-1, 1]) | not_contains(0)).get() is True
     assert (Pipe([-1, 0, 1]) | not_contains(0)).get() is False
-    assert (Pipe([-1]) | concat([0]) | not_contains(0)).get() is False
+    assert (Pipe([-1]) | extend([0]) | not_contains(0)).get() is False
 
 
 def test_pad_with():
     assert [*pad_with("*", 5)([1, 2, 3])] == [1, 2, 3, "*", "*"]
     assert [*pad_with("*", 3)([1, 2, 3])] == [1, 2, 3]
     assert [*pad_with("*", 2)([1, 2, 3])] == [1, 2]
     assert [*pad_with("*", 0)([1, 2, 3])] == []
@@ -368,29 +450,30 @@
     assert pipe.get() == [[2, 4], [1, 3]]
     pipe = (Pipe([2, 4, 6, 8]) | partition(is_even) | map_(list) | list)
     assert pipe.get() == [[2, 4, 6, 8], []]
     pipe = (Pipe([1, 3, 5, 7]) | partition(is_even) | map_(list) | list)
     assert pipe.get() == [[], [1, 3, 5, 7]]
 
 
-# noinspection PyShadowingNames,PyDefaultArgument
+# noinspection PyDefaultArgument
 def test_peek():
     res = []
-    pipe = (Pipe([1, 2, 3]) | peek(lambda e, res=res: res.append(e)) | list)
+    pipe = (Pipe([1, 2, 3]) | peek(lambda e, r=res: r.append(e)) | list)
     assert res == [1, 2, 3] and pipe.get() == [1, 2, 3]
 
     # is lazy
     res = []
     pipe = (Pipe([0, 0, 1, 2])
-            | peek(lambda e, res=res: res.append(e))
+            | peek(lambda e, r=res: r.append(e))
             | first(2)
             | list)
     assert res == [0, 0] and pipe.get() == [0, 0]
 
 
+# noinspection PyShadowingNames,PyDefaultArgument
 def test_reduce():
     pipe = Pipe(range(11)) | reduce(add)
     assert pipe.get() == sum(range(11))
     pipe = Pipe([1]) | reduce(add)
     assert pipe.get() == 1
 
 
@@ -406,14 +489,32 @@
     assert (Pipe([1, 2, 3, 2]) | remove_last(3) | list).get() == [1, 2, 2]
     assert (Pipe([1, 2, 3, 2]) | remove_last(1) | list).get() == [2, 3, 2]
     assert (Pipe([1, 2, 3, 2]) | remove_last(4) | list).get() == [1, 2, 3, 2]
     assert (Pipe([]) | remove_last(4) | list).get() == []
     assert (Pipe([1]) | remove_last(1) | list).get() == []
 
 
+def test_replace():
+    assert [*replace("a", "x")(["a", "b", "c"])] == ["x", "b", "c"]
+    assert [*replace("d", "x")(["a", "b", "c"])] == ["a", "b", "c"]
+    assert [*replace("a", "x")([])] == []
+    assert [*replace("a", None)(["a", "b", "c"])] == [None, "b", "c"]
+    assert [*replace("a", "x")(["a", "b", "a"])] == ["x", "b", "x"]
+    assert [*replace("a", "x")(["a", "a", "a"])] == ["x", "x", "x"]
+    assert [*replace(None, "X")(["a", None, "c"])] == ["a", "X", "c"]
+
+
+def test_rstrip():
+    assert [*rstrip(0)([0, 0, 3, 5, 0, 0])] == [0, 0, 3, 5]
+    assert [*rstrip(0)([3, 5, 0, 0])] == [3, 5]
+    assert [*rstrip(0)([0, 0, 3, 5])] == [0, 0, 3, 5]
+    assert [*rstrip(0)([3, 5])] == [3, 5]
+    assert [*rstrip(0)([])] == []
+
+
 def test_scan():
     assert (Pipe([]) | scan(add) | list).get() == []
     assert (Pipe([1]) | scan(add) | list).get() == [1]
     assert (Pipe([1, 2, 3]) | scan(add) | list).get() == [1, 3, 6]
 
 
 def test_slice():
@@ -481,14 +582,32 @@
 def test_starred():
     assert (Pipe([1, 2]) | starred(add)).get() == 3
     stream = StringIO()
     (Pipe([1, 2]) | starred(print, file=stream, sep="~", end="")).get()
     assert stream.getvalue() == "1~2"
 
 
+def test_strip():
+    assert [*strip(0)([0, 0, 3, 5, 0, 0])] == [3, 5]
+    assert [*strip(0)([3, 5, 0, 0])] == [3, 5]
+    assert [*strip(0)([0, 0, 3, 5])] == [3, 5]
+    assert [*strip(0)([3, 5])] == [3, 5]
+    assert [*strip(0)([])] == []
+
+
+def test_strip_while():
+    assert [*strip_while(it % 2 == 0)([0, 2, 3, 5, 6, 8])] == [3, 5]
+    assert [*strip_while(it % 2 == 0)([3, 5, 6, 8])] == [3, 5]
+    assert [*strip_while(it % 2 == 0)([0, 2, 3, 5])] == [3, 5]
+    assert [*strip_while(it % 2 == 0)([3, 5])] == [3, 5]
+    assert [*strip_while(it % 2 == 0)([])] == []
+    assert [*strip_while(it % 2 == 0)([0, 1, 0, 1, 0])] == [1, 0, 1]
+    assert [*strip_while(it % 2 == 0)([0, 0, 0])] == []
+
+
 def test_sum_by():
     assert sum_by(it * it)([1, 2, 3, 4]) == 30
     assert sum_by(len)(["1", "22", "ttt"]) == 6
     assert sum_by(it + it, start=[])([[1], [2, 3]]) == [1, 1, 2, 3, 2, 3]
 
 
 def test_take():
@@ -554,59 +673,58 @@
     assert (Pipe([[1]]) | transpose | map_(list) | list).get() == [[1]]
     assert (Pipe([[1, 2]]) | transpose | map_(list) | list).get() == [[1], [2]]
     assert (Pipe([[1], [2]]) | transpose | map_(list) | list).get() == [[1, 2]]
 
 
 def test_try_map():
     pipe = (Pipe([])
-            | try_map(lambda x: 1 / x, ZeroDivisionError, 0)
+            | try_map(lambda x: 1 / x, ZeroDivisionError, default=0)
             | list)
     assert pipe.get() == []
     pipe = (Pipe(range(1, 3))
             | map_(Fraction)
-            | try_map(lambda x: 1 / x, ZeroDivisionError, Fraction(0))
+            | try_map(lambda x: 1 / x, ZeroDivisionError, default=Fraction(0))
             | list)
     assert pipe.get() == [Fraction(1, 1), Fraction(1, 2)]
     pipe = (Pipe(range(-1, 2))
             | map_(Fraction)
-            | try_map(lambda x: 1 / x, ZeroDivisionError, Fraction(0))
+            | try_map(lambda x: 1 / x, ZeroDivisionError, default=Fraction(0))
             | list)
     assert pipe.get() == [Fraction(-1, 1), Fraction(0, 1), Fraction(1, 1)]
     pipe = (Pipe(range(-1, 2))
             | map_(Fraction)
-            | try_map(lambda x: 1 / x, default=ZeroDivisionError,
-                      ignore_errors=True)
+            | try_map(lambda x: 1 / x)
             | list)
     assert pipe.get() == [Fraction(-1, 1), Fraction(1, 1)]
 
     with raises(ZeroDivisionError):
         (Pipe(range(-1, 2))
          | map_(Fraction)
-         | try_map(lambda x: 1 / x, IndexError, Fraction(0))
+         | try_map(lambda x: 1 / x, IndexError, default=Fraction(0))
          | list).get()
 
 
 def test_windowed():
     assert (Pipe([1]) | windowed(1) | map_(list) | list).get() == [[1]]
     pipe = (Pipe([1, 2, 3]) | windowed(2) | map_(list) | list)
     assert pipe.get() == [[1, 2], [2, 3]]
 
     assert [*windowed(4, strict=False)([1, 2, 3])] == []
     assert [*windowed(-1, strict=False)([1, 2, 3])] == []
     assert [*windowed(-1, strict=False, partial=True)([1, 2, 3])] == []
     assert [[*e] for e in windowed(1, strict=False)([1])] == [[1]]
     assert [[*e] for e in
             windowed(2, strict=False)([1, 2, 3])] == [[1, 2], [2, 3]]
-    assert [[*e] for e in windowed(2, strict=False, partial=True)([1, 2, 3])]\
+    assert [[*e] for e in windowed(2, strict=False, partial=True)([1, 2, 3])] \
            == [[1, 2], [2, 3], [3]]
-    assert [[*e] for e in windowed(3, strict=False, partial=True)([1, 2, 3])]\
+    assert [[*e] for e in windowed(3, strict=False, partial=True)([1, 2, 3])] \
            == [[1, 2, 3], [2, 3], [3]]
-    assert [[*e] for e in windowed(3, partial=True)([1, 2, 3])]\
+    assert [[*e] for e in windowed(3, partial=True)([1, 2, 3])] \
            == [[1, 2, 3], [2, 3], [3]]
-    assert [[*e] for e in windowed(4, strict=False, partial=True)([1, 2, 3])]\
+    assert [[*e] for e in windowed(4, strict=False, partial=True)([1, 2, 3])] \
            == [[1, 2, 3], [2, 3], [3]]
 
     with raises(ValueError):
         (Pipe([]) | windowed(1) | list).get()
 
     with raises(ValueError):
         (Pipe([1]) | windowed(2) | list).get()
@@ -628,7 +746,22 @@
     assert pipe.get() == [["a", "ab", "abc"], [1, 2, 3]]
 
     pipe = (Pipe([(1, 2), (3, 4), (5, 6)])
             | unzip
             | map_(list)
             | list)
     assert pipe.get() == [[1, 3, 5], [2, 4, 6]]
+
+
+def test_wrap():
+    assert (Pipe([]) | wrap([]) | list).get() == []
+    assert (Pipe(["a"]) | wrap([]) | list).get() == ["a"]
+    assert (Pipe([]) | wrap(["b"]) | list).get() == ["b", "b"]
+    assert (Pipe(["a"]) | wrap(["b"]) | list).get() == ["b", "a", "b"]
+    pipe = (Pipe(["a", "b", "c"])
+            | wrap(iter(["d", "e", "f"]))
+            | list)
+    assert pipe.get() == list("defabcdef")
+    pipe = (Pipe(["a", "b", "c"])
+            | wrap(iter(["d", "e", "f"]), reverse_left=True)
+            | list)
+    assert pipe.get() == list("fedabcdef")
```

### Comparing `pipe-utils-0.2.2/tests/test_mappings.py` & `pipe-utils-0.3.0/tests/test_mappings.py`

 * *Files identical despite different names*

### Comparing `pipe-utils-0.2.2/tests/test_override.py` & `pipe-utils-0.3.0/tests/test_override.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pytest
 from pytest import raises
 
 from pipe_utils.override import *
 
 
 def test_override_all():
     assert (Pipe(range(0, 11, 2)) | all(is_even)).get() is True
@@ -71,16 +72,26 @@
     assert IsNot(a)(b)
     assert IsNot(None)(b)
     assert IsNot(a)(None)
     assert IsNot([1, 2])([1, 2])
 
 
 def test_raise():
-    with raises(ZeroDivisionError):
+    with pytest.raises(ZeroDivisionError):
         Raise(ZeroDivisionError())
-    with raises(ZeroDivisionError):
+    with pytest.raises(ZeroDivisionError) as e:
         Raise(ZeroDivisionError)
-    with raises(ValueError) as e:
+    assert e.value.__cause__ is None
+    with pytest.raises(ValueError) as e:
         Raise(ValueError("Uh oh!"), from_=TypeError("Oops!"))
     assert str(e.value) == "Uh oh!"
     assert isinstance(e.value.__cause__, TypeError)
     assert str(e.value.__cause__) == "Oops!"
+
+    with pytest.raises(ValueError) as e:
+        try:
+            1 / 0
+        except ZeroDivisionError:
+            Raise(ValueError("Oops!"), from_=None)
+    assert e.value.__suppress_context__ is True
+    assert e.value.__cause__ is None
+    assert str(e.value) == "Oops!"
```

### Comparing `pipe-utils-0.2.2/tests/test_pipe.py` & `pipe-utils-0.3.0/tests/test_pipe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import operator
 from io import StringIO
 
-from pytest import raises
+import pytest
 
-from pipe_utils import Pipe
+from pipe_utils import Pipe, it, map_
 from pipe_utils.pipe import Catch, Then
 
 
 def test_pipe_yields_data():
     assert Pipe(5).get() == 5
     assert Pipe([1, 2, 3]).get_or_default([2, 4, 8]) == [1, 2, 3]
     assert Pipe("Hello").get_or_raise(ValueError) == "Hello"
@@ -47,17 +47,17 @@
     pipe = (
             Pipe([-1, 0, 1])
             | (lambda data: map(lambda x: 1 / x, data))
             | list
     )
     assert pipe.get_or_default(-1) == -1
 
-    with raises(ZeroDivisionError):
+    with pytest.raises(ZeroDivisionError):
         pipe.get()
-    with raises(TypeError) as e:
+    with pytest.raises(TypeError) as e:
         pipe.get_or_raise(TypeError("Oops!!"))
     assert "Oops!!" in str(e.value)
 
 
 def test_args():
     stream = StringIO()
     Pipe("Hello") | Then(print, end=", World", file=stream)
@@ -70,15 +70,15 @@
 
 def test_catch():
     assert (Pipe([-1, 0, 1])
             .then(lambda data: map(lambda x: 1 / x, data))
             .then(list)
             .catch(ZeroDivisionError, lambda _: [0])
             ).get() == [0]
-    with raises(ZeroDivisionError):
+    with pytest.raises(ZeroDivisionError):
         (
             Pipe([-1, 0, 1])
             .then(lambda data: map(lambda x: 1 / x, data))
             .then(list)
             .catch(TypeError, lambda _: [0])
         ).get()
 
@@ -89,47 +89,70 @@
                    | (operator.truediv, 0)
                    | (operator.add, 1)
                    | Then(print, end="")
            ).get_or_default("Oops!") == "Oops!"
 
 
 def test_pipe_with_non_function():
-    with raises(ValueError):
+    with pytest.raises(ValueError):
         Pipe([]) | 4
 
 
 def test_get_or_default_ignores_wrong_exception_type():
-    with raises(TypeError):
+    with pytest.raises(TypeError):
         p = Pipe([]) | (operator.add, "abc")
         p.get_or_default("Oops!", catch=ValueError)
 
-    with raises(ValueError):
+    with pytest.raises(ValueError):
         p = Pipe("Hello") | int
         p.get_or_default("Oops!", catch=IndexError)
 
 
 def test_get_or_raise_ignores_wrong_exception_type():
     class PipeError(Exception): ...
 
-    with raises(TypeError):
+    with pytest.raises(TypeError):
         p = Pipe([]) | (operator.add, "abc")
         p.get_or_raise(PipeError("Oops!"), catch=ValueError)
 
-    with raises(ValueError):
+    with pytest.raises(ValueError):
         p = Pipe("Hello") | int
         p.get_or_raise(PipeError("Oops!"), catch=IndexError)
 
 
 def test_pipe_then_and_catch_classes():
     assert (
                    Pipe([-1, 0, 1])
                    | Then(lambda data: map(lambda x: 1 / x, data))
                    | Then(list)
                    | Catch(ZeroDivisionError, lambda _: [0])
            ).get() == [0]
-    with raises(ZeroDivisionError):
+    with pytest.raises(ZeroDivisionError):
         (
                 Pipe([-1, 0, 1])
                 | Then(lambda data: map(lambda x: 1 / x, data))
                 | Then(list)
                 | Catch(TypeError, lambda _: [0])
         ).get()
+
+
+def test_get_or_raise_controls_error_chaining():
+    with pytest.raises(ValueError) as e:
+        (
+            Pipe(range(-1, 2))
+            .then(map_(1 / it))
+            .then(list)
+        ).get_or_raise(
+            ValueError("Oops!"), catch=ZeroDivisionError, chained=False
+        )
+    assert e.value.__cause__ is None
+    assert str(e.value) == "Oops!"
+    with pytest.raises(ValueError) as e:
+        (
+            Pipe(range(-1, 2))
+            .then(map_(1 / it))
+            .then(list)
+        ).get_or_raise(
+            ValueError("Oops!"), catch=ZeroDivisionError, chained=True
+        )
+    assert isinstance(e.value.__cause__, ZeroDivisionError)
+    assert str(e.value) == "Oops!"
```

