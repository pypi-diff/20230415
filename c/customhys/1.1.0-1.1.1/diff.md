# Comparing `tmp/customhys-1.1.0.tar.gz` & `tmp/customhys-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customhys-1.1.0.tar", last modified: Tue Mar 14 20:57:24 2023, max compression
+gzip compressed data, was "customhys-1.1.1.tar", last modified: Fri Apr 14 23:24:26 2023, max compression
```

## Comparing `customhys-1.1.0.tar` & `customhys-1.1.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-03-14 20:57:24.430812 customhys-1.1.0/
--rw-r--r--   0 jcrvz      (501) staff       (20)     1080 2022-03-15 16:08:28.000000 customhys-1.1.0/LICENSE
--rw-r--r--   0 jcrvz      (501) staff       (20)      122 2022-03-25 21:13:14.000000 customhys-1.1.0/MANIFEST.in
--rw-r--r--   0 jcrvz      (501) staff       (20)    11518 2023-03-14 20:57:24.430933 customhys-1.1.0/PKG-INFO
--rw-r--r--   0 jcrvz      (501) staff       (20)    10931 2023-03-14 20:51:49.000000 customhys-1.1.0/README.md
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-03-14 20:57:24.398760 customhys-1.1.0/customhys/
--rw-r--r--   0 jcrvz      (501) staff       (20)      188 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/__init__.py
--rw-r--r--   0 jcrvz      (501) staff       (20)   124795 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/benchmark_func.py
--rw-r--r--   0 jcrvz      (501) staff       (20)     8163 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/characterisation.py
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-03-14 20:57:24.407265 customhys-1.1.0/customhys/collections/
--rw-r--r--   0 jcrvz      (501) staff       (20)  1265347 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/collections/automatic.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)     8469 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/collections/basicmetaheuristics.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)    21255 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/collections/default.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)    92837 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/collections/operators_collection.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)   255391 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/collections/operators_weights.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     2842 2023-03-14 16:54:51.000000 customhys-1.1.0/customhys/collections/short_collection.txt
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-03-14 20:57:24.409935 customhys-1.1.0/customhys/exconf/
--rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/exconf/basic_metaheuristic.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1717 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/exconf/brute_force.json
--rw-r--r--   0 jcrvz      (501) staff       (20)      299 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/exconf/demo.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1147 2023-03-14 16:54:51.000000 customhys-1.1.0/customhys/exconf/demo_neural_network.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/exconf/long1.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1763 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/exconf/short1.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1713 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/exconf/short2.json
--rw-r--r--   0 jcrvz      (501) staff       (20)    18492 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/experiment.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    62520 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/hyperheuristic.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    13900 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/machine_learning.py
--rw-r--r--   0 jcrvz      (501) staff       (20)     7311 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/metaheuristic.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    45073 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/operators.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    15755 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/population.py
--rw-r--r--   0 jcrvz      (501) staff       (20)      483 2023-03-14 16:54:51.000000 customhys-1.1.0/customhys/test_solvers.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    18587 2023-03-14 16:55:50.000000 customhys-1.1.0/customhys/tools.py
--rw-r--r--   0 jcrvz      (501) staff       (20)     9834 2022-03-15 16:08:28.000000 customhys-1.1.0/customhys/visualisation.py
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-03-14 20:57:24.400715 customhys-1.1.0/customhys.egg-info/
--rw-r--r--   0 jcrvz      (501) staff       (20)    11518 2023-03-14 20:57:24.000000 customhys-1.1.0/customhys.egg-info/PKG-INFO
--rw-r--r--   0 jcrvz      (501) staff       (20)     1255 2023-03-14 20:57:24.000000 customhys-1.1.0/customhys.egg-info/SOURCES.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)        1 2023-03-14 20:57:24.000000 customhys-1.1.0/customhys.egg-info/dependency_links.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)       10 2023-03-14 20:57:24.000000 customhys-1.1.0/customhys.egg-info/top_level.txt
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-03-14 20:57:24.426528 customhys-1.1.0/docfiles/
--rw-r--r--   0 jcrvz      (501) staff       (20)   905189 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/SearchOperators_CEC.pdf
--rw-r--r--   0 jcrvz      (501) staff       (20)    16429 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/cas_logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)    42755 2023-03-14 16:55:35.000000 customhys-1.1.0/docfiles/chm_logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)    28786 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/conacyt-logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   209268 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/dependency_diagram.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   743430 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/heuristics.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   137732 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/logoTEC_full.png
--rw-r--r--   0 jcrvz      (501) staff       (20)  1614825 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/methodology_cec_a.png
--rw-r--r--   0 jcrvz      (501) staff       (20)  2074059 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/methodology_cec_b.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   452031 2022-03-15 16:08:28.000000 customhys-1.1.0/docfiles/operators.png
--rw-r--r--   0 jcrvz      (501) staff       (20)       86 2022-03-25 15:25:53.000000 customhys-1.1.0/pyproject.toml
--rw-r--r--   0 jcrvz      (501) staff       (20)       81 2023-03-14 20:57:24.431214 customhys-1.1.0/setup.cfg
--rw-r--r--   0 jcrvz      (501) staff       (20)      913 2023-03-14 20:57:18.000000 customhys-1.1.0/setup.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.760408 customhys-1.1.1/
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1080 2023-03-16 23:22:43.000000 customhys-1.1.1/LICENSE
+-rw-r--r--   0 jcrvz      (501) staff       (20)      122 2023-03-16 23:22:43.000000 customhys-1.1.1/MANIFEST.in
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11537 2023-04-14 23:24:26.760568 customhys-1.1.1/PKG-INFO
+-rw-r--r--   0 jcrvz      (501) staff       (20)    10931 2023-03-16 23:22:43.000000 customhys-1.1.1/README.md
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.740152 customhys-1.1.1/customhys/
+-rw-r--r--   0 jcrvz      (501) staff       (20)      218 2023-03-22 04:12:13.000000 customhys-1.1.1/customhys/__init__.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)   126445 2023-03-24 05:56:36.000000 customhys-1.1.1/customhys/benchmark_func.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)     8163 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/characterisation.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.745262 customhys-1.1.1/customhys/collections/
+-rw-r--r--   0 jcrvz      (501) staff       (20)  1265347 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/automatic.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)     8469 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/basicmetaheuristics.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)    21255 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/default.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)    92837 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/operators_collection.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)   255391 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/operators_weights.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     2842 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/short_collection.txt
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.746724 customhys-1.1.1/customhys/exconf/
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/basic_metaheuristic.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1717 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/brute_force.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)      299 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/demo.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1147 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/demo_neural_network.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/long1.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1763 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/short1.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1713 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/short2.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)    18465 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/experiment.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    62676 2023-03-21 16:52:55.000000 customhys-1.1.1/customhys/hyperheuristic.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    13900 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/machine_learning.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)     7304 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/metaheuristic.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    45073 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/operators.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    15755 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/population.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)      483 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/test_solvers.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    19272 2023-03-22 04:12:13.000000 customhys-1.1.1/customhys/tools.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11413 2023-03-22 04:12:13.000000 customhys-1.1.1/customhys/visualisation.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.740876 customhys-1.1.1/customhys.egg-info/
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11537 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/PKG-INFO
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1287 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/SOURCES.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)        1 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/dependency_links.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)      227 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/requires.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)       10 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/top_level.txt
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.758082 customhys-1.1.1/docfiles/
+-rw-r--r--   0 jcrvz      (501) staff       (20)   905189 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/SearchOperators_CEC.pdf
+-rw-r--r--   0 jcrvz      (501) staff       (20)    16429 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/cas_logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)    42755 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/chm_logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)    28786 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/conacyt-logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   209268 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/dependency_diagram.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   743430 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/heuristics.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   137732 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/logoTEC_full.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)  1614825 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/methodology_cec_a.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)  2074059 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/methodology_cec_b.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   452031 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/operators.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)       86 2023-03-16 23:22:43.000000 customhys-1.1.1/pyproject.toml
+-rw-r--r--   0 jcrvz      (501) staff       (20)       81 2023-04-14 23:24:26.760892 customhys-1.1.1/setup.cfg
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1345 2023-03-22 04:12:13.000000 customhys-1.1.1/setup.py
```

### Comparing `customhys-1.1.0/LICENSE` & `customhys-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/PKG-INFO` & `customhys-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: customhys
-Version: 1.1.0
+Version: 1.1.1
 Summary: This framework provides tools for solving, but not limited to, continuous optimisation problems using a hyper-heuristic approach for customising metaheuristics. 
 Home-page: https://github.com/jcrvz/customhys
 Author: Jorge Mario Cruz-Duarte
 Author-email: jorge.cruz@tec.mx
 License: MIT License
 Keywords: metaheuristics,hyper-heuristic,optimization,automatic design,global optimization,evolutionary computation,bio-inspired,algorithm design
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: ML
 License-File: LICENSE
 
 # customhys
 
 <div>
     <img align="left" alt="Module Dependency Diagram" src="https://raw.githubusercontent.com/jcrvz/customhys/master/docfiles/chm_logo.png" title="Customhys logo" width="25%"/>
 </div>
