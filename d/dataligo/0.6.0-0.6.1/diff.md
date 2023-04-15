# Comparing `tmp/dataligo-0.6.0.tar.gz` & `tmp/dataligo-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alchemist/Desktop/OpenSource/dataligo/dist/.tmp-i1sanzu2/dataligo-0.6.0.tar", last modified: Sat Apr 15 19:23:50 2023, max compression
+gzip compressed data, was "/home/alchemist/Desktop/OpenSource/dataligo/dist/.tmp-u1pfyily/dataligo-0.6.1.tar", last modified: Sat Apr 15 19:35:56 2023, max compression
```

## Comparing `dataligo-0.6.0.tar` & `dataligo-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:23:50.000000 dataligo-0.6.0/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-04-15 19:19:37.000000 dataligo-0.6.0/LICENSE
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    18870 2023-04-15 19:23:50.000000 dataligo-0.6.0/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5330 2023-04-15 19:19:37.000000 dataligo-0.6.0/README.md
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:23:50.000000 dataligo-0.6.0/dataligo.egg-info/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    18870 2023-04-15 19:23:50.000000 dataligo-0.6.0/dataligo.egg-info/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      191 2023-04-15 19:23:50.000000 dataligo-0.6.0/dataligo.egg-info/SOURCES.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-15 19:23:50.000000 dataligo-0.6.0/dataligo.egg-info/dependency_links.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      334 2023-04-15 19:23:50.000000 dataligo-0.6.0/dataligo.egg-info/requires.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-04-15 19:23:50.000000 dataligo-0.6.0/dataligo.egg-info/top_level.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1675 2023-04-15 19:20:48.000000 dataligo-0.6.0/pyproject.toml
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-15 19:23:50.000000 dataligo-0.6.0/setup.cfg
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:35:56.000000 dataligo-0.6.1/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-04-15 19:19:37.000000 dataligo-0.6.1/LICENSE
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    18882 2023-04-15 19:35:56.000000 dataligo-0.6.1/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5330 2023-04-15 19:19:37.000000 dataligo-0.6.1/README.md
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    18882 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      191 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/SOURCES.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/dependency_links.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      334 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/requires.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-04-15 19:35:56.000000 dataligo-0.6.1/dataligo.egg-info/top_level.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1687 2023-04-15 19:34:51.000000 dataligo-0.6.1/pyproject.toml
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-15 19:35:56.000000 dataligo-0.6.1/setup.cfg
```

### Comparing `dataligo-0.6.0/LICENSE` & `dataligo-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataligo-0.6.0/PKG-INFO` & `dataligo-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,15 +203,15 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/VinishUchiha/dataligo
 Keywords: connectors,datalake reader,datawarehouse reader,dataconnector,nosql connector
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `dataligo-0.6.0/README.md` & `dataligo-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dataligo-0.6.0/dataligo.egg-info/PKG-INFO` & `dataligo-0.6.1/dataligo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,15 +203,15 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/VinishUchiha/dataligo
 Keywords: connectors,datalake reader,datawarehouse reader,dataconnector,nosql connector
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `dataligo-0.6.0/pyproject.toml` & `dataligo-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataligo"
-version = "0.6.0"
+version = "0.6.1"
 description = "A library to accelerate ML and ETL pipeline by connecting all data sources"
 readme = "README.md"
 authors = [{ name = "Vinish M", email = "vinishuchiha@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["connectors", "datalake reader","datawarehouse reader", "dataconnector", "nosql connector"]
 dependencies = [
     "boto3 >= 1.26.93",
     "google-cloud-storage >= 2.7.0",
@@ -42,15 +42,15 @@
 [project.urls]
 Homepage = "https://github.com/VinishUchiha/dataligo"
 
 [tool.setuptools]
 py-modules = ["dataligo"]
 
 [tool.bumpver]
-current_version = "0.6.0"
+current_version = "0.6.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

