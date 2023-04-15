# Comparing `tmp/pyroscopegridding-0.2.0.tar.gz` & `tmp/pyroscopegridding-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.2.0.tar", last modified: Sat Apr 15 01:27:58 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.2.1.tar", last modified: Sat Apr 15 01:56:53 2023, max compression
```

## Comparing `pyroscopegridding-0.2.0.tar` & `pyroscopegridding-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:27:59.756297 pyroscopegridding-0.2.0/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:27:59.751294 pyroscopegridding-0.2.0/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.0/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:27:59.486259 pyroscopegridding-0.2.0/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.0/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.0/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.0/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.0/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.0/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26288 2023-04-15 01:27:46.000000 pyroscopegridding-0.2.0/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.0/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.0/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.2.0/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.0/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:27:59.718397 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:27:59.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:27:59.759298 pyroscopegridding-0.2.0/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:27:55.000000 pyroscopegridding-0.2.0/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:56:54.173748 pyroscopegridding-0.2.1/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:56:54.169576 pyroscopegridding-0.2.1/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.1/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:56:53.932240 pyroscopegridding-0.2.1/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.1/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.1/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.1/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.1/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.1/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26288 2023-04-15 01:27:46.000000 pyroscopegridding-0.2.1/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.1/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.1/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.1/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.1/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:56:54.137920 pyroscopegridding-0.2.1/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:56:52.000000 pyroscopegridding-0.2.1/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:56:53.000000 pyroscopegridding-0.2.1/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:56:52.000000 pyroscopegridding-0.2.1/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:56:52.000000 pyroscopegridding-0.2.1/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-04-15 01:56:52.000000 pyroscopegridding-0.2.1/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:56:52.000000 pyroscopegridding-0.2.1/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:56:54.175053 pyroscopegridding-0.2.1/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1787 2023-04-15 01:56:37.000000 pyroscopegridding-0.2.1/setup.py
```

### Comparing `pyroscopegridding-0.2.0/PKG-INFO` & `pyroscopegridding-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.2.0/README.md` & `pyroscopegridding-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.2.1/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.2.1/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.2.1/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/gridding.py` & `pyroscopegridding-0.2.1/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/gtools.py` & `pyroscopegridding-0.2.1/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.2.1/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.2.1/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.2.1/pyroscopegridding/solar_zenith.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,14 @@
 
 import numba as nb
 from numba import jit
 from numba import cuda
 
 from joblib import Parallel, delayed
 
-"""
-def get_SZA(row):
-    time_obj = pd.to_datetime(row['Date_UTC']) + pd.to_timedelta(row['Time_UTC'], unit='h')
-    time_obj = time_obj.replace(tzinfo=dt.timezone.utc)
-    lat, lon = row['Lat'], row['Lon']
-    
-    return get_altitude(lat, lon, time_obj)
-"""
 
 #global variables 
 rad = 180/math.pi
 
 ### solar declination angle
 """
```

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.2.1/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.2.1/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.2.0/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.2.1/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.0/setup.py` & `pyroscopegridding-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.2.0',      # Initial version
+    version = '0.2.1',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
@@ -27,15 +27,16 @@
             'numpy',
             'joblib',
             #'cuda',
             'netCDF4',
             'pyhdf',
             'pyyaml',
             'numba',
-            'argparse'
+            'argparse',
+            'pandas'
         ],
     classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Developers',     
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3',      #supported versions
```

