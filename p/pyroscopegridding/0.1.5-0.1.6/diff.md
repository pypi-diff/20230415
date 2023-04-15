# Comparing `tmp/pyroscopegridding-0.1.5.tar.gz` & `tmp/pyroscopegridding-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.1.5.tar", last modified: Sat Apr 15 00:56:25 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.1.6.tar", last modified: Sat Apr 15 01:01:43 2023, max compression
```

## Comparing `pyroscopegridding-0.1.5.tar` & `pyroscopegridding-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 00:56:26.690924 pyroscopegridding-0.1.5/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 00:56:26.685923 pyroscopegridding-0.1.5/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.5/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 00:56:26.416282 pyroscopegridding-0.1.5/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.5/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3697 2023-04-15 00:54:43.000000 pyroscopegridding-0.1.5/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.1.5/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33600 2023-04-15 00:44:13.000000 pyroscopegridding-0.1.5/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.1.5/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26096 2023-04-15 00:55:44.000000 pyroscopegridding-0.1.5/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.1.5/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.5/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.5/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5113 2023-04-15 00:45:57.000000 pyroscopegridding-0.1.5/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 00:56:26.653838 pyroscopegridding-0.1.5/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 00:56:25.000000 pyroscopegridding-0.1.5/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 00:56:25.000000 pyroscopegridding-0.1.5/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 00:56:25.000000 pyroscopegridding-0.1.5/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 00:56:25.000000 pyroscopegridding-0.1.5/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 00:56:25.000000 pyroscopegridding-0.1.5/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 00:56:25.000000 pyroscopegridding-0.1.5/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 00:56:26.694834 pyroscopegridding-0.1.5/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 00:55:54.000000 pyroscopegridding-0.1.5/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:01:44.654090 pyroscopegridding-0.1.6/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:01:44.650553 pyroscopegridding-0.1.6/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.6/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:01:44.404136 pyroscopegridding-0.1.6/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.6/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3697 2023-04-15 00:54:43.000000 pyroscopegridding-0.1.6/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.1.6/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33648 2023-04-15 01:00:32.000000 pyroscopegridding-0.1.6/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.1.6/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26096 2023-04-15 00:55:44.000000 pyroscopegridding-0.1.6/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.1.6/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.6/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.6/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.1.6/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:01:44.617512 pyroscopegridding-0.1.6/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:01:43.000000 pyroscopegridding-0.1.6/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:01:43.000000 pyroscopegridding-0.1.6/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:01:43.000000 pyroscopegridding-0.1.6/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:01:43.000000 pyroscopegridding-0.1.6/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:01:43.000000 pyroscopegridding-0.1.6/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:01:43.000000 pyroscopegridding-0.1.6/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:01:44.655187 pyroscopegridding-0.1.6/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:01:39.000000 pyroscopegridding-0.1.6/setup.py
```

### Comparing `pyroscopegridding-0.1.5/PKG-INFO` & `pyroscopegridding-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.5/README.md` & `pyroscopegridding-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.1.6/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.1.6/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.1.6/pyroscopegridding/grid_ncf.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 import time
 
 from pyroscopegridding.gridding import *
 from pyroscopegridding.sat_data_input import *
 from pyroscopegridding.filter_data import *
 from pyroscopegridding.naming_conventions import *
 from pyroscopegridding.solar_zenith import *
+from pyroscopegridding.fileparser import *
+
 #import gridding
 #import sat_data_input
 #import filter_data
 #import naming_conventions
 #import solar_zenith
 
 import datetime
@@ -50,15 +52,15 @@
 # keys are satellite names, values = array of filepaths
 # returns 1D array of satellite file inputs
 def sat_list_name_concat(file_list):
     file_inputs = []
     
     for key in file_list:
         for f in file_list[key]:
-            f = convert_path_to_linx(f)
+            f = convert_path_to_linux(f)
             file_inputs.append(f[(f.rfind("/") + 1):])
     
     return file_inputs
 
 
 # filename - 'gridNet.nc' (this is what it saves to)
 # sat_files - list of satellite files to pull data from
@@ -106,15 +108,15 @@
     ds.RangeBeginningTime = time_time
     ds.RangeEndingDate = time_end_date
     ds.RangeEndingTime = time_end_time
     ds.ProcessingLevel = "Level 3"
     ds.ShortName = "AERDT_L3_MEASURES_QD_HH"
     
     print("FILENAME:", filename)
-    filename = convert_path_to_linx(filename) #convert to linux pwd
+    filename = convert_path_to_linux(filename) #convert to linux pwd
     cut_index = filename.rindex("/")
     filename_without_path = filename[cut_index+1 :]
     ds.GranuleID = filename_without_path
     
     production_yyyymmdd = filename_without_path[-11:-3]
     currtime = datetime.datetime.now()
     production_hhmmss = currtime.strftime("%H%M%S")
```

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/gridding.py` & `pyroscopegridding-0.1.6/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/gtools.py` & `pyroscopegridding-0.1.6/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.1.6/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.1.6/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.1.6/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.1.6/pyroscopegridding/time_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #
 
 # due to the introduction of the time variable, we need to know the time of the sensor data
 # this information is not given in the file itself, but rather the file name
 # e.g. "AERDT_L2_ABI_G16.A2021008.0850.001.nc" --> 10/08/2021 8:50 AM
 import datetime
 
+from pyroscopegridding.fileparser import *
+
 full_satellite_list = ['ABI_G16', 'ABI_G17', 'AHI_H08', 'VIIRS_SNPP', 'MOD04', 'MODIS_T', 'MODIS_A', 'MYD04']
 
 # given 'yyyy/mm/dd/hr/mm' string
 # converts to datetime object
 def to_datetime(date_string):
     format = '%Y/%m/%d/%H/%M'
     d = datetime.datetime.strptime(date_string, format)
```

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.1.6/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.5/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.1.6/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.5/setup.py` & `pyroscopegridding-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.1.5',      # Initial version
+    version = '0.1.6',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
```

