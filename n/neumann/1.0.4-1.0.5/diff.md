# Comparing `tmp/neumann-1.0.4.tar.gz` & `tmp/neumann-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neumann-1.0.4.tar", last modified: Wed Mar 15 19:21:31 2023, max compression
+gzip compressed data, was "neumann-1.0.5.tar", last modified: Fri Apr 14 22:48:24 2023, max compression
```

## Comparing `neumann-1.0.4.tar` & `neumann-1.0.5.tar`

### file list

```diff
@@ -1,70 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.625266 neumann-1.0.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-03-15 19:21:24.000000 neumann-1.0.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-03-15 19:21:24.000000 neumann-1.0.4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-03-15 19:21:31.625266 neumann-1.0.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4789 2023-03-15 19:21:24.000000 neumann-1.0.4/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-03-15 19:21:24.000000 neumann-1.0.4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-03-15 19:21:24.000000 neumann-1.0.4/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-03-15 19:21:31.625266 neumann-1.0.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-03-15 19:21:24.000000 neumann-1.0.4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.613266 neumann-1.0.4/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.617266 neumann-1.0.4/src/neumann/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.617266 neumann-1.0.4/src/neumann/approx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/approx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/approx/func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7210 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/approx/lagrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9853 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/approx/mls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5607 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/arraysetops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/decorate.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.617266 neumann-1.0.4/src/neumann/function/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/function/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/function/constraint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9141 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/function/function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/function/functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3851 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/function/metafunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/function/relation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/function/testfunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/hist.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.621266 neumann-1.0.4/src/neumann/linalg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/abstract.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26648 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frame.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.621266 neumann-1.0.4/src/neumann/linalg/frontal/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frontal/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frontal/frontal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frontal/frutils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frontal/path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frontal/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frontal/proc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/frontal/topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12266 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/solve.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.621266 neumann-1.0.4/src/neumann/linalg/sparse/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/sparse/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10045 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/sparse/csr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10297 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/sparse/jaggedarray.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/sparse/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12663 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/tensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/top.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23195 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6357 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/linalg/vector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4333 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/logical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/numint.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.625266 neumann-1.0.4/src/neumann/optimize/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/optimize/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/optimize/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14973 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/optimize/ga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31396 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/optimize/lp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.625266 neumann-1.0.4/src/neumann/topology/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/topology/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5492 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/topology/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-03-15 19:21:24.000000 neumann-1.0.4/src/neumann/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-15 19:21:31.617266 neumann-1.0.4/src/neumann.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-03-15 19:21:31.000000 neumann-1.0.4/src/neumann.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1673 2023-03-15 19:21:31.000000 neumann-1.0.4/src/neumann.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-15 19:21:31.000000 neumann-1.0.4/src/neumann.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-15 19:21:31.000000 neumann-1.0.4/src/neumann.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-03-15 19:21:31.000000 neumann-1.0.4/src/neumann.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-03-15 19:21:31.000000 neumann-1.0.4/src/neumann.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-04-14 22:48:17.000000 neumann-1.0.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-04-14 22:48:17.000000 neumann-1.0.5/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-04-14 22:48:24.336143 neumann-1.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4789 2023-04-14 22:48:17.000000 neumann-1.0.5/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-04-14 22:48:17.000000 neumann-1.0.5/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-04-14 22:48:17.000000 neumann-1.0.5/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-14 22:48:24.336143 neumann-1.0.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-04-14 22:48:17.000000 neumann-1.0.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.324144 neumann-1.0.5/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.328143 neumann-1.0.5/src/neumann/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.328143 neumann-1.0.5/src/neumann/approx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7210 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/lagrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9853 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/mls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5607 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/arraysetops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/decorate.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.332143 neumann-1.0.5/src/neumann/function/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/constraint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9141 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3851 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/metafunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/relation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/testfunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/hist.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.332143 neumann-1.0.5/src/neumann/linalg/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/abstract.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26648 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frame.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.332143 neumann-1.0.5/src/neumann/linalg/frontal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/frontal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/frutils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/path.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/proc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12864 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/solve.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/src/neumann/linalg/sparse/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10045 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/csr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10297 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/jaggedarray.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12663 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/tensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/top.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24706 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6769 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/vector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4333 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/numint.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/src/neumann/optimize/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14973 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31396 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/lp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/src/neumann/topology/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/topology/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5492 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/topology/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.328143 neumann-1.0.5/src/neumann.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1856 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1185 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_approx.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33836 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_linalg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3776 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7684 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_lpp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_numint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_utils.py
```

### Comparing `neumann-1.0.4/LICENSE` & `neumann-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/PKG-INFO` & `neumann-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neumann
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Home-page: https://github.com/dewloosh/Neumann
-Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.4.zip
+Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.5.zip
 Author: Bence Balogh
 Author-email: dewloosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `neumann-1.0.4/README.md` & `neumann-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/setup.py` & `neumann-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/approx/func.py` & `neumann-1.0.5/src/neumann/approx/func.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/approx/lagrange.py` & `neumann-1.0.5/src/neumann/approx/lagrange.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/approx/mls.py` & `neumann-1.0.5/src/neumann/approx/mls.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/arraysetops.py` & `neumann-1.0.5/src/neumann/arraysetops.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/decorate.py` & `neumann-1.0.5/src/neumann/decorate.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/function/constraint.py` & `neumann-1.0.5/src/neumann/function/constraint.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/function/function.py` & `neumann-1.0.5/src/neumann/function/function.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/function/functions.py` & `neumann-1.0.5/src/neumann/function/functions.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/function/metafunction.py` & `neumann-1.0.5/src/neumann/function/metafunction.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/function/relation.py` & `neumann-1.0.5/src/neumann/function/relation.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/function/testfunction.py` & `neumann-1.0.5/src/neumann/function/testfunction.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/hist.py` & `neumann-1.0.5/src/neumann/hist.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/abstract.py` & `neumann-1.0.5/src/neumann/linalg/abstract.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/frame.py` & `neumann-1.0.5/src/neumann/linalg/frame.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/frontal/frontal.py` & `neumann-1.0.5/src/neumann/linalg/frontal/frontal.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/frontal/frutils.py` & `neumann-1.0.5/src/neumann/linalg/frontal/frutils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/frontal/path.py` & `neumann-1.0.5/src/neumann/linalg/frontal/path.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/frontal/postproc.py` & `neumann-1.0.5/src/neumann/linalg/frontal/postproc.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/frontal/proc.py` & `neumann-1.0.5/src/neumann/linalg/frontal/proc.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/frontal/topo.py` & `neumann-1.0.5/src/neumann/linalg/frontal/topo.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/meta.py` & `neumann-1.0.5/src/neumann/linalg/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,35 +120,53 @@
 
     def __init__(self, *args, cls_params=None, contiguous: bool = True, **kwargs):
         if len(args) > 0 and isinstance(args[0], np.ndarray):
             buf = ascont(args[0]) if contiguous else args[0]
         else:
             buf = np.array(*args, **kwargs)
         cls_params = dict() if cls_params is None else cls_params
+        buf = np.array(buf, dtype=float)
         self._array = self._array_cls_(
             shape=buf.shape, buffer=buf, dtype=buf.dtype, **cls_params
         )
         super(ArrayWrapper, self).__init__(wrap=self._array)
 
     @property
     def dim(self) -> int:
         """
         Returns the dimension of the array.
         """
         return len(self._array.shape)
 
     @property
-    def minmax(self) -> Tuple:
+    def minmax(self) -> Tuple[float]:
         """
         Returns the minimum and maximum values of the array.
-
-        .. versionadded:: 0.0.4
-
         """
         return minmax(self._array)
+    
+    def chop(self, tol:float=1e-12) -> "ArrayWrapper":
+        """
+        Sets very small values (in an absolute sense) to zero.
+
+        .. versionadded:: 1.0.5
+        
+        Parameters
+        ----------
+        tol: float, Optional
+            The values whose absolute value is less than this limit are
+            set to zero. Default is 1e-12.
+        
+        Returns
+        -------
+        ~`neumann.linalg.meta.ArrayWrapper`
+            The object the call was made upon.
+        """
+        self._array[np.where(np.abs(self._array) < tol)] = 0.0
+        return self
 
     def __array__(self, dtype=None):
         if dtype is not None:
             return self._array.astype(dtype)
         return self._array
 
     def __getitem__(self, key):
@@ -215,19 +233,19 @@
         ...
 
     @abstractmethod
     def show(self) -> ndarray:
         ...
 
     @abstractmethod
-    def orient(self) -> "TensorLike":
+    def orient(self) -> "FrameLike":
         ...
 
     @abstractmethod
-    def orient_new(self) -> "TensorLike":
+    def orient_new(self) -> "FrameLike":
         ...
 
     @abstractmethod
     def Gram(self) -> ndarray:
         ...
 
     @abstractmethod
```

