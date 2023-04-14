# Comparing `tmp/pyodide-build-0.23.0a1.tar.gz` & `tmp/pyodide-build-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-build-0.23.0a1.tar", last modified: Tue Jan 24 07:46:59 2023, max compression
+gzip compressed data, was "pyodide-build-0.23.1.tar", last modified: Fri Apr 14 22:15:34 2023, max compression
```

## Comparing `pyodide-build-0.23.0a1.tar` & `pyodide-build-0.23.1.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.653053 pyodide-build-0.23.0a1/pyodide_build/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/_f2c_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/_py_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26739 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/buildall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29050 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/buildpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/pyodide_build/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/build_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/create_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/py_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/cli/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/create_pypa_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/create_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/install_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11496 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/mkpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/pyodide_build/out_of_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/out_of_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/out_of_tree/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/out_of_tree/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/out_of_tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/out_of_tree/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/pypabuild.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20109 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/pywasmcross.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/pyzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/pyodide_build/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.653053 pyodide-build-0.23.0a1/pyodide_build/tools/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.653053 pyodide-build-0.23.0a1/pyodide_build/tools/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/pyodide_build/tools/cmake/Modules/Platform/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyodide_build/tools/pyo3_config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/pyodide_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-24 07:46:59.000000 pyodide-build-0.23.0a1/pyodide_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-24 07:46:59.000000 pyodide-build-0.23.0a1/pyodide_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 07:46:59.000000 pyodide-build-0.23.0a1/pyodide_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-24 07:46:59.000000 pyodide-build-0.23.0a1/pyodide_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-24 07:46:59.000000 pyodide-build-0.23.0a1/pyodide_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-24 07:46:59.000000 pyodide-build-0.23.0a1/pyodide_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-24 07:46:59.657053 pyodide-build-0.23.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-24 07:46:45.000000 pyodide-build-0.23.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/_f2c_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/_py_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27665 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/buildall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31327 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/buildpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/build_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/create_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/py_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/create_pypa_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/create_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/install_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8595 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/mkpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/out_of_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/pypabuild.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20853 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/pywasmcross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/pyzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.213459 pyodide-build-0.23.1/pyodide_build/tools/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.213459 pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/Platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/tools/pyo3_config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/pyodide_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/setup.py
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/__main__.py` & `pyodide-build-0.23.1/pyodide_build/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 #!/usr/bin/env python3
 import argparse
 import sys
 
-from . import buildall, buildpkg, create_xbuildenv, install_xbuildenv, mkpkg, serve
+from . import buildpkg, create_xbuildenv, install_xbuildenv, serve
 from .common import init_environment
 
 
 def make_parser() -> argparse.ArgumentParser:
-    """Create an argument parser with argparse"""
+    """Create an argument parser with argparse
 
-    main_parser = argparse.ArgumentParser(prog="pyodide")
-    main_parser.description = "A command line interface (CLI) for pyodide_build"
+    This is an internal CLI.
+    """
+
+    main_parser = argparse.ArgumentParser(prog="pyodide-build")
+    main_parser.description = (
+        "An internal command line interface (CLI) for pyodide_build\n"
+        "Users should instead use the main `pyodide` CLI."
+    )
     subparsers = main_parser.add_subparsers(help="action")
 
     for command_name, module in (
         ("buildpkg", buildpkg),
-        ("buildall", buildall),
         ("serve", serve),
-        ("mkpkg", mkpkg),
         ("create_xbuildenv", create_xbuildenv),
         ("install_xbuildenv", install_xbuildenv),
     ):
         if "sphinx" in sys.modules and command_name in [
             "buildpkg",
-            "buildall",
             "pywasmcross",
         ]:
             # Likely building documentation, skip private API
             continue
         parser = module.make_parser(subparsers.add_parser(command_name))
         parser.set_defaults(func=module.main)
     return main_parser
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/_f2c_fixes.py` & `pyodide-build-0.23.1/pyodide_build/_f2c_fixes.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,29 @@
                 int second_(real *t) {
                     *t = clock()/1000;
                     return 0;
                 }
                 """
             )
 
+    # In numpy 1.24 f2py changed its treatment of character argument. In
+    # particular it does not generate a ftnlen parameter for each
+    # character parameter but f2c still generates it. The following code
+    # removes unneeded ftnlen parameters from the f2ced signature. The
+    # problematic subroutines and parameters are the ones with a type character
+    # in scipy/sparse/linalg/_eigen/arpack/arpack.pyf.src
+    if "eupd.c" in str(f2c_output):
+        # put signature on a single line to make replacement more
+        # straightforward
+        regrouped_lines = regroup_lines(lines)
+        lines = [
+            re.sub(r",?\s*ftnlen\s*(howmny_len|bmat_len)", "", line)
+            for line in regrouped_lines
+        ]
+
     with open(f2c_output, "w") as f:
         f.writelines(lines)
 
     return None
 
 
 def add_externs_to_structs(lines: list[str]) -> None:
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/buildall.py` & `pyodide-build-0.23.1/pyodide_build/buildall.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python3
 
 """
 Build all of the packages in a given directory.
 """
 
-import argparse
-import copy
 import dataclasses
 import hashlib
 import json
 import shutil
 import subprocess
 import sys
 from collections import defaultdict
@@ -24,19 +22,20 @@
 from typing import Any
 
 from rich.live import Live
 from rich.progress import BarColumn, Progress, TimeElapsedColumn
 from rich.spinner import Spinner
 from rich.table import Table
 
-from . import common
+from . import common, recipe
 from .buildpkg import needs_rebuild
-from .common import find_matching_wheels, find_missing_executables
+from .common import find_matching_wheels, find_missing_executables, repack_zip_archive
 from .io import MetaConfig, _BuildSpecTypes
 from .logger import console_stdout, logger
+from .pywasmcross import BuildArgs
 
 
 class BuildError(Exception):
     def __init__(self, returncode: int) -> None:
         self.returncode = returncode
         super().__init__()
 
@@ -71,34 +70,30 @@
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.name})"
 
     def needs_rebuild(self) -> bool:
         return needs_rebuild(self.pkgdir, self.pkgdir / "build", self.meta.source)
 
-    def build(self, args: Any) -> None:
+    def build(self, build_args: BuildArgs) -> None:
         raise NotImplementedError()
 
     def dist_artifact_path(self) -> Path:
         raise NotImplementedError()
 
     def tests_path(self) -> Path | None:
         return None
 
 
 @dataclasses.dataclass
 class Package(BasePackage):
-    def __init__(self, pkgdir: Path):
+    def __init__(self, pkgdir: Path, config: MetaConfig):
         self.pkgdir = pkgdir
+        self.meta = config.copy(deep=True)
 
-        pkgpath = pkgdir / "meta.yaml"
-        if not pkgpath.is_file():
-            raise ValueError(f"Directory {pkgdir} does not contain meta.yaml")
-
-        self.meta = MetaConfig.from_yaml(pkgpath)
         self.name = self.meta.package.name
         self.version = self.meta.package.version
         self.disabled = self.meta.package.disabled
         self.package_type = self.meta.build.package_type
 
         assert self.name == pkgdir.name, f"{self.name} != {pkgdir.name}"
 
@@ -126,50 +121,45 @@
     def tests_path(self) -> Path | None:
         tests = list((self.pkgdir / "dist").glob("*-tests.tar"))
         assert len(tests) <= 1
         if tests:
             return tests[0]
         return None
 
-    def build(self, args: Any) -> None:
-
+    def build(self, build_args: BuildArgs) -> None:
         p = subprocess.run(
             [
                 sys.executable,
                 "-m",
                 "pyodide_build",
                 "buildpkg",
                 str(self.pkgdir / "meta.yaml"),
-                f"--cflags={args.cflags}",
-                f"--cxxflags={args.cxxflags}",
-                f"--ldflags={args.ldflags}",
-                f"--target-install-dir={args.target_install_dir}",
-                f"--host-install-dir={args.host_install_dir}",
+                f"--cflags={build_args.cflags}",
+                f"--cxxflags={build_args.cxxflags}",
+                f"--ldflags={build_args.ldflags}",
+                f"--target-install-dir={build_args.target_install_dir}",
+                f"--host-install-dir={build_args.host_install_dir}",
                 # Either this package has been updated and this doesn't
                 # matter, or this package is dependent on a package that has
                 # been updated and should be rebuilt even though its own
                 # files haven't been updated.
                 "--force-rebuild",
             ],
             check=False,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
 
-        log_dir = Path(args.log_dir).resolve() if args.log_dir else None
-        if log_dir and (self.pkgdir / "build.log").exists():
-            log_dir.mkdir(exist_ok=True, parents=True)
-            shutil.copy(
-                self.pkgdir / "build.log",
-                log_dir / f"{self.name}.log",
-            )
-
         if p.returncode != 0:
             logger.error(f"Error building {self.name}. Printing build logs.")
-            logger.error((self.pkgdir / "build.log").read_text(encoding="utf-8"))
+            logfile = self.pkgdir / "build.log"
+            if logfile.is_file():
+                logger.error(logfile.read_text(encoding="utf-8"))
+            else:
+                logger.error("ERROR: No build log found.")
             logger.error("ERROR: cancelling buildall")
             raise BuildError(p.returncode)
 
 
 class PackageStatus:
     def __init__(
         self, *, name: str, idx: int, thread: int, total_packages: int
@@ -245,146 +235,206 @@
         """Step the progress bar by one (to show that a package finished)"""
         self.progress.update(self.task, advance=1)
 
     def __rich__(self):
         return self.main_grid
 
 
-def validate_dependencies(pkg_map: dict[str, BasePackage]) -> None:
+def _validate_package_map(pkg_map: dict[str, BasePackage]) -> bool:
+    # Check if dependencies are valid
     for pkg_name, pkg in pkg_map.items():
         for runtime_dep_name in pkg.run_dependencies:
             runtime_dep = pkg_map[runtime_dep_name]
             if runtime_dep.package_type == "static_library":
                 raise ValueError(
                     f"{pkg_name} has an invalid dependency: {runtime_dep_name}. Static libraries must be a host dependency."
                 )
 
+    # Check executables required to build packages are available
+    missing_executables = defaultdict(list)
+    for name, pkg in pkg_map.items():
+        for exe in find_missing_executables(pkg.executables_required):
+            missing_executables[exe].append(name)
+
+    if missing_executables:
+        error_msg = "The following executables are missing in the host system:\n"
+        for executable, pkgs in missing_executables.items():
+            error_msg += f"- {executable} (required by: {', '.join(pkgs)})\n"
+
+        raise RuntimeError(error_msg)
+
+    return True
+
+
+def _parse_package_query(query: list[str] | str | None) -> tuple[set[str], set[str]]:
+    """
+    Parse a package query string into a list of requested packages and a list of
+    disabled packages.
+
+    Parameters
+    ----------
+    query
+        A list of packages to build, this can be a comma separated string.
+
+    Returns
+    -------
+    A tuple of two lists, the first list contains requested packages, the second
+    list contains disabled packages.
+
+    Examples
+    --------
+    >>> _parse_package_query(None)
+    (set(), set())
+    >>> requested, disabled = _parse_package_query("a,b,c")
+    >>> requested == {'a', 'b', 'c'}, disabled == set()
+    (True, True)
+    >>> requested, disabled = _parse_package_query("a,b,!c")
+    >>> requested == {'a', 'b'}, disabled == {'c'}
+    (True, True)
+    >>> requested, disabled = _parse_package_query(["a", "b", "!c"])
+    >>> requested == {'a', 'b'}, disabled == {'c'}
+    (True, True)
+    """
+    if not query:
+        query = []
+
+    if isinstance(query, str):
+        query = [el.strip() for el in query.split(",")]
+
+    requested = set()
+    disabled = set()
+
+    for name in query:
+        if not name:  # empty string
+            continue
+
+        if name.startswith("!"):
+            disabled.add(name[1:])
+        else:
+            requested.add(name)
+
+    return requested, disabled
+
 
 def generate_dependency_graph(
-    packages_dir: Path, packages: set[str]
+    packages_dir: Path,
+    requested: set[str],
+    disabled: set[str] | None = None,
 ) -> dict[str, BasePackage]:
-    """This generates a dependency graph for listed packages.
+    """This generates a dependency graph for given packages.
 
     A node in the graph is a BasePackage object defined above, which maintains
     a list of dependencies and also dependents. That is, each node stores both
     incoming and outgoing edges.
 
     The dependencies and dependents are stored via their name, and we have a
     lookup table pkg_map: Dict[str, BasePackage] to look up the corresponding
     BasePackage object. The function returns pkg_map, which contains all
     packages in the graph as its values.
 
-    Parameters:
-     - packages_dir: directory that contains packages
-     - packages: set of packages to build. If None, then all packages in
-       packages_dir are compiled.
-
-    Returns:
-     - pkg_map: dictionary mapping package names to BasePackage objects
+    Parameters
+    ----------
+    packages_dir
+        A directory that contains packages
+    requested
+        A set of packages to build
+    disabled
+        A set of packages to not build
+
+    Returns
+    -------
+    A dictionary mapping package names to BasePackage objects
     """
+
     pkg: BasePackage
     pkgname: str
     pkg_map: dict[str, BasePackage] = {}
 
-    if "*" in packages:
-        packages.discard("*")
-        packages.update(
-            str(x.name) for x in packages_dir.iterdir() if (x / "meta.yaml").is_file()
-        )
-
-    no_numpy_dependents = "no-numpy-dependents" in packages
-    if no_numpy_dependents:
-        packages.discard("no-numpy-dependents")
-
-    disabled_packages = set()
-    for pkgname in list(packages):
-        if pkgname.startswith("!"):
-            packages.discard(pkgname)
-            disabled_packages.add(pkgname[1:])
-
-    # Record which packages were requested. We need this information because
-    # some packages are reachable from the initial set but are only reachable
-    # via a disabled dependency.
-    # Example: scikit-learn needs joblib & scipy, scipy needs numpy but numpy disabled.
-    # We don't want to build joblib.
-    requested = set(packages)
+    if not disabled:
+        disabled = set()
 
     # Create dependency graph.
     # On first pass add all dependencies regardless of whether
     # disabled since it might happen because of a transitive dependency
     graph = {}
