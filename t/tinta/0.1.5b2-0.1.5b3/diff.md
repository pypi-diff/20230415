# Comparing `tmp/tinta-0.1.5b2.tar.gz` & `tmp/tinta-0.1.5b3.tar.gz`

## Comparing `tinta-0.1.5b2.tar` & `tinta-0.1.5b3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.gitattributes
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.pylintrc
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.5b2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.5b2/DESCRIPTION.rst
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.5b2/MANIFEST.in
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 tinta-0.1.5b2/Pipfile
--rw-r--r--   0        0        0    24383 2020-02-02 00:00:00.000000 tinta-0.1.5b2/Pipfile.lock
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 tinta-0.1.5b2/license.md
--rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 tinta-0.1.5b2/publish.sh
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinta-0.1.5b2/pytest.ini
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tinta-0.1.5b2/requirements.txt
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 tinta-0.1.5b2/setup.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.github/workflows/publish-test.yml
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.vscode/launch.json
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.vscode/settings.json
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.vscode/tasks.json
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 tinta-0.1.5b2/examples/basic_usage.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.5b2/examples/colors.ini
--rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.5b2/examples/tinta-discover.png
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tests/conftest.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tests/launch.json
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tests/test_discover.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tests/test_tinta.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tinta/__init__.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tinta/__main__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tinta/colors.ini
--rw-r--r--   0        0        0     7533 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tinta/discover.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 tinta-0.1.5b2/tinta/tinta.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 tinta-0.1.5b2/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.5b2/LICENSE
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 tinta-0.1.5b2/README.md
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 tinta-0.1.5b2/pyproject.toml
--rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 tinta-0.1.5b2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.gitattributes
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.pylintrc
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.5b3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.5b3/DESCRIPTION.rst
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.5b3/MANIFEST.in
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 tinta-0.1.5b3/Pipfile
+-rw-r--r--   0        0        0    24383 2020-02-02 00:00:00.000000 tinta-0.1.5b3/Pipfile.lock
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 tinta-0.1.5b3/license.md
+-rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 tinta-0.1.5b3/publish.sh
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinta-0.1.5b3/pytest.ini
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tinta-0.1.5b3/requirements.txt
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 tinta-0.1.5b3/setup.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.github/workflows/publish-test.yml
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.vscode/launch.json
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.vscode/settings.json
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.vscode/tasks.json
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 tinta-0.1.5b3/examples/basic_usage.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.5b3/examples/colors.ini
+-rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.5b3/examples/tinta-discover.png
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tests/conftest.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tests/launch.json
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tests/test_discover.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tests/test_tinta.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tinta/__init__.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tinta/__main__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tinta/colors.ini
+-rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tinta/discover.py
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 tinta-0.1.5b3/tinta/tinta.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 tinta-0.1.5b3/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.5b3/LICENSE
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 tinta-0.1.5b3/README.md
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 tinta-0.1.5b3/pyproject.toml
+-rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 tinta-0.1.5b3/PKG-INFO
```

### Comparing `tinta-0.1.5b2/CODE_OF_CONDUCT.md` & `tinta-0.1.5b3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/Pipfile.lock` & `tinta-0.1.5b3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/license.md` & `tinta-0.1.5b3/license.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/publish.sh` & `tinta-0.1.5b3/publish.sh`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/setup.py` & `tinta-0.1.5b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 from setuptools import setup
 
 with Path('README.md').open(encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='tinta',
-      version='0.1.5b2',
+      version='0.1.5b3',
       description='Tinta, a magical console output tool.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/brandonscript/tinta',
       author='Brandon Shelley',
       author_email='brandon@pacificaviator.co',
       install_requires=['ansicolors'],
```

### Comparing `tinta-0.1.5b2/.github/workflows/publish-test.yml` & `tinta-0.1.5b3/.github/workflows/publish-test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
 on:
   release:
     types: [published]
 
   workflow_dispatch:
 
