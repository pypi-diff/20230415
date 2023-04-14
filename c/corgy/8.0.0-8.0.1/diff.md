# Comparing `tmp/corgy-8.0.0.tar.gz` & `tmp/corgy-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-8.0.0.tar", max compression
+gzip compressed data, was "corgy-8.0.1.tar", max compression
```

## Comparing `corgy-8.0.0.tar` & `corgy-8.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    29010 2023-04-14 21:42:45.442256 corgy-8.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-04-14 21:42:45.442256 corgy-8.0.0/LICENSE
--rw-r--r--   0        0        0     4158 2023-04-14 21:42:45.442256 corgy-8.0.0/README.md
--rw-r--r--   0        0        0      395 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_annotations.py
--rw-r--r--   0        0        0    48599 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_corgy.py
--rw-r--r--   0        0        0     6228 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_corgyparser.py
--rw-r--r--   0        0        0    36993 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_helpfmt.py
--rw-r--r--   0        0        0    17249 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-04-14 21:43:27.343100 corgy-8.0.0/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_expand.py
--rw-r--r--   0        0        0     3413 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_subclass.py
--rw-r--r--   0        0        0    33057 2023-04-14 21:42:45.442256 corgy-8.0.0/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-04-14 21:42:45.442256 corgy-8.0.0/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-04-14 21:42:45.442256 corgy-8.0.0/docs/index.md
--rw-r--r--   0        0        0     2679 2023-04-14 21:43:27.339100 corgy-8.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 21:42:45.442256 corgy-8.0.0/tests/__init__.py
--rw-r--r--   0        0        0    89079 2023-04-14 21:42:45.442256 corgy-8.0.0/tests/test_corgy.py
--rw-r--r--   0        0        0    16513 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/test_corgyparser.py
--rw-r--r--   0        0        0      780 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/test_doctests.py
--rw-r--r--   0        0        0    47095 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 corgy-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0    29299 2023-04-14 22:10:02.982388 corgy-8.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-04-14 22:10:02.982388 corgy-8.0.1/LICENSE
+-rw-r--r--   0        0        0     4158 2023-04-14 22:10:02.982388 corgy-8.0.1/README.md
+-rw-r--r--   0        0        0      395 2023-04-14 22:10:02.982388 corgy-8.0.1/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-04-14 22:10:02.982388 corgy-8.0.1/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-04-14 22:10:02.982388 corgy-8.0.1/corgy/_annotations.py
+-rw-r--r--   0        0        0    48599 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_corgy.py
+-rw-r--r--   0        0        0     6237 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    36993 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    17249 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-04-14 22:10:38.026691 corgy-8.0.1/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3413 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-04-14 22:10:02.986388 corgy-8.0.1/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    33057 2023-04-14 22:10:02.986388 corgy-8.0.1/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-04-14 22:10:02.986388 corgy-8.0.1/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-04-14 22:10:02.986388 corgy-8.0.1/docs/index.md
+-rw-r--r--   0        0        0     2679 2023-04-14 22:10:38.026691 corgy-8.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    89079 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_corgy.py
+-rw-r--r--   0        0        0    16681 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      780 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_doctests.py
+-rw-r--r--   0        0        0    47095 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-04-14 22:10:02.986388 corgy-8.0.1/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 corgy-8.0.1/PKG-INFO
```

### Comparing `corgy-8.0.0/CHANGELOG.md` & `corgy-8.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [8.0.1](https://github.com/jayanthkoushik/corgy/compare/v8.0.0...v8.0.1) (2023-04-14)
+
+
+### Bug Fixes
+
+* raise `ArgumentError` instead of `ArgumentTypeError` from `CorgyParserAction` ([f798132](https://github.com/jayanthkoushik/corgy/commit/f79813285a80ffeaf6d61a56b4829ec882d90372))
+
 ## [8.0.0](https://github.com/jayanthkoushik/corgy/compare/v7.0.0...v8.0.0) (2023-04-14)
 
 
 ### ⚠ BREAKING CHANGES
 
 * The following path based types have been removed from
 `Corgy.types`: `ReadableFile`, `WritableFile`, `InputDirectory`,
```

### Comparing `corgy-8.0.0/LICENSE` & `corgy-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/README.md` & `corgy-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/_actions.py` & `corgy-8.0.1/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/_corgy.py` & `corgy-8.0.1/corgy/_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/_corgyparser.py` & `corgy-8.0.1/corgy/_corgyparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import sys
-from argparse import Action, ArgumentTypeError
+from argparse import Action, ArgumentError
 from functools import partial
 from typing import Any, Callable, Collection, List, NamedTuple, Optional, Union
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -42,15 +42,15 @@
             if self._choices is not None and val not in self._choices:
                 raise ValueError(
                     f"invalid choice: {val} (choose from "
                     f"{', '.join(map(str, self._choices))})"
                 )
             setattr(namespace, self.dest, val)
         except ValueError as e:
-            raise ArgumentTypeError from e
+            raise ArgumentError(self, str(e)) from None
 
 
 def corgyparser(
     *var_names: str,
     metavar: Optional[str] = None,
     nargs: Union[None, Literal["*", "+"], int] = None,
 ) -> Callable[[Union[Callable[[str], Any], CorgyParser]], CorgyParser]:
```

### Comparing `corgy-8.0.0/corgy/_helpfmt.py` & `corgy-8.0.1/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/_meta.py` & `corgy-8.0.1/corgy/_meta.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/types/__init__.py` & `corgy-8.0.1/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/types/_expand.py` & `corgy-8.0.1/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/types/_initargs.py` & `corgy-8.0.1/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/types/_inputfile.py` & `corgy-8.0.1/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/types/_keyvaluepairs.py` & `corgy-8.0.1/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/types/_outputfile.py` & `corgy-8.0.1/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/corgy/types/_subclass.py` & `corgy-8.0.1/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/docs/corgy.md` & `corgy-8.0.1/docs/corgy.md`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/docs/corgy.types.md` & `corgy-8.0.1/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/pyproject.toml` & `corgy-8.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "8.0.0"  # managed by `poetry-dynamic-versioning`
+version = "8.0.1"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-8.0.0/tests/test_corgy.py` & `corgy-8.0.1/tests/test_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/test_corgyparser.py` & `corgy-8.0.1/tests/test_corgyparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
 import sys
 from argparse import ArgumentParser, ArgumentTypeError
+from contextlib import redirect_stderr
 from functools import partial
+from io import StringIO
 from typing import ClassVar, Optional, Tuple
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 
 if sys.version_info >= (3, 9):
     from typing import Annotated, Literal
 else:
@@ -420,22 +422,23 @@
             @staticmethod
             def parsex(s):
                 return sum(map(int, s))
 
         orig_parse_args = ArgumentParser.parse_args
 
         def _run_with_args(*cmd_args):
-            parser = ArgumentParser()
-            parser.parse_args = lambda: orig_parse_args(
-                parser, ["--x"] + list(cmd_args)
-            )
-            args = C.parse_from_cmdline(parser)
-            return args.x
+            with redirect_stderr(StringIO()):
+                parser = ArgumentParser()
+                parser.parse_args = lambda: orig_parse_args(
+                    parser, ["--x"] + list(cmd_args)
+                )
+                args = C.parse_from_cmdline(parser)
+                return args.x
 
-        with self.assertRaises(ArgumentTypeError):
+        with self.assertRaises(SystemExit):
             _run_with_args("2", "3", "4")
         self.assertEqual(_run_with_args("1", "2", "3", "4"), 10)
 
     def test_corgy_cls_respects_optional_with_custom_parser(self):
         class C(Corgy):
             x: Optional[int]
 
@@ -469,32 +472,33 @@
                     s = [s_tup[2 * _i], s_tup[2 * _i + 1]]
                     o_list.append((int(s[0]), float(s[1])))
                 return tuple(o_list)
 
         orig_parse_args = ArgumentParser.parse_args
 
         def _run_with_args(*cmd_args):
-            parser = ArgumentParser()
-            parser.parse_args = lambda: orig_parse_args(
-                parser, ["--x"] + list(cmd_args)
-            )
-            args = C.parse_from_cmdline(parser)
-            return args.x
+            with redirect_stderr(StringIO()):
+                parser = ArgumentParser()
+                parser.parse_args = lambda: orig_parse_args(
+                    parser, ["--x"] + list(cmd_args)
+                )
+                args = C.parse_from_cmdline(parser)
+                return args.x
 
         self.assertTupleEqual(_run_with_args("1", "2.1"), ((1, 2.1),))
         self.assertTupleEqual(
             _run_with_args("1", "2.1", "3", "4.1"), ((1, 2.1), (3, 4.1))
         )
-        with self.assertRaises(ArgumentTypeError):
+        with self.assertRaises(SystemExit):
             _run_with_args("1", "two")
-        with self.assertRaises(ArgumentTypeError):
+        with self.assertRaises(SystemExit):
             _run_with_args("1.1", "2.1")
-        with self.assertRaises(ArgumentTypeError):
+        with self.assertRaises(SystemExit):
             _run_with_args("1", "2.1", "3")
-        with self.assertRaises(ArgumentTypeError):
+        with self.assertRaises(SystemExit):
             _run_with_args()
 
     def test_custom_parsers_handle_required_attrs(self):
         class C(Corgy):
             x: Required[int]
 
             @corgyparser("x")
```

### Comparing `corgy-8.0.0/tests/test_doctests.py` & `corgy-8.0.1/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/test_helpfmt.py` & `corgy-8.0.1/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/types/_specialtmps.py` & `corgy-8.0.1/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/types/_test_file.py` & `corgy-8.0.1/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/types/test_initargs.py` & `corgy-8.0.1/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/types/test_inputfiles.py` & `corgy-8.0.1/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/types/test_keyvaluepairs.py` & `corgy-8.0.1/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/types/test_outputfiles.py` & `corgy-8.0.1/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/tests/types/test_subclass.py` & `corgy-8.0.1/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.0.0/PKG-INFO` & `corgy-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 8.0.0
+Version: 8.0.1
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