+    all_recipes = recipe.load_all_recipes(packages_dir)
+    no_numpy_dependents = "no-numpy-dependents" in requested
+    requested.discard("no-numpy-dependents")
+    packages = requested.copy()
+
     while packages:
         pkgname = packages.pop()
 
-        pkg = Package(packages_dir / pkgname)
+        if pkgname not in all_recipes:
+            raise ValueError(
+                f"No metadata file found for the following package: {pkgname}"
+            )
+
+        pkg = Package(packages_dir / pkgname, all_recipes[pkgname])
         pkg_map[pkgname] = pkg
         graph[pkgname] = pkg.dependencies
         for dep in pkg.dependencies:
             if pkg_map.get(dep) is None:
                 packages.add(dep)
 
-    validate_dependencies(pkg_map)
-
     # Traverse in build order (dependencies first then dependents)
     # Mark a package as disabled if they've either been explicitly disabled
     # or if any of its transitive dependencies were marked disabled.
     for pkgname in TopologicalSorter(graph).static_order():
         pkg = pkg_map[pkgname]
-        if pkgname in disabled_packages:
+        if pkgname in disabled:
             pkg.disabled = True
             continue
         if no_numpy_dependents and "numpy" in pkg.dependencies:
             pkg.disabled = True
             continue
         for dep in pkg.dependencies:
             if pkg_map[dep].disabled:
                 pkg.disabled = True
                 break
 
     # Now traverse in reverse build order (dependents first then their
     # dependencies).
     # Locate the subset of packages that are transitive dependencies of packages
     # that are requested and not disabled.
+    requested_with_deps = requested.copy()
     for pkgname in reversed(list(TopologicalSorter(graph).static_order())):
         pkg = pkg_map[pkgname]
         if pkg.disabled:
-            requested.discard(pkgname)
+            requested_with_deps.discard(pkgname)
             continue
 
-        if pkgname not in requested:
+        if pkgname not in requested_with_deps:
             continue
 
-        requested.update(pkg.dependencies)
+        requested_with_deps.update(pkg.dependencies)
         for dep in pkg.host_dependencies:
             pkg_map[dep].host_dependents.add(pkg.name)
 
-    # Check executables required to build packages
-    missing_executables = defaultdict(list)
-    for name in requested:
-        pkg = pkg_map[name]
-        for exe in find_missing_executables(pkg.executables_required):
-            missing_executables[exe].append(name)
+    pkg_map = {name: pkg_map[name] for name in requested_with_deps}
 
-    if missing_executables:
-        error_msg = "The following executables are missing in the host system:\n"
-        for executable, pkgs in missing_executables.items():
-            error_msg += f"- {executable} (required by: {', '.join(pkgs)})\n"
-
-        raise RuntimeError(error_msg)
+    _validate_package_map(pkg_map)
 
-    return {name: pkg_map[name] for name in requested}
+    return pkg_map
 
 
 def job_priority(pkg: BasePackage) -> int:
     if pkg.name == "numpy":
         return 0
     else:
         return 1
 
 
+def is_rust_package(pkg: BasePackage) -> bool:
+    """
+    Check if a package requires rust toolchain to build.
+    """
+    return any([q in pkg.executables_required for q in ("rustc", "cargo", "rustup")])
+
+
 def format_name_list(l: list[str]) -> str:
     """
     >>> format_name_list(["regex"])
     'regex'
     >>> format_name_list(["regex", "parso"])
     'regex and parso'
     >>> format_name_list(["regex", "parso", "jedi"])
@@ -425,37 +475,42 @@
     for pkg in pkg_map.values():
         # Otherwise, rebuild packages that have been updated and their dependents.
         if pkg.needs_rebuild():
             mark_package_needs_build(pkg_map, pkg, needs_build)
     return needs_build
 
 
-def build_from_graph(pkg_map: dict[str, BasePackage], args: argparse.Namespace) -> None:
+def build_from_graph(
+    pkg_map: dict[str, BasePackage],
+    build_args: BuildArgs,
+    n_jobs: int = 1,
+    force_rebuild: bool = False,
+) -> None:
     """
-    This builds packages in pkg_map in parallel, building at most args.n_jobs
+    This builds packages in pkg_map in parallel, building at most n_jobs
     packages at once.
 
     We have a priority queue of packages we are ready to build (build_queue),
     where a package is ready to build if all its dependencies are built. The
     priority is based on the number of dependents --- we prefer to build
     packages with more dependents first.
 
-    To build packages in parallel, we use a thread pool of args.n_jobs many
+    To build packages in parallel, we use a thread pool of n_jobs many
     threads listening to build_queue. When the thread is free, it takes an
     item off build_queue and builds it. Once the package is built, it sends the
     package to the built_queue. The main thread listens to the built_queue and
     checks if any of the dependents are ready to be built. If so, it adds the
     package to the build queue.
     """
 
     # Insert packages into build_queue. We *must* do this after counting
     # dependents, because the ordering ought not to change after insertion.
     build_queue: PriorityQueue[tuple[int, BasePackage]] = PriorityQueue()
 
-    if args.force_rebuild:
+    if force_rebuild:
         # If "force_rebuild" is set, just rebuild everything
         needs_build = set(pkg_map.keys())
     else:
         needs_build = generate_needs_build_set(pkg_map)
 
     # We won't rebuild the complement of the packages that we will build.
     already_built = set(pkg_map.keys()).difference(needs_build)
@@ -483,49 +538,70 @@
         pkg = pkg_map[pkg_name]
         if len(pkg.unbuilt_host_dependencies) == 0:
             build_queue.put((job_priority(pkg), pkg))
 
     built_queue: Queue[BasePackage | Exception] = Queue()
     thread_lock = Lock()
     queue_idx = 1
+    building_rust_pkg = False
     progress_formatter = ReplProgressFormatter(len(needs_build))
 
     def builder(n: int) -> None:
-        nonlocal queue_idx
+        nonlocal queue_idx, building_rust_pkg
         while True:
-            pkg = build_queue.get()[1]
+            _, pkg = build_queue.get()
 
             with thread_lock:
+                if is_rust_package(pkg):
+                    # Don't build multiple rust packages at the same time.
+                    # See: https://github.com/pyodide/pyodide/issues/3565
+                    # Note that if there are only rust packages left in the queue,
+                    # this will keep pushing and popping packages until the current rust package
+                    # is built. This is not ideal but presumably the overhead is negligible.
+                    if building_rust_pkg:
+                        build_queue.put((job_priority(pkg), pkg))
+
+                        # Release the GIL so new packages get queued
+                        sleep(0.1)
+                        continue
+
+                    building_rust_pkg = True
+
                 pkg._queue_idx = queue_idx
                 queue_idx += 1
 
             pkg_status = progress_formatter.add_package(
                 name=pkg.name,
                 idx=pkg._queue_idx,
                 thread=n,
                 total_packages=len(needs_build),
             )
             t0 = perf_counter()
 
             success = True
             try:
-                pkg.build(args)
+                pkg.build(build_args)
             except Exception as e:
                 built_queue.put(e)
                 success = False
                 return
             finally:
                 pkg_status.finish(success, perf_counter() - t0)
                 progress_formatter.remove_package(pkg_status)
 
             built_queue.put(pkg)
+
+            with thread_lock:
+                if is_rust_package(pkg):
+                    building_rust_pkg = False
+
             # Release the GIL so new packages get queued
             sleep(0.01)
 
-    for n in range(0, args.n_jobs):
+    for n in range(0, n_jobs):
         Thread(target=builder, args=(n + 1,), daemon=True).start()
 
     num_built = len(already_built)
     with Live(progress_formatter, console=console_stdout):
         while num_built < len(pkg_map):
             match built_queue.get():
                 case BuildError() as err:
@@ -567,14 +643,15 @@
             continue
         pkg_entry: Any = {
             "name": name,
             "version": pkg.version,
             "file_name": pkg.file_name,
             "install_dir": pkg.install_dir,
             "sha256": _generate_package_hash(Path(output_dir, pkg.file_name)),
+            "package_type": pkg.package_type,
             "imports": [],
         }
 
         pkg_type = pkg.package_type
         if pkg_type in ("shared_library", "cpython_module"):
             # We handle cpython modules as shared libraries
             pkg_entry["shared_library"] = True
@@ -614,197 +691,138 @@
 
 
 def generate_repodata(
     output_dir: Path, pkg_map: dict[str, BasePackage]
 ) -> dict[str, dict[str, Any]]:
     """Generate the package.json file"""
 
-    import sys
-
-    sys.path.append(str(common.get_pyodide_root() / "src/py"))
-    from pyodide import __version__
+    from . import __version__
 
     # Build package.json data.
     [platform, _, arch] = common.platform().rpartition("_")
     info = {
         "arch": arch,
         "platform": platform,
+        # This assumes that pyodide-build version == pyodide version.
         "version": __version__,
         "python": sys.version.partition(" ")[0],
     }
     packages = generate_packagedata(output_dir, pkg_map)
     return dict(info=info, packages=packages)
 
 
 def copy_packages_to_dist_dir(
-    packages: Iterable[BasePackage], output_dir: Path
+    packages: Iterable[BasePackage], output_dir: Path, compression_level: int = 6
 ) -> None:
     for pkg in packages:
         if pkg.package_type == "static_library":
             continue
 
-        shutil.copy(pkg.dist_artifact_path(), output_dir)
+        dist_artifact_path = pkg.dist_artifact_path()
+
+        shutil.copy(dist_artifact_path, output_dir)
+        repack_zip_archive(
+            output_dir / dist_artifact_path.name, compression_level=compression_level
+        )
 
         test_path = pkg.tests_path()
         if test_path:
             shutil.copy(test_path, output_dir)
 
 
 def build_packages(
-    packages_dir: Path, args: argparse.Namespace
+    packages_dir: Path,
+    targets: str,
+    build_args: BuildArgs,
+    n_jobs: int = 1,
+    force_rebuild: bool = False,
 ) -> dict[str, BasePackage]:
-    packages = common._parse_package_subset(args.only)
-    pkg_map = generate_dependency_graph(packages_dir, packages)
+    requested, disabled = _parse_package_query(targets)
+    requested_packages = recipe.load_recipes(packages_dir, requested)
+    pkg_map = generate_dependency_graph(
+        packages_dir, set(requested_packages.keys()), disabled
+    )
 
-    build_from_graph(pkg_map, args)
+    build_from_graph(pkg_map, build_args, n_jobs, force_rebuild)
     for pkg in pkg_map.values():
         assert isinstance(pkg, Package)
 
         if pkg.package_type == "static_library":
             continue
 
         pkg.file_name = pkg.dist_artifact_path().name
         pkg.unvendored_tests = pkg.tests_path()
 
     return pkg_map
 
 
-def install_packages(pkg_map: dict[str, BasePackage], output_dir: Path) -> None:
+def copy_logs(pkg_map: dict[str, BasePackage], log_dir: Path) -> None:
+    """
+    Copy build logs of packages to the log directory.
+    Parameters
+    ----------
+    pkg_map
+        A dictionary mapping package names to package objects.
+    log_dir
+        The directory to copy the logs to.
+    """
+
+    log_dir.mkdir(exist_ok=True, parents=True)
+    logger.info(f"Copying build logs to {log_dir}")
+
+    for pkg in pkg_map.values():
+        log_file = pkg.pkgdir / "build.log"
+        if log_file.exists():
+            shutil.copy(log_file, log_dir / f"{pkg.name}.log")
+        else:
+            logger.warning(f"Warning: {pkg.name} has no build log")
+
+
+def install_packages(
+    pkg_map: dict[str, BasePackage], output_dir: Path, compression_level: int = 6
+) -> None:
     """
     Install packages into the output directory.
     - copies build artifacts (wheel, zip, ...) to the output directory
     - create repodata.json
 
 
     pkg_map
         package map created from build_packages
 
     output_dir
         output directory to install packages into
     """
 
     output_dir.mkdir(exist_ok=True, parents=True)
-    copy_packages_to_dist_dir(pkg_map.values(), output_dir)
-    package_data = generate_repodata(output_dir, pkg_map)
 
-    with open(output_dir / "repodata.json", "w") as fd:
-        json.dump(package_data, fd)
-        fd.write("\n")
+    logger.info(f"Copying built packages to {output_dir}")
+    copy_packages_to_dist_dir(
+        pkg_map.values(), output_dir, compression_level=compression_level
+    )
 
+    repodata_path = output_dir / "repodata.json"
+    logger.info(f"Writing repodata.json to {repodata_path}")
 
-def make_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.description = (
-        "Build all the packages in a given directory\n\n"
-        "Unless the --only option is provided\n\n"
-        "Note: this is a private endpoint that should not be used "
-        "outside of the pyodide Makefile."
-    )
-    parser.add_argument(
-        "dir",
-        type=str,
-        nargs=1,
-        default="packages",
-        help="Input directory containing a tree of package definitions",
-    )
-    parser.add_argument(
-        "output",
-        type=str,
-        nargs=1,
-        default="dist",
-        help="Output directory in which to put all built packages",
-    )
-    parser.add_argument(
-        "--cflags",
-        type=str,
-        nargs="?",
-        default=None,
-        help="Extra compiling flags. Default: SIDE_MODULE_CFLAGS",
-    )
-    parser.add_argument(
-        "--cxxflags",
-        type=str,
-        nargs="?",
-        default=None,
-        help=("Extra C++ specific compiling flags. " "Default: SIDE_MODULE_CXXFLAGS"),
-    )
-    parser.add_argument(
-        "--ldflags",
-        type=str,
-        nargs="?",
-        default=None,
-        help="Extra linking flags. Default: SIDE_MODULE_LDFLAGS",
-    )
-    parser.add_argument(
-        "--target-install-dir",
-        type=str,
-        nargs="?",
-        default=None,
-        help="The path to the target Python installation. Default: TARGETINSTALLDIR",
-    )
-    parser.add_argument(
-        "--host-install-dir",
-        type=str,
-        nargs="?",
-        default=None,
-        help=("Directory for installing built host packages. Default: HOSTINSTALLDIR"),
-    )
-    parser.add_argument(
-        "--log-dir",
-        type=str,
-        dest="log_dir",
-        nargs="?",
-        default=None,
-        help=("Directory to place log files"),
-    )
-    parser.add_argument(
-        "--only",
-        type=str,
-        nargs="?",
-        default=None,
-        help=("Only build the specified packages, provided as a comma-separated list"),
-    )
-    parser.add_argument(
-        "--force-rebuild",
-        action="store_true",
-        help=(
-            "Force rebuild of all packages regardless of whether they appear to have been updated"
-        ),
-    )
-    parser.add_argument(
-        "--n-jobs",
-        type=int,
-        nargs="?",
-        default=4,
-        help="Number of packages to build in parallel",
-    )
-    return parser
+    package_data = generate_repodata(output_dir, pkg_map)
+    with repodata_path.open("w") as fd:
+        json.dump(package_data, fd)
+        fd.write("\n")
 
 
-def set_default_args(args: argparse.Namespace) -> argparse.Namespace:
-    args = copy.deepcopy(args)
+def set_default_build_args(build_args: BuildArgs) -> BuildArgs:
+    args = dataclasses.replace(build_args)
 
     if args.cflags is None:
-        args.cflags = common.get_make_flag("SIDE_MODULE_CFLAGS")
+        args.cflags = common.get_make_flag("SIDE_MODULE_CFLAGS")  # type: ignore[unreachable]
     if args.cxxflags is None:
-        args.cxxflags = common.get_make_flag("SIDE_MODULE_CXXFLAGS")
+        args.cxxflags = common.get_make_flag("SIDE_MODULE_CXXFLAGS")  # type: ignore[unreachable]
     if args.ldflags is None:
-        args.ldflags = common.get_make_flag("SIDE_MODULE_LDFLAGS")
+        args.ldflags = common.get_make_flag("SIDE_MODULE_LDFLAGS")  # type: ignore[unreachable]
     if args.target_install_dir is None:
-        args.target_install_dir = common.get_make_flag("TARGETINSTALLDIR")
+        args.target_install_dir = common.get_make_flag("TARGETINSTALLDIR")  # type: ignore[unreachable]
     if args.host_install_dir is None:
-        args.host_install_dir = common.get_make_flag("HOSTINSTALLDIR")
+        args.host_install_dir = common.get_make_flag("HOSTINSTALLDIR")  # type: ignore[unreachable]
+    if args.compression_level is None:
+        args.compression_level = int(common.get_make_flag("PYODIDE_ZIP_COMPRESSION_LEVEL"))  # type: ignore[unreachable]
 
     return args
-
-
-def main(args: argparse.Namespace) -> None:
-    packages_dir = Path(args.dir[0]).resolve()
-    outputdir = Path(args.output[0]).resolve()
-    args = set_default_args(args)
-    pkg_map = build_packages(packages_dir, args)
-    install_packages(pkg_map, outputdir)
-
-
-if __name__ == "__main__":
-    parser = make_parser(argparse.ArgumentParser())
-    args = parser.parse_args()
-    main(args)
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/buildpkg.py` & `pyodide-build-0.23.1/pyodide_build/buildpkg.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 Builds a Pyodide package.
 """
 
 import argparse
 import cgi
 import fnmatch