### Comparing `neumann-1.0.4/src/neumann/linalg/solve.py` & `neumann-1.0.5/src/neumann/linalg/solve.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/sparse/csr.py` & `neumann-1.0.5/src/neumann/linalg/sparse/csr.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/sparse/jaggedarray.py` & `neumann-1.0.5/src/neumann/linalg/sparse/jaggedarray.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/sparse/utils.py` & `neumann-1.0.5/src/neumann/linalg/sparse/utils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/tensor.py` & `neumann-1.0.5/src/neumann/linalg/tensor.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/top.py` & `neumann-1.0.5/src/neumann/linalg/top.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/linalg/utils.py` & `neumann-1.0.5/src/neumann/linalg/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "normalize",
     "normalize2d",
     "norm",
     "norm2d",
     "linspace",
     "linspace1d",
     "inv",
+    "show_vector"
 ]
 
 
 def permutation_tensor(dim: int = 3) -> ndarray:
     """
     Returns the Levi-Civita pseudotensor for N dimensions.
 
@@ -271,16 +272,56 @@
         raise TypeError("Invalid types encountered for dot product.")
     if not all([isinstance(x, (ndarray, ArrayWrapper, list)) for x in [a, b]]):
         raise TypeError("Invalid types encountered for dot product.")
     inputs = [x._array if isinstance(x, ArrayWrapper) else x for x in [a, b]]
     return np.cross(*inputs, *args, **kwargs)
 
 
+def show_vector(dcm: ndarray, arr: ndarray) -> ndarray:
+    """
+    Returns the coordinates of a single or multiple vectors in a frame specified
+    by one or several DCM matrices. The function can handle the following scenarios:
+    
+        - a single (1d) vector and a single (2d) dcm matrix (trivial case)
+        - a stack of vectors (2d) and a single (2d) dcm matrix
+        - a stack of fectors (2d) and dcm matrices for each vector in the stack (3d)
+        
+    .. versionadded:: 1.0.5
+
+    Parameters
+    ----------
+    dcm : numpy.ndarray
+        The dcm matrix of the transformation as a 2d or 3d float array.
+    arr : numpy.ndarray
+        1d or 2d float array of coordinates of a single vector. If it is 2d, then
+        it is assumed that the coordinates of the i-th vector are accessible as
+        `arr[i]`.
+
+    Returns
+    -------
+    numpy.ndarray
+        The new coordinates with the same shape as `arr`.
+    """
+    if len(arr.shape) == 1 and len(dcm.shape) == 2:
+        return _show_vector(dcm, arr)  # dcm @ arr
+    elif len(arr.shape) == 2 and len(dcm.shape) == 2:
+        return _show_vectors(dcm, arr)  # dcm @ arr
+    elif len(arr.shape) == 2 and len(dcm.shape) == 3:
+        return _show_vectors_multi(dcm, arr)  # dcm @ arr
+    else:
+        msg = (
+            "Mismatch in shapes!"
+            f"Input one has shape {dcm.shape} and input two has shape {arr.shape}."
+            "See the docs for the correct input shapes."
+        )
+        raise LinalgOperationInputError(msg)
+
+
 @njit(nogil=True, cache=__cache)
-def _show_vector(dcm: np.ndarray, arr: np.ndarray) -> ndarray:
+def _show_vector(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of a single vector in a frame specified
     by a DCM matrix.
 
     Parameters
     ----------
     dcm : numpy.ndarray
@@ -293,15 +334,15 @@
     numpy.ndarray
         The new coordinates of the vector with the same shape as `arr`.
     """
     return dcm @ arr
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def _show_vectors(dcm: np.ndarray, arr: np.ndarray) -> ndarray:
+def _show_vectors(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of multiple vectors in a frame specified
     by a DCM matrix.
 
     Parameters
     ----------
     dcm : numpy.ndarray
@@ -317,15 +358,15 @@
     res = np.zeros_like(arr)
     for i in prange(arr.shape[0]):
         res[i] = dcm @ arr[i, :]
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def _show_vectors_multi(dcm: np.ndarray, arr: np.ndarray) -> ndarray:
+def _show_vectors_multi(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of multiple vectors and multiple DCM matrices.
 
     Parameters
     ----------
     dcm : numpy.ndarray
         The dcm matrix of the transformation as a 3d float array.
@@ -340,15 +381,15 @@
     res = np.zeros_like(arr)
     for i in prange(arr.shape[0]):
         res[i] = dcm[i] @ arr[i, :]
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def _transpose_multi(dcm: np.ndarray) -> ndarray:
+def _transpose_multi(dcm: ndarray) -> ndarray:
     N = dcm.shape[0]
     res = np.zeros_like(dcm)
     for i in prange(N):
         res[i] = dcm[i].T
     return res
```

### Comparing `neumann-1.0.4/src/neumann/linalg/vector.py` & `neumann-1.0.5/src/neumann/linalg/vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from copy import deepcopy as dcopy
 
-import numpy as np
 from numpy import ndarray
 import numbers
 
-from .utils import _show_vector, _show_vectors
+from .utils import show_vector
 from .frame import ReferenceFrame as Frame
 from .abstract import AbstractTensor
 
 
 __all__ = ["Vector"]
 
 
@@ -31,14 +30,15 @@
     kwargs : dict, Optional
         Keyword arguments forwarded to `numpy.ndarray`.
 
     Examples
     --------
     Import the necessary classes:
 
+    >>> import numpy as np
     >>> from neumann.linalg import Vector, ReferenceFrame
 
     Create a default frame in 3d space, and create 2 others, each
     being rotated with 30 degrees around the third axis.
 
     >>> A = ReferenceFrame(dim=3)
     >>> B = A.orient_new('Body', [0, 0, 30*np.pi/180], 'XYZ')
@@ -128,18 +128,15 @@
             The components of the vector in a specified frame, or
             the ambient frame, depending on the arguments.
         """
         if not isinstance(dcm, ndarray):
             if target is None:
                 target = self._frame_cls_(dim=self._array.shape[-1])
             dcm = self.frame.dcm(target=target)
-        if len(self.array.shape) == 1:
-            return _show_vector(dcm, self.array)  # dcm @ arr
-        else:
-            return _show_vectors(dcm, self.array)  # dcm @ arr
+        return show_vector(dcm, self.array)  # dcm @ arr
 
     def orient(self, *args, dcm: ndarray = None, **kwargs) -> "Vector":
         """
         Orients the vector inplace. If the transformation is not specified by 'dcm',
         all arguments are forwarded to `orient_new`.
 
         Parameters
@@ -155,17 +152,25 @@
         See Also
         --------
         :func:`orient_new`
         """
         if not isinstance(dcm, ndarray):
             fcls = self.__class__._frame_cls_
             dcm = fcls.eye(dim=len(self)).orient_new(*args, **kwargs).dcm()
-            self.array = dcm.T @ self._array
+            #self.array = dcm.T @ self._array
+            self.array = show_vector(dcm.T, self.array)
+            #self.array = np.linalg.inv(dcm) @ self._array
+            # FIXME check this
         else:
-            self.array = np.linalg.inv(dcm) @ self._array
+            self.array = show_vector(dcm.T, self.array)
+            #self.array = dcm.T @ self._array
+            # FIXME check if inversion is necessary here
+            # inversion might be necessary here because it is uncertain if the
+            # dcm matrix was fabricated properly.
+            #self.array = np.linalg.inv(dcm) @ self._array
         return self
 
     def orient_new(self, *args, **kwargs) -> "Vector":
         """
         Returns a transformed version of the instance.
 
         Returns
@@ -176,14 +181,16 @@
         See Also
         --------
         :func:`orient`
         """
         fcls = self.__class__._frame_cls_
         dcm = fcls.eye(dim=len(self)).orient_new(*args, **kwargs).dcm()
         array = dcm.T @ self._array
+        # FIXME check if inversion is necessary or not
+        #array = np.linalg.inv(dcm) @ self._array
         return Vector(array, frame=self.frame)
 
     def copy(self, deep: bool = False, name: str = None) -> "Vector":
         """
         Returns a shallow or deep copy of this object, depending of the
         argument `deepcopy` (default is False).
         """
```

### Comparing `neumann-1.0.4/src/neumann/logical.py` & `neumann-1.0.5/src/neumann/logical.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/numint.py` & `neumann-1.0.5/src/neumann/numint.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/optimize/ga.py` & `neumann-1.0.5/src/neumann/optimize/ga.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/optimize/lp.py` & `neumann-1.0.5/src/neumann/optimize/lp.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/topology/graph.py` & `neumann-1.0.5/src/neumann/topology/graph.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann/utils.py` & `neumann-1.0.5/src/neumann/utils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.4/src/neumann.egg-info/PKG-INFO` & `neumann-1.0.5/src/neumann.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neumann
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Home-page: https://github.com/dewloosh/Neumann
-Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.4.zip
+Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.5.zip
 Author: Bence Balogh
 Author-email: dewloosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

