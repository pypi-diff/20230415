# Comparing `tmp/standard-transform-1.2.0.tar.gz` & `tmp/standard-transform-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard-transform-1.2.0.tar", last modified: Mon Apr 10 23:43:14 2023, max compression
+gzip compressed data, was "standard-transform-1.3.0.tar", last modified: Sat Apr 15 06:35:29 2023, max compression
```

## Comparing `standard-transform-1.2.0.tar` & `standard-transform-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.214937 standard-transform-1.2.0/
--rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.2.0/LICENSE
--rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-04-10 23:37:06.000000 standard-transform-1.2.0/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     7737 2023-04-10 23:43:14.214778 standard-transform-1.2.0/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     7411 2023-04-10 23:37:06.000000 standard-transform-1.2.0/README.md
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-03-28 05:17:19.000000 standard-transform-1.2.0/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-10 23:43:14.214983 standard-transform-1.2.0/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1597 2023-04-10 23:43:10.000000 standard-transform-1.2.0/setup.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.212911 standard-transform-1.2.0/standard_transform/
--rw-r--r--   0 caseysm    (501) staff       (20)      270 2023-04-10 23:40:16.000000 standard-transform-1.2.0/standard_transform/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     7066 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/base.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.214117 standard-transform-1.2.0/standard_transform/data/
--rw-r--r--   0 caseysm    (501) staff       (20)     5384 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/data/v1dd_um_streamline.json
--rw-r--r--   0 caseysm    (501) staff       (20)     4892 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/datasets.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9256 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/streamlines.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1973 2023-02-25 05:35:09.000000 standard-transform-1.2.0/standard_transform/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.213966 standard-transform-1.2.0/standard_transform.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     7737 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      506 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/top_level.txt
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.214435 standard-transform-1.2.0/test/
--rw-r--r--   0 caseysm    (501) staff       (20)     1394 2023-04-10 23:37:06.000000 standard-transform-1.2.0/test/test_streamline.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.2.0/test/test_tform.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.905051 standard-transform-1.3.0/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.3.0/LICENSE
+-rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-04-10 23:37:06.000000 standard-transform-1.3.0/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-15 06:35:29.904875 standard-transform-1.3.0/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     7821 2023-04-15 06:33:04.000000 standard-transform-1.3.0/README.md
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-03-28 05:17:19.000000 standard-transform-1.3.0/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-15 06:35:29.905097 standard-transform-1.3.0/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1597 2023-04-10 23:43:10.000000 standard-transform-1.3.0/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.902946 standard-transform-1.3.0/standard_transform/
+-rw-r--r--   0 caseysm    (501) staff       (20)      270 2023-04-15 06:35:10.000000 standard-transform-1.3.0/standard_transform/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     7066 2023-04-10 23:37:06.000000 standard-transform-1.3.0/standard_transform/base.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.904003 standard-transform-1.3.0/standard_transform/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)    11518 2023-04-15 02:44:52.000000 standard-transform-1.3.0/standard_transform/data/minnie_um_streamline.json
+-rw-r--r--   0 caseysm    (501) staff       (20)     5384 2023-04-10 23:37:06.000000 standard-transform-1.3.0/standard_transform/data/v1dd_um_streamline.json
+-rw-r--r--   0 caseysm    (501) staff       (20)     5320 2023-04-15 05:43:54.000000 standard-transform-1.3.0/standard_transform/datasets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9256 2023-04-10 23:37:06.000000 standard-transform-1.3.0/standard_transform/streamlines.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1973 2023-02-25 05:35:09.000000 standard-transform-1.3.0/standard_transform/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.903571 standard-transform-1.3.0/standard_transform.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      556 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/top_level.txt
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.904559 standard-transform-1.3.0/test/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1394 2023-04-10 23:37:06.000000 standard-transform-1.3.0/test/test_streamline.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.3.0/test/test_tform.py
```

### Comparing `standard-transform-1.2.0/LICENSE` & `standard-transform-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `standard-transform-1.2.0/PKG-INFO` & `standard-transform-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-transform
-Version: 1.2.0
+Version: 1.3.0
 Summary: Define and repeat basic affine transformation tasks for datasets
 Home-page: https://github.com/ceesem/standard_transform
 Author: Casey Schneider-Mizell
 Author-email: caseys@alleninstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -101,14 +101,15 @@
 streamline.depth_along(xyz, depth_from=0)
 ```
 
 Similarly, you can put all of these together to get a point in the curvilienar space of the streamline, akin to cylindrical coordinates, where the x axis is radial distance and the y axis is depth along the streamline. For each point, an equivalent location in x,z space is found with the same radial distance and angle as the original x and z.
 ```python
 xyz_rad = streamline.radial_points(xyz0, pts)
 ```
