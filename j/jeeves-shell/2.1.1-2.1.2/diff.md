# Comparing `tmp/jeeves_shell-2.1.1.tar.gz` & `tmp/jeeves_shell-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_shell-2.1.1.tar", max compression
+gzip compressed data, was "jeeves_shell-2.1.2.tar", max compression
```

## Comparing `jeeves_shell-2.1.1.tar` & `jeeves_shell-2.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.1/LICENSE
--rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.1/README.md
--rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.1/jeeves_shell/__init__.py
--rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.1/jeeves_shell/cli.py
--rw-r--r--   0        0        0     3205 2023-04-15 13:30:18.136327 jeeves_shell-2.1.1/jeeves_shell/discover.py
--rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.1/jeeves_shell/entry_points.py
--rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.1/jeeves_shell/errors.py
--rw-r--r--   0        0        0      620 2022-12-11 17:45:07.129586 jeeves_shell-2.1.1/jeeves_shell/import_by_path.py
--rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.1/jeeves_shell/jeeves.py
--rw-r--r--   0        0        0     1606 2023-04-15 13:21:35.506382 jeeves_shell-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 jeeves_shell-2.1.1/setup.py
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 jeeves_shell-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.2/LICENSE
+-rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.2/README.md
+-rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.2/jeeves_shell/__init__.py
+-rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.2/jeeves_shell/cli.py
+-rw-r--r--   0        0        0     3491 2023-04-15 14:02:36.175635 jeeves_shell-2.1.2/jeeves_shell/discover.py
+-rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.2/jeeves_shell/entry_points.py
+-rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.2/jeeves_shell/errors.py
+-rw-r--r--   0        0        0      620 2022-12-11 17:45:07.129586 jeeves_shell-2.1.2/jeeves_shell/import_by_path.py
+-rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.2/jeeves_shell/jeeves.py
+-rw-r--r--   0        0        0     1606 2023-04-15 14:02:51.735740 jeeves_shell-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 jeeves_shell-2.1.2/setup.py
+-rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 jeeves_shell-2.1.2/PKG-INFO
```

### Comparing `jeeves_shell-2.1.1/LICENSE` & `jeeves_shell-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.1/README.md` & `jeeves_shell-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.1/jeeves_shell/cli.py` & `jeeves_shell-2.1.2/jeeves_shell/cli.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.1/jeeves_shell/discover.py` & `jeeves_shell-2.1.2/jeeves_shell/discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import logging
 import os
 import string
 import types
 from pathlib import Path
 from typing import Any, Iterable, List, Optional, Tuple
 
@@ -61,28 +62,35 @@
     jeeves_file_name: str = 'jeeves.py',
 ) -> Iterable[Tuple[str, Any]]:
     try:
         jeeves_module = import_by_path(path=directory / jeeves_file_name)
     except FileNotFoundError as err:
         logger.debug('File not found: %s', err.filename)
         return
+    except RuntimeError as err:
+        logger.debug('Error while building spec: %s', err)
+        return
 
     for name, command in vars(jeeves_module).items():  # noqa: WPS421
         if not _is_name_suitable(name):
             continue
 
         if _is_function(command) or _is_typer(command):
             yield name, command
 
 
 def _augment_app_with_jeeves_file(
     app: Jeeves,
     path: Path,
 ) -> Jeeves:      # pragma: nocover
-    for _name, command in retrieve_commands_from_jeeves_file(path):
+    commands = itertools.chain(
+        retrieve_commands_from_jeeves_file(path, jeeves_file_name='jeeves.py'),
+        retrieve_commands_from_jeeves_file(path, jeeves_file_name='jeeves'),
+    )
+    for _name, command in commands:
         if _is_typer(command):
             app.add_typer(command)
         else:
             app.command()(command)
 
     return app
```

### Comparing `jeeves_shell-2.1.1/jeeves_shell/import_by_path.py` & `jeeves_shell-2.1.2/jeeves_shell/import_by_path.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.1/pyproject.toml` & `jeeves_shell-2.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jeeves-shell"
 description = "Pythonic replacement for GNU Make"
-version = "2.1.1"
+version = "2.1.2"
 license = "MIT"
 
 authors = []
 
 readme = "README.md"
 
 repository = "https://github.com/jeeves-sh/jeeves-shell"
```

### Comparing `jeeves_shell-2.1.1/setup.py` & `jeeves_shell-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['j = jeeves_shell.cli:app']}
 
 setup_kwargs = {
     'name': 'jeeves-shell',
-    'version': '2.1.1',
+    'version': '2.1.2',
     'description': 'Pythonic replacement for GNU Make',
     'long_description': '# Jeeves Shell\n\n[![Build Status](https://github.com/jeeves-sh/jeeves-shell/workflows/test/badge.svg?branch=master&event=push)](https://github.com/jeeves-sh/jeeves-shell/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/jeeves-sh/jeeves-shell/branch/master/graph/badge.svg)](https://codecov.io/gh/jeeves-sh/jeeves-shell)\n[![Python Version](https://img.shields.io/pypi/pyversions/jeeves-shell.svg)](https://pypi.org/project/jeeves-shell/)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\nA Pythonic replacement for GNU Make, with re-usability and modularity added as a bonus.\n\n\n## Installation\n\n```bash\npip install jeeves-shell\n```\n\n## License\n\n[MIT](https://github.com/jeeves-sh/jeeves-shell/blob/master/LICENSE)\n\n\n## Credits\n\nThis project was generated with [`wemake-python-package`](https://github.com/wemake-services/wemake-python-package).\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jeeves-sh/jeeves-shell',
```

### Comparing `jeeves_shell-2.1.1/PKG-INFO` & `jeeves_shell-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeeves-shell
-Version: 2.1.1
+Version: 2.1.2
 Summary: Pythonic replacement for GNU Make
 Home-page: https://github.com/jeeves-sh/jeeves-shell
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

