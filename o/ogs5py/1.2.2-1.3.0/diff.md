# Comparing `tmp/ogs5py-1.2.2.tar.gz` & `tmp/ogs5py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogs5py-1.2.2.tar", last modified: Wed May 25 19:41:31 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ogs5py-1.2.2.tar` & `ogs5py-1.3.0.tar`

### file list

```diff
@@ -1,118 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-05-25 19:40:31.000000 ogs5py-1.2.2/AUTHORS.md
--rwxr-xr-x   0 runner    (1001) docker     (121)    13147 2022-05-25 19:40:31.000000 ogs5py-1.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-05-25 19:40:31.000000 ogs5py-1.2.2/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-05-25 19:40:31.000000 ogs5py-1.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-05-25 19:40:31.000000 ogs5py-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-25 19:40:31.000000 ogs5py-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8124 2022-05-25 19:41:31.883388 ogs5py-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6062 2022-05-25 19:40:31.000000 ogs5py-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.875387 ogs5py-1.2.2/ogs5py/
--rw-r--r--   0 runner    (1001) docker     (121)     3269 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-25 19:41:30.000000 ogs5py-1.2.2/ogs5py/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.875387 ogs5py-1.2.2/ogs5py/fileclasses/
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.875387 ogs5py-1.2.2/ogs5py/fileclasses/asc/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/asc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/asc/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    40859 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/bc/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/bc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/bc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/cct/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/cct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/cct/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/ddc/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/ddc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3019 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/ddc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/fct/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/fct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/fct/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/gem/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/gem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10233 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/gem/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/gli/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/gli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20629 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/gli/checker.py
--rw-r--r--   0 runner    (1001) docker     (121)    34179 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/gli/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     6427 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/gli/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    16231 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/gli/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/ic/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/ic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10359 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/ic/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/krc/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/krc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6030 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/krc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/mcp/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mcp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/mfp/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mfp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mfp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/mmp/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mmp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/mpd/
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/mpd/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/msh/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14702 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/checker.py
--rw-r--r--   0 runner    (1001) docker     (121)    42007 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    19335 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9354 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/gmsh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3035 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    31001 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/msh_io.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14941 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msh/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/msp/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/msp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.879387 ogs5py-1.2.2/ogs5py/fileclasses/num/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/num/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/num/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/out/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/out/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/out/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/pcs/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/pcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/pcs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/pct/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/pct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/pct/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/pqc/
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/pqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/pqc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/rei/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/rei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/rei/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/rfd/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/rfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/rfd/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/st/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/st/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/fileclasses/tim/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/tim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/fileclasses/tim/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    43016 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/ogs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/reader/
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17774 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/reader/techelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/reader/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     6262 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/reader/vtkhelper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4990 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/tools/download.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14227 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/tools/output.py
--rw-r--r--   0 runner    (1001) docker     (121)    10804 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/tools/script.py
--rw-r--r--   0 runner    (1001) docker     (121)    31826 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     8530 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/tools/types.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1621 2022-05-25 19:40:31.000000 ogs5py-1.2.2/ogs5py/tools/vtk_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/ogs5py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-05-25 19:41:31.000000 ogs5py-1.2.2/ogs5py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-05-25 19:40:31.000000 ogs5py-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-05-25 19:41:31.887388 ogs5py-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 19:41:31.883388 ogs5py-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5390 2022-05-25 19:40:31.000000 ogs5py-1.2.2/tests/test_ogs5py.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/_version.py
+-rw-r--r--   0        0        0    42931 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/ogs.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/__init__.py
+-rw-r--r--   0        0        0    40857 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/base.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/asc/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/asc/core.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/bc/__init__.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/bc/core.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/cct/__init__.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/cct/core.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/ddc/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/ddc/core.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/fct/__init__.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/fct/core.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/gem/__init__.py
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/gem/core.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/gli/__init__.py
+-rw-r--r--   0        0        0    20629 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/gli/checker.py
+-rw-r--r--   0        0        0    34182 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/gli/core.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/gli/generator.py
+-rw-r--r--   0        0        0    16231 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/gli/tools.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/ic/__init__.py
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/ic/core.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/krc/__init__.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/krc/core.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mcp/__init__.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mcp/core.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mfp/__init__.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mfp/core.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mmp/__init__.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mmp/core.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mpd/__init__.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/mpd/core.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/__init__.py
+-rw-r--r--   0        0        0    14702 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/checker.py
+-rw-r--r--   0        0        0    42010 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/core.py
+-rw-r--r--   0        0        0    19313 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/generator.py
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/gmsh.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/helpers.py
+-rwxr-xr-x   0        0        0    30999 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/msh_io.py
+-rwxr-xr-x   0        0        0    14941 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/tools.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msh/viewer.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msp/__init__.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/msp/core.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/num/__init__.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/num/core.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/out/__init__.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/out/core.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/pcs/__init__.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/pcs/core.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/pct/__init__.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/pct/core.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/pqc/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/pqc/core.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/rei/__init__.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/rei/core.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/rfd/__init__.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/rfd/core.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/st/__init__.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/st/core.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/tim/__init__.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/fileclasses/tim/core.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/reader/__init__.py
+-rw-r--r--   0        0        0    17774 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/reader/reader.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/reader/techelper.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/reader/tools.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/reader/vtkhelper.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/tools/__init__.py
+-rwxr-xr-x   0        0        0     4974 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/tools/download.py
+-rwxr-xr-x   0        0        0    14394 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/tools/output.py
+-rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/tools/script.py
+-rw-r--r--   0        0        0    31784 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/tools/tools.py
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/tools/types.py
+-rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 ogs5py-1.3.0/src/ogs5py/tools/vtk_viewer.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 ogs5py-1.3.0/tests/test_ogs5py.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 ogs5py-1.3.0/.gitignore
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 ogs5py-1.3.0/AUTHORS.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ogs5py-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 ogs5py-1.3.0/README.md
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 ogs5py-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 ogs5py-1.3.0/PKG-INFO
```

