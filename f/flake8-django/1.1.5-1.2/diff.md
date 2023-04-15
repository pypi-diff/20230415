# Comparing `tmp/flake8-django-1.1.5.tar.gz` & `tmp/flake8_django-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-django-1.1.5.tar", max compression
+gzip compressed data, was "flake8_django-1.2.tar", max compression
```

## Comparing `flake8-django-1.1.5.tar` & `flake8_django-1.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     3393 2022-08-10 20:12:15.744827 flake8-django-1.1.5/README.md
--rw-r--r--   0        0        0       67 2022-08-10 20:12:15.744919 flake8-django-1.1.5/flake8_django/__init__.py
--rw-r--r--   0        0        0     2020 2022-08-10 20:12:15.744991 flake8-django-1.1.5/flake8_django/checker.py
--rw-r--r--   0        0        0      501 2022-08-10 20:12:15.745093 flake8-django-1.1.5/flake8_django/checkers/__init__.py
--rw-r--r--   0        0        0     1680 2022-08-10 20:12:15.745168 flake8-django-1.1.5/flake8_django/checkers/base_model_checker.py
--rw-r--r--   0        0        0      528 2022-08-10 20:12:15.745233 flake8-django-1.1.5/flake8_django/checkers/checker.py
--rw-r--r--   0        0        0      828 2022-08-10 20:12:15.745299 flake8-django-1.1.5/flake8_django/checkers/decorator.py
--rw-r--r--   0        0        0      504 2022-08-10 20:12:15.745364 flake8-django-1.1.5/flake8_django/checkers/issue.py
--rw-r--r--   0        0        0     3888 2022-08-10 20:12:15.745445 flake8-django-1.1.5/flake8_django/checkers/model_content_order.py
--rw-r--r--   0        0        0     1023 2022-08-10 20:12:15.745514 flake8-django-1.1.5/flake8_django/checkers/model_dunder_str.py
--rw-r--r--   0        0        0     1438 2022-08-10 20:12:15.745587 flake8-django-1.1.5/flake8_django/checkers/model_fields.py
--rw-r--r--   0        0        0     2134 2022-08-10 20:12:15.745661 flake8-django-1.1.5/flake8_django/checkers/model_form.py
--rw-r--r--   0        0        0     2378 2022-08-10 20:12:15.745725 flake8-django-1.1.5/flake8_django/checkers/model_meta.py
--rw-r--r--   0        0        0      731 2022-08-10 20:12:15.745787 flake8-django-1.1.5/flake8_django/checkers/render.py
--rw-r--r--   0        0        0      907 2022-08-10 20:12:15.746065 flake8-django-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     4309 2022-08-10 20:13:27.906842 flake8-django-1.1.5/setup.py
--rw-r--r--   0        0        0     4421 2022-08-10 20:13:27.907056 flake8-django-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3393 2022-08-10 20:12:15.744827 flake8_django-1.2/README.md
+-rw-r--r--   0        0        0       67 2022-08-10 20:12:15.744919 flake8_django-1.2/flake8_django/__init__.py
+-rw-r--r--   0        0        0     2020 2022-08-10 20:12:15.744991 flake8_django-1.2/flake8_django/checker.py
+-rw-r--r--   0        0        0      501 2022-08-10 20:12:15.745093 flake8_django-1.2/flake8_django/checkers/__init__.py
+-rw-r--r--   0        0        0     1680 2022-08-10 20:12:15.745168 flake8_django-1.2/flake8_django/checkers/base_model_checker.py
+-rw-r--r--   0        0        0      528 2022-08-10 20:12:15.745233 flake8_django-1.2/flake8_django/checkers/checker.py
+-rw-r--r--   0        0        0      828 2022-08-10 20:12:15.745299 flake8_django-1.2/flake8_django/checkers/decorator.py
+-rw-r--r--   0        0        0      504 2022-08-10 20:12:15.745364 flake8_django-1.2/flake8_django/checkers/issue.py
+-rw-r--r--   0        0        0     3888 2022-08-10 20:12:15.745445 flake8_django-1.2/flake8_django/checkers/model_content_order.py
+-rw-r--r--   0        0        0     1023 2022-08-10 20:12:15.745514 flake8_django-1.2/flake8_django/checkers/model_dunder_str.py
+-rw-r--r--   0        0        0     1438 2022-08-10 20:12:15.745587 flake8_django-1.2/flake8_django/checkers/model_fields.py
+-rw-r--r--   0        0        0     2134 2022-08-10 20:12:15.745661 flake8_django-1.2/flake8_django/checkers/model_form.py
+-rw-r--r--   0        0        0     2378 2022-08-10 20:12:15.745725 flake8_django-1.2/flake8_django/checkers/model_meta.py
+-rw-r--r--   0        0        0      731 2022-08-10 20:12:15.745787 flake8_django-1.2/flake8_django/checkers/render.py
+-rw-r--r--   0        0        0      941 2023-04-15 10:01:06.825521 flake8_django-1.2/pyproject.toml
+-rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 flake8_django-1.2/PKG-INFO
```

### Comparing `flake8-django-1.1.5/README.md` & `flake8_django-1.2/README.md`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checker.py` & `flake8_django-1.2/flake8_django/checker.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/base_model_checker.py` & `flake8_django-1.2/flake8_django/checkers/base_model_checker.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/checker.py` & `flake8_django-1.2/flake8_django/checkers/checker.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/decorator.py` & `flake8_django-1.2/flake8_django/checkers/decorator.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/model_content_order.py` & `flake8_django-1.2/flake8_django/checkers/model_content_order.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/model_dunder_str.py` & `flake8_django-1.2/flake8_django/checkers/model_dunder_str.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/model_fields.py` & `flake8_django-1.2/flake8_django/checkers/model_fields.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/model_form.py` & `flake8_django-1.2/flake8_django/checkers/model_form.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/model_meta.py` & `flake8_django-1.2/flake8_django/checkers/model_meta.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/flake8_django/checkers/render.py` & `flake8_django-1.2/flake8_django/checkers/render.py`

 * *Files identical despite different names*

