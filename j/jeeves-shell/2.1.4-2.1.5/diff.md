# Comparing `tmp/jeeves_shell-2.1.4.tar.gz` & `tmp/jeeves_shell-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_shell-2.1.4.tar", max compression
+gzip compressed data, was "jeeves_shell-2.1.5.tar", max compression
```

## Comparing `jeeves_shell-2.1.4.tar` & `jeeves_shell-2.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.4/LICENSE
--rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.4/README.md
--rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.4/jeeves_shell/__init__.py
--rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.4/jeeves_shell/cli.py
--rw-r--r--   0        0        0     3328 2023-04-15 21:35:59.602828 jeeves_shell-2.1.4/jeeves_shell/discover.py
--rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.4/jeeves_shell/entry_points.py
--rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.4/jeeves_shell/errors.py
--rw-r--r--   0        0        0      192 2023-04-15 21:18:06.757963 jeeves_shell-2.1.4/jeeves_shell/import_by_path.py
--rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.4/jeeves_shell/jeeves.py
--rw-r--r--   0        0        0     1606 2023-04-15 21:36:13.526953 jeeves_shell-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 jeeves_shell-2.1.4/setup.py
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 jeeves_shell-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.5/LICENSE
+-rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.5/README.md
+-rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.5/jeeves_shell/__init__.py
+-rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.5/jeeves_shell/cli.py
+-rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.5/jeeves_shell/discover.py
+-rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.5/jeeves_shell/entry_points.py
+-rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.5/jeeves_shell/errors.py
+-rw-r--r--   0        0        0      192 2023-04-15 21:18:06.757963 jeeves_shell-2.1.5/jeeves_shell/import_by_path.py
+-rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.5/jeeves_shell/jeeves.py
+-rw-r--r--   0        0        0     1606 2023-04-15 21:43:21.558622 jeeves_shell-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 jeeves_shell-2.1.5/setup.py
+-rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 jeeves_shell-2.1.5/PKG-INFO
```

### Comparing `jeeves_shell-2.1.4/LICENSE` & `jeeves_shell-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.4/README.md` & `jeeves_shell-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.4/jeeves_shell/cli.py` & `jeeves_shell-2.1.5/jeeves_shell/cli.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.4/jeeves_shell/discover.py` & `jeeves_shell-2.1.5/jeeves_shell/discover.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,17 +81,17 @@
 
 
 def _augment_app_with_jeeves_file(
     app: Jeeves,
     path: Path,
 ) -> Jeeves:      # pragma: nocover
     commands = retrieve_commands_from_jeeves_file(path)
-    for _name, command in commands:
+    for name, command in commands:
         if _is_typer(command):
-            app.add_typer(command)
+            app.add_typer(typer_instance=command, name=name)
         else:
             app.command()(command)
 
     return app
 
 
 def _configure_callback(app: Jeeves) -> Jeeves:
```

### Comparing `jeeves_shell-2.1.4/pyproject.toml` & `jeeves_shell-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jeeves-shell"
 description = "Pythonic replacement for GNU Make"
-version = "2.1.4"
+version = "2.1.5"
 license = "MIT"
 
 authors = []
 
 readme = "README.md"
 
 repository = "https://github.com/jeeves-sh/jeeves-shell"
```

### Comparing `jeeves_shell-2.1.4/setup.py` & `jeeves_shell-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['j = jeeves_shell.cli:app']}
 
 setup_kwargs = {
     'name': 'jeeves-shell',
-    'version': '2.1.4',
+    'version': '2.1.5',
     'description': 'Pythonic replacement for GNU Make',
     'long_description': '# Jeeves Shell\n\n[![Build Status](https://github.com/jeeves-sh/jeeves-shell/workflows/test/badge.svg?branch=master&event=push)](https://github.com/jeeves-sh/jeeves-shell/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/jeeves-sh/jeeves-shell/branch/master/graph/badge.svg)](https://codecov.io/gh/jeeves-sh/jeeves-shell)\n[![Python Version](https://img.shields.io/pypi/pyversions/jeeves-shell.svg)](https://pypi.org/project/jeeves-shell/)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\nA Pythonic replacement for GNU Make, with re-usability and modularity added as a bonus.\n\n\n## Installation\n\n```bash\npip install jeeves-shell\n```\n\n## License\n\n[MIT](https://github.com/jeeves-sh/jeeves-shell/blob/master/LICENSE)\n\n\n## Credits\n\nThis project was generated with [`wemake-python-package`](https://github.com/wemake-services/wemake-python-package).\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jeeves-sh/jeeves-shell',
```

### Comparing `jeeves_shell-2.1.4/PKG-INFO` & `jeeves_shell-2.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeeves-shell
-Version: 2.1.4
+Version: 2.1.5
 Summary: Pythonic replacement for GNU Make
 Home-page: https://github.com/jeeves-sh/jeeves-shell
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

