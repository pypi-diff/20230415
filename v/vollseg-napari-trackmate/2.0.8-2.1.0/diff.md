# Comparing `tmp/vollseg-napari-trackmate-2.0.8.tar.gz` & `tmp/vollseg-napari-trackmate-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-trackmate/dist/.tmp-i2m6jxe6/vollseg-napari-trackmate-2.0.8.tar", last modified: Sat Apr 15 12:25:04 2023, max compression
+gzip compressed data, was "vollseg-napari-trackmate-2.1.0.tar", last modified: Mon Apr  3 07:24:15 2023, max compression
```

## Comparing `vollseg-napari-trackmate-2.0.8.tar` & `vollseg-napari-trackmate-2.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:04.935500 vollseg-napari-trackmate-2.0.8/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:03.655946 vollseg-napari-trackmate-2.0.8/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:03.917446 vollseg-napari-trackmate-2.0.8/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:03.982438 vollseg-napari-trackmate-2.0.8/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-12-31 12:38:29.000000 vollseg-napari-trackmate-2.0.8/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-15 12:25:04.937737 vollseg-napari-trackmate-2.0.8/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2911 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      274 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1876 2023-04-15 12:25:04.949623 vollseg-napari-trackmate-2.0.8/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:03.685414 vollseg-napari-trackmate-2.0.8/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:04.310847 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      433 2023-01-24 18:36:39.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    10964 2022-12-29 02:30:28.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_data_model.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2118 2023-02-01 20:25:52.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:04.819528 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 19:22:05.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      115 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      566 2023-01-07 18:24:47.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      133 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-04-15 12:25:02.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    89613 2023-04-15 12:24:17.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      357 2023-01-07 18:24:48.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/launch.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1514 2023-01-03 11:40:24.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:04.878459 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-15 12:25:04.546779 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4320 2023-04-15 12:25:02.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1189 2023-04-15 12:25:03.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-15 12:25:02.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       82 2023-04-15 12:25:02.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-04-15 12:25:02.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-15 12:25:02.000000 vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      619 2022-12-31 10:29:11.000000 vollseg-napari-trackmate-2.0.8/tox.ini
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.027612 vollseg-napari-trackmate-2.1.0/
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.922360 vollseg-napari-trackmate-2.1.0/.github/
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.937639 vollseg-napari-trackmate-2.1.0/.github/workflows/
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     2814 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.github/workflows/test_and_deploy.yml
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      992 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.gitignore
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.939868 vollseg-napari-trackmate-2.1.0/.napari-hub/
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      463 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.napari-hub/DESCRIPTION.md
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      542 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.napari-hub/config.yml
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1211 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/.pre-commit-config.yaml
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1487 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/LICENSE
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)       96 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/MANIFEST.in
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     4320 2023-04-03 07:24:15.028030 vollseg-napari-trackmate-2.1.0/PKG-INFO
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     2911 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/README.md
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      274 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/pyproject.toml
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1876 2023-04-03 07:24:15.029601 vollseg-napari-trackmate-2.1.0/setup.cfg
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.926238 vollseg-napari-trackmate-2.1.0/src/
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:14.991164 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      433 2023-01-26 21:14:09.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/__init__.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)    10964 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_data_model.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      644 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_sample_data.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     2118 2023-02-01 20:38:39.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.011274 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)        0 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/__init__.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      107 2023-01-07 19:22:38.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      115 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      566 2023-01-07 18:28:11.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      133 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      160 2023-04-03 07:24:14.984625 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_version.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)    81982 2023-04-03 07:22:29.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_widget.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      923 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_writer.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      357 2023-01-07 18:28:11.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/launch.py
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1514 2023-01-03 12:16:33.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/napari.yaml
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.012279 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/resources/
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     6153 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxr-s---   0 uzj81mi  (302337) jsy      (302032)        0 2023-04-03 07:24:15.003440 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     4320 2023-04-03 07:24:14.992907 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)     1189 2023-04-03 07:24:14.995047 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)        1 2023-04-03 07:24:14.996819 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)       82 2023-04-03 07:24:14.998719 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)       85 2023-04-03 07:24:14.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)       25 2023-04-03 07:24:14.000000 vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rw-r-----   0 uzj81mi  (302337) jsy      (302032)      619 2022-12-31 20:17:26.000000 vollseg-napari-trackmate-2.1.0/tox.ini
```

### Comparing `vollseg-napari-trackmate-2.0.8/.github/workflows/test_and_deploy.yml` & `vollseg-napari-trackmate-2.1.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/.gitignore` & `vollseg-napari-trackmate-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/.napari-hub/config.yml` & `vollseg-napari-trackmate-2.1.0/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/.pre-commit-config.yaml` & `vollseg-napari-trackmate-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/LICENSE` & `vollseg-napari-trackmate-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/PKG-INFO` & `vollseg-napari-trackmate-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.0.8
+Version: 2.1.0
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.0.8/README.md` & `vollseg-napari-trackmate-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/setup.cfg` & `vollseg-napari-trackmate-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_data_model.py` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_sample_data.py` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_widget.py` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -843,96 +843,75 @@
         _Color_tracks(spot_attributes, track_attributes)
 
     def _refreshTrackData(pred):
 
         nonlocal _to_analyze
         unique_tracks, unique_tracks_properties, track_id = pred
         features = {
-            "time": np.asarray(unique_tracks_properties, dtype="float16")[
+            "time": np.asarray(unique_tracks_properties, dtype="float64")[
                 :, 0
             ],
             "generation": np.asarray(
-                unique_tracks_properties, dtype="float16"
+                unique_tracks_properties, dtype="float64"
             )[:, 2],
-            "radius": np.asarray(unique_tracks_properties, dtype="float16")[
+            "speed": np.asarray(unique_tracks_properties, dtype="float64")[
                 :, 3
             ],
-            "volume_pixels": np.asarray(
-                unique_tracks_properties, dtype="float16"
+            "directional_change_rate": np.asarray(
+                unique_tracks_properties, dtype="float64"
             )[:, 4],
-            "eccentricity_comp_first": np.asarray(
-                unique_tracks_properties, dtype="float16"
+            "total-intensity": np.asarray(
+                unique_tracks_properties, dtype="float64"
             )[:, 5],
-            "eccentricity_comp_second": np.asarray(
-                unique_tracks_properties, dtype="float16"
+            "volume_pixels": np.asarray(
+                unique_tracks_properties, dtype="float64"
             )[:, 6],
-            "surface_area": np.asarray(
-                unique_tracks_properties, dtype="float16"
+            "acceleration": np.asarray(
+                unique_tracks_properties, dtype="float64"
             )[:, 7],
             "cluster_class": np.asarray(
-                unique_tracks_properties, dtype="float16"
+                unique_tracks_properties, dtype="float64"
             )[:, 8],
             "cluster_score": np.asarray(
-                unique_tracks_properties, dtype="float16"
+                unique_tracks_properties, dtype="float64"
             )[:, 9],
-            "total_intensity": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 10],
-            "speed": np.asarray(unique_tracks_properties, dtype="float16")[
-                :, 11
-            ],
-            "motion_angle": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 12],
-            "acceleration": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 13],
-            "distance_cell_mask": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 14],
-            "radial_angle": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 15],
-            "cell_axis_mask": np.asarray(
-                unique_tracks_properties, dtype="float16"
-            )[:, 16],
         }
         print("Refreshing track data")
         for layer in list(plugin.viewer.value.layers):
             if (
                 "Track" == layer.name
                 or "Boxes" == layer.name
                 or "Track_points" == layer.name
             ):
                 plugin.viewer.value.layers.remove(layer)
-
+        vertices = unique_tracks[:, 1:]
+        plugin.viewer.value.add_points(vertices, name="Track_points", size=1)
+        print("Added vertices")
         plugin.viewer.value.add_tracks(
             unique_tracks,
             name="Track",
             features=features,
         )
         print("Track data refreshed")
         if str(track_id) not in TrackidBox and track_id is not None:
             _to_analyze = [int(track_id)]
         show_phenotype()
         select_track_nature()
 
     def show_phenotype():
 
-        nonlocal _to_analyze, size_catagories_json, _trackmate_objects
+        nonlocal _to_analyze, size_catagories_json
 
         phenotype_plot_class._reset_container(
             phenotype_plot_class.scroll_layout
         )
-
-        if _to_analyze is not None and _trackmate_objects is not None:
+        if _to_analyze is not None:
 
             unique_fft_properties = []
             unique_shape_properties = []
-            unique_dynamic_properties = []
             phenotype_plot_class._repeat_after_plot()
             plot_ax = phenotype_plot_class.plot_ax
             plot_ax.cla()
 
             for unique_track_id in _to_analyze:
 
                 for k in _trackmate_objects.unique_fft_properties[
@@ -973,53 +952,26 @@
                             cluster_volume,
                             cluster_eccentricity_comp_first,
                             cluster_eccentricity_comp_second,
                             cluster_surface_area,
                             cluster_class,
                             cluster_class_score,
                         ) = unique_shape_properties_tracklet
-
-                        unique_dynamic_properties_tracklet = (
-                            _trackmate_objects.unique_dynamic_properties[
-                                unique_track_id
-                            ][k]
-                        )
-                        (
-                            cluster_time,
-                            cluster_speed,
-                            cluster_motion_angle,
-                            cluster_acceleration,
-                            cluster_distance_cell_mask,
-                            cluster_radial_angle,
-                            cluster_cell_axis_mask,
-                        ) = unique_dynamic_properties_tracklet
-
                         cluster_class_name = []
                         if size_catagories_json is not None:
                             for i in range(cluster_class.shape[0]):
                                 if cluster_class[i] is not None:
                                     cluster_class_name.append(
                                         size_catagories_json[
                                             str(int(cluster_class[i]))
                                         ]
                                     )
                                 else:
                                     cluster_class_name.append(None)
 
-                        unique_dynamic_properties.append(
-                            [
-                                cluster_time,
-                                cluster_speed,
-                                cluster_motion_angle,
-                                cluster_acceleration,
-                                cluster_distance_cell_mask,
-                                cluster_radial_angle,
-                                cluster_cell_axis_mask,
-                            ]
-                        )
                         if size_catagories_json is None:
 
                             unique_shape_properties.append(
                                 [
                                     cluster_time,
                                     cluster_radius,
                                     cluster_volume,
@@ -1044,68 +996,15 @@
                                     cluster_class,
                                     cluster_class_score,
                                     cluster_class_name,
                                 ]
                             )
 
                         global_data_cluster_plot = []
-
-                        global_data_dynamic_cluster_plot = []
-
-                        for count, i in enumerate(
-                            range(len(unique_dynamic_properties))
-                        ):
-
-                            current_unique_dynamic_properties = (
-                                unique_dynamic_properties[i]
-                            )
-                            cluster_time = current_unique_dynamic_properties[0]
-                            cluster_speed = current_unique_dynamic_properties[
-                                1
-                            ]
-                            cluster_motion_angle = (
-                                current_unique_dynamic_properties[2]
-                            )
-                            cluster_acceleration = (
-                                current_unique_dynamic_properties[3]
-                            )
-                            cluster_distance_cell_mask = (
-                                current_unique_dynamic_properties[4]
-                            )
-                            cluster_radial_angle = (
-                                current_unique_dynamic_properties[5]
-                            )
-                            cluster_cell_axis_mask = (
-                                current_unique_dynamic_properties[6]
-                            )
-
-                            data_dynamic_cluster_plot = pd.DataFrame(
-                                {
-                                    "Time": cluster_time,
-                                    "Speed": cluster_speed,
-                                    "Motion Angle": cluster_motion_angle,
-                                    "Acceleration": cluster_acceleration,
-                                    "Distance cell to tissue": cluster_distance_cell_mask,
-                                    "Radial Angle": cluster_radial_angle,
-                                    "Cell Axis Mask": cluster_cell_axis_mask,
-                                }
-                            )
-
-                            if len(global_data_dynamic_cluster_plot) == 0:
-                                global_data_dynamic_cluster_plot = (
-                                    data_dynamic_cluster_plot
-                                )
-                            else:
-                                global_data_dynamic_cluster_plot = pd.concat(
-                                    [
-                                        global_data_dynamic_cluster_plot,
-                                        data_dynamic_cluster_plot,
-                                    ],
-                                    ignore_index=True,
-                                )
+                        index_array = []
 
                         for count, i in enumerate(
                             range(len(unique_shape_properties))
                         ):
 
                             current_unique_shape_properties = (
                                 unique_shape_properties[i]
@@ -1155,193 +1054,137 @@
                                         "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
                                         "Surface_Area": cluster_surface_area,
                                         "Class": cluster_class,
                                         "Class_Score": cluster_class_score,
                                     }
                                 )
 
+                            for _ in range(np.asarray(cluster_time).shape[0]):
+                                index_array.append(int(count))
+
+                            data_cluster_plot = data_cluster_plot.mask(
+                                data_cluster_plot.astype(object).eq("None")
+                            ).dropna()
+
                             if len(global_data_cluster_plot) == 0:
                                 global_data_cluster_plot = data_cluster_plot
                             else:
                                 global_data_cluster_plot = pd.concat(
                                     [
                                         global_data_cluster_plot,
                                         data_cluster_plot,
                                     ],
                                     ignore_index=True,
                                 )
 
             if len(_to_analyze) <= 2:
+                global_data_cluster_plot["index"] = index_array[
+                    0 : len(global_data_cluster_plot)
+                ]
 
-                sns.lineplot(
-                    global_data_dynamic_cluster_plot,
-                    x="Time",
-                    y="Speed",
-                    ax=plot_ax,
-                )
-
-                plot_ax.set_title("Speed")
-                plot_ax.set_xlabel("Time (min)")
-
-                phenotype_plot_class._repeat_after_plot()
-                plot_ax = phenotype_plot_class.plot_ax
-
-                sns.lineplot(
-                    global_data_dynamic_cluster_plot,
-                    x="Time",
-                    y="Motion Angle",
-                    ax=plot_ax,
-                )
-
-                plot_ax.set_title("Motion Angle")
-                plot_ax.set_xlabel("Time (min)")
-
-                phenotype_plot_class._repeat_after_plot()
-                plot_ax = phenotype_plot_class.plot_ax
-
-                sns.lineplot(
-                    global_data_dynamic_cluster_plot,
-                    x="Time",
-                    y="Radial Angle",
-                    ax=plot_ax,
-                )
-
-                plot_ax.set_title("Radial Angle")
-                plot_ax.set_xlabel("Time (min)")
-
-                phenotype_plot_class._repeat_after_plot()
-                plot_ax = phenotype_plot_class.plot_ax
-
-                sns.lineplot(
-                    global_data_dynamic_cluster_plot,
-                    x="Time",
-                    y="Acceleration",
-                    ax=plot_ax,
-                )
-
-                plot_ax.set_title("Acceleration")
-                plot_ax.set_xlabel("Time (min)")
-
-                phenotype_plot_class._repeat_after_plot()
-                plot_ax = phenotype_plot_class.plot_ax
-
-                sns.lineplot(
-                    global_data_dynamic_cluster_plot,
-                    x="Time",
-                    y="Distance cell to tissue",
-                    ax=plot_ax,
+                global_data_cluster_plot = global_data_cluster_plot.set_index(
+                    "index"
                 )
-
-                plot_ax.set_title("Distance cell to tissue")
-                plot_ax.set_xlabel("Time (min)")
-
-                phenotype_plot_class._repeat_after_plot()
-                plot_ax = phenotype_plot_class.plot_ax
-
-                sns.lineplot(
-                    global_data_dynamic_cluster_plot,
-                    x="Time",
-                    y="Cell Axis Mask",
-                    ax=plot_ax,
+                global_data_cluster_plot.drop_duplicates(
+                    global_data_cluster_plot
                 )
-
-                plot_ax.set_title("Cell Axis Mask")
+                if size_catagories_json is None:
+                    sns.lineplot(
+                        global_data_cluster_plot,
+                        x="Time",
+                        y="Class",
+                        hue=global_data_cluster_plot.index.values.tolist(),
+                        ax=plot_ax,
+                    )
+                    sns.move_legend(plot_ax, "lower right")
+                if size_catagories_json is not None:
+                    sns.lineplot(
+                        global_data_cluster_plot,
+                        x="Time",
+                        y="Class_Name",
+                        hue=global_data_cluster_plot.index.values.tolist(),
+                        ax=plot_ax,
+                    )
+                    sns.move_legend(plot_ax, "lower right")
+                plot_ax.set_title("Cluster class")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Radius",
+                    hue=global_data_cluster_plot.index.values.tolist(),
                     ax=plot_ax,
                 )
-
+                sns.move_legend(plot_ax, "lower right")
                 plot_ax.set_title("Radius")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Volume",
+                    hue=global_data_cluster_plot.index.values.tolist(),
                     ax=plot_ax,
                 )
-
+                sns.move_legend(plot_ax, "lower right")
                 plot_ax.set_title("Volume")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Surface_Area",
+                    hue=global_data_cluster_plot.index.values.tolist(),
                     ax=plot_ax,
                 )
-
+                sns.move_legend(plot_ax, "lower right")
                 plot_ax.set_title("Surface_Area")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_First",
+                    hue=global_data_cluster_plot.index.values.tolist(),
                     ax=plot_ax,
                 )
-
+                sns.move_legend(plot_ax, "lower right")
                 plot_ax.set_title("Eccentricity Comp First")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_Second",
+                    hue=global_data_cluster_plot.index.values.tolist(),
                     ax=plot_ax,
                 )
-
+                sns.move_legend(plot_ax, "lower right")
                 plot_ax.set_title("Eccentricity Comp Second")
                 plot_ax.set_xlabel("Time (min)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
-                if not global_data_cluster_plot["Class"].isna().all():
-                    if size_catagories_json is None:
-                        sns.lineplot(
-                            global_data_cluster_plot,
-                            x="Time",
-                            y="Class",
-                            ax=plot_ax,
-                        )
-
-                    if size_catagories_json is not None:
-                        sns.lineplot(
-                            global_data_cluster_plot,
-                            x="Time",
-                            y="Class_Name",
-                            ax=plot_ax,
-                        )
-
-                    plot_ax.set_title("Cluster class")
-                    plot_ax.set_xlabel("Time (min)")
-
-                    phenotype_plot_class._repeat_after_plot()
-                    plot_ax = phenotype_plot_class.plot_ax
-
             data_fft_plot = pd.DataFrame(
                 {
                     "Frequ": unique_fft_properties[0][2],
                     "Amplitude": np.sum(unique_fft_properties, axis=0)[3],
                 }
             )
 
@@ -1583,30 +1426,14 @@
                     plot_ax.set_ylabel("Class")
 
                     stat_plot_class._repeat_after_plot()
                     plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
-                    _trackmate_objects.mitotic_mean_distance_cell_mask,
-                    _trackmate_objects.mitotic_var_distance_cell_mask,
-                    linestyle="None",
-                    marker=".",
-                    mfc="green",
-                    ecolor="green",
-                )
-                plot_ax.set_title("Cell-tissue distance")
-                plot_ax.set_xlabel("Time (min)")
-                plot_ax.set_ylabel("um")
-
-                stat_plot_class._repeat_after_plot()
-                plot_ax = stat_plot_class.plot_ax
-
-                plot_ax.errorbar(
-                    _trackmate_objects.time,
                     _trackmate_objects.mitotic_mean_directional_change,
                     _trackmate_objects.mitotic_var_directional_change,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
@@ -1749,30 +1576,14 @@
                     plot_ax.set_ylabel("Class")
 
                     stat_plot_class._repeat_after_plot()
                     plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
-                    _trackmate_objects.non_mitotic_mean_distance_cell_mask,
-                    _trackmate_objects.non_mitotic_var_distance_cell_mask,
-                    linestyle="None",
-                    marker=".",
-                    mfc="green",
-                    ecolor="green",
-                )
-                plot_ax.set_title("Cell-tissue distance")
-                plot_ax.set_xlabel("Time (min)")
-                plot_ax.set_ylabel("um")
-
-                stat_plot_class._repeat_after_plot()
-                plot_ax = stat_plot_class.plot_ax
-
-                plot_ax.errorbar(
-                    _trackmate_objects.time,
                     _trackmate_objects.non_mitotic_mean_directional_change,
                     _trackmate_objects.non_mitotic_var_directional_change,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
@@ -1912,30 +1723,14 @@
                     plot_ax.set_ylabel("Class")
 
                     stat_plot_class._repeat_after_plot()
                     plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
-                    _trackmate_objects.all_mean_distance_cell_mask,
-                    _trackmate_objects.all_var_distance_cell_mask,
-                    linestyle="None",
-                    marker=".",
-                    mfc="green",
-                    ecolor="green",
-                )
-                plot_ax.set_title("Cell-tissue distance")
-                plot_ax.set_xlabel("Time (min)")
-                plot_ax.set_ylabel("um")
-
-                stat_plot_class._repeat_after_plot()
-                plot_ax = stat_plot_class.plot_ax
-
-                plot_ax.errorbar(
-                    _trackmate_objects.time,
                     _trackmate_objects.all_mean_directional_change,
                     _trackmate_objects.all_var_directional_change,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
@@ -2228,15 +2023,14 @@
         if (
             _trackmate_objects is not None
             and _track_ids_analyze is not None
             and value is not None
         ):
 
             track_id = value
-
             show_track(track_id)
 
     widget_for_cloud_auto_encoder_modeltype = {
         CloudAutoEncoder: plugin.cloud_auto_encoder_model,
         "No(Encoder)": plugin.cloud_auto_encoder_model_none,
         CUSTOM_MODEL_CLOUD_AUTO_ENCODER: plugin.model_folder_cloud_auto,
     }
@@ -2316,18 +2110,17 @@
             model_cluster = get_model_cluster(
                 *model_selected_cloud_auto_encoder,
                 *model_selected_cluster,
             )
 
             try:
                 device = torch.device("cuda:0")
-                model_cluster.to(device)
             except ValueError:
                 device = torch.device("cpu")
-                model_cluster.to(device)
+            model_cluster.to(device)
         else:
             model_cluster = None
 
         plugin.progress_bar.value = 0
         plugin.progress_bar.show()
         num_points = 0
         if model_selected_cloud_auto_encoder is not None:
```

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/_writer.py` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/napari.yaml` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.0.8
+Version: 2.1.0
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.0.8/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg-napari-trackmate-2.1.0/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.0.8/tox.ini` & `vollseg-napari-trackmate-2.1.0/tox.ini`

 * *Files identical despite different names*

