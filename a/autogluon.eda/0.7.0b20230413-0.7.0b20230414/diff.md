# Comparing `tmp/autogluon.eda-0.7.0b20230413.tar.gz` & `tmp/autogluon.eda-0.7.0b20230414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.eda-0.7.0b20230413.tar", last modified: Thu Apr 13 09:04:51 2023, max compression
+gzip compressed data, was "autogluon.eda-0.7.0b20230414.tar", last modified: Fri Apr 14 09:04:40 2023, max compression
```

## Comparing `autogluon.eda-0.7.0b20230413.tar` & `autogluon.eda-0.7.0b20230414.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-13 09:04:51.812993 autogluon.eda-0.7.0b20230413/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/autogluon/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    23617 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/autogluon/eda/auto/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61305 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/auto/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/autogluon/eda/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-13 09:03:58.000000 autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/shift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:04:51.808992 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:04:51.000000 autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.299186 autogluon.eda-0.7.0b20230414/
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-14 09:04:40.299186 autogluon.eda-0.7.0b20230414/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-14 09:04:40.299186 autogluon.eda-0.7.0b20230414/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.291185 autogluon.eda-0.7.0b20230414/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.295185 autogluon.eda-0.7.0b20230414/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.295185 autogluon.eda-0.7.0b20230414/src/autogluon/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.295185 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.295185 autogluon.eda-0.7.0b20230414/src/autogluon/eda/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77558 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/auto/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.295185 autogluon.eda-0.7.0b20230414/src/autogluon/eda/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.299186 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 09:03:45.000000 autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/shift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:04:40.295185 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:04:40.000000 autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/zip-safe
```

### Comparing `autogluon.eda-0.7.0b20230413/PKG-INFO` & `autogluon.eda-0.7.0b20230414/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.7.0b20230413
+Version: 0.7.0b20230414
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.eda-0.7.0b20230413/setup.cfg` & `autogluon.eda-0.7.0b20230414/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 	flake8
 	pytest-cov
 	{[pkg-imports]deps}
 commands = 
 	pytest {posargs}
 
 [testenv:typecheck]
-basepython = python3.8
 deps = 
 	pytest
 	pytest-mypy
 	types-requests
 	types-setuptools
 	{[pkg-imports]deps}
 commands =
```

### Comparing `autogluon.eda-0.7.0b20230413/setup.py` & `autogluon.eda-0.7.0b20230414/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     'matplotlib>=3.4,<3.7',
     'missingno>=0.5.1,<0.6',
     'phik>=0.12.2,<0.13',
     'seaborn>=0.12.0,<0.13',
     'ipywidgets>=7.7.1,<9.0',  # min versions guidance: 7.7.1 collab/kaggle
     'shap>=0.41,<0.42',
     'yellowbrick>=1.5,<1.6',
+    'pyod>=1.0,<1.1',
+    'suod>=0.0.8,<0.1',
     f'autogluon.core=={version}',
     f'autogluon.common=={version}',
     f'autogluon.features=={version}',
     f'autogluon.tabular=={version}',
 ]
 
 extras_require = dict()
