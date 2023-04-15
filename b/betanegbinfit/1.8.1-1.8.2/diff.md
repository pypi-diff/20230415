# Comparing `tmp/betanegbinfit-1.8.1.tar.gz` & `tmp/betanegbinfit-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanegbinfit-1.8.1.tar", last modified: Tue Apr  4 13:55:26 2023, max compression
+gzip compressed data, was "betanegbinfit-1.8.2.tar", last modified: Sat Apr 15 17:19:59 2023, max compression
```

## Comparing `betanegbinfit-1.8.1.tar` & `betanegbinfit-1.8.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-04 13:55:26.990703 betanegbinfit-1.8.1/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-04 13:55:26.990703 betanegbinfit-1.8.1/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.8.1/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-04 13:55:26.987370 betanegbinfit-1.8.1/betanegbinfit/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      726 2023-04-04 13:54:18.000000 betanegbinfit-1.8.1/betanegbinfit/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/betacdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/betainc.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/bridge_mixalime.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/cdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/create.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    32670 2023-04-04 13:54:13.000000 betanegbinfit-1.8.1/betanegbinfit/distributions.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/hyp.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-04 13:55:26.990703 betanegbinfit-1.8.1/betanegbinfit/models/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/models/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/models/model.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/models/model_line.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/models/model_line_lrt.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/models/model_mixture.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/models/model_mixtures.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/models/model_window.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/stats.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-03-30 18:19:57.000000 betanegbinfit-1.8.1/betanegbinfit/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-04 13:55:26.990703 betanegbinfit-1.8.1/betanegbinfit.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-04 13:55:26.000000 betanegbinfit-1.8.1/betanegbinfit.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-04-04 13:55:26.000000 betanegbinfit-1.8.1/betanegbinfit.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-04-04 13:55:26.000000 betanegbinfit-1.8.1/betanegbinfit.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-04-04 13:55:26.000000 betanegbinfit-1.8.1/betanegbinfit.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-04-04 13:55:26.000000 betanegbinfit-1.8.1/betanegbinfit.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-04-04 13:55:26.990703 betanegbinfit-1.8.1/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)      912 2022-11-01 11:37:53.000000 betanegbinfit-1.8.1/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.8.2/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/betanegbinfit/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      739 2023-04-15 17:17:28.000000 betanegbinfit-1.8.2/betanegbinfit/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       46 2023-04-15 17:17:43.000000 betanegbinfit-1.8.2/betanegbinfit/__version__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/betacdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/betainc.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/bridge_mixalime.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/cdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/create.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    32670 2023-04-04 13:54:13.000000 betanegbinfit-1.8.2/betanegbinfit/distributions.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/hyp.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/betanegbinfit/models/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_line.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_line_lrt.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_mixture.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_mixtures.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_window.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/stats.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/betanegbinfit.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      806 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      924 2023-04-15 17:18:42.000000 betanegbinfit-1.8.2/setup.py
```

### Comparing `betanegbinfit-1.8.1/PKG-INFO` & `betanegbinfit-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.8.1
+Version: 1.8.2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `betanegbinfit-1.8.1/README.md` & `betanegbinfit-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/__init__.py` & `betanegbinfit-1.8.2/betanegbinfit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .__version__ import __version__
 import warnings
 # This will omit annoying FutureWarnings by JAX and RutimeWarnings caused by
 # estimates being clipped at bounds.
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
 
 
@@ -17,11 +18,8 @@
 from . import bridge_mixalime
 from .utils import run
 from gmpy2 import get_context
 from mpmath import mp
 
 _precision = 1024
 get_context().precision = _precision
-mp.prec = _precision
-
-
-__version__ = "1.8.1"
+mp.prec = _precision
```

### Comparing `betanegbinfit-1.8.1/betanegbinfit/betacdnb.py` & `betanegbinfit-1.8.2/betanegbinfit/betacdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/betainc.py` & `betanegbinfit-1.8.2/betanegbinfit/betainc.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/bridge_mixalime.py` & `betanegbinfit-1.8.2/betanegbinfit/bridge_mixalime.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/cdnb.py` & `betanegbinfit-1.8.2/betanegbinfit/cdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/combine.py` & `betanegbinfit-1.8.2/betanegbinfit/combine.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/create.py` & `betanegbinfit-1.8.2/betanegbinfit/create.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/distributions.py` & `betanegbinfit-1.8.2/betanegbinfit/distributions.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/hyp.py` & `betanegbinfit-1.8.2/betanegbinfit/hyp.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/models/model.py` & `betanegbinfit-1.8.2/betanegbinfit/models/model.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/models/model_line.py` & `betanegbinfit-1.8.2/betanegbinfit/models/model_line.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/models/model_line_lrt.py` & `betanegbinfit-1.8.2/betanegbinfit/models/model_line_lrt.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/models/model_mixture.py` & `betanegbinfit-1.8.2/betanegbinfit/models/model_mixture.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/models/model_mixtures.py` & `betanegbinfit-1.8.2/betanegbinfit/models/model_mixtures.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/models/model_window.py` & `betanegbinfit-1.8.2/betanegbinfit/models/model_window.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/plot.py` & `betanegbinfit-1.8.2/betanegbinfit/plot.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/stats.py` & `betanegbinfit-1.8.2/betanegbinfit/stats.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/tests.py` & `betanegbinfit-1.8.2/betanegbinfit/tests.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit/utils.py` & `betanegbinfit-1.8.2/betanegbinfit/utils.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.1/betanegbinfit.egg-info/PKG-INFO` & `betanegbinfit-1.8.2/betanegbinfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.8.1
+Version: 1.8.2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `betanegbinfit-1.8.1/betanegbinfit.egg-info/SOURCES.txt` & `betanegbinfit-1.8.2/betanegbinfit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 betanegbinfit/__init__.py
+betanegbinfit/__version__.py
 betanegbinfit/betacdnb.py
 betanegbinfit/betainc.py
 betanegbinfit/bridge_mixalime.py
 betanegbinfit/cdnb.py
 betanegbinfit/combine.py
 betanegbinfit/create.py
 betanegbinfit/distributions.py
```

### Comparing `betanegbinfit-1.8.1/setup.py` & `betanegbinfit-1.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-from betanegbinfit import __version__
+from betanegbinfit.__version__ import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(	
       install_requires=['scipy', 'numpy', 'pandas', 'jax', 'jaxlib', 'gmpy2', 'mpmath'],
       include_package_data=True,
```