+NOTE! While better than nothing, the Minnie65 streamline is much more accurate on the VISp side of the dataset (low x values) than on the HVA side (high x values). The right approach will involve creating a streamline that is interpolates values as a function of x and z instead of being a constant. To do this, we need to either create a lot more streamlines by hand (not too hard, but time consuming) or automatically generate streamlines from skeletons. This will be the ideal solution, but for now, treat the streamline as a good approximation for the VISp side of the dataset. 
 
 ## Datasets
 
 Datasets are a convenient way to store a transform and streamline together, and are the easiest way to get started.
 There are two datasets currently available, `minnie65` and `v1dd`.
 To get a dataset, simply import it and initialize it.
 Datasets have a transform and streamline, and can be used to transform points or get streamline information.
@@ -122,17 +123,14 @@
 Or to get the streamline at a particular point:
 ```python
 v1dd_ds.streamline_nm.radial_distance(xyz0, xyz1)
 ```
 
 A particular resolution can be used by passing it as an argument to `dataset.transform_res(voxel_resolution)` or `dataset.streamline_res(voxel_resolution)`.
 
-Note: Currently a data-driven streamline is only available for v1dd.
-Minnie65 is using a placeholder "identity streamline" that is just a straight line in the y direction.
-
 ### Minnie65
 
 * `minnie_transform_nm` : Transform from nanometer units in the original Minnie65 space to microns in a space where the pial surface is flat in x and z along y=0.
 
 * `minnie_transform_vx` : Transform from voxel units in the original Minnie65 space to microns in a space where the pial surface is flat in x and z along y=0. By default, `minnie_transform_vx()` assumes a voxel size of `[4,4,40]` nm/voxel, but specifying a voxel resolution (for example, with `minnie_transform_vx(voxel_resolution=[8,8,40])`) will use a different scale.
 
 Both functions will also take dataframe columns, for example `tform.apply(df['pt_position])`.
```

### Comparing `standard-transform-1.2.0/README.md` & `standard-transform-1.3.0/standard_transform.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: standard-transform
+Version: 1.3.0
+Summary: Define and repeat basic affine transformation tasks for datasets
+Home-page: https://github.com/ceesem/standard_transform
+Author: Casey Schneider-Mizell
+Author-email: caseys@alleninstitute.org
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # standard_transforms
 
 Orient and scale points in EM datasets consistently and easily.
 
 When working with EM data, often the orientation of the dataset does not match the desired orientation in space. For example, in cortical data you might want "down" to correspond to the direction orthogonal to the pial surface. This package includes prebaked affine transforms for two datasets, Minnie65 and V1dd, to convert from voxel or nanometer coordinates to a consistent oriented frame in microns.
 
 Install via `pip install standard-transform`.
