# Comparing `tmp/pyroscopegridding-0.1.7.tar.gz` & `tmp/pyroscopegridding-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.1.7.tar", last modified: Sat Apr 15 01:09:09 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.1.8.tar", last modified: Sat Apr 15 01:11:41 2023, max compression
```

## Comparing `pyroscopegridding-0.1.7.tar` & `pyroscopegridding-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:09:10.439726 pyroscopegridding-0.1.7/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:09:10.436725 pyroscopegridding-0.1.7/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.7/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:09:10.181039 pyroscopegridding-0.1.7/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.7/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3697 2023-04-15 00:54:43.000000 pyroscopegridding-0.1.7/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.1.7/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33678 2023-04-15 01:08:41.000000 pyroscopegridding-0.1.7/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.1.7/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26096 2023-04-15 00:55:44.000000 pyroscopegridding-0.1.7/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.1.7/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.7/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.7/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.1.7/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:09:10.403632 pyroscopegridding-0.1.7/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:09:08.000000 pyroscopegridding-0.1.7/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:09:09.000000 pyroscopegridding-0.1.7/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:09:08.000000 pyroscopegridding-0.1.7/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:09:08.000000 pyroscopegridding-0.1.7/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:09:09.000000 pyroscopegridding-0.1.7/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:09:09.000000 pyroscopegridding-0.1.7/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:09:10.442087 pyroscopegridding-0.1.7/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:09:06.000000 pyroscopegridding-0.1.7/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:11:42.083251 pyroscopegridding-0.1.8/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:11:42.072121 pyroscopegridding-0.1.8/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.8/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:11:41.819845 pyroscopegridding-0.1.8/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.8/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3697 2023-04-15 00:54:43.000000 pyroscopegridding-0.1.8/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.1.8/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33715 2023-04-15 01:11:20.000000 pyroscopegridding-0.1.8/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.1.8/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26096 2023-04-15 00:55:44.000000 pyroscopegridding-0.1.8/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.1.8/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.8/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.8/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.1.8/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:11:42.034198 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:11:41.000000 pyroscopegridding-0.1.8/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:11:42.089603 pyroscopegridding-0.1.8/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:11:19.000000 pyroscopegridding-0.1.8/setup.py
```

### Comparing `pyroscopegridding-0.1.7/PKG-INFO` & `pyroscopegridding-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.7
+Version: 0.1.8
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.7/README.md` & `pyroscopegridding-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.1.8/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.1.8/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.1.8/pyroscopegridding/grid_ncf.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,14 +293,15 @@
     # [[time0: [sat1], [sat2], ... ], ...[timek: [sat1], [sat2], ....]] 
     # we assume we receive a signle dict for a time interval though
     for i, s_name in enumerate(filelist.keys()): 
         start_timer = time.time()
 
         for s in filelist.get(s_name):
             print("WORK SENSOR: ", s_name)
+            s = os.path.normpath(s)
             print("FILE: ", str(s))
             L2FID,GeoID,PhyID = open_file(s)
 
             # check for hdf files 
             if (str(s).split(".")[-1] == "hdf"):
                 geo_list = ['Latitude', 'Longitude']
                 lat,lon,phy_vars, meta = filter_data_hdf(GeoID, PhyID, geo_list, phy_list, phy_hdf)
```

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/gridding.py` & `pyroscopegridding-0.1.8/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/gtools.py` & `pyroscopegridding-0.1.8/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.1.8/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.1.8/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.1.8/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.1.8/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.1.8/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.7
+Version: 0.1.8
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.7/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.1.8/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.7/setup.py` & `pyroscopegridding-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.1.7',      # Initial version
+    version = '0.1.8',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
```

