# Comparing `tmp/pyVHDLModel-0.8.1.tar.gz` & `tmp/pyVHDLModel-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVHDLModel-0.8.1.tar", last modified: Wed Jun  9 16:29:25 2021, max compression
+gzip compressed data, was "pyVHDLModel-0.9.0.tar", last modified: Sun Jun 13 21:37:56 2021, max compression
```

## Comparing `pyVHDLModel-0.8.1.tar` & `pyVHDLModel-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 16:29:25.693196 pyVHDLModel-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2021-06-09 16:29:18.000000 pyVHDLModel-0.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     6303 2021-06-09 16:29:25.693196 pyVHDLModel-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4589 2021-06-09 16:29:18.000000 pyVHDLModel-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 16:29:25.693196 pyVHDLModel-0.8.1/pyVHDLModel/
--rw-r--r--   0 runner    (1001) docker     (121)    30828 2021-06-09 16:29:18.000000 pyVHDLModel-0.8.1/pyVHDLModel/VHDLModel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-06-09 16:29:18.000000 pyVHDLModel-0.8.1/pyVHDLModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 16:29:25.693196 pyVHDLModel-0.8.1/pyVHDLModel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6303 2021-06-09 16:29:25.000000 pyVHDLModel-0.8.1/pyVHDLModel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-06-09 16:29:25.000000 pyVHDLModel-0.8.1/pyVHDLModel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-09 16:29:25.000000 pyVHDLModel-0.8.1/pyVHDLModel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-06-09 16:29:25.000000 pyVHDLModel-0.8.1/pyVHDLModel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-09 16:29:25.000000 pyVHDLModel-0.8.1/pyVHDLModel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-09 16:29:25.693196 pyVHDLModel-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3710 2021-06-09 16:29:18.000000 pyVHDLModel-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 21:37:56.605517 pyVHDLModel-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    10571 2021-06-13 21:37:54.000000 pyVHDLModel-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6303 2021-06-13 21:37:56.601517 pyVHDLModel-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4589 2021-06-13 21:37:54.000000 pyVHDLModel-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 21:37:56.601517 pyVHDLModel-0.9.0/pyVHDLModel/
+-rw-r--r--   0 runner    (1001) docker     (121)    40953 2021-06-13 21:37:54.000000 pyVHDLModel-0.9.0/pyVHDLModel/VHDLModel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-06-13 21:37:54.000000 pyVHDLModel-0.9.0/pyVHDLModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 21:37:56.601517 pyVHDLModel-0.9.0/pyVHDLModel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6303 2021-06-13 21:37:56.000000 pyVHDLModel-0.9.0/pyVHDLModel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-06-13 21:37:56.000000 pyVHDLModel-0.9.0/pyVHDLModel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-13 21:37:56.000000 pyVHDLModel-0.9.0/pyVHDLModel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-06-13 21:37:56.000000 pyVHDLModel-0.9.0/pyVHDLModel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-13 21:37:56.000000 pyVHDLModel-0.9.0/pyVHDLModel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-13 21:37:56.605517 pyVHDLModel-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3710 2021-06-13 21:37:54.000000 pyVHDLModel-0.9.0/setup.py
```

### Comparing `pyVHDLModel-0.8.1/LICENSE.md` & `pyVHDLModel-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyVHDLModel-0.8.1/PKG-INFO` & `pyVHDLModel-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVHDLModel
-Version: 0.8.1
+Version: 0.9.0
 Summary: An abstract VHDL language model.
 Home-page: https://github.com/vhdl/pyVHDLModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://vhdl.github.io/pyVHDLModel
 Project-URL: Source Code, https://github.com/vhdl/pyVHDLModel
```

### Comparing `pyVHDLModel-0.8.1/README.md` & `pyVHDLModel-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyVHDLModel-0.8.1/pyVHDLModel/__init__.py` & `pyVHDLModel-0.9.0/pyVHDLModel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVHDLModel-0.8.1/pyVHDLModel.egg-info/PKG-INFO` & `pyVHDLModel-0.9.0/pyVHDLModel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVHDLModel
-Version: 0.8.1
+Version: 0.9.0
 Summary: An abstract VHDL language model.
 Home-page: https://github.com/vhdl/pyVHDLModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://vhdl.github.io/pyVHDLModel
 Project-URL: Source Code, https://github.com/vhdl/pyVHDLModel
```

### Comparing `pyVHDLModel-0.8.1/setup.py` & `pyVHDLModel-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 # Derive URLs
 sourceCodeURL =     "https://github.com/{namespace}/{projectName}".format(namespace=gitHubNamespace, projectName=projectName)
 documentationURL =  "https://{namespace}.github.io/{projectName}".format(namespace=gitHubNamespace, projectName=projectName)
 
 # Assemble all package information
 setuptools_setup(
 	name=projectName,
-	version="0.8.1",
+	version="0.9.0",
 
 	author="Patrick Lehmann",
 	author_email="Paebbels@gmail.com",
 	# maintainer="Patrick Lehmann",
 	# maintainer_email="Paebbels@gmail.com",
   license='Apache 2.0',
```

