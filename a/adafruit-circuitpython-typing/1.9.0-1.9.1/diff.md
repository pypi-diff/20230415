# Comparing `tmp/adafruit-circuitpython-typing-1.9.0.tar.gz` & `tmp/adafruit-circuitpython-typing-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-typing-1.9.0.tar", last modified: Mon Mar 20 23:40:24 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-typing-1.9.1.tar", last modified: Sat Apr 15 03:58:57 2023, max compression
```

## Comparing `adafruit-circuitpython-typing-1.9.0.tar` & `adafruit-circuitpython-typing-1.9.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.189885 adafruit-circuitpython-typing-1.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.181885 adafruit-circuitpython-typing-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.185885 adafruit-circuitpython-typing-1.9.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.185885 adafruit-circuitpython-typing-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.185885 adafruit-circuitpython-typing-1.9.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-20 23:40:24.189885 adafruit-circuitpython-typing-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.185885 adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-20 23:40:24.000000 adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-20 23:40:24.000000 adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 23:40:24.000000 adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-20 23:40:24.000000 adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-20 23:40:24.000000 adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.189885 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/device_drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/led.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/pwmio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/circuitpython_typing/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.189885 adafruit-circuitpython-typing-1.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.189885 adafruit-circuitpython-typing-1.9.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 23:40:24.189885 adafruit-circuitpython-typing-1.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/examples/typing_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-20 23:40:15.000000 adafruit-circuitpython-typing-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-20 23:40:04.000000 adafruit-circuitpython-typing-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 23:40:24.189885 adafruit-circuitpython-typing-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.455895 adafruit-circuitpython-typing-1.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.443895 adafruit-circuitpython-typing-1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.447895 adafruit-circuitpython-typing-1.9.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.447895 adafruit-circuitpython-typing-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.447895 adafruit-circuitpython-typing-1.9.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-15 03:58:57.455895 adafruit-circuitpython-typing-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.451895 adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-15 03:58:57.000000 adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-15 03:58:57.000000 adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:58:57.000000 adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-15 03:58:57.000000 adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 03:58:57.000000 adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.451895 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/device_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/led.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/pwmio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/circuitpython_typing/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.455895 adafruit-circuitpython-typing-1.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.455895 adafruit-circuitpython-typing-1.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:58:57.455895 adafruit-circuitpython-typing-1.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/examples/typing_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-15 03:58:47.000000 adafruit-circuitpython-typing-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-15 03:58:37.000000 adafruit-circuitpython-typing-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:58:57.455895 adafruit-circuitpython-typing-1.9.1/setup.cfg
```

### Comparing `adafruit-circuitpython-typing-1.9.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-typing-1.9.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/.gitignore` & `adafruit-circuitpython-typing-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/.pre-commit-config.yaml` & `adafruit-circuitpython-typing-1.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/.pylintrc` & `adafruit-circuitpython-typing-1.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-typing-1.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/LICENSE` & `adafruit-circuitpython-typing-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-typing-1.9.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/LICENSES/MIT.txt` & `adafruit-circuitpython-typing-1.9.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-typing-1.9.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/PKG-INFO` & `adafruit-circuitpython-typing-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-typing
-Version: 1.9.0
+Version: 1.9.1
 Summary: Types needed for type annotation that are not in `typing`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Typing
 Keywords: adafruit,blinka,circuitpython,micropython,circuitpython_typing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -71,15 +71,15 @@
     python3 -m venv .venv
     source .venv/bin/activate
     pip3 install adafruit-circuitpython-typing
 
 
 Documentation
 =============
-API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/circuitpython_typing/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/adafruit-circuitpython-typing/en/latest/>`_.
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
```

### Comparing `adafruit-circuitpython-typing-1.9.0/README.rst` & `adafruit-circuitpython-typing-1.9.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     python3 -m venv .venv
     source .venv/bin/activate
     pip3 install adafruit-circuitpython-typing
 
 
 Documentation
 =============
-API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/circuitpython_typing/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/adafruit-circuitpython-typing/en/latest/>`_.
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
```

### Comparing `adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/PKG-INFO` & `adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-typing
-Version: 1.9.0
+Version: 1.9.1
 Summary: Types needed for type annotation that are not in `typing`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Typing
 Keywords: adafruit,blinka,circuitpython,micropython,circuitpython_typing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -71,15 +71,15 @@
     python3 -m venv .venv
     source .venv/bin/activate
     pip3 install adafruit-circuitpython-typing
 
 
 Documentation
 =============
-API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/circuitpython_typing/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/adafruit-circuitpython-typing/en/latest/>`_.
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
```

### Comparing `adafruit-circuitpython-typing-1.9.0/adafruit_circuitpython_typing.egg-info/SOURCES.txt` & `adafruit-circuitpython-typing-1.9.1/adafruit_circuitpython_typing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/__init__.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Types needed for type annotation that are not in `typing`
 
 
 * Author(s): Alec Delaney, Dan Halbert, Randy Hudson
 """
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Typing.git"
 
 import array
 from typing import Union, Optional
 from typing_extensions import Protocol, TypeAlias  # Safety import for Python 3.7
 
 # Lists below are alphabetized.
```

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/device_drivers.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/device_drivers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/http.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/http.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/io.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/io.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/led.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/led.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/pil.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/pil.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/pwmio.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/pwmio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/circuitpython_typing/socket.py` & `adafruit-circuitpython-typing-1.9.1/circuitpython_typing/socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/docs/_static/favicon.ico` & `adafruit-circuitpython-typing-1.9.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/docs/conf.py` & `adafruit-circuitpython-typing-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/docs/index.rst` & `adafruit-circuitpython-typing-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.0/pyproject.toml` & `adafruit-circuitpython-typing-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-typing"
 description = "Types needed for type annotation that are not in `typing`"
-version = "1.9.0"
+version = "1.9.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Typing"}
 keywords = [
     "adafruit",
```