-import hashlib
 import json
 import os
 import shutil
 import subprocess
 import sys
 import sysconfig
 import textwrap
@@ -23,22 +22,25 @@
 from textwrap import dedent
 from types import TracebackType
 from typing import Any, TextIO, cast
 from urllib import request
 
 from . import common, pypabuild
 from .common import (
+    _get_sha256_checksum,
     chdir,
     exit_with_stdio,
     find_matching_wheels,
     find_missing_executables,
+    make_zip_archive,
     set_build_environment,
 )
 from .io import MetaConfig, _BuildSpec, _SourceSpec
 from .logger import logger
+from .pywasmcross import BuildArgs
 
 
 def _make_whlfile(
     *args: Any, owner: int | None = None, group: int | None = None, **kwargs: Any
 ) -> str:
     return shutil._make_zipfile(*args, **kwargs)  # type: ignore[attr-defined]
 
@@ -117,15 +119,18 @@
 @contextmanager
 def get_bash_runner() -> Iterator[BashRunnerWithSharedEnvironment]:
     PYODIDE_ROOT = os.environ["PYODIDE_ROOT"]
     env: dict[str, str] = {}
     set_build_environment(env)
 
     with BashRunnerWithSharedEnvironment(env=env) as b:
-        b.run(f"source {PYODIDE_ROOT}/pyodide_env.sh", stderr=subprocess.DEVNULL)
+        # Working in-tree, add emscripten toolchain into PATH and set ccache
+        if Path(PYODIDE_ROOT, "pyodide_env.sh").exists():
+            b.run(f"source {PYODIDE_ROOT}/pyodide_env.sh", stderr=subprocess.DEVNULL)
+
         yield b
 
 
 def check_checksum(archive: Path, source_metadata: _SourceSpec) -> None:
     """
     Checks that an archive matches the checksum in the package metadata.
 
@@ -136,24 +141,19 @@
         the path to the archive we wish to checksum
     source_metadata
         The source section from meta.yaml.
     """
     if source_metadata.sha256 is None:
         return
     checksum = source_metadata.sha256
-    CHUNK_SIZE = 1 << 16
-    h = hashlib.sha256()
-    with open(archive, "rb") as fd:
-        while True:
-            chunk = fd.read(CHUNK_SIZE)
-            h.update(chunk)
-            if len(chunk) < CHUNK_SIZE:
-                break
-    if h.hexdigest() != checksum:
-        raise ValueError(f"Invalid sha256 checksum: {h.hexdigest()}")
+    real_checksum = _get_sha256_checksum(archive)
+    if real_checksum != checksum:
+        raise ValueError(
+            f"Invalid sha256 checksum: {real_checksum} != {checksum} (expected)"
+        )
 
 
 def trim_archive_extension(tarballname: str) -> str:
     for extension in [
         ".tar.gz",
         ".tgz",
         ".tar",
@@ -413,24 +413,25 @@
         cxxflags=build_metadata.cxxflags,
         ldflags=build_metadata.ldflags,
         target_install_dir=target_install_dir,
         exports=build_metadata.exports,
     )
     backend_flags = build_metadata.backend_flags
 
-    with chdir(srcpath), build_env_ctx as build_env:
+    with build_env_ctx as build_env:
         if build_metadata.cross_script is not None:
             with BashRunnerWithSharedEnvironment(build_env) as runner:
-                runner.run(build_metadata.cross_script)
+                runner.run(build_metadata.cross_script, cwd=srcpath)
                 build_env = runner.env
 
         from .pypabuild import build
 
+        outpath = srcpath / "dist"
         try:
-            build(build_env, backend_flags)
+            build(srcpath, outpath, build_env, backend_flags)
         except BaseException:
             build_log_path = Path("build.log")
             if build_log_path.exists():
                 build_log_path.unlink()
             raise
 
 
@@ -689,38 +690,34 @@
     for source_file in source_files():
         source_file = Path(source_file)
         if source_file.stat().st_mtime > package_time:
             return True
     return False
 
 
-def build_package(
+def _build_package_inner(
     pkg_root: Path,
     pkg: MetaConfig,
+    build_args: BuildArgs,
     *,
-    target_install_dir: str,
-    host_install_dir: str,
-    force_rebuild: bool,
-    continue_: bool,
+    force_rebuild: bool = False,
+    continue_: bool = False,
 ) -> None:
     """
-    Build the package. The main entrypoint in this module.
+    Build the package.
 
     pkg_root
         The path to the root directory for the package. Generally
         $PYODIDE_ROOT/packages/<PACKAGES>
 
     pkg
         The package metadata parsed from the meta.yaml file in pkg_root
 
-    target_install_dir
-        The path to the target Python installation
-
-    host_install_dir
-        Directory for installing built host packages.
+    build_args
+        The extra build arguments passed to the build script.
     """
     source_metadata = pkg.source
     build_metadata = pkg.build
     name = pkg.package.name
     version = pkg.package.version
     build_dir = pkg_root / "build"
     dist_dir = pkg_root / "dist"
@@ -753,57 +750,185 @@
             f"directory at the path {srcpath}, but that path does not exist."
         )
 
     import os
     import subprocess
     import sys
 
-    tee = subprocess.Popen(["tee", pkg_root / "build.log"], stdin=subprocess.PIPE)
-    # Cause tee's stdin to get a copy of our stdin/stdout (as well as that
-    # of any child processes we spawn)
-    os.dup2(tee.stdin.fileno(), sys.stdout.fileno())  # type: ignore[union-attr]
-    os.dup2(tee.stdin.fileno(), sys.stderr.fileno())  # type: ignore[union-attr]
+    try:
+        stdout_fileno = sys.stdout.fileno()
+        stderr_fileno = sys.stderr.fileno()
+
+        tee = subprocess.Popen(["tee", pkg_root / "build.log"], stdin=subprocess.PIPE)
+
+        # Cause tee's stdin to get a copy of our stdin/stdout (as well as that
+        # of any child processes we spawn)
+        os.dup2(tee.stdin.fileno(), stdout_fileno)  # type: ignore[union-attr]
+        os.dup2(tee.stdin.fileno(), stderr_fileno)  # type: ignore[union-attr]
+    except OSError:
+        # This normally happens when testing
+        logger.warning("stdout/stderr does not have a fileno, not logging to file")
 
     with chdir(pkg_root), get_bash_runner() as bash_runner:
         bash_runner.env["PKGDIR"] = str(pkg_root)
         bash_runner.env["PKG_VERSION"] = version
         bash_runner.env["PKG_BUILD_DIR"] = str(srcpath)
+        bash_runner.env["DISTDIR"] = str(src_dist_dir)
         if not continue_:
             clear_only = package_type == "cpython_module"
             prepare_source(build_dir, srcpath, source_metadata, clear_only=clear_only)
             patch(pkg_root, srcpath, source_metadata)
 
+        src_dist_dir.mkdir(exist_ok=True, parents=True)
         run_script(build_dir, srcpath, build_metadata, bash_runner)
 
         if package_type == "static_library":
             # Nothing needs to be done for a static library
             pass
         elif package_type in ("shared_library", "cpython_module"):
             # If shared library, we copy .so files to dist_dir
             # and create a zip archive of the .so files
             shutil.rmtree(dist_dir, ignore_errors=True)
             dist_dir.mkdir(parents=True)
-            shutil.make_archive(str(dist_dir / src_dir_name), "zip", src_dist_dir)
+            make_zip_archive(dist_dir / f"{src_dir_name}.zip", src_dist_dir)
         else:  # wheel
             if not finished_wheel:
                 compile(
                     name,
                     srcpath,
                     build_metadata,
                     bash_runner,
-                    target_install_dir=target_install_dir,
+                    target_install_dir=build_args.target_install_dir,
                 )
 
-            package_wheel(name, srcpath, build_metadata, bash_runner, host_install_dir)
+            package_wheel(
+                name, srcpath, build_metadata, bash_runner, build_args.host_install_dir
+            )
             shutil.rmtree(dist_dir, ignore_errors=True)
             shutil.copytree(src_dist_dir, dist_dir)
 
         create_packaged_token(build_dir)
 
 
+def _load_package_config(package_dir: Path) -> tuple[Path, MetaConfig]:
+    """
+    Load the package configuration from the given directory.
+
+    Parameters
+    ----------
+    package_dir
+        The directory containing the package configuration, or the path to the
+        package configuration file.
+
+    Returns
+    -------
+    pkg_dir
+        The directory containing the package configuration.
+    pkg
+        The package configuration.
+    """
+    if not package_dir.exists():
+        raise FileNotFoundError(f"Package directory {package_dir} does not exist")
+
+    if package_dir.is_dir():
+        meta_file = package_dir / "meta.yaml"
+    else:
+        meta_file = package_dir
+        package_dir = meta_file.parent
+
+    return package_dir, MetaConfig.from_yaml(meta_file)
+
+
+def _check_exetuables(pkg: MetaConfig) -> None:
+    """
+    Check that the executables required to build the package are available.
+
+    Parameters
+    ----------
+    pkg : MetaConfig
+        The package configuration.
+
+    """
+    missing_executables = find_missing_executables(pkg.requirements.executable)
+    if missing_executables:
+        missing_string = ", ".join(missing_executables)
+        error_msg = (
+            "The following executables are required but missing in the host system: "
+            + missing_string
+        )
+        raise RuntimeError(error_msg)
+
+
+def build_package(
+    package: str | Path,
+    build_args: BuildArgs,
+    force_rebuild: bool = False,
+    continue_: bool = False,
+) -> None:
+    """
+    Build the package. The main entrypoint in this module.
+
+    Parameters
+    ----------
+    package
+        The path to the package configuration file or the directory containing
+        the package configuration file.
+
+    build_args
+        The extra build arguments passed to the build script.
+
+    force_rebuild
+        If True, the package will be rebuilt even if it is already up-to-date.
+
+    continue_
+        If True, continue a build from the middle. For debugging. Implies "--force-rebuild".
+    """
+
+    force_rebuild = force_rebuild or continue_
+
+    meta_file = Path(package).resolve()
+    pkg_root, pkg = _load_package_config(meta_file)
+
+    _check_exetuables(pkg)
+
+    pkg.build.cflags += f" {build_args.cflags}"
+    pkg.build.cxxflags += f" {build_args.cxxflags}"
+    pkg.build.ldflags += f" {build_args.ldflags}"
+
+    name = pkg.package.name
+    t0 = datetime.now()
+    timestamp = t0.strftime("%Y-%m-%d %H:%M:%S")
+    logger.info(f"[{timestamp}] Building package {name}...")
+    success = True
+    try:
+        _build_package_inner(
+            pkg_root,
+            pkg,
+            build_args,
+            force_rebuild=force_rebuild,
+            continue_=continue_,
+        )
+
+    except Exception:
+        success = False
+        raise
+    finally:
+        t1 = datetime.now()
+        datestamp = "[{}]".format(t1.strftime("%Y-%m-%d %H:%M:%S"))
+        total_seconds = f"{(t1 - t0).total_seconds():.1f}"
+        status = "Succeeded" if success else "Failed"
+        msg = (
+            f"{datestamp} {status} building package {name} in {total_seconds} seconds."
+        )
+        if success:
+            logger.success(msg)
+        else:
+            logger.error(msg)
+
+
 def make_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.description = (
         "Build a pyodide package.\n\n"
         "Note: this is a private endpoint that should not be used "
         "outside of the Pyodide Makefile."
     )
     parser.add_argument(
@@ -867,65 +992,22 @@
             ).strip()
         ),
     )
     return parser
 
 
 def main(args: argparse.Namespace) -> None:
-    continue_ = not not args.continue_
-    # --continue implies --force-rebuild
-    force_rebuild = args.force_rebuild or continue_
-
-    meta_file = Path(args.package[0]).resolve()
-
-    pkg_root = meta_file.parent
-    pkg = MetaConfig.from_yaml(meta_file)
-
-    pkg.build.cflags += f" {args.cflags}"
-    pkg.build.cxxflags += f" {args.cxxflags}"
-    pkg.build.ldflags += f" {args.ldflags}"
-
-    missing_executables = find_missing_executables(pkg.requirements.executable)
-    if missing_executables:
-        missing_string = ", ".join(missing_executables)
-        error_msg = (
-            "The following executables are required but missing in the host system: "
-            + missing_string
-        )
-        raise RuntimeError(error_msg)
-
-    name = pkg.package.name
-    t0 = datetime.now()
-    timestamp = t0.strftime("%Y-%m-%d %H:%M:%S")
-    logger.info(f"[{timestamp}] Building package {name}...")
-    success = True
-    try:
-        build_package(
-            pkg_root,
-            pkg,
-            target_install_dir=args.target_install_dir,
-            host_install_dir=args.host_install_dir,
-            force_rebuild=force_rebuild,
-            continue_=continue_,
-        )
-
-    except Exception:
-        success = False
-        raise
-    finally:
-        t1 = datetime.now()
-        datestamp = "[{}]".format(t1.strftime("%Y-%m-%d %H:%M:%S"))
-        total_seconds = f"{(t1 - t0).total_seconds():.1f}"
-        status = "Succeeded" if success else "Failed"
-        msg = (
-            f"{datestamp} {status} building package {name} in {total_seconds} seconds."
-        )
-        if success:
-            logger.success(msg)
-        else:
-            logger.error(msg)
+    build_args = BuildArgs(
+        pkgname="",
+        cflags=args.cflags,
+        cxxflags=args.cxxflags,
+        ldflags=args.ldflags,
+        target_install_dir=args.target_install_dir,
+        host_install_dir=args.host_install_dir,
+    )
+    build_package(args.package[0], build_args, args.force_rebuild, args.continue_)
 
 
 if __name__ == "__main__":
     parser = make_parser(argparse.ArgumentParser())
     args = parser.parse_args()
     main(args)
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/cli/build.py` & `pyodide-build-0.23.1/pyodide_build/cli/build.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,170 +1,225 @@
-import os
 import re
 import shutil
 import tempfile
 from pathlib import Path
 from typing import Optional
 from urllib.parse import urlparse
 
 import requests
 import typer
 
 from .. import common
 from ..out_of_tree import build
-from ..out_of_tree.pypi import build_dependencies_for_wheel, fetch_pypi_package
+from ..out_of_tree.pypi import (
+    build_dependencies_for_wheel,
+    build_wheels_from_pypi_requirements,
+    fetch_pypi_package,
+)
 from ..out_of_tree.utils import initialize_pyodide_root
 
 
 def pypi(
     package: str,
+    output_directory: Path,
     exports: str = typer.Option(
         "requested",
         help="Which symbols should be exported when linking .so files?",
     ),
     ctx: typer.Context = typer.Context,
 ) -> Path:
     """Fetch a wheel from pypi, or build from source if none available."""
     initialize_pyodide_root()
     common.check_emscripten_version()
     backend_flags = ctx.args
-    curdir = Path.cwd()
-    (curdir / "dist").mkdir(exist_ok=True)
-
     with tempfile.TemporaryDirectory() as tmpdir:
-        temppath = Path(tmpdir)
+        srcdir = Path(tmpdir)
 
         # get package from pypi
-        package_path = fetch_pypi_package(package, temppath)
+        package_path = fetch_pypi_package(package, srcdir)
         if not package_path.is_dir():
             # a pure-python wheel has been downloaded - just copy to dist folder
-            dest_file = curdir / "dist" / package_path.name
-            shutil.copyfile(str(package_path), curdir / "dist" / package_path.name)
+            dest_file = output_directory / package_path.name
+            shutil.copyfile(str(package_path), output_directory / package_path.name)
             print(f"Successfully fetched: {package_path.name}")
             return dest_file
 
-        # sdist - needs building
-        os.chdir(tmpdir)
-        built_wheel = build.run(exports, backend_flags, outdir=curdir / "dist")
-        os.chdir(curdir)
+        built_wheel = build.run(srcdir, output_directory, exports, backend_flags)
         return built_wheel
 
 
+def download_url(url: str, output_directory: Path) -> str:
+    with requests.get(url, stream=True) as response:
+        urlpath = Path(urlparse(response.url).path)
+        if urlpath.suffix == ".gz":
+            urlpath = urlpath.with_suffix("")
+        file_name = urlpath.name
+        with open(output_directory / file_name, "wb") as f:
+            for chunk in response.iter_content(chunk_size=1 << 20):
+                f.write(chunk)
+        return file_name
+
+
 def url(
     package_url: str,
+    output_directory: Path,
     exports: str = typer.Option(
         "requested",
         help="Which symbols should be exported when linking .so files?",
     ),
     ctx: typer.Context = typer.Context,
 ) -> Path:
     """Fetch a wheel or build sdist from url."""
     initialize_pyodide_root()
     common.check_emscripten_version()
     backend_flags = ctx.args
-    curdir = Path.cwd()
-    (curdir / "dist").mkdir(exist_ok=True)
-    with requests.get(package_url, stream=True) as response:
-        parsed_url = urlparse(response.url)
-        filename = os.path.basename(parsed_url.path)
-        name_base, ext = os.path.splitext(filename)
-        if ext == ".gz" and name_base.rfind(".") != -1:
-            ext = name_base[name_base.rfind(".") :] + ext
-        if ext.lower() == ".whl":
-            # just copy wheel into dist and return
-            out_path = Path(f"dist/{filename}").resolve()
-            with open(out_path, "b") as f:
-                for chunk in response.iter_content(chunk_size=1048576):
-                    f.write(chunk)
-            return out_path
-        else:
-            tf = tempfile.NamedTemporaryFile(suffix=ext, delete=False)
-            for chunk in response.iter_content(chunk_size=1048576):
-                tf.write(chunk)
-            tf.close()
-            with tempfile.TemporaryDirectory() as tmpdir:
-                temppath = Path(tmpdir)
-                shutil.unpack_archive(tf.name, tmpdir)
-                folder_list = list(temppath.iterdir())
-                if len(folder_list) == 1 and folder_list[0].is_dir():
-                    # unzipped into subfolder
-                    os.chdir(folder_list[0])
-                else:
-                    # unzipped here
-                    os.chdir(temppath)
-                wheel_path = build.run(exports, backend_flags, outdir=curdir / "dist")
-            os.unlink(tf.name)
-            return wheel_path
+    with tempfile.TemporaryDirectory() as tmpdir:
+        tmppath = Path(tmpdir)
+        filename = download_url(package_url, tmppath)
+        if Path(filename).suffix == ".whl":
+            shutil.move(tmppath / filename, output_directory / filename)
+            return output_directory / filename
+
+        builddir = tmppath / "build"
+        shutil.unpack_archive(tmppath / filename, builddir)
+        files = list(builddir.iterdir())
+        if len(files) == 1 and files[0].is_dir():
+            # unzipped into subfolder
+            builddir = files[0]
+        wheel_path = build.run(builddir, output_directory, exports, backend_flags)
+        return wheel_path
 
 
 def source(
-    source_location: str,
+    source_location: Path,
+    output_directory: Path,
     exports: str = typer.Option(
         "requested",
         help="Which symbols should be exported when linking .so files?",
     ),
     ctx: typer.Context = typer.Context,
 ) -> Path:
     """Use pypa/build to build a Python package from source"""
     initialize_pyodide_root()
-    orig_dir = Path.cwd()
-    if source_location != ".":
-        # build in this folder
-        os.chdir(source_location)
     common.check_emscripten_version()
     backend_flags = ctx.args
-    built_wheel = build.run(exports, backend_flags, outdir=orig_dir / "dist")
-    os.chdir(orig_dir)
+    built_wheel = build.run(source_location, output_directory, exports, backend_flags)
     return built_wheel
 
 
 # simple 'pyodide build' command
 def main(
     source_location: "Optional[str]" = typer.Argument(
         "",
         help="Build source, can be source folder, pypi version specification, or url to a source dist archive or wheel file. If this is blank, it will build the current directory.",
     ),
+    output_directory: str = typer.Option(
+        "./dist",
+        help="which directory should the output be placed into?",
+    ),
+    requirements_txt: str = typer.Option(
+        "",
+        "--requirements",
+        "-r",
+        help="Build a list of package requirements from a requirements.txt file",
+    ),
     exports: str = typer.Option(
         "requested",
         help="Which symbols should be exported when linking .so files?",
     ),
     build_dependencies: bool = typer.Option(
         False, help="Fetch non-pyodide dependencies from pypi and build them too."
     ),
+    output_lockfile: str = typer.Option(
+        "",
+        help="Output list of resolved dependencies to a file in requirements.txt format",
+    ),
     skip_dependency: list[str] = typer.Option(
         [],
         help="Skip building or resolving a single dependency. Use multiple times or provide a comma separated list to skip multiple dependencies.",
     ),
+    compression_level: int = typer.Option(
+        6, help="Compression level to use for the created zip file"
+    ),
     ctx: typer.Context = typer.Context,
 ) -> None:
     """Use pypa/build to build a Python package from source, pypi or url."""
+    outpath = Path(output_directory).resolve()
+    outpath.mkdir(exist_ok=True)
     extras: list[str] = []
+
+    if len(requirements_txt) > 0:
+        # a requirements.txt - build it (and optionally deps)
+        if not Path(requirements_txt).exists():
+            raise RuntimeError(
+                f"Couldn't find requirements text file {requirements_txt}"
+            )
+        reqs = []
+        with open(requirements_txt) as f:
+            raw_reqs = [x.strip() for x in f.readlines()]
+        for x in raw_reqs:
+            # remove comments
+            comment_pos = x.find("#")
+            if comment_pos != -1:
+                x = x[:comment_pos].strip()
+            if len(x) > 0:
+                if x[0] == "-":
+                    raise RuntimeError(
+                        f"pyodide build only supports name-based PEP508 requirements. [{x}] will not work."
+                    )
+                if x.find("@") != -1:
+                    raise RuntimeError(
+                        f"pyodide build does not support URL based requirements. [{x}] will not work"
+                    )
+                reqs.append(x)
+        try:
+            build_wheels_from_pypi_requirements(
+                reqs,
+                outpath,
+                build_dependencies,
+                skip_dependency,
+                exports,
+                ctx.args,
+                output_lockfile=output_lockfile,
+            )
+        except BaseException as e:
+            import traceback
+
+            print("Failed building multiple wheels:", traceback.format_exc())
+            raise e
+        return
+
     if source_location is not None:
         extras = re.findall(r"\[(\w+)\]", source_location)
         if len(extras) != 0:
             source_location = source_location[0 : source_location.find("[")]
-
     if not source_location:
         # build the current folder
-        wheel = source(".", exports, ctx)
+        wheel = source(Path.cwd(), outpath, exports, ctx)
     elif source_location.find("://") != -1:
-        wheel = url(source_location, exports, ctx)
+        wheel = url(source_location, outpath, exports, ctx)
     elif Path(source_location).is_dir():
         # a folder, build it
-        wheel = source(source_location, exports, ctx)
+        wheel = source(Path(source_location).resolve(), outpath, exports, ctx)
     elif source_location.find("/") == -1:
         # try fetch or build from pypi
-        wheel = pypi(source_location, exports, ctx)
+        wheel = pypi(source_location, outpath, exports, ctx)
     else:
         raise RuntimeError(f"Couldn't determine source type for {source_location}")
     # now build deps for wheel
     if build_dependencies:
         try:
             build_dependencies_for_wheel(
-                wheel, extras, skip_dependency, exports, ctx.args
+                wheel,
+                extras,
+                skip_dependency,
+                exports,
+                ctx.args,
+                output_lockfile=output_lockfile,
+                compression_level=compression_level,
             )
         except BaseException as e:
             import traceback
 
             print("Failed building dependencies for wheel:", traceback.format_exc())
             wheel.unlink()
             raise e
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/cli/config.py` & `pyodide-build-0.23.1/pyodide_build/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.0a1/pyodide_build/cli/create_zipfile.py` & `pyodide-build-0.23.1/pyodide_build/cli/create_zipfile.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,25 +2,35 @@
 
 import typer
 
 from ..pyzip import create_zipfile
 
 
 def main(
-    libdir: Path = typer.Argument(
-        ..., help="Path to the directory containing the Python standard library."
+    libdir: list[Path] = typer.Argument(
+        ...,
+        help="List of paths to the directory containing the Python standard library or extra packages.",
     ),
     pycompile: bool = typer.Option(
         False, help="Whether to compile the .py files into .pyc."
     ),
     output: Path = typer.Option(
         "python.zip", help="Path to the output zip file. Defaults to python.zip."
     ),
+    compression_level: int = typer.Option(
+        6, help="Compression level to use for the created zip file"
+    ),
 ) -> None:
     """
     Bundle Python standard libraries into a zip file.
     """
-    create_zipfile(libdir, output, pycompile=pycompile, filterfunc=None)
+    create_zipfile(
+        libdir,
+        output,
+        pycompile=pycompile,
+        filterfunc=None,
+        compression_level=compression_level,
+    )
     typer.echo(f"Zip file created at {output.resolve()}")
 
 
 main.typer_kwargs = {"hidden": True}  # type: ignore[attr-defined]
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/cli/skeleton.py` & `pyodide-build-0.23.1/pyodide_build/cli/skeleton.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Create or update a package recipe skeleton,
 # inspired from `conda skeleton` command.
 
+import sys
 from pathlib import Path
 
 import typer
 
 from .. import common, mkpkg
+from ..logger import logger
 
 app = typer.Typer()
 
 
 @app.callback(no_args_is_help=True)  # type: ignore[misc]
 def callback() -> None:
     """Add a new package build recipe or update an existing recipe"""
@@ -35,32 +37,51 @@
         help="The version of the package, if not specified, latest version will be used.",
     ),
     source_format: str = typer.Option(
         None,
         help="Which source format is preferred. Options are wheel or sdist. "
         "If not specified, then either a wheel or an sdist will be used. ",
     ),
