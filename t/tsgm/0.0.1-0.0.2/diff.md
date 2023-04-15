# Comparing `tmp/tsgm-0.0.1.tar.gz` & `tmp/tsgm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsgm-0.0.1.tar", last modified: Wed Mar  1 14:18:38 2023, max compression
+gzip compressed data, was "tsgm-0.0.2.tar", last modified: Sat Apr 15 10:49:11 2023, max compression
```

## Comparing `tsgm-0.0.1.tar` & `tsgm-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,59 @@
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.710865 tsgm-0.0.1/
--rw-r--r--   0 e102949  (703710771) staff       (20)    11357 2022-06-03 08:35:55.000000 tsgm-0.0.1/LICENSE
--rw-r--r--   0 e102949  (703710771) staff       (20)      427 2023-03-01 14:18:38.711336 tsgm-0.0.1/PKG-INFO
--rw-r--r--   0 e102949  (703710771) staff       (20)     3079 2023-02-02 16:49:34.000000 tsgm-0.0.1/README.md
--rw-r--r--   0 e102949  (703710771) staff       (20)      339 2023-03-01 14:18:38.715598 tsgm-0.0.1/setup.cfg
--rw-r--r--   0 e102949  (703710771) staff       (20)     1572 2023-03-01 14:18:20.000000 tsgm-0.0.1/setup.py
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.386641 tsgm-0.0.1/tsgm/
--rw-r--r--   0 e102949  (703710771) staff       (20)      142 2022-06-03 08:40:33.000000 tsgm-0.0.1/tsgm/__init__.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     5094 2022-11-01 15:23:30.000000 tsgm-0.0.1/tsgm/dataset.py
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.443706 tsgm-0.0.1/tsgm/metrics/
--rw-r--r--   0 e102949  (703710771) staff       (20)      201 2022-06-03 08:40:33.000000 tsgm-0.0.1/tsgm/metrics/__init__.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     7260 2022-11-01 15:43:19.000000 tsgm-0.0.1/tsgm/metrics/metrics.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     1497 2022-10-12 14:09:58.000000 tsgm-0.0.1/tsgm/metrics/statistics.py
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.576895 tsgm-0.0.1/tsgm/models/
--rw-r--r--   0 e102949  (703710771) staff       (20)      235 2023-01-17 14:11:43.000000 tsgm-0.0.1/tsgm/models/__init__.py
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.604122 tsgm-0.0.1/tsgm/models/architectures/
--rw-r--r--   0 e102949  (703710771) staff       (20)       58 2022-08-23 14:33:28.000000 tsgm-0.0.1/tsgm/models/architectures/__init__.py
--rw-r--r--   0 e102949  (703710771) staff       (20)    23186 2022-12-13 14:49:47.000000 tsgm-0.0.1/tsgm/models/architectures/zoo.py
--rw-r--r--   0 e102949  (703710771) staff       (20)    10021 2023-03-01 11:07:04.000000 tsgm-0.0.1/tsgm/models/augmentations.py
--rw-r--r--   0 e102949  (703710771) staff       (20)    12265 2022-12-13 14:20:13.000000 tsgm-0.0.1/tsgm/models/cgan.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     8330 2022-11-29 18:14:34.000000 tsgm-0.0.1/tsgm/models/cvae.py
--rw-r--r--   0 e102949  (703710771) staff       (20)       67 2022-06-03 08:40:33.000000 tsgm-0.0.1/tsgm/models/gp.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     3302 2022-08-07 18:06:43.000000 tsgm-0.0.1/tsgm/models/monitors.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     1522 2022-09-09 13:31:25.000000 tsgm-0.0.1/tsgm/models/sts.py
--rw-r--r--   0 e102949  (703710771) staff       (20)    21860 2022-12-13 09:27:40.000000 tsgm-0.0.1/tsgm/models/timeGAN.py
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.627711 tsgm-0.0.1/tsgm/optimization/
--rw-r--r--   0 e102949  (703710771) staff       (20)       29 2022-06-03 08:40:33.000000 tsgm-0.0.1/tsgm/optimization/__init__.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     2984 2022-07-28 10:40:03.000000 tsgm-0.0.1/tsgm/optimization/abc.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     3224 2022-07-28 11:46:35.000000 tsgm-0.0.1/tsgm/simulator.py
--rw-r--r--   0 e102949  (703710771) staff       (20)      181 2022-06-03 08:40:33.000000 tsgm-0.0.1/tsgm/types.py
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.708897 tsgm-0.0.1/tsgm/utils/
--rw-r--r--   0 e102949  (703710771) staff       (20)      258 2023-03-01 13:25:40.000000 tsgm-0.0.1/tsgm/utils/__init__.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     1332 2022-07-29 08:47:58.000000 tsgm-0.0.1/tsgm/utils/data_processing.py
--rw-r--r--   0 e102949  (703710771) staff       (20)    11314 2022-11-09 09:32:15.000000 tsgm-0.0.1/tsgm/utils/datasets.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     2569 2023-03-01 10:31:58.000000 tsgm-0.0.1/tsgm/utils/dtw.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     2439 2022-08-23 14:45:00.000000 tsgm-0.0.1/tsgm/utils/file_utils.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     4538 2022-08-14 10:02:45.000000 tsgm-0.0.1/tsgm/utils/mmd.py
--rw-r--r--   0 e102949  (703710771) staff       (20)      783 2022-10-19 08:43:28.000000 tsgm-0.0.1/tsgm/utils/utils.py
--rw-r--r--   0 e102949  (703710771) staff       (20)     7829 2022-12-13 09:27:40.000000 tsgm-0.0.1/tsgm/utils/visualization.py
-drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-03-01 14:18:38.407198 tsgm-0.0.1/tsgm.egg-info/
--rw-r--r--   0 e102949  (703710771) staff       (20)      427 2023-03-01 14:18:38.000000 tsgm-0.0.1/tsgm.egg-info/PKG-INFO
--rw-r--r--   0 e102949  (703710771) staff       (20)      835 2023-03-01 14:18:38.000000 tsgm-0.0.1/tsgm.egg-info/SOURCES.txt
--rw-r--r--   0 e102949  (703710771) staff       (20)        1 2023-03-01 14:18:38.000000 tsgm-0.0.1/tsgm.egg-info/dependency_links.txt
--rw-r--r--   0 e102949  (703710771) staff       (20)       66 2023-03-01 14:18:38.000000 tsgm-0.0.1/tsgm.egg-info/entry_points.txt
--rw-r--r--   0 e102949  (703710771) staff       (20)       45 2023-03-01 14:18:38.000000 tsgm-0.0.1/tsgm.egg-info/requires.txt
--rw-r--r--   0 e102949  (703710771) staff       (20)        5 2023-03-01 14:18:38.000000 tsgm-0.0.1/tsgm.egg-info/top_level.txt
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.427285 tsgm-0.0.2/
+-rw-r--r--   0 e102949  (703710771) staff       (20)    11357 2022-06-03 08:35:55.000000 tsgm-0.0.2/LICENSE
+-rw-r--r--   0 e102949  (703710771) staff       (20)     4844 2023-04-15 10:49:11.427689 tsgm-0.0.2/PKG-INFO
+-rw-r--r--   0 e102949  (703710771) staff       (20)     4376 2023-04-15 10:43:50.000000 tsgm-0.0.2/README.md
+-rw-r--r--   0 e102949  (703710771) staff       (20)      339 2023-04-15 10:49:11.434536 tsgm-0.0.2/setup.cfg
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1969 2023-04-15 10:46:09.000000 tsgm-0.0.2/setup.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.326497 tsgm-0.0.2/tests/
+-rw-r--r--   0 e102949  (703710771) staff       (20)     2417 2022-08-07 18:17:53.000000 tsgm-0.0.2/tests/test_abc.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1747 2023-02-15 11:28:25.000000 tsgm-0.0.2/tests/test_augmentations.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     8989 2023-04-14 18:56:18.000000 tsgm-0.0.2/tests/test_cgan.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)      553 2022-06-03 08:40:29.000000 tsgm-0.0.2/tests/test_dataset.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     3612 2022-08-07 18:34:15.000000 tsgm-0.0.2/tests/test_downstream_models.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     4882 2022-11-01 15:28:31.000000 tsgm-0.0.2/tests/test_metrics.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1420 2022-08-07 18:17:48.000000 tsgm-0.0.2/tests/test_monitors.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)      394 2022-06-03 08:40:29.000000 tsgm-0.0.2/tests/test_simulator.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)      313 2022-06-03 08:40:29.000000 tsgm-0.0.2/tests/test_sts.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     2322 2022-10-15 18:38:56.000000 tsgm-0.0.2/tests/test_timegan.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     6039 2022-11-09 09:28:21.000000 tsgm-0.0.2/tests/test_utils.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1999 2022-06-03 08:40:29.000000 tsgm-0.0.2/tests/test_vae.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)      801 2022-06-03 08:40:29.000000 tsgm-0.0.2/tests/test_zoo.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.333042 tsgm-0.0.2/tsgm/
+-rw-r--r--   0 e102949  (703710771) staff       (20)      142 2022-06-03 08:40:33.000000 tsgm-0.0.2/tsgm/__init__.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     5094 2022-11-01 15:23:30.000000 tsgm-0.0.2/tsgm/dataset.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.353494 tsgm-0.0.2/tsgm/metrics/
+-rw-r--r--   0 e102949  (703710771) staff       (20)      201 2022-06-03 08:40:33.000000 tsgm-0.0.2/tsgm/metrics/__init__.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     7260 2022-11-01 15:43:19.000000 tsgm-0.0.2/tsgm/metrics/metrics.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1497 2022-10-12 14:09:58.000000 tsgm-0.0.2/tsgm/metrics/statistics.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.373714 tsgm-0.0.2/tsgm/models/
+-rw-r--r--   0 e102949  (703710771) staff       (20)      235 2023-01-17 14:11:43.000000 tsgm-0.0.2/tsgm/models/__init__.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.383715 tsgm-0.0.2/tsgm/models/architectures/
+-rw-r--r--   0 e102949  (703710771) staff       (20)       58 2022-08-23 14:33:28.000000 tsgm-0.0.2/tsgm/models/architectures/__init__.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)    23186 2022-12-13 14:49:47.000000 tsgm-0.0.2/tsgm/models/architectures/zoo.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)    10021 2023-03-01 11:07:04.000000 tsgm-0.0.2/tsgm/models/augmentations.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)    12416 2023-04-14 18:55:20.000000 tsgm-0.0.2/tsgm/models/cgan.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     8330 2022-11-29 18:14:34.000000 tsgm-0.0.2/tsgm/models/cvae.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)       67 2022-06-03 08:40:33.000000 tsgm-0.0.2/tsgm/models/gp.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     3302 2022-08-07 18:06:43.000000 tsgm-0.0.2/tsgm/models/monitors.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1522 2022-09-09 13:31:25.000000 tsgm-0.0.2/tsgm/models/sts.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)    21724 2023-04-14 18:35:04.000000 tsgm-0.0.2/tsgm/models/timeGAN.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.407144 tsgm-0.0.2/tsgm/optimization/
+-rw-r--r--   0 e102949  (703710771) staff       (20)       29 2022-06-03 08:40:33.000000 tsgm-0.0.2/tsgm/optimization/__init__.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     2984 2022-07-28 10:40:03.000000 tsgm-0.0.2/tsgm/optimization/abc.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     3224 2022-07-28 11:46:35.000000 tsgm-0.0.2/tsgm/simulator.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)      181 2022-06-03 08:40:33.000000 tsgm-0.0.2/tsgm/types.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.424830 tsgm-0.0.2/tsgm/utils/
+-rw-r--r--   0 e102949  (703710771) staff       (20)      258 2023-03-01 13:25:40.000000 tsgm-0.0.2/tsgm/utils/__init__.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1332 2022-07-29 08:47:58.000000 tsgm-0.0.2/tsgm/utils/data_processing.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)    11314 2022-11-09 09:32:15.000000 tsgm-0.0.2/tsgm/utils/datasets.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     2439 2023-03-16 11:00:17.000000 tsgm-0.0.2/tsgm/utils/file_utils.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     4538 2022-08-14 10:02:45.000000 tsgm-0.0.2/tsgm/utils/mmd.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)      783 2022-10-19 08:43:28.000000 tsgm-0.0.2/tsgm/utils/utils.py
+-rw-r--r--   0 e102949  (703710771) staff       (20)     7829 2022-12-13 09:27:40.000000 tsgm-0.0.2/tsgm/utils/visualization.py
+drwxr-xr-x   0 e102949  (703710771) staff       (20)        0 2023-04-15 10:49:11.347258 tsgm-0.0.2/tsgm.egg-info/
+-rw-r--r--   0 e102949  (703710771) staff       (20)     4844 2023-04-15 10:49:11.000000 tsgm-0.0.2/tsgm.egg-info/PKG-INFO
+-rw-r--r--   0 e102949  (703710771) staff       (20)     1101 2023-04-15 10:49:11.000000 tsgm-0.0.2/tsgm.egg-info/SOURCES.txt
+-rw-r--r--   0 e102949  (703710771) staff       (20)        1 2023-04-15 10:49:11.000000 tsgm-0.0.2/tsgm.egg-info/dependency_links.txt
+-rw-r--r--   0 e102949  (703710771) staff       (20)       66 2023-04-15 10:49:11.000000 tsgm-0.0.2/tsgm.egg-info/entry_points.txt
+-rw-r--r--   0 e102949  (703710771) staff       (20)      117 2023-04-15 10:49:11.000000 tsgm-0.0.2/tsgm.egg-info/requires.txt
+-rw-r--r--   0 e102949  (703710771) staff       (20)        5 2023-04-15 10:49:11.000000 tsgm-0.0.2/tsgm.egg-info/top_level.txt
```

### Comparing `tsgm-0.0.1/LICENSE` & `tsgm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/setup.py` & `tsgm-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,29 +31,45 @@
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 
+def read_file(filename: str) -> str:
+    with open(filename, encoding="utf-8") as f:
+        return f.read().strip()
+
+
+readme_text = read_file("README.md")
+
+
 setup(name='tsgm',
-      version='0.0.1',
+      version='0.0.2',
       description='Time Series Generative Modelling Framework',
       author=author,
       author_email='',
       maintainer=author,
       maintainer_email='',
       url=url,
       download_url='',
       keywords=keywords,
-      long_description="",
+      long_description=readme_text,
+      long_description_content_type='text/markdown',
       license=license,
       entry_points={
         "console_scripts": ["tsgm-gd=cli.gd:main", "tsgm-eval=cli.eval:main"],
       },
       install_requires=[
-          "tensorflow==2.9.1",
-          "scipy>=1.7.3",
-          "numpy>=1.21.6",
+          "scipy",
+          "numpy",          
+          "networkx",
+          "seaborn",
+          "scikit-learn",
+          "prettytable",
+          "yfinance",
+          "tqdm",
+          "tensorflow >= 2.4.0",
+          "tensorflow-probability >= 0.12.0",
       ],
       package_data={'tsgm': ['README.md']},
       packages=find_packages())
