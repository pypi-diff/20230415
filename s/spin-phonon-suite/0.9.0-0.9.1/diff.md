# Comparing `tmp/spin_phonon_suite-0.9.0.tar.gz` & `tmp/spin_phonon_suite-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin_phonon_suite-0.9.0.tar", last modified: Thu Sep  1 14:45:32 2022, max compression
+gzip compressed data, was "spin_phonon_suite-0.9.1.tar", last modified: Thu Sep 22 16:44:44 2022, max compression
```

## Comparing `spin_phonon_suite-0.9.0.tar` & `spin_phonon_suite-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 14:45:32.916545 spin_phonon_suite-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3750 2022-09-01 14:45:32.915545 spin_phonon_suite-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3031 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-01 14:45:32.916545 spin_phonon_suite-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1624 2022-09-01 14:45:30.000000 spin_phonon_suite-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 14:45:32.913545 spin_phonon_suite-0.9.0/spin_phonon_suite/
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2022-09-01 14:45:30.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    26225 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/cells.py
--rw-rw-rw-   0 root         (0) root         (0)    34571 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    10565 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/derivative.py
--rw-rw-rw-   0 root         (0) root         (0)     8653 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/distortion.py
--rw-rw-rw-   0 root         (0) root         (0)     2906 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/func.py
--rw-rw-rw-   0 root         (0) root         (0)    12030 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/lvc.py
--rw-rw-rw-   0 root         (0) root         (0)    10800 2022-09-01 14:44:41.000000 spin_phonon_suite-0.9.0/spin_phonon_suite/vibrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 14:45:32.915545 spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3750 2022-09-01 14:45:32.000000 spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2022-09-01 14:45:32.000000 spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-01 14:45:32.000000 spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2022-09-01 14:45:32.000000 spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      125 2022-09-01 14:45:32.000000 spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-09-01 14:45:32.000000 spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35085 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3750 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      215 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2022-09-22 16:44:41.000000 spin_phonon_suite-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 16:44:44.620681 spin_phonon_suite-0.9.1/spin_phonon_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2022-09-22 16:44:41.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26274 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/cells.py
+-rw-rw-rw-   0 root         (0) root         (0)    34571 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    10565 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)     8653 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/distortion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2906 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/func.py
+-rw-rw-rw-   0 root         (0) root         (0)    12030 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/lvc.py
+-rw-rw-rw-   0 root         (0) root         (0)    10800 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/vibrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3750 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/top_level.txt
```

### Comparing `spin_phonon_suite-0.9.0/LICENSE` & `spin_phonon_suite-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/PKG-INFO` & `spin_phonon_suite-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin_phonon_suite
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-0.9.0/README.md` & `spin_phonon_suite-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/setup.py` & `spin_phonon_suite-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 setuptools.setup(
     name='spin_phonon_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian', # noqa
@@ -37,15 +37,16 @@
         'xyz_py>=5.1.0',
         'angmom_suite>=1.10.0',
         'hpc_suite',
         'matplotlib',
         'findiff',
         'gaussian_suite>=1.8.0',
         'phonopy',
-        'molvis>=0.3.0'
+        'molvis>=0.3.0',
+        'molcas_suite'
         ],
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'spin_phonon_suite = spin_phonon_suite.cli:main'
             ]
         }
```

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite/cells.py` & `spin_phonon_suite-0.9.1/spin_phonon_suite/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,14 +799,15 @@
             f.write("/{}.ENV.{:d}.0s.0s.\n".format(label, it+1))
             f.write("Dummy basis set for atomic charges of environment\n")
             f.write("no ref\n")
             f.write("{:.9f} 0\n".format(charge))
             f.write("0 0\n")
 
     with open(xyz_file, 'w') as f:
+        f.write("{:d}\n\n".format(len(labels)))
         for it, (label, coord) in enumerate(zip(labels, coords)):
             f.write(
                 "{}.ENV.{:d} {:.9f} {:.9f} {:.9f}\n".format(
                     label, it+1, *coord
                 )
             )
     return
@@ -832,8 +833,8 @@
 
     viewer = mvis.Viewer(
         objects=[ms1, ms2],
         extra_div_args=viewer_div_args,
         extra_style_args=viewer_style_args
     )
 
-    return viewer
+    return viewer
```

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite/cli.py` & `spin_phonon_suite-0.9.1/spin_phonon_suite/cli.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite/derivative.py` & `spin_phonon_suite-0.9.1/spin_phonon_suite/derivative.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite/distortion.py` & `spin_phonon_suite-0.9.1/spin_phonon_suite/distortion.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite/func.py` & `spin_phonon_suite-0.9.1/spin_phonon_suite/func.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite/lvc.py` & `spin_phonon_suite-0.9.1/spin_phonon_suite/lvc.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite/vibrations.py` & `spin_phonon_suite-0.9.1/spin_phonon_suite/vibrations.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/PKG-INFO` & `spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-phonon-suite
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-0.9.0/spin_phonon_suite.egg-info/SOURCES.txt` & `spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

