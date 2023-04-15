# Comparing `tmp/reactpy_jupyter-0.8.0.tar.gz` & `tmp/reactpy_jupyter-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_jupyter-0.8.0.tar", last modified: Sat Apr 15 01:28:08 2023, max compression
+gzip compressed data, was "reactpy_jupyter-0.8.1.tar", last modified: Sat Apr 15 01:57:24 2023, max compression
```

## Comparing `reactpy_jupyter-0.8.0.tar` & `reactpy_jupyter-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-04-15 01:28:08.694770 reactpy_jupyter-0.8.0/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1070 2023-04-12 03:10:15.000000 reactpy_jupyter-0.8.0/LICENSE
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       90 2023-04-14 17:00:53.000000 reactpy_jupyter-0.8.0/MANIFEST.in
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3861 2023-04-15 01:28:08.694770 reactpy_jupyter-0.8.0/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2964 2023-04-14 17:00:53.000000 reactpy_jupyter-0.8.0/README.md
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-04-15 01:28:08.686770 reactpy_jupyter-0.8.0/jupyter-config/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-04-15 01:28:08.690770 reactpy_jupyter-0.8.0/jupyter-config/jupyter_server_config.d/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      115 2023-04-14 17:00:53.000000 reactpy_jupyter-0.8.0/jupyter-config/jupyter_server_config.d/reactpy-jupyter.json
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      389 2023-04-15 01:23:50.000000 reactpy_jupyter-0.8.0/pyproject.toml
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-04-15 01:28:08.690770 reactpy_jupyter-0.8.0/reactpy_jupyter/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      637 2023-04-15 01:23:50.000000 reactpy_jupyter-0.8.0/reactpy_jupyter/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3975 2023-04-15 01:23:50.000000 reactpy_jupyter-0.8.0/reactpy_jupyter/import_resources.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1289 2023-04-15 01:23:50.000000 reactpy_jupyter-0.8.0/reactpy_jupyter/ipython_extension.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1277 2023-04-15 01:23:50.000000 reactpy_jupyter-0.8.0/reactpy_jupyter/jupyter_server_extension.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-04-15 01:28:08.694770 reactpy_jupyter-0.8.0/reactpy_jupyter/static/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)   744360 2023-04-15 01:28:08.000000 reactpy_jupyter-0.8.0/reactpy_jupyter/static/index.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4304 2023-04-15 01:23:50.000000 reactpy_jupyter-0.8.0/reactpy_jupyter/widget.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-04-15 01:28:08.694770 reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3861 2023-04-15 01:28:08.000000 reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      558 2023-04-15 01:28:08.000000 reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-04-15 01:28:08.000000 reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-04-12 03:54:41.000000 reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/not-zip-safe
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       86 2023-04-15 01:28:08.000000 reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       16 2023-04-15 01:28:08.000000 reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/top_level.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1208 2023-04-15 01:28:08.698770 reactpy_jupyter-0.8.0/setup.cfg
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5717 2023-04-15 01:23:50.000000 reactpy_jupyter-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 01:57:24.277758 reactpy_jupyter-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-15 01:57:24.277758 reactpy_jupyter-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 01:57:24.273758 reactpy_jupyter-0.8.1/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 01:57:24.277758 reactpy_jupyter-0.8.1/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/jupyter-config/jupyter_server_config.d/reactpy-jupyter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 01:57:24.277758 reactpy_jupyter-0.8.1/reactpy_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/reactpy_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/reactpy_jupyter/import_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/reactpy_jupyter/ipython_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/reactpy_jupyter/jupyter_server_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 01:57:24.277758 reactpy_jupyter-0.8.1/reactpy_jupyter/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   744360 2023-04-15 01:57:24.000000 reactpy_jupyter-0.8.1/reactpy_jupyter/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/reactpy_jupyter/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 01:57:24.277758 reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-15 01:57:24.000000 reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-15 01:57:24.000000 reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 01:57:24.000000 reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 01:57:08.000000 reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-15 01:57:24.000000 reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 01:57:24.000000 reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-15 01:57:24.281758 reactpy_jupyter-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-15 01:56:41.000000 reactpy_jupyter-0.8.1/setup.py
```

### Comparing `reactpy_jupyter-0.8.0/LICENSE` & `reactpy_jupyter-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.8.0/PKG-INFO` & `reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: reactpy_jupyter
-Version: 0.8.0
+Name: reactpy-jupyter
+Version: 0.8.1
 Summary: It's React, but in Python
 Home-page: https://github.com/reactive-python/reactpy
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -114,20 +114,19 @@
 ## Development Installation
 
 For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
 
     $ git clone https://github.com/reactive-python/reactpy-jupyter.git
     $ cd reactpy-jupyter
     $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix reactpy_jupyter
-    $ jupyter nbextension enable --py --sys-prefix reactpy_jupyter
 
-When actively developing your extension for JupyterLab, run the command:
+To automatically re-build and refresh Jupyter when making changes start a Vite dev server:
 
-    $ jupyter labextension develop --overwrite reactpy_jupyter
+    $ npx vite
 
