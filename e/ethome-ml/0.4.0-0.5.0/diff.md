# Comparing `tmp/ethome-ml-0.4.0.tar.gz` & `tmp/ethome-ml-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/blansdel/projects/ethome/dist/.tmp-bicpah43/ethome-ml-0.4.0.tar", last modified: Fri Feb 10 23:05:07 2023, max compression
+gzip compressed data, was "ethome-ml-0.5.0.tar", last modified: Sat Apr 15 02:30:39 2023, max compression
```

## Comparing `ethome-ml-0.4.0.tar` & `ethome-ml-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.874086 ethome-ml-0.4.0/
--rw-r--r--   0 blansdel (66183) domain users (76937)     1069 2022-09-22 06:23:05.000000 ethome-ml-0.4.0/LICENSE
--rw-r--r--   0 blansdel (66183) domain users (76937)      192 2022-09-22 06:23:05.000000 ethome-ml-0.4.0/MANIFEST.in
--rw-r--r--   0 blansdel (66183) domain users (76937)     4513 2023-02-10 23:05:07.874086 ethome-ml-0.4.0/PKG-INFO
--rw-r--r--   0 blansdel (66183) domain users (76937)     3995 2023-01-13 21:39:22.000000 ethome-ml-0.4.0/README.md
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.838086 ethome-ml-0.4.0/ethome/
--rw-r--r--   0 blansdel (66183) domain users (76937)      770 2023-02-10 23:02:19.000000 ethome-ml-0.4.0/ethome/__init__.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      301 2022-09-22 06:23:05.000000 ethome-ml-0.4.0/ethome/config.py
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.838086 ethome-ml-0.4.0/ethome/data/
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.834087 ethome-ml-0.4.0/ethome/data/dlc/
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.870086 ethome-ml-0.4.0/ethome/data/dlc/openfield/
--rw-r--r--   0 blansdel (66183) domain users (76937)   525609 2022-09-22 06:23:05.000000 ethome-ml-0.4.0/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv
--rw-r--r--   0 blansdel (66183) domain users (76937) 16565151 2022-09-22 06:23:06.000000 ethome-ml-0.4.0/ethome/data/sample_dataframe.pkl
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.838086 ethome-ml-0.4.0/ethome/features/
--rw-r--r--   0 blansdel (66183) domain users (76937)      313 2023-01-13 01:35:12.000000 ethome-ml-0.4.0/ethome/features/__init__.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     8958 2022-10-16 04:21:59.000000 ethome-ml-0.4.0/ethome/features/cnn1d.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    11996 2022-10-16 04:22:06.000000 ethome-ml-0.4.0/ethome/features/dl_features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     6876 2023-01-13 16:33:40.000000 ethome-ml-0.4.0/ethome/features/features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    12688 2022-10-13 05:56:34.000000 ethome-ml-0.4.0/ethome/features/generic_features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    26081 2022-09-25 06:01:10.000000 ethome-ml-0.4.0/ethome/features/mars_features.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     2437 2022-09-22 06:23:06.000000 ethome-ml-0.4.0/ethome/interpolation.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    16621 2023-01-13 21:19:24.000000 ethome-ml-0.4.0/ethome/io.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     4110 2022-09-23 05:03:34.000000 ethome-ml-0.4.0/ethome/models.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    17145 2022-09-23 05:46:22.000000 ethome-ml-0.4.0/ethome/plot.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     9809 2022-09-22 06:23:06.000000 ethome-ml-0.4.0/ethome/unsupervised.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      574 2022-09-22 06:23:06.000000 ethome-ml-0.4.0/ethome/utils.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      106 2023-01-13 21:53:31.000000 ethome-ml-0.4.0/ethome/version.py
--rw-r--r--   0 blansdel (66183) domain users (76937)    31588 2023-01-13 16:00:56.000000 ethome-ml-0.4.0/ethome/video.py
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.874086 ethome-ml-0.4.0/ethome_ml.egg-info/
--rw-r--r--   0 blansdel (66183) domain users (76937)     4513 2023-02-10 23:05:07.000000 ethome-ml-0.4.0/ethome_ml.egg-info/PKG-INFO
--rw-r--r--   0 blansdel (66183) domain users (76937)      812 2023-02-10 23:05:07.000000 ethome-ml-0.4.0/ethome_ml.egg-info/SOURCES.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)        1 2023-02-10 23:05:07.000000 ethome-ml-0.4.0/ethome_ml.egg-info/dependency_links.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)       94 2023-02-10 23:05:07.000000 ethome-ml-0.4.0/ethome_ml.egg-info/requires.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)        7 2023-02-10 23:05:07.000000 ethome-ml-0.4.0/ethome_ml.egg-info/top_level.txt
--rw-r--r--   0 blansdel (66183) domain users (76937)      104 2022-09-22 06:23:06.000000 ethome-ml-0.4.0/pyproject.toml
--rw-r--r--   0 blansdel (66183) domain users (76937)      810 2023-02-10 23:05:07.874086 ethome-ml-0.4.0/setup.cfg
-drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-02-10 23:05:07.874086 ethome-ml-0.4.0/tests/
--rw-r--r--   0 blansdel (66183) domain users (76937)    17953 2023-01-13 15:30:56.000000 ethome-ml-0.4.0/tests/test_analysis.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     3870 2022-10-17 04:44:36.000000 ethome-ml-0.4.0/tests/test_io.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      335 2022-09-29 21:17:44.000000 ethome-ml-0.4.0/tests/test_models.py
--rw-r--r--   0 blansdel (66183) domain users (76937)     1760 2022-10-17 04:13:29.000000 ethome-ml-0.4.0/tests/test_unsupervised.py
--rw-r--r--   0 blansdel (66183) domain users (76937)      180 2022-09-22 06:23:06.000000 ethome-ml-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.862668 ethome-ml-0.5.0/
+-rw-r--r--   0 blansdel (66183) domain users (76937)     1069 2022-09-22 06:23:05.000000 ethome-ml-0.5.0/LICENSE
+-rw-r--r--   0 blansdel (66183) domain users (76937)      192 2022-09-22 06:23:05.000000 ethome-ml-0.5.0/MANIFEST.in
+-rw-r--r--   0 blansdel (66183) domain users (76937)     4520 2023-04-15 02:30:39.862668 ethome-ml-0.5.0/PKG-INFO
+-rw-r--r--   0 blansdel (66183) domain users (76937)     4002 2023-03-14 20:35:45.000000 ethome-ml-0.5.0/README.md
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.846668 ethome-ml-0.5.0/ethome/
+-rw-r--r--   0 blansdel (66183) domain users (76937)     1220 2023-04-15 02:30:31.000000 ethome-ml-0.5.0/ethome/__init__.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      301 2022-09-22 06:23:05.000000 ethome-ml-0.5.0/ethome/config.py
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.846668 ethome-ml-0.5.0/ethome/data/
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.846668 ethome-ml-0.5.0/ethome/data/dlc/
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.862668 ethome-ml-0.5.0/ethome/data/dlc/openfield/
+-rw-r--r--   0 blansdel (66183) domain users (76937)   525609 2022-09-22 06:23:05.000000 ethome-ml-0.5.0/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv
+-rw-r--r--   0 blansdel (66183) domain users (76937) 16565151 2022-09-22 06:23:06.000000 ethome-ml-0.5.0/ethome/data/sample_dataframe.pkl
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.846668 ethome-ml-0.5.0/ethome/features/
+-rw-r--r--   0 blansdel (66183) domain users (76937)      313 2023-01-13 01:35:12.000000 ethome-ml-0.5.0/ethome/features/__init__.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     8249 2023-02-17 05:56:11.000000 ethome-ml-0.5.0/ethome/features/cnn1d.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    11809 2023-02-17 05:44:55.000000 ethome-ml-0.5.0/ethome/features/dl_features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     6876 2023-01-13 16:33:40.000000 ethome-ml-0.5.0/ethome/features/features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    12688 2022-10-13 05:56:34.000000 ethome-ml-0.5.0/ethome/features/generic_features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    26081 2022-09-25 06:01:10.000000 ethome-ml-0.5.0/ethome/features/mars_features.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     2437 2022-09-22 06:23:06.000000 ethome-ml-0.5.0/ethome/interpolation.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    25297 2023-03-17 22:00:55.000000 ethome-ml-0.5.0/ethome/io.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     4110 2022-09-23 05:03:34.000000 ethome-ml-0.5.0/ethome/models.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    17215 2023-03-18 02:35:37.000000 ethome-ml-0.5.0/ethome/plot.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    10903 2023-03-18 02:38:27.000000 ethome-ml-0.5.0/ethome/unsupervised.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      713 2023-02-17 05:36:45.000000 ethome-ml-0.5.0/ethome/utils.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      106 2023-01-13 21:53:31.000000 ethome-ml-0.5.0/ethome/version.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)    33534 2023-03-18 14:42:48.000000 ethome-ml-0.5.0/ethome/video.py
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.862668 ethome-ml-0.5.0/ethome_ml.egg-info/
+-rw-r--r--   0 blansdel (66183) domain users (76937)     4520 2023-04-15 02:30:39.000000 ethome-ml-0.5.0/ethome_ml.egg-info/PKG-INFO
+-rw-r--r--   0 blansdel (66183) domain users (76937)      831 2023-04-15 02:30:39.000000 ethome-ml-0.5.0/ethome_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)        1 2023-04-15 02:30:39.000000 ethome-ml-0.5.0/ethome_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)       94 2023-04-15 02:30:39.000000 ethome-ml-0.5.0/ethome_ml.egg-info/requires.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)        7 2023-04-15 02:30:39.000000 ethome-ml-0.5.0/ethome_ml.egg-info/top_level.txt
+-rw-r--r--   0 blansdel (66183) domain users (76937)      104 2022-09-22 06:23:06.000000 ethome-ml-0.5.0/pyproject.toml
+-rw-r--r--   0 blansdel (66183) domain users (76937)      810 2023-04-15 02:30:39.862668 ethome-ml-0.5.0/setup.cfg
+drwxr-xr-x   0 blansdel (66183) domain users (76937)        0 2023-04-15 02:30:39.862668 ethome-ml-0.5.0/tests/
+-rw-r--r--   0 blansdel (66183) domain users (76937)    17953 2023-01-13 15:30:56.000000 ethome-ml-0.5.0/tests/test_analysis.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     5556 2023-04-12 05:01:57.000000 ethome-ml-0.5.0/tests/test_io.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      335 2022-09-29 21:17:44.000000 ethome-ml-0.5.0/tests/test_models.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      515 2023-03-18 02:54:17.000000 ethome-ml-0.5.0/tests/test_plot.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)     1973 2023-03-18 02:42:38.000000 ethome-ml-0.5.0/tests/test_unsupervised.py
+-rw-r--r--   0 blansdel (66183) domain users (76937)      180 2022-09-22 06:23:06.000000 ethome-ml-0.5.0/tests/test_utils.py
```

### Comparing `ethome-ml-0.4.0/LICENSE` & `ethome-ml-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/PKG-INFO` & `ethome-ml-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethome-ml
-Version: 0.4.0
+Version: 0.5.0
 Summary: Machine learning for animal behavior analysis
 Home-page: https://github.com/benlansdell/ethome
 Author: Ben Lansdell
 Author-email: ben.lansdell@gmail.com
 Project-URL: Bug Tracker, https://github.com/benlansdell/ethome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 ![build](https://github.com/benlansdell/ethome/actions/workflows/workflow.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ethome-ml.svg)](https://badge.fury.io/py/ethome-ml)
 
 # Ethome
 
 Tools for machine learning of animal behavior.
 