```

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/base.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/dataset.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/explain.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/interaction.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 from scipy import stats
 from scipy.cluster import hierarchy as hc
 from scipy.stats import spearmanr
 
 from .. import AnalysisState
 from .base import AbstractAnalysis
 
-__all__ = ["Correlation", "CorrelationSignificance", "FeatureInteraction", "DistributionFit"]
+__all__ = [
+    "Correlation",
+    "CorrelationSignificance",
+    "FeatureInteraction",
+    "DistributionFit",
+    "FeatureDistanceAnalysis",
+]
 
 from autogluon.common.features.types import R_FLOAT, R_INT
 
 
 class Correlation(AbstractAnalysis):
     """
     Correlation analysis.
```

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/missing.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/model.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/shift.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/shift.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 
 
 class XShiftDetector(AbstractAnalysis, StateCheckMixin):
     """Detect a change in covariate (X) distribution between training and test, which we call XShift.  It can tell you
     if your training set is not representative of your test set distribution.  This is done with a Classifier 2
     Sample Test.
 
+    State attributes
+
+    - `state.xshift_results`: outputs the results of XShift detection,
+        dict of
+            - `detection_status`: bool, True if detected
+            - `test_statistic`: float, the C2ST statistic
+            - `pvalue`: float, the p-value using permutation test
+            - `pvalue_threshold`: float, the decision p-value threshold
+            - `feature_importance`: DataFrame, the feature importance dataframe, if computed
+
     Parameters
     ----------
     classifier_class : an AutoGluon predictor, such as autogluon.tabular.TabularPredictor (default)
         The predictor that will be fit on training set and predict the test set
     compute_fi : bool, default = True
         To compute the feature importances set to True, this can be computationally intensive
     pvalue_thresh : float, default = 0.01
@@ -39,23 +49,14 @@
     classifier_fit_kwargs : dict, default = {}
         The kwargs passed to the classifier's `fit` call, a member of classifier_class
     num_permutations: int, default = 1000
         The number of permutations used for any permutation based method
     test_size_2st: float, default = 0.3
         The size of the test set in the training test split in 2ST
 
-    State attributes
-    ----------------
-    state.xshift_results: outputs the results of XShift detection,
-        dict of
-            - 'detection_status': bool, True if detected
-            - 'test_statistic': float, the C2ST statistic
-            - 'pvalue': float, the p-value using permutation test
-            - 'pvalue_threshold': float, the decision p-value threshold
-            - 'feature_importance': DataFrame, the feature importance dataframe, if computed
     """
 
     def __init__(
         self,
         classifier_class: Any = TabularPredictor,
         compute_fi: bool = True,
         pvalue_thresh: float = 0.01,
```

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/analysis/transform.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/auto/simple.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/auto/simple.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from autogluon.common.utils.log_utils import verbosity2loglevel
 from autogluon.features import CategoryFeatureGenerator
 from autogluon.tabular import TabularPredictor
 
 from .. import AnalysisState
 from ..analysis import (
+    AnomalyDetectorAnalysis,
     ApplyFeatureGenerator,
     AutoGluonModelEvaluator,
     AutoGluonModelQuickFit,
     Correlation,
     DistributionFit,
     FeatureInteraction,
     MissingValuesAnalysis,
@@ -27,17 +28,19 @@
     LabelInsightsAnalysis,
     RawTypesAnalysis,
     Sampler,
     SpecialTypesAnalysis,
     VariableTypeAnalysis,
 )
 from ..analysis.interaction import FeatureDistanceAnalysis
-from ..state import expand_nested_args_into_nested_maps, is_key_present_in_state
+from ..state import is_key_present_in_state
+from ..utils.common import expand_nested_args_into_nested_maps, get_empty_dict_if_none
 from ..utils.defaults import QuickFitDefaults
 from ..visualization import (
+    AnomalyScoresVisualization,
     ConfusionMatrix,
     CorrelationVisualization,
     DatasetStatistics,
     DatasetTypeMismatch,
     ExplainForcePlot,
     ExplainWaterfallPlot,
     FeatureImportance,
@@ -57,19 +60,20 @@
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "analyze",
     "analyze_interaction",
     "covariate_shift_detection",
     "dataset_overview",
+    "detect_anomalies",
+    "explain_rows",
     "missing_values_analysis",
+    "partial_dependence_plots",
     "quick_fit",
     "target_analysis",
-    "explain_rows",
-    "partial_dependence_plots",
 ]
 
 DEFAULT_SAMPLE_SIZE = 10000
 
 
 def analyze(
     train_data: Optional[pd.DataFrame] = None,
@@ -121,14 +125,29 @@
         If using logging, you can alternatively control amount of information printed via `logger.setLevel(L)`,
         where `L` ranges from 0 to 50 (Note: higher values of `L` correspond to fewer print statements, opposite of verbosity levels).
 
     Returns
     -------
     state after `fit` call if `return_state` is `True`; `None` otherwise
 
+    Examples
+    --------
+    >>> import autogluon.eda.analysis as eda
+    >>> import autogluon.eda.visualization as viz
+    >>> import autogluon.eda.auto as auto
+    >>> state = auto.analyze(
+    >>>     train_data=..., label=..., return_state=True,
+    >>>     anlz_facets=[
+    >>>         # Add analysis chain here
+    >>>     ],
+    >>>     viz_facets=[
+    >>>         # Add visualization facets here
+    >>>     ]
+    >>> )
+
     """
 
     if viz_facets is None:
         viz_facets = []
 
     if anlz_facets is None:
         anlz_facets = []
@@ -188,15 +207,15 @@
     y: Optional[str], default = None
     hue: Optional[str], default = None
     fit_distributions: Union[bool, str, List[str]], default = False,
         If `True`, or list of distributions is provided, then fit distributions. Performed only if `y` and `hue` are not present.
     chart_args: Optional[dict], default = None
         kwargs to pass into visualization component
     fig_args: Optional[Dict[str, Any]], default = None,
-        kwargs to pass into chart figure
+        kwargs to pass into visualization component
 
     Examples
     --------
     >>> import pandas as pd
     >>> import autogluon.eda.auto as auto
     >>>
     >>> df_train = pd.DataFrame(...)
@@ -316,14 +335,29 @@
         - samples with the least distance from the other class - candidates for labeling
 
     Supported `fig_args`/`chart_args` keys:
         - `confusion_matrix.<property>` - confusion matrix chart for classification predictor
         - `regression_eval.<property>` - regression predictor results chart
         - `feature_importance.<property>` - feature importance barplot chart
 
+    State attributes
+
+    - `model`
+        trained model
+    - `model_evaluation.importance`
+        feature importance calculated using the trained model
+    - `model_evaluation.leaderboard`
+        trained models leaderboard
+    - `model_evaluation.highest_error`
+        misclassified rows with the highest error between prediction and ground truth
+    - `model_evaluation.undecided` (classification only)
+        misclassified rows with the prediction closest to the decision boundary
+    - `model_evaluation.confusion_matrix` (classification only)
+        confusion matrix values
+
     Parameters
     ----------
     train_data: DataFrame
         training dataset
     test_data: DataFrame
         test dataset
     label: str
@@ -373,14 +407,15 @@
     Returns
     -------
         state after `fit` call if `return_state` is `True`; `None` otherwise
 
     Examples
     --------
     >>> import autogluon.eda.analysis as eda
+    >>> import autogluon.eda.auto as auto
     >>>
     >>> # Quick fit
     >>> state = auto.quick_fit(
     >>>     train_data=..., label=...,
     >>>     return_state=True,  # return state object from call
     >>>     fig_args={"regression_eval.figsize": (8,6)},  # customize regression evaluation `figsize`
     >>>     chart_args={"regression_eval.residuals_plot_mode": "hist"}  # customize regression evaluation `residuals_plot_mode`
@@ -707,14 +742,15 @@
             VariableTypeAnalysis(),
             XShiftDetector(classifier_kwargs=dict(path=path, verbosity=verbosity), classifier_fit_kwargs=fit_args),
         ],
         viz_facets=[XShiftSummary()],
     )
 
     # Plot distribution differences between datasets
+    # TODO: move `vars_to_plot` calculation to analysis
     xshift_results: AnalysisState = state.xshift_results  # type: ignore # state is always present
     if xshift_results.detection_status:
         fi = xshift_results.feature_importance
         fi = fi[fi.p_value <= xshift_results.pvalue_threshold]
         vars_to_plot = fi.index.tolist()[: XShiftSummary.MAX_FEATURES_TO_DISPLAY]
         if len(vars_to_plot) > 0:
             _train_data = train_data[vars_to_plot].copy()
@@ -767,20 +803,14 @@
         if _is_lightgbm_available():
             fit_args["hyperparameters"] = QuickFitDefaults.DEFAULT_LGBM_CONFIG
         else:
             fit_args["hyperparameters"] = QuickFitDefaults.DEFAULT_RF_CONFIG
     return fit_args
 
 
-def get_empty_dict_if_none(value) -> dict:
-    if value is None:
-        value = {}
-    return value
-
-
 def target_analysis(
     train_data: pd.DataFrame,
     label: str,
     test_data: Optional[pd.DataFrame] = None,
     problem_type: str = "auto",
     fit_distributions: Union[bool, str, List[str]] = True,
     sample: Union[None, int, float] = DEFAULT_SAMPLE_SIZE,
@@ -1097,14 +1127,35 @@
         is observed.
     return_state: bool, default = False
         return state if `True`
     fit_args: Optional[Dict[str, Any]], default = None,
         kwargs for `ShapAnalysis`.
     kwargs
 
+    Examples
+    --------
+    >>> import autogluon.eda.auto as auto
+    >>>
+    >>> state = auto.quick_fit(
+    >>>     train_data=...,
+    >>>     label=...,
+    >>>     return_state=True,
+    >>> )
+    >>>
+    >>> # quick_fit stored model in `state.model`, and can be passed here.
+    >>> # This will visualize 1st row of rows with the highest errors;
+    >>> # these rows are stored under `state.model_evaluation.highest_error`
+    >>> auto.explain_rows(
+    >>>     train_data=...,
+    >>>     model=state.model,
+    >>>     display_rows=True,
+    >>>     rows=state.model_evaluation.highest_error[:1],
+    >>>     plot='waterfall',  # visualize as waterfall plot
+    >>> )
+
     See Also
     --------
     :py:class:`~shap.KernelExplainer`
     :py:class:`~autogluon.eda.analysis.explain.ShapAnalysis`
     :py:class:`~autogluon.eda.visualization.explain.ExplainForcePlot`
     :py:class:`~autogluon.eda.visualization.explain.ExplainWaterfallPlot`
     """
@@ -1148,14 +1199,18 @@
     chart_args: Optional[Dict[str, Dict[str, Any]]] = None,
     show_help_text: bool = True,
     return_state: bool = False,
     col_number_warning: int = 20,
     **fit_args,
 ):
     """
+    Partial Dependence Plot (PDP)
+
+    Analyze and interpret the relationship between a target variable and a specific feature in a machine learning model.
+    PDP helps in understanding the marginal effect of a feature on the predicted outcome while holding other features constant
 
     The visualizations have two modes:
     - Display Partial Dependence Plots (PDP) with Individual Conditional Expectation (ICE) - this is the default mode of operation
     - Two-Way PDP plots - this mode can be selected via passing two `features` and setting `two_way = True`
 
     ICE plots complement PDP by showing the relationship between a feature and the model's output for each individual instance in the dataset.
     ICE lines (blue) can be overlaid on PDPs (red) to provide a more detailed view of how the model behaves for specific instances.
@@ -1195,14 +1250,19 @@
         For example, if one feature measures the length of an object and another measures its width, a two-way PDP could show how the
         combination of these features affects the predicted outcome.
     - `Domain knowledge`: If domain knowledge suggests that the relationship between two features might be important for the model's output,
         a two-way PDP can help to explore and validate these hypotheses.
     - `Feature importance`: If feature importance analysis ranks both features high in the leaderboard, it might be beneficial
         to examine their joint effect on the model's predictions.
 
+    State attributes
+
+    - `pdp_id_to_category_mappings`
+        Categorical are represented in charts as numbers; id to value mappings are available in this property.
+
     Parameters
     ----------
     train_data: DataFrame
         training dataset
     label: str
         target variable
     target: Optional[Any], default = None
@@ -1222,25 +1282,36 @@
         `None` means no sampling
         See also :func:`autogluon.eda.analysis.dataset.Sampler`
     fig_args: Optional[Dict[str, Any]], default = None
         kwargs to pass into chart figure
     chart_args: Optional[dict], default = None
         kwargs to pass into visualization component
     show_help_text:bool, default = True
+        if `True` shows additional information how to interpret the data
     return_state: bool, default = False
         return state if `True`
     col_number_warning: int, default = 20
         number of features to visualize after which the warning will be displayed to warn about rendering time
     fit_args: Optional[Dict[str, Dict[str, Any]]], default = None,
         kwargs to pass into `TabularPredictor` fit.
 
     Returns
     -------
     state after `fit` call if `return_state` is `True`; `None` otherwise
 
+    Examples
+    --------
+    >>> import autogluon.eda.auto as auto
+    >>>
+    >>> # Plot all features in a grid
+    >>> auto.partial_dependence_plots(train_data=..., label=...)
+    >>>
+    >>> # Plot two-way feature interaction for features `feature_a` and `feature_b`
+    >>> auto.partial_dependence_plots(train_data=..., label=..., features=['feature_a', 'feature_b'], two_way=True)
+
     See Also
     --------
     :py:class:`~autogluon.eda.visualization.interaction.PDPInteractions`
     """
 
     chart_args, fig_args, features = _validate_and_normalize_pdp_args(
         train_data, features, fig_args, chart_args, col_number_warning
@@ -1280,15 +1351,16 @@
                 "* **Feature value range**: Observe the range of the feature values on both axes to understand the domain of the interaction. "
                 "This can help you identify whether the model is making predictions within reasonable bounds or if there are extrapolations "
                 "beyond the training data.\n"
                 "* **Areas of high uncertainty**: Look for areas in the plot where the predictions are less certain, which may be indicated by "
                 "larger confidence intervals, higher variance, or fewer data points. These areas may require further investigation or additional data.\n"
                 "* **Outliers and anomalies**: Check for any outliers or anomalies in the plot that may indicate issues with the model or the data. "
                 "These could be regions of the plot with unexpected patterns or values that do not align with the overall trend.\n"
-                "* **Sensitivity to feature values**: Assess how sensitive the predicted outcome is to changes in the feature values.",
+                "* **Sensitivity to feature values**: Assess how sensitive the predicted outcome is to changes in the feature values.\n\n"
+                "<sub><sup>Use `show_help_text=False` to hide this information when calling this function.</sup></sub>",
                 condition_fn=lambda _: show_help_text and two_way,
             ),
             MarkdownSectionComponent("### Partial Dependence Plots", condition_fn=lambda _: not two_way),
             MarkdownSectionComponent(
                 "Individual Conditional Expectation (ICE) plots complement Partial Dependence Plots (PDP) by showing the "
                 "relationship between a feature and the model's output for each individual instance in the dataset. ICE lines (blue) "
                 "can be overlaid on PDPs (red) to provide a more detailed view of how the model behaves for specific instances. "
@@ -1303,15 +1375,16 @@
                 "between the feature and the model's output for individual instances. This may suggest interactions between the feature "
                 "of interest and other features.\n"
                 "* **Outliers**: Look for any ICE lines that are very different from the majority of the lines. This may indicate potential "
                 "outliers or instances that have unique relationships with the feature of interest.\n"
                 "* **Confidence** intervals: If available, examine the confidence intervals around the PDP line. Wider intervals may indicate "
                 "a less certain relationship between the feature and the model's output, while narrower intervals suggest a more robust relationship.\n"
                 "* **Interactions**: By comparing PDPs and ICE plots for different features, you may detect potential interactions between features. "
-                "If the ICE lines change significantly when comparing two features, this might suggest an interaction effect.",
+                "If the ICE lines change significantly when comparing two features, this might suggest an interaction effect.\n\n"
+                "<sub><sup>Use `show_help_text=False` to hide this information when calling this function.</sup></sub>",
                 condition_fn=lambda _: show_help_text and not two_way,
             ),
             PDPInteractions(features=features, two_way=two_way, fig_args=fig_args, sample=max_ice_lines, target=target, **chart_args),  # type: ignore
             MarkdownSectionComponent(
                 f"The following variable(s) are categorical: {cats}. They are represented as the numbers in the figures above. "
                 f"Mappings are available in `state.pdp_id_to_category_mappings`. The`state` can be returned from this call via adding `return_state=True`.",
                 condition_fn=lambda _: len(id_to_category_mappings) > 0,
@@ -1380,7 +1453,254 @@
                 k: {i: v for i, v in enumerate(v.tolist())} for k, v in gen.category_map.items()
             }
 
     if features is not None:
         id_to_category_mappings = {k: v for k, v in id_to_category_mappings.items() if k in features}
 
     return pdp_data, state, id_to_category_mappings  # type: ignore
+
+
+def detect_anomalies(
+    train_data: pd.DataFrame,
+    label: str,
+    test_data: Optional[pd.DataFrame] = None,
+    val_data: Optional[pd.DataFrame] = None,
+    explain_top_n_anomalies: Optional[int] = None,
+    show_top_n_anomalies: Optional[int] = 10,
+    threshold_stds: float = 3,
+    show_help_text: bool = True,
+    state: Union[None, dict, AnalysisState] = None,
+    sample: Union[None, int, float] = DEFAULT_SAMPLE_SIZE,
+    return_state: bool = False,
+    fig_args: Optional[Dict[str, Any]] = None,
+    chart_args: Optional[Dict[str, Any]] = None,
+    **anomaly_detector_kwargs,
+) -> Optional[AnalysisState]:
+    """
+    Anomaly Detection
+
+    This method is used to identify unusual patterns or behaviors in data that deviate significantly from the norm.
+    It's best used when finding outliers, rare events, or suspicious activities that could indicate fraud, defects, or system failures.
+
+    When interpreting anomaly scores, consider:
+
+    - `Threshold`:
+        Determine a suitable threshold to separate normal from anomalous data points, based on domain knowledge or statistical methods.
+    - `Context`:
+        Examine the context of anomalies, including time, location, and surrounding data points, to identify possible causes.
+    - `False positives/negatives`:
+        Be aware of the trade-offs between false positives (normal points classified as anomalies) and false negatives (anomalies missed).
+    - `Feature relevance`:
+        Ensure the features used for anomaly detection are relevant and contribute to the model's performance.
+    - `Model performance`:
+        Regularly evaluate and update the model to maintain its accuracy and effectiveness.
+
+    It's important to understand the context and domain knowledge before deciding on an appropriate approach to deal with anomalies.
+    The choice of method depends on the data's nature, the cause of anomalies, and the problem being addressed.
+    The common ways to deal with anomalies:
+
+    - `Removal`:
+        If an anomaly is a result of an error, noise, or irrelevance to the analysis, it can be removed from the dataset
+        to prevent it from affecting the model's performance.
+    - `Imputation`:
+        Replace anomalous values with appropriate substitutes, such as the mean, median, or mode of the feature,
+        or by using more advanced techniques like regression or k-nearest neighbors.
+    - `Transformation`:
+        Apply transformations like log, square root, or z-score to normalize the data and reduce the impact of extreme values.
+        Absolute dates might be transformed into relative features like age of the item.
+    - `Capping`:
+        Set upper and lower bounds for a feature, and replace values outside these limits with the bounds themselves.
+        This method is also known as winsorizing.
+    - `Separate modeling`:
+        Treat anomalies as a distinct group and build a separate model for them, or use specialized algorithms designed
+        for handling outliers, such as robust regression or one-class SVM.
+    - `Incorporate as a feature`:
+        Create a new binary feature indicating the presence of an anomaly, which can be useful if anomalies have predictive value.
+
+    State attributes
+
+    - `anomaly_detection.scores.<dataset>`
+        scores for each of the datasets passed into analysis (i.e. `train_data`, `test_data`)
+    - `state.anomaly_detection.anomalies.<dataset>`
+        data points considered as anomalies - original rows with added `score` column sorted in descending score order.
+        defined by `threshold_stds` parameter
+    - `anomaly_detection.anomaly_score_threshold`
+        anomaly score threshold above which data points are considered as anomalies;
+        defined by `threshold_stds` parameter
+
+    Parameters
+    ----------
+    train_data: DataFrame
+        training dataset
+    label: str
+        target variable
+    test_data: Optional[pd.DataFrame], default = None
+        test dataset
+    val_data: Optional[pd.DataFrame], default = None
+        validation dataset
+    explain_top_n_anomalies: Optional[int], default = None
+        explain the anomaly scores for n rows with the highest scores; don't perform analysis if value is `None` or `0`
+    show_top_n_anomalies: Optional[int], default = 10
+        display n rows with highest anomaly scores
+    threshold_stds: float, default = 3
+        specifies how many standard deviations above mean anomaly score considered as anomalies
+        (only needed for visualization, does not affect scores calculation)
+    show_help_text:bool, default = True
+        if `True` shows additional information how to interpret the data
+    state: Union[None, dict, AnalysisState], default = None
+        pass prior state if necessary; the object will be updated during `anlz_facets` `fit` call.
+    sample: Union[None, int, float], default = 10000
+        sample size; if `int`, then row number is used;
+        `float` must be between 0.0 and 1.0 and represents fraction of dataset to sample;
+        `None` means no sampling
+        See also :func:`autogluon.eda.analysis.dataset.Sampler`
+    return_state: bool, default = False
+        return state if `True`
+    fig_args: Optional[Dict[str, Any]], default = None,
+        kwargs to pass into visualization component
+    chart_args: Optional[dict], default = None
+        kwargs to pass into visualization component
+    anomaly_detector_kwargs
+        kwargs to pass into :py:class:`~autogluon.eda.analysis.anomaly.AnomalyDetectorAnalysis`
+
+    >>> import autogluon.eda.auto as auto
+    >>>
+    >>> state = auto.detect_anomalies(
+    >>>     train_data=...,
+    >>>     test_data=...,  # optional
+    >>>     label=...,
+    >>>     threshold_stds=3,
+    >>>     show_top_n_anomalies=5,
+    >>>     explain_top_n_anomalies=3,
+    >>>     return_state=True,
+    >>>     chart_args={
+    >>>         'normal.color': 'lightgrey',
+    >>>         'anomaly.color': 'orange',
+    >>>     }
+    >>> )
+    >>>
+    >>> # Getting anomaly scores from the analysis
+    >>> train_anomaly_scores = state.anomaly_detection.scores.train_data
+    >>> test_anomaly_scores = state.anomaly_detection.scores.test_data
+    >>>
+    >>> # Anomaly score threshold for specified level - see `threshold_stds` parameter
+    >>> anomaly_score_threshold = state.anomaly_detection.anomaly_score_threshold
+
+    Returns
+    -------
+    state after `fit` call if `return_state` is `True`; `None` otherwise
+
+    See Also
+    --------
+    :py:class:`~autogluon.eda.analysis.anomaly.AnomalyDetectorAnalysis`
+    :py:class:`~autogluon.eda.visualization.anomaly.AnomalyScoresVisualization`
+    """
+    fig_args_defaults = {"figsize": (12, 6)}
+    fig_args = {**fig_args_defaults, **get_empty_dict_if_none(fig_args).copy()}
+
+    chart_args = get_empty_dict_if_none(chart_args).copy()
+
+    store_explainability_data = (explain_top_n_anomalies is not None) and explain_top_n_anomalies > 0
+    _state: AnalysisState = analyze(  # type: ignore[assignment]  # always has value: return_state=True
+        train_data=train_data,
+        test_data=test_data,
+        val_data=val_data,
+        label=label,
+        state=state,
+        sample=sample,
+        return_state=True,
+        anlz_facets=[
+            ProblemTypeControl(),
+            ApplyFeatureGenerator(
+                category_to_numbers=True,
+                children=[
+                    AnomalyDetectorAnalysis(
+                        store_explainability_data=store_explainability_data, **anomaly_detector_kwargs
+                    ),
+                ],
+            ),
+        ],
+    )
+
+    analyze(
+        state=_state,
+        viz_facets=[
+            MarkdownSectionComponent("### Anomaly Detection Report"),
+            MarkdownSectionComponent(
+                "When interpreting anomaly scores, consider:\n"
+                "* **Threshold**: Determine a suitable threshold to separate normal from anomalous data points, "
+                "    based on domain knowledge or statistical methods.\n"
+                "* **Context**: Examine the context of anomalies, including time, location, and surrounding data points, to identify possible causes.\n"
+                "* **False positives/negatives**: Be aware of the trade-offs between false positives (normal points classified as anomalies) "
+                "    and false negatives (anomalies missed).\n"
+                "* **Feature relevance**: Ensure the features used for anomaly detection are relevant and contribute to the model's performance.\n"
+                "* **Model performance**: Regularly evaluate and update the model to maintain its accuracy and effectiveness.\n\n"
+                "It's important to understand the context and domain knowledge before deciding on an appropriate approach to deal with anomalies."
+                "he choice of method depends on the data's nature, the cause of anomalies, and the problem being addressed."
+                "he common ways to deal with anomalies:\n\n"
+                "* **Removal**: If an anomaly is a result of an error, noise, or irrelevance to the analysis, it can be removed from the dataset "
+                "    to prevent it from affecting the model's performance.\n"
+                "* **Imputation**: Replace anomalous values with appropriate substitutes, such as the mean, median, or mode of the feature,"
+                "    or by using more advanced techniques like regression or k-nearest neighbors.\n"
+                "* **Transformation**: Apply transformations like log, square root, or z-score to normalize the data and reduce the impact of extreme values.\n"
+                "    Absolute dates might be transformed into relative features like age of the item."
+                "* **Capping**: Set upper and lower bounds for a feature, and replace values outside these limits with the bounds themselves."
+                "    This method is also known as winsorizing.\n"
+                "* **Separate modeling**: Treat anomalies as a distinct group and build a separate model for them, or use specialized algorithms designed"
+                "    for handling outliers, such as robust regression or one-class SVM.\n"
+                "* **Incorporate as a feature**: Create a new binary feature indicating the presence of an anomaly, "
+                "    which can be useful if anomalies have predictive value.\n\n"
+                "<sub><sup>Use `show_help_text=False` to hide this information when calling this function.</sup></sub>",
+                condition_fn=lambda _: show_help_text,
+            ),
+            AnomalyScoresVisualization(threshold_stds=threshold_stds, headers=True, fig_args=fig_args, **chart_args),
+        ],
+    )
+
+    # Store anomalies with the scores into the state
+    _state.anomaly_detection.anomalies = {}
+    anomaly_score_threshold = _state.anomaly_detection.scores.train_data.std() * threshold_stds
+    _state.anomaly_detection.anomaly_score_threshold = anomaly_score_threshold
+    for ds, df in AbstractAnalysis.available_datasets(
+        AnalysisState({"train_data": train_data, "test_data": test_data, "val_data": val_data})
+    ):
+        anomaly_scores = _state.anomaly_detection.scores[ds]
+        anomaly_idx = anomaly_scores[anomaly_scores >= anomaly_score_threshold].sort_values(ascending=False).index
+        _state.anomaly_detection.anomalies[ds] = df.iloc[anomaly_idx].join(anomaly_scores)
+
+        if (show_top_n_anomalies is not None) and (show_top_n_anomalies > 0) and (len(anomaly_idx) > 0):
+            analyze(
+                state=_state,
+                viz_facets=[
+                    MarkdownSectionComponent(
+                        markdown=f"**Top-{show_top_n_anomalies} `{ds}` anomalies (total: {len(anomaly_idx)})**"
+                    ),
+                    PropertyRendererComponent(
+                        f"anomaly_detection.anomalies.{ds}", transform_fn=(lambda d: d.head(show_top_n_anomalies))
+                    ),
+                ],
+            )
+
+        if store_explainability_data:
+            analyze(
+                state=_state,
+                viz_facets=[
+                    MarkdownSectionComponent(
+                        markdown="⚠️ Please note that the feature values shown on the charts below are transformed "
+                        "into an internal representation; they may be encoded or modified based on internal preprocessing. "
+                        "Refer to the original datasets for the actual feature values."
+                    ),
+                    MarkdownSectionComponent(
+                        markdown="⚠️ The detector has seen this dataset; the may result in overly optimistic estimates. "
+                        "Although the anomaly score in the explanation might not match, the magnitude of the feature scores "
+                        "can still be utilized to evaluate the impact of the feature on the anomaly score.",
+                        condition_fn=(lambda _: ds == "train_data"),  # noqa: B023
+                    ),
+                ],
+            )
+
+            explain_rows(
+                **_state.anomaly_detection.explain_rows_fns[ds](anomaly_idx[:explain_top_n_anomalies]),
+                plot="waterfall",
+            )
+
+    return _state if return_state else None
```

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/state.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/state.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
-__all__ = ["AnalysisState", "StateCheckMixin", "is_key_present_in_state", "expand_nested_args_into_nested_maps"]
+__all__ = ["AnalysisState", "StateCheckMixin", "is_key_present_in_state"]
 
-from typing import Any, Dict
+from typing import Any
 
 
 class AnalysisState(dict):
     """Enabling dot.notation access to dictionary attributes and dynamic code assist in jupyter"""
 
     _getattr__ = dict.get
     __delattr__ = dict.__delitem__  # type: ignore
@@ -53,15 +53,15 @@
             list of the keys to check
 
         Returns
         -------
             True if at least one key from the `keys` list is present in the state
         """
         for k in keys:
-            if k in state:
+            if state.get(k, None) is not None:
                 return True
         self.logger.warning(f"{self.__class__.__name__}: at least one of the following keys must be present: {keys}")
         return False
 
     def all_keys_must_be_present(self, state: AnalysisState, *keys) -> bool:
         """
         Checks if all the keys are present in the state
@@ -73,15 +73,15 @@
         keys:
             list of the keys to check
 
         Returns
         -------
             True if all the key from the `keys` list are present in the state
         """
-        keys_not_present = [k for k in keys if k not in state.keys()]
+        keys_not_present = [k for k in keys if state.get(k, None) is None]
         can_handle = len(keys_not_present) == 0
         if not can_handle:
             self.logger.warning(
                 f'{self.__class__.__name__}: all of the following keys must be present: [{", ".join(keys)}]. '
                 f'The following keys are missing: [{", ".join(keys_not_present)}]'
             )
         return can_handle
@@ -105,36 +105,7 @@
     """
     path = state
     for p in key.split("."):
         if p not in path:
             return False
         path = path[p]
     return True
-
-
-def expand_nested_args_into_nested_maps(args: Dict[str, Any]) -> Dict[str, Any]:
-    """
-    Expands flat args with nested keys in dot notation into nested map (`{a.b.c: value} -> {'a': {'b': {'c': value}}}`)
-
-    Parameters
-    ----------
-    args: Dict[str, Any]
-        args to expand
-
-    Returns
-    -------
-    nested expanded map
-
-    """
-    result: Dict[str, Any] = {}
-    for k, v in args.items():
-        sub_keys = k.split(".")
-        curr_pointer = result
-        if len(sub_keys) > 1:
-            for subkey in sub_keys[:-1]:
-                if subkey not in curr_pointer:
-                    curr_pointer[subkey] = {}
-                curr_pointer = curr_pointer[subkey]
-        if type(curr_pointer) is not dict:
-            raise ValueError(f"{k} canot be added - the key is already present")
-        curr_pointer[sub_keys[-1]] = v
-    return result
```

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/utils/defaults.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/__init__.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from yellowbrick.style.rcmod import reset_orig
 
+from .anomaly import AnomalyScoresVisualization
 from .dataset import DatasetStatistics, DatasetTypeMismatch, LabelInsightsVisualization
 from .explain import ExplainForcePlot, ExplainWaterfallPlot
 from .interaction import (
     CorrelationSignificanceVisualization,
     CorrelationVisualization,
     FeatureDistanceAnalysisVisualization,
     FeatureInteractionVisualization,
```

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/base.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/dataset.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/explain.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/interaction.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/interaction.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/jupyter.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/jupyter.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/layouts.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/layouts.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/missing.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/model.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon/eda/visualization/shift.py` & `autogluon.eda-0.7.0b20230414/src/autogluon/eda/visualization/shift.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/PKG-INFO` & `autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.7.0b20230413
+Version: 0.7.0b20230414
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.eda-0.7.0b20230413/src/autogluon.eda.egg-info/SOURCES.txt` & `autogluon.eda-0.7.0b20230414/src/autogluon.eda.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 src/autogluon.eda.egg-info/requires.txt
 src/autogluon.eda.egg-info/top_level.txt
 src/autogluon.eda.egg-info/zip-safe
 src/autogluon/eda/__init__.py
 src/autogluon/eda/state.py
 src/autogluon/eda/version.py
 src/autogluon/eda/analysis/__init__.py
+src/autogluon/eda/analysis/anomaly.py
 src/autogluon/eda/analysis/base.py
 src/autogluon/eda/analysis/dataset.py
 src/autogluon/eda/analysis/explain.py
 src/autogluon/eda/analysis/interaction.py
 src/autogluon/eda/analysis/missing.py
 src/autogluon/eda/analysis/model.py
 src/autogluon/eda/analysis/shift.py
 src/autogluon/eda/analysis/transform.py
 src/autogluon/eda/auto/__init__.py
 src/autogluon/eda/auto/simple.py
 src/autogluon/eda/utils/__init__.py
+src/autogluon/eda/utils/common.py
 src/autogluon/eda/utils/defaults.py
 src/autogluon/eda/visualization/__init__.py
+src/autogluon/eda/visualization/anomaly.py
 src/autogluon/eda/visualization/base.py
 src/autogluon/eda/visualization/dataset.py
 src/autogluon/eda/visualization/explain.py
 src/autogluon/eda/visualization/interaction.py
 src/autogluon/eda/visualization/jupyter.py
 src/autogluon/eda/visualization/layouts.py
 src/autogluon/eda/visualization/missing.py
```

