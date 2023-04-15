# Comparing `tmp/splashlab-0.0.8.tar.gz` & `tmp/splashlab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splashlab-0.0.8.tar", last modified: Sun Feb 12 19:48:14 2023, max compression
+gzip compressed data, was "splashlab-0.0.9.tar", last modified: Thu Feb 23 06:22:45 2023, max compression
```

## Comparing `splashlab-0.0.8.tar` & `splashlab-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 19:48:14.115752 splashlab-0.0.8/
--rw-rw-rw-   0        0        0     1087 2023-02-12 17:06:38.000000 splashlab-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      682 2023-02-12 19:48:14.115752 splashlab-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-02-12 16:23:56.000000 splashlab-0.0.8/README.md
--rw-rw-rw-   0        0        0       86 2023-02-12 19:48:14.127263 splashlab-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1687 2023-02-12 19:47:20.000000 splashlab-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 19:48:14.095330 splashlab-0.0.8/splashlab/
--rw-rw-rw-   0        0        0        0 2023-02-12 18:31:45.000000 splashlab-0.0.8/splashlab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-12 19:48:14.115752 splashlab-0.0.8/splashlab/dimensional_analysis/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:34:04.000000 splashlab-0.0.8/splashlab/dimensional_analysis/__init__.py
--rw-rw-rw-   0        0        0     2238 2023-02-09 10:04:02.000000 splashlab-0.0.8/splashlab/dimensional_analysis/convert.py
--rw-rw-rw-   0        0        0     1954 2023-02-12 19:46:42.000000 splashlab-0.0.8/splashlab/dimensional_analysis/data_reader.py
--rw-rw-rw-   0        0        0     2155 2023-02-12 19:46:42.000000 splashlab-0.0.8/splashlab/dimensional_analysis/fluid_types.py
--rw-rw-rw-   0        0        0     1369 2023-02-12 19:46:42.000000 splashlab-0.0.8/splashlab/dimensional_analysis/group_of_parameter.py
--rw-rw-rw-   0        0        0     3597 2023-02-12 19:46:42.000000 splashlab-0.0.8/splashlab/dimensional_analysis/parameter.py
--rw-rw-rw-   0        0        0     7699 2023-02-12 19:46:42.000000 splashlab-0.0.8/splashlab/dimensional_analysis/unit.py
--rw-rw-rw-   0        0        0      897 2023-02-09 10:04:02.000000 splashlab-0.0.8/splashlab/dimensional_analysis/util.py
--rw-rw-rw-   0        0        0       86 2023-02-12 19:34:01.000000 splashlab-0.0.8/splashlab/test.py
-drwxrwxrwx   0        0        0        0 2023-02-12 19:48:14.112108 splashlab-0.0.8/splashlab.egg-info/
--rw-rw-rw-   0        0        0      682 2023-02-12 19:48:14.000000 splashlab-0.0.8/splashlab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2023-02-12 19:48:14.000000 splashlab-0.0.8/splashlab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 19:48:14.000000 splashlab-0.0.8/splashlab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-02-12 19:48:14.000000 splashlab-0.0.8/splashlab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-12 19:48:14.000000 splashlab-0.0.8/splashlab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.491730 splashlab-0.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-02-12 17:06:38.000000 splashlab-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      833 2023-02-23 06:22:45.491730 splashlab-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-02-12 16:23:56.000000 splashlab-0.0.9/README.md
+-rw-rw-rw-   0        0        0       86 2023-02-23 06:22:45.492853 splashlab-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1927 2023-02-23 06:22:01.000000 splashlab-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.395456 splashlab-0.0.9/splashlab/
+-rw-rw-rw-   0        0        0        0 2023-02-12 18:31:45.000000 splashlab-0.0.9/splashlab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.413474 splashlab-0.0.9/splashlab/computer_vision/
+-rw-rw-rw-   0        0        0        0 2023-02-23 05:59:44.000000 splashlab-0.0.9/splashlab/computer_vision/__init__.py
+-rw-rw-rw-   0        0        0     6819 2023-02-20 18:20:05.000000 splashlab-0.0.9/splashlab/computer_vision/image_util.py
+drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.475057 splashlab-0.0.9/splashlab/dimensional_analysis/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:34:04.000000 splashlab-0.0.9/splashlab/dimensional_analysis/__init__.py
+-rw-rw-rw-   0        0        0     2238 2023-02-09 10:04:02.000000 splashlab-0.0.9/splashlab/dimensional_analysis/convert.py
+-rw-rw-rw-   0        0        0     1954 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/data_reader.py
+-rw-rw-rw-   0        0        0     2155 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/fluid_types.py
+-rw-rw-rw-   0        0        0     1369 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/group_of_parameter.py
+-rw-rw-rw-   0        0        0     3597 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/parameter.py
+-rw-rw-rw-   0        0        0     7699 2023-02-12 19:46:42.000000 splashlab-0.0.9/splashlab/dimensional_analysis/unit.py
+-rw-rw-rw-   0        0        0      897 2023-02-09 10:04:02.000000 splashlab-0.0.9/splashlab/dimensional_analysis/util.py
+drwxrwxrwx   0        0        0        0 2023-02-23 06:22:45.413474 splashlab-0.0.9/splashlab.egg-info/
+-rw-rw-rw-   0        0        0      833 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-02-23 06:22:45.000000 splashlab-0.0.9/splashlab.egg-info/top_level.txt
```

### Comparing `splashlab-0.0.8/LICENSE` & `splashlab-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/PKG-INFO` & `splashlab-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: splashlab
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for fluid mechanic experimentalists
 Home-page: https://github.com/FluidsLab/SplashLab
 Download-URL: https://github.com/FluidsLab/SplashLab/archive/refs/tags/v0.0.8.tar.gz
 Author: Spencer Truman
 Author-email: trumans24@gmail.com
 License: MIT
 Keywords: Fluid Dynamics,Experiment
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# SplashLab
+Python packages intended to assist with experimental research in the field of fluid dynamics.
```

### Comparing `splashlab-0.0.8/setup.py` & `splashlab-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from distutils.core import setup
+with open("README.md", "r", encoding = "utf-8") as fh:
+    long_description = fh.read()
+
 setup(
   name = 'splashlab',         # How you named your package folder (MyLib)
-  packages = ['splashlab', 'splashlab.dimensional_analysis'],   # Chose the same as "name"
-  version = 'v0.0.8',      # Start with a small number and increase it with every change you make
+  long_description = long_description,
+  long_description_content_type = 'text/markdown',
+  packages = ['splashlab', 'splashlab.dimensional_analysis', 'splashlab.computer_vision'],   # Chose the same as "name"
+  version = 'v0.0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A package for fluid mechanic experimentalists',   # Give a short description about your library
   author = 'Spencer Truman',                   # Type in your name
   author_email = 'trumans24@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/FluidsLab/SplashLab',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/FluidsLab/SplashLab/archive/refs/tags/v0.0.8.tar.gz',    # I explain this later on
   keywords = ['Fluid Dynamics', 'Experiment'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'pandas',
           'sympy',
           'matplotlib',
+          'opencv-python'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

### Comparing `splashlab-0.0.8/splashlab/dimensional_analysis/convert.py` & `splashlab-0.0.9/splashlab/dimensional_analysis/convert.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/splashlab/dimensional_analysis/data_reader.py` & `splashlab-0.0.9/splashlab/dimensional_analysis/data_reader.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/splashlab/dimensional_analysis/fluid_types.py` & `splashlab-0.0.9/splashlab/dimensional_analysis/fluid_types.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/splashlab/dimensional_analysis/group_of_parameter.py` & `splashlab-0.0.9/splashlab/dimensional_analysis/group_of_parameter.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/splashlab/dimensional_analysis/parameter.py` & `splashlab-0.0.9/splashlab/dimensional_analysis/parameter.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/splashlab/dimensional_analysis/unit.py` & `splashlab-0.0.9/splashlab/dimensional_analysis/unit.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/splashlab/dimensional_analysis/util.py` & `splashlab-0.0.9/splashlab/dimensional_analysis/util.py`

 * *Files identical despite different names*

### Comparing `splashlab-0.0.8/splashlab.egg-info/PKG-INFO` & `splashlab-0.0.9/splashlab.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: splashlab
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for fluid mechanic experimentalists
 Home-page: https://github.com/FluidsLab/SplashLab
 Download-URL: https://github.com/FluidsLab/SplashLab/archive/refs/tags/v0.0.8.tar.gz
 Author: Spencer Truman
 Author-email: trumans24@gmail.com
 License: MIT
 Keywords: Fluid Dynamics,Experiment
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# SplashLab
+Python packages intended to assist with experimental research in the field of fluid dynamics.
```

### Comparing `splashlab-0.0.8/splashlab.egg-info/SOURCES.txt` & `splashlab-0.0.9/splashlab.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 splashlab/__init__.py
-splashlab/test.py
 splashlab.egg-info/PKG-INFO
 splashlab.egg-info/SOURCES.txt
 splashlab.egg-info/dependency_links.txt
 splashlab.egg-info/requires.txt
 splashlab.egg-info/top_level.txt
+splashlab/computer_vision/__init__.py
+splashlab/computer_vision/image_util.py
 splashlab/dimensional_analysis/__init__.py
 splashlab/dimensional_analysis/convert.py
 splashlab/dimensional_analysis/data_reader.py
 splashlab/dimensional_analysis/fluid_types.py
 splashlab/dimensional_analysis/group_of_parameter.py
 splashlab/dimensional_analysis/parameter.py
 splashlab/dimensional_analysis/unit.py
```

