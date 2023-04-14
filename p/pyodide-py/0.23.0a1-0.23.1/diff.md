# Comparing `tmp/pyodide-py-0.23.0a1.tar.gz` & `tmp/pyodide-py-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-py-0.23.0a1.tar", last modified: Tue Jan 24 07:47:08 2023, max compression
+gzip compressed data, was "pyodide-py-0.23.1.tar", last modified: Fri Apr 14 22:15:40 2023, max compression
```

## Comparing `pyodide-py-0.23.0a1.tar` & `pyodide-py-0.23.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:47:08.657260 pyodide-py-0.23.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-01-24 07:47:08.657260 pyodide-py-0.23.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:47:08.653260 pyodide-py-0.23.0a1/_pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/_pyodide/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    40467 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/_pyodide/_core_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/_pyodide/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/_pyodide/docs_argspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/_pyodide/docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:47:08.657260 pyodide-py-0.23.0a1/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/_package_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/_run_js.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/code.py
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:47:08.657260 pyodide-py-0.23.0a1/pyodide/ffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/ffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/ffi/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyodide/webloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:47:08.657260 pyodide-py-0.23.0a1/pyodide_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-01-24 07:47:08.000000 pyodide-py-0.23.0a1/pyodide_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-24 07:47:08.000000 pyodide-py-0.23.0a1/pyodide_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 07:47:08.000000 pyodide-py-0.23.0a1/pyodide_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-24 07:47:08.000000 pyodide-py-0.23.0a1/pyodide_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-24 07:47:08.657260 pyodide-py-0.23.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-24 07:46:51.000000 pyodide-py-0.23.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:40.907519 pyodide-py-0.23.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 22:15:40.907519 pyodide-py-0.23.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:40.899519 pyodide-py-0.23.1/_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/_pyodide/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42449 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/_pyodide/_core_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/_pyodide/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/_pyodide/docs_argspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/_pyodide/docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:40.903519 pyodide-py-0.23.1/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/_package_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/_run_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:40.903519 pyodide-py-0.23.1/pyodide/ffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/ffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/ffi/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyodide/webloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:40.907519 pyodide-py-0.23.1/pyodide_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 22:15:40.000000 pyodide-py-0.23.1/pyodide_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 22:15:40.000000 pyodide-py-0.23.1/pyodide_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:15:40.000000 pyodide-py-0.23.1/pyodide_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 22:15:40.000000 pyodide-py-0.23.1/pyodide_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 22:15:40.907519 pyodide-py-0.23.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-04-14 22:15:25.000000 pyodide-py-0.23.1/webbrowser.py
```

### Comparing `pyodide-py-0.23.0a1/PKG-INFO` & `pyodide-py-0.23.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.23.0a1
+Version: 0.23.1
 Summary: "A Python package providing core interpreter functionality for Pyodide."
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.23.0a1/README.md` & `pyodide-py-0.23.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.0a1/_pyodide/_base.py` & `pyodide-py-0.23.1/_pyodide/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return
     last_node = mod.body[-1]
 
     if isinstance(last_node, ast.Assign):
         # In this case there can be multiple targets as in `a = b = 1`.
         # We just take the first one.
         target = last_node.targets[0]
-    elif isinstance(last_node, (ast.AugAssign, ast.AnnAssign)):
+    elif isinstance(last_node, ast.AugAssign | ast.AnnAssign):
         target = last_node.target
     else:
         return
     if isinstance(target, ast.Name):
         last_node = ast.Expr(ast.Name(target.id, ast.Load()))
         mod.body.append(last_node)
         # Update the line numbers shown in error messages.
@@ -110,15 +110,15 @@
 def _last_expr_to_raise(mod: ast.Module) -> None:
     """If the final ast node is a statement, raise an EvalCodeResultException
     with the value of the statement.
     """
     if not mod.body:
         return
     last_node = mod.body[-1]
-    if not isinstance(mod.body[-1], (ast.Expr, ast.Await)):
+    if not isinstance(mod.body[-1], ast.Expr | ast.Await):
         return
     raise_expr = deepcopy(_raise_template_ast)
     # Replace x with our value in _raise_template_ast.
     raise_expr.exc.args[0] = last_node.value  # type: ignore[attr-defined]
     mod.body[-1] = raise_expr
 
 
@@ -165,16 +165,16 @@
 
 
 class CodeRunner:
     """This class allows fine control over the execution of a code block.
 
     It is primarily intended for REPLs and other sophisticated consumers that
     may wish to add their own AST transformations, separately signal to the user
-    when parsing is complete, etc. The simpler :any:`eval_code` and
-    :any:`eval_code_async` apis should be preferred when their flexibility
+    when parsing is complete, etc. The simpler :py:func:`eval_code` and
+    :py:func:`eval_code_async` apis should be preferred when their flexibility
     suffices.
 
     Parameters
     ----------
     source :
 
         The Python source code to run.
@@ -212,22 +212,22 @@
         The flags to compile with. See the documentation for the built-in
         :external:py:func:`compile` function.
     """
 
     ast: ast.Module
     """
     The ast from parsing ``source``. If you wish to do an ast transform,
-    modify this variable before calling :any:`CodeRunner.compile`.
+    modify this variable before calling :py:meth:`CodeRunner.compile`.
     """
 
     code: CodeType | None
     """
-    Once you call :any:`CodeRunner.compile` the compiled code will
+    Once you call :py:meth:`CodeRunner.compile` the compiled code will
     be available in the code field. You can modify this variable
-    before calling :any:`CodeRunner.run` to do a code transform.
+    before calling :py:meth:`CodeRunner.run` to do a code transform.
     """
 
     def __init__(
         self,
         source: str,
         *,
         return_mode: ReturnMode = "last_expr",
@@ -269,39 +269,43 @@
         self,
         globals: dict[str, Any] | None = None,
         locals: dict[str, Any] | None = None,
     ) -> Any:
         """Executes ``self.code``.
 
         Can only be used after calling compile. The code may not use top level
-        await, use :any:`CodeRunner.run_async` for code that uses top level
+        await, use :py:meth:`CodeRunner.run_async` for code that uses top level
         await.
 
         Parameters
         ----------
         globals :
 
             The global scope in which to execute code. This is used as the ``globals``
-            parameter for :any:`exec`. If ``globals`` is absent, a new empty dictionary is used.
+            parameter for :py:func:`exec`. If ``globals`` is absent, a new empty dictionary is used.
 
         locals :
 
             The local scope in which to execute code. This is used as the ``locals``
-            parameter for :any:`exec`. If ``locals`` is absent, the value of ``globals`` is
+            parameter for :py:func:`exec`. If ``locals`` is absent, the value of ``globals`` is
             used.
 
         Returns
         -------
 
             If the last nonwhitespace character of ``source`` is a semicolon,
             return ``None``. If the last statement is an expression, return the
             result of the expression. Use the ``return_mode`` and
             ``quiet_trailing_semicolon`` parameters to modify this default
             behavior.
         """