```

### Comparing `tsgm-0.0.1/tsgm/dataset.py` & `tsgm-0.0.2/tsgm/dataset.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/metrics/metrics.py` & `tsgm-0.0.2/tsgm/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/metrics/statistics.py` & `tsgm-0.0.2/tsgm/metrics/statistics.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/models/architectures/zoo.py` & `tsgm-0.0.2/tsgm/models/architectures/zoo.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/models/augmentations.py` & `tsgm-0.0.2/tsgm/models/augmentations.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/models/cgan.py` & `tsgm-0.0.2/tsgm/models/cgan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import tensorflow as tf
 from tensorflow import keras
-import tensorflow_privacy as tf_privacy
+try:
+    import tensorflow_privacy as tf_privacy
+    __tf_privacy_available = True
+except ModuleNotFoundError:
+    __tf_privacy_available = False
 
 import logging
 
 import tsgm
 
 
 logger = logging.getLogger('models')
 logger.setLevel(logging.DEBUG)
 
 
 def _is_dp_optimizer(optimizer: keras.optimizers.Optimizer) -> bool:
-    return isinstance(optimizer, tf_privacy.DPKerasAdagradOptimizer) or \
-        isinstance(optimizer, tf_privacy.DPKerasAdamOptimizer) or \
-        isinstance(optimizer, tf_privacy.DPKerasSGDOptimizer)
+    return __tf_privacy_available \
+        and (isinstance(optimizer, tf_privacy.DPKerasAdagradOptimizer)
+             or isinstance(optimizer, tf_privacy.DPKerasAdamOptimizer)
+             or isinstance(optimizer, tf_privacy.DPKerasSGDOptimizer))
 
 
 class GAN(keras.Model):
     """
     GAN implementation for unlabeled time series.
     """
     def __init__(self, discriminator: keras.Model, generator: keras.Model, latent_dim: int):
