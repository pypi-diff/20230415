# Comparing `tmp/napari_griottes-0.3.9.tar.gz` & `tmp/napari_griottes-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_griottes-0.3.9.tar", last modified: Fri Mar 10 16:27:12 2023, max compression
+gzip compressed data, was "napari_griottes-0.4.0.tar", last modified: Fri Apr 14 22:05:29 2023, max compression
```

## Comparing `napari_griottes-0.3.9.tar` & `napari_griottes-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:12.002077 napari_griottes-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:11.998077 napari_griottes-0.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:11.998077 napari_griottes-0.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:11.998077 napari_griottes-0.3.9/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-03-10 16:27:12.002077 napari_griottes-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-10 16:27:12.002077 napari_griottes-0.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:11.998077 napari_griottes-0.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:12.002077 napari_griottes-0.3.9/src/napari_griottes/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:12.002077 napari_griottes-0.3.9/src/napari_griottes/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-10 16:27:11.000000 napari_griottes-0.3.9/src/napari_griottes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/src/napari_griottes/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:27:12.002077 napari_griottes-0.3.9/src/napari_griottes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-03-10 16:27:11.000000 napari_griottes-0.3.9/src/napari_griottes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-10 16:27:11.000000 napari_griottes-0.3.9/src/napari_griottes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 16:27:11.000000 napari_griottes-0.3.9/src/napari_griottes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-10 16:27:11.000000 napari_griottes-0.3.9/src/napari_griottes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-10 16:27:11.000000 napari_griottes-0.3.9/src/napari_griottes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 16:27:11.000000 napari_griottes-0.3.9/src/napari_griottes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-10 16:26:26.000000 napari_griottes-0.3.9/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/src/napari_griottes/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/src/napari_griottes/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/src/napari_griottes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/vectors.py
```

### Comparing `napari_griottes-0.3.9/.github/workflows/test_and_deploy.yml` & `napari_griottes-0.4.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/.gitignore` & `napari_griottes-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/.napari/DESCRIPTION.md` & `napari_griottes-0.4.0/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/.pre-commit-config.yaml` & `napari_griottes-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/LICENSE` & `napari_griottes-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/PKG-INFO` & `napari_griottes-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_griottes
-Version: 0.3.9
+Version: 0.4.0
 Summary: Create graphs
 Home-page: https://github.com/aaristov/napari-griottes
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/aaristov/napari-griottes/issues
 Project-URL: Documentation, https://github.com/aaristov/napari-griottes#README.md
```

### Comparing `napari_griottes-0.3.9/README.md` & `napari_griottes-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/setup.cfg` & `napari_griottes-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 [options]
 packages = find:
 install_requires = 
 	griottes
 	networkx
 	numpy
-	pandas
+	pandas<2
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes/_reader.py` & `napari_griottes-0.4.0/src/napari_griottes/_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 import pandas
 import pandas as pd
 from tifffile import imread
 
 from ._widget import CNAME, POINT_PARAMS
 import logging 
