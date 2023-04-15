# Comparing `tmp/UncertainSCI-1.0rc1.tar.gz` & `tmp/UncertainSCI-1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UncertainSCI-1.0rc1.tar", last modified: Wed Apr  5 19:47:50 2023, max compression
+gzip compressed data, was "UncertainSCI-1.0rc2.tar", last modified: Sat Apr 15 18:43:35 2023, max compression
```

## Comparing `UncertainSCI-1.0rc1.tar` & `UncertainSCI-1.0rc2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:47:50.122054 UncertainSCI-1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-05 19:47:50.122054 UncertainSCI-1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:47:50.118054 UncertainSCI-1.0rc1/UncertainSCI/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31950 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/families.py
--rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/model_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/opoly1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/opolynd.py
--rw-r--r--   0 runner    (1001) docker     (123)    32747 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/pce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25585 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/ttr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:47:50.118054 UncertainSCI-1.0rc1/UncertainSCI/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/array_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/casting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/compute_moment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/prob.py
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/quad.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/verify_orthonormal.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-05 19:47:40.000000 UncertainSCI-1.0rc1/UncertainSCI/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:47:50.118054 UncertainSCI-1.0rc1/UncertainSCI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-05 19:47:50.000000 UncertainSCI-1.0rc1/UncertainSCI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-05 19:47:50.000000 UncertainSCI-1.0rc1/UncertainSCI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 19:47:50.000000 UncertainSCI-1.0rc1/UncertainSCI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-05 19:47:50.000000 UncertainSCI-1.0rc1/UncertainSCI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 19:47:50.000000 UncertainSCI-1.0rc1/UncertainSCI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-05 19:47:50.122054 UncertainSCI-1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:47:50.122054 UncertainSCI-1.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_fjacobi_inv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_hermite_inv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_jacobipolys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_laguerre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_laguerre_inv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_normalexp_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_pce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_polys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-05 19:47:41.000000 UncertainSCI-1.0rc1/tests/test_ttr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:43:35.600387 UncertainSCI-1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-15 18:43:35.600387 UncertainSCI-1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:43:35.596387 UncertainSCI-1.0rc2/UncertainSCI/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31950 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/families.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/model_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/opoly1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/opolynd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32745 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/pce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25585 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/ttr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:43:35.596387 UncertainSCI-1.0rc2/UncertainSCI/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/array_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/casting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/compute_moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/verify_orthonormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/UncertainSCI/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:43:35.596387 UncertainSCI-1.0rc2/UncertainSCI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-15 18:43:35.000000 UncertainSCI-1.0rc2/UncertainSCI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-15 18:43:35.000000 UncertainSCI-1.0rc2/UncertainSCI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:43:35.000000 UncertainSCI-1.0rc2/UncertainSCI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 18:43:35.000000 UncertainSCI-1.0rc2/UncertainSCI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 18:43:35.000000 UncertainSCI-1.0rc2/UncertainSCI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-15 18:43:35.600387 UncertainSCI-1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:43:35.600387 UncertainSCI-1.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_fjacobi_inv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_hermite_inv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_jacobipolys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_laguerre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_laguerre_inv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_normalexp_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_pce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_polys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-15 18:43:26.000000 UncertainSCI-1.0rc2/tests/test_ttr.py
```

### Comparing `UncertainSCI-1.0rc1/LICENSE` & `UncertainSCI-1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/distributions.py` & `UncertainSCI-1.0rc2/UncertainSCI/distributions.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/families.py` & `UncertainSCI-1.0rc2/UncertainSCI/families.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/indexing.py` & `UncertainSCI-1.0rc2/UncertainSCI/indexing.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/model_examples.py` & `UncertainSCI-1.0rc2/UncertainSCI/model_examples.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/opoly1d.py` & `UncertainSCI-1.0rc2/UncertainSCI/opoly1d.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/opolynd.py` & `UncertainSCI-1.0rc2/UncertainSCI/opolynd.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/pce.py` & `UncertainSCI-1.0rc2/UncertainSCI/pce.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             raise ValueError("Unsupported sample type '{0}' for input\
                               sample_type".format(self.sampling))
 
         self.set_weights()
 
     def integration_weights(self):
         """
-        Generates sample weights associated to integration."
+        Generates sample weights associated to integration.
         """
 
         if self.training == 'wlsq':
 
             p_standard = self.map_to_standard_space(self.samples)
 
             V = self.distribution.polys.eval(p_standard, self.index_set.get_indices())
