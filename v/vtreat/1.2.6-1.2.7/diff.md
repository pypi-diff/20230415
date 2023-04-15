# Comparing `tmp/vtreat-1.2.6.tar.gz` & `tmp/vtreat-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtreat-1.2.6.tar", last modified: Wed Dec 14 00:33:12 2022, max compression
+gzip compressed data, was "vtreat-1.2.7.tar", last modified: Fri Apr  7 18:42:46 2023, max compression
```

## Comparing `vtreat-1.2.6.tar` & `vtreat-1.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2022-12-14 00:33:12.347358 vtreat-1.2.6/
--rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:11:34.000000 vtreat-1.2.6/LICENSE
--rw-r--r--   0 johnmount   (501) staff       (20)     3207 2022-12-14 00:33:12.347089 vtreat-1.2.6/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)    35907 2022-01-27 17:04:33.000000 vtreat-1.2.6/README.md
--rw-r--r--   0 johnmount   (501) staff       (20)       38 2022-12-14 00:33:12.347450 vtreat-1.2.6/setup.cfg
--rw-r--r--   0 johnmount   (501) staff       (20)     3812 2022-12-14 00:16:11.000000 vtreat-1.2.6/setup.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2022-12-14 00:33:12.345076 vtreat-1.2.6/vtreat/
--rw-r--r--   0 johnmount   (501) staff       (20)     2643 2022-12-14 00:16:05.000000 vtreat-1.2.6/vtreat/__init__.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3699 2022-01-27 17:04:33.000000 vtreat-1.2.6/vtreat/cross_plan.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3632 2022-09-12 18:41:57.000000 vtreat-1.2.6/vtreat/effect_scaler.py
--rw-r--r--   0 johnmount   (501) staff       (20)     8158 2022-01-27 17:04:33.000000 vtreat-1.2.6/vtreat/stats_utils.py
--rw-r--r--   0 johnmount   (501) staff       (20)     1074 2022-01-27 17:04:33.000000 vtreat-1.2.6/vtreat/transform.py
--rw-r--r--   0 johnmount   (501) staff       (20)     8629 2022-01-27 17:04:33.000000 vtreat-1.2.6/vtreat/util.py
--rw-r--r--   0 johnmount   (501) staff       (20)    29728 2022-01-27 17:04:33.000000 vtreat-1.2.6/vtreat/vtreat_api.py
--rw-r--r--   0 johnmount   (501) staff       (20)     8031 2022-01-27 17:04:33.000000 vtreat-1.2.6/vtreat/vtreat_db_adapter.py
--rw-r--r--   0 johnmount   (501) staff       (20)    62607 2022-01-27 17:04:33.000000 vtreat-1.2.6/vtreat/vtreat_impl.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2022-12-14 00:33:12.346730 vtreat-1.2.6/vtreat.egg-info/
--rw-r--r--   0 johnmount   (501) staff       (20)     3207 2022-12-14 00:33:12.000000 vtreat-1.2.6/vtreat.egg-info/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      367 2022-12-14 00:33:12.000000 vtreat-1.2.6/vtreat.egg-info/SOURCES.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        1 2022-12-14 00:33:12.000000 vtreat-1.2.6/vtreat.egg-info/dependency_links.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       52 2022-12-14 00:33:12.000000 vtreat-1.2.6/vtreat.egg-info/requires.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        7 2022-12-14 00:33:12.000000 vtreat-1.2.6/vtreat.egg-info/top_level.txt
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:42:46.476559 vtreat-1.2.7/
+-rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:11:34.000000 vtreat-1.2.7/LICENSE
+-rw-r--r--   0 johnmount   (501) staff       (20)     3207 2023-04-07 18:42:46.476269 vtreat-1.2.7/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)    35907 2022-01-27 17:04:33.000000 vtreat-1.2.7/README.md
+-rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-07 18:42:46.476656 vtreat-1.2.7/setup.cfg
+-rw-r--r--   0 johnmount   (501) staff       (20)     3812 2022-12-14 00:59:42.000000 vtreat-1.2.7/setup.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:42:46.472226 vtreat-1.2.7/vtreat/
+-rw-r--r--   0 johnmount   (501) staff       (20)     2643 2022-12-14 00:59:35.000000 vtreat-1.2.7/vtreat/__init__.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3699 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/cross_plan.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3632 2022-09-12 18:41:57.000000 vtreat-1.2.7/vtreat/effect_scaler.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     8158 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/stats_utils.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     1074 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/transform.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     8629 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/util.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    29728 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/vtreat_api.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     8031 2022-12-24 16:28:04.000000 vtreat-1.2.7/vtreat/vtreat_db_adapter.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    62607 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/vtreat_impl.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:42:46.475857 vtreat-1.2.7/vtreat.egg-info/
+-rw-r--r--   0 johnmount   (501) staff       (20)     3207 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      367 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       52 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/requires.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        7 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/top_level.txt
```

### Comparing `vtreat-1.2.6/LICENSE` & `vtreat-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/PKG-INFO` & `vtreat-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtreat
-Version: 1.2.6
+Version: 1.2.7
 Summary: vtreat is a pandas.DataFrame processor/conditioner that prepares real-world data for predictive modeling in a statistically sound manner. 
 Home-page: https://github.com/WinVector/pyvtreat
 Author: John Mount, Nina Zumel
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `vtreat-1.2.6/README.md` & `vtreat-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/setup.py` & `vtreat-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 as a [`Python`/`Pandas` package](https://github.com/WinVector/vtreat),
 and also as an [`R` package](https://github.com/WinVector/vtreat).
 """
 
 
 setuptools.setup(
     name='vtreat',
-    version='1.2.6',
+    version='1.2.7',
     author='John Mount, Nina Zumel',
     author_email='jmount@win-vector.com',
     url='https://github.com/WinVector/pyvtreat',
     packages=setuptools.find_packages(where='.', exclude=['tests', 'Examples']),
     install_requires=[
         'numpy',
         'pandas',
```

