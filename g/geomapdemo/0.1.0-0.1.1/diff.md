# Comparing `tmp/geomapdemo-0.1.0.tar.gz` & `tmp/geomapdemo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.1.0.tar", last modified: Tue Apr 11 22:12:55 2023, max compression
+gzip compressed data, was "geomapdemo-0.1.1.tar", last modified: Sat Apr 15 18:57:58 2023, max compression
```

## Comparing `geomapdemo-0.1.0.tar` & `geomapdemo-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 22:12:55.000000 geomapdemo-0.1.0/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 22:12:55.625685 geomapdemo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-11 22:12:47.000000 geomapdemo-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-15 18:57:58.689623 geomapdemo-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/setup.py
```

### Comparing `geomapdemo-0.1.0/LICENSE` & `geomapdemo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.1.0/PKG-INFO` & `geomapdemo-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,26 +18,27 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geomapdemo
 
-
+[![Software License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
-
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
 
 **A python package for interactive mapping, testing.**
 
 
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
     
 
 ## Features
 
+-   Create random numbers and random text
 -   TODO
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.1.0/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.1.1/geomapdemo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,26 +18,27 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geomapdemo
 
-
+[![Software License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
-
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
 
 **A python package for interactive mapping, testing.**
 
 
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
     
 
 ## Features
 
+-   Create random numbers and random text
 -   TODO
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.1.0/setup.py` & `geomapdemo-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