+        if globals is None:
+            globals = {}
+        if locals is None:
+            locals = globals
         if not self._compiled:
             raise RuntimeError("Not yet compiled")
         if self.code is None:
             return None
         try:
             coroutine = eval(self.code, globals, locals)
             if coroutine:
@@ -317,40 +321,44 @@
     async def run_async(
         self,
         globals: dict[str, Any] | None = None,
         locals: dict[str, Any] | None = None,
     ) -> Any:
         """Runs ``self.code`` which may use top level await.
 
-        Can only be used after calling :any:`CodeRunner.compile`. If
+        Can only be used after calling :py:meth:`CodeRunner.compile`. If
         ``self.code`` uses top level await, automatically awaits the resulting
         coroutine.
 
         Parameters
         ----------
         globals :
 
             The global scope in which to execute code. This is used as the ``globals``
-            parameter for :any:`exec`. If ``globals`` is absent, a new empty dictionary is used.
+            parameter for :py:func:`exec`. If ``globals`` is absent, a new empty dictionary is used.
 
         locals :
 
             The local scope in which to execute code. This is used as the
-            ``locals`` parameter for :any:`exec`. If ``locals`` is absent, the
+            ``locals`` parameter for :py:func:`exec`. If ``locals`` is absent, the
             value of ``globals`` is used.
 
         Returns
         -------
 
             If the last nonwhitespace character of ``source`` is a semicolon,
             return ``None``. If the last statement is an expression, return the
             result of the expression. Use the ``return_mode`` and
             ``quiet_trailing_semicolon`` parameters to modify this default
             behavior.
         """
+        if globals is None:
+            globals = {}
+        if locals is None:
+            locals = globals
         if not self._compiled:
             raise RuntimeError("Not yet compiled")
         if self.code is None:
             return
         try:
             coroutine = eval(self.code, globals, locals)
             if coroutine:
@@ -376,21 +384,21 @@
     source :
 
         The Python source code to run.
 
     globals :
 
         The global scope in which to execute code. This is used as the
-        ``globals`` parameter for :any:`exec`. If ``globals`` is absent, a new
+        ``globals`` parameter for :py:func:`exec`. If ``globals`` is absent, a new
         empty dictionary is used.
 
     locals :
 
         The local scope in which to execute code. This is used as the ``locals``
-        parameter for :any:`exec`. If ``locals`` is absent, the value of
+        parameter for :py:func:`exec`. If ``locals`` is absent, the value of
         ``globals`` is used.
 
     return_mode :
 
         Specifies what should be returned. The options are:
 
         :'last_expr': return the last expression
@@ -469,32 +477,32 @@
     return_mode: ReturnMode = "last_expr",
     quiet_trailing_semicolon: bool = True,
     filename: str = "<exec>",
     flags: int = 0x0,
 ) -> Any:
     """Runs a code string asynchronously.
 
-    Uses :any:`ast.PyCF_ALLOW_TOP_LEVEL_AWAIT` to compile the code.
+    Uses :py:data:`ast.PyCF_ALLOW_TOP_LEVEL_AWAIT` to compile the code.
 
     Parameters
     ----------
     source :
 
         The Python source code to run.
 
     globals :
 
         The global scope in which to execute code. This is used as the
-        ``globals`` parameter for :any:`exec`. If ``globals`` is absent, a new
+        ``globals`` parameter for :py:func:`exec`. If ``globals`` is absent, a new
         empty dictionary is used.
 
     locals :
 
         The local scope in which to execute code. This is used as the ``locals``
-        parameter for :any:`exec`. If ``locals`` is absent, the value of
+        parameter for :py:func:`exec`. If ``locals`` is absent, the value of
         ``globals`` is used.
 
     return_mode :
 
         Specifies what should be returned. The options are:
 
         :'last_expr': return the last expression
@@ -553,15 +561,15 @@
     Returns
     -------
         A list of module names that are imported in ``source``. If ``source`` is not
         syntactically correct Python code (after dedenting), returns an empty list.
 
     Examples
     --------
-    >>> from pyodide import find_imports
+    >>> from pyodide.code import find_imports
     >>> source = "import numpy as np; import scipy.stats"
     >>> find_imports(source)
     ['numpy', 'scipy']
     """
     # handle mis-indented input from multi-line strings
     source = dedent(source)
```

### Comparing `pyodide-py-0.23.0a1/_pyodide/_core_docs.py` & `pyodide-py-0.23.1/_pyodide/_core_docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import sys
 from collections.abc import (
     AsyncIterator,
+    Awaitable,
     Callable,
     ItemsView,
     Iterable,
     Iterator,
     KeysView,
     Mapping,
     MutableMapping,
     Sequence,
     ValuesView,
 )
 from functools import reduce
 from types import TracebackType
-from typing import IO, Any, Awaitable, Generic, TypeVar, overload
+from typing import IO, Any, Generic, TypeVar, overload
 
 from .docs_argspec import docs_argspec
 
 # All docstrings for public `core` APIs should be extracted from here. We use
 # the utilities in `docstring.py` and `docstring.c` to format them
 # appropriately.
 
@@ -90,15 +91,15 @@
 
 class JsProxy(metaclass=_JsProxyMetaClass):
     """A proxy to make a JavaScript object behave like a Python object
 
     For more information see the :ref:`type-translations` documentation. In
     particular, see
     :ref:`the list of __dunder__ methods <type-translations-jsproxy>`
-    that are (conditionally) implemented on :any:`JsProxy`.
+    that are (conditionally) implemented on :py:class:`JsProxy`.
     """
 
     _js_type_flags: Any = 0
 
     def __new__(cls, arg=None, *args, **kwargs):
         if arg is _instantiate_token:
             return super().__new__(cls)
@@ -131,25 +132,56 @@
         "The JavaScript API ``Object.keys(object)``"
         raise NotImplementedError
 
     def object_values(self) -> "JsProxy":
         "The JavaScript API ``Object.values(object)``"
         raise NotImplementedError
 
