# Comparing `tmp/TerraVide-0.1.0.tar.gz` & `tmp/TerraVide-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraVide-0.1.0.tar", last modified: Fri Apr 14 00:39:24 2023, max compression
+gzip compressed data, was "TerraVide-0.1.2.tar", last modified: Sat Apr 15 02:42:28 2023, max compression
```

## Comparing `TerraVide-0.1.0.tar` & `TerraVide-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.484486 TerraVide-0.1.0/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.1.0/LICENSE.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1612 2023-04-14 00:39:24.484356 TerraVide-0.1.0/PKG-INFO
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.483620 TerraVide-0.1.0/TerraVide.egg-info/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1612 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/PKG-INFO
--rw-r--r--   0 sarangpramode   (501) staff       (20)      257 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/SOURCES.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/dependency_links.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        6 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/requires.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       13 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/top_level.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-14 00:39:24.484525 TerraVide-0.1.0/setup.cfg
--rw-r--r--   0 sarangpramode   (501) staff       (20)     2615 2023-04-14 00:30:38.000000 TerraVide-0.1.0/setup.py
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.482534 TerraVide-0.1.0/terravide/
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.484177 TerraVide-0.1.0/terravide/src/
--rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.1.0/terravide/src/__init__.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     4331 2023-04-14 00:24:49.000000 TerraVide-0.1.0/terravide/src/dataset.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1823 2023-04-14 00:38:04.000000 TerraVide-0.1.0/terravide/src/info.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:42:28.633860 TerraVide-0.1.2/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.1.2/LICENSE.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1395 2023-04-15 02:42:28.633690 TerraVide-0.1.2/PKG-INFO
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:42:28.632641 TerraVide-0.1.2/TerraVide.egg-info/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1395 2023-04-15 02:42:28.000000 TerraVide-0.1.2/TerraVide.egg-info/PKG-INFO
+-rw-r--r--   0 sarangpramode   (501) staff       (20)      272 2023-04-15 02:42:28.000000 TerraVide-0.1.2/TerraVide.egg-info/SOURCES.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-15 02:42:28.000000 TerraVide-0.1.2/TerraVide.egg-info/dependency_links.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        6 2023-04-15 02:42:28.000000 TerraVide-0.1.2/TerraVide.egg-info/requires.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       13 2023-04-15 02:42:28.000000 TerraVide-0.1.2/TerraVide.egg-info/top_level.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)      220 2023-04-14 21:41:12.000000 TerraVide-0.1.2/pyproject.toml
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-15 02:42:28.633908 TerraVide-0.1.2/setup.cfg
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     2615 2023-04-15 02:40:32.000000 TerraVide-0.1.2/setup.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:42:28.631261 TerraVide-0.1.2/terravide/
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:42:28.633257 TerraVide-0.1.2/terravide/src/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.1.2/terravide/src/__init__.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     5329 2023-04-15 00:07:47.000000 TerraVide-0.1.2/terravide/src/dataset.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1890 2023-04-14 22:26:22.000000 TerraVide-0.1.2/terravide/src/info.py
```

### Comparing `TerraVide-0.1.0/LICENSE.txt` & `TerraVide-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TerraVide-0.1.0/PKG-INFO` & `TerraVide-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.1.0
+Version: 0.1.2
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
 Author: Sarang Pramode
+Author-email: Sarang Pramode <sp872@cornell.edu>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -21,31 +22,17 @@
 
 # Installation
 
 ```python
 pip install terravide
 ```
 
-# Usage
+# Documentation
 
-### Dataset module
-```python
-import terravide.src.dataset as dataset
-
-# The dataset module allows you to build a dataset by downloading data from an FTP server
-
-# Default FTP Server - NYC Topobathymetric LiDAR Data (2017)
-
-# List Files in FTP server
-FileList = dataset.dataset.FTP_list_files(year=2021)
-
-# Download Files from FTP server
-dataset.FTP_download_lasfile('25192.las')
-
-```
+Visit Terravide's official documentation here : [TerraVide Docs](https://terravide.readthedocs.io/en/latest/)
 
 # License
 
 TerraVide is released under the MIT license.
```

### Comparing `TerraVide-0.1.0/TerraVide.egg-info/PKG-INFO` & `TerraVide-0.1.2/TerraVide.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.1.0
+Version: 0.1.2
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
 Author: Sarang Pramode
