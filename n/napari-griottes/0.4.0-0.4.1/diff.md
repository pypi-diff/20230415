# Comparing `tmp/napari_griottes-0.4.0.tar.gz` & `tmp/napari_griottes-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_griottes-0.4.0.tar", last modified: Fri Apr 14 22:05:29 2023, max compression
+gzip compressed data, was "napari_griottes-0.4.1.tar", last modified: Fri Apr 14 22:12:13 2023, max compression
```

## Comparing `napari_griottes-0.4.0.tar` & `napari_griottes-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.089607 napari_griottes-0.4.0/src/napari_griottes/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/src/napari_griottes/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/src/napari_griottes/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:05:29.093607 napari_griottes-0.4.0/src/napari_griottes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 22:05:29.000000 napari_griottes-0.4.0/src/napari_griottes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 22:05:10.000000 napari_griottes-0.4.0/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.056907 napari_griottes-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.056907 napari_griottes-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/src/napari_griottes/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/src/napari_griottes/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 22:12:13.000000 napari_griottes-0.4.1/src/napari_griottes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/src/napari_griottes/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:12:13.060907 napari_griottes-0.4.1/src/napari_griottes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-14 22:12:13.000000 napari_griottes-0.4.1/src/napari_griottes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-14 22:12:13.000000 napari_griottes-0.4.1/src/napari_griottes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:12:13.000000 napari_griottes-0.4.1/src/napari_griottes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 22:12:13.000000 napari_griottes-0.4.1/src/napari_griottes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 22:12:13.000000 napari_griottes-0.4.1/src/napari_griottes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 22:12:13.000000 napari_griottes-0.4.1/src/napari_griottes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 22:11:48.000000 napari_griottes-0.4.1/vectors.py
```

### Comparing `napari_griottes-0.4.0/.github/workflows/test_and_deploy.yml` & `napari_griottes-0.4.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/.gitignore` & `napari_griottes-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/.napari/DESCRIPTION.md` & `napari_griottes-0.4.1/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/.pre-commit-config.yaml` & `napari_griottes-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/LICENSE` & `napari_griottes-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/PKG-INFO` & `napari_griottes-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_griottes
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create graphs
 Home-page: https://github.com/aaristov/napari-griottes
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/aaristov/napari-griottes/issues
 Project-URL: Documentation, https://github.com/aaristov/napari-griottes#README.md
@@ -103,29 +103,27 @@
 
 
 https://user-images.githubusercontent.com/11408456/168237170-b43afd5a-26a4-4cdc-bc42-d3f46f138536.mp4
 
 
 ### Saving and recovering the graph
 
-Any graph you see in napari can be saved in .griottes format which is networkx.gpickle inside.
+Any graph you see in napari can be saved in .json format.
 1. Select he layers with connections
 2. Click File/Save Selected Layer
 3. Choose Griottes in drop-down menu
 4. Save
 
 In order to recover a previously saved graph in napari, you can simply drag-n-drop your file into napari, or use file open fialog.
 
 
 
 https://user-images.githubusercontent.com/11408456/167845853-e7071199-3f58-4d11-8d7b-c1358a150e6b.mp4
 
 
-Otherwise, you can open the graph with [neworkx.read_gpickle](https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gpickle.read_gpickle.html) function
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari_griottes-0.4.0/README.md` & `napari_griottes-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -75,29 +75,27 @@
 
 
 https://user-images.githubusercontent.com/11408456/168237170-b43afd5a-26a4-4cdc-bc42-d3f46f138536.mp4
 
 
 ### Saving and recovering the graph
 
-Any graph you see in napari can be saved in .griottes format which is networkx.gpickle inside.
+Any graph you see in napari can be saved in .json format.
 1. Select he layers with connections
 2. Click File/Save Selected Layer
 3. Choose Griottes in drop-down menu
 4. Save
 
 In order to recover a previously saved graph in napari, you can simply drag-n-drop your file into napari, or use file open fialog.
 
 
 
 https://user-images.githubusercontent.com/11408456/167845853-e7071199-3f58-4d11-8d7b-c1358a150e6b.mp4
 
 
-Otherwise, you can open the graph with [neworkx.read_gpickle](https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gpickle.read_gpickle.html) function
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari_griottes-0.4.0/setup.cfg` & `napari_griottes-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes/_reader.py` & `napari_griottes-0.4.1/src/napari_griottes/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes/_sample_data.py` & `napari_griottes-0.4.1/src/napari_griottes/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes/_tests/test_reader.py` & `napari_griottes-0.4.1/src/napari_griottes/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes/_tests/test_widget.py` & `napari_griottes-0.4.1/src/napari_griottes/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes/_widget.py` & `napari_griottes-0.4.1/src/napari_griottes/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes/_writer.py` & `napari_griottes-0.4.1/src/napari_griottes/_writer.py`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes/napari.yaml` & `napari_griottes-0.4.1/src/napari_griottes/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/src/napari_griottes.egg-info/PKG-INFO` & `napari_griottes-0.4.1/src/napari_griottes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-griottes
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create graphs
 Home-page: https://github.com/aaristov/napari-griottes
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/aaristov/napari-griottes/issues
 Project-URL: Documentation, https://github.com/aaristov/napari-griottes#README.md
@@ -103,29 +103,27 @@
 
 
 https://user-images.githubusercontent.com/11408456/168237170-b43afd5a-26a4-4cdc-bc42-d3f46f138536.mp4
 
 
 ### Saving and recovering the graph
 
-Any graph you see in napari can be saved in .griottes format which is networkx.gpickle inside.
+Any graph you see in napari can be saved in .json format.
 1. Select he layers with connections
 2. Click File/Save Selected Layer
 3. Choose Griottes in drop-down menu
 4. Save
 
 In order to recover a previously saved graph in napari, you can simply drag-n-drop your file into napari, or use file open fialog.
 
 
 
 https://user-images.githubusercontent.com/11408456/167845853-e7071199-3f58-4d11-8d7b-c1358a150e6b.mp4
 
 
-Otherwise, you can open the graph with [neworkx.read_gpickle](https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gpickle.read_gpickle.html) function
-
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari_griottes-0.4.0/src/napari_griottes.egg-info/SOURCES.txt` & `napari_griottes-0.4.1/src/napari_griottes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/tox.ini` & `napari_griottes-0.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `napari_griottes-0.4.0/vectors.py` & `napari_griottes-0.4.1/vectors.py`

 * *Files identical despite different names*