-    def as_object_map(self) -> "JsMutableMap[str, Any]":
+    def as_object_map(self, *, hereditary: bool = False) -> "JsMutableMap[str, Any]":
         """Returns a new JsProxy that treats the object as a map.
 
         The methods :py:func:`~operator.__getitem__`,
         :py:func:`~operator.__setitem__`, :py:func:`~operator.__contains__`,
         :py:meth:`~object.__len__`, etc will perform lookups via ``object[key]``
         or similar.
 
         Note that ``len(x.as_object_map())`` evaluates in O(n) time (it iterates
-        over the object and counts how many ownKeys it has). If you need to
-        compute the length in O(1) time, use a real ``Map`` instead.
+        over the object and counts how many :js:func:`~Reflect.ownKeys` it has).
+        If you need to compute the length in O(1) time, use a real
+        :js:class:`Map` instead.
+
+        Parameters
+        ----------
+        hereditary:
+            If ``True``, any "plain old objects" stored as values in the object
+            will be wrapped in `as_object_map` themselves.
+
+        Examples
+        --------
+
+        .. code-block:: python
+
+            from pyodide.code import run_js
+
+            o = run_js("({x : {y: 2}})")
+            # You have to access the properties of o as attributes
+            assert o.x.y == 2
+            with pytest.raises(TypeError):
+                o["x"] # is not subscriptable
+
+            # as_object_map allows us to access the property with getitem
+            assert o.as_object_map()["x"].y == 2
+
+            with pytest.raises(TypeError):
+                # The inner object is not subscriptable because hereditary is False.
+                o.as_object_map()["x"]["y"]
+
+            # When hereditary is True, the inner object is also subscriptable
+            assert o.as_object_map(hereditary=True)["x"]["y"] == 2
+
         """
         raise NotImplementedError
 
     def new(self, *args: Any, **kwargs: Any) -> "JsProxy":
         """Construct a new instance of the JavaScript object"""
         raise NotImplementedError
 
@@ -183,15 +215,15 @@
             ``default_converter`` takes three arguments. The first argument is
             the value to be converted.
 
         Examples
         --------
 
         Here are a couple examples of converter functions. In addition to the
-        normal conversions, convert ``Date`` to ``datetime``:
+        normal conversions, convert :js:class:`Date`` to :py:class:`~datetime.datetime`:
 
         .. code-block:: python
 
             from datetime import datetime
             def default_converter(value, _ignored1, _ignored2):
                 if value.constructor.name == "Date":
                     return datetime.fromtimestamp(d.valueOf()/1000)
@@ -216,15 +248,15 @@
             class Pair {
                 constructor(first, second){
                     this.first = first;
                     this.second = second;
                 }
             }
 
-        We can use the following ``default_converter`` to convert ``Pair`` to ``list``:
+        We can use the following ``default_converter`` to convert ``Pair`` to :py:class:`list`:
 
         .. code-block:: python
 
             def default_converter(value, convert, cache):
                 if value.constructor.name != "Pair":
                     return value
                 result = []
@@ -246,59 +278,61 @@
         infinite recurse. With it, we can successfully convert ``p`` to a list
         such that ``l[0] is l``.
         """
         raise NotImplementedError
 
 
 class JsDoubleProxy(JsProxy):
-    """A double proxy created with :any:`create_proxy`."""
+    """A double proxy created with :py:func:`create_proxy`."""
 
     _js_type_flags = ["IS_DOUBLE_PROXY"]
 
     def destroy(self) -> None:
         """Destroy the proxy."""
         pass
 
     def unwrap(self) -> Any:
-        """Unwrap a double proxy created with :any:`create_proxy` into the
+        """Unwrap a double proxy created with :py:func:`create_proxy` into the
         wrapped Python object.
         """
         raise NotImplementedError
 
 
 class JsPromise(JsProxy):
-    """A JsProxy of a promise (or some other awaitable JavaScript object).
+    """A :py:class:`~pyodide.ffi.JsProxy` of a :js:class:`Promise` or some other `thenable
+    <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise#thenables>`_
+    JavaScript object.
 
-    A JavaScript object is considered to be a Promise if it has a "then" method.
+    A JavaScript object is considered to be a :js:class:`Promise` if it has a ``then`` method.
     """
 
     _js_type_flags = ["IS_AWAITABLE"]
 
     def then(
         self, onfulfilled: Callable[[Any], Any], onrejected: Callable[[Any], Any]
     ) -> "JsPromise":
-        """The ``Promise.then`` API, wrapped to manage the lifetimes of the
+        """The :js:meth:`Promise.then` API, wrapped to manage the lifetimes of the
         handlers.
 
         Pyodide will automatically release the references to the handlers
         when the promise resolves.
         """
         raise NotImplementedError
 
     def catch(self, onrejected: Callable[[Any], Any], /) -> "JsPromise":
-        """The ``Promise.catch`` API, wrapped to manage the lifetimes of the
+        """The :js:meth:`Promise.catch` API, wrapped to manage the lifetimes of the
         handler.
 
         Pyodide will automatically release the references to the handler
         when the promise resolves.
         """
         raise NotImplementedError
 
     def finally_(self, onfinally: Callable[[], Any], /) -> "JsPromise":
-        """The ``Promise.finally`` API, wrapped to manage the lifetimes of
+        """The :js:meth:`Promise.finally` API, wrapped to manage the lifetimes of
         the handler.
 
         Pyodide will automatically release the references to the handler
         when the promise resolves. Note the trailing underscore in the name;
         this is needed because ``finally`` is a reserved keyword in Python.
         """
         raise NotImplementedError
@@ -434,38 +468,38 @@
 
     def __delitem__(self, idx: int | slice) -> None:
         pass
 
     def __len__(self) -> int:
         return 0
 
-    def extend(self, other: Iterable[T]) -> None:
+    def extend(self, other: Iterable[T], /) -> None:
         """Extend array by appending elements from the iterable."""
 
     def __reversed__(self) -> Iterator[T]:
         """Return a reverse iterator over the :js:class:`Array`."""
         raise NotImplementedError
 
     def pop(self, /, index: int = -1) -> T:
         """Remove and return the ``item`` at ``index`` (default last).
 
-        Raises :any:`IndexError` if list is empty or index is out of range.
+        Raises :py:exc:`IndexError` if list is empty or index is out of range.
         """
         raise NotImplementedError
 
     def push(self, /, object: T) -> None:
         pass
 
     def append(self, /, object: T) -> None:
         """Append object to the end of the list."""
 
     def index(self, /, value: T, start: int = 0, stop: int = sys.maxsize) -> int:
         """Return first ``index`` at which ``value`` appears in the ``Array``.
 
-        Raises :any:`ValueError` if the value is not present.
+        Raises :py:exc:`ValueError` if the value is not present.
         """
         raise NotImplementedError
 
     def count(self, /, x: T) -> int:
         """Return the number of times x appears in the list."""
         raise NotImplementedError
 