-    root: str = typer.Option(
-        None, help="The root directory of the Pyodide.", envvar="PYODIDE_ROOT"
-    ),
     recipe_dir: str = typer.Option(
         None,
         help="The directory containing the recipe of packages."
-        "If not specified, the default is `packages` in the root directory.",
+        "If not specified, the default is `<cwd>/packages`.",
     ),
 ) -> None:
     """
     Create a new package from PyPI.
     """
-    pyodide_root = common.search_pyodide_root(Path.cwd()) if not root else Path(root)
-    recipe_dir_ = pyodide_root / "packages" if not recipe_dir else Path(recipe_dir)
+
+    if recipe_dir:
+        recipe_dir_ = Path(recipe_dir)
+    else:
+        cwd = Path.cwd()
+
+        try:
+            root = common.search_pyodide_root(cwd)
+        except FileNotFoundError:
+            root = cwd
+
+        if common.in_xbuildenv():
+            root = cwd
+
+        recipe_dir_ = root / "packages"
 
     if update or update_patched:
-        mkpkg.update_package(
-            recipe_dir_,
-            name,
-            version,
-            source_fmt=source_format,  # type: ignore[arg-type]
-            update_patched=update_patched,
-        )
+        try:
+            mkpkg.update_package(
+                recipe_dir_,
+                name,
+                version,
+                source_fmt=source_format,  # type: ignore[arg-type]
+                update_patched=update_patched,
+            )
+        except mkpkg.MkpkgFailedException as e:
+            logger.error(f"{name} update failed: {e}")
+            sys.exit(1)
+        except mkpkg.MkpkgSkipped as e:
+            logger.warn(f"{name} update skipped: {e}")
+        except Exception:
+            print(name)
+            raise
     else:
         mkpkg.make_package(recipe_dir_, name, version, source_fmt=source_format)  # type: ignore[arg-type]
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/common.py` & `pyodide-build-0.23.1/pyodide_build/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import contextlib
 import functools
+import hashlib
 import os
 import re
 import shutil
 import subprocess
 import sys
 import textwrap
 import zipfile
 from collections import deque
 from collections.abc import Generator, Iterable, Iterator, Mapping
 from contextlib import contextmanager
 from pathlib import Path
+from tempfile import TemporaryDirectory
 from typing import Any, NoReturn
 
 if sys.version_info < (3, 11, 0):
     import tomli as tomllib
 else:
     import tomllib
 
 from packaging.tags import Tag, compatible_tags, cpython_tags
 from packaging.utils import parse_wheel_filename
 
-from .io import MetaConfig
 from .logger import logger
+from .recipe import load_all_recipes
 
 BUILD_VARS: set[str] = {
     "PATH",
     "PYTHONPATH",
     "PYODIDE_ROOT",
     "PYTHONINCLUDE",
     "NUMPY_LIB",
@@ -48,14 +50,16 @@
     "STDLIB_MODULE_CFLAGS",
     "UNISOLATED_PACKAGES",
     "WASM_LIBRARY_DIR",
     "WASM_PKG_CONFIG_PATH",
     "CARGO_BUILD_TARGET",
     "CARGO_TARGET_WASM32_UNKNOWN_EMSCRIPTEN_LINKER",
     "RUSTFLAGS",
+    "PYO3_CROSS_LIB_DIR",
+    "PYO3_CROSS_INCLUDE_DIR",
     "PYODIDE_EMSCRIPTEN_VERSION",
     "PLATFORM_TRIPLET",
     "SYSCONFIGDATA_DIR",
     "RUST_TOOLCHAIN",
 }
 
 
@@ -129,15 +133,15 @@
     """
     wheel_paths = list(wheel_paths)
     wheel_tags_list: list[frozenset[Tag]] = []
     for wheel in wheel_paths:
         _, _, _, tags = parse_wheel_filename(wheel.name)
         wheel_tags_list.append(tags)
     for supported_tag in pyodide_tags():
-        for wheel_path, wheel_tags in zip(wheel_paths, wheel_tags_list):
+        for wheel_path, wheel_tags in zip(wheel_paths, wheel_tags_list, strict=True):
             if supported_tag in wheel_tags:
                 yield wheel_path
 
 
 def parse_top_level_import_name(whlfile: Path) -> list[str] | None:
     """
     Parse the top-level import names from a wheel file.
@@ -180,91 +184,14 @@
             f"WARNING: failed to parse top level import name from {whlfile}."
         )
         return None
 
     return top_level_imports
 
 
