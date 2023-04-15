# Comparing `tmp/sharewifi-1.0.4.tar.gz` & `tmp/sharewifi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharewifi-1.0.4.tar", last modified: Sat Apr 15 13:53:43 2023, max compression
+gzip compressed data, was "sharewifi-1.0.5.tar", last modified: Sat Apr 15 14:06:07 2023, max compression
```

## Comparing `sharewifi-1.0.4.tar` & `sharewifi-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:53:43.365244 sharewifi-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-15 13:53:43.365244 sharewifi-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 13:53:43.365244 sharewifi-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-15 13:53:32.000000 sharewifi-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:53:43.365244 sharewifi-1.0.4/sharewifi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-15 13:53:43.000000 sharewifi-1.0.4/sharewifi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-15 13:53:43.000000 sharewifi-1.0.4/sharewifi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 13:53:43.000000 sharewifi-1.0.4/sharewifi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-15 13:53:43.000000 sharewifi-1.0.4/sharewifi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 13:53:43.000000 sharewifi-1.0.4/sharewifi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 13:53:43.000000 sharewifi-1.0.4/sharewifi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 14:06:07.471654 sharewifi-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-15 14:06:07.471654 sharewifi-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 14:06:07.471654 sharewifi-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-04-15 14:01:41.000000 sharewifi-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 14:06:07.471654 sharewifi-1.0.5/sharewifi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-15 14:06:07.000000 sharewifi-1.0.5/sharewifi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-15 14:06:07.000000 sharewifi-1.0.5/sharewifi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 14:06:07.000000 sharewifi-1.0.5/sharewifi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-15 14:06:07.000000 sharewifi-1.0.5/sharewifi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 14:06:07.000000 sharewifi-1.0.5/sharewifi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-15 14:06:07.000000 sharewifi-1.0.5/sharewifi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2366 2023-04-15 13:29:52.000000 sharewifi-1.0.5/sharewifi.py
```

### Comparing `sharewifi-1.0.4/PKG-INFO` & `sharewifi-1.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: sharewifi
-Version: 1.0.4
-Summary: Generate QR codes for sharing WiFi network credentials
+Version: 1.0.5
+Summary: A package to generate QR codes for WiFi networks
 Home-page: https://github.com/4NK1T/sharewifi
 Author: Ankit Pandey
 Author-email: ashuankitpandey@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 
 UNKNOWN
```

### Comparing `sharewifi-1.0.4/sharewifi.egg-info/PKG-INFO` & `sharewifi-1.0.5/sharewifi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: sharewifi
-Version: 1.0.4
-Summary: Generate QR codes for sharing WiFi network credentials
+Version: 1.0.5
+Summary: A package to generate QR codes for WiFi networks
 Home-page: https://github.com/4NK1T/sharewifi
 Author: Ankit Pandey
 Author-email: ashuankitpandey@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 
 UNKNOWN
```