@@ -554,15 +588,15 @@
     """A JavaScript mutable map
 
     To be considered a mutable map, a JavaScript object must have a ``get``
     method, a ``has`` method, a ``size`` or a ``length`` property which is a
     number (idiomatically it should be called ``size``) and it must be iterable.
 
     Instances of the JavaScript builtin ``Map`` class are ``JsMutableMap`` s.
-    Also proxies returned by :any:`JsProxy.as_object_map` are instances of
+    Also proxies returned by :py:meth:`JsProxy.as_object_map` are instances of
     ``JsMap`` .
     """
 
     _js_type_flags = ["HAS_GET | HAS_SET | HAS_LENGTH | IS_ITERABLE", "IS_OBJECT_MAP"]
 
     @overload
     def pop(self, key: KT, /) -> VT:
@@ -619,15 +653,15 @@
                 Either a mapping or an iterable of pairs. This can be left out.
 
             kwargs:  ``VT``
 
                 Extra key-values pairs to insert into the map. Only usable for
                 inserting extra strings.
 
-        If ``other`` is present and is a :any:`Mapping` or has a ``keys``
+        If ``other`` is present and is a :py:class:`~collections.abc.Mapping` or has a ``keys``
         method, does
 
         .. code-block:: python
 
             for k in other:
                 self[k] = other[k]
 
@@ -653,15 +687,15 @@
     def __delitem__(self, idx: KT) -> None:
         return None
 
 
 class JsIterator(JsProxy, Generic[Tco]):
     """A JsProxy of a JavaScript iterator.
 
-    An object is a :any:`JsAsyncIterator` if it has a :js:meth:`~Iterator.next` method and either has a
+    An object is a :py:class:`JsAsyncIterator` if it has a :js:meth:`~Iterator.next` method and either has a
     :js:data:`Symbol.iterator` or has no :js:data:`Symbol.asyncIterator`.
     """
 
     _js_type_flags = ["IS_ITERATOR"]
 
     def __next__(self) -> Tco:
         raise NotImplementedError
@@ -669,15 +703,15 @@
     def __iter__(self) -> Iterator[Tco]:
         raise NotImplementedError
 
 
 class JsAsyncIterator(JsProxy, Generic[Tco]):
     """A JsProxy of a JavaScript async iterator.
 
-    An object is a :any:`JsAsyncIterator` if it has a
+    An object is a :py:class:`JsAsyncIterator` if it has a
     :js:meth:`~AsyncIterator.next` method and either has a
     :js:data:`Symbol.asyncIterator` or has no :js:data:`Symbol.iterator`
     """
 
     _js_type_flags = ["IS_ASYNC_ITERATOR"]
 
     def __anext__(self) -> Awaitable[Tco]:
@@ -727,15 +761,15 @@
 
     def send(self, value: Tcontra) -> Tco:
         """
         Resumes the execution and "sends" a value into the generator function.
 
         The ``value`` argument becomes the result of the current yield
         expression. The ``send()`` method returns the next value yielded by the
-        generator, or raises :any:`StopIteration` if the generator exits without
+        generator, or raises :py:exc:`StopIteration` if the generator exits without
         yielding another value. When ``send()`` is called to start the
         generator, the argument will be ignored. Unlike in Python, we cannot
         detect that the generator hasn't started yet, and no error will be
         thrown if the argument of a not-started generator is not ``None``.
         """
         raise NotImplementedError
 
@@ -765,15 +799,15 @@
         *args: Any,
     ) -> Tco:
         """
         Raises an exception at the point where the generator was paused, and
         returns the next value yielded by the generator function.
 
         If the generator exits without yielding another value, a
-        :any:`StopIteration` exception is raised. If the generator function does
+        :py:exc:`StopIteration` exception is raised. If the generator function does
         not catch the passed-in exception, or raises a different exception, then
         that exception propagates to the caller.
 
         In typical use, this is called with a single exception instance similar
         to the way the raise keyword is used.
 
         For backwards compatibility, however, a second signature is supported,
@@ -783,34 +817,34 @@
         instance. If traceback is provided, it is set on the exception,
         otherwise any existing ``__traceback__`` attribute stored in value may
         be cleared.
         """
         raise NotImplementedError
 
     def close(self) -> None:
-        """Raises a :any:`GeneratorExit` at the point where the generator
+        """Raises a :py:exc:`GeneratorExit` at the point where the generator
         function was paused.
 
         If the generator function then exits gracefully, is already closed, or
-        raises :any:`GeneratorExit` (by not catching the exception), ``close()``
+        raises :py:exc:`GeneratorExit` (by not catching the exception), ``close()``
         returns to its caller. If the generator yields a value, a
-        :any:`RuntimeError` is raised. If the generator raises any other
+        :py:exc:`RuntimeError` is raised. If the generator raises any other
         exception, it is propagated to the caller. ``close()`` does nothing if
         the generator has already exited due to an exception or normal exit.
         """
 
     def __next__(self) -> Tco:
         raise NotImplementedError
 
     def __iter__(self) -> "JsGenerator[Tco, Tcontra, Vco]":
         raise NotImplementedError
 
 
 class JsFetchResponse(JsProxy):
-    """A :any:`JsFetchResponse` object represents a :js:data:`Response` to a
+    """A :py:class:`JsFetchResponse` object represents a :js:data:`Response` to a
     :js:func:`fetch` request.
     """
 
     bodyUsed: bool
     ok: bool
     redirected: bool
     status: int
@@ -854,15 +888,15 @@
     def asend(self, value: Tcontra, /) -> Awaitable[Tco]:
         """Resumes the execution and "sends" a value into the async generator
         function.
 
         The ``value`` argument becomes the result of the current yield
         expression. The awaitable returned by the ``asend()`` method will return
         the next value yielded by the generator or raises
-        :any:`StopAsyncIteration` if the asynchronous generator returns. If the
+        :py:exc:`StopAsyncIteration` if the asynchronous generator returns. If the
         generator returned a value, this value is discarded (because in Python
         async generators cannot return a value).
 
         When ``asend()`` is called to start the generator, the argument will be
         ignored. Unlike in Python, we cannot detect that the generator hasn't
         started yet, and no error will be thrown if the argument of a
         not-started generator is not ``None``.
@@ -891,31 +925,31 @@
 
     @docs_argspec("(self, error: BaseException, /) -> Tco")
     def athrow(self, value: Any, *args: Any) -> Awaitable[Tco]:
         """Resumes the execution and raises an exception at the point where the
         generator was paused.
 
         The awaitable returned by ``athrow()`` method will return the next value
