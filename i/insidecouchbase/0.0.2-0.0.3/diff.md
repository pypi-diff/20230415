# Comparing `tmp/insidecouchbase-0.0.2.tar.gz` & `tmp/insidecouchbase-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidecouchbase-0.0.2.tar", last modified: Sat Apr 15 11:03:15 2023, max compression
+gzip compressed data, was "insidecouchbase-0.0.3.tar", last modified: Sat Apr 15 11:09:09 2023, max compression
```

## Comparing `insidecouchbase-0.0.2.tar` & `insidecouchbase-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:03:15.918052 insidecouchbase-0.0.2/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-15 09:54:30.000000 insidecouchbase-0.0.2/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     5996 2023-04-15 11:03:15.918052 insidecouchbase-0.0.2/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     5486 2023-04-15 09:54:22.000000 insidecouchbase-0.0.2/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-15 10:44:14.000000 insidecouchbase-0.0.2/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-15 11:03:15.918052 insidecouchbase-0.0.2/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)      836 2023-04-15 11:03:11.000000 insidecouchbase-0.0.2/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:03:15.918052 insidecouchbase-0.0.2/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:03:15.918052 insidecouchbase-0.0.2/src/couchbase/
--rw-rw-r--   0 demir     (1000) demir     (1000)       16 2023-04-15 11:01:07.000000 insidecouchbase-0.0.2/src/couchbase/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    13500 2023-04-15 10:12:06.000000 insidecouchbase-0.0.2/src/couchbase/couchbase.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:03:15.918052 insidecouchbase-0.0.2/src/insidecouchbase.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     5996 2023-04-15 11:03:15.000000 insidecouchbase-0.0.2/src/insidecouchbase.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      276 2023-04-15 11:03:15.000000 insidecouchbase-0.0.2/src/insidecouchbase.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 11:03:15.000000 insidecouchbase-0.0.2/src/insidecouchbase.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-15 11:03:15.000000 insidecouchbase-0.0.2/src/insidecouchbase.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-15 09:54:30.000000 insidecouchbase-0.0.3/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5996 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5486 2023-04-15 09:54:22.000000 insidecouchbase-0.0.3/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-15 10:44:14.000000 insidecouchbase-0.0.3/pyproject.toml
+-rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)      836 2023-04-15 11:08:33.000000 insidecouchbase-0.0.3/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/src/couchbase/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       40 2023-04-15 11:08:25.000000 insidecouchbase-0.0.3/src/couchbase/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    13500 2023-04-15 10:12:06.000000 insidecouchbase-0.0.3/src/couchbase/couchbase.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:09:09.505312 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5996 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      276 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-15 11:09:09.000000 insidecouchbase-0.0.3/src/insidecouchbase.egg-info/top_level.txt
```

### Comparing `insidecouchbase-0.0.2/LICENSE` & `insidecouchbase-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.2/PKG-INFO` & `insidecouchbase-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidecouchbase
-Version: 0.0.2
+Version: 0.0.3
 Summary: Couchbase checker
 Home-page: https://github.com/adiosamig/insidecocuhbase
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `insidecouchbase-0.0.2/README.md` & `insidecouchbase-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.2/setup.cfg` & `insidecouchbase-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.2/setup.py` & `insidecouchbase-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidecouchbase",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
     description = "Couchbase checker",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidecocuhbase",
     project_urls = {
```

### Comparing `insidecouchbase-0.0.2/src/couchbase/couchbase.py` & `insidecouchbase-0.0.3/src/couchbase/couchbase.py`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.2/src/insidecouchbase.egg-info/PKG-INFO` & `insidecouchbase-0.0.3/src/insidecouchbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidecouchbase
-Version: 0.0.2
+Version: 0.0.3
 Summary: Couchbase checker
 Home-page: https://github.com/adiosamig/insidecocuhbase
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

