# Comparing `tmp/sigmaepsilon-0.0.32.tar.gz` & `tmp/sigmaepsilon-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon-0.0.32.tar", last modified: Tue Apr 11 18:41:09 2023, max compression
+gzip compressed data, was "sigmaepsilon-0.0.33.tar", last modified: Fri Apr 14 23:55:40 2023, max compression
```

## Comparing `sigmaepsilon-0.0.32.tar` & `sigmaepsilon-0.0.33.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.837811 sigmaepsilon-0.0.32/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36022 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-11 18:41:09.837811 sigmaepsilon-0.0.32/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3777 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-11 18:41:09.837811 sigmaepsilon-0.0.32/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2229 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.817811 sigmaepsilon-0.0.32/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.821811 sigmaepsilon-0.0.32/src/sigmaepsilon/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      345 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.821811 sigmaepsilon-0.0.32/src/sigmaepsilon/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/core/material.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.825811 sigmaepsilon-0.0.32/src/sigmaepsilon/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/examples/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/examples/downloads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3046 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/examples/examples.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.825811 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/Q5V.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11142 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/andes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14798 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/bernoulli2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/bernoulli3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11203 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/celldata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/cst.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46938 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/elem.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/gen/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/gen/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7675 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/gen/b2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9905 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/gen/b3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/lst.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6554 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1134 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/wedge.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/dofmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12459 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11699 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/femsolver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/linemesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5804 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/beam.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/membrane.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2844 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/mindlinplate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/mindlinshell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/solid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3687 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/solid3d.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2372 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/surface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/mesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/metamesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7644 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/pointdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19982 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/structure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fem/surfacemesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/beam.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16520 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/loads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3264 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/plate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15433 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11996 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/preproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/problem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2355 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/proc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/material/beam/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/beam/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/material/beam/bernoulli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/beam/bernoulli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7415 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/beam/bernoulli/section.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.829811 sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5160 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/rve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6183 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2723 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/sym.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1504 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/tensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14057 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4212 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/membrane.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5730 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10528 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/mindlin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/joint/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/joint/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18323 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/joint/cubejoint.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8481 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/oc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.833811 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9073 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/cells/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10935 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/cells/cells.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7332 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/dyn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6038 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/eigsolve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16553 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/fem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7213 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/imap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8165 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/linsolve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6541 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17705 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/preproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4588 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/tr.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.837811 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2316 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2123 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/hmh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/material.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8490 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/mindlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10269 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4180 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/surface.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.821811 sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-11 18:41:09.000000 sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4156 2023-04-11 18:41:09.000000 sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-11 18:41:09.000000 sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-11 18:41:09.000000 sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-04-11 18:41:09.000000 sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-11 18:41:09.000000 sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/test-requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 18:41:09.837811 sigmaepsilon-0.0.32/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33548 2023-04-11 18:41:04.000000 sigmaepsilon-0.0.32/tests/test_bernoulli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:40.001651 sigmaepsilon-0.0.33/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36022 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-14 23:55:40.001651 sigmaepsilon-0.0.33/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3777 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-14 23:55:40.001651 sigmaepsilon-0.0.33/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2229 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.981650 sigmaepsilon-0.0.33/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.985651 sigmaepsilon-0.0.33/src/sigmaepsilon/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      345 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.985651 sigmaepsilon-0.0.33/src/sigmaepsilon/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/core/material.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.985651 sigmaepsilon-0.0.33/src/sigmaepsilon/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/examples/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/examples/downloads.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3046 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/examples/examples.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.989651 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.989651 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/Q5V.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11142 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/andes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14798 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/bernoulli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/bernoulli2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/bernoulli3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11203 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/celldata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/cst.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    46938 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/elem.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.993651 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/gen/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/gen/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7675 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/gen/b2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9905 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/gen/b3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/lst.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6554 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1134 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/wedge.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/dofmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12459 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/ebc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11699 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/femsolver.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/linemesh.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.993651 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5804 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/beam.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/membrane.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2844 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/mindlinplate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/mindlinshell.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/solid.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3687 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/solid3d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2372 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/surface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/mesh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/metamesh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7644 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/pointdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19982 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/structure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fem/surfacemesh.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.993651 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/beam.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16520 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/loads.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3264 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/plate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15433 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11996 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/preproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/problem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2355 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/proc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.993651 sigmaepsilon-0.0.33/src/sigmaepsilon/material/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.993651 sigmaepsilon-0.0.33/src/sigmaepsilon/material/beam/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/beam/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.993651 sigmaepsilon-0.0.33/src/sigmaepsilon/material/beam/bernoulli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/beam/bernoulli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7415 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/beam/bernoulli/section.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.993651 sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/ebc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5160 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/rve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6183 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2723 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/sym.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1504 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/tensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14057 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4212 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/membrane.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5730 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10528 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/mindlin.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/joint/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/joint/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18323 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/joint/cubejoint.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8481 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/oc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.997651 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9073 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/cells/bernoulli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10935 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/cells/cells.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7332 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/dyn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/ebc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6038 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/eigsolve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16553 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/fem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7213 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/imap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8165 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/linsolve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6541 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17705 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/preproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4588 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/tr.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:40.001651 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2316 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/bernoulli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2123 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/hmh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/material.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8490 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/mindlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10269 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4180 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/surface.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:39.985651 sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-14 23:55:39.000000 sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4156 2023-04-14 23:55:39.000000 sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 23:55:39.000000 sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 23:55:39.000000 sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-04-14 23:55:39.000000 sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-14 23:55:39.000000 sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/test-requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 23:55:40.001651 sigmaepsilon-0.0.33/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33548 2023-04-14 23:55:34.000000 sigmaepsilon-0.0.33/tests/test_bernoulli.py
```

### Comparing `sigmaepsilon-0.0.32/LICENSE` & `sigmaepsilon-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/PKG-INFO` & `sigmaepsilon-0.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon
-Version: 0.0.32
+Version: 0.0.33
 Summary: High-Performance Computational Mechanics in Python.
 Home-page: https://github.com/dewloosh/sigmaepsilon
-Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.32.zip
+Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.33.zip
 Author: Bence Balogh
 Author-email: benceeok@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sigmaepsilon-0.0.32/README.md` & `sigmaepsilon-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/setup.py` & `sigmaepsilon-0.0.33/setup.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/examples/downloads.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/examples/examples.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/examples/examples.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/Q5V.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/Q5V.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/__init__.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/andes.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/andes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/bernoulli.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/bernoulli.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/bernoulli2.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/bernoulli2.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/bernoulli3.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/bernoulli3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/celldata.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/celldata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/cst.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/cst.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/elem.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/elem.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/gen/b2.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/gen/b2.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/gen/b3.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/gen/b3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/lst.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/lst.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/meta.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/meta.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/q4.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/q4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/cells/q9.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/cells/q9.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/dofmap.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/dofmap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/ebc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/ebc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/femsolver.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/femsolver.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/linemesh.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/linemesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/beam.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/beam.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/membrane.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/membrane.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/mindlinplate.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/mindlinplate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/mindlinshell.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/mindlinshell.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/solid.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/solid.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/solid3d.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/solid3d.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/material/surface.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/material/surface.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/mesh.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/mesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/metamesh.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/metamesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/pointdata.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/pointdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/structure.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/structure.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fem/surfacemesh.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fem/surfacemesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/beam.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/beam.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/loads.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/loads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/plate.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/plate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/postproc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/preproc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/preproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/proc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/proc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/fourier/utils.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/fourier/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/beam/bernoulli/section.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/beam/bernoulli/section.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/ebc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/ebc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/rve.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/rve.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/homg/utils.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/homg/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/sym.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/sym.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/tensor.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/tensor.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/hooke/utils.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/hooke/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/membrane.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/membrane.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/meta.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/meta.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/material/surface/mindlin.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/material/surface/mindlin.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/joint/cubejoint.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/joint/cubejoint.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/filter.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/filter.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/oc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/oc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/topopt/oc/utils.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/topopt/oc/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/cells/bernoulli.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/cells/bernoulli.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/cells/cells.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/cells/cells.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/dyn.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/dyn.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/ebc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/ebc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/eigsolve.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/eigsolve.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/fem.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/fem.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/imap.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/imap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/linsolve.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/linsolve.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/postproc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/preproc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/preproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/fem/tr.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/fem/tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/bernoulli.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/bernoulli.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/hmh.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/hmh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/material.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/material.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/mindlin.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/mindlin.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/postproc.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon/utils/material/surface.py` & `sigmaepsilon-0.0.33/src/sigmaepsilon/utils/material/surface.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/PKG-INFO` & `sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon
-Version: 0.0.32
+Version: 0.0.33
 Summary: High-Performance Computational Mechanics in Python.
 Home-page: https://github.com/dewloosh/sigmaepsilon
-Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.32.zip
+Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.33.zip
 Author: Bence Balogh
 Author-email: benceeok@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sigmaepsilon-0.0.32/src/sigmaepsilon.egg-info/SOURCES.txt` & `sigmaepsilon-0.0.33/src/sigmaepsilon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.32/tests/test_bernoulli.py` & `sigmaepsilon-0.0.33/tests/test_bernoulli.py`

 * *Files identical despite different names*

