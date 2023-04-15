# Comparing `tmp/mrgrain.cdk-esbuild-4.1.5.tar.gz` & `tmp/mrgrain.cdk-esbuild-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrgrain.cdk-esbuild-4.1.5.tar", last modified: Sat Apr  1 05:07:50 2023, max compression
+gzip compressed data, was "mrgrain.cdk-esbuild-4.1.6.tar", last modified: Sat Apr 15 05:06:13 2023, max compression
```

## Comparing `mrgrain.cdk-esbuild-4.1.5.tar` & `mrgrain.cdk-esbuild-4.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:07:50.656652 mrgrain.cdk-esbuild-4.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-04-01 05:07:50.656652 mrgrain.cdk-esbuild-4.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 05:07:50.656652 mrgrain.cdk-esbuild-4.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:07:50.652652 mrgrain.cdk-esbuild-4.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:07:50.652652 mrgrain.cdk-esbuild-4.1.5/src/mrgrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:07:50.656652 mrgrain.cdk-esbuild-4.1.5/src/mrgrain/cdk_esbuild/
--rw-r--r--   0 runner    (1001) docker     (123)   393083 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain/cdk_esbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:07:50.656652 mrgrain.cdk-esbuild-4.1.5/src/mrgrain/cdk_esbuild/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain/cdk_esbuild/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81277 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.1.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 05:07:35.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain/cdk_esbuild/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 05:07:50.656652 mrgrain.cdk-esbuild-4.1.5/src/mrgrain.cdk_esbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-04-01 05:07:50.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-01 05:07:50.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 05:07:50.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-01 05:07:50.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain.cdk_esbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-01 05:07:50.000000 mrgrain.cdk-esbuild-4.1.5/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.522446 mrgrain.cdk-esbuild-4.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.522446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)   393083 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81277 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.1.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
```

### Comparing `mrgrain.cdk-esbuild-4.1.5/LICENSE` & `mrgrain.cdk-esbuild-4.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.1.5/PKG-INFO` & `mrgrain.cdk-esbuild-4.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.1.5
+Version: 4.1.6
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `mrgrain.cdk-esbuild-4.1.5/README.md` & `mrgrain.cdk-esbuild-4.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.1.5/setup.py` & `mrgrain.cdk-esbuild-4.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mrgrain.cdk-esbuild",
-    "version": "4.1.5",
+    "version": "4.1.6",
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "license": "MIT",
     "url": "https://github.com/mrgrain/cdk-esbuild",
     "long_description_content_type": "text/markdown",
     "author": "Moritz Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "mrgrain.cdk_esbuild",
         "mrgrain.cdk_esbuild._jsii"
     ],
     "package_data": {
         "mrgrain.cdk_esbuild._jsii": [
-            "cdk-esbuild@4.1.5.jsii.tgz"
+            "cdk-esbuild@4.1.6.jsii.tgz"
         ],
         "mrgrain.cdk_esbuild": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.12.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `mrgrain.cdk-esbuild-4.1.5/src/mrgrain/cdk_esbuild/__init__.py` & `mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.1.5/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO` & `mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.1.5
+Version: 4.1.6
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

