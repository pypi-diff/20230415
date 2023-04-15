# Comparing `tmp/insidecouchbase-0.0.3.tar.gz` & `tmp/insidecouchbase-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidecouchbase-0.0.3.tar", last modified: Sat Apr 15 11:09:09 2023, max compression
+gzip compressed data, was "insidecouchbase-0.0.4.tar", last modified: Sat Apr 15 11:26:34 2023, max compression
```

## Comparing `insidecouchbase-0.0.3.tar` & `insidecouchbase-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-15 09:54:30.000000 insidecouchbase-0.0.3/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     5996 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     5486 2023-04-15 09:54:22.000000 insidecouchbase-0.0.3/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-15 10:44:14.000000 insidecouchbase-0.0.3/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)      836 2023-04-15 11:08:33.000000 insidecouchbase-0.0.3/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/src/couchbase/
--rw-rw-r--   0 demir     (1000) demir     (1000)       40 2023-04-15 11:08:25.000000 insidecouchbase-0.0.3/src/couchbase/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    13500 2023-04-15 10:12:06.000000 insidecouchbase-0.0.3/src/couchbase/couchbase.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     5996 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      276 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-15 09:54:30.000000 insidecouchbase-0.0.4/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5198 2023-04-15 11:23:55.000000 insidecouchbase-0.0.4/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-15 10:44:14.000000 insidecouchbase-0.0.4/pyproject.toml
+-rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-04-15 11:26:13.000000 insidecouchbase-0.0.4/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/src/couchbase/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       40 2023-04-15 11:08:25.000000 insidecouchbase-0.0.4/src/couchbase/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    13516 2023-04-15 11:22:04.000000 insidecouchbase-0.0.4/src/couchbase/couchbase.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      318 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/top_level.txt
```

### Comparing `insidecouchbase-0.0.3/LICENSE` & `insidecouchbase-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.3/PKG-INFO` & `insidecouchbase-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: insidecouchbase
-Version: 0.0.3
-Summary: Couchbase checker
-Home-page: https://github.com/adiosamig/insidecocuhbase
-Author: Huseyin Demir
-Author-email: huseyin.d3r@gmail.com
-Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Couchbase Complete Snapshot 
 
 ![](https://upload.wikimedia.org/wikipedia/commons/6/67/Couchbase%2C_Inc._official_logo.png)
 
 Couchbase complete snapshot is responsible for collecting metrics from a single cluster and evaluating the results according to the **production best practices**
 
 
@@ -41,24 +26,34 @@
 
 ### XDCR Health Check List
 
 - XDCR cluster versions should be the with the production cluster.
 
 ## Installation and Running
 
-1. Clone the repository
+1. Install the module
 
 ```bash
-https://github.com/adiosamig/couchbase-complete-snapshot.git
+pip3 install insidecouchbase
 ```
 
 2. Run the following command in repo's directory.
 
 ```python
-python3 couchbase-snapshot.py 127.0.0.1 user_name password
+import couchbase
+
+demo=couchbase.couchbasePlatform('127.0.0.1','Administrator','test123')
+demo.getClusterVersion()
+demo.getUsersOnCluster()
+demo.getXdcrConnections()
+demo.getNodesOnCluster()
+demo.prepareBucketData()
+demo.getSettings()
+demo.getRebalance()
+demo.takePicture()
 ```
 Example results
 
 ```
 ----- Cluster Nodes -----
 +----+-----------------+-----------------+---------------+-----------------+-----------------------+
 |    | nodeIP          | clusterMember   | healtStatus   | services        | couchbaseVersion      |
@@ -97,23 +92,15 @@
 |    | problemStatement                                                                                                   | problemArea       | problemSeverity   |
 |----+--------------------------------------------------------------------------------------------------------------------+-------------------+-------------------|
 |  0 | XDCR and Production cluster versions are different                                                                 | 172.17.0.7 - XDCR | Critical          |
 |  1 | The node has multiple couchbase services.For production MDS model should be followed.                              | 172.17.0.5:8091   | Medium            |
 |  2 | Email alerts are disabled                                                                                          | Cluster           | Critical          |
 |  3 | Default node exporter port can not be reached.If node exporter port is different from default ignore this problem. | Monitoring        | Medium            |
 +----+--------------------------------------------------------------------------------------------------------------------+-------------------+-------------------+
------ Ping Test Results -----
-+----+-----------------+-------------+---------------+
-|    | nodeIp          | pingState   |   latency(us) |
-|----+-----------------+-------------+---------------|
-|  0 | 172.17.0.2:8091 | ok          |           615 |
-|  1 | 172.17.0.3:8091 | ok          |           577 |
-|  2 | 172.17.0.4:8091 | ok          |           550 |
-|  3 | 172.17.0.5:8091 | ok          |           648 |
-+----+-----------------+-------------+---------------+
+
 ```
 
 
 ## Supported Couchbase Version
 
 - Couchbase 7.0.X
 - Couchbase 7.1.X
```

### Comparing `insidecouchbase-0.0.3/setup.cfg` & `insidecouchbase-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.3/setup.py` & `insidecouchbase-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidecouchbase",
-    version = "0.0.3",
+    version = "0.0.4",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
-    description = "Couchbase checker",
+    description = "Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidecocuhbase",
+    install_requires=[
+        'requests',
+        'tabulate',
+        'pandas',
+        'requests'
+    ],
     project_urls = {
         "Bug Tracker": "https://github.com/adiosamig/insidecocuhbase/issues",
     },
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `insidecouchbase-0.0.3/src/couchbase/couchbase.py` & `insidecouchbase-0.0.4/src/couchbase/couchbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,8 +276,8 @@
                     "problemArea": 'Bucket',
                     "problemSeverity": 'Critical'
                 }
                 checkResults.append(checkModel)
         dataFrameResults=pd.DataFrame(checkResults)
         print("----- Check Notes -----")
         print(tabulate(dataFrameResults, headers = 'keys', tablefmt = 'psql'))
-        return clusterNodes
+        return f''' Finished healtcheck.'''
```

### Comparing `insidecouchbase-0.0.3/src/insidecouchbase.egg-info/PKG-INFO` & `insidecouchbase-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: insidecouchbase
-Version: 0.0.3
-Summary: Couchbase checker
+Version: 0.0.4
+Summary: Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication
 Home-page: https://github.com/adiosamig/insidecocuhbase
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,24 +41,34 @@
 
 ### XDCR Health Check List
 
 - XDCR cluster versions should be the with the production cluster.
 
 ## Installation and Running
 
-1. Clone the repository
+1. Install the module
 
 ```bash
-https://github.com/adiosamig/couchbase-complete-snapshot.git
+pip3 install insidecouchbase
 ```
 
 2. Run the following command in repo's directory.
 
 ```python
-python3 couchbase-snapshot.py 127.0.0.1 user_name password
+import couchbase
+
+demo=couchbase.couchbasePlatform('127.0.0.1','Administrator','test123')
+demo.getClusterVersion()
+demo.getUsersOnCluster()
+demo.getXdcrConnections()
+demo.getNodesOnCluster()
+demo.prepareBucketData()
+demo.getSettings()
+demo.getRebalance()
+demo.takePicture()
 ```
 Example results
 
 ```
 ----- Cluster Nodes -----
 +----+-----------------+-----------------+---------------+-----------------+-----------------------+
 |    | nodeIP          | clusterMember   | healtStatus   | services        | couchbaseVersion      |
@@ -97,23 +107,15 @@
 |    | problemStatement                                                                                                   | problemArea       | problemSeverity   |
 |----+--------------------------------------------------------------------------------------------------------------------+-------------------+-------------------|
 |  0 | XDCR and Production cluster versions are different                                                                 | 172.17.0.7 - XDCR | Critical          |
 |  1 | The node has multiple couchbase services.For production MDS model should be followed.                              | 172.17.0.5:8091   | Medium            |
 |  2 | Email alerts are disabled                                                                                          | Cluster           | Critical          |
 |  3 | Default node exporter port can not be reached.If node exporter port is different from default ignore this problem. | Monitoring        | Medium            |
 +----+--------------------------------------------------------------------------------------------------------------------+-------------------+-------------------+
------ Ping Test Results -----
-+----+-----------------+-------------+---------------+
-|    | nodeIp          | pingState   |   latency(us) |
-|----+-----------------+-------------+---------------|
-|  0 | 172.17.0.2:8091 | ok          |           615 |
-|  1 | 172.17.0.3:8091 | ok          |           577 |
-|  2 | 172.17.0.4:8091 | ok          |           550 |
-|  3 | 172.17.0.5:8091 | ok          |           648 |
-+----+-----------------+-------------+---------------+
+
 ```
 
 
 ## Supported Couchbase Version
 
 - Couchbase 7.0.X
 - Couchbase 7.1.X
```