+  push:
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
+    branches:
+      - main
+
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
```

### Comparing `tinta-0.1.5b2/.github/workflows/publish.yml` & `tinta-0.1.5b3/.github/workflows/publish.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 # You can also reference a tag or branch, but the action may change without warning.
 
 name: Publish Tinta to PyPI
 permissions:
   contents: read
   packages: write
   id-token: write
-  
+
 on:
   release:
     types: [published]
 
   workflow_dispatch:
 
+  push:
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
+    branches:
+      - main
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
```

### Comparing `tinta-0.1.5b2/.github/workflows/run-tests.yml` & `tinta-0.1.5b3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/.vscode/launch.json` & `tinta-0.1.5b3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/.vscode/settings.json` & `tinta-0.1.5b3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/.vscode/tasks.json` & `tinta-0.1.5b3/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/examples/basic_usage.py` & `tinta-0.1.5b3/examples/basic_usage.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/examples/tinta-discover.png` & `tinta-0.1.5b3/examples/tinta-discover.png`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/tests/conftest.py` & `tinta-0.1.5b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/tests/launch.json` & `tinta-0.1.5b3/tests/launch.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/tests/test_discover.py` & `tinta-0.1.5b3/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/tests/test_tinta.py` & `tinta-0.1.5b3/tests/test_tinta.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/tinta/__init__.py` & `tinta-0.1.5b3/tinta/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 from logging import getLogger
 
-__version__ = "0.1.5b2"
+__version__ = "0.1.5b3"
 
 logger = getLogger(__name__)
 
 try:
     from .tinta import Tinta
 except ImportError as e:
     logger.warning(e)
```

### Comparing `tinta-0.1.5b2/tinta/__main__.py` & `tinta-0.1.5b3/tinta/__main__.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/tinta/discover.py` & `tinta-0.1.5b3/tinta/discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,28 +143,28 @@
                          flatten(color_sets['dark']['color2']) +
                          flatten(color_sets['dark']['color3']) +
                          color_sets['dark']['greyscale'] + [0, 1, 2, 3, 4, 5, 6, 8, 9])
 
     return code in dark_colors
 
 
-def colorbox(code: int, text_only: bool = False) -> str:
+def colorbox(code: int, background: bool = False) -> str:
     """Returns a padded, styled box for the given color. If the color is 
     too dark, the text is white, otherwise dark grey.
     """
 
     # if color is too dark, use white text, otherwise black
     text_color = 15 if is_dark(code) else 0
 
     text = f"{str(code).rjust(4)} "
 
-    if text_only:
-        return f'\033[0m\033[38;5;{code}m{text}\033[0m'
-    else:
+    if background:
         return f'\033[0m\033[48;5;{code}m\033[38;5;{text_color}m{text}\033[0m'
+    else:
+        return f'\033[0m\033[38;5;{code}m{text}\033[0m'
 
 
 def discover(background: bool = False):
     """Prints all 256 colors in a matrix on your system."""
 
     print("Standard: ", end='')
     for col in color_sets['standard']:
```

### Comparing `tinta-0.1.5b2/tinta/tinta.py` & `tinta-0.1.5b3/tinta/tinta.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/.gitignore` & `tinta-0.1.5b3/.gitignore`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/LICENSE` & `tinta-0.1.5b3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/README.md` & `tinta-0.1.5b3/README.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.5b2/pyproject.toml` & `tinta-0.1.5b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 [project]
 name = "tinta"
-version = "0.1.5b2"
+version = "0.1.5b3"
 description = "Tinta, a magical console output tool."
  authors = [
   { name="Brandon Shelley", email="brandon@pacificaviator.co" },
 ]
 license = "MIT"
 readme = "README.md"
 keywords = ["console", "colors", "ansi", "print", "terminal", "development"]
```

### Comparing `tinta-0.1.5b2/PKG-INFO` & `tinta-0.1.5b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinta
-Version: 0.1.5b2
+Version: 0.1.5b3
 Summary: Tinta, a magical console output tool.
 Project-URL: homepage, https://github.com/brandonscript/tinta
 Project-URL: repository, https://github.com/brandonscript/tinta
 Author-email: Brandon Shelley <brandon@pacificaviator.co>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ansi,colors,console,development,print,terminal
```

