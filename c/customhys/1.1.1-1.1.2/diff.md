# Comparing `tmp/customhys-1.1.1.tar.gz` & `tmp/customhys-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customhys-1.1.1.tar", last modified: Fri Apr 14 23:24:26 2023, max compression
+gzip compressed data, was "customhys-1.1.2.tar", last modified: Sat Apr 15 01:20:47 2023, max compression
```

## Comparing `customhys-1.1.1.tar` & `customhys-1.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.760408 customhys-1.1.1/
--rw-r--r--   0 jcrvz      (501) staff       (20)     1080 2023-03-16 23:22:43.000000 customhys-1.1.1/LICENSE
--rw-r--r--   0 jcrvz      (501) staff       (20)      122 2023-03-16 23:22:43.000000 customhys-1.1.1/MANIFEST.in
--rw-r--r--   0 jcrvz      (501) staff       (20)    11537 2023-04-14 23:24:26.760568 customhys-1.1.1/PKG-INFO
--rw-r--r--   0 jcrvz      (501) staff       (20)    10931 2023-03-16 23:22:43.000000 customhys-1.1.1/README.md
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.740152 customhys-1.1.1/customhys/
--rw-r--r--   0 jcrvz      (501) staff       (20)      218 2023-03-22 04:12:13.000000 customhys-1.1.1/customhys/__init__.py
--rw-r--r--   0 jcrvz      (501) staff       (20)   126445 2023-03-24 05:56:36.000000 customhys-1.1.1/customhys/benchmark_func.py
--rw-r--r--   0 jcrvz      (501) staff       (20)     8163 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/characterisation.py
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.745262 customhys-1.1.1/customhys/collections/
--rw-r--r--   0 jcrvz      (501) staff       (20)  1265347 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/automatic.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)     8469 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/basicmetaheuristics.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)    21255 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/default.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)    92837 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/operators_collection.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)   255391 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/operators_weights.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     2842 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/collections/short_collection.txt
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.746724 customhys-1.1.1/customhys/exconf/
--rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/basic_metaheuristic.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1717 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/brute_force.json
--rw-r--r--   0 jcrvz      (501) staff       (20)      299 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/demo.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1147 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/demo_neural_network.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/long1.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1763 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/short1.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1713 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/exconf/short2.json
--rw-r--r--   0 jcrvz      (501) staff       (20)    18465 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/experiment.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    62676 2023-03-21 16:52:55.000000 customhys-1.1.1/customhys/hyperheuristic.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    13900 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/machine_learning.py
--rw-r--r--   0 jcrvz      (501) staff       (20)     7304 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/metaheuristic.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    45073 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/operators.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    15755 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/population.py
--rw-r--r--   0 jcrvz      (501) staff       (20)      483 2023-03-16 23:22:43.000000 customhys-1.1.1/customhys/test_solvers.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    19272 2023-03-22 04:12:13.000000 customhys-1.1.1/customhys/tools.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    11413 2023-03-22 04:12:13.000000 customhys-1.1.1/customhys/visualisation.py
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.740876 customhys-1.1.1/customhys.egg-info/
--rw-r--r--   0 jcrvz      (501) staff       (20)    11537 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/PKG-INFO
--rw-r--r--   0 jcrvz      (501) staff       (20)     1287 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/SOURCES.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)        1 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/dependency_links.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)      227 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/requires.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)       10 2023-04-14 23:24:26.000000 customhys-1.1.1/customhys.egg-info/top_level.txt
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-14 23:24:26.758082 customhys-1.1.1/docfiles/
--rw-r--r--   0 jcrvz      (501) staff       (20)   905189 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/SearchOperators_CEC.pdf
--rw-r--r--   0 jcrvz      (501) staff       (20)    16429 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/cas_logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)    42755 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/chm_logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)    28786 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/conacyt-logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   209268 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/dependency_diagram.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   743430 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/heuristics.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   137732 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/logoTEC_full.png
--rw-r--r--   0 jcrvz      (501) staff       (20)  1614825 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/methodology_cec_a.png
--rw-r--r--   0 jcrvz      (501) staff       (20)  2074059 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/methodology_cec_b.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   452031 2023-03-16 23:22:43.000000 customhys-1.1.1/docfiles/operators.png
--rw-r--r--   0 jcrvz      (501) staff       (20)       86 2023-03-16 23:22:43.000000 customhys-1.1.1/pyproject.toml
--rw-r--r--   0 jcrvz      (501) staff       (20)       81 2023-04-14 23:24:26.760892 customhys-1.1.1/setup.cfg
--rw-r--r--   0 jcrvz      (501) staff       (20)     1345 2023-03-22 04:12:13.000000 customhys-1.1.1/setup.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-15 01:20:47.228020 customhys-1.1.2/
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1080 2023-03-16 23:22:43.000000 customhys-1.1.2/LICENSE
+-rw-r--r--   0 jcrvz      (501) staff       (20)      122 2023-03-16 23:22:43.000000 customhys-1.1.2/MANIFEST.in
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11537 2023-04-15 01:20:47.228221 customhys-1.1.2/PKG-INFO
+-rw-r--r--   0 jcrvz      (501) staff       (20)    10931 2023-03-16 23:22:43.000000 customhys-1.1.2/README.md
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-15 01:20:47.209881 customhys-1.1.2/customhys/
+-rw-r--r--   0 jcrvz      (501) staff       (20)      218 2023-04-15 01:18:11.000000 customhys-1.1.2/customhys/__init__.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)   126494 2023-04-15 01:20:04.000000 customhys-1.1.2/customhys/benchmark_func.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)     8163 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/characterisation.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-15 01:20:47.214803 customhys-1.1.2/customhys/collections/
+-rw-r--r--   0 jcrvz      (501) staff       (20)  1265347 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/collections/automatic.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)     8469 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/collections/basicmetaheuristics.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)    21255 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/collections/default.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)    92837 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/collections/operators_collection.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)   255391 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/collections/operators_weights.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     2842 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/collections/short_collection.txt
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-15 01:20:47.216013 customhys-1.1.2/customhys/exconf/
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/exconf/basic_metaheuristic.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1717 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/exconf/brute_force.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)      299 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/exconf/demo.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1147 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/exconf/demo_neural_network.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/exconf/long1.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1763 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/exconf/short1.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1713 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/exconf/short2.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)    18465 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/experiment.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    62676 2023-03-21 16:52:55.000000 customhys-1.1.2/customhys/hyperheuristic.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    13900 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/machine_learning.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)     7304 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/metaheuristic.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    45073 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/operators.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    15755 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/population.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)      483 2023-03-16 23:22:43.000000 customhys-1.1.2/customhys/test_solvers.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    19272 2023-03-22 04:12:13.000000 customhys-1.1.2/customhys/tools.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11413 2023-03-22 04:12:13.000000 customhys-1.1.2/customhys/visualisation.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-15 01:20:47.210438 customhys-1.1.2/customhys.egg-info/
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11537 2023-04-15 01:20:47.000000 customhys-1.1.2/customhys.egg-info/PKG-INFO
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1287 2023-04-15 01:20:47.000000 customhys-1.1.2/customhys.egg-info/SOURCES.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)        1 2023-04-15 01:20:47.000000 customhys-1.1.2/customhys.egg-info/dependency_links.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)      227 2023-04-15 01:20:47.000000 customhys-1.1.2/customhys.egg-info/requires.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)       10 2023-04-15 01:20:47.000000 customhys-1.1.2/customhys.egg-info/top_level.txt
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-04-15 01:20:47.226801 customhys-1.1.2/docfiles/
+-rw-r--r--   0 jcrvz      (501) staff       (20)   905189 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/SearchOperators_CEC.pdf
+-rw-r--r--   0 jcrvz      (501) staff       (20)    16429 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/cas_logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)    42755 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/chm_logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)    28786 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/conacyt-logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   209268 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/dependency_diagram.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   743430 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/heuristics.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   137732 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/logoTEC_full.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)  1614825 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/methodology_cec_a.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)  2074059 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/methodology_cec_b.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   452031 2023-03-16 23:22:43.000000 customhys-1.1.2/docfiles/operators.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)       86 2023-03-16 23:22:43.000000 customhys-1.1.2/pyproject.toml
+-rw-r--r--   0 jcrvz      (501) staff       (20)       81 2023-04-15 01:20:47.228571 customhys-1.1.2/setup.cfg
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1345 2023-04-15 01:16:29.000000 customhys-1.1.2/setup.py
```

### Comparing `customhys-1.1.1/LICENSE` & `customhys-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/PKG-INFO` & `customhys-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customhys
-Version: 1.1.1
+Version: 1.1.2
 Summary: This framework provides tools for solving, but not limited to, continuous optimisation problems using a hyper-heuristic approach for customising metaheuristics. 
 Home-page: https://github.com/jcrvz/customhys
 Author: Jorge Mario Cruz-Duarte
 Author-email: jorge.cruz@tec.mx
 License: MIT License
 Keywords: metaheuristics,hyper-heuristic,optimization,automatic design,global optimization,evolutionary computation,bio-inspired,algorithm design
 Requires-Python: >=3.8
