# Comparing `tmp/barbell2_bodycomp-0.3.0.tar.gz` & `tmp/barbell2_bodycomp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbell2_bodycomp-0.3.0.tar", last modified: Thu Apr 13 11:39:22 2023, max compression
+gzip compressed data, was "dist/barbell2_bodycomp-0.4.0.tar", last modified: Sat Apr 15 07:09:24 2023, max compression
```

## Comparing `barbell2_bodycomp-0.3.0.tar` & `barbell2_bodycomp-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.294780 barbell2_bodycomp-0.3.0/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-13 11:39:22.294564 barbell2_bodycomp-0.3.0/PKG-INFO
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.290507 barbell2_bodycomp-0.3.0/barbell2_bodycomp/
--rw-r--r--   0 ralph      (501) staff       (20)      105 2023-04-13 11:39:07.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     4456 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/calculator.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.293900 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/
--rw-r--r--   0 ralph      (501) staff       (20)       55 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2nifti.py
--rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2npy.py
--rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2nrrd.py
--rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2png.py
--rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/tag2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/tag2npy.py
--rw-r--r--   0 ralph      (501) staff       (20)     6046 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/seg.py
--rw-r--r--   0 ralph      (501) staff       (20)     1374 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/selectroi.py
--rw-r--r--   0 ralph      (501) staff       (20)     5788 2023-04-13 11:13:27.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/selectslice.py
--rw-r--r--   0 ralph      (501) staff       (20)     1586 2023-04-13 11:15:28.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/totalseg.py
--rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp/utils.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-13 11:39:22.291948 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      804 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/not-zip-safe
--rw-r--r--   0 ralph      (501) staff       (20)       40 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/requires.txt
--rw-r--r--   0 ralph      (501) staff       (20)       18 2023-04-13 11:39:22.000000 barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-13 11:39:22.294844 barbell2_bodycomp-0.3.0/setup.cfg
--rw-r--r--   0 ralph      (501) staff       (20)     1414 2023-04-13 11:38:29.000000 barbell2_bodycomp-0.3.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.467263 barbell2_bodycomp-0.4.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 07:09:24.466997 barbell2_bodycomp-0.4.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.462636 barbell2_bodycomp-0.4.0/barbell2_bodycomp/
+-rw-r--r--   0 ralph      (501) staff       (20)      392 2023-04-15 07:09:19.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     4465 2023-04-13 12:43:05.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/calculator.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.466278 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/
+-rw-r--r--   0 ralph      (501) staff       (20)      403 2023-04-13 11:54:27.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2nifti.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2npy.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2nrrd.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2png.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/tag2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/tag2npy.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.466627 barbell2_bodycomp-0.4.0/barbell2_bodycomp/pipeline/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2023-04-13 11:55:38.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/pipeline/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     3152 2023-04-15 07:05:04.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/pipeline/bodycomp.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6054 2023-04-13 11:59:22.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/seg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1394 2023-04-13 12:19:43.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectroi.py
+-rw-r--r--   0 ralph      (501) staff       (20)     5804 2023-04-13 12:19:18.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectslice.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1586 2023-04-13 11:15:28.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/totalseg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.464418 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      882 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       68 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       18 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 07:09:24.467342 barbell2_bodycomp-0.4.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1456 2023-04-13 12:44:51.000000 barbell2_bodycomp-0.4.0/setup.py
```

### Comparing `barbell2_bodycomp-0.3.0/PKG-INFO` & `barbell2_bodycomp-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2_bodycomp
-Version: 0.3.0
+Version: 0.4.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/calculator.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import logging
 import pydicom
 import numpy as np
 
-from barbell2.utils import calculate_area, calculate_mean_radiation_attenuation, get_pixels
+from barbell2_bodycomp.utils import calculate_area, calculate_mean_radiation_attenuation, get_pixels
 
 logger = logging.getLogger(__name__)
 
 
 class BodyCompositionCalculator:
 
     MUSCLE = 1
```

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2nifti.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/dcm2npy.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2npy.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2dcm.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2nrrd.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2nrrd.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/npy2png.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2png.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/convert/tag2dcm.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/tag2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/seg.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/seg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import json
 import zipfile
 import logging
 import pydicom
 import numpy as np
 
-from barbell2.utils import is_dicom_file, get_pixels
+from barbell2_bodycomp.utils import is_dicom_file, get_pixels
 
 logger = logging.getLogger(__name__)
 
 
 class MuscleFatSegmentator:
 
     ARGMAX = 0
@@ -22,15 +22,15 @@
         self.mode = MuscleFatSegmentator.ARGMAX
         self.output_directory = None
         self.output_segmentation_files = None
 
     @staticmethod
     def load_model(file_path):
         import tensorflow as tf
-        model_directory = '/tmp/barbell2/bodycomp/seg.py'
+        model_directory = '/tmp/barbell2_bodycomp/model'
         os.makedirs(model_directory, exist_ok=True)
         with zipfile.ZipFile(file_path) as zip_obj:
             zip_obj.extractall(path=model_directory)
         return tf.keras.models.load_model(model_directory, compile=False)
 
     @staticmethod
     def load_params(file_path):
```

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/selectroi.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectroi.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     VERTEBRAE_T4 = 'vertebrae_T4.nii.gz'
     VERTEBRAE_L2 = 'vertebrae_L2.nii.gz'
     VERTEBRAE_L3 = 'vertebrae_L3.nii.gz'
     VERTEBRAE_L4 = 'vertebrae_L4.nii.gz'
 
     def __init__(self):
         self.input_directory = None
-        self.roi = None
         self.output_directory = None
+        self.roi = RoiSelector.VERTEBRAE_L3
         self.overwrite = True
         self.output_file = None
 
     @staticmethod
     def exists(f):
         return os.path.isfile(f)
```

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/selectslice.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectslice.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     TOP = 3
     BOTTOM = 4
 
     def __init__(self):
         self.input_roi = None
         self.input_volume = None
         self.input_dicom_directory = None
-        self.mode = None
+        self.mode = SliceSelector.MEDIAN
         self.output_files = None
 
     @staticmethod
     def has_duplicate_objects(roi):
         # TODO: Implement this!
         return False
```

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/totalseg.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/totalseg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp/utils.py` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/PKG-INFO` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: barbell2-bodycomp
-Version: 0.3.0
+Version: 0.4.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.3.0/barbell2_bodycomp.egg-info/SOURCES.txt` & `barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 barbell2_bodycomp/convert/__init__.py
 barbell2_bodycomp/convert/dcm2nifti.py
 barbell2_bodycomp/convert/dcm2npy.py
 barbell2_bodycomp/convert/npy2dcm.py
 barbell2_bodycomp/convert/npy2nrrd.py
 barbell2_bodycomp/convert/npy2png.py
 barbell2_bodycomp/convert/tag2dcm.py
-barbell2_bodycomp/convert/tag2npy.py
+barbell2_bodycomp/convert/tag2npy.py
+barbell2_bodycomp/pipeline/__init__.py
+barbell2_bodycomp/pipeline/bodycomp.py
```

### Comparing `barbell2_bodycomp-0.3.0/setup.py` & `barbell2_bodycomp-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 requirements = [
     'numpy',
     'pydicom',
     'pynrrd',
     'matplotlib',
     'nibabel',
+    'tensorflow',
+    'totalsegmentator',
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
```

