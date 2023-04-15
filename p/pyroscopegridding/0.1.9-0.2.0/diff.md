# Comparing `tmp/pyroscopegridding-0.1.9.tar.gz` & `tmp/pyroscopegridding-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.1.9.tar", last modified: Sat Apr 15 01:15:40 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.2.0.tar", last modified: Sat Apr 15 01:27:58 2023, max compression
```

## Comparing `pyroscopegridding-0.1.9.tar` & `pyroscopegridding-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:15:41.808006 pyroscopegridding-0.1.9/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:15:41.802007 pyroscopegridding-0.1.9/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.9/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:15:41.461958 pyroscopegridding-0.1.9/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.9/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3697 2023-04-15 01:15:16.000000 pyroscopegridding-0.1.9/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.1.9/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33858 2023-04-15 01:15:22.000000 pyroscopegridding-0.1.9/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.1.9/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26096 2023-04-15 00:55:44.000000 pyroscopegridding-0.1.9/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.1.9/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.9/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.9/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.1.9/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:15:41.759313 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:15:40.000000 pyroscopegridding-0.1.9/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:15:41.809608 pyroscopegridding-0.1.9/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:15:29.000000 pyroscopegridding-0.1.9/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:27:59.756297 pyroscopegridding-0.2.0/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:27:59.751294 pyroscopegridding-0.2.0/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.0/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:27:59.486259 pyroscopegridding-0.2.0/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.0/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.0/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.0/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.0/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.0/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26288 2023-04-15 01:27:46.000000 pyroscopegridding-0.2.0/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.0/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.0/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.2.0/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.0/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 01:27:59.718397 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 01:27:59.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 01:27:58.000000 pyroscopegridding-0.2.0/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 01:27:59.759298 pyroscopegridding-0.2.0/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-15 01:27:55.000000 pyroscopegridding-0.2.0/setup.py
```

### Comparing `pyroscopegridding-0.1.9/PKG-INFO` & `pyroscopegridding-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.9
+Version: 0.2.0
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.9/README.md` & `pyroscopegridding-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.2.0/pyroscopegridding/fileparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,35 +25,40 @@
     
     return new_path
 
 def convert_path_to_windows(path):
     new_path = path.replace("/mnt/c", "C:")
     new_path = new_path.replace("/", "\\")
     
-    
     return new_path
 
+def convert_to_other_system(path):
+    if "/" in path: #linux path
+        return convert_path_to_windows(path)
+    else:
+        return convert_path_to_linux(path)
+
 # given path to text file contaings paths to files to read read out as list of files within
 def read_file_sat_data(fileloc):
     lines = []
 
     with open(fileloc) as f:
-        lines = [os.path.normpath(line.rstrip('\n')) for line in f]
+        lines = [convert_path_to_linux(line.rstrip('\n')) for line in f]
 
     #print(lines)
     return lines
 
 # given folder path with files inside, read out list of files within
 def read_folder_sat_data(folderloc):
     #convert all to linux
     folderloc = convert_path_to_linux(folderloc)
     
     files = os.listdir(folderloc)
     #reads all files in folder and converts to path of system type
-    lines = [os.path.normpath(folderloc+"/"+f) for f in files]
+    lines = [folderloc+"/"+f for f in files]
     
     return lines
 
 # netCDF_multi_time(filelist, gsize, geo_list, phy_list, output, time_interval, time_start, time_end)
 def read_in_commands(fileloc):
     cmds = []
 
@@ -92,15 +97,15 @@
     f = []
     filelist = []
     for (dirpath, dirnames, filenames) in walk(path):
         #assume all in linux
         filenames_path = [convert_path_to_linux(dirpath)+"/"+f if convert_path_to_linux(dirpath)[-1]!="/" else convert_path_to_linux(dirpath)+f for f in filenames]
         
         #convert to system path setting
-        filenames_path = [os.path.normpath(f) for f in filenames_path]
+        #filenames_path = [os.path.normpath(f) for f in filenames_path]
         filelist = filelist + filenames_path
         
     return filelist
 
 if __name__ == '__main__':
     path = "/mnt/c/Users/bobgr/Desktop/NASA Spring 2023/Gridtools Package (Code, README, inputs, outputs, examples, verification)/"
```

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.2.0/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.2.0/pyroscopegridding/grid_ncf.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,21 +294,20 @@
     # [[time0: [sat1], [sat2], ... ], ...[timek: [sat1], [sat2], ....]] 
     # we assume we receive a signle dict for a time interval though
     for i, s_name in enumerate(filelist.keys()): 
         start_timer = time.time()
 
         for s in filelist.get(s_name):
             print("WORK SENSOR: ", s_name)
-            s = os.path.normpath(s)
-            print("FILE: ", str(s))
+            print("FILE ORIGINAL: ", str(s))
+            if not os.path.exists(s):
+                s = convert_to_other_system(s)
+            print("FILE INPUT: ", str(s))
             
-            try:
-                L2FID,GeoID,PhyID = open_file(s)
-            except:
-                L2FID,GeoID,PhyID = open_file(convert_path_to_windows(s))
+            L2FID,GeoID,PhyID = open_file(s)
 
             # check for hdf files 
             if (str(s).split(".")[-1] == "hdf"):
                 geo_list = ['Latitude', 'Longitude']
                 lat,lon,phy_vars, meta = filter_data_hdf(GeoID, PhyID, geo_list, phy_list, phy_hdf)
                 L2FID.end()
```

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/gridding.py` & `pyroscopegridding-0.2.0/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/gtools.py` & `pyroscopegridding-0.2.0/pyroscopegridding/gtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,15 @@
     for f in split_files:
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
         processing_date = sys_time()
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
-        name = os.path.normpath(name)
+        #name = os.path.normpath(name)
         
         #print(f) f = dict (key: sensor, values: array of filelocs)
         # print(split_files)
         
         #print("\n\nNAME:", name)
         #print("\n\TIME STRING:", curr)
         #print("\n\PROCESS DATE:", time_interval)
@@ -374,15 +374,17 @@
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
     
 # output - folder location
 def netCDF_yaml_config_time(file_name, time_start, time_end):
-
+    if not os.path.exists(file_name):
+        file_name = convert_to_other_system(file_name)
+        
     grid_settings, variables, file_io = read_config(file_name)
 
     start_timer = time.time()
 
     geo_list = variables["geo_var"]
     phy_list = variables["phy_var"]
     phy_nc = variables["phy_var_nc"]
@@ -429,14 +431,16 @@
     for f in split_files:
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
         processing_date = sys_time()
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
+        if not os.path.exists(name):
+            name = convert_to_other_system(name)
         
         ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
```

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.2.0/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.2.0/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.2.0/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.2.0/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.2.0/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.1.9
+Version: 0.2.0
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.1.9/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.2.0/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.1.9/setup.py` & `pyroscopegridding-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.1.9',      # Initial version
+    version = '0.2.0',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
```