-        yielded by the generator or raises :any:`StopAsyncIteration` if the
+        yielded by the generator or raises :py:exc:`StopAsyncIteration` if the
         asynchronous generator returns. If the generator returned a value, this
         value is discarded (because in Python async generators cannot return a
         value). If the generator function does not catch the passed-in
         exception, or raises a different exception, then that exception
         propagates to the caller.
         """
         raise NotImplementedError
 
     def aclose(self) -> Awaitable[None]:
-        """Raises a :any:`GeneratorExit` at the point where the generator
+        """Raises a :py:exc:`GeneratorExit` at the point where the generator
         function was paused.
 
         If the generator function then exits gracefully, is already closed, or
-        raises :any:`GeneratorExit` (by not catching the exception),
+        raises :py:exc:`GeneratorExit` (by not catching the exception),
         ``aclose()`` returns to its caller. If the generator yields a value, a
-        :any:`RuntimeError` is raised. If the generator raises any other
+        :py:exc:`RuntimeError` is raised. If the generator raises any other
         exception, it is propagated to the caller. ``aclose()`` does nothing if
         the generator has already exited due to an exception or normal exit.
         """
         raise NotImplementedError
 
 
 class JsCallable(JsProxy):
@@ -926,40 +960,48 @@
 
 
 class JsOnceCallable(JsCallable):
     def destroy(self):
         pass
 
 
-class JsRawException(JsProxy):
-    @property
-    def name(self) -> str:
-        return ""
-
-    @property
-    def message(self) -> str:
-        return ""
+class JsException(JsProxy, Exception):
+    """A JavaScript Error.
 
-    @property
-    def stack(self) -> str:
-        return ""
+    These are pickleable unlike other JsProxies.
+    """
 
+    # Note: Unlike many of these classes, this one is never actually seen by the
+    # user IN_BROWSER (it's replaced by a different JsException in
+    # pyodide._core). We use it to unpickle errors so we need it to be
+    # instantiable.
+    def __new__(cls, *args, **kwargs):
+        if args[0] == _instantiate_token:
+            return super().__new__(cls, *args, **kwargs)
+        return cls._new_exc(*args, **kwargs)
+
+    @classmethod
+    def _new_exc(cls, name: str, message: str = "", stack: str = "") -> "JsException":
+        result = super().__new__(JsException, _instantiate_token)
+        result.name = name
+        result.message = message
+        result.stack = stack
+        return result
+
+    def __str__(self):
+        return f"{self.name}: {self.message}"
 
-class JsException(Exception):
-    """
-    A wrapper around a JavaScript Error to allow it to be thrown in Python.
+    name: str
+    """The name of the error type"""
 
-    The js_error field contains a JsProxy for the wrapped error.
-    See :ref:`type-translations-errors`.
-    """
+    message: str
+    """The error message"""
 
-    @property
-    def js_error(self) -> JsRawException:
-        """The original JavaScript error"""
-        return JsRawException(_instantiate_token)
+    stack: str
+    """The JavaScript stack trace"""
 
 
 class ConversionError(Exception):
     """An error thrown when conversion between JavaScript and Python fails."""
 
 
 class InternalError(Exception):
@@ -999,34 +1041,36 @@
     """
     return obj  # type: ignore[return-value]
 
 
 def create_proxy(
     obj: Any, /, *, capture_this: bool = False, roundtrip: bool = True
 ) -> JsDoubleProxy:
-    """Create a :any:`JsProxy` of a :any:`PyProxy`.
+    """Create a :py:class:`JsProxy` of a :js:class:`~pyodide.ffi.PyProxy`.
 
-    This allows explicit control over the lifetime of the :any:`PyProxy` from
-    Python: call the :py:meth:`~JsDoubleProxy.destroy` API when done.
+    This allows explicit control over the lifetime of the
+    :js:class:`~pyodide.ffi.PyProxy` from Python: call the
+    :py:meth:`~JsDoubleProxy.destroy` API when done.
 
     Parameters
     ----------
     obj:
         The object to wrap.
 
     capture_this :
-        If the object is callable, should ``this`` be passed as the first argument
-        when calling it from JavaScript.
+        If the object is callable, should ``this`` be passed as the first
+        argument when calling it from JavaScript.
 
     roundtrip:
         When the proxy is converted back from JavaScript to Python, if this is
         ``True`` it is converted into a double proxy. If ``False``, it is
         unwrapped into a Python object. In the case that ``roundtrip`` is
-        ``True`` it is possible to unwrap a double proxy with the :any:`unwrap`
-        method. This is useful to allow easier control of lifetimes from Python:
+        ``True`` it is possible to unwrap a double proxy with the
+        :py:meth:`JsDoubleProxy.unwrap` method. This is useful to allow easier
+        control of lifetimes from Python:
 
         .. code-block:: python
 
             from js import o
             d = {}
             o.d = create_proxy(d, roundtrip=True)
             o.d.destroy() # Destroys the proxy created with create_proxy
@@ -1101,39 +1145,39 @@
     default_converter: Callable[
         [Any, Callable[[Any], JsProxy], Callable[[Any, JsProxy], None]], JsProxy
     ]
     | None = None,
 ) -> Any:
     """Convert the object to JavaScript.
 
-    This is similar to :any:`PyProxy.toJs`, but for use from Python. If the
+    This is similar to :js:meth:`~pyodide.ffi.PyProxy.toJs`, but for use from Python. If the
     object can be implicitly translated to JavaScript, it will be returned
     unchanged. If the object cannot be converted into JavaScript, this method
-    will return a :any:`JsProxy` of a :any:`PyProxy`, as if you had used
+    will return a :py:class:`JsProxy` of a :js:class:`~pyodide.ffi.PyProxy`, as if you had used
     :func:`~pyodide.ffi.create_proxy`.
 
     See :ref:`type-translations-pyproxy-to-js` for more information.
 
     Parameters
     ----------
     obj :
         The Python object to convert
 
     depth :
         The maximum depth to do the conversion. Negative numbers are treated as
         infinite. Set this to 1 to do a shallow conversion.
 
     pyproxies:
-        Should be a JavaScript ``Array``. If provided, any ``PyProxies``
-        generated will be stored here. You can later use :any:`destroy_proxies`
+        Should be a JavaScript :js:class:`Array`. If provided, any ``PyProxies``
+        generated will be stored here. You can later use :py:meth:`destroy_proxies`
         if you want to destroy the proxies from Python (or from JavaScript you
-        can just iterate over the ``Array`` and destroy the proxies).
+        can just iterate over the :js:class:`Array` and destroy the proxies).
 
     create_pyproxies:
-        If you set this to :any:`False`, :any:`to_js` will raise an error rather
+        If you set this to :py:data:`False`, :py:func:`to_js` will raise an error rather
         than creating any pyproxies.
 
     dict_converter:
         This converter if provided receives a (JavaScript) iterable of
         (JavaScript) pairs [key, value]. It is expected to return the desired
         result of the dict conversion. Some suggested values for this argument:
 
