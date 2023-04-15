# Comparing `tmp/insidecouchbase-0.0.4.tar.gz` & `tmp/insidecouchbase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidecouchbase-0.0.4.tar", last modified: Sat Apr 15 11:26:34 2023, max compression
+gzip compressed data, was "insidecouchbase-0.0.5.tar", last modified: Sat Apr 15 11:33:13 2023, max compression
```

## Comparing `insidecouchbase-0.0.4.tar` & `insidecouchbase-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-15 09:54:30.000000 insidecouchbase-0.0.4/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     5198 2023-04-15 11:23:55.000000 insidecouchbase-0.0.4/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-15 10:44:14.000000 insidecouchbase-0.0.4/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-04-15 11:26:13.000000 insidecouchbase-0.0.4/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/src/couchbase/
--rw-rw-r--   0 demir     (1000) demir     (1000)       40 2023-04-15 11:08:25.000000 insidecouchbase-0.0.4/src/couchbase/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    13516 2023-04-15 11:22:04.000000 insidecouchbase-0.0.4/src/couchbase/couchbase.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:26:34.259082 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      318 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-15 11:26:34.000000 insidecouchbase-0.0.4/src/insidecouchbase.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-15 09:54:30.000000 insidecouchbase-0.0.5/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5198 2023-04-15 11:23:55.000000 insidecouchbase-0.0.5/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-15 10:44:14.000000 insidecouchbase-0.0.5/pyproject.toml
+-rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-04-15 11:32:47.000000 insidecouchbase-0.0.5/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/src/couchbase/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       40 2023-04-15 11:08:25.000000 insidecouchbase-0.0.5/src/couchbase/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    13465 2023-04-15 11:32:22.000000 insidecouchbase-0.0.5/src/couchbase/couchbase.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      318 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/top_level.txt
```

### Comparing `insidecouchbase-0.0.4/LICENSE` & `insidecouchbase-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.4/PKG-INFO` & `insidecouchbase-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidecouchbase
-Version: 0.0.4
+Version: 0.0.5
 Summary: Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication
 Home-page: https://github.com/adiosamig/insidecocuhbase
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `insidecouchbase-0.0.4/README.md` & `insidecouchbase-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.4/setup.cfg` & `insidecouchbase-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.4/setup.py` & `insidecouchbase-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidecouchbase",
-    version = "0.0.4",
+    version = "0.0.5",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
     description = "Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidecocuhbase",
     install_requires=[
```

### Comparing `insidecouchbase-0.0.4/src/couchbase/couchbase.py` & `insidecouchbase-0.0.5/src/couchbase/couchbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,15 @@
             urlForHealth = f"http://{self.hostname}:8091/settings/rbac/users"
             getNodeDetails = requests.get(
                 url=urlForHealth, auth=(self.logininformation, self.loginsecret))
             resultParsed = getNodeDetails.json()
             userList=[]
             for user in resultParsed:
                 userModel={
-                    "userName": user.get('name'),
-                    "userRole": user.get('roles')
+                    "userName": user.get('name')
                 }
                 userList.append(userModel)
             self.usersOnCluster=userList
         except Exception as couchbaseBucketException:
             print(couchbaseBucketException)
     def getClusterName(self):
         try:
```

### Comparing `insidecouchbase-0.0.4/src/insidecouchbase.egg-info/PKG-INFO` & `insidecouchbase-0.0.5/src/insidecouchbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidecouchbase
-Version: 0.0.4
+Version: 0.0.5
 Summary: Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication
 Home-page: https://github.com/adiosamig/insidecocuhbase
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

