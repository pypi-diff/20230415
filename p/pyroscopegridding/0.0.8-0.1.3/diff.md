# Comparing `tmp/pyroscopegridding-0.0.8.tar.gz` & `tmp/pyroscopegridding-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.0.8.tar", last modified: Fri Apr 14 16:07:51 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.1.3.tar", last modified: Fri Apr 14 21:52:36 2023, max compression
```

## Comparing `pyroscopegridding-0.0.8.tar` & `pyroscopegridding-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 16:07:51.449628 pyroscopegridding-0.0.8/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 16:07:51.446629 pyroscopegridding-0.0.8/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.0.8/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 16:07:51.300626 pyroscopegridding-0.0.8/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.0.8/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2637 2023-04-14 15:49:58.000000 pyroscopegridding-0.0.8/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10388 2023-04-14 15:50:51.000000 pyroscopegridding-0.0.8/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33643 2023-04-14 16:03:37.000000 pyroscopegridding-0.0.8/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10464 2023-04-14 16:03:48.000000 pyroscopegridding-0.0.8/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26242 2023-04-14 16:07:35.000000 pyroscopegridding-0.0.8/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9309 2023-04-14 14:25:01.000000 pyroscopegridding-0.0.8/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.8/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.0.8/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     4779 2023-04-14 16:04:41.000000 pyroscopegridding-0.0.8/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 16:07:51.418630 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-14 16:07:51.450628 pyroscopegridding-0.0.8/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-14 16:07:42.000000 pyroscopegridding-0.0.8/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 21:52:37.605202 pyroscopegridding-0.1.3/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 21:52:37.602203 pyroscopegridding-0.1.3/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.1.3/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 21:52:37.469763 pyroscopegridding-0.1.3/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.1.3/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2637 2023-04-14 15:49:58.000000 pyroscopegridding-0.1.3/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10388 2023-04-14 15:50:51.000000 pyroscopegridding-0.1.3/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33642 2023-04-14 21:41:41.000000 pyroscopegridding-0.1.3/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10464 2023-04-14 16:03:48.000000 pyroscopegridding-0.1.3/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26057 2023-04-14 21:49:30.000000 pyroscopegridding-0.1.3/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 21:36:50.000000 pyroscopegridding-0.1.3/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.1.3/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.1.3/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5071 2023-04-14 17:35:10.000000 pyroscopegridding-0.1.3/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 21:52:37.582288 pyroscopegridding-0.1.3/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 21:52:37.000000 pyroscopegridding-0.1.3/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-14 21:52:37.000000 pyroscopegridding-0.1.3/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-14 21:52:37.000000 pyroscopegridding-0.1.3/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-14 21:52:37.000000 pyroscopegridding-0.1.3/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-14 21:52:37.000000 pyroscopegridding-0.1.3/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-14 21:52:37.000000 pyroscopegridding-0.1.3/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-14 21:52:37.606202 pyroscopegridding-0.1.3/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-14 21:49:23.000000 pyroscopegridding-0.1.3/setup.py
```

### Comparing `pyroscopegridding-0.0.8/PKG-INFO` & `pyroscopegridding-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.0.8
+Version: 0.1.3
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.0.8/README.md` & `pyroscopegridding-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.1.3/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.1.3/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.1.3/pyroscopegridding/grid_ncf.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import time
 
 #import gridding
 #import sat_data_input
 #import filter_data
 #import naming_conventions
 #import solar_zenith
-#import datetime
+import datetime
 
 # full satellite list 
 # used to check if any satellites are missing
 #full_satellite_list = ['AERDT_L2_ABI_G16', 'AERDT_L2_ABI_G17', 'AERDT_L2_AHI_H08', 'AERDT_L2_VIIRS_SNPP', 'MOD04_L2', 'MYD04_L2']
 full_satellite_list = ['ABI_G16', 'ABI_G17', 'AHI_H08', 'VIIRS_SNPP', 'MOD04', 'MYD04']
