# Comparing `tmp/TerraVide-0.1.4.tar.gz` & `tmp/TerraVide-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraVide-0.1.4.tar", last modified: Sat Apr 15 02:55:09 2023, max compression
+gzip compressed data, was "TerraVide-0.1.5.tar", last modified: Sat Apr 15 03:09:43 2023, max compression
```

## Comparing `TerraVide-0.1.4.tar` & `TerraVide-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:55:09.358120 TerraVide-0.1.4/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.1.4/LICENSE.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1395 2023-04-15 02:55:09.357977 TerraVide-0.1.4/PKG-INFO
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:55:09.357399 TerraVide-0.1.4/TerraVide.egg-info/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1395 2023-04-15 02:55:09.000000 TerraVide-0.1.4/TerraVide.egg-info/PKG-INFO
--rw-r--r--   0 sarangpramode   (501) staff       (20)      240 2023-04-15 02:55:09.000000 TerraVide-0.1.4/TerraVide.egg-info/SOURCES.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-15 02:55:09.000000 TerraVide-0.1.4/TerraVide.egg-info/dependency_links.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       48 2023-04-15 02:55:09.000000 TerraVide-0.1.4/TerraVide.egg-info/top_level.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)      220 2023-04-14 21:41:12.000000 TerraVide-0.1.4/pyproject.toml
--rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-15 02:55:09.358159 TerraVide-0.1.4/setup.cfg
--rw-r--r--   0 sarangpramode   (501) staff       (20)     2552 2023-04-15 02:53:49.000000 TerraVide-0.1.4/setup.py
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:55:09.356195 TerraVide-0.1.4/terravide/
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 02:55:09.357787 TerraVide-0.1.4/terravide/src/
--rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.1.4/terravide/src/__init__.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     5329 2023-04-15 00:07:47.000000 TerraVide-0.1.4/terravide/src/dataset.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1890 2023-04-14 22:26:22.000000 TerraVide-0.1.4/terravide/src/info.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.999806 TerraVide-0.1.5/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.1.5/LICENSE.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1346 2023-04-15 03:09:42.999616 TerraVide-0.1.5/PKG-INFO
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.998626 TerraVide-0.1.5/TerraVide.egg-info/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1346 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/PKG-INFO
+-rw-r--r--   0 sarangpramode   (501) staff       (20)      348 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/SOURCES.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/dependency_links.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       23 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/requires.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       23 2023-04-15 03:09:42.000000 TerraVide-0.1.5/TerraVide.egg-info/top_level.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-15 03:09:42.999856 TerraVide-0.1.5/setup.cfg
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     2699 2023-04-15 03:08:07.000000 TerraVide-0.1.5/setup.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.998740 TerraVide-0.1.5/terravide/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:35.000000 TerraVide-0.1.5/terravide/__init__.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-15 03:09:42.999299 TerraVide-0.1.5/terravide/src/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1521 2023-04-15 00:08:30.000000 TerraVide-0.1.5/terravide/src/GroundClassification.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     6683 2023-04-15 00:33:25.000000 TerraVide-0.1.5/terravide/src/Preprocessing.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.1.5/terravide/src/__init__.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     5329 2023-04-15 00:07:47.000000 TerraVide-0.1.5/terravide/src/dataset.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1890 2023-04-14 22:26:22.000000 TerraVide-0.1.5/terravide/src/info.py
```

### Comparing `TerraVide-0.1.4/LICENSE.txt` & `TerraVide-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TerraVide-0.1.4/PKG-INFO` & `TerraVide-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.1.4
+Version: 0.1.5
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
 Author: Sarang Pramode
-Author-email: Sarang Pramode <sp872@cornell.edu>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `TerraVide-0.1.4/TerraVide.egg-info/PKG-INFO` & `TerraVide-0.1.5/TerraVide.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.1.4
+Version: 0.1.5
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
 Author: Sarang Pramode
-Author-email: Sarang Pramode <sp872@cornell.edu>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `TerraVide-0.1.4/setup.py` & `TerraVide-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,25 +25,33 @@
 #------------------------------------------------------------------------------------------------------------------------------
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+print(setuptools.find_packages())
+
 setuptools.setup(
     name="TerraVide",                     # This is the name of the package
-    version="0.1.4",                        #release version
+    version="0.1.5",                        #release version
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
-    py_modules=["info","dataset","GroundClassification","Preprocessing"]          # Name of the python package                   
+    py_modules=["info","dataset"],             # Name of the python package
+    install_requires=[              # Install other dependencies if any
+        "numpy",
+        "pandas",
+        "os",
+        "ftplib",
+    ]                     
 )
```

### Comparing `TerraVide-0.1.4/terravide/src/dataset.py` & `TerraVide-0.1.5/terravide/src/dataset.py`

 * *Files identical despite different names*

### Comparing `TerraVide-0.1.4/terravide/src/info.py` & `TerraVide-0.1.5/terravide/src/info.py`

 * *Files identical despite different names*