@@ -91,14 +101,15 @@
 streamline.depth_along(xyz, depth_from=0)
 ```
 
 Similarly, you can put all of these together to get a point in the curvilienar space of the streamline, akin to cylindrical coordinates, where the x axis is radial distance and the y axis is depth along the streamline. For each point, an equivalent location in x,z space is found with the same radial distance and angle as the original x and z.
 ```python
 xyz_rad = streamline.radial_points(xyz0, pts)
 ```
+NOTE! While better than nothing, the Minnie65 streamline is much more accurate on the VISp side of the dataset (low x values) than on the HVA side (high x values). The right approach will involve creating a streamline that is interpolates values as a function of x and z instead of being a constant. To do this, we need to either create a lot more streamlines by hand (not too hard, but time consuming) or automatically generate streamlines from skeletons. This will be the ideal solution, but for now, treat the streamline as a good approximation for the VISp side of the dataset. 
 
 ## Datasets
 
 Datasets are a convenient way to store a transform and streamline together, and are the easiest way to get started.
 There are two datasets currently available, `minnie65` and `v1dd`.
 To get a dataset, simply import it and initialize it.
 Datasets have a transform and streamline, and can be used to transform points or get streamline information.
@@ -112,17 +123,14 @@
 Or to get the streamline at a particular point:
 ```python
 v1dd_ds.streamline_nm.radial_distance(xyz0, xyz1)
 ```
 
 A particular resolution can be used by passing it as an argument to `dataset.transform_res(voxel_resolution)` or `dataset.streamline_res(voxel_resolution)`.
 
-Note: Currently a data-driven streamline is only available for v1dd.
-Minnie65 is using a placeholder "identity streamline" that is just a straight line in the y direction.
-
 ### Minnie65
 
 * `minnie_transform_nm` : Transform from nanometer units in the original Minnie65 space to microns in a space where the pial surface is flat in x and z along y=0.
 
 * `minnie_transform_vx` : Transform from voxel units in the original Minnie65 space to microns in a space where the pial surface is flat in x and z along y=0. By default, `minnie_transform_vx()` assumes a voxel size of `[4,4,40]` nm/voxel, but specifying a voxel resolution (for example, with `minnie_transform_vx(voxel_resolution=[8,8,40])`) will use a different scale.
 
 Both functions will also take dataframe columns, for example `tform.apply(df['pt_position])`.
```

### Comparing `standard-transform-1.2.0/setup.py` & `standard-transform-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.2.0/standard_transform/base.py` & `standard-transform-1.3.0/standard_transform/base.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.2.0/standard_transform/data/v1dd_um_streamline.json` & `standard-transform-1.3.0/standard_transform/data/v1dd_um_streamline.json`

 * *Files identical despite different names*

### Comparing `standard-transform-1.2.0/standard_transform/datasets.py` & `standard-transform-1.3.0/standard_transform/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from .base import TransformSequence, R, identity_transform
 from .streamlines import Streamline, identity_streamline
 import numpy as np
+import json
 import os
+import warnings
+
+def _get_data_path(filename):
+    return os.path.join(os.path.dirname(__file__), 'data', filename)
+
+V1DD_STREAMLINE_POINT_FILE = _get_data_path('v1dd_um_streamline.json')
+MINNIE_STREAMLINE_POINT_FILE = _get_data_path('minnie_um_streamline.json')
 
-V1DD_STREAMLINE_POINT_FILE = os.path.join(
-    os.path.dirname(__file__),
-    'data',
-    'v1dd_um_streamline.json',
-)
 MINNIE_VOXEL_RESOLUTION = np.array([4, 4, 40])
 V1DD_VOXEL_RESOLUTION = np.array([9, 9, 45])
 
 MINNIE_PIA_POINT_NM = np.array([183013, 83535, 21480]) * [4,4,45]
 V1DD_PIA_POINT_NM = np.array([101249, 32249, 9145]) * [9,9,45]
 
+def _rotation_from_up_vector(up):
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        rot, _ = R.align_vectors(np.array([[0, 1, 0]]), [up])
+    return rot
 
 def _minnie_transforms( tform, pia_point ):
     angle_offset = 5
     
     tform.add_rotation("z", angle_offset, degrees=True)
     tform.add_translation(
         [0, -tform.apply_project("y", pia_point), 0]
     )
     tform.add_scaling(1 / 1000)
     return tform
 
 def _v1dd_transforms( tform, pia_point):
     up = np.array([-0.00497765, 0.96349375, 0.26768454])
-    rot, _ = R.align_vectors(np.array([[0, 1, 0]]), [up])
-
+    rot = _rotation_from_up_vector(up)
     angles = rot.as_euler("xyz", degrees=True)
 
     for ind, ang in zip(["x", "y", "z"], angles):
         tform.add_rotation(ind, ang, degrees=True)
 
     tform.add_translation([0, -tform.apply_project("y", pia_point), 0])
     tform.add_scaling(1 / 1000)
@@ -63,38 +70,42 @@
     return _v1dd_transforms(v1dd_transform, V1DD_PIA_POINT_NM)
 
 #### STREAMLINES
 
 
 def v1dd_streamline_nm():
     "Streamline for v1dd dataset for nm coordinates"
-    import json
     with open(V1DD_STREAMLINE_POINT_FILE, 'r') as f:
         points = np.array(json.load(f))
     return Streamline(points, tform=v1dd_transform_nm(), transform_points=False)
 
 def v1dd_streamline_vx(voxel_resolution=V1DD_VOXEL_RESOLUTION):
     "Streamline for v1dd dataset for voxel coordinates"
-    import json
     with open(V1DD_STREAMLINE_POINT_FILE, 'r') as f:
         points = np.array(json.load(f))
     return Streamline(points, tform=v1dd_transform_vx(voxel_resolution), transform_points=False)
 
 def minnie_streamline_nm():
     "Streamline for minnie65 dataset for nm coordinates"
+    with open(MINNIE_STREAMLINE_POINT_FILE, 'r') as f:
+        points = np.array(json.load(f))
+
     return Streamline(
-        np.array([[0, 0, 0], [0, 1, 0]]),
+        points,
         tform=minnie_transform_nm(),
         transform_points=False,
     )
 
 def minnie_streamline_vx(voxel_resolution=MINNIE_VOXEL_RESOLUTION):
     "Streamline for minnie65 dataset for voxel coordinates"
+    with open(MINNIE_STREAMLINE_POINT_FILE, 'r') as f:
+        points = np.array(json.load(f))
+
     return Streamline(
-        np.array([[0, 0, 0], [0, 1000, 0]]),
+        points,
         tform=minnie_transform_vx(voxel_resolution),
         transform_points=False,
     )
 
 ## Dataset object
 class Dataset(object):
     def __init__(
```

### Comparing `standard-transform-1.2.0/standard_transform/streamlines.py` & `standard-transform-1.3.0/standard_transform/streamlines.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.2.0/standard_transform/utils.py` & `standard-transform-1.3.0/standard_transform/utils.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.2.0/standard_transform.egg-info/PKG-INFO` & `standard-transform-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: standard-transform
-Version: 1.2.0
-Summary: Define and repeat basic affine transformation tasks for datasets
-Home-page: https://github.com/ceesem/standard_transform
-Author: Casey Schneider-Mizell
-Author-email: caseys@alleninstitute.org
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # standard_transforms
 
 Orient and scale points in EM datasets consistently and easily.
 
 When working with EM data, often the orientation of the dataset does not match the desired orientation in space. For example, in cortical data you might want "down" to correspond to the direction orthogonal to the pial surface. This package includes prebaked affine transforms for two datasets, Minnie65 and V1dd, to convert from voxel or nanometer coordinates to a consistent oriented frame in microns.
 
 Install via `pip install standard-transform`.
@@ -101,14 +91,15 @@
 streamline.depth_along(xyz, depth_from=0)
 ```
 
 Similarly, you can put all of these together to get a point in the curvilienar space of the streamline, akin to cylindrical coordinates, where the x axis is radial distance and the y axis is depth along the streamline. For each point, an equivalent location in x,z space is found with the same radial distance and angle as the original x and z.
 ```python
 xyz_rad = streamline.radial_points(xyz0, pts)
 ```
+NOTE! While better than nothing, the Minnie65 streamline is much more accurate on the VISp side of the dataset (low x values) than on the HVA side (high x values). The right approach will involve creating a streamline that is interpolates values as a function of x and z instead of being a constant. To do this, we need to either create a lot more streamlines by hand (not too hard, but time consuming) or automatically generate streamlines from skeletons. This will be the ideal solution, but for now, treat the streamline as a good approximation for the VISp side of the dataset. 
 
 ## Datasets
 
 Datasets are a convenient way to store a transform and streamline together, and are the easiest way to get started.
 There are two datasets currently available, `minnie65` and `v1dd`.
 To get a dataset, simply import it and initialize it.
 Datasets have a transform and streamline, and can be used to transform points or get streamline information.
@@ -122,17 +113,14 @@
 Or to get the streamline at a particular point:
 ```python
 v1dd_ds.streamline_nm.radial_distance(xyz0, xyz1)
 ```
 
 A particular resolution can be used by passing it as an argument to `dataset.transform_res(voxel_resolution)` or `dataset.streamline_res(voxel_resolution)`.
 
-Note: Currently a data-driven streamline is only available for v1dd.
-Minnie65 is using a placeholder "identity streamline" that is just a straight line in the y direction.
-
 ### Minnie65
 
 * `minnie_transform_nm` : Transform from nanometer units in the original Minnie65 space to microns in a space where the pial surface is flat in x and z along y=0.
 
 * `minnie_transform_vx` : Transform from voxel units in the original Minnie65 space to microns in a space where the pial surface is flat in x and z along y=0. By default, `minnie_transform_vx()` assumes a voxel size of `[4,4,40]` nm/voxel, but specifying a voxel resolution (for example, with `minnie_transform_vx(voxel_resolution=[8,8,40])`) will use a different scale.
 
 Both functions will also take dataframe columns, for example `tform.apply(df['pt_position])`.
```

### Comparing `standard-transform-1.2.0/test/test_streamline.py` & `standard-transform-1.3.0/test/test_streamline.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.2.0/test/test_tform.py` & `standard-transform-1.3.0/test/test_tform.py`

 * *Files identical despite different names*