### Comparing `ogs5py-1.2.2/LICENSE` & `ogs5py-1.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2019 Sebastian Mueller
+Copyright (c) 2023 Sebastian Mueller
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ogs5py-1.2.2/PKG-INFO` & `ogs5py-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 Metadata-Version: 2.1
 Name: ogs5py
-Version: 1.2.2
+Version: 1.3.0
 Summary: ogs5py: a python API for OpenGeoSys5
-Home-page: https://github.com/GeoStat-Framework/ogs5py
-Author: Sebastian Müller, Falk Heße
-Author-email: info@geostat-framework.org
-Maintainer: Sebastian Müller
-Maintainer-email: info@geostat-framework.org
-License: MIT
 Project-URL: Homepage, https://geostat-framework.org/#ogs5py
 Project-URL: Documentation, https://ogs5py.readthedocs.io
 Project-URL: Source, https://github.com/GeoStat-Framework/ogs5py
 Project-URL: Tracker, https://github.com/GeoStat-Framework/ogs5py/issues
 Project-URL: Changelog, https://github.com/GeoStat-Framework/ogs5py/blob/main/CHANGELOG.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/ogs5py
-Platform: any
+Author-email: "Sebastian Müller, Falk Heße" <info@geostat-framework.org>
+License-Expression: MIT
+License-File: AUTHORS.md
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Requires-Python: >=3.7
+Requires-Dist: lxml>=4
+Requires-Dist: meshio>=4
+Requires-Dist: numpy>=1.14.5
+Requires-Dist: pandas>=0.23.2
+Requires-Dist: pexpect>=4
+Requires-Dist: vtk>=9
+Provides-Extra: check
+Requires-Dist: black<24,>=23; extra == 'check'
+Requires-Dist: isort[colors]<6; extra == 'check'
 Provides-Extra: doc
