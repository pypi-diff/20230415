# Comparing `tmp/pandas_selector-1.3.3.tar.gz` & `tmp/pandas_selector-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_selector-1.3.3.tar", max compression
+gzip compressed data, was "pandas_selector-1.3.4.tar", max compression
```

## Comparing `pandas_selector-1.3.3.tar` & `pandas_selector-1.3.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      770 2023-04-05 16:52:10.827363 pandas_selector-1.3.3/pandas_selector/__init__.py
--rw-r--r--   0        0        0      560 2023-04-05 16:52:10.827363 pandas_selector-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      704 2023-04-05 16:52:11.324280 pandas_selector-1.3.3/setup.py
--rw-r--r--   0        0        0      691 2023-04-05 16:52:11.324578 pandas_selector-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      770 2023-04-15 19:33:39.244775 pandas_selector-1.3.4/pandas_selector/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-15 19:33:39.244775 pandas_selector-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-04-15 19:33:40.190523 pandas_selector-1.3.4/setup.py
+-rw-r--r--   0        0        0      691 2023-04-15 19:33:40.190787 pandas_selector-1.3.4/PKG-INFO
```

### Comparing `pandas_selector-1.3.3/pandas_selector/__init__.py` & `pandas_selector-1.3.4/pandas_selector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Stub package to simplify upgrading after renaming :mod:`pandas_selector` to :mod:`pandas_paddles`."""
 from warnings import warn
 
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 __all__ = ["DF", "S", "C"]
 
 warn("""\
 The package pandas_selector is deprecated in favor of pandas_paddles. Please replace pandas_selector by pandas_paddles in your dependencies and update your code by replacing
     from pandas_selector import ...
 with
     from pandas_paddles import ...
```

### Comparing `pandas_selector-1.3.3/pyproject.toml` & `pandas_selector-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pandas_selector"
-version = "1.3.3"
+version = "1.3.4"
 description = "Stub package to install the matching pandas_paddles"
 authors = ["Eike von Seggern <eikevons@mailbox.org>"]
 repository = "https://github.com/eikevons/pandas-paddles.git"
 license = "MIT"
 classifiers = [
   "Development Status :: 7 - Inactive"
 ]
 include ["pandas_selector/__init__.py"]
 exclude ["pandas_selector/__init__.py.IN"]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
-pandas_paddles = "1.3.3"
+pandas_paddles = "1.3.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pandas_selector-1.3.3/setup.py` & `pandas_selector-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pandas_selector']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas_paddles==1.3.3']
+['pandas_paddles==1.3.4']
 
 setup_kwargs = {
     'name': 'pandas-selector',
-    'version': '1.3.3',
+    'version': '1.3.4',
     'description': 'Stub package to install the matching pandas_paddles',
     'long_description': None,
     'author': 'Eike von Seggern',
     'author_email': 'eikevons@mailbox.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/eikevons/pandas-paddles.git',
```

### Comparing `pandas_selector-1.3.3/PKG-INFO` & `pandas_selector-1.3.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pandas-selector
-Version: 1.3.3
+Version: 1.3.4
 Summary: Stub package to install the matching pandas_paddles
 Home-page: https://github.com/eikevons/pandas-paddles.git
 License: MIT
 Author: Eike von Seggern
 Author-email: eikevons@mailbox.org
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pandas_paddles (==1.3.3)
+Requires-Dist: pandas_paddles (==1.3.4)
 Project-URL: Repository, https://github.com/eikevons/pandas-paddles.git
```

