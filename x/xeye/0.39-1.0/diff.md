# Comparing `tmp/xeye-0.39.tar.gz` & `tmp/xeye-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeye-0.39.tar", last modified: Wed Apr 12 21:32:16 2023, max compression
+gzip compressed data, was "xeye-1.0.tar", last modified: Fri Apr 14 23:06:36 2023, max compression
```

## Comparing `xeye-0.39.tar` & `xeye-1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-12 21:32:16.614309 xeye-0.39/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-0.39/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    16104 2023-04-12 21:32:16.613751 xeye-0.39/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14349 2023-04-12 21:11:08.000000 xeye-0.39/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      704 2023-04-12 21:30:21.000000 xeye-0.39/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-12 21:32:16.614445 xeye-0.39/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-12 21:32:16.611145 xeye-0.39/xeye/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      268 2023-04-12 21:30:16.000000 xeye-0.39/xeye/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5924 2023-04-11 10:09:31.000000 xeye-0.39/xeye/build_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14901 2023-04-11 16:04:14.000000 xeye-0.39/xeye/dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14881 2023-04-11 09:14:50.000000 xeye-0.39/xeye/fast_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4518 2023-04-11 09:52:09.000000 xeye-0.39/xeye/manual_dataset.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-12 21:32:16.613082 xeye-0.39/xeye.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    16104 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      270 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-04-12 21:32:16.000000 xeye-0.39/xeye.egg-info/top_level.txt
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-14 23:06:36.567728 xeye-1.0/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-1.0/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    16247 2023-04-14 23:06:36.567330 xeye-1.0/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14492 2023-04-13 21:06:25.000000 xeye-1.0/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      703 2023-04-14 23:05:00.000000 xeye-1.0/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-14 23:06:36.567820 xeye-1.0/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-14 23:06:36.565330 xeye-1.0/xeye/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      267 2023-04-14 23:04:52.000000 xeye-1.0/xeye/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5924 2023-04-11 10:09:31.000000 xeye-1.0/xeye/build_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14901 2023-04-11 16:04:14.000000 xeye-1.0/xeye/dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14881 2023-04-11 09:14:50.000000 xeye-1.0/xeye/fast_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4518 2023-04-11 09:52:09.000000 xeye-1.0/xeye/manual_dataset.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-14 23:06:36.566866 xeye-1.0/xeye.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    16247 2023-04-14 23:06:36.000000 xeye-1.0/xeye.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      270 2023-04-14 23:06:36.000000 xeye-1.0/xeye.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-14 23:06:36.000000 xeye-1.0/xeye.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-04-14 23:06:36.000000 xeye-1.0/xeye.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-04-14 23:06:36.000000 xeye-1.0/xeye.egg-info/top_level.txt
```

### Comparing `xeye-0.39/LICENSE` & `xeye-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xeye-0.39/PKG-INFO` & `xeye-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.39
+Version: 1.0
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -29,15 +29,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  
 # Xeye
-[![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://xeye.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
 
 - [Xeye](#xeye)
   - [Installation](#installation)
   - [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
   - [Xeye functionalities](#xeye-functionalities)
   - [Create a dataset with full terminal UI (Dataset)](#create-a-dataset-with-full-terminal-ui-dataset)
     - [Other useful methods](#other-useful-methods)
@@ -379,9 +379,7 @@
 * **label**: List of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
 * **size**: Tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
 * **color**: Defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
 * **split**: Defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
 * **perc**: Defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
 
 When you want to use the **BuildDataset** class, you need to have .npz files containing images with the same types of colour spaces (all grayscale images or RGB).
-
-
```

### Comparing `xeye-0.39/README.md` & `xeye-1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
  
 # Xeye
-[![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://xeye.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
 
 - [Xeye](#xeye)
   - [Installation](#installation)
   - [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
   - [Xeye functionalities](#xeye-functionalities)
   - [Create a dataset with full terminal UI (Dataset)](#create-a-dataset-with-full-terminal-ui-dataset)
     - [Other useful methods](#other-useful-methods)
@@ -345,10 +345,8 @@
 * **path**: List of files (.npz) path you want to include in the new dataset
 * **label**: List of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
 * **size**: Tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
 * **color**: Defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
 * **split**: Defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
 * **perc**: Defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
 
-When you want to use the **BuildDataset** class, you need to have .npz files containing images with the same types of colour spaces (all grayscale images or RGB).
-
-
+When you want to use the **BuildDataset** class, you need to have .npz files containing images with the same types of colour spaces (all grayscale images or RGB).
```

### Comparing `xeye-0.39/pyproject.toml` & `xeye-1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xeye"
-version = "0.39"
+version = "1.0"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Create datasets for computer vision applications"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `xeye-0.39/xeye/build_dataset.py` & `xeye-1.0/xeye/build_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.39/xeye/dataset.py` & `xeye-1.0/xeye/dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.39/xeye/fast_dataset.py` & `xeye-1.0/xeye/fast_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.39/xeye/manual_dataset.py` & `xeye-1.0/xeye/manual_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.39/xeye.egg-info/PKG-INFO` & `xeye-1.0/xeye.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.39
+Version: 1.0
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -29,15 +29,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
  
 # Xeye
-[![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://xeye.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/xeye.svg)](https://badge.fury.io/py/xeye) ![PyPI - Downloads](https://img.shields.io/pypi/dm/xeye) 
 
 - [Xeye](#xeye)
   - [Installation](#installation)
   - [Xeye datasets for deep learning](#xeye-datasets-for-deep-learning)
   - [Xeye functionalities](#xeye-functionalities)
   - [Create a dataset with full terminal UI (Dataset)](#create-a-dataset-with-full-terminal-ui-dataset)
     - [Other useful methods](#other-useful-methods)
@@ -379,9 +379,7 @@
 * **label**: List of ordinal integer values representing the class type of the images inside a .npz file contained in the new dataset. In the example script, the first .npz file images are associated with class 0, while the second .npz file images are associated with class 1. Remember: always start with 0.
 * **size**: Tuple (height, width) for the images in the new dataset created. The default value (None) indicates that new images have the maximum height and width found in the datasets listed as dimensions
 * **color**: Defines if the images contained in the .npz files are RGB or grayscale. A boolean value, by default, is set to True (meaning RGB images).
 * **split**: Defines if you want to build a dataset split in train-test or not. A boolean value, by default, is set to True.
 * **perc**: Defines the percentage of images assigned to the test dataset. A floating value between (0,1). It's set to 0.1 by default.
 
 When you want to use the **BuildDataset** class, you need to have .npz files containing images with the same types of colour spaces (all grayscale images or RGB).
-
-
```

