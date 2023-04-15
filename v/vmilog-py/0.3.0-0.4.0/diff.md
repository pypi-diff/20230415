# Comparing `tmp/vmilog-py-0.3.0.tar.gz` & `tmp/vmilog-py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmilog-py-0.3.0.tar", last modified: Tue Apr 11 10:01:45 2023, max compression
+gzip compressed data, was "vmilog-py-0.4.0.tar", last modified: Sat Apr 15 06:57:21 2023, max compression
```

## Comparing `vmilog-py-0.3.0.tar` & `vmilog-py-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:45.811862 vmilog-py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 10:01:19.000000 vmilog-py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-11 10:01:45.811862 vmilog-py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 10:01:19.000000 vmilog-py-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:01:45.811862 vmilog-py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-11 10:01:19.000000 vmilog-py-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:45.807861 vmilog-py-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:45.811862 vmilog-py-0.3.0/src/vmi485tousb/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 10:01:19.000000 vmilog-py-0.3.0/src/vmi485tousb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-11 10:01:19.000000 vmilog-py-0.3.0/src/vmi485tousb/_uartChannel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:45.811862 vmilog-py-0.3.0/src/vmilog/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 10:01:19.000000 vmilog-py-0.3.0/src/vmilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-11 10:01:19.000000 vmilog-py-0.3.0/src/vmilog/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:45.811862 vmilog-py-0.3.0/src/vmilog_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-11 10:01:45.000000 vmilog-py-0.3.0/src/vmilog_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 10:01:45.000000 vmilog-py-0.3.0/src/vmilog_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:01:45.000000 vmilog-py-0.3.0/src/vmilog_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 10:01:45.000000 vmilog-py-0.3.0/src/vmilog_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:57:21.686068 vmilog-py-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-15 06:57:21.686068 vmilog-py-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 06:57:21.686068 vmilog-py-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:57:21.682068 vmilog-py-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:57:21.686068 vmilog-py-0.4.0/src/vmi485tousb/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/src/vmi485tousb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/src/vmi485tousb/_uartChannel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:57:21.686068 vmilog-py-0.4.0/src/vmilog/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/src/vmilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/src/vmilog/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:57:21.686068 vmilog-py-0.4.0/src/vmilog_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-15 06:57:21.000000 vmilog-py-0.4.0/src/vmilog_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-15 06:57:21.000000 vmilog-py-0.4.0/src/vmilog_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 06:57:21.000000 vmilog-py-0.4.0/src/vmilog_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 06:57:21.000000 vmilog-py-0.4.0/src/vmilog_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:57:21.686068 vmilog-py-0.4.0/src/vmimpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/src/vmimpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-15 06:57:04.000000 vmilog-py-0.4.0/src/vmimpeg/_stream.py
```

### Comparing `vmilog-py-0.3.0/LICENSE` & `vmilog-py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.3.0/setup.py` & `vmilog-py-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.0"
+VERSION = "0.4.0"
 
 install_requires = [
 ]
 
 setup(
     name="vmilog-py",
     version=VERSION,
```

### Comparing `vmilog-py-0.3.0/src/vmi485tousb/_uartChannel.py` & `vmilog-py-0.4.0/src/vmi485tousb/_uartChannel.py`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.3.0/src/vmilog/_logging.py` & `vmilog-py-0.4.0/src/vmilog/_logging.py`

 * *Files identical despite different names*

