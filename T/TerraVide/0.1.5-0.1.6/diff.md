# Comparing `tmp/TerraVide-0.1.5.tar.gz` & `tmp/TerraVide-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraVide-0.1.5.tar", last modified: Sat Apr 15 03:09:43 2023, max compression
+gzip compressed data, was "TerraVide-0.1.6.tar", last modified: Sat Apr 15 03:13:22 2023, max compression
```

## Comparing `TerraVide-0.1.5.tar` & `TerraVide-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.999806 TerraVide-0.1.5/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.1.5/LICENSE.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1346 2023-04-15 03:09:42.999616 TerraVide-0.1.5/PKG-INFO
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.998626 TerraVide-0.1.5/TerraVide.egg-info/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1346 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/PKG-INFO
--rw-r--r--   0 sarangpramode   (501) staff       (20)      348 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/SOURCES.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/dependency_links.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       23 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/requires.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       23 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/top_level.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-15 03:09:42.999856 TerraVide-0.1.5/setup.cfg
--rw-r--r--   0 sarangpramode   (501) staff       (20)     2699 2023-04-15 03:08:07.000000 TerraVide-0.1.5/setup.py
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.998740 TerraVide-0.1.5/terravide/
--rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:35.000000 TerraVide-0.1.5/terravide/__init__.py
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.999299 TerraVide-0.1.5/terravide/src/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1521 2023-04-15 00:08:30.000000 TerraVide-0.1.5/terravide/src/GroundClassification.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     6683 2023-04-15 00:33:25.000000 TerraVide-0.1.5/terravide/src/Preprocessing.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.1.5/terravide/src/__init__.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     5329 2023-04-15 00:07:47.000000 TerraVide-0.1.5/terravide/src/dataset.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1890 2023-04-14 22:26:22.000000 TerraVide-0.1.5/terravide/src/info.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:13:22.375229 TerraVide-0.1.6/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.1.6/LICENSE.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1346 2023-04-15 03:13:22.375081 TerraVide-0.1.6/PKG-INFO
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:13:22.374247 TerraVide-0.1.6/TerraVide.egg-info/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1346 2023-04-15 03:13:22.000000 TerraVide-0.1.6/TerraVide.egg-info/PKG-INFO
+-rw-r--r--   0 sarangpramode   (501) staff       (20)      348 2023-04-15 03:13:22.000000 TerraVide-0.1.6/TerraVide.egg-info/SOURCES.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-15 03:13:22.000000 TerraVide-0.1.6/TerraVide.egg-info/dependency_links.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       19 2023-04-15 03:13:22.000000 TerraVide-0.1.6/TerraVide.egg-info/requires.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       10 2023-04-15 03:13:22.000000 TerraVide-0.1.6/TerraVide.egg-info/top_level.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-15 03:13:22.375273 TerraVide-0.1.6/setup.cfg
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     2685 2023-04-15 03:13:11.000000 TerraVide-0.1.6/setup.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:13:22.374361 TerraVide-0.1.6/terravide/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:35.000000 TerraVide-0.1.6/terravide/__init__.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:13:22.374888 TerraVide-0.1.6/terravide/src/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1521 2023-04-15 00:08:30.000000 TerraVide-0.1.6/terravide/src/GroundClassification.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     6683 2023-04-15 00:33:25.000000 TerraVide-0.1.6/terravide/src/Preprocessing.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.1.6/terravide/src/__init__.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     5329 2023-04-15 00:07:47.000000 TerraVide-0.1.6/terravide/src/dataset.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1890 2023-04-14 22:26:22.000000 TerraVide-0.1.6/terravide/src/info.py
```

### Comparing `TerraVide-0.1.5/LICENSE.txt` & `TerraVide-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TerraVide-0.1.5/PKG-INFO` & `TerraVide-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.1.5
+Version: 0.1.6
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
 Author: Sarang Pramode
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TerraVide-0.1.5/TerraVide.egg-info/PKG-INFO` & `TerraVide-0.1.6/TerraVide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.1.5
+Version: 0.1.6
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
 Author: Sarang Pramode
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TerraVide-0.1.5/setup.py` & `TerraVide-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,29 +29,28 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 print(setuptools.find_packages())
 
 setuptools.setup(
     name="TerraVide",                     # This is the name of the package
-    version="0.1.5",                        #release version
+    version="0.1.6",                        #release version
     author="Sarang Pramode",                     # Full name of the author
     description="An open source python package to process and simulate large urban environments mapped with LiDAR data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     license='MIT',
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
-    py_modules=["info","dataset"],             # Name of the python package
+    #py_modules=["info","dataset"],             # Name of the python package
     install_requires=[              # Install other dependencies if any
         "numpy",
         "pandas",
-        "os",
-        "ftplib",
+        "laspy",
     ]                     
 )
```

### Comparing `TerraVide-0.1.5/terravide/src/GroundClassification.py` & `TerraVide-0.1.6/terravide/src/GroundClassification.py`

 * *Files identical despite different names*

### Comparing `TerraVide-0.1.5/terravide/src/Preprocessing.py` & `TerraVide-0.1.6/terravide/src/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `TerraVide-0.1.5/terravide/src/dataset.py` & `TerraVide-0.1.6/terravide/src/dataset.py`

 * *Files identical despite different names*

### Comparing `TerraVide-0.1.5/terravide/src/info.py` & `TerraVide-0.1.6/terravide/src/info.py`

 * *Files identical despite different names*