@@ -1183,15 +1227,15 @@
     .. code-block:: python
 
         class Pair:
             def __init__(self, first, second):
                 self.first = first self.second = second
 
     We can use the following ``default_converter`` to convert ``Pair`` to
-    ``Array``:
+    :js:class:`Array`:
 
     .. code-block:: python
 
         from js import Array
 
         def default_converter(value, convert, cache):
             if not isinstance(value, Pair):
@@ -1215,16 +1259,16 @@
     return obj
 
 
 def destroy_proxies(pyproxies: JsArray[Any], /) -> None:
     """Destroy all PyProxies in a JavaScript array.
 
     pyproxies must be a JavaScript Array of PyProxies. Intended for use
-    with the arrays created from the "pyproxies" argument of :any:`PyProxy.toJs`
-    and :any:`to_js`. This method is necessary because indexing the Array from
+    with the arrays created from the "pyproxies" argument of :js:meth:`~pyodide.ffi.PyProxy.toJs`
+    and :py:func:`to_js`. This method is necessary because indexing the Array from
     Python automatically unwraps the PyProxy into the wrapped Python object.
     """
     pass
 
 
 __name__ = _save_name
 del _save_name
```

### Comparing `pyodide-py-0.23.0a1/_pyodide/_importhook.py` & `pyodide-py-0.23.1/_pyodide/_importhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 
     def register_js_module(self, name: str, jsproxy: Any) -> None:
         """
         Registers ``jsproxy`` as a JavaScript module named ``name``. The module
         can then be imported from Python using the standard Python import
         system. If another module by the same name has already been imported,
         this won't have much effect unless you also delete the imported module
-        from :any:`sys.modules`. This is called by the JavaScript API
-        :any:`pyodide.registerJsModule`.
+        from :py:data:`sys.modules`. This is called by the JavaScript API
+        :js:func:`pyodide.registerJsModule`.
 
         Parameters
         ----------
         name :
             Name of js module
 
         jsproxy :
@@ -70,20 +70,20 @@
                 f"Argument 'jsproxy' must be a JsProxy, not {type(jsproxy).__name__!r}"
             )
         self.jsproxies[name] = jsproxy
 
     def unregister_js_module(self, name: str) -> None:
         """
         Unregisters a JavaScript module with given name that has been previously
-        registered with :any:`pyodide.registerJsModule` or
-        :any:`pyodide.ffi.register_js_module`. If a JavaScript module with that name
+        registered with :js:func:`pyodide.registerJsModule` or
+        :py:func:`pyodide.ffi.register_js_module`. If a JavaScript module with that name
         does not already exist, will raise an error. If the module has already
         been imported, this won't have much effect unless you also delete the
-        imported module from ``sys.modules``. This is called by the JavaScript
-        API :any:`pyodide.unregisterJsModule`.
+        imported module from :py:data:`sys.modules`. This is called by the JavaScript
+        API :js:func:`pyodide.unregisterJsModule`.
 
         Parameters
         ----------
         name :
             Name of the module to unregister
         """
         try:
@@ -130,17 +130,15 @@
         if isinstance(importer, JsFinder):
             raise RuntimeError("JsFinder already registered")
 
     sys.meta_path.append(jsfinder)
 
 
 STDLIBS = sys.stdlib_module_names | {"test"}
-# TODO: Move this list to js side
-UNVENDORED_STDLIBS = ["distutils", "ssl", "lzma", "sqlite3", "hashlib"]
-UNVENDORED_STDLIBS_AND_TEST = UNVENDORED_STDLIBS + ["test"]
+UNVENDORED_STDLIBS_AND_TEST: set[str] = set()
 
 
 from importlib import _bootstrap  # type: ignore[attr-defined]
 
 orig_get_module_not_found_error: Any = None
 REPODATA_PACKAGES_IMPORT_TO_PACKAGE_NAME: dict[str, str] = {}
 
@@ -152,15 +150,14 @@
 You can install it by calling:
   await micropip.install("{package_name}") in Python, or
   await pyodide.loadPackage("{package_name}") in JavaScript\
 """
 
 
 def get_module_not_found_error(import_name):
-
     package_name = REPODATA_PACKAGES_IMPORT_TO_PACKAGE_NAME.get(import_name, "")
 
     if not package_name and import_name not in STDLIBS:
         return orig_get_module_not_found_error(import_name)
 
     if package_name in UNVENDORED_STDLIBS_AND_TEST:
         msg = "The module '{package_name}' is unvendored from the Python standard library in the Pyodide distribution."
@@ -176,19 +173,21 @@
 
     msg += SEE_PACKAGE_LOADING
     return ModuleNotFoundError(
         msg.format(import_name=import_name, package_name=package_name)
     )
 
 
-def register_module_not_found_hook(packages: Any) -> None:
+def register_module_not_found_hook(packages: Any, unvendored: Any) -> None:
     """
     A function that adds UnvendoredStdlibFinder to the end of sys.meta_path.
 
     Note that this finder must be placed in the end of meta_paths
     in order to prevent any unexpected side effects.
     """
     global orig_get_module_not_found_error
     global REPODATA_PACKAGES_IMPORT_TO_PACKAGE_NAME
+    global UNVENDORED_STDLIBS_AND_TEST
     REPODATA_PACKAGES_IMPORT_TO_PACKAGE_NAME = packages.to_py()
+    UNVENDORED_STDLIBS_AND_TEST = set(unvendored.to_py())
     orig_get_module_not_found_error = _bootstrap._get_module_not_found_error
     _bootstrap._get_module_not_found_error = get_module_not_found_error
```

### Comparing `pyodide-py-0.23.0a1/_pyodide/docs_argspec.py` & `pyodide-py-0.23.1/_pyodide/docs_argspec.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.0a1/_pyodide/docstring.py` & `pyodide-py-0.23.1/_pyodide/docstring.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.0a1/pyodide/_package_loader.py` & `pyodide-py-0.23.1/pyodide/_package_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     shutil.register_archive_format("whl", make_whlfile, description="Wheel file")
     shutil.register_unpack_format(
         "whl", [".whl", ".wheel"], shutil._unpack_zipfile, description="Wheel file"  # type: ignore[attr-defined]
     )
 
 
 def get_format(format: str) -> str:
-    for (fmt, extensions, _) in shutil.get_unpack_formats():
+    for fmt, extensions, _ in shutil.get_unpack_formats():
         if format == fmt:
             return fmt
         if format in extensions:
             return fmt
         if "." + format in extensions:
             return fmt
     raise ValueError(f"Unrecognized format {format}")
@@ -206,14 +206,16 @@
     if target:
         extract_path = TARGETS[target]
     elif extract_dir:
         extract_path = Path(extract_dir)
     else:
         extract_path = Path(".")
     filename = filename.rpartition("/")[-1]