-ALWAYS_PACKAGES = {
-    "pyparsing",
-    "packaging",
-    "micropip",
-    "distutils",
-    "test",
-    "ssl",
-    "lzma",
-    "sqlite3",
-    "hashlib",
-}
-
-CORE_PACKAGES = {
-    "micropip",
-    "pyparsing",
-    "pytz",
-    "packaging",
-    "Jinja2",
-    "regex",
-    "fpcast-test",
-    "sharedlib-test-py",
-    "cpp-exceptions-test",
-    "pytest",
-    "tblib",
-}
-
-CORE_SCIPY_PACKAGES = {
-    "numpy",
-    "scipy",
-    "pandas",
-    "matplotlib",
-    "scikit-learn",
-    "joblib",
-    "pytest",
-}
-
-
-def _parse_package_subset(query: str | None) -> set[str]:
-    """Parse the list of packages specified with PYODIDE_PACKAGES env var.
-
-    Also add the list of mandatory packages: ["pyparsing", "packaging",
-    "micropip"]
-
-    Supports following meta-packages,
-     - 'core': corresponds to packages needed to run the core test suite
-       {"micropip", "pyparsing", "pytz", "packaging", "Jinja2", "fpcast-test"}. This is the default option
-       if query is None.
-     - 'min-scipy-stack': includes the "core" meta-package as well as some of the
-       core packages from the scientific python stack and their dependencies:
-       {"numpy", "scipy", "pandas", "matplotlib", "scikit-learn", "joblib", "pytest"}.
-       This option is non exhaustive and is mainly intended to make build faster
-       while testing a diverse set of scientific packages.
-     - '*': corresponds to all packages (returns None)
-
-    Note: None as input is equivalent to PYODIDE_PACKAGES being unset and leads
-    to only the core packages being built.
-
-    Returns:
-      a set of package names to build or None (build all packages).
-    """
-    if query is None:
-        query = "core"
-
-    packages = {el.strip() for el in query.split(",")}
-    packages.update(ALWAYS_PACKAGES)
-    # handle meta-packages
-    if "core" in packages:
-        packages |= CORE_PACKAGES
-        packages.discard("core")
-    if "min-scipy-stack" in packages:
-        packages |= CORE_PACKAGES | CORE_SCIPY_PACKAGES
-        packages.discard("min-scipy-stack")
-
-    packages.discard("")
-    return packages
-
-
 def get_make_flag(name: str) -> str:
     """Get flags from makefile.envs.
 
     For building packages we currently use:
         SIDE_MODULE_LDFLAGS
         SIDE_MODULE_CFLAGS
         SIDE_MODULE_CXXFLAGS
@@ -291,14 +218,19 @@
     PYODIDE_ROOT = get_pyodide_root()
     environment = {}
     result = subprocess.run(
         ["make", "-f", str(PYODIDE_ROOT / "Makefile.envs"), ".output_vars"],
         capture_output=True,
         text=True,
     )
+
+    if result.returncode != 0:
+        logger.error("ERROR: Failed to load environment variables from Makefile.envs")
+        exit_with_stdio(result)
+
     for line in result.stdout.splitlines():
         equalPos = line.find("=")
         if equalPos != -1:
             varname = line[0:equalPos]
 
             if varname not in BUILD_VARS:
                 continue
@@ -409,21 +341,19 @@
     PYODIDE_ROOT = get_pyodide_root()
     unisolated_file = PYODIDE_ROOT / "unisolated.txt"
     if unisolated_file.exists():
         # in xbuild env, read from file
         unisolated_packages = unisolated_file.read_text().splitlines()
     else:
         unisolated_packages = []
-        for pkg in (PYODIDE_ROOT / "packages").glob("*/meta.yaml"):
-            try:
-                config = MetaConfig.from_yaml(pkg)
-            except Exception as e:
-                raise ValueError(f"Could not parse {pkg}.") from e
+        recipe_dir = PYODIDE_ROOT / "packages"
+        recipes = load_all_recipes(recipe_dir)
+        for name, config in recipes.items():
             if config.build.cross_build_env:
-                unisolated_packages.append(config.package.name)
+                unisolated_packages.append(name)
     os.environ["UNISOLATED_PACKAGES"] = json.dumps(unisolated_packages)
     return unisolated_packages
 
 
 @contextlib.contextmanager
 def replace_env(build_env: Mapping[str, str]) -> Generator[None, None, None]:
     old_environ = dict(os.environ)
@@ -481,7 +411,86 @@
 
     tools_dir = Path(__file__).parent / "tools"
 
     env["CMAKE_TOOLCHAIN_FILE"] = str(
         tools_dir / "cmake/Modules/Platform/Emscripten.cmake"
     )
     env["PYO3_CONFIG_FILE"] = str(tools_dir / "pyo3_config.ini")
+
+
+def get_num_cores() -> int:
+    """
+    Return the number of CPUs the current process can use.
+    If the number of CPUs cannot be determined, return 1.
+    """
+    import loky
+
+    return loky.cpu_count()
+
+
+def make_zip_archive(
+    archive_path: Path,
+    input_dir: Path,
+    compression_level: int = 6,
+) -> None:
+    """Create a zip archive out of a input folder
+
+    Parameters
+    ----------
+    archive_path
+       Path to the zip file that will be created
+    input_dir
+       input dir to compress
+    compression_level
+       compression level of the resulting zip file.
+    """
+    if compression_level > 0:
+        compression = zipfile.ZIP_DEFLATED
+    else:
+        compression = zipfile.ZIP_STORED
+
+    with zipfile.ZipFile(
+        archive_path, "w", compression=compression, compresslevel=compression_level
+    ) as zf:
+        for file in input_dir.rglob("*"):
+            zf.write(file, file.relative_to(input_dir))
+
+
+def repack_zip_archive(archive_path: Path, compression_level: int = 6) -> None:
+    """Repack zip archive with a different compression level"""
+    if compression_level > 0:
+        compression = zipfile.ZIP_DEFLATED
+    else:
+        compression = zipfile.ZIP_STORED
+
+    with TemporaryDirectory() as temp_dir:
+        input_path = Path(temp_dir) / archive_path.name
+        shutil.move(archive_path, input_path)
+        with zipfile.ZipFile(input_path) as fh_zip_in, zipfile.ZipFile(
+            archive_path, "w", compression=compression, compresslevel=compression_level
+        ) as fh_zip_out:
+            for name in fh_zip_in.namelist():
+                fh_zip_out.writestr(name, fh_zip_in.read(name))
+
+
+def _get_sha256_checksum(archive: Path) -> str:
+    """Compute the sha256 checksum of a file
+
+    Parameters
+    ----------
+    archive
+        the path to the archive we wish to checksum
+
+    Returns
+    -------
+    checksum
+         sha256 checksum of the archive
+    """
+    CHUNK_SIZE = 1 << 16
+    h = hashlib.sha256()
+    with open(archive, "rb") as fd:
+        while True:
+            chunk = fd.read(CHUNK_SIZE)
+            h.update(chunk)
+            if len(chunk) < CHUNK_SIZE:
+                break
+    return h.hexdigest()
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/create_pypa_index.py` & `pyodide-build-0.23.1/pyodide_build/create_pypa_index.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.0a1/pyodide_build/create_xbuildenv.py` & `pyodide-build-0.23.1/pyodide_build/create_xbuildenv.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from .common import (
     exit_with_stdio,
     get_make_flag,
     get_pyodide_root,
     get_unisolated_packages,
 )
-from .io import MetaConfig
 from .logger import logger
+from .recipe import load_all_recipes
 
 
 def make_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.description = (
         "Create xbuild env.\n\n"
         "Note: this is a private endpoint that should not be used "
         "outside of the Pyodide Makefile."
@@ -27,17 +27,17 @@
     site_packages = Path(get_make_flag("HOSTSITEPACKAGES"))
     # Store package cross-build-files into site_packages_extras in the same tree
     # structure as they would appear in the real package.
     # In install_xbuildenv, we will use:
     # pip install -t $HOSTSITEPACKAGES -r requirements.txt
     # cp site-packages-extras $HOSTSITEPACKAGES
     site_packages_extras = xbuildenv_path / "site-packages-extras"
-    for pkg in (PYODIDE_ROOT / "packages").glob("**/meta.yaml"):
-        config = MetaConfig.from_yaml(pkg)
-        xbuild_files = config.build.cross_build_files
+    recipes = load_all_recipes(PYODIDE_ROOT / "packages")
+    for recipe in recipes.values():
+        xbuild_files = recipe.build.cross_build_files
         for path in xbuild_files:
             target = site_packages_extras / path
             target.parent.mkdir(parents=True, exist_ok=True)
             shutil.copy(site_packages / path, target)
 
 
 def get_relative_path(pyodide_root: Path, flag: str) -> Path:
@@ -53,16 +53,16 @@
     xbuildenv_path.mkdir(exist_ok=True)
     to_copy: list[Path] = [
         pythoninclude,
         sysconfig_dir,
         Path("Makefile.envs"),
         wasm_lib_dir / "cmake",
         Path("dist/repodata.json"),
-        Path("dist/pyodide_py.tar"),
         Path("dist/python"),
+        Path("dist/python_stdlib.zip"),
     ]
     to_copy.extend(
         x.relative_to(pyodide_root) for x in (pyodide_root / "dist").glob("pyodide.*")
     )
     # Some ad-hoc stuff here to moderate size. We'd like to include all of
     # wasm_lib_dir but there's 180mb of it. Better to leave out all the video
     # codecs and stuff.
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/io.py` & `pyodide-build-0.23.1/pyodide_build/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pydantic import BaseModel, Field
 
 
 class _PackageSpec(BaseModel):
     name: str
     version: str
     top_level: list[str] = Field([], alias="top-level")
-    tag: str = Field("", alias="_tag")
+    tag: list[str] = Field([])
     disabled: bool = Field(False, alias="_disabled")
 
     class Config:
         extra = pydantic.Extra.forbid
 
 
 class _SourceSpec(BaseModel):
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/logger.py` & `pyodide-build-0.23.1/pyodide_build/logger.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.0a1/pyodide_build/mkpkg.py` & `pyodide-build-0.23.1/pyodide_build/mkpkg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
 
-import argparse
 import contextlib
 import json
-import os
 import shutil
 import subprocess
 import tempfile
 import urllib.error
 import urllib.request
 import warnings
 from collections.abc import Iterator
@@ -44,14 +42,18 @@
     info: dict[str, Any]
     last_serial: int
     releases: dict[str, list[dict[str, Any]]]
     urls: list[URLDict]
     vulnerabilities: list[Any]
 
 
+class MkpkgSkipped(Exception):
+    pass
+
+
 class MkpkgFailedException(Exception):
     pass
 
 
 SDIST_EXTENSIONS = tuple(
     extension
     for (name, extensions, description) in shutil.get_unpack_formats()
@@ -213,30 +215,30 @@
 def update_package(
     root: Path,
     package: str,
     version: str | None = None,
     update_patched: bool = True,
     source_fmt: Literal["wheel", "sdist"] | None = None,
 ) -> None:
-
     yaml = YAML()
 
     meta_path = root / package / "meta.yaml"
     if not meta_path.exists():
         logger.error(f"{meta_path} does not exist")
         exit(1)
 
     yaml_content = yaml.load(meta_path.read_bytes())
 
-    if "url" not in yaml_content["source"]:
-        raise MkpkgFailedException(f"Skipping: {package} is a local package!")
-
     build_info = yaml_content.get("build", {})
-    if build_info.get("library", False) or build_info.get("sharedlibrary", False):
-        raise MkpkgFailedException(f"Skipping: {package} is a library!")
+    ty = build_info.get("type", None)
+    if ty in ["static_library", "shared_library", "cpython_module"]:
+        raise MkpkgSkipped(f"{package} is a {ty.replace('_', ' ')}!")
+
+    if "url" not in yaml_content["source"]:
+        raise MkpkgSkipped(f"{package} is a local package!")
 
     if yaml_content["source"]["url"].endswith("whl"):
         old_fmt = "wheel"
     else:
         old_fmt = "sdist"
 
     pypi_metadata = _get_metadata(package, version)
@@ -281,90 +283,7 @@
     yaml_content["source"]["sha256"] = dist_metadata["digests"]["sha256"]
     yaml_content["package"]["version"] = pypi_metadata["info"]["version"]
 
     yaml.dump(yaml_content, meta_path)
     run_prettier(meta_path)
 
     logger.success(f"Updated {package} from {local_ver} to {pypi_ver}.")
-
-
-def make_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.description = """
-Make a new pyodide package. Creates a simple template that will work
-for most pure Python packages, but will have to be edited for more
-complex things.""".strip()
-    parser.add_argument("package", type=str, nargs=1, help="The package name on PyPI")
-    parser.add_argument("--update", action="store_true", help="Update existing package")
-    parser.add_argument(
-        "--update-if-not-patched",
-        action="store_true",
-        help="Update existing package if it has no patches",
-    )
-    parser.add_argument(
-        "--source-format",
-        help="Which source format is preferred. Options are wheel or sdist. "
-        "If none is provided, then either a wheel or an sdist will be used. "
-        "When updating a package, the type will be kept the same if possible.",
-    )
-    parser.add_argument(
-        "--version",
-        type=str,
-        default=None,
-        help="Package version string, "
-        "e.g. v1.2.1 (defaults to latest stable release)",
-    )
-    parser.add_argument(
-        "--recipe-dir",
-        type=str,
-        default="packages",
-        help="Directory to create the recipe in (defaults to PYODIDE_ROOT/packages)",
-    )
-    return parser
-
-
-def main(args: argparse.Namespace) -> None:
-    PYODIDE_ROOT = os.environ.get("PYODIDE_ROOT")
-    if PYODIDE_ROOT is None:
-        raise ValueError("PYODIDE_ROOT is not set")
-
-    if os.path.isabs(args.recipe_dir):
-        recipe_dir = Path(args.recipe_dir)
-    else:
-        recipe_dir = (Path(PYODIDE_ROOT) / args.recipe_dir).resolve()
-
-    try:
-        package = args.package[0]
-        if args.update:
-            update_package(
-                recipe_dir,
-                package,
-                args.version,
-                update_patched=True,
-                source_fmt=args.source_format,
-            )
-            return
-        if args.update_if_not_patched:
-            update_package(
-                recipe_dir,
-                package,
-                args.version,
-                update_patched=False,
-                source_fmt=args.source_format,
-            )
-            return
-        make_package(recipe_dir, package, args.version, source_fmt=args.source_format)
-    except MkpkgFailedException as e:
-        # This produces two types of error messages:
-        #
-        # When the request to get the pypi json fails, it produces a message like:
-        # "Failed to load metadata for libxslt from https://pypi.org/pypi/libxslt/json: HTTP Error 404: Not Found"
-        #
-        # If there is no sdist it prints an error message like:
-        # "No sdist URL found for package swiglpk (https://pypi.org/project/swiglpk/)"
-        logger.error(e.args[0])
-        exit(1)
-
-
-if __name__ == "__main__":
-    parser = make_parser(argparse.ArgumentParser())
-    args = parser.parse_args()
-    main(args)
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/out_of_tree/build.py` & `pyodide-build-0.23.1/pyodide_build/out_of_tree/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 from pathlib import Path
 from typing import Any
 
 from .. import common, pypabuild
 
 
-def run(exports: Any, args: list[str], outdir: Path | None = None) -> Path:
-    if outdir is None:
-        outdir = Path("./dist")
+def run(srcdir: Path, outdir: Path, exports: Any, args: list[str]) -> Path:
+    outdir = outdir.resolve()
     cflags = common.get_make_flag("SIDE_MODULE_CFLAGS")
     cflags += f" {os.environ.get('CFLAGS', '')}"
     cxxflags = common.get_make_flag("SIDE_MODULE_CXXFLAGS")
     cxxflags += f" {os.environ.get('CXXFLAGS', '')}"
     ldflags = common.get_make_flag("SIDE_MODULE_LDFLAGS")
     ldflags += f" {os.environ.get('LDFLAGS', '')}"
     env = os.environ.copy()
@@ -24,9 +23,9 @@
         cxxflags=cxxflags,
         ldflags=ldflags,
         target_install_dir="",
         exports=exports,
     )
 
     with build_env_ctx as env:
-        built_wheel = pypabuild.build(env, " ".join(args), outdir=str(outdir))
+        built_wheel = pypabuild.build(srcdir, outdir, env, " ".join(args))
     return Path(built_wheel)
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/out_of_tree/pypi.py` & `pyodide-build-0.23.1/pyodide_build/out_of_tree/pypi.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from packaging.version import Version
 from resolvelib import BaseReporter, Resolver
 from resolvelib.providers import AbstractProvider
 from unearth.evaluator import TargetPython
 from unearth.finder import PackageFinder
 
 from .. import common
-from ..common import chdir
+from ..common import repack_zip_archive
 from ..logger import logger
 from . import build
 
 _PYPI_INDEX = ["https://pypi.org/simple/"]
 _PYPI_TRUSTED_HOSTS = ["pypi.org"]
 
 
@@ -40,14 +40,17 @@
     """
     Context manager to redirect stdout or stderr. It does it with filenos and things rather than
     just changing sys.stdout, so that output of subprocesses is also redirected.
     """
     if stream is None:
         stream = sys.stdout
     try:
+        if not hasattr(stream, "fileno"):
+            yield
+            return
         stream_fd = stream.fileno()
     except io.UnsupportedOperation:
         # in case we're already capturing to something that isn't really a file
         # e.g. in pytest
         yield
         return
     if type(to) == str:
@@ -72,44 +75,46 @@
 @cache
 def _get_built_wheel_internal(url):
     parsed_url = urlparse(url)
     gz_name = Path(parsed_url.path).name
 
     cache_entry: dict[str, Any] = {}
     build_dir = tempfile.TemporaryDirectory()
+    build_path = Path(build_dir.name)
+
     cache_entry["build_dir"] = build_dir
-    with chdir(Path(build_dir.name)):
-        with tempfile.NamedTemporaryFile(suffix=".tar.gz", delete=False) as f:
-            data = requests.get(url).content
-            f.write(data)
-            f.close()
-            shutil.unpack_archive(f.name, build_dir.name)
-            os.unlink(f.name)
-            files = list(Path(build_dir.name).iterdir())
-            if len(files) == 1 and files[0].is_dir():
-                os.chdir(Path(build_dir.name, files[0]))
-            else:
-                os.chdir(build_dir.name)
-        logger.info(f"Building wheel for {gz_name}...")
-        with tempfile.NamedTemporaryFile(mode="w+") as f:
-            try:
-                with (
-                    stream_redirected(to=f, stream=sys.stdout),
-                    stream_redirected(to=f, stream=sys.stderr),
-                ):
-                    wheel_path = build.run(
-                        PyPIProvider.BUILD_EXPORTS,
-                        PyPIProvider.BUILD_FLAGS,
-                        outdir=Path(build_dir.name) / "dist",
-                    )
-            except BaseException as e:
-                logger.error(" Failed\n Error is:")
-                f.seek(0)
-                logger.stderr(f.read())
-                raise e
+    with tempfile.NamedTemporaryFile(suffix=".tar.gz", delete=False) as f:
+        data = requests.get(url).content
+        f.write(data)
+        f.close()
+        shutil.unpack_archive(f.name, build_path)
+        os.unlink(f.name)
+        files = list(build_path.iterdir())
+        if len(files) == 1 and files[0].is_dir():
+            source_path = build_path / files[0]
+        else:
+            source_path = build_path
+    logger.info(f"Building wheel for {gz_name}...")
+    with (
+        tempfile.NamedTemporaryFile(mode="w+") as logfile,
+        stream_redirected(to=logfile, stream=sys.stdout),
+        stream_redirected(to=logfile, stream=sys.stderr),
+    ):
+        try:
+            wheel_path = build.run(
+                source_path,
+                build_path / "dist",
+                PyPIProvider.BUILD_EXPORTS,
+                PyPIProvider.BUILD_FLAGS,
+            )
+        except BaseException as e:
+            logger.error(" Failed\n Error is:")
+            logfile.seek(0)
+            logger.stderr(logfile.read())
+            raise e
 
     logger.success("Success")
 
     cache_entry["path"] = wheel_path
     return cache_entry
 
 
@@ -187,23 +192,29 @@
     )
     matches = pf.find_all_packages(package_name)
     for i in matches:
         # TODO: ignore sourcedists if wheel for same version exists
         yield Candidate(i.name, i.version, url=i.link.url, extras=extras)
 
 
-def download_or_build_wheel(url: str, target_directory: Path) -> None:
+def download_or_build_wheel(
+    url: str, target_directory: Path, compression_level: int = 6
+) -> None:
     parsed_url = urlparse(url)
     if parsed_url.path.endswith("gz"):
         wheel_file = get_built_wheel(url)
         shutil.copy(wheel_file, target_directory)
+        wheel_path = target_directory / wheel_file.name
     elif parsed_url.path.endswith(".whl"):
-        with open(target_directory / Path(parsed_url.path).name, "wb") as f:
+        wheel_path = target_directory / Path(parsed_url.path).name
+        with open(wheel_path, "wb") as f:
             f.write(requests.get(url).content)
 
+    repack_zip_archive(wheel_path, compression_level=compression_level)
+
 
 def get_metadata_for_wheel(url):
     parsed_url = urlparse(url)
     if parsed_url.path.endswith("gz"):
         wheel_file = get_built_wheel(url)
         wheel_stream: BinaryIO = open(wheel_file, "rb")
     elif parsed_url.path.endswith(".whl"):
@@ -218,19 +229,21 @@
                 return p.parse(cast(BinaryIO, z.open(n)), headersonly=True)
 
     # If we didn't find the metadata, return an empty dict
     return EmailMessage()
 
 
 class PyPIProvider(APBase):
-
     BUILD_FLAGS: list[str] = []
     BUILD_SKIP: list[str] = []
     BUILD_EXPORTS: str = ""
 
+    def __init__(self, build_dependencies: bool):
+        self.build_dependencies = build_dependencies
+
     def identify(self, requirement_or_candidate):
         base = canonicalize_name(requirement_or_candidate.name)
         return base
 
     def get_extras_for(self, requirement_or_candidate):
         # Extras is a set, which is not hashable
         return tuple(sorted(requirement_or_candidate.extras))
@@ -270,17 +283,18 @@
     def is_satisfied_by(self, requirement, candidate):
         if canonicalize_name(requirement.name) != candidate.name:
             return False
         return candidate.version in requirement.specifier
 
     def get_dependencies(self, candidate):
         deps = []
-        for d in candidate.dependencies:
-            if d.name not in PyPIProvider.BUILD_SKIP:
-                deps.append(d)
+        if self.build_dependencies:
+            for d in candidate.dependencies:
+                if d.name not in PyPIProvider.BUILD_SKIP:
+                    deps.append(d)
         if candidate.extras:
             # add the base package as a dependency too, so we can avoid conflicts between same package
             # but with different extras
             req = self.get_base_requirement(candidate)
             deps.append(req)
         return deps
 
@@ -293,76 +307,148 @@
     else:
         # jupyterlite all.json format
         for k in json_data.keys():
             if "releases" in json_data[k]:
                 yield k
 
 
-def build_dependencies_for_wheel(
-    wheel: Path,
-    extras: list[str],
-    skip_dependency: list[str],
-    exports: str,
-    build_flags: list[str],
-) -> None:
-    """Extract dependencies from this wheel and build pypi dependencies
-    for each one in ./dist/
-
-    n.b. because dependency resolution may need to backtrack, this
-    is potentially quite slow in the case that one needs to build an
-    sdist in order to discover dependencies of a candidate sub-dependency.
-    """
-    metadata = None
+def _parse_skip_list(skip_dependency: list[str]) -> None:
     PyPIProvider.BUILD_SKIP = []
     for skip in skip_dependency:
         split_deps = skip.split(",")
         for dep in split_deps:
             if dep.endswith(".json"):
                 # a pyodide json file
                 # or a jupyterlite json file
                 # skip all packages in it
                 PyPIProvider.BUILD_SKIP.extend(_get_json_package_list(Path(dep)))
             else:
                 PyPIProvider.BUILD_SKIP.append(dep)
 
-    PyPIProvider.BUILD_EXPORTS = exports
-    PyPIProvider.BUILD_FLAGS = build_flags
-    with ZipFile(wheel) as z:
-        for n in z.namelist():
-            if n.endswith(".dist-info/METADATA"):
-                p = BytesParser()
-                metadata = p.parse(cast(BinaryIO, z.open(n)), headersonly=True)
-    if metadata is None:
-        raise RuntimeError(f"Can't find package metadata in {wheel}")
 
-    deps: list[str] = metadata.get_all("Requires-Dist", [])
+def _resolve_and_build(
+    deps: list[str],
+    target_folder: Path,
+    build_dependencies: bool,
+    extras: list[str],
+    output_lockfile: str | None,
+    compression_level: int = 6,
+) -> None:
     requirements = []
 
     target_env = {
-        "extra": ",".join(extras),
         "python_version": f'{common.get_make_flag("PYMAJOR")}.{common.get_make_flag("PYMINOR")}',
         "sys_platform": common.platform().split("_")[0],
+        "extra": ",".join(extras),
     }
 
     for d in deps:
         r = Requirement(d)
         if (r.name not in PyPIProvider.BUILD_SKIP) and (
             (not r.marker) or r.marker.evaluate(target_env)
         ):
             requirements.append(r)
 
     # Create the (reusable) resolver.
-    provider = PyPIProvider()
+    provider = PyPIProvider(build_dependencies=build_dependencies)
     reporter = BaseReporter()
     resolver: Resolver[Requirement, Candidate, str] = Resolver(provider, reporter)
 
     # Kick off the resolution process, and get the final result.
     result = resolver.resolve(requirements)
+    target_folder.mkdir(parents=True, exist_ok=True)
+    version_file = None
+    if output_lockfile is not None and len(output_lockfile) > 0:
+        version_file = open(output_lockfile, "w")
     for x in result.mapping.values():
-        download_or_build_wheel(x.url, wheel.parent)
+        download_or_build_wheel(x.url, target_folder)
+        if len(x.extras) > 0:
+            extratxt = "[" + ",".join(x.extras) + "]"
+        else:
+            extratxt = ""
+        if version_file:
+            version_file.write(f"{x.name}{extratxt}=={x.version}\n")
+    if version_file:
+        version_file.close()
+
+
+def build_wheels_from_pypi_requirements(
+    reqs: list[str],
+    target_folder: Path,
+    build_dependencies: bool,
+    skip_dependency: list[str],
+    exports: str,
+    build_flags: list[str],
+    output_lockfile: str | None,
+) -> None:
+    """
+    Given a list of package requirements, build or fetch them. If build_dependencies is true, then
+    package dependencies will be built or fetched also.
+    """
+    _parse_skip_list(skip_dependency)
+    PyPIProvider.BUILD_EXPORTS = exports
+    PyPIProvider.BUILD_FLAGS = build_flags
+    _resolve_and_build(
+        reqs,
+        target_folder,
+        build_dependencies,
+        extras=[],
+        output_lockfile=output_lockfile,
+    )
+
+
+def build_dependencies_for_wheel(
+    wheel: Path,
+    extras: list[str],
+    skip_dependency: list[str],
+    exports: str,
+    build_flags: list[str],
+    output_lockfile: str | None,
+    compression_level: int = 6,
+) -> None:
+    """Extract dependencies from this wheel and build pypi dependencies
+    for each one in ./dist/
+
+    n.b. because dependency resolution may need to backtrack, this
+    is potentially quite slow in the case that one needs to build an
+    sdist in order to discover dependencies of a candidate sub-dependency.
+    """
+    metadata = None
+    _parse_skip_list(skip_dependency)
+
+    PyPIProvider.BUILD_EXPORTS = exports
+    PyPIProvider.BUILD_FLAGS = build_flags
+    with ZipFile(wheel) as z:
+        for n in z.namelist():
+            if n.endswith(".dist-info/METADATA"):
+                p = BytesParser()
+                metadata = p.parse(cast(BinaryIO, z.open(n)), headersonly=True)
+    if metadata is None:
+        raise RuntimeError(f"Can't find package metadata in {wheel}")
+
+    deps: list[str] = metadata.get_all("Requires-Dist", [])
+    metadata.get("version")
+    _resolve_and_build(
+        deps,
+        wheel.parent,
+        build_dependencies=True,
+        extras=extras,
+        output_lockfile=output_lockfile,
+        compression_level=compression_level,
+    )
+    # add the current wheel to the package-versions.txt
+    if output_lockfile is not None and len(output_lockfile) > 0:
+        with open(output_lockfile, "a") as version_txt:
+            name = metadata.get("Name")
+            version = metadata.get("Version")
+            if extras:
+                extratxt = "[" + ",".join(extras) + "]"
+            else:
+                extratxt = ""
+            version_txt.write(f"{name}{extratxt}=={version}\n")
 
 
 def fetch_pypi_package(package_spec: str, destdir: Path) -> Path:
     pf = PackageFinder(
         index_urls=_PYPI_INDEX,
         trusted_hosts=_PYPI_TRUSTED_HOSTS,
         target_python=get_target_python(),
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/out_of_tree/utils.py` & `pyodide-build-0.23.1/pyodide_build/out_of_tree/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,14 @@
         install_xbuildenv(__version__, env)
 
 
 def initialize_pyodide_root(*, quiet: bool = False) -> None:
     if "PYODIDE_ROOT" in os.environ:
         return
     try:
-        os.environ["PYODIDE_ROOT"] = str(search_pyodide_root(__file__))
+        os.environ["PYODIDE_ROOT"] = str(search_pyodide_root(Path.cwd()))
         return
     except FileNotFoundError:
         pass
-    env = Path(".pyodide-xbuildenv")
+    env = Path(".pyodide-xbuildenv").resolve()
     os.environ["PYODIDE_ROOT"] = str(env / "xbuildenv/pyodide-root")
     ensure_env_installed(env, quiet=quiet)
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/out_of_tree/venv.py` & `pyodide-build-0.23.1/pyodide_build/out_of_tree/venv.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,19 +93,32 @@
         ],
         capture_output=True,
         encoding="utf8",
     )
     check_result(result, "ERROR: failed to invoke Pyodide")
     platform_data = result.stdout
     sysconfigdata_dir = Path(get_make_flag("TARGETINSTALLDIR")) / "sysconfigdata"
-
     return dedent(
-        f"""\
+        """\
         import os
         import sys
+        """
+        # when pip installs an executable it uses sys.executable to create the
+        # shebang for the installed executable. The shebang for pip points to
+        # python-host but we want the shebang of the executable that we install
+        # to point to Pyodide python. We monkeypatch distlib.scripts.get_executable
+        # to return the value with the host suffix removed.
+        """
+        from pip._vendor.distlib import scripts
+        def get_executable():
+            return sys.executable.removesuffix("-host")
+
+        scripts.get_executable = get_executable
+        """
+        f"""
         os_name, sys_platform, multiarch, host_platform = {platform_data}
         os.name = os_name
         orig_platform = sys.platform
         sys.platform = sys_platform
         sys.implementation._multiarch = multiarch
         os.environ["_PYTHON_HOST_PLATFORM"] = host_platform
         os.environ["_PYTHON_SYSCONFIGDATA_NAME"] = f'_sysconfigdata_{{sys.abiflags}}_{{sys.platform}}_{{sys.implementation._multiarch}}'
@@ -121,14 +134,16 @@
 def create_pip_script(venv_bin):
     """Create pip and write it into the virtualenv bin folder."""
     # pip needs to run in the host Python not in Pyodide, so we'll use the host
     # Python in the shebang. Use whichever Python was used to invoke
     # pyodide venv.
     host_python_path = venv_bin / f"python{get_pyversion()}-host"
     host_python_path.symlink_to(sys.executable)
+    # in case someone needs a Python-version-agnostic way to refer to python-host
+    (venv_bin / "python-host").symlink_to(sys.executable)
 
     (venv_bin / "pip").write_text(
         # Other than the shebang and the monkey patch, this is exactly what
         # normal pip looks like.
         f"#!{host_python_path} -s\n"
         + get_pip_monkeypatch(venv_bin)
         + dedent(
@@ -191,20 +206,20 @@
     to_load = ["micropip"]
     result = subprocess.run(
         [
             venv_bin / "python",
             "-c",
             dedent(
                 f"""