+import json
 
 
 
 def napari_get_reader(path):
     """A basic implementation of a Reader contribution.
 
     Parameters
@@ -38,37 +39,41 @@
 
     # if we know we cannot read the file, we immediately return None.
     if path.endswith(".tif") or path.endswith(".tiff"):
         return read_tif
 
     if path.endswith(".csv"):
         return read_csv
-
-    if path.endswith(".griottes"):
-        return read_griottes
+    
+    if path.endswith(".json"):
+        return load_graph_from_json
 
     # otherwise we return the *function* that can read ``path``.
     if path.endswith(".npy"):
         return reader_numpy
 
     return None
 
 
 def read_tif(path="", **kwargs):
     print(f"Opening {path}")
     data = imread(path)
     print(f"input shape: {data.shape}")
+    if data.ndim < 3:
+        channel_axis = None
+    else:
+        channel_axis = 0
     if data.shape[-1] < 10:
         dims = list(range(data.ndim))
         last_dim = dims.pop()
         dims.insert(0, last_dim)
         data = data.transpose(*dims)
         print(f"transpose -> {data.shape}")
 
-    return [(data, {"channel_axis": 0, **kwargs}, "image")]
+    return [(data, {"channel_axis": channel_axis, **kwargs}, "image")]
 
 
 def read_csv(path, **kwargs):
     data = pandas.read_csv(path, index_col=None)
     try:
         return colorized_points(data, metadata={"path": path})
     except Exception as e:
@@ -103,19 +108,35 @@
                 ),
                 **kwargs,
             },
             "points",
         )
     ]
 
-def read_griottes(
-    path,
-):
 
-    G = nx.read_gpickle(path)
+def load_graph_from_json(filename):
+    with open(filename, 'r') as file:
+        data = json.load(file)
+
+    graph = nx.Graph()
+
+    for node_data in data['nodes']:
+        node_id, props = node_data
+        graph.add_node(node_id, **props)
+
+    for edge_data in data['edges']:
+        source, target, props = edge_data
+        graph.add_edge(source, target, **props)
+
+    return read_graph(graph)
+
+
+def read_graph(
+    G,
+):
     pos = nx.get_node_attributes(G, "pos")
 
     try:
         centers = pd.DataFrame(
             [
                 {"z": v[0], "y": v[1], "x": v[2], "label": k}
                 for k, v in pos.items()
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes/_sample_data.py` & `napari_griottes-0.4.0/src/napari_griottes/_sample_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,25 @@
 GRIOTTES_DATA = [
     ("zebrafish_brain_cell_labels.tiff", read_tif),
     ("zebrafish_cell_properties.csv", read_csv),
 ]
 
 
 def make_zebrafish_data():
-    return _load_griottes_sample_data(
-        *GRIOTTES_DATA[0],
-        name=["ch 1", "ch 2", "ch 3", "ch 4", "labels"],
-        colormap=["cyan", "yellow", "magenta", "red", "viridis"],
-    )
+    data = _load_griottes_sample_data(*GRIOTTES_DATA[0])[0][0]
+    return[
+        (
+            d, {"name": name}, layer_type) \
+            for d, name, layer_type in \
+            zip(
+                data, 
+                ["ch 1", "ch 2", "ch 3", "ch 4", "labels"],
+                ["image", "image", "image", "image", "labels" ]
+            )
+    ]
 
 
 def make_cell_properties():
 
     return _load_griottes_sample_data(*GRIOTTES_DATA[1])
 
 
@@ -36,15 +42,15 @@
     url,
     file_path,
 ):
     import shutil
 
     import urllib3
 
-    print(f"Donloading {url}")
+    print(f"Downloading {url}")
     c = urllib3.PoolManager()
     with c.request("GET", url, preload_content=False) as resp, open(
         file_path, "wb"
     ) as out_file:
         shutil.copyfileobj(resp, out_file)
     resp.release_conn()
     print(f"Saved {file_path}")
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes/_tests/test_reader.py` & `napari_griottes-0.4.0/src/napari_griottes/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/src/napari_griottes/_tests/test_widget.py` & `napari_griottes-0.4.0/src/napari_griottes/_tests/test_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     assert len(viewer.layers) == nlayers + 2
     
     saver = save_graph()
     savepath = os.path.join(os.path.curdir, "test.tif")
     
     saver(viewer.layers[-1], path=savepath)
 
-    assert os.path.exists(savepath+".griottes")
-    os.remove(savepath+".griottes")
+    assert os.path.exists(savepath+".json")
+    os.remove(savepath+".json")
 
 
 def test_contact_graph(make_napari_viewer, capsys):
     viewer = make_napari_viewer()
     viewer.open_sample("napari-griottes", "zebra")
     nlayers = len(viewer.layers)
     # this time, our widget will be a MagicFactory or FunctionGui instance
@@ -47,16 +47,20 @@
     assert len(viewer.layers) == nlayers + 2
     
     saver = save_graph()
     savepath = os.path.join(os.path.curdir, "test.tif")
     
     saver(viewer.layers[-1], path=savepath)
 
-    assert os.path.exists(savepath+".griottes")
-    os.remove(savepath+".griottes")
+    assert os.path.exists(ppp:=savepath+".json")
+
+    layers = viewer.open(ppp, plugin="napari-griottes")
+    assert len(layers) == 2
+
+    os.remove(savepath+".json")
 
 def test_geometric_graph(make_napari_viewer, capsys):
     viewer = make_napari_viewer()
     viewer.open_sample("napari-griottes", "zebra")
     nlayers = len(viewer.layers)
     # this time, our widget will be a MagicFactory or FunctionGui instance
     my_widget = make_graph()
@@ -71,9 +75,9 @@
     assert len(viewer.layers) == nlayers + 2
     
     saver = save_graph()
     savepath = os.path.join(os.path.curdir, "test.tif")
     
     saver(viewer.layers[-1], path=savepath)
 
-    assert os.path.exists(savepath+".griottes")
-    os.remove(savepath+".griottes")
+    assert os.path.exists(savepath+".json")
+    os.remove(savepath+".json")
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes/_widget.py` & `napari_griottes-0.4.0/src/napari_griottes/_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 """
 import griottes
 import napari
 import networkx as nx
 import numpy as np
 import pandas as pd
 from magicgui import magic_factory