+Author-email: Sarang Pramode <sp872@cornell.edu>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -21,31 +22,17 @@
 
 # Installation
 
 ```python
 pip install terravide
 ```
 
-# Usage
+# Documentation
 
-### Dataset module
-```python
-import terravide.src.dataset as dataset
-
-# The dataset module allows you to build a dataset by downloading data from an FTP server
-
-# Default FTP Server - NYC Topobathymetric LiDAR Data (2017)
-
-# List Files in FTP server
-FileList = dataset.dataset.FTP_list_files(year=2021)
-
-# Download Files from FTP server
-dataset.FTP_download_lasfile('25192.las')
-
-```
+Visit Terravide's official documentation here : [TerraVide Docs](https://terravide.readthedocs.io/en/latest/)
 
 # License
 
 TerraVide is released under the MIT license.
```

### Comparing `TerraVide-0.1.0/setup.py` & `TerraVide-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TerraVide",                     # This is the name of the package
-    version="0.1.0",                        #release version
+    version="0.1.2",                        #release version
     author="Sarang Pramode",                     # Full name of the author
     description="An open source python package to process and simulate large urban environments mapped with LiDAR data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     license='MIT',
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
```

### Comparing `TerraVide-0.1.0/terravide/src/dataset.py` & `TerraVide-0.1.2/terravide/src/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -58,14 +58,22 @@
 
         #Close FTP connection
         ftp.close()
 
     return None
 
 def FTP_GetFileList(datayear=2017):
+    """Get list of all files in the FTP directory of NYC scans
+
+    Args:
+        datayear (int, optional): _description_. Defaults to 2017.
+
+    Returns:
+        _type_: filenames in the FTP server as a list
+    """    
 
     assert datayear in [2017,2021], "NYC recorded lidar data only during 2017 and 2021, default is 2021"
 
     domain = 'ftp.gis.ny.gov'
     ftp_datadir = None
     if datayear == 2017:
         ftp_datadir =  'elevation/LIDAR/NYC_TopoBathymetric2017'
@@ -81,21 +89,21 @@
     ftp.cwd(ftp_datadir)
     
 
     filenames = ftp.nlst() # get filenames within the directory
     return filenames
 
 def FTP_list_files(datayear=2021):
-    """List all files in the lidar directory of NYC scans
+    """List all files in the FTP directory of NYC scans
 
     Args:
         datayear (int, optional): _description_. Defaults to 2021.
 
     Returns:
-        None: _description_
+        None: prints to console
     """
 
     assert datayear in [2017,2021], "NYC recorded lidar data only during 2017 and 2021, default is 2021"
 
     domain = 'ftp.gis.ny.gov'
     ftp_datadir = None
     if datayear == 2017:
@@ -110,14 +118,40 @@
     #enter data directory
     ftp.cwd(ftp_datadir)
 
     ftp.retrlines('LIST')
 
     return None
 
+def Get_filenames(folder_path:str, year:int)->list:
+    """Get list of filenames in a folder Generated by the FTP_download_lasfile function
+
+    Args:
+        folder_path (str): path to folder
+        year (int): subfolder name designated by year of data (2017, 2021)
+
+    Returns:
+        list: _description_
+    """
+    folder_path = folder_path+'NYC_'+str(year)+'/'
+    filenames = [f for f in os.listdir(folder_path) if os.path.isfile(os.path.join(folder_path, f))]
+    return filenames
+
+def Delete_File(file_path:str)->None:
+    """Delete a file
+
+    Args:
+        file_path (str): path to file
+    """    
+    if os.path.isfile(file_path):
+        os.remove(file_path)
+        print(f"{file_path} has been deleted.")
+    else:
+        print(f"{file_path} not found.")
+
 
 if __name__ == '__main__':
 
     DEFAULT_FOLDER_PATH = "Datasets/FTP_files/LiDAR/"
     # Get Year Input from User
     year = int(input("Enter Desired YEAR [2017 and 2021 supported] : "))
     # Get List of filnames on FTP server
```

### Comparing `TerraVide-0.1.0/terravide/src/info.py` & `TerraVide-0.1.2/terravide/src/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,7 +35,12 @@
     print('''
     MIT License (MIT)''')
 
 # Function to print the author
 def author():
     print('''
     Author :  Sarang Pramode''')
+
+if __name__ == '__main__':
+    about()
+    license()
+    author()
```

