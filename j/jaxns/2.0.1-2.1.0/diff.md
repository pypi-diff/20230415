# Comparing `tmp/jaxns-2.0.1.tar.gz` & `tmp/jaxns-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxns-2.0.1.tar", last modified: Wed Mar  8 22:56:08 2023, max compression
+gzip compressed data, was "jaxns-2.1.0.tar", last modified: Sat Apr 15 13:41:40 2023, max compression
```

## Comparing `jaxns-2.0.1.tar` & `jaxns-2.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.712297 jaxns-2.0.1/
--rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2022-10-13 02:52:05.000000 jaxns-2.0.1/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     3391 2023-03-08 22:56:08.712297 jaxns-2.0.1/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     2952 2023-03-08 22:05:30.000000 jaxns-2.0.1/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.708297 jaxns-2.0.1/jaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      344 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10087 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/adaptive_refinement.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4949 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/initial_state.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.708297 jaxns-2.0.1/jaxns/internals/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.0.1/jaxns/internals/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12443 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4824 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2022-10-13 02:52:05.000000 jaxns-2.0.1/jaxns/internals/shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.712297 jaxns-2.0.1/jaxns/internals/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.0.1/jaxns/internals/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/tests/test_linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/tests/test_log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2842 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/tests/test_maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2022-12-29 07:48:31.000000 jaxns-2.0.1/jaxns/internals/tests/test_shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/internals/tests/test_stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.712297 jaxns-2.0.1/jaxns/likelihood_samplers/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.0.1/jaxns/likelihood_samplers/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    21852 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/likelihood_samplers/multi_ellipsoid_utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.712297 jaxns-2.0.1/jaxns/likelihood_samplers/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.0.1/jaxns/likelihood_samplers/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1753 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    17458 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16040 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/plotting.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    11830 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2716 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    26123 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/slice_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9157 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/special_priors.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8725 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/static_slice.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3878 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/static_uniform.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    17405 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5697 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/termination.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.712297 jaxns-2.0.1/jaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3561 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/tests/test_initial_state.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    14429 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/tests/test_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8024 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/tests/test_prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      976 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/tests/test_random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    13733 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/tests/test_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5040 2023-03-08 22:42:25.000000 jaxns-2.0.1/jaxns/types.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/uniform_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    14966 2023-01-03 05:33:37.000000 jaxns-2.0.1/jaxns/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-03-08 22:56:08.708297 jaxns-2.0.1/jaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     3391 2023-03-08 22:56:08.000000 jaxns-2.0.1/jaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1367 2023-03-08 22:56:08.000000 jaxns-2.0.1/jaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-03-08 22:56:08.000000 jaxns-2.0.1/jaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-03-08 22:56:08.000000 jaxns-2.0.1/jaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 jaxns-2.0.1/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-03-08 22:56:08.712297 jaxns-2.0.1/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-03-08 22:46:32.000000 jaxns-2.0.1/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2022-10-13 02:52:05.000000 jaxns-2.1.0/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3692 2023-04-15 13:41:40.401876 jaxns-2.1.0/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3253 2023-04-15 05:01:38.000000 jaxns-2.1.0/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.397876 jaxns-2.1.0/jaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      344 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10208 2023-04-14 22:54:16.000000 jaxns-2.1.0/jaxns/adaptive_refinement.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5281 2023-04-15 05:17:24.000000 jaxns-2.1.0/jaxns/initial_state.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.397876 jaxns-2.1.0/jaxns/internals/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/internals/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12443 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4824 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/internals/shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/internals/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/internals/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2842 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2022-12-29 07:48:31.000000 jaxns-2.1.0/jaxns/internals/tests/test_shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/likelihood_samplers/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/likelihood_samplers/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    21852 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/likelihood_samplers/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/likelihood_samplers/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1753 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18710 2023-04-15 01:00:38.000000 jaxns-2.1.0/jaxns/nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16040 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/plotting.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11830 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2716 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    26123 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/slice_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9157 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/special_priors.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     8748 2023-04-15 04:48:14.000000 jaxns-2.1.0/jaxns/static_slice.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3878 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/static_uniform.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17405 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5697 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/termination.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3561 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_initial_state.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    14429 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     8024 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      976 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13733 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5040 2023-03-08 22:42:25.000000 jaxns-2.1.0/jaxns/types.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/uniform_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15180 2023-04-15 00:09:56.000000 jaxns-2.1.0/jaxns/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.397876 jaxns-2.1.0/jaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3692 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1367 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 jaxns-2.1.0/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-04-15 13:41:40.401876 jaxns-2.1.0/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-04-15 04:58:33.000000 jaxns-2.1.0/setup.py
```

### Comparing `jaxns-2.0.1/LICENSE` & `jaxns-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/PKG-INFO` & `jaxns-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.0.1
+Version: 2.1.0
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![https://pypi.org/project/jaxns/](https://img.shields.io/pypi/v/jaxns.svg)
 
-![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/master/jaxns_logo.png)
+![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 
 # What is it?
 Provides a probabilistic programming framework based on nested sampling. It's coded in JAX in a manner that allows lowering the entire inference algorithm to XLA primitives, which are JIT-compiled for high performance. You can read about it here: (https://arxiv.org/abs/2012.15286)
 
 JAXNS uses a unique adaptive algorithm that enables arbitrary precision computing of evidence. Stay tuned for the paper that explains it.
 
+# Documentation
+
+You can check out the docs [here](https://jaxns.readthedocs.io/en/latest/#).
+
 # Install
 
-Note: JAXNS requires >= Python 3.9, and is tested on 3.9, 3.10, and 3.11.
+Note: JAXNS requires >= Python 3.8, and is tested on 3.8, 3.9, 3.10, and 3.11.
 
 Make sure you have JAX and the usual suspects with `pip install jax jaxlib numpy matplotlib scipy`, optionally also `scikit-learn` and `haiku-dm` for some examples. 
 Install with `pip install jaxns` or `pip install git+http://github.com/Joshuaalbert/jaxns.git` for the (no promises) bleeding-edge.
 
 # Getting help and contributing examples
 
 I'm really encourage anyone in the scientific community to get involved and join the discussion forum.
@@ -44,14 +48,18 @@
 # Speed test comparison with other nested sampling packages
 
 JAXNS is much faster than PolyChord, MultiNEST, and dynesty, typically achieving two to three orders of magnitude improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likeihood evaluations, JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by controlling some precision parameters.
 
 # Change Log
 
+8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
+
+3 January, 2023 -- JAXNS 2.0 released. Complete overhaul of components. New way to build models.
+
 5 August, 2022 -- JAXNS 1.1.1 released. Pytree shaped priors.
 
 2 June, 2022 -- JAXNS 1.1.0 released. Dynamic sampling takes advantage of adaptive refinement. Parallelisation. Bayesian opt and global opt modules.
 
 30 May, 2022 -- JAXNS 1.0.1 released. Improvements to speed, parallelisation, and structure of code.
 
 9 April, 2022 -- JAXNS 1.0.0 released. Parallel sampling, dynamic search, and adaptive refinement. Global optimiser released.
```

### Comparing `jaxns-2.0.1/README.md` & `jaxns-2.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 ![https://pypi.org/project/jaxns/](https://img.shields.io/pypi/v/jaxns.svg)
 
-![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/master/jaxns_logo.png)
+![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 
 # What is it?
 Provides a probabilistic programming framework based on nested sampling. It's coded in JAX in a manner that allows lowering the entire inference algorithm to XLA primitives, which are JIT-compiled for high performance. You can read about it here: (https://arxiv.org/abs/2012.15286)
 
 JAXNS uses a unique adaptive algorithm that enables arbitrary precision computing of evidence. Stay tuned for the paper that explains it.
 
+# Documentation
+
+You can check out the docs [here](https://jaxns.readthedocs.io/en/latest/#).
+
 # Install
 
-Note: JAXNS requires >= Python 3.9, and is tested on 3.9, 3.10, and 3.11.
+Note: JAXNS requires >= Python 3.8, and is tested on 3.8, 3.9, 3.10, and 3.11.
 
 Make sure you have JAX and the usual suspects with `pip install jax jaxlib numpy matplotlib scipy`, optionally also `scikit-learn` and `haiku-dm` for some examples. 
 Install with `pip install jaxns` or `pip install git+http://github.com/Joshuaalbert/jaxns.git` for the (no promises) bleeding-edge.
 
 # Getting help and contributing examples
 
 I'm really encourage anyone in the scientific community to get involved and join the discussion forum.
@@ -30,14 +34,18 @@
 # Speed test comparison with other nested sampling packages
 
 JAXNS is much faster than PolyChord, MultiNEST, and dynesty, typically achieving two to three orders of magnitude improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likeihood evaluations, JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by controlling some precision parameters.
 
 # Change Log
 
+8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
+
+3 January, 2023 -- JAXNS 2.0 released. Complete overhaul of components. New way to build models.
+
 5 August, 2022 -- JAXNS 1.1.1 released. Pytree shaped priors.
 
 2 June, 2022 -- JAXNS 1.1.0 released. Dynamic sampling takes advantage of adaptive refinement. Parallelisation. Bayesian opt and global opt modules.
 
 30 May, 2022 -- JAXNS 1.0.1 released. Improvements to speed, parallelisation, and structure of code.
 
 9 April, 2022 -- JAXNS 1.0.0 released. Parallel sampling, dynamic search, and adaptive refinement. Global optimiser released.
```

### Comparing `jaxns-2.0.1/jaxns/adaptive_refinement.py` & `jaxns-2.1.0/jaxns/adaptive_refinement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import Tuple, Optional
+from typing import Tuple, Optional, NamedTuple
 
 from etils.array_types import PRNGKey, FloatArray, IntArray, BoolArray
 from jax import core, numpy as jnp, tree_map, random, jit
 from jax._src.lax.control_flow import while_loop
 
 from jaxns.internals.maps import chunked_pmap
 from jaxns.internals.stats import linear_to_log_stats
@@ -120,93 +120,102 @@
             state: state to improve
             iid_state: state with only the i.i.d. samples
             non_iid_reservoir: samples that are not deemed i.i.d.
 
         Returns:
             state where all samples are considered i.i.d. sampled within their respective likelihood constraints
         """
+
         # update each sample one slice at a time until the stopping condition
 
-        CarryType = Tuple[PRNGKey, Reservoir, FloatArray, FloatArray, IntArray, PreprocessType]
+        class CarryType(NamedTuple):
+            key: PRNGKey
+            reservoir: Reservoir
+            last_log_Z_mean: FloatArray
+            last_diff_log_Z_mean: FloatArray
+            patience: IntArray
+            preprocess_data: PreprocessType
 
         def cond(body_state: CarryType) -> BoolArray:
             (_, _, _, _, patience, _) = body_state
             done = jnp.greater_equal(patience, self.uncert_improvement_patience)
             return jnp.bitwise_not(done)
 
         def body(body_state: CarryType) -> CarryType:
-            (key, old_reservoir, last_log_Z_mean, last_diff_log_Z_mean, patience, preprocess_data) = body_state
-
-            batch_size = old_reservoir.iid.size
+            batch_size = body_state.reservoir.iid.size
 
-            key, combine_key, improve_key = random.split(key, 3)
+            key, combine_key, improve_key = random.split(body_state.key, 3)
 
             parallel_improvement = chunked_pmap(
-                lambda key, seed_point, log_L_constraint: self._single_improvement(key=key, seed_point=seed_point,
-                                                                                   log_L_constraint=log_L_constraint,
-                                                                                   preprocess_data=preprocess_data),
+                lambda key, seed_point, log_L_constraint: self._single_improvement(
+                    key=key,
+                    seed_point=seed_point,
+                    log_L_constraint=log_L_constraint,
+                    preprocess_data=body_state.preprocess_data
+                ),
                 chunksize=self.num_parallel_samplers,
                 batch_size=batch_size)
             seed_points = SeedPoint(
-                U0=old_reservoir.point_U,
-                log_L0=old_reservoir.log_L
+                U0=body_state.reservoir.point_U,
+                log_L0=body_state.reservoir.log_L
             )
             update_reservoir = parallel_improvement(random.split(improve_key, batch_size),
                                                     seed_points,
-                                                    old_reservoir.log_L_constraint)
+                                                    body_state.reservoir.log_L_constraint)
 
             update_reservoir = update_reservoir._replace(
-                num_slices=update_reservoir.num_slices + old_reservoir.num_slices,
+                num_slices=update_reservoir.num_slices + body_state.reservoir.num_slices,
                 num_likelihood_evaluations=(update_reservoir.num_likelihood_evaluations
-                                            + old_reservoir.num_likelihood_evaluations)
+                                            + body_state.reservoir.num_likelihood_evaluations)
             )
 
             updated_state = self.combine_state(state=iid_state, update_reservoir=update_reservoir)
             evidence_calculation, sample_stats = analyse_sample_collection(
                 sample_collection=updated_state.sample_collection,
                 sorted_collection=True
             )
             log_Z_mean, log_Z_var = linear_to_log_stats(
                 log_f_mean=evidence_calculation.log_Z_mean,
                 log_f2_mean=evidence_calculation.log_Z2_mean
             )
-            nan_last_log_Z_mean = jnp.isnan(last_log_Z_mean)
+            nan_last_log_Z_mean = jnp.isnan(body_state.last_log_Z_mean)
             nan_log_Z_var = jnp.isnan(log_Z_var)
             nan_log_Z_mean = jnp.isnan(log_Z_mean)
 
-            diff_log_Z_mean = jnp.abs(last_log_Z_mean - log_Z_mean)
+            diff_log_Z_mean = jnp.abs(body_state.last_log_Z_mean - log_Z_mean)
             small_change = jnp.square(2. * diff_log_Z_mean) < log_Z_var
-            decreasing_change = diff_log_Z_mean < last_diff_log_Z_mean
+            decreasing_change = diff_log_Z_mean < body_state.last_diff_log_Z_mean
             stable = decreasing_change | small_change
             reset_patience = jnp.bitwise_not(stable) | (nan_log_Z_mean | nan_last_log_Z_mean | nan_log_Z_var)
-            patience = jnp.where(reset_patience, jnp.zeros_like(patience), patience + jnp.ones_like(patience))
+            patience = jnp.where(reset_patience, jnp.zeros_like(body_state.patience),
+                                 body_state.patience + jnp.ones_like(body_state.patience))
             preprocess_data = self.slice_sampler.preprocess(updated_state)
-            return (key, update_reservoir, log_Z_mean, diff_log_Z_mean, patience, preprocess_data)
+            return CarryType(key, update_reservoir, log_Z_mean, diff_log_Z_mean, patience, preprocess_data)
 
         preprocess_data = self.slice_sampler.preprocess(state)
 
         key, improve_key = random.split(state.key, 2)
         init_evidence_calculation, _ = analyse_sample_collection(
             sample_collection=state.sample_collection,
             sorted_collection=True
         )
         init_log_Z_mean, _ = linear_to_log_stats(
             log_f_mean=init_evidence_calculation.log_Z_mean,
             log_f2_mean=init_evidence_calculation.log_Z2_mean
         )
 
-        init_body_state: CarryType = (
+        init_body_state: CarryType = CarryType(
             improve_key, non_iid_reservoir, init_log_Z_mean, jnp.asarray(0., float_type), jnp.asarray(0, int_type),
             preprocess_data)
-        (_, update_reservoir, _, _, _, _) = while_loop(cond,
-                                                       body,
-                                                       init_body_state)
+        output_state = while_loop(cond,
+                                  body,
+                                  init_body_state)
 
         # mark as iid now <==> the evidence stopped changing
-        update_reservoir = update_reservoir._replace(iid=jnp.ones_like(update_reservoir.iid))
+        update_reservoir = output_state.reservoir._replace(iid=jnp.ones_like(output_state.reservoir.iid))
 
         updated_state = self.combine_state(state=iid_state, update_reservoir=update_reservoir)
 
         updated_state = updated_state._replace(key=key)
         return updated_state
 
     def __call__(self, state: NestedSamplerState) -> NestedSamplerState:
```

### Comparing `jaxns-2.0.1/jaxns/initial_state.py` & `jaxns-2.1.0/jaxns/initial_state.py`

 * *Files 21% similar despite different names*

```diff
@@ -64,14 +64,32 @@
     _, samples = scan(lambda s, key: (s, sampler.single_sample(key=key, log_L_constraint=-jnp.inf)),
                       (),
                       random.split(key, num_live_points))
     reservoir = Reservoir(*samples)
     return LivePoints(reservoir=reservoir)
 
 
+def sort_sample_collection(sample_collection: SampleCollection) -> SampleCollection:
+    """
+    Sort a sample collection lexigraphically.
+
+    Args:
+        sample_collection: sample collections
+
+    Returns:
+        sample collection sorted
+    """
+    idx_sort = jnp.lexsort((sample_collection.reservoir.log_L_constraint,
+                            sample_collection.reservoir.log_L))
+    sample_collection = sample_collection._replace(
+        reservoir=tree_map(lambda x: x[idx_sort], sample_collection.reservoir)
+    )
+    return sample_collection
+
+
 def get_live_points_from_samples(state: NestedSamplerState, log_L_constraint: FloatArray, num_live_points: int,
                                  sorted_collection: bool = True) \
         -> Tuple[NestedSamplerState, LivePoints]:
     """
     Extract live points from the samples already collected.
 
     Args:
@@ -90,19 +108,15 @@
     # 1. sort samples
     # 2. find the largest index, s, where sample.log_L_constraint[s] <= log_L_constraint
     # 3. select without replacement `num_live_points` indices from 0..s (inclusive)
     # 4. replace those indices with an empty sample
 
     sample_collection = state.sample_collection
     if not sorted_collection:
-        idx_sort = jnp.lexsort((sample_collection.reservoir.log_L_constraint,
-                                sample_collection.reservoir.log_L))
-        sample_collection = sample_collection._replace(
-            reservoir=tree_map(lambda x: x[idx_sort], sample_collection.reservoir)
-        )
+        sample_collection = sort_sample_collection(sample_collection)
 
     # find the largest index, s, where sample.log_L_constraint[s] <= log_L_constraint
     idx_supremum = jnp.searchsorted(sample_collection.reservoir.log_L_constraint, log_L_constraint, side='right') - 1
     idx_supremum = int(idx_supremum)
     key, sample_key = random.split(state.key)
     take_indices = resample_indicies(key=sample_key,
                                      log_weights=None,
```

### Comparing `jaxns-2.0.1/jaxns/internals/linalg.py` & `jaxns-2.1.0/jaxns/internals/linalg.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/log_semiring.py` & `jaxns-2.1.0/jaxns/internals/log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/maps.py` & `jaxns-2.1.0/jaxns/internals/maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/shapes.py` & `jaxns-2.1.0/jaxns/internals/shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/stats.py` & `jaxns-2.1.0/jaxns/internals/stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/tests/test_log_semiring.py` & `jaxns-2.1.0/jaxns/internals/tests/test_log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/tests/test_maps.py` & `jaxns-2.1.0/jaxns/internals/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/tests/test_shapes.py` & `jaxns-2.1.0/jaxns/internals/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/internals/tests/test_stats.py` & `jaxns-2.1.0/jaxns/internals/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/likelihood_samplers/multi_ellipsoid_utils.py` & `jaxns-2.1.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py` & `jaxns-2.1.0/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/model.py` & `jaxns-2.1.0/jaxns/model.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/nested_sampler.py` & `jaxns-2.1.0/jaxns/nested_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional, Tuple, Union, List
 
 import tensorflow_probability.substrates.jax as tfp
 from etils.array_types import PRNGKey, IntArray
 from jax import random, numpy as jnp, core, tree_map, vmap, jit
 
 from jaxns.adaptive_refinement import AdaptiveRefinement
-from jaxns.initial_state import init_sample_collection, get_uniform_init_live_points
+from jaxns.initial_state import init_sample_collection, get_uniform_init_live_points, get_live_points_from_samples
 from jaxns.internals.log_semiring import LogSpace, normalise_log_space
 from jaxns.internals.stats import linear_to_log_stats, effective_sample_size
 from jaxns.model import Model
 from jaxns.plotting import plot_cornerplot, plot_diagnostics
 from jaxns.slice_sampler import UniDimSliceSampler, AbstractSliceSampler
 from jaxns.static_slice import StaticSlice
 from jaxns.static_uniform import StaticUniform
@@ -32,20 +32,25 @@
 class NestedSampler:
     def __init__(self, model: Model, num_live_points: Union[int, float], num_parallel_samplers: int,
                  max_samples: Union[int, float]):
         remainder = int(num_live_points) % num_parallel_samplers
         extra = (num_parallel_samplers - remainder) % num_parallel_samplers
         if extra > 0:
             logger.warning(
-                f"Increasing max_samples ({num_live_points}) by {extra} to closest multiple of num_parallel_samplers.")
+                f"Increasing num_live_points ({num_live_points}) by {extra} to closest multiple of num_parallel_samplers.")
         self.num_live_points = int(num_live_points + extra)
         self.num_parallel_samplers = int(num_parallel_samplers)
         self.model = model
 
-        self.max_samples = int(max_samples)
+        remainder = int(max_samples) % num_parallel_samplers
+        extra = (num_parallel_samplers - remainder) % num_parallel_samplers
+        if extra > 0:
+            logger.warning(
+                f"Increasing max_samples ({max_samples}) by {extra} to closest multiple of num_parallel_samplers.")
+        self.max_samples = int(max_samples + extra)
 
     def resize_state(self, state: NestedSamplerState, max_num_samples: int) -> NestedSamplerState:
         """
         Grow the state to the size of max_num_samples.
 
         Args:
             state: state to enlarge
@@ -56,24 +61,26 @@
         """
         reservoir = state.sample_collection.reservoir
         if max_num_samples <= reservoir.log_L.size:
             logger.warning(
                 f"expected max_num_samples larger than the current size {reservoir.log_L.size}")
             return state
         diff_size = max_num_samples - reservoir.log_L.size
+        if diff_size <= 0:
+            return state
         reservoir_extra = init_sample_collection(size=diff_size, model=self.model).reservoir
         reservoir = tree_map(lambda old, update: jnp.concatenate([old, update], axis=0),
                              reservoir,
                              reservoir_extra)
         return state._replace(sample_collection=state.sample_collection._replace(reservoir=reservoir))
 
     def summary(self, results: NestedSamplerResults) -> str:
         return summary(results)
 
-    def plot_cornerplot(self, results: NestedSamplerResults, vars: Optional[List[str]]=None):
+    def plot_cornerplot(self, results: NestedSamplerResults, vars: Optional[List[str]] = None):
         plot_cornerplot(results, vars=vars)
 
     def plot_diagnostics(self, results: NestedSamplerResults):
         plot_diagnostics(results)
 
     def save_results(self, results: NestedSamplerResults, save_file: str):
         save_results(results, save_file)
@@ -159,14 +166,17 @@
             # total_num_samples / total_num_likelihood_evaluations
             termination_reason=termination_reason,  # termination condition as bit mask
             num_slices=sample_collection.reservoir.num_slices,
             samples=samples)
 
 
 class ApproximateNestedSampler(NestedSampler):
+    """
+    Performs nested sampling, producing only weakly i.i.d. samples during the shrinkage process.
+    """
     def __init__(self, model: Model, num_live_points: Union[int, float], num_parallel_samplers: int,
                  max_samples: Union[int, float],
                  slice_sampler: Optional[AbstractSliceSampler] = None):
         super(ApproximateNestedSampler, self).__init__(model=model, num_live_points=num_live_points,
                                                        num_parallel_samplers=num_parallel_samplers,
                                                        max_samples=max_samples)
 
@@ -349,14 +359,30 @@
             state: state (may be approximate, i.e. non-iid samples.)
 
         Returns:
             state with samples considered iid sampled from the likelihood constraint
         """
         return self.adaptive_refinement(state)
 
+    def prepare_new_iteration(self, state: NestedSamplerState, log_L_constraint: float,
+                              sorted_collection: bool = True) -> Tuple[NestedSamplerState, LivePoints]:
+        """
+        Extract live points from the samples already collected.
+
+        Args:
+            state: the current state
+            log_L_constraint: the contour to sample above
+            sorted_collection: whether the sample collection is already sorted
+
+        Returns:
+            a new state, and live points
+        """
+        return get_live_points_from_samples(state=state, log_L_constraint=log_L_constraint,
+                                            num_live_points=self.num_live_points, sorted_collection=sorted_collection)
+
     def __call__(self, key: PRNGKey, term_cond: TerminationCondition, *,
                  init_state: Optional[NestedSamplerState] = None,
                  live_points: Optional[LivePoints] = None) -> Tuple[IntArray, NestedSamplerState]:
         """
         Performs approximate nested sampling followed by adaptive refinement.
 
         Args:
```

### Comparing `jaxns-2.0.1/jaxns/plotting.py` & `jaxns-2.1.0/jaxns/plotting.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/prior.py` & `jaxns-2.1.0/jaxns/prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/random.py` & `jaxns-2.1.0/jaxns/random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/slice_sampler.py` & `jaxns-2.1.0/jaxns/slice_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/special_priors.py` & `jaxns-2.1.0/jaxns/special_priors.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/static_slice.py` & `jaxns-2.1.0/jaxns/static_slice.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,189 +1,204 @@
 import logging
-from typing import Tuple
+from typing import Tuple, NamedTuple, TypeVar
 
 from etils.array_types import PRNGKey, IntArray, BoolArray
 from jax import tree_map, numpy as jnp, random, pmap
 from jax._src.lax.control_flow import scan, while_loop
+from jax._src.lax.parallel import all_gather
 
 from jaxns.model import Model
 from jaxns.slice_sampler import PreprocessType, AbstractSliceSampler
 from jaxns.statistics import analyse_sample_collection
 from jaxns.termination import determine_termination
 from jaxns.types import NestedSamplerState, Reservoir, LivePoints, TerminationCondition, int_type
 from jaxns.utils import collect_samples
 
 logger = logging.getLogger('jaxns')
 
 __all__ = ['StaticSlice']
 
+T = TypeVar('T')
+
+
+def remove_chunk_dim(py_tree: T) -> T:
+    def _remove_chunk_dim(a):
+        shape = list(a.shape)
+        shape = [shape[0] * shape[1]] + shape[2:]
+        return jnp.reshape(a, shape)
+
+    return tree_map(_remove_chunk_dim, py_tree)
+
+
+def add_chunk_dim(py_tree: T, chunk_size: int) -> T:
+    def _add_chunk_dim(a):
+        shape = list(a.shape)
+        shape = [chunk_size, shape[0] // chunk_size] + shape[1:]
+        return jnp.reshape(a, shape)
+
+    return tree_map(_add_chunk_dim, py_tree)
+
 
 class StaticSlice:
     """
     Performs parallel nested sampling with a static number of samples.
-    This uses the fact that the union of samples from N independent static nested samplers with M live points is
+    This uses the fact that the union of samples from N independent perfect static nested samplers with M live points is
     equivalent to a single nested sampler with N*M live points.
     """
 
     def __init__(self, model: Model, slice_sampler: AbstractSliceSampler, num_live_points: int, num_slices: int,
                  num_parallel_samplers: int = 1):
-        # ensure we can split up request into equal parallel batches of work.
-        remainder = num_live_points % num_parallel_samplers
-        extra = (num_parallel_samplers - remainder) % num_parallel_samplers
-        if extra > 0:
-            logger.warning(
-                f"Increasing max_samples ({num_live_points}) by {extra} to closest multiple of num_parallel_samplers.")
-        self.num_live_points = num_live_points + extra
+        if num_live_points % num_parallel_samplers != 0:
+            raise ValueError(
+                f"num_live_points {num_live_points} must divide num_parallel_samplers {num_parallel_samplers}"
+            )
+        self.num_live_points = num_live_points
         self.num_parallel_samplers = num_parallel_samplers
         self.model = model
         self.slice_sampler = slice_sampler
         if num_slices < 1:
             raise ValueError(f"num_slices should be > 0, got {num_slices}.")
         self.num_slices = num_slices
 
-    def _single_thread_ns(self,
-                          key: PRNGKey,
-                          live_points: LivePoints,
-                          num_slices: IntArray,
-                          preprocess_data: PreprocessType) -> Tuple[Reservoir, LivePoints]:
+    def _single_live_point_shrink(self,
+                                  key: PRNGKey,
+                                  live_points: LivePoints,
+                                  num_slices: IntArray,
+                                  preprocess_data: PreprocessType) -> Tuple[Reservoir, LivePoints]:
         """
         Run nested sampling to replace an entire live point reservoir via shrinkage.
 
         Args:
             key: PRNGKey
             live_points: live points
             num_slices: slice sampling `num_slices` parameter
 
         Returns:
             dead point reservoir, live points, slice stats
         """
-        CarryType = Tuple[PRNGKey, LivePoints]
+
+        class CarryType(NamedTuple):
+            key: PRNGKey
+            live_points: LivePoints
+
         ResultType = Reservoir
 
         def body(carry: CarryType, unused_X: IntArray) -> Tuple[CarryType, ResultType]:
             del unused_X
-            (key, live_points) = carry
-            idx_min = jnp.argmin(live_points.reservoir.log_L)
-            dead_point: Reservoir = tree_map(lambda x: x[idx_min], live_points.reservoir)
+            idx_min = jnp.argmin(carry.live_points.reservoir.log_L)
+            dead_point: Reservoir = tree_map(lambda x: x[idx_min], carry.live_points.reservoir)
             log_L_dead = dead_point.log_L
 
             # contour becomes log_L_dead if log_L_dead is not supremum of live-points, else we choose the original
             # constraint of dead point. Note: we are at liberty to choose any log_L level as a contour so long as we
             # can sample within it uniformly.
-            on_supremum = jnp.equal(log_L_dead, jnp.max(live_points.reservoir.log_L))
+            on_supremum = jnp.equal(log_L_dead, jnp.max(carry.live_points.reservoir.log_L))
             log_L_contour = jnp.where(on_supremum, dead_point.log_L_constraint, log_L_dead)
 
             # replace dead point with a new sample about contour
-            key, seed_key, sample_key = random.split(key, 3)
+            key, seed_key, sample_key = random.split(carry.key, 3)
 
             seed_point = self.slice_sampler.get_seed_point(key=seed_key,
-                                                           live_points=live_points,
+                                                           live_points=carry.live_points,
                                                            log_L_constraint=log_L_contour)
             sample = self.slice_sampler.get_sample(key=sample_key,
                                                    seed_point=seed_point,
                                                    log_L_constraint=log_L_contour,
                                                    num_slices=num_slices,
                                                    preprocess_data=preprocess_data)
 
             live_points_reservoir = tree_map(lambda old, update: old.at[idx_min].set(update),
-                                             live_points.reservoir, Reservoir(*sample))
-            live_points = live_points._replace(reservoir=live_points_reservoir)
+                                             carry.live_points.reservoir, Reservoir(*sample))
+            live_points = carry.live_points._replace(reservoir=live_points_reservoir)
 
-            return (key, live_points), dead_point
+            return CarryType(key, live_points), dead_point
 
         (_, live_points), dead_reservoir = scan(body,
-                                                (key, live_points),
+                                                CarryType(key, live_points),
                                                 live_points.reservoir.log_L)
         return (dead_reservoir, live_points)
 
-    def __call__(self, state: NestedSamplerState,
-                 live_points: LivePoints,
-                 termination_cond: TerminationCondition
-                 ) -> Tuple[IntArray, NestedSamplerState, LivePoints]:
-        """
-        Performs nested sampling from an initial state with a static number of live points at each shrinkage step, and
-        terminating upon ANY of the terminiation criteria being met.
-
-        Args:
-            state: the current state of sampler
-            live_points: the live points to start sampling from
-            num_slices: the number of slices to take per prior dimension
-            termination_cond: the conditions for termination
+    def _single_thread_ns(self, state: NestedSamplerState, live_points: LivePoints,
+                          termination_cond: TerminationCondition):
 
-        Returns:
-            termination_reason, final state, and live points
-        """
-        if live_points.reservoir.log_L.size != self.num_live_points:
-            raise ValueError(
-                f"live points reservoir is the wrong size. "
-                f"Got {live_points.reservoir.log_L.size} but expected {self.num_live_points}.")
-
-        single_thread_sampler = lambda key, live_points, preprocess_data: self._single_thread_ns(
-            key=key,
-            live_points=live_points,
-            num_slices=self.num_slices,
-            preprocess_data=preprocess_data
-        )
-
-        CarryType = Tuple[BoolArray, IntArray, NestedSamplerState, LivePoints]
+        class CarryType(NamedTuple):
+            done: BoolArray
+            termination_reason: IntArray
+            state: NestedSamplerState
+            live_points: LivePoints
 
         def body(body_state: CarryType) -> CarryType:
-            (_, _, state, live_points) = body_state
-
-            key, sample_key = random.split(state.key, 2)
-            state = state._replace(key=key)
+            key, sample_key = random.split(body_state.state.key, 2)
+            state = body_state.state._replace(key=key)
 
             preprocess_data = self.slice_sampler.preprocess(state)
 
-            if self.num_parallel_samplers > 1:  # prepare live points to split up
-
-                # TODO(Joshuaalbert): rewrite using pgather to compute preprocess data locally on each device,
-                #  getting rid of outer loop.
-
-                parallel_single_thread_sampler = pmap(lambda key, live_points: single_thread_sampler(
-                    key=key, live_points=live_points, preprocess_data=preprocess_data))
+            (dead_reservoir, live_points) = self._single_live_point_shrink(
+                key=sample_key,
+                live_points=body_state.live_points,
+                num_slices=self.num_slices,
+                preprocess_data=preprocess_data
+            )
 
-                def _add_chunk_dim(a):
-                    shape = list(a.shape)
-                    shape = [self.num_parallel_samplers, shape[0] // self.num_parallel_samplers] + shape[1:]
-                    return jnp.reshape(a, shape)
-
-                live_points = tree_map(_add_chunk_dim, live_points)
-
-                keys = random.split(sample_key, self.num_parallel_samplers)
-                # parallel sampling
-                dead_reservoir, live_points = parallel_single_thread_sampler(keys, live_points)
-
-                # concatenate reservoir samples
-                def _remove_chunk_dim(a):
-                    shape = list(a.shape)
-                    shape = [shape[0] * shape[1]] + shape[2:]
-                    return jnp.reshape(a, shape)
-
-                (dead_reservoir, live_points) = tree_map(_remove_chunk_dim, (dead_reservoir, live_points))
-            else:
-                (dead_reservoir, live_points) = single_thread_sampler(key=sample_key, live_points=live_points,
-                                                                      preprocess_data=preprocess_data)
+            all_dead_reservoir: Reservoir = remove_chunk_dim(all_gather(dead_reservoir, 'i'))
 
             # update the state with sampled points from last round
-            new_state = collect_samples(state, dead_reservoir)
+            new_state = collect_samples(state, all_dead_reservoir)
+
             evidence_calculation, sample_stats = analyse_sample_collection(
                 sample_collection=new_state.sample_collection,
                 sorted_collection=True
             )
             done, termination_reason = determine_termination(
                 term_cond=termination_cond,
                 sample_collection=new_state.sample_collection,
                 evidence_calculation=evidence_calculation,
                 live_points=live_points
             )
 
-            return (done, termination_reason, new_state, live_points)
+            return CarryType(done=done, termination_reason=termination_reason, state=new_state,
+                             live_points=live_points)
 
-        (_, termination_reason, state, live_points) = while_loop(
+        output_carry = while_loop(
             lambda body_state: jnp.bitwise_not(body_state[0]),
             body,
-            (jnp.asarray(False, jnp.bool_),
-             jnp.asarray(0, int_type), state, live_points)
+            CarryType(done=jnp.asarray(False, jnp.bool_),
+                      termination_reason=jnp.asarray(0, int_type), state=state, live_points=live_points)
         )
 
+        return output_carry.termination_reason, output_carry.state, output_carry.live_points
+
+    def __call__(self, state: NestedSamplerState,
+                 live_points: LivePoints,
+                 termination_cond: TerminationCondition
+                 ) -> Tuple[IntArray, NestedSamplerState, LivePoints]:
+        """
+        Performs nested sampling from an initial state with a static number of live points at each shrinkage step, and
+        terminating upon ANY of the terminiation criteria being met.
+
+        Args:
+            state: the current state of sampler
+            live_points: the live points to start sampling from
+            termination_cond: the conditions for termination
+
+        Returns:
+            termination_reason, final state, and live points
+        """
+        if live_points.reservoir.log_L.size != self.num_live_points:
+            raise ValueError(
+                f"live points reservoir is the wrong size. "
+                f"Got {live_points.reservoir.log_L.size} but expected {self.num_live_points}.")
+
+        chunked_live_points = add_chunk_dim(live_points, self.num_parallel_samplers)
+
+        parallel_ns = pmap(lambda live_points: self._single_thread_ns(
+            state=state,
+            live_points=live_points,
+            termination_cond=termination_cond
+        ), axis_name='i')
+
+        chunked_termination_reason, chunked_state, chunked_live_points = parallel_ns(chunked_live_points)
+
+        termination_reason, state = tree_map(lambda x: x[0], (chunked_termination_reason, chunked_state))
+        live_points = remove_chunk_dim(chunked_live_points)
+
         return termination_reason, state, live_points
```

### Comparing `jaxns-2.0.1/jaxns/static_uniform.py` & `jaxns-2.1.0/jaxns/static_uniform.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/statistics.py` & `jaxns-2.1.0/jaxns/statistics.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/termination.py` & `jaxns-2.1.0/jaxns/termination.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/tests/test_initial_state.py` & `jaxns-2.1.0/jaxns/tests/test_initial_state.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/tests/test_nested_sampler.py` & `jaxns-2.1.0/jaxns/tests/test_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/tests/test_prior.py` & `jaxns-2.1.0/jaxns/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/tests/test_random.py` & `jaxns-2.1.0/jaxns/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/tests/test_statistics.py` & `jaxns-2.1.0/jaxns/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/types.py` & `jaxns-2.1.0/jaxns/types.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/uniform_sampler.py` & `jaxns-2.1.0/jaxns/uniform_sampler.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/jaxns/utils.py` & `jaxns-2.1.0/jaxns/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,24 @@
            'analytic_posterior_samples',
            'analytic_log_evidence',
            'save_pytree',
            'save_results',
            'load_pytree',
            'load_results']
 
-
 def sort_samples(sample_collection: SampleCollection):
+    """
+    Sorts a sample collection lexigraphically, first on log_L then on log_L_constraint.
+
+    Args:
+        sample_collection: sample collection to sort
+
+    Returns:
+        sorted sample collection
+    """
     idx_sort = jnp.lexsort((sample_collection.reservoir.log_L_constraint,
                             sample_collection.reservoir.log_L))
     sample_collection = sample_collection._replace(
         reservoir=tree_map(lambda x: x[idx_sort], sample_collection.reservoir)
     )
     return sample_collection
```

### Comparing `jaxns-2.0.1/jaxns.egg-info/PKG-INFO` & `jaxns-2.1.0/jaxns.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.0.1
+Version: 2.1.0
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![https://pypi.org/project/jaxns/](https://img.shields.io/pypi/v/jaxns.svg)
 
-![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/master/jaxns_logo.png)
+![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
 
 # What is it?
 Provides a probabilistic programming framework based on nested sampling. It's coded in JAX in a manner that allows lowering the entire inference algorithm to XLA primitives, which are JIT-compiled for high performance. You can read about it here: (https://arxiv.org/abs/2012.15286)
 
 JAXNS uses a unique adaptive algorithm that enables arbitrary precision computing of evidence. Stay tuned for the paper that explains it.
 
+# Documentation
+
+You can check out the docs [here](https://jaxns.readthedocs.io/en/latest/#).
+
 # Install
 
-Note: JAXNS requires >= Python 3.9, and is tested on 3.9, 3.10, and 3.11.
+Note: JAXNS requires >= Python 3.8, and is tested on 3.8, 3.9, 3.10, and 3.11.
 
 Make sure you have JAX and the usual suspects with `pip install jax jaxlib numpy matplotlib scipy`, optionally also `scikit-learn` and `haiku-dm` for some examples. 
 Install with `pip install jaxns` or `pip install git+http://github.com/Joshuaalbert/jaxns.git` for the (no promises) bleeding-edge.
 
 # Getting help and contributing examples
 
 I'm really encourage anyone in the scientific community to get involved and join the discussion forum.
@@ -44,14 +48,18 @@
 # Speed test comparison with other nested sampling packages
 
 JAXNS is much faster than PolyChord, MultiNEST, and dynesty, typically achieving two to three orders of magnitude improvement in speed on cheap likelihood evaluations.
 This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likeihood evaluations, JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by controlling some precision parameters.
 
 # Change Log
 
+8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
+
+3 January, 2023 -- JAXNS 2.0 released. Complete overhaul of components. New way to build models.
+
 5 August, 2022 -- JAXNS 1.1.1 released. Pytree shaped priors.
 
 2 June, 2022 -- JAXNS 1.1.0 released. Dynamic sampling takes advantage of adaptive refinement. Parallelisation. Bayesian opt and global opt modules.
 
 30 May, 2022 -- JAXNS 1.0.1 released. Improvements to speed, parallelisation, and structure of code.
 
 9 April, 2022 -- JAXNS 1.0.0 released. Parallel sampling, dynamic search, and adaptive refinement. Global optimiser released.
```

### Comparing `jaxns-2.0.1/jaxns.egg-info/SOURCES.txt` & `jaxns-2.1.0/jaxns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxns-2.0.1/setup.py` & `jaxns-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup_requires = ['jax>=' + __minimum_jax_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='jaxns',
-      version='2.0.1',
+      version='2.1.0',
       description='Nested Sampling in JAX',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/jaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