```

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/gridding.py` & `pyroscopegridding-0.1.3/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/gtools.py` & `pyroscopegridding-0.1.3/pyroscopegridding/gtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 # Gtools
 #
 # the control for the file. It parses command line arguments and calls to grid_ncf
 #
 
 #import other module files
 from concurrent.futures import process
+from pyroscopegridding.filter_data import *
+from pyroscopegridding.fileparser import *
+from pyroscopegridding.sat_data_input import *
+from pyroscopegridding.gridding import *
+from pyroscopegridding.grid_ncf import *
+from pyroscopegridding.time_conv import *
 #import sat_data_input
 #import filter_data
 #import gridding
 #import grid_ncf
 #import fileparser # comment for specific file functions
 #import time_conv
 
@@ -135,19 +141,19 @@
 """
 #gridNC_time(limit, gsize, indata, inlat, inlon, 1, phy_list, geo_list, sat_files[:10], fpath + "viirs_time_compv1.nc")
 def netCDF_multi(filelist, geo_list, phy_list, output):
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
     print(filelist)
 
-    lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
+    lat,lon,phy_vars = multi_sensor_grid_data(filelist, phy_list, geo_list)
 
     print(lat)
     print(lon)
     print(phy_vars)
 
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
@@ -167,22 +173,22 @@
 def netCDF_multi_time(filelist, gsize, geo_list, phy_list, output, time_interval, time_start, time_end):
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
 
-    lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
+    lat,lon,phy_vars = multi_sensor_grid_data(filelist, phy_list, geo_list)
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
     gsize = float(gsize)
     indata = phy_vars
     inlat=lat
     inlon = lon
 
@@ -196,20 +202,20 @@
     start_timer = time.time()
     
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
 
     gsize = float(gsize)
 
     curr = start
     for f in split_files:
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
 
@@ -226,26 +232,26 @@
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(gsize)
 
     curr = start
     for f in split_files:
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
 
@@ -262,26 +268,26 @@
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
     print(geo_list)
     phy_list = phy_list.split(" ")
     print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
-    filelist = fileparser.read_file_sat_data(filelist)
+    filelist = read_file_sat_data(filelist)
 
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(gsize)
 
     curr = start
     for f in split_files:
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #print(f)
@@ -294,163 +300,163 @@
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
 
 # output - folder location
 def netCDF_yaml_config(file_name):
 
-    grid_settings, variables, file_io = fileparser.read_config(file_name)
+    grid_settings, variables, file_io = read_config(file_name)
 
     start_timer = time.time()
 
     geo_list = variables["geo_var"]
     phy_list = variables["phy_var"]
     phy_nc = variables["phy_var_nc"]
     phy_hdf = variables["phy_var_hdf"]
     limit = grid_settings["limit"]
     pixel_range = variables["pixel_range"]
     
     # list of file paths for specific files to read
     if file_io["file_directory_folder"] == "NA":
         if file_io["file_location_folder"] == "NA":
-            filelist = fileparser.read_file_sat_data(file_io["file_location_file"])
+            filelist = read_file_sat_data(file_io["file_location_file"])
         else:
-            filelist = fileparser.read_folder_sat_data(file_io["file_location_folder"])
+            filelist = read_folder_sat_data(file_io["file_location_folder"])
     else:
-        filelist = fileparser.read_directory_sat_data(file_io["file_directory_folder"])
+        filelist = read_directory_sat_data(file_io["file_directory_folder"])
         
         
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
     print("static file:", static_file)
 
     time_start = grid_settings["time_start"]
     time_end = grid_settings["time_end"]
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
     time_interval = grid_settings["time_interval"]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(grid_settings["gridsize"])
 
     curr = start
     outputfolder = file_io["output_location"]
     outputname = file_io["output_name"]
     
     count= 0
     for f in split_files:
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
-        processing_date = time_conv.sys_time()
+        processing_date = sys_time()
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
         #print(f) f = dict (key: sensor, values: array of filelocs)
         # print(split_files)
         
         #print("\n\nNAME:", name)
         #print("\n\TIME STRING:", curr)
         #print("\n\PROCESS DATE:", time_interval)
         
         # grid files
         #grid_nc_sensor_statistics_metadata
         
-        ds = grid_ncf.grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
+        ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
     
 # output - folder location
 def netCDF_yaml_config_time(file_name, time_start, time_end):
 
-    grid_settings, variables, file_io = fileparser.read_config(file_name)
+    grid_settings, variables, file_io = read_config(file_name)
 
     start_timer = time.time()
 
     geo_list = variables["geo_var"]
     phy_list = variables["phy_var"]
     phy_nc = variables["phy_var_nc"]
     phy_hdf = variables["phy_var_hdf"]
     limit = grid_settings["limit"]
     pixel_range = variables["pixel_range"]
     
     # list of file paths for specific files to read
     if file_io["file_directory_folder"] == "NA":
         if file_io["file_location_folder"] == "NA":
-            filelist = fileparser.read_file_sat_data(file_io["file_location_file"])
+            filelist = read_file_sat_data(file_io["file_location_file"])
         else:
-            filelist = fileparser.read_folder_sat_data(file_io["file_location_folder"])
+            filelist = read_folder_sat_data(file_io["file_location_folder"])
     else:
-        filelist = fileparser.read_directory_sat_data(file_io["file_directory_folder"])
+        filelist = read_directory_sat_data(file_io["file_directory_folder"])
         
     print("FILELIST: ", filelist)
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
     print("static file:", static_file)
 
     #time_start = grid_settings["time_start"]
     #time_end = grid_settings["time_end"]
-    start = time_conv.to_datetime(time_start)
-    end = time_conv.to_datetime(time_end)
+    start = to_datetime(time_start)
+    end = to_datetime(time_end)
     
 
     # [[filenames for a time interval] , [], []]
     time_interval = grid_settings["time_interval"]
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
     
     # [{sensor: array of filenames}, {}, {}, {}, {}]
     # code should record bugs - always six sensors available
     # code should report that modis is not available
-    split_files = time_conv.split_filenames(split_files)
+    split_files = split_filenames(split_files)
 
     gsize = float(grid_settings["gridsize"])
 
     curr = start
     outputfolder = file_io["output_location"]
     outputname = file_io["output_name"]
     
     count= 0
     for f in split_files:
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
-        processing_date = time_conv.sys_time()
+        processing_date = sys_time()
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
-        ds = grid_ncf.grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
+        ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
 
     
 
 def execute_file(filename):
-    filelist, gsize, time_interval, start, end, output, geo_list, phy_list = fileparser.read_in_commands(filename)
-    lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
+    filelist, gsize, time_interval, start, end, output, geo_list, phy_list = read_in_commands(filename)
+    lat,lon,phy_vars = multi_sensor_grid_data(filelist, phy_list, geo_list)
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
     gsize = float(gsize)
     indata = phy_vars
     inlat=lat
     inlon = lon
 
-    split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
+    split_files = split_filetimes(filelist, start, end, int(time_interval))
 
     #grid_ncf.grid_nc_mult_files_time(limit, gsize, indata, inlat, inlon, phy_list, geo_list, split_files, output)
 
 
 
 def main():
     # parser object
```

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.1.3/pyroscopegridding/naming_conventions.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         curr_stat = ""
         for stat in statistics_references_long_LEOGEO:
             if statistic == stat:
                 name = statistics_references_long_LEOGEO[stat]
                 curr_stat = statistic
                 if statistic =="Mean" or statistic =="STD" or statistic =="Pixels" or statistic == "TotalPixels":
                     if filtered:
-                        name = name + " " + "AOD at 0.55 micron (Optical_Depth_Land_And_Ocean) for both ocean (Average) and land (corrected) with all quality data (Quality flag = 0, 1, 2, 3)"
+                        name = name + " " + "AOD at 0.55 micron (Optical_Depth_Land_And_Ocean) for both ocean (Average) (Quality flag = 1, 2, 3)  and land (corrected) (Quality flag = 3)"
                     else:
                         name = name + " " + "AOD at 0.55 micron (Image_Optical_Depth_Land_And_Ocean) for both ocean (Average) and land (corrected) with all quality data (Quality flag = 0, 1, 2, 3)"
         for sensor_key in sensor_references_long: #add appropriate sensor name
             if sensor_key in sensor_name:
                 #name = name + " " + sensor_references_long[sensor_key] 
                 if aod_long != None:
                     name = name + " " + aod_long
```

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.1.3/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.1.3/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.1.3/pyroscopegridding/time_conv.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 
 # due to the introduction of the time variable, we need to know the time of the sensor data
 # this information is not given in the file itself, but rather the file name
 # e.g. "AERDT_L2_ABI_G16.A2021008.0850.001.nc" --> 10/08/2021 8:50 AM
 import datetime
 
-full_satellite_list = ['ABI_G16', 'ABI_G17', 'AHI_H08', 'VIIRS_SNPP', 'MOD04', 'MYD04']
+full_satellite_list = ['ABI_G16', 'ABI_G17', 'AHI_H08', 'VIIRS_SNPP', 'MOD04', 'MODIS_T', 'MODIS_A', 'MYD04']
 
 # given 'yyyy/mm/dd/hr/mm' string
 # converts to datetime object
 def to_datetime(date_string):
     format = '%Y/%m/%d/%H/%M'
     d = datetime.datetime.strptime(date_string, format)
 
@@ -85,15 +85,19 @@
             #retrieve sensor name from file format
             s_name = f.split("/")[-1].split(".")[0]
             
             #check to see if sensor is from list of the six measures satellites
             for measures_satellite in full_satellite_list:
                 if measures_satellite in s_name:
                     s_name = measures_satellite
-                    
+                    if measures_satellite == "MOD04" or measures_satellite == "MODIS_T":
+                        s_name = "MOD04"
+                    elif measures_satellite == "MYD04" or measures_satellite == "MODIS_A":
+                        s_name = "MYD04"
+                        
             if s_name not in d: # add to dict if not already present
                 d[s_name] = [f]
             else:
                 d[s_name].append(f)
 
         #split_files.append(list(d.values()))
         split_files.append(d)
```

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.1.3/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.0.8
+Version: 0.1.3
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.0.8/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.1.3/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.8/setup.py` & `pyroscopegridding-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.1.3'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.0.8',      # Initial version
+    version = '0.1.3',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
```