```

### Comparing `tsgm-0.0.1/tsgm/models/cvae.py` & `tsgm-0.0.2/tsgm/models/cvae.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/models/monitors.py` & `tsgm-0.0.2/tsgm/models/monitors.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/models/sts.py` & `tsgm-0.0.2/tsgm/models/sts.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/models/timeGAN.py` & `tsgm-0.0.2/tsgm/models/timeGAN.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.python.types.core import TensorLike
 import numpy as np
-from copy import deepcopy
 from tqdm import tqdm, trange
 from collections import OrderedDict
 import typing
 
 import logging
 
 from tsgm.models.architectures.zoo import BasicRecurrentArchitecture
@@ -124,27 +123,24 @@
             network_type=self.module,
             name="Generator",
         ).build()
 
         # ----------------------------
         # Optimizers: call .compile() to set them
         # ----------------------------
-        DEFAULT_ADAM = keras.optimizers.Adam()
-        self.autoencoder_opt = deepcopy(DEFAULT_ADAM)
-        self.adversarialsup_opt = deepcopy(DEFAULT_ADAM)
-        self.generator_opt = deepcopy(DEFAULT_ADAM)
-        self.embedder_opt = deepcopy(DEFAULT_ADAM)
-        self.discriminator_opt = deepcopy(DEFAULT_ADAM)
+        self.autoencoder_opt = keras.optimizers.Adam()
+        self.adversarialsup_opt = keras.optimizers.Adam()
+        self.generator_opt = keras.optimizers.Adam()
+        self.embedder_opt = keras.optimizers.Adam()
+        self.discriminator_opt = keras.optimizers.Adam()
         # ----------------------------
         # Loss functions: call .compile() to set them
         # ----------------------------
