# Comparing `tmp/cross_cal_resourcesat-0.1.2.tar.gz` & `tmp/cross_cal_resourcesat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cross_cal_resourcesat-0.1.2.tar", last modified: Tue Apr 11 18:52:08 2023, max compression
+gzip compressed data, was "cross_cal_resourcesat-0.1.3.tar", last modified: Sat Apr 15 21:26:05 2023, max compression
```

## Comparing `cross_cal_resourcesat-0.1.2.tar` & `cross_cal_resourcesat-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:52:08.051851 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/cross_cal_resourcesat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:26:05.665328 cross_cal_resourcesat-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-15 21:26:05.665328 cross_cal_resourcesat-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:26:05.665328 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat/cross_cal_resourcesat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat/landsat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:26:05.665328 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-15 21:26:05.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 21:26:05.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 21:26:05.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:26:05.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 21:26:05.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 21:26:05.000000 cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-15 21:26:05.665328 cross_cal_resourcesat-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-15 21:25:56.000000 cross_cal_resourcesat-0.1.3/setup.py
```

### Comparing `cross_cal_resourcesat-0.1.2/LICENSE` & `cross_cal_resourcesat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cross_cal_resourcesat-0.1.2/PKG-INFO` & `cross_cal_resourcesat-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cross_cal_resourcesat
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.
 Home-page: https://github.com/akhi9661/cross_cal_resourcesat
 Author: Akhilesh Kumar
 Author-email: akhiraj9661@gmail.com
 License: MIT license
 Keywords: cross_cal_resourcesat
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,17 +21,18 @@
 License-File: LICENSE
 
 # cross_cal_resourcesat
 
 
 [![image](https://img.shields.io/pypi/v/cross_cal_resourcesat.svg)](https://pypi.python.org/pypi/cross_cal_resourcesat)
 [![image](https://img.shields.io/conda/vn/conda-forge/cross_cal_resourcesat.svg)](https://anaconda.org/conda-forge/cross_cal_resourcesat)
-[![Python Versions](https://img.shields.io/pypi/pyversions/ocm2.svg)](https://pypi.org/project/cross_cal_resourcesat/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/cross_cal_resourcesat.svg)](https://pypi.org/project/cross_cal_resourcesat/)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![image](https://github.com/opengeos/leafmap/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
+[![image](https://github.com/akhi9661/cross_cal_resourcesat/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
+[![image](https://github.com/akhi9661/cross_cal_resourcesat/workflows/Linux%20build/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat/actions)
 
 ---
 
 ## Introduction
 
 This package applies a cross calibrates LISS III and AWiFS with the help of a reference image like Landsat 8 and Sentinel 2.
```

### Comparing `cross_cal_resourcesat-0.1.2/README.md` & `cross_cal_resourcesat-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # cross_cal_resourcesat
 
 
 [![image](https://img.shields.io/pypi/v/cross_cal_resourcesat.svg)](https://pypi.python.org/pypi/cross_cal_resourcesat)
 [![image](https://img.shields.io/conda/vn/conda-forge/cross_cal_resourcesat.svg)](https://anaconda.org/conda-forge/cross_cal_resourcesat)
-[![Python Versions](https://img.shields.io/pypi/pyversions/ocm2.svg)](https://pypi.org/project/cross_cal_resourcesat/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/cross_cal_resourcesat.svg)](https://pypi.org/project/cross_cal_resourcesat/)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![image](https://github.com/opengeos/leafmap/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
+[![image](https://github.com/akhi9661/cross_cal_resourcesat/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
+[![image](https://github.com/akhi9661/cross_cal_resourcesat/workflows/Linux%20build/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat/actions)
 
 ---
 
 ## Introduction
 
 This package applies a cross calibrates LISS III and AWiFS with the help of a reference image like Landsat 8 and Sentinel 2.
```

### Comparing `cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/cross_cal_resourcesat.py` & `cross_cal_resourcesat-0.1.3/cross_cal_resourcesat/cross_cal_resourcesat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ The following package contains the functions to perform cross calibration between LISS III and AWiFS and the reference image. 
 """
 
 import rasterio, os, re, math, glob, shutil
 from osgeo import gdal, osr, gdalconst
-import numpy as np
+import numpy as np 
+from cross_cal_resourcesat import landsat
 
 def meta(inpf, keyword):
 
     """ 
     This function reads the metadata file of the LISS III and AWiFS images and returns the value of the keyword provided.
     Parameters:
             inpf (str): path to folder containing the radiance image and the *_META.txt file
@@ -132,14 +133,20 @@
     if reference_sensor == 'Sentinel 2':
         for i, filename in enumerate(files_ref):
             with rasterio.open(os.path.join(inpf_ref, filename)) as src:
                 multi_band_ref[:,:,i] = src.read(1).astype('float32')*0.0001
 
     elif reference_sensor == 'Landsat 8':
         for i, filename in enumerate(files_ref):
+            opf = landsat.landsat_ref(inpf_ref, filename)
+            with rasterio.open(os.path.join(opf, filename)) as src:
+                multi_band_ref[:,:,i] = src.read(1).astype('float32')
+    
+    else:
+        for i, filename in enumerate(files_ref):
             with rasterio.open(os.path.join(inpf_ref, filename)) as src:
                 multi_band_ref[:,:,i] = src.read(1).astype('float32')
             
     profile.update(count = multi_band_ref.shape[2])
     profile.update(dtype = 'float32')
     op_ref = os.path.join(inpf_ref, 'composite_ref.TIF')
     with rasterio.open(op_ref, 'w', **profile) as dst:
@@ -253,25 +260,25 @@
     os.remove(opf_resample)
     os.remove(file_liss)
     os.remove(file_ref)
     
     print("'Done'")
     return (sbaf, cal_liss, band_liss, band_reference)
 
-def do_calibration(inpf_liss, inpf_ref, reference_sensor = 'Sentinel 2'):
+def do_calibration(inpf_liss, inpf_ref, reference_sensor):
 
     """
     This is the main function. 
     It calls the `do_ref` function to create the reflectance images of LISS III or AWiFS and the reference image.
     Then calls `do_mulitband` function to create layer stacks. Finally calls `calc_calibration` for calibration factors.
     
     Parameters:
             inpf_liss (str): path to folder containing the reflectance images of LISS III or AWiFS
             inpf_ref (str): path to folder containing the reflectance images of the reference image
-            reference_sensor (str, optional): name of the reference sensor. Default is 'Sentinel 2'
+            reference_sensor (str, optional): name of the reference sensor.
 
     Returns:
             None
     """
 
     opf = os.path.join(inpf_liss, 'Reflectance')
     if os.path.exists(opf):
```

### Comparing `cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/PKG-INFO` & `cross_cal_resourcesat-0.1.3/cross_cal_resourcesat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cross-cal-resourcesat
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.
 Home-page: https://github.com/akhi9661/cross_cal_resourcesat
 Author: Akhilesh Kumar
 Author-email: akhiraj9661@gmail.com
 License: MIT license
 Keywords: cross_cal_resourcesat
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,17 +21,18 @@
 License-File: LICENSE
 
 # cross_cal_resourcesat
 
 
 [![image](https://img.shields.io/pypi/v/cross_cal_resourcesat.svg)](https://pypi.python.org/pypi/cross_cal_resourcesat)
 [![image](https://img.shields.io/conda/vn/conda-forge/cross_cal_resourcesat.svg)](https://anaconda.org/conda-forge/cross_cal_resourcesat)
-[![Python Versions](https://img.shields.io/pypi/pyversions/ocm2.svg)](https://pypi.org/project/cross_cal_resourcesat/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/cross_cal_resourcesat.svg)](https://pypi.org/project/cross_cal_resourcesat/)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![image](https://github.com/opengeos/leafmap/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
+[![image](https://github.com/akhi9661/cross_cal_resourcesat/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
+[![image](https://github.com/akhi9661/cross_cal_resourcesat/workflows/Linux%20build/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat/actions)
 
 ---
 
 ## Introduction
 
 This package applies a cross calibrates LISS III and AWiFS with the help of a reference image like Landsat 8 and Sentinel 2.
```

### Comparing `cross_cal_resourcesat-0.1.2/setup.py` & `cross_cal_resourcesat-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='cross_cal_resourcesat',
     name='cross_cal_resourcesat',
     packages=find_packages(include=['cross_cal_resourcesat', 'cross_cal_resourcesat.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/akhi9661/cross_cal_resourcesat',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