-Provides-Extra: show
+Requires-Dist: m2r2>=0.2.8; extra == 'doc'
+Requires-Dist: numpydoc>=1.1; extra == 'doc'
+Requires-Dist: sphinx-rtd-theme>=1; extra == 'doc'
+Requires-Dist: sphinx>=4; extra == 'doc'
 Provides-Extra: gmsh
+Requires-Dist: gmsh; extra == 'gmsh'
+Provides-Extra: show
+Requires-Dist: mayavi; extra == 'show'
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest-cov>=3; extra == 'test'
+Description-Content-Type: text/markdown
 
 # Welcome to ogs5py
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2546767.svg)](https://doi.org/10.5281/zenodo.2546767)
 [![PyPI version](https://badge.fury.io/py/ogs5py.svg)](https://badge.fury.io/py/ogs5py)
 [![Continuous Integration](https://github.com/GeoStat-Framework/ogs5py/actions/workflows/main.yml/badge.svg)](https://github.com/GeoStat-Framework/ogs5py/actions/workflows/main.yml)
 [![Coverage Status](https://coveralls.io/repos/github/GeoStat-Framework/ogs5py/badge.svg?branch=main)](https://coveralls.io/github/GeoStat-Framework/ogs5py?branch=main)
@@ -223,15 +235,15 @@
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[MIT][gpl_link] © 2018-2022 (inspired by Falk Hesse and Miao Jing)
+[MIT][gpl_link] © 2018-2023 (inspired by Falk Hesse and Miao Jing)
 
 This project is based on [OGSPY][ogspy_link].
 
 [ogspy_link]: https://github.com/fhesze/OGSPY
 [gpl_link]: https://github.com/GeoStat-Framework/ogs5py/blob/main/LICENSE
 [ogs5_link]: https://www.opengeosys.org/ogs-5/
 [doc_link]: https://ogs5py.readthedocs.io/
```

### Comparing `ogs5py-1.2.2/README.md` & `ogs5py-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[MIT][gpl_link] © 2018-2022 (inspired by Falk Hesse and Miao Jing)
+[MIT][gpl_link] © 2018-2023 (inspired by Falk Hesse and Miao Jing)
 
 This project is based on [OGSPY][ogspy_link].
 
 [ogspy_link]: https://github.com/fhesze/OGSPY
 [gpl_link]: https://github.com/GeoStat-Framework/ogs5py/blob/main/LICENSE
 [ogs5_link]: https://www.opengeosys.org/ogs-5/
 [doc_link]: https://ogs5py.readthedocs.io/
```

### Comparing `ogs5py-1.2.2/ogs5py/__init__.py` & `ogs5py-1.3.0/src/ogs5py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 
 The following functionalities are directly provided on module-level.
 
 Subpackages
 ===========
 
 .. autosummary::
-    fileclasses
-    reader
-    tools
+   :toctree: api
+
+   fileclasses
+   reader
+   tools
 
 Classes
 =======
 
 OGS model Base Class
 ^^^^^^^^^^^^^^^^^^^^
 Class to setup an ogs model
 
 .. autosummary::
-   :toctree: generated
+   :toctree: api
 
    OGS
 
 File Classes
 ^^^^^^^^^^^^
 Classes for all OGS5 Files. See: :any:`ogs5py.fileclasses`
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/__init__.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 
 .. currentmodule:: ogs5py.fileclasses
 
 Subpackages
 ^^^^^^^^^^^
 
 .. autosummary::
+   :toctree:
+
    base
    gli
    msh
 
 File Classes
 ^^^^^^^^^^^^
 Classes for all OGS5 Files
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    ASC
    BC
    CCT
    DDC
    FCT
    GEM
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/asc/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/asc/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/base.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 .. currentmodule:: ogs5py.fileclasses.base
 
 File Classes
 ^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    File
    LineFile
    BlockFile
    MultiFile
 
 ----
@@ -496,15 +496,15 @@
                 + ": get_block - block has no unique sub-keys and can not be "
                 + "represented as dict."
             )
 
         return main_key, sub_key, cont
 
     def update_block(self, index=None, main_key=None, **block):
-        """
+        r"""
         Update a Block from the actual file.
 
         Parameters
         ----------
         index : int or None, optional
             Positional index of the block of interest. As default, the last
             one is used. Default: None
@@ -532,15 +532,15 @@
         upd_block.update(block)
         # remove the old one
         self.del_main_keyword(main_index=index, del_all=False)
         # set the updated one
         self.add_block(index=index, **upd_block)
 
     def add_block(self, index=None, main_key=None, **block):
-        """
+        r"""
         Add a new Block to the actual file.
 
         Keywords are the sub keywords of the actual file type:
 
         #MAIN_KEY
          $SUBKEY1
           content1 ...
@@ -613,15 +613,15 @@
         for skey in self.SKEYS[mindex]:
             if skey not in block:
                 continue
             self.add_sub_keyword(skey, main_index=index)
             self.add_multi_content(block[skey], main_index=index)
 
     def append_to_block(self, index=None, **block):
-        """
+        r"""
         Append data to an existing Block in the actual file.
 
         Keywords are the sub keywords of the actual file type:
 
         #MAIN_KEY
          $SUBKEY1
           content1 ...
@@ -1121,15 +1121,15 @@
                     out += CON_IND + " ...\n"
         if self.mainkw:
             out += "#STOP"
         return out
 
 
 class MultiFile:
-    """
+    r"""
     Class holding mulitple files of the same type.
 
     Parameters
     ----------
     base : :class:`object`
         Base class for the files
     **standard
@@ -1178,15 +1178,15 @@
     def __getattr__(self, attr):
         """Pretend to be actual File."""
         if self.id is not None:
             return getattr(self[self.id], attr)
         return None
 
     def add(self, *args, **kwargs):
-        """Add a new instance of the base class with *args and **kwargs."""
+        r"""Add a new instance of the base class with given args and kwargs."""
         kw = copy.deepcopy(self.standard)
         kw.update(kwargs)
         self.append(self._base(*args, **kw))
 
     def append(self, file):
         """Append a new file to the list."""
         self._list.append(file)
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/bc/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/bc/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/cct/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/cct/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/ddc/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/ddc/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/fct/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/fct/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/gem/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/gem/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/gli/checker.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/gli/checker.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/gli/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/gli/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,15 +477,15 @@
         """
         self.POINTS = shift_points(self.POINTS, vector)
 
     def generate(self, generator="rectangular", **kwargs):
         """
         Use a gli-generator from the generator module.
 
-        See: :any:`ogs5py.fileclasses.gli.generator`
+        See: :py:mod:`ogs5py.fileclasses.gli.generator`
 
         Parameters
         ----------
         generator : str
             set the generator from the generator module
         **kwargs
             kwargs will be forwarded to the generator in use
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/gli/generator.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/gli/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 .. currentmodule:: ogs5py.fileclasses.gli.generator
 
 Generators
 ^^^^^^^^^^
 These generators can be called with :any:`GLI.generate`
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    rectangular
    radial
 
 ----
 """
 import numpy as np
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/gli/tools.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/gli/tools.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/ic/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/ic/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/krc/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/krc/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/mcp/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/mcp/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/mfp/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/mfp/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/mmp/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/mmp/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/mpd/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/mpd/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/checker.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/checker.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -996,15 +996,15 @@
         """
         remove_dim(self._dict, remove=remove)
 
     def generate(self, generator="rectangular", **kwargs):
         """
         Use a mesh-generator from the generator module.
 
-        See: :any:`ogs5py.fileclasses.msh.generator`
+        See: :py:mod:`ogs5py.fileclasses.msh.generator`
 
         Parameters
         ----------
         generator : str
             set the generator from the generator module
         **kwargs
             kwargs will be forwarded to the generator in use
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/generator.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 .. currentmodule:: ogs5py.fileclasses.msh.generator
 
 Generators
 ^^^^^^^^^^
 These generators can be called with :any:`MSH.generate`
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    rectangular
    radial
    grid_adapter2D
    grid_adapter3D
    block_adapter3D
    gmsh
@@ -241,17 +241,17 @@
     lay_no = r_no * angles
 
     if dim == 2:
         node_no = angles * r_no
         element_no = angles * (r_no - 1)
         if closed:
             node_no += 1
-            elem_mid_arr = np.zeros((angles, 3), dtype=np.int)
+            elem_mid_arr = np.zeros((angles, 3), dtype=int)
 
-        element_arr = np.zeros((element_no, 4), dtype=np.int)
+        element_arr = np.zeros((element_no, 4), dtype=int)
         node_arr = np.zeros((node_no, 3))
 
         for ri, re in enumerate(rad):
             for n in range(angles):
                 no = n + ri * angles
                 node_arr[no, :] = [
                     x0 + re * np.cos(n / angles * 2 * np.pi),
@@ -275,17 +275,17 @@
             element_dict["tri"] = elem_mid_arr
 
     elif dim == 3:
         node_no = angles * r_no * z_no
         element_no = angles * (r_no - 1) * (z_no - 1)
         if closed:
             node_no += z_no
-            elem_mid_arr = np.zeros((angles * (z_no - 1), 6), dtype=np.int)
+            elem_mid_arr = np.zeros((angles * (z_no - 1), 6), dtype=int)
 
-        element_arr = np.zeros((element_no, 8), dtype=np.int)
+        element_arr = np.zeros((element_no, 8), dtype=int)
         node_arr = np.zeros((node_no, 3))
 
         # write nodes
         for z in range(z_no):
             for ri, re in enumerate(rad):
                 for n in range(angles):
                     no = n + ri * angles + z * r_no * angles
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/gmsh.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/gmsh.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/helpers.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/helpers.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/msh_io.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/msh_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,14 @@
 
     import pandas as pd
 
     # initilize the output
     out = dcp(EMPTY_MSH)
 
     with open(filepath, "r", encoding=encoding) as msh:
-
         head = msh.readline()
         if head.strip().startswith("#0#0#0#1#"):
             if verbose:
                 print("got right header:")
                 print(head)
             # first line should contain 3 numbers: 0 no_nodes no_elements
             line = msh.readline()
@@ -439,15 +438,14 @@
     with open(filepath, "w") as msh:
         if top_com:
             if verbose:
                 print("write top comment")
             print(str(top_com), file=msh)
 
         for i, mesh_i in enumerate(mesh):
-
             if verbose:
                 print("write 'FEM_MSH' number: " + str(i))
             msh.write("#FEM_MSH\n")
 
             for key in mesh_i["mesh_data"]:
                 if verbose:
                     print("write " + key)
```

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/tools.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/tools.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msh/viewer.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msh/viewer.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/msp/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/msp/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/num/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/num/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/out/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/out/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/pcs/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/pcs/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/pct/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/pct/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/pqc/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/pqc/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/rei/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/rei/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/rfd/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/rfd/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/st/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/st/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/fileclasses/tim/core.py` & `ogs5py-1.3.0/src/ogs5py/fileclasses/tim/core.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/ogs.py` & `ogs5py-1.3.0/src/ogs5py/ogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,9 @@
 # -*- coding: utf-8 -*-
-"""
-Base Class for an OGS5 run.
-
-.. currentmodule:: ogs5py.ogs
-
-OGS Class
-^^^^^^^^^
-
-.. autosummary::
-
-   OGS
-
-----
-"""
+"""Base Class for an OGS5 run."""
 import glob
 import os
 import shutil
 import sys
 import time
 import warnings
 from copy import deepcopy as dcp
@@ -1018,15 +1005,15 @@
 
         Parameters
         ----------
         pcs : string or None, optional
             specify the PCS type that should be collected
             Possible values are:
 
-                - None/"" (no PCS_TYPE specified in *.out)
+                - None/"" (no PCS_TYPE specified in \*.out)
                 - "NO_PCS"
                 - "GROUNDWATER_FLOW"
                 - "LIQUID_FLOW"
                 - "RICHARDS_FLOW"
                 - "AIR_FLOW"
                 - "MULTI_PHASE_FLOW"
                 - "PS_GLOBAL"
```

### Comparing `ogs5py-1.2.2/ogs5py/reader/reader.py` & `ogs5py-1.3.0/src/ogs5py/reader/reader.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/reader/techelper.py` & `ogs5py-1.3.0/src/ogs5py/reader/techelper.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/reader/tools.py` & `ogs5py-1.3.0/src/ogs5py/reader/tools.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/reader/vtkhelper.py` & `ogs5py-1.3.0/src/ogs5py/reader/vtkhelper.py`

 * *Files identical despite different names*

### Comparing `ogs5py-1.2.2/ogs5py/tools/download.py` & `ogs5py-1.3.0/src/ogs5py/tools/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 
 Downloader
 ^^^^^^^^^^
 
 A downloading routine to get the OSG5 executable.
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    download_ogs
    add_exe
    reset_download
    OGS5PY_CONFIG
-
-----
 """
 import os
 import platform
 import shutil
 import tarfile
 import zipfile
 from tempfile import TemporaryDirectory
```

### Comparing `ogs5py-1.2.2/ogs5py/tools/output.py` & `ogs5py-1.3.0/src/ogs5py/tools/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # -*- coding: utf-8 -*-
-"""Tools for ogs5py output files (independent from VTK package)."""
+"""
+Tools for ogs5py output files (independent from VTK package).
+
+.. currentmodule:: ogs5py.tools.output
+
+Helpers
+^^^^^^^
+
+.. autosummary::
+   :toctree:
+
+   get_output_files
+   readpvd_single
+   split_ply_path
+   split_pnt_path
+"""
 import glob
 import os
 import re
 import xml.etree.ElementTree as ET
 
 import numpy as np
 
@@ -284,28 +299,28 @@
     output["pvd_info"] = pvd_info
     output["files"] = files
     output["infos"] = infos
     return output
 
 
 def get_output_files(task_root, task_id, pcs=None, typ="VTK", element=None):
-    """
+    r"""
     Get a list of output file paths.
 
     Parameters
     ----------
     task_root : string
         string containing the path to the directory containing the ogs output
     task_id : string
         string containing the file name of the ogs task without extension
     pcs : string or None, optional
         specify the PCS type that should be collected
         Possible values are:
 
-            - None/"" (no PCS_TYPE specified in *.out)
+            - None/"" (no PCS_TYPE specified in \*.out)
             - "NO_PCS"
             - "GROUNDWATER_FLOW"
             - "LIQUID_FLOW"
             - "RICHARDS_FLOW"
             - "AIR_FLOW"
             - "MULTI_PHASE_FLOW"
             - "PS_GLOBAL"
```

### Comparing `ogs5py-1.2.2/ogs5py/tools/script.py` & `ogs5py-1.3.0/src/ogs5py/tools/script.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,30 @@
 
 .. currentmodule:: ogs5py.tools.script
 
 Generator
 ^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    gen_script
 
 Helpers
 ^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    formater
    get_line
    tab
    add_block_file
    add_load_file
    add_list_file
-
-----
 """
 import os
 import shutil
 
 from ogs5py.fileclasses.base import BlockFile
 from ogs5py.tools.types import MULTI_FILES, OGS_EXT, STRTYPE
```

### Comparing `ogs5py-1.2.2/ogs5py/tools/tools.py` & `ogs5py-1.3.0/src/ogs5py/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 .. currentmodule:: ogs5py.tools.tools
 
 Classes
 ^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    Output
 
 File related
 ^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    search_mkey
    uncomment
    is_key
    is_mkey
    is_skey
    get_key
@@ -33,37 +33,35 @@
    split_file_path
    is_str_array
 
 Geometric tools
 ^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    rotate_points
    shift_points
    transform_points
    hull_deform
    rotation_matrix
    volume
    centroid
 
 Array tools
 ^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    unique_rows
    replace
    by_id
    specialrange
    generate_time
-
-----
 """
 import ast
 import collections
 import glob
 import itertools
 import os
 import sys
@@ -311,15 +309,15 @@
     content : anything
         Single object, or list of objects, or list of lists of objects.
     """
     # strings could be detected as iterable, so check this first
     if isinstance(content, STRTYPE):
         return [[content]]
     # convert iterators (like zip)
-    if isinstance(content, collections.Iterator):
+    if isinstance(content, collections.abc.Iterator):
         content = list(content)
     # check for a single content thats not a string
     try:
         iter(content)
     except TypeError:
         return [[content]]
     # check if any list in in the given list
```

### Comparing `ogs5py-1.2.2/ogs5py/tools/types.py` & `ogs5py-1.3.0/src/ogs5py/tools/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,14 +50,89 @@
    PCS_TYP
    PCS_EXT
    PRIM_VAR
    PRIM_VAR_BY_PCS
    OGS_EXT
    MULTI_FILES
 
+----
+
+.. autodata:: EMPTY_GLI
+
+.. autodata:: GLI_KEYS
+
+.. autodata:: GLI_KEY_LIST
+
+.. autodata:: EMPTY_PLY
+
+.. autodata:: PLY_KEYS
+
+.. autodata:: PLY_KEY_LIST
+
+.. autodata:: PLY_TYPES
+
+.. autodata:: EMPTY_SRF
+
+.. autodata:: SRF_KEYS
+
+.. autodata:: SRF_KEY_LIST
+
+.. autodata:: SRF_TYPES
+
+.. autodata:: EMPTY_VOL
+
+.. autodata:: VOL_KEYS
+
+.. autodata:: VOL_KEY_LIST
+
+.. autodata:: VOL_TYPES
+
+.. autodata:: EMPTY_MSH
+
+.. autodata:: MESH_KEYS
+
+.. autodata:: MESH_DATA_KEYS
+
+.. autodata:: ELEM_1D
+
+.. autodata:: ELEM_2D
+
+.. autodata:: ELEM_3D
+
+.. autodata:: ELEM_DIM
+
+.. autodata:: ELEM_NAMES
+
+.. autodata:: ELEM_TYP
+
+.. autodata:: ELEM_TYP1D
+
+.. autodata:: ELEM_TYP2D
+
+.. autodata:: ELEM_TYP3D
+
+.. autodata:: VTK_TYP
+
+.. autodata:: MESHIO_NAMES
+
+.. autodata:: NODE_NO
+
+.. autodata:: STRTYPE
+
+.. autodata:: PCS_TYP
+
+.. autodata:: PCS_EXT
+
+.. autodata:: PRIM_VAR
+
+.. autodata:: PRIM_VAR_BY_PCS
+
+.. autodata:: OGS_EXT
+
+.. autodata:: MULTI_FILES
 """
 import numpy as np
 
 STRTYPE = str
 """type: base string type"""
 
 # keylists for the gli entries and templates for entries
```

### Comparing `ogs5py-1.2.2/ogs5py/tools/vtk_viewer.py` & `ogs5py-1.3.0/src/ogs5py/tools/vtk_viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # -*- coding: utf-8 -*-
-"""Viewer for a vtk file."""
+"""
+Viewer for a vtk file.
+
+.. currentmodule:: ogs5py.tools.vtk_viewer
+
+Viewer
+^^^^^^
+
+.. autosummary::
+   :toctree:
+
+   show_vtk
+"""
 # import os
 # os.environ["QT_API"] = "pyqt"
 # os.environ["ETS_TOOLKIT"] = "qt4"
 
 MAYA_AVAIL = True
 try:
     from mayavi import mlab
```

### Comparing `ogs5py-1.2.2/tests/test_ogs5py.py` & `ogs5py-1.3.0/tests/test_ogs5py.py`

 * *Files identical despite different names*