+
+    extract_path.mkdir(parents=True, exist_ok=True)
     with NamedTemporaryFile(suffix=filename) as f:
         buffer._into_file(f)
         shutil.unpack_archive(f.name, extract_path, format)
         suffix = Path(filename).suffix
         if suffix == ".whl":
             set_wheel_installer(filename, f, extract_path, installer, source)
         if calculate_dynlibs:
```

### Comparing `pyodide-py-0.23.0a1/pyodide/_state.py` & `pyodide-py-0.23.1/pyodide/_state.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.0a1/pyodide/code.py` & `pyodide-py-0.23.1/pyodide/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def run_js(code: str, /) -> Any:
     """
     A wrapper for the :js:func:`eval` function.
 
     Runs ``code`` as a Javascript code string and returns the result. Unlike
-    :js:func:`eval`, if ``code`` is not a string we raise a :any:`TypeError`.
+    :js:func:`eval`, if ``code`` is not a string we raise a :py:exc:`TypeError`.
     """
     from js import eval as eval_
 
     if not isinstance(code, str):
         raise TypeError(
             f"argument should have type 'string' not type '{type(code).__name__}'"
         )
```

### Comparing `pyodide-py-0.23.0a1/pyodide/console.py` & `pyodide-py-0.23.1/pyodide/console.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 ConsoleFutureStatus = Literal["incomplete", "syntax-error", "complete"]
 INCOMPLETE: ConsoleFutureStatus = "incomplete"
 SYNTAX_ERROR: ConsoleFutureStatus = "syntax-error"
 COMPLETE: ConsoleFutureStatus = "complete"
 
 
 class ConsoleFuture(Future[Any]):
-    """A future with extra fields used as the return value for :any:`Console` apis."""
+    """A future with extra fields used as the return value for :py:class:`Console` apis."""
 
     syntax_check: ConsoleFutureStatus
     """
     The status of the future. The values mean the following:
 
     :'incomplete': Input is incomplete. The future has already been resolved
                  with result ``None``.
@@ -191,63 +191,67 @@
     """Interactive Pyodide console
 
     An interactive console based on the Python standard library
     :py:class:`~code.InteractiveConsole` that manages stream redirections and
     asynchronous execution of the code.
 
     The stream callbacks can be modified directly by assigning to
-    :any:`Console.stdin_callback` (for example) as long as
+    :py:attr:`~Console.stdin_callback` (for example) as long as
     ``persistent_stream_redirection`` is ``False``.
 
     Parameters
     ----------
     globals :
 
         The global namespace in which to evaluate the code. Defaults to a new
         empty dictionary.
 
     stdin_callback :
 
-        Function to call at each read from :any:`sys.stdin`. Defaults to :any:`None`.
+        Function to call at each read from :py:data:`sys.stdin`. Defaults to :py:data:`None`.
 
     stdout_callback :
 
-        Function to call at each write to :any:`sys.stdout`. Defaults to :any:`None`.
+        Function to call at each write to :py:data:`sys.stdout`. Defaults to :py:data:`None`.
 
     stderr_callback :
 
-        Function to call at each write to :any:`sys.stderr`. Defaults to :any:`None`.
+        Function to call at each write to :py:data:`sys.stderr`. Defaults to :py:data:`None`.
 
     persistent_stream_redirection :
 
         Should redirection of standard streams be kept between calls to
-        :py:meth:`~Console.runcode`? Defaults to :any:`False`.
+        :py:meth:`~Console.runcode`? Defaults to :py:data:`False`.
 
     filename :
 
         The file name to report in error messages. Defaults to ``"<console>"``.
     """
 
     globals: dict[str, Any]
     """The namespace used as the globals"""
 
     stdin_callback: Callable[[int], str] | None
-    """The function to call at each read from :any:`sys.stdin`"""
+    """The function to call at each read from :py:data:`sys.stdin`"""
 
     stdout_callback: Callable[[str], None] | None
-    """Function to call at each write to :any:`sys.stdout`."""
+    """Function to call at each write to :py:data:`sys.stdout`."""
 
     stderr_callback: Callable[[str], None] | None
-    """Function to call at each write to :any:`sys.stderr`."""
+    """Function to call at each write to :py:data:`sys.stderr`."""
 
     buffer: list[str]
-    """The list of strings that have been :any:`pushed <Console.push>` to the console."""
+    """The list of lines of code that have been the argument to
+    :py:meth:`~Console.push`.
+
+    This is emptied whenever the code is executed.
+    """
 
     completer_word_break_characters: str
-    """The set of characters considered by :any:`complete <Console.complete>` to be word breaks."""
+    """The set of characters considered by :py:meth:`~Console.complete` to be word breaks."""
 
     def __init__(
         self,
         globals: dict[str, Any] | None = None,
         *,
         stdin_callback: Callable[[int], str] | None = None,
         stdout_callback: Callable[[str], None] | None = None,
@@ -387,15 +391,15 @@
         sys.last_traceback = None
         return "".join(traceback.format_exception_only(type(e), e))
 
     def num_frames_to_keep(self, tb: TracebackType | None) -> int:
         keep_frames = False
         kept_frames = 0
         # Try to trim out stack frames inside our code
-        for (frame, _) in traceback.walk_tb(tb):
+        for frame, _ in traceback.walk_tb(tb):
             keep_frames = keep_frames or frame.f_code.co_filename == "<console>"
             keep_frames = keep_frames or frame.f_code.co_filename == "<exec>"
             if keep_frames:
                 kept_frames += 1
         return kept_frames
 
     def formattraceback(self, e: BaseException) -> str:
@@ -443,17 +447,17 @@
         ----------
         source :
 
             The source string to complete at the end.
 
         Returns
         -------
-        completions : :any:`list`\[:any:`str`]
+        completions : :py:class:`list`\[:py:class:`str`]
             A list of completion strings.
-        start : :any:`int`
+        start : :py:class:`int`
             The index where completion starts.
 
         Examples
         --------
         >>> shell = Console()
         >>> shell.complete("str.isa")
         (['str.isalnum(', 'str.isalpha(', 'str.isascii('], 0)
@@ -466,25 +470,25 @@
             completions = self._completer.attr_matches(source)
         else:
             completions = self._completer.global_matches(source)
         return completions, start
 
 
 class PyodideConsole(Console):
-    """A subclass of :any:`Console` that uses :any:`pyodide.loadPackagesFromImports` before running the code."""
+    """A subclass of :py:class:`Console` that uses :js:func:`pyodide.loadPackagesFromImports` before running the code."""
 
     async def runcode(self, source: str, code: CodeRunner) -> ConsoleFuture:
         """Execute a code object.
         All exceptions are caught except SystemExit, which is reraised.
         Returns
         -------
             The return value is a dependent sum type with the following possibilities:
             * `("success", result : Any)` -- the code executed successfully
             * `("exception", message : str)` -- An exception occurred. `message` is the
