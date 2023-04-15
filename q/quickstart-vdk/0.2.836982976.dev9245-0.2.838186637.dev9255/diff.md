# Comparing `tmp/quickstart-vdk-0.2.836982976.dev9245.tar.gz` & `tmp/quickstart-vdk-0.2.838186637.dev9255.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.836982976.dev9245.tar", last modified: Fri Apr 14 04:25:13 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.838186637.dev9255.tar", last modified: Sat Apr 15 04:26:34 2023, max compression
```

## Comparing `quickstart-vdk-0.2.836982976.dev9245.tar` & `quickstart-vdk-0.2.838186637.dev9255.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 04:25:13.454599 quickstart-vdk-0.2.836982976.dev9245/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-14 04:25:13.454599 quickstart-vdk-0.2.836982976.dev9245/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-14 04:22:36.000000 quickstart-vdk-0.2.836982976.dev9245/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 04:25:13.454599 quickstart-vdk-0.2.836982976.dev9245/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-14 04:25:13.000000 quickstart-vdk-0.2.836982976.dev9245/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-14 04:25:13.000000 quickstart-vdk-0.2.836982976.dev9245/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 04:25:13.000000 quickstart-vdk-0.2.836982976.dev9245/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-14 04:25:13.000000 quickstart-vdk-0.2.836982976.dev9245/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-14 04:25:13.000000 quickstart-vdk-0.2.836982976.dev9245/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 04:25:13.454599 quickstart-vdk-0.2.836982976.dev9245/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-14 04:25:05.000000 quickstart-vdk-0.2.836982976.dev9245/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 04:25:13.454599 quickstart-vdk-0.2.836982976.dev9245/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 04:22:36.000000 quickstart-vdk-0.2.836982976.dev9245/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 04:26:34.703131 quickstart-vdk-0.2.838186637.dev9255/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-15 04:26:34.703131 quickstart-vdk-0.2.838186637.dev9255/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-15 04:23:57.000000 quickstart-vdk-0.2.838186637.dev9255/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 04:26:34.699131 quickstart-vdk-0.2.838186637.dev9255/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-15 04:26:34.000000 quickstart-vdk-0.2.838186637.dev9255/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-15 04:26:34.000000 quickstart-vdk-0.2.838186637.dev9255/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 04:26:34.000000 quickstart-vdk-0.2.838186637.dev9255/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-15 04:26:34.000000 quickstart-vdk-0.2.838186637.dev9255/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-15 04:26:34.000000 quickstart-vdk-0.2.838186637.dev9255/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 04:26:34.703131 quickstart-vdk-0.2.838186637.dev9255/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-15 04:26:26.000000 quickstart-vdk-0.2.838186637.dev9255/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 04:26:34.703131 quickstart-vdk-0.2.838186637.dev9255/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-15 04:23:57.000000 quickstart-vdk-0.2.838186637.dev9255/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.836982976.dev9245/PKG-INFO` & `quickstart-vdk-0.2.838186637.dev9255/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.836982976.dev9245
+Version: 0.2.838186637.dev9255
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.836982976.dev9245/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.838186637.dev9255/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.836982976.dev9245
+Version: 0.2.838186637.dev9255
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.836982976.dev9245/setup.py` & `quickstart-vdk-0.2.838186637.dev9255/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.836982976.dev9245"
+__version__ = "0.2.838186637.dev9255"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

