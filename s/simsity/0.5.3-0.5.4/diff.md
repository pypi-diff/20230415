# Comparing `tmp/simsity-0.5.3.tar.gz` & `tmp/simsity-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simsity-0.5.3.tar", last modified: Tue Apr 11 14:16:26 2023, max compression
+gzip compressed data, was "dist/simsity-0.5.4.tar", last modified: Sat Apr 15 12:14:53 2023, max compression
```

## Comparing `simsity-0.5.3.tar` & `simsity-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 14:16:26.256640 simsity-0.5.3/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-11 14:16:26.256640 simsity-0.5.3/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1827 2023-04-11 13:48:43.000000 simsity-0.5.3/README.md
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-11 14:16:26.256640 simsity-0.5.3/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1399 2023-04-11 14:07:41.000000 simsity-0.5.3/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 14:16:26.256640 simsity-0.5.3/simsity/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4062 2023-04-11 14:03:54.000000 simsity-0.5.3/simsity/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1015 2023-03-28 14:20:47.000000 simsity-0.5.3/simsity/datasets.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2022-12-20 12:12:03.000000 simsity-0.5.3/simsity/error.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 14:16:26.256640 simsity-0.5.3/simsity.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      229 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      150 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/top_level.txt
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:14:53.726307 simsity-0.5.4/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-15 12:14:53.726307 simsity-0.5.4/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1827 2023-04-11 13:48:43.000000 simsity-0.5.4/README.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-15 12:14:53.726307 simsity-0.5.4/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1399 2023-04-15 12:10:27.000000 simsity-0.5.4/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:14:53.726307 simsity-0.5.4/simsity/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4240 2023-04-15 12:09:09.000000 simsity-0.5.4/simsity/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1015 2023-03-28 14:20:47.000000 simsity-0.5.4/simsity/datasets.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2022-12-20 12:12:03.000000 simsity-0.5.4/simsity/error.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:14:53.726307 simsity-0.5.4/simsity.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      229 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      150 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/top_level.txt
```

### Comparing `simsity-0.5.3/PKG-INFO` & `simsity-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simsity
-Version: 0.5.3
+Version: 0.5.4
 Summary: Super Simple Similarity Service
 Home-page: https://github.com/koaning/simsity/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/koaning/simsity/
 Project-URL: Source Code, https://github.com/koaning/simsity/
 Project-URL: Issue Tracker, https://github.com/koaning/simsity/issues
```

### Comparing `simsity-0.5.3/README.md` & `simsity-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `simsity-0.5.3/setup.py` & `simsity-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 all_packages = base_packages
 dev_packages = all_packages + test_packages
 
 
 setup(
     name="simsity",
-    version="0.5.3",
+    version="0.5.4",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
     description="Super Simple Similarity Service",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/koaning/simsity/",
     project_urls={
```

### Comparing `simsity-0.5.3/simsity/__init__.py` & `simsity-0.5.4/simsity/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from queue import LifoQueue
 import datetime as dt
 import itertools as it
 from pathlib import Path
-from typing import Iterable, Protocol
+from typing import Iterable, Protocol, Callable, Union
 
 import srsly
 from hnswlib import Index
 from tqdm import tqdm
 
 DB_NAME = "db.gz.json"
 INDEX_NAME = "index.bin"
@@ -28,15 +28,15 @@
 
     def query(self, query, n=10):
         """
         Query using approximate nearest neighbors
 
         The object handles the encoder/data from disk.
         """
-        arr = self.encoder.transform(query)
+        arr = encode_data(self.encoder, query)
         return self.query_vector(query=arr, n=n)
 
     def query_vector(self, query, n=10):
         """Query using a vector."""
         labels, distances = self.index.knn_query(query, k=n)
         out = [self.db[int(label)] for label in labels[0]]
         return out, list(distances[0])
@@ -74,17 +74,24 @@
 
 def batch(iterable, n=1):
     length = len(iterable)
     for ndx in range(0, length, n):
         yield iterable[ndx : min(ndx + n, length)]
 
 
+def encode_data(encoder, data):
+    if callable(encoder):
+        return encoder(data)
+    else:
+        return encoder.transform(data)
+
+
 def create_index(
     data: Iterable,
-    encoder: Transformer,
+    encoder: Union[Transformer, Callable],
     path: Path = None,
     space="cosine",
     pbar=True,
     batch_size=500,
 ):
     """
     Creates a simple ANN index. Uses hnswlib under the hood.
@@ -93,15 +100,15 @@
     index = None
     batches = batch(data, batch_size)
     if pbar:
         batches, batches_copy = it.tee(batches)
         total = sum(1 for _ in batches_copy)
         batches = tqdm(batches, desc="indexing", total=total)
     for b in batches:
-        encoded = encoder.transform(b)
+        encoded = encode_data(encoder, b)
         if not index:
             dim = encoded.shape[1]
             index = Index(space=space, dim=dim)
             index.init_index(max_elements=len(data))
         index.add_items(encoded)
     if path:
         path = Path(path)
```

### Comparing `simsity-0.5.3/simsity/datasets.py` & `simsity-0.5.4/simsity/datasets.py`

 * *Files identical despite different names*

### Comparing `simsity-0.5.3/simsity/error.py` & `simsity-0.5.4/simsity/error.py`

 * *Files identical despite different names*

### Comparing `simsity-0.5.3/simsity.egg-info/PKG-INFO` & `simsity-0.5.4/simsity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simsity
-Version: 0.5.3
+Version: 0.5.4
 Summary: Super Simple Similarity Service
 Home-page: https://github.com/koaning/simsity/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/koaning/simsity/
 Project-URL: Source Code, https://github.com/koaning/simsity/
 Project-URL: Issue Tracker, https://github.com/koaning/simsity/issues
```

