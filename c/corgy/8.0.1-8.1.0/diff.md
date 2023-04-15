# Comparing `tmp/corgy-8.0.1.tar.gz` & `tmp/corgy-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-8.0.1.tar", max compression
+gzip compressed data, was "corgy-8.1.0.tar", max compression
```

## Comparing `corgy-8.0.1.tar` & `corgy-8.1.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
--rw-r--r--   0        0        0    29299 2023-04-14 22:10:02.982388 corgy-8.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-04-14 22:10:02.982388 corgy-8.0.1/LICENSE
--rw-r--r--   0        0        0     4158 2023-04-14 22:10:02.982388 corgy-8.0.1/README.md
--rw-r--r--   0        0        0      395 2023-04-14 22:10:02.982388 corgy-8.0.1/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-04-14 22:10:02.982388 corgy-8.0.1/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-04-14 22:10:02.982388 corgy-8.0.1/corgy/_annotations.py
--rw-r--r--   0        0        0    48599 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_corgy.py
--rw-r--r--   0        0        0     6237 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_corgyparser.py
--rw-r--r--   0        0        0    36993 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_helpfmt.py
--rw-r--r--   0        0        0    17249 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-04-14 22:10:38.026691 corgy-8.0.1/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_expand.py
--rw-r--r--   0        0        0     3413 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_subclass.py
--rw-r--r--   0        0        0    33057 2023-04-14 22:10:02.986388 corgy-8.0.1/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-04-14 22:10:02.986388 corgy-8.0.1/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-04-14 22:10:02.986388 corgy-8.0.1/docs/index.md
--rw-r--r--   0        0        0     2679 2023-04-14 22:10:38.026691 corgy-8.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/__init__.py
--rw-r--r--   0        0        0    89079 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_corgy.py
--rw-r--r--   0        0        0    16681 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_corgyparser.py
--rw-r--r--   0        0        0      780 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_doctests.py
--rw-r--r--   0        0        0    47095 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 corgy-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0    30107 2023-04-15 15:45:19.590671 corgy-8.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-04-15 15:45:19.590671 corgy-8.1.0/LICENSE
+-rw-r--r--   0        0        0     4196 2023-04-15 15:45:19.590671 corgy-8.1.0/README.md
+-rw-r--r--   0        0        0      468 2023-04-15 15:45:19.590671 corgy-8.1.0/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-04-15 15:45:19.590671 corgy-8.1.0/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-04-15 15:45:19.590671 corgy-8.1.0/corgy/_annotations.py
+-rw-r--r--   0        0        0    49762 2023-04-15 15:45:19.590671 corgy-8.1.0/corgy/_corgy.py
+-rw-r--r--   0        0        0     3233 2023-04-15 15:45:19.590671 corgy-8.1.0/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    36993 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    18067 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-04-15 15:46:10.056386 corgy-8.1.0/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3413 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-04-15 15:45:19.594671 corgy-8.1.0/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    35296 2023-04-15 15:45:19.594671 corgy-8.1.0/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-04-15 15:45:19.594671 corgy-8.1.0/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-04-15 15:45:19.594671 corgy-8.1.0/docs/index.md
+-rw-r--r--   0        0        0     2679 2023-04-15 15:46:10.056386 corgy-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    89079 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/test_corgy.py
+-rw-r--r--   0        0        0     4240 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    16681 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/test_doctests.py
+-rw-r--r--   0        0        0    47095 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-04-15 15:45:19.594671 corgy-8.1.0/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-04-15 15:45:19.598671 corgy-8.1.0/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-04-15 15:45:19.598671 corgy-8.1.0/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-04-15 15:45:19.598671 corgy-8.1.0/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-8.1.0/PKG-INFO
```

### Comparing `corgy-8.0.1/CHANGELOG.md` & `corgy-8.1.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [8.1.0](https://github.com/jayanthkoushik/corgy/compare/v8.0.1...v8.1.0) (2023-04-15)
+
+
+### Features
+
+* add support for custom attribute value checkers through `corgychecker` ([7904676](https://github.com/jayanthkoushik/corgy/commit/79046766f130f30a46d7d4ee52e9f5b387f6c5e9))
+* show attribute name in `ValueError` raised by `Corgy.from_dict` and `Corgy.load_dict` ([b73c5cf](https://github.com/jayanthkoushik/corgy/commit/b73c5cf9b618c21ee2dfd7d8f0b19beb89ad4337))
+* show attribute name in `ValueError` raised by `Corgy` in `setattr` ([c8fc1b2](https://github.com/jayanthkoushik/corgy/commit/c8fc1b22e97864fac14d486f8d8d428036816d37))
+
+
+### Bug Fixes
+
+* do not discard return value from custom checkers ([d5f4caf](https://github.com/jayanthkoushik/corgy/commit/d5f4cafa716dc226be3f310bb0faa371840778cb))
+
 ### [8.0.1](https://github.com/jayanthkoushik/corgy/compare/v8.0.0...v8.0.1) (2023-04-14)
 
 
 ### Bug Fixes
 
 * raise `ArgumentError` instead of `ArgumentTypeError` from `CorgyParserAction` ([f798132](https://github.com/jayanthkoushik/corgy/commit/f79813285a80ffeaf6d61a56b4829ec882d90372))
```

### Comparing `corgy-8.0.1/LICENSE` & `corgy-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/README.md` & `corgy-8.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,20 @@
   >>> class C(Corgy):
   ...     x: int
   ...     y: Tuple[int, int]
 
   >>> C(x="1")
   Traceback (most recent call last):
       ...
-  ValueError: invalid value for type '<class 'int'>': '1'
+  ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 
   >>> C(y=(1, 2, 3))
   Traceback (most recent call last):
       ...
-  ValueError: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
+  ValueError: error setting `y`: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
 
   ```
 
 * **Dictionary interface**: `Corgy` instances can be converted to/from
   dictionaries.
 
   ```pycon
```

### Comparing `corgy-8.0.1/corgy/_actions.py` & `corgy-8.1.0/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/_corgy.py` & `corgy-8.1.0/corgy/_corgy.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,21 @@
         A(x=1, y=2.1)
 
     Attribute values are type-checked, and `ValueError` is raised on type mismatch::
 
         >>> a = A(x="1")
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type '<class 'int'>': '1'
+        ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 
         >>> a = A()
         >>> a.x = "1"
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type '<class 'int'>': '1'
+        ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 
         >>> class A(Corgy):
         ...     x: int = "1"
         Traceback (most recent call last):
             ...
         ValueError: default value type mismatch for 'x'
 
@@ -346,73 +346,77 @@
         >>> a.w = [1, 2]
         >>> a
         A(x=[1, 2], y=('1', '2'), z={1.0, 2.0}, w=[1, 2])
 
         >>> a.x = [1, "2"]
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type '<class 'int'>': '2'
+        ValueError: error setting `x`: invalid value for type '<class 'int'>': '2'
 
         >>> a.x = (1, 2)      # `Sequence` accepts any sequence type
 
-        >>> a.y = ["1", "2"]  # `Tuple` only accepts tuples
+        >>> # `Tuple` only accepts tuples
+        >>> a.y = ["1", "2"]  # doctest: +NORMALIZE_WHITESPACE
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type 'typing.Tuple[str]': ['1', '2']
+        ValueError: error setting `y`: invalid value for type 'typing.Tuple[str]':
+        ['1', '2']
 
     The collection length can be controlled by the arguments of the type annotation.
     Note, however, that `typing.Sequence/typing.List/typing.Set` do not
     accept multiple arguments, and so, cannot be used if collection length has to be
     specified. On Python < 3.9, only `typing.Tuple` can be used for controlling
     collection lengths.
 
     To specify that a collection must be non-empty, use ellipsis (`...`) as the second
     argument of the type::
 
         >>> class A(Corgy):
         ...     x: Tuple[int, ...]
 
         >>> a = A()
-        >>> a.x = tuple()
+        >>> a.x = tuple()  # doctest: +NORMALIZE_WHITESPACE
         Traceback (most recent call last):
             ...
-        ValueError: expected non-empty collection for type 'typing.Tuple[int, ...]'
+        ValueError: error setting `x`: expected non-empty collection for type
+        'typing.Tuple[int, ...]'
 
     Collections can also be restricted to be of a fixed length::
 
         >>> class A(Corgy):
         ...     x: Tuple[int, str]
         ...     y: Tuple[int, int, int]
 
         >>> a = A()
         >>> a.x = (1, 1)
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type '<class 'str'>': 1
+        ValueError: error setting `x`: invalid value for type '<class 'str'>': 1
 
         >>> a.y = (1, 1)  # doctest: +NORMALIZE_WHITESPACE
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type 'typing.Tuple[int, int, int]': (1, 1):
-        expected exactly '3' elements
+        ValueError: error setting `y`: invalid value for type
+        'typing.Tuple[int, int, int]': (1, 1): expected exactly '3' elements
 
     *Literals*
     `typing.Literal` can be used to specify that an attribute takes one of a fixed set
     of values::
 
         >>> class A(Corgy):
         ...     x: Literal[0, 1, "2"]
 
         >>> a = A()
         >>> a.x = 0
         >>> a.x = "2"
         >>> a.x = "1"  # doctest: +IGNORE_EXCEPTION_DETAIL
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type 'typing.Literal[0, 1, '2']': '1'
+        ValueError: error setting `x`: invalid value for type
+        'typing.Literal[0, 1, '2']': '1'
 
     Type annotations can be nested; for instance,
     `Sequence[Literal[0, 1, 2], Literal[0, 1, 2]]` represents a sequence of length 2,
     where each element is either 0, 1, or 2.
 
     A fixed set of attribute values can also be specified by adding a `__choices__`
     attribute to the argument type, containing a collection of choices::
@@ -424,15 +428,15 @@
         ...     x: T
 
         >>> a = A()
         >>> a.x = 1
         >>> a.x = 3  # doctest: +NORMALIZE_WHITESPACE
         Traceback (most recent call last):
             ...
-        ValueError: invalid value for type '<class 'T'>': 3:
+        ValueError: error setting `x`: invalid value for type '<class 'T'>': 3:
         expected one of: (1, 2)
 
     Note that choices specified in this way are not type-checked to ensure that they
     match the argument type; in the above example, `__choices__` could be set to
     `(1, "2")`.
     """
 
@@ -1095,14 +1099,18 @@
 
             >>> A.from_dict({"x": "one", "g": G(x=1)})
             A(x='one', g=G(x=1))
             >>> A.from_dict({"x": "one", "g": {"x": 1}})
             A(x='one', g=G(x=1))
             >>> A.from_dict({"x": "one", "g": {"x": "1"}}, try_cast=True)
             A(x='one', g=G(x=1))
+            >>> G.from_dict({"x": "1"})
+            Traceback (most recent call last):
+                ...
+            ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 
         Group attributes can also be passed directly in the dictionary by prefixing
         their names with the group name and a colon::
 
             >>> A.from_dict({"x": "one", "g:x": 1})
             A(x='one', g=G(x=1))
 
@@ -1145,17 +1153,23 @@
         for grp_name, grp_args in grp_args_map.items():
             grp_type = cls_attrs[grp_name]
             main_args_map[grp_name] = grp_type.from_dict(grp_args, try_cast)
 
         cls_attrs = cls.attrs()
         for arg_name, arg_val in main_args_map.copy().items():
             if arg_name in cls_attrs:
-                main_args_map[arg_name] = check_val_type(
-                    arg_val, cls_attrs[arg_name], try_cast, try_load_corgy_dicts=True
-                )
+                try:
+                    main_args_map[arg_name] = check_val_type(
+                        arg_val,
+                        cls_attrs[arg_name],
+                        try_cast,
+                        try_load_corgy_dicts=True,
+                    )
+                except ValueError as e:
+                    raise ValueError(f"error setting `{arg_name}`: {e}") from None
         return cls(**main_args_map)
 
     def load_dict(
         self, d: Dict[str, Any], try_cast: bool = False, strict: bool = False
     ) -> None:
         """Load a dictionary into an instance of the class.
 
@@ -1183,14 +1197,22 @@
             >>> _i == id(a)
             True
             >>> a.load_dict({"y": "three"}, strict=True)
             >>> a
             A(y='three')
             >>> _i == id(a)
             True
+            >>> a = A()
+            >>> a.load_dict({"x": "1"})
+            Traceback (most recent call last):
+                ...
+            ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
+            >>> a.load_dict({"x": "1"}, try_cast=True)
+            >>> a
+            A(x=1)
 
         """
         main_args_map: Dict[str, Any] = defaultdict(dict)
         cls_attrs = self.attrs()
 
         for arg_name, arg_val in d.items():
             if ":" in arg_name:
@@ -1223,17 +1245,20 @@
                 try:
                     arg_obj = getattr(self, arg_name)
                 except AttributeError:
                     setattr(self, arg_name, arg_type.from_dict(arg_new_val))
                 else:
                     arg_obj.load_dict(arg_new_val, try_cast, strict)
             else:
-                arg_new_val = check_val_type(
-                    arg_new_val, arg_type, try_cast, try_load_corgy_dicts=True
-                )
+                try:
+                    arg_new_val = check_val_type(
+                        arg_new_val, arg_type, try_cast, try_load_corgy_dicts=True
+                    )
+                except ValueError as e:
+                    raise ValueError(f"error setting `{arg_name}`: {e}") from None
                 setattr(self, arg_name, arg_new_val)
 
     @classmethod
     def parse_from_cmdline(
         cls: Type[_T],
         parser: Optional[ArgumentParser] = None,
         defaults: Optional[Mapping[str, Any]] = None,
```

### Comparing `corgy-8.0.1/corgy/_corgyparser.py` & `corgy-8.1.0/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/_helpfmt.py` & `corgy-8.1.0/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/_meta.py` & `corgy-8.1.0/corgy/_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 if sys.version_info >= (3, 9):
     from typing import get_type_hints, Literal
 else:
     from typing_extensions import Literal, get_type_hints
 
 from ._annotations import NOT_REQUIRED, REQUIRED
+from ._corgychecker import CorgyChecker
 from ._corgyparser import CorgyParser
 
 
 def is_union_type(t) -> bool:
     """Check if the argument is a union type."""
     # This checks for the `|` based syntax introduced in Python 3.10.
     p310_check = sys.version_info >= (3, 10) and t.__class__ is UnionType
@@ -168,15 +169,16 @@
 class CorgyMeta(type):
     """Metaclass for `Corgy`.
 
     Modifies class creation by parsing type annotations, and creating properties for
     each annotated attribute. Default values and custom parsers are stored in the
     `__defaults` and `__parsers` attributes. Custom flags, if present, are stored in
     the `__flags` attribute. `Required` and `NotRequired` annotations are extracted,
-    and required attributes are stored in `__required`.
+    and required attributes are stored in `__required`. Attribute value checkers, if
+    present, are stored in `__checkers`.
     """
 
     __slots__ = ()
 
     def __new__(cls, name, bases, namespace, **kwds) -> CorgyMeta:
         try:
             _make_slots = kwds.pop("corgy_make_slots")
@@ -196,14 +198,15 @@
 
         cls_annotations = namespace.get("__annotations__", {})
         namespace["__annotations__"] = {}
         namespace["__defaults"] = {}
         namespace["__flags"] = {}
         namespace["__parsers"] = {}
         namespace["__helps"] = {}
+        namespace["__checkers"] = {}
         namespace["__required"] = set()
 
         # Temp set of not required attributes--to handle inheritance from
         # non-`Corgy` classes.
         _not_required = set()
 
         # Extract `corgy_freeze_after_init` (default `False`).
@@ -223,14 +226,15 @@
                 namespace["__annotations__"].update(_base_annotations)
                 if isinstance(base, cls):
                     # `base` is also a `Corgy` class.
                     namespace["__defaults"].update(getattr(base, "__defaults"))
                     namespace["__flags"].update(getattr(base, "__flags"))
                     namespace["__parsers"].update(getattr(base, "__parsers"))
                     namespace["__helps"].update(getattr(base, "__helps"))
+                    namespace["__checkers"].update(getattr(base, "__checkers"))
                     namespace["__required"].update(getattr(base, "__required"))
                     # Add not required attributes to temp set.
                     _base_required = getattr(base, "__required")
                     for _var_name in _base_annotations:
                         if _var_name not in _base_required:
                             _not_required.add(_var_name)
                 else:
@@ -380,25 +384,31 @@
                         f"`{var_name}`"
                     )
                 namespace["__slots__"].append(f"__{var_name}")
 
         if _make_slots:
             namespace["__slots__"] = tuple(namespace["__slots__"])
 
-        # Store custom parsers in a dict.
+        # Store custom parsers and checkers in a dict.
         for _, v in namespace.items():
-            if not isinstance(v, CorgyParser):
+            if not isinstance(v, (CorgyParser, CorgyChecker)):
                 continue
             for var_name in v.var_names:
                 if (var_name in namespace["__annotations__"]) and isinstance(
                     namespace[var_name], property
                 ):
-                    namespace["__parsers"][var_name] = v.fparse
+                    if isinstance(v, CorgyParser):
+                        namespace["__parsers"][var_name] = v.fparse
+                    else:
+                        namespace["__checkers"][var_name] = v.fcheck
                 else:
-                    raise TypeError(f"invalid target for corgyparser: {var_name}")
+                    _type = (
+                        "corgyparser" if isinstance(v, CorgyParser) else "corgychecker"
+                    )
+                    raise TypeError(f"invalid target for {_type}: {var_name}")
 
         return super().__new__(cls, name, bases, namespace, **kwds)
 
     @staticmethod
     def _create_var_property(cls_name, var_name, var_type, var_doc) -> property:
         # Properties are stored in private instance variables prefixed with `__`, and
         # must be accessed as `_<cls>__<var_name>`.
@@ -406,15 +416,22 @@
             with suppress(AttributeError):
                 return getattr(self, f"_{cls_name.lstrip('_')}__{var_name}")
             raise AttributeError(f"no value available for attribute `{var_name}`")
 
         def var_fset(self, val):
             if getattr(self, f"_{cls_name.lstrip('_')}__frozen"):
                 raise TypeError(f"cannot set `{var_name}`: object is frozen")
-            check_val_type(val, var_type)
+            _checkers = getattr(self, "__checkers")
+            try:
+                check_val_type(val, var_type)
+                if var_name in _checkers:
+                    _checkers[var_name](val)
+            except ValueError as e:
+                raise ValueError(f"error setting `{var_name}`: {e}") from None
+
             setattr(self, f"_{cls_name.lstrip('_')}__{var_name}", val)
 
         def var_fdel(self):
             if getattr(self, f"_{cls_name.lstrip('_')}__frozen"):
                 raise TypeError(f"cannot delete `{var_name}`: object is frozen")
             if var_name in getattr(self, "__required"):
                 raise TypeError(f"attribute `{var_name}` cannot be unset")
```

### Comparing `corgy-8.0.1/corgy/types/__init__.py` & `corgy-8.1.0/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/types/_expand.py` & `corgy-8.1.0/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/types/_initargs.py` & `corgy-8.1.0/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/types/_inputfile.py` & `corgy-8.1.0/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/types/_keyvaluepairs.py` & `corgy-8.1.0/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/types/_outputfile.py` & `corgy-8.1.0/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/corgy/types/_subclass.py` & `corgy-8.1.0/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/docs/corgy.md` & `corgy-8.1.0/docs/corgy.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,21 @@
 
 Attribute values are type-checked, and `ValueError` is raised on type mismatch:
 
 ```python
 >>> a = A(x="1")
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type '<class 'int'>': '1'
+ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 
 >>> a = A()
 >>> a.x = "1"
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type '<class 'int'>': '1'
+ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 
 >>> class A(Corgy):
 ...     x: int = "1"
 Traceback (most recent call last):
     ...
 ValueError: default value type mismatch for 'x'
 ```
@@ -352,22 +352,24 @@
 >>> a.w = [1, 2]
 >>> a
 A(x=[1, 2], y=('1', '2'), z={1.0, 2.0}, w=[1, 2])
 
 >>> a.x = [1, "2"]
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type '<class 'int'>': '2'
+ValueError: error setting `x`: invalid value for type '<class 'int'>': '2'
 
 >>> a.x = (1, 2)      # `Sequence` accepts any sequence type
 
->>> a.y = ["1", "2"]  # `Tuple` only accepts tuples
+>>> # `Tuple` only accepts tuples
+>>> a.y = ["1", "2"]
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type 'typing.Tuple[str]': ['1', '2']
+ValueError: error setting `y`: invalid value for type 'typing.Tuple[str]':
+['1', '2']
 ```
 
 The collection length can be controlled by the arguments of the type annotation.
 Note, however, that `typing.Sequence/typing.List/typing.Set` do not
 accept multiple arguments, and so, cannot be used if collection length has to be
 specified. On Python < 3.9, only `typing.Tuple` can be used for controlling
 collection lengths.
@@ -379,35 +381,36 @@
 >>> class A(Corgy):
 ...     x: Tuple[int, ...]
 
 >>> a = A()
 >>> a.x = tuple()
 Traceback (most recent call last):
     ...
-ValueError: expected non-empty collection for type 'typing.Tuple[int, ...]'
+ValueError: error setting `x`: expected non-empty collection for type
+'typing.Tuple[int, ...]'
 ```
 
 Collections can also be restricted to be of a fixed length:
 
 ```python
 >>> class A(Corgy):
 ...     x: Tuple[int, str]
 ...     y: Tuple[int, int, int]
 
 >>> a = A()
 >>> a.x = (1, 1)
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type '<class 'str'>': 1
+ValueError: error setting `x`: invalid value for type '<class 'str'>': 1
 
 >>> a.y = (1, 1)
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type 'typing.Tuple[int, int, int]': (1, 1):
-expected exactly '3' elements
+ValueError: error setting `y`: invalid value for type
+'typing.Tuple[int, int, int]': (1, 1): expected exactly '3' elements
 ```
 
 *Literals*
 `typing.Literal` can be used to specify that an attribute takes one of a fixed set
 of values:
 
 ```python
@@ -416,15 +419,16 @@
 
 >>> a = A()
 >>> a.x = 0
 >>> a.x = "2"
 >>> a.x = "1"
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type 'typing.Literal[0, 1, '2']': '1'
+ValueError: error setting `x`: invalid value for type
+'typing.Literal[0, 1, '2']': '1'
 ```
 
 Type annotations can be nested; for instance,
 `Sequence[Literal[0, 1, 2], Literal[0, 1, 2]]` represents a sequence of length 2,
 where each element is either 0, 1, or 2.
 
 A fixed set of attribute values can also be specified by adding a `__choices__`
@@ -438,15 +442,15 @@
 ...     x: T
 
 >>> a = A()
 >>> a.x = 1
 >>> a.x = 3
 Traceback (most recent call last):
     ...
-ValueError: invalid value for type '<class 'T'>': 3:
+ValueError: error setting `x`: invalid value for type '<class 'T'>': 3:
 expected one of: (1, 2)
 ```
 
 Note that choices specified in this way are not type-checked to ensure that they
 match the argument type; in the above example, `__choices__` could be set to
 `(1, "2")`.
 
@@ -828,14 +832,18 @@
 
 >>> A.from_dict({"x": "one", "g": G(x=1)})
 A(x='one', g=G(x=1))
 >>> A.from_dict({"x": "one", "g": {"x": 1}})
 A(x='one', g=G(x=1))
 >>> A.from_dict({"x": "one", "g": {"x": "1"}}, try_cast=True)
 A(x='one', g=G(x=1))
+>>> G.from_dict({"x": "1"})
+Traceback (most recent call last):
+    ...
+ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 ```
 
 Group attributes can also be passed directly in the dictionary by prefixing
 their names with the group name and a colon:
 
 ```python
 >>> A.from_dict({"x": "one", "g:x": 1})
@@ -886,14 +894,22 @@
 >>> _i == id(a)
 True
 >>> a.load_dict({"y": "three"}, strict=True)
 >>> a
 A(y='three')
 >>> _i == id(a)
 True
+>>> a = A()
+>>> a.load_dict({"x": "1"})
+Traceback (most recent call last):
+    ...
+ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
+>>> a.load_dict({"x": "1"}, try_cast=True)
+>>> a
+A(x=1)
 ```
 
 
 #### _classmethod_ parse_from_cmdline(parser=None, defaults=None, \*\*parser_args)
 Return an instance of the class parsed from command line arguments.
 
 
@@ -984,14 +1000,76 @@
 >>> del a.y
 Traceback (most recent call last):
     ...
 TypeError: cannot delete `y`: object is frozen
 ```
 
 
+### corgy.corgychecker(\*var_names)
+Decorate a function as a custom checker for one or more attributes.
+
+To use a custom function for checking the value of a `Corgy` attribute, use this
+decorator. Checking functions must be static, and should only accept a single
+argument, the value to be checked. They should raise `ValueError` to indicate value
+mismatch. Decorating the function with `@staticmethod` is optional, but prevents
+type errors. `@corgychecker` must be the final decorator in the decorator chain.
+
+Custom checkers are called _after_ type checking, so the values passed to them will
+be of type corresponding to one of the assigned attributes.
+
+
+* **Parameters**
+
+    **var_names** – The attributes associated with the decorated checker.
+
+
+Example:
+
+```python
+>>> from corgy import Corgy, corgychecker
+
+>>> class A(Corgy):
+...     x: int
+...     @corgychecker("x")
+...     @staticmethod
+...     def check_x(val):
+...         if val % 2:
+...             raise ValueError(f"'{val}' is not even")
+
+>>> a = A()
+>>> a.x = 2
+>>> a.x = 3
+Traceback (most recent call last):
+   ...
+ValueError: error setting `x`: '3' is not even
+```
+
+Multiple attributes can use the same checker, either by chaining `corgychecker`, or
+by passing all attribute names directly:
+
+```python
+>>> from typing import Sequence
+
+>>> class A(Corgy):
+...     x: int
+...     y: float
+...     z: str
+...     w: Sequence[int]
+...     @corgychecker("x")
+...     @corgychecker("y")
+...     def check_num(val):
+...         if val < 0:
+...             raise ValueError("should be non-negative")
+...     @corgychecker("z", "w")
+...     def check_seq(val):
+...         if len(val) > 10:
+...             raise ValueError("too long")
+```
+
+
 ### corgy.corgyparser(\*var_names, metavar=None, nargs=None)
 Decorate a function as a custom parser for one or more attributes.
 
 To use a custom function for parsing a `Corgy` attribute, use this decorator.
 Parsing functions must be static, and should only accept a single argument.
 Decorating the function with `@staticmethod` is optional, but prevents type errors.
 `@corgyparser` must be the final decorator in the decorator chain.
```

### Comparing `corgy-8.0.1/docs/corgy.types.md` & `corgy-8.1.0/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/pyproject.toml` & `corgy-8.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "8.0.1"  # managed by `poetry-dynamic-versioning`
+version = "8.1.0"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-8.0.1/tests/test_corgy.py` & `corgy-8.1.0/tests/test_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/test_corgyparser.py` & `corgy-8.1.0/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/test_doctests.py` & `corgy-8.1.0/tests/test_doctests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from doctest import DocFileSuite
 
 import corgy
 import corgy.types
 
 DOCTEST_MODULES = {
-    corgy: ["_corgy.py", "_corgyparser.py", "_helpfmt.py"],
+    corgy: ["_corgy.py", "_corgychecker.py", "_corgyparser.py", "_helpfmt.py"],
     corgy.types: [
         "_initargs.py",
         "_inputfile.py",
         "_keyvaluepairs.py",
         "_outputfile.py",
         "_subclass.py",
     ],
```

### Comparing `corgy-8.0.1/tests/test_helpfmt.py` & `corgy-8.1.0/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/types/_specialtmps.py` & `corgy-8.1.0/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/types/_test_file.py` & `corgy-8.1.0/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/types/test_initargs.py` & `corgy-8.1.0/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/types/test_inputfiles.py` & `corgy-8.1.0/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/types/test_keyvaluepairs.py` & `corgy-8.1.0/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/types/test_outputfiles.py` & `corgy-8.1.0/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/tests/types/test_subclass.py` & `corgy-8.1.0/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.1/PKG-INFO` & `corgy-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 8.0.1
+Version: 8.1.0
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
@@ -62,20 +62,20 @@
   >>> class C(Corgy):
   ...     x: int
   ...     y: Tuple[int, int]
 
   >>> C(x="1")
   Traceback (most recent call last):
       ...
-  ValueError: invalid value for type '<class 'int'>': '1'
+  ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
 
   >>> C(y=(1, 2, 3))
   Traceback (most recent call last):
       ...
-  ValueError: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
+  ValueError: error setting `y`: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
 
   ```
 
 * **Dictionary interface**: `Corgy` instances can be converted to/from
   dictionaries.
 
   ```pycon
```

