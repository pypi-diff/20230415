# Comparing `tmp/sharewifi-1.0.2.tar.gz` & `tmp/sharewifi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharewifi-1.0.2.tar", last modified: Sat Apr 15 13:30:05 2023, max compression
+gzip compressed data, was "sharewifi-1.0.3.tar", last modified: Sat Apr 15 13:44:04 2023, max compression
```

## Comparing `sharewifi-1.0.2.tar` & `sharewifi-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:30:05.965188 sharewifi-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-15 13:30:05.965188 sharewifi-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 13:30:05.965188 sharewifi-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-15 13:29:38.000000 sharewifi-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:30:05.965188 sharewifi-1.0.2/sharewifi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-15 13:30:05.000000 sharewifi-1.0.2/sharewifi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-15 13:30:05.000000 sharewifi-1.0.2/sharewifi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 13:30:05.000000 sharewifi-1.0.2/sharewifi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-15 13:30:05.000000 sharewifi-1.0.2/sharewifi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 13:30:05.000000 sharewifi-1.0.2/sharewifi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 13:30:05.000000 sharewifi-1.0.2/sharewifi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:44:04.813221 sharewifi-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-15 13:44:04.813221 sharewifi-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 13:44:04.813221 sharewifi-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-15 13:43:44.000000 sharewifi-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:44:04.813221 sharewifi-1.0.3/sharewifi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-15 13:44:04.000000 sharewifi-1.0.3/sharewifi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-15 13:44:04.000000 sharewifi-1.0.3/sharewifi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 13:44:04.000000 sharewifi-1.0.3/sharewifi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-15 13:44:04.000000 sharewifi-1.0.3/sharewifi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 13:44:04.000000 sharewifi-1.0.3/sharewifi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 13:44:04.000000 sharewifi-1.0.3/sharewifi.egg-info/top_level.txt
```

### Comparing `sharewifi-1.0.2/PKG-INFO` & `sharewifi-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharewifi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate QR codes for sharing WiFi network credentials
 Home-page: https://github.com/4NK1T/sharewifi
 Author: Ankit Pandey
 Author-email: ashuankitpandey@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sharewifi-1.0.2/setup.py` & `sharewifi-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sharewifi',
-    version='1.0.2',
+    version='1.0.3',
     description='Generate QR codes for sharing WiFi network credentials',
     url='https://github.com/4NK1T/sharewifi',
     author='Ankit Pandey',
     author_email='ashuankitpandey@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         'console_scripts': [
-            'sharewifi=sharewifi.sharewifi:generateQR'
+            'sharewifi=sharewifi:generateQR'
         ]
     },
     install_requires=[
         'qrcode',
         'click',
         'cffi',
         'pycparser',
```

### Comparing `sharewifi-1.0.2/sharewifi.egg-info/PKG-INFO` & `sharewifi-1.0.3/sharewifi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharewifi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate QR codes for sharing WiFi network credentials
 Home-page: https://github.com/4NK1T/sharewifi
 Author: Ankit Pandey
 Author-email: ashuankitpandey@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

