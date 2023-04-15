# Comparing `tmp/pylint_keyword_only_args_plugin-0.1.0.tar.gz` & `tmp/pylint_keyword_only_args_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_keyword_only_args_plugin-0.1.0.tar", max compression
+gzip compressed data, was "pylint_keyword_only_args_plugin-0.2.0.tar", max compression
```

## Comparing `pylint_keyword_only_args_plugin-0.1.0.tar` & `pylint_keyword_only_args_plugin-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      232 2023-04-14 02:47:21.898835 pylint_keyword_only_args_plugin-0.1.0/README.md
--rw-r--r--   0        0        0       71 2023-04-14 02:31:08.436703 pylint_keyword_only_args_plugin-0.1.0/pylint_keyword_only_args_plugin/__init__.py
--rw-r--r--   0        0        0      683 2023-04-14 02:44:39.978827 pylint_keyword_only_args_plugin-0.1.0/pylint_keyword_only_args_plugin/checker.py
--rw-r--r--   0        0        0      159 2023-04-14 02:30:27.305357 pylint_keyword_only_args_plugin-0.1.0/pylint_keyword_only_args_plugin/keyword_only_args.py
--rw-r--r--   0        0        0     1038 2023-04-14 02:47:39.361240 pylint_keyword_only_args_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pylint_keyword_only_args_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-04-14 02:47:21.898835 pylint_keyword_only_args_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0       71 2023-04-14 02:31:08.436703 pylint_keyword_only_args_plugin-0.2.0/pylint_keyword_only_args_plugin/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-15 05:43:00.184647 pylint_keyword_only_args_plugin-0.2.0/pylint_keyword_only_args_plugin/checker.py
+-rw-r--r--   0        0        0      159 2023-04-14 02:30:27.305357 pylint_keyword_only_args_plugin-0.2.0/pylint_keyword_only_args_plugin/keyword_only_args.py
+-rw-r--r--   0        0        0     1025 2023-04-15 05:48:32.519358 pylint_keyword_only_args_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 pylint_keyword_only_args_plugin-0.2.0/PKG-INFO
```

### Comparing `pylint_keyword_only_args_plugin-0.1.0/pyproject.toml` & `pylint_keyword_only_args_plugin-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-keyword-only-args-plugin"
-version = "0.1.0"
+version = "0.2.0"
 description = "Plugin for pylint which checks that call statements has only keyword args"
 authors = ["Konstantin Shestakov <winmasta@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/winmasta"
 repository = "https://github.com/winmasta"
 keywords = ["pylint", "positional", "args", "lint"]
@@ -15,15 +15,14 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pylint = "*"
-pytest = "*"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
```

### Comparing `pylint_keyword_only_args_plugin-0.1.0/PKG-INFO` & `pylint_keyword_only_args_plugin-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-keyword-only-args-plugin
-Version: 0.1.0
+Version: 0.2.0
 Summary: Plugin for pylint which checks that call statements has only keyword args
 Home-page: https://github.com/winmasta
 License: MIT
 Keywords: pylint,positional,args,lint
 Author: Konstantin Shestakov
 Author-email: winmasta@yandex.ru
 Requires-Python: >=3.11,<4.0
@@ -13,15 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: pylint
-Requires-Dist: pytest
 Project-URL: Repository, https://github.com/winmasta
 Description-Content-Type: text/markdown
 
 ## Plugin for pylint which checks that call statements has only keyword args
 
 Install:
 ```bash
```

