# Comparing `tmp/pyroscopegridding-0.2.2.tar.gz` & `tmp/pyroscopegridding-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.2.2.tar", last modified: Sat Apr 15 02:05:35 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.2.3.tar", last modified: Sat Apr 15 02:08:59 2023, max compression
```

## Comparing `pyroscopegridding-0.2.2.tar` & `pyroscopegridding-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 02:05:36.640709 pyroscopegridding-0.2.2/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      781 2023-04-15 02:05:36.635714 pyroscopegridding-0.2.2/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.2/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 02:05:36.319237 pyroscopegridding-0.2.2/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.2/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.2/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.2/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.2/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.2/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26288 2023-04-15 01:27:46.000000 pyroscopegridding-0.2.2/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.2/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.2/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.2/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.2/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 02:05:36.598337 pyroscopegridding-0.2.2/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      781 2023-04-15 02:05:35.000000 pyroscopegridding-0.2.2/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 02:05:35.000000 pyroscopegridding-0.2.2/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 02:05:35.000000 pyroscopegridding-0.2.2/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 02:05:35.000000 pyroscopegridding-0.2.2/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-04-15 02:05:35.000000 pyroscopegridding-0.2.2/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 02:05:35.000000 pyroscopegridding-0.2.2/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 02:05:36.642709 pyroscopegridding-0.2.2/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1830 2023-04-15 02:04:31.000000 pyroscopegridding-0.2.2/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 02:09:00.555730 pyroscopegridding-0.2.3/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-04-15 02:09:00.551586 pyroscopegridding-0.2.3/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.3/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 02:09:00.279437 pyroscopegridding-0.2.3/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.3/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.3/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.3/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.3/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.3/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26288 2023-04-15 01:27:46.000000 pyroscopegridding-0.2.3/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.3/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.3/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.3/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.3/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-15 02:09:00.522886 pyroscopegridding-0.2.3/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-04-15 02:08:59.000000 pyroscopegridding-0.2.3/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-15 02:08:59.000000 pyroscopegridding-0.2.3/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-15 02:08:59.000000 pyroscopegridding-0.2.3/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-15 02:08:59.000000 pyroscopegridding-0.2.3/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-04-15 02:08:59.000000 pyroscopegridding-0.2.3/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-15 02:08:59.000000 pyroscopegridding-0.2.3/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-15 02:09:00.556729 pyroscopegridding-0.2.3/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1799 2023-04-15 02:08:50.000000 pyroscopegridding-0.2.3/setup.py
```

### Comparing `pyroscopegridding-0.2.2/README.md` & `pyroscopegridding-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.2.3/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.2.3/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.2.3/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/gridding.py` & `pyroscopegridding-0.2.3/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/gtools.py` & `pyroscopegridding-0.2.3/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.2.3/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.2.3/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.2.3/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.2.3/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.2.3/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.2/setup.py` & `pyroscopegridding-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 import codecs
-import os
+from pathlib import Path
 
-VERSION = '0.2.2'
-DESCRIPTION = 'Data fusion package for satellite data transformation.'
-LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.2.2',      # Initial version
+    version = '0.2.3',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
-    long_description = "file: README.md",
+    long_description = long_description,
+    long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
     entry_points ={
         'console_scripts': [
```

