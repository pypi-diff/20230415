# Comparing `tmp/mtsa-0.0.8.tar.gz` & `tmp/mtsa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtsa-0.0.8.tar", last modified: Fri Jan 13 19:37:05 2023, max compression
+gzip compressed data, was "mtsa-0.0.9.tar", last modified: Thu Mar 16 02:30:50 2023, max compression
```

## Comparing `mtsa-0.0.8.tar` & `mtsa-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 19:37:05.846967 mtsa-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      766 2023-01-13 19:37:05.848642 mtsa-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2023-01-13 19:33:50.000000 mtsa-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 19:37:05.632165 mtsa-0.0.8/mtsa/
--rw-r--r--   0 root         (0) root         (0)      170 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/correlation_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 19:37:05.753273 mtsa-0.0.8/mtsa/features/
--rw-r--r--   0 root         (0) root         (0)       39 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/features/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3007 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/features/mel.py
--rw-r--r--   0 root         (0) root         (0)     1253 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/features/stats.py
--rw-r--r--   0 root         (0) root         (0)      202 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/metrics.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/model_selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 19:37:05.791514 mtsa-0.0.8/mtsa/models/
--rw-r--r--   0 root         (0) root         (0)      107 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5878 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/models/hitachi.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/models/mfccmix.py
--rw-r--r--   0 root         (0) root         (0)     2948 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/pipelines.py
--rw-r--r--   0 root         (0) root         (0)     8892 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/plotters.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/training.py
--rw-r--r--   0 root         (0) root         (0)     5570 2023-01-13 19:33:51.000000 mtsa-0.0.8/mtsa/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 19:37:05.724659 mtsa-0.0.8/mtsa.egg-info/
--rw-r--r--   0 root         (0) root         (0)      766 2023-01-13 19:37:05.000000 mtsa-0.0.8/mtsa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-01-13 19:37:05.000000 mtsa-0.0.8/mtsa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:37:05.000000 mtsa-0.0.8/mtsa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      176 2023-01-13 19:37:05.000000 mtsa-0.0.8/mtsa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-13 19:37:05.000000 mtsa-0.0.8/mtsa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:37:05.000000 mtsa-0.0.8/mtsa.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-13 19:33:51.000000 mtsa-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      732 2023-01-13 19:37:05.857720 mtsa-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 19:37:05.840672 mtsa-0.0.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 19:33:51.000000 mtsa-0.0.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      413 2023-01-13 19:33:51.000000 mtsa-0.0.8/tests/test_DCASE2020_task2.py
--rw-r--r--   0 root         (0) root         (0)      357 2023-01-13 19:33:51.000000 mtsa-0.0.8/tests/test_hitachi.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-01-13 19:33:51.000000 mtsa-0.0.8/tests/test_mfccmix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 02:30:50.874837 mtsa-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      775 2023-03-16 02:30:50.874837 mtsa-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2023-03-16 02:29:09.000000 mtsa-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 02:30:50.870838 mtsa-0.0.9/mtsa/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/correlation_networks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 02:30:50.870838 mtsa-0.0.9/mtsa/features/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/features/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/features/mel.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/features/stats.py
+-rw-r--r--   0 root         (0) root         (0)      202 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-03-16 02:29:09.000000 mtsa-0.0.9/mtsa/model_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 02:30:50.870838 mtsa-0.0.9/mtsa/models/
+-rw-r--r--   0 root         (0) root         (0)      107 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5877 2023-03-16 02:29:09.000000 mtsa-0.0.9/mtsa/models/hitachi.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-03-16 02:29:09.000000 mtsa-0.0.9/mtsa/models/mfccmix.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-03-16 02:29:09.000000 mtsa-0.0.9/mtsa/pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-03-16 02:29:09.000000 mtsa-0.0.9/mtsa/plotters.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-17 10:13:07.000000 mtsa-0.0.9/mtsa/training.py
+-rw-r--r--   0 root         (0) root         (0)     4591 2023-03-16 02:29:09.000000 mtsa-0.0.9/mtsa/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 02:30:50.870838 mtsa-0.0.9/mtsa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      775 2023-03-16 02:30:50.000000 mtsa-0.0.9/mtsa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-03-16 02:30:50.000000 mtsa-0.0.9/mtsa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 02:30:50.000000 mtsa-0.0.9/mtsa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      190 2023-03-16 02:30:50.000000 mtsa-0.0.9/mtsa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-03-16 02:30:50.000000 mtsa-0.0.9/mtsa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 02:30:50.000000 mtsa-0.0.9/mtsa.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2023-01-17 10:13:07.000000 mtsa-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      747 2023-03-16 02:30:50.874837 mtsa-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 02:30:50.870838 mtsa-0.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-17 10:13:07.000000 mtsa-0.0.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      413 2023-01-17 10:13:07.000000 mtsa-0.0.9/tests/test_DCASE2020_task2.py
+-rw-r--r--   0 root         (0) root         (0)      357 2023-01-17 10:13:07.000000 mtsa-0.0.9/tests/test_hitachi.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-01-17 10:13:07.000000 mtsa-0.0.9/tests/test_mfccmix.py
```

### Comparing `mtsa-0.0.8/PKG-INFO` & `mtsa-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsa
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multiple Time Series Analysis
 Home-page: https://github.com/diegompin/mtsa
 Author: Diego Pinheiro
 Author-email: diegompin@gmail.com
 License: BSD 3-Clause License
 Keywords: mtsa,setuptools
 Classifier: License :: OSI Approved :: BSD License
