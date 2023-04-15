# Comparing `tmp/pavegen-0.1.0.tar.gz` & `tmp/pavegen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pavegen-0.1.0.tar", last modified: Sat Apr 15 04:08:54 2023, max compression
+gzip compressed data, was "pavegen-0.1.1.tar", last modified: Sat Apr 15 04:22:05 2023, max compression
```

## Comparing `pavegen-0.1.0.tar` & `pavegen-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:08:54.953269 pavegen-0.1.0/
--rw-r--r--   0 onr5547  (530804311) 1162086330      605 2023-04-15 04:08:54.953146 pavegen-0.1.0/PKG-INFO
-drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:08:54.952108 pavegen-0.1.0/models/
--rw-rw-r--   0 onr5547  (530804311) 1162086330     1677 2023-04-15 00:58:30.000000 pavegen-0.1.0/models/GenPav.py
--rw-rw-r--   0 onr5547  (530804311) 1162086330        0 2023-04-15 00:53:06.000000 pavegen-0.1.0/models/__init__.py
-drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:08:54.952723 pavegen-0.1.0/pavegen.egg-info/
--rw-r--r--   0 onr5547  (530804311) 1162086330      605 2023-04-15 04:08:54.000000 pavegen-0.1.0/pavegen.egg-info/PKG-INFO
--rw-r--r--   0 onr5547  (530804311) 1162086330      230 2023-04-15 04:08:54.000000 pavegen-0.1.0/pavegen.egg-info/SOURCES.txt
--rw-r--r--   0 onr5547  (530804311) 1162086330        1 2023-04-15 04:08:54.000000 pavegen-0.1.0/pavegen.egg-info/dependency_links.txt
--rw-r--r--   0 onr5547  (530804311) 1162086330       42 2023-04-15 04:08:54.000000 pavegen-0.1.0/pavegen.egg-info/requires.txt
--rw-r--r--   0 onr5547  (530804311) 1162086330       13 2023-04-15 04:08:54.000000 pavegen-0.1.0/pavegen.egg-info/top_level.txt
--rw-r--r--   0 onr5547  (530804311) 1162086330       38 2023-04-15 04:08:54.953325 pavegen-0.1.0/setup.cfg
--rw-rw-r--   0 onr5547  (530804311) 1162086330      983 2023-04-15 03:24:04.000000 pavegen-0.1.0/setup.py
-drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:08:54.952969 pavegen-0.1.0/utils/
--rw-rw-r--   0 onr5547  (530804311) 1162086330        0 2023-04-15 00:54:04.000000 pavegen-0.1.0/utils/__init__.py
--rw-rw-r--   0 onr5547  (530804311) 1162086330     2809 2023-04-15 01:01:58.000000 pavegen-0.1.0/utils/func.py
+drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:22:05.304059 pavegen-0.1.1/
+-rw-r--r--   0 onr5547  (530804311) 1162086330      510 2023-04-15 04:22:05.303941 pavegen-0.1.1/PKG-INFO
+drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:22:05.302774 pavegen-0.1.1/models/
+-rw-rw-r--   0 onr5547  (530804311) 1162086330     1677 2023-04-15 00:58:30.000000 pavegen-0.1.1/models/GenPav.py
+-rw-rw-r--   0 onr5547  (530804311) 1162086330        0 2023-04-15 00:53:06.000000 pavegen-0.1.1/models/__init__.py
+drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:22:05.303481 pavegen-0.1.1/pavegen.egg-info/
+-rw-r--r--   0 onr5547  (530804311) 1162086330      510 2023-04-15 04:22:05.000000 pavegen-0.1.1/pavegen.egg-info/PKG-INFO
+-rw-r--r--   0 onr5547  (530804311) 1162086330      230 2023-04-15 04:22:05.000000 pavegen-0.1.1/pavegen.egg-info/SOURCES.txt
+-rw-r--r--   0 onr5547  (530804311) 1162086330        1 2023-04-15 04:22:05.000000 pavegen-0.1.1/pavegen.egg-info/dependency_links.txt
+-rw-r--r--   0 onr5547  (530804311) 1162086330       42 2023-04-15 04:22:05.000000 pavegen-0.1.1/pavegen.egg-info/requires.txt
+-rw-r--r--   0 onr5547  (530804311) 1162086330       13 2023-04-15 04:22:05.000000 pavegen-0.1.1/pavegen.egg-info/top_level.txt
+-rw-r--r--   0 onr5547  (530804311) 1162086330       38 2023-04-15 04:22:05.304118 pavegen-0.1.1/setup.cfg
+-rw-rw-r--   0 onr5547  (530804311) 1162086330      967 2023-04-15 04:21:51.000000 pavegen-0.1.1/setup.py
+drwxr-xr-x   0 onr5547  (530804311) 1162086330        0 2023-04-15 04:22:05.303767 pavegen-0.1.1/utils/
+-rw-rw-r--   0 onr5547  (530804311) 1162086330        0 2023-04-15 00:54:04.000000 pavegen-0.1.1/utils/__init__.py
+-rw-rw-r--   0 onr5547  (530804311) 1162086330     2809 2023-04-15 01:01:58.000000 pavegen-0.1.1/utils/func.py
```

### Comparing `pavegen-0.1.0/models/GenPav.py` & `pavegen-0.1.1/models/GenPav.py`

 * *Files identical despite different names*

### Comparing `pavegen-0.1.0/setup.py` & `pavegen-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pavegen',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
-    data_files=[('pavegen', ['best_model_pavegen_best_1.pth'])],
+    data_files=[('pavegen', ['model.pth'])],
     install_requires=[
         'numpy',
         'torch',
         'torchvision',
         'matplotlib',
         'Pillow',
     ],
     author='Armstrong Aboah',
     author_email='aboah1994@gmail.com',
     description='A short description of your package',
     # slong_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/your-username/my_package',
+    # long_description_content_type='text/markdown',
+    # url='https://github.com/your-username/my_package',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `pavegen-0.1.0/utils/func.py` & `pavegen-0.1.1/utils/func.py`

 * *Files identical despite different names*

