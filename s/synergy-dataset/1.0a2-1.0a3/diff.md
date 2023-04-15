# Comparing `tmp/synergy-dataset-1.0a2.tar.gz` & `tmp/synergy-dataset-1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synergy-dataset-1.0a2.tar", last modified: Sat Apr 15 18:25:27 2023, max compression
+gzip compressed data, was "synergy-dataset-1.0a3.tar", last modified: Sat Apr 15 18:35:15 2023, max compression
```

## Comparing `synergy-dataset-1.0a2.tar` & `synergy-dataset-1.0a3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:25:27.368358 synergy-dataset-1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:25:27.364358 synergy-dataset-1.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:25:27.364358 synergy-dataset-1.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 18:25:27.368358 synergy-dataset-1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:25:27.368358 synergy-dataset-1.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:25:27.364358 synergy-dataset-1.0a2/synergy_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/synergy_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/synergy_dataset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-15 18:25:27.000000 synergy-dataset-1.0a2/synergy_dataset/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/synergy_dataset/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:25:27.368358 synergy-dataset-1.0a2/synergy_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 18:25:27.000000 synergy-dataset-1.0a2/synergy_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-15 18:25:27.000000 synergy-dataset-1.0a2/synergy_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:25:27.000000 synergy-dataset-1.0a2/synergy_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 18:25:27.000000 synergy-dataset-1.0a2/synergy_dataset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-15 18:25:27.000000 synergy-dataset-1.0a2/synergy_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 18:25:27.000000 synergy-dataset-1.0a2/synergy_dataset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:25:27.368358 synergy-dataset-1.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-15 18:25:15.000000 synergy-dataset-1.0a2/tests/test_synergy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/synergy_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/synergy_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/synergy_dataset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-15 18:35:15.000000 synergy-dataset-1.0a3/synergy_dataset/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/synergy_dataset/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/synergy_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 18:35:15.000000 synergy-dataset-1.0a3/synergy_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-15 18:35:15.000000 synergy-dataset-1.0a3/synergy_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:35:15.000000 synergy-dataset-1.0a3/synergy_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 18:35:15.000000 synergy-dataset-1.0a3/synergy_dataset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-15 18:35:15.000000 synergy-dataset-1.0a3/synergy_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 18:35:15.000000 synergy-dataset-1.0a3/synergy_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:35:15.738136 synergy-dataset-1.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-15 18:34:59.000000 synergy-dataset-1.0a3/tests/test_synergy.py
```

### Comparing `synergy-dataset-1.0a2/.github/workflows/python-package.yml` & `synergy-dataset-1.0a3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a2/.github/workflows/python-publish.yml` & `synergy-dataset-1.0a3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a2/.gitignore` & `synergy-dataset-1.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a2/LICENSE` & `synergy-dataset-1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a2/PKG-INFO` & `synergy-dataset-1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a2
+Version: 1.0a3
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `synergy-dataset-1.0a2/README.md` & `synergy-dataset-1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a2/pyproject.toml` & `synergy-dataset-1.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a2/synergy_dataset/__main__.py` & `synergy-dataset-1.0a3/synergy_dataset/__main__.py`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a2/synergy_dataset/base.py` & `synergy-dataset-1.0a3/synergy_dataset/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 def _get_download_url(version=None, source="github"):
 
     if version is None:
         version = SYNERGY_VERSION
 
     if source == "github":
-        github_url = "https://github.com/asreview/systematic-review-datasets/archive/refs/tags/v{}.zip"  # noqa
+        github_url = "https://github.com/asreview/systematic-review-datasets/archive/refs/tags/{}.zip"  # noqa
         return github_url.format(version)
     else:
         raise ValueError("Unknown source")
 
 
 def _dataset_available():
     """Check if the dataset is available
```

### Comparing `synergy-dataset-1.0a2/synergy_dataset.egg-info/PKG-INFO` & `synergy-dataset-1.0a3/synergy_dataset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a2
+Version: 1.0a3
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `synergy-dataset-1.0a2/synergy_dataset.egg-info/SOURCES.txt` & `synergy-dataset-1.0a3/synergy_dataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

