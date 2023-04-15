# Comparing `tmp/pyroscopegridding-0.1.8.tar.gz` & `tmp/pyroscopegridding-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.1.8.tar", last modified: Sat Apr 15 01:11:41 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.1.9.tar", last modified: Sat Apr 15 01:15:40 2023, max compression
```

## Comparing `pyroscopegridding-0.1.8.tar` & `pyroscopegridding-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:11:42.083251 pyroscopegridding-0.1.8/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:11:42.072121 pyroscopegridding-0.1.8/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.8/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:11:41.819845 pyroscopegridding-0.1.8/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.8/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3697 2023-04-15 00:54:43.000000 pyroscopegridding-0.1.8/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.1.8/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33715 2023-04-15 01:11:20.000000 pyroscopegridding-0.1.8/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.1.8/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26096 2023-04-15 00:55:44.000000 pyroscopegridding-0.1.8/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.1.8/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.8/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.8/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.1.8/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:11:42.034198 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:11:42.089603 pyroscopegridding-0.1.8/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:11:19.000000 pyroscopegridding-0.1.8/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:15:41.808006 pyroscopegridding-0.1.9/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:15:41.802007 pyroscopegridding-0.1.9/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.9/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:15:41.461958 pyroscopegridding-0.1.9/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.9/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3697 2023-04-15 01:15:16.000000 pyroscopegridding-0.1.9/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.1.9/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33858 2023-04-15 01:15:22.000000 pyroscopegridding-0.1.9/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.1.9/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26096 2023-04-15 00:55:44.000000 pyroscopegridding-0.1.9/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.1.9/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.9/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.9/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.1.9/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:15:41.759313 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:15:41.809608 pyroscopegridding-0.1.9/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:15:29.000000 pyroscopegridding-0.1.9/setup.py
```

### Comparing `pyroscopegridding-0.1.8/PKG-INFO` & `pyroscopegridding-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.8/README.md` & `pyroscopegridding-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.1.9/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.1.9/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.1.9/pyroscopegridding/grid_ncf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # 4. Multi time file saving: 
 
 from http.client import MOVED_PERMANENTLY
 import netCDF4
 import numpy as np
 import numpy.ma as ma
 import time
+import os
 
 from pyroscopegridding.gridding import *
 from pyroscopegridding.sat_data_input import *
 from pyroscopegridding.filter_data import *
 from pyroscopegridding.naming_conventions import *
 from pyroscopegridding.solar_zenith import *
 from pyroscopegridding.fileparser import *
@@ -295,15 +296,19 @@
     for i, s_name in enumerate(filelist.keys()): 
         start_timer = time.time()
 
         for s in filelist.get(s_name):
             print("WORK SENSOR: ", s_name)
             s = os.path.normpath(s)
             print("FILE: ", str(s))
-            L2FID,GeoID,PhyID = open_file(s)
+            
+            try:
+                L2FID,GeoID,PhyID = open_file(s)
+            except:
+                L2FID,GeoID,PhyID = open_file(convert_path_to_windows(s))
 
             # check for hdf files 
             if (str(s).split(".")[-1] == "hdf"):
                 geo_list = ['Latitude', 'Longitude']
                 lat,lon,phy_vars, meta = filter_data_hdf(GeoID, PhyID, geo_list, phy_list, phy_hdf)
                 L2FID.end()
```

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/gridding.py` & `pyroscopegridding-0.1.9/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/gtools.py` & `pyroscopegridding-0.1.9/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.1.9/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.1.9/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.1.9/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.1.9/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.1.9/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.8/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.1.9/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.8/setup.py` & `pyroscopegridding-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.1.8',      # Initial version
+    version = '0.1.9',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
```

