# Comparing `tmp/ethome-ml-0.5.1.tar.gz` & `tmp/ethome-ml-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethome-ml-0.5.1.tar", last modified: Sat Apr 15 02:40:12 2023, max compression
+gzip compressed data, was "ethome-ml-0.5.2.tar", last modified: Sat Apr 15 02:53:56 2023, max compression
```

## Comparing `ethome-ml-0.5.1.tar` & `ethome-ml-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.751145 ethome-ml-0.5.1/
--rw-r--r--   0 blansdel (66183) domain users (76937)     1069 2022-09-22 06:23:05.000000 ethome-ml-0.5.1/LICENSE
--rw-r--r--   0 blansdel (66183) domain users (76937)      192 2022-09-22 06:23:05.000000 ethome-ml-0.5.1/MANIFEST.in
--rw-r--r--   0 blansdel (66183) domain users (76937)     4232 2023-04-15 02:40:12.751145 ethome-ml-0.5.1/PKG-INFO
--rw-r--r--   0 blansdel (66183) domain users (76937)     3713 2023-04-15 02:39:17.000000 ethome-ml-0.5.1/README.md
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.739144 ethome-ml-0.5.1/ethome/
--rw-r--r--   0 blansdel (66183) domain users (76937)     1220 2023-04-15 02:39:47.000000 ethome-ml-0.5.1/ethome/__init__.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      301 2022-09-22 06:23:05.000000 ethome-ml-0.5.1/ethome/config.py
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.739144 ethome-ml-0.5.1/ethome/data/
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.735144 ethome-ml-0.5.1/ethome/data/dlc/
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.751145 ethome-ml-0.5.1/ethome/data/dlc/openfield/
--rw-r--r--   0 blansdel (66183) domain users (76937)   525609 2022-09-22 06:23:05.000000 ethome-ml-0.5.1/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv
--rw-r--r--   0 blansdel (66183) domain users (76937) 16565151 2022-09-22 06:23:06.000000 ethome-ml-0.5.1/ethome/data/sample_dataframe.pkl
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.739144 ethome-ml-0.5.1/ethome/features/
--rw-r--r--   0 blansdel (66183) domain users (76937)      313 2023-01-13 01:35:12.000000 ethome-ml-0.5.1/ethome/features/__init__.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     8249 2023-02-17 05:56:11.000000 ethome-ml-0.5.1/ethome/features/cnn1d.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    11809 2023-02-17 05:44:55.000000 ethome-ml-0.5.1/ethome/features/dl_features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     6876 2023-01-13 16:33:40.000000 ethome-ml-0.5.1/ethome/features/features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    12688 2022-10-13 05:56:34.000000 ethome-ml-0.5.1/ethome/features/generic_features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    26081 2022-09-25 06:01:10.000000 ethome-ml-0.5.1/ethome/features/mars_features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     2437 2022-09-22 06:23:06.000000 ethome-ml-0.5.1/ethome/interpolation.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    25297 2023-03-17 22:00:55.000000 ethome-ml-0.5.1/ethome/io.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     4110 2022-09-23 05:03:34.000000 ethome-ml-0.5.1/ethome/models.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    17215 2023-03-18 02:35:37.000000 ethome-ml-0.5.1/ethome/plot.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    10903 2023-03-18 02:38:27.000000 ethome-ml-0.5.1/ethome/unsupervised.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      713 2023-02-17 05:36:45.000000 ethome-ml-0.5.1/ethome/utils.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      106 2023-01-13 21:53:31.000000 ethome-ml-0.5.1/ethome/version.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    33534 2023-03-18 14:42:48.000000 ethome-ml-0.5.1/ethome/video.py
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.751145 ethome-ml-0.5.1/ethome_ml.egg-info/
--rw-r--r--   0 blansdel (66183) domain users (76937)     4232 2023-04-15 02:40:12.000000 ethome-ml-0.5.1/ethome_ml.egg-info/PKG-INFO
--rw-r--r--   0 blansdel (66183) domain users (76937)      831 2023-04-15 02:40:12.000000 ethome-ml-0.5.1/ethome_ml.egg-info/SOURCES.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)        1 2023-04-15 02:40:12.000000 ethome-ml-0.5.1/ethome_ml.egg-info/dependency_links.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)       94 2023-04-15 02:40:12.000000 ethome-ml-0.5.1/ethome_ml.egg-info/requires.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)        7 2023-04-15 02:40:12.000000 ethome-ml-0.5.1/ethome_ml.egg-info/top_level.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)      104 2022-09-22 06:23:06.000000 ethome-ml-0.5.1/pyproject.toml
--rw-r--r--   0 blansdel (66183) domain users (76937)      810 2023-04-15 02:40:12.751145 ethome-ml-0.5.1/setup.cfg
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:40:12.751145 ethome-ml-0.5.1/tests/
--rw-r--r--   0 blansdel (66183) domain users (76937)    17953 2023-01-13 15:30:56.000000 ethome-ml-0.5.1/tests/test_analysis.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     5556 2023-04-12 05:01:57.000000 ethome-ml-0.5.1/tests/test_io.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      335 2022-09-29 21:17:44.000000 ethome-ml-0.5.1/tests/test_models.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      515 2023-03-18 02:54:17.000000 ethome-ml-0.5.1/tests/test_plot.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     1973 2023-03-18 02:42:38.000000 ethome-ml-0.5.1/tests/test_unsupervised.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      180 2022-09-22 06:23:06.000000 ethome-ml-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.479857 ethome-ml-0.5.2/
+-rw-r--r--   0 blansdel (66183) domain users (76937)     1069 2022-09-22 06:23:05.000000 ethome-ml-0.5.2/LICENSE
+-rw-r--r--   0 blansdel (66183) domain users (76937)      192 2022-09-22 06:23:05.000000 ethome-ml-0.5.2/MANIFEST.in
+-rw-r--r--   0 blansdel (66183) domain users (76937)     4475 2023-04-15 02:53:56.479857 ethome-ml-0.5.2/PKG-INFO
+-rw-r--r--   0 blansdel (66183) domain users (76937)     3956 2023-04-15 02:52:46.000000 ethome-ml-0.5.2/README.md
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.467857 ethome-ml-0.5.2/ethome/
+-rw-r--r--   0 blansdel (66183) domain users (76937)     1220 2023-04-15 02:53:37.000000 ethome-ml-0.5.2/ethome/__init__.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      301 2022-09-22 06:23:05.000000 ethome-ml-0.5.2/ethome/config.py
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.467857 ethome-ml-0.5.2/ethome/data/
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.463857 ethome-ml-0.5.2/ethome/data/dlc/
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.479857 ethome-ml-0.5.2/ethome/data/dlc/openfield/
+-rw-r--r--   0 blansdel (66183) domain users (76937)   525609 2022-09-22 06:23:05.000000 ethome-ml-0.5.2/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv
+-rw-r--r--   0 blansdel (66183) domain users (76937) 16565151 2022-09-22 06:23:06.000000 ethome-ml-0.5.2/ethome/data/sample_dataframe.pkl
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.467857 ethome-ml-0.5.2/ethome/features/
+-rw-r--r--   0 blansdel (66183) domain users (76937)      313 2023-01-13 01:35:12.000000 ethome-ml-0.5.2/ethome/features/__init__.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     8249 2023-02-17 05:56:11.000000 ethome-ml-0.5.2/ethome/features/cnn1d.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    11809 2023-02-17 05:44:55.000000 ethome-ml-0.5.2/ethome/features/dl_features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     6876 2023-01-13 16:33:40.000000 ethome-ml-0.5.2/ethome/features/features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    12688 2022-10-13 05:56:34.000000 ethome-ml-0.5.2/ethome/features/generic_features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    26081 2022-09-25 06:01:10.000000 ethome-ml-0.5.2/ethome/features/mars_features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     2437 2022-09-22 06:23:06.000000 ethome-ml-0.5.2/ethome/interpolation.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    25297 2023-03-17 22:00:55.000000 ethome-ml-0.5.2/ethome/io.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     4110 2022-09-23 05:03:34.000000 ethome-ml-0.5.2/ethome/models.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    17215 2023-03-18 02:35:37.000000 ethome-ml-0.5.2/ethome/plot.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    10903 2023-03-18 02:38:27.000000 ethome-ml-0.5.2/ethome/unsupervised.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      713 2023-02-17 05:36:45.000000 ethome-ml-0.5.2/ethome/utils.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      106 2023-01-13 21:53:31.000000 ethome-ml-0.5.2/ethome/version.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    33534 2023-03-18 14:42:48.000000 ethome-ml-0.5.2/ethome/video.py
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.479857 ethome-ml-0.5.2/ethome_ml.egg-info/
+-rw-r--r--   0 blansdel (66183) domain users (76937)     4475 2023-04-15 02:53:56.000000 ethome-ml-0.5.2/ethome_ml.egg-info/PKG-INFO
+-rw-r--r--   0 blansdel (66183) domain users (76937)      831 2023-04-15 02:53:56.000000 ethome-ml-0.5.2/ethome_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)        1 2023-04-15 02:53:56.000000 ethome-ml-0.5.2/ethome_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)       94 2023-04-15 02:53:56.000000 ethome-ml-0.5.2/ethome_ml.egg-info/requires.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)        7 2023-04-15 02:53:56.000000 ethome-ml-0.5.2/ethome_ml.egg-info/top_level.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)      104 2022-09-22 06:23:06.000000 ethome-ml-0.5.2/pyproject.toml
+-rw-r--r--   0 blansdel (66183) domain users (76937)      810 2023-04-15 02:53:56.479857 ethome-ml-0.5.2/setup.cfg
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:53:56.479857 ethome-ml-0.5.2/tests/
+-rw-r--r--   0 blansdel (66183) domain users (76937)    17953 2023-01-13 15:30:56.000000 ethome-ml-0.5.2/tests/test_analysis.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     5556 2023-04-12 05:01:57.000000 ethome-ml-0.5.2/tests/test_io.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      335 2022-09-29 21:17:44.000000 ethome-ml-0.5.2/tests/test_models.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      515 2023-03-18 02:54:17.000000 ethome-ml-0.5.2/tests/test_plot.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     1973 2023-03-18 02:42:38.000000 ethome-ml-0.5.2/tests/test_unsupervised.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      180 2022-09-22 06:23:06.000000 ethome-ml-0.5.2/tests/test_utils.py
```

### Comparing `ethome-ml-0.5.1/LICENSE` & `ethome-ml-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/PKG-INFO` & `ethome-ml-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethome-ml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Machine learning for animal behavior analysis
 Home-page: https://github.com/benlansdell/ethome
 Author: Ben Lansdell
 Author-email: ben.lansdell@gmail.com
 Project-URL: Bug Tracker, https://github.com/benlansdell/ethome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,26 +15,28 @@
 
 [![codecov](https://codecov.io/gh/benlansdell/ethome/branch/master/graph/badge.svg?token=IJ0JJBOGGS)](https://codecov.io/gh/benlansdell/ethome)
 ![build](https://github.com/benlansdell/ethome/actions/workflows/workflow.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ethome-ml.svg)](https://badge.fury.io/py/ethome-ml)
 
 # Ethome
 
-Tools for machine learning of animal behavior.
+Tools for machine learning of animal behavior. 
 
-This library interprets pose-tracking files (at present, from DLC, SLEAP or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
+This library interprets pose-tracking files and behavior annotations to create features, train behavior classifiers, interpolate pose tracking data and other common analysis tasks. 
+
+At present pose tracking data from DLC, SLEAP and NWB formats are supported, and behavior annotations from BORIS and NWB formats are supported.
 
 ## Features
 
 * Read in animal pose data and corresponding behavior annotations to make supervised learning easy
 * Scale data to desired physical units
 * Interpolate pose data to improve low-confidence predictions 
 * Create generic features for analysis and downstream ML tasks
 * Create features specifically for mouse resident-intruder setup
-* Quickly generate a movie with behavior predictions
+* Quickly generate plots and movies with behavior predictions
 
 ## Installation
 
 ```
 pip install ethome-ml
 ```
 
@@ -64,15 +66,19 @@
 
 A key functionality of `ethome` is the ability to easily create features for machine learning. You can use pre-built featuresets or make your own. For instance:
 ```python
 dataset.features.add('distances')
 ``` 
 will compute all distances between all body parts (both between and within animals).
 
-There are also featuresets specifically tailored for social mice studies (resident intruder). For this, you must have labeled your body parts in a certain way (refer to How To). But other, more generic, feature creation functions are provided that work for any animal configuration. 
+There are featuresets specifically tailored for social mice studies (resident intruder). For instance, 
+```
+dataset.features.add('cnn1d_prob')
+```
+Uses a pretrained CNN to output probabilities of 3 behaviors (attack, mount, social investigation). For this, you must have labeled your body parts in a certain way (refer to How To). Other, more generic, feature creation functions are provided that work for any animal configuration. 
 
 Now you can access a features table, labels, and groups for learning with `dataset.ml.features, dataset.ml.labels, dataset.ml.group`. From here it's easy to use some ML libraries to train a behavior classifier. For example:
 ```python
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import cross_val_score, LeaveOneGroupOut
 
 cv = LeaveOneGroupOut()
```

### Comparing `ethome-ml-0.5.1/README.md` & `ethome-ml-0.5.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [![codecov](https://codecov.io/gh/benlansdell/ethome/branch/master/graph/badge.svg?token=IJ0JJBOGGS)](https://codecov.io/gh/benlansdell/ethome)
 ![build](https://github.com/benlansdell/ethome/actions/workflows/workflow.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ethome-ml.svg)](https://badge.fury.io/py/ethome-ml)
 
 # Ethome
 
-Tools for machine learning of animal behavior.
+Tools for machine learning of animal behavior. 
 
-This library interprets pose-tracking files (at present, from DLC, SLEAP or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
+This library interprets pose-tracking files and behavior annotations to create features, train behavior classifiers, interpolate pose tracking data and other common analysis tasks. 
+
+At present pose tracking data from DLC, SLEAP and NWB formats are supported, and behavior annotations from BORIS and NWB formats are supported.
 
 ## Features
 
 * Read in animal pose data and corresponding behavior annotations to make supervised learning easy
 * Scale data to desired physical units
 * Interpolate pose data to improve low-confidence predictions 
 * Create generic features for analysis and downstream ML tasks
 * Create features specifically for mouse resident-intruder setup
-* Quickly generate a movie with behavior predictions
+* Quickly generate plots and movies with behavior predictions
 
 ## Installation
 
 ```
 pip install ethome-ml
 ```
 
@@ -49,15 +51,19 @@
 
 A key functionality of `ethome` is the ability to easily create features for machine learning. You can use pre-built featuresets or make your own. For instance:
 ```python
 dataset.features.add('distances')
 ``` 
 will compute all distances between all body parts (both between and within animals).
 
-There are also featuresets specifically tailored for social mice studies (resident intruder). For this, you must have labeled your body parts in a certain way (refer to How To). But other, more generic, feature creation functions are provided that work for any animal configuration. 
+There are featuresets specifically tailored for social mice studies (resident intruder). For instance, 
+```
+dataset.features.add('cnn1d_prob')
+```
+Uses a pretrained CNN to output probabilities of 3 behaviors (attack, mount, social investigation). For this, you must have labeled your body parts in a certain way (refer to How To). Other, more generic, feature creation functions are provided that work for any animal configuration. 
 
 Now you can access a features table, labels, and groups for learning with `dataset.ml.features, dataset.ml.labels, dataset.ml.group`. From here it's easy to use some ML libraries to train a behavior classifier. For example:
 ```python
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import cross_val_score, LeaveOneGroupOut
 
 cv = LeaveOneGroupOut()
```

### Comparing `ethome-ml-0.5.1/ethome/__init__.py` & `ethome-ml-0.5.2/ethome/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 #Suppress tensorflow import text...
 import os
 from importlib.util import find_spec 
 if find_spec('tensorflow') is not None:
     if 'TF_CPP_MIN_LOG_LEVEL' in os.environ:
         old_val = os.environ['TF_CPP_MIN_LOG_LEVEL']
```

### Comparing `ethome-ml-0.5.1/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv` & `ethome-ml-0.5.2/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/data/sample_dataframe.pkl` & `ethome-ml-0.5.2/ethome/data/sample_dataframe.pkl`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/features/cnn1d.py` & `ethome-ml-0.5.2/ethome/features/cnn1d.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/features/dl_features.py` & `ethome-ml-0.5.2/ethome/features/dl_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/features/features.py` & `ethome-ml-0.5.2/ethome/features/features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/features/generic_features.py` & `ethome-ml-0.5.2/ethome/features/generic_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/features/mars_features.py` & `ethome-ml-0.5.2/ethome/features/mars_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/interpolation.py` & `ethome-ml-0.5.2/ethome/interpolation.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/io.py` & `ethome-ml-0.5.2/ethome/io.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/models.py` & `ethome-ml-0.5.2/ethome/models.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/plot.py` & `ethome-ml-0.5.2/ethome/plot.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/unsupervised.py` & `ethome-ml-0.5.2/ethome/unsupervised.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/utils.py` & `ethome-ml-0.5.2/ethome/utils.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome/video.py` & `ethome-ml-0.5.2/ethome/video.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/ethome_ml.egg-info/PKG-INFO` & `ethome-ml-0.5.2/ethome_ml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethome-ml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Machine learning for animal behavior analysis
 Home-page: https://github.com/benlansdell/ethome
 Author: Ben Lansdell
 Author-email: ben.lansdell@gmail.com
 Project-URL: Bug Tracker, https://github.com/benlansdell/ethome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,26 +15,28 @@
 
 [![codecov](https://codecov.io/gh/benlansdell/ethome/branch/master/graph/badge.svg?token=IJ0JJBOGGS)](https://codecov.io/gh/benlansdell/ethome)
 ![build](https://github.com/benlansdell/ethome/actions/workflows/workflow.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ethome-ml.svg)](https://badge.fury.io/py/ethome-ml)
 
 # Ethome
 
-Tools for machine learning of animal behavior.
+Tools for machine learning of animal behavior. 
 
-This library interprets pose-tracking files (at present, from DLC, SLEAP or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
+This library interprets pose-tracking files and behavior annotations to create features, train behavior classifiers, interpolate pose tracking data and other common analysis tasks. 
+
+At present pose tracking data from DLC, SLEAP and NWB formats are supported, and behavior annotations from BORIS and NWB formats are supported.
 
 ## Features
 
 * Read in animal pose data and corresponding behavior annotations to make supervised learning easy
 * Scale data to desired physical units
 * Interpolate pose data to improve low-confidence predictions 
 * Create generic features for analysis and downstream ML tasks
 * Create features specifically for mouse resident-intruder setup
-* Quickly generate a movie with behavior predictions
+* Quickly generate plots and movies with behavior predictions
 
 ## Installation
 
 ```
 pip install ethome-ml
 ```
 
@@ -64,15 +66,19 @@
 
 A key functionality of `ethome` is the ability to easily create features for machine learning. You can use pre-built featuresets or make your own. For instance:
 ```python
 dataset.features.add('distances')
 ``` 
 will compute all distances between all body parts (both between and within animals).
 
-There are also featuresets specifically tailored for social mice studies (resident intruder). For this, you must have labeled your body parts in a certain way (refer to How To). But other, more generic, feature creation functions are provided that work for any animal configuration. 
+There are featuresets specifically tailored for social mice studies (resident intruder). For instance, 
+```
+dataset.features.add('cnn1d_prob')
+```
+Uses a pretrained CNN to output probabilities of 3 behaviors (attack, mount, social investigation). For this, you must have labeled your body parts in a certain way (refer to How To). Other, more generic, feature creation functions are provided that work for any animal configuration. 
 
 Now you can access a features table, labels, and groups for learning with `dataset.ml.features, dataset.ml.labels, dataset.ml.group`. From here it's easy to use some ML libraries to train a behavior classifier. For example:
 ```python
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import cross_val_score, LeaveOneGroupOut
 
 cv = LeaveOneGroupOut()
```

### Comparing `ethome-ml-0.5.1/ethome_ml.egg-info/SOURCES.txt` & `ethome-ml-0.5.2/ethome_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/setup.cfg` & `ethome-ml-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/tests/test_analysis.py` & `ethome-ml-0.5.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/tests/test_io.py` & `ethome-ml-0.5.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/tests/test_plot.py` & `ethome-ml-0.5.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.1/tests/test_unsupervised.py` & `ethome-ml-0.5.2/tests/test_unsupervised.py`

 * *Files identical despite different names*