-        DEFAULT_MSE = keras.losses.MeanSquaredError()
-        DEFAULT_BCE = keras.losses.BinaryCrossentropy()
-        self._mse = DEFAULT_MSE
-        self._bce = DEFAULT_BCE
+        self._mse = keras.losses.MeanSquaredError()
+        self._bce = keras.losses.BinaryCrossentropy()
 
         # --------------------------
         # All losses: will be populated in .fit()
         # --------------------------
         self.training_losses_history = LossTracker()
 
         # --------------------------
```

### Comparing `tsgm-0.0.1/tsgm/optimization/abc.py` & `tsgm-0.0.2/tsgm/optimization/abc.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/simulator.py` & `tsgm-0.0.2/tsgm/simulator.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/utils/data_processing.py` & `tsgm-0.0.2/tsgm/utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/utils/datasets.py` & `tsgm-0.0.2/tsgm/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/utils/file_utils.py` & `tsgm-0.0.2/tsgm/utils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         to_path, _ = os.path.splitext(from_path)
         to_path = os.path.dirname(to_path)
 
     extractor(from_path, to_path, pwd=pwd)
     os.remove(from_path)
 
 
-def download(url: str, path: str, md5: typing.Optional[str] = None, max_attempt: int = 2) -> None:
+def download(url: str, path: str, md5: typing.Optional[str] = None, max_attempt: int = 3) -> None:
     logger.info(f"### Downloading from {url} ###")
     os.makedirs(path, exist_ok=True)
     resource_name = url.split("/")[-1]
     path = os.path.join(path, resource_name)
     for attempt in range(max_attempt):
         logger.info(f"Attempt {attempt + 1} / {max_attempt}")
         urllib.request.urlretrieve(urllib.parse.quote(url, safe=":/"), path)