-This library interprets pose-tracking files (at present, from DLC or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
+This library interprets pose-tracking files (at present, from DLC, SLEAP or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
 
 ## Features
 
 * Read in animal pose data and corresponding behavior annotations to make supervised learning easy
 * Scale data to desired physical units
 * Interpolate pose data to improve low-confidence predictions 
 * Create generic features for analysis and downstream ML tasks
```

### Comparing `ethome-ml-0.4.0/README.md` & `ethome-ml-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ![build](https://github.com/benlansdell/ethome/actions/workflows/workflow.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ethome-ml.svg)](https://badge.fury.io/py/ethome-ml)
 
 # Ethome
 
 Tools for machine learning of animal behavior.
 
-This library interprets pose-tracking files (at present, from DLC or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
+This library interprets pose-tracking files (at present, from DLC, SLEAP or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
 
 ## Features
 
 * Read in animal pose data and corresponding behavior annotations to make supervised learning easy
 * Scale data to desired physical units
 * Interpolate pose data to improve low-confidence predictions 
 * Create generic features for analysis and downstream ML tasks
```

### Comparing `ethome-ml-0.4.0/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv` & `ethome-ml-0.5.0/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/ethome/data/sample_dataframe.pkl` & `ethome-ml-0.5.0/ethome/data/sample_dataframe.pkl`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/ethome/features/cnn1d.py` & `ethome-ml-0.5.0/ethome/features/cnn1d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,26 @@
-import warnings
 import numpy as np 
 import pandas as pd 
 
-try:
-    import tensorflow.keras as keras
-    from keras.models import Sequential
-    import keras.layers as layers
-    import keras
-    has_keras = True
-except ImportError:
-    warnings.warn("Keras not found. Deep learning-based features are not available", RuntimeWarning)
-    has_keras = False
-
+from ..utils import check_keras
 from .mars_features import make_features_mars, make_features_mars_distr
 
 def build_baseline_model(input_dim, layer_channels=(512, 256), dropout_rate=0., 
                         learning_rate=1e-3, conv_size=5, num_classes = 4,
                         class_weight = None):
 
-    if not has_keras:
+    if not check_keras():
         raise RuntimeError("Keras not found. Deep learning-based features are not available")
 
-    print(f"dropout_rate: {dropout_rate}, learning_rate: {learning_rate}, layer_channels: {layer_channels}, conv_size: {conv_size}")
+    import tensorflow.keras as keras
+    from keras.models import Sequential
+    import keras.layers as layers
+    #import keras
 
-    # def add_dense_bn_activate(model, out_dim, activation='relu', drop=0.):
-    #     model.add(layers.Dense(out_dim))
-    #     model.add(layers.BatchNormalization())
-    #     model.add(layers.Activation('relu'))
-    #     if drop > 0:
-    #         model.add(layers.Dropout(rate=drop))
-    #     return model
+    print(f"dropout_rate: {dropout_rate}, learning_rate: {learning_rate}, layer_channels: {layer_channels}, conv_size: {conv_size}")
 
     def add_conv_bn_activate(model, out_dim, activation='relu', conv_size=3, drop=0.):
         model.add(layers.Conv1D(out_dim, conv_size))
         model.add(layers.BatchNormalization())
         model.add(layers.Activation('relu'))
         model.add(layers.MaxPooling1D(2, 2))
         if drop > 0:
@@ -140,104 +127,105 @@
             features.append(distances)
 
     features = np.vstack(features).T
 
     return features, features.shape[1:]
     #output (4509, X) = (frame, feature) 
 
-if has_keras:
-    class MABe_Generator(keras.utils.Sequence):
-        def __init__(self, pose_dict, 
-                    batch_size, dim, 
-                    use_conv, num_classes, augment=False,
-                    class_to_number=None,
-                    past_frames=0, future_frames=0, 
-                    frame_gap=1, shuffle=False,
-                    mode='fit', featurize = features_identity):
-            self.batch_size = batch_size
-            self.featurize = featurize
-            self.video_keys = list(pose_dict.keys())
-            self.dim = dim
-            self.use_conv = use_conv
-            self.past_frames = past_frames
-            self.future_frames = future_frames
-            self.frame_gap = frame_gap
-            self.shuffle = shuffle
-            self.num_classes=num_classes
-            self.augment = augment
-            self.mode = mode
-
-            self.class_to_number = class_to_number
-
-            self.video_indexes = []
-            self.frame_indexes = []
-            self.X = {}
-            self.pad = self.past_frames * self.frame_gap
-            future_pad = self.future_frames * self.frame_gap
-            pad_width = (self.pad, future_pad), (0, 0), (0, 0), (0, 0)
-            self.seq_lengths = {}
-            for vc, key in enumerate(self.video_keys):
-                nframes = len(pose_dict[key]['keypoints'])
-                self.video_indexes.extend([vc for _ in range(nframes)])
-                self.frame_indexes.extend(range(nframes))
-                self.X[key],_ = self.featurize(np.pad(pose_dict[key]['keypoints'], pad_width))
-                self.seq_lengths[key] = nframes
-            
-            self.class_weights = np.ones(num_classes)
-            
-            self.X_dtype = self.X[key].dtype
-
-            self.indexes = list(range(len(self.frame_indexes)))
-
-            if self.mode == 'predict':
-                extra_predicts = -len(self.indexes) % self.batch_size # So that last part is not missed
-                self.indexes.extend(self.indexes[:extra_predicts])
-                self.indexes = np.array(self.indexes)
-            
-            self.on_epoch_end()
-
-        def __len__(self):
-            return len(self.indexes) // self.batch_size
-
-        def augment_fn(self, x):
-            # Rotate
-            angle = (np.random.rand()-0.5) * (np.pi * 2)
-            c, s = np.cos(angle), np.sin(angle)
-            rot = np.array([[c, -s], [s, c]])
-            x = np.dot(x, rot)
-
-            # Shift - All get shifted together
-            shift = (np.random.rand(2)-0.5) * 2 * 0.25
-            x = x + shift
-            return x
-
-        def __getitem__(self, index):
-            bs = self.batch_size
-            indexes = self.indexes[index*bs:(index+1)*bs]
-            X = np.empty((bs, *self.dim), self.X_dtype)
+class MABe_Generator:
+    def __init__(self, pose_dict, 
+                batch_size, dim, 
+                use_conv, num_classes, augment=False,
+                class_to_number=None,
+                past_frames=0, future_frames=0, 
+                frame_gap=1, shuffle=False,
+                mode='fit', featurize = features_identity):
+        self.batch_size = batch_size
+        self.featurize = featurize
+        self.video_keys = list(pose_dict.keys())
+        self.dim = dim
+        self.use_conv = use_conv
+        self.past_frames = past_frames
+        self.future_frames = future_frames
+        self.frame_gap = frame_gap
+        self.shuffle = shuffle
+        self.num_classes=num_classes
+        self.augment = augment
+        self.mode = mode
+
+        self.class_to_number = class_to_number
+
+        self.video_indexes = []
+        self.frame_indexes = []
+        self.X = {}
+        self.pad = self.past_frames * self.frame_gap
+        future_pad = self.future_frames * self.frame_gap
+        pad_width = (self.pad, future_pad), (0, 0), (0, 0), (0, 0)
+        self.seq_lengths = {}
+        for vc, key in enumerate(self.video_keys):
+            nframes = len(pose_dict[key]['keypoints'])
+            self.video_indexes.extend([vc for _ in range(nframes)])
+            self.frame_indexes.extend(range(nframes))
+            self.X[key],_ = self.featurize(np.pad(pose_dict[key]['keypoints'], pad_width))
+            self.seq_lengths[key] = nframes
+        
+        self.class_weights = np.ones(num_classes)
+        
+        self.X_dtype = self.X[key].dtype
+
+        self.indexes = list(range(len(self.frame_indexes)))
+
+        if self.mode == 'predict':
+            extra_predicts = -len(self.indexes) % self.batch_size # So that last part is not missed
+            self.indexes.extend(self.indexes[:extra_predicts])
+            self.indexes = np.array(self.indexes)
+        
+        self.on_epoch_end()
+
+    def __len__(self):
+        return len(self.indexes) // self.batch_size
+
+    def augment_fn(self, x):
+        # Rotate
+        angle = (np.random.rand()-0.5) * (np.pi * 2)
+        c, s = np.cos(angle), np.sin(angle)
+        rot = np.array([[c, -s], [s, c]])
+        x = np.dot(x, rot)
+
+        # Shift - All get shifted together
+        shift = (np.random.rand(2)-0.5) * 2 * 0.25
+        x = x + shift
+        return x
+
+    def __getitem__(self, index):
+        bs = self.batch_size
+        indexes = self.indexes[index*bs:(index+1)*bs]
+        X = np.empty((bs, *self.dim), self.X_dtype)
+        if self.mode == 'predict':
+            vkey_fi_list = []
+        for bi, idx in enumerate(indexes):
+            vkey = self.video_keys[self.video_indexes[idx]]
+            fi = self.frame_indexes[idx]
             if self.mode == 'predict':
-                vkey_fi_list = []
-            for bi, idx in enumerate(indexes):
-                vkey = self.video_keys[self.video_indexes[idx]]
-                fi = self.frame_indexes[idx]
-                if self.mode == 'predict':
-                    vkey_fi_list.append((vkey, fi))
-                fi = fi + self.pad
-                start = fi - self.past_frames*self.frame_gap
-                stop = fi + (self.future_frames + 1)*self.frame_gap
-                assert start >= 0
-
-                Xi = self.X[vkey][start:stop:self.frame_gap].copy()
-            
-                if self.augment:
-                    Xi = self.augment_fn(Xi)
-                X[bi] = np.reshape(Xi, self.dim)
-
-            if self.mode == 'predict':
-                return X, vkey_fi_list
-
-        def on_epoch_end(self):
-            if self.shuffle == True:
-                np.random.shuffle(self.indexes)
-else:
-    class MABe_Generator(object):
-        pass
+                vkey_fi_list.append((vkey, fi))
+            fi = fi + self.pad
+            start = fi - self.past_frames*self.frame_gap
+            stop = fi + (self.future_frames + 1)*self.frame_gap
+            assert start >= 0
+
+            Xi = self.X[vkey][start:stop:self.frame_gap].copy()
+        
+            if self.augment:
+                Xi = self.augment_fn(Xi)
+            X[bi] = np.reshape(Xi, self.dim)
+
+        if self.mode == 'predict':
+            return X, vkey_fi_list
+
+    def on_epoch_end(self):
+        if self.shuffle == True:
+            np.random.shuffle(self.indexes)
+
+    def __iter__(self):
+        """Create a generator that iterate over the Sequence."""
+        for item in (self[i] for i in range(len(self))):
+            yield item
```

### Comparing `ethome-ml-0.4.0/ethome/features/dl_features.py` & `ethome-ml-0.5.0/ethome/features/dl_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 import numpy as np
 import json 
 import pandas as pd
 import tqdm
 import os
 from copy import deepcopy
-import warnings
 
 from ethome.features.cnn1d import build_baseline_model
 from ethome.features.cnn1d import MABe_Generator, features_identity
 from .cnn1d import *
-
-try:
-    import tensorflow.keras as keras
-    has_keras = True
-except ImportError:
-    warnings.warn("Keras not found. Deep learning-based features are not available", RuntimeWarning)
-    has_keras = False
+from ..utils import check_keras
 
 THIS_FILE_DIR = os.path.dirname(os.path.realpath(__file__))
 
 default_config = {"val_size": 0.2,
                     "normalize": True,
                     "split_videos": False,
                     "future_frames": 50,
@@ -282,15 +275,15 @@
     final_df = pd.concat(dfs, axis = 0)
     return final_df
 
 def compute_dl_probability_features(df : pd.DataFrame, raw_col_names : list, **kwargs):
 
     animal_setup = df.pose.animal_setup
 
-    if not has_keras:
+    if not check_keras():
         raise RuntimeError("Keras not found. Deep learning-based features are not available")
 
     test_data = convert_to_mars_format(df, raw_col_names, animal_setup)
     parametersweep = 'test_run_distances'
     build_model = build_baseline_model
     Generator = MABe_Generator
     use_callbacks = False
```

### Comparing `ethome-ml-0.4.0/ethome/features/features.py` & `ethome-ml-0.5.0/ethome/features/features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/ethome/features/generic_features.py` & `ethome-ml-0.5.0/ethome/features/generic_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/ethome/features/mars_features.py` & `ethome-ml-0.5.0/ethome/features/mars_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/ethome/interpolation.py` & `ethome-ml-0.5.0/ethome/interpolation.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/ethome/io.py` & `ethome-ml-0.5.0/ethome/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """ Loading and saving tracking and behavior annotation files """
 import pandas as pd
 import pickle
 import numpy as np
 from itertools import product
 from joblib import dump, load
 import os
+import h5py
 from glob import glob
 import warnings
 from pynwb import NWBHDF5IO
+from collections import defaultdict
 
 XY_IDS = ['x', 'y']
 XYLIKELIHOOD_IDS = ['x', 'y', 'likelihood']
 
 def uniquifier(seq):
     """Return a sequence (e.g. list) with unique elements only, but maintaining original list order"""
     seen = set()
@@ -50,42 +52,236 @@
                     part_renamer : dict = None, 
                     animal_renamer : dict = None,
                     read_likelihoods : bool = True,
                     labels : pd.DataFrame = None) -> tuple:
     """Read in tracks from DLC.
 
     Args:
-        fn_in: csv file that has DLC tracks
+        fn_in: csv or h5 file that has DLC tracks
         part_renamer: dictionary to rename body parts, if needed 
         animal_renamer: dictionary to rename animals, if needed
         read_likelihoods: default True. Whether to attach DLC likelihoods to table
 
     Returns:
         Pandas DataFrame with (n_animals*2*n_body_parts) columns plus with filename and frame, 
             List of body parts,
             List of animals,
             Columns names for DLC tracks (excluding likelihoods, if read in),
             Scorer
     """
 
-    df = pd.read_csv(fn_in, header = [0,1,2,3], index_col = 0)
-    return _read_DLC_tracks(df, fn_in, part_renamer, animal_renamer, read_likelihoods, labels)
+    ext = os.path.splitext(fn_in)[1]
+    if ext == 'h5' or ext == 'hdf5' or ext == 'hdf':
+        df = pd.read_hdf(fn_in)
+        ext = 'h5'
+    else:
+        df = pd.read_csv(fn_in, header = [0,1,2,3], index_col = 0)
+        ext = 'csv'
+    return _read_DLC_tracks(df, fn_in, part_renamer, animal_renamer, read_likelihoods, labels, ext)
+
+def read_sleap_tracks(fn_in : str, 
+                    part_renamer : dict = None, 
+                    animal_renamer : dict = None,
+                    read_likelihoods : bool = True,
+                    labels : pd.DataFrame = None) -> tuple:
+    """Read in tracks from SLEAP.
+
+    Args:
+        fn_in: csv or h5 file that has sleap tracks
+        part_renamer: dictionary to rename body parts, if needed 
+        animal_renamer: dictionary to rename animals, if needed
+        read_likelihoods: default True. Whether to attach DLC likelihoods to table
+
+    Returns:
+        Pandas DataFrame with (n_animals*2*n_body_parts) columns plus with filename and frame, 
+            List of body parts,
+            List of animals,
+            Columns names for DLC tracks (excluding likelihoods, if read in),
+            Scorer
+    """
+
+    df = _load_sleap_data(fn_in, multi_animal=False)
+    return _read_sleap_tracks(df, fn_in, part_renamer, animal_renamer, read_likelihoods, labels)
+
+## This is from here
+## https://github.com/YttriLab/A-SOID/blob/d03302b3d35e22b0348b9f199998f293d8d741cd/asoid/utils/import_data.py
+## Under the following license:
+# The Clear BSD License
+# Copyright (c) 2022, YttriLab, SchwarzLab
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted for academic and research use only (subject to the limitations in the disclaimer below) provided that the following conditions are met:
+
+#      * Redistributions of source code must retain the above copyright notice,
+#      this list of conditions and the following disclaimer.
+
+#      * Redistributions in binary form must reproduce the above copyright
+#      notice, this list of conditions and the following disclaimer in the
+#      documentation and/or other materials provided with the distribution.
+
+#      * Neither the name of the copyright holder nor the names of its
+#      contributors may be used to endorse or promote products derived from this
+#      software without specific prior written permission.
+
+# NO EXPRESS OR IMPLIED LICENSES TO ANY PARTY'S PATENT RIGHTS ARE GRANTED BY
+# THIS LICENSE. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND
+# CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+# PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
+# BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
+# IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+def _load_sleap_data(path, multi_animal=False):
+    """loads sleap data h5 format from file path and returns it as pd.DataFrame
+    As sleap body parts (nodes) are not ordered in a particular way, we sort them alphabetically.
+    As sleap tracks do not export a score/likelihood but cut off automatically (nan), we are simulating a likelihood
+     value for compatability with feature extraction functions"""
+    # TODO: discriminate with multiple animal from single instance model output
+    with h5py.File(path, "r") as f:
+        # occupancy_matrix = f['track_occupancy'][:]
+        # track_names = f['track_names'][:]
+        tracks_matrix = f["tracks"][:].T
+        animals = []
+        temp_tracks = None
+        for an in np.arange(tracks_matrix.shape[3]):
+            animals.append('Animal{}'.format(an))
+            if temp_tracks is None:
+                temp_tracks = tracks_matrix[:, :, :, an]
+            else:
+                temp_tracks = np.concatenate([temp_tracks, tracks_matrix[:, :, :, an]], axis=1)
+
+        bodyparts = f["node_names"][:].astype("U13")
+    # preallocate array including dummy likelihood for similarity between dlc and sleap import
+    # can be changed later if sleap files incorporate scores at any time in the future
+    likelihood_matrix = np.ones((temp_tracks.shape[0], temp_tracks.shape[1], 1))
+    sleap_matrix = np.concatenate((temp_tracks, likelihood_matrix), axis=2)
+    # # reshape tracks into 2d format (x,y, likelihood)*len(bps)
+    sleap_array = np.reshape(sleap_matrix, (sleap_matrix.shape[0], sleap_matrix.shape[1] * sleap_matrix.shape[2]))
+    # create beautiful multiindex columns to easily sort by bodypart
+
+    column_names = pd.MultiIndex.from_product([animals, bodyparts, ('x', 'y', 'likelihood')],
+                                              names=['individuals', 'bodypart', 'coords'])
+
+    # create dataframe from both
+    df = pd.DataFrame(sleap_array, columns=column_names)
+    # #change any nan values (lost tracking) to 0
+    # TODO: confirm that this is the way to go
+    for i, ani in enumerate(animals):
+        for bp in bodyparts:
+            # find any nan either in x or y coordinates. Usually they are paired, but you never know!
+            any_nan = np.any(pd.isna(df[[(ani, bp, 'x'), (ani, bp, 'x')]]).values, axis=1)
+            # get the indexes of the boolean mask
+            nan_indexes = np.argwhere(any_nan).flatten()
+            # set all nan index to 0
+            df[(ani, bp, 'likelihood')][nan_indexes] = 0
+
+    # SLEAP comes with NaN values, so we need to get rid of them!
+    # first linear interpolation
+    clean_df = df.interpolate(method="linear", limit_direction='forward')
+    # backward fill with first valid entry to take care of NaNs in the beginning
+    clean_df.fillna(method="bfill", inplace=True)
+    # sort bodyparts by alphabet
+    clean_df = clean_df.reindex(columns=sorted(bodyparts), level=1)
+    return clean_df
+
+def _read_sleap_tracks(df : pd.DataFrame, 
+                       fn_in : str, 
+                       part_renamer : dict = None, 
+                       animal_renamer : dict = None,
+                       read_likelihoods : bool = True,
+                       labels : pd.DataFrame = None) -> tuple:
+
+    if 'time' in df.columns:
+        times = df['time'].reset_index(drop = True)
+        df.drop(columns = 'time', inplace = True)
+    else:
+        times = None
+
+    scorer = 'sleap'
+
+    cols = list(df.columns)
+
+    animals = uniquifier([i[0] for i in cols])
+    body_parts = uniquifier([i[1] for i in cols])
+
+    n_body_parts = len(body_parts)
+    n_animals = len(animals)
+
+    dlc_tracks = np.array(df)
+    n_rows = dlc_tracks.shape[0]
+    selected_cols = [[3*i, 3*i+1] for i in range(n_body_parts*n_animals)]
+    #This line flattens the array here... may be clearer using numpy reshape?
+    selected_cols = [j for i in selected_cols for j in i]
+
+    prob_cols = [3*i+2 for i in range(n_body_parts*n_animals)]
+    dlc_probs = dlc_tracks[:,prob_cols]
+    dlc_tracks = dlc_tracks[:,selected_cols]
+
+    #Put in shape:
+    # (frame, animal, x/y coord, body part)
+    dlc_tracks = dlc_tracks.reshape((n_rows, n_animals, n_body_parts, 2))
+    dlc_tracks = dlc_tracks.transpose([0, 1, 3, 2])
+
+    dlc_probs = dlc_probs.reshape((n_rows, n_animals, n_body_parts, 1))
+    dlc_probs = dlc_probs.transpose([0, 3, 1, 2])
+
+    #If we're going to rename items in the list, do it here
+    if part_renamer:
+        body_parts = _list_replace(body_parts, part_renamer)
+
+    if animal_renamer:
+        animals = _list_replace(animals, animal_renamer)
+
+    colnames = ['_'.join(a) for a in product(animals, XY_IDS, body_parts)]
+    prob_colnames = ['_'.join(a) for a in product(['likelihood'], animals, body_parts)]
+
+    dlc_probs = dlc_probs.reshape((n_rows, -1))
+    final_probs = pd.DataFrame(dlc_probs, columns = prob_colnames)
+
+    dlc_tracks = dlc_tracks.reshape((n_rows, -1))
+    final_df = pd.DataFrame(dlc_tracks, columns = colnames)
+
+    if read_likelihoods:
+        final_df = pd.concat([final_df, final_probs], axis = 1)
+
+    final_df['filename'] = fn_in
+    final_df['frame'] = final_df.index.copy()
+    if times is not None:
+        final_df['time'] = times
+
+    if labels is not None:
+        labels.index = final_df.index
+        final_df = pd.concat((final_df, labels), axis = 1)
+        final_df = final_df.rename(columns = {k:k[0] for k in labels.columns})
+        final_df.ml.label_cols = [p[0] for p in labels.columns]
+
+    return final_df, body_parts, animals, colnames, scorer
 
 def _read_DLC_tracks(df : pd.DataFrame, 
                      fn_in : str,
                      part_renamer : dict = None, 
                      animal_renamer : dict = None,
                      read_likelihoods : bool = True,
-                     labels : pd.DataFrame = None) -> tuple:
+                     labels : pd.DataFrame = None, 
+                     ext : str = 'csv') -> tuple:
 
     if 'individuals' in df.columns.names:
         df.columns = df.columns.set_names(['scorer', 'individuals', 'bodyparts', 'coords'])
         multi_animal = True
     else:
-        df = pd.read_csv(fn_in, header = [0,1,2], index_col = 0)
+        if ext == 'csv':
+            df = pd.read_csv(fn_in, header = [0,1,2], index_col = 0)
+        else:
+            df = pd.read_hdf(fn_in)
         df.columns = df.columns.set_names(['scorer', 'bodyparts', 'coords'])
         multi_animal = False
 
     if 'time' in df.columns:
         times = df['time'].reset_index(drop = True)
         df.drop(columns = 'time', inplace = True)
     else:
@@ -147,14 +343,15 @@
     if times is not None:
         final_df['time'] = times
 
     if labels is not None:
         labels.index = final_df.index
         final_df = pd.concat((final_df, labels), axis = 1)
         final_df = final_df.rename(columns = {k:k[0] for k in labels.columns})
+        final_df.ml.label_cols = [p[0] for p in labels.columns]
 
     return final_df, body_parts, animals, colnames, scorer
 
 ## This function is from DLC2NWB package: https://github.com/DeepLabCut/DLC2NWB/blob/10331daa1bfadb9c19d2e4957aa8752d74d5759b/dlc2nwb/utils.py#L307 
 #It's available under the following license:
 # MIT License
 
@@ -231,15 +428,15 @@
         objects = [read_nwbfile.processing["behavior"].data_interfaces[k] for \
                     k in object_keys if 'epoch.TimeIntervals' in str(type(read_nwbfile.processing["behavior"].data_interfaces[k]))]
         new_df = df.copy()
 
         cols = []
         for read_pe in objects:
             name = read_pe.name
-            col = 'annotation_' + name
+            col = 'label_' + name
             cols.append(col)
             new_df[col] = 0
             start_times = read_pe.start_time[:]
             stop_times = read_pe.stop_time[:]
             pairs = sorted(zip(start_times, stop_times))
             for idx, time in enumerate(new_df.index):
                 if len(pairs) == 0: break 
@@ -350,60 +547,58 @@
     cur_dir = os.path.dirname(os.path.abspath(__file__))
     path_in = os.path.join(cur_dir, 'data', 'sample_data.pkl')
     with open(path_in, 'rb') as handle:
         b = pickle.load(handle)
         #b = pd.read_pickle(handle)
     return b
 
-def read_boris_annotation(fn_in : str, fps : int, duration : float, behav_labels : dict = None) -> tuple:
+def read_boris_annotation(fn_in : str, fps : int, duration : float, behav_labels : list = None) -> tuple:
     """Read behavior annotation from BORIS exported csv file. 
 
     This will import behavior types specified (or all types, if behavior_list is None) and assign a numerical label to each. Overlapping annotations (those occurring simulataneously) are not supported. Any time the video is annotated as being in multiple states, the last state will be the one labeled.
     
     Args:
         fn_in: The filename with BORIS behavior annotations to load
         fps: The frames per second of the video
         duration: The duration of the video in seconds
         behav_labels: If provided, only import behaviors with these names. Default = None = import everything. 
     
     Returns:
-        A numpy array which indicates, for all frames, which behavior is occuring. 0 = no behavior, 1 and above are the labels of the behaviors.
-        A dictionary with keys the numerical labels and values the names of the behaviors. 
+        A dictionary of numpy arrays which gives, for all frames, which behavior is occuring. 0 = no behavior, 1 = behavior.
     """
 
     boris_labels = pd.read_csv(fn_in, skiprows = 15)
     if len(boris_labels) == 0:
         print("No data found in BORIS file,", fn_in)
         return np.array([]), {}
     fps_boris = int(boris_labels['FPS'][0])
     duration_boris = boris_labels['Total length'][0]
     if fps_boris != fps:
         warnings.warn(f"Warning: BORIS FPS is {fps_boris} but video is {fps} frames per second. Are the DLC and BORIS files from the same video?")
     if not np.isclose(duration_boris, duration, rtol = 0.01, atol = 0.01):
         warnings.warn(f"Warning: BORIS duration is {duration_boris} but video is {duration} seconds. Are the DLC and BORIS files from the same video?")
 
     n_bins = int(duration*fps)
-    ground_truth = np.zeros(n_bins)
+    ground_truth = defaultdict(lambda: np.zeros(n_bins))
 
     if behav_labels is None:
-        behaviors = boris_labels['Behavior'].unique()
-        behav_labels = {i+1:k for i,k in enumerate(behaviors)}
-
-    for behav_idx, behavior in behav_labels.items():
+        behav_labels = boris_labels['Behavior'].unique()
+    
+    for behavior in behav_labels:
         labels = boris_labels[boris_labels['Behavior'] == behavior]
         starts = labels.loc[labels['Status'] == 'START', 'Time']
         ends = labels.loc[labels['Status'] == 'STOP', 'Time']
         if len(ends) > len(starts)+1:
             raise ValueError(f"Too many {behavior} behaviors started and not stopped.")
         elif len(ends) == len(starts) + 1:
             ends.append(duration)
         for start, end in zip(starts, ends):
-            ground_truth[int(start*fps):int(end*fps)] = behav_idx
+            ground_truth[behavior][int(start*fps):int(end*fps)] = 1
 
-    return ground_truth, behav_labels
+    return ground_truth
 
 def create_behavior_labels(boris_files):
     """Create behavior labels from BORIS exported csv files.
     
     Args:
         boris_files: List of BORIS exported csv files
```

### Comparing `ethome-ml-0.4.0/ethome/models.py` & `ethome-ml-0.5.0/ethome/models.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/ethome/plot.py` & `ethome-ml-0.5.0/ethome/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,40 +7,42 @@
 from glob import glob
 import pandas as pd
 
 from ethome.config import global_config
 
 def plot_embedding(dataset : pd.DataFrame, 
                    col_names : list  = ['embedding_0', 'embedding_1'],
+                   col_labels : list = None,
                    color_col : str = None, 
                    figsize : tuple = (10,10),
-                   **kwargs) -> tuple:  # pragma: no cover
+                   **kwargs) -> tuple:
     """Scatterplot of a 2D TSNE or UMAP embedding from the dataset.
     
     Args:
         dataset: data
         col_names: list of column names to use for the x and y axes
         color_col: if provided, a column that will be used to color the points in the scatter plot
         figsize: tuple with the dimensions of the plot (in inches)
-        kwargs: All other keyword pairs are sent to Matplotlib's scatter function
+        **kwargs: All other keyword pairs are sent to Matplotlib's scatter function
 
     Returns:
         tuple (fig, axes). The Figure and Axes objects. 
     """
 
     if color_col is not None:
         c = dataset[color_col]
     else:
         c = None
 
     col1, col2 = col_names
-    fig, axes = plt.subplots(1,1, figsize = figsize)
+    fig, axes = plt.subplots(1, 1, figsize = figsize)
     axes.scatter(x = dataset[col1], y = dataset[col2], s = 1, c = c, **kwargs)
-    axes.set_xlabel('Embedding dim 1')
-    axes.set_ylabel('Embedding dim 2')
+    if col_labels is None: col_labels = col_names
+    axes.set_xlabel(col_labels[0])
+    axes.set_ylabel(col_labels[1])
     return fig, axes
 
 class MplColorHelper:  # pragma: no cover
 
     def __init__(self, cmap_name, start_val, stop_val):
         self.cmap_name = cmap_name
         self.cmap = plt.get_cmap(cmap_name)
```

### Comparing `ethome-ml-0.4.0/ethome/unsupervised.py` & `ethome-ml-0.5.0/ethome/unsupervised.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,39 @@
     
     tsne_data = StandardScaler().fit_transform(dataset[cols])
     random_indices = np.random.choice(tsne_data.shape[0], min(N_rows, tsne_data.shape[0]), replace = False)
     tsne_data = tsne_data[random_indices, :]
     tsne_embedding = TSNE(n_components=n_components, init = 'pca', perplexity = perplexity).fit_transform(tsne_data)
     return tsne_embedding, random_indices
 
+def compute_umap_embedding(dataset : pd.DataFrame, 
+                           cols : list, 
+                           N_rows : int = 20000, 
+                           n_components = 2, 
+                           **kwargs) -> np.ndarray:
+    """Compute UMAP embedding. Compute based on a random subset of rows, then apply to all rows
+    
+    Args:
+        dataset: Input data
+        cols: A list of column names to produce the embedding for
+        N_rows: A number of rows to randomly sample for the embedding. Only these rows are embedded.
+        n_components: The number of dimensions to embed the data into.
+        **kwargs: Passed to UMAP constructor
+        
+    Returns:
+        - A numpy array with the embedding data
+    """
+    
+    umap_data = StandardScaler().fit_transform(dataset[cols])
+    random_indices = np.random.choice(umap_data.shape[0], min(N_rows, umap_data.shape[0]), replace = False)
+    umap_data_rand = umap_data[random_indices, :]
+    model = umap.UMAP(n_components=n_components, **kwargs)
+    model.fit(umap_data_rand)
+    return model.transform(umap_data)
+
 def compute_morlet(data : np.ndarray, 
                    dt : float = 1/30, 
                    n_freq : int = 5, 
                    w : float = 3) -> np.ndarray:
     """ Compute morlet wavelet transform of a time series.
     
     Args:
```

### Comparing `ethome-ml-0.4.0/ethome/video.py` & `ethome-ml-0.5.0/ethome/video.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import warnings
 import types 
 
 from glob import glob
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import cross_val_predict, LeaveOneGroupOut, PredefinedSplit
 
-from ethome.io import read_DLC_tracks, read_boris_annotation, uniquifier, create_behavior_labels, read_NWB_tracks
+from ethome.io import read_DLC_tracks, read_boris_annotation, uniquifier, create_behavior_labels, read_NWB_tracks, read_sleap_tracks
 from ethome.utils import checkFFMPEG
 from ethome.config import global_config
 from ethome.features import feature_class_maker, FEATURE_MAKERS
 
 #This converts everything to mm, or leaves them as pixels
 UNIT_DICT = {'mm':1, 'cm':10, 'm':1000, 'in':25.4, 'ft':304.8,
              'millimeters':1, 'centimeters':10, 'meters':1000, 'inches':25.4, 'feet':304.8,
@@ -32,27 +32,27 @@
     for fn, item in zip(tracking_files, items):
         metadata[fn][k] = item
 
 def create_metadata(tracking_files : list, **kwargs) -> dict:
     """
     Prepare a metadata dictionary for defining a ExperimentDataFrame. 
 
-    Only required argument is list of DLC tracking file names. 
+    Only required argument is list of pose tracking file names. 
 
     Any other keyword argument must be either a non-iterable object (e.g. a scalar parameter, like FPS)
-    that will be copied and tagged to each of the DLC tracking files, or an iterable object of the same
-    length of the list of DLC tracking files. Each element in the iterable will be tagged with the corresponding
-    DLC file.
+    that will be copied and tagged to each of the pose tracking files, or an iterable object of the same
+    length of the list of pose tracking files. Each element in the iterable will be tagged with the corresponding
+    pose-tracking file.
 
     Args:
-        tracking_files: List of DLC tracking .csvs
+        tracking_files: List of pose tracking files
         **kwargs: described as above
 
     Returns:
-        Dictionary whose keys are DLC tracking file names, and contains a dictionary with key,values containing the metadata provided
+        Dictionary whose keys are pose-tracking file names, and contains a dictionary with key,values containing the metadata provided
     """
 
     metadata = {}
     for fn in tracking_files:
         metadata[fn] = {}
     n_files = len(tracking_files)
 
@@ -64,15 +64,15 @@
                 _add_items_to_dict(tracking_files, metadata, k, v)
         else:
             _add_item_to_dict(tracking_files, metadata, k, v)
 
     return metadata
 
 def _convert_units(df):
-    # if 'frame_width', 'resolution' and 'frame_width_units' are provided, then we convert DLC tracks to these units.
+    # if 'frame_width', 'resolution' and 'frame_width_units' are provided, then we convert tracks to these units.
     if len(df.metadata.details) == 0:
         return 
     for col in df.columns:
         is_dlc_feature = False
         for ani in df.pose.animals:
             if col.startswith(ani):
                 is_dlc_feature = True
@@ -304,15 +304,18 @@
         new_features.columns = new_feat_cols
 
         #Don't add duplicated columns:
         notdupcols = [col for col in new_feat_cols if col not in df.columns]
         new_features = new_features[notdupcols]
 
         df.reset_index(drop = True, inplace = True)
-        df[notdupcols] = new_features.reset_index(drop = True)
+        #Suppress warnings here:
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            df[notdupcols] = new_features.reset_index(drop = True)
 
         if add_to_features:
             if self.active is not None:
                 self.active = list(self.active) + list(new_features.columns)
             else:
                 self.active = new_features.columns
         return list(new_features.columns)
@@ -511,15 +514,15 @@
             None. Data in this object is populated with contents of file."""
         return load_experiment(fn_in)
 
     def save_movie(self, label_columns, path_out : str, video_filenames = None) -> None: # pragma: no cover
         """Given columns indicating behavior predictions or whatever else, make a video
         with these predictions overlaid. 
 
-        ExperimentDataFrame metadata must have the keys 'video_file', so that the video associated with each set of DLC tracks is known.
+        ExperimentDataFrame metadata must have the keys 'video_file', so that the video associated with each set of pose tracks is known.
 
         Args:
             label_columns: list or dict of columns whose values to overlay on top of video. If dict, keys are the columns and values are the print-friendly version.
             path_out: the directory to output the videos too
             video_filenames: list or string. The set of videos to use. If not provided, then use all videos as given in the metadata.
 
         Returns:
@@ -540,14 +543,16 @@
             video_filenames = [video_filenames]
         if not video_filenames:
             video_filenames = self._obj.metadata.videos
         if type(label_columns) is list:
             label_columns = {k:k for k in label_columns}
 
         for video in video_filenames:
+            if 'fps' not in self._obj.metadata.details[video]:
+                raise ValueError(f"FPS not in metadata for video {video}, skipping. Provide FPS in dataset creation.")
             rate = 1/self._obj.metadata.details[video]['fps']
             vid_in = self._obj.metadata.details[video]['video_files']
             file_out = os.path.splitext(os.path.basename(vid_in))[0] + '_'.join(label_columns.keys()) + '.mp4'
             vid_out = os.path.join(path_out, file_out)
             label_strings = []
             for idx, (col,print_label) in enumerate(label_columns.items()):
                 this_y_offset = y_offset + y_inc*idx
@@ -557,63 +562,78 @@
             label_string = ','.join(label_strings)
 
             #ffmpeg is the fastest way to add this information to a video
             #Prepare the ffmpeg command
             cmd = f'ffmpeg -y -i {vid_in} -vf "{label_string}" {vid_out}'
             os.system(cmd)            
 
-    #I think... this is obsolete, and the other save is the right one
-    #def save(self, fn):
-    #    with open(fn, 'wb') as handle:
-    #        pickle.dump(self, handle, protocol=pickle.HIGHEST_PROTOCOL)
+def _create_from_dict(metadata, label_key, part_renamer, animal_renamer):
+    df = pd.DataFrame()
+    #req_cols = ['fps']
+    #Drop requirement this is provided. Just omit addition of time column, if fps omitted
+    req_cols = []
+    is_valid, should_rescale = _validate_metadata(metadata, req_cols)
+    if is_valid:   
+        df.metadata.details = metadata
+    else:
+        raise ValueError("Metadata not properly formatted. See docstring.")
+
+    if len(metadata) > 0:
+        _load_tracks(df, part_renamer, animal_renamer, rescale = should_rescale) 
+        _load_labels(df, set_as_label = True)
+
+    if should_rescale:
+        _convert_units(df)
+    elif 'scale_factor' in df.columns: 
+        df.drop(columns = 'scale_factor', inplace = True)
+
+    return df    
+
+def _create_from_list(metadata, label_key, part_renamer, animal_renamer):
+    if len(metadata) == 0:
+        return pd.DataFrame()
+    supported_exts = ['.csv', '.h5', '.nwb', '.hdf5']
+    exts = [os.path.splitext(m)[1] for m in metadata]
+    print(exts)
+    supported = [e in supported_exts for e in exts]
+    is_nwb = [e == 'nwb' for e in exts]
+    if not all(supported):
+        ValueError("Only NWB, dlc (csv) or SLEAP (h5, hdf5) formats are supported.")
+
+    if all(is_nwb):
+        df = _load_nwb(metadata, part_renamer, animal_renamer)
+    else:
+        metadata = {k:{} for k in metadata}
+        df = _create_from_dict(metadata, label_key, part_renamer, animal_renamer)
 
+    return df
 
 def create_dataset(metadata : dict = None, 
                      label_key : dict = None, 
                      part_renamer : dict = None,
                      animal_renamer : dict = None) -> pd.DataFrame:
-    """Houses DLC tracking data and behavior annotations in pandas DataFrame for ML, along with relevant metadata, features and behavior annotation labels.
+    """Houses pose-tracking data and behavior annotations in pandas DataFrame for ML, along with relevant metadata, features and behavior annotation labels.
 
     Args:
-        metadata: Dictionary whose keys are DLC tracking csvs, and value is a dictionary of associated metadata
+        metadata: Dictionary whose keys are pose tracking files, and value is a dictionary of associated metadata
             for that video. Most easiest to create with 'create_metadata'. 
-            Required keys are: ['fps']
         label_key: Default None. Dictionary whose keys are positive integers and values are behavior labels. If none, then this is inferred from the behavior annotation files provided.  
         part_renamer: Default None. Dictionary that can rename body parts from tracking files if needed (for feature creation, e.g.)
         animal_renamer: Default None. Dictionary that can rename animals from tracking files if needed
 
     Returns:
         DataFrame object. This is a pandas DataFrame with additional metadata and methods.
     """
 
     if type(metadata) is dict:
-
-        df = pd.DataFrame()
-        req_cols = ['fps']
-        is_valid, should_rescale = _validate_metadata(metadata, req_cols)
-        if is_valid:   
-            df.metadata.details = metadata
-        else:
-            raise ValueError("Metadata not properly formatted. See docstring.")
-
-        if len(metadata) > 0:
-            _load_tracks(df, part_renamer, animal_renamer, rescale = should_rescale) 
-            _load_labels(df, set_as_label = True)
-
-        if should_rescale:
-            _convert_units(df)
-        elif 'scale_factor' in df.columns: 
-            df.drop(columns = 'scale_factor', inplace = True)
-
+        df = _create_from_dict(metadata, label_key, part_renamer, animal_renamer)
     elif type(metadata) is str:
-        df = _load_nwb([metadata], part_renamer, animal_renamer)
-
+        df = _create_from_list([metadata], label_key, part_renamer, animal_renamer)
     elif type(metadata) is list:
-        df = _load_nwb(metadata, part_renamer, animal_renamer)
-
+        df = _create_from_list(metadata, label_key, part_renamer, animal_renamer)
     else:
         raise ValueError("Metadata not properly formatted. See docstring.")
 
     if label_key:
         df.metadata.label_key = label_key
 
     return df
@@ -648,34 +668,41 @@
     df.pose.body_parts = body_parts
     df.pose.animals = animals
     df.pose.animal_setup = {'mouse_ids': animals, 'bodypart_ids': body_parts, 'colnames': col_names}
     df.pose.raw_track_columns = col_names
     return df
 
 def _load_tracks(df, part_renamer, animal_renamer, rescale = False):
-    #For the moment only supports DLC
-    return _load_dlc_tracks(df, part_renamer, animal_renamer, rescale = rescale)
-
-def _load_dlc_tracks(df, part_renamer, animal_renamer, rescale = False):
-    """Add DLC tracks to DataFrame"""
-
+    """Add tracks to DataFrame"""
     dfs = []
     col_names_old = None
-    #Go through each video file and load DLC tracks
+    #Go through each video file and load tracks
     for fn in df.metadata.details.keys():
-        if fn.split('.')[-1] == 'nwb':
+        _, ext = os.path.splitext(fn)
+        if ext == '.nwb':
             df_fn, body_parts, animals, col_names, scorer, _ = read_NWB_tracks(fn, 
                                                                             part_renamer, 
                                                                             animal_renamer)
-        else:
+        elif ext == '.csv':
             df_fn, body_parts, animals, col_names, scorer = read_DLC_tracks(fn, 
                                                                             part_renamer, 
                                                                             animal_renamer)
+        else:
+            #Try DLC first, if this fails, read as SLEAP
+            try:
+                df_fn, body_parts, animals, col_names, scorer = read_DLC_tracks(fn, 
+                                                                                part_renamer, 
+                                                                                animal_renamer)
+            except:
+                df_fn, body_parts, animals, col_names, scorer = read_sleap_tracks(fn, 
+                                                                                part_renamer, 
+                                                                                animal_renamer)
+
         n_rows = len(df_fn)
-        if 'time' not in df_fn.columns:
+        if 'time' not in df_fn.columns and 'fps' in df.metadata.details[fn]:
             df_fn['time'] = df_fn['frame']/df.metadata.details[fn]['fps']
 
         if rescale and ('frame_width_units' in df.metadata.details[fn]) and \
                 ('frame_width' in df.metadata.details[fn]) and \
                 ('resolution' in df.metadata.details[fn]) and \
                 df.metadata.details[fn]['frame_width_units'].lower() in UNIT_DICT:
             unit_scale_factor = UNIT_DICT[df.metadata.details[fn]['frame_width_units'].lower()]
@@ -686,19 +713,20 @@
                 df.metadata.details[fn]['units'] = 'mm'
 
             df_fn['scale_factor'] = df.metadata.details[fn]['frame_width']/df.metadata.details[fn]['resolution'][1]*unit_scale_factor
         else:
             df_fn['scale_factor'] = 1
 
         dfs.append(df_fn)
-        df.metadata.details[fn]['duration'] = (n_rows)/df.metadata.details[fn]['fps']
+        if 'fps' in df.metadata.details[fn]:
+            df.metadata.details[fn]['duration'] = (n_rows)/df.metadata.details[fn]['fps']
         df.metadata.details[fn]['scorer'] = scorer
         if col_names_old is not None:
             if col_names != col_names_old:
-                raise RuntimeError("DLC files have different columns. Must all be from same project")
+                raise RuntimeError("Tracking files have different columns. Must all be from same project")
         col_names_old = col_names
 
     dfs = pd.concat(dfs, axis = 0)
     df[dfs.columns] = dfs
     df.reset_index(drop = True, inplace = True)
     df.pose.body_parts = body_parts
     df.pose.animals = animals
@@ -719,27 +747,32 @@
     if not df.metadata.label_key:
         label_files = []
         for fn in df.metadata.details.keys():
             if 'labels' in df.metadata.details[fn]:
                 label_files.append(df.metadata.details[fn]['labels'])
         df.metadata.label_key = create_behavior_labels(label_files)
 
+    label_cols = []
     for vid in df.metadata.details:
-        if 'labels' in df.metadata.details[vid]:
-
+        if 'labels' in df.metadata.details[vid] and 'fps' in df.metadata.details[vid]:
             fn_in = df.metadata.details[vid]['labels']
             fps = df.metadata.details[vid]['fps']
             duration = df.metadata.details[vid]['duration']
 
-            ground_truth, _ = read_boris_annotation(fn_in, fps, duration, df.metadata.label_key)
+            ground_truth = read_boris_annotation(fn_in, fps, duration, df.metadata.label_key.values())
 
-            df.loc[df['filename'] == vid, col_name] = ground_truth
+            for behavior in ground_truth:
+                col_name = 'label_' + behavior
+                label_cols.append(col_name)
+                if col_name not in df.columns:
+                    df[col_name] = 0.
+                df.loc[df['filename'] == vid, col_name] = ground_truth[behavior]
 
     if set_as_label:
-        df.ml.label_cols = col_name
+        df.ml.label_cols = list(set(label_cols))
 
 def load_experiment(fn_in : str) -> pd.DataFrame:
     """Load DataFrame from file.
     
     Args:
         fn_in: path to file to load
         
@@ -811,7 +844,8 @@
 
     if len(df.ml.features) == 0 or len(df.ml.labels) == 0 or len(df.ml.group) == 0:
         warnings.warn("features, labels or groups is empyt, cannot make predictions")
         return
 
     preds = cross_val_predict(model, df.ml.features, df.ml.labels, groups = df.ml.group, cv = cv)
     df['prediction'] = preds
+
```

### Comparing `ethome-ml-0.4.0/ethome_ml.egg-info/PKG-INFO` & `ethome-ml-0.5.0/ethome_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethome-ml
-Version: 0.4.0
+Version: 0.5.0
 Summary: Machine learning for animal behavior analysis
 Home-page: https://github.com/benlansdell/ethome
 Author: Ben Lansdell
 Author-email: ben.lansdell@gmail.com
 Project-URL: Bug Tracker, https://github.com/benlansdell/ethome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 ![build](https://github.com/benlansdell/ethome/actions/workflows/workflow.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ethome-ml.svg)](https://badge.fury.io/py/ethome-ml)
 
 # Ethome
 
 Tools for machine learning of animal behavior.
 
-This library interprets pose-tracking files (at present, from DLC or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
+This library interprets pose-tracking files (at present, from DLC, SLEAP or NWB formats) and behavior annotations (at present, from BORIS and NWB formats) to help train a behavior classifier, interpolate data and other common analysis tasks. 
 
 ## Features
 
 * Read in animal pose data and corresponding behavior annotations to make supervised learning easy
 * Scale data to desired physical units
 * Interpolate pose data to improve low-confidence predictions 
 * Create generic features for analysis and downstream ML tasks
```

### Comparing `ethome-ml-0.4.0/ethome_ml.egg-info/SOURCES.txt` & `ethome-ml-0.5.0/ethome_ml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 ethome_ml.egg-info/SOURCES.txt
 ethome_ml.egg-info/dependency_links.txt
 ethome_ml.egg-info/requires.txt
 ethome_ml.egg-info/top_level.txt
 tests/test_analysis.py
 tests/test_io.py
 tests/test_models.py
+tests/test_plot.py
 tests/test_unsupervised.py
 tests/test_utils.py
```

### Comparing `ethome-ml-0.4.0/setup.cfg` & `ethome-ml-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/tests/test_analysis.py` & `ethome-ml-0.5.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.4.0/tests/test_io.py` & `ethome-ml-0.5.0/tests/test_io.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,51 @@
 #####################
 ## Setup test code ##
 #####################
 
 import pandas as pd
 
+# def test_nwb_dandiset231_import():
+#     from ethome import create_dataset
+#     path = '/home/blansdel/projects/ethome/ethome/data/sample_nwb_dandiset_231.nwb'
+#     dataset = create_dataset(path)
+#     assert type(dataset) is pd.DataFrame
+
+def test_dataset_creation_list(tracking_files):
+
+    from ethome.io import get_sample_nwb_paths
+    from ethome import create_dataset
+    import os 
+    from glob import glob 
+
+    #Create dataset from openfield nwb and openfield DLC
+    cur_dir = os.path.dirname(os.path.abspath(__file__))
+    openfield_path = glob(os.path.join(cur_dir, '..', 'ethome', 'data', 'dlc', 'openfield', '*missingdata.csv'))[0]
+
+    nwb_path = get_sample_nwb_paths()
+    dataset = create_dataset([nwb_path, openfield_path], animal_renamer = {'PoseEstimation':'ind1'})
+    assert type(dataset) is pd.DataFrame
+
+    dataset = create_dataset(tracking_files)
+    assert type(dataset) is pd.DataFrame
+
 def test_nwb_import():
     from ethome.io import get_sample_nwb_paths
     from ethome import create_dataset
     path = get_sample_nwb_paths()
     dataset = create_dataset(path)
     assert type(dataset) is pd.DataFrame
 
+def test_sleap_import(sleap_file):
+    from ethome.io import read_sleap_tracks
+    df = read_sleap_tracks(sleap_file)
+    assert type(df[0]) is pd.DataFrame
+    assert df[1] == ['abdomen', 'eyeL', 'eyeR', 'forelegL4', 'forelegR4', 'head', 'hindlegL4', 'hindlegR4', 'midlegL4', 'midlegR4', 'thorax', 'wingL', 'wingR']
+    assert df[2] == ['Animal0', 'Animal1']
+
 def test_sample_data():
     from ethome.io import get_sample_data
     dataset = get_sample_data()
     assert type(dataset) is pd.DataFrame
 
 def test_sample_paths():
     from ethome.io import get_sample_data_paths
@@ -25,14 +56,24 @@
 
 def test_sample_singlemouse_data():
     from ethome.video import get_sample_openfield_data
     df = get_sample_openfield_data()
     assert df.pose.animals == ['ind1']
     assert len(df.columns) == 15
 
+def test_sample_simultaneous_behavior_data(tracking_files, simultaneous_labels):
+    import numpy as np
+    from ethome import create_dataset, create_metadata
+    metadata = create_metadata(tracking_files[:1], 
+                               labels = simultaneous_labels,
+                               fps = 30)
+
+    df = create_dataset(metadata)
+    assert 2 in np.unique(df.ml.labels.sum(axis = 1))
+
 def test_multiple_boris_behaviors():
     import os 
     from glob import glob 
     from ethome import create_dataset, create_metadata
     import numpy as np
 
     cur_dir = os.path.dirname(os.path.abspath(__file__))
@@ -58,15 +99,15 @@
     import os 
     from glob import glob 
     from ethome import create_dataset, create_metadata
 
     cur_dir = os.path.dirname(os.path.abspath(__file__))
     tracking_files = glob(os.path.join(cur_dir, '..', 'ethome', 'data', 'dlc', 'openfield', '*missingdata.csv'))
     fps = 30                         # (int) frames per second
-    resolution = (480, 640)        # (tuple) HxW in pixels
+    resolution = (480, 640)          # (tuple) HxW in pixels
     #Metadata is a dictionary that attaches each of the above parameters to the video/behavior annotations
     metadata = create_metadata(tracking_files, 
                             fps = fps, 
                             resolution = resolution)
 
     edf = create_dataset(metadata)
```

### Comparing `ethome-ml-0.4.0/tests/test_unsupervised.py` & `ethome-ml-0.5.0/tests/test_unsupervised.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 ## Setup test code ##
 #####################
 
 import pytest
 
 import numpy as np
 
-from ethome.unsupervised import compute_tsne_embedding, compute_morlet, \
+from ethome.unsupervised import compute_tsne_embedding, compute_morlet, compute_umap_embedding, \
                                   compute_density, compute_watershed, cluster_behaviors
 
 N_ROWS = 200
 
+def test_umap_embedding(dataset, default_track_cols):
+    embedding = compute_umap_embedding(dataset, default_track_cols, N_rows = N_ROWS)
+    assert embedding.shape == (len(dataset), 2)
+
 def test_tsne_embedding(dataset, default_track_cols):
     embedding, indices = compute_tsne_embedding(dataset, default_track_cols, N_rows = N_ROWS)
     assert embedding.shape == (N_ROWS, 2)
     assert len(indices) == N_ROWS
 
 def test_compute_morlet(dataset, default_track_cols):
     print(default_track_cols)
@@ -37,17 +41,16 @@
 
 def test_compute_watershed(dens_matrix):
     labels = compute_watershed(dens_matrix)
     assert labels.shape == dens_matrix.shape
 
 def test_cluster_behaviors(dataset, default_track_cols):
     cluster_results = cluster_behaviors(dataset, default_track_cols, N_rows = 200)
-
     assert 'embedding_index_0' in dataset.columns
     assert 'embedding_index_1' in dataset.columns
     assert 'unsup_behavior_label' in dataset.columns
 
     #Test Morlet
-    cluster_results = cluster_behaviors(dataset, default_track_cols, use_morlet = True, N_rows = 200)
+    #cluster_results = cluster_behaviors(dataset, default_track_cols, use_morlet = True, N_rows = 200)
 
     #Test TSNE
-    cluster_results = cluster_behaviors(dataset, default_track_cols, use_umap = False, N_rows = 200)
+    #cluster_results = cluster_behaviors(dataset, default_track_cols, use_umap = False, N_rows = 200)
```

