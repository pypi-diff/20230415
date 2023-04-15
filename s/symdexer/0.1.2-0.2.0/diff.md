# Comparing `tmp/symdexer-0.1.2.tar.gz` & `tmp/symdexer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.1.2.tar", last modified: Thu Apr 13 19:02:59 2023, max compression
+gzip compressed data, was "symdexer-0.2.0.tar", last modified: Fri Apr 14 20:57:28 2023, max compression
```

## Comparing `symdexer-0.1.2.tar` & `symdexer-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.172071 symdexer-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      548 2023-04-13 19:02:59.171071 symdexer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-04-13 01:29:38.000000 symdexer-0.1.2/README.md
--rw-rw-rw-   0        0        0      586 2023-04-13 19:01:36.000000 symdexer-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 19:02:59.172071 symdexer-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.138076 symdexer-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.153070 symdexer-0.1.2/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.1.2/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.1.2/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     1718 2023-04-13 17:01:00.000000 symdexer-0.1.2/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     2243 2023-04-13 17:04:05.000000 symdexer-0.1.2/src/symdexer/main.py
--rw-rw-rw-   0        0        0      564 2023-04-13 01:01:39.000000 symdexer-0.1.2/src/symdexer/modules.py
--rw-rw-rw-   0        0        0     1309 2023-04-13 17:01:00.000000 symdexer-0.1.2/src/symdexer/settings.py
--rw-rw-rw-   0        0        0      979 2023-04-13 02:29:44.000000 symdexer-0.1.2/src/symdexer/symbols.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:02:59.169071 symdexer-0.1.2/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      548 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 19:02:59.000000 symdexer-0.1.2/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.084179 symdexer-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      635 2023-04-14 20:57:28.083179 symdexer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.0/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-14 20:48:00.000000 symdexer-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 20:57:28.084179 symdexer-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.031178 symdexer-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.054188 symdexer-0.2.0/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.0/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.0/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     2829 2023-04-14 20:42:40.000000 symdexer-0.2.0/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     2884 2023-04-14 20:52:03.000000 symdexer-0.2.0/src/symdexer/main.py
+-rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.0/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.0/src/symdexer/symbols.py
+-rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.0/src/symdexer/types.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 20:47:18.000000 symdexer-0.2.0/src/symdexer/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.082180 symdexer-0.2.0/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.1.2/LICENSE.txt` & `symdexer-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.1.2/PKG-INFO` & `symdexer-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.1.2
-Summary: A CLI for finding symbols
+Version: 0.2.0
+Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Symdexer
 
 A command line utility for indexing and finding those pesky symbols in large packages.
+
+Help on how to use it can be viewed from the CLI, run `symdexer -h`.
+
```

### Comparing `symdexer-0.1.2/pyproject.toml` & `symdexer-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
-description = "A CLI for finding symbols"
+description = "A CLI for finding and indexing symbols"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 [project.scripts]
-symdexer = "symdexer.__main__:main"
+symdexer = "symdexer.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/antimach/symdexer"
```

### Comparing `symdexer-0.1.2/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.0/src/symdexer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.1.2
-Summary: A CLI for finding symbols
+Version: 0.2.0
+Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Symdexer
 
 A command line utility for indexing and finding those pesky symbols in large packages.
+
+Help on how to use it can be viewed from the CLI, run `symdexer -h`.
+
```

