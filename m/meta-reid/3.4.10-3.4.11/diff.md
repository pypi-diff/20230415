# Comparing `tmp/meta-reid-3.4.10.tar.gz` & `tmp/meta-reid-3.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-reid-3.4.10.tar", last modified: Tue Apr 11 04:03:19 2023, max compression
+gzip compressed data, was "dist/meta-reid-3.4.11.tar", last modified: Sat Apr 15 04:33:14 2023, max compression
```

## Comparing `meta-reid-3.4.10.tar` & `meta-reid-3.4.11.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/
--rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-04-11 04:03:19.000000 meta-reid-3.4.10/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-03-13 10:34:15.000000 meta-reid-3.4.10/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/meta_reid.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      499 2023-04-11 04:03:19.000000 meta-reid-3.4.10/meta_reid.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       69 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/
--rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-03-14 03:19:31.000000 meta-reid-3.4.10/metareid/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)       83 2023-03-14 03:19:10.000000 meta-reid-3.4.10/metareid/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-03-20 06:12:28.000000 meta-reid-3.4.10/metareid/app/onnx_to_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4299 2023-04-10 13:20:47.000000 meta-reid-3.4.10/metareid/app/reid_inference_trt.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)       60 2023-03-20 06:14:45.000000 meta-reid-3.4.10/metareid/model_zoo/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4789 2023-04-11 04:01:10.000000 meta-reid-3.4.10/metareid/model_zoo/trt_engine.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    12524 2023-03-20 06:16:43.000000 meta-reid-3.4.10/metareid/model_zoo/trt_export.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       50 2023-03-20 06:14:05.000000 meta-reid-3.4.10/metareid/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      608 2023-03-20 01:47:13.000000 meta-reid-3.4.10/metareid/utils/general.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-reid-3.4.10/metareid/utils/image_batch.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-11 04:03:19.000000 meta-reid-3.4.10/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      712 2023-04-11 04:02:20.000000 meta-reid-3.4.10/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-15 04:33:14.000000 meta-reid-3.4.11/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-04-15 04:33:14.000000 meta-reid-3.4.11/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-03-13 10:34:15.000000 meta-reid-3.4.11/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-15 04:33:14.000000 meta-reid-3.4.11/meta_reid.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-04-15 04:33:14.000000 meta-reid-3.4.11/meta_reid.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      499 2023-04-15 04:33:14.000000 meta-reid-3.4.11/meta_reid.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-15 04:33:14.000000 meta-reid-3.4.11/meta_reid.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       69 2023-04-15 04:33:14.000000 meta-reid-3.4.11/meta_reid.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-04-15 04:33:14.000000 meta-reid-3.4.11/meta_reid.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-15 04:33:14.000000 meta-reid-3.4.11/meta_reid.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-15 04:33:14.000000 meta-reid-3.4.11/metareid/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-03-14 03:19:31.000000 meta-reid-3.4.11/metareid/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-15 04:33:14.000000 meta-reid-3.4.11/metareid/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       83 2023-03-14 03:19:10.000000 meta-reid-3.4.11/metareid/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-03-20 06:12:28.000000 meta-reid-3.4.11/metareid/app/onnx_to_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4654 2023-04-15 04:28:49.000000 meta-reid-3.4.11/metareid/app/reid_inference_trt.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-15 04:33:14.000000 meta-reid-3.4.11/metareid/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       60 2023-03-20 06:14:45.000000 meta-reid-3.4.11/metareid/model_zoo/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4789 2023-04-11 04:01:10.000000 meta-reid-3.4.11/metareid/model_zoo/trt_engine.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    12524 2023-03-20 06:16:43.000000 meta-reid-3.4.11/metareid/model_zoo/trt_export.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-15 04:33:14.000000 meta-reid-3.4.11/metareid/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       50 2023-03-20 06:14:05.000000 meta-reid-3.4.11/metareid/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      608 2023-03-20 01:47:13.000000 meta-reid-3.4.11/metareid/utils/general.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-reid-3.4.11/metareid/utils/image_batch.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-15 04:33:14.000000 meta-reid-3.4.11/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      712 2023-04-15 04:29:48.000000 meta-reid-3.4.11/setup.py
```

### Comparing `meta-reid-3.4.10/metareid/app/onnx_to_trt.py` & `meta-reid-3.4.11/metareid/app/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.4.10/metareid/app/reid_inference_trt.py` & `meta-reid-3.4.11/metareid/app/reid_inference_trt.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,24 @@
     def __init__(self,
                  trt_file="models/baseline_R50.trt",
                  new_size=(224, 224),
                  gpu_idx=0,
                  batch_size=24,
                  class_nums=19,
                  use_gpu=False,
+                 total_memory=5000,
                  query_file_path='models/query_files.npy',
                  query_name_path='models/query_names.npy',
                  query_feature_path='models/query_features.npy'):
         self.new_size = new_size
         self.model = TrtEngine(trt_file, gpu_idx=gpu_idx, batch_size=batch_size)
         self.query_file_path = query_file_path
         self.query_name_path = query_name_path
         self.query_feature_path = query_feature_path
+        self.total_memory = total_memory
         self.query_files, self.query_names, self.query_features = self.load_features()
         self.use_gpu = use_gpu
         self.invert_index = self.get_invert_index(n_list=class_nums) if self.use_gpu else None
 
     def predict(self, image):
         # rgb
         if not isinstance(image, list): image = [image]
@@ -67,14 +69,20 @@
             self.query_names = np.append(self.query_names, query_name)
             self.query_features = np.vstack([self.query_features, query_feature])
         else:
             self.query_files = np.array([query_file])
             self.query_names = np.array([query_name])
             self.query_features = query_feature
 
+        if len(self.query_names) > self.total_memory:
+            t = len(self.query_names) - self.total_memory
+            self.query_files = self.query_files[-t:]
+            self.query_names = self.query_names[-t:]
+            self.query_features = self.query_features[-t:]
+
     def save_features(self):
         np.save(self.query_file_path, self.query_files)
         np.save(self.query_name_path, self.query_names)
         np.save(self.query_feature_path, self.query_features)
 
     def save_folder(self, img_dir):
         query_name = img_dir.split('/')[-1]
```

### Comparing `meta-reid-3.4.10/metareid/model_zoo/trt_engine.py` & `meta-reid-3.4.11/metareid/model_zoo/trt_engine.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.4.10/metareid/model_zoo/trt_export.py` & `meta-reid-3.4.11/metareid/model_zoo/trt_export.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.4.10/metareid/utils/general.py` & `meta-reid-3.4.11/metareid/utils/general.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.4.10/metareid/utils/image_batch.py` & `meta-reid-3.4.11/metareid/utils/image_batch.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.4.10/setup.py` & `meta-reid-3.4.11/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'pycuda',
     'numpy',
     'pillow',
     'tqdm',
     'faiss-gpu'
 ]
 
-__version__ = 'V3.04.10'
+__version__ = 'V3.04.11'
 
 setup(
     name='meta-reid',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvreid',
```