-from qtpy.QtWidgets import QHBoxLayout, QPushButton, QWidget
 import logging
-import pickle
 import os
 
+from ._writer import save_graph_to_json
+
 logger = logging.getLogger("griottes.widget")
 logger.setLevel(logging.INFO)
 
 FUNCS = {
     "Delaunay": griottes.generate_delaunay_graph,
     "Contact_graph": griottes.generate_contact_graph,
     "Geometric graph": griottes.generate_geometric_graph,
 }
 CNAME = "Graph"
 POINT_PARAMS = {"size":10,  "opacity": .8, "name": "Centers"}
 
 @magic_factory()
 def save_graph(
-    graph_layer: "napari.layers.Vectors",
+    graph_layer: "napari.layers.Layer",
     path: str
 ):
     graph = graph_layer.metadata["graph"]
     return _save_graph(graph=graph, path=path)
     
 
 @magic_factory(
-    auto_call=True,
+    auto_call=False,
     graph={
         "widget_type": "ComboBox",
         "choices": FUNCS.keys(),
     },
     distance={
         "widget_type": "Slider",
         "min": 10,
@@ -55,15 +55,15 @@
     graph: "str",
     distance: "int" = 85,
     thickness: "int" = 1,
 ) -> napari.types.LayerDataTuple:
 
     # logger.info(f"you have selected {img_layer}, {img_layer.data.shape}")
     datapath = label_layer.source.path
-    savepath = None if datapath is None else datapath + ".graph.griottes"
+    savepath = None if datapath is None else datapath + ".json"
 
     if point_layer is None:
         return make_point_layer(label_layer=label_layer)
     data = pd.DataFrame(point_layer.properties)
     repr(data.head())
     weights = thickness
     logger.info(f"{len(data)} nodes")
@@ -105,32 +105,33 @@
             lines = [[pos[i] for i in ids] for ids in list(G.edges)]
 
             vectors = lines2vectors(lines)
             logger.info(
                 f"{len(lines)} edges for {len(pos)}  positions computed, rendering...")
             data = vectors
             dtype = 'vectors'
-        except TypeError:
+        except (TypeError, UnboundLocalError, AssertionError):
             logger.info("contact graph")
             try:
                 G = FUNCS[graph](
                     label_layer.data,
                 )
                 pos = nx.get_node_attributes(G, "pos")
                 lines = [[pos[i] for i in ids] for ids in list(G.edges)]
             except Exception as e:
                 logger.error(f"Contact graph failed: {e}")
+                raise e
                 data = []
                 dtype = "vectors"
             try:
                 weights = [
                     0.2 * thickness * e[2]["weight"]
                     for e in G.edges(data=True)
                 ]
-            except IndexError:
+            except (IndexError, UnboundLocalError):
                 logger.warning(
                     "weights failed!",
                 )
                 weights = 0.2 * thickness
             data = lines
             dtype = 'shapes'
             kwargs = {"shape_type": "line", "name": "Contact graph"}
@@ -165,18 +166,17 @@
             "vectors",
         )
     ]
 
 
 def _save_graph(graph, path):
     try:
-        savepath = path if path.endswith(".griottes") else path + ".griottes"
+        savepath = path if path.endswith(".json") else path + ".json"
         assert not os.path.exists(savepath), f"File exists: {savepath}"
