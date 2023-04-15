# Comparing `tmp/makerlabs-0.30.tar.gz` & `tmp/makerlabs-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makerlabs-0.30.tar", last modified: Mon Feb 20 10:21:01 2023, max compression
+gzip compressed data, was "makerlabs-0.31.tar", last modified: Sat Apr 15 09:32:39 2023, max compression
```

## Comparing `makerlabs-0.30.tar` & `makerlabs-0.31.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-02-20 10:21:01.575381 makerlabs-0.30/
--rw-r--r--   0 massimo    (501) staff       (20)     7633 2021-02-28 19:17:44.000000 makerlabs-0.30/LICENSE.md
--rw-r--r--   0 massimo    (501) staff       (20)     2170 2023-02-20 10:21:01.575713 makerlabs-0.30/PKG-INFO
--rw-r--r--   0 massimo    (501) staff       (20)     1395 2023-02-20 10:19:56.000000 makerlabs-0.30/README.md
-drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-02-20 10:21:01.567190 makerlabs-0.30/makerlabs/
--rw-r--r--   0 massimo    (501) staff       (20)        0 2022-04-16 18:00:11.000000 makerlabs-0.30/makerlabs/__init__.py
--rw-r--r--   0 massimo    (501) staff       (20)     1817 2022-09-08 18:39:43.000000 makerlabs-0.30/makerlabs/classes.py
--rw-r--r--   0 massimo    (501) staff       (20)     5582 2023-02-19 22:33:12.000000 makerlabs-0.30/makerlabs/diybio_org.py
--rw-r--r--   0 massimo    (501) staff       (20)     3268 2023-02-19 22:34:41.000000 makerlabs-0.30/makerlabs/fablabs_io.py
--rw-r--r--   0 massimo    (501) staff       (20)     3528 2023-02-19 22:45:09.000000 makerlabs-0.30/makerlabs/hackaday_io.py
--rw-r--r--   0 massimo    (501) staff       (20)     8657 2023-02-19 22:35:18.000000 makerlabs-0.30/makerlabs/hackerspaces_org.py
--rw-r--r--   0 massimo    (501) staff       (20)     3062 2023-02-19 22:45:46.000000 makerlabs-0.30/makerlabs/makerfaire_com.py
--rw-r--r--   0 massimo    (501) staff       (20)     2630 2023-02-19 22:35:34.000000 makerlabs-0.30/makerlabs/makerspaces_make_co.py
--rw-r--r--   0 massimo    (501) staff       (20)     2705 2023-02-19 22:35:42.000000 makerlabs-0.30/makerlabs/makery_info.py
--rw-r--r--   0 massimo    (501) staff       (20)     7925 2023-02-19 22:35:49.000000 makerlabs-0.30/makerlabs/repaircafe_org.py
--rw-r--r--   0 massimo    (501) staff       (20)     3739 2023-02-19 22:46:55.000000 makerlabs-0.30/makerlabs/timeline.py
--rw-r--r--   0 massimo    (501) staff       (20)     4447 2022-09-12 10:56:14.000000 makerlabs-0.30/makerlabs/utils.py
-drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-02-20 10:21:01.574591 makerlabs-0.30/makerlabs.egg-info/
--rw-r--r--   0 massimo    (501) staff       (20)     2170 2023-02-20 10:21:01.000000 makerlabs-0.30/makerlabs.egg-info/PKG-INFO
--rw-r--r--   0 massimo    (501) staff       (20)      504 2023-02-20 10:21:01.000000 makerlabs-0.30/makerlabs.egg-info/SOURCES.txt
--rw-r--r--   0 massimo    (501) staff       (20)        1 2023-02-20 10:21:01.000000 makerlabs-0.30/makerlabs.egg-info/dependency_links.txt
--rw-r--r--   0 massimo    (501) staff       (20)      165 2023-02-20 10:21:01.000000 makerlabs-0.30/makerlabs.egg-info/requires.txt
--rw-r--r--   0 massimo    (501) staff       (20)       10 2023-02-20 10:21:01.000000 makerlabs-0.30/makerlabs.egg-info/top_level.txt
--rw-r--r--   0 massimo    (501) staff       (20)      495 2023-02-20 10:21:01.577629 makerlabs-0.30/setup.cfg
--rw-r--r--   0 massimo    (501) staff       (20)     1542 2023-02-20 10:19:49.000000 makerlabs-0.30/setup.py
+drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-15 09:32:39.453284 makerlabs-0.31/
+-rw-r--r--   0 massimo    (501) staff       (20)     7633 2021-02-28 19:17:44.000000 makerlabs-0.31/LICENSE.md
+-rw-r--r--   0 massimo    (501) staff       (20)     2177 2023-04-15 09:32:39.453616 makerlabs-0.31/PKG-INFO
+-rw-r--r--   0 massimo    (501) staff       (20)     1395 2023-02-20 10:19:56.000000 makerlabs-0.31/README.md
+drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-15 09:32:39.440235 makerlabs-0.31/makerlabs/
+-rw-r--r--   0 massimo    (501) staff       (20)        0 2022-04-16 18:00:11.000000 makerlabs-0.31/makerlabs/__init__.py
+-rw-r--r--   0 massimo    (501) staff       (20)     1817 2022-09-08 18:39:43.000000 makerlabs-0.31/makerlabs/classes.py
+-rw-r--r--   0 massimo    (501) staff       (20)     5582 2023-02-19 22:33:12.000000 makerlabs-0.31/makerlabs/diybio_org.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3280 2023-04-14 23:44:23.000000 makerlabs-0.31/makerlabs/fablabs_io.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3528 2023-02-19 22:45:09.000000 makerlabs-0.31/makerlabs/hackaday_io.py
+-rw-r--r--   0 massimo    (501) staff       (20)     8657 2023-02-19 22:35:18.000000 makerlabs-0.31/makerlabs/hackerspaces_org.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3062 2023-02-19 22:45:46.000000 makerlabs-0.31/makerlabs/makerfaire_com.py
+-rw-r--r--   0 massimo    (501) staff       (20)     2630 2023-02-19 22:35:34.000000 makerlabs-0.31/makerlabs/makerspaces_make_co.py
+-rw-r--r--   0 massimo    (501) staff       (20)     2705 2023-02-19 22:35:42.000000 makerlabs-0.31/makerlabs/makery_info.py
+-rw-r--r--   0 massimo    (501) staff       (20)     7925 2023-02-19 22:35:49.000000 makerlabs-0.31/makerlabs/repaircafe_org.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3739 2023-02-19 22:46:55.000000 makerlabs-0.31/makerlabs/timeline.py
+-rw-r--r--   0 massimo    (501) staff       (20)     4447 2022-09-12 10:56:14.000000 makerlabs-0.31/makerlabs/utils.py
+drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-15 09:32:39.452346 makerlabs-0.31/makerlabs.egg-info/
+-rw-r--r--   0 massimo    (501) staff       (20)     2177 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/PKG-INFO
+-rw-r--r--   0 massimo    (501) staff       (20)      504 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 massimo    (501) staff       (20)        1 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 massimo    (501) staff       (20)      165 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/requires.txt
+-rw-r--r--   0 massimo    (501) staff       (20)       10 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/top_level.txt
+-rw-r--r--   0 massimo    (501) staff       (20)      495 2023-04-15 09:32:39.455092 makerlabs-0.31/setup.cfg
+-rw-r--r--   0 massimo    (501) staff       (20)     1552 2023-04-15 09:29:41.000000 makerlabs-0.31/setup.py
```

### Comparing `makerlabs-0.30/LICENSE.md` & `makerlabs-0.31/LICENSE.md`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/PKG-INFO` & `makerlabs-0.31/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: makerlabs
-Version: 0.30
+Version: 0.31
 Home-page: https://github.com/openp2pdesign/makerlabs
-Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.30
+Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.31
 Author: Massimo Menichinelli
 Author-email: info@openp2pdesign.org
-Keywords: Fab Lab,Fab Lab,Makerspace,Hackerspace,Repair Cafes,Makers
+Keywords: Fab Lab,Fab Lab,Makerspace,Hackerspace,Repair Cafes,Makers,DIYbio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `makerlabs-0.30/README.md` & `makerlabs-0.31/README.md`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/classes.py` & `makerlabs-0.31/makerlabs/classes.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/diybio_org.py` & `makerlabs-0.31/makerlabs/diybio_org.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/fablabs_io.py` & `makerlabs-0.31/makerlabs/fablabs_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """Represents a Fab Lab as it is described on fablabs.io."""
 
     def __init__(self):
         self.source = "fablabs.io"
         self.lab_type = "Fab Lab"
 
 
-def data_from_fablabs_io():
+def data_from_fablabs_io(API_endpoint):
     """Gets data from fablabs.io."""
 
     data = requests.get(API_endpoint).json()
 
     return data
```

