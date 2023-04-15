# Comparing `tmp/scenedataset-1.0.0.tar.gz` & `tmp/scenedataset-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenedataset-1.0.0.tar", max compression
+gzip compressed data, was "scenedataset-1.0.1.tar", max compression
```

## Comparing `scenedataset-1.0.0.tar` & `scenedataset-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1516 2023-01-29 13:19:37.916816 scenedataset-1.0.0/LICENSE
--rw-r--r--   0        0        0     5392 2023-04-15 11:38:36.586969 scenedataset-1.0.0/README.md
--rw-r--r--   0        0        0      960 2023-04-15 11:40:13.812470 scenedataset-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-15 10:51:30.229547 scenedataset-1.0.0/src/scenedataset/__init__.py
--rw-r--r--   0        0        0    24564 2023-03-02 20:20:56.608344 scenedataset-1.0.0/src/scenedataset/scenedataset.py
--rw-r--r--   0        0        0      638 2023-03-01 15:26:58.069641 scenedataset-1.0.0/src/scenedataset/utils.py
--rw-r--r--   0        0        0     6460 1970-01-01 00:00:00.000000 scenedataset-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1516 2023-01-29 13:19:37.916816 scenedataset-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5392 2023-04-15 11:38:36.586969 scenedataset-1.0.1/README.md
+-rw-r--r--   0        0        0     1032 2023-04-15 11:50:50.322257 scenedataset-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-15 10:51:30.229547 scenedataset-1.0.1/src/scenedataset/__init__.py
+-rw-r--r--   0        0        0    24564 2023-03-02 20:20:56.608344 scenedataset-1.0.1/src/scenedataset/scenedataset.py
+-rw-r--r--   0        0        0      638 2023-03-01 15:26:58.069641 scenedataset-1.0.1/src/scenedataset/utils.py
+-rw-r--r--   0        0        0     6460 1970-01-01 00:00:00.000000 scenedataset-1.0.1/PKG-INFO
```

### Comparing `scenedataset-1.0.0/LICENSE` & `scenedataset-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scenedataset-1.0.0/README.md` & `scenedataset-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `scenedataset-1.0.0/pyproject.toml` & `scenedataset-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "scenedataset"
-version = "1.0.0"
+version = "1.0.1"
 description = "PyTorch dataset which uses PySceneDetect to split videos into scenes"
 authors = ["Farid Abdalla"]
 license = "BSD 3-Clause"
 readme = "README.md"
 
+[project.urls]
+"Homepage" = "https://github.com/Kurokabe/SceneDataset"
+
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 decord = ">=0.6.0"
 loguru = ">=0.6.0"
 scenedetect = ">=0.6.1"
 torch = ">=1.13.1"
 opencv-python = ">=4.7.0.68"
```

### Comparing `scenedataset-1.0.0/src/scenedataset/scenedataset.py` & `scenedataset-1.0.1/src/scenedataset/scenedataset.py`

 * *Files identical despite different names*

### Comparing `scenedataset-1.0.0/src/scenedataset/utils.py` & `scenedataset-1.0.1/src/scenedataset/utils.py`

 * *Files identical despite different names*

### Comparing `scenedataset-1.0.0/PKG-INFO` & `scenedataset-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenedataset
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyTorch dataset which uses PySceneDetect to split videos into scenes
 License: BSD 3-Clause
 Author: Farid Abdalla
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

