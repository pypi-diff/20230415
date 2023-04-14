# Comparing `tmp/symdexer-0.2.1.tar.gz` & `tmp/symdexer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.2.1.tar", last modified: Fri Apr 14 23:20:36 2023, max compression
+gzip compressed data, was "symdexer-0.2.2.tar", last modified: Fri Apr 14 23:45:36 2023, max compression
```

## Comparing `symdexer-0.2.1.tar` & `symdexer-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.928285 symdexer-0.2.1/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      635 2023-04-14 23:20:36.927286 symdexer-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.1/README.md
--rw-rw-rw-   0        0        0      595 2023-04-14 23:16:48.000000 symdexer-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 23:20:36.929286 symdexer-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.876286 symdexer-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.905286 symdexer-0.2.1/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.1/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.1/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     2907 2023-04-14 23:04:34.000000 symdexer-0.2.1/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     4008 2023-04-14 23:07:14.000000 symdexer-0.2.1/src/symdexer/main.py
--rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.1/src/symdexer/modules.py
--rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.1/src/symdexer/symbols.py
--rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.1/src/symdexer/types.py
--rw-rw-rw-   0        0        0       19 2023-04-14 23:16:54.000000 symdexer-0.2.1/src/symdexer/version.py
-drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.925288 symdexer-0.2.1/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      635 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 23:45:36.541323 symdexer-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      635 2023-04-14 23:45:36.541323 symdexer-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.2/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-14 23:43:55.000000 symdexer-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 23:45:36.542324 symdexer-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 23:45:36.509323 symdexer-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 23:45:36.526327 symdexer-0.2.2/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.2/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.2/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     2912 2023-04-14 23:43:51.000000 symdexer-0.2.2/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     4008 2023-04-14 23:07:14.000000 symdexer-0.2.2/src/symdexer/main.py
+-rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.2/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.2/src/symdexer/symbols.py
+-rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.2/src/symdexer/types.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 23:44:14.000000 symdexer-0.2.2/src/symdexer/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 23:45:36.539321 symdexer-0.2.2/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-04-14 23:45:36.000000 symdexer-0.2.2/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-14 23:45:36.000000 symdexer-0.2.2/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 23:45:36.000000 symdexer-0.2.2/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-14 23:45:36.000000 symdexer-0.2.2/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 23:45:36.000000 symdexer-0.2.2/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.2.1/LICENSE.txt` & `symdexer-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.1/PKG-INFO` & `symdexer-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `symdexer-0.2.1/pyproject.toml` & `symdexer-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding and indexing symbols"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `symdexer-0.2.1/src/symdexer/cache.py` & `symdexer-0.2.2/src/symdexer/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             return
 
         self.db.execute(
             """
             INSERT OR IGNORE INTO Module (name, path, changed)
             VALUES (?, ? ,?)
             """,
-            (module.name, module.path.resolve(), module.mtime),
+            (module.name, str(module.path.resolve()), module.mtime),
         )
 
         for symbol, sym_type in iter_symbols(module.path):
             self.db.execute(
                 """
                 INSERT OR IGNORE INTO Symbol (name, type, module)
                 VALUES (?, ? ,?)
```

### Comparing `symdexer-0.2.1/src/symdexer/main.py` & `symdexer-0.2.2/src/symdexer/main.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.1/src/symdexer/modules.py` & `symdexer-0.2.2/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.1/src/symdexer/symbols.py` & `symdexer-0.2.2/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.1/src/symdexer/types.py` & `symdexer-0.2.2/src/symdexer/types.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.1/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.2/src/symdexer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