-            result of calling :any:`Console.formattraceback`.
+            result of calling :py:meth:`Console.formattraceback`.
         """
         from pyodide_js import loadPackagesFromImports
 
         await loadPackagesFromImports(source)
         return await super().runcode(source, code)
```

### Comparing `pyodide-py-0.23.0a1/pyodide/ffi/__init__.py` & `pyodide-py-0.23.1/pyodide/ffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.0a1/pyodide/ffi/wrappers.py` & `pyodide-py-0.23.1/pyodide/ffi/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.0a1/pyodide/http.py` & `pyodide-py-0.23.1/pyodide/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,27 +50,27 @@
     """A wrapper for a Javascript fetch :js:data:`Response`.
 
     Parameters
     ----------
     url
         URL to fetch
     js_response
-        A :any:`JsProxy` of the fetch response
+        A :py:class:`~pyodide.ffi.JsProxy` of the fetch response
     """
 
     def __init__(self, url: str, js_response: JsFetchResponse):
         self._url = url
         self.js_response = js_response
 
     @property
     def body_used(self) -> bool:
         """Has the response been used yet?
 
         If so, attempting to retrieve the body again will raise an
-        :any:`OSError`. Use :py:meth:`~FetchResponse.clone` first to avoid this.
+        :py:exc:`OSError`. Use :py:meth:`~FetchResponse.clone` first to avoid this.
         See :js:attr:`Response.bodyUsed`.
         """
         return self.js_response.bodyUsed
 
     @property
     def ok(self) -> bool:
         """Was the request successful?
@@ -125,17 +125,17 @@
             raise OSError(
                 f"Request for {self._url} failed with status {self.status}: {self.status_text}"
             )
         if self.js_response.bodyUsed:
             raise OSError("Response body is already used")
 
     def clone(self) -> "FetchResponse":
-        """Return an identical copy of the :any:`FetchResponse`.
+        """Return an identical copy of the :py:class:`FetchResponse`.
 
-        This method exists to allow multiple uses of :any:`FetchResponse`
+        This method exists to allow multiple uses of :py:class:`FetchResponse`
         objects. See :js:meth:`Response.clone`.
         """
         if self.js_response.bodyUsed:
             raise OSError("Response body is already used")
         return FetchResponse(self._url, self.js_response.clone())
 
     async def buffer(self) -> JsBuffer:
@@ -157,15 +157,15 @@
 
         Any keyword arguments are passed to :py:func:`json.loads`.
         """
         self._raise_if_failed()
         return json.loads(await self.string(), **kwargs)
 
     async def memoryview(self) -> memoryview:
-        """Return the response body as a :any:`memoryview` object"""
+        """Return the response body as a :py:class:`memoryview` object"""
         self._raise_if_failed()
         return (await self.buffer()).to_memoryview()
 
     async def _into_file(self, f: IO[bytes] | IO[str]) -> None:
         """Write the data into an empty file with no copy.
 
         Warning: should only be used when f is an empty file, otherwise it may
@@ -202,31 +202,31 @@
         return (await self.buffer()).to_bytes()
 
     async def unpack_archive(
         self, *, extract_dir: str | None = None, format: str | None = None
     ) -> None:
         """Treat the data as an archive and unpack it into target directory.
 
-        Assumes that the file is an archive in a format that :any:`shutil` has
+        Assumes that the file is an archive in a format that :py:mod:`shutil` has
         an unpacker for. The arguments ``extract_dir`` and ``format`` are passed
-        directly on to :any:`shutil.unpack_archive`.
+        directly on to :py:func:`shutil.unpack_archive`.
 
         Parameters
         ----------
         extract_dir :
             Directory to extract the archive into. If not provided, the current
             working directory is used.
 
         format :
             The archive format: one of ``"zip"``, ``"tar"``, ``"gztar"``,
             ``"bztar"``. Or any other format registered with
             :py:func:`shutil.register_unpack_format`. If not provided,
             :py:meth:`unpack_archive` will use the archive file name extension and
             see if an unpacker was registered for that extension. In case none
-            is found, a :any:`ValueError` is raised.
+            is found, a :py:exc:`ValueError` is raised.
         """
         buf = await self.buffer()
         filename = self._url.rsplit("/", -1)[-1]
         unpack_buffer(buf, filename=filename, format=format, extract_dir=extract_dir)
 
 
 async def pyfetch(url: str, **kwargs: Any) -> FetchResponse:
@@ -247,8 +247,8 @@
         <https://developer.mozilla.org/en-US/docs/Web/API/fetch#options>`_.
     """
     try:
         return FetchResponse(
             url, await _jsfetch(url, to_js(kwargs, dict_converter=Object.fromEntries))
         )
     except JsException as e:
-        raise OSError(e.js_error.message) from None
+        raise OSError(e.message) from None
```

### Comparing `pyodide-py-0.23.0a1/pyodide/webloop.py` & `pyodide-py-0.23.1/pyodide/webloop.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
                         file=sys.stderr,
                     )
                     traceback.print_exc()
 
 
 class WebLoopPolicy(asyncio.DefaultEventLoopPolicy):
     """
-    A simple event loop policy for managing :any:`WebLoop`-based event loops.
+    A simple event loop policy for managing :py:class:`WebLoop`-based event loops.
     """
 
     def __init__(self):
         self._default_loop = None
 
     def get_event_loop(self):
         """Get the current event loop"""
```

### Comparing `pyodide-py-0.23.0a1/pyodide_py.egg-info/PKG-INFO` & `pyodide-py-0.23.1/pyodide_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.23.0a1
+Version: 0.23.1
 Summary: "A Python package providing core interpreter functionality for Pyodide."
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.23.0a1/pyodide_py.egg-info/SOURCES.txt` & `pyodide-py-0.23.1/pyodide_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+./webbrowser.py
 ./_pyodide/__init__.py
 ./_pyodide/_base.py
 ./_pyodide/_core_docs.py
 ./_pyodide/_importhook.py
 ./_pyodide/docs_argspec.py
 ./_pyodide/docstring.py
 ./pyodide/__init__.py
```

### Comparing `pyodide-py-0.23.0a1/setup.cfg` & `pyodide-py-0.23.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyodide-py
-version = 0.23.0a1
+version = 0.23.1
 author = Pyodide developers
 description = "A Python package providing core interpreter functionality for Pyodide."
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyodide/pyodide
 project_urls = 
 	Bug Tracker = https://github.com/pyodide/pyodide/issues
@@ -15,14 +15,15 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >=3.8
+py_modules = webbrowser
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

