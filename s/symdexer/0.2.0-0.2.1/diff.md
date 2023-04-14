# Comparing `tmp/symdexer-0.2.0.tar.gz` & `tmp/symdexer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symdexer-0.2.0.tar", last modified: Fri Apr 14 20:57:28 2023, max compression
+gzip compressed data, was "symdexer-0.2.1.tar", last modified: Fri Apr 14 23:20:36 2023, max compression
```

## Comparing `symdexer-0.2.0.tar` & `symdexer-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.084179 symdexer-0.2.0/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      635 2023-04-14 20:57:28.083179 symdexer-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.0/README.md
--rw-rw-rw-   0        0        0      595 2023-04-14 20:48:00.000000 symdexer-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 20:57:28.084179 symdexer-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.031178 symdexer-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.054188 symdexer-0.2.0/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.0/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.0/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     2829 2023-04-14 20:42:40.000000 symdexer-0.2.0/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     2884 2023-04-14 20:52:03.000000 symdexer-0.2.0/src/symdexer/main.py
--rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.0/src/symdexer/modules.py
--rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.0/src/symdexer/symbols.py
--rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.0/src/symdexer/types.py
--rw-rw-rw-   0        0        0       19 2023-04-14 20:47:18.000000 symdexer-0.2.0/src/symdexer/version.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:57:28.082180 symdexer-0.2.0/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      635 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 20:57:28.000000 symdexer-0.2.0/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.928285 symdexer-0.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      635 2023-04-14 23:20:36.927286 symdexer-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.1/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-14 23:16:48.000000 symdexer-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 23:20:36.929286 symdexer-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.876286 symdexer-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.905286 symdexer-0.2.1/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.1/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.1/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0     2907 2023-04-14 23:04:34.000000 symdexer-0.2.1/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     4008 2023-04-14 23:07:14.000000 symdexer-0.2.1/src/symdexer/main.py
+-rw-rw-rw-   0        0        0      723 2023-04-14 19:54:18.000000 symdexer-0.2.1/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 19:53:25.000000 symdexer-0.2.1/src/symdexer/symbols.py
+-rw-rw-rw-   0        0        0      667 2023-04-14 20:33:35.000000 symdexer-0.2.1/src/symdexer/types.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 23:16:54.000000 symdexer-0.2.1/src/symdexer/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 23:20:36.925288 symdexer-0.2.1/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 23:20:36.000000 symdexer-0.2.1/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.2.0/LICENSE.txt` & `symdexer-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.0/PKG-INFO` & `symdexer-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `symdexer-0.2.0/pyproject.toml` & `symdexer-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding and indexing symbols"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `symdexer-0.2.0/src/symdexer/cache.py` & `symdexer-0.2.1/src/symdexer/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,35 +59,36 @@
             return
 
         self.db.execute(
             """
             INSERT OR IGNORE INTO Module (name, path, changed)
             VALUES (?, ? ,?)
             """,
-            (module.name, str(module.path), module.mtime),
+            (module.name, module.path.resolve(), module.mtime),
         )
 
         for symbol, sym_type in iter_symbols(module.path):
             self.db.execute(
                 """
                 INSERT OR IGNORE INTO Symbol (name, type, module)
                 VALUES (?, ? ,?)
                 """,
                 (symbol, sym_type, module.name),
             )
 
-    def search(self, symbols: list[str], fuzzy: bool, types: list[str]) -> Generator[tuple[str, str], None, None]:
+    def search(self, symbols: list[str], fuzzy: bool, types: list[str]) -> Generator[tuple[str, str, str], None, None]:
         symbol_t = "name LIKE ?" if fuzzy else "name = ?"
         symbols_t = " OR ".join(symbol_t for _ in symbols)
         types_t = " OR ".join("type = ?" for _ in types)
 
         cursor = self.db.execute(
             f"""
-            SELECT GROUP_CONCAT(name, ", ") as names, module
+            SELECT GROUP_CONCAT(Symbol.name, ", ") as names, module, path
             FROM Symbol
+            INNER JOIN Module ON module = Module.name
             WHERE ({symbols_t}) AND ({types_t})
             GROUP BY
                 module
             ORDER BY
                 LENGTH(module) + LENGTH(names) ASC
             """,
             (*symbols, *types),
```

### Comparing `symdexer-0.2.0/src/symdexer/main.py` & `symdexer-0.2.1/src/symdexer/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,21 +3,31 @@
 
 from symdexer.version import VERSION
 from symdexer.cache import Cache
 from symdexer.symbols import SYM_TYPES
 from symdexer.types import package_type
 
 
-def find_command(cache_p: Path, symbols: list[str], fuzzy: bool, types: list[str]) -> None:
+def search_cache(cache_p: Path, symbols: list[str], fuzzy: bool, types: list[str]):
     if not cache_p.is_file():
         raise FileNotFoundError(f"Cache `{cache_p}` not found.")
 
     with Cache(cache_p) as cache:
-        for name, module in cache.search(symbols, fuzzy, types):
-            yield f"from {module} import {name}"
+        yield from cache.search(symbols, fuzzy, types)
+
+
+def find_command(cache_p: Path, symbols: list[str], fuzzy: bool, types: list[str]) -> None:
+    for names, module, _ in search_cache(cache_p, symbols, fuzzy):
+        yield f"from {module} import {names}"
+
+
+def locate_command(cache_p: Path, symbols: list[str], fuzzy: bool, types: list[str]) -> None:
+    for _, module, path in search_cache(cache_p, symbols, fuzzy):
+        yield module
+        yield path
 
 
 def index_command(cache_p: Path, packages: list[Path], reset: bool):
     if not cache_p.exists():
         reset = True
 
     with Cache(cache_p) as cache:
@@ -67,14 +77,43 @@
         "-t",
         "--types",
         dest="types",
         metavar="SYM_TYPE",
         choices=SYM_TYPES,
         default=SYM_TYPES,
         nargs="+",
+        help="Symbol types to show",
+    )
+
+    locate_parser = sub_parsers.add_parser(
+        "locate",
+        help="Locates the source paths of the modules where the given symbols reside",
+    )
+    locate_parser.add_argument(
+        "symbols",
+        metavar="SYMBOL",
+        nargs="+",
+        help="The symbols to look for",
+    )
+    locate_parser.add_argument(
+        "-f",
+        "--fuzzy",
+        dest="fuzzy",
+        action="store_true",
+        default=False,
+        help="If the symbols should be searched based on a pattern",
+    )
+    locate_parser.add_argument(
+        "-t",
+        "--types",
+        dest="types",
+        metavar="SYM_TYPE",
+        choices=SYM_TYPES,
+        default=SYM_TYPES,
+        nargs="+",
         help="Symbol types to show",
     )
 
     cache_parser = sub_parsers.add_parser(
         "index",
         help="Load symbols into cache",
     )
```

### Comparing `symdexer-0.2.0/src/symdexer/modules.py` & `symdexer-0.2.1/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.0/src/symdexer/symbols.py` & `symdexer-0.2.1/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.0/src/symdexer/types.py` & `symdexer-0.2.1/src/symdexer/types.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.0/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.1/src/symdexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

