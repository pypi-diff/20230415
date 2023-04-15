# Comparing `tmp/cvxpylayers-0.1.5.tar.gz` & `tmp/cvxpylayers-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cvxpylayers-0.1.5.tar", last modified: Thu Apr 15 20:12:55 2021, max compression
+gzip compressed data, was "cvxpylayers-0.1.6.tar", last modified: Sat Apr 15 17:01:45 2023, max compression
```

## Comparing `cvxpylayers-0.1.5.tar` & `cvxpylayers-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2021-04-15 20:12:55.532636 cvxpylayers-0.1.5/
--rw-rw-r--   0 akshay    (1000) akshay    (1000)    10159 2021-04-15 20:12:55.532636 cvxpylayers-0.1.5/PKG-INFO
--rw-rw-r--   0 akshay    (1000) akshay    (1000)     7911 2021-04-15 20:08:46.000000 cvxpylayers-0.1.5/README.md
-drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2021-04-15 20:12:55.528636 cvxpylayers-0.1.5/cvxpylayers/
--rw-rw-r--   0 akshay    (1000) akshay    (1000)       22 2020-06-03 19:55:07.000000 cvxpylayers-0.1.5/cvxpylayers/__init__.py
-drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2021-04-15 20:12:55.528636 cvxpylayers-0.1.5/cvxpylayers/jax/
--rw-rw-r--   0 akshay    (1000) akshay    (1000)       64 2021-04-15 20:08:46.000000 cvxpylayers-0.1.5/cvxpylayers/jax/__init__.py
--rw-rw-r--   0 akshay    (1000) akshay    (1000)    12476 2021-04-15 20:08:46.000000 cvxpylayers-0.1.5/cvxpylayers/jax/cvxpylayer.py
--rwxrwxr-x   0 akshay    (1000) akshay    (1000)    14087 2021-04-15 20:08:46.000000 cvxpylayers-0.1.5/cvxpylayers/jax/test_cvxpylayer.py
-drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2021-04-15 20:12:55.528636 cvxpylayers-0.1.5/cvxpylayers/tensorflow/
--rw-rw-r--   0 akshay    (1000) akshay    (1000)       71 2019-11-08 20:38:49.000000 cvxpylayers-0.1.5/cvxpylayers/tensorflow/__init__.py
--rw-rw-r--   0 akshay    (1000) akshay    (1000)    12651 2020-06-03 17:26:45.000000 cvxpylayers-0.1.5/cvxpylayers/tensorflow/cvxpylayer.py
--rw-rw-r--   0 akshay    (1000) akshay    (1000)    15238 2020-06-03 15:43:34.000000 cvxpylayers-0.1.5/cvxpylayers/tensorflow/test_cvxpylayer.py
-drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2021-04-15 20:12:55.532636 cvxpylayers-0.1.5/cvxpylayers/torch/
--rw-rw-r--   0 akshay    (1000) akshay    (1000)       66 2019-11-08 20:38:49.000000 cvxpylayers-0.1.5/cvxpylayers/torch/__init__.py
--rw-rw-r--   0 akshay    (1000) akshay    (1000)    15288 2020-06-03 15:43:34.000000 cvxpylayers-0.1.5/cvxpylayers/torch/cvxpylayer.py
--rwxrwxr-x   0 akshay    (1000) akshay    (1000)    13981 2020-06-03 15:43:34.000000 cvxpylayers-0.1.5/cvxpylayers/torch/test_cvxpylayer.py
-drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2021-04-15 20:12:55.528636 cvxpylayers-0.1.5/cvxpylayers.egg-info/
--rw-rw-r--   0 akshay    (1000) akshay    (1000)    10159 2021-04-15 20:12:55.000000 cvxpylayers-0.1.5/cvxpylayers.egg-info/PKG-INFO
--rw-rw-r--   0 akshay    (1000) akshay    (1000)      522 2021-04-15 20:12:55.000000 cvxpylayers-0.1.5/cvxpylayers.egg-info/SOURCES.txt
--rw-rw-r--   0 akshay    (1000) akshay    (1000)        1 2021-04-15 20:12:55.000000 cvxpylayers-0.1.5/cvxpylayers.egg-info/dependency_links.txt
--rw-rw-r--   0 akshay    (1000) akshay    (1000)       55 2021-04-15 20:12:55.000000 cvxpylayers-0.1.5/cvxpylayers.egg-info/requires.txt
--rw-rw-r--   0 akshay    (1000) akshay    (1000)       12 2021-04-15 20:12:55.000000 cvxpylayers-0.1.5/cvxpylayers.egg-info/top_level.txt
--rw-rw-r--   0 akshay    (1000) akshay    (1000)       38 2021-04-15 20:12:55.532636 cvxpylayers-0.1.5/setup.cfg
--rw-rw-r--   0 akshay    (1000) akshay    (1000)      646 2021-04-15 20:09:18.000000 cvxpylayers-0.1.5/setup.py
+drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)    11344 2019-11-08 20:38:49.000000 cvxpylayers-0.1.6/LICENSE
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)      191 2019-11-08 20:38:49.000000 cvxpylayers-0.1.6/NOTICE
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)     9540 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/PKG-INFO
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)     9216 2023-04-15 16:59:09.000000 cvxpylayers-0.1.6/README.md
+drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/cvxpylayers/
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)       22 2023-04-15 17:00:03.000000 cvxpylayers-0.1.6/cvxpylayers/__init__.py
+drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/cvxpylayers/jax/
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)       64 2021-04-15 20:08:46.000000 cvxpylayers-0.1.6/cvxpylayers/jax/__init__.py
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)    12476 2021-04-15 20:08:46.000000 cvxpylayers-0.1.6/cvxpylayers/jax/cvxpylayer.py
+-rwxrwxr-x   0 akshay    (1000) akshay    (1000)    14087 2021-04-15 20:08:46.000000 cvxpylayers-0.1.6/cvxpylayers/jax/test_cvxpylayer.py
+drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/cvxpylayers/tensorflow/
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)       71 2019-11-08 20:38:49.000000 cvxpylayers-0.1.6/cvxpylayers/tensorflow/__init__.py
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)    12651 2020-06-03 17:26:45.000000 cvxpylayers-0.1.6/cvxpylayers/tensorflow/cvxpylayer.py
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)    15238 2020-06-03 15:43:34.000000 cvxpylayers-0.1.6/cvxpylayers/tensorflow/test_cvxpylayer.py
+drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/cvxpylayers/torch/
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)       66 2019-11-08 20:38:49.000000 cvxpylayers-0.1.6/cvxpylayers/torch/__init__.py
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)    15379 2023-04-15 16:59:09.000000 cvxpylayers-0.1.6/cvxpylayers/torch/cvxpylayer.py
+-rwxrwxr-x   0 akshay    (1000) akshay    (1000)    13981 2020-06-03 15:43:34.000000 cvxpylayers-0.1.6/cvxpylayers/torch/test_cvxpylayer.py
+drwxrwxr-x   0 akshay    (1000) akshay    (1000)        0 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/cvxpylayers.egg-info/
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)     9540 2023-04-15 17:01:45.000000 cvxpylayers-0.1.6/cvxpylayers.egg-info/PKG-INFO
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)      537 2023-04-15 17:01:45.000000 cvxpylayers-0.1.6/cvxpylayers.egg-info/SOURCES.txt
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)        1 2023-04-15 17:01:45.000000 cvxpylayers-0.1.6/cvxpylayers.egg-info/dependency_links.txt
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)       55 2023-04-15 17:01:45.000000 cvxpylayers-0.1.6/cvxpylayers.egg-info/requires.txt
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)       12 2023-04-15 17:01:45.000000 cvxpylayers-0.1.6/cvxpylayers.egg-info/top_level.txt
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)       38 2023-04-15 17:01:45.431540 cvxpylayers-0.1.6/setup.cfg
+-rw-rw-r--   0 akshay    (1000) akshay    (1000)      646 2023-04-15 17:00:40.000000 cvxpylayers-0.1.6/setup.py
```

### Comparing `cvxpylayers-0.1.5/README.md` & `cvxpylayers-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: cvxpylayers
+Version: 0.1.6
+Summary: Differentiable convex optimization layers
+Home-page: https://github.com/cvxgrp/cvxpylayers
+License: Apache License, Version 2.0
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 ![cvxpylayers logo](cvxpylayers_logo.png)
 [![Build Status](https://travis-ci.org/cvxgrp/cvxpylayers.svg?branch=master)](https://travis-ci.org/cvxgrp/cvxpylayers)
 [![Build Status](https://ci.appveyor.com/api/projects/status/dhtbi9fb96mce56i/branch/master?svg=true)](https://ci.appveyor.com/project/sbarratt/cvxpylayers/branch/master)
 
 # cvxpylayers
 
 cvxpylayers is a Python library for constructing differentiable convex
@@ -174,14 +185,46 @@
 c_tch = torch.tensor(c.value, requires_grad=True)
 
 x_star, y_star, z_star = layer(a_tch, b_tch, c_tch)
 sum_of_solution = x_star + y_star + z_star
 sum_of_solution.backward()
 ```
 
+## Solvers
+
+At this time, we support two open-source solvers: [SCS](https://github.com/cvxgrp/scs) and [ECOS](https://github.com/embotech/ecos).
+SCS can be used to solve any problem expressible in CVXPY; ECOS can be used to solve problems that don't use
+the positive semidefinite or exponential cone (this roughly means that if you have positive semidefinite matrices
+or use atoms like `cp.log`, ECOS cannot be used to solve your problem via `cvxpylayers`).
+By default, `cvxpylayers` uses SCS to solve the problem.
+
+### Using ECOS
+First make sure that you have `cvxpylayers` and `diffcp` up to date,
+by running
+```
+pip install --upgrade cvxpylayers diffcp
+```
+Then, to use ECOS, you would pass the `solver_args` argument to the layer:
+```
+solution = layer(*params, solver_args={"solve_method": "ECOS"})
+```
+
+### Passing arguments to the solvers
+One can pass arguments to both SCS and ECOS by adding the argument as a key-value pair
+in the `solver_args` argument.
+For example, to increase the tolerance of SCS to `1e-8` one would write:
+```
+layer(*parameters, solver_args={"eps": 1e-8})
+```
+If SCS is not converging, we highly recommend switching to ECOS (if possible),
+and if not, using the following arguments to `SCS`:
+```
+solver_args={"eps": 1e-8, "max_iters": 10000, "acceleration_lookback": 0}
+``` 
+
 ## Examples
 Our [examples](examples) subdirectory contains simple applications of convex optimization
 layers in IPython notebooks.
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to
 discuss what you would like to change.
```

### Comparing `cvxpylayers-0.1.5/cvxpylayers/jax/cvxpylayer.py` & `cvxpylayers-0.1.6/cvxpylayers/jax/cvxpylayer.py`

 * *Files identical despite different names*

### Comparing `cvxpylayers-0.1.5/cvxpylayers/jax/test_cvxpylayer.py` & `cvxpylayers-0.1.6/cvxpylayers/jax/test_cvxpylayer.py`

 * *Files identical despite different names*

### Comparing `cvxpylayers-0.1.5/cvxpylayers/tensorflow/cvxpylayer.py` & `cvxpylayers-0.1.6/cvxpylayers/tensorflow/cvxpylayer.py`

 * *Files identical despite different names*

### Comparing `cvxpylayers-0.1.5/cvxpylayers/tensorflow/test_cvxpylayer.py` & `cvxpylayers-0.1.6/cvxpylayers/tensorflow/test_cvxpylayer.py`

 * *Files identical despite different names*

### Comparing `cvxpylayers-0.1.5/cvxpylayers/torch/cvxpylayer.py` & `cvxpylayers-0.1.6/cvxpylayers/torch/cvxpylayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,20 +102,21 @@
 
         if self.gp:
             for param in parameters:
                 if param.value is None:
                     raise ValueError("An initial value for each parameter is "
                                      "required when gp=True.")
             data, solving_chain, _ = problem.get_problem_data(
-                solver=cp.SCS, gp=True)
+                solver=cp.SCS, gp=True, solver_opts={'use_quad_obj': False})
             self.compiler = data[cp.settings.PARAM_PROB]
             self.dgp2dcp = solving_chain.get(cp.reductions.Dgp2Dcp)
             self.param_ids = [p.id for p in self.compiler.parameters]
         else:
-            data, _, _ = problem.get_problem_data(solver=cp.SCS)
+            data, _, _ = problem.get_problem_data(
+                solver=cp.SCS, solver_opts={'use_quad_obj': False})
             self.compiler = data[cp.settings.PARAM_PROB]
             self.param_ids = [p.id for p in self.param_order]
         self.cone_dims = dims_to_solver_dict(data["dims"])
 
     def forward(self, *params, solver_args={}):
         """Solve problem (or a batch of problems) corresponding to `params`
```

### Comparing `cvxpylayers-0.1.5/cvxpylayers/torch/test_cvxpylayer.py` & `cvxpylayers-0.1.6/cvxpylayers/torch/test_cvxpylayer.py`

 * *Files identical despite different names*

### Comparing `cvxpylayers-0.1.5/cvxpylayers.egg-info/SOURCES.txt` & `cvxpylayers-0.1.6/cvxpylayers.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+NOTICE
 README.md
 setup.py
 cvxpylayers/__init__.py
 cvxpylayers.egg-info/PKG-INFO
 cvxpylayers.egg-info/SOURCES.txt
 cvxpylayers.egg-info/dependency_links.txt
 cvxpylayers.egg-info/requires.txt
```

### Comparing `cvxpylayers-0.1.5/setup.py` & `cvxpylayers-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="cvxpylayers",
-    version="0.1.5",
+    version="0.1.6",
     description="Differentiable convex optimization layers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "numpy >= 1.15",
         "scipy >= 1.1.0",
```