```

### Comparing `customhys-1.1.0/README.md` & `customhys-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/benchmark_func.py` & `customhys-1.1.1/customhys/benchmark_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 This module is an upgraded version of the Keita Tomochika's module in
 https://github.com/keit0222/optimization-evaluation. The current module only contain N-dimensional functions. These
 functions are listed in ``__all__``.
 
-All these functions are based and revisited on the following research papers and web sites:
+All these functions are based and revisited on the following research papers and websites:
 
 - Momin Jamil and Xin-She Yang, A literature survey of benchmark functions for global optimization problems,
 Int. Journal of Mathematical Modelling and Numerical Optimisation, Vol. 4, No. 2, pp. 150–194 (2013), arXiv:1308.4008
 - Mazhar Ansari Ardeh, https://github.com/mazhar-ansari-ardeh, http://benchmarkfcns.xyz
 - Sonja Surjanovic and Derek Bingham, Simon Fraser University, https://www.sfu.ca/~ssurjano/optimization.html
 - Ali R. Al-Roomi (2015). Unconstrained Single-Objective Benchmark Functions Repository. Halifax, Nova Scotia,
 Canada, Dalhousie University, Electrical and Computer Engineering. https://www.al-roomi.org/benchmarks/unconstrained
@@ -20,17 +20,32 @@
 @author: Jorge Mario Cruz-Duarte (jcrvz.github.io), e-mail: jorge.cruz@tec.mx
 """
 
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import LightSource
+import abc
+
+_cec_functions = False
+try:
+    from optproblems import cec2005
+    _cec_functions = True
+
+except ImportError as e:
+    import warnings as wa
+
+    message = "`optproblems` not found! Please, install it to use the cec2005 benchmark functions"
+    wa.showwarning(message, ImportWarning, "benchmark_func.py", 29)
+
+import shutil
+if shutil.which("latex") is not None:
+    plt.rc('text', usetex=True)
+    plt.rc('font', family='serif', size=11)
 
-plt.rc('text', usetex=True)
-plt.rc('font', family='serif', size=11)
 
 __all__ = ['Ackley1', 'Ackley4', 'Alpine1', 'Alpine2', 'Bohachevsky', 'Brent', 'Brown', 'CarromTable', 'ChungReynolds',
            'Cigar', 'CosineMixture', 'CrossInTray', 'CrossLegTable', 'CrownedCross', 'Csendes', 'Deb1', 'Deb2',
            'DeflectedCorrugatedSpring', 'DixonPrice', 'DropWave', 'EggHolder', 'Ellipsoid', 'ExpandedDecreasingMinima',
            'ExpandedEqualMinima', 'ExpandedFiveUnevenPeakTrap', 'ExpandedTwoPeakTrap', 'ExpandedUnevenMinima',
            'Exponential', 'F2', 'Giunta', 'Griewank', 'HappyCat', 'HyperEllipsoid', 'InvertedCosineWave',
            'JennrichSampson', 'KTablet', 'Katsuura', 'Levy', 'LunacekN01', 'LunacekN02', 'Michalewicz', 'Mishra1',
@@ -204,39 +219,40 @@
         return self.min_search_range, self.max_search_range
 
     def set_search_range(self, min_search_range, max_search_range):
         """
         Define the problem domain given by the lower and upper boundaries. They could be 1-by-variable_num arrays or
         floats.
         :param min_search_range:
-            Lower boundary of the problem domain. It can be a numpy.array or a float.
+            Lower boundary of the problem domain. It can be a `numpy.array` or a float.
         :param max_search_range:
-            Upper boundary of the problem domain. It can be a numpy.array or a float.
+            Upper boundary of the problem domain. It can be a `numpy.array` or a float.
         :return: None.
         """
         if isinstance(min_search_range, (float, int)) and isinstance(max_search_range, (float, int)):
             self.min_search_range = np.array([min_search_range] * self.variable_num)
             self.max_search_range = np.array([max_search_range] * self.variable_num)
         else:
             if (len(min_search_range) == self.variable_num) and (len(max_search_range) == self.variable_num):
                 self.min_search_range = min_search_range
                 self.max_search_range = max_search_range
             else:
                 print('Invalid range!')
 
+    @abc.abstractmethod
     def get_func_val(self, variables, *args):
         """
         Evaluate the problem function without considering additions like noise, offset, etc.
         :param numpy.array variables:
             The position where the problem function is going to be evaluated.
         :param args:
             Additional arguments that some problem functions could consider.
         :return: float
         """
-        return -1
+        return None
 
     def get_function_value(self, variables, *args):
         """
         Evaluate the problem function considering additions like noise, offset, etc. This method calls ``get_func_val``.
         :param numpy.array variables:
             The position where the problem function is going to be evaluated.
         :param args:
@@ -253,15 +269,15 @@
         if self.__noise_type in ['gaussian', 'normal', 'gauss']:
             noise_value = np.random.randn()
         else:
             noise_value = np.random.rand()
 
         # Call ``get_func_val``with the modifications
         return self.__scale_function * self.get_func_val(variables, *args) + self.__noise_level * noise_value + \
-               self.__offset_function
+            self.__offset_function
 
     def get_function_values(self, samples):
         """
         Map the `get_function_value` method to evaluate a list of samples and return the evaluation for each sample.
         :param list samples:
             List of positions in the problem domain to be evaluated.
         :return: list
@@ -297,15 +313,15 @@
 
         # Initialise the figure
         fig = plt.figure(figsize=[4, 3], dpi=resolution, facecolor='w')
         ls = LightSource(azdeg=90, altdeg=45)
         rgb = ls.shade(matrix_z, plt.cm.jet)
 
         # Plot data
-        ax = fig.gca(projection='3d', proj_type='ortho')
+        ax = fig.add_subplot(111, projection='3d', proj_type='ortho')
         ax.plot_surface(matrix_x, matrix_y, matrix_z, rstride=1, cstride=1, linewidth=0.5,
                         antialiased=False, facecolors=rgb)  #
 
         # Adjust the labels
         ax.set_xlabel('$x_1$')
         ax.set_ylabel('$x_2$')
         ax.set_zlabel('$f(x, y)$')
@@ -346,14 +362,15 @@
         self.plot(samples, resolution)
 
         # Save it
         plt.tight_layout()
         self.plot_object.savefig(self.save_dir + self.func_name + '.' + ext)
         plt.show()
 
+    @abc.abstractmethod
     def get_formatted_problem(self, is_constrained=True, fts=None):
         """
         Return the problem in a simple format to be used in a solving procedure. This format contains the ``function``
         in lambda form, the ``boundaries`` as a tuple with the lower and upper boundaries, and the ``is_constrained``
         flag.
         :param bool is_constrained: Optional.
             Flag indicating if the problem domain has hard boundaries.
@@ -409,16 +426,16 @@
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         return np.exp(-0.2) * np.sum(np.sqrt(
             np.square(variables[:-1]) + np.square(variables[1:]))) + \