@@ -21,8 +21,8 @@
 
 Find an example [here](examples/MTSA.ipynb)
 
 
 ## The MFCC Paper 2023
 
 ```python
-python scripts/paper2023.py --path=/data/MIMII/  --n_components=230 --level=2 --output=/data/output/ --perplexity=40
+python scripts/paper2023.py --path=/data/MIMII/  --n_components=230 --level=2 --output=/data/output/ --perplexity=40 --runs=3
```

### Comparing `mtsa-0.0.8/mtsa/correlation_networks.py` & `mtsa-0.0.9/mtsa/correlation_networks.py`

 * *Files identical despite different names*

### Comparing `mtsa-0.0.8/mtsa/features/mel.py` & `mtsa-0.0.9/mtsa/features/mel.py`

 * *Files identical despite different names*

### Comparing `mtsa-0.0.8/mtsa/features/stats.py` & `mtsa-0.0.9/mtsa/features/stats.py`

 * *Files identical despite different names*

### Comparing `mtsa-0.0.8/mtsa/model_selection.py` & `mtsa-0.0.9/mtsa/model_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class MFCCMixCV(MFCCMix):
     
     def __init__(
         self,
         sampling_rate = 16000,
-        random_state = 10000,
+        random_state = None,
         cv=None) -> None:
         super(MFCCMixCV, self).__init__(
             random_state=random_state,
             sampling_rate=sampling_rate
             )
         if not cv:
             cv = ShuffleSplit(
```

### Comparing `mtsa-0.0.8/mtsa/models/hitachi.py` & `mtsa-0.0.9/mtsa/models/hitachi.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     
       :References:
     Purohit, Harsh, et al. "MIMII Dataset: Sound dataset for malfunctioning industrial machine investigation and inspection." arXiv preprint arXiv:1909.09347 (2019).
     
     """
     def __init__(self, 
                  sampling_rate=None,
-                 random_state = 10000,
+                 random_state = None,
                  n_mels=64,
                  frames=5,
                  n_fft=1024,
                  hop_length=512,
                  power=2.0,
                  mono=False,
                  epochs=50,
```

### Comparing `mtsa-0.0.8/mtsa/models/mfccmix.py` & `mtsa-0.0.9/mtsa/models/mfccmix.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 class MFCCMix(BaseEstimator, OutlierMixin):
 
     def __init__(self, 
                  final_model=FINAL_MODEL, 
                  features=FEATURES,
                  sampling_rate=None,
-                 random_state = 10000,
+                 random_state = None,
                  ) -> None:
         super().__init__()
         self.sampling_rate = sampling_rate
         self.final_model = final_model
         self.random_state = random_state
         self.features = features
         self.model = self._build_model()
```

### Comparing `mtsa-0.0.8/mtsa/pipelines.py` & `mtsa-0.0.9/mtsa/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     
     def plot_tsne(self, X_train, X_test, y_train, y_test, **kwargs):
         self.mtsa.fit(X_train, y_train)
         
         perplexity = 4
         if 'perplexity' in kwargs:
             perplexity = kwargs['perplexity']
-        tsne = TSNE(n_components=2, verbose=1, perplexity=perplexity, n_iter=300, random_state=10000)
+        tsne = TSNE(n_components=2, verbose=1, perplexity=perplexity, n_iter=300, random_state=None)
         
         X = self.mtsa.model['features'].fit_transform(
             self.mtsa.model['array2mfcc'].fit_transform(
             self.mtsa.model['wav2array'].fit_transform(X_test)))
         
         tsne_results = tsne.fit_transform(X)
         x = tsne_results[:,0]
```

### Comparing `mtsa-0.0.8/mtsa/plotters.py` & `mtsa-0.0.9/mtsa/plotters.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if name in kwargs: return kwargs[name]
     return default
 
 def get_tsne_results(model, X, y, **kwargs):
     n_components = _get_par('n_components', 2, **kwargs)
     perplexity = _get_par('perplexity', 4, **kwargs)
     n_iter = _get_par('n_iter', 300, **kwargs)
-    random_state = _get_par('random_state', 10000, **kwargs)
+    random_state = _get_par('random_state', None, **kwargs)
     tsne = TSNE(n_components=n_components, verbose=1, perplexity=perplexity, n_iter=n_iter, random_state=random_state)
     
     # Xt = model['features'].fit_transform(
     #     model['array2mfcc'].fit_transform(
     #     model['wav2array'].fit_transform(X)))
     
     tsne_results = tsne.fit_transform(X)
```

### Comparing `mtsa-0.0.8/mtsa.egg-info/PKG-INFO` & `mtsa-0.0.9/mtsa.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsa
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multiple Time Series Analysis
 Home-page: https://github.com/diegompin/mtsa
 Author: Diego Pinheiro
 Author-email: diegompin@gmail.com
 License: BSD 3-Clause License
 Keywords: mtsa,setuptools
 Classifier: License :: OSI Approved :: BSD License
@@ -21,8 +21,8 @@
 
 Find an example [here](examples/MTSA.ipynb)
 
 
 ## The MFCC Paper 2023
 
 ```python
-python scripts/paper2023.py --path=/data/MIMII/  --n_components=230 --level=2 --output=/data/output/ --perplexity=40
+python scripts/paper2023.py --path=/data/MIMII/  --n_components=230 --level=2 --output=/data/output/ --perplexity=40 --runs=3
```

### Comparing `mtsa-0.0.8/mtsa.egg-info/SOURCES.txt` & `mtsa-0.0.9/mtsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtsa-0.0.8/setup.cfg` & `mtsa-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mtsa
-version = 0.0.8
+version = 0.0.9
 author = Diego Pinheiro
 author_email = diegompin@gmail.com
 url = https://github.com/diegompin/mtsa
 description = Multiple Time Series Analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = mtsa, setuptools
@@ -25,12 +25,13 @@
 	scipy==1.10.0
 	ipykernel==6.16.0
 	librosa==0.9.2
 	scikit-learn==1.2.0
 	tensorflow==2.11.0
 	keras==2.11.0
 	seaborn==0.12.2
+	tables==3.8.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