-        with open(savepath, 'wb') as f:
-            pickle.dump(graph, f)
+        save_graph_to_json(graph, savepath)
         print(f"Saved graph to {savepath}")
         return [savepath]
     except Exception as e:
         print(f"Unable to save the graph to {savepath}: {e}")
 
         return None
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes/_writer.py` & `napari_griottes-0.4.0/src/napari_griottes/_writer.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,35 +7,58 @@
 Replace code below according to your needs.
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Sequence, Tuple, Union
 
 import networkx as nx
+import json
 
 if TYPE_CHECKING:
     DataType = Union[Any, Sequence[Any]]
     FullLayerData = Tuple[DataType, dict, str]
 
+import numpy as np
+
+def numpy_to_python(value):
+    if isinstance(value, np.generic):
+        return value.tolist()
+    return value
+
+def save_graph_to_json(graph, filename):
+    
+    with open(filename, 'w') as file:
+        json.dump({
+            "nodes": list(graph.nodes.data()),
+            "edges": list(graph.edges.data())
+        }, file, default=_ser)
+    return [filename]
+
+def _ser(o):
+    """convert types for json.dumps to work"""
+    try:
+        if isinstance(o, (int, np.int32, np.uint16, np.intc, np.int64)):
+            return int(o)
+        elif isinstance(o, (float, str)):
+            return o
+        else:
+            return list(o)
+    except TypeError as e:
+        print(o, type(o))
+        raise e
 
 def save_graph(path: str, data: FullLayerData, props: dict, **kwargs):
     """Writes a single layer graph"""
     try:
-        nx.write_gpickle(
-            props["metadata"]["graph"],
-            (
-                ppp := (
-                    path if path.endswith(".griottes") else path + ".griottes"
-                )
-            ),
-        )
-        print(f"Saved graph to {ppp}")
+        ppp = path if path.endswith(".json") else path + ".json"
+        out = save_graph_to_json(data.metadata["graph"], ppp)
+        print(f"Saved graph to {out}")
     except KeyError:
         print("Grapth not found, choose another layer")
-    return [ppp]
+    return [out]
 
 
 # (
 #     '/home/aaristov/test',
 
 #     [
 #         <class 'numpy.ndarray'> (2, 2) float64,
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes/napari.yaml` & `napari_griottes-0.4.0/src/napari_griottes/napari.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 contributions:
   commands:
     - id: napari-griottes.get_reader
       python_name: napari_griottes._reader:napari_get_reader
       title: Open data with Griottes
 
     - id: napari-griottes.save_graph
-      python_name: napari_griottes._writer:save_graph
+      python_name: napari_griottes._writer:save_graph_to_json
       title: Save graph with Griottes
 
     - id: napari-griottes.save_graph_widget
       python_name: napari_griottes._widget:save_graph
       title: Save graph 
 
     - id: napari-griottes.make_zebrafish_data
@@ -26,20 +26,20 @@
       python_name: napari_griottes._widget:make_graph
       title: Make graph
 
 
   readers:
     - command: napari-griottes.get_reader
       accepts_directories: false
-      filename_patterns: ['*.npy', '*.tif', '*.tiff', '*.csv','*.griottes']
+      filename_patterns: ['*.json', '*.npy', '*.tif', '*.tiff', '*.csv','*.griottes']
 
   writers:
     - command: napari-griottes.save_graph
       layer_types: ['shapes', 'vectors']
-      filename_extensions: ['.griottes']
+      filename_extensions: ['.json']
 
 
   sample_data:
     - command: napari-griottes.make_cell_properties
       display_name: Cell properties table 3D
       key: csv
     - command: napari-griottes.make_zebrafish_data
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes.egg-info/PKG-INFO` & `napari_griottes-0.4.0/src/napari_griottes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-griottes
-Version: 0.3.9
+Version: 0.4.0
 Summary: Create graphs
 Home-page: https://github.com/aaristov/napari-griottes
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/aaristov/napari-griottes/issues
 Project-URL: Documentation, https://github.com/aaristov/napari-griottes#README.md
```

### Comparing `napari_griottes-0.3.9/src/napari_griottes.egg-info/SOURCES.txt` & `napari_griottes-0.4.0/src/napari_griottes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/tox.ini` & `napari_griottes-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.3.9/vectors.py` & `napari_griottes-0.4.0/vectors.py`

 * *Files identical despite different names*