### Comparing `makerlabs-0.30/makerlabs/hackaday_io.py` & `makerlabs-0.31/makerlabs/hackaday_io.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/hackerspaces_org.py` & `makerlabs-0.31/makerlabs/hackerspaces_org.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/makerfaire_com.py` & `makerlabs-0.31/makerlabs/makerfaire_com.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/makerspaces_make_co.py` & `makerlabs-0.31/makerlabs/makerspaces_make_co.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/makery_info.py` & `makerlabs-0.31/makerlabs/makery_info.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/repaircafe_org.py` & `makerlabs-0.31/makerlabs/repaircafe_org.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/timeline.py` & `makerlabs-0.31/makerlabs/timeline.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs/utils.py` & `makerlabs-0.31/makerlabs/utils.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.30/makerlabs.egg-info/PKG-INFO` & `makerlabs-0.31/makerlabs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: makerlabs
-Version: 0.30
+Version: 0.31
 Home-page: https://github.com/openp2pdesign/makerlabs
-Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.30
+Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.31
 Author: Massimo Menichinelli
 Author-email: info@openp2pdesign.org
-Keywords: Fab Lab,Fab Lab,Makerspace,Hackerspace,Repair Cafes,Makers
+Keywords: Fab Lab,Fab Lab,Makerspace,Hackerspace,Repair Cafes,Makers,DIYbio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `makerlabs-0.30/setup.py` & `makerlabs-0.31/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,23 +27,23 @@
         "pytz",
         "requests",
         "six",
         "soupsieve",
         "urllib3",
         "us"
     ],
-    version='0.30',
+    version='0.31',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Massimo Menichinelli',
     author_email='info@openp2pdesign.org',
     url='https://github.com/openp2pdesign/makerlabs',
-    download_url='https://github.com/openp2pdesign/makerlabs/releases/tag/v0.30',
+    download_url='https://github.com/openp2pdesign/makerlabs/releases/tag/v0.31',
     keywords=['Fab Lab', 'Fab Lab', 'Makerspace', 'Hackerspace', 'Repair Cafes',
-              'Makers'],
+              'Makers', 'DIYbio'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "Environment :: Web Environment",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python",
```

