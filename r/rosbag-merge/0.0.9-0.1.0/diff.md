# Comparing `tmp/rosbag_merge-0.0.9.tar.gz` & `tmp/rosbag_merge-0.1.0.tar.gz`

## Comparing `rosbag_merge-0.0.9.tar` & `rosbag_merge-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/INSTALL.md
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/requirements.txt
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/.github/workflows/publish-to-pypi-and-test-pypi.yml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/examples/main_direct.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/__init__.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/bag_stream.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/csv_merge.py
--rwxr-xr-x   0        0        0     6382 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/main.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/merge_bags.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/rosbag_to_csv.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/topic_list.txt
--rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
--rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
--rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/.gitignore
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/LICENSE
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    16023 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/INSTALL.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/.github/workflows/publish-to-pypi-and-test-pypi.yml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/examples/main_direct.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/__init__.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/bag_stream.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/csv_merge.py
+-rwxr-xr-x   0        0        0     6382 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/main.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/merge_bags.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/rosbag_to_csv.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/topic_list.txt
+-rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
+-rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
+-rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/.gitignore
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/README.md
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16050 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/PKG-INFO
```

### Comparing `rosbag_merge-0.0.9/.github/workflows/publish-to-pypi-and-test-pypi.yml` & `rosbag_merge-0.1.0/.github/workflows/publish-to-pypi-and-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/examples/main_direct.py` & `rosbag_merge-0.1.0/examples/main_direct.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/src/rosbag_merge/bag_stream.py` & `rosbag_merge-0.1.0/src/rosbag_merge/bag_stream.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/src/rosbag_merge/csv_merge.py` & `rosbag_merge-0.1.0/src/rosbag_merge/csv_merge.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/src/rosbag_merge/main.py` & `rosbag_merge-0.1.0/src/rosbag_merge/main.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/src/rosbag_merge/merge_bags.py` & `rosbag_merge-0.1.0/src/rosbag_merge/merge_bags.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/src/rosbag_merge/rosbag_to_csv.py` & `rosbag_merge-0.1.0/src/rosbag_merge/rosbag_to_csv.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag` & `rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag` & `rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag` & `rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/LICENSE` & `rosbag_merge-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/README.md` & `rosbag_merge-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.9/pyproject.toml` & `rosbag_merge-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project]
 # add the distribution name of the package, the tar ball and python wheel use this name, this name goes the /home/$USER/.local/lib/python3.8/site-packages/
 name = "rosbag_merge"
 
 # version is the package version. See the version specifier specification
 # for more details on versions. Some build backends allow it to be 
 # specified another way, such as from a file or a git tag.
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Jonathan Sanabria", email="jonsanria@gmail.com" },
 ]
 description = "A gathering of tools for merging rosbags and saving their topic information to csv."
 readme = "README.md"
 license = { file="LICENSE" }
 
@@ -40,14 +40,15 @@
 dependencies = [
     "rosbag",
     "rospy",
     "dask",
     "pandas",
     "icecream",
     "tqdm",
+    "numpy==1.21" # wait for dask to solve solve AttributeError: module 'numpy' has no attribute 'typeDict'
 ]
 
 # this installs an executable in /home/$USER/.local/bin/rosbag-tools
 [project.scripts]
 rosbag-merge = "rosbag_merge.main:main"
 
 [project.urls]
```

### Comparing `rosbag_merge-0.0.9/PKG-INFO` & `rosbag_merge-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbag_merge
-Version: 0.0.9
+Version: 0.1.0
 Summary: A gathering of tools for merging rosbags and saving their topic information to csv.
 Project-URL: Homepage, https://github.com/1hada/rosbag-merge/
 Project-URL: Bug Tracker, https://github.com/1hada/rosbag-merge/issues/
 Author-email: Jonathan Sanabria <jonsanria@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -200,14 +200,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: dask
 Requires-Dist: icecream
+Requires-Dist: numpy==1.21
 Requires-Dist: pandas
 Requires-Dist: rosbag
 Requires-Dist: rospy
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
```