```

### Comparing `customhys-1.1.1/README.md` & `customhys-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/benchmark_func.py` & `customhys-1.1.2/customhys/benchmark_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
            'SchafferN4', 'SchafferN6', 'Schubert', 'Schubert3', 'Schubert4', 'SchumerSteiglitz', 'Schwefel',
            'Schwefel12', 'Schwefel204', 'Schwefel220', 'Schwefel221', 'Schwefel222', 'Schwefel223', 'Schwefel225',
            'Schwefel226', 'Sphere', 'Step', 'Step2', 'Step3', 'StepInt', 'Stochastic', 'StrechedVSineWave',
            'StyblinskiTang', 'SumSquares', 'Trid', 'Trigonometric1', 'Trigonometric2', 'TypeI', 'TypeII', 'Vincent',
            'WWavy', 'Weierstrass', 'Whitley', 'XinSheYang1', 'XinSheYang2', 'XinSheYang3', 'XinSheYang4', 'YaoLiu09',
            'Zakharov', 'ZeroSum']
 
+if _cec_functions:
+    __all__.append("CEC2005")
 
 # %% BASIC FUNCTION CLASS
 class BasicProblem:
     """
     This is the basic class for a generic optimisation problem.
     """
```

### Comparing `customhys-1.1.1/customhys/characterisation.py` & `customhys-1.1.2/customhys/characterisation.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/collections/automatic.txt` & `customhys-1.1.2/customhys/collections/automatic.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/collections/basicmetaheuristics.txt` & `customhys-1.1.2/customhys/collections/basicmetaheuristics.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/collections/default.txt` & `customhys-1.1.2/customhys/collections/default.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/collections/operators_collection.txt` & `customhys-1.1.2/customhys/collections/operators_collection.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/collections/operators_weights.json` & `customhys-1.1.2/customhys/collections/operators_weights.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/collections/short_collection.txt` & `customhys-1.1.2/customhys/collections/short_collection.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/exconf/basic_metaheuristic.json` & `customhys-1.1.2/customhys/exconf/basic_metaheuristic.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/exconf/brute_force.json` & `customhys-1.1.2/customhys/exconf/brute_force.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/exconf/demo_neural_network.json` & `customhys-1.1.2/customhys/exconf/demo_neural_network.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/exconf/long1.json` & `customhys-1.1.2/customhys/exconf/long1.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/exconf/short1.json` & `customhys-1.1.2/customhys/exconf/short1.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/exconf/short2.json` & `customhys-1.1.2/customhys/exconf/short2.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/experiment.py` & `customhys-1.1.2/customhys/experiment.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/hyperheuristic.py` & `customhys-1.1.2/customhys/hyperheuristic.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/machine_learning.py` & `customhys-1.1.2/customhys/machine_learning.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/metaheuristic.py` & `customhys-1.1.2/customhys/metaheuristic.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/operators.py` & `customhys-1.1.2/customhys/operators.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/population.py` & `customhys-1.1.2/customhys/population.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/tools.py` & `customhys-1.1.2/customhys/tools.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys/visualisation.py` & `customhys-1.1.2/customhys/visualisation.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/customhys.egg-info/PKG-INFO` & `customhys-1.1.2/customhys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customhys
-Version: 1.1.1
+Version: 1.1.2
 Summary: This framework provides tools for solving, but not limited to, continuous optimisation problems using a hyper-heuristic approach for customising metaheuristics. 
 Home-page: https://github.com/jcrvz/customhys
 Author: Jorge Mario Cruz-Duarte
 Author-email: jorge.cruz@tec.mx
 License: MIT License
 Keywords: metaheuristics,hyper-heuristic,optimization,automatic design,global optimization,evolutionary computation,bio-inspired,algorithm design
 Requires-Python: >=3.8
