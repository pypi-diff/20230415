# Comparing `tmp/toml-cli-0.3.1.tar.gz` & `tmp/toml_cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml-cli-0.3.1.tar", max compression
+gzip compressed data, was "toml_cli-0.4.0.tar", max compression
```

## Comparing `toml-cli-0.3.1.tar` & `toml_cli-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11357 2022-05-16 17:41:10.250257 toml-cli-0.3.1/LICENSE
--rw-r--r--   0        0        0      780 2022-05-16 17:41:10.250257 toml-cli-0.3.1/README.md
--rw-r--r--   0        0        0      597 2022-05-16 17:41:10.250257 toml-cli-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2323 2022-05-16 17:41:10.250257 toml-cli-0.3.1/toml_cli/__init__.py
--rw-r--r--   0        0        0     1603 2022-05-16 17:41:39.418598 toml-cli-0.3.1/setup.py
--rw-r--r--   0        0        0     1568 2022-05-16 17:41:39.419109 toml-cli-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 22:51:48.834797 toml_cli-0.4.0/LICENSE
+-rw-r--r--   0        0        0      780 2023-04-14 22:51:48.834797 toml_cli-0.4.0/README.md
+-rw-r--r--   0        0        0      646 2023-04-14 22:51:48.834797 toml_cli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2612 2023-04-14 22:51:48.834797 toml_cli-0.4.0/toml_cli/__init__.py
+-rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 toml_cli-0.4.0/PKG-INFO
```

### Comparing `toml-cli-0.3.1/LICENSE` & `toml_cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toml-cli-0.3.1/README.md` & `toml_cli-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `toml-cli-0.3.1/pyproject.toml` & `toml_cli-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "toml-cli"
-version = "0.3.1"
+version = "0.4.0"
 description = "Command line interface to read and write keys/values to/from toml files"
 authors = ["Marc Rijken"]
 license = "MIT"
 repository = "https://github.com/mrijken/toml-cli"
 readme = "README.md"
-packages = [
-    { include = "toml_cli" },
-]
+packages = [{ include = "toml_cli" }]
 
 [tool.poetry.scripts]
 toml = 'toml_cli:main'
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.7"
 typer = ">=0.3.2"
 tomlkit = ">=0.7.2"
 regex = ">=2020.7.14"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
-black = "^20.8b1"
+pytest = "^7.3.0"
+black = "^23.3.0"
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `toml-cli-0.3.1/toml_cli/__init__.py` & `toml_cli-0.4.0/toml_cli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,42 @@
+import json
 import pathlib
 from typing import Optional
 
 import tomlkit
 import tomlkit.exceptions
 import typer
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True)
 
 
 @app.command("get")
-def get(key: Optional[str] = typer.Argument(None), toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml"))):
+def get(
+    key: Optional[str] = typer.Argument(None),
+    toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml")),
+):
     """Get a value from a toml file"""
     toml_part = tomlkit.parse(toml_path.read_text())
 
     if key is not None:
         for key_part in key.split("."):
             toml_part = toml_part[key_part]
 
-    typer.echo(toml_part)
+    typer.echo(json.dumps(toml_part))
 
 
 @app.command("set")
 def set_(
     key: str,
     value: str,
     toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml")),
     to_int: bool = typer.Option(False),
     to_float: bool = typer.Option(False),
     to_bool: bool = typer.Option(False),
+    to_array: bool = typer.Option(False, help="accepts a valid json array and covert it to toml, ie [\"Amsterdam\",\"Rotterdam\"]"),
 ):
     """Set a value to a toml file"""
     toml_part = toml_file = tomlkit.parse(toml_path.read_text())
 
     for key_part in key.split(".")[:-1]:
         try:
             toml_part = toml_part[key_part]
@@ -39,38 +44,43 @@
             typer.echo(f"Key {key} can not set", err=True)
 
     if to_int:
         value = int(value)
     if to_float:
         value = float(value)
     if to_bool:
-        value = value.lower() in ['true', 'yes', 'y', '1']
+        value = value.lower() in ["true", "yes", "y", "1"]
+    if to_array:
+        value = json.loads(value)
 
     toml_part[key.split(".")[-1]] = value
 
     toml_path.write_text(tomlkit.dumps(toml_file))
 
 
 @app.command("add_section")
 def add_section(
-    key: str, toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml")),
+    key: str,
+    toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml")),
 ):
     """Add a section with the given key"""
     toml_part = toml_file = tomlkit.parse(toml_path.read_text())
 
     for key_part in key.split("."):
         if key_part not in toml_part:
             toml_part[key_part] = tomlkit.table()
         toml_part = toml_part[key_part]
 
     toml_path.write_text(tomlkit.dumps(toml_file))
 
 
 @app.command("unset")
-def unset(key: str, toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml"))):
+def unset(
+    key: str, toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml"))
+):
     """Unset a value from a toml file"""
     toml_part = toml_file = tomlkit.parse(toml_path.read_text())
 
     for key_part in key.split(".")[:-1]:
         try:
             toml_part = toml_part[key_part]
         except tomlkit.exceptions.NonExistentKey:
@@ -79,7 +89,11 @@
     del toml_part[key.split(".")[-1]]
 
     toml_path.write_text(tomlkit.dumps(toml_file))
 
 
 def main():
     app()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `toml-cli-0.3.1/PKG-INFO` & `toml_cli-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: toml-cli
-Version: 0.3.1
+Version: 0.4.0
 Summary: Command line interface to read and write keys/values to/from toml files
 Home-page: https://github.com/mrijken/toml-cli
 License: MIT
 Author: Marc Rijken
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: regex (>=2020.7.14)
 Requires-Dist: tomlkit (>=0.7.2)
 Requires-Dist: typer (>=0.3.2)
 Project-URL: Repository, https://github.com/mrijken/toml-cli
 Description-Content-Type: text/markdown
 
 # tom-cli
```

