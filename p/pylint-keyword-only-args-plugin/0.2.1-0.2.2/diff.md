# Comparing `tmp/pylint_keyword_only_args_plugin-0.2.1.tar.gz` & `tmp/pylint_keyword_only_args_plugin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_keyword_only_args_plugin-0.2.1.tar", max compression
+gzip compressed data, was "pylint_keyword_only_args_plugin-0.2.2.tar", max compression
```

## Comparing `pylint_keyword_only_args_plugin-0.2.1.tar` & `pylint_keyword_only_args_plugin-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      410 2023-04-15 06:23:07.303291 pylint_keyword_only_args_plugin-0.2.1/README.md
--rw-r--r--   0        0        0       71 2023-04-14 02:31:08.436703 pylint_keyword_only_args_plugin-0.2.1/pylint_keyword_only_args_plugin/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-15 06:23:31.730116 pylint_keyword_only_args_plugin-0.2.1/pylint_keyword_only_args_plugin/checker.py
--rw-r--r--   0        0        0      159 2023-04-14 02:30:27.305357 pylint_keyword_only_args_plugin-0.2.1/pylint_keyword_only_args_plugin/keyword_only_args.py
--rw-r--r--   0        0        0     1025 2023-04-15 06:23:31.734116 pylint_keyword_only_args_plugin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 pylint_keyword_only_args_plugin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-04-15 06:23:07.303291 pylint_keyword_only_args_plugin-0.2.2/README.md
+-rw-r--r--   0        0        0       71 2023-04-14 02:31:08.436703 pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/__init__.py
+-rw-r--r--   0        0        0     1455 2023-04-15 06:37:14.205163 pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/checker.py
+-rw-r--r--   0        0        0      159 2023-04-14 02:30:27.305357 pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/keyword_only_args.py
+-rw-r--r--   0        0        0     1025 2023-04-15 06:38:24.538133 pylint_keyword_only_args_plugin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 pylint_keyword_only_args_plugin-0.2.2/PKG-INFO
```

### Comparing `pylint_keyword_only_args_plugin-0.2.1/pylint_keyword_only_args_plugin/checker.py` & `pylint_keyword_only_args_plugin-0.2.2/pylint_keyword_only_args_plugin/checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import builtins
 from typing import Iterable
 
-from astroid.nodes import Call, Assign, Tuple
+from astroid.nodes import Call, Assign, Tuple, Attribute
 from pylint.checkers import BaseChecker
 
 
 class KeywordOnlyArgsChecker(BaseChecker):
     name = "keyword-only-args"
     priority = -100
     msgs = {
@@ -30,12 +30,17 @@
                 nodes = [node.value]
 
             if isinstance(node.value, Tuple):
                 nodes = node.value.elts
 
         skip_names_list = [*dir(builtins), *self.linter.config.skip_names_list.split(","), "Path"]
         for _node in nodes:
-            if _node.func.name in skip_names_list:
+            if isinstance(_node.func, Attribute):
+                node_name = _node.func.attrname
+            else:
+                node_name = _node.func.name
+
+            if node_name in skip_names_list:
                 return
 
-            if node.args:
+            if _node.args:
                 self.add_message("keyword-only-args", node=_node)
```

### Comparing `pylint_keyword_only_args_plugin-0.2.1/pyproject.toml` & `pylint_keyword_only_args_plugin-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-keyword-only-args-plugin"
-version = "0.2.1"
+version = "0.2.2"
 description = "Plugin for pylint which checks that call statements has only keyword args"
 authors = ["Konstantin Shestakov <winmasta@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/winmasta"
 repository = "https://github.com/winmasta"
 keywords = ["pylint", "positional", "args", "lint"]
```

### Comparing `pylint_keyword_only_args_plugin-0.2.1/PKG-INFO` & `pylint_keyword_only_args_plugin-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-keyword-only-args-plugin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Plugin for pylint which checks that call statements has only keyword args
 Home-page: https://github.com/winmasta
 License: MIT
 Keywords: pylint,positional,args,lint
 Author: Konstantin Shestakov
 Author-email: winmasta@yandex.ru
 Requires-Python: >=3.11,<4.0
```