-                from _pyodide._importhook import UNVENDORED_STDLIBS_AND_TEST;
-                from pyodide_js import loadPackage;
+                from pyodide_js import loadPackage
                 from pyodide_js._api import repodata_packages
+                from pyodide_js._api import repodata_unvendored_stdlibs_and_test
                 shared_libs = [pkgname for (pkgname,pkg) in repodata_packages.object_entries() if getattr(pkg, "shared_library", False)]
 
-                to_load = [*UNVENDORED_STDLIBS_AND_TEST, *shared_libs, *{to_load!r}]
+                to_load = [*repodata_unvendored_stdlibs_and_test, *shared_libs, *{to_load!r}]
                 loadPackage(to_load);
                 """
             ),
         ],
         capture_output=True,
         encoding="utf8",
     )
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/pypabuild.py` & `pyodide-build-0.23.1/pyodide_build/pypabuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,25 +70,24 @@
 
 def install_reqs(env: IsolatedEnv, reqs: set[str]) -> None:
     env.install(
         remove_avoided_requirements(
             reqs, get_unisolated_packages() + AVOIDED_REQUIREMENTS
         )
     )
-    # Some packages (numcodecs) don't declare cython as a build dependency and
-    # only recythonize if it is present. We need them to always recythonize so
-    # we always install cython. If the reqs included some cython version already
-    # then this won't do anything.
-    env.install(
-        [
-            "cython",
-            "pythran",
-            "setuptools<65.6.0",  # https://github.com/pypa/setuptools/issues/3693
-        ]
-    )
+
+    pinned_reqs = {
+        # Remove this when mypy releases a new version
+        # https://github.com/python/mypy/pull/14788
+        "types-setuptools": "types-setuptools<67.4.0.2"
+    }
+
+    for pkg, req in pinned_reqs.items():
+        if pkg in reqs:
+            env.install([req])
 
 
 def _build_in_isolated_env(
     build_env: Mapping[str, str],
     builder: ProjectBuilder,
     outdir: str,
     distribution: str,
@@ -151,33 +150,32 @@
     symlink_dir
         The directory where the symlinks will be created.
 
     Returns
     -------
     The dictionary of compiler environment variables that points to the symlinks.
     """
+
+    pywasmcross_exe = symlink_dir / "pywasmcross.py"
+    shutil.copy2(pywasmcross.__file__, pywasmcross_exe)
+    pywasmcross_exe.chmod(0o755)
+
     env = {}
     for symlink in pywasmcross.SYMLINKS:
         symlink_path = symlink_dir / symlink
         if os.path.lexists(symlink_path) and not symlink_path.exists():
             # remove broken symlink so it can be re-created
             symlink_path.unlink()
-        try:
-            pywasmcross_exe = shutil.which("_pywasmcross")
-            if pywasmcross_exe:
-                symlink_path.symlink_to(pywasmcross_exe)
-            else:
-                symlink_path.symlink_to(pywasmcross.__file__)
-        except FileExistsError:
-            pass
+
+        symlink_path.symlink_to(pywasmcross_exe)
         if symlink == "c++":
             var = "CXX"
         else:
             var = symlink.upper()
