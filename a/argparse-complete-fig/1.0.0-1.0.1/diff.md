# Comparing `tmp/argparse_complete_fig-1.0.0.tar.gz` & `tmp/argparse_complete_fig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse_complete_fig-1.0.0.tar", last modified: Fri Jul  1 08:05:02 2022, max compression
+gzip compressed data, was "argparse_complete_fig-1.0.1.tar", last modified: Sat Apr 15 15:02:53 2023, max compression
```

## Comparing `argparse_complete_fig-1.0.0.tar` & `argparse_complete_fig-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 seansullivan   (501) staff       (20)        0 2022-07-01 08:05:02.876134 argparse_complete_fig-1.0.0/
--rw-r--r--   0 seansullivan   (501) staff       (20)     1060 2022-07-01 04:01:29.000000 argparse_complete_fig-1.0.0/LICENSE
--rw-r--r--   0 seansullivan   (501) staff       (20)     1584 2022-07-01 08:05:02.876010 argparse_complete_fig-1.0.0/PKG-INFO
--rw-r--r--   0 seansullivan   (501) staff       (20)      916 2022-07-01 07:59:27.000000 argparse_complete_fig-1.0.0/README.md
-drwxr-xr-x   0 seansullivan   (501) staff       (20)        0 2022-07-01 08:05:02.875105 argparse_complete_fig-1.0.0/argparse_complete_fig/
--rw-r--r--   0 seansullivan   (501) staff       (20)      204 2022-07-01 07:25:59.000000 argparse_complete_fig-1.0.0/argparse_complete_fig/__init__.py
--rw-r--r--   0 seansullivan   (501) staff       (20)     6278 2022-07-01 07:27:50.000000 argparse_complete_fig-1.0.0/argparse_complete_fig/fig.py
-drwxr-xr-x   0 seansullivan   (501) staff       (20)        0 2022-07-01 08:05:02.875816 argparse_complete_fig-1.0.0/argparse_complete_fig.egg-info/
--rw-r--r--   0 seansullivan   (501) staff       (20)     1584 2022-07-01 08:05:02.000000 argparse_complete_fig-1.0.0/argparse_complete_fig.egg-info/PKG-INFO
--rw-r--r--   0 seansullivan   (501) staff       (20)      284 2022-07-01 08:05:02.000000 argparse_complete_fig-1.0.0/argparse_complete_fig.egg-info/SOURCES.txt
--rw-r--r--   0 seansullivan   (501) staff       (20)        1 2022-07-01 08:05:02.000000 argparse_complete_fig-1.0.0/argparse_complete_fig.egg-info/dependency_links.txt
--rw-r--r--   0 seansullivan   (501) staff       (20)       22 2022-07-01 08:05:02.000000 argparse_complete_fig-1.0.0/argparse_complete_fig.egg-info/top_level.txt
--rw-r--r--   0 seansullivan   (501) staff       (20)      788 2022-07-01 08:04:41.000000 argparse_complete_fig-1.0.0/pyproject.toml
--rw-r--r--   0 seansullivan   (501) staff       (20)       38 2022-07-01 08:05:02.876180 argparse_complete_fig-1.0.0/setup.cfg
--rw-r--r--   0 seansullivan   (501) staff       (20)       38 2022-07-01 06:16:42.000000 argparse_complete_fig-1.0.0/setup.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-04-15 15:02:53.690066 argparse_complete_fig-1.0.1/
+-rw-r--r--   0 federico   (501) staff       (20)     1060 2022-08-08 11:52:51.000000 argparse_complete_fig-1.0.1/LICENSE
+-rw-r--r--   0 federico   (501) staff       (20)     1584 2023-04-15 15:02:53.689938 argparse_complete_fig-1.0.1/PKG-INFO
+-rw-r--r--   0 federico   (501) staff       (20)      916 2022-08-08 11:52:51.000000 argparse_complete_fig-1.0.1/README.md
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-04-15 15:02:53.688944 argparse_complete_fig-1.0.1/argparse_complete_fig/
+-rw-r--r--   0 federico   (501) staff       (20)      204 2022-10-03 16:35:34.000000 argparse_complete_fig-1.0.1/argparse_complete_fig/__init__.py
+-rw-r--r--   0 federico   (501) staff       (20)     6474 2023-04-15 14:38:27.000000 argparse_complete_fig-1.0.1/argparse_complete_fig/fig.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-04-15 15:02:53.689476 argparse_complete_fig-1.0.1/argparse_complete_fig.egg-info/
+-rw-r--r--   0 federico   (501) staff       (20)     1584 2023-04-15 15:02:53.000000 argparse_complete_fig-1.0.1/argparse_complete_fig.egg-info/PKG-INFO
+-rw-r--r--   0 federico   (501) staff       (20)      302 2023-04-15 15:02:53.000000 argparse_complete_fig-1.0.1/argparse_complete_fig.egg-info/SOURCES.txt
+-rw-r--r--   0 federico   (501) staff       (20)        1 2023-04-15 15:02:53.000000 argparse_complete_fig-1.0.1/argparse_complete_fig.egg-info/dependency_links.txt
+-rw-r--r--   0 federico   (501) staff       (20)       22 2023-04-15 15:02:53.000000 argparse_complete_fig-1.0.1/argparse_complete_fig.egg-info/top_level.txt
+-rw-r--r--   0 federico   (501) staff       (20)      788 2023-04-15 15:00:05.000000 argparse_complete_fig-1.0.1/pyproject.toml
+-rw-r--r--   0 federico   (501) staff       (20)       38 2023-04-15 15:02:53.690107 argparse_complete_fig-1.0.1/setup.cfg
+-rwxr-xr-x   0 federico   (501) staff       (20)       38 2022-10-02 19:22:03.000000 argparse_complete_fig-1.0.1/setup.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-04-15 15:02:53.689614 argparse_complete_fig-1.0.1/tests/
+-rw-r--r--   0 federico   (501) staff       (20)     2931 2023-04-15 14:56:29.000000 argparse_complete_fig-1.0.1/tests/test_fig.py
```

### Comparing `argparse_complete_fig-1.0.0/LICENSE` & `argparse_complete_fig-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse_complete_fig-1.0.0/PKG-INFO` & `argparse_complete_fig-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse_complete_fig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Autogenerate completions for CLI tools built with argparse
 Author-email: Fig Team <hello@fig.io>
 Maintainer-email: Sean Sullivan <sean@fig.io>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/withfig/autocomplete-tools/issues
 Project-URL: Homepage, https://github.com/withfig/autocomplete-tools
 Keywords: argparse,fig,cli,completions,terminal,framework
