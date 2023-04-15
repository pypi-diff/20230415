# Comparing `tmp/pydtl_relativepath-0.0.1.tar.gz` & `tmp/pydtl_relativepath-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydtl_relativepath-0.0.1.tar", last modified: Sun Mar 12 18:22:37 2023, max compression
+gzip compressed data, was "pydtl_relativepath-0.1.0.tar", max compression
```

## Comparing `pydtl_relativepath-0.0.1.tar` & `pydtl_relativepath-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 18:22:37.886080 pydtl_relativepath-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-03-12 14:42:31.000000 pydtl_relativepath-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1132 2023-03-12 18:22:37.885119 pydtl_relativepath-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-03-12 18:21:35.000000 pydtl_relativepath-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 18:22:37.857138 pydtl_relativepath-0.0.1/pydtl_relativepath/
--rw-rw-rw-   0        0        0       39 2023-03-12 17:42:23.000000 pydtl_relativepath-0.0.1/pydtl_relativepath/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-03-12 18:08:52.000000 pydtl_relativepath-0.0.1/pydtl_relativepath/pydtl_relativepath.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:22:37.876171 pydtl_relativepath-0.0.1/pydtl_relativepath.egg-info/
--rw-rw-rw-   0        0        0     1132 2023-03-12 18:22:37.000000 pydtl_relativepath-0.0.1/pydtl_relativepath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-03-12 18:22:37.000000 pydtl_relativepath-0.0.1/pydtl_relativepath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 18:22:37.000000 pydtl_relativepath-0.0.1/pydtl_relativepath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-03-12 18:22:37.000000 pydtl_relativepath-0.0.1/pydtl_relativepath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 18:22:37.887076 pydtl_relativepath-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-03-12 15:38:03.000000 pydtl_relativepath-0.0.1/setup.py
+-rw-r--r--   0        0        0     1094 2023-03-12 14:42:31.684532 pydtl_relativepath-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1408 2023-04-15 16:27:37.325756 pydtl_relativepath-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      850 2023-04-15 17:43:11.612959 pydtl_relativepath-0.1.0/README.md
+-rw-r--r--   0        0        0       77 2023-04-15 16:59:25.097396 pydtl_relativepath-0.1.0/src/pydtl_relativepath/__init__.py
+-rw-r--r--   0        0        0     2555 2023-04-15 17:39:13.240363 pydtl_relativepath-0.1.0/src/pydtl_relativepath/pydtl_relativepath.py
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 pydtl_relativepath-0.1.0/PKG-INFO
```

### Comparing `pydtl_relativepath-0.0.1/LICENSE` & `pydtl_relativepath-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydtl_relativepath-0.0.1/pydtl_relativepath/pydtl_relativepath.py` & `pydtl_relativepath-0.1.0/src/pydtl_relativepath/pydtl_relativepath.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,61 @@
+"""
+Relative Path Utilities for multi-structured frameworks
+=======================================================
+
+Usage
+
+Whenever specifying a relative path use `rel2abs`
+
+See an Example below
+
+    from pydtl_relativepath import rel2abs as r2a
+    readmepath = r2a("README.txt")
+    print(open(readmepath, mode="r", encoding="utf-8").read())
+
+This will convert relative path specified to an absolute path relative to current file's directory
+Here, readmepath contains the absolute path for README.txt file
+and it is compatible with os.PathLike objects.
+"""
+
+
 import os
 import inspect
 
 
 class PathObj(os.PathLike):
     """Relative Path Object for all path handlings"""
-    def __init__(self, relative_path: str, root: str):
+
+    def __init__(self, relative_path: str, relative_to: str):
         """
         Path Object
 
         :param relative_path: Specify the relative path to be converted
-        :param root: Specify the root location. possible values: ['f' - current file's dir, 'c' - current working dir]
+        :param relative_to: Specify the root location. possible values: 'f' - current file's dir,
+                            'c' - current working dir
         """
 
         self.relative_path = relative_path
-        self.root_option = root
+        self.relative_to = relative_to
         self.absolute_path = self._frame_abs_path()
 
     def _frame_abs_path(self) -> str:
         root_path = ""
 
-        if self.root_option == 'f':
-            root_path = os.path.dirname(inspect.stack()[3].filename)  # current file's dir
-        elif self.root_option == 'c':
+        if self.relative_to == "f":
+            root_path = os.path.dirname(
+                inspect.stack()[3].filename
+            )  # current file's dir
+        elif self.relative_to == "c":
             root_path = os.path.abspath(os.curdir)  # current working dir
         else:
-            raise ValueError(f"Invalid root option [{self.root_option}]\nPossible options: "
-                              "['f' - current file's dir, 'c' - current working dir]")
+            raise ValueError(
+                f"Invalid root option [{self.relative_to}]\nPossible options: "
+                "'f' - current file's dir, 'c' - current working dir"
+            )
 
         abs_path = os.path.join(root_path, self.relative_path)
         return os.path.normcase(os.path.normpath(abs_path))
 
     def __repr__(self):
         return self.absolute_path
 
@@ -39,16 +65,17 @@
     def __fspath__(self):
         return self.absolute_path
 
     def __eq__(self, other):
         return os.path.samefile(self.absolute_path, other)
 
 
-def rel2abs(relative_path: str, root='f'):
+def rel2abs(relative_path: str, relative_to="f"):
     """
     Convert Relative Path to Absolute Path Object
 
     :param relative_path: Specify the relative path to be converted
-    :param root: Specify the root location. possible values: ['f' - current file's dir, 'c' - current working dir]
+    :param relative_to: Specify the root location. possible values: 'f' - current file's dir,
+                        'c' - current working dir
     """
 
-    return PathObj(relative_path=relative_path, root=root)
+    return PathObj(relative_path=relative_path, relative_to=relative_to)
```