### Comparing `flake8-django-1.1.5/pyproject.toml` & `flake8_django-1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "flake8-django"
-version = "1.1.5"
+version = "1.2"
 license = "GPL-3.0-or-later"
 description = "Plugin to catch bad style specific to Django Projects."
 authors = ["Rocio Aramberri Schegel <rocio.aramberri@schegel.net>"]
 readme = "README.md"
 keywords = ["flake8", "django", "lint"]
 repository = "https://github.com/rocioar/flake8-django"
 classifiers=[
     "Framework :: Flake8",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.plugins]
 [tool.poetry.plugins."flake8.extension"]
 DJ0 = "flake8_django:DjangoStyleChecker"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-flake8 = ">=3.8.4,<6"
+flake8 = ">=3.8.4,<7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 twine = "^4.0.1"
```

### Comparing `flake8-django-1.1.5/PKG-INFO` & `flake8_django-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: flake8-django
-Version: 1.1.5
+Version: 1.2
 Summary: Plugin to catch bad style specific to Django Projects.
 Home-page: https://github.com/rocioar/flake8-django
 License: GPL-3.0-or-later
 Keywords: flake8,django,lint
 Author: Rocio Aramberri Schegel
 Author-email: rocio.aramberri@schegel.net
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Dist: flake8 (>=3.8.4,<6)
+Requires-Dist: flake8 (>=3.8.4,<7)
 Project-URL: Repository, https://github.com/rocioar/flake8-django
 Description-Content-Type: text/markdown
 
 # flake8-django
 
 [![pypi](https://img.shields.io/pypi/v/flake8-django.svg)](https://pypi.python.org/pypi/flake8-django/)
 ![CI](https://github.com/rocioar/flake8-django/workflows/CI/badge.svg)[![Codecov](https://codecov.io/gh/rocioar/flake8-django/branch/master/graph/badge.svg)](https://codecov.io/gh/rocioar/flake8-django)
```