### Comparing `vtreat-1.2.6/vtreat/__init__.py` & `vtreat-1.2.7/vtreat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # noinspection PyUnresolvedReferences
 import numpy
 
 from vtreat.vtreat_api import *
 
 __docformat__ = "restructuredtext"
-__version__ = "1.2.6"
+__version__ = "1.2.7"
 
 __doc__ = """
 This<https://github.com/WinVector/pyvtreat> is the Python version of the vtreat data preparation system
 (also available as an R package<https://winvector.github.io/vtreat/>.
 
 vtreat is a DataFrame processor/conditioner that prepares
 real-world data for supervised machine learning or predictive modeling
```

### Comparing `vtreat-1.2.6/vtreat/cross_plan.py` & `vtreat-1.2.7/vtreat/cross_plan.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat/effect_scaler.py` & `vtreat-1.2.7/vtreat/effect_scaler.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat/stats_utils.py` & `vtreat-1.2.7/vtreat/stats_utils.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat/transform.py` & `vtreat-1.2.7/vtreat/transform.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat/util.py` & `vtreat-1.2.7/vtreat/util.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat/vtreat_api.py` & `vtreat-1.2.7/vtreat/vtreat_api.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat/vtreat_db_adapter.py` & `vtreat-1.2.7/vtreat/vtreat_db_adapter.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat/vtreat_impl.py` & `vtreat-1.2.7/vtreat/vtreat_impl.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.6/vtreat.egg-info/PKG-INFO` & `vtreat-1.2.7/vtreat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtreat
-Version: 1.2.6
+Version: 1.2.7
 Summary: vtreat is a pandas.DataFrame processor/conditioner that prepares real-world data for predictive modeling in a statistically sound manner. 
 Home-page: https://github.com/WinVector/pyvtreat
 Author: John Mount, Nina Zumel
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

