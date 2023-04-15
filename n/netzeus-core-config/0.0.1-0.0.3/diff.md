# Comparing `tmp/netzeus_core_config-0.0.1.tar.gz` & `tmp/netzeus_core_config-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netzeus_core_config-0.0.1.tar", last modified: Sat Apr 15 15:14:25 2023, max compression
+gzip compressed data, was "netzeus_core_config-0.0.3.tar", last modified: Sat Apr 15 15:18:37 2023, max compression
```

## Comparing `netzeus_core_config-0.0.1.tar` & `netzeus_core_config-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-15 15:14:25.187067 netzeus_core_config-0.0.1/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    11356 2023-04-15 15:12:42.000000 netzeus_core_config-0.0.1/LICENSE
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      521 2023-04-15 15:14:25.187067 netzeus_core_config-0.0.1/PKG-INFO
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      224 2023-04-15 14:27:10.000000 netzeus_core_config-0.0.1/README.md
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-15 15:14:25.179067 netzeus_core_config-0.0.1/netzeus_core_config/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)       71 2023-04-15 14:53:43.000000 netzeus_core_config-0.0.1/netzeus_core_config/__init__.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      829 2023-04-15 14:55:41.000000 netzeus_core_config-0.0.1/netzeus_core_config/config.py
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-15 15:14:25.183067 netzeus_core_config-0.0.1/netzeus_core_config.egg-info/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      521 2023-04-15 15:14:25.000000 netzeus_core_config-0.0.1/netzeus_core_config.egg-info/PKG-INFO
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      302 2023-04-15 15:14:25.000000 netzeus_core_config-0.0.1/netzeus_core_config.egg-info/SOURCES.txt
--rw-rw-r--   0 brandon   (1000) brandon   (1000)        1 2023-04-15 15:14:25.000000 netzeus_core_config-0.0.1/netzeus_core_config.egg-info/dependency_links.txt
--rw-rw-r--   0 brandon   (1000) brandon   (1000)       53 2023-04-15 15:14:25.000000 netzeus_core_config-0.0.1/netzeus_core_config.egg-info/requires.txt
--rw-rw-r--   0 brandon   (1000) brandon   (1000)       20 2023-04-15 15:14:25.000000 netzeus_core_config-0.0.1/netzeus_core_config.egg-info/top_level.txt
--rw-rw-r--   0 brandon   (1000) brandon   (1000)       38 2023-04-15 15:14:25.187067 netzeus_core_config-0.0.1/setup.cfg
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      635 2023-04-15 15:14:10.000000 netzeus_core_config-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:18:37.441632 netzeus_core_config-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-15 15:18:37.441632 netzeus_core_config-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-15 15:18:19.000000 netzeus_core_config-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:18:37.441632 netzeus_core_config-0.0.3/netzeus_core_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-15 15:18:19.000000 netzeus_core_config-0.0.3/netzeus_core_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-15 15:18:19.000000 netzeus_core_config-0.0.3/netzeus_core_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:18:37.441632 netzeus_core_config-0.0.3/netzeus_core_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-15 15:18:37.000000 netzeus_core_config-0.0.3/netzeus_core_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-15 15:18:37.000000 netzeus_core_config-0.0.3/netzeus_core_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:18:37.000000 netzeus_core_config-0.0.3/netzeus_core_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 15:18:37.000000 netzeus_core_config-0.0.3/netzeus_core_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 15:18:37.000000 netzeus_core_config-0.0.3/netzeus_core_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:18:37.441632 netzeus_core_config-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-15 15:18:19.000000 netzeus_core_config-0.0.3/setup.py
```

### Comparing `netzeus_core_config-0.0.1/netzeus_core_config/config.py` & `netzeus_core_config-0.0.3/netzeus_core_config/config.py`

 * *Files identical despite different names*

### Comparing `netzeus_core_config-0.0.1/setup.py` & `netzeus_core_config-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setup(
     name="netzeus_core_config",
-    version="0.0.1",
+    version="0.0.3",
     description="NetZeus Core Config module for managing configuration data across all microservices/plugins",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Brandon Spendlove",
     author_email="brandon.spendlove@netzeus.io",
     packages=find_packages(),
     include_package_data=True,
```