-               3. * np.sum(np.cos(2. * variables[:-1]) +
-                           np.sin(2. * variables[:-1]))
+            3. * np.sum(np.cos(2. * variables[:-1]) +
+                        np.sin(2. * variables[:-1]))
 
 
 # 6 - Class Alpine 1 function
 class Alpine1(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([10.] * self.variable_num)
@@ -662,16 +679,15 @@
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         xi = variables[:-1]
         xi1 = variables[1:]
         return np.sum(-(xi1 + 47.) * np.sin(np.sqrt(
-            np.abs(xi1 + xi / 2. + 47.))) - xi * np.sin(np.sqrt(
-            np.abs(xi - xi1 - 47.))))
+            np.abs(xi1 + xi / 2. + 47.))) - xi * np.sin(np.sqrt(np.abs(xi - xi1 - 47.))))
 
 
 # Class Expanded Two-Peak Trap function [Qu2016]
 class ExpandedTwoPeakTrap(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([100.] * self.variable_num)
@@ -694,15 +710,15 @@
                 return 160. * (y - 15.) / 15.
             elif 15. <= y < 20.:
                 return 200. * (15. - y) / 5.
             else:
                 return -200. + np.square(y - 20.)
 
         return np.sum(np.vectorize(get_cases)(variables + 20.)) + 200. * \
-               self.variable_num
+            self.variable_num
 
 
 # Class Expanded Five-Uneven-Peak Trap function [Qu2016]
 class ExpandedFiveUnevenPeakTrap(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([100.] * self.variable_num)
@@ -790,15 +806,15 @@
             if 0. <= y < 1.:
                 return -np.exp(-2. * np.log(2.) * np.square((y - 0.1) / 0.8)) * np.power(np.sin(
                     5. * np.pi * y), 6.)
             else:
                 return np.square(y)
 
         return np.sum(np.vectorize(get_cases)(variables + 0.1)) + \
-               self.variable_num
+            self.variable_num
 
 
 # Class Expanded Uneven Minima function [Qu2016]
 class ExpandedUnevenMinima(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([100.] * self.variable_num)
@@ -817,15 +833,15 @@
         def get_cases(y):
             if 0. <= y < 1.:
                 return -np.power(np.sin(5. * np.pi * (np.power(y, 3. / 4.) - 0.05)), 6.)
             else:
                 return np.square(y)
 
         return np.sum(np.vectorize(get_cases)(variables + 0.079699392688696)) - \
-               self.variable_num
+            self.variable_num
 
 
 # Class Vincent function [http://infinity77.net/global_optimization/test_functions_nd_V.html#go_benchmark
 # .VenterSobiezcczanskiSobieski]
 class Vincent(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
@@ -867,15 +883,15 @@
                 return np.square(0.25 - y) - np.sin(10. * np.log(2.5))
             elif 0.25 <= y <= 10.:
                 return np.sin(10. * np.log(y))
             else:
                 return np.square(y - 10.) - np.sin(10. * np.log(10))
 
         return np.sum(np.vectorize(get_cases)(variables + 4.1112) + 1.0) / \
-               self.variable_num
+            self.variable_num
 
 
 # 54 - Class Exponential function
 class Exponential(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([1.] * self.variable_num)
@@ -1321,15 +1337,15 @@
                          'Separable': False,
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         return 1. - np.cos(2. * np.pi * np.sqrt(np.sum(np.square(variables)))) + \
-               0.1 * np.sqrt(np.sum(np.square(variables)))
+            0.1 * np.sqrt(np.sum(np.square(variables)))
 
 
 # 111 - Class Sargan function
 class Sargan(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([100.] * self.variable_num)
@@ -1636,16 +1652,15 @@
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         return 0.5 * (self.variable_num - 1.) + np.sum((np.square(
             np.sin(np.sqrt(np.square(variables[:-1]) + np.square(
-                variables[1:])))) - 0.5) / np.square(1. + 0.001 * (
-                variables[:-1] + variables[1:])))
+                variables[1:])))) - 0.5) / np.square(1. + 0.001 * (variables[:-1] + variables[1:])))
 
 
 # 136* - Class Schaffer N1 function [http://benchmarkfcns.xyz/benchmarkfcns/schaffern1fcn.html]
 class SchafferN1(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([100.] * self.variable_num)
@@ -1659,16 +1674,15 @@
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         return 0.5 * (self.variable_num - 1.) + np.sum((np.square(
             np.sin(np.square(np.square(variables[:-1]) + np.square(
-                variables[1:])))) - 0.5) / np.square(1. + 0.001 * (
-                variables[:-1] + variables[1:])))
+                variables[1:])))) - 0.5) / np.square(1. + 0.001 * (variables[:-1] + variables[1:])))
 
 
 # 136* - Class Schaffer N2 function [http://benchmarkfcns.xyz/benchmarkfcns/schaffern2fcn.html]
 class SchafferN2(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([100.] * self.variable_num)
@@ -1936,16 +1950,15 @@
                          'Separable': False,
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         return 1 + np.sum(8. * np.square(np.sin(7. * np.square(
-            variables - 0.9))) + 6. * np.square(np.sin(14. * np.square(
-            variables - 0.9))) + np.square(variables - 0.9))
+            variables - 0.9))) + 6. * np.square(np.sin(14. * np.square(variables - 0.9))) + np.square(variables - 0.9))
 
 
 # 165 - Class W-Wavy function
 class WWavy(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([np.pi] * self.variable_num)
@@ -1958,15 +1971,15 @@
                          'Separable': True,
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, k=10., *args):
         return 1. - np.sum(np.cos(k * variables) * np.exp(-0.5 * np.square(variables))) / \
-               self.variable_num
+            self.variable_num
 
 
 # 166 - Class Weierstrass function
 class Weierstrass(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([0.5] * self.variable_num)
@@ -2066,16 +2079,16 @@
                          'Separable': False,
                          'Scalable': True,
                          'Unimodal': True,
                          'Convex': False}
 
     def get_func_val(self, variables, m=5., beta=15., *args):
         return np.exp(-np.sum(np.power(variables / beta, 2. * m))) - 2. \
-               * np.exp(-np.sum(np.square(variables))) \
-               * np.prod(np.square(np.cos(variables)))
+            * np.exp(-np.sum(np.square(variables))) \
+            * np.prod(np.square(np.cos(variables)))
 
 
 # 172 - Class Xin-She Yang 4 function
 class XinSheYang4(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([10.] * self.variable_num)
@@ -2088,16 +2101,15 @@
                          'Separable': False,
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         return (np.sum(np.square(np.sin(variables))) - np.exp(-np.sum(
-            np.square(variables)))) * np.exp(-np.sum(np.square(
-            np.sin(np.abs(variables)))))
+            np.square(variables)))) * np.exp(-np.sum(np.square(np.sin(np.abs(variables)))))
 
 
 # 173 - Class Zakharov function
 class Zakharov(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
         self.max_search_range = np.array([10.] * self.variable_num)
@@ -2447,15 +2459,15 @@
                          'Separable': False,
                          'Scalable': True,
                          'Unimodal': False,
                          'Convex': False}
 
     def get_func_val(self, variables, *args):
         return - (1. / 30.) * np.exp(2. * np.abs(1. - np.linalg.norm(variables) / np.pi)) * \
-               np.prod(np.square(np.cos(variables)))
+            np.prod(np.square(np.cos(variables)))
 
 
 # Class CrownedCross function [http://infinity77.net/global_optimization/test_functions_nd_C.html#go_benchmark
 # .CrownedCross]
 class CrownedCross(BasicProblem):
     def __init__(self, variable_num):
         super().__init__(variable_num)
@@ -2779,16 +2791,48 @@
 
     def get_func_val(self, variables, k=6., *args):
         x_vals = np.square(variables[:-1]) + np.square(variables[1:]) \
                  + 0.5 * variables[1:] * variables[:-1]
         return -np.sum(np.exp(-x_vals / 8.) * np.cos(4. * np.sqrt(x_vals)))
 
 
+# %% LOAD CEC2005 PROBLEM
+if _cec_functions:
+
+    class CEC2005(BasicProblem):
+        def __init__(self, f_name, variable_num, **kwargs):
+            super().__init__(variable_num)
+            self.func_name = f_name
+            self.variable_num = variable_num
+
+            f_initializer = eval(f'cec2005.{self.func_name}')
+            self.f_function = f_initializer(self.variable_num, **kwargs)
+
+            if self.func_name in ['F7', 'F25']:
+                self.is_constrained = False
+                self.min_search_range = np.array([-5] * self.variable_num)
+                self.max_search_range = np.array([5] * self.variable_num)
+            else:
+                self.is_constrained = True
+                self.min_search_range = np.array(self.f_function.min_bounds)
+                self.max_search_range = np.array(self.f_function.max_bounds)
+
+        def get_func_val(self, variables):
+            return self.f_function(variables)
+
+        def get_formatted_problem(self):
+            return dict(
+                function=self.f_function,
+                boundaries=(self.min_search_range, self.max_search_range),
+                is_constrained=self.is_constrained
+            )
+
+
 # %% TOOLS TO HANDLE THE PROBLEMS
-def list_functions(rnp=True, fts=None, wrd='1'):
+def list_functions(rnp: bool = True, fts: list = None, wrd: str = '1'):
     """
     This function lists all available functions in screen. It could be formatted for copy and paste in a latex document.
     :param bool rnp: Optional.
         Flag (return-not-print). If True, the function delivers a list but not print, otherwise, print but not return.
         An example of the list returned when rnp = True is:
             [[function1_weight, function1_id, function1_name, function1_features],
              [function2_weight, function2_id, function2_name, function2_features],
@@ -2828,62 +2872,66 @@
         for x in feature_strings:
             print("{} & {} & {} \\\\".format(*x[1:]))
     else:
         # Return the list
         return functions_features
 
 
-def for_all(property, dimensions=2):
+def for_all(characteristic, dimensions=2):
     """
     Read a determined property or attribute for all the problems and return a list.
