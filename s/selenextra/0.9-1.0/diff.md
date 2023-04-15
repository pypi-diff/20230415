# Comparing `tmp/selenextra-0.9.tar.gz` & `tmp/selenextra-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.9.tar", last modified: Sat Apr 15 06:18:46 2023, max compression
+gzip compressed data, was "selenextra-1.0.tar", last modified: Sat Apr 15 06:29:10 2023, max compression
```

## Comparing `selenextra-0.9.tar` & `selenextra-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 06:18:46.686995 selenextra-0.9/
--rw-rw-rw-   0        0        0    35823 2023-04-15 04:40:09.000000 selenextra-0.9/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-15 06:18:46.686995 selenextra-0.9/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-15 04:40:09.000000 selenextra-0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 06:18:46.679014 selenextra-0.9/selenextra/
--rw-rw-rw-   0        0        0     4629 2023-04-15 06:18:24.000000 selenextra-0.9/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-15 04:40:09.000000 selenextra-0.9/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-15 04:40:09.000000 selenextra-0.9/selenextra/patcher.py
-drwxrwxrwx   0        0        0        0 2023-04-15 06:18:46.684998 selenextra-0.9/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-15 06:18:46.000000 selenextra-0.9/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 06:18:46.686995 selenextra-0.9/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-15 06:18:13.000000 selenextra-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:29:10.658282 selenextra-1.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 06:25:51.000000 selenextra-1.0/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-04-15 06:29:10.657273 selenextra-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-15 06:25:51.000000 selenextra-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 06:29:10.651290 selenextra-1.0/selenextra/
+-rw-rw-rw-   0        0        0     4629 2023-04-15 06:25:51.000000 selenextra-1.0/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-15 06:25:51.000000 selenextra-1.0/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-15 06:25:51.000000 selenextra-1.0/selenextra/patcher.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:29:10.656276 selenextra-1.0/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 06:29:10.658282 selenextra-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      780 2023-04-15 06:28:31.000000 selenextra-1.0/setup.py
```

### Comparing `selenextra-0.9/LICENSE` & `selenextra-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.9/PKG-INFO` & `selenextra-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.9
+Version: 1.0
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.9/selenextra/__init__.py` & `selenextra-1.0/selenextra/__init__.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.9/selenextra/patcher.py` & `selenextra-1.0/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.9/selenextra.egg-info/PKG-INFO` & `selenextra-1.0/selenextra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.9
+Version: 1.0
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.9/setup.py` & `selenextra-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='0.9',
+    version='1.0',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
-        'scipy',
         'undetected_chromedriver',
         'selenium-wire'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.8',
```

