# Comparing `tmp/sball-0.9.6.tar.gz` & `tmp/sball-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sball-0.9.6.tar", last modified: Sat Apr 15 03:10:24 2023, max compression
+gzip compressed data, was "sball-1.0.0.tar", last modified: Sat Apr 15 03:15:00 2023, max compression
```

## Comparing `sball-0.9.6.tar` & `sball-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.516938 sball-0.9.6/
--rw-rw-rw-   0        0        0     4244 2023-04-15 03:10:24.514938 sball-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     3769 2023-04-15 03:09:19.000000 sball-0.9.6/README.md
--rw-rw-rw-   0        0        0      632 2023-04-15 03:05:45.000000 sball-0.9.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 03:10:24.516938 sball-0.9.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.495937 sball-0.9.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.503937 sball-0.9.6/src/sball/
--rw-rw-rw-   0        0        0       38 2023-04-15 03:05:38.000000 sball-0.9.6/src/sball/__init__.py
--rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-0.9.6/src/sball/__main__.py
--rw-rw-rw-   0        0        0     4972 2023-04-15 03:09:39.000000 sball-0.9.6/src/sball/sball.py
-drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.513938 sball-0.9.6/src/sball.egg-info/
--rw-rw-rw-   0        0        0     4244 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 03:15:00.797814 sball-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 03:14:00.000000 sball-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4267 2023-04-15 03:15:00.796618 sball-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3769 2023-04-15 03:09:19.000000 sball-1.0.0/README.md
+-rw-rw-rw-   0        0        0      632 2023-04-15 03:14:14.000000 sball-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 03:15:00.798618 sball-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 03:15:00.778620 sball-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 03:15:00.787619 sball-1.0.0/src/sball/
+-rw-rw-rw-   0        0        0       38 2023-04-15 03:14:27.000000 sball-1.0.0/src/sball/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-1.0.0/src/sball/__main__.py
+-rw-rw-rw-   0        0        0     4972 2023-04-15 03:09:39.000000 sball-1.0.0/src/sball/sball.py
+drwxrwxrwx   0        0        0        0 2023-04-15 03:15:00.794618 sball-1.0.0/src/sball.egg-info/
+-rw-rw-rw-   0        0        0     4267 2023-04-15 03:15:00.000000 sball-1.0.0/src/sball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-15 03:15:00.000000 sball-1.0.0/src/sball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 03:15:00.000000 sball-1.0.0/src/sball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-15 03:15:00.000000 sball-1.0.0/src/sball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 03:15:00.000000 sball-1.0.0/src/sball.egg-info/top_level.txt
```

### Comparing `sball-0.9.6/PKG-INFO` & `sball-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sball
-Version: 0.9.6
+Version: 1.0.0
 Summary: Submit scripts in job arrays using Yale's dSQ.
 Author-email: Michael Wilson <michael.a.wilson@yale.edu>
 Project-URL: Homepage, https://github.com/mawilson1234/sball
 Keywords: slurm,job array,sbatch,dSQ,dsq
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # sball
 
 `sball` facilitates submitting multiple scripts in Slurm job arrays using Yale's dSQ module. "sball" is short for "sbatch all".
 
 ## Usage
```

### Comparing `sball-0.9.6/README.md` & `sball-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sball-0.9.6/pyproject.toml` & `sball-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires=['setuptools', 'wheel']
 build-backend='setuptools.build_meta'
 
 [project]
 name='sball'
-version='0.9.6'
+version='1.0.0'
 description="Submit scripts in job arrays using Yale's dSQ."
 readme='README.md'
 authors=[{name="Michael Wilson", email='michael.a.wilson@yale.edu'}]
 classifiers=[
 	'Development Status :: 4 - Beta',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
```

### Comparing `sball-0.9.6/src/sball/sball.py` & `sball-1.0.0/src/sball/sball.py`

 * *Files identical despite different names*

### Comparing `sball-0.9.6/src/sball.egg-info/PKG-INFO` & `sball-1.0.0/src/sball.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sball
-Version: 0.9.6
+Version: 1.0.0
 Summary: Submit scripts in job arrays using Yale's dSQ.
 Author-email: Michael Wilson <michael.a.wilson@yale.edu>
 Project-URL: Homepage, https://github.com/mawilson1234/sball
 Keywords: slurm,job array,sbatch,dSQ,dsq
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # sball
 
 `sball` facilitates submitting multiple scripts in Slurm job arrays using Yale's dSQ module. "sball" is short for "sbatch all".
 
 ## Usage
```