-    :param str property:
+    :param str characteristic:
         Property to read. Please, check the attributes from a given problem object.
     :param int dimensions: Optional
         Dimension to initialise all the problems.
     :return: list
     """
-    if property == 'features':
+    if characteristic == 'features':
         return list_functions(rnp=True, fts=None)
     else:
         info = dict()
         # Read all functions and request their optimum data
         for ii in range(len(__all__)):
             function_name = __all__[ii]
-            info[function_name] = eval('{}({}).{}'.format(function_name, dimensions, property))
+            info[function_name] = eval('{}({}).{}'.format(function_name, dimensions, characteristic))
 
         return info
 
-def filter_problems(features=['Differentiable', 'Separable', 'Unimodal'], intersection=True):
+
+def filter_problems(features: list = None, intersection: bool = True):
     """
     Return a list of function names that have the features listed
     :param list[str] features: 
         List of features.
     :param bool intersection: 
         True if the problems needs to have all the features, false if at least one is needed.
     :return: list        
     """
-    functions_features = list_functions(rnp=True, fts=features)    
+    features = ['Differentiable', 'Separable', 'Unimodal'] if features is None else features
+
+    functions_features = list_functions(rnp=True, fts=features)
     features_length = len(features)
-    
+
     funct_names = []
     for funct_name, values in functions_features.items():
         good_features = sum(map(int, list(values['Code'])))
         if intersection and good_features == features_length:
             # Problem has all the features
             funct_names.append(funct_name)
         if not intersection and good_features > 0:
             # Problem has at least one feature
             funct_names.append(funct_name)
     return funct_names
 
+
 def choose_problem(problem_name=None, num_dimensions=None):
     """
     Select a problem from __all__ using its string name and create its object for a given number of dimensions. If no
     problem is specified, it prints the full list of the available problems.
-    :param str problem_name: Identificator name of the problem.
+    :param str problem_name: Identification name of the problem.
     :param int num_dimensions: Number of dimensions.
     :return problem: The problem object ready to evaluate.
     """
     if problem_name and num_dimensions:
         if problem_name == '<random>':
             return eval('{}({})'.format(__all__[np.random.randint(0, len(__all__))], num_dimensions))
         else:
```

### Comparing `customhys-1.1.0/customhys/characterisation.py` & `customhys-1.1.1/customhys/characterisation.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/collections/automatic.txt` & `customhys-1.1.1/customhys/collections/automatic.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/collections/basicmetaheuristics.txt` & `customhys-1.1.1/customhys/collections/basicmetaheuristics.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/collections/default.txt` & `customhys-1.1.1/customhys/collections/default.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/collections/operators_collection.txt` & `customhys-1.1.1/customhys/collections/operators_collection.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/collections/operators_weights.json` & `customhys-1.1.1/customhys/collections/operators_weights.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/collections/short_collection.txt` & `customhys-1.1.1/customhys/collections/short_collection.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/exconf/basic_metaheuristic.json` & `customhys-1.1.1/customhys/exconf/basic_metaheuristic.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/exconf/brute_force.json` & `customhys-1.1.1/customhys/exconf/brute_force.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/exconf/demo_neural_network.json` & `customhys-1.1.1/customhys/exconf/demo_neural_network.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/exconf/long1.json` & `customhys-1.1.1/customhys/exconf/long1.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/exconf/short1.json` & `customhys-1.1.1/customhys/exconf/short1.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/exconf/short2.json` & `customhys-1.1.1/customhys/exconf/short2.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/experiment.py` & `customhys-1.1.1/customhys/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Created on Mon Sep 30 13:42:15 2019
 
 @author: Jorge Mario Cruz-Duarte (jcrvz.github.io), e-mail: jorge.cruz@tec.mx
 """
 
 from . import hyperheuristic as hyp
-from . import operators as Operators
+from . import operators as op
 from . import benchmark_func as bf
 from . import tools as tl
 import multiprocessing
 from os import path
 
 
 # %% PREDEFINED CONFIGURATIONS
@@ -84,17 +84,17 @@
             'heuristic_collection_file':    'default.txt',  # Heuristic space located in /collections/
             'weights_dataset_file':         None,           # Weights or probability distribution of heuristic space
             'use_parallel':                 True,           # Run the experiment using a pool of processors
             'parallel_pool_size':           None,           # Number of processors available, None = Default
             'auto_collection_num_vals':     5               # Number of values for creating an automatic collection
 
             **NOTE 1:** 'experiment_type': 'default' or another name mean hyper-heuristic.