@@ -775,15 +775,15 @@
         """
         Computes global derivative-based sensitivity indices. For a
         PCE with respect to a :math:`d`-dimensional random variable :math:`Z`,
         then this senstivity index along dimension :math:`i` is defined as
 
         .. math::
 
-          S_i \\coloneqq E \\left[ p(Z) \\right] = \\int p(z) \\omega(z) d z,
+          S_i \\colon = E \\left[ p(Z) \\right] = \\int p(z) \\omega(z) d z,
 
         where :math:`E[\\cdot]` it expectation operator, :math:`p` is the PCE
         emulator, and :math:`\\omega` is the probability density function for
         the random variable :math:`Z`.
 
         These sensitivity indices measure the average rate-of-change of the PCE
         response with respect to dimension :math:`i`.
```

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/sampling.py` & `UncertainSCI-1.0rc2/UncertainSCI/sampling.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/transformations.py` & `UncertainSCI-1.0rc2/UncertainSCI/transformations.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/ttr.py` & `UncertainSCI-1.0rc2/UncertainSCI/ttr.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/utils/compute_moment.py` & `UncertainSCI-1.0rc2/UncertainSCI/utils/compute_moment.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/utils/linalg.py` & `UncertainSCI-1.0rc2/UncertainSCI/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/utils/prob.py` & `UncertainSCI-1.0rc2/UncertainSCI/utils/prob.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/utils/quad.py` & `UncertainSCI-1.0rc2/UncertainSCI/utils/quad.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI/vis.py` & `UncertainSCI-1.0rc2/UncertainSCI/vis.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/UncertainSCI.egg-info/SOURCES.txt` & `UncertainSCI-1.0rc2/UncertainSCI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/setup.py` & `UncertainSCI-1.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='UncertainSCI',
-    version='1.0-rc1',
+    version='1.0rc2',
     author='UncertainSCI Developers',
     author_email='uncertainsci@sci.utah.edu',
     packages=find_packages(),
     package_dir={'': '.'},
     download_url=r'https://github.com/SCIInstitute/UncertainSCI',
     description=r'A Non-invasive Uncertainty Quantification tool',
     long_description= long_description,
```

### Comparing `UncertainSCI-1.0rc1/tests/test_fjacobi_inv.py` & `UncertainSCI-1.0rc2/tests/test_fjacobi_inv.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_hermite_inv.py` & `UncertainSCI-1.0rc2/tests/test_hermite_inv.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_indexing.py` & `UncertainSCI-1.0rc2/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_jacobipolys.py` & `UncertainSCI-1.0rc2/tests/test_jacobipolys.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_laguerre.py` & `UncertainSCI-1.0rc2/tests/test_laguerre.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_laguerre_inv.py` & `UncertainSCI-1.0rc2/tests/test_laguerre_inv.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_linalg.py` & `UncertainSCI-1.0rc2/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_models.py` & `UncertainSCI-1.0rc2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_normalexp_dist.py` & `UncertainSCI-1.0rc2/tests/test_normalexp_dist.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_pce.py` & `UncertainSCI-1.0rc2/tests/test_pce.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_polys.py` & `UncertainSCI-1.0rc2/tests/test_polys.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_quad.py` & `UncertainSCI-1.0rc2/tests/test_quad.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_sampling.py` & `UncertainSCI-1.0rc2/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_transform.py` & `UncertainSCI-1.0rc2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `UncertainSCI-1.0rc1/tests/test_ttr.py` & `UncertainSCI-1.0rc2/tests/test_ttr.py`

 * *Files identical despite different names*

