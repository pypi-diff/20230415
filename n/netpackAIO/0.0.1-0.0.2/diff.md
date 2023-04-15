# Comparing `tmp/netpackAIO-0.0.1.tar.gz` & `tmp/netpackAIO-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpackAIO-0.0.1.tar", last modified: Sat Apr 15 00:35:20 2023, max compression
+gzip compressed data, was "netpackAIO-0.0.2.tar", last modified: Sat Apr 15 00:51:03 2023, max compression
```

## Comparing `netpackAIO-0.0.1.tar` & `netpackAIO-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:35:20.663677 netpackAIO-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2172 2023-04-15 00:35:20.664547 netpackAIO-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1661 2023-04-14 23:20:11.000000 netpackAIO-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 00:35:20.636550 netpackAIO-0.0.1/netpack/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.1/netpack/__init__.py
--rw-rw-rw-   0        0        0     3034 2023-04-14 21:45:51.000000 netpackAIO-0.0.1/netpack/func.py
--rw-rw-rw-   0        0        0      100 2023-04-14 20:40:41.000000 netpackAIO-0.0.1/netpack/test.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:35:20.661547 netpackAIO-0.0.1/netpackAIO.egg-info/
--rw-rw-rw-   0        0        0     2172 2023-04-15 00:35:20.000000 netpackAIO-0.0.1/netpackAIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-04-15 00:35:20.000000 netpackAIO-0.0.1/netpackAIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:35:20.000000 netpackAIO-0.0.1/netpackAIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 00:35:20.000000 netpackAIO-0.0.1/netpackAIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-15 00:35:20.669547 netpackAIO-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      634 2023-04-15 00:35:11.000000 netpackAIO-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:51:03.643650 netpackAIO-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2172 2023-04-15 00:51:03.643650 netpackAIO-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1661 2023-04-14 23:20:11.000000 netpackAIO-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:51:03.607649 netpackAIO-0.0.2/netpack/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.2/netpack/__init__.py
+-rw-rw-rw-   0        0        0     3034 2023-04-14 21:45:51.000000 netpackAIO-0.0.2/netpack/func.py
+-rw-rw-rw-   0        0        0      100 2023-04-14 20:40:41.000000 netpackAIO-0.0.2/netpack/test.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:51:03.641612 netpackAIO-0.0.2/netpackAIO.egg-info/
+-rw-rw-rw-   0        0        0     2172 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:51:03.650613 netpackAIO-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-04-15 00:50:45.000000 netpackAIO-0.0.2/setup.py
```

### Comparing `netpackAIO-0.0.1/LICENSE` & `netpackAIO-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.1/PKG-INFO` & `netpackAIO-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netpackAIO-0.0.1/README.md` & `netpackAIO-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.1/netpack/func.py` & `netpackAIO-0.0.2/netpack/func.py`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.1/netpackAIO.egg-info/PKG-INFO` & `netpackAIO-0.0.2/netpackAIO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netpackAIO-0.0.1/setup.py` & `netpackAIO-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='netpackAIO',
-    version='0.0.1',
+    version='0.0.2',
     description='A Python package for performing network-related tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Dongjie Zhang',
     author_email='crusade.ray@gmail.com',
     url='https://github.com/crusaderay/netpack',
     packages=find_packages(),
+    install_requires=['bs4==0.0.1', 'requests==2.28.2'],
     python_requires='>=3.6',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
+
+
+# $ pip install setuptools wheel
+# $ python setup.py sdist bdist_wheel
+# $ python -m twine register
+# $ python -m twine upload dist/*
```