```

### Comparing `tsgm-0.0.1/tsgm/utils/mmd.py` & `tsgm-0.0.2/tsgm/utils/mmd.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/utils/utils.py` & `tsgm-0.0.2/tsgm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm/utils/visualization.py` & `tsgm-0.0.2/tsgm/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.1/tsgm.egg-info/SOURCES.txt` & `tsgm-0.0.2/tsgm.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+tests/test_abc.py
+tests/test_augmentations.py
+tests/test_cgan.py
+tests/test_dataset.py
+tests/test_downstream_models.py
+tests/test_metrics.py
+tests/test_monitors.py
+tests/test_simulator.py
+tests/test_sts.py
+tests/test_timegan.py
+tests/test_utils.py
+tests/test_vae.py
+tests/test_zoo.py
 tsgm/__init__.py
 tsgm/dataset.py
 tsgm/simulator.py
 tsgm/types.py
 tsgm.egg-info/PKG-INFO
 tsgm.egg-info/SOURCES.txt
 tsgm.egg-info/dependency_links.txt
@@ -26,12 +39,11 @@
 tsgm/models/architectures/__init__.py
 tsgm/models/architectures/zoo.py
 tsgm/optimization/__init__.py
 tsgm/optimization/abc.py
 tsgm/utils/__init__.py
 tsgm/utils/data_processing.py
 tsgm/utils/datasets.py
-tsgm/utils/dtw.py
 tsgm/utils/file_utils.py
 tsgm/utils/mmd.py
 tsgm/utils/utils.py
 tsgm/utils/visualization.py
```