-Then you need to rebuild the JS when you make a code change:
+Then, before importing `reactpy_jupyter` set the following environment variable:
 
-    $ cd js
-    $ yarn run build
-
-You then need to refresh the JupyterLab page when your javascript changes.
+```python
+import os
+os.environ["REACTPY_JUPYTER_DEV"] = "1"
+import reactpy_jupyter
+```
```

### Comparing `reactpy_jupyter-0.8.0/README.md` & `reactpy_jupyter-0.8.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -87,20 +87,19 @@
 ## Development Installation
 
 For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
 
     $ git clone https://github.com/reactive-python/reactpy-jupyter.git
     $ cd reactpy-jupyter
     $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix reactpy_jupyter
-    $ jupyter nbextension enable --py --sys-prefix reactpy_jupyter
 
-When actively developing your extension for JupyterLab, run the command:
+To automatically re-build and refresh Jupyter when making changes start a Vite dev server:
 
-    $ jupyter labextension develop --overwrite reactpy_jupyter
+    $ npx vite
 
-Then you need to rebuild the JS when you make a code change:
+Then, before importing `reactpy_jupyter` set the following environment variable:
 
-    $ cd js
-    $ yarn run build
-
-You then need to refresh the JupyterLab page when your javascript changes.
+```python
+import os
+os.environ["REACTPY_JUPYTER_DEV"] = "1"
+import reactpy_jupyter
+```
```

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter/__init__.py` & `reactpy_jupyter-0.8.1/reactpy_jupyter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 from . import jupyter_server_extension
 from .import_resources import setup_import_resources
 from .ipython_extension import load_ipython_extension, unload_ipython_extension
 from .widget import LayoutWidget, run, set_import_source_base_url, widgetize
 
-__version__ = "0.8.0"  # DO NOT MODIFY
+__version__ = "0.8.1"  # DO NOT MODIFY
 
 __all__ = [
     "LayoutWidget",
     "widgetize",
     "run",
     "load_ipython_extension",
     "unload_ipython_extension",
```

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter/import_resources.py` & `reactpy_jupyter-0.8.1/reactpy_jupyter/import_resources.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter/ipython_extension.py` & `reactpy_jupyter-0.8.1/reactpy_jupyter/ipython_extension.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter/jupyter_server_extension.py` & `reactpy_jupyter-0.8.1/reactpy_jupyter/jupyter_server_extension.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter/static/index.js` & `reactpy_jupyter-0.8.1/reactpy_jupyter/static/index.js`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter/widget.py` & `reactpy_jupyter-0.8.1/reactpy_jupyter/widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 import asyncio
+import os
 from functools import wraps
 from pathlib import Path
 from queue import Queue as SyncQueue
 from threading import Thread
 from typing import Any, Awaitable, Callable
 
 import anywidget
 from IPython.display import DisplayHandle
 from IPython.display import display as ipython_display
 from jsonpointer import set_pointer
-from reactpy.config import REACTPY_DEBUG_MODE
 from reactpy.core.layout import Layout
 from reactpy.core.types import ComponentType
 from traitlets import Unicode
 from typing_extensions import ParamSpec
 
-if REACTPY_DEBUG_MODE.current:
+DEV = bool(int(os.environ.get("REACTPY_JUPYTER_DEV", "0")))
+
+if DEV:
     # from `npx vite`
     ESM = "http://localhost:5173/src/index.js?anywidget"
 else:
     # from `npx vite build`
     bundled_assets_dir = Path(__file__).parent / "static"
     ESM = (bundled_assets_dir / "index.js").read_text()
```

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/PKG-INFO` & `reactpy_jupyter-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: reactpy-jupyter
-Version: 0.8.0
+Name: reactpy_jupyter
+Version: 0.8.1
 Summary: It's React, but in Python
 Home-page: https://github.com/reactive-python/reactpy
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -114,20 +114,19 @@
 ## Development Installation
 
 For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
 
     $ git clone https://github.com/reactive-python/reactpy-jupyter.git
     $ cd reactpy-jupyter
     $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix reactpy_jupyter
-    $ jupyter nbextension enable --py --sys-prefix reactpy_jupyter
 
-When actively developing your extension for JupyterLab, run the command:
+To automatically re-build and refresh Jupyter when making changes start a Vite dev server:
 
-    $ jupyter labextension develop --overwrite reactpy_jupyter
+    $ npx vite
 
-Then you need to rebuild the JS when you make a code change:
+Then, before importing `reactpy_jupyter` set the following environment variable:
 
-    $ cd js
-    $ yarn run build
-
-You then need to refresh the JupyterLab page when your javascript changes.
+```python
+import os
+os.environ["REACTPY_JUPYTER_DEV"] = "1"
+import reactpy_jupyter
+```
```

### Comparing `reactpy_jupyter-0.8.0/reactpy_jupyter.egg-info/SOURCES.txt` & `reactpy_jupyter-0.8.1/reactpy_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.8.0/setup.cfg` & `reactpy_jupyter-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.8.0/setup.py` & `reactpy_jupyter-0.8.1/setup.py`

 * *Files identical despite different names*