-        env[var] = symlink
+        env[var] = str(symlink_path)
 
     return env
 
 
 @contextmanager
 def get_build_env(
     env: dict[str, str],
@@ -228,26 +226,26 @@
         env["_PYTHON_HOST_PLATFORM"] = common.platform()
         env["_PYTHON_SYSCONFIGDATA_NAME"] = os.environ["SYSCONFIG_NAME"]
         env["PYTHONPATH"] = str(sysconfig_dir)
         yield env
 
 
 def build(
-    build_env: Mapping[str, str], backend_flags: str, outdir: str | None = None
+    srcdir: Path,
+    outdir: Path,
+    build_env: Mapping[str, str],
+    backend_flags: str,
 ) -> str:
-    srcdir = Path.cwd()
-    if outdir is None:
-        outdir = str(srcdir / "dist")
     builder = _ProjectBuilder(str(srcdir))
     distribution = "wheel"
     config_settings = parse_backend_flags(backend_flags)
     try:
         with _handle_build_error():
             built = _build_in_isolated_env(
-                build_env, builder, outdir, distribution, config_settings
+                build_env, builder, str(outdir), distribution, config_settings
             )
             print("{bold}{green}Successfully built {}{reset}".format(built, **_STYLES))
             return built
     except Exception as e:  # pragma: no cover
         tb = traceback.format_exc().strip("\n")
         print("\n{dim}{}{reset}\n".format(tb, **_STYLES))
         _error(str(e))
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/pywasmcross.py` & `pyodide-build-0.23.1/pyodide_build/pywasmcross.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,33 +47,37 @@
 
     sys.path = PYWASMCROSS_ARGS.pop("PYTHONPATH")
     os.environ["PATH"] = PYWASMCROSS_ARGS.pop("PATH")
     # restore __name__ so that relative imports work as we expect
     __name__ = PYWASMCROSS_ARGS.pop("orig__name__")
 
 
+import dataclasses
 import shutil
 import subprocess
-from collections import namedtuple
 from collections.abc import Iterable, Iterator
 from typing import Literal, NoReturn
 
-ReplayArgs = namedtuple(
-    "ReplayArgs",
-    [
-        "pkgname",
-        "cflags",
-        "cxxflags",
-        "ldflags",
-        "target_install_dir",
-        "builddir",
-        "pythoninclude",
-        "exports",
-    ],
-)
+
+@dataclasses.dataclass(eq=False, order=False, kw_only=True)
+class BuildArgs:
+    """
+    Common arguments for building a package.
+    """
+
+    pkgname: str = ""
+    cflags: str = ""
+    cxxflags: str = ""
+    ldflags: str = ""
+    target_install_dir: str = ""  # The path to the target Python installation
+    host_install_dir: str = ""  # Directory for installing built host packages.
+    builddir: str = ""  # The path to run pypa/build
+    pythoninclude: str = ""
+    exports: Literal["whole_archive", "requested", "pyinit"] | list[str] = "pyinit"
+    compression_level: int = 6
 
 
 def replay_f2c(args: list[str], dryrun: bool = False) -> list[str] | None:
     """Apply f2c to compilation arguments
 
     Parameters
     ----------
@@ -281,14 +285,16 @@
         # On Mac, we need to omit some darwin-specific arguments
         "-bundle", "-undefined", "dynamic_lookup",
         # This flag is needed to build numpy with SIMD optimization which we currently disable
         "-mpopcnt",
         # gcc flag that clang does not support
         "-Bsymbolic-functions",
         '-fno-second-underscore',
+        '-fstack-protector',  # doesn't work?
+        '-fno-strict-overflow',  # warning: argument unused during compilation
     ]:
         return None
     # fmt: on
     return arg
 
 
 def get_cmake_compiler_flags() -> list[str]:
@@ -406,22 +412,35 @@
     if result.returncode:
         print(f"Command '{' '.join(args)}' failed. Output to stderr was:")
         print(result.stderr)
         sys.exit(result.returncode)
     return result.stdout.splitlines()
 
 
+def filter_objects(line: list[str]) -> list[str]:
+    """
+    Collect up all the object files and archive files being linked.
+    """
+    return [
+        arg
+        for arg in line
+        if arg.endswith((".a", ".o"))
+        or arg.startswith(
+            "@"
+        )  # response file (https://gcc.gnu.org/wiki/Response_Files)
+    ]
+
+
 def calculate_exports(line: list[str], export_all: bool) -> Iterable[str]:
     """
-    Collect up all the object files and archive files being linked and list out
-    symbols in them that are marked as public. If ``export_all`` is ``True``,
-    then return all public symbols. If not, return only the public symbols that
-    begin with `PyInit`.
+    List out symbols from object files and archive files that are marked as public.
+    If ``export_all`` is ``True``, then return all public symbols.
+    If not, return only the public symbols that begin with `PyInit`.
     """
-    objects = [arg for arg in line if arg.endswith((".a", ".o"))]
+    objects = filter_objects(line)
     exports = None
     # Using emnm is simpler but it cannot handle bitcode. If we're only
     # exporting the PyInit symbols, save effort by using nm.
     if export_all:
         exports = calculate_object_exports_readobj(objects)
     if exports is None:
         # Either export_all is false or we are linking at least one bitcode
@@ -449,29 +468,29 @@
     else:
         export_list = exports
     prefixed_exports = ["_" + x for x in export_list]
     yield f"-sEXPORTED_FUNCTIONS={prefixed_exports!r}"
 
 
 def handle_command_generate_args(
-    line: list[str], args: ReplayArgs, is_link_command: bool
+    line: list[str], build_args: BuildArgs, is_link_command: bool
 ) -> list[str]:
     """
     A helper command for `handle_command` that generates the new arguments for
     the compilation.
 
     Unlike `handle_command` this avoids I/O: it doesn't sys.exit, it doesn't run
     subprocesses, it doesn't create any files, and it doesn't write to stdout.
 
     Parameters
     ----------
     line The original compilation command as a list e.g., ["gcc", "-c",
         "input.c", "-o", "output.c"]
 
-    args The arguments that pywasmcross was invoked with
+    build_args The arguments that pywasmcross was invoked with
 
     is_link_command Is this a linker invocation?
 
     Returns
     -------
         An updated argument list suitable for use with emscripten.
 
@@ -539,23 +558,25 @@
             "-Werror=implicit-function-declaration",
             "-Werror=mismatched-parameter-types",
             "-Werror=return-type",
         ]
     )
 
     if is_link_command:
-        new_args.extend(args.ldflags.split())
-        new_args.extend(get_export_flags(line, args.exports))
+        new_args.extend(build_args.ldflags.split())
+        new_args.extend(get_export_flags(line, build_args.exports))
 
     if "-c" in line:
         if new_args[0] == "emcc":
-            new_args.extend(args.cflags.split())
+            new_args.extend(build_args.cflags.split())
         elif new_args[0] == "em++":
-            new_args.extend(args.cflags.split() + args.cxxflags.split())
-        new_args.extend(["-I", args.pythoninclude])
+            new_args.extend(build_args.cflags.split() + build_args.cxxflags.split())
+
+        if build_args.pythoninclude:
+            new_args.extend(["-I", build_args.pythoninclude])
 
     optflags_valid = [f"-O{tok}" for tok in "01234sz"]
     optflag = None
     # Identify the optflag (e.g. -O3) in cflags/cxxflags/ldflags. Last one has
     # priority.
     for arg in reversed(new_args):
         if arg in optflags_valid:
@@ -583,66 +604,65 @@
             # Ignore it.
             del new_args[-1]
             continue
 
         if arg.startswith("-l"):
             result = replay_genargs_handle_dashl(arg, used_libs)
         elif arg.startswith("-I"):
-            result = replay_genargs_handle_dashI(arg, args.target_install_dir)
+            result = replay_genargs_handle_dashI(arg, build_args.target_install_dir)
         elif arg.startswith("-Wl"):
             result = replay_genargs_handle_linker_opts(arg)
         else:
             result = replay_genargs_handle_argument(arg)
 
         if result:
             new_args.append(result)
 
     return new_args
 
 
 def handle_command(
     line: list[str],
-    args: ReplayArgs,
+    build_args: BuildArgs,
 ) -> NoReturn:
     """Handle a compilation command. Exit with an appropriate exit code when done.
 
     Parameters
     ----------
     line : iterable
        an iterable with the compilation arguments
-    args : {object, namedtuple}
-       an container with additional compilation options, in particular
-       containing ``args.cflags``, ``args.cxxflags``, and ``args.ldflags``
+    build_args : BuildArgs
+       a container with additional compilation options
     """
     # some libraries have different names on wasm e.g. png16 = png
     is_link_cmd = get_library_output(line) is not None
 
     if line[0] == "gfortran":
         if "-dumpversion" in line:
             sys.exit(subprocess.run(line).returncode)
         tmp = replay_f2c(line)
         if tmp is None:
             sys.exit(0)
         line = tmp
 
-    new_args = handle_command_generate_args(line, args, is_link_cmd)
+    new_args = handle_command_generate_args(line, build_args, is_link_cmd)
 
-    if args.pkgname == "scipy":
+    if build_args.pkgname == "scipy":
         from pyodide_build._f2c_fixes import scipy_fixes
 
         scipy_fixes(new_args)
 
     returncode = subprocess.run(new_args).returncode
 
     sys.exit(returncode)
 
 
 def compiler_main():
-    replay_args = ReplayArgs(**PYWASMCROSS_ARGS)
+    build_args = BuildArgs(**PYWASMCROSS_ARGS)
     basename = Path(sys.argv[0]).name
     args = list(sys.argv)
     args[0] = basename
-    sys.exit(handle_command(args, replay_args))
+    sys.exit(handle_command(args, build_args))
 
 
 if IS_COMPILER_INVOCATION:
     compiler_main()
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/serve.py` & `pyodide-build-0.23.1/pyodide_build/serve.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 class Handler(http.server.SimpleHTTPRequestHandler):
     def end_headers(self) -> None:
         self.send_header("Access-Control-Allow-Origin", "*")
         super().end_headers()
 
 
-Handler.extensions_map[".wasm"] = "application/wasm"
-
-
 def make_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.description = "Start a server with the supplied dist-dir and port."
     parser.add_argument(
         "--dist-dir",
         action="store",
         type=str,
         default="dist",
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake` & `pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -52,22 +52,18 @@
 # This is a hack which overrides find_library() to tell CMake to look at PIC dirs first.
 if ($ENV{CFLAGS} MATCHES "MEMORY64")
   set(CMAKE_LIBRARY_ARCHITECTURE "wasm64-emscripten/pic")
 else()
   set(CMAKE_LIBRARY_ARCHITECTURE "wasm32-emscripten/pic")
 endif()
 
-
-# Disable the usage of response file so objects are exposed to the commandline.
-# Our export calculation logic in pywasmcross needs to read object files.
-# TODO: support export calculation from the response file
 set(CMAKE_C_USE_RESPONSE_FILE_FOR_LIBRARIES 0)
 set(CMAKE_CXX_USE_RESPONSE_FILE_FOR_LIBRARIES 0)
-set(CMAKE_C_USE_RESPONSE_FILE_FOR_OBJECTS 0)
-set(CMAKE_CXX_USE_RESPONSE_FILE_FOR_OBJECTS 0)
+set(CMAKE_C_USE_RESPONSE_FILE_FOR_OBJECTS 1)
+set(CMAKE_CXX_USE_RESPONSE_FILE_FOR_OBJECTS 1)
 set(CMAKE_C_USE_RESPONSE_FILE_FOR_INCLUDES 1)
 set(CMAKE_CXX_USE_RESPONSE_FILE_FOR_INCLUDES 1)
 
 # Allow some of the variables to be overridden by the user by env variable
 # CMAKE_PROJECT_INCLUDE is a nice way to override some properties of the project
 # It can be set by passing -DCMAKE_PROJECT_INCLUDE=... to cmake
 # But some python packages will not allow users to pass extra arguments to cmake
```

### Comparing `pyodide-build-0.23.0a1/pyodide_build.egg-info/SOURCES.txt` & `pyodide-build-0.23.1/pyodide_build.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ./pyodide_build/__init__.py
 ./pyodide_build/__main__.py
 ./pyodide_build/_f2c_fixes.py
@@ -14,23 +16,25 @@
 ./pyodide_build/install_xbuildenv.py
 ./pyodide_build/io.py
 ./pyodide_build/logger.py
 ./pyodide_build/mkpkg.py
 ./pyodide_build/pypabuild.py
 ./pyodide_build/pywasmcross.py
 ./pyodide_build/pyzip.py
+./pyodide_build/recipe.py
 ./pyodide_build/serve.py
 ./pyodide_build/cli/__init__.py
 ./pyodide_build/cli/build.py
 ./pyodide_build/cli/build_recipes.py
 ./pyodide_build/cli/config.py
 ./pyodide_build/cli/create_zipfile.py
 ./pyodide_build/cli/py_compile.py
 ./pyodide_build/cli/skeleton.py
 ./pyodide_build/cli/venv.py
+./pyodide_build/cli/xbuildenv.py
 ./pyodide_build/out_of_tree/__init__.py
 ./pyodide_build/out_of_tree/build.py
 ./pyodide_build/out_of_tree/pypi.py
 ./pyodide_build/out_of_tree/utils.py
 ./pyodide_build/out_of_tree/venv.py
 ./pyodide_build/tools/pyo3_config.ini
 ./pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
```

### Comparing `pyodide-build-0.23.0a1/setup.cfg` & `pyodide-build-0.23.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 project_urls = 
 	Bug Tracker = https://github.com/pyodide/pyodide/issues
 	Documentation = https://pyodide.org/en/stable/
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 	Operating System :: OS Independent
+license = MPL-2.0
+license_files = 
+	LICENSE
 
 [options]
 package_dir = 
 	= .
 packages = find_namespace:
 python_requires = >=3.10
 install_requires = 
@@ -34,32 +37,36 @@
 	unearth~=0.6
 	requests
 	types-requests
 	typer
 	auditwheel-emscripten~=0.0.9
 	resolvelib
 	rich
+	loky
 
 [options.entry_points]
 console_scripts = 
 	pyodide-build = pyodide_build.__main__:main
-	_pywasmcross = pyodide_build.pywasmcross:compiler_main
 pyodide.cli = 
 	build = pyodide_build.cli.build:main
 	build-recipes = pyodide_build.cli.build_recipes:recipe
 	venv = pyodide_build.cli.venv:main
 	skeleton = pyodide_build.cli.skeleton:app
 	py-compile = pyodide_build.cli.py_compile:main
 	config = pyodide_build.cli.config:app
 	create-zipfile = pyodide_build.cli.create_zipfile:main
+	xbuildenv = pyodide_build.cli.xbuildenv:app
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-pyodide==0.23.2
+deploy = 
+	boto3
+	moto
 
 [options.packages.find]
 where = .
 exclude = 
 	pyodide_build.tests
 
 [options.package_data]
```