@@ -22,15 +22,15 @@
 with Python's built-in [argparse](https://docs.python.org/3/library/argparse.html) module.
 
 ### Installation
 
 Install the integration as a dependency using pip:
 
 ```bash
-pip install argparse_complete_fig
+pip install argparse-complete-fig
 ```
 
 ### Usage
 
 ```python
 import argparse
 from argparse_complete_fig import add_completion_spec_command
```

### Comparing `argparse_complete_fig-1.0.0/README.md` & `argparse_complete_fig-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with Python's built-in [argparse](https://docs.python.org/3/library/argparse.html) module.
 
 ### Installation
 
 Install the integration as a dependency using pip:
 
 ```bash
-pip install argparse_complete_fig
+pip install argparse-complete-fig
 ```
 
 ### Usage
 
 ```python
 import argparse
 from argparse_complete_fig import add_completion_spec_command
```

### Comparing `argparse_complete_fig-1.0.0/argparse_complete_fig/fig.py` & `argparse_complete_fig-1.0.1/argparse_complete_fig/fig.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,24 @@
         else:
             result["description"] = str(arg.help)
     elif arg.dest != argparse.SUPPRESS:
         result["description"] = str(arg.dest)
     return result
 
 
-def construct_args(arg, hooks, parser):
+def construct_args(arg, hooks, parser, add_descriptions = True):
     """Construct Fig arg array given an argparse argument."""
     arg_hook = hooks.get("arg")
 
     # Construct common base_arg object
     base_arg = get_base_suggestion(arg)
 