```

### Comparing `customhys-1.1.1/customhys.egg-info/SOURCES.txt` & `customhys-1.1.2/customhys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/SearchOperators_CEC.pdf` & `customhys-1.1.2/docfiles/SearchOperators_CEC.pdf`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/cas_logo.png` & `customhys-1.1.2/docfiles/cas_logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/chm_logo.png` & `customhys-1.1.2/docfiles/chm_logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/conacyt-logo.png` & `customhys-1.1.2/docfiles/conacyt-logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/dependency_diagram.png` & `customhys-1.1.2/docfiles/dependency_diagram.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/heuristics.png` & `customhys-1.1.2/docfiles/heuristics.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/logoTEC_full.png` & `customhys-1.1.2/docfiles/logoTEC_full.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/methodology_cec_a.png` & `customhys-1.1.2/docfiles/methodology_cec_a.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/methodology_cec_b.png` & `customhys-1.1.2/docfiles/methodology_cec_b.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/docfiles/operators.png` & `customhys-1.1.2/docfiles/operators.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.1/setup.py` & `customhys-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 # The text of the README file
 README = (pathlib.Path(__file__).parent / 'README.md').read_text()
 
 setuptools.setup(
     name='customhys',
-    version='1.1.1',
+    version='1.1.2',
     packages=setuptools.find_packages(),
     url='https://github.com/jcrvz/customhys',
     license='MIT License',
     author='Jorge Mario Cruz-Duarte',
     author_email='jorge.cruz@tec.mx',
     description='This framework provides tools for solving, but not limited to, continuous optimisation problems '
                 'using a hyper-heuristic approach for customising metaheuristics. ',
```