-            **NOTE 2:** If the collection does not exist and it is not a reserved one ('default.txt', 'automatic.txt',
+            **NOTE 2:** If the collection does not exist, and it is not a reserved one ('default.txt', 'automatic.txt',
             'basicmetaheuristics.txt', 'test_collection'), then an automatic heuristic space is generated with
-            ``Operators.build_operators`` with 'auto_collection_num_vals' as ``num_vals`` and
+            ``op.build_operators`` with 'auto_collection_num_vals' as ``num_vals`` and
             'heuristic_collection_file' as ``filename``.
             **NOTE 3:** # 'weights_dataset_file' must be determined in a pre-processing step. For the 'default'
             heuristic space, it is provided 'operators_weights.json'.
 
         :param dict hh_config:
             Configuration dictionary related to the hyper-heuristic procedure. Keys and default values are listed as
             follows:
@@ -105,15 +105,15 @@
             'num_replicas':                     50,         # Number of replicas for each metaheuristic implemented
             'num_steps':                        100,        # * Number of steps that the hyper-heuristic performs
             'max_temperature':                  200,        # * Initial temperature for HH-Simulated Annealing
             'stagnation_percentage':            0.3,        # * Percentage of stagnation used by the hyper-heuristic
             'cooling_rate':                     0.05        # * Cooling rate for HH-Simulated Annealing
 
             **NOTE 4:** Keys with * correspond to those that are only used when ``exp_config['experiment_type']`` is
-            neither 'brute_force' or 'basic_metaheuristic'.
+            neither 'brute_force' nor 'basic_metaheuristic'.
 
         :param dict prob_config:
             Configuration dictionary related to the problems to solve. Keys and default values are listed as follows:
 
             'dimensions':       [2, 5, 10, 20, 30, 40, 50], # List of dimensions for the problem domains
             'functions':        bf.__all__,                 # List of function names of the optimisation problems
             'is_constrained':   True                        # True if the problem domain is hard constrained
@@ -126,15 +126,15 @@
         # Check if the heuristic collection exists
         if not path.isfile('./collections/' + self.exp_config['heuristic_collection_file']):
             # If the name is a reserved one. These files cannot be not created automatically
             if exp_config['heuristic_collection_file'] in ['default.txt', 'automatic.txt', 'basicmetaheuristics.txt',
                                                            'test_collection', 'short_collection.txt']:
                 raise ExperimentError('This collection name is reserved and cannot be created automatically!')
             else:
-                Operators.build_operators(Operators.obtain_operators(
+                op.build_operators(op.obtain_operators(
                     num_vals=exp_config['auto_collection_num_vals']),
                     file_name=exp_config['heuristic_collection_file'].split('.')[0])
                 self.exp_config['weights_dataset_file'] = None
 
         # Check if the weights dataset not exist or required
         if self.exp_config['weights_dataset_file'] and (
                 self.exp_config['experiment_type'] not in ['brute_force', 'basic_metaheuristics']):
@@ -358,15 +358,15 @@
 
         print(f"\nRunning {exp_filename.split('.')[0]}" + tail_message)
 
         # Create the experiment to runs
         exp = Experiment(config_file=exp_filename)
 
         # print("* Experiment configuration: \n", "-" * 30 + "\n", json.dumps(exp.prob_config, indent=2, default=str))
-        # print("* Hyper-heuristic configuration: \n", "-" * 30 + "\n", json.dumps(exp.hh_config, indent=2, default=str))
+        # print("* Hyper-heuristic configuration: \n", "-" * 30 + "\n",json.dumps(exp.hh_config, indent=2, default=str))
         # print("* Problem configuration: \n", "-" * 30 + "\n", json.dumps(exp.prob_config, indent=2, default=str))
 
         # Run the experiment et voilà
         exp.run()
 
         # After run, it preprocesses all the raw data
         print(f"\nPreprocessing {exp_filename.split('.')[0]}" + tail_message)
```

### Comparing `customhys-1.1.0/customhys/hyperheuristic.py` & `customhys-1.1.1/customhys/hyperheuristic.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,36 @@
 import json
 import numpy as np
 import random
 import scipy.stats as st
 from datetime import datetime
 from os import makedirs as _create_path
 from os.path import exists as _check_path
-from os import environ as _environ
-import tensorflow as tf
-
-from . import operators as Operators
+from . import operators as op
 from . import tools as jt
 from .metaheuristic import Metaheuristic
-from .machine_learning import DatasetSequences, ModelPredictor
 
-# Remove Tensorflow warnings
-_environ['TF_CPP_MIN_LOG_LEVEL'] = '3' 
-tf.get_logger().setLevel('ERROR')
+_using_tensorflow = False
+try:
+    import tensorflow as tf
+    from .machine_learning import DatasetSequences, ModelPredictor
+
+    from os import environ as _environ
+
+    # Remove Tensorflow warnings
+    _environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
+    tf.get_logger().setLevel('ERROR')
+    _using_tensorflow = True
+
+except ImportError as e:
+    import warnings as wa
+
+    message = "`Tensorflow` not found! Please, install it to use the machine_learning module"
+    wa.showwarning(message, ImportWarning, "hyperheuristic.py", 23)
+
 
 class Hyperheuristic:
     """
     This is the Hyperheuristic class, each object corresponds to a hyper-heuristic process implemented with a heuristic
     collection from Operators to build metaheuristics using the Metaheuristic module.
     """
 
@@ -78,34 +89,34 @@
             with open('collections/' + heuristic_space, 'r') as operators_file:
                 self.heuristic_space = [eval(line.rstrip('\n')) for line in operators_file]
         else:
             raise HyperheuristicError('Invalid heuristic_space')
 
         # Assign default values
         if not parameters:
-            parameters = dict(cardinality=3,                    # Max. numb. of SOs in MHs, lvl:1
-                              cardinality_min=1,                # Min. numb. of SOs in MHs, lvl:1
-                              num_iterations=100,               # Iterations a MH performs, lvl:1
-                              num_agents=30,                    # Agents in population,     lvl:1
-                              as_mh=False,                      # HH sequence as a MH?,     lvl:2
-                              num_replicas=50,                  # Replicas per each MH,     lvl:2
-                              num_steps=200,                    # Trials per HH step,       lvl:2
-                              stagnation_percentage=0.37,       # Stagnation percentage,    lvl:2
-                              max_temperature=1,                # Initial temperature (SA), lvl:2
-                              min_temperature=1e-6,             # Min temperature (SA),     lvl:2
-                              cooling_rate=1e-3,                # Cooling rate (SA),        lvl:2
-                              temperature_scheme='fast',        # Temperature updating (SA),lvl:2
+            parameters = dict(cardinality=3,  # Max. numb. of SOs in MHs, lvl:1
+                              cardinality_min=1,  # Min. numb. of SOs in MHs, lvl:1
+                              num_iterations=100,  # Iterations a MH performs, lvl:1
+                              num_agents=30,  # Agents in population,     lvl:1
+                              as_mh=False,  # HH sequence as a MH?,     lvl:2
+                              num_replicas=50,  # Replicas per each MH,     lvl:2
+                              num_steps=200,  # Trials per HH step,       lvl:2
+                              stagnation_percentage=0.37,  # Stagnation percentage,    lvl:2
+                              max_temperature=1,  # Initial temperature (SA), lvl:2
+                              min_temperature=1e-6,  # Min temperature (SA),     lvl:2
+                              cooling_rate=1e-3,  # Cooling rate (SA),        lvl:2
+                              temperature_scheme='fast',  # Temperature updating (SA),lvl:2
                               acceptance_scheme='exponential',  # Acceptance mode,          lvl:2
-                              allow_weight_matrix=True,         # Weight matrix,            lvl:2 
-                              trial_overflow=False,             # Trial overflow policy,    lvl:2
-                              learnt_dataset=None,              # If it is a learnt dataset related with the heuristic space
-                              repeat_operators=True,            # Allow repeating SOs inSeq,lvl:2
-                              verbose=True,                     # Verbose process,          lvl:2
-                              learning_portion=0.37,            # Percent of seqs to learn  lvl:2
-                              solver='static')                  # Indicate which solver use lvl:1
+                              allow_weight_matrix=True,  # Weight matrix,            lvl:2
+                              trial_overflow=False,  # Trial overflow policy,    lvl:2
+                              learnt_dataset=None,  # If it is a learnt dataset related with the heuristic space
+                              repeat_operators=True,  # Allow repeating SOs inSeq,lvl:2
+                              verbose=True,  # Verbose process,          lvl:2
+                              learning_portion=0.37,  # Percent of seqs to learn  lvl:2
+                              solver='static')  # Indicate which solver use lvl:1
 
         # Read the problem
         if problem:
             self.problem = problem
         else:
             raise HyperheuristicError('Problem must be provided')
 
@@ -123,15 +134,14 @@
         self.file_label = file_label
 
         self.max_cardinality = None
         self.min_cardinality = None
         self.num_iterations = None
         self.toggle_seq_as_meta(parameters['as_mh'])
 
-
     def toggle_seq_as_meta(self, as_mh=None):
         if as_mh is None:
             self.parameters['as_mh'] = not self.parameters['as_mh']
             self.toggle_seq_as_meta(self.parameters['as_mh'])
         else:
             if as_mh:
                 self.max_cardinality = self.parameters['cardinality']
@@ -343,15 +353,14 @@
                 encoded_neighbour = self._obtain_candidate_solution(current_cardinality)
 
             else:
                 raise HyperheuristicError(f'Invalid action = {action} to perform!')
         else:
             raise HyperheuristicError('Invalid type of current solution!')
 
-
         # Return the neighbour sequence
         return encoded_neighbour
 
     def _obtain_temperature(self, step_val, function='boltzmann'):
         """
         Return the updated temperature according to a defined scheme ``function``.
         :param int step_val:
@@ -421,21 +430,19 @@
         """
         General finalisation approach implemented for the methodology working as a hyper-heuristic. It mainly depends on
         `step` (current iteration number) and `stag_counter` (current stagnation iteration number). There are other
          variables that can be considered such as `temperature`. These additional variables must be args[0] < 0.0.
         """
         return (step >= self.parameters['num_steps']) or (
                 self.__stagnation_check(stag_counter) and not self.parameters['trial_overflow']) or \
-               (any([var < 0.0 for var in args]))
-
+            (any([var < 0.0 for var in args]))
 
     def get_operators(self, sequence):
         return [self.heuristic_space[index] for index in sequence]
 
-
     def solve(self, mode=None, save_steps=True):
         mode = mode if mode is not None else self.parameters["solver"]
 
         if mode == 'dynamic':
             return self._solve_dynamic(save_steps)
         elif mode == 'neural_network':
             return self._solve_neural_network(save_steps)
@@ -472,15 +479,15 @@
         # SELECTOR: Initialise the best solution and its performance
         best_solution = np.copy(current_solution)
         best_performance = current_performance
 
         # Save this historical register, step = 0
         if save_steps:
             _save_step(0, dict(encoded_solution=best_solution, performance=best_performance,
-                            details=current_details), self.file_label)
+                               details=current_details), self.file_label)
 
         # Step, stagnation counter and its maximum value
         step = 0
         stag_counter = 0
         action = None
         temperature = self.parameters['max_temperature']
 
@@ -635,34 +642,35 @@
                         which_matrix = 'entered'
 
                 # Pick randomly a simple heuristic
                 candidate_enc_so = self._obtain_candidate_solution(sol=1, operators_weights=possible_transitions)
 
                 # Prepare before evaluate the last search operator and apply it
                 candidate_search_operator = self.get_operators([candidate_enc_so[-1]])
-                perturbators, selectors = Operators.process_operators(candidate_search_operator)
+                perturbators, selectors = op.process_operators(candidate_search_operator)
 
                 mh.apply_search_operator(perturbators[0], selectors[0])
 
                 # Extract the population and fitness values, and their best values
                 current_fitness = np.copy(mh.pop.global_best_fitness)
                 current_position = np.copy(mh.pop.rescale_back(mh.pop.global_best_position))
 
                 # Print update
                 if self.parameters['verbose']:
                     print(
                         '{} :: Rep: {:3d}, Step: {:3d}, Trial: {:3d}, SO: {:30s}, currPerf: {:.2e}, candPerf: {:.2e} '
                         'which: {:10s}'.format(
                             self.file_label, rep + 1, step + 1, stag_counter,
-                            candidate_search_operator[0][0] + ' & ' + candidate_search_operator[0][2][:4],
+                                             candidate_search_operator[0][0] + ' & ' + candidate_search_operator[0][2][
+                                                                                       :4],
                             best_fitness[-1], current_fitness, which_matrix), end=' ')
 
                 # If the candidate solution is better or equal than the current best solution
                 if self._check_acceptance(current_fitness - best_fitness[-1], 'probabilistic', prob=0.2):
-                    
+
                     # Update the current sequence and its characteristics
                     current_sequence.append(candidate_enc_so[-1])
 
                     best_fitness.append(current_fitness)
                     best_position.append(current_position)
                     fitness_data.append(np.copy(mh.pop.fitness))
                     positions_data.append(np.copy(mh.pop.get_positions()))
@@ -741,18 +749,21 @@
         
         :returns list, list: fitness_per_repetition, sequence_per_repetition
         """
         sequence_per_repetition = list()
         fitness_per_repetition = list()
 
         # Neural network model that predicts operators
-        model = self._get_neural_network_predictor()        
+        model = self._get_neural_network_predictor()
         for rep in range(self.parameters['num_replicas']):
             # Metaheuristic
-            mh = Metaheuristic(self.problem, num_agents=self.parameters['num_agents'], num_iterations=self.num_iterations)
+            mh = Metaheuristic(
+                self.problem,
+                num_agents=self.parameters['num_agents'],
+                num_iterations=self.num_iterations)
 
             # Initialiser
             mh.apply_initialiser()
 
             # Extract the population and fitness values, and their best values
             current_fitness = np.copy(mh.pop.global_best_fitness)
             current_position = np.copy(mh.pop.rescale_back(mh.pop.global_best_position))
@@ -778,29 +789,30 @@
                 if stag_counter == 0:
                     operator_prediction = model.predict(current_sequence)
                     operators_weights = normalize_weights(operator_prediction)
 
                 # Select a simple heuristic and apply it
                 candidate_enc_so = self._obtain_candidate_solution(sol=1, operators_weights=operators_weights)
                 candidate_search_operator = self.get_operators([candidate_enc_so[-1]])
-                perturbators, selectors = Operators.process_operators(candidate_search_operator)
+                perturbators, selectors = op.process_operators(candidate_search_operator)
 
                 mh.apply_search_operator(perturbators[0], selectors[0])
 
                 # Extract population and fitness values
                 current_fitness = np.copy(mh.pop.global_best_fitness)
                 current_position = np.copy(mh.pop.rescale_back(mh.pop.global_best_position))
 
                 # Print update
                 if self.parameters['verbose']:
                     print(
                         '{} :: Neural Network, Rep: {:3d}, Step: {:3d}, Trial: {:3d}, SO: {:30s}, currPerf: {:.2e}, candPerf: {:.2e}, '
                         'csl: {:3d}'.format(
                             self.file_label, rep + 1, step + 1, stag_counter,
-                            candidate_search_operator[0][0] + ' & ' + candidate_search_operator[0][2][:4],
+                                             candidate_search_operator[0][0] + ' & ' + candidate_search_operator[0][2][
+                                                                                       :4],
                             best_fitness[-1], current_fitness, len(self.current_space)), end=' ')
 
                 # If the candidate solution is better or equal than the current best solution
                 if current_fitness < best_fitness[-1]:
                     # Update the current sequence and its characteristics
                     current_sequence.append(candidate_enc_so[-1])
 
@@ -836,15 +848,15 @@
             # Print the best one
             if self.parameters['verbose']:
                 print('\nBest fitness: {},\nBest position: {}'.format(current_fitness, current_position))
 
             # Update the repetition register
             sequence_per_repetition.append(np.double(current_sequence).astype(int).tolist())
             fitness_per_repetition.append(np.double(best_fitness).tolist())
-            
+
             # Save this historical register
             if save_steps:
                 _save_step(rep,
                            dict(encoded_solution=np.array(current_sequence),
                                 best_fitness=np.double(best_fitness),
                                 best_positions=np.double(best_position),
                                 details=dict(
@@ -858,42 +870,41 @@
 
     def _get_neural_network_predictor(self):
         # Prepare model params
         model_params = self.parameters['model_params']
         model_params['file_label'] = self.file_label
         model_params['num_steps'] = self.parameters['num_steps']
         model_params['num_operators'] = self.num_operators
-        
+
         # Initialize model        
         model = ModelPredictor(model_params)
 
         # Load pre-trained model
         if model_params['load_model'] and model.load():
             return model
-        
+
         # Get training data
         seqfitness_train, seqrep_train = self._get_sample_sequences(model_params['sample_params'])
-        dataset = DatasetSequences(seqrep_train, seqfitness_train, 
+        dataset = DatasetSequences(seqrep_train, seqfitness_train,
                                    num_operators=self.num_operators,
                                    fitness_to_weight=model_params.get('fitness_to_weight', None))
         X, y, sample_weight = dataset.obtain_dataset()
 
         # Fit model
-        model.fit(X, y, model_params['epochs'], 
+        model.fit(X, y, model_params['epochs'],
                   sample_weight=sample_weight,
                   verbose=self.parameters['verbose'],
                   early_stopping_params=model_params.get('early_stopping', None),
                   verbose_statistics=self.parameters['verbose_statistics'])
 
         # Save trained model
         if model_params['save_model']:
             model.save()
         return model
 
-
     def evaluate_candidate_solution(self, encoded_sequence):
         """
         Evaluate the current sequence as a hyper/meta-heuristic. This process is repeated ``parameters['num_replicas']``
         times and, then, the performance is determined. In the end, the method returns the performance value and the
         details for all the runs. These details are ``historical_data``, ``fitness_data``, ``position_data``, and
         ``fitness_stats``. The elements from the ``encoded_sequence`` must be in the range of the ``num_operators``.
         :param list encoded_sequence:
@@ -932,15 +943,14 @@
         # Determine a performance metric once finish the repetitions
         fitness_stats = self.get_statistics(fitness_data)
 
         # Return the performance value and the corresponding details
         return self.get_performance(fitness_stats), dict(
             historical=historical_data, fitness=fitness_data, positions=position_data, statistics=fitness_stats)
 
-
     def brute_force(self, save_steps=True):
         """
         This method performs a brute force procedure solving the problem via all the available search operators without
         integrating a high-level search method. So, each search operator is used as a 1-cardinality metaheuristic.
         Results are directly saved as json files.
         :return: None.
         """
@@ -961,15 +971,14 @@
                 }, self.file_label)
 
             # Print update
             if self.parameters['verbose']:
                 print('{} :: Operator {} of {}, Perf: {}'.format(
                     self.file_label, operator_id + 1, self.num_operators, operator_performance))
 
-
     def basic_metaheuristics(self, save_steps=True):
         """
         This method performs a brute force procedure solving the problem via all the predefined metaheuristics in
         './collections/basicmetaheuristics.txt'. Many of them are 1-cardinality MHs but other are 2-cardinality ones.
         This process does not require a high-level search method. Results are directly saved as json files.
         :return: None.
         """
@@ -993,15 +1002,14 @@
                 }, self.file_label)
 
             # Print update
             if self.parameters['verbose']:
                 print('{} :: BasicMH {} of {}, Perf: {}'.format(
                     self.file_label, operator_id + 1, self.num_operators, operator_performance))
 
-
     @staticmethod
     def get_performance(statistics):
         """
         Return the performance from fitness values obtained from running a metaheuristic several times. This method uses
         the Median and Interquartile Range values for such a purpose:
             performance = Med{fitness values} + IQR{fitness values}
         **Note:** If an alternative formula is needed, check the commented options.
@@ -1009,15 +1017,14 @@
         :return: The computed performance.
         """
         # return statistics['Med']                                                                  # Option 1
         # return statistics['Avg'] + statistics['Std']                                              # Option 2
         return statistics['Med'] + statistics['IQR']  # Option 3
         # return statistics['Avg'] + statistics['Std'] + statistics['Med'] + statistics['IQR']      # Option 4
 
-
     @staticmethod
     def get_statistics(raw_data):
         """
         Return statistics from all the fitness values found after running a metaheuristic several times. The oncoming
         statistics are ``nob`` (number of observations), ``Min`` (minimum), ``Max`` (maximum), ``Avg`` (average),
         ``Std`` (standard deviation), ``Skw`` (skewness), ``Kur`` (kurtosis), ``IQR`` (interquartile range),
         ``Med`` (median), and ``MAD`` (Median absolute deviation).
@@ -1035,15 +1042,14 @@
                     Std=np.std(raw_data),
                     Skw=dst.skewness,
                     Kur=dst.kurtosis,
                     IQR=st.iqr(raw_data),
                     Med=np.median(raw_data),
                     MAD=st.median_abs_deviation(raw_data))
 
-
     def _get_sample_sequences(self, sample_params):
         """
         Retrieve or generate sequences to use them as data train
         :param dict kw_sequences_params: Store the following values:
             :param bool retrieve_sequences: True if would retrieve stored sequences,
                 False if it would generate sequences for the given problem.
             :param int limit_seqs: The maximum number of sequences to be consider.
@@ -1056,24 +1062,24 @@
         if sample_params['retrieve_sequences']:
             filters = dict({'collection': self.heuristic_space_label,
                             'limit_seqs': sample_params.get('limit_seqs', 100),
                             'dimensions': f'-{self.problem["dimensions"]}D-',
                             'population': f'-{self.parameters["num_agents"]}pop-',
                             'func_name': self.problem['func_name']})
             seqfitness, seqrep = _get_stored_sample_sequences(filters)
-        else:        
+        else:
             # Generate sequences from dynamic solver
             prev_num_replicas = self.parameters['num_replicas']
             prev_learning_portion = self.parameters['learning_portion']
             self.parameters['num_replicas'] = sample_params.get('limit_seqs', 100)
             self.parameters['learning_portion'] = sample_params.get('random', 0.37)
             seqfitness, seqrep, _ = self._solve_dynamic(save_steps=False)
             self.parameters['num_replicas'] = prev_num_replicas
             self.parameters['learning_portion'] = prev_learning_portion
-        
+
         # Filter sequences with best performance
         if 'filter' in sample_params:
             seqfitness_last = [sequence[-1] for sequence in seqfitness]
             if sample_params['filter'] == 'first_quartile':
                 top_value = np.quantile(seqfitness_last, 0.25)
             else:
                 raise HyperheuristicError(f'"{sample_params["filter"]}" is not supported yet!')
@@ -1085,30 +1091,29 @@
         if len(seqfitness) == 0 or len(seqrep) == 0:
             raise HyperheuristicError('There is no sample of sequences for training')
 
         # Store sequences if requested
         if sample_params['store_sequences']:
             # Order sequences according to its fitness
             indices_order = list(range(len(seqfitness)))
-            indices_order.sort(key = lambda idx: seqfitness[idx][-1])
+            indices_order.sort(key=lambda idx: seqfitness[idx][-1])
 
             sequences_to_save = dict()
             for idx in indices_order:
                 sequences_to_save[idx] = (seqfitness[idx], seqrep[idx])
-                
+
             # Store sequence without identificator of experiment : '-'.join(self.file_label.split('-')[:2]
-            sequences_name = '-'.join([self.problem['func_name'], 
-                                      f'{self.problem["dimensions"]}D', 
-                                      f'{self.parameters["num_agents"]}pop',
-                                      self.heuristic_space_label,
-                                      self.file_label])
+            sequences_name = '-'.join([self.problem['func_name'],
+                                       f'{self.problem["dimensions"]}D',
+                                       f'{self.parameters["num_agents"]}pop',
+                                       self.heuristic_space_label,
+                                       self.file_label])
             _save_sequences(sequences_name, sequences_to_save)
-    
-        return seqfitness, seqrep
 
+        return seqfitness, seqrep
 
     def _update_weights(self, sequences=None):
         if (self.weights is None) or (len(sequences) < int(self.parameters['num_replicas'] *
                                                            self.parameters['learning_portion']
                                                            ) if sequences is not None else False):
             # Create the weights array using a uniform distribution
             self.weights = np.ones(self.num_operators) / self.num_operators
@@ -1127,14 +1132,15 @@
                 if np.sum(temp_hist) > 0.0:
                     current_hist.append(np.ndarray.tolist(temp_hist / np.sum(temp_hist)))
                 else:
                     current_hist.append(np.ndarray.tolist(np.ones(self.num_operators) / self.num_operators))
 
             self.transition_matrix = np.array(current_hist)
 
+
 # %% ADDITIONAL TOOLS
 
 def _save_step(step_number, variable_to_save, prefix=''):
     """
     This method saves all the information corresponding to specific step.
     :param int step_number:
         Value of the current step in the hyper-heuristic procedure. If it is not a hyper-heuristic, this integer
@@ -1174,44 +1180,45 @@
     :return list, list: Return the list of sequences with their respective fitness. 
     """
     if not _check_path(folder_name):
         return [], []
 
     # Filter stored sequences
     essential_attributes = ['func_name', 'dimensions', 'population', 'collection']
+
     def is_valid_file(file_name):
         # Verify that its a valid problem
         return all(filters[attribute] in file_name
                    for attribute in essential_attributes)
 
-    files_in_folder = jt.read_subfolders(folder_name)
+    files_in_folder = jt.read_folder_files(folder_name)
     sequences_files = [file_name for file_name in files_in_folder if is_valid_file(file_name)]
 
     # Limit the number of sequences retreived from a problem
     limit_seqs = filters['limit_seqs']
     sequences_per_problem = dict()
 
     # Extract sequences from stored sequences files
     seqfitness, seqrep = [], []
     for sequences_file in sequences_files:
         problem_name = sequences_file[:sequences_file.rfind('.')].split('-')[0]
         if problem_name not in sequences_per_problem:
             # Initialise counter per problem
             sequences_per_problem[problem_name] = 0
-        
+
         # Check limit before read the json file
         if sequences_per_problem[problem_name] == limit_seqs:
             continue
 
         sequences_json = jt.read_json(folder_name + sequences_file)
         for fitness, sequence in sequences_json.values():
             # Check limit before append sequence
             if sequences_per_problem[problem_name] == limit_seqs:
                 break
-            
+
             # Append sequence
             seqfitness.append(fitness)
             seqrep.append(sequence)
             sequences_per_problem[problem_name] += 1
     return seqfitness, seqrep
 
 
@@ -1220,19 +1227,19 @@
     Save encoded sequences and its fitness to use them later to train ML models. 
     :param str file_name: Name of the file where the sequences will be stored.
     :param dict sequences_to_save: Sequences that will be stored.
     :return: None.
     """
     # Define the folder name
     folder_name = 'data_files/sequences/'
-    
+
     # Check if this path exists
     if not _check_path(folder_name):
         _create_path(folder_name)
-    
+
     # Overwrite or create file to store the sequences along its respective fitness
     with open(folder_name + f'{file_name}.json', 'w') as json_file:
         json.dump(sequences_to_save, json_file, cls=jt.NumpyEncoder)
 
 
 class HyperheuristicError(Exception):
     """
```

### Comparing `customhys-1.1.0/customhys/machine_learning.py` & `customhys-1.1.1/customhys/machine_learning.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/metaheuristic.py` & `customhys-1.1.1/customhys/metaheuristic.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 __operators__ = Operators.__all__
 __selectors__ = ['greedy', 'probabilistic', 'metropolis', 'all', 'none']
 
 
 class Metaheuristic:
     """
         This is the Metaheuristic class, each object corresponds to a metaheuristic implemented with a sequence of
-        search operators from Operators, and it is based on a population from Population.
+        search operators from op, and it is based on a population from Population.
     """
     def __init__(self, problem, search_operators=None, num_agents=30, num_iterations=100, initial_scheme='random'):
         """
         Create a population-based metaheuristic by employing different simple search operators.
 
         :param dict problem:
             This is a dictionary containing the 'function' that maps a 1-by-D array of real values to a real value,
```

### Comparing `customhys-1.1.0/customhys/operators.py` & `customhys-1.1.1/customhys/operators.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/population.py` & `customhys-1.1.1/customhys/population.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/customhys/tools.py` & `customhys-1.1.1/customhys/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,30 @@
 
                 # Rename the copied folder with prefix '.to_delete-'
                 call(['mv', main_folder + folders_with_date[index],
                       main_folder + '.to_delete-' + folders_with_date[index]])
                 print("Merged '{}' into '{}'!".format(folders_with_date[index], folders_with_date[indices[0]]))
 
 
-def read_subfolders(foldername):
+def read_folder_files(folder_name):
     """
     Return a list of all subfolders contained in a folder, ignoring all those starting with '.' (hidden ones).
-    :param str foldername: Name of the main folder.
+    :param str folder_name: Name of the main folder.
     :return: list.
     """
-    return [element for element in os.listdir(foldername) if not element.startswith('.')]
+    return [element for element in os.listdir(folder_name) if not element.startswith('.')]
+
+
+# def process_results(target_folder: str = None, output_name: str = None):
+#     if target_folder is None:
+#         raise FileNotFoundError("target_folder must be provided")
+#
+#     output_name = target_folder.split('/')[-1] if output_name is None else target_folder
+#
+#     folder_files = read_folder_files(target_folder)
 
 
 def preprocess_files(main_folder='data_files/raw/', kind='brute_force', only_laststep=True,
                      output_name='processed_data', experiment=''):
     """
     Return data from results saved in the main folder. This method save the summary file in json format. Take in account
     that ``output_name = 'brute_force'`` has a special behaviour due to each json file stored in sub-folders correspond
@@ -168,15 +177,15 @@
         Label of the experiment. This parameter help to filter the results if multiple experiments are performed at the
         same time. Default is an empty string, which would process all the results from the given folder.
 
     :return: dict.
     """
     # TODO: Revise this method to enhance its performance.
     # Get folders and exclude hidden ones
-    raw_folders = filter(lambda name: len(name.split('-')) >= 2, read_subfolders(main_folder))
+    raw_folders = filter(lambda name: len(name.split('-')) >= 2, read_folder_files(main_folder))
 
     # Sort subfolder names by problem name & dimensions
     subfolder_names_raw = sorted(raw_folders, key=lambda x: int(x.split('-')[1].strip('D')))
 
     if len(experiment) > 0:
         subfolder_names = filter(lambda name: len(name.split('-')) >= 3 and '-'.join(name.split('-')[2:]) == experiment,
                                  subfolder_names_raw)
@@ -276,15 +285,15 @@
             with open(temporal_full_path + '/' + file_name, 'r') as json_file:
                 temporal_data = json.load(json_file)
 
             if kind in ['dynamic_metaheuristic', 'neural_network']:
                 file_data[label_operator].append(operator_id)
                 file_data['encoded_solution'].append(temporal_data['encoded_solution'])
                 file_data['hist_fitness'].append(temporal_data['best_fitness'])
-                
+
             elif kind in ['unknown', 'dynamic_transfer_learning']:
                 if len(file_data) != 0:
                     keys_to_use = list(file_data.keys())
                 else:
                     keys_to_use = list(temporal_data.keys())
 
                 if only_laststep and operator_id == last_step:
@@ -401,58 +410,70 @@
     with open(data_file, 'r') as json_file:
         data = json.load(json_file)
 
     # Return only the data variable
     return data
 
 
-def merge_json(data_folder, list_of_fields=None):
-    final_file_path = data_folder + '/' + data_folder.split('/')[-1] + '.csv'
-    file_names = [element for element in os.listdir(data_folder) if ((not element.startswith('.'))
-                                                                     and element.endswith('.json'))]
+def merge_json(data_folder: str, list_of_fields: list = None, save_file: bool = True) -> None:
+    raw_file_names = [element for element in os.listdir(data_folder) if (
+            (not element.startswith('.')) and element.endswith('.json'))]
+
+    file_names = sorted(raw_file_names, key=lambda x: int(x.split('-')[0]))
 
     temporal_pretable = list()
 
     for file_name in tqdm(file_names):
         temporal_data = read_json(data_folder + '/' + file_name)
 
         if (len(temporal_pretable) == 0) and (not list_of_fields):
             list_of_fields = list(temporal_data.keys())
 
-        temporal_pretable.append({field: temporal_data[field] for field in list_of_fields})
-
-    _ = pd.DataFrame(temporal_pretable).to_csv(final_file_path)
-    print('Merged file saved: {}'.format(final_file_path))
-
+        temporal_pretable.append(
+            {**{"file_name": file_name, "step": int(file_name.split('-')[0])},
+             **{field: temporal_data[field] for field in list_of_fields}}
+        )
+
+    # df = pd.DataFrame(temporal_pretable)
+
+    if save_file:
+        path = data_folder.split('/')
+        final_file_path = "/".join(path[:-1] + [path[-1]])
+        save_json(temporal_pretable, final_file_path)
+
+        # df.to_csv(final_file_path + '.csv')
+        # print('Merged file saved: {}'.format(final_file_path + '.csv'))
+        print('Merged file saved: {}'.format(final_file_path + '.json'))
 
 class NumpyEncoder(json.JSONEncoder):
     """
     Numpy encoder
     """
+
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         return json.JSONEncoder.default(self, obj)
 
 
 if __name__ == '__main__':
     # Import module for calling this code from command-line
     import argparse
-    
+
     parser = argparse.ArgumentParser(
         description='Process results for a given experiment to make comparisons and visualisation with other experiments.'
     )
-    parser.add_argument('experiment', 
-                        metavar='experiment_filename', 
+    parser.add_argument('experiment',
+                        metavar='experiment_filename',
                         type=str, nargs=1,
                         help='Name of finished experiment')
-    parser.add_argument('kind', 
-                        metavar='kind', 
+    parser.add_argument('kind',
+                        metavar='kind',
                         type=str, nargs=1,
                         help='Kind of finished experiment')
-    
+
     exp_name = parser.parse_args().experiment[0]
     kind = parser.parse_args().kind[0]
-    preprocess_files(main_folder='data_files/raw-'+exp_name, 
-                     kind=kind, 
-                     experiment=exp_name, 
+    preprocess_files(main_folder='data_files/raw-' + exp_name,
+                     kind=kind,
+                     experiment=exp_name,
                      output_name=exp_name)
```

### Comparing `customhys-1.1.0/customhys.egg-info/PKG-INFO` & `customhys-1.1.1/customhys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: customhys
-Version: 1.1.0
+Version: 1.1.1
 Summary: This framework provides tools for solving, but not limited to, continuous optimisation problems using a hyper-heuristic approach for customising metaheuristics. 
 Home-page: https://github.com/jcrvz/customhys
 Author: Jorge Mario Cruz-Duarte
 Author-email: jorge.cruz@tec.mx
 License: MIT License
 Keywords: metaheuristics,hyper-heuristic,optimization,automatic design,global optimization,evolutionary computation,bio-inspired,algorithm design
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: ML
 License-File: LICENSE
 
 # customhys
 
 <div>
     <img align="left" alt="Module Dependency Diagram" src="https://raw.githubusercontent.com/jcrvz/customhys/master/docfiles/chm_logo.png" title="Customhys logo" width="25%"/>
 </div>
```

### Comparing `customhys-1.1.0/customhys.egg-info/SOURCES.txt` & `customhys-1.1.1/customhys.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 customhys/population.py
 customhys/test_solvers.py
 customhys/tools.py
 customhys/visualisation.py
 customhys.egg-info/PKG-INFO
 customhys.egg-info/SOURCES.txt
 customhys.egg-info/dependency_links.txt
+customhys.egg-info/requires.txt
 customhys.egg-info/top_level.txt
 customhys/collections/automatic.txt
 customhys/collections/basicmetaheuristics.txt
 customhys/collections/default.txt
 customhys/collections/operators_collection.txt
 customhys/collections/operators_weights.json
 customhys/collections/short_collection.txt
```

### Comparing `customhys-1.1.0/docfiles/SearchOperators_CEC.pdf` & `customhys-1.1.1/docfiles/SearchOperators_CEC.pdf`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/cas_logo.png` & `customhys-1.1.1/docfiles/cas_logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/chm_logo.png` & `customhys-1.1.1/docfiles/chm_logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/conacyt-logo.png` & `customhys-1.1.1/docfiles/conacyt-logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/dependency_diagram.png` & `customhys-1.1.1/docfiles/dependency_diagram.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/heuristics.png` & `customhys-1.1.1/docfiles/heuristics.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/logoTEC_full.png` & `customhys-1.1.1/docfiles/logoTEC_full.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/methodology_cec_a.png` & `customhys-1.1.1/docfiles/methodology_cec_a.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/methodology_cec_b.png` & `customhys-1.1.1/docfiles/methodology_cec_b.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/docfiles/operators.png` & `customhys-1.1.1/docfiles/operators.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.0/setup.py` & `customhys-1.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,37 @@
 import pathlib
 
 # The text of the README file
 README = (pathlib.Path(__file__).parent / 'README.md').read_text()
 
 setuptools.setup(
     name='customhys',
-    version='1.1.0',
+    version='1.1.1',
     packages=setuptools.find_packages(),
     url='https://github.com/jcrvz/customhys',
     license='MIT License',
     author='Jorge Mario Cruz-Duarte',
     author_email='jorge.cruz@tec.mx',
     description='This framework provides tools for solving, but not limited to, continuous optimisation problems '
                 'using a hyper-heuristic approach for customising metaheuristics. ',
     long_description_content_type='text/markdown',
     long_description=README,
     keywords=['metaheuristics', 'hyper-heuristic', 'optimization', 'automatic design', 'global optimization',
               'evolutionary computation', 'bio-inspired', 'algorithm design'],
     python_requires=">=3.8",
+    install_requires=[
+        "numpy>=1.22.0",
+        "scipy>=1.5.0",
+        "matplotlib>=3.2.2",
+        "tqdm>=4.47.0",
+        "scikit-learn>=1.2.2",
+        "pandas>=1.5.3",
+    ],
+    extras_require={
+        "ML": [
+            "tensorflow>=2.8.0; sys_platform != 'darwin'",
+            "tensorflow-macos>=2.11.0; sys_platform == 'darwin'",
+            "tensorflow-metal>=0.7.1; sys_platform == 'darwin'",
+        ]
+    },
     include_package_data=True
 )
```