+    if not add_descriptions and "description" in base_arg:
+      del base_arg["description"]
+
     if hasattr(arg.choices, '__iter__'):
         base_arg["suggestions"] = [str(a) for a in arg.choices]
 
     args = get_arg_list(arg)
 
     # Get names for each arg
     names = get_arg_names(arg, len(args))
@@ -71,15 +74,15 @@
             arg_hook(arg, parser)
 
     return args
 
 
 def construct_option(arg, hooks, parser):
     """Construct Fig option given an argparse argument."""
-    option_args = construct_args(arg, hooks, parser)
+    option_args = construct_args(arg, hooks, parser, add_descriptions=False)
     if len(arg.option_strings) > 1:
         name = [str(name) for name in arg.option_strings]
     else:
         name = arg.option_strings[0]
 
     option = {
         "name": name,
@@ -176,31 +179,33 @@
 const completionSpec: Fig.Spec = {json.dumps(spec, indent=2)}
 export default completionSpec;"""
 
 
 class GenerateFigSpecAction(argparse.Action):
     def __init__(
         self,
-        dest=argparse.SUPPRESS,
-        help="Generate fig completion spec for this parser."
+        option_strings,
+        help="Generate fig completion spec for this parser",
+        *args,
+        **kwargs,
     ):
         super(GenerateFigSpecAction, self).__init__(
-            option_strings=["--generate-fig-spec"],
-            dest=dest,
+            option_strings=option_strings,
+            dest=argparse.SUPPRESS,
             default=argparse.SUPPRESS,
             help=help,
-            nargs=0
+            nargs=0,
         )
 
     def __call__(self, parser, namespace, values, option_string=None):
         def option_hook(option, _parser):
             if option["name"] == "--generate-fig-spec":
                 option["priority"] = 0
 
         hooks = {"option": option_hook}
         spec = generate_completion_spec(parser, hooks)
         print(spec)
         parser.exit()
 
 
 def add_completion_spec_command(parser):
-    parser.add_argument(action=GenerateFigSpecAction)
+    parser.add_argument("--generate-fig-spec", action=GenerateFigSpecAction)
```

### Comparing `argparse_complete_fig-1.0.0/argparse_complete_fig.egg-info/PKG-INFO` & `argparse_complete_fig-1.0.1/argparse_complete_fig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-complete-fig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Autogenerate completions for CLI tools built with argparse
 Author-email: Fig Team <hello@fig.io>
 Maintainer-email: Sean Sullivan <sean@fig.io>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/withfig/autocomplete-tools/issues
 Project-URL: Homepage, https://github.com/withfig/autocomplete-tools
 Keywords: argparse,fig,cli,completions,terminal,framework
@@ -22,15 +22,15 @@
 with Python's built-in [argparse](https://docs.python.org/3/library/argparse.html) module.
 
 ### Installation
 
 Install the integration as a dependency using pip:
 
 ```bash
-pip install argparse_complete_fig
+pip install argparse-complete-fig
 ```
 
 ### Usage
 
 ```python
 import argparse
 from argparse_complete_fig import add_completion_spec_command
```

### Comparing `argparse_complete_fig-1.0.0/pyproject.toml` & `argparse_complete_fig-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "argparse_complete_fig"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "Fig Team", email =  "hello@fig.io" }]
 maintainers = [{ name = "Sean Sullivan", email =  "sean@fig.io" }]
 description = "Autogenerate completions for CLI tools built with argparse"
 readme = "README.md"
 requires-python = ">=3.5"
 license = { text = "MIT" }
 keywords = ["argparse", "fig", "cli", "completions", "terminal", "framework"]
```

