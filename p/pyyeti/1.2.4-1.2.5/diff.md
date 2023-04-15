# Comparing `tmp/pyyeti-1.2.4.tar.gz` & `tmp/pyyeti-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyeti-1.2.4.tar", last modified: Mon Apr  3 21:09:53 2023, max compression
+gzip compressed data, was "pyyeti-1.2.5.tar", last modified: Sat Apr 15 20:29:11 2023, max compression
```

## Comparing `pyyeti-1.2.4.tar` & `pyyeti-1.2.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.070954 pyyeti-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-03 21:09:33.000000 pyyeti-1.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-03 21:09:33.000000 pyyeti-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-03 21:09:53.070954 pyyeti-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-03 21:09:33.000000 pyyeti-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.066954 pyyeti-1.2.4/pyyeti/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   105070 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.066954 pyyeti-1.2.4/pyyeti/cla/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/_magpct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/_rptext1.py
--rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/_rptpct1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/_rpttab1.py
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    50972 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/dr_def.py
--rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/dr_event.py
--rw-r--r--   0 runner    (1001) docker     (123)   111221 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/dr_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/dr_results_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cla/rel_disp_dtm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/column_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/cyclecount.py
--rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/datacursor.py
--rw-r--r--   0 runner    (1001) docker     (123)   124529 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    49094 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/era.py
--rw-r--r--   0 runner    (1001) docker     (123)    42901 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/expmint.py
--rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/fdepsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/frclim.py
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/guitools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/locate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.066954 pyyeti-1.2.4/pyyeti/nastran/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/nastran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131262 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/nastran/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)   134540 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/nastran/n2p.py
--rw-r--r--   0 runner    (1001) docker     (123)   120906 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/nastran/op2.py
--rw-r--r--   0 runner    (1001) docker     (123)    91322 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/nastran/op4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.070954 pyyeti-1.2.4/pyyeti/ode/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/_base_ode_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/freqdirect.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/frf_mode_participation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/solvecdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/solveexp1.py
--rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/solveexp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27243 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/solvenewmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    69128 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ode/solveunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/pp.py
--rw-r--r--   0 runner    (1001) docker     (123)    42978 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/psd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.070954 pyyeti-1.2.4/pyyeti/rainflow/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/rainflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/rainflow/c_rain.c
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/rainflow/py_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    74708 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/srs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ssmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-04-03 21:09:33.000000 pyyeti-1.2.4/pyyeti/ytools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.066954 pyyeti-1.2.4/pyyeti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-03 21:09:53.000000 pyyeti-1.2.4/pyyeti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-03 21:09:53.000000 pyyeti-1.2.4/pyyeti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 21:09:53.000000 pyyeti-1.2.4/pyyeti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-03 21:09:53.000000 pyyeti-1.2.4/pyyeti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 21:09:53.000000 pyyeti-1.2.4/pyyeti.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.070954 pyyeti-1.2.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-04-03 21:09:33.000000 pyyeti-1.2.4/scripts/lsop2
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-04-03 21:09:33.000000 pyyeti-1.2.4/scripts/lsop4
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-03 21:09:53.070954 pyyeti-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-03 21:09:33.000000 pyyeti-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.062954 pyyeti-1.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.070954 pyyeti-1.2.4/tests/nas2cam_csuper/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nas2cam_csuper/inboard.asm
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nas2cam_csuper/inboard.op4
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nas2cam_csuper/inboard.pch
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nas2cam_csuper/nas2cam.op2
--rw-r--r--   0 runner    (1001) docker     (123)   147552 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nas2cam_csuper/nas2cam.op4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:09:53.070954 pyyeti-1.2.4/tests/nastran_drm12/
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nastran_drm12/drm12.op2
--rw-r--r--   0 runner    (1001) docker     (123)    77852 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nastran_drm12/drm12.op4
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nastran_drm12/inboard_nas2cam.op2
--rw-r--r--   0 runner    (1001) docker     (123)    51624 2023-04-03 21:09:33.000000 pyyeti-1.2.4/tests/nastran_drm12/inboard_nas2cam.op4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.040841 pyyeti-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-15 20:28:46.000000 pyyeti-1.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-15 20:28:46.000000 pyyeti-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-15 20:29:11.040841 pyyeti-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-15 20:28:46.000000 pyyeti-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.036841 pyyeti-1.2.5/pyyeti/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105070 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.036841 pyyeti-1.2.5/pyyeti/cla/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/_magpct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/_rptext1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/_rptpct1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/_rpttab1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50972 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/dr_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/dr_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111221 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/dr_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/dr_results_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cla/rel_disp_dtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/column_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/cyclecount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/datacursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124529 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49094 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/era.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42901 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/expmint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/fdepsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/frclim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/guitools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/locate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.036841 pyyeti-1.2.5/pyyeti/nastran/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/nastran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131611 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/nastran/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134540 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/nastran/n2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120906 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/nastran/op2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91322 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/nastran/op4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.040841 pyyeti-1.2.5/pyyeti/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/_base_ode_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/freqdirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/frf_mode_participation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/solvecdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/solveexp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/solveexp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27243 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/solvenewmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69128 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ode/solveunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42978 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/psd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.040841 pyyeti-1.2.5/pyyeti/rainflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/rainflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/rainflow/c_rain.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/rainflow/py_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74708 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/srs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ssmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-04-15 20:28:46.000000 pyyeti-1.2.5/pyyeti/ytools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.036841 pyyeti-1.2.5/pyyeti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-15 20:29:10.000000 pyyeti-1.2.5/pyyeti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-15 20:29:11.000000 pyyeti-1.2.5/pyyeti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:29:10.000000 pyyeti-1.2.5/pyyeti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-15 20:29:10.000000 pyyeti-1.2.5/pyyeti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 20:29:10.000000 pyyeti-1.2.5/pyyeti.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.040841 pyyeti-1.2.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-04-15 20:28:46.000000 pyyeti-1.2.5/scripts/lsop2
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-04-15 20:28:46.000000 pyyeti-1.2.5/scripts/lsop4
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 20:29:11.040841 pyyeti-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-15 20:28:46.000000 pyyeti-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.032841 pyyeti-1.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.040841 pyyeti-1.2.5/tests/nas2cam_csuper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nas2cam_csuper/inboard.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nas2cam_csuper/inboard.op4
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nas2cam_csuper/inboard.pch
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nas2cam_csuper/nas2cam.op2
+-rw-r--r--   0 runner    (1001) docker     (123)   147552 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nas2cam_csuper/nas2cam.op4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:29:11.040841 pyyeti-1.2.5/tests/nastran_drm12/
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nastran_drm12/drm12.op2
+-rw-r--r--   0 runner    (1001) docker     (123)    77852 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nastran_drm12/drm12.op4
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nastran_drm12/inboard_nas2cam.op2
+-rw-r--r--   0 runner    (1001) docker     (123)    51624 2023-04-15 20:28:46.000000 pyyeti-1.2.5/tests/nastran_drm12/inboard_nas2cam.op4
```

### Comparing `pyyeti-1.2.4/LICENSE.txt` & `pyyeti-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/PKG-INFO` & `pyyeti-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.2.4
+Version: 1.2.5
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.2.4 Summary: Tools mostly related
+Metadata-Version: 2.1 Name: pyyeti Version: 1.2.5 Summary: Tools mostly related
 to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
 Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: C
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `pyyeti-1.2.4/README.md` & `pyyeti-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/__init__.py` & `pyyeti-1.2.5/pyyeti/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cb.py` & `pyyeti-1.2.5/pyyeti/cb.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/_magpct.py` & `pyyeti-1.2.5/pyyeti/cla/_magpct.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/_rptext1.py` & `pyyeti-1.2.5/pyyeti/cla/_rptext1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/_rptpct1.py` & `pyyeti-1.2.5/pyyeti/cla/_rptpct1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/_rpttab1.py` & `pyyeti-1.2.5/pyyeti/cla/_rpttab1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/_utilities.py` & `pyyeti-1.2.5/pyyeti/cla/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/dr_def.py` & `pyyeti-1.2.5/pyyeti/cla/dr_def.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/dr_event.py` & `pyyeti-1.2.5/pyyeti/cla/dr_event.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/dr_results.py` & `pyyeti-1.2.5/pyyeti/cla/dr_results.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/dr_results_plots.py` & `pyyeti-1.2.5/pyyeti/cla/dr_results_plots.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cla/rel_disp_dtm.py` & `pyyeti-1.2.5/pyyeti/cla/rel_disp_dtm.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/column_plotter.py` & `pyyeti-1.2.5/pyyeti/column_plotter.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/cyclecount.py` & `pyyeti-1.2.5/pyyeti/cyclecount.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/datacursor.py` & `pyyeti-1.2.5/pyyeti/datacursor.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/dsp.py` & `pyyeti-1.2.5/pyyeti/dsp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/era.py` & `pyyeti-1.2.5/pyyeti/era.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/expmint.py` & `pyyeti-1.2.5/pyyeti/expmint.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/fdepsd.py` & `pyyeti-1.2.5/pyyeti/fdepsd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/frclim.py` & `pyyeti-1.2.5/pyyeti/frclim.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/guitools.py` & `pyyeti-1.2.5/pyyeti/guitools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/locate.py` & `pyyeti-1.2.5/pyyeti/locate.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/nastran/bulk.py` & `pyyeti-1.2.5/pyyeti/nastran/bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -2785,5420 +2785,5442 @@
 0000ae00: 206e 702e 6873 7461 636b 2828 762c 206e   np.hstack((v, n
 0000ae10: 702e 7a65 726f 7328 286e 702e 7369 7a65  p.zeros((np.size
 0000ae20: 2876 2c20 3029 2c20 3820 2d20 6329 2929  (v, 0), 8 - c)))
 0000ae30: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
 0000ae40: 2076 0a0a 0a64 6566 205f 636f 6e76 6572   v...def _conver
 0000ae50: 745f 6361 7264 2863 6172 6429 3a0a 2020  t_card(card):.  
 0000ae60: 2020 6966 206c 656e 2863 6172 6429 2021    if len(card) !
-0000ae70: 3d20 3132 3a0a 2020 2020 2020 2020 7261  = 12:.        ra
-0000ae80: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-0000ae90: 2020 2020 2020 2020 2020 2020 6622 6578              f"ex
-0000aea0: 7065 6374 6564 2031 3220 6669 656c 6473  pected 12 fields
-0000aeb0: 2062 7574 2067 6f74 207b 6c65 6e28 6361   but got {len(ca
-0000aec0: 7264 297d 2c20 6368 6563 6b3a 207b 6361  rd)}, check: {ca
-0000aed0: 7264 5b30 5d7d 2c20 7b63 6172 645b 315d  rd[0]}, {card[1]
-0000aee0: 7d22 0a20 2020 2020 2020 2029 0a20 2020  }".        ).   
-0000aef0: 2063 6861 7220 3d20 6361 7264 5b30 5d5b   char = card[0][
-0000af00: 355d 0a20 2020 2069 6620 6368 6172 2069  5].    if char i
-0000af10: 6e20 2272 5222 3a0a 2020 2020 2020 2020  n "rR":.        
-0000af20: 6374 7970 6520 3d20 310a 2020 2020 656c  ctype = 1.    el
-0000af30: 6966 2063 6861 7220 696e 2022 6343 223a  if char in "cC":
-0000af40: 0a20 2020 2020 2020 2063 7479 7065 203d  .        ctype =
-0000af50: 2032 0a20 2020 2065 6c73 653a 0a20 2020   2.    else:.   
-0000af60: 2020 2020 2063 7479 7065 203d 2033 0a0a       ctype = 3..
-0000af70: 2020 2020 2320 666f 7220 6572 726f 7220      # for error 
-0000af80: 6d65 7373 6167 652c 2069 6e20 6361 7365  message, in case
-0000af90: 2069 7427 7320 6e65 6564 6564 3a0a 2020   it's needed:.  
-0000afa0: 2020 6e61 6d65 2c20 6964 656e 7420 3d20    name, ident = 
-0000afb0: 6361 7264 5b30 5d2c 2063 6172 645b 315d  card[0], card[1]
-0000afc0: 0a0a 2020 2020 6361 7264 5b30 5d2c 2063  ..    card[0], c
-0000afd0: 6172 645b 315d 203d 2063 6172 645b 315d  ard[1] = card[1]
-0000afe0: 2c20 6374 7970 650a 2020 2020 7472 793a  , ctype.    try:
-0000aff0: 0a20 2020 2020 2020 2063 6172 6420 3d20  .        card = 
-0000b000: 6e70 2e61 7272 6179 2863 6172 6429 2e61  np.array(card).a
-0000b010: 7374 7970 6528 666c 6f61 7429 0a20 2020  stype(float).   
-0000b020: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-0000b030: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-0000b040: 206d 7367 203d 2066 227b 652e 6172 6773   msg = f"{e.args
-0000b050: 5b30 5d7d 2c20 6368 6563 6b3a 207b 6e61  [0]}, check: {na
-0000b060: 6d65 7d2c 207b 6964 656e 747d 220a 2020  me}, {ident}".  
-0000b070: 2020 2020 2020 652e 6172 6773 203d 2028        e.args = (
-0000b080: 6d73 672c 290a 2020 2020 2020 2020 7261  msg,).        ra
-0000b090: 6973 650a 0a20 2020 2072 6574 7572 6e20  ise..    return 
-0000b0a0: 6361 7264 0a0a 0a64 6566 2072 6463 6f72  card...def rdcor
-0000b0b0: 6432 6361 7264 7328 6629 3a0a 2020 2020  d2cards(f):.    
-0000b0c0: 2222 220a 2020 2020 5265 6164 2043 4f52  """.    Read COR
-0000b0d0: 4432 2a20 6361 7264 7320 6672 6f6d 2061  D2* cards from a
-0000b0e0: 204e 6173 7472 616e 2062 756c 6b20 6669   Nastran bulk fi
-0000b0f0: 6c65 0a0a 2020 2020 5061 7261 6d65 7465  le..    Paramete
-0000b100: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0000b110: 2d0a 2020 2020 6620 3a20 7374 7269 6e67  -.    f : string
-0000b120: 206f 7220 6669 6c65 5f6c 696b 6520 6f72   or file_like or
-0000b130: 204e 6f6e 650a 2020 2020 2020 2020 4569   None.        Ei
-0000b140: 7468 6572 2061 206e 616d 6520 6f66 2061  ther a name of a
-0000b150: 2066 696c 652c 206f 7220 6973 2061 2066   file, or is a f
-0000b160: 696c 655f 6c69 6b65 206f 626a 6563 7420  ile_like object 
-0000b170: 6173 2072 6574 7572 6e65 640a 2020 2020  as returned.    
-0000b180: 2020 2020 6279 203a 6675 6e63 3a60 6f70      by :func:`op
-0000b190: 656e 602e 2049 6620 6669 6c65 5f6c 696b  en`. If file_lik
-0000b1a0: 6520 6f62 6a65 6374 2c20 6974 2069 7320  e object, it is 
-0000b1b0: 7265 776f 756e 6420 6669 7273 742e 2043  rewound first. C
-0000b1c0: 616e 0a20 2020 2020 2020 2061 6c73 6f20  an.        also 
-0000b1d0: 6265 2074 6865 206e 616d 6520 6f66 2061  be the name of a
-0000b1e0: 2064 6972 6563 746f 7279 206f 7220 4e6f   directory or No
-0000b1f0: 6e65 3b20 696e 2074 6865 7365 2063 6173  ne; in these cas
-0000b200: 6573 2c20 6120 4755 490a 2020 2020 2020  es, a GUI.      
-0000b210: 2020 6973 206f 7065 6e65 6420 666f 7220    is opened for 
-0000b220: 6669 6c65 2073 656c 6563 7469 6f6e 2e0a  file selection..
-0000b230: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-0000b240: 202d 2d2d 2d2d 2d2d 0a20 2020 2064 6963   -------.    dic
-0000b250: 7469 6f6e 6172 790a 2020 2020 2020 2020  tionary.        
-0000b260: 4469 6374 696f 6e61 7279 2077 6974 6820  Dictionary with 
-0000b270: 7468 6520 6b65 7973 2062 6569 6e67 2074  the keys being t
-0000b280: 6865 2063 6f6f 7264 696e 6174 6520 7379  he coordinate sy
-0000b290: 7374 656d 2069 6420 616e 640a 2020 2020  stem id and.    
-0000b2a0: 2020 2020 7468 6520 7661 6c75 6573 2062      the values b
-0000b2b0: 6569 6e67 2074 6865 2035 7833 206d 6174  eing the 5x3 mat
-0000b2c0: 7269 783a 3a0a 0a20 2020 2020 2020 2020  rix::..         
-0000b2d0: 2020 205b 6964 2020 7479 7065 2030 5d20     [id  type 0] 
-0000b2e0: 2023 206f 7574 7075 7420 636f 6f72 642e   # output coord.
-0000b2f0: 2073 7973 2e20 6964 2061 6e64 2074 7970   sys. id and typ
-0000b300: 650a 2020 2020 2020 2020 2020 2020 5b78  e.            [x
-0000b310: 6f20 2079 6f20 207a 6f5d 2020 2320 6f72  o  yo  zo]  # or
-0000b320: 6967 696e 206f 6620 636f 6f72 642e 2073  igin of coord. s
-0000b330: 7973 7465 6d0a 2020 2020 2020 2020 2020  ystem.          
-0000b340: 2020 5b20 2020 2054 2020 2020 205d 2020    [    T     ]  
-0000b350: 2320 3378 3320 7472 616e 7366 6f72 6d61  # 3x3 transforma
-0000b360: 7469 6f6e 2074 6f20 6261 7369 630a 2020  tion to basic.  
-0000b370: 2020 2020 2020 2020 2020 4e6f 7465 2074            Note t
-0000b380: 6861 7420 5420 6973 2066 6f72 2074 6865  hat T is for the
-0000b390: 2063 6f6f 7264 696e 6174 6520 7379 7374   coordinate syst
-0000b3a0: 656d 2c20 6e6f 7420 6120 6772 6964 0a20  em, not a grid. 
-0000b3b0: 2020 2020 2020 2020 2020 2028 756e 6c65             (unle
-0000b3c0: 7373 2074 7970 6520 3d20 3120 7768 6963  ss type = 1 whic
-0000b3d0: 6820 6d65 616e 7320 7265 6374 616e 6775  h means rectangu
-0000b3e0: 6c61 7229 0a0a 2020 2020 5365 6520 616c  lar)..    See al
-0000b3f0: 736f 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  so.    --------.
-0000b400: 2020 2020 3a66 756e 633a 6062 756c 6b32      :func:`bulk2
-0000b410: 7573 6574 602c 203a 6675 6e63 3a60 7264  uset`, :func:`rd
-0000b420: 6361 7264 7360 2e0a 2020 2020 2222 220a  cards`..    """.
-0000b430: 2020 2020 6361 7264 7320 3d20 7264 6361      cards = rdca
-0000b440: 7264 7328 0a20 2020 2020 2020 2066 2c20  rds(.        f, 
-0000b450: 7222 2863 6f72 6432 5b72 6373 5d29 5c62  r"(cord2[rcs])\b
-0000b460: 222c 2072 6574 7572 6e5f 7661 723d 226c  ", return_var="l
-0000b470: 6973 7422 2c20 7265 6765 783d 5472 7565  ist", regex=True
-0000b480: 2c20 6b65 6570 5f6e 616d 653d 5472 7565  , keep_name=True
-0000b490: 2c20 626c 616e 6b3d 300a 2020 2020 290a  , blank=0.    ).
-0000b4a0: 0a20 2020 2069 6620 6361 7264 7320 6973  .    if cards is
-0000b4b0: 204e 6f6e 653a 0a20 2020 2020 2020 2072   None:.        r
-0000b4c0: 6574 7572 6e20 7b7d 0a0a 2020 2020 7265  eturn {}..    re
-0000b4d0: 7475 726e 206e 3270 2e62 7569 6c64 5f63  turn n2p.build_c
-0000b4e0: 6f6f 7264 7328 6e70 2e61 7272 6179 285b  oords(np.array([
-0000b4f0: 5f63 6f6e 7665 7274 5f63 6172 6428 6361  _convert_card(ca
-0000b500: 7264 2920 666f 7220 6361 7264 2069 6e20  rd) for card in 
-0000b510: 6361 7264 735d 2929 0a0a 0a64 6566 2077  cards]))...def w
-0000b520: 7467 7269 6473 280a 2020 2020 662c 0a20  tgrids(.    f,. 
-0000b530: 2020 2067 7269 6473 2c0a 2020 2020 6370     grids,.    cp
-0000b540: 3d30 2c0a 2020 2020 7879 7a3d 6e70 2e61  =0,.    xyz=np.a
-0000b550: 7272 6179 285b 5b30 2e30 2c20 302e 302c  rray([[0.0, 0.0,
-0000b560: 2030 2e30 5d5d 292c 0a20 2020 2063 643d   0.0]]),.    cd=
-0000b570: 302c 0a20 2020 2070 733d 2222 2c0a 2020  0,.    ps="",.  
-0000b580: 2020 7365 6964 3d22 222c 0a20 2020 2066    seid="",.    f
-0000b590: 6f72 6d3d 227b 3a31 362e 3866 7d22 2c0a  orm="{:16.8f}",.
-0000b5a0: 293a 0a20 2020 2022 2222 0a20 2020 2057  ):.    """.    W
-0000b5b0: 7269 7465 7320 4e61 7374 7261 6e20 4752  rites Nastran GR
-0000b5c0: 4944 2063 6172 6473 2074 6f20 6120 6669  ID cards to a fi
-0000b5d0: 6c65 2e0a 0a20 2020 2050 6172 616d 6574  le...    Paramet
-0000b5e0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-0000b5f0: 2d2d 0a20 2020 2066 203a 2073 7472 696e  --.    f : strin
-0000b600: 6720 6f72 2066 696c 655f 6c69 6b65 206f  g or file_like o
-0000b610: 7220 3120 6f72 204e 6f6e 650a 2020 2020  r 1 or None.    
-0000b620: 2020 2020 4569 7468 6572 2061 206e 616d      Either a nam
-0000b630: 6520 6f66 2061 2066 696c 652c 206f 7220  e of a file, or 
-0000b640: 6973 2061 2066 696c 655f 6c69 6b65 206f  is a file_like o
-0000b650: 626a 6563 7420 6173 2072 6574 7572 6e65  bject as returne
-0000b660: 640a 2020 2020 2020 2020 6279 203a 6675  d.        by :fu
-0000b670: 6e63 3a60 6f70 656e 6020 6f72 203a 636c  nc:`open` or :cl
-0000b680: 6173 733a 6069 6f2e 5374 7269 6e67 494f  ass:`io.StringIO
-0000b690: 602e 2049 6e70 7574 2061 7320 696e 7465  `. Input as inte
-0000b6a0: 6765 7220 3120 746f 0a20 2020 2020 2020  ger 1 to.       
-0000b6b0: 2077 7269 7465 2074 6f20 7374 646f 7574   write to stdout
-0000b6c0: 2e20 4361 6e20 616c 736f 2062 6520 7468  . Can also be th
-0000b6d0: 6520 6e61 6d65 206f 6620 6120 6469 7265  e name of a dire
-0000b6e0: 6374 6f72 7920 6f72 204e 6f6e 653b 0a20  ctory or None;. 
-0000b6f0: 2020 2020 2020 2069 6e20 7468 6573 6520         in these 
-0000b700: 6361 7365 732c 2061 2047 5549 2069 7320  cases, a GUI is 
-0000b710: 6f70 656e 6564 2066 6f72 2066 696c 6520  opened for file 
-0000b720: 7365 6c65 6374 696f 6e2e 0a20 2020 2067  selection..    g
-0000b730: 7269 6473 203a 2031 6420 6172 7261 795f  rids : 1d array_
-0000b740: 6c69 6b65 3b20 6c65 6e67 7468 204e 0a20  like; length N. 
-0000b750: 2020 2020 2020 2056 6563 746f 7220 6f66         Vector of
-0000b760: 2067 7269 6420 6964 732e 2054 6865 206c   grid ids. The l
-0000b770: 656e 6774 6820 6f66 2060 6772 6964 7360  ength of `grids`
-0000b780: 2077 696c 6c20 6265 2072 6566 6572 656e   will be referen
-0000b790: 6365 640a 2020 2020 2020 2020 6173 2060  ced.        as `
-0000b7a0: 604e 6060 2069 6e20 6578 706c 616e 6174  `N`` in explanat
-0000b7b0: 696f 6e73 2062 656c 6f77 2e0a 2020 2020  ions below..    
-0000b7c0: 6370 203a 2069 6e74 6567 6572 2073 6361  cp : integer sca
-0000b7d0: 6c61 7220 6f72 2076 6563 746f 720a 2020  lar or vector.  
-0000b7e0: 2020 2020 2020 4964 206f 6620 636f 6f72        Id of coor
-0000b7f0: 6469 6e61 7465 2073 7973 7465 6d28 7329  dinate system(s)
-0000b800: 2067 7269 6473 2061 7265 2064 6566 696e   grids are defin
-0000b810: 6564 2069 6e3b 2065 6974 6865 7220 7363  ed in; either sc
-0000b820: 616c 6172 0a20 2020 2020 2020 206f 7220  alar.        or 
-0000b830: 7665 6374 6f72 2077 6974 6820 4e20 726f  vector with N ro
-0000b840: 7773 2e0a 2020 2020 7879 7a20 3a20 3264  ws..    xyz : 2d
-0000b850: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
-0000b860: 2020 2020 332d 636f 6c75 6d6e 206d 6174      3-column mat
-0000b870: 7269 7820 6f66 2067 7269 6420 6c6f 6361  rix of grid loca
-0000b880: 7469 6f6e 733b 2031 2072 6f77 206f 7220  tions; 1 row or 
-0000b890: 4e20 726f 7773 2e0a 2020 2020 6364 203a  N rows..    cd :
-0000b8a0: 2069 6e74 6567 6572 2073 6361 6c61 7220   integer scalar 
-0000b8b0: 6f72 2076 6563 746f 720a 2020 2020 2020  or vector.      
-0000b8c0: 2020 4964 206f 6620 6469 7370 6c61 6365    Id of displace
-0000b8d0: 6d65 6e74 2063 6f6f 7264 696e 6174 6520  ment coordinate 
-0000b8e0: 7379 7374 656d 2066 6f72 2067 7269 6473  system for grids
-0000b8f0: 3b20 6569 7468 6572 2073 6361 6c61 720a  ; either scalar.
-0000b900: 2020 2020 2020 2020 6f72 2076 6563 746f          or vecto
-0000b910: 7220 7769 7468 204e 2072 6f77 732e 0a20  r with N rows.. 
-0000b920: 2020 2070 7320 3a20 696e 7465 6765 7220     ps : integer 
-0000b930: 7363 616c 6172 206f 7220 7665 6374 6f72  scalar or vector
-0000b940: 0a20 2020 2020 2020 2050 6572 6d61 6e65  .        Permane
-0000b950: 6e74 2063 6f6e 7374 7261 696e 7473 2066  nt constraints f
-0000b960: 6f72 2067 7269 6473 2c20 6567 3a20 3132  or grids, eg: 12
-0000b970: 3334 3536 3b20 6569 7468 6572 2073 6361  3456; either sca
-0000b980: 6c61 7220 6f72 0a20 2020 2020 2020 2076  lar or.        v
-0000b990: 6563 746f 7220 7769 7468 204e 2072 6f77  ector with N row
-0000b9a0: 732e 0a20 2020 2073 6569 6420 3a20 696e  s..    seid : in
-0000b9b0: 7465 6765 7220 7363 616c 6172 206f 7220  teger scalar or 
-0000b9c0: 7665 6374 6f72 0a20 2020 2020 2020 2053  vector.        S
-0000b9d0: 7570 6572 656c 656d 656e 7420 6964 3b20  uperelement id; 
-0000b9e0: 6569 7468 6572 2073 6361 6c61 7220 6f72  either scalar or
-0000b9f0: 2076 6563 746f 7220 7769 7468 204e 2072   vector with N r
-0000ba00: 6f77 732e 0a20 2020 2066 6f72 6d61 7420  ows..    format 
-0000ba10: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-0000ba20: 2053 7472 696e 6720 7370 6563 6966 7969   String specifyi
-0000ba30: 6e67 2066 6f72 6d61 7420 6f66 2058 595a  ng format of XYZ
-0000ba40: 2076 616c 7565 733b 206d 7573 7420 7072   values; must pr
-0000ba50: 6f64 7563 6520 3820 6f72 2031 360a 2020  oduce 8 or 16.  
-0000ba60: 2020 2020 2020 6368 6172 6163 7465 7220        character 
-0000ba70: 7374 7269 6e67 732e 0a0a 2020 2020 5265  strings...    Re
-0000ba80: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-0000ba90: 2d0a 2020 2020 4e6f 6e65 0a0a 2020 2020  -.    None..    
-0000baa0: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
-0000bab0: 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20 6672  -----.    >>> fr
-0000bac0: 6f6d 2070 7979 6574 6920 696d 706f 7274  om pyyeti import
-0000bad0: 206e 6173 7472 616e 0a20 2020 203e 3e3e   nastran.    >>>
-0000bae0: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
-0000baf0: 206e 700a 2020 2020 3e3e 3e20 6e61 7374   np.    >>> nast
-0000bb00: 7261 6e2e 7774 6772 6964 7328 312c 206e  ran.wtgrids(1, n
-0000bb10: 702e 6172 616e 6765 2831 2c20 3429 290a  p.arange(1, 4)).
-0000bb20: 2020 2020 4752 4944 2a20 2020 2020 2020      GRID*       
-0000bb30: 2020 2020 2020 2020 2020 2031 2020 2020             1    
-0000bb40: 2020 2020 2020 2020 2020 2030 2020 2020             0    
-0000bb50: 2020 302e 3030 3030 3030 3030 2020 2020    0.00000000    
-0000bb60: 2020 302e 3030 3030 3030 3030 0a20 2020    0.00000000.   
-0000bb70: 202a 2020 2020 2020 2020 2020 2020 2030   *             0
-0000bb80: 2e30 3030 3030 3030 3020 2020 2020 2020  .00000000       
-0000bb90: 2020 2020 2020 2020 300a 2020 2020 4752          0.    GR
-0000bba0: 4944 2a20 2020 2020 2020 2020 2020 2020  ID*             
-0000bbb0: 2020 2020 2032 2020 2020 2020 2020 2020       2          
-0000bbc0: 2020 2020 2030 2020 2020 2020 302e 3030       0      0.00
-0000bbd0: 3030 3030 3030 2020 2020 2020 302e 3030  000000      0.00
-0000bbe0: 3030 3030 3030 0a20 2020 202a 2020 2020  000000.    *    
-0000bbf0: 2020 2020 2020 2020 2030 2e30 3030 3030           0.00000
-0000bc00: 3030 3020 2020 2020 2020 2020 2020 2020  000             
-0000bc10: 2020 300a 2020 2020 4752 4944 2a20 2020    0.    GRID*   
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-0000bc40: 2020 2020 2020 302e 3030 3030 3030 3030        0.00000000
-0000bc50: 2020 2020 2020 302e 3030 3030 3030 3030        0.00000000
-0000bc60: 0a20 2020 202a 2020 2020 2020 2020 2020  .    *          
-0000bc70: 2020 2030 2e30 3030 3030 3030 3020 2020     0.00000000   
-0000bc80: 2020 2020 2020 2020 2020 2020 300a 2020              0.  
-0000bc90: 2020 3e3e 3e20 7879 7a20 3d20 6e70 2e61    >>> xyz = np.a
-0000bca0: 7272 6179 285b 5b2e 312c 202e 322c 202e  rray([[.1, .2, .
-0000bcb0: 335d 2c20 5b31 2e31 2c20 312e 322c 2031  3], [1.1, 1.2, 1
-0000bcc0: 2e33 5d5d 290a 2020 2020 3e3e 3e20 6e61  .3]]).    >>> na
-0000bcd0: 7374 7261 6e2e 7774 6772 6964 7328 312c  stran.wtgrids(1,
-0000bce0: 205b 3130 302c 2032 3030 5d2c 2078 797a   [100, 200], xyz
-0000bcf0: 3d78 797a 2c20 6364 3d31 302c 0a20 2020  =xyz, cd=10,.   
-0000bd00: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
-0000bd10: 2020 2020 2066 6f72 6d3d 277b 3a38 2e32       form='{:8.2
-0000bd20: 667d 2729 0a20 2020 2047 5249 4420 2020  f}').    GRID   
-0000bd30: 2020 2020 2020 3130 3020 2020 2020 2020        100       
-0000bd40: 3020 2020 2030 2e31 3020 2020 2030 2e32  0    0.10    0.2
-0000bd50: 3020 2020 2030 2e33 3020 2020 2020 2031  0    0.30      1
-0000bd60: 300a 2020 2020 4752 4944 2020 2020 2020  0.    GRID      
-0000bd70: 2020 2032 3030 2020 2020 2020 2030 2020     200       0  
-0000bd80: 2020 312e 3130 2020 2020 312e 3230 2020    1.10    1.20  
-0000bd90: 2020 312e 3330 2020 2020 2020 3130 0a20    1.30      10. 
-0000bda0: 2020 2022 2222 0a20 2020 2067 7269 6473     """.    grids
-0000bdb0: 203d 206e 702e 6174 6c65 6173 745f 3164   = np.atleast_1d
-0000bdc0: 2867 7269 6473 292e 7261 7665 6c28 290a  (grids).ravel().
-0000bdd0: 2020 2020 7879 7a20 3d20 6e70 2e61 746c      xyz = np.atl
-0000bde0: 6561 7374 5f32 6428 7879 7a29 0a20 2020  east_2d(xyz).   
-0000bdf0: 2074 6573 7473 7472 203d 2066 6f72 6d2e   teststr = form.
-0000be00: 666f 726d 6174 2831 2e30 290a 2020 2020  format(1.0).    
-0000be10: 6c65 6e67 7468 203d 206c 656e 2874 6573  length = len(tes
-0000be20: 7473 7472 290a 2020 2020 6966 206c 656e  tstr).    if len
-0000be30: 6774 6820 213d 2038 2061 6e64 206c 656e  gth != 8 and len
-0000be40: 6774 6820 213d 2031 363a 0a20 2020 2020  gth != 16:.     
-0000be50: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000be60: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-0000be70: 2066 2260 666f 726d 6020 7072 6f64 7563   f"`form` produc
-0000be80: 6573 2061 207b 6c65 6e67 7468 7d20 6c65  es a {length} le
-0000be90: 6e67 7468 2073 7472 696e 672e 2049 7420  ngth string. It 
-0000bea0: 6d75 7374 2062 6520 3820 6f72 2031 362e  must be 8 or 16.
-0000beb0: 5c6e 220a 2020 2020 2020 2020 290a 2020  \n".        ).  
-0000bec0: 2020 6966 2070 7320 3d3d 2073 6569 6420    if ps == seid 
-0000bed0: 3d3d 2022 223a 0a20 2020 2020 2020 2069  == "":.        i
-0000bee0: 6620 6c65 6e28 7465 7374 7374 7229 203e  f len(teststr) >
-0000bef0: 2038 3a0a 2020 2020 2020 2020 2020 2020   8:.            
-0000bf00: 7374 7269 6e67 203d 2028 0a20 2020 2020  string = (.     
-0000bf10: 2020 2020 2020 2020 2020 2022 4752 4944             "GRID
-0000bf20: 2a20 2020 7b3a 3136 647d 7b3a 3136 647d  *   {:16d}{:16d}
-0000bf30: 2220 2b20 666f 726d 202a 2032 202b 2022  " + form * 2 + "
-0000bf40: 5c6e 2a20 2020 2020 2020 2220 2b20 666f  \n*       " + fo
-0000bf50: 726d 202b 2022 7b3a 3136 647d 5c6e 220a  rm + "{:16d}\n".
-0000bf60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000bf70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000bf80: 2020 2020 2020 2020 7374 7269 6e67 203d          string =
-0000bf90: 2022 4752 4944 2020 2020 7b3a 3864 7d7b   "GRID    {:8d}{
-0000bfa0: 3a38 647d 2220 2b20 666f 726d 202a 2033  :8d}" + form * 3
-0000bfb0: 202b 2022 7b3a 3864 7d5c 6e22 0a20 2020   + "{:8d}\n".   
-0000bfc0: 2020 2020 2077 7269 7465 722e 7665 6377       writer.vecw
-0000bfd0: 7269 7465 2866 2c20 7374 7269 6e67 2c20  rite(f, string, 
-0000bfe0: 6772 6964 732c 2063 702c 2078 797a 5b3a  grids, cp, xyz[:
-0000bff0: 2c20 305d 2c20 7879 7a5b 3a2c 2031 5d2c  , 0], xyz[:, 1],
-0000c000: 2078 797a 5b3a 2c20 325d 2c20 6364 290a   xyz[:, 2], cd).
-0000c010: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000c020: 2020 6966 206c 656e 2874 6573 7473 7472    if len(teststr
-0000c030: 2920 3e20 383a 0a20 2020 2020 2020 2020  ) > 8:.         
-0000c040: 2020 2073 7472 696e 6720 3d20 280a 2020     string = (.  
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2247                "G
-0000c060: 5249 442a 2020 207b 3a31 3664 7d7b 3a31  RID*   {:16d}{:1
-0000c070: 3664 7d22 0a20 2020 2020 2020 2020 2020  6d}".           
-0000c080: 2020 2020 202b 2066 6f72 6d20 2a20 320a       + form * 2.
-0000c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0a0: 2b20 225c 6e2a 2020 2020 2020 2022 0a20  + "\n*       ". 
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0000c0c0: 2066 6f72 6d0a 2020 2020 2020 2020 2020   form.          
-0000c0d0: 2020 2020 2020 2b20 227b 3a31 3664 7d7b        + "{:16d}{
-0000c0e0: 3a3e 3136 7d7b 3a3e 3136 7d5c 6e22 0a20  :>16}{:>16}\n". 
-0000c0f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000c100: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000c110: 2020 2020 2020 2073 7472 696e 6720 3d20         string = 
-0000c120: 2247 5249 4420 2020 207b 3a38 647d 7b3a  "GRID    {:8d}{:
-0000c130: 3864 7d22 202b 2066 6f72 6d20 2a20 3320  8d}" + form * 3 
-0000c140: 2b20 227b 3a38 647d 7b3a 3e38 7d7b 3a3e  + "{:8d}{:>8}{:>
-0000c150: 387d 5c6e 220a 2020 2020 2020 2020 7772  8}\n".        wr
-0000c160: 6974 6572 2e76 6563 7772 6974 6528 0a20  iter.vecwrite(. 
-0000c170: 2020 2020 2020 2020 2020 2066 2c20 7374             f, st
-0000c180: 7269 6e67 2c20 6772 6964 732c 2063 702c  ring, grids, cp,
-0000c190: 2078 797a 5b3a 2c20 305d 2c20 7879 7a5b   xyz[:, 0], xyz[
-0000c1a0: 3a2c 2031 5d2c 2078 797a 5b3a 2c20 325d  :, 1], xyz[:, 2]
-0000c1b0: 2c20 6364 2c20 7073 2c20 7365 6964 0a20  , cd, ps, seid. 
-0000c1c0: 2020 2020 2020 2029 0a0a 0a64 6566 2072         )...def r
-0000c1d0: 6474 6162 6c65 6431 2866 2c20 6e61 6d65  dtabled1(f, name
-0000c1e0: 3d22 7461 626c 6564 3122 293a 0a20 2020  ="tabled1"):.   
-0000c1f0: 2022 2222 0a20 2020 2052 6561 6420 4e61   """.    Read Na
-0000c200: 7374 7261 6e20 5441 424c 4544 3120 6f72  stran TABLED1 or
-0000c210: 206f 7468 6572 2069 6465 6e74 6963 616c   other identical
-0000c220: 6c79 2066 6f72 6d61 7474 6564 2063 6172  ly formatted car
-0000c230: 6473 2066 726f 6d20 610a 2020 2020 4e61  ds from a.    Na
-0000c240: 7374 7261 6e20 6275 6c6b 2066 696c 652e  stran bulk file.
-0000c250: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0000c260: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0000c270: 2020 2020 6620 3a20 7374 7269 6e67 206f      f : string o
-0000c280: 7220 6669 6c65 5f6c 696b 6520 6f72 204e  r file_like or N
-0000c290: 6f6e 650a 2020 2020 2020 2020 4569 7468  one.        Eith
-0000c2a0: 6572 2061 206e 616d 6520 6f66 2061 2066  er a name of a f
-0000c2b0: 696c 652c 206f 7220 6973 2061 2066 696c  ile, or is a fil
-0000c2c0: 655f 6c69 6b65 206f 626a 6563 7420 6173  e_like object as
-0000c2d0: 2072 6574 7572 6e65 640a 2020 2020 2020   returned.      
-0000c2e0: 2020 6279 203a 6675 6e63 3a60 6f70 656e    by :func:`open
-0000c2f0: 602e 2049 6620 6669 6c65 5f6c 696b 6520  `. If file_like 
-0000c300: 6f62 6a65 6374 2c20 6974 2069 7320 7265  object, it is re
-0000c310: 776f 756e 6420 6669 7273 742e 2043 616e  wound first. Can
-0000c320: 0a20 2020 2020 2020 2061 6c73 6f20 6265  .        also be
-0000c330: 2074 6865 206e 616d 6520 6f66 2061 2064   the name of a d
-0000c340: 6972 6563 746f 7279 206f 7220 4e6f 6e65  irectory or None
-0000c350: 3b20 696e 2074 6865 7365 2063 6173 6573  ; in these cases
-0000c360: 2c20 6120 4755 490a 2020 2020 2020 2020  , a GUI.        
-0000c370: 6973 206f 7065 6e65 6420 666f 7220 6669  is opened for fi
-0000c380: 6c65 2073 656c 6563 7469 6f6e 2e0a 2020  le selection..  
-0000c390: 2020 6e61 6d65 203a 2073 7472 696e 673b    name : string;
-0000c3a0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000c3b0: 2020 4e61 6d65 206f 6620 6361 7264 7320    Name of cards 
-0000c3c0: 746f 2072 6561 642e 0a0a 2020 2020 5265  to read...    Re
-0000c3d0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-0000c3e0: 2d0a 2020 2020 6463 7420 3a20 6469 6374  -.    dct : dict
-0000c3f0: 696f 6e61 7279 0a20 2020 2020 2020 2044  ionary.        D
-0000c400: 6963 7469 6f6e 6172 7920 6f66 2054 4142  ictionary of TAB
-0000c410: 4c45 4431 2028 6f72 2073 696d 696c 6172  LED1 (or similar
-0000c420: 2920 6361 7264 733a 0a0a 2020 2020 2020  ) cards:..      
-0000c430: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-0000c440: 3a20 6e6f 6e65 0a0a 2020 2020 2020 2020  : none..        
-0000c450: 2020 2020 7b49 4431 3a20 5b74 696d 652c      {ID1: [time,
-0000c460: 2064 6174 615d 2c0a 2020 2020 2020 2020   data],.        
-0000c470: 2020 2020 2049 4432 3a20 5b74 696d 652c       ID2: [time,
-0000c480: 2064 6174 615d 2c20 2e2e 2e7d 0a0a 2020   data], ...}..  
-0000c490: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
-0000c4a0: 2d0a 2020 2020 5468 6973 2072 6f75 7469  -.    This routi
-0000c4b0: 6e65 2075 7365 7320 3a66 756e 633a 6072  ne uses :func:`r
-0000c4c0: 6463 6172 6473 6020 746f 206c 6f61 6420  dcards` to load 
-0000c4d0: 7468 6520 6461 7461 2028 6361 6e20 7265  the data (can re
-0000c4e0: 6164 2038 0a20 2020 206f 7220 3136 2066  ad 8.    or 16 f
-0000c4f0: 6978 6564 2066 6965 6c64 206f 7220 636f  ixed field or co
-0000c500: 6d6d 612d 6465 6c69 6d69 7465 6429 2e0a  mma-delimited)..
-0000c510: 0a20 2020 2053 6565 2061 6c73 6f0a 2020  .    See also.  
-0000c520: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203a    --------.    :
-0000c530: 6675 6e63 3a60 7774 7461 626c 6564 3160  func:`wttabled1`
-0000c540: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
-0000c550: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-0000c560: 3e3e 3e20 6672 6f6d 2070 7979 6574 6920  >>> from pyyeti 
-0000c570: 696d 706f 7274 206e 6173 7472 616e 0a20  import nastran. 
-0000c580: 2020 203e 3e3e 2069 6d70 6f72 7420 6e75     >>> import nu
-0000c590: 6d70 7920 6173 206e 700a 2020 2020 3e3e  mpy as np.    >>
-0000c5a0: 3e20 6672 6f6d 2069 6f20 696d 706f 7274  > from io import
-0000c5b0: 2053 7472 696e 6749 4f0a 2020 2020 3e3e   StringIO.    >>
-0000c5c0: 3e20 7420 3d20 6e70 2e61 7261 6e67 6528  > t = np.arange(
-0000c5d0: 302c 2031 2c20 2e30 3529 0a20 2020 203e  0, 1, .05).    >
-0000c5e0: 3e3e 2064 203d 206e 702e 7369 6e28 322a  >> d = np.sin(2*
-0000c5f0: 6e70 2e70 692a 332a 7429 0a20 2020 203e  np.pi*3*t).    >
-0000c600: 3e3e 2077 6974 6820 5374 7269 6e67 494f  >> with StringIO
-0000c610: 2829 2061 7320 663a 0a20 2020 202e 2e2e  () as f:.    ...
-0000c620: 2020 2020 206e 6173 7472 616e 2e77 7474       nastran.wtt
-0000c630: 6162 6c65 6431 2866 2c20 3430 3030 2c20  abled1(f, 4000, 
-0000c640: 742c 2064 2c20 2733 2048 7a20 5369 6e65  t, d, '3 Hz Sine
-0000c650: 2057 6176 6527 2c0a 2020 2020 2e2e 2e20   Wave',.    ... 
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c670: 2020 2020 2020 666f 726d 3d27 7b3a 382e        form='{:8.
-0000c680: 3266 7d7b 3a38 2e35 667d 2729 0a20 2020  2f}{:8.5f}').   
-0000c690: 202e 2e2e 2020 2020 2064 6374 203d 206e   ...     dct = n
-0000c6a0: 6173 7472 616e 2e72 6474 6162 6c65 6431  astran.rdtabled1
-0000c6b0: 2866 290a 2020 2020 3e3e 3e20 6e70 2e61  (f).    >>> np.a
-0000c6c0: 6c6c 636c 6f73 6528 742c 2064 6374 5b34  llclose(t, dct[4
-0000c6d0: 3030 305d 5b3a 2c20 305d 290a 2020 2020  000][:, 0]).    
-0000c6e0: 5472 7565 0a20 2020 203e 3e3e 206e 702e  True.    >>> np.
-0000c6f0: 616c 6c63 6c6f 7365 2864 2c20 6463 745b  allclose(d, dct[
-0000c700: 3430 3030 5d5b 3a2c 2031 5d29 0a20 2020  4000][:, 1]).   
-0000c710: 2054 7275 650a 2020 2020 2222 220a 2020   True.    """.  
-0000c720: 2020 6420 3d20 7264 6361 7264 7328 662c    d = rdcards(f,
-0000c730: 206e 616d 652c 2072 6574 7572 6e5f 7661   name, return_va
-0000c740: 723d 2264 6963 7422 290a 2020 2020 666f  r="dict").    fo
-0000c750: 7220 7469 6420 696e 2064 3a0a 2020 2020  r tid in d:.    
-0000c760: 2020 2020 7665 6320 3d20 645b 7469 645d      vec = d[tid]
-0000c770: 0a20 2020 2020 2020 2064 5b74 6964 5d20  .        d[tid] 
-0000c780: 3d20 6e70 2e76 7374 6163 6b28 5b76 6563  = np.vstack([vec
-0000c790: 5b38 3a2d 313a 325d 2c20 7665 635b 393a  [8:-1:2], vec[9:
-0000c7a0: 2d31 3a32 5d5d 292e 540a 2020 2020 7265  -1:2]]).T.    re
-0000c7b0: 7475 726e 2064 0a0a 0a40 6775 6974 6f6f  turn d...@guitoo
-0000c7c0: 6c73 2e77 7269 7465 5f74 6578 745f 6669  ls.write_text_fi
-0000c7d0: 6c65 0a64 6566 2077 7474 6162 6c65 6431  le.def wttabled1
-0000c7e0: 2866 2c20 7469 642c 2074 2c20 642c 2074  (f, tid, t, d, t
-0000c7f0: 6974 6c65 3d4e 6f6e 652c 2066 6f72 6d3d  itle=None, form=
-0000c800: 227b 3a31 362e 3945 7d7b 3a31 362e 3945  "{:16.9E}{:16.9E
-0000c810: 7d22 2c20 7461 626c 6573 7472 3d22 5441  }", tablestr="TA
-0000c820: 424c 4544 3122 293a 0a20 2020 2022 2222  BLED1"):.    """
-0000c830: 0a20 2020 2057 7269 7465 7320 6120 4e61  .    Writes a Na
-0000c840: 7374 7261 6e20 5441 424c 4544 3120 286f  stran TABLED1 (o
-0000c850: 7220 7369 6d69 6c61 7229 2063 6172 6420  r similar) card 
-0000c860: 746f 2061 2066 696c 652e 0a0a 2020 2020  to a file...    
-0000c870: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-0000c880: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6620  ---------.    f 
-0000c890: 3a20 7374 7269 6e67 206f 7220 6669 6c65  : string or file
-0000c8a0: 5f6c 696b 6520 6f72 2031 206f 7220 4e6f  _like or 1 or No
-0000c8b0: 6e65 0a20 2020 2020 2020 2045 6974 6865  ne.        Eithe
-0000c8c0: 7220 6120 6e61 6d65 206f 6620 6120 6669  r a name of a fi
-0000c8d0: 6c65 2c20 6f72 2069 7320 6120 6669 6c65  le, or is a file
-0000c8e0: 5f6c 696b 6520 6f62 6a65 6374 2061 7320  _like object as 
-0000c8f0: 7265 7475 726e 6564 0a20 2020 2020 2020  returned.       
-0000c900: 2062 7920 3a66 756e 633a 606f 7065 6e60   by :func:`open`
-0000c910: 206f 7220 3a63 6c61 7373 3a60 696f 2e53   or :class:`io.S
-0000c920: 7472 696e 6749 4f60 2e20 496e 7075 7420  tringIO`. Input 
-0000c930: 6173 2069 6e74 6567 6572 2031 2074 6f0a  as integer 1 to.
-0000c940: 2020 2020 2020 2020 7772 6974 6520 746f          write to
-0000c950: 2073 7464 6f75 742e 2043 616e 2061 6c73   stdout. Can als
-0000c960: 6f20 6265 2074 6865 206e 616d 6520 6f66  o be the name of
-0000c970: 2061 2064 6972 6563 746f 7279 206f 7220   a directory or 
-0000c980: 4e6f 6e65 3b0a 2020 2020 2020 2020 696e  None;.        in
-0000c990: 2074 6865 7365 2063 6173 6573 2c20 6120   these cases, a 
-0000c9a0: 4755 4920 6973 206f 7065 6e65 6420 666f  GUI is opened fo
-0000c9b0: 7220 6669 6c65 2073 656c 6563 7469 6f6e  r file selection
-0000c9c0: 2e0a 2020 2020 7469 6420 3a20 696e 7465  ..    tid : inte
-0000c9d0: 6765 720a 2020 2020 2020 2020 4944 2066  ger.        ID f
-0000c9e0: 6f72 2054 4142 4c45 4431 2063 6172 640a  or TABLED1 card.
-0000c9f0: 2020 2020 7420 3a20 3164 2061 7272 6179      t : 1d array
-0000ca00: 5f6c 696b 650a 2020 2020 2020 2020 7469  _like.        ti
-0000ca10: 6d65 2076 6563 746f 720a 2020 2020 6420  me vector.    d 
-0000ca20: 3a20 3164 2061 7272 6179 5f6c 696b 650a  : 1d array_like.
-0000ca30: 2020 2020 2020 2020 6461 7461 2076 6563          data vec
-0000ca40: 746f 720a 2020 2020 7469 746c 6520 3a20  tor.    title : 
-0000ca50: 7374 7269 6e67 206f 7220 4e6f 6e65 3b20  string or None; 
-0000ca60: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0000ca70: 2049 6620 6120 7374 7269 6e67 2c20 6974   If a string, it
-0000ca80: 2069 7320 7772 6974 7465 6e20 6173 2061   is written as a
-0000ca90: 2063 6f6d 6d65 6e74 2062 6566 6f72 6520   comment before 
-0000caa0: 7461 626c 652e 2049 6620 4e6f 6e65 2c0a  table. If None,.
-0000cab0: 2020 2020 2020 2020 6e6f 2073 7472 696e          no strin
-0000cac0: 6720 6973 2077 7269 7474 656e 2e0a 2020  g is written..  
-0000cad0: 2020 666f 726d 203a 2073 7472 696e 673b    form : string;
-0000cae0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000caf0: 2020 5374 7269 6e67 2073 7065 6369 6679    String specify
-0000cb00: 696e 6720 7468 6520 666f 726d 6174 206f  ing the format o
-0000cb10: 6620 6120 7369 6e67 6c65 205b 7469 6d65  f a single [time
-0000cb20: 2c20 6461 7461 5d20 7061 6972 2e0a 2020  , data] pair..  
-0000cb30: 2020 2020 2020 4578 7065 6374 6564 2074        Expected t
-0000cb40: 6f20 7265 7375 6c74 2069 6e20 6120 7374  o result in a st
-0000cb50: 7269 6e67 2065 6974 6865 7220 3136 206f  ring either 16 o
-0000cb60: 7220 3332 2063 6861 7261 6374 6572 730a  r 32 characters.
-0000cb70: 2020 2020 2020 2020 6c6f 6e67 2e0a 2020          long..  
-0000cb80: 2020 7461 626c 6573 7472 203a 2073 7472    tablestr : str
-0000cb90: 696e 673b 206f 7074 696f 6e61 6c0a 2020  ing; optional.  
-0000cba0: 2020 2020 2020 4e61 6d65 206f 6620 6361        Name of ca
-0000cbb0: 7264 2074 6f20 7772 6974 653b 206d 7573  rd to write; mus
-0000cbc0: 7420 6265 2073 616d 6520 666f 726d 6174  t be same format
-0000cbd0: 2061 7320 5441 424c 4544 312e 0a0a 2020   as TABLED1...  
-0000cbe0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-0000cbf0: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a0a  -----.    None..
-0000cc00: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
-0000cc10: 2d2d 2d0a 2020 2020 496e 2074 6865 2066  ---.    In the f
-0000cc20: 6f72 6d61 7420 7374 7269 6e67 2c20 696e  ormat string, in
-0000cc30: 636c 7564 6520 6120 2320 7369 676e 2074  clude a # sign t
-0000cc40: 6f20 666f 7263 6520 6120 6465 6369 6d61  o force a decima
-0000cc50: 6c20 706f 696e 7420 746f 0a20 2020 2061  l point to.    a
-0000cc60: 7070 6561 7220 7769 7468 6f75 7420 7472  ppear without tr
-0000cc70: 6169 6c69 6e67 2064 6967 6974 732e 2046  ailing digits. F
-0000cc80: 6f72 2065 7861 6d70 6c65 2c20 277b 3a38  or example, '{:8
-0000cc90: 2e32 667d 7b3a 2338 2e30 667d 270a 2020  .2f}{:#8.0f}'.  
-0000cca0: 2020 776f 756c 6420 7072 696e 7420 6c69    would print li
-0000ccb0: 6b65 2074 6869 733a 2027 2031 322e 3334  ke this: ' 12.34
-0000ccc0: 2031 3233 3435 362e 272e 0a0a 2020 2020   123456.'...    
-0000ccd0: 5365 6520 616c 736f 0a20 2020 202d 2d2d  See also.    ---
-0000cce0: 2d2d 2d2d 2d0a 2020 2020 3a66 756e 633a  -----.    :func:
-0000ccf0: 6072 6474 6162 6c65 6431 600a 0a20 2020  `rdtabled1`..   
-0000cd00: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
-0000cd10: 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e 2066  ------.    >>> f
-0000cd20: 726f 6d20 7079 7965 7469 2069 6d70 6f72  rom pyyeti impor
-0000cd30: 7420 6e61 7374 7261 6e0a 2020 2020 3e3e  t nastran.    >>
-0000cd40: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
-0000cd50: 7320 6e70 0a20 2020 203e 3e3e 2074 203d  s np.    >>> t =
-0000cd60: 206e 702e 6172 616e 6765 2830 2c20 2e39   np.arange(0, .9
-0000cd70: 312c 202e 3035 290a 2020 2020 3e3e 3e20  1, .05).    >>> 
-0000cd80: 6420 3d20 6e70 2e73 696e 2832 2a6e 702e  d = np.sin(2*np.
-0000cd90: 7069 2a33 2a74 290a 2020 2020 3e3e 3e20  pi*3*t).    >>> 
-0000cda0: 6e61 7374 7261 6e2e 7774 7461 626c 6564  nastran.wttabled
-0000cdb0: 3128 312c 2034 3030 302c 2074 2c20 642c  1(1, 4000, t, d,
-0000cdc0: 2027 3320 487a 2053 696e 6520 5761 7665   '3 Hz Sine Wave
-0000cdd0: 272c 0a20 2020 202e 2e2e 2020 2020 2020  ',.    ...      
-0000cde0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000cdf0: 6d3d 277b 3a38 2e32 667d 7b3a 382e 3566  m='{:8.2f}{:8.5f
-0000ce00: 7d27 290a 2020 2020 2420 3320 487a 2053  }').    $ 3 Hz S
-0000ce10: 696e 6520 5761 7665 0a20 2020 2054 4142  ine Wave.    TAB
-0000ce20: 4c45 4431 2020 2020 2034 3030 300a 2020  LED1     4000.  
-0000ce30: 2020 2020 2020 2020 2020 2020 2020 302e                0.
-0000ce40: 3030 2030 2e30 3030 3030 2020 2020 302e  00 0.00000    0.
-0000ce50: 3035 2030 2e38 3039 3032 2020 2020 302e  05 0.80902    0.
-0000ce60: 3130 2030 2e39 3531 3036 2020 2020 302e  10 0.95106    0.
-0000ce70: 3135 2030 2e33 3039 3032 0a20 2020 2020  15 0.30902.     
-0000ce80: 2020 2020 2020 2020 2020 2030 2e32 302d             0.20-
-0000ce90: 302e 3538 3737 3920 2020 2030 2e32 352d  0.58779    0.25-
-0000cea0: 312e 3030 3030 3020 2020 2030 2e33 302d  1.00000    0.30-
-0000ceb0: 302e 3538 3737 3920 2020 2030 2e33 3520  0.58779    0.35 
-0000cec0: 302e 3330 3930 320a 2020 2020 2020 2020  0.30902.        
-0000ced0: 2020 2020 2020 2020 302e 3430 2030 2e39          0.40 0.9
-0000cee0: 3531 3036 2020 2020 302e 3435 2030 2e38  5106    0.45 0.8
-0000cef0: 3039 3032 2020 2020 302e 3530 2030 2e30  0902    0.50 0.0
-0000cf00: 3030 3030 2020 2020 302e 3535 2d30 2e38  0000    0.55-0.8
-0000cf10: 3039 3032 0a20 2020 2020 2020 2020 2020  0902.           
-0000cf20: 2020 2020 2030 2e36 302d 302e 3935 3130       0.60-0.9510
-0000cf30: 3620 2020 2030 2e36 352d 302e 3330 3930  6    0.65-0.3090
-0000cf40: 3220 2020 2030 2e37 3020 302e 3538 3737  2    0.70 0.5877
-0000cf50: 3920 2020 2030 2e37 3520 312e 3030 3030  9    0.75 1.0000
-0000cf60: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0000cf70: 2020 302e 3830 2030 2e35 3837 3739 2020    0.80 0.58779  
-0000cf80: 2020 302e 3835 2d30 2e33 3039 3032 2020    0.85-0.30902  
-0000cf90: 2020 302e 3930 2d30 2e39 3531 3036 454e    0.90-0.95106EN
-0000cfa0: 4454 0a20 2020 203e 3e3e 206e 6173 7472  DT.    >>> nastr
-0000cfb0: 616e 2e77 7474 6162 6c65 6431 2831 2c20  an.wttabled1(1, 
-0000cfc0: 3430 3030 2c20 5b31 2c20 322c 2033 5d2c  4000, [1, 2, 3],
-0000cfd0: 205b 312c 2032 2c20 335d 2c0a 2020 2020   [1, 2, 3],.    
-0000cfe0: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
-0000cff0: 2020 2020 2020 666f 726d 3d27 7b3a 3136        form='{:16
-0000d000: 2e32 667d 7b3a 3136 2e35 667d 2729 0a20  .2f}{:16.5f}'). 
-0000d010: 2020 2054 4142 4c45 4431 2a20 2020 2020     TABLED1*     
-0000d020: 2020 2020 2020 2034 3030 300a 2020 2020         4000.    
-0000d030: 2a0a 2020 2020 2a20 2020 2020 2020 2020  *.    *         
-0000d040: 2020 2020 2020 2020 2020 312e 3030 2020            1.00  
-0000d050: 2020 2020 2020 2031 2e30 3030 3030 2020         1.00000  
-0000d060: 2020 2020 2020 2020 2020 322e 3030 2020            2.00  
-0000d070: 2020 2020 2020 2032 2e30 3030 3030 0a20         2.00000. 
-0000d080: 2020 202a 2020 2020 2020 2020 2020 2020     *            
-0000d090: 2020 2020 2020 2033 2e30 3020 2020 2020         3.00     
-0000d0a0: 2020 2020 332e 3030 3030 3045 4e44 540a      3.00000ENDT.
-0000d0b0: 2020 2020 2222 220a 2020 2020 742c 2064      """.    t, d
-0000d0c0: 203d 206e 702e 6174 6c65 6173 745f 3164   = np.atleast_1d
-0000d0d0: 2874 2c20 6429 0a20 2020 2074 203d 2074  (t, d).    t = t
-0000d0e0: 2e72 6176 656c 2829 0a20 2020 2064 203d  .ravel().    d =
-0000d0f0: 2064 2e72 6176 656c 2829 0a20 2020 206e   d.ravel().    n
-0000d100: 7074 7320 3d20 6c65 6e28 7429 0a20 2020  pts = len(t).   
-0000d110: 2069 6620 6c65 6e28 6429 2021 3d20 6e70   if len(d) != np
-0000d120: 7473 3a0a 2020 2020 2020 2020 7261 6973  ts:.        rais
-0000d130: 6520 5661 6c75 6545 7272 6f72 2866 226c  e ValueError(f"l
-0000d140: 656e 2864 2920 6973 207b 6c65 6e28 6429  en(d) is {len(d)
-0000d150: 7d20 6275 7420 6c65 6e28 7429 2069 7320  } but len(t) is 
-0000d160: 7b6e 7074 737d 2229 0a0a 2020 2020 2320  {npts}")..    # 
-0000d170: 6465 7465 726d 696e 6520 6966 2075 7369  determine if usi
-0000d180: 6e67 2073 696e 676c 6520 6f72 2064 6f75  ng single or dou
-0000d190: 626c 6520 6669 656c 643a 0a20 2020 206e  ble field:.    n
-0000d1a0: 203d 206c 656e 2866 6f72 6d2e 666f 726d   = len(form.form
-0000d1b0: 6174 2831 2c20 3129 290a 2020 2020 6966  at(1, 1)).    if
-0000d1c0: 206e 2021 3d20 3136 2061 6e64 206e 2021   n != 16 and n !
-0000d1d0: 3d20 3332 3a0a 2020 2020 2020 2020 7261  = 32:.        ra
-0000d1e0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-0000d1f0: 2260 666f 726d 6020 7072 6f64 7563 6573  "`form` produces
-0000d200: 2061 207b 6e7d 206c 656e 6774 6820 7374   a {n} length st
-0000d210: 7269 6e67 2e20 4974 206d 7573 7420 6265  ring. It must be
-0000d220: 2031 3620 6f72 2033 322e 2229 0a20 2020   16 or 32.").   
-0000d230: 2069 6620 7469 746c 653a 0a20 2020 2020   if title:.     
-0000d240: 2020 2066 2e77 7269 7465 2866 2224 207b     f.write(f"$ {
-0000d250: 7469 746c 653a 737d 5c6e 2229 0a20 2020  title:s}\n").   
-0000d260: 2069 6620 6e20 3d3d 2033 323a 0a20 2020   if n == 32:.   
-0000d270: 2020 2020 2074 6162 6c65 7374 7220 3d20       tablestr = 
-0000d280: 7461 626c 6573 7472 202b 2022 2a22 0a20  tablestr + "*". 
-0000d290: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
-0000d2a0: 227b 7461 626c 6573 7472 3a3c 3873 7d7b  "{tablestr:<8s}{
-0000d2b0: 7469 643a 3136 647d 5c6e 2a5c 6e22 290a  tid:16d}\n*\n").
-0000d2c0: 2020 2020 2020 2020 726f 7773 203d 206e          rows = n
-0000d2d0: 7074 7320 2f2f 2032 0a20 2020 2020 2020  pts // 2.       
-0000d2e0: 2072 203d 2072 6f77 7320 2a20 320a 2020   r = rows * 2.  
-0000d2f0: 2020 2020 2020 7772 6974 6572 2e76 6563        writer.vec
-0000d300: 7772 6974 6528 0a20 2020 2020 2020 2020  write(.         
-0000d310: 2020 2066 2c20 222a 2020 2020 2020 2022     f, "*       "
-0000d320: 202b 2066 6f72 6d20 2a20 3220 2b20 225c   + form * 2 + "\
-0000d330: 6e22 2c20 745b 3a72 3a32 5d2c 2064 5b3a  n", t[:r:2], d[:
-0000d340: 723a 325d 2c20 745b 313a 723a 325d 2c20  r:2], t[1:r:2], 
-0000d350: 645b 313a 723a 325d 0a20 2020 2020 2020  d[1:r:2].       
-0000d360: 2029 0a20 2020 2020 2020 2066 2e77 7269   ).        f.wri
-0000d370: 7465 2822 2a20 2020 2020 2020 2229 0a20  te("*       "). 
-0000d380: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-0000d390: 7261 6e67 6528 722c 206e 7074 7329 3a0a  range(r, npts):.
-0000d3a0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-0000d3b0: 6974 6528 666f 726d 2e66 6f72 6d61 7428  ite(form.format(
-0000d3c0: 745b 6a5d 2c20 645b 6a5d 2929 0a20 2020  t[j], d[j])).   
-0000d3d0: 2065 6c73 653a 0a20 2020 2020 2020 2066   else:.        f
-0000d3e0: 2e77 7269 7465 2866 227b 7461 626c 6573  .write(f"{tables
-0000d3f0: 7472 3a3c 3873 7d7b 7469 643a 3864 7d5c  tr:<8s}{tid:8d}\
-0000d400: 6e22 290a 2020 2020 2020 2020 726f 7773  n").        rows
-0000d410: 203d 206e 7074 7320 2f2f 2034 0a20 2020   = npts // 4.   
-0000d420: 2020 2020 2072 203d 2072 6f77 7320 2a20       r = rows * 
-0000d430: 340a 2020 2020 2020 2020 7772 6974 6572  4.        writer
-0000d440: 2e76 6563 7772 6974 6528 0a20 2020 2020  .vecwrite(.     
-0000d450: 2020 2020 2020 2066 2c0a 2020 2020 2020         f,.      
-0000d460: 2020 2020 2020 2220 2020 2020 2020 2022        "        "
-0000d470: 202b 2066 6f72 6d20 2a20 3420 2b20 225c   + form * 4 + "\
-0000d480: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-0000d490: 745b 3a72 3a34 5d2c 0a20 2020 2020 2020  t[:r:4],.       
-0000d4a0: 2020 2020 2064 5b3a 723a 345d 2c0a 2020       d[:r:4],.  
-0000d4b0: 2020 2020 2020 2020 2020 745b 313a 723a            t[1:r:
-0000d4c0: 345d 2c0a 2020 2020 2020 2020 2020 2020  4],.            
-0000d4d0: 645b 313a 723a 345d 2c0a 2020 2020 2020  d[1:r:4],.      
-0000d4e0: 2020 2020 2020 745b 323a 723a 345d 2c0a        t[2:r:4],.
-0000d4f0: 2020 2020 2020 2020 2020 2020 645b 323a              d[2:
-0000d500: 723a 345d 2c0a 2020 2020 2020 2020 2020  r:4],.          
-0000d510: 2020 745b 333a 723a 345d 2c0a 2020 2020    t[3:r:4],.    
-0000d520: 2020 2020 2020 2020 645b 333a 723a 345d          d[3:r:4]
-0000d530: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000d540: 2020 2020 662e 7772 6974 6528 2220 2020      f.write("   
-0000d550: 2020 2020 2022 290a 2020 2020 2020 2020       ").        
-0000d560: 666f 7220 6a20 696e 2072 616e 6765 2872  for j in range(r
-0000d570: 2c20 6e70 7473 293a 0a20 2020 2020 2020  , npts):.       
-0000d580: 2020 2020 2066 2e77 7269 7465 2866 6f72       f.write(for
-0000d590: 6d2e 666f 726d 6174 2874 5b6a 5d2c 2064  m.format(t[j], d
-0000d5a0: 5b6a 5d29 290a 2020 2020 662e 7772 6974  [j])).    f.writ
-0000d5b0: 6528 2245 4e44 545c 6e22 290a 0a0a 6465  e("ENDT\n")...de
-0000d5c0: 6620 6275 6c6b 3275 7365 7428 2a61 7267  f bulk2uset(*arg
-0000d5d0: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
-0000d5e0: 5265 6164 2043 4f52 4432 2a20 616e 6420  Read CORD2* and 
-0000d5f0: 4752 4944 2063 6172 6473 2066 726f 6d20  GRID cards from 
-0000d600: 6669 6c65 2873 2920 746f 206d 616b 6520  file(s) to make 
-0000d610: 6120 5553 4554 2074 6162 6c65 0a0a 2020  a USET table..  
-0000d620: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000d630: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000d640: 2a61 7267 730a 2020 2020 2020 2020 4669  *args.        Fi
-0000d650: 6c65 206e 616d 6573 206f 7220 6669 6c65  le names or file
-0000d660: 2068 616e 646c 6573 2061 7320 7265 7475   handles as retu
-0000d670: 726e 6564 2062 7920 3a66 756e 633a 606f  rned by :func:`o
-0000d680: 7065 6e60 2e20 4669 6c65 730a 2020 2020  pen`. Files.    
-0000d690: 2020 2020 7265 6665 7272 6564 2074 6f20      referred to 
-0000d6a0: 6279 2068 616e 646c 6520 6172 6520 7265  by handle are re
-0000d6b0: 776f 756e 6420 6669 7273 742e 2041 2047  wound first. A G
-0000d6c0: 5549 2069 7320 6f70 656e 2066 6f72 0a20  UI is open for. 
-0000d6d0: 2020 2020 2020 2066 696c 6520 7365 6c65         file sele
-0000d6e0: 6374 696f 6e20 6966 206e 6f20 6172 6775  ction if no argu
-0000d6f0: 6d65 6e74 7320 6172 6520 7072 6f76 6964  ments are provid
-0000d700: 6564 206f 7220 6966 2061 6e20 6172 6775  ed or if an argu
-0000d710: 6d65 6e74 0a20 2020 2020 2020 2069 7320  ment.        is 
-0000d720: 6569 7468 6572 2061 2064 6972 6563 746f  either a directo
-0000d730: 7279 206e 616d 6520 6f72 204e 6f6e 652e  ry name or None.
-0000d740: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0000d750: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7573    -------.    us
-0000d760: 6574 203a 2070 616e 6461 7320 4461 7461  et : pandas Data
-0000d770: 4672 616d 650a 2020 2020 2020 2020 4120  Frame.        A 
-0000d780: 4461 7461 4672 616d 6520 6173 206f 7574  DataFrame as out
-0000d790: 7075 7420 6279 0a20 2020 2020 2020 203a  put by.        :
-0000d7a0: 6675 6e63 3a60 7079 7965 7469 2e6e 6173  func:`pyyeti.nas
-0000d7b0: 7472 616e 2e6f 7032 2e4f 5032 2e72 646e  tran.op2.OP2.rdn
-0000d7c0: 3263 6f70 3260 0a20 2020 2063 6f6f 7264  2cop2`.    coord
-0000d7d0: 7265 6620 3a20 6469 6374 696f 6e61 7279  ref : dictionary
-0000d7e0: 0a20 2020 2020 2020 2044 6963 7469 6f6e  .        Diction
-0000d7f0: 6172 7920 7769 7468 2074 6865 206b 6579  ary with the key
-0000d800: 7320 6265 696e 6720 7468 6520 636f 6f72  s being the coor
-0000d810: 6469 6e61 7465 2073 7973 7465 6d20 6964  dinate system id
-0000d820: 2061 6e64 0a20 2020 2020 2020 2074 6865   and.        the
-0000d830: 2076 616c 7565 7320 6265 696e 6720 7468   values being th
-0000d840: 6520 3578 3320 6d61 7472 6978 3a3a 0a0a  e 5x3 matrix::..
-0000d850: 2020 2020 2020 2020 2020 2020 5b69 6420              [id 
-0000d860: 2074 7970 6520 305d 2020 2320 6f75 7470   type 0]  # outp
-0000d870: 7574 2063 6f6f 7264 2e20 7379 732e 2069  ut coord. sys. i
-0000d880: 6420 616e 6420 7479 7065 0a20 2020 2020  d and type.     
-0000d890: 2020 2020 2020 205b 786f 2020 796f 2020         [xo  yo  
-0000d8a0: 7a6f 5d20 2023 206f 7269 6769 6e20 6f66  zo]  # origin of
-0000d8b0: 2063 6f6f 7264 2e20 7379 7374 656d 0a20   coord. system. 
-0000d8c0: 2020 2020 2020 2020 2020 205b 2020 2020             [    
-0000d8d0: 5420 2020 2020 5d20 2023 2033 7833 2074  T     ]  # 3x3 t
-0000d8e0: 7261 6e73 666f 726d 6174 696f 6e20 746f  ransformation to
-0000d8f0: 2062 6173 6963 0a20 2020 2020 2020 2020   basic.         
-0000d900: 2020 204e 6f74 6520 7468 6174 2054 2069     Note that T i
-0000d910: 7320 666f 7220 7468 6520 636f 6f72 6469  s for the coordi
-0000d920: 6e61 7465 2073 7973 7465 6d2c 206e 6f74  nate system, not
-0000d930: 2061 2067 7269 640a 2020 2020 2020 2020   a grid.        
-0000d940: 2020 2020 2875 6e6c 6573 7320 7479 7065      (unless type
-0000d950: 203d 2031 2077 6869 6368 206d 6561 6e73   = 1 which means
-0000d960: 2072 6563 7461 6e67 756c 6172 290a 0a20   rectangular).. 
-0000d970: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-0000d980: 2d2d 0a20 2020 2054 6869 7320 6973 2074  --.    This is t
-0000d990: 6865 2072 6576 6572 7365 206f 6620 3a66  he reverse of :f
-0000d9a0: 756e 633a 6075 7365 7432 6275 6c6b 602e  unc:`uset2bulk`.
-0000d9b0: 0a0a 2020 2020 4e6f 7465 2074 6861 7420  ..    Note that 
-0000d9c0: 3a66 756e 633a 6061 736d 3275 7365 7460  :func:`asm2uset`
-0000d9d0: 2069 7320 7369 6d69 6c61 7220 746f 2074   is similar to t
-0000d9e0: 6869 7320 726f 7574 696e 6520 6275 7420  his routine but 
-0000d9f0: 7772 6974 7465 6e0a 2020 2020 7370 6563  written.    spec
-0000da00: 6966 6963 616c 6c79 2066 6f72 204e 6173  ifically for Nas
-0000da10: 7472 616e 202e 6173 6d20 6669 6c65 732e  tran .asm files.
-0000da20: 2054 6861 7420 726f 7574 696e 6520 7769   That routine wi
-0000da30: 6c6c 2072 6574 7572 6e20 610a 2020 2020  ll return a.    
-0000da40: 5553 4554 2074 6162 6c65 206f 7264 6572  USET table order
-0000da50: 6564 2074 6f20 6d61 7463 6820 7468 6520  ed to match the 
-0000da60: 6d6f 6465 6c20 2861 6363 6f72 6469 6e67  model (according
-0000da70: 2074 6f20 7468 6520 5345 434f 4e43 540a   to the SECONCT.
-0000da80: 2020 2020 6361 7264 293b 2069 7420 616c      card); it al
-0000da90: 736f 2072 6574 7572 6e73 2061 2062 2d73  so returns a b-s
-0000daa0: 6574 2062 6f6f 6c65 616e 2070 6172 7469  et boolean parti
-0000dab0: 7469 6f6e 2076 6563 746f 722e 0a0a 2020  tion vector...  
-0000dac0: 2020 416c 6c20 6772 6964 7320 6172 6520    All grids are 
-0000dad0: 7075 7420 696e 2074 6865 2027 6227 2073  put in the 'b' s
-0000dae0: 6574 2e20 5468 6973 2072 6f75 7469 6e65  et. This routine
-0000daf0: 2075 7365 730a 2020 2020 3a66 756e 633a   uses.    :func:
-0000db00: 6070 7979 6574 692e 6e61 7374 7261 6e2e  `pyyeti.nastran.
-0000db10: 6e32 702e 6164 6467 7269 6460 2074 6f20  n2p.addgrid` to 
-0000db20: 6275 696c 6420 7468 6520 6f75 7470 7574  build the output
-0000db30: 2e0a 0a20 2020 2053 6565 2061 6c73 6f0a  ...    See also.
-0000db40: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-0000db50: 203a 6675 6e63 3a60 6173 6d32 7573 6574   :func:`asm2uset
-0000db60: 602c 203a 6675 6e63 3a60 7573 6574 3262  `, :func:`uset2b
-0000db70: 756c 6b60 2c20 3a66 756e 633a 6072 6463  ulk`, :func:`rdc
-0000db80: 6172 6473 602c 0a20 2020 203a 6675 6e63  ards`,.    :func
-0000db90: 3a60 7264 6772 6964 7360 2c20 3a66 756e  :`rdgrids`, :fun
-0000dba0: 633a 6070 7979 6574 692e 6e61 7374 7261  c:`pyyeti.nastra
-0000dbb0: 6e2e 6f70 322e 4f50 322e 7264 6e32 636f  n.op2.OP2.rdn2co
-0000dbc0: 7032 602c 0a20 2020 203a 6d6f 643a 6070  p2`,.    :mod:`p
-0000dbd0: 7979 6574 692e 6e61 7374 7261 6e2e 6e32  yyeti.nastran.n2
-0000dbe0: 7060 2e0a 2020 2020 2222 220a 2020 2020  p`..    """.    
-0000dbf0: 6772 6964 7320 3d20 6e70 2e7a 6572 6f73  grids = np.zeros
-0000dc00: 2828 302c 2038 2929 0a20 2020 2063 6f6f  ((0, 8)).    coo
-0000dc10: 7264 7320 3d20 7b7d 0a0a 2020 2020 6966  rds = {}..    if
-0000dc20: 206c 656e 2861 7267 7329 203d 3d20 303a   len(args) == 0:
-0000dc30: 0a20 2020 2020 2020 2061 7267 7320 3d20  .        args = 
-0000dc40: 5b4e 6f6e 655d 0a0a 2020 2020 666f 7220  [None]..    for 
-0000dc50: 6620 696e 2061 7267 733a 0a20 2020 2020  f in args:.     
-0000dc60: 2020 2066 203d 2067 7569 746f 6f6c 732e     f = guitools.
-0000dc70: 6765 745f 6669 6c65 5f6e 616d 6528 662c  get_file_name(f,
-0000dc80: 2072 6561 643d 5472 7565 290a 2020 2020   read=True).    
-0000dc90: 2020 2020 636f 6f72 6473 2e75 7064 6174      coords.updat
-0000dca0: 6528 7264 636f 7264 3263 6172 6473 2866  e(rdcord2cards(f
-0000dcb0: 2929 0a20 2020 2020 2020 2067 203d 2072  )).        g = r
-0000dcc0: 6467 7269 6473 2866 290a 2020 2020 2020  dgrids(f).      
-0000dcd0: 2020 6966 2067 2069 7320 6e6f 7420 4e6f    if g is not No
-0000dce0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000dcf0: 6772 6964 7320 3d20 6e70 2e76 7374 6163  grids = np.vstac
-0000dd00: 6b28 2867 7269 6473 2c20 6729 290a 0a20  k((grids, g)).. 
-0000dd10: 2020 2069 203d 206e 702e 6172 6773 6f72     i = np.argsor
-0000dd20: 7428 6772 6964 735b 3a2c 2030 5d29 0a20  t(grids[:, 0]). 
-0000dd30: 2020 2067 7269 6473 203d 2067 7269 6473     grids = grids
-0000dd40: 5b69 2c20 3a5d 0a20 2020 2075 7365 7420  [i, :].    uset 
-0000dd50: 3d20 6e32 702e 6164 6467 7269 6428 0a20  = n2p.addgrid(. 
-0000dd60: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
-0000dd70: 2020 2020 2067 7269 6473 5b3a 2c20 305d       grids[:, 0]
-0000dd80: 2e61 7374 7970 6528 6e70 2e69 6e74 3634  .astype(np.int64
-0000dd90: 292c 0a20 2020 2020 2020 2022 6222 2c0a  ),.        "b",.
-0000dda0: 2020 2020 2020 2020 6772 6964 735b 3a2c          grids[:,
-0000ddb0: 2031 5d2c 0a20 2020 2020 2020 2067 7269   1],.        gri
-0000ddc0: 6473 5b3a 2c20 323a 355d 2c0a 2020 2020  ds[:, 2:5],.    
-0000ddd0: 2020 2020 6772 6964 735b 3a2c 2035 5d2c      grids[:, 5],
-0000dde0: 0a20 2020 2020 2020 2063 6f6f 7264 732c  .        coords,
-0000ddf0: 0a20 2020 2029 0a20 2020 2072 6574 7572  .    ).    retur
-0000de00: 6e20 7573 6574 2c20 636f 6f72 6473 0a0a  n uset, coords..
-0000de10: 0a40 6775 6974 6f6f 6c73 2e77 7269 7465  .@guitools.write
-0000de20: 5f74 6578 745f 6669 6c65 0a64 6566 2075  _text_file.def u
-0000de30: 7365 7432 6275 6c6b 2866 2c20 7573 6574  set2bulk(f, uset
-0000de40: 293a 0a20 2020 2022 2222 0a20 2020 2057  ):.    """.    W
-0000de50: 7269 7465 2043 4f52 4432 2a20 616e 6420  rite CORD2* and 
-0000de60: 4752 4944 2063 6172 6473 2066 726f 6d20  GRID cards from 
-0000de70: 6120 5553 4554 2074 6162 6c65 0a0a 2020  a USET table..  
-0000de80: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000de90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000dea0: 6620 3a20 7374 7269 6e67 206f 7220 6669  f : string or fi
-0000deb0: 6c65 5f6c 696b 6520 6f72 2031 206f 7220  le_like or 1 or 
-0000dec0: 4e6f 6e65 0a20 2020 2020 2020 2045 6974  None.        Eit
-0000ded0: 6865 7220 6120 6e61 6d65 206f 6620 6120  her a name of a 
-0000dee0: 6669 6c65 2c20 6f72 2069 7320 6120 6669  file, or is a fi
-0000def0: 6c65 5f6c 696b 6520 6f62 6a65 6374 2061  le_like object a
-0000df00: 7320 7265 7475 726e 6564 0a20 2020 2020  s returned.     
-0000df10: 2020 2062 7920 3a66 756e 633a 606f 7065     by :func:`ope
-0000df20: 6e60 206f 7220 3a63 6c61 7373 3a60 696f  n` or :class:`io
-0000df30: 2e53 7472 696e 6749 4f60 2e20 496e 7075  .StringIO`. Inpu
-0000df40: 7420 6173 2069 6e74 6567 6572 2031 2074  t as integer 1 t
-0000df50: 6f0a 2020 2020 2020 2020 7772 6974 6520  o.        write 
-0000df60: 746f 2073 7464 6f75 742e 2043 616e 2061  to stdout. Can a
-0000df70: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
-0000df80: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
-0000df90: 7220 4e6f 6e65 3b0a 2020 2020 2020 2020  r None;.        
-0000dfa0: 696e 2074 6865 7365 2063 6173 6573 2c20  in these cases, 
-0000dfb0: 6120 4755 4920 6973 206f 7065 6e65 6420  a GUI is opened 
-0000dfc0: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
-0000dfd0: 6f6e 2e0a 2020 2020 7573 6574 203a 2070  on..    uset : p
-0000dfe0: 616e 6461 7320 4461 7461 4672 616d 650a  andas DataFrame.
-0000dff0: 2020 2020 2020 2020 4120 4461 7461 4672          A DataFr
-0000e000: 616d 6520 6173 206f 7574 7075 7420 6279  ame as output by
-0000e010: 0a20 2020 2020 2020 203a 6675 6e63 3a60  .        :func:`
-0000e020: 7079 7965 7469 2e6e 6173 7472 616e 2e6f  pyyeti.nastran.o
-0000e030: 7032 2e4f 5032 2e72 646e 3263 6f70 3260  p2.OP2.rdn2cop2`
-0000e040: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0000e050: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f    -------.    No
-0000e060: 6e65 0a0a 2020 2020 4e6f 7465 730a 2020  ne..    Notes.  
-0000e070: 2020 2d2d 2d2d 2d0a 2020 2020 5468 6973    -----.    This
-0000e080: 2069 7320 7468 6520 7265 7665 7273 6520   is the reverse 
-0000e090: 6f66 203a 6675 6e63 3a60 6275 6c6b 3275  of :func:`bulk2u
-0000e0a0: 7365 7460 2e0a 0a20 2020 2053 6565 2061  set`...    See a
-0000e0b0: 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d  lso.    --------
-0000e0c0: 0a20 2020 203a 6675 6e63 3a60 6275 6c6b  .    :func:`bulk
-0000e0d0: 3275 7365 7460 2c20 3a66 756e 633a 6070  2uset`, :func:`p
-0000e0e0: 7979 6574 692e 6e61 7374 7261 6e2e 6e32  yyeti.nastran.n2
-0000e0f0: 702e 6d6b 636f 7264 6361 7264 696e 666f  p.mkcordcardinfo
-0000e100: 602c 0a20 2020 203a 6675 6e63 3a60 7774  `,.    :func:`wt
-0000e110: 636f 6f72 6463 6172 6473 602c 203a 6675  coordcards`, :fu
-0000e120: 6e63 3a60 7774 6772 6964 7360 2e0a 2020  nc:`wtgrids`..  
-0000e130: 2020 2222 220a 0a20 2020 2023 2047 6574    """..    # Get
-0000e140: 2073 6f6d 6520 6461 7461 2066 726f 6d20   some data from 
-0000e150: 7468 6520 7573 6574 2074 6162 6c65 3a0a  the uset table:.
-0000e160: 2020 2020 6369 203d 206e 3270 2e6d 6b63      ci = n2p.mkc
-0000e170: 6f72 6463 6172 6469 6e66 6f28 7573 6574  ordcardinfo(uset
-0000e180: 290a 2020 2020 6772 6964 7320 3d20 7573  ).    grids = us
-0000e190: 6574 2e69 6e64 6578 2e67 6574 5f6c 6576  et.index.get_lev
-0000e1a0: 656c 5f76 616c 7565 7328 2269 6422 290a  el_values("id").
-0000e1b0: 2020 2020 646f 6620 3d20 7573 6574 2e69      dof = uset.i
-0000e1c0: 6e64 6578 2e67 6574 5f6c 6576 656c 5f76  ndex.get_level_v
-0000e1d0: 616c 7565 7328 2264 6f66 2229 0a20 2020  alues("dof").   
-0000e1e0: 2070 7620 3d20 646f 6620 3d3d 2031 0a20   pv = dof == 1. 
-0000e1f0: 2020 2067 7269 6473 203d 2067 7269 6473     grids = grids
-0000e200: 5b70 765d 0a20 2020 2078 797a 203d 2075  [pv].    xyz = u
-0000e210: 7365 742e 6c6f 635b 7076 2c20 2278 223a  set.loc[pv, "x":
-0000e220: 227a 225d 2e76 616c 7565 730a 2020 2020  "z"].values.    
-0000e230: 7076 203d 2064 6f66 203d 3d20 320a 2020  pv = dof == 2.  
-0000e240: 2020 6364 203d 2075 7365 742e 6c6f 635b    cd = uset.loc[
-0000e250: 7076 2c20 2278 225d 2e76 616c 7565 732e  pv, "x"].values.
-0000e260: 6173 7479 7065 2869 6e74 290a 0a20 2020  astype(int)..   
-0000e270: 2023 2057 7269 7465 2063 6f6f 7264 696e   # Write coordin
-0000e280: 6174 6520 7379 7374 656d 2063 6172 6473  ate system cards
-0000e290: 2069 6620 6e65 6564 6564 3a0a 2020 2020   if needed:.    
-0000e2a0: 6966 2063 693a 0a20 2020 2020 2020 2066  if ci:.        f
-0000e2b0: 2e77 7269 7465 2822 245c 6e24 2043 4f4f  .write("$\n$ COO
-0000e2c0: 5244 494e 4154 4520 5359 5354 454d 2044  RDINATE SYSTEM D
-0000e2d0: 4154 415c 6e24 5c6e 2229 0a20 2020 2020  ATA\n$\n").     
-0000e2e0: 2020 2077 7463 6f6f 7264 6361 7264 7328     wtcoordcards(
-0000e2f0: 662c 2063 6929 0a0a 2020 2020 2320 5772  f, ci)..    # Wr
-0000e300: 6974 6520 4772 6964 2064 6174 613a 0a20  ite Grid data:. 
-0000e310: 2020 2066 2e77 7269 7465 2822 245c 6e24     f.write("$\n$
-0000e320: 2047 5249 4420 4441 5441 5c6e 245c 6e22   GRID DATA\n$\n"
-0000e330: 290a 2020 2020 7774 6772 6964 7328 662c  ).    wtgrids(f,
-0000e340: 2067 7269 6473 2c20 302c 2078 797a 2c20   grids, 0, xyz, 
-0000e350: 6364 290a 0a0a 6465 6620 7264 7370 6f69  cd)...def rdspoi
-0000e360: 6e74 7328 6629 3a0a 2020 2020 7222 2222  nts(f):.    r"""
-0000e370: 0a20 2020 2052 6561 6420 4e61 7374 7261  .    Read Nastra
-0000e380: 6e20 5350 4f49 4e54 2063 6172 6473 2066  n SPOINT cards f
-0000e390: 726f 6d20 6120 4e61 7374 7261 6e20 6275  rom a Nastran bu
-0000e3a0: 6c6b 2066 696c 652e 0a0a 2020 2020 5061  lk file...    Pa
-0000e3b0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0000e3c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6620 3a20  -------.    f : 
-0000e3d0: 7374 7269 6e67 206f 7220 6669 6c65 5f6c  string or file_l
-0000e3e0: 696b 6520 6f72 204e 6f6e 650a 2020 2020  ike or None.    
-0000e3f0: 2020 2020 4569 7468 6572 2061 206e 616d      Either a nam
-0000e400: 6520 6f66 2061 2066 696c 652c 206f 7220  e of a file, or 
-0000e410: 6973 2061 2066 696c 655f 6c69 6b65 206f  is a file_like o
-0000e420: 626a 6563 7420 6173 2072 6574 7572 6e65  bject as returne
-0000e430: 640a 2020 2020 2020 2020 6279 203a 6675  d.        by :fu
-0000e440: 6e63 3a60 6f70 656e 602e 2049 6620 6669  nc:`open`. If fi
-0000e450: 6c65 5f6c 696b 6520 6f62 6a65 6374 2c20  le_like object, 
-0000e460: 6974 2069 7320 7265 776f 756e 6420 6669  it is rewound fi
-0000e470: 7273 742e 2043 616e 0a20 2020 2020 2020  rst. Can.       
-0000e480: 2061 6c73 6f20 6265 2074 6865 206e 616d   also be the nam
-0000e490: 6520 6f66 2061 2064 6972 6563 746f 7279  e of a directory
-0000e4a0: 206f 7220 4e6f 6e65 3b20 696e 2074 6865   or None; in the
-0000e4b0: 7365 2063 6173 6573 2c20 6120 4755 490a  se cases, a GUI.
-0000e4c0: 2020 2020 2020 2020 6973 206f 7065 6e65          is opene
-0000e4d0: 6420 666f 7220 6669 6c65 2073 656c 6563  d for file selec
-0000e4e0: 7469 6f6e 2e0a 0a20 2020 2052 6574 7572  tion...    Retur
-0000e4f0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0000e500: 2020 2073 706f 696e 7473 203a 2031 6420     spoints : 1d 
-0000e510: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
-0000e520: 4172 7261 7920 6f66 2053 504f 494e 5420  Array of SPOINT 
-0000e530: 6964 732e 2057 696c 6c20 6265 2065 6d70  ids. Will be emp
-0000e540: 7479 2069 6620 6e6f 2053 504f 494e 5420  ty if no SPOINT 
-0000e550: 6361 7264 7320 666f 756e 642e 0a0a 2020  cards found...  
-0000e560: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
-0000e570: 2d0a 2020 2020 5468 6973 2072 6f75 7469  -.    This routi
-0000e580: 6e65 2075 7365 7320 3a66 756e 633a 6072  ne uses :func:`r
-0000e590: 6463 6172 6473 6020 746f 206c 6f61 6420  dcards` to load 
-0000e5a0: 7468 6520 6461 7461 2e0a 0a20 2020 2045  the data...    E
-0000e5b0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-0000e5c0: 2d2d 2d2d 0a20 2020 203e 3e3e 2066 726f  ----.    >>> fro
-0000e5d0: 6d20 7079 7965 7469 2069 6d70 6f72 7420  m pyyeti import 
-0000e5e0: 6e61 7374 7261 6e0a 2020 2020 3e3e 3e20  nastran.    >>> 
-0000e5f0: 6672 6f6d 2069 6f20 696d 706f 7274 2053  from io import S
-0000e600: 7472 696e 6749 4f0a 2020 2020 3e3e 3e20  tringIO.    >>> 
-0000e610: 6275 6c6b 6461 7461 203d 2028 0a20 2020  bulkdata = (.   
-0000e620: 202e 2e2e 2020 2020 2022 5350 4f49 4e54   ...     "SPOINT
-0000e630: 2c31 2c32 2c31 3030 5c6e 220a 2020 2020  ,1,2,100\n".    
-0000e640: 2e2e 2e20 2020 2020 2253 504f 494e 542c  ...     "SPOINT,
-0000e650: 3230 302c 5448 5255 2c32 3032 5c6e 220a  200,THRU,202\n".
-0000e660: 2020 2020 2e2e 2e20 2020 2020 2253 504f      ...     "SPO
-0000e670: 494e 542c 355c 6e22 0a20 2020 202e 2e2e  INT,5\n".    ...
-0000e680: 2029 0a20 2020 203e 3e3e 2077 6974 6820   ).    >>> with 
-0000e690: 5374 7269 6e67 494f 2862 756c 6b64 6174  StringIO(bulkdat
-0000e6a0: 6129 2061 7320 663a 0a20 2020 202e 2e2e  a) as f:.    ...
-0000e6b0: 2020 2020 2073 706f 696e 7473 203d 206e       spoints = n
-0000e6c0: 6173 7472 616e 2e72 6473 706f 696e 7473  astran.rdspoints
-0000e6d0: 2866 290a 2020 2020 3e3e 3e20 7370 6f69  (f).    >>> spoi
-0000e6e0: 6e74 7320 2020 2020 2020 2020 2020 2020  nts             
-0000e6f0: 2020 2020 2020 2020 2023 2064 6f63 7465           # docte
-0000e700: 7374 3a20 2b45 4c4c 4950 5349 530a 2020  st: +ELLIPSIS.  
-0000e710: 2020 6172 7261 7928 5b20 2031 2c20 2020    array([  1,   
-0000e720: 322c 2031 3030 2c20 3230 302c 2032 3031  2, 100, 200, 201
-0000e730: 2c20 3230 322c 2020 2035 5d2e 2e2e 290a  , 202,   5]...).
-0000e740: 2020 2020 3e3e 3e20 7769 7468 2053 7472      >>> with Str
-0000e750: 696e 6749 4f28 226e 6f20 6461 7461 2229  ingIO("no data")
-0000e760: 2061 7320 663a 0a20 2020 202e 2e2e 2020   as f:.    ...  
-0000e770: 2020 2073 706f 696e 7473 203d 206e 6173     spoints = nas
-0000e780: 7472 616e 2e72 6473 706f 696e 7473 2866  tran.rdspoints(f
-0000e790: 290a 2020 2020 3e3e 3e20 7370 6f69 6e74  ).    >>> spoint
-0000e7a0: 7320 2020 2020 2020 2020 2020 2020 2020  s               
-0000e7b0: 2020 2020 2020 2023 2064 6f63 7465 7374         # doctest
-0000e7c0: 3a20 2b45 4c4c 4950 5349 530a 2020 2020  : +ELLIPSIS.    
-0000e7d0: 6172 7261 7928 5b5d 2e2e 2e29 0a0a 2020  array([]...)..  
-0000e7e0: 2020 2222 220a 2020 2020 7370 6f69 6e74    """.    spoint
-0000e7f0: 5f64 6174 6120 3d20 7264 6361 7264 7328  _data = rdcards(
-0000e800: 662c 2022 7370 6f69 6e74 222c 2072 6574  f, "spoint", ret
-0000e810: 7572 6e5f 7661 723d 226c 6973 7422 290a  urn_var="list").
-0000e820: 2020 2020 7370 6f69 6e74 7320 3d20 5b5d      spoints = []
-0000e830: 0a20 2020 2069 6620 7370 6f69 6e74 5f64  .    if spoint_d
-0000e840: 6174 6120 6973 206e 6f74 204e 6f6e 653a  ata is not None:
-0000e850: 0a20 2020 2020 2020 2066 6f72 2063 6172  .        for car
-0000e860: 6420 696e 2073 706f 696e 745f 6461 7461  d in spoint_data
-0000e870: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000e880: 206c 656e 2863 6172 6429 203e 2032 2061   len(card) > 2 a
-0000e890: 6e64 2069 7369 6e73 7461 6e63 6528 6361  nd isinstance(ca
-0000e8a0: 7264 5b31 5d2c 2073 7472 2920 616e 6420  rd[1], str) and 
-0000e8b0: 6361 7264 5b31 5d2e 6c6f 7765 7228 2920  card[1].lower() 
-0000e8c0: 3d3d 2022 7468 7275 223a 0a20 2020 2020  == "thru":.     
-0000e8d0: 2020 2020 2020 2020 2020 2073 706f 696e             spoin
-0000e8e0: 7473 2e65 7874 656e 6428 5b69 2066 6f72  ts.extend([i for
-0000e8f0: 2069 2069 6e20 7261 6e67 6528 6361 7264   i in range(card
-0000e900: 5b30 5d2c 2063 6172 645b 325d 202b 2031  [0], card[2] + 1
-0000e910: 295d 290a 2020 2020 2020 2020 2020 2020  )]).            
-0000e920: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000e930: 2020 2020 2020 7370 6f69 6e74 732e 6578        spoints.ex
-0000e940: 7465 6e64 2863 6172 6429 0a20 2020 2072  tend(card).    r
-0000e950: 6574 7572 6e20 6e70 2e61 7272 6179 2873  eturn np.array(s
-0000e960: 706f 696e 7473 2c20 6474 7970 653d 6e70  points, dtype=np
-0000e970: 2e69 6e74 3634 290a 0a0a 6465 6620 7264  .int64)...def rd
-0000e980: 7365 636f 6e63 7428 6629 3a0a 2020 2020  seconct(f):.    
-0000e990: 7222 2222 0a20 2020 2052 6561 6420 4e61  r""".    Read Na
-0000e9a0: 7374 7261 6e20 5345 434f 4e43 5420 6361  stran SECONCT ca
-0000e9b0: 7264 7320 6672 6f6d 2061 204e 6173 7472  rds from a Nastr
-0000e9c0: 616e 2062 756c 6b20 6669 6c65 2e0a 0a20  an bulk file... 
-0000e9d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000e9e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000e9f0: 2066 203a 2073 7472 696e 6720 6f72 2066   f : string or f
-0000ea00: 696c 655f 6c69 6b65 206f 7220 4e6f 6e65  ile_like or None
-0000ea10: 0a20 2020 2020 2020 2045 6974 6865 7220  .        Either 
-0000ea20: 6120 6e61 6d65 206f 6620 6120 6669 6c65  a name of a file
-0000ea30: 2c20 6f72 2069 7320 6120 6669 6c65 5f6c  , or is a file_l
-0000ea40: 696b 6520 6f62 6a65 6374 2061 7320 7265  ike object as re
-0000ea50: 7475 726e 6564 0a20 2020 2020 2020 2062  turned.        b
-0000ea60: 7920 3a66 756e 633a 606f 7065 6e60 2e20  y :func:`open`. 
-0000ea70: 4966 2066 696c 655f 6c69 6b65 206f 626a  If file_like obj
-0000ea80: 6563 742c 2069 7420 6973 2072 6577 6f75  ect, it is rewou
-0000ea90: 6e64 2066 6972 7374 2e20 4361 6e0a 2020  nd first. Can.  
-0000eaa0: 2020 2020 2020 616c 736f 2062 6520 7468        also be th
-0000eab0: 6520 6e61 6d65 206f 6620 6120 6469 7265  e name of a dire
-0000eac0: 6374 6f72 7920 6f72 204e 6f6e 653b 2069  ctory or None; i
-0000ead0: 6e20 7468 6573 6520 6361 7365 732c 2061  n these cases, a
-0000eae0: 2047 5549 0a20 2020 2020 2020 2069 7320   GUI.        is 
-0000eaf0: 6f70 656e 6564 2066 6f72 2066 696c 6520  opened for file 
-0000eb00: 7365 6c65 6374 696f 6e2e 0a0a 2020 2020  selection...    
-0000eb10: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000eb20: 2d2d 2d0a 2020 2020 615f 6964 732c 2062  ---.    a_ids, b
-0000eb30: 5f69 6473 203a 2031 6420 6e64 6172 7261  _ids : 1d ndarra
-0000eb40: 7973 0a20 2020 2020 2020 2041 7272 6179  ys.        Array
-0000eb50: 206f 6620 4752 4944 2061 6e64 2053 504f   of GRID and SPO
-0000eb60: 494e 5420 6964 7320 666f 7220 7375 7065  INT ids for supe
-0000eb70: 7265 6c65 6d65 6e74 2041 2061 6e64 0a20  relement A and. 
-0000eb80: 2020 2020 2020 2073 7570 6572 656c 656d         superelem
-0000eb90: 656e 7420 422c 2072 6573 7065 6374 6976  ent B, respectiv
-0000eba0: 656c 792e 2042 6f74 6820 6f75 7470 7574  ely. Both output
-0000ebb0: 7320 7769 6c6c 2062 6520 656d 7074 7920  s will be empty 
-0000ebc0: 6966 206e 6f0a 2020 2020 2020 2020 5345  if no.        SE
-0000ebd0: 434f 4e43 5420 6361 7264 7320 666f 756e  CONCT cards foun
-0000ebe0: 642e 0a0a 2020 2020 4e6f 7465 730a 2020  d...    Notes.  
-0000ebf0: 2020 2d2d 2d2d 2d0a 2020 2020 5468 6973    -----.    This
-0000ec00: 2072 6f75 7469 6e65 2075 7365 7320 3a66   routine uses :f
-0000ec10: 756e 633a 6072 6463 6172 6473 6020 746f  unc:`rdcards` to
-0000ec20: 206c 6f61 6420 7468 6520 6461 7461 2e0a   load the data..
-0000ec30: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-0000ec40: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e    --------.    >
-0000ec50: 3e3e 2066 726f 6d20 696f 2069 6d70 6f72  >> from io impor
-0000ec60: 7420 5374 7269 6e67 494f 0a20 2020 203e  t StringIO.    >
-0000ec70: 3e3e 2066 726f 6d20 7079 7965 7469 2069  >> from pyyeti i
-0000ec80: 6d70 6f72 7420 6e61 7374 7261 6e0a 2020  mport nastran.  
-0000ec90: 2020 3e3e 3e20 6275 6c6b 6461 7461 203d    >>> bulkdata =
-0000eca0: 2028 0a20 2020 202e 2e2e 2020 2020 2022   (.    ...     "
-0000ecb0: 5345 434f 4e43 542c 3130 312c 302c 2c4e  SECONCT,101,0,,N
-0000ecc0: 4f5c 6e22 0a20 2020 202e 2e2e 2020 2020  O\n".    ...    
-0000ecd0: 2022 2c33 2c33 302c 3131 2c31 3130 2c31   ",3,30,11,110,1
-0000ece0: 392c 3139 302c 3237 2c32 3730 5c6e 220a  9,190,27,270\n".
-0000ecf0: 2020 2020 2e2e 2e20 2020 2020 2224 5c6e      ...     "$\n
-0000ed00: 220a 2020 2020 2e2e 2e20 2020 2020 2253  ".    ...     "S
-0000ed10: 4543 4f4e 4354 2c31 3031 2c30 2c2c 4e4f  ECONCT,101,0,,NO
-0000ed20: 5c6e 220a 2020 2020 2e2e 2e20 2020 2020  \n".    ...     
-0000ed30: 222c 3131 3031 2c54 4852 552c 3131 3034  ",1101,THRU,1104
-0000ed40: 2c32 3130 312c 5448 5255 2c32 3130 345c  ,2101,THRU,2104\
-0000ed50: 6e22 0a20 2020 202e 2e2e 2029 0a20 2020  n".    ... ).   
-0000ed60: 203e 3e3e 2077 6974 6820 5374 7269 6e67   >>> with String
-0000ed70: 494f 2862 756c 6b64 6174 6129 2061 7320  IO(bulkdata) as 
-0000ed80: 663a 0a20 2020 202e 2e2e 2020 2020 2061  f:.    ...     a
-0000ed90: 5f69 6473 2c20 625f 6964 7320 3d20 6e61  _ids, b_ids = na
-0000eda0: 7374 7261 6e2e 7264 7365 636f 6e63 7428  stran.rdseconct(
-0000edb0: 6629 0a20 2020 203e 3e3e 2061 5f69 6473  f).    >>> a_ids
-0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edd0: 2020 2020 2020 2320 646f 6374 6573 743a        # doctest:
-0000ede0: 202b 454c 4c49 5053 4953 0a20 2020 2061   +ELLIPSIS.    a
-0000edf0: 7272 6179 285b 2020 2033 2c20 2020 3131  rray([   3,   11
-0000ee00: 2c20 2020 3139 2c20 2020 3237 2c20 3131  ,   19,   27, 11
-0000ee10: 3031 2c20 3131 3032 2c20 3131 3033 2c20  01, 1102, 1103, 
-0000ee20: 3131 3034 5d2e 2e2e 290a 2020 2020 3e3e  1104]...).    >>
-0000ee30: 3e20 625f 6964 7320 2020 2020 2020 2020  > b_ids         
-0000ee40: 2020 2020 2020 2020 2020 2020 2023 2064               # d
-0000ee50: 6f63 7465 7374 3a20 2b45 4c4c 4950 5349  octest: +ELLIPSI
-0000ee60: 530a 2020 2020 6172 7261 7928 5b20 2033  S.    array([  3
-0000ee70: 302c 2020 3131 302c 2020 3139 302c 2020  0,  110,  190,  
-0000ee80: 3237 302c 2032 3130 312c 2032 3130 322c  270, 2101, 2102,
-0000ee90: 2032 3130 332c 2032 3130 345d 2e2e 2e29   2103, 2104]...)
-0000eea0: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-0000eeb0: 6620 5f67 6574 5f70 6169 7273 2863 6172  f _get_pairs(car
-0000eec0: 6429 3a0a 2020 2020 2020 2020 2320 7472  d):.        # tr
-0000eed0: 756e 6361 7465 2061 6e64 2066 696c 7465  uncate and filte
-0000eee0: 7220 6f75 7420 626c 616e 6b73 3a0a 2020  r out blanks:.  
-0000eef0: 2020 2020 2020 6361 7264 203d 205b 6920        card = [i 
-0000ef00: 666f 7220 6920 696e 2063 6172 645b 383a  for i in card[8:
-0000ef10: 5d20 6966 2069 5d0a 2020 2020 2020 2020  ] if i].        
-0000ef20: 6974 203d 2069 7465 7228 6361 7264 290a  it = iter(card).
-0000ef30: 2020 2020 2020 2020 666f 7220 612c 2062          for a, b
-0000ef40: 2069 6e20 7a69 7028 6974 2c20 6974 293a   in zip(it, it):
-0000ef50: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
-0000ef60: 6c64 2061 2c20 620a 0a20 2020 2073 6563  ld a, b..    sec
-0000ef70: 6f6e 6374 5f64 6174 6120 3d20 7264 6361  onct_data = rdca
-0000ef80: 7264 7328 662c 2022 7365 636f 6e63 7422  rds(f, "seconct"
-0000ef90: 2c20 7265 7475 726e 5f76 6172 3d22 6c69  , return_var="li
-0000efa0: 7374 2229 0a20 2020 2061 5f69 6473 203d  st").    a_ids =
-0000efb0: 205b 5d0a 2020 2020 625f 6964 7320 3d20   [].    b_ids = 
-0000efc0: 5b5d 0a20 2020 2069 6620 7365 636f 6e63  [].    if seconc
-0000efd0: 745f 6461 7461 2069 7320 6e6f 7420 4e6f  t_data is not No
-0000efe0: 6e65 3a0a 2020 2020 2020 2020 666f 7220  ne:.        for 
-0000eff0: 6361 7264 2069 6e20 7365 636f 6e63 745f  card in seconct_
-0000f000: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-0000f010: 2020 6974 203d 2069 7465 7228 5f67 6574    it = iter(_get
-0000f020: 5f70 6169 7273 2863 6172 6429 290a 2020  _pairs(card)).  
-0000f030: 2020 2020 2020 2020 2020 666f 7220 612c            for a,
-0000f040: 2062 2069 6e20 6974 3a0a 2020 2020 2020   b in it:.      
-0000f050: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0000f060: 6e73 7461 6e63 6528 622c 2073 7472 293a  nstance(b, str):
-0000f070: 2020 2320 6974 206d 7573 7420 6265 2022    # it must be "
-0000f080: 5448 5255 220a 2020 2020 2020 2020 2020  THRU".          
-0000f090: 2020 2020 2020 2020 2020 2320 4254 4120            # BTA 
-0000f0a0: 7361 7973 2049 276d 2061 206a 6572 6b20  says I'm a jerk 
-0000f0b0: 6966 2049 2064 6f6e 2774 2063 6865 636b  if I don't check
-0000f0c0: 2066 6f72 2022 5448 5255 2220 3a29 0a20   for "THRU" :). 
-0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0e0: 2020 2061 322c 2062 3120 3d20 6e65 7874     a2, b1 = next
-0000f0f0: 2869 7429 0a20 2020 2020 2020 2020 2020  (it).           
-0000f100: 2020 2020 2020 2020 2074 6872 752c 2062           thru, b
-0000f110: 3220 3d20 6e65 7874 2869 7429 0a20 2020  2 = next(it).   
-0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f130: 2061 5f69 6473 2e65 7874 656e 6428 5b69   a_ids.extend([i
-0000f140: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0000f150: 612c 2061 3220 2b20 3129 5d29 0a20 2020  a, a2 + 1)]).   
-0000f160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f170: 2062 5f69 6473 2e65 7874 656e 6428 5b69   b_ids.extend([i
-0000f180: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0000f190: 6231 2c20 6232 202b 2031 295d 290a 2020  b1, b2 + 1)]).  
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000f1b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000f1c0: 2020 2020 2020 2020 615f 6964 732e 6170          a_ids.ap
-0000f1d0: 7065 6e64 2861 290a 2020 2020 2020 2020  pend(a).        
-0000f1e0: 2020 2020 2020 2020 2020 2020 625f 6964              b_id
-0000f1f0: 732e 6170 7065 6e64 2862 290a 2020 2020  s.append(b).    
-0000f200: 7265 7475 726e 206e 702e 6172 7261 7928  return np.array(
-0000f210: 615f 6964 732c 2064 7479 7065 3d6e 702e  a_ids, dtype=np.
-0000f220: 696e 7436 3429 2c20 6e70 2e61 7272 6179  int64), np.array
-0000f230: 2862 5f69 6473 2c20 6474 7970 653d 6e70  (b_ids, dtype=np
-0000f240: 2e69 6e74 3634 290a 0a0a 4067 7569 746f  .int64)...@guito
-0000f250: 6f6c 732e 7265 6164 5f74 6578 745f 6669  ols.read_text_fi
-0000f260: 6c65 0a64 6566 2061 736d 3275 7365 7428  le.def asm2uset(
-0000f270: 662c 2074 7279 5f72 6465 7874 726e 3d54  f, try_rdextrn=T
-0000f280: 7275 6529 3a0a 2020 2020 7222 2222 0a20  rue):.    r""". 
-0000f290: 2020 2052 6561 6420 434f 5244 322a 2061     Read CORD2* a
-0000f2a0: 6e64 2047 5249 4420 6361 7264 7320 6672  nd GRID cards fr
-0000f2b0: 6f6d 2061 2022 2e61 736d 2220 6669 6c65  om a ".asm" file
-0000f2c0: 2074 6f20 6d61 6b65 2061 2055 5345 5420   to make a USET 
-0000f2d0: 7461 626c 650a 0a20 2020 2050 6172 616d  table..    Param
-0000f2e0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0000f2f0: 2d2d 2d2d 0a20 2020 2066 203a 2073 7472  ----.    f : str
-0000f300: 696e 6720 6f72 2066 696c 655f 6c69 6b65  ing or file_like
-0000f310: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
-0000f320: 2045 6974 6865 7220 6120 6e61 6d65 206f   Either a name o
-0000f330: 6620 6120 6669 6c65 2c20 6f72 2069 7320  f a file, or is 
-0000f340: 6120 6669 6c65 5f6c 696b 6520 6f62 6a65  a file_like obje
-0000f350: 6374 2061 7320 7265 7475 726e 6564 0a20  ct as returned. 
-0000f360: 2020 2020 2020 2062 7920 3a66 756e 633a         by :func:
-0000f370: 606f 7065 6e60 2e20 4966 2066 696c 655f  `open`. If file_
-0000f380: 6c69 6b65 206f 626a 6563 742c 2069 7420  like object, it 
-0000f390: 6973 2072 6577 6f75 6e64 2066 6972 7374  is rewound first
-0000f3a0: 2e20 4361 6e0a 2020 2020 2020 2020 616c  . Can.        al
-0000f3b0: 736f 2062 6520 7468 6520 6e61 6d65 206f  so be the name o
-0000f3c0: 6620 6120 6469 7265 6374 6f72 7920 6f72  f a directory or
-0000f3d0: 204e 6f6e 653b 2069 6e20 7468 6573 6520   None; in these 
-0000f3e0: 6361 7365 732c 2061 2047 5549 0a20 2020  cases, a GUI.   
-0000f3f0: 2020 2020 2069 7320 6f70 656e 6564 2066       is opened f
-0000f400: 6f72 2066 696c 6520 7365 6c65 6374 696f  or file selectio
-0000f410: 6e2e 0a20 2020 2074 7279 5f72 6465 7874  n..    try_rdext
-0000f420: 726e 203a 2062 6f6f 6c3b 206f 7074 696f  rn : bool; optio
-0000f430: 6e61 6c0a 2020 2020 2020 2020 4966 2054  nal.        If T
-0000f440: 7275 652c 2072 6f75 7469 6e65 2077 696c  rue, routine wil
-0000f450: 6c20 6174 7465 6d70 7420 746f 2072 6561  l attempt to rea
-0000f460: 6420 7468 6520 2245 5854 524e 2220 6361  d the "EXTRN" ca
-0000f470: 7264 2066 726f 6d0a 2020 2020 2020 2020  rd from.        
-0000f480: 7468 6520 222e 7063 6822 2066 696c 652e  the ".pch" file.
-0000f490: 2049 6620 6120 6669 6c65 6e61 6d65 2063   If a filename c
-0000f4a0: 616e 6e6f 7420 6265 2064 6574 6572 6d69  annot be determi
-0000f4b0: 6e65 6420 6672 6f6d 2060 6660 2c0a 2020  ned from `f`,.  
-0000f4c0: 2020 2020 2020 7468 6520 6174 7465 6d70        the attemp
-0000f4d0: 7420 746f 2074 6865 2022 4558 5452 4e22  t to the "EXTRN"
-0000f4e0: 2063 6172 6420 6973 2071 7569 6574 6c79   card is quietly
-0000f4f0: 2073 6b69 7070 6564 2061 6e64 2065 6163   skipped and eac
-0000f500: 680a 2020 2020 2020 2020 622d 7365 7420  h.        b-set 
-0000f510: 6e6f 6465 2069 7320 6173 7375 6d65 6420  node is assumed 
-0000f520: 746f 2068 6176 6520 616c 6c20 3620 444f  to have all 6 DO
-0000f530: 462e 2053 6565 204e 6f74 6573 2062 656c  F. See Notes bel
-0000f540: 6f77 2e0a 0a20 2020 2052 6574 7572 6e73  ow...    Returns
-0000f550: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-0000f560: 2075 7365 7420 3a20 7061 6e64 6173 2044   uset : pandas D
-0000f570: 6174 6146 7261 6d65 0a20 2020 2020 2020  ataFrame.       
-0000f580: 2041 2044 6174 6146 7261 6d65 2061 7320   A DataFrame as 
-0000f590: 6f75 7470 7574 2062 790a 2020 2020 2020  output by.      
-0000f5a0: 2020 3a66 756e 633a 6070 7979 6574 692e    :func:`pyyeti.
-0000f5b0: 6e61 7374 7261 6e2e 6f70 322e 4f50 322e  nastran.op2.OP2.
-0000f5c0: 7264 6e32 636f 7032 602e 2043 6f6e 7461  rdn2cop2`. Conta
-0000f5d0: 696e 7320 616c 6c20 4752 4944 2061 6e64  ins all GRID and
-0000f5e0: 0a20 2020 2020 2020 2053 504f 494e 5420  .        SPOINT 
-0000f5f0: 444f 4620 696e 2074 6865 202e 6173 6d20  DOF in the .asm 
-0000f600: 6669 6c65 2069 6e20 7468 6520 6f72 6465  file in the orde
-0000f610: 7220 7370 6563 6966 6965 6420 6f6e 2074  r specified on t
-0000f620: 6865 0a20 2020 2020 2020 2053 4543 4f4e  he.        SECON
-0000f630: 4354 2063 6172 642e 2054 6869 7320 6973  CT card. This is
-0000f640: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
-0000f650: 2074 6865 206d 6f64 656c 206d 6174 7269   the model matri
-0000f660: 6365 7320 2865 672c 0a20 2020 2020 2020  ces (eg,.       
-0000f670: 2069 6e20 7468 6520 2e6f 7034 2066 696c   in the .op4 fil
-0000f680: 6529 2e0a 2020 2020 636f 6f72 6472 6566  e)..    coordref
-0000f690: 203a 2064 6963 7469 6f6e 6172 790a 2020   : dictionary.  
-0000f6a0: 2020 2020 2020 4469 6374 696f 6e61 7279        Dictionary
-0000f6b0: 2077 6974 6820 7468 6520 6b65 7973 2062   with the keys b
-0000f6c0: 6569 6e67 2074 6865 2063 6f6f 7264 696e  eing the coordin
-0000f6d0: 6174 6520 7379 7374 656d 2069 6420 616e  ate system id an
-0000f6e0: 640a 2020 2020 2020 2020 7468 6520 7661  d.        the va
-0000f6f0: 6c75 6573 2062 6569 6e67 2074 6865 2035  lues being the 5
-0000f700: 7833 206d 6174 7269 783a 3a0a 0a20 2020  x3 matrix::..   
-0000f710: 2020 2020 2020 2020 205b 6964 2020 7479           [id  ty
-0000f720: 7065 2030 5d20 2023 206f 7574 7075 7420  pe 0]  # output 
-0000f730: 636f 6f72 642e 2073 7973 2e20 6964 2061  coord. sys. id a
-0000f740: 6e64 2074 7970 650a 2020 2020 2020 2020  nd type.        
-0000f750: 2020 2020 5b78 6f20 2079 6f20 207a 6f5d      [xo  yo  zo]
-0000f760: 2020 2320 6f72 6967 696e 206f 6620 636f    # origin of co
-0000f770: 6f72 642e 2073 7973 7465 6d0a 2020 2020  ord. system.    
-0000f780: 2020 2020 2020 2020 5b20 2020 2054 2020          [    T  
-0000f790: 2020 205d 2020 2320 3378 3320 7472 616e     ]  # 3x3 tran
-0000f7a0: 7366 6f72 6d61 7469 6f6e 2074 6f20 6261  sformation to ba
-0000f7b0: 7369 630a 2020 2020 2020 2020 2020 2020  sic.            
-0000f7c0: 4e6f 7465 2074 6861 7420 5420 6973 2066  Note that T is f
-0000f7d0: 6f72 2074 6865 2063 6f6f 7264 696e 6174  or the coordinat
-0000f7e0: 6520 7379 7374 656d 2c20 6e6f 7420 6120  e system, not a 
-0000f7f0: 6772 6964 0a20 2020 2020 2020 2020 2020  grid.           
-0000f800: 2028 756e 6c65 7373 2074 7970 6520 3d20   (unless type = 
-0000f810: 3120 7768 6963 6820 6d65 616e 7320 7265  1 which means re
-0000f820: 6374 616e 6775 6c61 7229 0a0a 2020 2020  ctangular)..    
-0000f830: 6273 6574 5f62 6f6f 6c20 3a20 3164 206e  bset_bool : 1d n
-0000f840: 6461 7272 6179 0a20 2020 2020 2020 2041  darray.        A
-0000f850: 2062 6f6f 6c65 616e 2070 6172 7469 7469   boolean partiti
-0000f860: 6f6e 2076 6563 746f 7220 7769 7468 2054  on vector with T
-0000f870: 7275 6520 666f 7220 7468 6520 622d 7365  rue for the b-se
-0000f880: 742e 2054 6869 7320 6973 0a20 2020 2020  t. This is.     
-0000f890: 2020 2063 7265 6174 6564 2066 6f72 2063     created for c
-0000f8a0: 6f6e 7665 6e69 656e 6365 2062 793a 3a0a  onvenience by::.
-0000f8b0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-0000f8c0: 6d20 7079 7965 7469 2069 6d70 6f72 7420  m pyyeti import 
-0000f8d0: 6e61 7374 7261 6e0a 2020 2020 2020 2020  nastran.        
-0000f8e0: 2020 2020 6273 6574 5f62 6f6f 6c20 3d20      bset_bool = 
-0000f8f0: 6e61 7374 7261 6e2e 6d6b 7365 7470 7628  nastran.mksetpv(
-0000f900: 7573 6574 2c20 2761 272c 2027 6227 290a  uset, 'a', 'b').
-0000f910: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
-0000f920: 2d2d 2d2d 0a20 2020 2054 6869 7320 726f  ----.    This ro
-0000f930: 7574 696e 6520 7769 6c6c 2061 7474 656d  utine will attem
-0000f940: 7074 2074 6f20 7265 6164 2074 6865 2022  pt to read the "
-0000f950: 4558 5452 4e22 2063 6172 6420 6672 6f6d  EXTRN" card from
-0000f960: 2074 6865 202e 7063 680a 2020 2020 6669   the .pch.    fi
-0000f970: 6c65 2069 6e20 6361 7365 2073 6f6d 6520  le in case some 
-0000f980: 622d 7365 7420 6e6f 6465 7320 646f 206e  b-set nodes do n
-0000f990: 6f74 2069 6e63 6c75 6465 2061 6c6c 2036  ot include all 6
-0000f9a0: 2044 4f46 2e20 466f 720a 2020 2020 6578   DOF. For.    ex
-0000f9b0: 616d 706c 652c 2061 206d 6f64 656c 2063  ample, a model c
-0000f9c0: 6f75 6c64 2068 6176 6520 3720 622d 7365  ould have 7 b-se
-0000f9d0: 7420 444f 4620 616e 6420 3120 712d 7365  t DOF and 1 q-se
-0000f9e0: 7420 444f 462e 2049 6620 7468 6520 370a  t DOF. If the 7.
-0000f9f0: 2020 2020 622d 7365 7420 444f 4620 6172      b-set DOF ar
-0000fa00: 6520 636f 6d70 6f73 6564 206f 6620 616c  e composed of al
-0000fa10: 6c20 3620 444f 4620 666f 7220 6e6f 6465  l 6 DOF for node
-0000fa20: 2031 3030 2061 6e64 206a 7573 7420 7468   100 and just th
-0000fa30: 650a 2020 2020 7365 636f 6e64 2044 4f46  e.    second DOF
-0000fa40: 2066 6f72 206e 6f64 6520 3230 302c 2074   for node 200, t
-0000fa50: 6865 2045 5854 524e 2063 6172 6420 776f  he EXTRN card wo
-0000fa60: 756c 6420 6c69 6b65 2074 6869 733a 3a0a  uld like this::.
-0000fa70: 0a20 2020 2020 2020 2045 5854 524e 2c31  .        EXTRN,1
-0000fa80: 3030 2c31 3233 3435 362c 3230 302c 322c  00,123456,200,2,
-0000fa90: 3130 3031 2c30 0a0a 2020 2020 4578 616d  1001,0..    Exam
-0000faa0: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-0000fab0: 2d0a 2020 2020 3e3e 3e20 696d 706f 7274  -.    >>> import
-0000fac0: 206e 756d 7079 2061 7320 6e70 0a20 2020   numpy as np.   
-0000fad0: 203e 3e3e 2066 726f 6d20 696f 2069 6d70   >>> from io imp
-0000fae0: 6f72 7420 5374 7269 6e67 494f 0a20 2020  ort StringIO.   
-0000faf0: 203e 3e3e 2066 726f 6d20 7079 7965 7469   >>> from pyyeti
-0000fb00: 2069 6d70 6f72 7420 6e61 7374 7261 6e0a   import nastran.
-0000fb10: 2020 2020 3e3e 3e20 6173 6d5f 6275 6c6b      >>> asm_bulk
-0000fb20: 203d 2028 0a20 2020 202e 2e2e 2020 2020   = (.    ...    
-0000fb30: 2224 2053 4531 3031 2041 5353 454d 424c  "$ SE101 ASSEMBL
-0000fb40: 5920 4649 4c45 5c6e 220a 2020 2020 2e2e  Y FILE\n".    ..
-0000fb50: 2e20 2020 2022 5345 4255 4c4b 2c31 3031  .    "SEBULK,101
-0000fb60: 2c45 5854 4f50 342c 2c4d 414e 5541 4c2c  ,EXTOP4,,MANUAL,
-0000fb70: 2c2c 3130 315c 6e22 0a20 2020 202e 2e2e  ,,101\n".    ...
-0000fb80: 2020 2020 2253 4543 4f4e 4354 2c31 3031      "SECONCT,101
-0000fb90: 2c30 2c2c 4e4f 5c6e 220a 2020 2020 2e2e  ,0,,NO\n".    ..
-0000fba0: 2e20 2020 2022 2c33 2c33 2c31 3130 2c31  .    ",3,3,110,1
-0000fbb0: 3130 2c31 392c 3139 2c32 372c 3237 5c6e  10,19,19,27,27\n
-0000fbc0: 220a 2020 2020 2e2e 2e20 2020 2022 2420  ".    ...    "$ 
-0000fbd0: 436f 6f72 6469 6e61 7465 2031 303a 5c6e  Coordinate 10:\n
-0000fbe0: 220a 2020 2020 2e2e 2e20 2020 2022 434f  ".    ...    "CO
-0000fbf0: 5244 3252 2c31 302c 302c 302e 302c 302e  RD2R,10,0,0.0,0.
-0000fc00: 302c 302e 302c 312e 302c 302e 302c 302e  0,0.0,1.0,0.0,0.
-0000fc10: 305c 6e22 0a20 2020 202e 2e2e 2020 2020  0\n".    ...    
-0000fc20: 222c 302e 302c 312e 302c 302e 305c 6e22  ",0.0,1.0,0.0\n"
-0000fc30: 0a20 2020 202e 2e2e 2020 2020 2247 5249  .    ...    "GRI
-0000fc40: 442c 332c 302c 3630 302e 2c30 2e2c 3330  D,3,0,600.,0.,30
-0000fc50: 302e 2c30 5c6e 220a 2020 2020 2e2e 2e20  0.,0\n".    ... 
-0000fc60: 2020 2022 4752 4944 2c31 392c 302c 3630     "GRID,19,0,60
-0000fc70: 302e 2c33 3030 2e2c 302e 2c30 5c6e 220a  0.,300.,0.,0\n".
-0000fc80: 2020 2020 2e2e 2e20 2020 2022 4752 4944      ...    "GRID
-0000fc90: 2c32 372c 302c 3630 302e 2c30 2e2c 302e  ,27,0,600.,0.,0.
-0000fca0: 5c6e 220a 2020 2020 2e2e 2e20 2020 2022  \n".    ...    "
-0000fcb0: 5350 4f49 4e54 2c31 3130 5c6e 220a 2020  SPOINT,110\n".  
-0000fcc0: 2020 2e2e 2e20 290a 2020 2020 3e3e 3e20    ... ).    >>> 
-0000fcd0: 7769 7468 2053 7472 696e 6749 4f28 6173  with StringIO(as
-0000fce0: 6d5f 6275 6c6b 2920 6173 2066 3a0a 2020  m_bulk) as f:.  
-0000fcf0: 2020 2e2e 2e20 2020 2020 752c 2063 2c20    ...     u, c, 
-0000fd00: 6220 3d20 6e61 7374 7261 6e2e 6173 6d32  b = nastran.asm2
-0000fd10: 7573 6574 2866 290a 2020 2020 3e3e 3e20  uset(f).    >>> 
-0000fd20: 7520 2020 2020 2020 2020 2020 2023 2064  u            # d
-0000fd30: 6f63 7465 7374 3a20 2b45 4c4c 4950 5349  octest: +ELLIPSI
-0000fd40: 530a 2020 2020 2020 2020 2020 2020 2020  S.              
-0000fd50: 6e61 7373 6574 2020 2020 2020 7820 2020  nasset      x   
-0000fd60: 2020 2079 2020 2020 2020 7a0a 2020 2020     y      z.    
-0000fd70: 6964 2020 646f 662e 2e2e 0a20 2020 2033  id  dof....    3
-0000fd80: 2020 2031 2020 2020 3230 3937 3135 3420     1    2097154 
-0000fd90: 2036 3030 2e30 2020 2020 302e 3020 2033   600.0    0.0  3
-0000fda0: 3030 2e30 0a20 2020 2020 2020 2032 2020  00.0.        2  
-0000fdb0: 2020 3230 3937 3135 3420 2020 2030 2e30    2097154    0.0
-0000fdc0: 2020 2020 312e 3020 2020 2030 2e30 0a20      1.0    0.0. 
-0000fdd0: 2020 2020 2020 2033 2020 2020 3230 3937         3    2097
-0000fde0: 3135 3420 2020 2030 2e30 2020 2020 302e  154    0.0    0.
-0000fdf0: 3020 2020 2030 2e30 0a20 2020 2020 2020  0    0.0.       
-0000fe00: 2034 2020 2020 3230 3937 3135 3420 2020   4    2097154   
-0000fe10: 2031 2e30 2020 2020 302e 3020 2020 2030   1.0    0.0    0
-0000fe20: 2e30 0a20 2020 2020 2020 2035 2020 2020  .0.        5    
-0000fe30: 3230 3937 3135 3420 2020 2030 2e30 2020  2097154    0.0  
-0000fe40: 2020 312e 3020 2020 2030 2e30 0a20 2020    1.0    0.0.   
-0000fe50: 2020 2020 2036 2020 2020 3230 3937 3135       6    209715
-0000fe60: 3420 2020 2030 2e30 2020 2020 302e 3020  4    0.0    0.0 
-0000fe70: 2020 2031 2e30 0a20 2020 2031 3130 2030     1.0.    110 0
-0000fe80: 2020 2020 3431 3934 3330 3420 2020 2030      4194304    0
-0000fe90: 2e30 2020 2020 302e 3020 2020 2030 2e30  .0    0.0    0.0
-0000fea0: 0a20 2020 2031 3920 2031 2020 2020 3230  .    19  1    20
-0000feb0: 3937 3135 3420 2036 3030 2e30 2020 3330  97154  600.0  30
-0000fec0: 302e 3020 2020 2030 2e30 0a20 2020 2020  0.0    0.0.     
-0000fed0: 2020 2032 2020 2020 3230 3937 3135 3420     2    2097154 
-0000fee0: 2020 2030 2e30 2020 2020 312e 3020 2020     0.0    1.0   
-0000fef0: 2030 2e30 0a20 2020 2020 2020 2033 2020   0.0.        3  
-0000ff00: 2020 3230 3937 3135 3420 2020 2030 2e30    2097154    0.0
-0000ff10: 2020 2020 302e 3020 2020 2030 2e30 0a20      0.0    0.0. 
-0000ff20: 2020 2020 2020 2034 2020 2020 3230 3937         4    2097
-0000ff30: 3135 3420 2020 2031 2e30 2020 2020 302e  154    1.0    0.
-0000ff40: 3020 2020 2030 2e30 0a20 2020 2020 2020  0    0.0.       
-0000ff50: 2035 2020 2020 3230 3937 3135 3420 2020   5    2097154   
-0000ff60: 2030 2e30 2020 2020 312e 3020 2020 2030   0.0    1.0    0
-0000ff70: 2e30 0a20 2020 2020 2020 2036 2020 2020  .0.        6    
-0000ff80: 3230 3937 3135 3420 2020 2030 2e30 2020  2097154    0.0  
-0000ff90: 2020 302e 3020 2020 2031 2e30 0a20 2020    0.0    1.0.   
-0000ffa0: 2032 3720 2031 2020 2020 3230 3937 3135   27  1    209715
-0000ffb0: 3420 2036 3030 2e30 2020 2020 302e 3020  4  600.0    0.0 
-0000ffc0: 2020 2030 2e30 0a20 2020 2020 2020 2032     0.0.        2
-0000ffd0: 2020 2020 3230 3937 3135 3420 2020 2030      2097154    0
-0000ffe0: 2e30 2020 2020 312e 3020 2020 2030 2e30  .0    1.0    0.0
-0000fff0: 0a20 2020 2020 2020 2033 2020 2020 3230  .        3    20
-00010000: 3937 3135 3420 2020 2030 2e30 2020 2020  97154    0.0    
-00010010: 302e 3020 2020 2030 2e30 0a20 2020 2020  0.0    0.0.     
-00010020: 2020 2034 2020 2020 3230 3937 3135 3420     4    2097154 
-00010030: 2020 2031 2e30 2020 2020 302e 3020 2020     1.0    0.0   
-00010040: 2030 2e30 0a20 2020 2020 2020 2035 2020   0.0.        5  
-00010050: 2020 3230 3937 3135 3420 2020 2030 2e30    2097154    0.0
-00010060: 2020 2020 312e 3020 2020 2030 2e30 0a20      1.0    0.0. 
-00010070: 2020 2020 2020 2036 2020 2020 3230 3937         6    2097
-00010080: 3135 3420 2020 2030 2e30 2020 2020 302e  154    0.0    0.
-00010090: 3020 2020 2031 2e30 0a20 2020 203e 3e3e  0    1.0.    >>>
-000100a0: 2063 2020 2020 2020 2020 2020 2020 2320   c            # 
-000100b0: 646f 6374 6573 743a 202b 534b 4950 0a20  doctest: +SKIP. 
-000100c0: 2020 207b 303a 2061 7272 6179 285b 5b20     {0: array([[ 
-000100d0: 302e 2c20 2031 2e2c 2020 302e 5d2c 0a20  0.,  1.,  0.],. 
-000100e0: 2020 2020 2020 2020 2020 205b 2030 2e2c             [ 0.,
-000100f0: 2020 302e 2c20 2030 2e5d 2c0a 2020 2020    0.,  0.],.    
-00010100: 2020 2020 2020 2020 5b20 312e 2c20 2030          [ 1.,  0
-00010110: 2e2c 2020 302e 5d2c 0a20 2020 2020 2020  .,  0.],.       
-00010120: 2020 2020 205b 2030 2e2c 2020 312e 2c20       [ 0.,  1., 
-00010130: 2030 2e5d 2c0a 2020 2020 2020 2020 2020   0.],.          
-00010140: 2020 5b20 302e 2c20 2030 2e2c 2020 312e    [ 0.,  0.,  1.
-00010150: 5d5d 292c 0a20 2020 2020 3130 3a20 6172  ]]),.     10: ar
-00010160: 7261 7928 5b5b 2031 302e 2c20 2020 312e  ray([[ 10.,   1.
-00010170: 2c20 2020 302e 5d2c 0a20 2020 2020 2020  ,   0.],.       
-00010180: 2020 2020 205b 2020 302e 2c20 2020 302e       [  0.,   0.
-00010190: 2c20 2020 302e 5d2c 0a20 2020 2020 2020  ,   0.],.       
-000101a0: 2020 2020 205b 2020 302e 2c20 2020 302e       [  0.,   0.
-000101b0: 2c20 2020 312e 5d2c 0a20 2020 2020 2020  ,   1.],.       
-000101c0: 2020 2020 205b 2020 312e 2c20 2020 302e       [  1.,   0.
-000101d0: 2c20 2020 302e 5d2c 0a20 2020 2020 2020  ,   0.],.       
-000101e0: 2020 2020 205b 2020 302e 2c20 2020 312e       [  0.,   1.
-000101f0: 2c20 2020 302e 5d5d 297d 0a20 2020 203e  ,   0.]])}.    >
-00010200: 3e3e 206e 702e 7365 745f 7072 696e 746f  >> np.set_printo
-00010210: 7074 696f 6e73 286c 696e 6577 6964 7468  ptions(linewidth
-00010220: 3d35 3529 0a20 2020 203e 3e3e 2062 0a20  =55).    >>> b. 
-00010230: 2020 2061 7272 6179 285b 2054 7275 652c     array([ True,
-00010240: 2020 5472 7565 2c20 2054 7275 652c 2020    True,  True,  
-00010250: 5472 7565 2c20 2054 7275 652c 2020 5472  True,  True,  Tr
-00010260: 7565 2c20 4661 6c73 652c 0a20 2020 2020  ue, False,.     
-00010270: 2020 2020 2020 2054 7275 652c 2020 5472         True,  Tr
-00010280: 7565 2c20 2054 7275 652c 2020 5472 7565  ue,  True,  True
-00010290: 2c20 2054 7275 652c 2020 5472 7565 2c20  ,  True,  True, 
-000102a0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000102b0: 2020 2054 7275 652c 2020 5472 7565 2c20     True,  True, 
-000102c0: 2054 7275 652c 2020 5472 7565 2c20 2054   True,  True,  T
-000102d0: 7275 655d 2c20 6474 7970 653d 626f 6f6c  rue], dtype=bool
-000102e0: 290a 2020 2020 2222 220a 2020 2020 7573  ).    """.    us
-000102f0: 6574 2c20 636f 6f72 6473 203d 2062 756c  et, coords = bul
-00010300: 6b32 7573 6574 2866 290a 0a20 2020 2023  k2uset(f)..    #
-00010310: 2061 6464 2073 706f 696e 7473 2074 6f20   add spoints to 
-00010320: 7573 6574 2074 6162 6c65 3a0a 2020 2020  uset table:.    
-00010330: 7370 6f69 6e74 7320 3d20 7264 7370 6f69  spoints = rdspoi
-00010340: 6e74 7328 6629 0a20 2020 2069 6620 7370  nts(f).    if sp
-00010350: 6f69 6e74 7320 6973 206e 6f74 204e 6f6e  oints is not Non
-00010360: 653a 0a20 2020 2020 2020 206e 203d 206c  e:.        n = l
-00010370: 656e 2873 706f 696e 7473 290a 2020 2020  en(spoints).    
-00010380: 2020 2020 646f 6620 3d20 6e70 2e7a 6572      dof = np.zer
-00010390: 6f73 2828 6e2c 2032 292c 206e 702e 696e  os((n, 2), np.in
-000103a0: 7436 3429 0a20 2020 2020 2020 2064 6f66  t64).        dof
-000103b0: 5b3a 2c20 305d 203d 2073 706f 696e 7473  [:, 0] = spoints
-000103c0: 0a20 2020 2020 2020 2075 7365 745f 7370  .        uset_sp
-000103d0: 6f69 6e74 7320 3d20 6e32 702e 6d61 6b65  oints = n2p.make
-000103e0: 5f75 7365 7428 646f 662c 206e 3270 2e6d  _uset(dof, n2p.m
-000103f0: 6b75 7365 746d 6173 6b28 2271 2229 2c20  kusetmask("q"), 
-00010400: 6e70 2e7a 6572 6f73 2828 6e2c 2033 2929  np.zeros((n, 3))
-00010410: 290a 2020 2020 2020 2020 7573 6574 203d  ).        uset =
-00010420: 2070 642e 636f 6e63 6174 285b 7573 6574   pd.concat([uset
-00010430: 2c20 7573 6574 5f73 706f 696e 7473 5d2c  , uset_spoints],
-00010440: 2061 7869 733d 3029 0a0a 2020 2020 6966   axis=0)..    if
-00010450: 2074 7279 5f72 6465 7874 726e 3a0a 2020   try_rdextrn:.  
-00010460: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00010470: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
-00010480: 3d20 662e 6e61 6d65 0a20 2020 2020 2020  = f.name.       
-00010490: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
-000104a0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-000104b0: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
-000104c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000104d0: 2020 2064 6f66 203d 2072 6465 7874 726e     dof = rdextrn
-000104e0: 2866 696c 656e 616d 652e 7265 706c 6163  (filename.replac
-000104f0: 6528 222e 6173 6d22 2c20 222e 7063 6822  e(".asm", ".pch"
-00010500: 2929 0a20 2020 2020 2020 2020 2020 2075  )).            u
-00010510: 7365 745f 6f72 6465 7265 6420 3d20 7573  set_ordered = us
-00010520: 6574 2e6c 6f63 5b6c 6973 7428 646f 6629  et.loc[list(dof)
-00010530: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
-00010540: 7475 726e 2075 7365 745f 6f72 6465 7265  turn uset_ordere
-00010550: 642c 2063 6f6f 7264 732c 206e 3270 2e6d  d, coords, n2p.m
-00010560: 6b73 6574 7076 2875 7365 745f 6f72 6465  ksetpv(uset_orde
-00010570: 7265 642c 2022 6122 2c20 2262 2229 0a0a  red, "a", "b")..
-00010580: 2020 2020 615f 6964 7320 3d20 7264 7365      a_ids = rdse
-00010590: 636f 6e63 7428 6629 5b30 5d0a 2020 2020  conct(f)[0].    
-000105a0: 7573 6574 5f6f 7264 6572 6564 203d 2075  uset_ordered = u
-000105b0: 7365 742e 6c6f 635b 615f 6964 735d 0a20  set.loc[a_ids]. 
-000105c0: 2020 2069 6620 7573 6574 5f6f 7264 6572     if uset_order
-000105d0: 6564 2e73 6861 7065 5b30 5d20 213d 2075  ed.shape[0] != u
-000105e0: 7365 742e 7368 6170 655b 305d 3a0a 2020  set.shape[0]:.  
-000105f0: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-00010600: 696d 6545 7272 6f72 280a 2020 2020 2020  imeError(.      
-00010610: 2020 2020 2020 224e 756d 6265 7220 6f66        "Number of
-00010620: 2053 4543 4f4e 4354 2073 7570 6572 656c   SECONCT superel
-00010630: 656d 656e 7420 2741 2720 444f 4620 646f  ement 'A' DOF do
-00010640: 206e 6f74 206d 6174 6368 2047 5249 4420   not match GRID 
-00010650: 616e 6422 0a20 2020 2020 2020 2020 2020  and".           
-00010660: 2022 2053 504f 494e 5420 6361 7264 7320   " SPOINT cards 
-00010670: 696e 2066 696c 653a 5c6e 220a 2020 2020  in file:\n".    
-00010680: 2020 2020 2020 2020 6622 2020 2020 2320          f"    # 
-00010690: 444f 4620 6f6e 2053 4543 4f4e 4354 203d  DOF on SECONCT =
-000106a0: 207b 7573 6574 5f6f 7264 6572 6564 2e73   {uset_ordered.s
-000106b0: 6861 7065 5b30 5d7d 5c6e 220a 2020 2020  hape[0]}\n".    
-000106c0: 2020 2020 2020 2020 6622 2020 2020 2320          f"    # 
-000106d0: 444f 4620 6f6e 2047 5249 4453 2f53 504f  DOF on GRIDS/SPO
-000106e0: 494e 5453 203d 207b 7573 6574 2e73 6861  INTS = {uset.sha
-000106f0: 7065 5b30 5d7d 220a 2020 2020 2020 2020  pe[0]}".        
-00010700: 290a 0a20 2020 2072 6574 7572 6e20 7573  )..    return us
-00010710: 6574 5f6f 7264 6572 6564 2c20 636f 6f72  et_ordered, coor
-00010720: 6473 2c20 6e32 702e 6d6b 7365 7470 7628  ds, n2p.mksetpv(
-00010730: 7573 6574 5f6f 7264 6572 6564 2c20 2261  uset_ordered, "a
-00010740: 222c 2022 6222 290a 0a0a 6465 6620 7264  ", "b")...def rd
-00010750: 7774 6275 6c6b 2866 696e 2c20 666f 7574  wtbulk(fin, fout
-00010760: 293a 0a20 2020 2022 2222 0a20 2020 2047  ):.    """.    G
-00010770: 6574 2062 756c 6b20 6461 7461 2066 726f  et bulk data fro
-00010780: 6d20 6120 736f 7274 6564 204e 6173 7472  m a sorted Nastr
-00010790: 616e 206f 7574 7075 7420 6669 6c65 2e0a  an output file..
-000107a0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-000107b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000107c0: 2020 2066 696e 203a 2073 7472 696e 6720     fin : string 
-000107d0: 6f72 2066 696c 655f 6c69 6b65 206f 7220  or file_like or 
-000107e0: 4e6f 6e65 0a20 2020 2020 2020 2045 6974  None.        Eit
-000107f0: 6865 7220 6120 6e61 6d65 206f 6620 6120  her a name of a 
-00010800: 6669 6c65 2c20 6f72 2069 7320 6120 6669  file, or is a fi
-00010810: 6c65 5f6c 696b 6520 6f62 6a65 6374 2061  le_like object a
-00010820: 7320 7265 7475 726e 6564 0a20 2020 2020  s returned.     
-00010830: 2020 2062 7920 3a66 756e 633a 606f 7065     by :func:`ope
-00010840: 6e60 2e20 4966 2066 696c 655f 6c69 6b65  n`. If file_like
-00010850: 206f 626a 6563 742c 2069 7420 6973 2072   object, it is r
-00010860: 6577 6f75 6e64 2066 6972 7374 2e20 4361  ewound first. Ca
-00010870: 6e0a 2020 2020 2020 2020 616c 736f 2062  n.        also b
-00010880: 6520 7468 6520 6e61 6d65 206f 6620 6120  e the name of a 
-00010890: 6469 7265 6374 6f72 7920 6f72 204e 6f6e  directory or Non
-000108a0: 653b 2069 6e20 7468 6573 6520 6361 7365  e; in these case
-000108b0: 732c 2061 2047 5549 0a20 2020 2020 2020  s, a GUI.       
-000108c0: 2069 7320 6f70 656e 6564 2066 6f72 2066   is opened for f
-000108d0: 696c 6520 7365 6c65 6374 696f 6e2e 0a20  ile selection.. 
-000108e0: 2020 2066 6f75 7420 3a20 7374 7269 6e67     fout : string
-000108f0: 206f 7220 6669 6c65 5f6c 696b 6520 6f72   or file_like or
-00010900: 2031 206f 7220 4e6f 6e65 0a20 2020 2020   1 or None.     
-00010910: 2020 2045 6974 6865 7220 6120 6e61 6d65     Either a name
-00010920: 206f 6620 6120 6669 6c65 2c20 6f72 2069   of a file, or i
-00010930: 7320 6120 6669 6c65 5f6c 696b 6520 6f62  s a file_like ob
-00010940: 6a65 6374 2061 7320 7265 7475 726e 6564  ject as returned
-00010950: 0a20 2020 2020 2020 2062 7920 3a66 756e  .        by :fun
-00010960: 633a 606f 7065 6e60 206f 7220 3a63 6c61  c:`open` or :cla
-00010970: 7373 3a60 696f 2e53 7472 696e 6749 4f60  ss:`io.StringIO`
-00010980: 2e20 496e 7075 7420 6173 2069 6e74 6567  . Input as integ
-00010990: 6572 2031 2074 6f0a 2020 2020 2020 2020  er 1 to.        
-000109a0: 7772 6974 6520 746f 2073 7464 6f75 742e  write to stdout.
-000109b0: 2043 616e 2061 6c73 6f20 6265 2074 6865   Can also be the
-000109c0: 206e 616d 6520 6f66 2061 2064 6972 6563   name of a direc
-000109d0: 746f 7279 206f 7220 4e6f 6e65 3b0a 2020  tory or None;.  
-000109e0: 2020 2020 2020 696e 2074 6865 7365 2063        in these c
-000109f0: 6173 6573 2c20 6120 4755 4920 6973 206f  ases, a GUI is o
-00010a00: 7065 6e65 6420 666f 7220 6669 6c65 2073  pened for file s
-00010a10: 656c 6563 7469 6f6e 2e0a 0a20 2020 2052  election...    R
-00010a20: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00010a30: 2d2d 0a20 2020 204e 6f6e 650a 0a20 2020  --.    None..   
-00010a40: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-00010a50: 0a20 2020 2052 6561 6473 2074 6865 2062  .    Reads the b
-00010a60: 756c 6b20 6461 7461 2066 726f 6d20 696e  ulk data from in
-00010a70: 7075 7420 6669 6c65 2061 6e64 2077 7269  put file and wri
-00010a80: 7465 7320 6974 2074 6f20 7468 6520 6f75  tes it to the ou
-00010a90: 7470 7574 0a20 2020 2066 696c 652e 2041  tput.    file. A
-00010aa0: 6c6c 2063 6f6e 7469 6e75 6174 696f 6e20  ll continuation 
-00010ab0: 636f 6465 7320 6172 6520 7374 7269 7070  codes are stripp
-00010ac0: 6564 206f 6666 2e0a 0a20 2020 2048 6173  ed off...    Has
-00010ad0: 206e 6f74 2062 6565 6e20 7465 7374 6564   not been tested
-00010ae0: 206f 6e20 756e 736f 7274 6564 2062 756c   on unsorted bul
-00010af0: 6b2e 0a0a 2020 2020 4578 616d 706c 6520  k...    Example 
-00010b00: 7573 6167 653a 3a0a 0a20 2020 2020 2020  usage::..       
-00010b10: 2066 726f 6d20 7079 7965 7469 2069 6d70   from pyyeti imp
-00010b20: 6f72 7420 6e61 7374 7261 6e0a 2020 2020  ort nastran.    
-00010b30: 2020 2020 6e61 7374 7261 6e2e 7264 7774      nastran.rdwt
-00010b40: 6275 6c6b 2827 6d65 636f 312e 6f75 7427  bulk('meco1.out'
-00010b50: 2c20 276d 6563 6f31 2e62 6c6b 2729 0a20  , 'meco1.blk'). 
-00010b60: 2020 2022 2222 0a0a 2020 2020 4067 7569     """..    @gui
-00010b70: 746f 6f6c 732e 7265 6164 5f74 6578 745f  tools.read_text_
-00010b80: 6669 6c65 0a20 2020 2064 6566 205f 7264  file.    def _rd
-00010b90: 6275 6c6b 2866 293a 0a20 2020 2020 2020  bulk(f):.       
-00010ba0: 2066 7365 6172 6368 2866 2c20 2243 4f55   fsearch(f, "COU
-00010bb0: 4e54 2020 2020 2020 2020 2e20 2020 3120  NT        .   1 
-00010bc0: 202e 2e20 2020 3220 202e 2e20 2020 3322   ..   2  ..   3"
-00010bd0: 290a 2020 2020 2020 2020 7320 3d20 5b5d  ).        s = []
-00010be0: 0a20 2020 2020 2020 2070 726f 6720 3d20  .        prog = 
-00010bf0: 7265 2e63 6f6d 7069 6c65 2872 225b 205d  re.compile(r"[ ]
-00010c00: 7b31 337d 5b20 302d 395d 7b38 7d2d 5b20  {13}[ 0-9]{8}-[ 
-00010c10: 5d7b 387d 282e 7b37 327d 2922 290a 2020  ]{8}(.{72})").  
-00010c20: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
-00010c30: 6e20 663a 0a20 2020 2020 2020 2020 2020  n f:.           
-00010c40: 2069 6620 6c69 6e65 2e73 7461 7274 7377   if line.startsw
-00010c50: 6974 6828 2220 2020 2020 2020 2020 2020  ith("           
-00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c70: 2020 2045 4e44 4441 5441 2229 3a0a 2020     ENDDATA"):.  
-00010c80: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00010c90: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00010ca0: 6d20 3d20 7072 6f67 2e6d 6174 6368 286c  m = prog.match(l
-00010cb0: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
-00010cc0: 2069 6620 6d3a 0a20 2020 2020 2020 2020   if m:.         
-00010cd0: 2020 2020 2020 206d 6174 6368 203d 206d         match = m
-00010ce0: 2e67 726f 7570 2831 292e 7374 7269 7028  .group(1).strip(
-00010cf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010d00: 2020 6966 206d 6174 6368 5b30 5d20 3d3d    if match[0] ==
-00010d10: 2022 2b22 206f 7220 6d61 7463 685b 305d   "+" or match[0]
-00010d20: 203d 3d20 222a 223a 0a20 2020 2020 2020   == "*":.       
-00010d30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010d40: 6c65 6e28 6d61 7463 6829 203e 2038 3a0a  len(match) > 8:.
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
-00010d70: 6d61 7463 685b 305d 202b 2022 2020 2020  match[0] + "    
-00010d80: 2020 2022 202b 206d 6174 6368 5b38 3a5d     " + match[8:]
-00010d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010da0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000ae70: 3d20 3132 3a0a 2020 2020 2020 2020 6966  = 12:.        if
+0000ae80: 206c 656e 2863 6172 6429 203d 3d20 3133   len(card) == 13
+0000ae90: 2061 6e64 2063 6172 645b 3132 5d20 3d3d   and card[12] ==
+0000aea0: 2030 2061 6e64 2069 7369 6e73 7461 6e63   0 and isinstanc
+0000aeb0: 6528 6361 7264 5b31 325d 2c20 696e 7429  e(card[12], int)
+0000aec0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
+0000aed0: 7264 203d 2063 6172 645b 3a31 325d 0a20  rd = card[:12]. 
+0000aee0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000aef0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000af00: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+0000af10: 2020 2020 2020 2020 2020 2066 2265 7870             f"exp
+0000af20: 6563 7465 6420 3132 2066 6965 6c64 7320  ected 12 fields 
+0000af30: 6275 7420 676f 7420 7b6c 656e 2863 6172  but got {len(car
+0000af40: 6429 7d2c 2063 6865 636b 3a20 7b63 6172  d)}, check: {car
+0000af50: 645b 305d 7d2c 207b 6361 7264 5b31 5d7d  d[0]}, {card[1]}
+0000af60: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0000af70: 2020 2020 6368 6172 203d 2063 6172 645b      char = card[
+0000af80: 305d 5b35 5d0a 2020 2020 6966 2063 6861  0][5].    if cha
+0000af90: 7220 696e 2022 7252 223a 0a20 2020 2020  r in "rR":.     
+0000afa0: 2020 2063 7479 7065 203d 2031 0a20 2020     ctype = 1.   
+0000afb0: 2065 6c69 6620 6368 6172 2069 6e20 2263   elif char in "c
+0000afc0: 4322 3a0a 2020 2020 2020 2020 6374 7970  C":.        ctyp
+0000afd0: 6520 3d20 320a 2020 2020 656c 7365 3a0a  e = 2.    else:.
+0000afe0: 2020 2020 2020 2020 6374 7970 6520 3d20          ctype = 
+0000aff0: 330a 0a20 2020 2023 2066 6f72 2065 7272  3..    # for err
+0000b000: 6f72 206d 6573 7361 6765 2c20 696e 2063  or message, in c
+0000b010: 6173 6520 6974 2773 206e 6565 6465 643a  ase it's needed:
+0000b020: 0a20 2020 206e 616d 652c 2069 6465 6e74  .    name, ident
+0000b030: 203d 2063 6172 645b 305d 2c20 6361 7264   = card[0], card
+0000b040: 5b31 5d0a 0a20 2020 2063 6172 645b 305d  [1]..    card[0]
+0000b050: 2c20 6361 7264 5b31 5d20 3d20 6361 7264  , card[1] = card
+0000b060: 5b31 5d2c 2063 7479 7065 0a20 2020 2074  [1], ctype.    t
+0000b070: 7279 3a0a 2020 2020 2020 2020 6361 7264  ry:.        card
+0000b080: 203d 206e 702e 6172 7261 7928 6361 7264   = np.array(card
+0000b090: 292e 6173 7479 7065 2866 6c6f 6174 290a  ).astype(float).
+0000b0a0: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+0000b0b0: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+0000b0c0: 2020 2020 6d73 6720 3d20 6622 7b65 2e61      msg = f"{e.a
+0000b0d0: 7267 735b 305d 7d2c 2063 6865 636b 3a20  rgs[0]}, check: 
+0000b0e0: 7b6e 616d 657d 2c20 7b69 6465 6e74 7d22  {name}, {ident}"
+0000b0f0: 0a20 2020 2020 2020 2065 2e61 7267 7320  .        e.args 
+0000b100: 3d20 286d 7367 2c29 0a20 2020 2020 2020  = (msg,).       
+0000b110: 2072 6169 7365 0a0a 2020 2020 7265 7475   raise..    retu
+0000b120: 726e 2063 6172 640a 0a0a 6465 6620 7264  rn card...def rd
+0000b130: 636f 7264 3263 6172 6473 2866 293a 0a20  cord2cards(f):. 
+0000b140: 2020 2022 2222 0a20 2020 2052 6561 6420     """.    Read 
+0000b150: 434f 5244 322a 2063 6172 6473 2066 726f  CORD2* cards fro
+0000b160: 6d20 6120 4e61 7374 7261 6e20 6275 6c6b  m a Nastran bulk
+0000b170: 2066 696c 650a 0a20 2020 2050 6172 616d   file..    Param
+0000b180: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0000b190: 2d2d 2d2d 0a20 2020 2066 203a 2073 7472  ----.    f : str
+0000b1a0: 696e 6720 6f72 2066 696c 655f 6c69 6b65  ing or file_like
+0000b1b0: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+0000b1c0: 2045 6974 6865 7220 6120 6e61 6d65 206f   Either a name o
+0000b1d0: 6620 6120 6669 6c65 2c20 6f72 2069 7320  f a file, or is 
+0000b1e0: 6120 6669 6c65 5f6c 696b 6520 6f62 6a65  a file_like obje
+0000b1f0: 6374 2061 7320 7265 7475 726e 6564 0a20  ct as returned. 
+0000b200: 2020 2020 2020 2062 7920 3a66 756e 633a         by :func:
+0000b210: 606f 7065 6e60 2e20 4966 2066 696c 655f  `open`. If file_
+0000b220: 6c69 6b65 206f 626a 6563 742c 2069 7420  like object, it 
+0000b230: 6973 2072 6577 6f75 6e64 2066 6972 7374  is rewound first
+0000b240: 2e20 4361 6e0a 2020 2020 2020 2020 616c  . Can.        al
+0000b250: 736f 2062 6520 7468 6520 6e61 6d65 206f  so be the name o
+0000b260: 6620 6120 6469 7265 6374 6f72 7920 6f72  f a directory or
+0000b270: 204e 6f6e 653b 2069 6e20 7468 6573 6520   None; in these 
+0000b280: 6361 7365 732c 2061 2047 5549 0a20 2020  cases, a GUI.   
+0000b290: 2020 2020 2069 7320 6f70 656e 6564 2066       is opened f
+0000b2a0: 6f72 2066 696c 6520 7365 6c65 6374 696f  or file selectio
+0000b2b0: 6e2e 0a0a 2020 2020 5265 7475 726e 730a  n...    Returns.
+0000b2c0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0000b2d0: 6469 6374 696f 6e61 7279 0a20 2020 2020  dictionary.     
+0000b2e0: 2020 2044 6963 7469 6f6e 6172 7920 7769     Dictionary wi
+0000b2f0: 7468 2074 6865 206b 6579 7320 6265 696e  th the keys bein
+0000b300: 6720 7468 6520 636f 6f72 6469 6e61 7465  g the coordinate
+0000b310: 2073 7973 7465 6d20 6964 2061 6e64 0a20   system id and. 
+0000b320: 2020 2020 2020 2074 6865 2076 616c 7565         the value
+0000b330: 7320 6265 696e 6720 7468 6520 3578 3320  s being the 5x3 
+0000b340: 6d61 7472 6978 3a3a 0a0a 2020 2020 2020  matrix::..      
+0000b350: 2020 2020 2020 5b69 6420 2074 7970 6520        [id  type 
+0000b360: 305d 2020 2320 6f75 7470 7574 2063 6f6f  0]  # output coo
+0000b370: 7264 2e20 7379 732e 2069 6420 616e 6420  rd. sys. id and 
+0000b380: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
+0000b390: 205b 786f 2020 796f 2020 7a6f 5d20 2023   [xo  yo  zo]  #
+0000b3a0: 206f 7269 6769 6e20 6f66 2063 6f6f 7264   origin of coord
+0000b3b0: 2e20 7379 7374 656d 0a20 2020 2020 2020  . system.       
+0000b3c0: 2020 2020 205b 2020 2020 5420 2020 2020       [    T     
+0000b3d0: 5d20 2023 2033 7833 2074 7261 6e73 666f  ]  # 3x3 transfo
+0000b3e0: 726d 6174 696f 6e20 746f 2062 6173 6963  rmation to basic
+0000b3f0: 0a20 2020 2020 2020 2020 2020 204e 6f74  .            Not
+0000b400: 6520 7468 6174 2054 2069 7320 666f 7220  e that T is for 
+0000b410: 7468 6520 636f 6f72 6469 6e61 7465 2073  the coordinate s
+0000b420: 7973 7465 6d2c 206e 6f74 2061 2067 7269  ystem, not a gri
+0000b430: 640a 2020 2020 2020 2020 2020 2020 2875  d.            (u
+0000b440: 6e6c 6573 7320 7479 7065 203d 2031 2077  nless type = 1 w
+0000b450: 6869 6368 206d 6561 6e73 2072 6563 7461  hich means recta
+0000b460: 6e67 756c 6172 290a 0a20 2020 204e 6f74  ngular)..    Not
+0000b470: 6573 0a20 2020 202d 2d2d 2d2d 0a20 2020  es.    -----.   
+0000b480: 2054 6869 7320 726f 7574 696e 6520 7573   This routine us
+0000b490: 6573 203a 6675 6e63 3a60 7079 7965 7469  es :func:`pyyeti
+0000b4a0: 2e6e 6173 7472 616e 2e6e 3270 2e62 7569  .nastran.n2p.bui
+0000b4b0: 6c64 5f63 6f6f 7264 7360 2074 6f20 6275  ld_coords` to bu
+0000b4c0: 696c 640a 2020 2020 7468 6520 6f75 7470  ild.    the outp
+0000b4d0: 7574 2e0a 0a20 2020 2053 6565 2061 6c73  ut...    See als
+0000b4e0: 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  o.    --------. 
+0000b4f0: 2020 203a 6675 6e63 3a60 6173 6d32 7573     :func:`asm2us
+0000b500: 6574 602c 203a 6675 6e63 3a60 6275 6c6b  et`, :func:`bulk
+0000b510: 3275 7365 7460 2c20 3a66 756e 633a 6072  2uset`, :func:`r
+0000b520: 6463 6172 6473 602c 0a20 2020 203a 6675  dcards`,.    :fu
+0000b530: 6e63 3a60 7079 7965 7469 2e6e 6173 7472  nc:`pyyeti.nastr
+0000b540: 616e 2e6e 3270 2e62 7569 6c64 5f63 6f6f  an.n2p.build_coo
+0000b550: 7264 7360 0a20 2020 2022 2222 0a20 2020  rds`.    """.   
+0000b560: 2063 6172 6473 203d 2072 6463 6172 6473   cards = rdcards
+0000b570: 280a 2020 2020 2020 2020 662c 2072 2228  (.        f, r"(
+0000b580: 636f 7264 325b 7263 735d 295c 6222 2c20  cord2[rcs])\b", 
+0000b590: 7265 7475 726e 5f76 6172 3d22 6c69 7374  return_var="list
+0000b5a0: 222c 2072 6567 6578 3d54 7275 652c 206b  ", regex=True, k
+0000b5b0: 6565 705f 6e61 6d65 3d54 7275 652c 2062  eep_name=True, b
+0000b5c0: 6c61 6e6b 3d30 0a20 2020 2029 0a0a 2020  lank=0.    )..  
+0000b5d0: 2020 6966 2063 6172 6473 2069 7320 4e6f    if cards is No
+0000b5e0: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
+0000b5f0: 726e 207b 7d0a 0a20 2020 2072 6574 7572  rn {}..    retur
+0000b600: 6e20 6e32 702e 6275 696c 645f 636f 6f72  n n2p.build_coor
+0000b610: 6473 286e 702e 6172 7261 7928 5b5f 636f  ds(np.array([_co
+0000b620: 6e76 6572 745f 6361 7264 2863 6172 6429  nvert_card(card)
+0000b630: 2066 6f72 2063 6172 6420 696e 2063 6172   for card in car
+0000b640: 6473 5d29 290a 0a0a 6465 6620 7774 6772  ds]))...def wtgr
+0000b650: 6964 7328 0a20 2020 2066 2c0a 2020 2020  ids(.    f,.    
+0000b660: 6772 6964 732c 0a20 2020 2063 703d 302c  grids,.    cp=0,
+0000b670: 0a20 2020 2078 797a 3d6e 702e 6172 7261  .    xyz=np.arra
+0000b680: 7928 5b5b 302e 302c 2030 2e30 2c20 302e  y([[0.0, 0.0, 0.
+0000b690: 305d 5d29 2c0a 2020 2020 6364 3d30 2c0a  0]]),.    cd=0,.
+0000b6a0: 2020 2020 7073 3d22 222c 0a20 2020 2073      ps="",.    s
+0000b6b0: 6569 643d 2222 2c0a 2020 2020 666f 726d  eid="",.    form
+0000b6c0: 3d22 7b3a 3136 2e38 667d 222c 0a29 3a0a  ="{:16.8f}",.):.
+0000b6d0: 2020 2020 2222 220a 2020 2020 5772 6974      """.    Writ
+0000b6e0: 6573 204e 6173 7472 616e 2047 5249 4420  es Nastran GRID 
+0000b6f0: 6361 7264 7320 746f 2061 2066 696c 652e  cards to a file.
+0000b700: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0000b710: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0000b720: 2020 2020 6620 3a20 7374 7269 6e67 206f      f : string o
+0000b730: 7220 6669 6c65 5f6c 696b 6520 6f72 2031  r file_like or 1
+0000b740: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+0000b750: 2045 6974 6865 7220 6120 6e61 6d65 206f   Either a name o
+0000b760: 6620 6120 6669 6c65 2c20 6f72 2069 7320  f a file, or is 
+0000b770: 6120 6669 6c65 5f6c 696b 6520 6f62 6a65  a file_like obje
+0000b780: 6374 2061 7320 7265 7475 726e 6564 0a20  ct as returned. 
+0000b790: 2020 2020 2020 2062 7920 3a66 756e 633a         by :func:
+0000b7a0: 606f 7065 6e60 206f 7220 3a63 6c61 7373  `open` or :class
+0000b7b0: 3a60 696f 2e53 7472 696e 6749 4f60 2e20  :`io.StringIO`. 
+0000b7c0: 496e 7075 7420 6173 2069 6e74 6567 6572  Input as integer
+0000b7d0: 2031 2074 6f0a 2020 2020 2020 2020 7772   1 to.        wr
+0000b7e0: 6974 6520 746f 2073 7464 6f75 742e 2043  ite to stdout. C
+0000b7f0: 616e 2061 6c73 6f20 6265 2074 6865 206e  an also be the n
+0000b800: 616d 6520 6f66 2061 2064 6972 6563 746f  ame of a directo
+0000b810: 7279 206f 7220 4e6f 6e65 3b0a 2020 2020  ry or None;.    
+0000b820: 2020 2020 696e 2074 6865 7365 2063 6173      in these cas
+0000b830: 6573 2c20 6120 4755 4920 6973 206f 7065  es, a GUI is ope
+0000b840: 6e65 6420 666f 7220 6669 6c65 2073 656c  ned for file sel
+0000b850: 6563 7469 6f6e 2e0a 2020 2020 6772 6964  ection..    grid
+0000b860: 7320 3a20 3164 2061 7272 6179 5f6c 696b  s : 1d array_lik
+0000b870: 653b 206c 656e 6774 6820 4e0a 2020 2020  e; length N.    
+0000b880: 2020 2020 5665 6374 6f72 206f 6620 6772      Vector of gr
+0000b890: 6964 2069 6473 2e20 5468 6520 6c65 6e67  id ids. The leng
+0000b8a0: 7468 206f 6620 6067 7269 6473 6020 7769  th of `grids` wi
+0000b8b0: 6c6c 2062 6520 7265 6665 7265 6e63 6564  ll be referenced
+0000b8c0: 0a20 2020 2020 2020 2061 7320 6060 4e60  .        as ``N`
+0000b8d0: 6020 696e 2065 7870 6c61 6e61 7469 6f6e  ` in explanation
+0000b8e0: 7320 6265 6c6f 772e 0a20 2020 2063 7020  s below..    cp 
+0000b8f0: 3a20 696e 7465 6765 7220 7363 616c 6172  : integer scalar
+0000b900: 206f 7220 7665 6374 6f72 0a20 2020 2020   or vector.     
+0000b910: 2020 2049 6420 6f66 2063 6f6f 7264 696e     Id of coordin
+0000b920: 6174 6520 7379 7374 656d 2873 2920 6772  ate system(s) gr
+0000b930: 6964 7320 6172 6520 6465 6669 6e65 6420  ids are defined 
+0000b940: 696e 3b20 6569 7468 6572 2073 6361 6c61  in; either scala
+0000b950: 720a 2020 2020 2020 2020 6f72 2076 6563  r.        or vec
+0000b960: 746f 7220 7769 7468 204e 2072 6f77 732e  tor with N rows.
+0000b970: 0a20 2020 2078 797a 203a 2032 6420 6172  .    xyz : 2d ar
+0000b980: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
+0000b990: 2033 2d63 6f6c 756d 6e20 6d61 7472 6978   3-column matrix
+0000b9a0: 206f 6620 6772 6964 206c 6f63 6174 696f   of grid locatio
+0000b9b0: 6e73 3b20 3120 726f 7720 6f72 204e 2072  ns; 1 row or N r
+0000b9c0: 6f77 732e 0a20 2020 2063 6420 3a20 696e  ows..    cd : in
+0000b9d0: 7465 6765 7220 7363 616c 6172 206f 7220  teger scalar or 
+0000b9e0: 7665 6374 6f72 0a20 2020 2020 2020 2049  vector.        I
+0000b9f0: 6420 6f66 2064 6973 706c 6163 656d 656e  d of displacemen
+0000ba00: 7420 636f 6f72 6469 6e61 7465 2073 7973  t coordinate sys
+0000ba10: 7465 6d20 666f 7220 6772 6964 733b 2065  tem for grids; e
+0000ba20: 6974 6865 7220 7363 616c 6172 0a20 2020  ither scalar.   
+0000ba30: 2020 2020 206f 7220 7665 6374 6f72 2077       or vector w
+0000ba40: 6974 6820 4e20 726f 7773 2e0a 2020 2020  ith N rows..    
+0000ba50: 7073 203a 2069 6e74 6567 6572 2073 6361  ps : integer sca
+0000ba60: 6c61 7220 6f72 2076 6563 746f 720a 2020  lar or vector.  
+0000ba70: 2020 2020 2020 5065 726d 616e 656e 7420        Permanent 
+0000ba80: 636f 6e73 7472 6169 6e74 7320 666f 7220  constraints for 
+0000ba90: 6772 6964 732c 2065 673a 2031 3233 3435  grids, eg: 12345
+0000baa0: 363b 2065 6974 6865 7220 7363 616c 6172  6; either scalar
+0000bab0: 206f 720a 2020 2020 2020 2020 7665 6374   or.        vect
+0000bac0: 6f72 2077 6974 6820 4e20 726f 7773 2e0a  or with N rows..
+0000bad0: 2020 2020 7365 6964 203a 2069 6e74 6567      seid : integ
+0000bae0: 6572 2073 6361 6c61 7220 6f72 2076 6563  er scalar or vec
+0000baf0: 746f 720a 2020 2020 2020 2020 5375 7065  tor.        Supe
+0000bb00: 7265 6c65 6d65 6e74 2069 643b 2065 6974  relement id; eit
+0000bb10: 6865 7220 7363 616c 6172 206f 7220 7665  her scalar or ve
+0000bb20: 6374 6f72 2077 6974 6820 4e20 726f 7773  ctor with N rows
+0000bb30: 2e0a 2020 2020 666f 726d 6174 203a 2073  ..    format : s
+0000bb40: 7472 696e 670a 2020 2020 2020 2020 5374  tring.        St
+0000bb50: 7269 6e67 2073 7065 6369 6679 696e 6720  ring specifying 
+0000bb60: 666f 726d 6174 206f 6620 5859 5a20 7661  format of XYZ va
+0000bb70: 6c75 6573 3b20 6d75 7374 2070 726f 6475  lues; must produ
+0000bb80: 6365 2038 206f 7220 3136 0a20 2020 2020  ce 8 or 16.     
+0000bb90: 2020 2063 6861 7261 6374 6572 2073 7472     character str
+0000bba0: 696e 6773 2e0a 0a20 2020 2052 6574 7572  ings...    Retur
+0000bbb0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+0000bbc0: 2020 204e 6f6e 650a 0a20 2020 2045 7861     None..    Exa
+0000bbd0: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+0000bbe0: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
+0000bbf0: 7079 7965 7469 2069 6d70 6f72 7420 6e61  pyyeti import na
+0000bc00: 7374 7261 6e0a 2020 2020 3e3e 3e20 696d  stran.    >>> im
+0000bc10: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+0000bc20: 0a20 2020 203e 3e3e 206e 6173 7472 616e  .    >>> nastran
+0000bc30: 2e77 7467 7269 6473 2831 2c20 6e70 2e61  .wtgrids(1, np.a
+0000bc40: 7261 6e67 6528 312c 2034 2929 0a20 2020  range(1, 4)).   
+0000bc50: 2047 5249 442a 2020 2020 2020 2020 2020   GRID*          
+0000bc60: 2020 2020 2020 2020 3120 2020 2020 2020          1       
+0000bc70: 2020 2020 2020 2020 3020 2020 2020 2030          0      0
+0000bc80: 2e30 3030 3030 3030 3020 2020 2020 2030  .00000000      0
+0000bc90: 2e30 3030 3030 3030 300a 2020 2020 2a20  .00000000.    * 
+0000bca0: 2020 2020 2020 2020 2020 2020 302e 3030              0.00
+0000bcb0: 3030 3030 3030 2020 2020 2020 2020 2020  000000          
+0000bcc0: 2020 2020 2030 0a20 2020 2047 5249 442a       0.    GRID*
+0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bce0: 2020 3220 2020 2020 2020 2020 2020 2020    2             
+0000bcf0: 2020 3020 2020 2020 2030 2e30 3030 3030    0      0.00000
+0000bd00: 3030 3020 2020 2020 2030 2e30 3030 3030  000      0.00000
+0000bd10: 3030 300a 2020 2020 2a20 2020 2020 2020  000.    *       
+0000bd20: 2020 2020 2020 302e 3030 3030 3030 3030        0.00000000
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0000bd40: 0a20 2020 2047 5249 442a 2020 2020 2020  .    GRID*      
+0000bd50: 2020 2020 2020 2020 2020 2020 3320 2020              3   
+0000bd60: 2020 2020 2020 2020 2020 2020 3020 2020              0   
+0000bd70: 2020 2030 2e30 3030 3030 3030 3020 2020     0.00000000   
+0000bd80: 2020 2030 2e30 3030 3030 3030 300a 2020     0.00000000.  
+0000bd90: 2020 2a20 2020 2020 2020 2020 2020 2020    *             
+0000bda0: 302e 3030 3030 3030 3030 2020 2020 2020  0.00000000      
+0000bdb0: 2020 2020 2020 2020 2030 0a20 2020 203e           0.    >
+0000bdc0: 3e3e 2078 797a 203d 206e 702e 6172 7261  >> xyz = np.arra
+0000bdd0: 7928 5b5b 2e31 2c20 2e32 2c20 2e33 5d2c  y([[.1, .2, .3],
+0000bde0: 205b 312e 312c 2031 2e32 2c20 312e 335d   [1.1, 1.2, 1.3]
+0000bdf0: 5d29 0a20 2020 203e 3e3e 206e 6173 7472  ]).    >>> nastr
+0000be00: 616e 2e77 7467 7269 6473 2831 2c20 5b31  an.wtgrids(1, [1
+0000be10: 3030 2c20 3230 305d 2c20 7879 7a3d 7879  00, 200], xyz=xy
+0000be20: 7a2c 2063 643d 3130 2c0a 2020 2020 2e2e  z, cd=10,.    ..
+0000be30: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+0000be40: 2020 666f 726d 3d27 7b3a 382e 3266 7d27    form='{:8.2f}'
+0000be50: 290a 2020 2020 4752 4944 2020 2020 2020  ).    GRID      
+0000be60: 2020 2031 3030 2020 2020 2020 2030 2020     100       0  
+0000be70: 2020 302e 3130 2020 2020 302e 3230 2020    0.10    0.20  
+0000be80: 2020 302e 3330 2020 2020 2020 3130 0a20    0.30      10. 
+0000be90: 2020 2047 5249 4420 2020 2020 2020 2020     GRID         
+0000bea0: 3230 3020 2020 2020 2020 3020 2020 2031  200       0    1
+0000beb0: 2e31 3020 2020 2031 2e32 3020 2020 2031  .10    1.20    1
+0000bec0: 2e33 3020 2020 2020 2031 300a 2020 2020  .30      10.    
+0000bed0: 2222 220a 2020 2020 6772 6964 7320 3d20  """.    grids = 
+0000bee0: 6e70 2e61 746c 6561 7374 5f31 6428 6772  np.atleast_1d(gr
+0000bef0: 6964 7329 2e72 6176 656c 2829 0a20 2020  ids).ravel().   
+0000bf00: 2078 797a 203d 206e 702e 6174 6c65 6173   xyz = np.atleas
+0000bf10: 745f 3264 2878 797a 290a 2020 2020 7465  t_2d(xyz).    te
+0000bf20: 7374 7374 7220 3d20 666f 726d 2e66 6f72  ststr = form.for
+0000bf30: 6d61 7428 312e 3029 0a20 2020 206c 656e  mat(1.0).    len
+0000bf40: 6774 6820 3d20 6c65 6e28 7465 7374 7374  gth = len(testst
+0000bf50: 7229 0a20 2020 2069 6620 6c65 6e67 7468  r).    if length
+0000bf60: 2021 3d20 3820 616e 6420 6c65 6e67 7468   != 8 and length
+0000bf70: 2021 3d20 3136 3a0a 2020 2020 2020 2020   != 16:.        
+0000bf80: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000bf90: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+0000bfa0: 6066 6f72 6d60 2070 726f 6475 6365 7320  `form` produces 
+0000bfb0: 6120 7b6c 656e 6774 687d 206c 656e 6774  a {length} lengt
+0000bfc0: 6820 7374 7269 6e67 2e20 4974 206d 7573  h string. It mus
+0000bfd0: 7420 6265 2038 206f 7220 3136 2e5c 6e22  t be 8 or 16.\n"
+0000bfe0: 0a20 2020 2020 2020 2029 0a20 2020 2069  .        ).    i
+0000bff0: 6620 7073 203d 3d20 7365 6964 203d 3d20  f ps == seid == 
+0000c000: 2222 3a0a 2020 2020 2020 2020 6966 206c  "":.        if l
+0000c010: 656e 2874 6573 7473 7472 2920 3e20 383a  en(teststr) > 8:
+0000c020: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+0000c030: 696e 6720 3d20 280a 2020 2020 2020 2020  ing = (.        
+0000c040: 2020 2020 2020 2020 2247 5249 442a 2020          "GRID*  
+0000c050: 207b 3a31 3664 7d7b 3a31 3664 7d22 202b   {:16d}{:16d}" +
+0000c060: 2066 6f72 6d20 2a20 3220 2b20 225c 6e2a   form * 2 + "\n*
+0000c070: 2020 2020 2020 2022 202b 2066 6f72 6d20         " + form 
+0000c080: 2b20 227b 3a31 3664 7d5c 6e22 0a20 2020  + "{:16d}\n".   
+0000c090: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000c0a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c0b0: 2020 2020 2073 7472 696e 6720 3d20 2247       string = "G
+0000c0c0: 5249 4420 2020 207b 3a38 647d 7b3a 3864  RID    {:8d}{:8d
+0000c0d0: 7d22 202b 2066 6f72 6d20 2a20 3320 2b20  }" + form * 3 + 
+0000c0e0: 227b 3a38 647d 5c6e 220a 2020 2020 2020  "{:8d}\n".      
+0000c0f0: 2020 7772 6974 6572 2e76 6563 7772 6974    writer.vecwrit
+0000c100: 6528 662c 2073 7472 696e 672c 2067 7269  e(f, string, gri
+0000c110: 6473 2c20 6370 2c20 7879 7a5b 3a2c 2030  ds, cp, xyz[:, 0
+0000c120: 5d2c 2078 797a 5b3a 2c20 315d 2c20 7879  ], xyz[:, 1], xy
+0000c130: 7a5b 3a2c 2032 5d2c 2063 6429 0a20 2020  z[:, 2], cd).   
+0000c140: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+0000c150: 6620 6c65 6e28 7465 7374 7374 7229 203e  f len(teststr) >
+0000c160: 2038 3a0a 2020 2020 2020 2020 2020 2020   8:.            
+0000c170: 7374 7269 6e67 203d 2028 0a20 2020 2020  string = (.     
+0000c180: 2020 2020 2020 2020 2020 2022 4752 4944             "GRID
+0000c190: 2a20 2020 7b3a 3136 647d 7b3a 3136 647d  *   {:16d}{:16d}
+0000c1a0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000c1b0: 2020 2b20 666f 726d 202a 2032 0a20 2020    + form * 2.   
+0000c1c0: 2020 2020 2020 2020 2020 2020 202b 2022               + "
+0000c1d0: 5c6e 2a20 2020 2020 2020 220a 2020 2020  \n*       ".    
+0000c1e0: 2020 2020 2020 2020 2020 2020 2b20 666f              + fo
+0000c1f0: 726d 0a20 2020 2020 2020 2020 2020 2020  rm.             
+0000c200: 2020 202b 2022 7b3a 3136 647d 7b3a 3e31     + "{:16d}{:>1
+0000c210: 367d 7b3a 3e31 367d 5c6e 220a 2020 2020  6}{:>16}\n".    
+0000c220: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000c230: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000c240: 2020 2020 7374 7269 6e67 203d 2022 4752      string = "GR
+0000c250: 4944 2020 2020 7b3a 3864 7d7b 3a38 647d  ID    {:8d}{:8d}
+0000c260: 2220 2b20 666f 726d 202a 2033 202b 2022  " + form * 3 + "
+0000c270: 7b3a 3864 7d7b 3a3e 387d 7b3a 3e38 7d5c  {:8d}{:>8}{:>8}\
+0000c280: 6e22 0a20 2020 2020 2020 2077 7269 7465  n".        write
+0000c290: 722e 7665 6377 7269 7465 280a 2020 2020  r.vecwrite(.    
+0000c2a0: 2020 2020 2020 2020 662c 2073 7472 696e          f, strin
+0000c2b0: 672c 2067 7269 6473 2c20 6370 2c20 7879  g, grids, cp, xy
+0000c2c0: 7a5b 3a2c 2030 5d2c 2078 797a 5b3a 2c20  z[:, 0], xyz[:, 
+0000c2d0: 315d 2c20 7879 7a5b 3a2c 2032 5d2c 2063  1], xyz[:, 2], c
+0000c2e0: 642c 2070 732c 2073 6569 640a 2020 2020  d, ps, seid.    
+0000c2f0: 2020 2020 290a 0a0a 6465 6620 7264 7461      )...def rdta
+0000c300: 626c 6564 3128 662c 206e 616d 653d 2274  bled1(f, name="t
+0000c310: 6162 6c65 6431 2229 3a0a 2020 2020 2222  abled1"):.    ""
+0000c320: 220a 2020 2020 5265 6164 204e 6173 7472  ".    Read Nastr
+0000c330: 616e 2054 4142 4c45 4431 206f 7220 6f74  an TABLED1 or ot
+0000c340: 6865 7220 6964 656e 7469 6361 6c6c 7920  her identically 
+0000c350: 666f 726d 6174 7465 6420 6361 7264 7320  formatted cards 
+0000c360: 6672 6f6d 2061 0a20 2020 204e 6173 7472  from a.    Nastr
+0000c370: 616e 2062 756c 6b20 6669 6c65 2e0a 0a20  an bulk file... 
+0000c380: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000c390: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000c3a0: 2066 203a 2073 7472 696e 6720 6f72 2066   f : string or f
+0000c3b0: 696c 655f 6c69 6b65 206f 7220 4e6f 6e65  ile_like or None
+0000c3c0: 0a20 2020 2020 2020 2045 6974 6865 7220  .        Either 
+0000c3d0: 6120 6e61 6d65 206f 6620 6120 6669 6c65  a name of a file
+0000c3e0: 2c20 6f72 2069 7320 6120 6669 6c65 5f6c  , or is a file_l
+0000c3f0: 696b 6520 6f62 6a65 6374 2061 7320 7265  ike object as re
+0000c400: 7475 726e 6564 0a20 2020 2020 2020 2062  turned.        b
+0000c410: 7920 3a66 756e 633a 606f 7065 6e60 2e20  y :func:`open`. 
+0000c420: 4966 2066 696c 655f 6c69 6b65 206f 626a  If file_like obj
+0000c430: 6563 742c 2069 7420 6973 2072 6577 6f75  ect, it is rewou
+0000c440: 6e64 2066 6972 7374 2e20 4361 6e0a 2020  nd first. Can.  
+0000c450: 2020 2020 2020 616c 736f 2062 6520 7468        also be th
+0000c460: 6520 6e61 6d65 206f 6620 6120 6469 7265  e name of a dire
+0000c470: 6374 6f72 7920 6f72 204e 6f6e 653b 2069  ctory or None; i
+0000c480: 6e20 7468 6573 6520 6361 7365 732c 2061  n these cases, a
+0000c490: 2047 5549 0a20 2020 2020 2020 2069 7320   GUI.        is 
+0000c4a0: 6f70 656e 6564 2066 6f72 2066 696c 6520  opened for file 
+0000c4b0: 7365 6c65 6374 696f 6e2e 0a20 2020 206e  selection..    n
+0000c4c0: 616d 6520 3a20 7374 7269 6e67 3b20 6f70  ame : string; op
+0000c4d0: 7469 6f6e 616c 0a20 2020 2020 2020 204e  tional.        N
+0000c4e0: 616d 6520 6f66 2063 6172 6473 2074 6f20  ame of cards to 
+0000c4f0: 7265 6164 2e0a 0a20 2020 2052 6574 7572  read...    Retur
+0000c500: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+0000c510: 2020 2064 6374 203a 2064 6963 7469 6f6e     dct : diction
+0000c520: 6172 790a 2020 2020 2020 2020 4469 6374  ary.        Dict
+0000c530: 696f 6e61 7279 206f 6620 5441 424c 4544  ionary of TABLED
+0000c540: 3120 286f 7220 7369 6d69 6c61 7229 2063  1 (or similar) c
+0000c550: 6172 6473 3a0a 0a20 2020 2020 2020 202e  ards:..        .
+0000c560: 2e20 636f 6465 2d62 6c6f 636b 3a3a 206e  . code-block:: n
+0000c570: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
+0000c580: 207b 4944 313a 205b 7469 6d65 2c20 6461   {ID1: [time, da
+0000c590: 7461 5d2c 0a20 2020 2020 2020 2020 2020  ta],.           
+0000c5a0: 2020 4944 323a 205b 7469 6d65 2c20 6461    ID2: [time, da
+0000c5b0: 7461 5d2c 202e 2e2e 7d0a 0a20 2020 204e  ta], ...}..    N
+0000c5c0: 6f74 6573 0a20 2020 202d 2d2d 2d2d 0a20  otes.    -----. 
+0000c5d0: 2020 2054 6869 7320 726f 7574 696e 6520     This routine 
+0000c5e0: 7573 6573 203a 6675 6e63 3a60 7264 6361  uses :func:`rdca
+0000c5f0: 7264 7360 2074 6f20 6c6f 6164 2074 6865  rds` to load the
+0000c600: 2064 6174 6120 2863 616e 2072 6561 6420   data (can read 
+0000c610: 380a 2020 2020 6f72 2031 3620 6669 7865  8.    or 16 fixe
+0000c620: 6420 6669 656c 6420 6f72 2063 6f6d 6d61  d field or comma
+0000c630: 2d64 656c 696d 6974 6564 292e 0a0a 2020  -delimited)...  
+0000c640: 2020 5365 6520 616c 736f 0a20 2020 202d    See also.    -
+0000c650: 2d2d 2d2d 2d2d 2d0a 2020 2020 3a66 756e  -------.    :fun
+0000c660: 633a 6077 7474 6162 6c65 6431 600a 0a20  c:`wttabled1`.. 
+0000c670: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+0000c680: 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e  --------.    >>>
+0000c690: 2066 726f 6d20 7079 7965 7469 2069 6d70   from pyyeti imp
+0000c6a0: 6f72 7420 6e61 7374 7261 6e0a 2020 2020  ort nastran.    
+0000c6b0: 3e3e 3e20 696d 706f 7274 206e 756d 7079  >>> import numpy
+0000c6c0: 2061 7320 6e70 0a20 2020 203e 3e3e 2066   as np.    >>> f
+0000c6d0: 726f 6d20 696f 2069 6d70 6f72 7420 5374  rom io import St
+0000c6e0: 7269 6e67 494f 0a20 2020 203e 3e3e 2074  ringIO.    >>> t
+0000c6f0: 203d 206e 702e 6172 616e 6765 2830 2c20   = np.arange(0, 
+0000c700: 312c 202e 3035 290a 2020 2020 3e3e 3e20  1, .05).    >>> 
+0000c710: 6420 3d20 6e70 2e73 696e 2832 2a6e 702e  d = np.sin(2*np.
+0000c720: 7069 2a33 2a74 290a 2020 2020 3e3e 3e20  pi*3*t).    >>> 
+0000c730: 7769 7468 2053 7472 696e 6749 4f28 2920  with StringIO() 
+0000c740: 6173 2066 3a0a 2020 2020 2e2e 2e20 2020  as f:.    ...   
+0000c750: 2020 6e61 7374 7261 6e2e 7774 7461 626c    nastran.wttabl
+0000c760: 6564 3128 662c 2034 3030 302c 2074 2c20  ed1(f, 4000, t, 
+0000c770: 642c 2027 3320 487a 2053 696e 6520 5761  d, '3 Hz Sine Wa
+0000c780: 7665 272c 0a20 2020 202e 2e2e 2020 2020  ve',.    ...    
+0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7a0: 2020 2066 6f72 6d3d 277b 3a38 2e32 667d     form='{:8.2f}
+0000c7b0: 7b3a 382e 3566 7d27 290a 2020 2020 2e2e  {:8.5f}').    ..
+0000c7c0: 2e20 2020 2020 6463 7420 3d20 6e61 7374  .     dct = nast
+0000c7d0: 7261 6e2e 7264 7461 626c 6564 3128 6629  ran.rdtabled1(f)
+0000c7e0: 0a20 2020 203e 3e3e 206e 702e 616c 6c63  .    >>> np.allc
+0000c7f0: 6c6f 7365 2874 2c20 6463 745b 3430 3030  lose(t, dct[4000
+0000c800: 5d5b 3a2c 2030 5d29 0a20 2020 2054 7275  ][:, 0]).    Tru
+0000c810: 650a 2020 2020 3e3e 3e20 6e70 2e61 6c6c  e.    >>> np.all
+0000c820: 636c 6f73 6528 642c 2064 6374 5b34 3030  close(d, dct[400
+0000c830: 305d 5b3a 2c20 315d 290a 2020 2020 5472  0][:, 1]).    Tr
+0000c840: 7565 0a20 2020 2022 2222 0a20 2020 2064  ue.    """.    d
+0000c850: 203d 2072 6463 6172 6473 2866 2c20 6e61   = rdcards(f, na
+0000c860: 6d65 2c20 7265 7475 726e 5f76 6172 3d22  me, return_var="
+0000c870: 6469 6374 2229 0a20 2020 2066 6f72 2074  dict").    for t
+0000c880: 6964 2069 6e20 643a 0a20 2020 2020 2020  id in d:.       
+0000c890: 2076 6563 203d 2064 5b74 6964 5d0a 2020   vec = d[tid].  
+0000c8a0: 2020 2020 2020 645b 7469 645d 203d 206e        d[tid] = n
+0000c8b0: 702e 7673 7461 636b 285b 7665 635b 383a  p.vstack([vec[8:
+0000c8c0: 2d31 3a32 5d2c 2076 6563 5b39 3a2d 313a  -1:2], vec[9:-1:
+0000c8d0: 325d 5d29 2e54 0a20 2020 2072 6574 7572  2]]).T.    retur
+0000c8e0: 6e20 640a 0a0a 4067 7569 746f 6f6c 732e  n d...@guitools.
+0000c8f0: 7772 6974 655f 7465 7874 5f66 696c 650a  write_text_file.
+0000c900: 6465 6620 7774 7461 626c 6564 3128 662c  def wttabled1(f,
+0000c910: 2074 6964 2c20 742c 2064 2c20 7469 746c   tid, t, d, titl
+0000c920: 653d 4e6f 6e65 2c20 666f 726d 3d22 7b3a  e=None, form="{:
+0000c930: 3136 2e39 457d 7b3a 3136 2e39 457d 222c  16.9E}{:16.9E}",
+0000c940: 2074 6162 6c65 7374 723d 2254 4142 4c45   tablestr="TABLE
+0000c950: 4431 2229 3a0a 2020 2020 2222 220a 2020  D1"):.    """.  
+0000c960: 2020 5772 6974 6573 2061 204e 6173 7472    Writes a Nastr
+0000c970: 616e 2054 4142 4c45 4431 2028 6f72 2073  an TABLED1 (or s
+0000c980: 696d 696c 6172 2920 6361 7264 2074 6f20  imilar) card to 
+0000c990: 6120 6669 6c65 2e0a 0a20 2020 2050 6172  a file...    Par
+0000c9a0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0000c9b0: 2d2d 2d2d 2d2d 0a20 2020 2066 203a 2073  ------.    f : s
+0000c9c0: 7472 696e 6720 6f72 2066 696c 655f 6c69  tring or file_li
+0000c9d0: 6b65 206f 7220 3120 6f72 204e 6f6e 650a  ke or 1 or None.
+0000c9e0: 2020 2020 2020 2020 4569 7468 6572 2061          Either a
+0000c9f0: 206e 616d 6520 6f66 2061 2066 696c 652c   name of a file,
+0000ca00: 206f 7220 6973 2061 2066 696c 655f 6c69   or is a file_li
+0000ca10: 6b65 206f 626a 6563 7420 6173 2072 6574  ke object as ret
+0000ca20: 7572 6e65 640a 2020 2020 2020 2020 6279  urned.        by
+0000ca30: 203a 6675 6e63 3a60 6f70 656e 6020 6f72   :func:`open` or
+0000ca40: 203a 636c 6173 733a 6069 6f2e 5374 7269   :class:`io.Stri
+0000ca50: 6e67 494f 602e 2049 6e70 7574 2061 7320  ngIO`. Input as 
+0000ca60: 696e 7465 6765 7220 3120 746f 0a20 2020  integer 1 to.   
+0000ca70: 2020 2020 2077 7269 7465 2074 6f20 7374       write to st
+0000ca80: 646f 7574 2e20 4361 6e20 616c 736f 2062  dout. Can also b
+0000ca90: 6520 7468 6520 6e61 6d65 206f 6620 6120  e the name of a 
+0000caa0: 6469 7265 6374 6f72 7920 6f72 204e 6f6e  directory or Non
+0000cab0: 653b 0a20 2020 2020 2020 2069 6e20 7468  e;.        in th
+0000cac0: 6573 6520 6361 7365 732c 2061 2047 5549  ese cases, a GUI
+0000cad0: 2069 7320 6f70 656e 6564 2066 6f72 2066   is opened for f
+0000cae0: 696c 6520 7365 6c65 6374 696f 6e2e 0a20  ile selection.. 
+0000caf0: 2020 2074 6964 203a 2069 6e74 6567 6572     tid : integer
+0000cb00: 0a20 2020 2020 2020 2049 4420 666f 7220  .        ID for 
+0000cb10: 5441 424c 4544 3120 6361 7264 0a20 2020  TABLED1 card.   
+0000cb20: 2074 203a 2031 6420 6172 7261 795f 6c69   t : 1d array_li
+0000cb30: 6b65 0a20 2020 2020 2020 2074 696d 6520  ke.        time 
+0000cb40: 7665 6374 6f72 0a20 2020 2064 203a 2031  vector.    d : 1
+0000cb50: 6420 6172 7261 795f 6c69 6b65 0a20 2020  d array_like.   
+0000cb60: 2020 2020 2064 6174 6120 7665 6374 6f72       data vector
+0000cb70: 0a20 2020 2074 6974 6c65 203a 2073 7472  .    title : str
+0000cb80: 696e 6720 6f72 204e 6f6e 653b 206f 7074  ing or None; opt
+0000cb90: 696f 6e61 6c0a 2020 2020 2020 2020 4966  ional.        If
+0000cba0: 2061 2073 7472 696e 672c 2069 7420 6973   a string, it is
+0000cbb0: 2077 7269 7474 656e 2061 7320 6120 636f   written as a co
+0000cbc0: 6d6d 656e 7420 6265 666f 7265 2074 6162  mment before tab
+0000cbd0: 6c65 2e20 4966 204e 6f6e 652c 0a20 2020  le. If None,.   
+0000cbe0: 2020 2020 206e 6f20 7374 7269 6e67 2069       no string i
+0000cbf0: 7320 7772 6974 7465 6e2e 0a20 2020 2066  s written..    f
+0000cc00: 6f72 6d20 3a20 7374 7269 6e67 3b20 6f70  orm : string; op
+0000cc10: 7469 6f6e 616c 0a20 2020 2020 2020 2053  tional.        S
+0000cc20: 7472 696e 6720 7370 6563 6966 7969 6e67  tring specifying
+0000cc30: 2074 6865 2066 6f72 6d61 7420 6f66 2061   the format of a
+0000cc40: 2073 696e 676c 6520 5b74 696d 652c 2064   single [time, d
+0000cc50: 6174 615d 2070 6169 722e 0a20 2020 2020  ata] pair..     
+0000cc60: 2020 2045 7870 6563 7465 6420 746f 2072     Expected to r
+0000cc70: 6573 756c 7420 696e 2061 2073 7472 696e  esult in a strin
+0000cc80: 6720 6569 7468 6572 2031 3620 6f72 2033  g either 16 or 3
+0000cc90: 3220 6368 6172 6163 7465 7273 0a20 2020  2 characters.   
+0000cca0: 2020 2020 206c 6f6e 672e 0a20 2020 2074       long..    t
+0000ccb0: 6162 6c65 7374 7220 3a20 7374 7269 6e67  ablestr : string
+0000ccc0: 3b20 6f70 7469 6f6e 616c 0a20 2020 2020  ; optional.     
+0000ccd0: 2020 204e 616d 6520 6f66 2063 6172 6420     Name of card 
+0000cce0: 746f 2077 7269 7465 3b20 6d75 7374 2062  to write; must b
+0000ccf0: 6520 7361 6d65 2066 6f72 6d61 7420 6173  e same format as
+0000cd00: 2054 4142 4c45 4431 2e0a 0a20 2020 2052   TABLED1...    R
+0000cd10: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0000cd20: 2d2d 0a20 2020 204e 6f6e 650a 0a20 2020  --.    None..   
+0000cd30: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
+0000cd40: 0a20 2020 2049 6e20 7468 6520 666f 726d  .    In the form
+0000cd50: 6174 2073 7472 696e 672c 2069 6e63 6c75  at string, inclu
+0000cd60: 6465 2061 2023 2073 6967 6e20 746f 2066  de a # sign to f
+0000cd70: 6f72 6365 2061 2064 6563 696d 616c 2070  orce a decimal p
+0000cd80: 6f69 6e74 2074 6f0a 2020 2020 6170 7065  oint to.    appe
+0000cd90: 6172 2077 6974 686f 7574 2074 7261 696c  ar without trail
+0000cda0: 696e 6720 6469 6769 7473 2e20 466f 7220  ing digits. For 
+0000cdb0: 6578 616d 706c 652c 2027 7b3a 382e 3266  example, '{:8.2f
+0000cdc0: 7d7b 3a23 382e 3066 7d27 0a20 2020 2077  }{:#8.0f}'.    w
+0000cdd0: 6f75 6c64 2070 7269 6e74 206c 696b 6520  ould print like 
+0000cde0: 7468 6973 3a20 2720 3132 2e33 3420 3132  this: ' 12.34 12
+0000cdf0: 3334 3536 2e27 2e0a 0a20 2020 2053 6565  3456.'...    See
+0000ce00: 2061 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d   also.    ------
+0000ce10: 2d2d 0a20 2020 203a 6675 6e63 3a60 7264  --.    :func:`rd
+0000ce20: 7461 626c 6564 3160 0a0a 2020 2020 4578  tabled1`..    Ex
+0000ce30: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0000ce40: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
+0000ce50: 2070 7979 6574 6920 696d 706f 7274 206e   pyyeti import n
+0000ce60: 6173 7472 616e 0a20 2020 203e 3e3e 2069  astran.    >>> i
+0000ce70: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+0000ce80: 700a 2020 2020 3e3e 3e20 7420 3d20 6e70  p.    >>> t = np
+0000ce90: 2e61 7261 6e67 6528 302c 202e 3931 2c20  .arange(0, .91, 
+0000cea0: 2e30 3529 0a20 2020 203e 3e3e 2064 203d  .05).    >>> d =
+0000ceb0: 206e 702e 7369 6e28 322a 6e70 2e70 692a   np.sin(2*np.pi*
+0000cec0: 332a 7429 0a20 2020 203e 3e3e 206e 6173  3*t).    >>> nas
+0000ced0: 7472 616e 2e77 7474 6162 6c65 6431 2831  tran.wttabled1(1
+0000cee0: 2c20 3430 3030 2c20 742c 2064 2c20 2733  , 4000, t, d, '3
+0000cef0: 2048 7a20 5369 6e65 2057 6176 6527 2c0a   Hz Sine Wave',.
+0000cf00: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+0000cf10: 2020 2020 2020 2020 2020 666f 726d 3d27            form='
+0000cf20: 7b3a 382e 3266 7d7b 3a38 2e35 667d 2729  {:8.2f}{:8.5f}')
+0000cf30: 0a20 2020 2024 2033 2048 7a20 5369 6e65  .    $ 3 Hz Sine
+0000cf40: 2057 6176 650a 2020 2020 5441 424c 4544   Wave.    TABLED
+0000cf50: 3120 2020 2020 3430 3030 0a20 2020 2020  1     4000.     
+0000cf60: 2020 2020 2020 2020 2020 2030 2e30 3020             0.00 
+0000cf70: 302e 3030 3030 3020 2020 2030 2e30 3520  0.00000    0.05 
+0000cf80: 302e 3830 3930 3220 2020 2030 2e31 3020  0.80902    0.10 
+0000cf90: 302e 3935 3130 3620 2020 2030 2e31 3520  0.95106    0.15 
+0000cfa0: 302e 3330 3930 320a 2020 2020 2020 2020  0.30902.        
+0000cfb0: 2020 2020 2020 2020 302e 3230 2d30 2e35          0.20-0.5
+0000cfc0: 3837 3739 2020 2020 302e 3235 2d31 2e30  8779    0.25-1.0
+0000cfd0: 3030 3030 2020 2020 302e 3330 2d30 2e35  0000    0.30-0.5
+0000cfe0: 3837 3739 2020 2020 302e 3335 2030 2e33  8779    0.35 0.3
+0000cff0: 3039 3032 0a20 2020 2020 2020 2020 2020  0902.           
+0000d000: 2020 2020 2030 2e34 3020 302e 3935 3130       0.40 0.9510
+0000d010: 3620 2020 2030 2e34 3520 302e 3830 3930  6    0.45 0.8090
+0000d020: 3220 2020 2030 2e35 3020 302e 3030 3030  2    0.50 0.0000
+0000d030: 3020 2020 2030 2e35 352d 302e 3830 3930  0    0.55-0.8090
+0000d040: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+0000d050: 2020 302e 3630 2d30 2e39 3531 3036 2020    0.60-0.95106  
+0000d060: 2020 302e 3635 2d30 2e33 3039 3032 2020    0.65-0.30902  
+0000d070: 2020 302e 3730 2030 2e35 3837 3739 2020    0.70 0.58779  
+0000d080: 2020 302e 3735 2031 2e30 3030 3030 0a20    0.75 1.00000. 
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0000d0a0: 2e38 3020 302e 3538 3737 3920 2020 2030  .80 0.58779    0
+0000d0b0: 2e38 352d 302e 3330 3930 3220 2020 2030  .85-0.30902    0
+0000d0c0: 2e39 302d 302e 3935 3130 3645 4e44 540a  .90-0.95106ENDT.
+0000d0d0: 2020 2020 3e3e 3e20 6e61 7374 7261 6e2e      >>> nastran.
+0000d0e0: 7774 7461 626c 6564 3128 312c 2034 3030  wttabled1(1, 400
+0000d0f0: 302c 205b 312c 2032 2c20 335d 2c20 5b31  0, [1, 2, 3], [1
+0000d100: 2c20 322c 2033 5d2c 0a20 2020 202e 2e2e  , 2, 3],.    ...
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2020 2066 6f72 6d3d 277b 3a31 362e 3266     form='{:16.2f
+0000d130: 7d7b 3a31 362e 3566 7d27 290a 2020 2020  }{:16.5f}').    
+0000d140: 5441 424c 4544 312a 2020 2020 2020 2020  TABLED1*        
+0000d150: 2020 2020 3430 3030 0a20 2020 202a 0a20      4000.    *. 
+0000d160: 2020 202a 2020 2020 2020 2020 2020 2020     *            
+0000d170: 2020 2020 2020 2031 2e30 3020 2020 2020         1.00     
+0000d180: 2020 2020 312e 3030 3030 3020 2020 2020      1.00000     
+0000d190: 2020 2020 2020 2032 2e30 3020 2020 2020         2.00     
+0000d1a0: 2020 2020 322e 3030 3030 300a 2020 2020      2.00000.    
+0000d1b0: 2a20 2020 2020 2020 2020 2020 2020 2020  *               
+0000d1c0: 2020 2020 332e 3030 2020 2020 2020 2020      3.00        
+0000d1d0: 2033 2e30 3030 3030 454e 4454 0a20 2020   3.00000ENDT.   
+0000d1e0: 2022 2222 0a20 2020 2074 2c20 6420 3d20   """.    t, d = 
+0000d1f0: 6e70 2e61 746c 6561 7374 5f31 6428 742c  np.atleast_1d(t,
+0000d200: 2064 290a 2020 2020 7420 3d20 742e 7261   d).    t = t.ra
+0000d210: 7665 6c28 290a 2020 2020 6420 3d20 642e  vel().    d = d.
+0000d220: 7261 7665 6c28 290a 2020 2020 6e70 7473  ravel().    npts
+0000d230: 203d 206c 656e 2874 290a 2020 2020 6966   = len(t).    if
+0000d240: 206c 656e 2864 2920 213d 206e 7074 733a   len(d) != npts:
+0000d250: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+0000d260: 616c 7565 4572 726f 7228 6622 6c65 6e28  alueError(f"len(
+0000d270: 6429 2069 7320 7b6c 656e 2864 297d 2062  d) is {len(d)} b
+0000d280: 7574 206c 656e 2874 2920 6973 207b 6e70  ut len(t) is {np
+0000d290: 7473 7d22 290a 0a20 2020 2023 2064 6574  ts}")..    # det
+0000d2a0: 6572 6d69 6e65 2069 6620 7573 696e 6720  ermine if using 
+0000d2b0: 7369 6e67 6c65 206f 7220 646f 7562 6c65  single or double
+0000d2c0: 2066 6965 6c64 3a0a 2020 2020 6e20 3d20   field:.    n = 
+0000d2d0: 6c65 6e28 666f 726d 2e66 6f72 6d61 7428  len(form.format(
+0000d2e0: 312c 2031 2929 0a20 2020 2069 6620 6e20  1, 1)).    if n 
+0000d2f0: 213d 2031 3620 616e 6420 6e20 213d 2033  != 16 and n != 3
+0000d300: 323a 0a20 2020 2020 2020 2072 6169 7365  2:.        raise
+0000d310: 2056 616c 7565 4572 726f 7228 6622 6066   ValueError(f"`f
+0000d320: 6f72 6d60 2070 726f 6475 6365 7320 6120  orm` produces a 
+0000d330: 7b6e 7d20 6c65 6e67 7468 2073 7472 696e  {n} length strin
+0000d340: 672e 2049 7420 6d75 7374 2062 6520 3136  g. It must be 16
+0000d350: 206f 7220 3332 2e22 290a 2020 2020 6966   or 32.").    if
+0000d360: 2074 6974 6c65 3a0a 2020 2020 2020 2020   title:.        
+0000d370: 662e 7772 6974 6528 6622 2420 7b74 6974  f.write(f"$ {tit
+0000d380: 6c65 3a73 7d5c 6e22 290a 2020 2020 6966  le:s}\n").    if
+0000d390: 206e 203d 3d20 3332 3a0a 2020 2020 2020   n == 32:.      
+0000d3a0: 2020 7461 626c 6573 7472 203d 2074 6162    tablestr = tab
+0000d3b0: 6c65 7374 7220 2b20 222a 220a 2020 2020  lestr + "*".    
+0000d3c0: 2020 2020 662e 7772 6974 6528 6622 7b74      f.write(f"{t
+0000d3d0: 6162 6c65 7374 723a 3c38 737d 7b74 6964  ablestr:<8s}{tid
+0000d3e0: 3a31 3664 7d5c 6e2a 5c6e 2229 0a20 2020  :16d}\n*\n").   
+0000d3f0: 2020 2020 2072 6f77 7320 3d20 6e70 7473       rows = npts
+0000d400: 202f 2f20 320a 2020 2020 2020 2020 7220   // 2.        r 
+0000d410: 3d20 726f 7773 202a 2032 0a20 2020 2020  = rows * 2.     
+0000d420: 2020 2077 7269 7465 722e 7665 6377 7269     writer.vecwri
+0000d430: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
+0000d440: 662c 2022 2a20 2020 2020 2020 2220 2b20  f, "*       " + 
+0000d450: 666f 726d 202a 2032 202b 2022 5c6e 222c  form * 2 + "\n",
+0000d460: 2074 5b3a 723a 325d 2c20 645b 3a72 3a32   t[:r:2], d[:r:2
+0000d470: 5d2c 2074 5b31 3a72 3a32 5d2c 2064 5b31  ], t[1:r:2], d[1
+0000d480: 3a72 3a32 5d0a 2020 2020 2020 2020 290a  :r:2].        ).
+0000d490: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+0000d4a0: 222a 2020 2020 2020 2022 290a 2020 2020  "*       ").    
+0000d4b0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0000d4c0: 6765 2872 2c20 6e70 7473 293a 0a20 2020  ge(r, npts):.   
+0000d4d0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+0000d4e0: 2866 6f72 6d2e 666f 726d 6174 2874 5b6a  (form.format(t[j
+0000d4f0: 5d2c 2064 5b6a 5d29 290a 2020 2020 656c  ], d[j])).    el
+0000d500: 7365 3a0a 2020 2020 2020 2020 662e 7772  se:.        f.wr
+0000d510: 6974 6528 6622 7b74 6162 6c65 7374 723a  ite(f"{tablestr:
+0000d520: 3c38 737d 7b74 6964 3a38 647d 5c6e 2229  <8s}{tid:8d}\n")
+0000d530: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
+0000d540: 6e70 7473 202f 2f20 340a 2020 2020 2020  npts // 4.      
+0000d550: 2020 7220 3d20 726f 7773 202a 2034 0a20    r = rows * 4. 
+0000d560: 2020 2020 2020 2077 7269 7465 722e 7665         writer.ve
+0000d570: 6377 7269 7465 280a 2020 2020 2020 2020  cwrite(.        
+0000d580: 2020 2020 662c 0a20 2020 2020 2020 2020      f,.         
+0000d590: 2020 2022 2020 2020 2020 2020 2220 2b20     "        " + 
+0000d5a0: 666f 726d 202a 2034 202b 2022 5c6e 222c  form * 4 + "\n",
+0000d5b0: 0a20 2020 2020 2020 2020 2020 2074 5b3a  .            t[:
+0000d5c0: 723a 345d 2c0a 2020 2020 2020 2020 2020  r:4],.          
+0000d5d0: 2020 645b 3a72 3a34 5d2c 0a20 2020 2020    d[:r:4],.     
+0000d5e0: 2020 2020 2020 2074 5b31 3a72 3a34 5d2c         t[1:r:4],
+0000d5f0: 0a20 2020 2020 2020 2020 2020 2064 5b31  .            d[1
+0000d600: 3a72 3a34 5d2c 0a20 2020 2020 2020 2020  :r:4],.         
+0000d610: 2020 2074 5b32 3a72 3a34 5d2c 0a20 2020     t[2:r:4],.   
+0000d620: 2020 2020 2020 2020 2064 5b32 3a72 3a34           d[2:r:4
+0000d630: 5d2c 0a20 2020 2020 2020 2020 2020 2074  ],.            t
+0000d640: 5b33 3a72 3a34 5d2c 0a20 2020 2020 2020  [3:r:4],.       
+0000d650: 2020 2020 2064 5b33 3a72 3a34 5d2c 0a20       d[3:r:4],. 
+0000d660: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d670: 2066 2e77 7269 7465 2822 2020 2020 2020   f.write("      
+0000d680: 2020 2229 0a20 2020 2020 2020 2066 6f72    ").        for
+0000d690: 206a 2069 6e20 7261 6e67 6528 722c 206e   j in range(r, n
+0000d6a0: 7074 7329 3a0a 2020 2020 2020 2020 2020  pts):.          
+0000d6b0: 2020 662e 7772 6974 6528 666f 726d 2e66    f.write(form.f
+0000d6c0: 6f72 6d61 7428 745b 6a5d 2c20 645b 6a5d  ormat(t[j], d[j]
+0000d6d0: 2929 0a20 2020 2066 2e77 7269 7465 2822  )).    f.write("
+0000d6e0: 454e 4454 5c6e 2229 0a0a 0a64 6566 2062  ENDT\n")...def b
+0000d6f0: 756c 6b32 7573 6574 282a 6172 6773 293a  ulk2uset(*args):
+0000d700: 0a20 2020 2022 2222 0a20 2020 2052 6561  .    """.    Rea
+0000d710: 6420 434f 5244 322a 2061 6e64 2047 5249  d CORD2* and GRI
+0000d720: 4420 6361 7264 7320 6672 6f6d 2066 696c  D cards from fil
+0000d730: 6528 7329 2074 6f20 6d61 6b65 2061 2055  e(s) to make a U
+0000d740: 5345 5420 7461 626c 650a 0a20 2020 2050  SET table..    P
+0000d750: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+0000d760: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202a 6172  --------.    *ar
+0000d770: 6773 0a20 2020 2020 2020 2046 696c 6520  gs.        File 
+0000d780: 6e61 6d65 7320 6f72 2066 696c 6520 6861  names or file ha
+0000d790: 6e64 6c65 7320 6173 2072 6574 7572 6e65  ndles as returne
+0000d7a0: 6420 6279 203a 6675 6e63 3a60 6f70 656e  d by :func:`open
+0000d7b0: 602e 2046 696c 6573 0a20 2020 2020 2020  `. Files.       
+0000d7c0: 2072 6566 6572 7265 6420 746f 2062 7920   referred to by 
+0000d7d0: 6861 6e64 6c65 2061 7265 2072 6577 6f75  handle are rewou
+0000d7e0: 6e64 2066 6972 7374 2e20 4120 4755 4920  nd first. A GUI 
+0000d7f0: 6973 206f 7065 6e20 666f 720a 2020 2020  is open for.    
+0000d800: 2020 2020 6669 6c65 2073 656c 6563 7469      file selecti
+0000d810: 6f6e 2069 6620 6e6f 2061 7267 756d 656e  on if no argumen
+0000d820: 7473 2061 7265 2070 726f 7669 6465 6420  ts are provided 
+0000d830: 6f72 2069 6620 616e 2061 7267 756d 656e  or if an argumen
+0000d840: 740a 2020 2020 2020 2020 6973 2065 6974  t.        is eit
+0000d850: 6865 7220 6120 6469 7265 6374 6f72 7920  her a directory 
+0000d860: 6e61 6d65 206f 7220 4e6f 6e65 2e0a 0a20  name or None... 
+0000d870: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+0000d880: 2d2d 2d2d 2d2d 0a20 2020 2075 7365 7420  ------.    uset 
+0000d890: 3a20 7061 6e64 6173 2044 6174 6146 7261  : pandas DataFra
+0000d8a0: 6d65 0a20 2020 2020 2020 2041 2044 6174  me.        A Dat
+0000d8b0: 6146 7261 6d65 2061 7320 6f75 7470 7574  aFrame as output
+0000d8c0: 2062 790a 2020 2020 2020 2020 3a66 756e   by.        :fun
+0000d8d0: 633a 6070 7979 6574 692e 6e61 7374 7261  c:`pyyeti.nastra
+0000d8e0: 6e2e 6f70 322e 4f50 322e 7264 6e32 636f  n.op2.OP2.rdn2co
+0000d8f0: 7032 600a 2020 2020 636f 6f72 6472 6566  p2`.    coordref
+0000d900: 203a 2064 6963 7469 6f6e 6172 790a 2020   : dictionary.  
+0000d910: 2020 2020 2020 4469 6374 696f 6e61 7279        Dictionary
+0000d920: 2077 6974 6820 7468 6520 6b65 7973 2062   with the keys b
+0000d930: 6569 6e67 2074 6865 2063 6f6f 7264 696e  eing the coordin
+0000d940: 6174 6520 7379 7374 656d 2069 6420 616e  ate system id an
+0000d950: 640a 2020 2020 2020 2020 7468 6520 7661  d.        the va
+0000d960: 6c75 6573 2062 6569 6e67 2074 6865 2035  lues being the 5
+0000d970: 7833 206d 6174 7269 783a 3a0a 0a20 2020  x3 matrix::..   
+0000d980: 2020 2020 2020 2020 205b 6964 2020 7479           [id  ty
+0000d990: 7065 2030 5d20 2023 206f 7574 7075 7420  pe 0]  # output 
+0000d9a0: 636f 6f72 642e 2073 7973 2e20 6964 2061  coord. sys. id a
+0000d9b0: 6e64 2074 7970 650a 2020 2020 2020 2020  nd type.        
+0000d9c0: 2020 2020 5b78 6f20 2079 6f20 207a 6f5d      [xo  yo  zo]
+0000d9d0: 2020 2320 6f72 6967 696e 206f 6620 636f    # origin of co
+0000d9e0: 6f72 642e 2073 7973 7465 6d0a 2020 2020  ord. system.    
+0000d9f0: 2020 2020 2020 2020 5b20 2020 2054 2020          [    T  
+0000da00: 2020 205d 2020 2320 3378 3320 7472 616e     ]  # 3x3 tran
+0000da10: 7366 6f72 6d61 7469 6f6e 2074 6f20 6261  sformation to ba
+0000da20: 7369 630a 2020 2020 2020 2020 2020 2020  sic.            
+0000da30: 4e6f 7465 2074 6861 7420 5420 6973 2066  Note that T is f
+0000da40: 6f72 2074 6865 2063 6f6f 7264 696e 6174  or the coordinat
+0000da50: 6520 7379 7374 656d 2c20 6e6f 7420 6120  e system, not a 
+0000da60: 6772 6964 0a20 2020 2020 2020 2020 2020  grid.           
+0000da70: 2028 756e 6c65 7373 2074 7970 6520 3d20   (unless type = 
+0000da80: 3120 7768 6963 6820 6d65 616e 7320 7265  1 which means re
+0000da90: 6374 616e 6775 6c61 7229 0a0a 2020 2020  ctangular)..    
+0000daa0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+0000dab0: 2020 2020 5468 6973 2069 7320 7468 6520      This is the 
+0000dac0: 7265 7665 7273 6520 6f66 203a 6675 6e63  reverse of :func
+0000dad0: 3a60 7573 6574 3262 756c 6b60 2e0a 0a20  :`uset2bulk`... 
+0000dae0: 2020 204e 6f74 6520 7468 6174 203a 6675     Note that :fu
+0000daf0: 6e63 3a60 6173 6d32 7573 6574 6020 6973  nc:`asm2uset` is
+0000db00: 2073 696d 696c 6172 2074 6f20 7468 6973   similar to this
+0000db10: 2072 6f75 7469 6e65 2062 7574 2077 7269   routine but wri
+0000db20: 7474 656e 0a20 2020 2073 7065 6369 6669  tten.    specifi
+0000db30: 6361 6c6c 7920 666f 7220 4e61 7374 7261  cally for Nastra
+0000db40: 6e20 2e61 736d 2066 696c 6573 2e20 5468  n .asm files. Th
+0000db50: 6174 2072 6f75 7469 6e65 2077 696c 6c20  at routine will 
+0000db60: 7265 7475 726e 2061 0a20 2020 2055 5345  return a.    USE
+0000db70: 5420 7461 626c 6520 6f72 6465 7265 6420  T table ordered 
+0000db80: 746f 206d 6174 6368 2074 6865 206d 6f64  to match the mod
+0000db90: 656c 2028 6163 636f 7264 696e 6720 746f  el (according to
+0000dba0: 2074 6865 2053 4543 4f4e 4354 0a20 2020   the SECONCT.   
+0000dbb0: 2063 6172 6429 3b20 6974 2061 6c73 6f20   card); it also 
+0000dbc0: 7265 7475 726e 7320 6120 622d 7365 7420  returns a b-set 
+0000dbd0: 626f 6f6c 6561 6e20 7061 7274 6974 696f  boolean partitio
+0000dbe0: 6e20 7665 6374 6f72 2e0a 0a20 2020 2041  n vector...    A
+0000dbf0: 6c6c 2067 7269 6473 2061 7265 2070 7574  ll grids are put
+0000dc00: 2069 6e20 7468 6520 2762 2720 7365 742e   in the 'b' set.
+0000dc10: 2054 6869 7320 726f 7574 696e 6520 7573   This routine us
+0000dc20: 6573 0a20 2020 203a 6675 6e63 3a60 7079  es.    :func:`py
+0000dc30: 7965 7469 2e6e 6173 7472 616e 2e6e 3270  yeti.nastran.n2p
+0000dc40: 2e61 6464 6772 6964 6020 746f 2062 7569  .addgrid` to bui
+0000dc50: 6c64 2074 6865 206f 7574 7075 742e 0a0a  ld the output...
+0000dc60: 2020 2020 5365 6520 616c 736f 0a20 2020      See also.   
+0000dc70: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3a66   --------.    :f
+0000dc80: 756e 633a 6061 736d 3275 7365 7460 2c20  unc:`asm2uset`, 
+0000dc90: 3a66 756e 633a 6075 7365 7432 6275 6c6b  :func:`uset2bulk
+0000dca0: 602c 203a 6675 6e63 3a60 7264 6361 7264  `, :func:`rdcard
+0000dcb0: 7360 2c0a 2020 2020 3a66 756e 633a 6072  s`,.    :func:`r
+0000dcc0: 6467 7269 6473 602c 203a 6675 6e63 3a60  dgrids`, :func:`
+0000dcd0: 7079 7965 7469 2e6e 6173 7472 616e 2e6f  pyyeti.nastran.o
+0000dce0: 7032 2e4f 5032 2e72 646e 3263 6f70 3260  p2.OP2.rdn2cop2`
+0000dcf0: 2c0a 2020 2020 3a66 756e 633a 6070 7979  ,.    :func:`pyy
+0000dd00: 6574 692e 6e61 7374 7261 6e2e 6e32 702e  eti.nastran.n2p.
+0000dd10: 6164 6467 7269 6460 2c20 3a6d 6f64 3a60  addgrid`, :mod:`
+0000dd20: 7079 7965 7469 2e6e 6173 7472 616e 2e6e  pyyeti.nastran.n
+0000dd30: 3270 602e 0a20 2020 2022 2222 0a20 2020  2p`..    """.   
+0000dd40: 2067 7269 6473 203d 206e 702e 7a65 726f   grids = np.zero
+0000dd50: 7328 2830 2c20 3829 290a 2020 2020 636f  s((0, 8)).    co
+0000dd60: 6f72 6473 203d 207b 7d0a 0a20 2020 2069  ords = {}..    i
+0000dd70: 6620 6c65 6e28 6172 6773 2920 3d3d 2030  f len(args) == 0
+0000dd80: 3a0a 2020 2020 2020 2020 6172 6773 203d  :.        args =
+0000dd90: 205b 4e6f 6e65 5d0a 0a20 2020 2066 6f72   [None]..    for
+0000dda0: 2066 2069 6e20 6172 6773 3a0a 2020 2020   f in args:.    
+0000ddb0: 2020 2020 6620 3d20 6775 6974 6f6f 6c73      f = guitools
+0000ddc0: 2e67 6574 5f66 696c 655f 6e61 6d65 2866  .get_file_name(f
+0000ddd0: 2c20 7265 6164 3d54 7275 6529 0a20 2020  , read=True).   
+0000dde0: 2020 2020 2063 6f6f 7264 732e 7570 6461       coords.upda
+0000ddf0: 7465 2872 6463 6f72 6432 6361 7264 7328  te(rdcord2cards(
+0000de00: 6629 290a 2020 2020 2020 2020 6720 3d20  f)).        g = 
+0000de10: 7264 6772 6964 7328 6629 0a20 2020 2020  rdgrids(f).     
+0000de20: 2020 2069 6620 6720 6973 206e 6f74 204e     if g is not N
+0000de30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000de40: 2067 7269 6473 203d 206e 702e 7673 7461   grids = np.vsta
+0000de50: 636b 2828 6772 6964 732c 2067 2929 0a0a  ck((grids, g))..
+0000de60: 2020 2020 6920 3d20 6e70 2e61 7267 736f      i = np.argso
+0000de70: 7274 2867 7269 6473 5b3a 2c20 305d 290a  rt(grids[:, 0]).
+0000de80: 2020 2020 6772 6964 7320 3d20 6772 6964      grids = grid
+0000de90: 735b 692c 203a 5d0a 2020 2020 7573 6574  s[i, :].    uset
+0000dea0: 203d 206e 3270 2e61 6464 6772 6964 280a   = n2p.addgrid(.
+0000deb0: 2020 2020 2020 2020 4e6f 6e65 2c0a 2020          None,.  
+0000dec0: 2020 2020 2020 6772 6964 735b 3a2c 2030        grids[:, 0
+0000ded0: 5d2e 6173 7479 7065 286e 702e 696e 7436  ].astype(np.int6
+0000dee0: 3429 2c0a 2020 2020 2020 2020 2262 222c  4),.        "b",
+0000def0: 0a20 2020 2020 2020 2067 7269 6473 5b3a  .        grids[:
+0000df00: 2c20 315d 2c0a 2020 2020 2020 2020 6772  , 1],.        gr
+0000df10: 6964 735b 3a2c 2032 3a35 5d2c 0a20 2020  ids[:, 2:5],.   
+0000df20: 2020 2020 2067 7269 6473 5b3a 2c20 355d       grids[:, 5]
+0000df30: 2c0a 2020 2020 2020 2020 636f 6f72 6473  ,.        coords
+0000df40: 2c0a 2020 2020 290a 2020 2020 7265 7475  ,.    ).    retu
+0000df50: 726e 2075 7365 742c 2063 6f6f 7264 730a  rn uset, coords.
+0000df60: 0a0a 4067 7569 746f 6f6c 732e 7772 6974  ..@guitools.writ
+0000df70: 655f 7465 7874 5f66 696c 650a 6465 6620  e_text_file.def 
+0000df80: 7573 6574 3262 756c 6b28 662c 2075 7365  uset2bulk(f, use
+0000df90: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
+0000dfa0: 5772 6974 6520 434f 5244 322a 2061 6e64  Write CORD2* and
+0000dfb0: 2047 5249 4420 6361 7264 7320 6672 6f6d   GRID cards from
+0000dfc0: 2061 2055 5345 5420 7461 626c 650a 0a20   a USET table.. 
+0000dfd0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000dfe0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000dff0: 2066 203a 2073 7472 696e 6720 6f72 2066   f : string or f
+0000e000: 696c 655f 6c69 6b65 206f 7220 3120 6f72  ile_like or 1 or
+0000e010: 204e 6f6e 650a 2020 2020 2020 2020 4569   None.        Ei
+0000e020: 7468 6572 2061 206e 616d 6520 6f66 2061  ther a name of a
+0000e030: 2066 696c 652c 206f 7220 6973 2061 2066   file, or is a f
+0000e040: 696c 655f 6c69 6b65 206f 626a 6563 7420  ile_like object 
+0000e050: 6173 2072 6574 7572 6e65 640a 2020 2020  as returned.    
+0000e060: 2020 2020 6279 203a 6675 6e63 3a60 6f70      by :func:`op
+0000e070: 656e 6020 6f72 203a 636c 6173 733a 6069  en` or :class:`i
+0000e080: 6f2e 5374 7269 6e67 494f 602e 2049 6e70  o.StringIO`. Inp
+0000e090: 7574 2061 7320 696e 7465 6765 7220 3120  ut as integer 1 
+0000e0a0: 746f 0a20 2020 2020 2020 2077 7269 7465  to.        write
+0000e0b0: 2074 6f20 7374 646f 7574 2e20 4361 6e20   to stdout. Can 
+0000e0c0: 616c 736f 2062 6520 7468 6520 6e61 6d65  also be the name
+0000e0d0: 206f 6620 6120 6469 7265 6374 6f72 7920   of a directory 
+0000e0e0: 6f72 204e 6f6e 653b 0a20 2020 2020 2020  or None;.       
+0000e0f0: 2069 6e20 7468 6573 6520 6361 7365 732c   in these cases,
+0000e100: 2061 2047 5549 2069 7320 6f70 656e 6564   a GUI is opened
+0000e110: 2066 6f72 2066 696c 6520 7365 6c65 6374   for file select
+0000e120: 696f 6e2e 0a20 2020 2075 7365 7420 3a20  ion..    uset : 
+0000e130: 7061 6e64 6173 2044 6174 6146 7261 6d65  pandas DataFrame
+0000e140: 0a20 2020 2020 2020 2041 2044 6174 6146  .        A DataF
+0000e150: 7261 6d65 2061 7320 6f75 7470 7574 2062  rame as output b
+0000e160: 790a 2020 2020 2020 2020 3a66 756e 633a  y.        :func:
+0000e170: 6070 7979 6574 692e 6e61 7374 7261 6e2e  `pyyeti.nastran.
+0000e180: 6f70 322e 4f50 322e 7264 6e32 636f 7032  op2.OP2.rdn2cop2
+0000e190: 600a 0a20 2020 2052 6574 7572 6e73 0a20  `..    Returns. 
+0000e1a0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 204e     -------.    N
+0000e1b0: 6f6e 650a 0a20 2020 204e 6f74 6573 0a20  one..    Notes. 
+0000e1c0: 2020 202d 2d2d 2d2d 0a20 2020 2054 6869     -----.    Thi
+0000e1d0: 7320 6973 2074 6865 2072 6576 6572 7365  s is the reverse
+0000e1e0: 206f 6620 3a66 756e 633a 6062 756c 6b32   of :func:`bulk2
+0000e1f0: 7573 6574 602e 0a0a 2020 2020 5365 6520  uset`...    See 
+0000e200: 616c 736f 0a20 2020 202d 2d2d 2d2d 2d2d  also.    -------
+0000e210: 2d0a 2020 2020 3a66 756e 633a 6062 756c  -.    :func:`bul
+0000e220: 6b32 7573 6574 602c 203a 6675 6e63 3a60  k2uset`, :func:`
+0000e230: 7079 7965 7469 2e6e 6173 7472 616e 2e6e  pyyeti.nastran.n
+0000e240: 3270 2e6d 6b63 6f72 6463 6172 6469 6e66  2p.mkcordcardinf
+0000e250: 6f60 2c0a 2020 2020 3a66 756e 633a 6077  o`,.    :func:`w
+0000e260: 7463 6f6f 7264 6361 7264 7360 2c20 3a66  tcoordcards`, :f
+0000e270: 756e 633a 6077 7467 7269 6473 602e 0a20  unc:`wtgrids`.. 
+0000e280: 2020 2022 2222 0a0a 2020 2020 2320 4765     """..    # Ge
+0000e290: 7420 736f 6d65 2064 6174 6120 6672 6f6d  t some data from
+0000e2a0: 2074 6865 2075 7365 7420 7461 626c 653a   the uset table:
+0000e2b0: 0a20 2020 2063 6920 3d20 6e32 702e 6d6b  .    ci = n2p.mk
+0000e2c0: 636f 7264 6361 7264 696e 666f 2875 7365  cordcardinfo(use
+0000e2d0: 7429 0a20 2020 2067 7269 6473 203d 2075  t).    grids = u
+0000e2e0: 7365 742e 696e 6465 782e 6765 745f 6c65  set.index.get_le
+0000e2f0: 7665 6c5f 7661 6c75 6573 2822 6964 2229  vel_values("id")
+0000e300: 0a20 2020 2064 6f66 203d 2075 7365 742e  .    dof = uset.
+0000e310: 696e 6465 782e 6765 745f 6c65 7665 6c5f  index.get_level_
+0000e320: 7661 6c75 6573 2822 646f 6622 290a 2020  values("dof").  
+0000e330: 2020 7076 203d 2064 6f66 203d 3d20 310a    pv = dof == 1.
+0000e340: 2020 2020 6772 6964 7320 3d20 6772 6964      grids = grid
+0000e350: 735b 7076 5d0a 2020 2020 7879 7a20 3d20  s[pv].    xyz = 
+0000e360: 7573 6574 2e6c 6f63 5b70 762c 2022 7822  uset.loc[pv, "x"
+0000e370: 3a22 7a22 5d2e 7661 6c75 6573 0a20 2020  :"z"].values.   
+0000e380: 2070 7620 3d20 646f 6620 3d3d 2032 0a20   pv = dof == 2. 
+0000e390: 2020 2063 6420 3d20 7573 6574 2e6c 6f63     cd = uset.loc
+0000e3a0: 5b70 762c 2022 7822 5d2e 7661 6c75 6573  [pv, "x"].values
+0000e3b0: 2e61 7374 7970 6528 696e 7429 0a0a 2020  .astype(int)..  
+0000e3c0: 2020 2320 5772 6974 6520 636f 6f72 6469    # Write coordi
+0000e3d0: 6e61 7465 2073 7973 7465 6d20 6361 7264  nate system card
+0000e3e0: 7320 6966 206e 6565 6465 643a 0a20 2020  s if needed:.   
+0000e3f0: 2069 6620 6369 3a0a 2020 2020 2020 2020   if ci:.        
+0000e400: 662e 7772 6974 6528 2224 5c6e 2420 434f  f.write("$\n$ CO
+0000e410: 4f52 4449 4e41 5445 2053 5953 5445 4d20  ORDINATE SYSTEM 
+0000e420: 4441 5441 5c6e 245c 6e22 290a 2020 2020  DATA\n$\n").    
+0000e430: 2020 2020 7774 636f 6f72 6463 6172 6473      wtcoordcards
+0000e440: 2866 2c20 6369 290a 0a20 2020 2023 2057  (f, ci)..    # W
+0000e450: 7269 7465 2047 7269 6420 6461 7461 3a0a  rite Grid data:.
+0000e460: 2020 2020 662e 7772 6974 6528 2224 5c6e      f.write("$\n
+0000e470: 2420 4752 4944 2044 4154 415c 6e24 5c6e  $ GRID DATA\n$\n
+0000e480: 2229 0a20 2020 2077 7467 7269 6473 2866  ").    wtgrids(f
+0000e490: 2c20 6772 6964 732c 2030 2c20 7879 7a2c  , grids, 0, xyz,
+0000e4a0: 2063 6429 0a0a 0a64 6566 2072 6473 706f   cd)...def rdspo
+0000e4b0: 696e 7473 2866 293a 0a20 2020 2072 2222  ints(f):.    r""
+0000e4c0: 220a 2020 2020 5265 6164 204e 6173 7472  ".    Read Nastr
+0000e4d0: 616e 2053 504f 494e 5420 6361 7264 7320  an SPOINT cards 
+0000e4e0: 6672 6f6d 2061 204e 6173 7472 616e 2062  from a Nastran b
+0000e4f0: 756c 6b20 6669 6c65 2e0a 0a20 2020 2050  ulk file...    P
+0000e500: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+0000e510: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 203a  --------.    f :
+0000e520: 2073 7472 696e 6720 6f72 2066 696c 655f   string or file_
+0000e530: 6c69 6b65 206f 7220 4e6f 6e65 0a20 2020  like or None.   
+0000e540: 2020 2020 2045 6974 6865 7220 6120 6e61       Either a na
+0000e550: 6d65 206f 6620 6120 6669 6c65 2c20 6f72  me of a file, or
+0000e560: 2069 7320 6120 6669 6c65 5f6c 696b 6520   is a file_like 
+0000e570: 6f62 6a65 6374 2061 7320 7265 7475 726e  object as return
+0000e580: 6564 0a20 2020 2020 2020 2062 7920 3a66  ed.        by :f
+0000e590: 756e 633a 606f 7065 6e60 2e20 4966 2066  unc:`open`. If f
+0000e5a0: 696c 655f 6c69 6b65 206f 626a 6563 742c  ile_like object,
+0000e5b0: 2069 7420 6973 2072 6577 6f75 6e64 2066   it is rewound f
+0000e5c0: 6972 7374 2e20 4361 6e0a 2020 2020 2020  irst. Can.      
+0000e5d0: 2020 616c 736f 2062 6520 7468 6520 6e61    also be the na
+0000e5e0: 6d65 206f 6620 6120 6469 7265 6374 6f72  me of a director
+0000e5f0: 7920 6f72 204e 6f6e 653b 2069 6e20 7468  y or None; in th
+0000e600: 6573 6520 6361 7365 732c 2061 2047 5549  ese cases, a GUI
+0000e610: 0a20 2020 2020 2020 2069 7320 6f70 656e  .        is open
+0000e620: 6564 2066 6f72 2066 696c 6520 7365 6c65  ed for file sele
+0000e630: 6374 696f 6e2e 0a0a 2020 2020 5265 7475  ction...    Retu
+0000e640: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0000e650: 2020 2020 7370 6f69 6e74 7320 3a20 3164      spoints : 1d
+0000e660: 206e 6461 7272 6179 0a20 2020 2020 2020   ndarray.       
+0000e670: 2041 7272 6179 206f 6620 5350 4f49 4e54   Array of SPOINT
+0000e680: 2069 6473 2e20 5769 6c6c 2062 6520 656d   ids. Will be em
+0000e690: 7074 7920 6966 206e 6f20 5350 4f49 4e54  pty if no SPOINT
+0000e6a0: 2063 6172 6473 2066 6f75 6e64 2e0a 0a20   cards found... 
+0000e6b0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+0000e6c0: 2d2d 0a20 2020 2054 6869 7320 726f 7574  --.    This rout
+0000e6d0: 696e 6520 7573 6573 203a 6675 6e63 3a60  ine uses :func:`
+0000e6e0: 7264 6361 7264 7360 2074 6f20 6c6f 6164  rdcards` to load
+0000e6f0: 2074 6865 2064 6174 612e 0a0a 2020 2020   the data...    
+0000e700: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
+0000e710: 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20 6672  -----.    >>> fr
+0000e720: 6f6d 2070 7979 6574 6920 696d 706f 7274  om pyyeti import
+0000e730: 206e 6173 7472 616e 0a20 2020 203e 3e3e   nastran.    >>>
+0000e740: 2066 726f 6d20 696f 2069 6d70 6f72 7420   from io import 
+0000e750: 5374 7269 6e67 494f 0a20 2020 203e 3e3e  StringIO.    >>>
+0000e760: 2062 756c 6b64 6174 6120 3d20 280a 2020   bulkdata = (.  
+0000e770: 2020 2e2e 2e20 2020 2020 2253 504f 494e    ...     "SPOIN
+0000e780: 542c 312c 322c 3130 305c 6e22 0a20 2020  T,1,2,100\n".   
+0000e790: 202e 2e2e 2020 2020 2022 5350 4f49 4e54   ...     "SPOINT
+0000e7a0: 2c32 3030 2c54 4852 552c 3230 325c 6e22  ,200,THRU,202\n"
+0000e7b0: 0a20 2020 202e 2e2e 2020 2020 2022 5350  .    ...     "SP
+0000e7c0: 4f49 4e54 2c35 5c6e 220a 2020 2020 2e2e  OINT,5\n".    ..
+0000e7d0: 2e20 290a 2020 2020 3e3e 3e20 7769 7468  . ).    >>> with
+0000e7e0: 2053 7472 696e 6749 4f28 6275 6c6b 6461   StringIO(bulkda
+0000e7f0: 7461 2920 6173 2066 3a0a 2020 2020 2e2e  ta) as f:.    ..
+0000e800: 2e20 2020 2020 7370 6f69 6e74 7320 3d20  .     spoints = 
+0000e810: 6e61 7374 7261 6e2e 7264 7370 6f69 6e74  nastran.rdspoint
+0000e820: 7328 6629 0a20 2020 203e 3e3e 2073 706f  s(f).    >>> spo
+0000e830: 696e 7473 2020 2020 2020 2020 2020 2020  ints            
+0000e840: 2020 2020 2020 2020 2020 2320 646f 6374            # doct
+0000e850: 6573 743a 202b 454c 4c49 5053 4953 0a20  est: +ELLIPSIS. 
+0000e860: 2020 2061 7272 6179 285b 2020 312c 2020     array([  1,  
+0000e870: 2032 2c20 3130 302c 2032 3030 2c20 3230   2, 100, 200, 20
+0000e880: 312c 2032 3032 2c20 2020 355d 2e2e 2e29  1, 202,   5]...)
+0000e890: 0a20 2020 203e 3e3e 2077 6974 6820 5374  .    >>> with St
+0000e8a0: 7269 6e67 494f 2822 6e6f 2064 6174 6122  ringIO("no data"
+0000e8b0: 2920 6173 2066 3a0a 2020 2020 2e2e 2e20  ) as f:.    ... 
+0000e8c0: 2020 2020 7370 6f69 6e74 7320 3d20 6e61      spoints = na
+0000e8d0: 7374 7261 6e2e 7264 7370 6f69 6e74 7328  stran.rdspoints(
+0000e8e0: 6629 0a20 2020 203e 3e3e 2073 706f 696e  f).    >>> spoin
+0000e8f0: 7473 2020 2020 2020 2020 2020 2020 2020  ts              
+0000e900: 2020 2020 2020 2020 2320 646f 6374 6573          # doctes
+0000e910: 743a 202b 454c 4c49 5053 4953 0a20 2020  t: +ELLIPSIS.   
+0000e920: 2061 7272 6179 285b 5d2e 2e2e 290a 0a20   array([]...).. 
+0000e930: 2020 2022 2222 0a20 2020 2073 706f 696e     """.    spoin
+0000e940: 745f 6461 7461 203d 2072 6463 6172 6473  t_data = rdcards
+0000e950: 2866 2c20 2273 706f 696e 7422 2c20 7265  (f, "spoint", re
+0000e960: 7475 726e 5f76 6172 3d22 6c69 7374 2229  turn_var="list")
+0000e970: 0a20 2020 2073 706f 696e 7473 203d 205b  .    spoints = [
+0000e980: 5d0a 2020 2020 6966 2073 706f 696e 745f  ].    if spoint_
+0000e990: 6461 7461 2069 7320 6e6f 7420 4e6f 6e65  data is not None
+0000e9a0: 3a0a 2020 2020 2020 2020 666f 7220 6361  :.        for ca
+0000e9b0: 7264 2069 6e20 7370 6f69 6e74 5f64 6174  rd in spoint_dat
+0000e9c0: 613a 0a20 2020 2020 2020 2020 2020 2069  a:.            i
+0000e9d0: 6620 6c65 6e28 6361 7264 2920 3e20 3220  f len(card) > 2 
+0000e9e0: 616e 6420 6973 696e 7374 616e 6365 2863  and isinstance(c
+0000e9f0: 6172 645b 315d 2c20 7374 7229 2061 6e64  ard[1], str) and
+0000ea00: 2063 6172 645b 315d 2e6c 6f77 6572 2829   card[1].lower()
+0000ea10: 203d 3d20 2274 6872 7522 3a0a 2020 2020   == "thru":.    
+0000ea20: 2020 2020 2020 2020 2020 2020 7370 6f69              spoi
+0000ea30: 6e74 732e 6578 7465 6e64 285b 6920 666f  nts.extend([i fo
+0000ea40: 7220 6920 696e 2072 616e 6765 2863 6172  r i in range(car
+0000ea50: 645b 305d 2c20 6361 7264 5b32 5d20 2b20  d[0], card[2] + 
+0000ea60: 3129 5d29 0a20 2020 2020 2020 2020 2020  1)]).           
+0000ea70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000ea80: 2020 2020 2020 2073 706f 696e 7473 2e65         spoints.e
+0000ea90: 7874 656e 6428 6361 7264 290a 2020 2020  xtend(card).    
+0000eaa0: 7265 7475 726e 206e 702e 6172 7261 7928  return np.array(
+0000eab0: 7370 6f69 6e74 732c 2064 7479 7065 3d6e  spoints, dtype=n
+0000eac0: 702e 696e 7436 3429 0a0a 0a64 6566 2072  p.int64)...def r
+0000ead0: 6473 6563 6f6e 6374 2866 293a 0a20 2020  dseconct(f):.   
+0000eae0: 2072 2222 220a 2020 2020 5265 6164 204e   r""".    Read N
+0000eaf0: 6173 7472 616e 2053 4543 4f4e 4354 2063  astran SECONCT c
+0000eb00: 6172 6473 2066 726f 6d20 6120 4e61 7374  ards from a Nast
+0000eb10: 7261 6e20 6275 6c6b 2066 696c 652e 0a0a  ran bulk file...
+0000eb20: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000eb30: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000eb40: 2020 6620 3a20 7374 7269 6e67 206f 7220    f : string or 
+0000eb50: 6669 6c65 5f6c 696b 6520 6f72 204e 6f6e  file_like or Non
+0000eb60: 650a 2020 2020 2020 2020 4569 7468 6572  e.        Either
+0000eb70: 2061 206e 616d 6520 6f66 2061 2066 696c   a name of a fil
+0000eb80: 652c 206f 7220 6973 2061 2066 696c 655f  e, or is a file_
+0000eb90: 6c69 6b65 206f 626a 6563 7420 6173 2072  like object as r
+0000eba0: 6574 7572 6e65 640a 2020 2020 2020 2020  eturned.        
+0000ebb0: 6279 203a 6675 6e63 3a60 6f70 656e 602e  by :func:`open`.
+0000ebc0: 2049 6620 6669 6c65 5f6c 696b 6520 6f62   If file_like ob
+0000ebd0: 6a65 6374 2c20 6974 2069 7320 7265 776f  ject, it is rewo
+0000ebe0: 756e 6420 6669 7273 742e 2043 616e 0a20  und first. Can. 
+0000ebf0: 2020 2020 2020 2061 6c73 6f20 6265 2074         also be t
+0000ec00: 6865 206e 616d 6520 6f66 2061 2064 6972  he name of a dir
+0000ec10: 6563 746f 7279 206f 7220 4e6f 6e65 3b20  ectory or None; 
+0000ec20: 696e 2074 6865 7365 2063 6173 6573 2c20  in these cases, 
+0000ec30: 6120 4755 490a 2020 2020 2020 2020 6973  a GUI.        is
+0000ec40: 206f 7065 6e65 6420 666f 7220 6669 6c65   opened for file
+0000ec50: 2073 656c 6563 7469 6f6e 2e0a 0a20 2020   selection...   
+0000ec60: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+0000ec70: 2d2d 2d2d 0a20 2020 2061 5f69 6473 2c20  ----.    a_ids, 
+0000ec80: 625f 6964 7320 3a20 3164 206e 6461 7272  b_ids : 1d ndarr
+0000ec90: 6179 730a 2020 2020 2020 2020 4172 7261  ays.        Arra
+0000eca0: 7920 6f66 2047 5249 4420 616e 6420 5350  y of GRID and SP
+0000ecb0: 4f49 4e54 2069 6473 2066 6f72 2073 7570  OINT ids for sup
+0000ecc0: 6572 656c 656d 656e 7420 4120 616e 640a  erelement A and.
+0000ecd0: 2020 2020 2020 2020 7375 7065 7265 6c65          superele
+0000ece0: 6d65 6e74 2042 2c20 7265 7370 6563 7469  ment B, respecti
+0000ecf0: 7665 6c79 2e20 426f 7468 206f 7574 7075  vely. Both outpu
+0000ed00: 7473 2077 696c 6c20 6265 2065 6d70 7479  ts will be empty
+0000ed10: 2069 6620 6e6f 0a20 2020 2020 2020 2053   if no.        S
+0000ed20: 4543 4f4e 4354 2063 6172 6473 2066 6f75  ECONCT cards fou
+0000ed30: 6e64 2e0a 0a20 2020 204e 6f74 6573 0a20  nd...    Notes. 
+0000ed40: 2020 202d 2d2d 2d2d 0a20 2020 2054 6869     -----.    Thi
+0000ed50: 7320 726f 7574 696e 6520 7573 6573 203a  s routine uses :
+0000ed60: 6675 6e63 3a60 7264 6361 7264 7360 2074  func:`rdcards` t
+0000ed70: 6f20 6c6f 6164 2074 6865 2064 6174 612e  o load the data.
+0000ed80: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
+0000ed90: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+0000eda0: 3e3e 3e20 6672 6f6d 2069 6f20 696d 706f  >>> from io impo
+0000edb0: 7274 2053 7472 696e 6749 4f0a 2020 2020  rt StringIO.    
+0000edc0: 3e3e 3e20 6672 6f6d 2070 7979 6574 6920  >>> from pyyeti 
+0000edd0: 696d 706f 7274 206e 6173 7472 616e 0a20  import nastran. 
+0000ede0: 2020 203e 3e3e 2062 756c 6b64 6174 6120     >>> bulkdata 
+0000edf0: 3d20 280a 2020 2020 2e2e 2e20 2020 2020  = (.    ...     
+0000ee00: 2253 4543 4f4e 4354 2c31 3031 2c30 2c2c  "SECONCT,101,0,,
+0000ee10: 4e4f 5c6e 220a 2020 2020 2e2e 2e20 2020  NO\n".    ...   
+0000ee20: 2020 222c 332c 3330 2c31 312c 3131 302c    ",3,30,11,110,
+0000ee30: 3139 2c31 3930 2c32 372c 3237 305c 6e22  19,190,27,270\n"
+0000ee40: 0a20 2020 202e 2e2e 2020 2020 2022 245c  .    ...     "$\
+0000ee50: 6e22 0a20 2020 202e 2e2e 2020 2020 2022  n".    ...     "
+0000ee60: 5345 434f 4e43 542c 3130 312c 302c 2c4e  SECONCT,101,0,,N
+0000ee70: 4f5c 6e22 0a20 2020 202e 2e2e 2020 2020  O\n".    ...    
+0000ee80: 2022 2c31 3130 312c 5448 5255 2c31 3130   ",1101,THRU,110
+0000ee90: 342c 3231 3031 2c54 4852 552c 3231 3034  4,2101,THRU,2104
+0000eea0: 5c6e 220a 2020 2020 2e2e 2e20 290a 2020  \n".    ... ).  
+0000eeb0: 2020 3e3e 3e20 7769 7468 2053 7472 696e    >>> with Strin
+0000eec0: 6749 4f28 6275 6c6b 6461 7461 2920 6173  gIO(bulkdata) as
+0000eed0: 2066 3a0a 2020 2020 2e2e 2e20 2020 2020   f:.    ...     
+0000eee0: 615f 6964 732c 2062 5f69 6473 203d 206e  a_ids, b_ids = n
+0000eef0: 6173 7472 616e 2e72 6473 6563 6f6e 6374  astran.rdseconct
+0000ef00: 2866 290a 2020 2020 3e3e 3e20 615f 6964  (f).    >>> a_id
+0000ef10: 7320 2020 2020 2020 2020 2020 2020 2020  s               
+0000ef20: 2020 2020 2020 2023 2064 6f63 7465 7374         # doctest
+0000ef30: 3a20 2b45 4c4c 4950 5349 530a 2020 2020  : +ELLIPSIS.    
+0000ef40: 6172 7261 7928 5b20 2020 332c 2020 2031  array([   3,   1
+0000ef50: 312c 2020 2031 392c 2020 2032 372c 2031  1,   19,   27, 1
+0000ef60: 3130 312c 2031 3130 322c 2031 3130 332c  101, 1102, 1103,
+0000ef70: 2031 3130 345d 2e2e 2e29 0a20 2020 203e   1104]...).    >
+0000ef80: 3e3e 2062 5f69 6473 2020 2020 2020 2020  >> b_ids        
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000efa0: 646f 6374 6573 743a 202b 454c 4c49 5053  doctest: +ELLIPS
+0000efb0: 4953 0a20 2020 2061 7272 6179 285b 2020  IS.    array([  
+0000efc0: 3330 2c20 2031 3130 2c20 2031 3930 2c20  30,  110,  190, 
+0000efd0: 2032 3730 2c20 3231 3031 2c20 3231 3032   270, 2101, 2102
+0000efe0: 2c20 3231 3033 2c20 3231 3034 5d2e 2e2e  , 2103, 2104]...
+0000eff0: 290a 2020 2020 2222 220a 0a20 2020 2064  ).    """..    d
+0000f000: 6566 205f 6765 745f 7061 6972 7328 6361  ef _get_pairs(ca
+0000f010: 7264 293a 0a20 2020 2020 2020 2023 2074  rd):.        # t
+0000f020: 7275 6e63 6174 6520 616e 6420 6669 6c74  runcate and filt
+0000f030: 6572 206f 7574 2062 6c61 6e6b 733a 0a20  er out blanks:. 
+0000f040: 2020 2020 2020 2063 6172 6420 3d20 5b69         card = [i
+0000f050: 2066 6f72 2069 2069 6e20 6361 7264 5b38   for i in card[8
+0000f060: 3a5d 2069 6620 695d 0a20 2020 2020 2020  :] if i].       
+0000f070: 2069 7420 3d20 6974 6572 2863 6172 6429   it = iter(card)
+0000f080: 0a20 2020 2020 2020 2066 6f72 2061 2c20  .        for a, 
+0000f090: 6220 696e 207a 6970 2869 742c 2069 7429  b in zip(it, it)
+0000f0a0: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
+0000f0b0: 656c 6420 612c 2062 0a0a 2020 2020 7365  eld a, b..    se
+0000f0c0: 636f 6e63 745f 6461 7461 203d 2072 6463  conct_data = rdc
+0000f0d0: 6172 6473 2866 2c20 2273 6563 6f6e 6374  ards(f, "seconct
+0000f0e0: 222c 2072 6574 7572 6e5f 7661 723d 226c  ", return_var="l
+0000f0f0: 6973 7422 290a 2020 2020 615f 6964 7320  ist").    a_ids 
+0000f100: 3d20 5b5d 0a20 2020 2062 5f69 6473 203d  = [].    b_ids =
+0000f110: 205b 5d0a 2020 2020 6966 2073 6563 6f6e   [].    if secon
+0000f120: 6374 5f64 6174 6120 6973 206e 6f74 204e  ct_data is not N
+0000f130: 6f6e 653a 0a20 2020 2020 2020 2066 6f72  one:.        for
+0000f140: 2063 6172 6420 696e 2073 6563 6f6e 6374   card in seconct
+0000f150: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
+0000f160: 2020 2069 7420 3d20 6974 6572 285f 6765     it = iter(_ge
+0000f170: 745f 7061 6972 7328 6361 7264 2929 0a20  t_pairs(card)). 
+0000f180: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
+0000f190: 2c20 6220 696e 2069 743a 0a20 2020 2020  , b in it:.     
+0000f1a0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000f1b0: 696e 7374 616e 6365 2862 2c20 7374 7229  instance(b, str)
+0000f1c0: 3a20 2023 2069 7420 6d75 7374 2062 6520  :  # it must be 
+0000f1d0: 2254 4852 5522 0a20 2020 2020 2020 2020  "THRU".         
+0000f1e0: 2020 2020 2020 2020 2020 2023 2042 5441             # BTA
+0000f1f0: 2073 6179 7320 4927 6d20 6120 6a65 726b   says I'm a jerk
+0000f200: 2069 6620 4920 646f 6e27 7420 6368 6563   if I don't chec
+0000f210: 6b20 666f 7220 2254 4852 5522 203a 290a  k for "THRU" :).
+0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f230: 2020 2020 6132 2c20 6231 203d 206e 6578      a2, b1 = nex
+0000f240: 7428 6974 290a 2020 2020 2020 2020 2020  t(it).          
+0000f250: 2020 2020 2020 2020 2020 7468 7275 2c20            thru, 
+0000f260: 6232 203d 206e 6578 7428 6974 290a 2020  b2 = next(it).  
+0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f280: 2020 615f 6964 732e 6578 7465 6e64 285b    a_ids.extend([
+0000f290: 6920 666f 7220 6920 696e 2072 616e 6765  i for i in range
+0000f2a0: 2861 2c20 6132 202b 2031 295d 290a 2020  (a, a2 + 1)]).  
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 2020 625f 6964 732e 6578 7465 6e64 285b    b_ids.extend([
+0000f2d0: 6920 666f 7220 6920 696e 2072 616e 6765  i for i in range
+0000f2e0: 2862 312c 2062 3220 2b20 3129 5d29 0a20  (b1, b2 + 1)]). 
+0000f2f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000f300: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000f310: 2020 2020 2020 2020 2061 5f69 6473 2e61           a_ids.a
+0000f320: 7070 656e 6428 6129 0a20 2020 2020 2020  ppend(a).       
+0000f330: 2020 2020 2020 2020 2020 2020 2062 5f69               b_i
+0000f340: 6473 2e61 7070 656e 6428 6229 0a20 2020  ds.append(b).   
+0000f350: 2072 6574 7572 6e20 6e70 2e61 7272 6179   return np.array
+0000f360: 2861 5f69 6473 2c20 6474 7970 653d 6e70  (a_ids, dtype=np
+0000f370: 2e69 6e74 3634 292c 206e 702e 6172 7261  .int64), np.arra
+0000f380: 7928 625f 6964 732c 2064 7479 7065 3d6e  y(b_ids, dtype=n
+0000f390: 702e 696e 7436 3429 0a0a 0a40 6775 6974  p.int64)...@guit
+0000f3a0: 6f6f 6c73 2e72 6561 645f 7465 7874 5f66  ools.read_text_f
+0000f3b0: 696c 650a 6465 6620 6173 6d32 7573 6574  ile.def asm2uset
+0000f3c0: 2866 2c20 7472 795f 7264 6578 7472 6e3d  (f, try_rdextrn=
+0000f3d0: 5472 7565 293a 0a20 2020 2072 2222 220a  True):.    r""".
+0000f3e0: 2020 2020 5265 6164 2043 4f52 4432 2a20      Read CORD2* 
+0000f3f0: 616e 6420 4752 4944 2063 6172 6473 2066  and GRID cards f
+0000f400: 726f 6d20 6120 222e 6173 6d22 2066 696c  rom a ".asm" fil
+0000f410: 6520 746f 206d 616b 6520 6120 5553 4554  e to make a USET
+0000f420: 2074 6162 6c65 0a0a 2020 2020 5061 7261   table..    Para
+0000f430: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0000f440: 2d2d 2d2d 2d0a 2020 2020 6620 3a20 7374  -----.    f : st
+0000f450: 7269 6e67 206f 7220 6669 6c65 5f6c 696b  ring or file_lik
+0000f460: 6520 6f72 204e 6f6e 650a 2020 2020 2020  e or None.      
+0000f470: 2020 4569 7468 6572 2061 206e 616d 6520    Either a name 
+0000f480: 6f66 2061 2066 696c 652c 206f 7220 6973  of a file, or is
+0000f490: 2061 2066 696c 655f 6c69 6b65 206f 626a   a file_like obj
+0000f4a0: 6563 7420 6173 2072 6574 7572 6e65 640a  ect as returned.
+0000f4b0: 2020 2020 2020 2020 6279 203a 6675 6e63          by :func
+0000f4c0: 3a60 6f70 656e 602e 2049 6620 6669 6c65  :`open`. If file
+0000f4d0: 5f6c 696b 6520 6f62 6a65 6374 2c20 6974  _like object, it
+0000f4e0: 2069 7320 7265 776f 756e 6420 6669 7273   is rewound firs
+0000f4f0: 742e 2043 616e 0a20 2020 2020 2020 2061  t. Can.        a
+0000f500: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
+0000f510: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
+0000f520: 7220 4e6f 6e65 3b20 696e 2074 6865 7365  r None; in these
+0000f530: 2063 6173 6573 2c20 6120 4755 490a 2020   cases, a GUI.  
+0000f540: 2020 2020 2020 6973 206f 7065 6e65 6420        is opened 
+0000f550: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
+0000f560: 6f6e 2e0a 2020 2020 7472 795f 7264 6578  on..    try_rdex
+0000f570: 7472 6e20 3a20 626f 6f6c 3b20 6f70 7469  trn : bool; opti
+0000f580: 6f6e 616c 0a20 2020 2020 2020 2049 6620  onal.        If 
+0000f590: 5472 7565 2c20 726f 7574 696e 6520 7769  True, routine wi
+0000f5a0: 6c6c 2061 7474 656d 7074 2074 6f20 7265  ll attempt to re
+0000f5b0: 6164 2074 6865 2022 4558 5452 4e22 2063  ad the "EXTRN" c
+0000f5c0: 6172 6420 6672 6f6d 0a20 2020 2020 2020  ard from.       
+0000f5d0: 2074 6865 2022 2e70 6368 2220 6669 6c65   the ".pch" file
+0000f5e0: 2e20 4966 2061 2066 696c 656e 616d 6520  . If a filename 
+0000f5f0: 6361 6e6e 6f74 2062 6520 6465 7465 726d  cannot be determ
+0000f600: 696e 6564 2066 726f 6d20 6066 602c 0a20  ined from `f`,. 
+0000f610: 2020 2020 2020 2074 6865 2061 7474 656d         the attem
+0000f620: 7074 2074 6f20 7468 6520 2245 5854 524e  pt to the "EXTRN
+0000f630: 2220 6361 7264 2069 7320 7175 6965 746c  " card is quietl
+0000f640: 7920 736b 6970 7065 6420 616e 6420 6561  y skipped and ea
+0000f650: 6368 0a20 2020 2020 2020 2062 2d73 6574  ch.        b-set
+0000f660: 206e 6f64 6520 6973 2061 7373 756d 6564   node is assumed
+0000f670: 2074 6f20 6861 7665 2061 6c6c 2036 2044   to have all 6 D
+0000f680: 4f46 2e20 5365 6520 4e6f 7465 7320 6265  OF. See Notes be
+0000f690: 6c6f 772e 0a0a 2020 2020 5265 7475 726e  low...    Return
+0000f6a0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+0000f6b0: 2020 7573 6574 203a 2070 616e 6461 7320    uset : pandas 
+0000f6c0: 4461 7461 4672 616d 650a 2020 2020 2020  DataFrame.      
+0000f6d0: 2020 4120 4461 7461 4672 616d 6520 6173    A DataFrame as
+0000f6e0: 206f 7574 7075 7420 6279 0a20 2020 2020   output by.     
+0000f6f0: 2020 203a 6675 6e63 3a60 7079 7965 7469     :func:`pyyeti
+0000f700: 2e6e 6173 7472 616e 2e6f 7032 2e4f 5032  .nastran.op2.OP2
+0000f710: 2e72 646e 3263 6f70 3260 2e20 436f 6e74  .rdn2cop2`. Cont
+0000f720: 6169 6e73 2061 6c6c 2047 5249 4420 616e  ains all GRID an
+0000f730: 640a 2020 2020 2020 2020 5350 4f49 4e54  d.        SPOINT
+0000f740: 2044 4f46 2069 6e20 7468 6520 2e61 736d   DOF in the .asm
+0000f750: 2066 696c 6520 696e 2074 6865 206f 7264   file in the ord
+0000f760: 6572 2073 7065 6369 6669 6564 206f 6e20  er specified on 
+0000f770: 7468 650a 2020 2020 2020 2020 5345 434f  the.        SECO
+0000f780: 4e43 5420 6361 7264 2e20 5468 6973 2069  NCT card. This i
+0000f790: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
+0000f7a0: 6820 7468 6520 6d6f 6465 6c20 6d61 7472  h the model matr
+0000f7b0: 6963 6573 2028 6567 2c0a 2020 2020 2020  ices (eg,.      
+0000f7c0: 2020 696e 2074 6865 202e 6f70 3420 6669    in the .op4 fi
+0000f7d0: 6c65 292e 0a20 2020 2063 6f6f 7264 7265  le)..    coordre
+0000f7e0: 6620 3a20 6469 6374 696f 6e61 7279 0a20  f : dictionary. 
+0000f7f0: 2020 2020 2020 2044 6963 7469 6f6e 6172         Dictionar
+0000f800: 7920 7769 7468 2074 6865 206b 6579 7320  y with the keys 
+0000f810: 6265 696e 6720 7468 6520 636f 6f72 6469  being the coordi
+0000f820: 6e61 7465 2073 7973 7465 6d20 6964 2061  nate system id a
+0000f830: 6e64 0a20 2020 2020 2020 2074 6865 2076  nd.        the v
+0000f840: 616c 7565 7320 6265 696e 6720 7468 6520  alues being the 
+0000f850: 3578 3320 6d61 7472 6978 3a3a 0a0a 2020  5x3 matrix::..  
+0000f860: 2020 2020 2020 2020 2020 5b69 6420 2074            [id  t
+0000f870: 7970 6520 305d 2020 2320 6f75 7470 7574  ype 0]  # output
+0000f880: 2063 6f6f 7264 2e20 7379 732e 2069 6420   coord. sys. id 
+0000f890: 616e 6420 7479 7065 0a20 2020 2020 2020  and type.       
+0000f8a0: 2020 2020 205b 786f 2020 796f 2020 7a6f       [xo  yo  zo
+0000f8b0: 5d20 2023 206f 7269 6769 6e20 6f66 2063  ]  # origin of c
+0000f8c0: 6f6f 7264 2e20 7379 7374 656d 0a20 2020  oord. system.   
+0000f8d0: 2020 2020 2020 2020 205b 2020 2020 5420           [    T 
+0000f8e0: 2020 2020 5d20 2023 2033 7833 2074 7261      ]  # 3x3 tra
+0000f8f0: 6e73 666f 726d 6174 696f 6e20 746f 2062  nsformation to b
+0000f900: 6173 6963 0a20 2020 2020 2020 2020 2020  asic.           
+0000f910: 204e 6f74 6520 7468 6174 2054 2069 7320   Note that T is 
+0000f920: 666f 7220 7468 6520 636f 6f72 6469 6e61  for the coordina
+0000f930: 7465 2073 7973 7465 6d2c 206e 6f74 2061  te system, not a
+0000f940: 2067 7269 640a 2020 2020 2020 2020 2020   grid.          
+0000f950: 2020 2875 6e6c 6573 7320 7479 7065 203d    (unless type =
+0000f960: 2031 2077 6869 6368 206d 6561 6e73 2072   1 which means r
+0000f970: 6563 7461 6e67 756c 6172 290a 0a20 2020  ectangular)..   
+0000f980: 2062 7365 745f 626f 6f6c 203a 2031 6420   bset_bool : 1d 
+0000f990: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+0000f9a0: 4120 626f 6f6c 6561 6e20 7061 7274 6974  A boolean partit
+0000f9b0: 696f 6e20 7665 6374 6f72 2077 6974 6820  ion vector with 
+0000f9c0: 5472 7565 2066 6f72 2074 6865 2062 2d73  True for the b-s
+0000f9d0: 6574 2e20 5468 6973 2069 730a 2020 2020  et. This is.    
+0000f9e0: 2020 2020 6372 6561 7465 6420 666f 7220      created for 
+0000f9f0: 636f 6e76 656e 6965 6e63 6520 6279 3a3a  convenience by::
+0000fa00: 0a0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
+0000fa10: 6f6d 2070 7979 6574 6920 696d 706f 7274  om pyyeti import
+0000fa20: 206e 6173 7472 616e 0a20 2020 2020 2020   nastran.       
+0000fa30: 2020 2020 2062 7365 745f 626f 6f6c 203d       bset_bool =
+0000fa40: 206e 6173 7472 616e 2e6d 6b73 6574 7076   nastran.mksetpv
+0000fa50: 2875 7365 742c 2027 6127 2c20 2762 2729  (uset, 'a', 'b')
+0000fa60: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
+0000fa70: 2d2d 2d2d 2d0a 2020 2020 5468 6973 2072  -----.    This r
+0000fa80: 6f75 7469 6e65 2077 696c 6c20 6174 7465  outine will atte
+0000fa90: 6d70 7420 746f 2072 6561 6420 7468 6520  mpt to read the 
+0000faa0: 2245 5854 524e 2220 6361 7264 2066 726f  "EXTRN" card fro
+0000fab0: 6d20 7468 6520 2e70 6368 0a20 2020 2066  m the .pch.    f
+0000fac0: 696c 6520 696e 2063 6173 6520 736f 6d65  ile in case some
+0000fad0: 2062 2d73 6574 206e 6f64 6573 2064 6f20   b-set nodes do 
+0000fae0: 6e6f 7420 696e 636c 7564 6520 616c 6c20  not include all 
+0000faf0: 3620 444f 462e 2046 6f72 0a20 2020 2065  6 DOF. For.    e
+0000fb00: 7861 6d70 6c65 2c20 6120 6d6f 6465 6c20  xample, a model 
+0000fb10: 636f 756c 6420 6861 7665 2037 2062 2d73  could have 7 b-s
+0000fb20: 6574 2044 4f46 2061 6e64 2031 2071 2d73  et DOF and 1 q-s
+0000fb30: 6574 2044 4f46 2e20 4966 2074 6865 2037  et DOF. If the 7
+0000fb40: 0a20 2020 2062 2d73 6574 2044 4f46 2061  .    b-set DOF a
+0000fb50: 7265 2063 6f6d 706f 7365 6420 6f66 2061  re composed of a
+0000fb60: 6c6c 2036 2044 4f46 2066 6f72 206e 6f64  ll 6 DOF for nod
+0000fb70: 6520 3130 3020 616e 6420 6a75 7374 2074  e 100 and just t
+0000fb80: 6865 0a20 2020 2073 6563 6f6e 6420 444f  he.    second DO
+0000fb90: 4620 666f 7220 6e6f 6465 2032 3030 2c20  F for node 200, 
+0000fba0: 7468 6520 4558 5452 4e20 6361 7264 2077  the EXTRN card w
+0000fbb0: 6f75 6c64 206c 696b 6520 7468 6973 3a3a  ould like this::
+0000fbc0: 0a0a 2020 2020 2020 2020 4558 5452 4e2c  ..        EXTRN,
+0000fbd0: 3130 302c 3132 3334 3536 2c32 3030 2c32  100,123456,200,2
+0000fbe0: 2c31 3030 312c 300a 0a20 2020 2045 7861  ,1001,0..    Exa
+0000fbf0: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+0000fc00: 2d2d 0a20 2020 203e 3e3e 2069 6d70 6f72  --.    >>> impor
+0000fc10: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
+0000fc20: 2020 3e3e 3e20 6672 6f6d 2069 6f20 696d    >>> from io im
+0000fc30: 706f 7274 2053 7472 696e 6749 4f0a 2020  port StringIO.  
+0000fc40: 2020 3e3e 3e20 6672 6f6d 2070 7979 6574    >>> from pyyet
+0000fc50: 6920 696d 706f 7274 206e 6173 7472 616e  i import nastran
+0000fc60: 0a20 2020 203e 3e3e 2061 736d 5f62 756c  .    >>> asm_bul
+0000fc70: 6b20 3d20 280a 2020 2020 2e2e 2e20 2020  k = (.    ...   
+0000fc80: 2022 2420 5345 3130 3120 4153 5345 4d42   "$ SE101 ASSEMB
+0000fc90: 4c59 2046 494c 455c 6e22 0a20 2020 202e  LY FILE\n".    .
+0000fca0: 2e2e 2020 2020 2253 4542 554c 4b2c 3130  ..    "SEBULK,10
+0000fcb0: 312c 4558 544f 5034 2c2c 4d41 4e55 414c  1,EXTOP4,,MANUAL
+0000fcc0: 2c2c 2c31 3031 5c6e 220a 2020 2020 2e2e  ,,,101\n".    ..
+0000fcd0: 2e20 2020 2022 5345 434f 4e43 542c 3130  .    "SECONCT,10
+0000fce0: 312c 302c 2c4e 4f5c 6e22 0a20 2020 202e  1,0,,NO\n".    .
+0000fcf0: 2e2e 2020 2020 222c 332c 332c 3131 302c  ..    ",3,3,110,
+0000fd00: 3131 302c 3139 2c31 392c 3237 2c32 375c  110,19,19,27,27\
+0000fd10: 6e22 0a20 2020 202e 2e2e 2020 2020 2224  n".    ...    "$
+0000fd20: 2043 6f6f 7264 696e 6174 6520 3130 3a5c   Coordinate 10:\
+0000fd30: 6e22 0a20 2020 202e 2e2e 2020 2020 2243  n".    ...    "C
+0000fd40: 4f52 4432 522c 3130 2c30 2c30 2e30 2c30  ORD2R,10,0,0.0,0
+0000fd50: 2e30 2c30 2e30 2c31 2e30 2c30 2e30 2c30  .0,0.0,1.0,0.0,0
+0000fd60: 2e30 5c6e 220a 2020 2020 2e2e 2e20 2020  .0\n".    ...   
+0000fd70: 2022 2c30 2e30 2c31 2e30 2c30 2e30 5c6e   ",0.0,1.0,0.0\n
+0000fd80: 220a 2020 2020 2e2e 2e20 2020 2022 4752  ".    ...    "GR
+0000fd90: 4944 2c33 2c30 2c36 3030 2e2c 302e 2c33  ID,3,0,600.,0.,3
+0000fda0: 3030 2e2c 305c 6e22 0a20 2020 202e 2e2e  00.,0\n".    ...
+0000fdb0: 2020 2020 2247 5249 442c 3139 2c30 2c36      "GRID,19,0,6
+0000fdc0: 3030 2e2c 3330 302e 2c30 2e2c 305c 6e22  00.,300.,0.,0\n"
+0000fdd0: 0a20 2020 202e 2e2e 2020 2020 2247 5249  .    ...    "GRI
+0000fde0: 442c 3237 2c30 2c36 3030 2e2c 302e 2c30  D,27,0,600.,0.,0
+0000fdf0: 2e5c 6e22 0a20 2020 202e 2e2e 2020 2020  .\n".    ...    
+0000fe00: 2253 504f 494e 542c 3131 305c 6e22 0a20  "SPOINT,110\n". 
+0000fe10: 2020 202e 2e2e 2029 0a20 2020 203e 3e3e     ... ).    >>>
+0000fe20: 2077 6974 6820 5374 7269 6e67 494f 2861   with StringIO(a
+0000fe30: 736d 5f62 756c 6b29 2061 7320 663a 0a20  sm_bulk) as f:. 
+0000fe40: 2020 202e 2e2e 2020 2020 2075 2c20 632c     ...     u, c,
+0000fe50: 2062 203d 206e 6173 7472 616e 2e61 736d   b = nastran.asm
+0000fe60: 3275 7365 7428 6629 0a20 2020 203e 3e3e  2uset(f).    >>>
+0000fe70: 2075 2020 2020 2020 2020 2020 2020 2320   u            # 
+0000fe80: 646f 6374 6573 743a 202b 454c 4c49 5053  doctest: +ELLIPS
+0000fe90: 4953 0a20 2020 2020 2020 2020 2020 2020  IS.             
+0000fea0: 206e 6173 7365 7420 2020 2020 2078 2020   nasset      x  
+0000feb0: 2020 2020 7920 2020 2020 207a 0a20 2020      y      z.   
+0000fec0: 2069 6420 2064 6f66 2e2e 2e0a 2020 2020   id  dof....    
+0000fed0: 3320 2020 3120 2020 2032 3039 3731 3534  3   1    2097154
+0000fee0: 2020 3630 302e 3020 2020 2030 2e30 2020    600.0    0.0  
+0000fef0: 3330 302e 300a 2020 2020 2020 2020 3220  300.0.        2 
+0000ff00: 2020 2032 3039 3731 3534 2020 2020 302e     2097154    0.
+0000ff10: 3020 2020 2031 2e30 2020 2020 302e 300a  0    1.0    0.0.
+0000ff20: 2020 2020 2020 2020 3320 2020 2032 3039          3    209
+0000ff30: 3731 3534 2020 2020 302e 3020 2020 2030  7154    0.0    0
+0000ff40: 2e30 2020 2020 302e 300a 2020 2020 2020  .0    0.0.      
+0000ff50: 2020 3420 2020 2032 3039 3731 3534 2020    4    2097154  
+0000ff60: 2020 312e 3020 2020 2030 2e30 2020 2020    1.0    0.0    
+0000ff70: 302e 300a 2020 2020 2020 2020 3520 2020  0.0.        5   
+0000ff80: 2032 3039 3731 3534 2020 2020 302e 3020   2097154    0.0 
+0000ff90: 2020 2031 2e30 2020 2020 302e 300a 2020     1.0    0.0.  
+0000ffa0: 2020 2020 2020 3620 2020 2032 3039 3731        6    20971
+0000ffb0: 3534 2020 2020 302e 3020 2020 2030 2e30  54    0.0    0.0
+0000ffc0: 2020 2020 312e 300a 2020 2020 3131 3020      1.0.    110 
+0000ffd0: 3020 2020 2034 3139 3433 3034 2020 2020  0    4194304    
+0000ffe0: 302e 3020 2020 2030 2e30 2020 2020 302e  0.0    0.0    0.
+0000fff0: 300a 2020 2020 3139 2020 3120 2020 2032  0.    19  1    2
+00010000: 3039 3731 3534 2020 3630 302e 3020 2033  097154  600.0  3
+00010010: 3030 2e30 2020 2020 302e 300a 2020 2020  00.0    0.0.    
+00010020: 2020 2020 3220 2020 2032 3039 3731 3534      2    2097154
+00010030: 2020 2020 302e 3020 2020 2031 2e30 2020      0.0    1.0  
+00010040: 2020 302e 300a 2020 2020 2020 2020 3320    0.0.        3 
+00010050: 2020 2032 3039 3731 3534 2020 2020 302e     2097154    0.
+00010060: 3020 2020 2030 2e30 2020 2020 302e 300a  0    0.0    0.0.
+00010070: 2020 2020 2020 2020 3420 2020 2032 3039          4    209
+00010080: 3731 3534 2020 2020 312e 3020 2020 2030  7154    1.0    0
+00010090: 2e30 2020 2020 302e 300a 2020 2020 2020  .0    0.0.      
+000100a0: 2020 3520 2020 2032 3039 3731 3534 2020    5    2097154  
+000100b0: 2020 302e 3020 2020 2031 2e30 2020 2020    0.0    1.0    
+000100c0: 302e 300a 2020 2020 2020 2020 3620 2020  0.0.        6   
+000100d0: 2032 3039 3731 3534 2020 2020 302e 3020   2097154    0.0 
+000100e0: 2020 2030 2e30 2020 2020 312e 300a 2020     0.0    1.0.  
+000100f0: 2020 3237 2020 3120 2020 2032 3039 3731    27  1    20971
+00010100: 3534 2020 3630 302e 3020 2020 2030 2e30  54  600.0    0.0
+00010110: 2020 2020 302e 300a 2020 2020 2020 2020      0.0.        
+00010120: 3220 2020 2032 3039 3731 3534 2020 2020  2    2097154    
+00010130: 302e 3020 2020 2031 2e30 2020 2020 302e  0.0    1.0    0.
+00010140: 300a 2020 2020 2020 2020 3320 2020 2032  0.        3    2
+00010150: 3039 3731 3534 2020 2020 302e 3020 2020  097154    0.0   
+00010160: 2030 2e30 2020 2020 302e 300a 2020 2020   0.0    0.0.    
+00010170: 2020 2020 3420 2020 2032 3039 3731 3534      4    2097154
+00010180: 2020 2020 312e 3020 2020 2030 2e30 2020      1.0    0.0  
+00010190: 2020 302e 300a 2020 2020 2020 2020 3520    0.0.        5 
+000101a0: 2020 2032 3039 3731 3534 2020 2020 302e     2097154    0.
+000101b0: 3020 2020 2031 2e30 2020 2020 302e 300a  0    1.0    0.0.
+000101c0: 2020 2020 2020 2020 3620 2020 2032 3039          6    209
+000101d0: 3731 3534 2020 2020 302e 3020 2020 2030  7154    0.0    0
+000101e0: 2e30 2020 2020 312e 300a 2020 2020 3e3e  .0    1.0.    >>
+000101f0: 3e20 6320 2020 2020 2020 2020 2020 2023  > c            #
+00010200: 2064 6f63 7465 7374 3a20 2b53 4b49 500a   doctest: +SKIP.
+00010210: 2020 2020 7b30 3a20 6172 7261 7928 5b5b      {0: array([[
+00010220: 2030 2e2c 2020 312e 2c20 2030 2e5d 2c0a   0.,  1.,  0.],.
+00010230: 2020 2020 2020 2020 2020 2020 5b20 302e              [ 0.
+00010240: 2c20 2030 2e2c 2020 302e 5d2c 0a20 2020  ,  0.,  0.],.   
+00010250: 2020 2020 2020 2020 205b 2031 2e2c 2020           [ 1.,  
+00010260: 302e 2c20 2030 2e5d 2c0a 2020 2020 2020  0.,  0.],.      
+00010270: 2020 2020 2020 5b20 302e 2c20 2031 2e2c        [ 0.,  1.,
+00010280: 2020 302e 5d2c 0a20 2020 2020 2020 2020    0.],.         
+00010290: 2020 205b 2030 2e2c 2020 302e 2c20 2031     [ 0.,  0.,  1
+000102a0: 2e5d 5d29 2c0a 2020 2020 2031 303a 2061  .]]),.     10: a
+000102b0: 7272 6179 285b 5b20 3130 2e2c 2020 2031  rray([[ 10.,   1
+000102c0: 2e2c 2020 2030 2e5d 2c0a 2020 2020 2020  .,   0.],.      
+000102d0: 2020 2020 2020 5b20 2030 2e2c 2020 2030        [  0.,   0
+000102e0: 2e2c 2020 2030 2e5d 2c0a 2020 2020 2020  .,   0.],.      
+000102f0: 2020 2020 2020 5b20 2030 2e2c 2020 2030        [  0.,   0
+00010300: 2e2c 2020 2031 2e5d 2c0a 2020 2020 2020  .,   1.],.      
+00010310: 2020 2020 2020 5b20 2031 2e2c 2020 2030        [  1.,   0
+00010320: 2e2c 2020 2030 2e5d 2c0a 2020 2020 2020  .,   0.],.      
+00010330: 2020 2020 2020 5b20 2030 2e2c 2020 2031        [  0.,   1
+00010340: 2e2c 2020 2030 2e5d 5d29 7d0a 2020 2020  .,   0.]])}.    
+00010350: 3e3e 3e20 6e70 2e73 6574 5f70 7269 6e74  >>> np.set_print
+00010360: 6f70 7469 6f6e 7328 6c69 6e65 7769 6474  options(linewidt
+00010370: 683d 3535 290a 2020 2020 3e3e 3e20 620a  h=55).    >>> b.
+00010380: 2020 2020 6172 7261 7928 5b20 5472 7565      array([ True
+00010390: 2c20 2054 7275 652c 2020 5472 7565 2c20  ,  True,  True, 
+000103a0: 2054 7275 652c 2020 5472 7565 2c20 2054   True,  True,  T
+000103b0: 7275 652c 2046 616c 7365 2c0a 2020 2020  rue, False,.    
+000103c0: 2020 2020 2020 2020 5472 7565 2c20 2054          True,  T
+000103d0: 7275 652c 2020 5472 7565 2c20 2054 7275  rue,  True,  Tru
+000103e0: 652c 2020 5472 7565 2c20 2054 7275 652c  e,  True,  True,
+000103f0: 2020 5472 7565 2c0a 2020 2020 2020 2020    True,.        
+00010400: 2020 2020 5472 7565 2c20 2054 7275 652c      True,  True,
+00010410: 2020 5472 7565 2c20 2054 7275 652c 2020    True,  True,  
+00010420: 5472 7565 5d2c 2064 7479 7065 3d62 6f6f  True], dtype=boo
+00010430: 6c29 0a20 2020 2022 2222 0a20 2020 2075  l).    """.    u
+00010440: 7365 742c 2063 6f6f 7264 7320 3d20 6275  set, coords = bu
+00010450: 6c6b 3275 7365 7428 6629 0a0a 2020 2020  lk2uset(f)..    
+00010460: 2320 6164 6420 7370 6f69 6e74 7320 746f  # add spoints to
+00010470: 2075 7365 7420 7461 626c 653a 0a20 2020   uset table:.   
+00010480: 2073 706f 696e 7473 203d 2072 6473 706f   spoints = rdspo
+00010490: 696e 7473 2866 290a 2020 2020 6966 2073  ints(f).    if s
+000104a0: 706f 696e 7473 2069 7320 6e6f 7420 4e6f  points is not No
+000104b0: 6e65 3a0a 2020 2020 2020 2020 6e20 3d20  ne:.        n = 
+000104c0: 6c65 6e28 7370 6f69 6e74 7329 0a20 2020  len(spoints).   
+000104d0: 2020 2020 2064 6f66 203d 206e 702e 7a65       dof = np.ze
+000104e0: 726f 7328 286e 2c20 3229 2c20 6e70 2e69  ros((n, 2), np.i
+000104f0: 6e74 3634 290a 2020 2020 2020 2020 646f  nt64).        do
+00010500: 665b 3a2c 2030 5d20 3d20 7370 6f69 6e74  f[:, 0] = spoint
+00010510: 730a 2020 2020 2020 2020 7573 6574 5f73  s.        uset_s
+00010520: 706f 696e 7473 203d 206e 3270 2e6d 616b  points = n2p.mak
+00010530: 655f 7573 6574 2864 6f66 2c20 6e32 702e  e_uset(dof, n2p.
+00010540: 6d6b 7573 6574 6d61 736b 2822 7122 292c  mkusetmask("q"),
+00010550: 206e 702e 7a65 726f 7328 286e 2c20 3329   np.zeros((n, 3)
+00010560: 2929 0a20 2020 2020 2020 2075 7365 7420  )).        uset 
+00010570: 3d20 7064 2e63 6f6e 6361 7428 5b75 7365  = pd.concat([use
+00010580: 742c 2075 7365 745f 7370 6f69 6e74 735d  t, uset_spoints]
+00010590: 2c20 6178 6973 3d30 290a 0a20 2020 2069  , axis=0)..    i
+000105a0: 6620 7472 795f 7264 6578 7472 6e3a 0a20  f try_rdextrn:. 
+000105b0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+000105c0: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+000105d0: 203d 2066 2e6e 616d 650a 2020 2020 2020   = f.name.      
+000105e0: 2020 6578 6365 7074 2041 7474 7269 6275    except Attribu
+000105f0: 7465 4572 726f 723a 0a20 2020 2020 2020  teError:.       
+00010600: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
+00010610: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010620: 2020 2020 646f 6620 3d20 7264 6578 7472      dof = rdextr
+00010630: 6e28 6669 6c65 6e61 6d65 2e72 6570 6c61  n(filename.repla
+00010640: 6365 2822 2e61 736d 222c 2022 2e70 6368  ce(".asm", ".pch
+00010650: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+00010660: 7573 6574 5f6f 7264 6572 6564 203d 2075  uset_ordered = u
+00010670: 7365 742e 6c6f 635b 6c69 7374 2864 6f66  set.loc[list(dof
+00010680: 295d 0a20 2020 2020 2020 2020 2020 2072  )].            r
+00010690: 6574 7572 6e20 7573 6574 5f6f 7264 6572  eturn uset_order
+000106a0: 6564 2c20 636f 6f72 6473 2c20 6e32 702e  ed, coords, n2p.
+000106b0: 6d6b 7365 7470 7628 7573 6574 5f6f 7264  mksetpv(uset_ord
+000106c0: 6572 6564 2c20 2261 222c 2022 6222 290a  ered, "a", "b").
+000106d0: 0a20 2020 2061 5f69 6473 203d 2072 6473  .    a_ids = rds
+000106e0: 6563 6f6e 6374 2866 295b 305d 0a20 2020  econct(f)[0].   
+000106f0: 2075 7365 745f 6f72 6465 7265 6420 3d20   uset_ordered = 
+00010700: 7573 6574 2e6c 6f63 5b61 5f69 6473 5d0a  uset.loc[a_ids].
+00010710: 2020 2020 6966 2075 7365 745f 6f72 6465      if uset_orde
+00010720: 7265 642e 7368 6170 655b 305d 2021 3d20  red.shape[0] != 
+00010730: 7573 6574 2e73 6861 7065 5b30 5d3a 0a20  uset.shape[0]:. 
+00010740: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00010750: 7469 6d65 4572 726f 7228 0a20 2020 2020  timeError(.     
+00010760: 2020 2020 2020 2022 4e75 6d62 6572 206f         "Number o
+00010770: 6620 5345 434f 4e43 5420 7375 7065 7265  f SECONCT supere
+00010780: 6c65 6d65 6e74 2027 4127 2044 4f46 2064  lement 'A' DOF d
+00010790: 6f20 6e6f 7420 6d61 7463 6820 4752 4944  o not match GRID
+000107a0: 2061 6e64 220a 2020 2020 2020 2020 2020   and".          
+000107b0: 2020 2220 5350 4f49 4e54 2063 6172 6473    " SPOINT cards
+000107c0: 2069 6e20 6669 6c65 3a5c 6e22 0a20 2020   in file:\n".   
+000107d0: 2020 2020 2020 2020 2066 2220 2020 2023           f"    #
+000107e0: 2044 4f46 206f 6e20 5345 434f 4e43 5420   DOF on SECONCT 
+000107f0: 3d20 7b75 7365 745f 6f72 6465 7265 642e  = {uset_ordered.
+00010800: 7368 6170 655b 305d 7d5c 6e22 0a20 2020  shape[0]}\n".   
+00010810: 2020 2020 2020 2020 2066 2220 2020 2023           f"    #
+00010820: 2044 4f46 206f 6e20 4752 4944 532f 5350   DOF on GRIDS/SP
+00010830: 4f49 4e54 5320 3d20 7b75 7365 742e 7368  OINTS = {uset.sh
+00010840: 6170 655b 305d 7d22 0a20 2020 2020 2020  ape[0]}".       
+00010850: 2029 0a0a 2020 2020 7265 7475 726e 2075   )..    return u
+00010860: 7365 745f 6f72 6465 7265 642c 2063 6f6f  set_ordered, coo
+00010870: 7264 732c 206e 3270 2e6d 6b73 6574 7076  rds, n2p.mksetpv
+00010880: 2875 7365 745f 6f72 6465 7265 642c 2022  (uset_ordered, "
+00010890: 6122 2c20 2262 2229 0a0a 0a64 6566 2072  a", "b")...def r
+000108a0: 6477 7462 756c 6b28 6669 6e2c 2066 6f75  dwtbulk(fin, fou
+000108b0: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
+000108c0: 4765 7420 6275 6c6b 2064 6174 6120 6672  Get bulk data fr
+000108d0: 6f6d 2061 2073 6f72 7465 6420 4e61 7374  om a sorted Nast
+000108e0: 7261 6e20 6f75 7470 7574 2066 696c 652e  ran output file.
+000108f0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00010900: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00010910: 2020 2020 6669 6e20 3a20 7374 7269 6e67      fin : string
+00010920: 206f 7220 6669 6c65 5f6c 696b 6520 6f72   or file_like or
+00010930: 204e 6f6e 650a 2020 2020 2020 2020 4569   None.        Ei
+00010940: 7468 6572 2061 206e 616d 6520 6f66 2061  ther a name of a
+00010950: 2066 696c 652c 206f 7220 6973 2061 2066   file, or is a f
+00010960: 696c 655f 6c69 6b65 206f 626a 6563 7420  ile_like object 
+00010970: 6173 2072 6574 7572 6e65 640a 2020 2020  as returned.    
+00010980: 2020 2020 6279 203a 6675 6e63 3a60 6f70      by :func:`op
+00010990: 656e 602e 2049 6620 6669 6c65 5f6c 696b  en`. If file_lik
+000109a0: 6520 6f62 6a65 6374 2c20 6974 2069 7320  e object, it is 
+000109b0: 7265 776f 756e 6420 6669 7273 742e 2043  rewound first. C
+000109c0: 616e 0a20 2020 2020 2020 2061 6c73 6f20  an.        also 
+000109d0: 6265 2074 6865 206e 616d 6520 6f66 2061  be the name of a
+000109e0: 2064 6972 6563 746f 7279 206f 7220 4e6f   directory or No
+000109f0: 6e65 3b20 696e 2074 6865 7365 2063 6173  ne; in these cas
+00010a00: 6573 2c20 6120 4755 490a 2020 2020 2020  es, a GUI.      
+00010a10: 2020 6973 206f 7065 6e65 6420 666f 7220    is opened for 
+00010a20: 6669 6c65 2073 656c 6563 7469 6f6e 2e0a  file selection..
+00010a30: 2020 2020 666f 7574 203a 2073 7472 696e      fout : strin
+00010a40: 6720 6f72 2066 696c 655f 6c69 6b65 206f  g or file_like o
+00010a50: 7220 3120 6f72 204e 6f6e 650a 2020 2020  r 1 or None.    
+00010a60: 2020 2020 4569 7468 6572 2061 206e 616d      Either a nam
+00010a70: 6520 6f66 2061 2066 696c 652c 206f 7220  e of a file, or 
+00010a80: 6973 2061 2066 696c 655f 6c69 6b65 206f  is a file_like o
+00010a90: 626a 6563 7420 6173 2072 6574 7572 6e65  bject as returne
+00010aa0: 640a 2020 2020 2020 2020 6279 203a 6675  d.        by :fu
+00010ab0: 6e63 3a60 6f70 656e 6020 6f72 203a 636c  nc:`open` or :cl
+00010ac0: 6173 733a 6069 6f2e 5374 7269 6e67 494f  ass:`io.StringIO
+00010ad0: 602e 2049 6e70 7574 2061 7320 696e 7465  `. Input as inte
+00010ae0: 6765 7220 3120 746f 0a20 2020 2020 2020  ger 1 to.       
+00010af0: 2077 7269 7465 2074 6f20 7374 646f 7574   write to stdout
+00010b00: 2e20 4361 6e20 616c 736f 2062 6520 7468  . Can also be th
+00010b10: 6520 6e61 6d65 206f 6620 6120 6469 7265  e name of a dire
+00010b20: 6374 6f72 7920 6f72 204e 6f6e 653b 0a20  ctory or None;. 
+00010b30: 2020 2020 2020 2069 6e20 7468 6573 6520         in these 
+00010b40: 6361 7365 732c 2061 2047 5549 2069 7320  cases, a GUI is 
+00010b50: 6f70 656e 6564 2066 6f72 2066 696c 6520  opened for file 
+00010b60: 7365 6c65 6374 696f 6e2e 0a0a 2020 2020  selection...    
+00010b70: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00010b80: 2d2d 2d0a 2020 2020 4e6f 6e65 0a0a 2020  ---.    None..  
+00010b90: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
+00010ba0: 2d0a 2020 2020 5265 6164 7320 7468 6520  -.    Reads the 
+00010bb0: 6275 6c6b 2064 6174 6120 6672 6f6d 2069  bulk data from i
+00010bc0: 6e70 7574 2066 696c 6520 616e 6420 7772  nput file and wr
+00010bd0: 6974 6573 2069 7420 746f 2074 6865 206f  ites it to the o
+00010be0: 7574 7075 740a 2020 2020 6669 6c65 2e20  utput.    file. 
+00010bf0: 416c 6c20 636f 6e74 696e 7561 7469 6f6e  All continuation
+00010c00: 2063 6f64 6573 2061 7265 2073 7472 6970   codes are strip
+00010c10: 7065 6420 6f66 662e 0a0a 2020 2020 4861  ped off...    Ha
+00010c20: 7320 6e6f 7420 6265 656e 2074 6573 7465  s not been teste
+00010c30: 6420 6f6e 2075 6e73 6f72 7465 6420 6275  d on unsorted bu
+00010c40: 6c6b 2e0a 0a20 2020 2045 7861 6d70 6c65  lk...    Example
+00010c50: 2075 7361 6765 3a3a 0a0a 2020 2020 2020   usage::..      
+00010c60: 2020 6672 6f6d 2070 7979 6574 6920 696d    from pyyeti im
+00010c70: 706f 7274 206e 6173 7472 616e 0a20 2020  port nastran.   
+00010c80: 2020 2020 206e 6173 7472 616e 2e72 6477       nastran.rdw
+00010c90: 7462 756c 6b28 276d 6563 6f31 2e6f 7574  tbulk('meco1.out
+00010ca0: 272c 2027 6d65 636f 312e 626c 6b27 290a  ', 'meco1.blk').
+00010cb0: 2020 2020 2222 220a 0a20 2020 2040 6775      """..    @gu
+00010cc0: 6974 6f6f 6c73 2e72 6561 645f 7465 7874  itools.read_text
+00010cd0: 5f66 696c 650a 2020 2020 6465 6620 5f72  _file.    def _r
+00010ce0: 6462 756c 6b28 6629 3a0a 2020 2020 2020  dbulk(f):.      
+00010cf0: 2020 6673 6561 7263 6828 662c 2022 434f    fsearch(f, "CO
+00010d00: 554e 5420 2020 2020 2020 202e 2020 2031  UNT        .   1
+00010d10: 2020 2e2e 2020 2032 2020 2e2e 2020 2033    ..   2  ..   3
+00010d20: 2229 0a20 2020 2020 2020 2073 203d 205b  ").        s = [
+00010d30: 5d0a 2020 2020 2020 2020 7072 6f67 203d  ].        prog =
+00010d40: 2072 652e 636f 6d70 696c 6528 7222 5b20   re.compile(r"[ 
+00010d50: 5d7b 3133 7d5b 2030 2d39 5d7b 387d 2d5b  ]{13}[ 0-9]{8}-[
+00010d60: 205d 7b38 7d28 2e7b 3732 7d29 2229 0a20   ]{8}(.{72})"). 
+00010d70: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
+00010d80: 696e 2066 3a0a 2020 2020 2020 2020 2020  in f:.          
+00010d90: 2020 6966 206c 696e 652e 7374 6172 7473    if line.starts
+00010da0: 7769 7468 2822 2020 2020 2020 2020 2020  with("          
 00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 2020 206d 6174 6368 203d 206d 6174 6368     match = match
-00010dd0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00010de0: 2020 2020 732e 6170 7065 6e64 286d 6174      s.append(mat
-00010df0: 6368 290a 2020 2020 2020 2020 7265 7475  ch).        retu
-00010e00: 726e 2022 5c6e 222e 6a6f 696e 2873 2920  rn "\n".join(s) 
-00010e10: 2b20 225c 6e22 0a0a 2020 2020 4067 7569  + "\n"..    @gui
-00010e20: 746f 6f6c 732e 7772 6974 655f 7465 7874  tools.write_text
-00010e30: 5f66 696c 650a 2020 2020 6465 6620 5f77  _file.    def _w
-00010e40: 7462 756c 6b28 662c 2062 6c6b 293a 0a20  tbulk(f, blk):. 
-00010e50: 2020 2020 2020 2066 2e77 7269 7465 2862         f.write(b
-00010e60: 6c6b 290a 0a20 2020 205f 7774 6275 6c6b  lk)..    _wtbulk
-00010e70: 2866 6f75 742c 205f 7264 6275 6c6b 2866  (fout, _rdbulk(f
-00010e80: 696e 2929 0a0a 0a40 6775 6974 6f6f 6c73  in))...@guitools
-00010e90: 2e72 6561 645f 7465 7874 5f66 696c 650a  .read_text_file.
-00010ea0: 6465 6620 7264 6569 6765 6e28 662c 2075  def rdeigen(f, u
-00010eb0: 7365 5f70 616e 6461 733d 5472 7565 293a  se_pandas=True):
-00010ec0: 0a20 2020 2022 2222 0a20 2020 2052 6561  .    """.    Rea
-00010ed0: 6420 6569 6765 6e76 616c 7565 2074 6162  d eigenvalue tab
-00010ee0: 6c65 7320 6672 6f6d 2061 204e 6173 7472  les from a Nastr
-00010ef0: 616e 2066 3036 2066 696c 652e 0a0a 2020  an f06 file...  
-00010f00: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00010f10: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00010f20: 6620 3a20 7374 7269 6e67 206f 7220 6669  f : string or fi
-00010f30: 6c65 5f6c 696b 6520 6f72 204e 6f6e 650a  le_like or None.
-00010f40: 2020 2020 2020 2020 4569 7468 6572 2061          Either a
-00010f50: 206e 616d 6520 6f66 2061 2066 696c 652c   name of a file,
-00010f60: 206f 7220 6973 2061 2066 696c 655f 6c69   or is a file_li
-00010f70: 6b65 206f 626a 6563 7420 6173 2072 6574  ke object as ret
-00010f80: 7572 6e65 640a 2020 2020 2020 2020 6279  urned.        by
-00010f90: 203a 6675 6e63 3a60 6f70 656e 602e 2049   :func:`open`. I
-00010fa0: 6620 6669 6c65 5f6c 696b 6520 6f62 6a65  f file_like obje
-00010fb0: 6374 2c20 6974 2069 7320 7265 776f 756e  ct, it is rewoun
-00010fc0: 6420 6669 7273 742e 2043 616e 0a20 2020  d first. Can.   
-00010fd0: 2020 2020 2061 6c73 6f20 6265 2074 6865       also be the
-00010fe0: 206e 616d 6520 6f66 2061 2064 6972 6563   name of a direc
-00010ff0: 746f 7279 206f 7220 4e6f 6e65 3b20 696e  tory or None; in
-00011000: 2074 6865 7365 2063 6173 6573 2c20 6120   these cases, a 
-00011010: 4755 490a 2020 2020 2020 2020 6973 206f  GUI.        is o
-00011020: 7065 6e65 6420 666f 7220 6669 6c65 2073  pened for file s
-00011030: 656c 6563 7469 6f6e 2e0a 2020 2020 7573  election..    us
-00011040: 655f 7061 6e64 6173 203a 2062 6f6f 6c3b  e_pandas : bool;
-00011050: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00011060: 2020 4966 2054 7275 652c 2074 6865 2076    If True, the v
-00011070: 616c 7565 7320 7265 7475 726e 6564 2069  alues returned i
-00011080: 6e20 7468 6520 6469 6374 696f 6e61 7279  n the dictionary
-00011090: 2077 696c 6c20 6265 2070 616e 6461 730a   will be pandas.
-000110a0: 2020 2020 2020 2020 4461 7461 4672 616d          DataFram
-000110b0: 6573 0a0a 2020 2020 5265 7475 726e 730a  es..    Returns.
-000110c0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000110d0: 6469 6374 696f 6e61 7279 0a20 2020 2020  dictionary.     
-000110e0: 2020 2054 6865 206b 6579 7320 6172 6520     The keys are 
-000110f0: 7468 6520 7375 7065 7265 6c65 6d65 6e74  the superelement
-00011100: 2049 4473 2061 6e64 2074 6865 2076 616c   IDs and the val
-00011110: 7565 7320 6973 2074 6865 2037 0a20 2020  ues is the 7.   
-00011120: 2020 2020 2063 6f6c 756d 6e20 6569 6765       column eige
-00011130: 6e76 616c 7565 2074 6162 6c65 3a20 5b6d  nvalue table: [m
-00011140: 6f64 6520 6e75 6d62 6572 2c20 6578 7472  ode number, extr
-00011150: 6163 7469 6f6e 206f 7264 6572 2c0a 2020  action order,.  
-00011160: 2020 2020 2020 6569 6765 6e76 616c 7565        eigenvalue
-00011170: 2c20 7261 6469 616e 732c 2063 7963 6c65  , radians, cycle
-00011180: 732c 2067 656e 6572 616c 697a 6564 206d  s, generalized m
-00011190: 6173 732c 2067 656e 6572 616c 697a 6564  ass, generalized
-000111a0: 0a20 2020 2020 2020 2073 7469 6666 6e65  .        stiffne
-000111b0: 7373 5d0a 0a20 2020 204e 6f74 6573 0a20  ss]..    Notes. 
-000111c0: 2020 202d 2d2d 2d2d 0a20 2020 2054 6865     -----.    The
-000111d0: 206c 6173 7420 7461 626c 6520 7265 6164   last table read
-000111e0: 2066 6f72 2061 2073 7570 6572 656c 656d   for a superelem
-000111f0: 656e 7420 7265 706c 6163 6573 2074 6162  ent replaces tab
-00011200: 6c65 7320 7072 6576 696f 7573 6c79 0a20  les previously. 
-00011210: 2020 2072 6561 6420 696e 2e0a 0a20 2020     read in...   
-00011220: 2049 6620 7468 6520 7061 6e64 6173 206f   If the pandas o
-00011230: 7574 7075 7420 6973 2063 686f 7365 6e20  utput is chosen 
-00011240: 2874 6865 2064 6566 6175 6c74 2920 7468  (the default) th
-00011250: 6520 6d6f 6465 206e 756d 6265 7220 6973  e mode number is
-00011260: 0a20 2020 2075 7365 6420 6173 2074 6865  .    used as the
-00011270: 2060 696e 6465 7860 2061 6e64 2060 636f   `index` and `co
-00011280: 6c75 6d6e 7360 2069 733a 3a0a 0a20 2020  lumns` is::..   
-00011290: 2020 2020 2063 203d 205b 274d 6f64 6520       c = ['Mode 
-000112a0: 2327 2c20 2765 7874 2023 272c 2027 6569  #', 'ext #', 'ei
-000112b0: 6765 6e76 616c 7565 272c 2027 7261 6469  genvalue', 'radi
-000112c0: 616e 7327 2c0a 2020 2020 2020 2020 2020  ans',.          
-000112d0: 2020 2027 6379 636c 6573 272c 2027 6765     'cycles', 'ge
-000112e0: 6e6d 6173 7327 2c20 2767 656e 7374 6966  nmass', 'genstif
-000112f0: 275d 0a20 2020 2022 2222 0a0a 2020 2020  '].    """..    
-00011300: 6465 6620 5f66 696e 645f 6569 6765 6e28  def _find_eigen(
-00011310: 6629 3a0a 2020 2020 2020 2020 5345 203d  f):.        SE =
-00011320: 2022 5355 5045 5245 4c45 4d45 4e54 2022   "SUPERELEMENT "
-00011330: 0a20 2020 2020 2020 2045 4947 203d 2022  .        EIG = "
-00011340: 5220 4520 4120 4c20 2020 4520 4920 4720  R E A L   E I G 
-00011350: 4520 4e20 5620 4120 4c20 5520 4520 5322  E N V A L U E S"
-00011360: 0a20 2020 2020 2020 2073 6520 3d20 300a  .        se = 0.
-00011370: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
-00011380: 2069 6e20 663a 0a20 2020 2020 2020 2020   in f:.         
-00011390: 2020 2069 6620 6c65 6e28 6c69 6e65 2920     if len(line) 
-000113a0: 3e20 3131 3620 616e 6420 6c69 6e65 5b31  > 116 and line[1
-000113b0: 3034 3a5d 2e73 7461 7274 7377 6974 6828  04:].startswith(
-000113c0: 5345 293a 0a20 2020 2020 2020 2020 2020  SE):.           
-000113d0: 2020 2020 2073 6520 3d20 696e 7428 6c69       se = int(li
-000113e0: 6e65 5b31 3136 3a5d 290a 2020 2020 2020  ne[116:]).      
-000113f0: 2020 2020 2020 6966 206c 656e 286c 696e        if len(lin
-00011400: 6529 203e 2037 3620 616e 6420 6c69 6e65  e) > 76 and line
-00011410: 5b34 363a 5d2e 7374 6172 7473 7769 7468  [46:].startswith
-00011420: 2845 4947 293a 0a20 2020 2020 2020 2020  (EIG):.         
-00011430: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011450: 4e6f 6e65 0a0a 2020 2020 6465 6620 5f72  None..    def _r
-00011460: 645f 6569 6765 6e5f 7461 626c 6528 6629  d_eigen_table(f)
-00011470: 3a0a 2020 2020 2020 2020 2222 2245 6967  :.        """Eig
-00011480: 656e 7661 6c75 6520 7461 626c 6520 666f  envalue table fo
-00011490: 756e 642c 2072 6561 6420 6974 2e22 2222  und, read it."""
-000114a0: 0a20 2020 2020 2020 2066 6f72 206c 696e  .        for lin
-000114b0: 6520 696e 2066 3a0a 2020 2020 2020 2020  e in f:.        
-000114c0: 2020 2020 6966 206c 696e 652e 7374 6172      if line.star
-000114d0: 7473 7769 7468 2822 2020 2020 4e4f 2e22  tswith("    NO."
-000114e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000114f0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00011500: 2074 6162 6c65 203d 205b 5d0a 2020 2020   table = [].    
-00011510: 2020 2020 636f 6e74 696e 7565 6420 3d20      continued = 
-00011520: 5472 7565 0a20 2020 2020 2020 2077 6869  True.        whi
-00011530: 6c65 2063 6f6e 7469 6e75 6564 3a0a 2020  le continued:.  
-00011540: 2020 2020 2020 2020 2020 666f 7220 6c69            for li
-00011550: 6e65 2069 6e20 663a 0a20 2020 2020 2020  ne in f:.       
-00011560: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011580: 2020 726f 7720 3d20 5b66 6c6f 6174 2869    row = [float(i
-00011590: 2920 666f 7220 6920 696e 206c 696e 652e  ) for i in line.
-000115a0: 7370 6c69 7428 295d 0a20 2020 2020 2020  split()].       
-000115b0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-000115c0: 5661 6c75 6545 7272 6f72 3a0a 2020 2020  ValueError:.    
-000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115e0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-000115f0: 2020 2020 2020 6966 206c 656e 2872 6f77        if len(row
-00011600: 2920 3d3d 2037 3a0a 2020 2020 2020 2020  ) == 7:.        
-00011610: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00011620: 652e 6170 7065 6e64 2872 6f77 290a 2020  e.append(row).  
-00011630: 2020 2020 2020 2020 2020 666f 7220 5f20            for _ 
-00011640: 696e 2072 616e 6765 2838 293a 0a20 2020  in range(8):.   
-00011650: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-00011660: 6520 3d20 662e 7265 6164 6c69 6e65 2829  e = f.readline()
-00011670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011680: 2069 6620 6c69 6e65 2e73 7461 7274 7377   if line.startsw
-00011690: 6974 6828 2231 2022 293a 0a20 2020 2020  ith("1 "):.     
-000116a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000116b0: 6f6e 7469 6e75 6564 203d 2046 616c 7365  ontinued = False
-000116c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000116d0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-000116e0: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
-000116f0: 6e65 2e73 7461 7274 7377 6974 6828 2220  ne.startswith(" 
-00011700: 2020 204e 4f2e 2229 3a0a 2020 2020 2020     NO."):.      
-00011710: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00011720: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00011730: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00011740: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00011750: 2020 2020 7265 7475 726e 206e 702e 6172      return np.ar
-00011760: 7261 7928 7461 626c 6529 0a0a 2020 2020  ray(table)..    
-00011770: 6463 7420 3d20 7b7d 0a20 2020 2066 2e73  dct = {}.    f.s
-00011780: 6565 6b28 302c 2030 290a 2020 2020 7768  eek(0, 0).    wh
-00011790: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
-000117a0: 2020 7365 203d 205f 6669 6e64 5f65 6967    se = _find_eig
-000117b0: 656e 2866 290a 2020 2020 2020 2020 6966  en(f).        if
-000117c0: 2073 6520 6973 204e 6f6e 653a 0a20 2020   se is None:.   
-000117d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000117e0: 6463 740a 2020 2020 2020 2020 7461 626c  dct.        tabl
-000117f0: 6520 3d20 5f72 645f 6569 6765 6e5f 7461  e = _rd_eigen_ta
-00011800: 626c 6528 6629 0a20 2020 2020 2020 2069  ble(f).        i
-00011810: 6620 7573 655f 7061 6e64 6173 3a0a 2020  f use_pandas:.  
-00011820: 2020 2020 2020 2020 2020 6920 3d20 7461            i = ta
-00011830: 626c 655b 3a2c 2030 5d2e 6173 7479 7065  ble[:, 0].astype
-00011840: 2869 6e74 290a 2020 2020 2020 2020 2020  (int).          
-00011850: 2020 6320 3d20 5b0a 2020 2020 2020 2020    c = [.        
-00011860: 2020 2020 2020 2020 226d 6f64 6520 2322          "mode #"
-00011870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011880: 2020 2265 7874 2023 222c 0a20 2020 2020    "ext #",.     
-00011890: 2020 2020 2020 2020 2020 2022 6569 6765             "eige
-000118a0: 6e76 616c 7565 222c 0a20 2020 2020 2020  nvalue",.       
-000118b0: 2020 2020 2020 2020 2022 7261 6469 616e           "radian
-000118c0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000118d0: 2020 2020 2263 7963 6c65 7322 2c0a 2020      "cycles",.  
-000118e0: 2020 2020 2020 2020 2020 2020 2020 2267                "g
-000118f0: 656e 6d61 7373 222c 0a20 2020 2020 2020  enmass",.       
-00011900: 2020 2020 2020 2020 2022 6765 6e73 7469           "gensti
-00011910: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
-00011920: 5d0a 2020 2020 2020 2020 2020 2020 7461  ].            ta
-00011930: 626c 6520 3d20 7064 2e44 6174 6146 7261  ble = pd.DataFra
-00011940: 6d65 2874 6162 6c65 2c20 696e 6465 783d  me(table, index=
-00011950: 692c 2063 6f6c 756d 6e73 3d63 290a 2020  i, columns=c).  
-00011960: 2020 2020 2020 6463 745b 7365 5d20 3d20        dct[se] = 
-00011970: 7461 626c 650a 0a0a 4067 7569 746f 6f6c  table...@guitool
-00011980: 732e 7772 6974 655f 7465 7874 5f66 696c  s.write_text_fil
-00011990: 650a 6465 6620 7774 6e61 7369 6e74 7328  e.def wtnasints(
-000119a0: 662c 2073 7461 7274 2c20 696e 7473 293a  f, start, ints):
-000119b0: 0a20 2020 2022 2222 0a20 2020 2055 7469  .    """.    Uti
-000119c0: 6c69 7479 2072 6f75 7469 6e65 2066 6f72  lity routine for
-000119d0: 2074 6865 206e 6173 7472 616e 2027 7774   the nastran 'wt
-000119e0: 2a27 2072 6f75 7469 6e65 732e 0a0a 2020  *' routines...  
-000119f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00011a00: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00011a10: 6620 3a20 7374 7269 6e67 206f 7220 6669  f : string or fi
-00011a20: 6c65 5f6c 696b 6520 6f72 2031 206f 7220  le_like or 1 or 
-00011a30: 4e6f 6e65 0a20 2020 2020 2020 2045 6974  None.        Eit
-00011a40: 6865 7220 6120 6e61 6d65 206f 6620 6120  her a name of a 
-00011a50: 6669 6c65 2c20 6f72 2069 7320 6120 6669  file, or is a fi
-00011a60: 6c65 5f6c 696b 6520 6f62 6a65 6374 2061  le_like object a
-00011a70: 7320 7265 7475 726e 6564 0a20 2020 2020  s returned.     
-00011a80: 2020 2062 7920 3a66 756e 633a 606f 7065     by :func:`ope
-00011a90: 6e60 206f 7220 3a63 6c61 7373 3a60 696f  n` or :class:`io
-00011aa0: 2e53 7472 696e 6749 4f60 2e20 496e 7075  .StringIO`. Inpu
-00011ab0: 7420 6173 2069 6e74 6567 6572 2031 2074  t as integer 1 t
-00011ac0: 6f0a 2020 2020 2020 2020 7772 6974 6520  o.        write 
-00011ad0: 746f 2073 7464 6f75 742e 2043 616e 2061  to stdout. Can a
-00011ae0: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
-00011af0: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
-00011b00: 7220 4e6f 6e65 3b0a 2020 2020 2020 2020  r None;.        
-00011b10: 696e 2074 6865 7365 2063 6173 6573 2c20  in these cases, 
-00011b20: 6120 4755 4920 6973 206f 7065 6e65 6420  a GUI is opened 
-00011b30: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
-00011b40: 6f6e 2e0a 2020 2020 7374 6172 7420 3a20  on..    start : 
-00011b50: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-00011b60: 4265 6769 6e6e 696e 6720 6669 656c 6420  Beginning field 
-00011b70: 666f 7220 7468 6520 696e 7465 6765 7273  for the integers
-00011b80: 3b20 6361 7264 206e 616d 6520 6973 2069  ; card name is i
-00011b90: 6e20 6669 656c 6420 312c 2073 6f0a 2020  n field 1, so.  
-00011ba0: 2020 2020 2020 7374 6172 7420 7368 6f75        start shou
-00011bb0: 6c64 2062 6520 3e3d 2032 2e0a 2020 2020  ld be >= 2..    
-00011bc0: 696e 7473 203a 2031 6420 6172 7261 795f  ints : 1d array_
-00011bd0: 6c69 6b65 0a20 2020 2020 2020 2056 6563  like.        Vec
-00011be0: 746f 7220 6f66 2069 6e74 6567 6572 7320  tor of integers 
-00011bf0: 746f 2077 7269 7465 0a0a 2020 2020 5265  to write..    Re
-00011c00: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00011c10: 2d0a 2020 2020 4e6f 6e65 0a0a 2020 2020  -.    None..    
-00011c20: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
-00011c30: 0a20 2020 2054 6869 7320 726f 7574 696e  .    This routin
-00011c40: 6520 6973 2074 7970 6963 616c 6c79 206e  e is typically n
-00011c50: 6f74 2063 616c 6c65 6420 6469 7265 6374  ot called direct
-00011c60: 6c79 2c20 6275 7420 636f 756c 6420 6265  ly, but could be
-00011c70: 2075 7365 6675 6c0a 2020 2020 746f 2077   useful.    to w
-00011c80: 7269 7465 2063 6172 6473 2074 6861 7420  rite cards that 
-00011c90: 6172 6520 6e6f 7420 616c 7265 6164 7920  are not already 
-00011ca0: 6163 636f 756e 7465 6420 666f 7220 696e  accounted for in
-00011cb0: 2074 6869 730a 2020 2020 6d6f 6475 6c65   this.    module
-00011cc0: 2e20 4173 2061 6e20 6578 616d 706c 6520  . As an example 
-00011cd0: 7573 6167 652c 2068 6572 6520 6973 2074  usage, here is t
-00011ce0: 6865 2063 6f64 6520 696e 7369 6465 0a20  he code inside. 
-00011cf0: 2020 203a 6675 6e63 3a60 7774 6373 7570     :func:`wtcsup
-00011d00: 6572 603a 3a0a 0a20 2020 2020 2020 2066  er`::..        f
-00011d10: 2e77 7269 7465 2866 2243 5355 5045 5220  .write(f"CSUPER 
-00011d20: 207b 7375 7065 7269 643a 3864 7d7b 303a   {superid:8d}{0:
-00011d30: 3864 7d22 290a 2020 2020 2020 2020 7774  8d}").        wt
-00011d40: 6e61 7369 6e74 7328 662c 2034 2c20 6772  nasints(f, 4, gr
-00011d50: 6964 7329 0a0a 2020 2020 4578 616d 706c  ids)..    Exampl
-00011d60: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
-00011d70: 2020 2020 3e3e 3e20 696d 706f 7274 206e      >>> import n
-00011d80: 756d 7079 2061 7320 6e70 0a20 2020 203e  umpy as np.    >
-00011d90: 3e3e 2066 726f 6d20 7079 7965 7469 2069  >> from pyyeti i
-00011da0: 6d70 6f72 7420 6e61 7374 7261 6e0a 2020  mport nastran.  
-00011db0: 2020 3e3e 3e20 6e61 7374 7261 6e2e 7774    >>> nastran.wt
-00011dc0: 6e61 7369 6e74 7328 312c 2032 2c20 6e70  nasints(1, 2, np
-00011dd0: 2e61 7261 6e67 6528 3238 2929 0a20 2020  .arange(28)).   
-00011de0: 2020 2020 2020 2020 3020 2020 2020 2020          0       
-00011df0: 3120 2020 2020 2020 3220 2020 2020 2020  1       2       
-00011e00: 3320 2020 2020 2020 3420 2020 2020 2020  3       4       
-00011e10: 3520 2020 2020 2020 3620 2020 2020 2020  5       6       
-00011e20: 370a 2020 2020 2020 2020 2020 2020 2020  7.              
-00011e30: 2020 2020 2038 2020 2020 2020 2039 2020       8       9  
-00011e40: 2020 2020 3130 2020 2020 2020 3131 2020      10      11  
-00011e50: 2020 2020 3132 2020 2020 2020 3133 2020      12      13  
-00011e60: 2020 2020 3134 2020 2020 2020 3135 0a20      14      15. 
-00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e80: 2031 3620 2020 2020 2031 3720 2020 2020   16      17     
-00011e90: 2031 3820 2020 2020 2031 3920 2020 2020   18      19     
-00011ea0: 2032 3020 2020 2020 2032 3120 2020 2020   20      21     
-00011eb0: 2032 3220 2020 2020 2032 330a 2020 2020   22      23.    
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 3234                24
-00011ed0: 2020 2020 2020 3235 2020 2020 2020 3236        25      26
-00011ee0: 2020 2020 2020 3237 0a20 2020 2022 2222        27.    """
-00011ef0: 0a20 2020 206e 203d 206c 656e 2869 6e74  .    n = len(int
-00011f00: 7329 0a20 2020 2066 6972 7374 6c69 6e65  s).    firstline
-00011f10: 203d 2031 3020 2d20 7374 6172 740a 2020   = 10 - start.  
-00011f20: 2020 6966 206e 203e 3d20 6669 7273 746c    if n >= firstl
-00011f30: 696e 653a 0a20 2020 2020 2020 2069 203d  ine:.        i =
-00011f40: 2066 6972 7374 6c69 6e65 0a20 2020 2020   firstline.     
-00011f50: 2020 2066 2e77 7269 7465 2828 227b 3a38     f.write(("{:8
-00011f60: 647d 2220 2a20 6920 2b20 225c 6e22 292e  d}" * i + "\n").
-00011f70: 666f 726d 6174 282a 696e 7473 5b3a 695d  format(*ints[:i]
-00011f80: 2929 0a20 2020 2020 2020 2077 6869 6c65  )).        while
-00011f90: 206e 203e 3d20 6920 2b20 383a 0a20 2020   n >= i + 8:.   
-00011fa0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00011fb0: 2828 227b 3a38 737d 2220 2b20 227b 3a38  (("{:8s}" + "{:8
-00011fc0: 647d 2220 2a20 3820 2b20 225c 6e22 292e  d}" * 8 + "\n").
-00011fd0: 666f 726d 6174 2822 222c 202a 696e 7473  format("", *ints
-00011fe0: 5b69 203a 2069 202b 2038 5d29 290a 2020  [i : i + 8])).  
-00011ff0: 2020 2020 2020 2020 2020 6920 2b3d 2038            i += 8
-00012000: 0a20 2020 2020 2020 2069 6620 6e20 3e20  .        if n > 
-00012010: 693a 0a20 2020 2020 2020 2020 2020 206e  i:.            n
-00012020: 202d 3d20 690a 2020 2020 2020 2020 2020   -= i.          
-00012030: 2020 662e 7772 6974 6528 2822 7b3a 3873    f.write(("{:8s
-00012040: 7d22 202b 2022 7b3a 3864 7d22 202a 206e  }" + "{:8d}" * n
-00012050: 202b 2022 5c6e 2229 2e66 6f72 6d61 7428   + "\n").format(
-00012060: 2222 2c20 2a69 6e74 735b 693a 5d29 290a  "", *ints[i:])).
-00012070: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012080: 2020 662e 7772 6974 6528 2822 7b3a 3864    f.write(("{:8d
-00012090: 7d22 202a 206e 202b 2022 5c6e 2229 2e66  }" * n + "\n").f
-000120a0: 6f72 6d61 7428 2a69 6e74 7329 290a 0a0a  ormat(*ints))...
-000120b0: 6465 6620 7264 6373 7570 6572 7328 6629  def rdcsupers(f)
-000120c0: 3a0a 2020 2020 7222 2222 0a20 2020 2052  :.    r""".    R
-000120d0: 6561 6420 4353 5550 4552 2065 6e74 7269  ead CSUPER entri
-000120e0: 6573 0a0a 2020 2020 5061 7261 6d65 7465  es..    Paramete
-000120f0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00012100: 2d0a 2020 2020 6620 3a20 7374 7269 6e67  -.    f : string
-00012110: 206f 7220 6669 6c65 5f6c 696b 6520 6f72   or file_like or
-00012120: 204e 6f6e 650a 2020 2020 2020 2020 4569   None.        Ei
-00012130: 7468 6572 2061 2066 696c 656e 616d 652c  ther a filename,
-00012140: 206f 7220 6973 2061 2066 696c 655f 6c69   or is a file_li
-00012150: 6b65 206f 626a 6563 7420 6173 2072 6574  ke object as ret
-00012160: 7572 6e65 640a 2020 2020 2020 2020 6279  urned.        by
-00012170: 203a 6675 6e63 3a60 6f70 656e 602e 2049   :func:`open`. I
-00012180: 6620 6669 6c65 5f6c 696b 6520 6f62 6a65  f file_like obje
-00012190: 6374 2c20 6974 2069 7320 7265 776f 756e  ct, it is rewoun
-000121a0: 6420 6669 7273 742e 2043 616e 0a20 2020  d first. Can.   
-000121b0: 2020 2020 2061 6c73 6f20 6265 2074 6865       also be the
-000121c0: 206e 616d 6520 6f66 2061 2064 6972 6563   name of a direc
-000121d0: 746f 7279 206f 7220 4e6f 6e65 3b20 696e  tory or None; in
-000121e0: 2074 6865 7365 2063 6173 6573 2c20 6120   these cases, a 
-000121f0: 4755 490a 2020 2020 2020 2020 6973 206f  GUI.        is o
-00012200: 7065 6e65 6420 666f 7220 6669 6c65 2073  pened for file s
-00012210: 656c 6563 7469 6f6e 2e0a 0a20 2020 2052  election...    R
-00012220: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00012230: 2d2d 0a20 2020 2064 6963 7469 6f6e 6172  --.    dictionar
-00012240: 790a 2020 2020 2020 2020 5468 6520 6469  y.        The di
-00012250: 6374 696f 6e61 7279 206b 6579 7320 6172  ctionary keys ar
-00012260: 6520 7468 6520 4353 5550 4552 2049 4473  e the CSUPER IDs
-00012270: 2e20 5468 6520 6469 6374 696f 6e61 7279  . The dictionary
-00012280: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00012290: 6172 6520 616c 6c20 7468 6520 6964 7320  are all the ids 
-000122a0: 6672 6f6d 2074 6865 2043 5355 5045 5220  from the CSUPER 
-000122b0: 6361 7264 2069 6e20 7468 6520 666f 726d  card in the form
-000122c0: 3a20 5b63 7375 7065 725f 6964 2c20 302c  : [csuper_id, 0,
-000122d0: 0a20 2020 2020 2020 206e 6f64 655f 6964  .        node_id
-000122e0: 5f31 2c20 6e6f 6465 5f69 645f 322c 20e2  _1, node_id_2, .
-000122f0: 80a6 206e 6f64 655f 6964 5f6e 5d0a 0a20  .. node_id_n].. 
-00012300: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-00012310: 2d2d 0a20 2020 2041 6e79 2022 5448 5255  --.    Any "THRU
-00012320: 2220 6669 656c 6473 2077 696c 6c20 6265  " fields will be
-00012330: 2073 6574 2074 6f20 2d31 2e20 5468 6973   set to -1. This
-00012340: 2072 6f75 7469 6e65 2073 696d 706c 7920   routine simply 
-00012350: 6361 6c6c 7320 7468 650a 2020 2020 6d6f  calls the.    mo
-00012360: 7265 2067 656e 6572 616c 2072 6f75 7469  re general routi
-00012370: 6e65 203a 6675 6e63 3a60 7264 6361 7264  ne :func:`rdcard
-00012380: 7360 3a3a 0a0a 2020 2020 2020 2020 7264  s`::..        rd
-00012390: 6361 7264 7328 662c 2027 6373 7570 6572  cards(f, 'csuper
-000123a0: 272c 2072 6574 7572 6e5f 7661 723d 2764  ', return_var='d
-000123b0: 6963 7427 2c20 6474 7970 653d 6e70 2e69  ict', dtype=np.i
-000123c0: 6e74 3634 2c20 626c 616e 6b3d 2d31 290a  nt64, blank=-1).
-000123d0: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-000123e0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e    --------.    >
-000123f0: 3e3e 2069 6d70 6f72 7420 6e75 6d70 7920  >> import numpy 
-00012400: 6173 206e 700a 2020 2020 3e3e 3e20 6672  as np.    >>> fr
-00012410: 6f6d 2070 7979 6574 6920 696d 706f 7274  om pyyeti import
-00012420: 206e 6173 7472 616e 0a20 2020 203e 3e3e   nastran.    >>>
-00012430: 2066 726f 6d20 696f 2069 6d70 6f72 7420   from io import 
-00012440: 5374 7269 6e67 494f 0a20 2020 203e 3e3e  StringIO.    >>>
-00012450: 206e 702e 7365 745f 7072 696e 746f 7074   np.set_printopt
-00012460: 696f 6e73 286c 696e 6577 6964 7468 3d36  ions(linewidth=6
-00012470: 3029 0a20 2020 203e 3e3e 2066 203d 2053  0).    >>> f = S
-00012480: 7472 696e 6749 4f28 2243 5355 5045 522c  tringIO("CSUPER,
-00012490: 3130 312c 302c 332c 3131 2c31 392c 3237  101,0,3,11,19,27
-000124a0: 2c31 3939 3530 3031 2c31 3939 3530 3032  ,1995001,1995002
-000124b0: 5c6e 220a 2020 2020 2e2e 2e20 2020 2020  \n".    ...     
-000124c0: 2020 2020 2020 2020 2022 2c31 3939 3530           ",19950
-000124d0: 3033 2c74 6872 752c 3139 3935 3031 3020  03,thru,1995010 
-000124e0: 2024 2063 6f6d 6d65 6e74 2229 0a20 2020   $ comment").   
-000124f0: 203e 3e3e 206e 6173 7472 616e 2e72 6463   >>> nastran.rdc
-00012500: 7375 7065 7273 2866 2920 2020 2020 2020  supers(f)       
-00012510: 2020 2020 2020 2320 646f 6374 6573 743a        # doctest:
-00012520: 202b 454c 4c49 5053 4953 0a20 2020 207b   +ELLIPSIS.    {
-00012530: 3130 313a 2061 7272 6179 285b 2020 2020  101: array([    
-00012540: 3130 312c 2020 2020 2020 2030 2c20 2020  101,       0,   
-00012550: 2020 2020 332c 2020 2020 2020 3131 2c20      3,      11, 
-00012560: 2020 2020 2031 392c 2020 2020 2020 3237       19,      27
-00012570: 2c0a 2020 2020 2020 2020 2020 2031 3939  ,.           199
-00012580: 3530 3031 2c20 3139 3935 3030 322c 2031  5001, 1995002, 1
-00012590: 3939 3530 3033 2c20 2020 2020 202d 312c  995003,      -1,
-000125a0: 2031 3939 3530 3130 5d2e 2e2e 297d 0a20   1995010]...)}. 
-000125b0: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
-000125c0: 6e20 7264 6361 7264 7328 662c 2022 6373  n rdcards(f, "cs
-000125d0: 7570 6572 222c 2072 6574 7572 6e5f 7661  uper", return_va
-000125e0: 723d 2264 6963 7422 2c20 6474 7970 653d  r="dict", dtype=
-000125f0: 6e70 2e69 6e74 3634 2c20 626c 616e 6b3d  np.int64, blank=
-00012600: 2d31 290a 0a0a 6465 6620 7264 6578 7472  -1)...def rdextr
-00012610: 6e28 662c 2065 7870 616e 643d 5472 7565  n(f, expand=True
-00012620: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
-00012630: 5265 6164 2045 5854 524e 2065 6e74 7279  Read EXTRN entry
-00012640: 2066 726f 6d20 2e70 6368 2066 696c 6520   from .pch file 
-00012650: 6372 6561 7465 6420 6279 204e 6173 7472  created by Nastr
-00012660: 616e 0a0a 2020 2020 5061 7261 6d65 7465  an..    Paramete
-00012670: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00012680: 2d0a 2020 2020 6620 3a20 7374 7269 6e67  -.    f : string
-00012690: 206f 7220 6669 6c65 5f6c 696b 6520 6f72   or file_like or
-000126a0: 204e 6f6e 650a 2020 2020 2020 2020 4569   None.        Ei
-000126b0: 7468 6572 2061 206e 616d 6520 6f66 2061  ther a name of a
-000126c0: 2066 696c 652c 206f 7220 6973 2061 2066   file, or is a f
-000126d0: 696c 655f 6c69 6b65 206f 626a 6563 7420  ile_like object 
-000126e0: 6173 2072 6574 7572 6e65 640a 2020 2020  as returned.    
-000126f0: 2020 2020 6279 203a 6675 6e63 3a60 6f70      by :func:`op
-00012700: 656e 602e 2049 6620 6669 6c65 5f6c 696b  en`. If file_lik
-00012710: 6520 6f62 6a65 6374 2c20 6974 2069 7320  e object, it is 
-00012720: 7265 776f 756e 6420 6669 7273 742e 2043  rewound first. C
-00012730: 616e 0a20 2020 2020 2020 2061 6c73 6f20  an.        also 
-00012740: 6265 2074 6865 206e 616d 6520 6f66 2061  be the name of a
-00012750: 2064 6972 6563 746f 7279 206f 7220 4e6f   directory or No
-00012760: 6e65 3b20 696e 2074 6865 7365 2063 6173  ne; in these cas
-00012770: 6573 2c20 6120 4755 490a 2020 2020 2020  es, a GUI.      
-00012780: 2020 6973 206f 7065 6e65 6420 666f 7220    is opened for 
-00012790: 6669 6c65 2073 656c 6563 7469 6f6e 2e0a  file selection..
-000127a0: 2020 2020 6578 7061 6e64 203a 2062 6f6f      expand : boo
-000127b0: 6c3b 206f 7074 696f 6e61 6c0a 2020 2020  l; optional.    
-000127c0: 2020 2020 4966 2054 7275 652c 2065 7870      If True, exp
-000127d0: 616e 6420 726f 7773 206c 696b 6520 7468  and rows like th
-000127e0: 6973 3a3a 0a0a 2020 2020 2020 2020 2020  is::..          
-000127f0: 2020 5b31 3030 2c20 3132 3334 3536 5d0a    [100, 123456].
-00012800: 0a20 2020 2020 2020 2069 6e74 6f20 3620  .        into 6 
-00012810: 7365 7061 7261 7465 2072 6f77 7320 6c69  separate rows li
-00012820: 6b65 2074 6869 733a 3a0a 0a20 2020 2020  ke this::..     
-00012830: 2020 2020 2020 205b 3130 302c 2031 5d2c         [100, 1],
-00012840: 0a20 2020 2020 2020 2020 2020 205b 3130  .            [10
-00012850: 302c 2032 5d2c 0a20 2020 2020 2020 2020  0, 2],.         
-00012860: 2020 205b 3130 302c 2033 5d2c 0a20 2020     [100, 3],.   
-00012870: 2020 2020 2020 2020 205b 3130 302c 2034           [100, 4
-00012880: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00012890: 3130 302c 2035 5d2c 0a20 2020 2020 2020  100, 5],.       
-000128a0: 2020 2020 205b 3130 302c 2036 5d2c 0a0a       [100, 6],..
-000128b0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000128c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 3264 206e  -------.    2d n
-000128d0: 6461 7272 6179 0a20 2020 2020 2020 2054  darray.        T
-000128e0: 776f 2063 6f6c 756d 6e20 6172 7261 793a  wo column array:
-000128f0: 205b 4944 2c20 444f 465d 0a0a 2020 2020   [ID, DOF]..    
-00012900: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
-00012910: 2020 2020 5468 6520 6578 7061 6e73 696f      The expansio
-00012920: 6e20 6973 2064 6f6e 6520 6279 203a 6675  n is done by :fu
-00012930: 6e63 3a60 7079 7965 7469 2e6e 6173 7472  nc:`pyyeti.nastr
-00012940: 616e 2e6e 3270 2e65 7870 616e 6464 6f66  an.n2p.expanddof
-00012950: 602e 0a0a 2020 2020 4578 616d 706c 6573  `...    Examples
-00012960: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-00012970: 2020 3e3e 3e20 6672 6f6d 2070 7979 6574    >>> from pyyet
-00012980: 6920 696d 706f 7274 206e 6173 7472 616e  i import nastran
-00012990: 0a20 2020 203e 3e3e 2066 726f 6d20 696f  .    >>> from io
-000129a0: 2069 6d70 6f72 7420 5374 7269 6e67 494f   import StringIO
-000129b0: 0a20 2020 203e 3e3e 2066 203d 2053 7472  .    >>> f = Str
-000129c0: 696e 6749 4f28 2745 5854 524e 2c33 2c31  ingIO('EXTRN,3,1
-000129d0: 3233 3435 362c 3131 2c31 3233 3435 362c  23456,11,123456,
-000129e0: 3139 2c31 3233 3435 362c 3237 2c31 3233  19,123456,27,123
-000129f0: 3435 365c 6e27 0a20 2020 202e 2e2e 2020  456\n'.    ...  
-00012a00: 2020 2020 2020 2020 2020 2020 272c 3239              ',29
-00012a10: 3935 3030 312c 302c 3239 3935 3030 322c  95001,0,2995002,
-00012a20: 302c 3239 3935 3030 332c 302c 3239 3935  0,2995003,0,2995
-00012a30: 3030 342c 305c 6e27 0a20 2020 202e 2e2e  004,0\n'.    ...
-00012a40: 2020 2020 2020 2020 2020 2020 2020 272c                ',
-00012a50: 3239 3935 3030 352c 302c 3239 3935 3030  2995005,0,299500
-00012a60: 362c 302c 3239 3935 3030 372c 302c 3239  6,0,2995007,0,29
-00012a70: 3935 3030 382c 305c 6e27 290a 2020 2020  95008,0\n').    
-00012a80: 3e3e 3e20 6e61 7374 7261 6e2e 7264 6578  >>> nastran.rdex
-00012a90: 7472 6e28 662c 2065 7870 616e 643d 4661  trn(f, expand=Fa
-00012aa0: 6c73 6529 2020 2023 2064 6f63 7465 7374  lse)   # doctest
-00012ab0: 3a20 2b45 4c4c 4950 5349 530a 2020 2020  : +ELLIPSIS.    
-00012ac0: 6172 7261 7928 5b5b 2020 2020 2020 332c  array([[      3,
-00012ad0: 2020 3132 3334 3536 5d2c 0a20 2020 2020    123456],.     
-00012ae0: 2020 2020 2020 5b20 2020 2020 3131 2c20        [     11, 
-00012af0: 2031 3233 3435 365d 2c0a 2020 2020 2020   123456],.      
-00012b00: 2020 2020 205b 2020 2020 2031 392c 2020       [     19,  
-00012b10: 3132 3334 3536 5d2c 0a20 2020 2020 2020  123456],.       
-00012b20: 2020 2020 5b20 2020 2020 3237 2c20 2031      [     27,  1
-00012b30: 3233 3435 365d 2c0a 2020 2020 2020 2020  23456],.        
-00012b40: 2020 205b 3239 3935 3030 312c 2020 2020     [2995001,    
-00012b50: 2020 2030 5d2c 0a20 2020 2020 2020 2020     0],.         
-00012b60: 2020 5b32 3939 3530 3032 2c20 2020 2020    [2995002,     
-00012b70: 2020 305d 2c0a 2020 2020 2020 2020 2020    0],.          
-00012b80: 205b 3239 3935 3030 332c 2020 2020 2020   [2995003,      
-00012b90: 2030 5d2c 0a20 2020 2020 2020 2020 2020   0],.           
-00012ba0: 5b32 3939 3530 3034 2c20 2020 2020 2020  [2995004,       
-00012bb0: 305d 2c0a 2020 2020 2020 2020 2020 205b  0],.           [
-00012bc0: 3239 3935 3030 352c 2020 2020 2020 2030  2995005,       0
-00012bd0: 5d2c 0a20 2020 2020 2020 2020 2020 5b32  ],.           [2
-00012be0: 3939 3530 3036 2c20 2020 2020 2020 305d  995006,       0]
-00012bf0: 2c0a 2020 2020 2020 2020 2020 205b 3239  ,.           [29
-00012c00: 3935 3030 372c 2020 2020 2020 2030 5d2c  95007,       0],
-00012c10: 0a20 2020 2020 2020 2020 2020 5b32 3939  .           [299
-00012c20: 3530 3038 2c20 2020 2020 2020 305d 5d2e  5008,       0]].
-00012c30: 2e2e 290a 2020 2020 3e3e 3e20 6620 3d20  ..).    >>> f = 
-00012c40: 5374 7269 6e67 494f 2827 4558 5452 4e2c  StringIO('EXTRN,
-00012c50: 332c 3132 3334 3536 2c32 3939 3530 3031  3,123456,2995001
-00012c60: 2c30 2729 0a20 2020 203e 3e3e 206e 6173  ,0').    >>> nas
-00012c70: 7472 616e 2e72 6465 7874 726e 2866 2920  tran.rdextrn(f) 
-00012c80: 2020 2020 2020 2020 2020 2020 2320 646f              # do
-00012c90: 6374 6573 743a 202b 454c 4c49 5053 4953  ctest: +ELLIPSIS
-00012ca0: 0a20 2020 2061 7272 6179 285b 5b20 2020  .    array([[   
-00012cb0: 2020 2033 2c20 2020 2020 2020 315d 2c0a     3,       1],.
-00012cc0: 2020 2020 2020 2020 2020 205b 2020 2020             [    
-00012cd0: 2020 332c 2020 2020 2020 2032 5d2c 0a20    3,       2],. 
-00012ce0: 2020 2020 2020 2020 2020 5b20 2020 2020            [     
-00012cf0: 2033 2c20 2020 2020 2020 335d 2c0a 2020   3,       3],.  
-00012d00: 2020 2020 2020 2020 205b 2020 2020 2020           [      
-00012d10: 332c 2020 2020 2020 2034 5d2c 0a20 2020  3,       4],.   
-00012d20: 2020 2020 2020 2020 5b20 2020 2020 2033          [      3
-00012d30: 2c20 2020 2020 2020 355d 2c0a 2020 2020  ,       5],.    
-00012d40: 2020 2020 2020 205b 2020 2020 2020 332c         [      3,
-00012d50: 2020 2020 2020 2036 5d2c 0a20 2020 2020         6],.     
-00012d60: 2020 2020 2020 5b32 3939 3530 3031 2c20        [2995001, 
-00012d70: 2020 2020 2020 305d 5d2e 2e2e 290a 2020        0]]...).  
-00012d80: 2020 2222 220a 2020 2020 6578 7472 6e20    """.    extrn 
-00012d90: 3d20 7264 6361 7264 7328 662c 2022 6578  = rdcards(f, "ex
-00012da0: 7472 6e22 2c20 6474 7970 653d 6e70 2e69  trn", dtype=np.i
-00012db0: 6e74 3634 292e 7265 7368 6170 6528 2d31  nt64).reshape(-1
-00012dc0: 2c20 3229 0a20 2020 2069 6620 6578 7061  , 2).    if expa
-00012dd0: 6e64 3a0a 2020 2020 2020 2020 6578 7472  nd:.        extr
-00012de0: 6e20 3d20 6e32 702e 6578 7061 6e64 646f  n = n2p.expanddo
-00012df0: 6628 6578 7472 6e29 0a20 2020 2072 6574  f(extrn).    ret
-00012e00: 7572 6e20 6578 7472 6e0a 0a0a 4067 7569  urn extrn...@gui
-00012e10: 746f 6f6c 732e 7772 6974 655f 7465 7874  tools.write_text
-00012e20: 5f66 696c 650a 6465 6620 7774 6373 7570  _file.def wtcsup
-00012e30: 6572 2866 2c20 7375 7065 7269 642c 2067  er(f, superid, g
-00012e40: 7269 6473 293a 0a20 2020 2022 2222 0a20  rids):.    """. 
-00012e50: 2020 2057 7269 7465 7320 6120 4e61 7374     Writes a Nast
-00012e60: 7261 6e20 4353 5550 4552 2063 6172 6420  ran CSUPER card 
-00012e70: 746f 2061 2066 696c 652e 0a0a 2020 2020  to a file...    
-00012e80: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00012e90: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6620  ---------.    f 
-00012ea0: 3a20 7374 7269 6e67 206f 7220 6669 6c65  : string or file
-00012eb0: 5f6c 696b 6520 6f72 2031 206f 7220 4e6f  _like or 1 or No
-00012ec0: 6e65 0a20 2020 2020 2020 2045 6974 6865  ne.        Eithe
-00012ed0: 7220 6120 6e61 6d65 206f 6620 6120 6669  r a name of a fi
-00012ee0: 6c65 2c20 6f72 2069 7320 6120 6669 6c65  le, or is a file
-00012ef0: 5f6c 696b 6520 6f62 6a65 6374 2061 7320  _like object as 
-00012f00: 7265 7475 726e 6564 0a20 2020 2020 2020  returned.       
-00012f10: 2062 7920 3a66 756e 633a 606f 7065 6e60   by :func:`open`
-00012f20: 206f 7220 3a63 6c61 7373 3a60 696f 2e53   or :class:`io.S
-00012f30: 7472 696e 6749 4f60 2e20 496e 7075 7420  tringIO`. Input 
-00012f40: 6173 2069 6e74 6567 6572 2031 2074 6f0a  as integer 1 to.
-00012f50: 2020 2020 2020 2020 7772 6974 6520 746f          write to
-00012f60: 2073 7464 6f75 742e 2043 616e 2061 6c73   stdout. Can als
-00012f70: 6f20 6265 2074 6865 206e 616d 6520 6f66  o be the name of
-00012f80: 2061 2064 6972 6563 746f 7279 206f 7220   a directory or 
-00012f90: 4e6f 6e65 3b0a 2020 2020 2020 2020 696e  None;.        in
-00012fa0: 2074 6865 7365 2063 6173 6573 2c20 6120   these cases, a 
-00012fb0: 4755 4920 6973 206f 7065 6e65 6420 666f  GUI is opened fo
-00012fc0: 7220 6669 6c65 2073 656c 6563 7469 6f6e  r file selection
-00012fd0: 2e0a 2020 2020 7375 7065 7269 6420 3a20  ..    superid : 
-00012fe0: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-00012ff0: 5375 7065 7265 6c65 6d65 6e74 2049 440a  Superelement ID.
-00013000: 2020 2020 6772 6964 7320 3a20 3164 2061      grids : 1d a
-00013010: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
-00013020: 2020 5665 6374 6f72 206f 6620 6772 6964    Vector of grid
-00013030: 2069 6473 2e0a 0a20 2020 2052 6574 7572   ids...    Retur
-00013040: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00013050: 2020 204e 6f6e 650a 0a20 2020 2045 7861     None..    Exa
-00013060: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
-00013070: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
-00013080: 7079 7965 7469 2069 6d70 6f72 7420 6e61  pyyeti import na
-00013090: 7374 7261 6e0a 2020 2020 3e3e 3e20 696d  stran.    >>> im
-000130a0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-000130b0: 0a20 2020 203e 3e3e 206e 6173 7472 616e  .    >>> nastran
-000130c0: 2e77 7463 7375 7065 7228 312c 2031 3030  .wtcsuper(1, 100
-000130d0: 2c20 6e70 2e61 7261 6e67 6528 312c 2031  , np.arange(1, 1
-000130e0: 3029 290a 2020 2020 4353 5550 4552 2020  0)).    CSUPER  
-000130f0: 2020 2020 2031 3030 2020 2020 2020 2030       100       0
-00013100: 2020 2020 2020 2031 2020 2020 2020 2032         1       2
-00013110: 2020 2020 2020 2033 2020 2020 2020 2034         3       4
-00013120: 2020 2020 2020 2035 2020 2020 2020 2036         5       6
-00013130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013140: 2020 2020 3720 2020 2020 2020 3820 2020      7       8   
-00013150: 2020 2020 390a 2020 2020 2222 220a 2020      9.    """.  
-00013160: 2020 662e 7772 6974 6528 6622 4353 5550    f.write(f"CSUP
-00013170: 4552 2020 7b73 7570 6572 6964 3a38 647d  ER  {superid:8d}
-00013180: 7b30 3a38 647d 2229 0a20 2020 2077 746e  {0:8d}").    wtn
-00013190: 6173 696e 7473 2866 2c20 342c 2067 7269  asints(f, 4, gri
-000131a0: 6473 290a 0a0a 4067 7569 746f 6f6c 732e  ds)...@guitools.
-000131b0: 7772 6974 655f 7465 7874 5f66 696c 650a  write_text_file.
-000131c0: 6465 6620 7774 7370 6331 2866 2c20 6569  def wtspc1(f, ei
-000131d0: 642c 2064 6f66 2c20 6772 6964 732c 206e  d, dof, grids, n
-000131e0: 616d 653d 2253 5043 3122 293a 0a20 2020  ame="SPC1"):.   
-000131f0: 2022 2222 0a20 2020 2057 7269 7465 7320   """.    Writes 
-00013200: 6120 4e61 7374 7261 6e20 5350 4331 2028  a Nastran SPC1 (
-00013210: 6f72 2073 696d 696c 6172 2920 6361 7264  or similar) card
-00013220: 2074 6f20 6120 6669 6c65 2e0a 0a20 2020   to a file...   
-00013230: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00013240: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066  ----------.    f
-00013250: 203a 2073 7472 696e 6720 6f72 2066 696c   : string or fil
-00013260: 655f 6c69 6b65 206f 7220 3120 6f72 204e  e_like or 1 or N
-00013270: 6f6e 650a 2020 2020 2020 2020 4569 7468  one.        Eith
-00013280: 6572 2061 206e 616d 6520 6f66 2061 2066  er a name of a f
-00013290: 696c 652c 206f 7220 6973 2061 2066 696c  ile, or is a fil
-000132a0: 655f 6c69 6b65 206f 626a 6563 7420 6173  e_like object as
-000132b0: 2072 6574 7572 6e65 640a 2020 2020 2020   returned.      
-000132c0: 2020 6279 203a 6675 6e63 3a60 6f70 656e    by :func:`open
-000132d0: 6020 6f72 203a 636c 6173 733a 6069 6f2e  ` or :class:`io.
-000132e0: 5374 7269 6e67 494f 602e 2049 6e70 7574  StringIO`. Input
-000132f0: 2061 7320 696e 7465 6765 7220 3120 746f   as integer 1 to
-00013300: 0a20 2020 2020 2020 2077 7269 7465 2074  .        write t
-00013310: 6f20 7374 646f 7574 2e20 4361 6e20 616c  o stdout. Can al
-00013320: 736f 2062 6520 7468 6520 6e61 6d65 206f  so be the name o
-00013330: 6620 6120 6469 7265 6374 6f72 7920 6f72  f a directory or
-00013340: 204e 6f6e 653b 0a20 2020 2020 2020 2069   None;.        i
-00013350: 6e20 7468 6573 6520 6361 7365 732c 2061  n these cases, a
-00013360: 2047 5549 2069 7320 6f70 656e 6564 2066   GUI is opened f
-00013370: 6f72 2066 696c 6520 7365 6c65 6374 696f  or file selectio
-00013380: 6e2e 0a20 2020 2065 6964 203a 2069 6e74  n..    eid : int
-00013390: 6567 6572 0a20 2020 2020 2020 2045 6c65  eger.        Ele
-000133a0: 6d65 6e74 2049 440a 2020 2020 646f 6620  ment ID.    dof 
-000133b0: 3a20 696e 7465 6765 720a 2020 2020 2020  : integer.      
-000133c0: 2020 416e 2069 6e74 6567 6572 2063 6f6e    An integer con
-000133d0: 6361 7465 6e61 7469 6f6e 206f 6620 7468  catenation of th
-000133e0: 6520 444f 4620 2865 783a 2031 3233 3435  e DOF (ex: 12345
-000133f0: 3629 0a20 2020 2067 7269 6473 203a 2031  6).    grids : 1
-00013400: 6420 6172 7261 795f 6c69 6b65 0a20 2020  d array_like.   
-00013410: 2020 2020 2056 6563 746f 7220 6f66 2067       Vector of g
-00013420: 7269 6420 6964 732e 0a20 2020 206e 616d  rid ids..    nam
-00013430: 6520 3a20 7374 7269 6e67 3b20 6f70 7469  e : string; opti
-00013440: 6f6e 616c 0a20 2020 2020 2020 204e 616d  onal.        Nam
-00013450: 6520 6f66 204e 4153 5452 414e 2063 6172  e of NASTRAN car
-00013460: 6420 746f 2077 7269 7465 3b20 6361 7264  d to write; card
-00013470: 206d 7573 7420 6265 2069 6e20 7361 6d65   must be in same
-00013480: 2066 6f72 6d61 7420 6173 0a20 2020 2020   format as.     
-00013490: 2020 2074 6865 2053 5043 3120 6361 7264     the SPC1 card
-000134a0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-000134b0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 204e     -------.    N
-000134c0: 6f6e 650a 0a20 2020 2045 7861 6d70 6c65  one..    Example
-000134d0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-000134e0: 2020 203e 3e3e 2066 726f 6d20 7079 7965     >>> from pyye
-000134f0: 7469 2069 6d70 6f72 7420 6e61 7374 7261  ti import nastra
-00013500: 6e0a 2020 2020 3e3e 3e20 696d 706f 7274  n.    >>> import
-00013510: 206e 756d 7079 2061 7320 6e70 0a20 2020   numpy as np.   
-00013520: 203e 3e3e 206e 6173 7472 616e 2e77 7473   >>> nastran.wts
-00013530: 7063 3128 312c 2031 2c20 3132 3334 3536  pc1(1, 1, 123456
-00013540: 2c20 6e70 2e61 7261 6e67 6528 312c 2031  , np.arange(1, 1
-00013550: 3029 290a 2020 2020 5350 4331 2020 2020  0)).    SPC1    
-00013560: 2020 2020 2020 2031 2020 3132 3334 3536         1  123456
-00013570: 2020 2020 2020 2031 2020 2020 2020 2032         1       2
-00013580: 2020 2020 2020 2033 2020 2020 2020 2034         3       4
-00013590: 2020 2020 2020 2035 2020 2020 2020 2036         5       6
-000135a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000135b0: 2020 2020 3720 2020 2020 2020 3820 2020      7       8   
-000135c0: 2020 2020 390a 2020 2020 3e3e 3e20 6e61      9.    >>> na
-000135d0: 7374 7261 6e2e 7774 7370 6331 2831 2c20  stran.wtspc1(1, 
-000135e0: 3230 302c 2031 3233 3435 362c 206e 702e  200, 123456, np.
-000135f0: 6172 616e 6765 2832 3030 312c 2032 3033  arange(2001, 203
-00013600: 3129 2c0a 2020 2020 2e2e 2e20 2020 2020  1),.    ...     
-00013610: 2020 2020 2020 2020 2020 2027 5345 5153             'SEQS
-00013620: 4554 3127 290a 2020 2020 5345 5153 4554  ET1').    SEQSET
-00013630: 3120 2020 2020 2032 3030 2020 3132 3334  1      200  1234
-00013640: 3536 2020 2020 3230 3031 2020 2020 3230  56    2001    20
-00013650: 3032 2020 2020 3230 3033 2020 2020 3230  02    2003    20
-00013660: 3034 2020 2020 3230 3035 2020 2020 3230  04    2005    20
-00013670: 3036 0a20 2020 2020 2020 2020 2020 2020  06.             
-00013680: 2020 2032 3030 3720 2020 2032 3030 3820     2007    2008 
-00013690: 2020 2032 3030 3920 2020 2032 3031 3020     2009    2010 
-000136a0: 2020 2032 3031 3120 2020 2032 3031 3220     2011    2012 
-000136b0: 2020 2032 3031 3320 2020 2032 3031 340a     2013    2014.
-000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136d0: 3230 3135 2020 2020 3230 3136 2020 2020  2015    2016    
-000136e0: 3230 3137 2020 2020 3230 3138 2020 2020  2017    2018    
-000136f0: 3230 3139 2020 2020 3230 3230 2020 2020  2019    2020    
-00013700: 3230 3231 2020 2020 3230 3232 0a20 2020  2021    2022.   
-00013710: 2020 2020 2020 2020 2020 2020 2032 3032               202
-00013720: 3320 2020 2032 3032 3420 2020 2032 3032  3    2024    202
-00013730: 3520 2020 2032 3032 3620 2020 2032 3032  5    2026    202
-00013740: 3720 2020 2032 3032 3820 2020 2032 3032  7    2028    202
-00013750: 3920 2020 2032 3033 300a 2020 2020 2222  9    2030.    ""
-00013760: 220a 2020 2020 662e 7772 6974 6528 6622  ".    f.write(f"
-00013770: 7b6e 616d 653a 3c38 737d 7b65 6964 3a38  {name:<8s}{eid:8
-00013780: 647d 7b64 6f66 3a38 647d 2229 0a20 2020  d}{dof:8d}").   
-00013790: 2077 746e 6173 696e 7473 2866 2c20 342c   wtnasints(f, 4,
-000137a0: 2067 7269 6473 290a 0a0a 4067 7569 746f   grids)...@guito
-000137b0: 6f6c 732e 7772 6974 655f 7465 7874 5f66  ols.write_text_f
-000137c0: 696c 650a 6465 6620 7774 7873 6574 3128  ile.def wtxset1(
-000137d0: 662c 2064 6f66 2c20 6772 6964 732c 206e  f, dof, grids, n
-000137e0: 616d 653d 2242 5345 5431 2229 3a0a 2020  ame="BSET1"):.  
-000137f0: 2020 2222 220a 2020 2020 5772 6974 6573    """.    Writes
-00013800: 2061 204e 6173 7472 616e 2042 5345 5431   a Nastran BSET1
-00013810: 2c20 5153 4554 3120 286f 7220 7369 6d69  , QSET1 (or simi
-00013820: 6c61 7229 2063 6172 6420 746f 2061 2066  lar) card to a f
-00013830: 696c 652e 0a0a 2020 2020 5061 7261 6d65  ile...    Parame
-00013840: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00013850: 2d2d 2d0a 2020 2020 6620 3a20 7374 7269  ---.    f : stri
-00013860: 6e67 206f 7220 6669 6c65 5f6c 696b 6520  ng or file_like 
-00013870: 6f72 2031 206f 7220 4e6f 6e65 0a20 2020  or 1 or None.   
-00013880: 2020 2020 2045 6974 6865 7220 6120 6e61       Either a na
-00013890: 6d65 206f 6620 6120 6669 6c65 2c20 6f72  me of a file, or
-000138a0: 2069 7320 6120 6669 6c65 5f6c 696b 6520   is a file_like 
-000138b0: 6f62 6a65 6374 2061 7320 7265 7475 726e  object as return
-000138c0: 6564 0a20 2020 2020 2020 2062 7920 3a66  ed.        by :f
-000138d0: 756e 633a 606f 7065 6e60 206f 7220 3a63  unc:`open` or :c
-000138e0: 6c61 7373 3a60 696f 2e53 7472 696e 6749  lass:`io.StringI
-000138f0: 4f60 2e20 496e 7075 7420 6173 2069 6e74  O`. Input as int
-00013900: 6567 6572 2031 2074 6f0a 2020 2020 2020  eger 1 to.      
-00013910: 2020 7772 6974 6520 746f 2073 7464 6f75    write to stdou
-00013920: 742e 2043 616e 2061 6c73 6f20 6265 2074  t. Can also be t
-00013930: 6865 206e 616d 6520 6f66 2061 2064 6972  he name of a dir
-00013940: 6563 746f 7279 206f 7220 4e6f 6e65 3b0a  ectory or None;.
-00013950: 2020 2020 2020 2020 696e 2074 6865 7365          in these
-00013960: 2063 6173 6573 2c20 6120 4755 4920 6973   cases, a GUI is
-00013970: 206f 7065 6e65 6420 666f 7220 6669 6c65   opened for file
-00013980: 2073 656c 6563 7469 6f6e 2e0a 2020 2020   selection..    
-00013990: 646f 6620 3a20 696e 7465 6765 720a 2020  dof : integer.  
-000139a0: 2020 2020 2020 416e 2069 6e74 6567 6572        An integer
-000139b0: 2063 6f6e 6361 7465 6e61 7469 6f6e 206f   concatenation o
-000139c0: 6620 7468 6520 444f 4620 2865 783a 2031  f the DOF (ex: 1
-000139d0: 3233 3435 3629 0a20 2020 2067 7269 6473  23456).    grids
-000139e0: 203a 2031 6420 6172 7261 795f 6c69 6b65   : 1d array_like
-000139f0: 0a20 2020 2020 2020 2056 6563 746f 7220  .        Vector 
-00013a00: 6f66 2067 7269 6420 6964 732e 0a20 2020  of grid ids..   
-00013a10: 206e 616d 6520 3a20 7374 7269 6e67 3b20   name : string; 
-00013a20: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00013a30: 204e 616d 6520 6f66 204e 4153 5452 414e   Name of NASTRAN
-00013a40: 2063 6172 6420 746f 2077 7269 7465 3b20   card to write; 
-00013a50: 6361 7264 206d 7573 7420 6265 2069 6e20  card must be in 
-00013a60: 7361 6d65 2066 6f72 6d61 7420 6173 0a20  same format as. 
-00013a70: 2020 2020 2020 2074 6865 2053 5043 3120         the SPC1 
-00013a80: 6361 7264 2e0a 0a20 2020 2052 6574 7572  card...    Retur
-00013a90: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00013aa0: 2020 204e 6f6e 650a 0a20 2020 2045 7861     None..    Exa
-00013ab0: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
-00013ac0: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
-00013ad0: 7079 7965 7469 2069 6d70 6f72 7420 6e61  pyyeti import na
-00013ae0: 7374 7261 6e0a 2020 2020 3e3e 3e20 696d  stran.    >>> im
-00013af0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-00013b00: 0a20 2020 203e 3e3e 206e 6173 7472 616e  .    >>> nastran
-00013b10: 2e77 7478 7365 7431 2831 2c20 3132 3334  .wtxset1(1, 1234
-00013b20: 3536 2c20 6e70 2e61 7261 6e67 6528 312c  56, np.arange(1,
-00013b30: 2031 3129 290a 2020 2020 4253 4554 3120   11)).    BSET1 
-00013b40: 2020 2020 3132 3334 3536 2020 2020 2020      123456      
-00013b50: 2031 2020 2020 2020 2032 2020 2020 2020   1       2      
-00013b60: 2033 2020 2020 2020 2034 2020 2020 2020   3       4      
-00013b70: 2035 2020 2020 2020 2036 2020 2020 2020   5       6      
-00013b80: 2037 0a20 2020 2020 2020 2020 2020 2020   7.             
-00013b90: 2020 2020 2020 3820 2020 2020 2020 3920        8       9 
-00013ba0: 2020 2020 2031 300a 2020 2020 3e3e 3e20       10.    >>> 
-00013bb0: 6e61 7374 7261 6e2e 7774 7873 6574 3128  nastran.wtxset1(
-00013bc0: 312c 2030 2c20 6e70 2e61 7261 6e67 6528  1, 0, np.arange(
-00013bd0: 3230 3031 2c20 3230 3133 292c 2027 5153  2001, 2013), 'QS
-00013be0: 4554 3127 290a 2020 2020 5153 4554 3120  ET1').    QSET1 
-00013bf0: 2020 2020 2020 2020 2030 2020 2020 3230           0    20
-00013c00: 3031 2020 2020 3230 3032 2020 2020 3230  01    2002    20
-00013c10: 3033 2020 2020 3230 3034 2020 2020 3230  03    2004    20
-00013c20: 3035 2020 2020 3230 3036 2020 2020 3230  05    2006    20
-00013c30: 3037 0a20 2020 2020 2020 2020 2020 2020  07.             
-00013c40: 2020 2032 3030 3820 2020 2032 3030 3920     2008    2009 
-00013c50: 2020 2032 3031 3020 2020 2032 3031 3120     2010    2011 
-00013c60: 2020 2032 3031 320a 2020 2020 2222 220a     2012.    """.
-00013c70: 2020 2020 662e 7772 6974 6528 6622 7b6e      f.write(f"{n
-00013c80: 616d 653a 3c38 737d 7b64 6f66 3a38 647d  ame:<8s}{dof:8d}
-00013c90: 2229 0a20 2020 2077 746e 6173 696e 7473  ").    wtnasints
-00013ca0: 2866 2c20 332c 2067 7269 6473 290a 0a0a  (f, 3, grids)...
-00013cb0: 4067 7569 746f 6f6c 732e 7772 6974 655f  @guitools.write_
-00013cc0: 7465 7874 5f66 696c 650a 6465 6620 7774  text_file.def wt
-00013cd0: 7163 7365 7428 662c 2073 7461 7274 6772  qcset(f, startgr
-00013ce0: 6964 2c20 6e71 293a 0a20 2020 2022 2222  id, nq):.    """
-00013cf0: 0a20 2020 2057 7269 7465 7320 4e61 7374  .    Writes Nast
-00013d00: 7261 6e20 5153 4554 3120 616e 6420 4353  ran QSET1 and CS
-00013d10: 4554 3120 6361 7264 7320 666f 7220 4752  ET1 cards for GR
-00013d20: 4944 206d 6f64 616c 2044 4f46 2066 6f72  ID modal DOF for
-00013d30: 2075 7365 2069 6e0a 2020 2020 7468 6520   use in.    the 
-00013d40: 444d 4150 2022 7874 6d61 7472 6978 222e  DMAP "xtmatrix".
-00013d50: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00013d60: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00013d70: 2020 2020 6620 3a20 7374 7269 6e67 206f      f : string o
-00013d80: 7220 6669 6c65 5f6c 696b 6520 6f72 2031  r file_like or 1
-00013d90: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
-00013da0: 2045 6974 6865 7220 6120 6e61 6d65 206f   Either a name o
-00013db0: 6620 6120 6669 6c65 2c20 6f72 2069 7320  f a file, or is 
-00013dc0: 6120 6669 6c65 5f6c 696b 6520 6f62 6a65  a file_like obje
-00013dd0: 6374 2061 7320 7265 7475 726e 6564 0a20  ct as returned. 
-00013de0: 2020 2020 2020 2062 7920 3a66 756e 633a         by :func:
-00013df0: 606f 7065 6e60 206f 7220 3a63 6c61 7373  `open` or :class
-00013e00: 3a60 696f 2e53 7472 696e 6749 4f60 2e20  :`io.StringIO`. 
-00013e10: 496e 7075 7420 6173 2069 6e74 6567 6572  Input as integer
-00013e20: 2031 2074 6f0a 2020 2020 2020 2020 7772   1 to.        wr
-00013e30: 6974 6520 746f 2073 7464 6f75 742e 2043  ite to stdout. C
-00013e40: 616e 2061 6c73 6f20 6265 2074 6865 206e  an also be the n
-00013e50: 616d 6520 6f66 2061 2064 6972 6563 746f  ame of a directo
-00013e60: 7279 206f 7220 4e6f 6e65 3b0a 2020 2020  ry or None;.    
-00013e70: 2020 2020 696e 2074 6865 7365 2063 6173      in these cas
-00013e80: 6573 2c20 6120 4755 4920 6973 206f 7065  es, a GUI is ope
-00013e90: 6e65 6420 666f 7220 6669 6c65 2073 656c  ned for file sel
-00013ea0: 6563 7469 6f6e 2e0a 2020 2020 7374 6172  ection..    star
-00013eb0: 7467 7269 6420 3a20 696e 7465 6765 720a  tgrid : integer.
-00013ec0: 2020 2020 2020 2020 5468 6520 7374 6172          The star
-00013ed0: 7420 4944 2066 6f72 2074 6865 206d 6f64  t ID for the mod
-00013ee0: 616c 2067 7269 6473 2074 6861 7420 6e65  al grids that ne
-00013ef0: 6564 2074 6f20 6265 2061 7373 6967 6e65  ed to be assigne
-00013f00: 6420 746f 0a20 2020 2020 2020 2074 6865  d to.        the
-00013f10: 2051 2d73 6574 2061 6e64 2043 2d73 6574   Q-set and C-set
-00013f20: 2e20 416e 7920 6578 7472 6120 444f 4620  . Any extra DOF 
-00013f30: 6172 6520 6173 7369 676e 6564 2074 6f20  are assigned to 
-00013f40: 7468 6520 432d 7365 742e 0a20 2020 2020  the C-set..     
-00013f50: 2020 2043 7265 6174 6564 2067 7269 6420     Created grid 
-00013f60: 4944 7320 7769 6c6c 2062 6520 7365 7175  IDs will be sequ
-00013f70: 656e 7469 616c 2e0a 2020 2020 6e71 203a  ential..    nq :
-00013f80: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
-00013f90: 204e 756d 6265 7220 6f66 206d 6f64 616c   Number of modal
-00013fa0: 2044 4f46 0a0a 2020 2020 5265 7475 726e   DOF..    Return
-00013fb0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00013fc0: 2020 4e6f 6e65 0a0a 2020 2020 4578 616d    None..    Exam
-00013fd0: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-00013fe0: 2d0a 2020 2020 3e3e 3e20 6672 6f6d 2070  -.    >>> from p
-00013ff0: 7979 6574 6920 696d 706f 7274 206e 6173  yyeti import nas
-00014000: 7472 616e 0a20 2020 203e 3e3e 2069 6d70  tran.    >>> imp
-00014010: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00014020: 2020 2020 3e3e 3e20 6e61 7374 7261 6e2e      >>> nastran.
-00014030: 7774 7163 7365 7428 312c 2039 3930 3030  wtqcset(1, 99000
-00014040: 312c 2031 3429 0a20 2020 2051 5345 5431  1, 14).    QSET1
-00014050: 2020 2020 2031 3233 3435 3620 2039 3930       123456  990
-00014060: 3030 3120 5448 5255 2020 2020 2039 3930  001 THRU     990
-00014070: 3030 320a 2020 2020 5153 4554 3120 2020  002.    QSET1   
-00014080: 2020 2020 2020 3132 2020 3939 3030 3033        12  990003
-00014090: 0a20 2020 2043 5345 5431 2020 2020 2020  .    CSET1      
-000140a0: 2033 3435 3620 2039 3930 3030 330a 2020   3456  990003.  
-000140b0: 2020 2222 220a 2020 2020 6e67 7269 6473    """.    ngrids
-000140c0: 203d 2028 6e71 202b 2035 2920 2f2f 2036   = (nq + 5) // 6
-000140d0: 0a20 2020 2065 6e64 6772 6964 203d 2073  .    endgrid = s
-000140e0: 7461 7274 6772 6964 202b 206e 6772 6964  tartgrid + ngrid
-000140f0: 7320 2d20 310a 2020 2020 7864 6f66 203d  s - 1.    xdof =
-00014100: 206e 7120 2d20 3620 2a20 286e 6772 6964   nq - 6 * (ngrid
-00014110: 7320 2d20 3129 0a20 2020 2078 646f 6673  s - 1).    xdofs
-00014120: 203d 2022 3132 3334 3536 225b 3a78 646f   = "123456"[:xdo
-00014130: 665d 0a20 2020 2063 646f 6673 203d 2022  f].    cdofs = "
-00014140: 3132 3334 3536 225b 7864 6f66 3a5d 0a20  123456"[xdof:]. 
-00014150: 2020 2023 2077 7269 7465 2071 7365 7420     # write qset 
-00014160: 616e 6420 6373 6574 2063 6172 6473 3a0a  and cset cards:.
-00014170: 2020 2020 6966 2078 646f 6620 3d3d 2036      if xdof == 6
-00014180: 3a0a 2020 2020 2020 2020 6966 206e 6772  :.        if ngr
-00014190: 6964 7320 3e20 313a 0a20 2020 2020 2020  ids > 1:.       
-000141a0: 2020 2020 2066 2e77 7269 7465 280a 2020       f.write(.  
-000141b0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000141c0: 7b27 5153 4554 3127 3a3c 3873 7d7b 3132  {'QSET1':<8s}{12
-000141d0: 3334 3536 3a38 647d 7b73 7461 7274 6772  3456:8d}{startgr
-000141e0: 6964 3a38 647d 7b27 2054 4852 5520 273a  id:8d}{' THRU ':
-000141f0: 3c38 737d 7b65 6e64 6772 6964 3a38 647d  <8s}{endgrid:8d}
-00014200: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00014210: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00014220: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00014230: 6974 6528 6622 7b27 5153 4554 3127 3a3c  ite(f"{'QSET1':<
-00014240: 3873 7d7b 3132 3334 3536 3a38 647d 7b73  8s}{123456:8d}{s
-00014250: 7461 7274 6772 6964 3a38 647d 5c6e 2229  tartgrid:8d}\n")
-00014260: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00014270: 2020 2069 6620 6e67 7269 6473 203e 2032     if ngrids > 2
-00014280: 3a0a 2020 2020 2020 2020 2020 2020 662e  :.            f.
-00014290: 7772 6974 6528 0a20 2020 2020 2020 2020  write(.         
-000142a0: 2020 2020 2020 2066 227b 2751 5345 5431         f"{'QSET1
-000142b0: 273a 3c38 737d 7b31 3233 3435 363a 3864  ':<8s}{123456:8d
-000142c0: 7d7b 7374 6172 7467 7269 643a 3864 7d7b  }{startgrid:8d}{
-000142d0: 2720 5448 5255 2027 3a3c 3873 7d22 0a20  ' THRU ':<8s}". 
-000142e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000142f0: 227b 656e 6467 7269 6420 2d20 313a 3864  "{endgrid - 1:8d
-00014300: 7d5c 6e22 0a20 2020 2020 2020 2020 2020  }\n".           
-00014310: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-00014320: 6e67 7269 6473 203d 3d20 323a 0a20 2020  ngrids == 2:.   
-00014330: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00014340: 2866 227b 2751 5345 5431 273a 3c38 737d  (f"{'QSET1':<8s}
-00014350: 7b31 3233 3435 363a 3864 7d7b 7374 6172  {123456:8d}{star
-00014360: 7467 7269 643a 3864 7d5c 6e22 290a 2020  tgrid:8d}\n").  
-00014370: 2020 2020 2020 662e 7772 6974 6528 6622        f.write(f"
-00014380: 7b27 5153 4554 3127 3a3c 3873 7d7b 7864  {'QSET1':<8s}{xd
-00014390: 6f66 733a 3e38 737d 7b65 6e64 6772 6964  ofs:>8s}{endgrid
-000143a0: 3a38 647d 5c6e 2229 0a20 2020 2020 2020  :8d}\n").       
-000143b0: 2066 2e77 7269 7465 2866 227b 2743 5345   f.write(f"{'CSE
-000143c0: 5431 273a 3c38 737d 7b63 646f 6673 3a3e  T1':<8s}{cdofs:>
-000143d0: 3873 7d7b 656e 6467 7269 643a 3864 7d5c  8s}{endgrid:8d}\
-000143e0: 6e22 290a 0a0a 4067 7569 746f 6f6c 732e  n")...@guitools.
-000143f0: 7772 6974 655f 7465 7874 5f66 696c 650a  write_text_file.
-00014400: 6465 6620 7774 7262 6532 2866 2c20 6569  def wtrbe2(f, ei
-00014410: 642c 2069 6e64 6570 2c20 646f 662c 2064  d, indep, dof, d
-00014420: 6570 293a 0a20 2020 2022 2222 0a20 2020  ep):.    """.   
-00014430: 2057 7269 7465 7320 6120 4e61 7374 7261   Writes a Nastra
-00014440: 6e20 5242 4532 2063 6172 6420 746f 2061  n RBE2 card to a
-00014450: 2066 696c 652e 0a0a 2020 2020 5061 7261   file...    Para
-00014460: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00014470: 2d2d 2d2d 2d0a 2020 2020 6620 3a20 7374  -----.    f : st
-00014480: 7269 6e67 206f 7220 6669 6c65 5f6c 696b  ring or file_lik
-00014490: 6520 6f72 2031 206f 7220 4e6f 6e65 0a20  e or 1 or None. 
-000144a0: 2020 2020 2020 2045 6974 6865 7220 6120         Either a 
-000144b0: 6e61 6d65 206f 6620 6120 6669 6c65 2c20  name of a file, 
-000144c0: 6f72 2069 7320 6120 6669 6c65 5f6c 696b  or is a file_lik
-000144d0: 6520 6f62 6a65 6374 2061 7320 7265 7475  e object as retu
-000144e0: 726e 6564 0a20 2020 2020 2020 2062 7920  rned.        by 
-000144f0: 3a66 756e 633a 606f 7065 6e60 206f 7220  :func:`open` or 
-00014500: 3a63 6c61 7373 3a60 696f 2e53 7472 696e  :class:`io.Strin
-00014510: 6749 4f60 2e20 496e 7075 7420 6173 2069  gIO`. Input as i
-00014520: 6e74 6567 6572 2031 2074 6f0a 2020 2020  nteger 1 to.    
-00014530: 2020 2020 7772 6974 6520 746f 2073 7464      write to std
-00014540: 6f75 742e 2043 616e 2061 6c73 6f20 6265  out. Can also be
-00014550: 2074 6865 206e 616d 6520 6f66 2061 2064   the name of a d
-00014560: 6972 6563 746f 7279 206f 7220 4e6f 6e65  irectory or None
-00014570: 3b0a 2020 2020 2020 2020 696e 2074 6865  ;.        in the
-00014580: 7365 2063 6173 6573 2c20 6120 4755 4920  se cases, a GUI 
-00014590: 6973 206f 7065 6e65 6420 666f 7220 6669  is opened for fi
-000145a0: 6c65 2073 656c 6563 7469 6f6e 2e0a 2020  le selection..  
-000145b0: 2020 6569 6420 3a20 696e 7465 6765 720a    eid : integer.
-000145c0: 2020 2020 2020 2020 456c 656d 656e 7420          Element 
-000145d0: 4944 0a20 2020 2069 6e64 6570 203a 2069  ID.    indep : i
-000145e0: 6e74 6567 6572 0a20 2020 2020 2020 2049  nteger.        I
-000145f0: 6e64 6570 656e 6465 6e74 2067 7269 6420  ndependent grid 
-00014600: 4944 2e20 416c 6c20 3620 444f 4620 6172  ID. All 6 DOF ar
-00014610: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
-00014620: 696e 6465 7065 6e64 656e 740a 2020 2020  independent.    
-00014630: 2020 2020 616e 6420 6172 6520 6e6f 7420      and are not 
-00014640: 7370 6563 6966 6965 642e 0a20 2020 2064  specified..    d
-00014650: 6f66 203a 2069 6e74 6567 6572 0a20 2020  of : integer.   
-00014660: 2020 2020 2041 6e20 696e 7465 6765 7220       An integer 
-00014670: 636f 6e63 6174 656e 6174 696f 6e20 6f66  concatenation of
-00014680: 2074 6865 2044 4f46 2028 6578 3a20 3132   the DOF (ex: 12
-00014690: 3334 3536 2920 7468 6174 2061 7070 6c69  3456) that appli
-000146a0: 6573 0a20 2020 2020 2020 2066 6f72 2061  es.        for a
-000146b0: 6c6c 2074 6865 2064 6570 656e 6465 6e74  ll the dependent
-000146c0: 2044 4f46 2e0a 2020 2020 6465 7020 3a20   DOF..    dep : 
-000146d0: 3164 2061 7272 6179 5f6c 696b 650a 2020  1d array_like.  
-000146e0: 2020 2020 2020 5665 6374 6f72 206f 6620        Vector of 
-000146f0: 6465 7065 6e64 656e 7420 6772 6964 2049  dependent grid I
-00014700: 4473 0a0a 2020 2020 5265 7475 726e 730a  Ds..    Returns.
-00014710: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00014720: 4e6f 6e65 0a0a 2020 2020 4578 616d 706c  None..    Exampl
-00014730: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
-00014740: 2020 2020 3e3e 3e20 6672 6f6d 2070 7979      >>> from pyy
-00014750: 6574 6920 696d 706f 7274 206e 6173 7472  eti import nastr
-00014760: 616e 0a20 2020 203e 3e3e 2069 6d70 6f72  an.    >>> impor
-00014770: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
-00014780: 2020 3e3e 3e20 6e61 7374 7261 6e2e 7774    >>> nastran.wt
-00014790: 7262 6532 2831 2c20 312c 2031 3030 2c20  rbe2(1, 1, 100, 
-000147a0: 3132 3334 3536 2c20 6e70 2e61 7261 6e67  123456, np.arang
-000147b0: 6528 3130 312c 2031 3131 2929 0a20 2020  e(101, 111)).   
-000147c0: 2052 4245 3220 2020 2020 2020 2020 2020   RBE2           
-000147d0: 3120 2020 2020 3130 3020 2031 3233 3435  1     100  12345
-000147e0: 3620 2020 2020 3130 3120 2020 2020 3130  6     101     10
-000147f0: 3220 2020 2020 3130 3320 2020 2020 3130  2     103     10
-00014800: 3420 2020 2020 3130 350a 2020 2020 2020  4     105.      
-00014810: 2020 2020 2020 2020 2020 2031 3036 2020             106  
-00014820: 2020 2031 3037 2020 2020 2031 3038 2020     107     108  
-00014830: 2020 2031 3039 2020 2020 2031 3130 0a20     109     110. 
-00014840: 2020 2022 2222 0a20 2020 2066 2e77 7269     """.    f.wri
-00014850: 7465 2866 2252 4245 3220 2020 207b 6569  te(f"RBE2    {ei
-00014860: 643a 3864 7d7b 696e 6465 703a 3864 7d7b  d:8d}{indep:8d}{
-00014870: 646f 663a 3864 7d22 290a 2020 2020 7774  dof:8d}").    wt
-00014880: 6e61 7369 6e74 7328 662c 2035 2c20 6465  nasints(f, 5, de
-00014890: 7029 0a0a 0a40 6775 6974 6f6f 6c73 2e77  p)...@guitools.w
-000148a0: 7269 7465 5f74 6578 745f 6669 6c65 0a64  rite_text_file.d
-000148b0: 6566 2077 7472 6265 3328 662c 2065 6964  ef wtrbe3(f, eid
-000148c0: 2c20 4752 4944 5f64 6570 2c20 444f 465f  , GRID_dep, DOF_
-000148d0: 6465 702c 2049 6e64 5f4c 6973 742c 2055  dep, Ind_List, U
-000148e0: 4d5f 4c69 7374 3d4e 6f6e 652c 2061 6c70  M_List=None, alp
-000148f0: 6861 3d4e 6f6e 6529 3a0a 2020 2020 2222  ha=None):.    ""
-00014900: 220a 2020 2020 5772 6974 6573 2061 204e  ".    Writes a N
-00014910: 6173 7472 616e 2052 4245 3320 6361 7264  astran RBE3 card
-00014920: 2074 6f20 6120 6669 6c65 2e0a 0a20 2020   to a file...   
-00014930: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00014940: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066  ----------.    f
-00014950: 203a 2073 7472 696e 6720 6f72 2066 696c   : string or fil
-00014960: 655f 6c69 6b65 206f 7220 3120 6f72 204e  e_like or 1 or N
-00014970: 6f6e 650a 2020 2020 2020 2020 4569 7468  one.        Eith
-00014980: 6572 2061 206e 616d 6520 6f66 2061 2066  er a name of a f
-00014990: 696c 652c 206f 7220 6973 2061 2066 696c  ile, or is a fil
-000149a0: 655f 6c69 6b65 206f 626a 6563 7420 6173  e_like object as
-000149b0: 2072 6574 7572 6e65 640a 2020 2020 2020   returned.      
-000149c0: 2020 6279 203a 6675 6e63 3a60 6f70 656e    by :func:`open
-000149d0: 6020 6f72 203a 636c 6173 733a 6069 6f2e  ` or :class:`io.
-000149e0: 5374 7269 6e67 494f 602e 2049 6e70 7574  StringIO`. Input
-000149f0: 2061 7320 696e 7465 6765 7220 3120 746f   as integer 1 to
-00014a00: 0a20 2020 2020 2020 2077 7269 7465 2074  .        write t
-00014a10: 6f20 7374 646f 7574 2e20 4361 6e20 616c  o stdout. Can al
-00014a20: 736f 2062 6520 7468 6520 6e61 6d65 206f  so be the name o
-00014a30: 6620 6120 6469 7265 6374 6f72 7920 6f72  f a directory or
-00014a40: 204e 6f6e 653b 0a20 2020 2020 2020 2069   None;.        i
-00014a50: 6e20 7468 6573 6520 6361 7365 732c 2061  n these cases, a
-00014a60: 2047 5549 2069 7320 6f70 656e 6564 2066   GUI is opened f
-00014a70: 6f72 2066 696c 6520 7365 6c65 6374 696f  or file selectio
-00014a80: 6e2e 0a20 2020 2065 6964 203a 2069 6e74  n..    eid : int
-00014a90: 6567 6572 0a20 2020 2020 2020 2045 6c65  eger.        Ele
-00014aa0: 6d65 6e74 2049 440a 2020 2020 4752 4944  ment ID.    GRID
-00014ab0: 5f64 6570 203a 2069 6e74 6567 6572 0a20  _dep : integer. 
-00014ac0: 2020 2020 2020 2044 6570 656e 6465 6e74         Dependent
-00014ad0: 2067 7269 6420 4944 0a20 2020 2044 4f46   grid ID.    DOF
-00014ae0: 5f64 6570 203a 2069 6e74 6567 6572 0a20  _dep : integer. 
-00014af0: 2020 2020 2020 2041 6e20 696e 7465 6765         An intege
-00014b00: 7220 636f 6e63 6174 656e 6174 696f 6e20  r concatenation 
-00014b10: 6f66 2074 6865 2044 4f46 2028 6578 3a20  of the DOF (ex: 
-00014b20: 3132 3334 3536 290a 2020 2020 496e 645f  123456).    Ind_
-00014b30: 4c69 7374 203a 206c 6973 740a 2020 2020  List : list.    
-00014b40: 2020 2020 5b20 444f 465f 496e 6431 2c20      [ DOF_Ind1, 
-00014b50: 4752 4944 535f 496e 6431 2c20 444f 465f  GRIDS_Ind1, DOF_
-00014b60: 496e 6432 2c20 4752 4944 535f 496e 6432  Ind2, GRIDS_Ind2
-00014b70: 2c20 2e2e 2e20 5d2c 2077 6865 7265 3a3a  , ... ], where::
-00014b80: 0a0a 2020 2020 2020 2020 2020 2020 444f  ..            DO
-00014b90: 465f 496e 6431 2020 203a 2031 206f 7220  F_Ind1   : 1 or 
-00014ba0: 3220 656c 656d 656e 7420 6172 7261 795f  2 element array_
-00014bb0: 6c69 6b65 2063 6f6e 7461 696e 696e 6720  like containing 
-00014bc0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00014bd0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-00014be0: 706f 6e65 6e74 2044 4f46 2028 6965 2c20  ponent DOF (ie, 
-00014bf0: 3132 3334 3536 2920 6f66 2074 6865 206e  123456) of the n
-00014c00: 6f64 6573 2069 6e0a 2020 2020 2020 2020  odes in.        
-00014c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c20: 2047 5249 4453 5f49 6e64 3120 616e 642c   GRIDS_Ind1 and,
-00014c30: 206f 7074 696f 6e61 6c6c 792c 2074 6865   optionally, the
-00014c40: 2077 6569 6768 7469 6e67 0a20 2020 2020   weighting.     
-00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c60: 2020 2020 6661 6374 6f72 2066 6f72 2074      factor for t
-00014c70: 6865 7365 2044 4f46 2e20 4966 206e 6f74  hese DOF. If not
-00014c80: 2069 6e70 7574 2c20 7468 650a 2020 2020   input, the.    
-00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ca0: 2020 2020 2077 6569 6768 7469 6e67 2066       weighting f
-00014cb0: 6163 746f 7220 6465 6661 756c 7473 2074  actor defaults t
-00014cc0: 6f20 312e 302e 0a20 2020 2020 2020 2020  o 1.0..         
-00014cd0: 2020 2047 5249 4453 5f49 6e64 3120 3a20     GRIDS_Ind1 : 
-00014ce0: 6172 7261 795f 6c69 6b65 206f 6620 6e6f  array_like of no
-00014cf0: 6465 2069 6473 2063 6f72 7265 7370 6f6e  de ids correspon
-00014d00: 6469 6e67 2074 6f0a 2020 2020 2020 2020  ding to.        
-00014d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d20: 2044 4f46 5f49 6e64 310a 2020 2020 2020   DOF_Ind1.      
-00014d30: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00014d40: 2020 2020 2020 6567 3a20 205b 205b 3132        eg:  [ [12
-00014d50: 332c 2031 2e32 5d2c 205b 3935 2c20 3139  3, 1.2], [95, 19
-00014d60: 352c 2031 3030 305d 2c20 3132 3334 3536  5, 1000], 123456
-00014d70: 2c20 3935 5d0a 0a20 2020 2020 2020 2060  , 95]..        `
-00014d80: 496e 645f 4c69 7374 6020 6d75 7374 2062  Ind_List` must b
-00014d90: 6520 6576 656e 206c 656e 6774 682e 0a0a  e even length...
-00014da0: 2020 2020 554d 5f4c 6973 7420 3a20 4e6f      UM_List : No
-00014db0: 6e65 206f 7220 6c69 7374 3b20 6f70 7469  ne or list; opti
-00014dc0: 6f6e 616c 0a20 2020 2020 2020 205b 2047  onal.        [ G
-00014dd0: 5249 445f 4d53 4554 312c 2044 4f46 5f4d  RID_MSET1, DOF_M
-00014de0: 5345 5431 2c20 4752 4944 5f4d 5345 5432  SET1, GRID_MSET2
-00014df0: 2c20 444f 465f 4d53 4554 322c 202e 2e2e  , DOF_MSET2, ...
-00014e00: 205d 2077 6865 7265 3a3a 0a0a 2020 2020   ] where::..    
-00014e10: 2020 2020 2020 2020 2020 4752 4944 5f4d            GRID_M
-00014e20: 5345 5431 203a 2066 6972 7374 2067 7269  SET1 : first gri
-00014e30: 6420 696e 2074 6865 204d 2d73 6574 0a20  d in the M-set. 
-00014e40: 2020 2020 2020 2020 2020 2020 2044 4f46               DOF
-00014e50: 5f4d 5345 5431 2020 3a20 444f 4620 6f66  _MSET1  : DOF of
-00014e60: 2066 6972 7374 2067 7269 6420 696e 204d   first grid in M
-00014e70: 2d73 6574 2028 696e 7465 6765 7220 7375  -set (integer su
-00014e80: 6273 6574 0a20 2020 2020 2020 2020 2020  bset.           
-00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ea0: 6f66 2031 3233 3435 3629 2e20 4e6f 2077  of 123456). No w
-00014eb0: 6569 6768 7469 6e67 2066 6163 746f 7273  eighting factors
-00014ec0: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
-00014ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ee0: 616c 6c6f 7765 6420 6865 7265 2e0a 2020  allowed here..  
-00014ef0: 2020 2020 2020 2020 2020 2020 4752 4944              GRID
-00014f00: 5f4d 5345 5432 203a 2073 6563 6f6e 6420  _MSET2 : second 
-00014f10: 6772 6964 2069 6e20 7468 6520 4d2d 7365  grid in the M-se
-00014f20: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00014f30: 444f 465f 4d53 4554 3220 203a 2044 4f46  DOF_MSET2  : DOF
-00014f40: 206f 6620 7365 636f 6e64 2067 7269 6420   of second grid 
-00014f50: 696e 204d 2d73 6574 0a20 2020 2020 2020  in M-set.       
-00014f60: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
-00014f70: 616c 7068 6120 3a20 4e6f 6e65 206f 7220  alpha : None or 
-00014f80: 7374 7269 6e67 3b20 6f70 7469 6f6e 616c  string; optional
-00014f90: 0a20 2020 2020 2020 2054 6865 726d 616c  .        Thermal
-00014fa0: 2065 7870 616e 7369 6f6e 2063 6f65 6666   expansion coeff
-00014fb0: 6963 6965 6e74 2069 6e20 6120 382d 6368  icient in a 8-ch
-00014fc0: 6172 2073 7472 696e 6720 286f 7220 6c65  ar string (or le
-00014fd0: 7373 292e 0a0a 2020 2020 5265 7475 726e  ss)...    Return
-00014fe0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00014ff0: 2020 4e6f 6e65 0a0a 2020 2020 4578 616d    None..    Exam
-00015000: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-00015010: 2d0a 2020 2020 3e3e 3e20 6672 6f6d 2070  -.    >>> from p
-00015020: 7979 6574 6920 696d 706f 7274 206e 6173  yyeti import nas
-00015030: 7472 616e 0a20 2020 203e 3e3e 206e 6173  tran.    >>> nas
-00015040: 7472 616e 2e77 7472 6265 3328 312c 2031  tran.wtrbe3(1, 1
-00015050: 3030 2c20 3939 3030 2c20 3132 3334 3536  00, 9900, 123456
-00015060: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
-00015070: 2020 2020 2020 2020 205b 3132 332c 205b           [123, [
-00015080: 3939 3031 2c20 3939 3032 2c20 3939 3033  9901, 9902, 9903
-00015090: 2c20 3939 3034 5d2c 0a20 2020 202e 2e2e  , 9904],.    ...
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150b0: 2031 3233 3435 362c 205b 3435 3030 3031   123456, [450001
-000150c0: 2c20 3230 305d 5d29 0a20 2020 2052 4245  , 200]]).    RBE
-000150d0: 3320 2020 2020 2020 2020 3130 3020 2020  3         100   
-000150e0: 2020 2020 2020 2020 2039 3930 3020 2031           9900  1
-000150f0: 3233 3435 3620 2020 312e 3030 3020 2020  23456   1.000   
-00015100: 2020 3132 3320 2020 2039 3930 3120 2020    123    9901   
-00015110: 2039 3930 320a 2020 2020 2020 2020 2020   9902.          
-00015120: 2020 2020 2020 3939 3033 2020 2020 3939        9903    99
-00015130: 3034 2020 2031 2e30 3030 2020 3132 3334  04   1.000  1234
-00015140: 3536 2020 3435 3030 3031 2020 2020 2032  56  450001     2
-00015150: 3030 0a20 2020 203e 3e3e 206e 6173 7472  00.    >>> nastr
-00015160: 616e 2e77 7472 6265 3328 312c 2031 3030  an.wtrbe3(1, 100
-00015170: 2c20 3939 3030 2c20 3132 3334 3536 2c0a  , 9900, 123456,.
-00015180: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
-00015190: 2020 2020 2020 205b 3132 332c 205b 3939         [123, [99
-000151a0: 3031 2c20 3939 3032 2c20 3939 3033 2c20  01, 9902, 9903, 
-000151b0: 3939 3034 5d2c 0a20 2020 202e 2e2e 2020  9904],.    ...  
-000151c0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000151d0: 3132 3334 3536 2c20 312e 325d 2c20 5b34  123456, 1.2], [4
-000151e0: 3530 3030 312c 2032 3030 5d5d 2c0a 2020  50001, 200]],.  
-000151f0: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
-00015200: 2020 2020 2055 4d5f 4c69 7374 3d5b 3939       UM_List=[99
-00015210: 3031 2c20 3132 2c20 3939 3032 2c20 332c  01, 12, 9902, 3,
-00015220: 2039 3930 332c 2031 322c 2039 3930 342c   9903, 12, 9904,
-00015230: 2033 5d2c 0a20 2020 202e 2e2e 2020 2020   3],.    ...    
-00015240: 2020 2020 2020 2020 2020 2020 616c 7068              alph
-00015250: 613d 2736 2e35 652d 3627 290a 2020 2020  a='6.5e-6').    
-00015260: 5242 4533 2020 2020 2020 2020 2031 3030  RBE3         100
-00015270: 2020 2020 2020 2020 2020 2020 3939 3030              9900
-00015280: 2020 3132 3334 3536 2020 2031 2e30 3030    123456   1.000
-00015290: 2020 2020 2031 3233 2020 2020 3939 3031       123    9901
-000152a0: 2020 2020 3939 3032 0a20 2020 2020 2020      9902.       
-000152b0: 2020 2020 2020 2020 2039 3930 3320 2020           9903   
-000152c0: 2039 3930 3420 2020 312e 3230 3020 2031   9904   1.200  1
-000152d0: 3233 3435 3620 2034 3530 3030 3120 2020  23456  450001   
-000152e0: 2020 3230 300a 2020 2020 2020 2020 2020    200.          
-000152f0: 2020 554d 2020 2020 2020 2020 2020 3939    UM          99
-00015300: 3031 2020 2020 2020 3132 2020 2020 3939  01      12    99
-00015310: 3032 2020 2020 2020 2033 2020 2020 3939  02       3    99
-00015320: 3033 2020 2020 2020 3132 0a20 2020 2020  03      12.     
-00015330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015340: 2020 2039 3930 3420 2020 2020 2020 330a     9904       3.
-00015350: 2020 2020 2020 2020 2020 2020 414c 5048              ALPH
-00015360: 4120 2020 2020 362e 3565 2d36 0a20 2020  A     6.5e-6.   
-00015370: 2022 2222 0a20 2020 2069 6620 6c65 6e28   """.    if len(
-00015380: 496e 645f 4c69 7374 2920 2620 313a 0a20  Ind_List) & 1:. 
-00015390: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000153a0: 7565 4572 726f 7228 6622 6049 6e64 5f4c  ueError(f"`Ind_L
-000153b0: 6973 7460 206d 7573 7420 6861 7665 2065  ist` must have e
-000153c0: 7665 6e20 6c65 6e67 7468 2028 6974 2069  ven length (it i
-000153d0: 7320 7b6c 656e 2849 6e64 5f4c 6973 7429  s {len(Ind_List)
-000153e0: 7d29 2229 0a0a 2020 2020 662e 7772 6974  })")..    f.writ
-000153f0: 6528 6622 5242 4533 2020 2020 7b65 6964  e(f"RBE3    {eid
-00015400: 3a38 647d 2020 2020 2020 2020 7b47 5249  :8d}        {GRI
-00015410: 445f 6465 703a 3864 7d7b 444f 465f 6465  D_dep:8d}{DOF_de
-00015420: 703a 3864 7d22 290a 2020 2020 6669 656c  p:8d}").    fiel
-00015430: 6420 3d20 350a 0a20 2020 2064 6566 205f  d = 5..    def _
-00015440: 496e 635f 4669 656c 6428 662c 2066 6965  Inc_Field(f, fie
-00015450: 6c64 293a 0a20 2020 2020 2020 2066 6965  ld):.        fie
-00015460: 6c64 202b 3d20 310a 2020 2020 2020 2020  ld += 1.        
-00015470: 6966 2066 6965 6c64 203d 3d20 3130 3a0a  if field == 10:.
-00015480: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00015490: 6974 6528 225c 6e20 2020 2020 2020 2022  ite("\n        "
-000154a0: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
-000154b0: 656c 6420 3d20 320a 2020 2020 2020 2020  eld = 2.        
-000154c0: 7265 7475 726e 2066 6965 6c64 0a0a 2020  return field..  
-000154d0: 2020 2320 6c6f 6f70 206f 7665 7220 696e    # loop over in
-000154e0: 6465 7065 6e64 656e 7473 0a20 2020 2066  dependents.    f
-000154f0: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-00015500: 206c 656e 2849 6e64 5f4c 6973 7429 2c20   len(Ind_List), 
-00015510: 3229 3a0a 2020 2020 2020 2020 444f 465f  2):.        DOF_
-00015520: 696e 6420 3d20 6e70 2e61 746c 6561 7374  ind = np.atleast
-00015530: 5f31 6428 496e 645f 4c69 7374 5b6a 5d29  _1d(Ind_List[j])
-00015540: 0a20 2020 2020 2020 2047 5249 4453 5f69  .        GRIDS_i
-00015550: 6e64 203d 206e 702e 6174 6c65 6173 745f  nd = np.atleast_
-00015560: 3164 2849 6e64 5f4c 6973 745b 6a20 2b20  1d(Ind_List[j + 
-00015570: 315d 290a 2020 2020 2020 2020 646f 6620  1]).        dof 
-00015580: 3d20 696e 7428 444f 465f 696e 645b 305d  = int(DOF_ind[0]
-00015590: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-000155a0: 2844 4f46 5f69 6e64 2920 3d3d 2032 3a0a  (DOF_ind) == 2:.
-000155b0: 2020 2020 2020 2020 2020 2020 7774 203d              wt =
-000155c0: 2066 6c6f 6174 2844 4f46 5f69 6e64 5b31   float(DOF_ind[1
-000155d0: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
-000155e0: 0a20 2020 2020 2020 2020 2020 2077 7420  .            wt 
-000155f0: 3d20 312e 300a 2020 2020 2020 2020 6669  = 1.0.        fi
-00015600: 656c 6420 3d20 5f49 6e63 5f46 6965 6c64  eld = _Inc_Field
-00015610: 2866 2c20 6669 656c 6429 0a20 2020 2020  (f, field).     
-00015620: 2020 2066 2e77 7269 7465 2866 227b 7774     f.write(f"{wt
-00015630: 3a38 2e33 667d 2229 0a20 2020 2020 2020  :8.3f}").       
-00015640: 2066 6965 6c64 203d 205f 496e 635f 4669   field = _Inc_Fi
-00015650: 656c 6428 662c 2066 6965 6c64 290a 2020  eld(f, field).  
-00015660: 2020 2020 2020 662e 7772 6974 6528 6622        f.write(f"
-00015670: 7b64 6f66 3a38 647d 2229 0a20 2020 2020  {dof:8d}").     
-00015680: 2020 2066 6f72 2067 2069 6e20 4752 4944     for g in GRID
-00015690: 535f 696e 643a 0a20 2020 2020 2020 2020  S_ind:.         
-000156a0: 2020 2066 6965 6c64 203d 205f 496e 635f     field = _Inc_
-000156b0: 4669 656c 6428 662c 2066 6965 6c64 290a  Field(f, field).
-000156c0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-000156d0: 6974 6528 6622 7b67 3a38 647d 2229 0a20  ite(f"{g:8d}"). 
-000156e0: 2020 2066 2e77 7269 7465 2822 5c6e 2229     f.write("\n")
-000156f0: 0a0a 2020 2020 6465 6620 5f49 6e63 5f55  ..    def _Inc_U
-00015700: 4d5f 4669 656c 6428 662c 2066 6965 6c64  M_Field(f, field
-00015710: 293a 0a20 2020 2020 2020 2066 6965 6c64  ):.        field
-00015720: 202b 3d20 310a 2020 2020 2020 2020 6966   += 1.        if
-00015730: 2066 6965 6c64 203d 3d20 393a 0a20 2020   field == 9:.   
-00015740: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00015750: 2822 5c6e 2020 2020 2020 2020 2020 2020  ("\n            
-00015760: 2020 2020 2229 0a20 2020 2020 2020 2020      ").         
-00015770: 2020 2066 6965 6c64 203d 2033 0a20 2020     field = 3.   
-00015780: 2020 2020 2072 6574 7572 6e20 6669 656c       return fiel
-00015790: 640a 0a20 2020 2069 6620 554d 5f4c 6973  d..    if UM_Lis
-000157a0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-000157b0: 2020 2020 2020 2066 2e77 7269 7465 2822         f.write("
-000157c0: 2020 2020 2020 2020 554d 2020 2020 2020          UM      
-000157d0: 2229 0a20 2020 2020 2020 2066 6965 6c64  ").        field
-000157e0: 203d 2032 0a20 2020 2020 2020 2066 6f72   = 2.        for
-000157f0: 206a 2069 6e20 554d 5f4c 6973 743a 0a20   j in UM_List:. 
-00015800: 2020 2020 2020 2020 2020 2066 6965 6c64             field
-00015810: 203d 205f 496e 635f 554d 5f46 6965 6c64   = _Inc_UM_Field
-00015820: 2866 2c20 6669 656c 6429 0a20 2020 2020  (f, field).     
-00015830: 2020 2020 2020 2066 2e77 7269 7465 2822         f.write("
-00015840: 7b3a 3864 7d22 2e66 6f72 6d61 7428 6a29  {:8d}".format(j)
-00015850: 290a 2020 2020 2020 2020 662e 7772 6974  ).        f.writ
-00015860: 6528 225c 6e22 290a 0a20 2020 2069 6620  e("\n")..    if 
-00015870: 616c 7068 6120 6973 206e 6f74 204e 6f6e  alpha is not Non
-00015880: 653a 0a20 2020 2020 2020 2066 2e77 7269  e:.        f.wri
-00015890: 7465 2866 2220 2020 2020 2020 2041 4c50  te(f"        ALP
-000158a0: 4841 2020 207b 616c 7068 613a 3e38 737d  HA   {alpha:>8s}
-000158b0: 5c6e 2229 0a0a 0a40 6775 6974 6f6f 6c73  \n")...@guitools
-000158c0: 2e77 7269 7465 5f74 6578 745f 6669 6c65  .write_text_file
-000158d0: 0a64 6566 2077 7473 6573 6574 2866 2c20  .def wtseset(f, 
-000158e0: 7375 7065 7269 642c 2067 7269 6473 293a  superid, grids):
-000158f0: 0a20 2020 2022 2222 0a20 2020 2057 7269  .    """.    Wri
-00015900: 7465 7320 6120 4e61 7374 7261 6e20 5345  tes a Nastran SE
-00015910: 5345 5420 6361 7264 2074 6f20 6120 6669  SET card to a fi
-00015920: 6c65 2e0a 0a20 2020 2050 6172 616d 6574  le...    Paramet
-00015930: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00015940: 2d2d 0a20 2020 2066 203a 2073 7472 696e  --.    f : strin
-00015950: 6720 6f72 2066 696c 655f 6c69 6b65 206f  g or file_like o
-00015960: 7220 3120 6f72 204e 6f6e 650a 2020 2020  r 1 or None.    
-00015970: 2020 2020 4569 7468 6572 2061 206e 616d      Either a nam
-00015980: 6520 6f66 2061 2066 696c 652c 206f 7220  e of a file, or 
-00015990: 6973 2061 2066 696c 655f 6c69 6b65 206f  is a file_like o
-000159a0: 626a 6563 7420 6173 2072 6574 7572 6e65  bject as returne
-000159b0: 640a 2020 2020 2020 2020 6279 203a 6675  d.        by :fu
-000159c0: 6e63 3a60 6f70 656e 6020 6f72 203a 636c  nc:`open` or :cl
-000159d0: 6173 733a 6069 6f2e 5374 7269 6e67 494f  ass:`io.StringIO
-000159e0: 602e 2049 6e70 7574 2061 7320 696e 7465  `. Input as inte
-000159f0: 6765 7220 3120 746f 0a20 2020 2020 2020  ger 1 to.       
-00015a00: 2077 7269 7465 2074 6f20 7374 646f 7574   write to stdout
-00015a10: 2e20 4361 6e20 616c 736f 2062 6520 7468  . Can also be th
-00015a20: 6520 6e61 6d65 206f 6620 6120 6469 7265  e name of a dire
-00015a30: 6374 6f72 7920 6f72 204e 6f6e 653b 0a20  ctory or None;. 
-00015a40: 2020 2020 2020 2069 6e20 7468 6573 6520         in these 
-00015a50: 6361 7365 732c 2061 2047 5549 2069 7320  cases, a GUI is 
-00015a60: 6f70 656e 6564 2066 6f72 2066 696c 6520  opened for file 
-00015a70: 7365 6c65 6374 696f 6e2e 0a20 2020 2073  selection..    s
-00015a80: 7570 6572 6964 3a20 696e 7465 6765 720a  uperid: integer.
-00015a90: 2020 2020 2020 2020 5375 7065 7265 6c65          Superele
-00015aa0: 6d65 6e74 2049 440a 2020 2020 6772 6964  ment ID.    grid
-00015ab0: 7320 3a20 3164 2061 7272 6179 5f6c 696b  s : 1d array_lik
-00015ac0: 650a 2020 2020 2020 2020 5665 6374 6f72  e.        Vector
-00015ad0: 206f 6620 6772 6964 2069 6473 2e0a 0a20   of grid ids... 
-00015ae0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00015af0: 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e 650a  ------.    None.
-00015b00: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-00015b10: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e    --------.    >
-00015b20: 3e3e 2066 726f 6d20 7079 7965 7469 2069  >> from pyyeti i
-00015b30: 6d70 6f72 7420 6e61 7374 7261 6e0a 2020  mport nastran.  
-00015b40: 2020 3e3e 3e20 696d 706f 7274 206e 756d    >>> import num
-00015b50: 7079 2061 7320 6e70 0a20 2020 203e 3e3e  py as np.    >>>
-00015b60: 206e 6173 7472 616e 2e77 7473 6573 6574   nastran.wtseset
-00015b70: 2831 2c20 3130 302c 206e 702e 6172 616e  (1, 100, np.aran
-00015b80: 6765 2831 2c20 3236 2929 0a20 2020 2053  ge(1, 26)).    S
-00015b90: 4553 4554 2020 2020 2020 2020 3130 3020  ESET        100 
-00015ba0: 2020 2020 2020 3120 2020 2020 2020 3220        1       2 
-00015bb0: 2020 2020 2020 3320 2020 2020 2020 3420        3       4 
-00015bc0: 2020 2020 2020 3520 2020 2020 2020 3620        5       6 
-00015bd0: 2020 2020 2020 370a 2020 2020 5345 5345        7.    SESE
-00015be0: 5420 2020 2020 2020 2031 3030 2020 2020  T        100    
-00015bf0: 2020 2038 2020 2020 2020 2039 2020 2020     8       9    
-00015c00: 2020 3130 2020 2020 2020 3131 2020 2020    10      11    
-00015c10: 2020 3132 2020 2020 2020 3133 2020 2020    12      13    
-00015c20: 2020 3134 0a20 2020 2053 4553 4554 2020    14.    SESET  
-00015c30: 2020 2020 2020 3130 3020 2020 2020 2031        100      1
-00015c40: 3520 2020 2020 2031 3620 2020 2020 2031  5      16      1
-00015c50: 3720 2020 2020 2031 3820 2020 2020 2031  7      18      1
-00015c60: 3920 2020 2020 2032 3020 2020 2020 2032  9      20      2
-00015c70: 310a 2020 2020 5345 5345 5420 2020 2020  1.    SESET     
-00015c80: 2020 2031 3030 2020 2020 2020 3232 2020     100      22  
-00015c90: 2020 2020 3233 2020 2020 2020 3234 2020      23      24  
-00015ca0: 2020 2020 3235 0a20 2020 2022 2222 0a20      25.    """. 
-00015cb0: 2020 206e 203d 206c 656e 2867 7269 6473     n = len(grids
-00015cc0: 290a 2020 2020 2320 3720 6772 6964 7320  ).    # 7 grids 
-00015cd0: 7065 7220 5345 5345 543a 0a20 2020 2066  per SESET:.    f
-00015ce0: 726d 203d 2022 5345 5345 5420 2020 7b3a  rm = "SESET   {:
-00015cf0: 3864 7d22 202b 2022 7b3a 3864 7d22 202a  8d}" + "{:8d}" *
-00015d00: 2037 202b 2022 5c6e 220a 2020 2020 6920   7 + "\n".    i 
-00015d10: 3d20 300a 2020 2020 7768 696c 6520 6920  = 0.    while i 
-00015d20: 2b20 3720 3c3d 206e 3a0a 2020 2020 2020  + 7 <= n:.      
-00015d30: 2020 662e 7772 6974 6528 6672 6d2e 666f    f.write(frm.fo
-00015d40: 726d 6174 2873 7570 6572 6964 2c20 2a67  rmat(superid, *g
-00015d50: 7269 6473 5b69 203a 2069 202b 2037 5d29  rids[i : i + 7])
-00015d60: 290a 2020 2020 2020 2020 6920 2b3d 2037  ).        i += 7
-00015d70: 0a20 2020 2069 6620 6920 3c20 6e3a 0a20  .    if i < n:. 
-00015d80: 2020 2020 2020 2066 726d 203d 2022 5345         frm = "SE
-00015d90: 5345 5420 2020 7b3a 3864 7d22 202b 2022  SET   {:8d}" + "
-00015da0: 7b3a 3864 7d22 202a 2028 6e20 2d20 6929  {:8d}" * (n - i)
-00015db0: 202b 2022 5c6e 220a 2020 2020 2020 2020   + "\n".        
-00015dc0: 662e 7772 6974 6528 6672 6d2e 666f 726d  f.write(frm.form
-00015dd0: 6174 2873 7570 6572 6964 2c20 2a67 7269  at(superid, *gri
-00015de0: 6473 5b69 3a5d 2929 0a0a 0a40 6775 6974  ds[i:]))...@guit
-00015df0: 6f6f 6c73 2e77 7269 7465 5f74 6578 745f  ools.write_text_
-00015e00: 6669 6c65 0a64 6566 2077 7473 6574 2866  file.def wtset(f
-00015e10: 2c20 7365 7469 642c 2069 6473 293a 0a20  , setid, ids):. 
-00015e20: 2020 2022 2222 0a20 2020 2057 7269 7465     """.    Write
-00015e30: 7320 6120 4e61 7374 7261 6e20 6361 7365  s a Nastran case
-00015e40: 2d63 6f6e 7472 6f6c 2053 4554 2063 6172  -control SET car
-00015e50: 6420 746f 2061 2066 696c 652e 0a0a 2020  d to a file...  
-00015e60: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00015e70: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00015e80: 6620 3a20 7374 7269 6e67 206f 7220 6669  f : string or fi
-00015e90: 6c65 5f6c 696b 6520 6f72 2031 206f 7220  le_like or 1 or 
-00015ea0: 4e6f 6e65 0a20 2020 2020 2020 2045 6974  None.        Eit
-00015eb0: 6865 7220 6120 6e61 6d65 206f 6620 6120  her a name of a 
-00015ec0: 6669 6c65 2c20 6f72 2069 7320 6120 6669  file, or is a fi
-00015ed0: 6c65 5f6c 696b 6520 6f62 6a65 6374 2061  le_like object a
-00015ee0: 7320 7265 7475 726e 6564 0a20 2020 2020  s returned.     
-00015ef0: 2020 2062 7920 3a66 756e 633a 606f 7065     by :func:`ope
-00015f00: 6e60 206f 7220 3a63 6c61 7373 3a60 696f  n` or :class:`io
-00015f10: 2e53 7472 696e 6749 4f60 2e20 496e 7075  .StringIO`. Inpu
-00015f20: 7420 6173 2069 6e74 6567 6572 2031 2074  t as integer 1 t
-00015f30: 6f0a 2020 2020 2020 2020 7772 6974 6520  o.        write 
-00015f40: 746f 2073 7464 6f75 742e 2043 616e 2061  to stdout. Can a
-00015f50: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
-00015f60: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
-00015f70: 7220 4e6f 6e65 3b0a 2020 2020 2020 2020  r None;.        
-00015f80: 696e 2074 6865 7365 2063 6173 6573 2c20  in these cases, 
-00015f90: 6120 4755 4920 6973 206f 7065 6e65 6420  a GUI is opened 
-00015fa0: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
-00015fb0: 6f6e 2e0a 2020 2020 7365 7469 643a 2069  on..    setid: i
-00015fc0: 6e74 6567 6572 0a20 2020 2020 2020 2053  nteger.        S
-00015fd0: 6574 2049 440a 2020 2020 6964 7320 3a20  et ID.    ids : 
-00015fe0: 3164 2061 7272 6179 5f6c 696b 650a 2020  1d array_like.  
-00015ff0: 2020 2020 2020 5665 6374 6f72 206f 6620        Vector of 
-00016000: 4944 730a 0a20 2020 2052 6574 7572 6e73  IDs..    Returns
-00016010: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00016020: 204e 6f6e 650a 0a20 2020 2045 7861 6d70   None..    Examp
-00016030: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-00016040: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
-00016050: 7965 7469 2069 6d70 6f72 7420 6e61 7374  yeti import nast
-00016060: 7261 6e0a 2020 2020 3e3e 3e20 696d 706f  ran.    >>> impo
-00016070: 7274 206e 756d 7079 2061 7320 6e70 0a20  rt numpy as np. 
-00016080: 2020 203e 3e3e 206e 6173 7472 616e 2e77     >>> nastran.w
-00016090: 7473 6574 2831 2c20 3130 302c 206e 702e  tset(1, 100, np.
-000160a0: 6172 616e 6765 2831 2c20 3236 2929 0a20  arange(1, 26)). 
-000160b0: 2020 2053 4554 2031 3030 203d 2031 2c20     SET 100 = 1, 
-000160c0: 322c 2033 2c20 342c 2035 2c20 362c 2037  2, 3, 4, 5, 6, 7
-000160d0: 2c0a 2020 2020 2038 2c20 392c 2031 302c  ,.     8, 9, 10,
-000160e0: 2031 312c 2031 322c 2031 332c 2031 342c   11, 12, 13, 14,
-000160f0: 0a20 2020 2020 3135 2c20 3136 2c20 3137  .     15, 16, 17
-00016100: 2c20 3138 2c20 3139 2c20 3230 2c20 3231  , 18, 19, 20, 21
-00016110: 2c0a 2020 2020 2032 322c 2032 332c 2032  ,.     22, 23, 2
-00016120: 342c 2032 350a 2020 2020 2222 220a 2020  4, 25.    """.  
-00016130: 2020 662e 7772 6974 6528 6622 5345 5420    f.write(f"SET 
-00016140: 7b73 6574 6964 7d20 3d22 290a 2020 2020  {setid} =").    
-00016150: 6e20 3d20 6c65 6e28 6964 7329 0a20 2020  n = len(ids).   
-00016160: 2023 2037 2069 6473 2070 6572 206c 696e   # 7 ids per lin
-00016170: 653a 0a20 2020 2066 726d 203d 2022 207b  e:.    frm = " {
-00016180: 3a64 7d2c 2220 2a20 3720 2b20 225c 6e22  :d}," * 7 + "\n"
-00016190: 0a20 2020 2069 203d 2030 0a20 2020 2077  .    i = 0.    w
-000161a0: 6869 6c65 2069 202b 2037 203c 206e 3a0a  hile i + 7 < n:.
-000161b0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-000161c0: 6672 6d2e 666f 726d 6174 282a 6964 735b  frm.format(*ids[
-000161d0: 6920 3a20 6920 2b20 375d 2929 0a20 2020  i : i + 7])).   
-000161e0: 2020 2020 2069 202b 3d20 370a 2020 2020       i += 7.    
-000161f0: 6672 6d20 3d20 2220 7b3a 647d 2c22 202a  frm = " {:d}," *
-00016200: 2028 6e20 2d20 6920 2d20 3129 202b 2022   (n - i - 1) + "
-00016210: 207b 3a64 7d5c 6e22 0a20 2020 2066 2e77   {:d}\n".    f.w
-00016220: 7269 7465 2866 726d 2e66 6f72 6d61 7428  rite(frm.format(
-00016230: 2a69 6473 5b69 3a5d 2929 0a0a 0a40 6775  *ids[i:]))...@gu
-00016240: 6974 6f6f 6c73 2e77 7269 7465 5f74 6578  itools.write_tex
-00016250: 745f 6669 6c65 0a64 6566 2077 7472 7370  t_file.def wtrsp
-00016260: 6c69 6e65 2866 2c20 7269 642c 2069 6473  line(f, rid, ids
-00016270: 2c20 446f 4c3d 2230 2e31 2229 3a0a 2020  , DoL="0.1"):.  
-00016280: 2020 2222 220a 2020 2020 5772 6974 6520    """.    Write 
-00016290: 4e61 7374 7261 6e20 5253 504c 494e 4520  Nastran RSPLINE 
-000162a0: 6361 7264 2873 292e 0a0a 2020 2020 5061  card(s)...    Pa
-000162b0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-000162c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6620 3a20  -------.    f : 
-000162d0: 7374 7269 6e67 206f 7220 6669 6c65 5f6c  string or file_l
-000162e0: 696b 6520 6f72 2031 206f 7220 4e6f 6e65  ike or 1 or None
-000162f0: 0a20 2020 2020 2020 2045 6974 6865 7220  .        Either 
-00016300: 6120 6e61 6d65 206f 6620 6120 6669 6c65  a name of a file
-00016310: 2c20 6f72 2069 7320 6120 6669 6c65 5f6c  , or is a file_l
-00016320: 696b 6520 6f62 6a65 6374 2061 7320 7265  ike object as re
-00016330: 7475 726e 6564 0a20 2020 2020 2020 2062  turned.        b
-00016340: 7920 3a66 756e 633a 606f 7065 6e60 206f  y :func:`open` o
-00016350: 7220 3a63 6c61 7373 3a60 696f 2e53 7472  r :class:`io.Str
-00016360: 696e 6749 4f60 2e20 496e 7075 7420 6173  ingIO`. Input as
-00016370: 2069 6e74 6567 6572 2031 2074 6f0a 2020   integer 1 to.  
-00016380: 2020 2020 2020 7772 6974 6520 746f 2073        write to s
-00016390: 7464 6f75 742e 2043 616e 2061 6c73 6f20  tdout. Can also 
-000163a0: 6265 2074 6865 206e 616d 6520 6f66 2061  be the name of a
-000163b0: 2064 6972 6563 746f 7279 206f 7220 4e6f   directory or No
-000163c0: 6e65 3b0a 2020 2020 2020 2020 696e 2074  ne;.        in t
-000163d0: 6865 7365 2063 6173 6573 2c20 6120 4755  hese cases, a GU
-000163e0: 4920 6973 206f 7065 6e65 6420 666f 7220  I is opened for 
-000163f0: 6669 6c65 2073 656c 6563 7469 6f6e 2e0a  file selection..
-00016400: 2020 2020 7269 6420 3a20 696e 7465 6765      rid : intege
-00016410: 720a 2020 2020 2020 2020 4944 2066 6f72  r.        ID for
-00016420: 2031 7374 2052 5350 4c49 4e45 3b20 6765   1st RSPLINE; ge
-00016430: 7473 2069 6e63 7265 6d65 6e74 6564 2062  ts incremented b
-00016440: 7920 3120 666f 7220 6561 6368 2052 5350  y 1 for each RSP
-00016450: 4c49 4e45 0a20 2020 2069 6473 203a 2032  LINE.    ids : 2
-00016460: 6420 6172 7261 795f 6c69 6b65 0a20 2020  d array_like.   
-00016470: 2020 2020 2032 2063 6f6c 756d 6e20 6d61       2 column ma
-00016480: 7472 6978 3a20 5b67 7269 645f 6964 732c  trix: [grid_ids,
-00016490: 2069 6e64 6570 656e 6465 6e74 5f66 6c61   independent_fla
-000164a0: 675d 3b20 6861 7320 6772 6964 7320 666f  g]; has grids fo
-000164b0: 720a 2020 2020 2020 2020 5253 504c 494e  r.        RSPLIN
-000164c0: 4520 696e 2064 6573 6972 6564 206f 7264  E in desired ord
-000164d0: 6572 2061 6e64 2061 2030 206f 7220 3120  er and a 0 or 1 
-000164e0: 666c 6167 2066 6f72 2065 6163 6820 7768  flag for each wh
-000164f0: 6572 6520 310a 2020 2020 2020 2020 6d65  ere 1.        me
-00016500: 616e 7320 7468 6520 6772 6964 2069 7320  ans the grid is 
-00016510: 696e 6465 7065 6e64 656e 742e 204e 6f74  independent. Not
-00016520: 653a 2074 6865 2031 7374 2061 6e64 206c  e: the 1st and l
-00016530: 6173 7420 6772 6964 730a 2020 2020 2020  ast grids.      
-00016540: 2020 6d75 7374 2062 6520 696e 6465 7065    must be indepe
-00016550: 6e64 656e 742e 0a20 2020 2044 6f4c 203a  ndent..    DoL :
-00016560: 2073 7472 696e 6720 6f72 2072 6561 6c20   string or real 
-00016570: 7363 616c 6172 0a20 2020 2020 2020 2053  scalar.        S
-00016580: 7065 6369 6669 6573 2072 6174 696f 206f  pecifies ratio o
-00016590: 6620 6469 616d 6574 6572 206f 6620 656c  f diameter of el
-000165a0: 6173 7469 6320 7475 6265 2074 6f20 7468  astic tube to th
-000165b0: 6520 7375 6d20 6f66 2074 6865 0a20 2020  e sum of the.   
-000165c0: 2020 2020 206c 656e 6774 6873 206f 6620       lengths of 
-000165d0: 616c 6c20 7365 676d 656e 7473 2e20 5772  all segments. Wr
-000165e0: 6974 7465 6e20 7769 7468 3a20 6060 6627  itten with: ``f'
-000165f0: 7b44 6f4c 3a3c 387d 2760 600a 0a20 2020  {DoL:<8}'``..   
-00016600: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-00016610: 2d2d 2d2d 0a20 2020 204e 6f6e 650a 0a20  ----.    None.. 
-00016620: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-00016630: 2d2d 0a20 2020 2054 6865 2052 5350 4c49  --.    The RSPLI
-00016640: 4e45 7320 7769 6c6c 2066 6f6c 6c6f 7720  NEs will follow 
-00016650: 7468 6973 2070 6174 7465 726e 3a3a 0a0a  this pattern::..
-00016660: 2020 2020 2020 2020 5253 504c 494e 4531          RSPLINE1
-00016670: 2020 696e 6465 7065 6e64 656e 7431 202d    independent1 -
-00016680: 2064 6570 656e 6465 6e74 7331 202d 2069   dependents1 - i
-00016690: 6e64 6570 656e 6465 6e74 320a 2020 2020  ndependent2.    
-000166a0: 2020 2020 5253 504c 494e 4532 2020 696e      RSPLINE2  in
-000166b0: 6465 7065 6e64 656e 7432 202d 2064 6570  dependent2 - dep
-000166c0: 656e 6465 6e74 7332 202d 2069 6e64 6570  endents2 - indep
-000166d0: 656e 6465 6e74 330a 2020 2020 2020 2020  endent3.        
-000166e0: 2e2e 2e0a 0a20 2020 204e 6f74 6520 7468  .....    Note th
-000166f0: 6174 2074 6865 7265 2063 616e 2062 6520  at there can be 
-00016700: 6d75 6c74 6970 6c65 2064 6570 656e 6465  multiple depende
-00016710: 6e74 7320 7361 6e64 7769 6368 6564 2062  nts sandwiched b
-00016720: 6574 7765 656e 2074 6865 0a20 2020 2074  etween the.    t
-00016730: 776f 206f 7574 7369 6465 2069 6e64 6570  wo outside indep
-00016740: 656e 6465 6e74 206e 6f64 6573 2070 6572  endent nodes per
-00016750: 2052 5350 4c49 4e45 2e0a 0a20 2020 2054   RSPLINE...    T
-00016760: 6865 2073 706c 696e 6520 656c 656d 656e  he spline elemen
-00016770: 7420 6173 7375 6d65 7320 6120 6c69 6e65  t assumes a line
-00016780: 6172 2069 6e74 6572 706f 6c61 7469 6f6e  ar interpolation
-00016790: 2066 6f72 2064 6973 706c 6163 656d 656e   for displacemen
-000167a0: 740a 2020 2020 616e 6420 746f 7273 696f  t.    and torsio
-000167b0: 6e20 616c 6f6e 6720 7468 6520 6178 6973  n along the axis
-000167c0: 206f 6620 7468 6520 7370 6c69 6e65 2c20   of the spline, 
-000167d0: 6120 7175 6164 7261 7469 630a 2020 2020  a quadratic.    
-000167e0: 696e 7465 7270 6f6c 6174 696f 6e20 666f  interpolation fo
-000167f0: 7220 726f 7461 7469 6f6e 7320 6e6f 726d  r rotations norm
-00016800: 616c 2074 6f20 7468 6520 6178 6973 206f  al to the axis o
-00016810: 6620 7468 6520 7370 6c69 6e65 2c20 616e  f the spline, an
-00016820: 640a 2020 2020 6120 6375 6269 6320 696e  d.    a cubic in
-00016830: 7465 7270 6f6c 6174 696f 6e20 666f 7220  terpolation for 
-00016840: 6469 7370 6c61 6365 6d65 6e74 7320 6e6f  displacements no
-00016850: 726d 616c 2074 6f20 7468 6520 6178 6973  rmal to the axis
-00016860: 206f 6620 7468 650a 2020 2020 7370 6c69   of the.    spli
-00016870: 6e65 2e0a 0a20 2020 2053 6565 2061 6c73  ne...    See als
-00016880: 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  o.    --------. 
-00016890: 2020 203a 6675 6e63 3a60 7774 7273 706c     :func:`wtrspl
-000168a0: 696e 655f 7269 6e67 7360 0a0a 2020 2020  ine_rings`..    
-000168b0: 5261 6973 6573 0a20 2020 202d 2d2d 2d2d  Raises.    -----
-000168c0: 2d0a 2020 2020 5661 6c75 6545 7272 6f72  -.    ValueError
-000168d0: 0a0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
-000168e0: 7265 2061 7265 206c 6573 7320 7468 616e  re are less than
-000168f0: 2033 2067 7269 6473 2066 6f72 2052 5350   3 grids for RSP
-00016900: 4c49 4e45 2e0a 0a20 2020 2020 2020 2049  LINE...        I
-00016910: 6620 6569 7468 6572 2074 6865 2066 6972  f either the fir
-00016920: 7374 206f 7220 6c61 7374 2067 7269 6473  st or last grids
-00016930: 2069 7320 6465 7065 6e64 656e 742e 0a0a   is dependent...
-00016940: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-00016950: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
-00016960: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
-00016970: 7320 6e70 0a20 2020 203e 3e3e 2066 726f  s np.    >>> fro
-00016980: 6d20 7079 7965 7469 2069 6d70 6f72 7420  m pyyeti import 
-00016990: 6e61 7374 7261 6e0a 2020 2020 3e3e 3e20  nastran.    >>> 
-000169a0: 6964 7320 3d20 6e70 2e61 7272 6179 285b  ids = np.array([
-000169b0: 5b31 3030 2c20 315d 2c0a 2020 2020 2e2e  [100, 1],.    ..
-000169c0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-000169d0: 2020 5b31 3031 2c20 305d 2c0a 2020 2020    [101, 0],.    
-000169e0: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
-000169f0: 2020 2020 5b31 3032 2c20 305d 2c0a 2020      [102, 0],.  
-00016a00: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
-00016a10: 2020 2020 2020 5b31 3033 2c20 315d 2c0a        [103, 1],.
-00016a20: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
-00016a30: 2020 2020 2020 2020 5b31 3034 2c20 305d          [104, 0]
-00016a40: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
-00016a50: 2020 2020 2020 2020 2020 5b31 3035 2c20            [105, 
-00016a60: 315d 5d29 0a20 2020 203e 3e3e 206e 6173  1]]).    >>> nas
-00016a70: 7472 616e 2e77 7472 7370 6c69 6e65 2831  tran.wtrspline(1
-00016a80: 2c20 3130 2c20 6964 7329 0a20 2020 2052  , 10, ids).    R
-00016a90: 5350 4c49 4e45 2020 2020 2020 2031 3020  SPLINE       10 
-00016aa0: 2020 2020 302e 3120 2020 2020 3130 3020      0.1     100 
-00016ab0: 2020 2020 3130 3120 2031 3233 3435 3620      101  123456 
-00016ac0: 2020 2020 3130 3220 2031 3233 3435 3620      102  123456 
-00016ad0: 2020 2020 3130 330a 2020 2020 5253 504c      103.    RSPL
-00016ae0: 494e 4520 2020 2020 2020 3131 2020 2020  INE       11    
-00016af0: 2030 2e31 2020 2020 2031 3033 2020 2020   0.1     103    
-00016b00: 2031 3034 2020 3132 3334 3536 2020 2020   104  123456    
-00016b10: 2031 3035 0a20 2020 2022 2222 0a20 2020   105.    """.   
-00016b20: 2069 6473 203d 206e 702e 6174 6c65 6173   ids = np.atleas
-00016b30: 745f 3264 2869 6473 292e 6173 7479 7065  t_2d(ids).astype
-00016b40: 286e 702e 696e 7436 3429 0a20 2020 204e  (np.int64).    N
-00016b50: 203d 2069 6473 2e73 6861 7065 5b30 5d0a   = ids.shape[0].
-00016b60: 2020 2020 6966 204e 203c 2033 3a0a 2020      if N < 3:.  
-00016b70: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00016b80: 6545 7272 6f72 2822 6e6f 7420 656e 6f75  eError("not enou
-00016b90: 6768 2067 7269 6473 2066 6f72 2052 5350  gh grids for RSP
-00016ba0: 4c49 4e45 2229 0a0a 2020 2020 6964 732c  LINE")..    ids,
-00016bb0: 2069 6e64 203d 2069 6473 2e54 0a20 2020   ind = ids.T.   
-00016bc0: 2069 6620 696e 642e 616c 6c28 293a 0a20   if ind.all():. 
-00016bd0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00016be0: 7565 4572 726f 7228 2274 6865 7265 2061  ueError("there a
-00016bf0: 7265 206e 6f20 6465 7065 6e64 656e 7420  re no dependent 
-00016c00: 444f 4620 666f 7220 5253 504c 494e 4522  DOF for RSPLINE"
-00016c10: 290a 0a20 2020 2069 6620 6e6f 7420 696e  )..    if not in
-00016c20: 645b 305d 203d 3d20 696e 645b 2d31 5d20  d[0] == ind[-1] 
-00016c30: 3d3d 2031 3a0a 2020 2020 2020 2020 7261  == 1:.        ra
-00016c40: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00016c50: 7468 6520 6669 7273 7420 616e 6420 6c61  the first and la
-00016c60: 7374 2067 7269 6473 206d 7573 7420 6265  st grids must be
-00016c70: 2069 6e64 6570 656e 6465 6e74 2229 0a0a   independent")..
-00016c80: 2020 2020 2320 6669 6e64 2069 6e64 6963      # find indic
-00016c90: 6573 206f 6620 616c 6c20 6465 7065 6e64  es of all depend
-00016ca0: 656e 7473 3a0a 2020 2020 6465 7073 203d  ents:.    deps =
-00016cb0: 2028 696e 6420 3d3d 2030 292e 6e6f 6e7a   (ind == 0).nonz
-00016cc0: 6572 6f28 295b 305d 0a0a 2020 2020 2320  ero()[0]..    # 
-00016cd0: 6669 6e64 2067 6170 7320 696e 2069 6e64  find gaps in ind
-00016ce0: 6963 6573 206f 6620 6465 7065 6e64 656e  ices of dependen
-00016cf0: 7473 206c 6973 743a 0a20 2020 2067 6170  ts list:.    gap
-00016d00: 7320 3d20 286e 702e 6469 6666 2864 6570  s = (np.diff(dep
-00016d10: 7329 2021 3d20 3129 2e6e 6f6e 7a65 726f  s) != 1).nonzero
-00016d20: 2829 5b30 5d0a 0a20 2020 2023 2073 7461  ()[0]..    # sta
-00016d30: 7274 696e 6720 696e 6469 6365 7320 6f66  rting indices of
-00016d40: 2064 6570 656e 6465 6e74 733a 0a20 2020   dependents:.   
-00016d50: 2066 6972 7374 7320 3d20 6465 7073 5b6e   firsts = deps[n
-00016d60: 702e 6873 7461 636b 2828 302c 2067 6170  p.hstack((0, gap
-00016d70: 7320 2b20 3129 295d 0a0a 2020 2020 2320  s + 1))]..    # 
-00016d80: 656e 6469 6e67 2069 6e64 6963 6573 206f  ending indices o
-00016d90: 6620 6465 7065 6e64 656e 7473 3a0a 2020  f dependents:.  
-00016da0: 2020 6c61 7374 7320 3d20 6465 7073 5b6e    lasts = deps[n
-00016db0: 702e 6873 7461 636b 2828 6761 7073 2c20  p.hstack((gaps, 
-00016dc0: 6c65 6e28 6465 7073 2920 2d20 3129 295d  len(deps) - 1))]
-00016dd0: 0a0a 2020 2020 2320 7772 6974 6520 6f6e  ..    # write on
-00016de0: 6520 5253 504c 494e 4520 7065 7220 7365  e RSPLINE per se
-00016df0: 7269 6573 206f 6620 6465 7065 6e64 656e  ries of dependen
-00016e00: 7473 3a0a 2020 2020 666f 7220 6430 2c20  ts:.    for d0, 
-00016e10: 6431 2069 6e20 7a69 7028 6669 7273 7473  d1 in zip(firsts
-00016e20: 2c20 6c61 7374 7329 3a0a 2020 2020 2020  , lasts):.      
-00016e30: 2020 662e 7772 6974 6528 6622 5253 504c    f.write(f"RSPL
-00016e40: 494e 4520 7b72 6964 3a38 7d7b 446f 4c3a  INE {rid:8}{DoL:
-00016e50: 3e38 7d7b 6964 735b 6430 202d 2031 5d3a  >8}{ids[d0 - 1]:
-00016e60: 387d 2229 0a20 2020 2020 2020 2072 6964  8}").        rid
-00016e70: 202b 3d20 310a 2020 2020 2020 2020 6669   += 1.        fi
-00016e80: 656c 6420 3d20 3520 2023 206e 6578 7420  eld = 5  # next 
-00016e90: 6e61 7374 7261 6e20 6669 656c 6420 2831  nastran field (1
-00016ea0: 2074 6f20 3130 290a 0a20 2020 2020 2020   to 10)..       
-00016eb0: 2023 2077 7269 7465 2061 6c6c 2062 7574   # write all but
-00016ec0: 206c 6173 7420 6772 6964 206f 6620 6375   last grid of cu
-00016ed0: 7272 656e 7420 7365 676d 656e 743a 0a20  rrent segment:. 
-00016ee0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-00016ef0: 7261 6e67 6528 6430 2c20 6431 202b 2031  range(d0, d1 + 1
-00016f00: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-00016f10: 2e77 7269 7465 2866 227b 6964 735b 6a5d  .write(f"{ids[j]
-00016f20: 3a38 7d22 290a 2020 2020 2020 2020 2020  :8}").          
-00016f30: 2020 6669 656c 6420 2b3d 2031 0a20 2020    field += 1.   
-00016f40: 2020 2020 2020 2020 2069 6620 6669 656c           if fiel
-00016f50: 6420 3d3d 2031 303a 0a20 2020 2020 2020  d == 10:.       
-00016f60: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00016f70: 2822 5c6e 2020 2020 2020 2020 2229 0a20  ("\n        "). 
-00016f80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00016f90: 6965 6c64 203d 2032 0a20 2020 2020 2020  ield = 2.       
-00016fa0: 2020 2020 2066 2e77 7269 7465 2822 2020       f.write("  
-00016fb0: 3132 3334 3536 2229 0a20 2020 2020 2020  123456").       
-00016fc0: 2020 2020 2066 6965 6c64 202b 3d20 310a       field += 1.
-00016fd0: 0a20 2020 2020 2020 2023 2077 7269 7465  .        # write
-00016fe0: 2063 6c6f 7369 6e67 2069 6e64 6570 656e   closing indepen
-00016ff0: 6465 6e74 3a0a 2020 2020 2020 2020 662e  dent:.        f.
-00017000: 7772 6974 6528 6622 7b69 6473 5b64 3120  write(f"{ids[d1 
-00017010: 2b20 315d 3a38 7d5c 6e22 290a 0a0a 6465  + 1]:8}\n")...de
-00017020: 6620 5f69 6e74 6572 7365 6374 2863 6972  f _intersect(cir
-00017030: 6341 2c20 6369 7263 422c 2078 7941 2c20  cA, circB, xyA, 
-00017040: 6472 6177 3d46 616c 7365 293a 0a20 2020  draw=False):.   
-00017050: 2022 2222 0a20 2020 2046 696e 6420 7768   """.    Find wh
-00017060: 6572 6520 6120 6c69 6e65 2074 6861 7420  ere a line that 
-00017070: 7061 7373 6573 2074 6872 6f75 6768 2074  passes through t
-00017080: 6865 2063 656e 7465 7220 6f66 2063 6972  he center of cir
-00017090: 6341 2061 6e64 0a20 2020 2070 6f69 6e74  cA and.    point
-000170a0: 2078 7941 2069 6e74 6572 7365 6374 7320   xyA intersects 
-000170b0: 6369 7263 422e 0a0a 2020 2020 5061 7261  circB...    Para
-000170c0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-000170d0: 2d2d 2d2d 2d0a 2020 2020 6369 7263 4120  -----.    circA 
-000170e0: 3a20 332d 656c 656d 656e 7420 6172 7261  : 3-element arra
-000170f0: 795f 6c69 6b65 0a20 2020 2020 2020 205b  y_like.        [
-00017100: 7863 2c20 7963 2c20 525d 2066 6f72 2063  xc, yc, R] for c
-00017110: 6972 636c 6520 410a 2020 2020 6369 7263  ircle A.    circ
-00017120: 4220 3a20 332d 656c 656d 656e 7420 6172  B : 3-element ar
-00017130: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-00017140: 205b 7863 2c20 7963 2c20 525d 2066 6f72   [xc, yc, R] for
-00017150: 2063 6972 636c 6520 420a 2020 2020 7879   circle B.    xy
-00017160: 4120 3a20 322d 656c 656d 656e 7420 6172  A : 2-element ar
-00017170: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-00017180: 205b 782c 2079 5d20 706f 696e 7420 2870   [x, y] point (p
-00017190: 726f 6261 626c 7920 6f6e 2063 6972 636c  robably on circl
-000171a0: 6520 4129 0a20 2020 2064 7261 7720 3a20  e A).    draw : 
-000171b0: 626f 6f6c 3b20 6f70 7469 6f6e 616c 0a20  bool; optional. 
-000171c0: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-000171d0: 706c 6f74 2063 6972 636c 6573 2061 6e64  plot circles and
-000171e0: 2070 6f69 6e74 7320 666f 7220 7669 7375   points for visu
-000171f0: 616c 2069 6e73 7065 6374 696f 6e20 696e  al inspection in
-00017200: 0a20 2020 2020 2020 2066 6967 7572 6520  .        figure 
-00017210: 2769 6e74 6572 7365 6374 270a 0a20 2020  'intersect'..   
-00017220: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-00017230: 2d2d 2d2d 0a20 2020 2070 7420 3a20 3164  ----.    pt : 1d
-00017240: 206e 6461 7272 6179 0a20 2020 2020 2020   ndarray.       
-00017250: 205b 782c 2079 5d20 6c6f 6361 7469 6f6e   [x, y] location
-00017260: 206f 6620 696e 7465 7273 6563 7469 6f6e   of intersection
-00017270: 2070 6f69 6e74 2063 6c6f 7365 7374 2074   point closest t
-00017280: 6f20 7879 410a 0a20 2020 2045 7861 6d70  o xyA..    Examp
-00017290: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-000172a0: 0a20 2020 202e 2e20 706c 6f74 3a3a 0a20  .    .. plot::. 
-000172b0: 2020 2020 2020 203a 636f 6e74 6578 743a         :context:
-000172c0: 2063 6c6f 7365 2d66 6967 730a 0a20 2020   close-figs..   
-000172d0: 2020 2020 203e 3e3e 2066 726f 6d20 7079       >>> from py
-000172e0: 7965 7469 2e6e 6173 7472 616e 2e62 756c  yeti.nastran.bul
-000172f0: 6b20 696d 706f 7274 205f 696e 7465 7273  k import _inters
-00017300: 6563 740a 2020 2020 2020 2020 3e3e 3e20  ect.        >>> 
-00017310: 6369 7263 4120 3d20 2830 2e2c 2030 2e2c  circA = (0., 0.,
-00017320: 2031 302e 290a 2020 2020 2020 2020 3e3e   10.).        >>
-00017330: 3e20 6369 7263 4220 3d20 2830 2e2c 2030  > circB = (0., 0
-00017340: 2e2c 2031 352e 290a 2020 2020 2020 2020  ., 15.).        
-00017350: 3e3e 3e20 7879 4120 3d20 2830 2e2c 2035  >>> xyA = (0., 5
-00017360: 2e29 0a20 2020 2020 2020 203e 3e3e 205f  .).        >>> _
-00017370: 696e 7465 7273 6563 7428 6369 7263 412c  intersect(circA,
-00017380: 2063 6972 6342 2c20 5b30 2e2c 2031 2e5d   circB, [0., 1.]
-00017390: 2c20 6472 6177 3d31 290a 2020 2020 2020  , draw=1).      
-000173a0: 2020 6172 7261 7928 5b20 2030 2e2c 2020    array([  0.,  
-000173b0: 3135 2e5d 290a 2020 2020 2020 2020 3e3e  15.]).        >>
-000173c0: 3e20 5f69 6e74 6572 7365 6374 2863 6972  > _intersect(cir
-000173d0: 6341 2c20 6369 7263 422c 205b 302e 2c20  cA, circB, [0., 
-000173e0: 2d31 2e5d 290a 2020 2020 2020 2020 6172  -1.]).        ar
-000173f0: 7261 7928 5b20 2030 2e2c 202d 3135 2e5d  ray([  0., -15.]
-00017400: 290a 2020 2020 2020 2020 3e3e 3e20 5f69  ).        >>> _i
-00017410: 6e74 6572 7365 6374 2863 6972 6341 2c20  ntersect(circA, 
-00017420: 6369 7263 422c 205b 312e 2c20 302e 5d29  circB, [1., 0.])
-00017430: 0a20 2020 2020 2020 2061 7272 6179 285b  .        array([
-00017440: 2031 352e 2c20 2020 302e 5d29 0a20 2020   15.,   0.]).   
-00017450: 2020 2020 203e 3e3e 205f 696e 7465 7273       >>> _inters
-00017460: 6563 7428 6369 7263 412c 2063 6972 6342  ect(circA, circB
-00017470: 2c20 5b2d 312e 2c20 302e 5d29 0a20 2020  , [-1., 0.]).   
-00017480: 2020 2020 2061 7272 6179 285b 2d31 352e       array([-15.
-00017490: 2c20 2020 302e 5d29 0a20 2020 2022 2222  ,   0.]).    """
-000174a0: 0a20 2020 2028 7831 2c20 7931 2c20 5231  .    (x1, y1, R1
-000174b0: 2920 3d20 6369 7263 410a 2020 2020 2878  ) = circA.    (x
-000174c0: 322c 2079 3229 203d 2078 7941 0a20 2020  2, y2) = xyA.   
-000174d0: 2028 7833 2c20 7933 2c20 5233 2920 3d20   (x3, y3, R3) = 
-000174e0: 6369 7263 420a 2020 2020 6966 2061 6273  circB.    if abs
-000174f0: 2878 3220 2d20 7831 2920 3e20 3130 3020  (x2 - x1) > 100 
-00017500: 2a20 6e70 2e66 696e 666f 2866 6c6f 6174  * np.finfo(float
-00017510: 292e 6570 733a 0a20 2020 2020 2020 206d  ).eps:.        m
-00017520: 203d 2028 7932 202d 2079 3129 202f 2028   = (y2 - y1) / (
-00017530: 7832 202d 2078 3129 0a20 2020 2020 2020  x2 - x1).       
-00017540: 2062 203d 2028 7832 202a 2079 3120 2d20   b = (x2 * y1 - 
-00017550: 7831 202a 2079 3229 202f 2028 7832 202d  x1 * y2) / (x2 -
-00017560: 2078 3129 0a20 2020 2020 2020 2023 2028   x1).        # (
-00017570: 6d78 2b62 2d79 3329 2a2a 3220 2b20 2878  mx+b-y3)**2 + (x
-00017580: 2d78 3329 2a2a 3220 3d20 5233 2a2a 320a  -x3)**2 = R3**2.
-00017590: 2020 2020 2020 2020 6132 203d 206d 202a          a2 = m *
-000175a0: 206d 202b 2031 0a20 2020 2020 2020 2061   m + 1.        a
-000175b0: 3120 3d20 3220 2a20 286d 202a 2028 6220  1 = 2 * (m * (b 
-000175c0: 2d20 7933 2920 2d20 7833 2920 2f20 6132  - y3) - x3) / a2
-000175d0: 0a20 2020 2020 2020 2061 3020 3d20 2828  .        a0 = ((
-000175e0: 6220 2d20 7933 2920 2a2a 2032 202b 2078  b - y3) ** 2 + x
-000175f0: 3320 2a2a 2032 202d 2052 3320 2a2a 2032  3 ** 2 - R3 ** 2
-00017600: 2920 2f20 6132 0a20 2020 2020 2020 2078  ) / a2.        x
-00017610: 3120 3d20 2d61 3120 2f20 3220 2b20 6e70  1 = -a1 / 2 + np
-00017620: 2e73 7172 7428 2861 3120 2f20 3229 202a  .sqrt((a1 / 2) *
-00017630: 2a20 3220 2d20 6130 290a 2020 2020 2020  * 2 - a0).      
-00017640: 2020 7832 203d 202d 6131 202f 2032 202d    x2 = -a1 / 2 -
-00017650: 206e 702e 7371 7274 2828 6131 202f 2032   np.sqrt((a1 / 2
-00017660: 2920 2a2a 2032 202d 2061 3029 0a20 2020  ) ** 2 - a0).   
-00017670: 2020 2020 2079 3120 3d20 6d20 2a20 7831       y1 = m * x1
-00017680: 202b 2062 0a20 2020 2020 2020 2079 3220   + b.        y2 
-00017690: 3d20 6d20 2a20 7832 202b 2062 0a20 2020  = m * x2 + b.   
-000176a0: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
-000176b0: 206c 696e 6520 6973 2076 6572 7469 6361   line is vertica
-000176c0: 6c20 2878 3120 2620 7832 2061 7265 2075  l (x1 & x2 are u
-000176d0: 6e63 6861 6e67 6564 290a 2020 2020 2020  nchanged).      
-000176e0: 2020 2320 2020 2028 792d 7933 292a 2a32    #    (y-y3)**2
-000176f0: 202b 2028 7831 2d78 3329 2a2a 3220 3d20   + (x1-x3)**2 = 
-00017700: 5233 2a2a 320a 2020 2020 2020 2020 2320  R3**2.        # 
-00017710: 2020 2079 2d79 3320 3d20 2b2d 206e 702e     y-y3 = +- np.
-00017720: 7371 7274 2852 332a 2a32 202d 2028 7831  sqrt(R3**2 - (x1
-00017730: 2d78 3329 2a2a 3229 0a20 2020 2020 2020  -x3)**2).       
-00017740: 2079 3120 3d20 7933 202b 206e 702e 7371   y1 = y3 + np.sq
-00017750: 7274 2852 3320 2a2a 2032 202d 2028 7831  rt(R3 ** 2 - (x1
-00017760: 202d 2078 3329 202a 2a20 3229 0a20 2020   - x3) ** 2).   
-00017770: 2020 2020 2079 3220 3d20 7933 202d 206e       y2 = y3 - n
-00017780: 702e 7371 7274 2852 3320 2a2a 2032 202d  p.sqrt(R3 ** 2 -
-00017790: 2028 7831 202d 2078 3329 202a 2a20 3229   (x1 - x3) ** 2)
-000177a0: 0a20 2020 2065 7272 3120 3d20 6162 7328  .    err1 = abs(
-000177b0: 7879 415b 305d 202d 2078 3129 202b 2061  xyA[0] - x1) + a
-000177c0: 6273 2878 7941 5b31 5d20 2d20 7931 290a  bs(xyA[1] - y1).
-000177d0: 2020 2020 6572 7232 203d 2061 6273 2878      err2 = abs(x
-000177e0: 7941 5b30 5d20 2d20 7832 2920 2b20 6162  yA[0] - x2) + ab
-000177f0: 7328 7879 415b 315d 202d 2079 3229 0a20  s(xyA[1] - y2). 
-00017800: 2020 2069 6620 6572 7231 203c 2065 7272     if err1 < err
-00017810: 323a 0a20 2020 2020 2020 2070 7420 3d20  2:.        pt = 
-00017820: 6e70 2e61 7272 6179 285b 7831 2c20 7931  np.array([x1, y1
-00017830: 5d29 0a20 2020 2065 6c73 653a 0a20 2020  ]).    else:.   
-00017840: 2020 2020 2070 7420 3d20 6e70 2e61 7272       pt = np.arr
-00017850: 6179 285b 7832 2c20 7932 5d29 0a20 2020  ay([x2, y2]).   
-00017860: 2069 6620 6472 6177 3a0a 2020 2020 2020   if draw:.      
-00017870: 2020 706c 742e 6669 6775 7265 2822 696e    plt.figure("in
-00017880: 7465 7273 6563 7422 290a 2020 2020 2020  tersect").      
-00017890: 2020 706c 742e 636c 6628 290a 2020 2020    plt.clf().    
-000178a0: 2020 2020 7468 203d 206e 702e 6172 616e      th = np.aran
-000178b0: 6765 2830 2c20 3336 3129 202a 206e 702e  ge(0, 361) * np.
-000178c0: 7069 202f 2031 3830 2e30 0a20 2020 2020  pi / 180.0.     
-000178d0: 2020 2028 7831 2c20 7931 2c20 5231 2920     (x1, y1, R1) 
-000178e0: 3d20 6369 7263 410a 2020 2020 2020 2020  = circA.        
-000178f0: 706c 742e 706c 6f74 2878 3120 2b20 5231  plt.plot(x1 + R1
-00017900: 202a 206e 702e 636f 7328 7468 292c 2079   * np.cos(th), y
-00017910: 3120 2b20 5231 202a 206e 702e 7369 6e28  1 + R1 * np.sin(
-00017920: 7468 292c 206c 6162 656c 3d22 4369 7263  th), label="Circ
-00017930: 4122 290a 2020 2020 2020 2020 706c 742e  A").        plt.
-00017940: 706c 6f74 2878 3320 2b20 5233 202a 206e  plot(x3 + R3 * n
-00017950: 702e 636f 7328 7468 292c 2079 3320 2b20  p.cos(th), y3 + 
-00017960: 5233 202a 206e 702e 7369 6e28 7468 292c  R3 * np.sin(th),
-00017970: 206c 6162 656c 3d22 4369 7263 4222 290a   label="CircB").
-00017980: 2020 2020 2020 2020 706c 742e 7363 6174          plt.scat
-00017990: 7465 7228 2a78 7941 2c20 633d 2267 222c  ter(*xyA, c="g",
-000179a0: 206d 6172 6b65 723d 226f 222c 2073 3d36   marker="o", s=6
-000179b0: 302c 206c 6162 656c 3d22 7879 4122 290a  0, label="xyA").
-000179c0: 2020 2020 2020 2020 706c 742e 7363 6174          plt.scat
-000179d0: 7465 7228 2a70 742c 2063 3d22 6222 2c20  ter(*pt, c="b", 
-000179e0: 6d61 726b 6572 3d22 7622 2c20 733d 3630  marker="v", s=60
-000179f0: 2c20 6c61 6265 6c3d 2269 6e74 6572 7365  , label="interse
-00017a00: 6374 696f 6e20 6f6e 2043 6972 6342 2229  ction on CircB")
-00017a10: 0a20 2020 2020 2020 2070 6c74 2e61 7869  .        plt.axi
-00017a20: 7328 2265 7175 616c 2229 0a20 2020 2020  s("equal").     
-00017a30: 2020 2070 6c74 2e6c 6567 656e 6428 6c6f     plt.legend(lo
-00017a40: 633d 2262 6573 7422 2c20 7363 6174 7465  c="best", scatte
-00017a50: 7270 6f69 6e74 733d 3129 0a20 2020 2072  rpoints=1).    r
-00017a60: 6574 7572 6e20 7074 0a0a 0a64 6566 205f  eturn pt...def _
-00017a70: 6368 6563 6b5f 7a5f 616c 6967 6e6d 656e  check_z_alignmen
-00017a80: 7428 6369 7263 5f70 6172 6d73 2c20 746f  t(circ_parms, to
-00017a90: 6c29 3a0a 2020 2020 2320 4861 7665 2074  l):.    # Have t
-00017aa0: 776f 2064 6966 6665 7265 6e74 2074 7261  wo different tra
-00017ab0: 6e73 666f 726d 7320 746f 2061 206c 6f63  nsforms to a loc
-00017ac0: 616c 2073 7973 7465 6d20 2e2e 2e20 6861  al system ... ha
-00017ad0: 7665 2074 6f20 7573 650a 2020 2020 2320  ve to use.    # 
-00017ae0: 7361 6d65 206f 6e65 2074 6f20 6765 7420  same one to get 
-00017af0: 7072 6f70 6572 206e 6f64 6520 616c 6967  proper node alig
-00017b00: 6e69 6e67 2074 6f20 6f63 6375 7220 666f  ning to occur fo
-00017b10: 7220 5253 504c 494e 452e 2042 7574 2c0a  r RSPLINE. But,.
-00017b20: 2020 2020 2320 7468 6520 7a2d 6178 6973      # the z-axis
-00017b30: 2066 6f72 2062 6f74 6820 6265 7474 6572   for both better
-00017b40: 206d 6174 6368 2075 7020 2e2e 2e20 636f   match up ... co
-00017b50: 6d70 7574 6520 636f 7369 6e65 206f 6620  mpute cosine of 
-00017b60: 616e 676c 650a 2020 2020 2320 6265 7477  angle.    # betw
-00017b70: 6565 6e20 7468 6520 7477 6f20 7a2d 6178  een the two z-ax
-00017b80: 6573 202e 2e2e 2073 686f 756c 6420 6265  es ... should be
-00017b90: 2076 6572 7920 636c 6f73 6520 746f 2031   very close to 1
-00017ba0: 2e30 3a0a 2020 2020 7a31 203d 2063 6972  .0:.    z1 = cir
-00017bb0: 635f 7061 726d 735b 305d 2e62 6173 6963  c_parms[0].basic
-00017bc0: 326c 6f63 616c 5b32 5d0a 2020 2020 7a32  2local[2].    z2
-00017bd0: 203d 2063 6972 635f 7061 726d 735b 315d   = circ_parms[1]
-00017be0: 2e62 6173 6963 326c 6f63 616c 5b32 5d0a  .basic2local[2].
-00017bf0: 2020 2020 2320 7468 6573 6520 6172 6520      # these are 
-00017c00: 756e 6974 2076 6563 746f 7273 3b20 6e6f  unit vectors; no
-00017c10: 206e 6565 6420 746f 2064 6976 6964 6520   need to divide 
-00017c20: 6279 206d 6167 6e69 7475 6465 733a 0a20  by magnitudes:. 
-00017c30: 2020 2063 6f73 696e 6520 3d20 7a31 2e64     cosine = z1.d
-00017c40: 6f74 287a 3229 0a20 2020 2069 6620 6162  ot(z2).    if ab
-00017c50: 7328 636f 7369 6e65 2920 3c20 746f 6c3a  s(cosine) < tol:
-00017c60: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00017c70: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-00017c80: 2020 2020 2020 2022 7065 7270 656e 6469         "perpendi
-00017c90: 6375 6c61 7220 6469 7265 6374 696f 6e73  cular directions
-00017ca0: 206f 6620 6072 3167 7269 6473 6020 616e   of `r1grids` an
-00017cb0: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
-00017cc0: 6622 6072 3267 7269 6473 6020 646f 206e  f"`r2grids` do n
-00017cd0: 6f74 206d 6174 6368 3a20 7b7a 317d 2076  ot match: {z1} v
-00017ce0: 732e 207b 7a32 7d3b 2074 6865 2022 0a20  s. {z2}; the ". 
-00017cf0: 2020 2020 2020 2020 2020 2066 2263 6f73             f"cos
-00017d00: 696e 6520 6f66 2074 6865 2061 6e67 6c65  ine of the angle
-00017d10: 2062 6574 7765 656e 2074 6865 6d20 6973   between them is
-00017d20: 207b 636f 7369 6e65 7d22 0a20 2020 2020   {cosine}".     
-00017d30: 2020 2029 0a0a 0a64 6566 205f 7774 5f63     )...def _wt_c
-00017d40: 6972 636c 6531 5f63 6f6f 7264 2866 2c20  ircle1_coord(f, 
-00017d50: 636f 7264 5f69 642c 2063 656e 7465 722c  cord_id, center,
-00017d60: 2062 6173 6963 326c 6f63 616c 2c20 6e6f   basic2local, no
-00017d70: 6465 302c 206e 6f64 655f 6964 302c 206e  de0, node_id0, n
-00017d80: 616d 6573 293a 0a20 2020 2072 6566 5f63  ames):.    ref_c
-00017d90: 6f72 645f 6964 203d 2030 0a20 2020 2064  ord_id = 0.    d
-00017da0: 6973 7420 3d20 6d61 7828 312e 302c 206e  ist = max(1.0, n
-00017db0: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6365  p.linalg.norm(ce
-00017dc0: 6e74 6572 2929 0a20 2020 2070 203d 2031  nter)).    p = 1
-00017dd0: 3020 2a2a 206e 702e 666c 6f6f 7228 6e70  0 ** np.floor(np
-00017de0: 2e6c 6f67 3130 2864 6973 7429 290a 2020  .log10(dist)).  
-00017df0: 2020 6469 7374 203d 2072 6f75 6e64 2864    dist = round(d
-00017e00: 6973 7420 2f20 7029 202a 2070 0a20 2020  ist / p) * p.   
-00017e10: 206c 6f63 616c 5f63 6f72 6420 3d20 7b0a   local_cord = {.
-00017e20: 2020 2020 2020 2020 636f 7264 5f69 643a          cord_id:
-00017e30: 205b 0a20 2020 2020 2020 2020 2020 2022   [.            "
-00017e40: 434f 5244 3252 222c 0a20 2020 2020 2020  CORD2R",.       
-00017e50: 2020 2020 206e 702e 7673 7461 636b 280a       np.vstack(.
-00017e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00017e80: 2020 2020 2020 5b63 6f72 645f 6964 2c20        [cord_id, 
-00017e90: 312c 2072 6566 5f63 6f72 645f 6964 5d2c  1, ref_cord_id],
-00017ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017eb0: 2020 2020 2063 656e 7465 722c 0a20 2020       center,.   
-00017ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ed0: 2063 656e 7465 7220 2b20 6469 7374 202a   center + dist *
-00017ee0: 2062 6173 6963 326c 6f63 616c 5b32 5d2c   basic2local[2],
-00017ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017f00: 2020 2020 2063 656e 7465 7220 2b20 6469       center + di
-00017f10: 7374 202a 2062 6173 6963 326c 6f63 616c  st * basic2local
-00017f20: 5b30 5d2c 0a20 2020 2020 2020 2020 2020  [0],.           
-00017f30: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00017f40: 2020 2029 2c0a 2020 2020 2020 2020 5d0a     ),.        ].
-00017f50: 2020 2020 7d0a 2020 2020 636f 6d6d 656e      }.    commen
-00017f60: 7420 3d20 280a 2020 2020 2020 2020 6622  t = (.        f"
-00017f70: 4f72 6967 696e 206f 6620 6c6f 6361 6c20  Origin of local 
-00017f80: 434f 5244 3252 207b 636f 7264 5f69 647d  CORD2R {cord_id}
-00017f90: 2069 7320 6174 2063 656e 7465 7220 6f66   is at center of
-00017fa0: 207b 6e61 6d65 735b 305d 7d20 7269 6e67   {names[0]} ring
-00017fb0: 3b22 0a20 2020 2020 2020 2022 207a 2069  ;".        " z i
-00017fc0: 7320 7065 7270 656e 6469 6375 6c61 7220  s perpendicular 
-00017fd0: 746f 2070 6c61 6e65 206f 6620 6369 7263  to plane of circ
-00017fe0: 6c65 2c20 616e 6420 7820 6973 2061 6c69  le, and x is ali
-00017ff0: 676e 6564 2077 6974 6820 220a 2020 2020  gned with ".    
-00018000: 2020 2020 6622 6e6f 6465 207b 6e6f 6465      f"node {node
-00018010: 307d 2028 616e 6420 6e65 7720 6e6f 6465  0} (and new node
-00018020: 207b 6e6f 6465 5f69 6430 7d29 2e22 0a20   {node_id0}).". 
-00018030: 2020 2029 0a20 2020 2066 2e77 7269 7465     ).    f.write
-00018040: 286d 6b63 6f6d 6d65 6e74 2863 6f6d 6d65  (mkcomment(comme
-00018050: 6e74 2929 0a20 2020 2077 7463 6f6f 7264  nt)).    wtcoord
-00018060: 6361 7264 7328 662c 206c 6f63 616c 5f63  cards(f, local_c
-00018070: 6f72 6429 0a0a 0a64 6566 205f 7774 6772  ord)...def _wtgr
-00018080: 6964 735f 7262 6532 7328 0a20 2020 2066  ids_rbe2s(.    f
-00018090: 2c20 6369 7263 5f70 6172 6d73 2c20 6365  , circ_parms, ce
-000180a0: 6e74 6572 2c20 6261 7369 6332 6c6f 6361  nter, basic2loca
-000180b0: 6c2c 2063 6f72 645f 6964 2c20 6e6f 6465  l, cord_id, node
-000180c0: 5f69 6430 2c20 7262 6532 5f69 6430 2c20  _id0, rbe2_id0, 
-000180d0: 7269 6e67 315f 6964 732c 206e 616d 6573  ring1_ids, names
-000180e0: 0a29 3a0a 2020 2020 6e31 203d 2063 6972  .):.    n1 = cir
-000180f0: 635f 7061 726d 735b 305d 2e6c 6f63 616c  c_parms[0].local
-00018100: 2e73 6861 7065 5b31 5d0a 2020 2020 6e65  .shape[1].    ne
-00018110: 7770 7473 203d 206e 702e 7a65 726f 7328  wpts = np.zeros(
-00018120: 286e 312c 2033 2929 0a0a 2020 2020 2320  (n1, 3))..    # 
-00018130: 6465 6669 6e65 207a 206c 6f63 6174 696f  define z locatio
-00018140: 6e20 6f66 206e 6577 7074 733a 0a20 2020  n of newpts:.   
-00018150: 206e 6577 7074 735b 3a2c 2032 5d20 3d20   newpts[:, 2] = 
-00018160: 6369 7263 5f70 6172 6d73 5b31 5d2e 6c6f  circ_parms[1].lo
-00018170: 6361 6c5b 325d 2e6d 6561 6e28 290a 0a20  cal[2].mean().. 
-00018180: 2020 2023 2063 6f6d 7075 7465 2063 656e     # compute cen
-00018190: 7465 7220 6f66 2063 6972 636c 6520 3220  ter of circle 2 
-000181a0: 696e 206c 6f63 616c 2031 2063 6f6f 7264  in local 1 coord
-000181b0: 696e 6174 6573 3a0a 2020 2020 6365 6e74  inates:.    cent
-000181c0: 6572 3220 3d20 6261 7369 6332 6c6f 6361  er2 = basic2loca
-000181d0: 6c20 4020 2863 6972 635f 7061 726d 735b  l @ (circ_parms[
-000181e0: 315d 2e63 656e 7465 7220 2d20 6365 6e74  1].center - cent
-000181f0: 6572 290a 2020 2020 7261 6469 7573 203d  er).    radius =
-00018200: 2063 6972 635f 7061 726d 735b 305d 2e72   circ_parms[0].r
-00018210: 6164 6975 730a 2020 2020 666f 7220 6a20  adius.    for j 
-00018220: 696e 2072 616e 6765 286e 3129 3a0a 2020  in range(n1):.  
-00018230: 2020 2020 2020 6e65 7770 7473 5b6a 2c20        newpts[j, 
-00018240: 3a32 5d20 3d20 5f69 6e74 6572 7365 6374  :2] = _intersect
-00018250: 280a 2020 2020 2020 2020 2020 2020 5b30  (.            [0
-00018260: 2e30 2c20 302e 302c 2072 6164 6975 735d  .0, 0.0, radius]
-00018270: 2c0a 2020 2020 2020 2020 2020 2020 5b63  ,.            [c
-00018280: 656e 7465 7232 5b30 5d2c 2063 656e 7465  enter2[0], cente
-00018290: 7232 5b31 5d2c 2063 6972 635f 7061 726d  r2[1], circ_parm
-000182a0: 735b 315d 2e72 6164 6975 735d 2c0a 2020  s[1].radius],.  
-000182b0: 2020 2020 2020 2020 2020 6369 7263 5f70            circ_p
-000182c0: 6172 6d73 5b30 5d2e 6c6f 6361 6c5b 3a32  arms[0].local[:2
-000182d0: 2c20 6a5d 2c0a 2020 2020 2020 2020 290a  , j],.        ).
-000182e0: 0a20 2020 2023 2077 7269 7465 206e 6577  .    # write new
-000182f0: 2067 7269 6473 0a20 2020 2063 6f6d 6d65   grids.    comme
-00018300: 6e74 203d 2028 0a20 2020 2020 2020 2066  nt = (.        f
-00018310: 2247 7269 6473 2074 6f20 5242 4532 2074  "Grids to RBE2 t
-00018320: 6f20 7468 6520 7b6e 616d 6573 5b30 5d7d  o the {names[0]}
-00018330: 2067 7269 6473 2e20 5468 6573 6520 6772   grids. These gr
-00018340: 6964 7320 6c69 6e65 2022 0a20 2020 2020  ids line ".     
-00018350: 2020 2066 2275 7020 7769 7468 2074 6865     f"up with the
-00018360: 207b 6e61 6d65 735b 315d 7d20 6369 7263   {names[1]} circ
-00018370: 6c65 2073 6f20 7468 6174 2074 6865 2052  le so that the R
-00018380: 5350 4c49 4e45 2028 7768 6963 6820 220a  SPLINE (which ".
-00018390: 2020 2020 2020 2020 6622 7469 6573 2074          f"ties t
-000183a0: 6f67 6574 6865 7220 7468 6573 6520 6e65  ogether these ne
-000183b0: 7720 6772 6964 7320 616e 6420 7468 6520  w grids and the 
-000183c0: 7b6e 616d 6573 5b31 5d7d 2067 7269 6473  {names[1]} grids
-000183d0: 2920 7769 6c6c 2022 0a20 2020 2020 2020  ) will ".       
-000183e0: 2022 6265 2073 6d6f 6f74 682e 220a 2020   "be smooth.".  
-000183f0: 2020 290a 2020 2020 662e 7772 6974 6528    ).    f.write(
-00018400: 6d6b 636f 6d6d 656e 7428 636f 6d6d 656e  mkcomment(commen
-00018410: 7429 290a 2020 2020 7665 6320 3d20 6e70  t)).    vec = np
-00018420: 2e61 7261 6e67 6528 6e31 290a 2020 2020  .arange(n1).    
-00018430: 6e65 7769 6473 203d 206e 6f64 655f 6964  newids = node_id
-00018440: 3020 2b20 7665 630a 2020 2020 7262 6532  0 + vec.    rbe2
-00018450: 6964 7320 3d20 7262 6532 5f69 6430 202b  ids = rbe2_id0 +
-00018460: 2076 6563 0a20 2020 2077 7467 7269 6473   vec.    wtgrids
-00018470: 2866 2c20 6e65 7769 6473 2c20 7879 7a3d  (f, newids, xyz=
-00018480: 6e65 7770 7473 2c20 6370 3d63 6f72 645f  newpts, cp=cord_
-00018490: 6964 290a 0a20 2020 2063 6f6d 6d65 6e74  id)..    comment
-000184a0: 203d 2028 0a20 2020 2020 2020 2066 2252   = (.        f"R
-000184b0: 4245 3220 7468 6520 7b6e 616d 6573 5b30  BE2 the {names[0
-000184c0: 5d7d 206e 6f64 6573 2074 6f20 6e65 7720  ]} nodes to new 
-000184d0: 6e6f 6465 7320 6372 6561 7465 6420 6162  nodes created ab
-000184e0: 6f76 6520 220a 2020 2020 2020 2020 2228  ove ".        "(
-000184f0: 7468 6520 6e65 7720 6e6f 6465 7320 6172  the new nodes ar
-00018500: 6520 696e 6465 7065 6e64 656e 7429 3a22  e independent):"
-00018510: 0a20 2020 2029 0a20 2020 2066 2e77 7269  .    ).    f.wri
-00018520: 7465 286d 6b63 6f6d 6d65 6e74 2863 6f6d  te(mkcomment(com
-00018530: 6d65 6e74 2929 0a20 2020 2077 7269 7465  ment)).    write
-00018540: 722e 7665 6377 7269 7465 2866 2c20 2252  r.vecwrite(f, "R
-00018550: 4245 322c 7b7d 2c7b 7d2c 3132 3334 3536  BE2,{},{},123456
-00018560: 2c7b 7d5c 6e22 2c20 7262 6532 6964 732c  ,{}\n", rbe2ids,
-00018570: 206e 6577 6964 732c 2072 696e 6731 5f69   newids, ring1_i
-00018580: 6473 290a 2020 2020 7265 7475 726e 206e  ds).    return n
-00018590: 6577 7074 732c 206e 6577 6964 730a 0a0a  ewpts, newids...
-000185a0: 6465 6620 5f73 6f72 745f 6e5f 7772 6974  def _sort_n_writ
-000185b0: 6528 0a20 2020 2066 2c20 696e 6465 7065  e(.    f, indepe
-000185c0: 6e64 656e 742c 2063 6972 635f 7061 726d  ndent, circ_parm
-000185d0: 732c 206e 6577 7074 732c 206e 6577 6964  s, newpts, newid
-000185e0: 732c 2072 696e 6732 5f69 6473 2c20 7273  s, ring2_ids, rs
-000185f0: 706c 696e 655f 6964 302c 2044 6f4c 2c20  pline_id0, DoL, 
-00018600: 6e61 6d65 730a 293a 0a20 2020 206e 3120  names.):.    n1 
-00018610: 3d20 6369 7263 5f70 6172 6d73 5b30 5d2e  = circ_parms[0].
-00018620: 6c6f 6361 6c2e 7368 6170 655b 315d 0a20  local.shape[1]. 
-00018630: 2020 206e 3220 3d20 6369 7263 5f70 6172     n2 = circ_par
-00018640: 6d73 5b31 5d2e 6c6f 6361 6c2e 7368 6170  ms[1].local.shap
-00018650: 655b 315d 0a0a 2020 2020 2320 2d20 746f  e[1]..    # - to
-00018660: 2064 6f20 7468 6973 2069 6e20 6f72 6465   do this in orde
-00018670: 722c 2077 6520 6e65 6564 2074 6f20 636f  r, we need to co
-00018680: 6d70 7574 6520 7468 6569 7220 616e 676c  mpute their angl
-00018690: 6573 0a20 2020 2074 685f 3120 3d20 6e70  es.    th_1 = np
-000186a0: 2e61 7263 7461 6e32 286e 6577 7074 735b  .arctan2(newpts[
-000186b0: 3a2c 2031 5d2c 206e 6577 7074 735b 3a2c  :, 1], newpts[:,
-000186c0: 2030 5d29 0a20 2020 2072 325f 6c6f 6361   0]).    r2_loca
-000186d0: 6c20 3d20 6369 7263 5f70 6172 6d73 5b31  l = circ_parms[1
-000186e0: 5d2e 6c6f 6361 6c2e 540a 2020 2020 7468  ].local.T.    th
-000186f0: 5f32 203d 206e 702e 6172 6374 616e 3228  _2 = np.arctan2(
-00018700: 7232 5f6c 6f63 616c 5b3a 2c20 315d 2c20  r2_local[:, 1], 
-00018710: 7232 5f6c 6f63 616c 5b3a 2c20 305d 290a  r2_local[:, 0]).
-00018720: 2020 2020 7468 203d 206e 702e 6873 7461      th = np.hsta
-00018730: 636b 2828 7468 5f31 2c20 7468 5f32 2929  ck((th_1, th_2))
-00018740: 0a20 2020 2074 685b 7468 203c 202d 3165  .    th[th < -1e
-00018750: 2d38 5d20 2b3d 2032 202a 206e 702e 7069  -8] += 2 * np.pi
-00018760: 0a0a 2020 2020 6964 735f 3120 3d20 6e70  ..    ids_1 = np
-00018770: 2e63 6f6c 756d 6e5f 7374 6163 6b28 286e  .column_stack((n
-00018780: 6577 6964 732c 206e 702e 7a65 726f 7328  ewids, np.zeros(
-00018790: 6e31 2c20 6e70 2e69 6e74 3634 2929 290a  n1, np.int64))).
-000187a0: 2020 2020 6964 735f 3220 3d20 6e70 2e63      ids_2 = np.c
-000187b0: 6f6c 756d 6e5f 7374 6163 6b28 2872 696e  olumn_stack((rin
-000187c0: 6732 5f69 6473 2c20 6e70 2e7a 6572 6f73  g2_ids, np.zeros
-000187d0: 286e 322c 206e 702e 696e 7436 3429 2929  (n2, np.int64)))
-000187e0: 0a0a 2020 2020 6966 2069 6e64 6570 656e  ..    if indepen
-000187f0: 6465 6e74 203d 3d20 2272 696e 6731 223a  dent == "ring1":
-00018800: 0a20 2020 2020 2020 2063 6f6d 6d65 6e74  .        comment
-00018810: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00018820: 2066 2252 5350 4c49 4e45 2074 6865 207b   f"RSPLINE the {
-00018830: 6e61 6d65 735b 315d 7d20 6e6f 6465 7320  names[1]} nodes 
-00018840: 746f 2074 6865 206e 6577 206e 6f64 6573  to the new nodes
-00018850: 2063 7265 6174 6564 2022 0a20 2020 2020   created ".     
-00018860: 2020 2020 2020 2022 6162 6f76 652c 2077         "above, w
-00018870: 6974 6820 7468 6520 6e65 7720 6e6f 6465  ith the new node
-00018880: 7320 6265 696e 6720 696e 6465 7065 6e64  s being independ
-00018890: 656e 742e 220a 2020 2020 2020 2020 290a  ent.".        ).
-000188a0: 2020 2020 2020 2020 6964 735f 315b 3a2c          ids_1[:,
-000188b0: 2031 5d20 3d20 310a 2020 2020 656c 7365   1] = 1.    else
-000188c0: 3a0a 2020 2020 2020 2020 636f 6d6d 656e  :.        commen
-000188d0: 7420 3d20 280a 2020 2020 2020 2020 2020  t = (.          
-000188e0: 2020 6622 5253 504c 494e 4520 7468 6520    f"RSPLINE the 
-000188f0: 6e65 7720 6e6f 6465 7320 6372 6561 7465  new nodes create
-00018900: 6420 6162 6f76 6520 746f 2074 6865 207b  d above to the {
-00018910: 6e61 6d65 735b 315d 7d20 220a 2020 2020  names[1]} ".    
-00018920: 2020 2020 2020 2020 6622 6e6f 6465 732c          f"nodes,
-00018930: 2077 6974 6820 7468 6520 7b6e 616d 6573   with the {names
-00018940: 5b31 5d7d 206e 6f64 6573 2062 6569 6e67  [1]} nodes being
-00018950: 2069 6e64 6570 656e 6465 6e74 2e22 0a20   independent.". 
-00018960: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018970: 2069 6473 5f32 5b3a 2c20 315d 203d 2031   ids_2[:, 1] = 1
-00018980: 0a0a 2020 2020 662e 7772 6974 6528 6d6b  ..    f.write(mk
-00018990: 636f 6d6d 656e 7428 636f 6d6d 656e 7429  comment(comment)
-000189a0: 290a 2020 2020 6964 7320 3d20 6e70 2e76  ).    ids = np.v
-000189b0: 7374 6163 6b28 2869 6473 5f31 2c20 6964  stack((ids_1, id
-000189c0: 735f 3229 290a 0a20 2020 2023 2073 6f72  s_2))..    # sor
-000189d0: 7420 6279 2061 6e67 756c 6172 206c 6f63  t by angular loc
-000189e0: 6174 696f 6e3a 0a20 2020 2069 203d 206e  ation:.    i = n
-000189f0: 702e 6172 6773 6f72 7428 7468 290a 2020  p.argsort(th).  
-00018a00: 2020 6964 7320 3d20 6964 735b 695d 0a20    ids = ids[i]. 
-00018a10: 2020 2069 203d 2030 0a20 2020 2077 6869     i = 0.    whi
-00018a20: 6c65 2069 6473 5b69 2c20 315d 203d 3d20  le ids[i, 1] == 
-00018a30: 303a 0a20 2020 2020 2020 2069 202b 3d20  0:.        i += 
-00018a40: 310a 2020 2020 2320 7374 6163 6b20 6964  1.    # stack id
-00018a50: 732c 2065 6e73 7572 696e 6720 7374 6172  s, ensuring star
-00018a60: 7469 6e67 2061 6e64 2065 6e64 696e 6720  ting and ending 
-00018a70: 6e6f 6465 2069 7320 696e 6465 7065 6e64  node is independ
-00018a80: 656e 743a 0a20 2020 2069 6473 203d 206e  ent:.    ids = n
-00018a90: 702e 7673 7461 636b 2828 6964 735b 693a  p.vstack((ids[i:
-00018aa0: 5d2c 2069 6473 5b3a 695d 2c20 6964 735b  ], ids[:i], ids[
-00018ab0: 695d 2929 0a20 2020 2077 7472 7370 6c69  i])).    wtrspli
-00018ac0: 6e65 2866 2c20 7273 706c 696e 655f 6964  ne(f, rspline_id
-00018ad0: 302c 2069 6473 2c20 446f 4c3d 446f 4c29  0, ids, DoL=DoL)
-00018ae0: 0a20 2020 2072 6574 7572 6e20 6964 730a  .    return ids.
-00018af0: 0a0a 6465 6620 5f70 6c6f 745f 7273 706c  ..def _plot_rspl
-00018b00: 696e 6528 0a20 2020 2061 782c 0a20 2020  ine(.    ax,.   
-00018b10: 2063 6972 635f 7061 726d 732c 0a20 2020   circ_parms,.   
-00018b20: 2078 797a 2c0a 2020 2020 6e65 7770 7473   xyz,.    newpts
-00018b30: 2c0a 2020 2020 6e65 7769 6473 2c0a 2020  ,.    newids,.  
-00018b40: 2020 6261 7369 6332 6c6f 6361 6c2c 0a20    basic2local,. 
-00018b50: 2020 2063 656e 7465 722c 0a20 2020 2072     center,.    r
-00018b60: 7370 6c69 6e65 5f6e 6f64 6573 2c0a 2020  spline_nodes,.  
-00018b70: 2020 7269 6e67 325f 6964 732c 0a20 2020    ring2_ids,.   
-00018b80: 206e 616d 6573 2c0a 293a 0a20 2020 2066   names,.):.    f
-00018b90: 6f72 2069 7465 6d20 696e 2022 7879 7a22  or item in "xyz"
-00018ba0: 3a0a 2020 2020 2020 2020 6765 745f 6675  :.        get_fu
-00018bb0: 6e63 203d 2067 6574 6174 7472 2861 782c  nc = getattr(ax,
-00018bc0: 2066 2267 6574 5f7b 6974 656d 7d6c 6162   f"get_{item}lab
-00018bd0: 656c 2229 0a20 2020 2020 2020 2069 6620  el").        if 
-00018be0: 6e6f 7420 6765 745f 6675 6e63 2829 3a0a  not get_func():.
-00018bf0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-00018c00: 6675 6e63 203d 2067 6574 6174 7472 2861  func = getattr(a
-00018c10: 782c 2066 2273 6574 5f7b 6974 656d 7d6c  x, f"set_{item}l
-00018c20: 6162 656c 2229 0a20 2020 2020 2020 2020  abel").         
-00018c30: 2020 2073 6574 5f66 756e 6328 6974 656d     set_func(item
-00018c40: 2e75 7070 6572 2829 290a 0a20 2020 2023  .upper())..    #
-00018c50: 2064 7261 7720 7468 6520 6669 7420 666f   draw the fit fo
-00018c60: 7220 6369 7263 6c65 733a 0a20 2020 2074  r circles:.    t
-00018c70: 6820 3d20 6e70 2e64 6567 3272 6164 286e  h = np.deg2rad(n
-00018c80: 702e 6172 616e 6765 2830 2e30 2c20 3336  p.arange(0.0, 36
-00018c90: 3129 290a 2020 2020 666f 7220 6e75 6d2c  1)).    for num,
-00018ca0: 2028 7061 726d 732c 206c 696e 6529 2069   (parms, line) i
-00018cb0: 6e20 656e 756d 6572 6174 6528 7a69 7028  n enumerate(zip(
-00018cc0: 6369 7263 5f70 6172 6d73 2c20 2822 2b22  circ_parms, ("+"
-00018cd0: 2c20 2278 2229 2929 3a0a 2020 2020 2020  , "x"))):.      
-00018ce0: 2020 7820 3d20 7061 726d 732e 7261 6469    x = parms.radi
-00018cf0: 7573 202a 206e 702e 636f 7328 7468 290a  us * np.cos(th).
-00018d00: 2020 2020 2020 2020 7920 3d20 7061 726d          y = parm
-00018d10: 732e 7261 6469 7573 202a 206e 702e 7369  s.radius * np.si
-00018d20: 6e28 7468 290a 2020 2020 2020 2020 7a20  n(th).        z 
-00018d30: 3d20 3020 2a20 780a 2020 2020 2020 2020  = 0 * x.        
-00018d40: 2320 7472 616e 7366 6f72 6d20 746f 2062  # transform to b
-00018d50: 6173 6963 2063 6f6f 7264 696e 6174 6573  asic coordinates
-00018d60: 2061 6e64 2070 6c6f 743a 0a20 2020 2020   and plot:.     
-00018d70: 2020 2063 6972 636c 655f 6261 7369 6320     circle_basic 
-00018d80: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00018d90: 7061 726d 732e 6365 6e74 6572 202b 2028  parms.center + (
-00018da0: 6e70 2e63 6f6c 756d 6e5f 7374 6163 6b28  np.column_stack(
-00018db0: 2878 2c20 792c 207a 2929 2040 2070 6172  (x, y, z)) @ par
-00018dc0: 6d73 2e62 6173 6963 326c 6f63 616c 290a  ms.basic2local).
-00018dd0: 2020 2020 2020 2020 292e 540a 2020 2020          ).T.    
-00018de0: 2020 2020 6820 3d20 6178 2e70 6c6f 7428      h = ax.plot(
-00018df0: 0a20 2020 2020 2020 2020 2020 202a 7879  .            *xy
-00018e00: 7a5b 6e75 6d5d 2e54 2c0a 2020 2020 2020  z[num].T,.      
-00018e10: 2020 2020 2020 6c69 6e65 2c0a 2020 2020        line,.    
-00018e20: 2020 2020 2020 2020 6d61 726b 6572 7369          markersi
-00018e30: 7a65 3d38 2e30 2c0a 2020 2020 2020 2020  ze=8.0,.        
-00018e40: 2020 2020 6d61 726b 6572 6564 6765 7769      markeredgewi
-00018e50: 6474 683d 322e 302c 0a20 2020 2020 2020  dth=2.0,.       
-00018e60: 2020 2020 206c 6162 656c 3d66 227b 6e61       label=f"{na
-00018e70: 6d65 735b 6e75 6d5d 7d20 6e6f 6465 7322  mes[num]} nodes"
-00018e80: 2c0a 2020 2020 2020 2020 295b 305d 0a20  ,.        )[0]. 
-00018e90: 2020 2020 2020 2061 782e 706c 6f74 282a         ax.plot(*
-00018ea0: 6369 7263 6c65 5f62 6173 6963 2c20 682e  circle_basic, h.
-00018eb0: 6765 745f 636f 6c6f 7228 292c 206c 6162  get_color(), lab
-00018ec0: 656c 3d66 227b 6e61 6d65 735b 6e75 6d5d  el=f"{names[num]
-00018ed0: 7d20 6265 7374 2d66 6974 2063 6972 636c  } best-fit circl
-00018ee0: 6522 290a 0a20 2020 2023 2067 6574 2062  e")..    # get b
-00018ef0: 6173 6963 2063 6f6f 7264 696e 6174 6573  asic coordinates
-00018f00: 206f 6620 6e65 7770 7473 3a0a 2020 2020   of newpts:.    
-00018f10: 6e65 7770 7473 5f62 6173 6963 203d 206e  newpts_basic = n
-00018f20: 6577 7074 7320 4020 6261 7369 6332 6c6f  ewpts @ basic2lo
-00018f30: 6361 6c20 2b20 6365 6e74 6572 0a0a 2020  cal + center..  
-00018f40: 2020 7365 676d 656e 7473 203d 206e 702e    segments = np.
-00018f50: 656d 7074 7928 2833 202a 206e 6577 7074  empty((3 * newpt
-00018f60: 732e 7368 6170 655b 305d 2c20 3329 290a  s.shape[0], 3)).
-00018f70: 2020 2020 7365 676d 656e 7473 5b3a 3a33      segments[::3
-00018f80: 5d20 3d20 6e65 7770 7473 5f62 6173 6963  ] = newpts_basic
-00018f90: 0a20 2020 2073 6567 6d65 6e74 735b 313a  .    segments[1:
-00018fa0: 3a33 5d20 3d20 7879 7a5b 305d 0a20 2020  :3] = xyz[0].   
-00018fb0: 2073 6567 6d65 6e74 735b 323a 3a33 5d20   segments[2::3] 
-00018fc0: 3d20 6e70 2e6e 616e 0a0a 2020 2020 6820  = np.nan..    h 
-00018fd0: 3d20 6178 2e70 6c6f 7428 0a20 2020 2020  = ax.plot(.     
-00018fe0: 2020 202a 6e65 7770 7473 5f62 6173 6963     *newpts_basic
-00018ff0: 2e54 2c0a 2020 2020 2020 2020 226f 222c  .T,.        "o",
-00019000: 0a20 2020 2020 2020 206d 6172 6b65 7273  .        markers
-00019010: 697a 653d 352e 302c 0a20 2020 2020 2020  ize=5.0,.       
-00019020: 206d 6172 6b65 7265 6467 6577 6964 7468   markeredgewidth
-00019030: 3d32 2e30 2c0a 2020 2020 2020 2020 6c61  =2.0,.        la
-00019040: 6265 6c3d 2822 4e65 7720 7b7d 206e 6f64  bel=("New {} nod
-00019050: 6573 5c6e 202d 2073 686f 756c 6420 6265  es\n - should be
-00019060: 206f 6e20 7b7d 2063 6972 636c 6522 292e   on {} circle").
-00019070: 666f 726d 6174 282a 6e61 6d65 7329 2c0a  format(*names),.
-00019080: 2020 2020 295b 305d 0a20 2020 2061 782e      )[0].    ax.
-00019090: 706c 6f74 280a 2020 2020 2020 2020 2a73  plot(.        *s
-000190a0: 6567 6d65 6e74 732e 542c 0a20 2020 2020  egments.T,.     
-000190b0: 2020 2022 2d22 2c0a 2020 2020 2020 2020     "-",.        
-000190c0: 636f 6c6f 723d 682e 6765 745f 636f 6c6f  color=h.get_colo
-000190d0: 7228 292c 0a20 2020 2020 2020 206c 6162  r(),.        lab
-000190e0: 656c 3d66 2252 4245 3273 202d 2073 686f  el=f"RBE2s - sho
-000190f0: 756c 6420 6265 207b 6e61 6d65 735b 305d  uld be {names[0]
-00019100: 7d20 7261 6469 616c 222c 0a20 2020 2029  } radial",.    )
-00019110: 0a0a 2020 2020 2320 706c 6f74 2074 6865  ..    # plot the
-00019120: 2072 7370 6c69 6e65 3a0a 2020 2020 756e   rspline:.    un
-00019130: 736f 7274 6564 5f72 7370 6c69 6e65 5f6e  sorted_rspline_n
-00019140: 6f64 6573 203d 206e 702e 6873 7461 636b  odes = np.hstack
-00019150: 2828 6e65 7769 6473 2c20 7269 6e67 325f  ((newids, ring2_
-00019160: 6964 7329 290a 2020 2020 7076 203d 206c  ids)).    pv = l
-00019170: 6f63 6174 652e 6d61 745f 696e 7465 7273  ocate.mat_inters
-00019180: 6563 7428 756e 736f 7274 6564 5f72 7370  ect(unsorted_rsp
-00019190: 6c69 6e65 5f6e 6f64 6573 2c20 7273 706c  line_nodes, rspl
-000191a0: 696e 655f 6e6f 6465 735b 3a2c 2030 5d2c  ine_nodes[:, 0],
-000191b0: 2032 290a 0a20 2020 2072 7370 6c69 6e65   2)..    rspline
-000191c0: 5f78 797a 203d 206e 702e 7673 7461 636b  _xyz = np.vstack
-000191d0: 2828 6e65 7770 7473 5f62 6173 6963 2c20  ((newpts_basic, 
-000191e0: 7879 7a5b 315d 2929 5b70 765b 305d 5d0a  xyz[1]))[pv[0]].
-000191f0: 2020 2020 6178 2e70 6c6f 7428 2a72 7370      ax.plot(*rsp
-00019200: 6c69 6e65 5f78 797a 2e54 2c20 222d 2d22  line_xyz.T, "--"
-00019210: 2c20 616c 7068 613d 302e 372c 206c 696e  , alpha=0.7, lin
-00019220: 6577 6964 7468 3d33 2e30 2c20 6c61 6265  ewidth=3.0, labe
-00019230: 6c3d 2246 696e 616c 2052 5350 4c49 4e45  l="Final RSPLINE
-00019240: 2229 0a0a 2020 2020 7974 6f6f 6c73 2e61  ")..    ytools.a
-00019250: 7869 735f 6571 7561 6c5f 3364 2861 7829  xis_equal_3d(ax)
-00019260: 0a20 2020 2061 782e 6c65 6765 6e64 286c  .    ax.legend(l
-00019270: 6f63 3d22 7570 7065 7220 6c65 6674 222c  oc="upper left",
-00019280: 2062 626f 785f 746f 5f61 6e63 686f 723d   bbox_to_anchor=
-00019290: 2831 2e30 2c20 312e 3029 290a 2020 2020  (1.0, 1.0)).    
-000192a0: 6178 2e67 6574 5f66 6967 7572 6528 292e  ax.get_figure().
-000192b0: 7469 6768 745f 6c61 796f 7574 2829 0a0a  tight_layout()..
-000192c0: 0a64 6566 2077 7472 7370 6c69 6e65 5f72  .def wtrspline_r
-000192d0: 696e 6773 280a 2020 2020 662c 0a20 2020  ings(.    f,.   
-000192e0: 2072 3167 7269 6473 2c0a 2020 2020 7232   r1grids,.    r2
-000192f0: 6772 6964 732c 0a20 2020 206e 6f64 655f  grids,.    node_
-00019300: 6964 302c 0a20 2020 2072 7370 6c69 6e65  id0,.    rspline
-00019310: 5f69 6430 2c0a 2020 2020 7262 6532 5f69  _id0,.    rbe2_i
-00019320: 6430 3d4e 6f6e 652c 0a20 2020 2063 6f72  d0=None,.    cor
-00019330: 645f 6964 3d4e 6f6e 652c 0a20 2020 206d  d_id=None,.    m
-00019340: 616b 6570 6c6f 743d 226e 6577 222c 0a20  akeplot="new",. 
-00019350: 2020 2044 6f4c 3d22 302e 3122 2c0a 2020     DoL="0.1",.  
-00019360: 2020 696e 6465 7065 6e64 656e 743d 2272    independent="r
-00019370: 696e 6731 222c 0a29 3a0a 2020 2020 2222  ing1",.):.    ""
-00019380: 220a 2020 2020 4372 6561 7465 7320 6120  ".    Creates a 
-00019390: 736d 6f6f 7468 2052 5350 4c49 4e45 2074  smooth RSPLINE t
-000193a0: 6f20 636f 6e6e 6563 7420 7477 6f20 7269  o connect two ri
-000193b0: 6e67 7320 6f66 2067 7269 6473 0a0a 2020  ngs of grids..  
-000193c0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000193d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000193e0: 6620 3a20 7374 7269 6e67 206f 7220 6669  f : string or fi
-000193f0: 6c65 5f6c 696b 6520 6f72 2031 206f 7220  le_like or 1 or 
-00019400: 4e6f 6e65 0a20 2020 2020 2020 2045 6974  None.        Eit
-00019410: 6865 7220 6120 6e61 6d65 206f 6620 6120  her a name of a 
-00019420: 6669 6c65 2c20 6f72 2069 7320 6120 6669  file, or is a fi
-00019430: 6c65 5f6c 696b 6520 6f62 6a65 6374 2061  le_like object a
-00019440: 7320 7265 7475 726e 6564 0a20 2020 2020  s returned.     
-00019450: 2020 2062 7920 3a66 756e 633a 606f 7065     by :func:`ope
-00019460: 6e60 206f 7220 3a63 6c61 7373 3a60 696f  n` or :class:`io
-00019470: 2e53 7472 696e 6749 4f60 2e20 496e 7075  .StringIO`. Inpu
-00019480: 7420 6173 2069 6e74 6567 6572 2031 2074  t as integer 1 t
-00019490: 6f0a 2020 2020 2020 2020 7772 6974 6520  o.        write 
-000194a0: 746f 2073 7464 6f75 742e 2043 616e 2061  to stdout. Can a
-000194b0: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
-000194c0: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
-000194d0: 7220 4e6f 6e65 3b0a 2020 2020 2020 2020  r None;.        
-000194e0: 696e 2074 6865 7365 2063 6173 6573 2c20  in these cases, 
-000194f0: 6120 4755 4920 6973 206f 7065 6e65 6420  a GUI is opened 
-00019500: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
-00019510: 6f6e 2e0a 2020 2020 7231 6772 6964 7320  on..    r1grids 
-00019520: 3a20 3264 2061 7272 6179 5f6c 696b 6520  : 2d array_like 
-00019530: 6f72 2044 6174 6146 7261 6d65 206f 7220  or DataFrame or 
-00019540: 7475 706c 650a 2020 2020 2020 2020 4967  tuple.        Ig
-00019550: 6e6f 7269 6e67 2074 6865 2074 7570 6c65  noring the tuple
-00019560: 2069 6e70 7574 206f 7074 696f 6e20 666f   input option fo
-00019570: 7220 6e6f 772c 2060 7231 6772 6964 7360  r now, `r1grids`
-00019580: 2063 6f6e 7461 696e 730a 2020 2020 2020   contains.      
-00019590: 2020 7468 6520 6964 7320 616e 6420 6c6f    the ids and lo
-000195a0: 6361 7469 6f6e 7320 6f66 2074 6865 2072  cations of the r
-000195b0: 696e 6720 3120 6772 6964 7320 696e 2062  ing 1 grids in b
-000195c0: 6173 6963 0a20 2020 2020 2020 2063 6f6f  asic.        coo
-000195d0: 7264 696e 6174 6573 2e20 4966 2032 6420  rdinates. If 2d 
-000195e0: 6172 7261 795f 6c69 6b65 2c20 6974 2068  array_like, it h
-000195f0: 6173 2034 2063 6f6c 756d 6e73 2064 6573  as 4 columns des
-00019600: 6372 6962 696e 6720 7468 650a 2020 2020  cribing the.    
-00019610: 2020 2020 7269 6e67 2031 2067 7269 6473      ring 1 grids
-00019620: 3a3a 0a0a 2020 2020 2020 2020 2020 2020  ::..            
-00019630: 205b 6964 2c20 782c 2079 2c20 7a5d 203c   [id, x, y, z] <
-00019640: 202d 2d20 6261 7369 6320 636f 6f72 6469   -- basic coordi
-00019650: 6e61 7465 730a 0a20 2020 2020 2020 2049  nates..        I
-00019660: 6620 4461 7461 4672 616d 652c 2069 7420  f DataFrame, it 
-00019670: 6973 2061 7373 756d 6564 2074 6f20 6265  is assumed to be
-00019680: 2074 6865 2055 5345 5420 4461 7461 4672   the USET DataFr
-00019690: 616d 650a 2020 2020 2020 2020 636f 6e74  ame.        cont
-000196a0: 6169 6e69 6e67 206a 7573 7420 7468 6520  aining just the 
-000196b0: 7269 6e67 2031 2067 7269 6473 2e20 5468  ring 1 grids. Th
-000196c0: 6520 666f 726d 6174 206f 6620 7468 6973  e format of this
-000196d0: 0a20 2020 2020 2020 2044 6174 6146 7261  .        DataFra
-000196e0: 6d65 2069 7320 6465 7363 7269 6265 6420  me is described 
-000196f0: 696e 0a20 2020 2020 2020 203a 6675 6e63  in.        :func
-00019700: 3a60 7079 7965 7469 2e6e 6173 7472 616e  :`pyyeti.nastran
-00019710: 2e6f 7032 2e4f 5032 2e72 646e 3263 6f70  .op2.OP2.rdn2cop
-00019720: 3260 2e0a 0a20 2020 2020 2020 2054 6865  2`...        The
-00019730: 2064 6566 6175 6c74 206e 616d 6520 696e   default name in
-00019740: 2074 6865 206f 7574 7075 7420 636f 6d6d   the output comm
-00019750: 656e 7473 2066 6f72 2072 696e 6720 3120  ents for ring 1 
-00019760: 6973 2027 5269 6e67 0a20 2020 2020 2020  is 'Ring.       
-00019770: 2031 272e 2042 7920 7573 696e 6720 7468   1'. By using th
-00019780: 6520 7475 706c 6520 696e 7075 7420 6f70  e tuple input op
-00019790: 7469 6f6e 2c20 796f 7520 6361 6e20 7072  tion, you can pr
-000197a0: 6f76 6964 6520 610a 2020 2020 2020 2020  ovide a.        
-000197b0: 6e61 6d65 2e20 466f 7220 6578 616d 706c  name. For exampl
-000197c0: 652c 2074 6865 2064 6566 6175 6c74 2069  e, the default i
-000197d0: 7320 6571 7569 7661 6c65 6e74 2074 6f3a  s equivalent to:
-000197e0: 3a0a 0a20 2020 2020 2020 2020 2020 2028  :..            (
-000197f0: 2752 696e 6720 3127 2c20 7231 6772 6964  'Ring 1', r1grid
-00019800: 7329 0a0a 2020 2020 2020 2020 2e2e 206e  s)..        .. n
-00019810: 6f74 653a 3a0a 2020 2020 2020 2020 2020  ote::.          
-00019820: 2020 204e 6f74 6520 7468 6174 2077 6865     Note that whe
-00019830: 6e20 7573 696e 6720 6120 5553 4554 2074  n using a USET t
-00019840: 6162 6c65 2c20 7468 6520 6772 6964 7320  able, the grids 
-00019850: 6361 6e20 6265 0a20 2020 2020 2020 2020  can be.         
-00019860: 2020 2020 6465 6669 6e65 6420 696e 2061      defined in a
-00019870: 6e79 206c 6f63 616c 2063 6f6f 7264 696e  ny local coordin
-00019880: 6174 6520 7379 7374 656d 2873 292e 2048  ate system(s). H
-00019890: 6f77 6576 6572 2c20 626f 7468 0a20 2020  owever, both.   
-000198a0: 2020 2020 2020 2020 2020 6072 3167 7269            `r1gri
-000198b0: 6473 6020 616e 6420 6072 3267 7269 6473  ds` and `r2grids
-000198c0: 6020 6d75 7374 2075 7365 2074 6865 2073  ` must use the s
-000198d0: 616d 6520 6261 7369 630a 2020 2020 2020  ame basic.      
-000198e0: 2020 2020 2020 2063 6f6f 7264 696e 6174         coordinat
-000198f0: 6520 7379 7374 656d 2e0a 0a20 2020 2072  e system...    r
-00019900: 3267 7269 6473 203a 2032 6420 6172 7261  2grids : 2d arra
-00019910: 795f 6c69 6b65 206f 7220 4461 7461 4672  y_like or DataFr
-00019920: 616d 6520 6f72 2074 7570 6c65 0a20 2020  ame or tuple.   
-00019930: 2020 2020 2043 6f6e 7461 696e 7320 7468       Contains th
-00019940: 6520 6964 7320 616e 6420 6c6f 6361 7469  e ids and locati
-00019950: 6f6e 7320 2861 6e64 206f 7074 696f 6e61  ons (and optiona
-00019960: 6c6c 792c 2074 6865 206e 616d 6529 206f  lly, the name) o
-00019970: 660a 2020 2020 2020 2020 7468 6520 7269  f.        the ri
-00019980: 6e67 2032 2067 7269 6473 2069 6e20 6261  ng 2 grids in ba
-00019990: 7369 6320 636f 6f72 6469 6e61 7465 732e  sic coordinates.
-000199a0: 2053 6565 2060 7231 6772 6964 7360 2066   See `r1grids` f
-000199b0: 6f72 0a20 2020 2020 2020 2064 6573 6372  or.        descr
-000199c0: 6970 7469 6f6e 206f 6620 666f 726d 6174  iption of format
-000199d0: 2e20 5468 6520 6465 6661 756c 7420 6e61  . The default na
-000199e0: 6d65 2066 6f72 2072 696e 6720 3220 6973  me for ring 2 is
-000199f0: 2027 5269 6e67 0a20 2020 2020 2020 2032   'Ring.        2
-00019a00: 272e 0a20 2020 206e 6f64 655f 6964 3020  '..    node_id0 
-00019a10: 3a20 696e 7465 6765 720a 2020 2020 2020  : integer.      
-00019a20: 2020 3173 7420 6964 206f 6620 6e65 7720    1st id of new 
-00019a30: 6e6f 6465 7320 6372 6561 7465 6420 746f  nodes created to
-00019a40: 2027 6d6f 7665 2720 7269 6e67 2031 206e   'move' ring 1 n
-00019a50: 6f64 6573 0a20 2020 2072 7370 6c69 6e65  odes.    rspline
-00019a60: 5f69 6430 203a 2069 6e74 6567 6572 0a20  _id0 : integer. 
-00019a70: 2020 2020 2020 2031 7374 2069 6420 6f66         1st id of
-00019a80: 2052 5350 4c49 4e45 730a 2020 2020 7262   RSPLINEs.    rb
-00019a90: 6532 5f69 6430 203a 2069 6e74 6567 6572  e2_id0 : integer
-00019aa0: 206f 7220 4e6f 6e65 3b20 6f70 7469 6f6e   or None; option
-00019ab0: 616c 0a20 2020 2020 2020 2031 7374 2069  al.        1st i
-00019ac0: 6420 6f66 2052 4245 3220 656c 656d 656e  d of RBE2 elemen
-00019ad0: 7473 2074 6861 7420 7769 6c6c 2063 6f6e  ts that will con
-00019ae0: 6e65 6374 206f 6c64 2072 696e 6720 3120  nect old ring 1 
-00019af0: 6e6f 6465 7320 746f 0a20 2020 2020 2020  nodes to.       
-00019b00: 206e 6577 206f 6e65 732e 2049 6620 4e6f   new ones. If No
-00019b10: 6e65 2c20 6060 7262 6532 5f69 6430 203d  ne, ``rbe2_id0 =
-00019b20: 206e 6f64 655f 6964 3060 602e 0a20 2020   node_id0``..   
-00019b30: 2063 6f72 645f 6964 203a 2069 6e74 6567   cord_id : integ
-00019b40: 6572 206f 7220 4e6f 6e65 3b20 6f70 7469  er or None; opti
-00019b50: 6f6e 616c 0a20 2020 2020 2020 2049 4420  onal.        ID 
-00019b60: 666f 7220 7468 6520 6c6f 6361 6c20 636f  for the local co
-00019b70: 6f72 6469 6e61 7465 2073 7973 7465 6d20  ordinate system 
-00019b80: 666f 7220 7468 6520 6072 3167 7269 6473  for the `r1grids
-00019b90: 602e 2049 6620 4e6f 6e65 2c0a 2020 2020  `. If None,.    
-00019ba0: 2020 2020 6974 2069 7320 7365 7420 746f      it is set to
-00019bb0: 2060 606e 6f64 655f 6964 3020 2a20 3130   ``node_id0 * 10
-00019bc0: 6060 2e0a 2020 2020 6d61 6b65 706c 6f74  ``..    makeplot
-00019bd0: 203a 2073 7472 696e 6720 6f72 2061 7865   : string or axe
-00019be0: 7320 6f62 6a65 6374 3b20 6f70 7469 6f6e  s object; option
-00019bf0: 616c 0a20 2020 2020 2020 2053 7065 6369  al.        Speci
-00019c00: 6669 6573 2069 6620 616e 6420 686f 7720  fies if and how 
-00019c10: 746f 2070 6c6f 7420 6461 7461 2073 686f  to plot data sho
-00019c20: 7769 6e67 2074 6865 2052 5350 4c49 4e45  wing the RSPLINE
-00019c30: 2e0a 0a20 2020 2020 2020 203d 3d3d 3d3d  ...        =====
-00019c40: 3d3d 3d3d 3d3d 2020 203d 3d3d 3d3d 3d3d  ======   =======
-00019c50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019c60: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020 2020  ========.       
-00019c70: 2060 6d61 6b65 706c 6f74 6020 2020 2044   `makeplot`    D
-00019c80: 6573 6372 6970 7469 6f6e 0a20 2020 2020  escription.     
-00019c90: 2020 203d 3d3d 3d3d 3d3d 3d3d 3d3d 2020     ===========  
-00019ca0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-00019cb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019cc0: 0a20 2020 2020 2020 2020 2020 2027 6e6f  .            'no
-00019cd0: 2720 2020 2020 2064 6f20 6e6f 7420 706c  '      do not pl
-00019ce0: 6f74 0a20 2020 2020 2020 2020 2763 6c65  ot.         'cle
-00019cf0: 6172 2720 2020 2020 2070 6c6f 7420 6166  ar'      plot af
-00019d00: 7465 7220 636c 6561 7269 6e67 2066 6967  ter clearing fig
-00019d10: 7572 650a 2020 2020 2020 2020 2020 2027  ure.           '
-00019d20: 6164 6427 2020 2020 2020 706c 6f74 2077  add'      plot w
-00019d30: 6974 686f 7574 2063 6c65 6172 696e 6720  ithout clearing 
-00019d40: 6669 6775 7265 0a20 2020 2020 2020 2020  figure.         
-00019d50: 2020 276e 6577 2720 2020 2020 2070 6c6f    'new'      plo
-00019d60: 7420 696e 206e 6577 2066 6967 7572 650a  t in new figure.
-00019d70: 2020 2020 2020 2020 6178 6573 206f 626a          axes obj
-00019d80: 6563 7420 2020 706c 6f74 2069 6e20 6769  ect   plot in gi
-00019d90: 7665 6e20 6178 6573 2028 6c69 6b65 2027  ven axes (like '
-00019da0: 6164 6427 290a 2020 2020 2020 2020 3d3d  add').        ==
-00019db0: 3d3d 3d3d 3d3d 3d3d 3d20 2020 3d3d 3d3d  =========   ====
-00019dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020  ===========..   
-00019de0: 2020 2020 204e 6f74 6520 7468 6174 2069       Note that i
-00019df0: 6620 606d 616b 6570 6c6f 7460 2069 7320  f `makeplot` is 
-00019e00: 2761 6464 2720 6f72 2061 6e20 6178 6573  'add' or an axes
-00019e10: 206f 626a 6563 742c 2069 7420 6d75 7374   object, it must
-00019e20: 2062 650a 2020 2020 2020 2020 3364 3b20   be.        3d; 
-00019e30: 6f74 6865 7277 6973 6520 6120 5661 6c75  otherwise a Valu
-00019e40: 6545 7272 6f72 2065 7863 6570 7469 6f6e  eError exception
-00019e50: 2069 7320 7261 6973 6564 2e0a 0a20 2020   is raised...   
-00019e60: 2044 6f4c 203a 2073 7472 696e 6720 6f72   DoL : string or
-00019e70: 2072 6561 6c20 7363 616c 6172 3b20 6f70   real scalar; op
-00019e80: 7469 6f6e 616c 0a20 2020 2020 2020 2053  tional.        S
-00019e90: 7065 6369 6669 6573 2072 6174 696f 206f  pecifies ratio o
-00019ea0: 6620 6469 616d 6574 6572 206f 6620 656c  f diameter of el
-00019eb0: 6173 7469 6320 7479 6265 2074 6f20 7468  astic tybe to th
-00019ec0: 6520 7375 6d20 6f66 2074 6865 0a20 2020  e sum of the.   
-00019ed0: 2020 2020 206c 656e 6774 6873 206f 6620       lengths of 
-00019ee0: 616c 6c20 7365 676d 656e 7473 2e20 5772  all segments. Wr
-00019ef0: 6974 7465 6e20 7769 7468 3a20 6060 6627  itten with: ``f'
-00019f00: 7b44 6f4c 3a3c 387d 2760 600a 2020 2020  {DoL:<8}'``.    
-00019f10: 696e 6465 7065 6e64 656e 7420 3a20 7374  independent : st
-00019f20: 723b 206f 7074 696f 6e61 6c0a 2020 2020  r; optional.    
-00019f30: 2020 2020 4569 7468 6572 2027 7269 6e67      Either 'ring
-00019f40: 3127 206f 7220 2772 696e 6732 2720 6f72  1' or 'ring2' or
-00019f50: 2074 6865 2061 7373 6967 6e65 6420 6e61   the assigned na
-00019f60: 6d65 2069 6620 6f6e 6520 7761 730a 2020  me if one was.  
-00019f70: 2020 2020 2020 7072 6f76 6964 6564 2069        provided i
-00019f80: 6e20 7468 6520 6072 3167 7269 6473 6020  n the `r1grids` 
-00019f90: 6f72 2060 7232 6772 6964 7360 2069 6e70  or `r2grids` inp
-00019fa0: 7574 2e20 5468 6973 2069 6e70 7574 2069  ut. This input i
-00019fb0: 730a 2020 2020 2020 2020 6361 7365 2d69  s.        case-i
-00019fc0: 6e73 656e 7369 7469 7665 2061 6e64 2061  nsensitive and a
-00019fd0: 6c6c 2073 7061 6365 7320 6172 6520 6967  ll spaces are ig
-00019fe0: 6e6f 7265 642c 2073 6f20 2752 696e 6720  nored, so 'Ring 
-00019ff0: 3127 2069 730a 2020 2020 2020 2020 7468  1' is.        th
-0001a000: 6520 7361 6d65 2061 7320 2772 696e 6731  e same as 'ring1
-0001a010: 272e 2053 7065 6369 6669 6573 2077 6869  '. Specifies whi
-0001a020: 6368 2072 696e 6720 7769 6c6c 2062 6520  ch ring will be 
-0001a030: 696e 6465 7065 6e64 656e 740a 2020 2020  independent.    
-0001a040: 2020 2020 6f6e 2074 6865 2052 5350 4c49      on the RSPLI
-0001a050: 4e45 732e 204e 6f74 6520 7468 6174 2069  NEs. Note that i
-0001a060: 7320 6469 6666 6572 656e 7420 7468 616e  s different than
-0001a070: 206a 7573 7420 7377 6974 6368 696e 670a   just switching.
-0001a080: 2020 2020 2020 2020 7468 6520 6f72 6465          the orde
-0001a090: 7220 6f66 2060 7231 6772 6964 7360 2061  r of `r1grids` a
-0001a0a0: 6e64 2060 7232 6772 6964 7360 2e20 5468  nd `r2grids`. Th
-0001a0b0: 6973 206f 7074 696f 6e20 6d6f 6469 6669  is option modifi
-0001a0c0: 6573 0a20 2020 2020 2020 2073 7465 7020  es.        step 
-0001a0d0: 3420 6265 6c6f 7720 7768 696c 6520 7377  4 below while sw
-0001a0e0: 6974 6368 696e 6720 6072 3167 7269 6473  itching `r1grids
-0001a0f0: 6020 616e 6420 6072 3267 7269 6473 6020  ` and `r2grids` 
-0001a100: 6d6f 6469 6669 6573 0a20 2020 2020 2020  modifies.       
-0001a110: 2061 6c6c 2074 6865 2073 7465 7073 2e0a   all the steps..
-0001a120: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-0001a130: 202d 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e   -------.    Non
-0001a140: 650a 0a20 2020 204e 6f74 6573 0a20 2020  e..    Notes.   
-0001a150: 202d 2d2d 2d2d 0a20 2020 2054 6869 7320   -----.    This 
-0001a160: 726f 7574 696e 6520 7772 6974 6573 2047  routine writes G
-0001a170: 5249 442c 2052 4245 3220 616e 6420 5253  RID, RBE2 and RS
-0001a180: 504c 494e 4520 6c69 6e65 7320 746f 2074  PLINE lines to t
-0001a190: 6865 206f 7574 7075 740a 2020 2020 6669  he output.    fi
-0001a1a0: 6c65 2e0a 0a20 2020 2054 6865 2061 7070  le...    The app
-0001a1b0: 726f 6163 6820 6973 2061 7320 666f 6c6c  roach is as foll
-0001a1c0: 6f77 7320 284e 203d 206e 756d 6265 7220  ows (N = number 
-0001a1d0: 6f66 2072 696e 6720 3120 6772 6964 7329  of ring 1 grids)
-0001a1e0: 3a0a 0a20 2020 2020 2031 2e20 4669 7420  :..      1. Fit 
-0001a1f0: 6120 6369 7263 6c65 2074 6872 6f75 6768  a circle through
-0001a200: 2062 6f74 6820 7468 6520 7269 6e67 2031   both the ring 1
-0001a210: 206e 6f64 6573 2061 6e64 2074 6865 2072   nodes and the r
-0001a220: 696e 6720 320a 2020 2020 2020 2020 206e  ing 2.         n
-0001a230: 6f64 6573 2e20 4120 6e65 7720 2272 696e  odes. A new "rin
-0001a240: 6720 3122 206c 6f63 616c 2063 6f6f 7264  g 1" local coord
-0001a250: 696e 6174 6520 7379 7374 656d 2069 7320  inate system is 
-0001a260: 6465 6669 6e65 6420 2873 6565 0a20 2020  defined (see.   
-0001a270: 2020 2020 2020 3a66 756e 633a 6070 7979        :func:`pyy
-0001a280: 6574 692e 7974 6f6f 6c73 2e66 6974 5f63  eti.ytools.fit_c
-0001a290: 6972 636c 655f 3364 6029 2074 6f20 7369  ircle_3d`) to si
-0001a2a0: 6d70 6c69 6679 2074 6865 2063 7265 6174  mplify the creat
-0001a2b0: 696f 6e0a 2020 2020 2020 2020 206f 6620  ion.         of 
-0001a2c0: 7468 6520 6e65 7720 5253 504c 494e 452e  the new RSPLINE.
-0001a2d0: 2049 6e20 7468 6520 6c6f 6361 6c20 7379   In the local sy
-0001a2e0: 7374 656d 2c20 7a20 6973 2070 6572 7065  stem, z is perpe
-0001a2f0: 6e64 6963 756c 6172 0a20 2020 2020 2020  ndicular.       
-0001a300: 2020 746f 2074 6865 2070 6c61 6e65 206f    to the plane o
-0001a310: 6620 7468 6520 6369 7263 6c65 2061 6e64  f the circle and
-0001a320: 2078 2069 7320 616c 6967 6e65 6420 7769   x is aligned wi
-0001a330: 7468 206e 6f64 6520 3120 6f66 0a20 2020  th node 1 of.   
-0001a340: 2020 2020 2020 7269 6e67 2031 2e0a 2020        ring 1..  
-0001a350: 2020 2020 322e 2043 7265 6174 6520 4e20      2. Create N 
-0001a360: 6e65 7720 7269 6e67 2031 2067 7269 6473  new ring 1 grids
-0001a370: 2061 7420 7374 6174 696f 6e20 616e 6420   at station and 
-0001a380: 7261 6469 7573 206f 6620 7269 6e67 2032  radius of ring 2
-0001a390: 0a20 2020 2020 2020 2020 6772 6964 732c  .         grids,
-0001a3a0: 2062 7574 2061 7420 7468 6520 7361 6d65   but at the same
-0001a3b0: 2061 6e67 756c 6172 206c 6f63 6174 696f   angular locatio
-0001a3c0: 6e20 6173 206f 7269 6769 6e61 6c20 4e2e  n as original N.
-0001a3d0: 0a20 2020 2020 2033 2e20 5242 4532 2074  .      3. RBE2 t
-0001a3e0: 6865 7365 206e 6577 2067 7269 6473 2074  hese new grids t
-0001a3f0: 6f20 7468 6520 4e20 6f72 6967 696e 616c  o the N original
-0001a400: 2067 7269 6473 2e20 5468 6520 6e65 7720   grids. The new 
-0001a410: 6772 6964 730a 2020 2020 2020 2020 2061  grids.         a
-0001a420: 7265 2069 6e64 6570 656e 6465 6e74 2e0a  re independent..
-0001a430: 2020 2020 2020 342e 2057 7269 7465 2052        4. Write R
-0001a440: 5350 4c49 4e45 2063 6172 6473 2075 7369  SPLINE cards usi
-0001a450: 6e67 203a 6675 6e63 3a60 7774 7273 706c  ng :func:`wtrspl
-0001a460: 696e 6560 2e20 5468 6520 6669 7273 740a  ine`. The first.
-0001a470: 2020 2020 2020 2020 2052 5350 4c49 4e45           RSPLINE
-0001a480: 2073 7461 7274 7320 6174 2074 6865 2069   starts at the i
-0001a490: 6e64 6570 656e 6465 6e74 2067 7269 6420  ndependent grid 
-0001a4a0: 286f 6e20 7269 6e67 2031 206f 7220 7269  (on ring 1 or ri
-0001a4b0: 6e67 2032 0a20 2020 2020 2020 2020 6163  ng 2.         ac
-0001a4c0: 636f 7264 696e 6720 746f 2060 696e 6465  cording to `inde
-0001a4d0: 7065 6e64 656e 7460 2920 7769 7468 2074  pendent`) with t
-0001a4e0: 6865 206c 6f77 6573 7420 616e 6775 6c61  he lowest angula
-0001a4f0: 720a 2020 2020 2020 2020 206c 6f63 6174  r.         locat
-0001a500: 696f 6e2e 2054 6865 2061 6e67 756c 6172  ion. The angular
-0001a510: 206c 6f63 6174 696f 6e73 2072 616e 6765   locations range
-0001a520: 2066 726f 6d20 3020 746f 2033 3630 2064   from 0 to 360 d
-0001a530: 6567 7265 6573 2c0a 2020 2020 2020 2020  egrees,.        
-0001a540: 2063 6f75 6e74 6572 2d63 6c6f 636b 7769   counter-clockwi
-0001a550: 7365 2e20 5468 6520 5253 504c 494e 4573  se. The RSPLINEs
-0001a560: 2070 726f 6365 6564 2063 6f75 6e74 6572   proceed counter
-0001a570: 2d63 6c6f 636b 7769 7365 0a20 2020 2020  -clockwise.     
-0001a580: 2020 2020 6172 6f75 6e64 2074 6865 2063      around the c
-0001a590: 6972 636c 652e 0a0a 2020 2020 5365 6520  ircle...    See 
-0001a5a0: 616c 736f 0a20 2020 202d 2d2d 2d2d 2d2d  also.    -------
-0001a5b0: 2d0a 2020 2020 3a66 756e 633a 6077 7472  -.    :func:`wtr
-0001a5c0: 7370 6c69 6e65 600a 0a20 2020 2052 6169  spline`..    Rai
-0001a5d0: 7365 730a 2020 2020 2d2d 2d2d 2d2d 0a20  ses.    ------. 
-0001a5e0: 2020 2056 616c 7565 4572 726f 720a 0a20     ValueError.. 
-0001a5f0: 2020 2020 2020 2057 6865 6e20 7468 6520         When the 
-0001a600: 7065 7270 656e 6469 6375 6c61 7220 6469  perpendicular di
-0001a610: 7265 6374 696f 6e73 206f 6620 6072 3167  rections of `r1g
-0001a620: 7269 6473 6020 616e 6420 6072 3267 7269  rids` and `r2gri
-0001a630: 6473 600a 2020 2020 2020 2020 646f 206e  ds`.        do n
-0001a640: 6f74 206d 6174 6368 2077 6974 6869 6e20  ot match within 
-0001a650: 746f 6c65 7261 6e63 653a 2061 6273 6f6c  tolerance: absol
-0001a660: 7574 6520 7661 6c75 6520 6f66 2074 6865  ute value of the
-0001a670: 2063 6f73 696e 6520 6f66 0a20 2020 2020   cosine of.     
-0001a680: 2020 2074 6865 2061 6e67 6c65 2062 6574     the angle bet
-0001a690: 7765 656e 2074 6865 2074 776f 2070 6572  ween the two per
-0001a6a0: 7065 6e64 6963 756c 6172 2064 6972 6563  pendicular direc
-0001a6b0: 7469 6f6e 7320 6d75 7374 2062 6520 3e0a  tions must be >.
-0001a6c0: 2020 2020 2020 2020 302e 3939 2e0a 0a20          0.99... 
-0001a6d0: 2020 2020 2020 2057 6865 6e20 6120 6072         When a `r
-0001a6e0: 3167 7269 6473 6020 6f72 2060 7232 6772  1grids` or `r2gr
-0001a6f0: 6964 7360 2044 6174 6146 7261 6d65 2064  ids` DataFrame d
-0001a700: 6f65 7320 6e6f 7420 6861 7665 2061 0a20  oes not have a. 
-0001a710: 2020 2020 2020 206d 756c 7469 706c 6520         multiple 
-0001a720: 6f66 2036 2072 6f77 732e 0a0a 2020 2020  of 6 rows...    
-0001a730: 2020 2020 5768 656e 2074 6865 2060 6d61      When the `ma
-0001a740: 6b65 706c 6f74 6020 6f70 7469 6f6e 2074  keplot` option t
-0001a750: 7269 6573 2074 6f20 6164 6420 746f 2061  ries to add to a
-0001a760: 6e20 6178 6573 206f 626a 6563 7420 7468  n axes object th
-0001a770: 6174 0a20 2020 2020 2020 2069 7320 6e6f  at.        is no
-0001a780: 7420 7573 696e 6720 6120 3364 2070 726f  t using a 3d pro
-0001a790: 6a65 6374 696f 6e2e 0a0a 2020 2020 4578  jection...    Ex
-0001a7a0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-0001a7b0: 2d2d 2d0a 2020 2020 4465 6669 6e65 2074  ---.    Define t
-0001a7c0: 776f 2072 696e 6773 206f 6620 6772 6964  wo rings of grid
-0001a7d0: 733a 0a0a 2020 2020 312e 2052 696e 6720  s:..    1. Ring 
-0001a7e0: 3120 7769 6c6c 2062 6520 6174 2073 7461  1 will be at sta
-0001a7f0: 7469 6f6e 2030 2e30 2077 6974 6820 3520  tion 0.0 with 5 
-0001a800: 6e6f 6465 7320 6f6e 2072 696e 6720 6f66  nodes on ring of
-0001a810: 2072 6164 6975 730a 2020 2020 2020 2035   radius.       5
-0001a820: 302e 2049 4473 2077 696c 6c20 6265 2031  0. IDs will be 1
-0001a830: 2074 6f20 352e 0a0a 2020 2020 322e 2052   to 5...    2. R
-0001a840: 696e 6720 3220 7769 6c6c 2062 6520 6174  ing 2 will be at
-0001a850: 2073 7461 7469 6f6e 2031 2e30 2077 6974   station 1.0 wit
-0001a860: 6820 3720 6e6f 6465 7320 6f6e 2072 696e  h 7 nodes on rin
-0001a870: 6720 6f66 2072 6164 6975 730a 2020 2020  g of radius.    
-0001a880: 2020 2034 352e 2049 4473 2077 696c 6c20     45. IDs will 
-0001a890: 6265 2031 3031 2074 6f20 3130 372e 0a0a  be 101 to 107...
-0001a8a0: 2020 2020 466f 7220 6465 6d6f 6e73 7472      For demonstr
-0001a8b0: 6174 696f 6e2c 2072 696e 6720 3120 7769  ation, ring 1 wi
-0001a8c0: 6c6c 2062 6520 6e61 6d65 6420 2753 7061  ll be named 'Spa
-0001a8d0: 6365 6372 6166 7427 2077 6869 6c65 2074  cecraft' while t
-0001a8e0: 6865 0a20 2020 2064 6566 6175 6c74 2077  he.    default w
-0001a8f0: 696c 6c20 6265 2061 6363 6570 7465 6420  ill be accepted 
-0001a900: 666f 7220 7269 6e67 2032 2028 7768 6963  for ring 2 (whic
-0001a910: 6820 6973 2027 5269 6e67 2032 2729 2e0a  h is 'Ring 2')..
-0001a920: 0a20 2020 202e 2e20 706c 6f74 3a3a 0a20  .    .. plot::. 
-0001a930: 2020 2020 2020 203a 636f 6e74 6578 743a         :context:
-0001a940: 2063 6c6f 7365 2d66 6967 730a 0a20 2020   close-figs..   
-0001a950: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-0001a960: 6e75 6d70 7920 6173 206e 700a 2020 2020  numpy as np.    
-0001a970: 2020 2020 3e3e 3e20 696d 706f 7274 206d      >>> import m
-0001a980: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
-0001a990: 2061 7320 706c 740a 2020 2020 2020 2020   as plt.        
-0001a9a0: 3e3e 3e20 6672 6f6d 2070 7979 6574 6920  >>> from pyyeti 
-0001a9b0: 696d 706f 7274 206e 6173 7472 616e 0a20  import nastran. 
-0001a9c0: 2020 2020 2020 203e 3e3e 2074 6865 7461         >>> theta
-0001a9d0: 3120 3d20 6e70 2e61 7261 6e67 6528 302c  1 = np.arange(0,
-0001a9e0: 2033 3539 2c20 3336 302f 3529 2a6e 702e   359, 360/5)*np.
-0001a9f0: 7069 2f31 3830 0a20 2020 2020 2020 203e  pi/180.        >
-0001aa00: 3e3e 2072 6164 3120 3d20 3530 2e0a 2020  >> rad1 = 50..  
-0001aa10: 2020 2020 2020 3e3e 3e20 7374 6131 203d        >>> sta1 =
-0001aa20: 2030 2e0a 2020 2020 2020 2020 3e3e 3e20   0..        >>> 
-0001aa30: 6e31 203d 206c 656e 2874 6865 7461 3129  n1 = len(theta1)
-0001aa40: 0a20 2020 2020 2020 203e 3e3e 2072 696e  .        >>> rin
-0001aa50: 6731 203d 206e 702e 7673 7461 636b 2828  g1 = np.vstack((
-0001aa60: 6e70 2e61 7261 6e67 6528 312c 206e 312b  np.arange(1, n1+
-0001aa70: 3129 2c20 2020 2020 2023 2049 440a 2020  1),      # ID.  
-0001aa80: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
-0001aa90: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-0001aaa0: 312a 6e70 2e6f 6e65 7328 6e31 292c 2020  1*np.ones(n1),  
-0001aab0: 2020 2020 2020 2320 780a 2020 2020 2020        # x.      
-0001aac0: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
-0001aad0: 2020 2020 2020 2020 2072 6164 312a 6e70           rad1*np
-0001aae0: 2e63 6f73 2874 6865 7461 3129 2c20 2020  .cos(theta1),   
-0001aaf0: 2020 2320 790a 2020 2020 2020 2020 2e2e    # y.        ..
-0001ab00: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ab10: 2020 2020 2072 6164 312a 6e70 2e73 696e       rad1*np.sin
-0001ab20: 2874 6865 7461 3129 2929 2e54 2020 2320  (theta1))).T  # 
-0001ab30: 7a0a 2020 2020 2020 2020 3e3e 3e20 2320  z.        >>> # 
-0001ab40: 5072 6f76 6964 6520 6120 6e61 6d65 2066  Provide a name f
-0001ab50: 6f72 2072 696e 6720 313a 0a20 2020 2020  or ring 1:.     
-0001ab60: 2020 203e 3e3e 2072 696e 6731 203d 2028     >>> ring1 = (
-0001ab70: 2753 7061 6365 6372 6166 7427 2c20 7269  'Spacecraft', ri
-0001ab80: 6e67 3129 0a20 2020 2020 2020 203e 3e3e  ng1).        >>>
-0001ab90: 2074 6865 7461 3220 3d20 6e70 2e61 7261   theta2 = np.ara
-0001aba0: 6e67 6528 3130 2c20 3335 392c 2033 3630  nge(10, 359, 360
-0001abb0: 2f37 292a 6e70 2e70 692f 3138 300a 2020  /7)*np.pi/180.  
-0001abc0: 2020 2020 2020 3e3e 3e20 7261 6432 203d        >>> rad2 =
-0001abd0: 2034 352e 0a20 2020 2020 2020 203e 3e3e   45..        >>>
-0001abe0: 2073 7461 3220 3d20 312e 0a20 2020 2020   sta2 = 1..     
-0001abf0: 2020 203e 3e3e 206e 3220 3d20 6c65 6e28     >>> n2 = len(
-0001ac00: 7468 6574 6132 290a 2020 2020 2020 2020  theta2).        
-0001ac10: 3e3e 3e20 7269 6e67 3220 3d20 6e70 2e76  >>> ring2 = np.v
-0001ac20: 7374 6163 6b28 286e 702e 6172 616e 6765  stack((np.arange
-0001ac30: 2831 2c20 6e32 2b31 292b 3130 302c 2020  (1, n2+1)+100,  
-0001ac40: 2320 4944 0a20 2020 2020 2020 202e 2e2e  # ID.        ...
-0001ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac60: 2020 2020 7374 6132 2a6e 702e 6f6e 6573      sta2*np.ones
-0001ac70: 286e 3229 2c20 2020 2020 2020 2023 2078  (n2),        # x
-0001ac80: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aca0: 7261 6432 2a6e 702e 636f 7328 7468 6574  rad2*np.cos(thet
-0001acb0: 6132 292c 2020 2020 2023 2079 0a20 2020  a2),     # y.   
-0001acc0: 2020 2020 202e 2e2e 2020 2020 2020 2020       ...        
-0001acd0: 2020 2020 2020 2020 2020 2020 7261 6432              rad2
-0001ace0: 2a6e 702e 7369 6e28 7468 6574 6132 2929  *np.sin(theta2))
-0001acf0: 292e 5420 2023 207a 0a20 2020 2020 2020  ).T  # z.       
-0001ad00: 203e 3e3e 2066 6967 203d 2070 6c74 2e66   >>> fig = plt.f
-0001ad10: 6967 7572 6528 2745 7861 6d70 6c65 272c  igure('Example',
-0001ad20: 2066 6967 7369 7a65 3d28 382c 2036 2929   figsize=(8, 6))
-0001ad30: 0a20 2020 2020 2020 203e 3e3e 2066 6967  .        >>> fig
-0001ad40: 2e63 6c66 2829 0a20 2020 2020 2020 203e  .clf().        >
-0001ad50: 3e3e 2061 7820 3d20 6669 672e 6164 645f  >> ax = fig.add_
-0001ad60: 7375 6270 6c6f 7428 312c 2031 2c20 312c  subplot(1, 1, 1,
-0001ad70: 2070 726f 6a65 6374 696f 6e3d 2733 6427   projection='3d'
-0001ad80: 290a 2020 2020 2020 2020 3e3e 3e20 6e61  ).        >>> na
-0001ad90: 7374 7261 6e2e 7774 7273 706c 696e 655f  stran.wtrspline_
-0001ada0: 7269 6e67 7328 0a20 2020 2020 2020 202e  rings(.        .
-0001adb0: 2e2e 2020 2020 2031 2c20 7269 6e67 312c  ..     1, ring1,
-0001adc0: 2072 696e 6732 2c20 3130 3031 2c20 3230   ring2, 1001, 20
-0001add0: 3031 2c0a 2020 2020 2020 2020 2e2e 2e20  01,.        ... 
-0001ade0: 2020 2020 6d61 6b65 706c 6f74 3d61 7829      makeplot=ax)
-0001adf0: 2020 2023 2064 6f63 7465 7374 3a20 2b53     # doctest: +S
-0001ae00: 4b49 500a 2020 2020 2020 2020 240a 2020  KIP.        $.  
-0001ae10: 2020 2020 2020 2420 4669 7420 6f66 2053        $ Fit of S
-0001ae20: 7061 6365 6372 6166 7420 6772 6964 733a  pacecraft grids:
-0001ae30: 0a20 2020 2020 2020 2024 2020 2020 2043  .        $     C
-0001ae40: 656e 7465 723a 205b 302e 3030 302c 2030  enter: [0.000, 0
-0001ae50: 2e30 3030 2c20 302e 3030 305d 2028 696e  .000, 0.000] (in
-0001ae60: 2062 6173 6963 290a 2020 2020 2020 2020   basic).        
-0001ae70: 2420 2020 2020 5261 6469 7573 3a20 3530  $     Radius: 50
-0001ae80: 2e30 0a20 2020 2020 2020 2024 0a20 2020  .0.        $.   
-0001ae90: 2020 2020 2024 2046 6974 206f 6620 5269       $ Fit of Ri
-0001aea0: 6e67 2032 2067 7269 6473 3a0a 2020 2020  ng 2 grids:.    
-0001aeb0: 2020 2020 2420 2020 2020 4365 6e74 6572      $     Center
-0001aec0: 3a20 5b31 2e30 3030 2c20 2d31 2e37 3736  : [1.000, -1.776
-0001aed0: 652d 3135 2c20 2d33 2e35 3533 652d 3135  e-15, -3.553e-15
-0001aee0: 5d20 2869 6e20 6261 7369 6329 0a20 2020  ] (in basic).   
-0001aef0: 2020 2020 2024 2020 2020 2052 6164 6975       $     Radiu
-0001af00: 733a 2034 352e 300a 2020 2020 2020 2020  s: 45.0.        
-0001af10: 240a 2020 2020 2020 2020 2420 4f72 6967  $.        $ Orig
-0001af20: 696e 206f 6620 6c6f 6361 6c20 434f 5244  in of local CORD
-0001af30: 3252 2031 3030 3130 2069 7320 6174 2063  2R 10010 is at c
-0001af40: 656e 7465 7220 6f66 2053 7061 6365 6372  enter of Spacecr
-0001af50: 6166 743b 207a 2069 730a 2020 2020 2020  aft; z is.      
-0001af60: 2020 2420 7065 7270 656e 6469 6375 6c61    $ perpendicula
-0001af70: 7220 746f 2070 6c61 6e65 206f 6620 6369  r to plane of ci
-0001af80: 7263 6c65 2c20 616e 6420 7820 6973 2061  rcle, and x is a
-0001af90: 6c69 676e 6564 2077 6974 6820 6e6f 6465  ligned with node
-0001afa0: 2031 2028 616e 640a 2020 2020 2020 2020   1 (and.        
-0001afb0: 2420 6e65 7720 6e6f 6465 2031 3030 3129  $ new node 1001)
-0001afc0: 2e0a 2020 2020 2020 2020 240a 2020 2020  ..        $.    
-0001afd0: 2020 2020 2420 436f 6f72 6469 6e61 7465      $ Coordinate
-0001afe0: 2031 3030 3130 3a0a 2020 2020 2020 2020   10010:.        
-0001aff0: 434f 5244 3252 2a20 2020 2020 2020 2020  CORD2R*         
-0001b000: 2020 2031 3030 3130 2020 2020 2020 2020     10010        
-0001b010: 2020 2020 2020 2030 2020 302e 3030 3030         0  0.0000
-0001b020: 3030 3030 652b 3030 2020 302e 3030 3030  0000e+00  0.0000
-0001b030: 3030 3030 652b 3030 2a0a 2020 2020 2020  0000e+00*.      
-0001b040: 2020 2a20 2020 2020 2020 2020 302e 3030    *         0.00
-0001b050: 3030 3030 3030 652b 3030 2020 312e 3030  000000e+00  1.00
-0001b060: 3030 3030 3030 652b 3030 2020 302e 3030  000000e+00  0.00
-0001b070: 3030 3030 3030 652b 3030 2020 302e 3030  000000e+00  0.00
-0001b080: 3030 3030 3030 652b 3030 2a0a 2020 2020  000000e+00*.    
-0001b090: 2020 2020 2a20 2020 2020 2020 2020 302e      *         0.
-0001b0a0: 3030 3030 3030 3030 652b 3030 2020 312e  00000000e+00  1.
-0001b0b0: 3030 3030 3030 3030 652b 3030 2020 302e  00000000e+00  0.
-0001b0c0: 3030 3030 3030 3030 652b 3030 0a20 2020  00000000e+00.   
-0001b0d0: 2020 2020 2024 0a20 2020 2020 2020 2024       $.        $
-0001b0e0: 2047 7269 6473 2074 6f20 5242 4532 2074   Grids to RBE2 t
-0001b0f0: 6f20 7468 6520 5370 6163 6563 7261 6674  o the Spacecraft
-0001b100: 2067 7269 6473 2e20 5468 6573 6520 6772   grids. These gr
-0001b110: 6964 7320 6c69 6e65 2075 7020 7769 7468  ids line up with
-0001b120: 2074 6865 0a20 2020 2020 2020 2024 2052   the.        $ R
-0001b130: 696e 6720 3220 6369 7263 6c65 2073 6f20  ing 2 circle so 
-0001b140: 7468 6174 2074 6865 2052 5350 4c49 4e45  that the RSPLINE
-0001b150: 2028 7768 6963 6820 7469 6573 2074 6f67   (which ties tog
-0001b160: 6574 6865 7220 7468 6573 6520 6e65 7720  ether these new 
-0001b170: 6772 6964 730a 2020 2020 2020 2020 2420  grids.        $ 
-0001b180: 616e 6420 7468 6520 5269 6e67 2032 2067  and the Ring 2 g
-0001b190: 7269 6473 2920 7769 6c6c 2062 6520 736d  rids) will be sm
-0001b1a0: 6f6f 7468 2e0a 2020 2020 2020 2020 240a  ooth..        $.
-0001b1b0: 2020 2020 2020 2020 4752 4944 2a20 2020          GRID*   
-0001b1c0: 2020 2020 2020 2020 2020 2020 3130 3031              1001
-0001b1d0: 2020 2020 2020 2020 2020 2031 3030 3130             10010
-0001b1e0: 2020 2020 2034 352e 3030 3030 3030 3030       45.00000000
-0001b1f0: 2020 2020 202d 302e 3030 3030 3030 3030       -0.00000000
-0001b200: 0a20 2020 2020 2020 202a 2020 2020 2020  .        *      
-0001b210: 2020 2020 2020 2031 2e30 3030 3030 3030         1.0000000
-0001b220: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0001b230: 300a 2020 2020 2020 2020 4752 4944 2a20  0.        GRID* 
-0001b240: 2020 2020 2020 2020 2020 2020 2020 3130                10
-0001b250: 3032 2020 2020 2020 2020 2020 2031 3030  02           100
-0001b260: 3130 2020 2020 2031 332e 3930 3537 3634  10     13.905764
-0001b270: 3735 2020 2020 2034 322e 3739 3735 3433  75     42.797543
-0001b280: 3233 0a20 2020 2020 2020 202a 2020 2020  23.        *    
-0001b290: 2020 2020 2020 2020 2031 2e30 3030 3030           1.00000
-0001b2a0: 3030 3020 2020 2020 2020 2020 2020 2020  000             
-0001b2b0: 2020 300a 2020 2020 2020 2020 4752 4944    0.        GRID
-0001b2c0: 2a20 2020 2020 2020 2020 2020 2020 2020  *               
-0001b2d0: 3130 3033 2020 2020 2020 2020 2020 2031  1003           1
-0001b2e0: 3030 3130 2020 2020 2d33 362e 3430 3537  0010    -36.4057
-0001b2f0: 3634 3735 2020 2020 2032 362e 3435 3033  6475     26.4503
-0001b300: 3336 3335 0a20 2020 2020 2020 202a 2020  3635.        *  
-0001b310: 2020 2020 2020 2020 2020 2031 2e30 3030             1.000
-0001b320: 3030 3030 3020 2020 2020 2020 2020 2020  00000           
-0001b330: 2020 2020 300a 2020 2020 2020 2020 4752      0.        GR
-0001b340: 4944 2a20 2020 2020 2020 2020 2020 2020  ID*             
-0001b350: 2020 3130 3034 2020 2020 2020 2020 2020    1004          
-0001b360: 2031 3030 3130 2020 2020 2d33 362e 3430   10010    -36.40
-0001b370: 3537 3634 3735 2020 2020 2d32 362e 3435  576475    -26.45
-0001b380: 3033 3336 3335 0a20 2020 2020 2020 202a  033635.        *
-0001b390: 2020 2020 2020 2020 2020 2020 2031 2e30               1.0
-0001b3a0: 3030 3030 3030 3020 2020 2020 2020 2020  0000000         
-0001b3b0: 2020 2020 2020 300a 2020 2020 2020 2020        0.        
-0001b3c0: 4752 4944 2a20 2020 2020 2020 2020 2020  GRID*           
-0001b3d0: 2020 2020 3130 3035 2020 2020 2020 2020      1005        
-0001b3e0: 2020 2031 3030 3130 2020 2020 2031 332e     10010     13.
-0001b3f0: 3930 3537 3634 3735 2020 2020 2d34 322e  90576475    -42.
-0001b400: 3739 3735 3433 3233 0a20 2020 2020 2020  79754323.       
-0001b410: 202a 2020 2020 2020 2020 2020 2020 2031   *             1
-0001b420: 2e30 3030 3030 3030 3020 2020 2020 2020  .00000000       
-0001b430: 2020 2020 2020 2020 300a 2020 2020 2020          0.      
-0001b440: 2020 240a 2020 2020 2020 2020 2420 5242    $.        $ RB
-0001b450: 4532 2074 6865 2053 7061 6365 6372 6166  E2 the Spacecraf
-0001b460: 7420 6e6f 6465 7320 746f 206e 6577 206e  t nodes to new n
-0001b470: 6f64 6573 2063 7265 6174 6564 2061 626f  odes created abo
-0001b480: 7665 2028 7468 6520 6e65 7720 6e6f 6465  ve (the new node
-0001b490: 730a 2020 2020 2020 2020 2420 6172 6520  s.        $ are 
-0001b4a0: 696e 6465 7065 6e64 656e 7429 3a0a 2020  independent):.  
-0001b4b0: 2020 2020 2020 240a 2020 2020 2020 2020        $.        
-0001b4c0: 5242 4532 2c31 3030 312c 3130 3031 2c31  RBE2,1001,1001,1
-0001b4d0: 3233 3435 362c 310a 2020 2020 2020 2020  23456,1.        
-0001b4e0: 5242 4532 2c31 3030 322c 3130 3032 2c31  RBE2,1002,1002,1
-0001b4f0: 3233 3435 362c 320a 2020 2020 2020 2020  23456,2.        
-0001b500: 5242 4532 2c31 3030 332c 3130 3033 2c31  RBE2,1003,1003,1
-0001b510: 3233 3435 362c 330a 2020 2020 2020 2020  23456,3.        
-0001b520: 5242 4532 2c31 3030 342c 3130 3034 2c31  RBE2,1004,1004,1
-0001b530: 3233 3435 362c 340a 2020 2020 2020 2020  23456,4.        
-0001b540: 5242 4532 2c31 3030 352c 3130 3035 2c31  RBE2,1005,1005,1
-0001b550: 3233 3435 362c 350a 2020 2020 2020 2020  23456,5.        
-0001b560: 240a 2020 2020 2020 2020 2420 5253 504c  $.        $ RSPL
-0001b570: 494e 4520 7468 6520 5269 6e67 2032 206e  INE the Ring 2 n
-0001b580: 6f64 6573 2074 6f20 7468 6520 6e65 7720  odes to the new 
-0001b590: 6e6f 6465 7320 6372 6561 7465 6420 6162  nodes created ab
-0001b5a0: 6f76 652c 2077 6974 6820 7468 6520 6e65  ove, with the ne
-0001b5b0: 770a 2020 2020 2020 2020 2420 6e6f 6465  w.        $ node
-0001b5c0: 7320 6265 696e 6720 696e 6465 7065 6e64  s being independ
-0001b5d0: 656e 742e 0a20 2020 2020 2020 2024 0a20  ent..        $. 
-0001b5e0: 2020 2020 2020 2052 5350 4c49 4e45 2020         RSPLINE  
-0001b5f0: 2020 2032 3030 3120 2020 2020 302e 3120     2001     0.1 
-0001b600: 2020 2031 3030 3120 2020 2020 3130 3120     1001     101 
-0001b610: 2031 3233 3435 3620 2020 2020 3130 3220   123456     102 
-0001b620: 2031 3233 3435 3620 2020 2031 3030 320a   123456    1002.
-0001b630: 2020 2020 2020 2020 5253 504c 494e 4520          RSPLINE 
-0001b640: 2020 2020 3230 3032 2020 2020 2030 2e31      2002     0.1
-0001b650: 2020 2020 3130 3032 2020 2020 2031 3033      1002     103
-0001b660: 2020 3132 3334 3536 2020 2020 3130 3033    123456    1003
-0001b670: 0a20 2020 2020 2020 2052 5350 4c49 4e45  .        RSPLINE
-0001b680: 2020 2020 2032 3030 3320 2020 2020 302e       2003     0.
-0001b690: 3120 2020 2031 3030 3320 2020 2020 3130  1    1003     10
-0001b6a0: 3420 2031 3233 3435 3620 2020 2020 3130  4  123456     10
-0001b6b0: 3520 2031 3233 3435 3620 2020 2031 3030  5  123456    100
-0001b6c0: 340a 2020 2020 2020 2020 5253 504c 494e  4.        RSPLIN
-0001b6d0: 4520 2020 2020 3230 3034 2020 2020 2030  E     2004     0
-0001b6e0: 2e31 2020 2020 3130 3034 2020 2020 2031  .1    1004     1
-0001b6f0: 3036 2020 3132 3334 3536 2020 2020 3130  06  123456    10
-0001b700: 3035 0a20 2020 2020 2020 2052 5350 4c49  05.        RSPLI
-0001b710: 4e45 2020 2020 2032 3030 3520 2020 2020  NE     2005     
-0001b720: 302e 3120 2020 2031 3030 3520 2020 2020  0.1    1005     
-0001b730: 3130 3720 2031 3233 3435 3620 2020 2031  107  123456    1
-0001b740: 3030 310a 2020 2020 2222 220a 0a20 2020  001.    """..   
-0001b750: 2064 6566 205f 6368 6563 6b5f 6772 6964   def _check_grid
-0001b760: 7328 6772 6964 732c 206e 616d 6529 3a0a  s(grids, name):.
-0001b770: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0001b780: 7461 6e63 6528 6772 6964 732c 2074 7570  tance(grids, tup
-0001b790: 6c65 2920 616e 6420 6c65 6e28 6772 6964  le) and len(grid
-0001b7a0: 7329 203d 3d20 323a 0a20 2020 2020 2020  s) == 2:.       
-0001b7b0: 2020 2020 2072 6574 7572 6e20 6772 6964       return grid
-0001b7c0: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-0001b7d0: 206e 616d 652c 2067 7269 6473 0a0a 2020   name, grids..  
-0001b7e0: 2020 6465 6620 5f64 6573 7061 6365 2873    def _despace(s
-0001b7f0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0001b800: 6e20 2822 222e 6a6f 696e 2873 2e73 706c  n ("".join(s.spl
-0001b810: 6974 2829 2929 2e6c 6f77 6572 2829 0a0a  it())).lower()..
-0001b820: 2020 2020 7231 6e61 6d65 2c20 7231 6772      r1name, r1gr
-0001b830: 6964 7320 3d20 5f63 6865 636b 5f67 7269  ids = _check_gri
-0001b840: 6473 2872 3167 7269 6473 2c20 2252 696e  ds(r1grids, "Rin
-0001b850: 6720 3122 290a 2020 2020 7232 6e61 6d65  g 1").    r2name
-0001b860: 2c20 7232 6772 6964 7320 3d20 5f63 6865  , r2grids = _che
-0001b870: 636b 5f67 7269 6473 2872 3267 7269 6473  ck_grids(r2grids
-0001b880: 2c20 2252 696e 6720 3222 290a 0a20 2020  , "Ring 2")..   
-0001b890: 2023 2065 6e73 7572 6520 7468 6174 2069   # ensure that i
-0001b8a0: 6e64 6570 656e 6465 6e74 2069 7320 6569  ndependent is ei
-0001b8b0: 7468 6572 2027 7269 6e67 3127 206f 7220  ther 'ring1' or 
-0001b8c0: 2772 696e 6732 273a 0a20 2020 2069 6e64  'ring2':.    ind
-0001b8d0: 6570 656e 6465 6e74 203d 205f 6465 7370  ependent = _desp
-0001b8e0: 6163 6528 696e 6465 7065 6e64 656e 7429  ace(independent)
-0001b8f0: 0a20 2020 2069 6620 696e 6465 7065 6e64  .    if independ
-0001b900: 656e 7420 3d3d 205f 6465 7370 6163 6528  ent == _despace(
-0001b910: 7231 6e61 6d65 293a 0a20 2020 2020 2020  r1name):.       
-0001b920: 2069 6e64 6570 656e 6465 6e74 203d 2022   independent = "
-0001b930: 7269 6e67 3122 0a20 2020 2065 6c69 6620  ring1".    elif 
-0001b940: 696e 6465 7065 6e64 656e 7420 3d3d 205f  independent == _
-0001b950: 6465 7370 6163 6528 7232 6e61 6d65 293a  despace(r2name):
-0001b960: 0a20 2020 2020 2020 2069 6e64 6570 656e  .        indepen
-0001b970: 6465 6e74 203d 2022 7269 6e67 3222 0a20  dent = "ring2". 
-0001b980: 2020 2069 6620 696e 6465 7065 6e64 656e     if independen
-0001b990: 7420 6e6f 7420 696e 2028 2272 696e 6731  t not in ("ring1
-0001b9a0: 222c 2022 7269 6e67 3222 293a 0a20 2020  ", "ring2"):.   
-0001b9b0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0001b9c0: 4572 726f 7228 2269 6e76 616c 6964 2060  Error("invalid `
-0001b9d0: 696e 6465 7065 6e64 656e 7460 206f 7074  independent` opt
-0001b9e0: 696f 6e22 290a 0a20 2020 2069 6620 7262  ion")..    if rb
-0001b9f0: 6532 5f69 6430 2069 7320 4e6f 6e65 3a0a  e2_id0 is None:.
-0001ba00: 2020 2020 2020 2020 7262 6532 5f69 6430          rbe2_id0
-0001ba10: 203d 206e 6f64 655f 6964 300a 2020 2020   = node_id0.    
-0001ba20: 6966 2063 6f72 645f 6964 2069 7320 4e6f  if cord_id is No
-0001ba30: 6e65 3a0a 2020 2020 2020 2020 636f 7264  ne:.        cord
-0001ba40: 5f69 6420 3d20 6e6f 6465 5f69 6430 202a  _id = node_id0 *
-0001ba50: 2031 300a 0a20 2020 206e 616d 6573 203d   10..    names =
-0001ba60: 2028 7231 6e61 6d65 2c20 7232 6e61 6d65   (r1name, r2name
-0001ba70: 290a 2020 2020 4944 7320 3d20 5b5d 0a20  ).    IDs = []. 
-0001ba80: 2020 2078 797a 203d 205b 5d0a 2020 2020     xyz = [].    
-0001ba90: 666f 7220 7269 6e67 2c20 6e61 6d65 2069  for ring, name i
-0001baa0: 6e20 2828 7231 6772 6964 732c 2022 7231  n ((r1grids, "r1
-0001bab0: 6772 6964 7322 292c 2028 7232 6772 6964  grids"), (r2grid
-0001bac0: 732c 2022 7232 6772 6964 7322 2929 3a0a  s, "r2grids")):.
-0001bad0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0001bae0: 7461 6e63 6528 7269 6e67 2c20 7064 2e44  tance(ring, pd.D
-0001baf0: 6174 6146 7261 6d65 293a 0a20 2020 2020  ataFrame):.     
-0001bb00: 2020 2020 2020 2072 203d 2072 696e 672e         r = ring.
-0001bb10: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
-0001bb20: 2020 2020 2069 6620 2872 202f 2f20 3629       if (r // 6)
-0001bb30: 202a 2036 2021 3d20 723a 0a20 2020 2020   * 6 != r:.     
-0001bb40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0001bb50: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-0001bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb70: 2066 226e 756d 6265 7220 6f66 2072 6f77   f"number of row
-0001bb80: 7320 607b 6e61 6d65 7d60 2069 7320 6e6f  s `{name}` is no
-0001bb90: 7420 2220 226d 756c 7469 706c 6520 6f66  t " "multiple of
-0001bba0: 2036 2066 6f72 2055 5345 5420 696e 7075   6 for USET inpu
-0001bbb0: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
-0001bbc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001bbd0: 2049 4473 2e61 7070 656e 6428 7269 6e67   IDs.append(ring
-0001bbe0: 2e69 6e64 6578 2e67 6574 5f6c 6576 656c  .index.get_level
-0001bbf0: 5f76 616c 7565 7328 2269 6422 295b 3a3a  _values("id")[::
-0001bc00: 365d 290a 2020 2020 2020 2020 2020 2020  6]).            
-0001bc10: 7879 7a2e 6170 7065 6e64 2872 696e 672e  xyz.append(ring.
-0001bc20: 696c 6f63 5b3a 3a36 2c20 313a 5d2e 7661  iloc[::6, 1:].va
-0001bc30: 6c75 6573 290a 2020 2020 2020 2020 656c  lues).        el
-0001bc40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001bc50: 7269 6e67 203d 206e 702e 6174 6c65 6173  ring = np.atleas
-0001bc60: 745f 3264 2872 696e 6729 0a20 2020 2020  t_2d(ring).     
-0001bc70: 2020 2020 2020 2049 4473 2e61 7070 656e         IDs.appen
-0001bc80: 6428 7269 6e67 5b3a 2c20 305d 2e61 7374  d(ring[:, 0].ast
-0001bc90: 7970 6528 6e70 2e69 6e74 3634 2929 0a20  ype(np.int64)). 
-0001bca0: 2020 2020 2020 2020 2020 2078 797a 2e61             xyz.a
-0001bcb0: 7070 656e 6428 7269 6e67 5b3a 2c20 313a  ppend(ring[:, 1:
-0001bcc0: 5d29 0a0a 2020 2020 2320 6669 7420 626f  ])..    # fit bo
-0001bcd0: 7468 2063 6972 636c 6573 3a0a 2020 2020  th circles:.    
-0001bce0: 6369 7263 5f70 6172 6d73 203d 205b 7974  circ_parms = [yt
-0001bcf0: 6f6f 6c73 2e66 6974 5f63 6972 636c 655f  ools.fit_circle_
-0001bd00: 3364 2878 797a 5b69 5d2e 5429 2066 6f72  3d(xyz[i].T) for
-0001bd10: 2069 2069 6e20 2830 2c20 3129 5d0a 0a20   i in (0, 1)].. 
-0001bd20: 2020 2023 207a 2061 7865 7320 6265 7474     # z axes bett
-0001bd30: 6572 2062 6520 616c 6967 6e65 643a 0a20  er be aligned:. 
-0001bd40: 2020 205f 6368 6563 6b5f 7a5f 616c 6967     _check_z_alig
-0001bd50: 6e6d 656e 7428 6369 7263 5f70 6172 6d73  nment(circ_parms
-0001bd60: 2c20 302e 3939 290a 0a20 2020 2023 2075  , 0.99)..    # u
-0001bd70: 7365 2031 7374 2062 6173 6963 326c 6f63  se 1st basic2loc
-0001bd80: 616c 2074 7261 6e73 666f 726d 206f 6e20  al transform on 
-0001bd90: 7365 636f 6e64 2073 6574 206f 6620 6461  second set of da
-0001bda0: 7461 2074 6f20 6765 7420 616c 6c0a 2020  ta to get all.  
-0001bdb0: 2020 2320 636f 6f72 6469 6e61 7465 7320    # coordinates 
-0001bdc0: 696e 2073 616d 6520 6c6f 6361 6c20 7379  in same local sy
-0001bdd0: 7374 656d 3a0a 2020 2020 6261 7369 6332  stem:.    basic2
-0001bde0: 6c6f 6361 6c20 3d20 6369 7263 5f70 6172  local = circ_par
-0001bdf0: 6d73 5b30 5d2e 6261 7369 6332 6c6f 6361  ms[0].basic2loca
-0001be00: 6c0a 2020 2020 6365 6e74 6572 203d 2063  l.    center = c
-0001be10: 6972 635f 7061 726d 735b 305d 2e63 656e  irc_parms[0].cen
-0001be20: 7465 720a 2020 2020 6369 7263 5f70 6172  ter.    circ_par
-0001be30: 6d73 5b31 5d2e 6c6f 6361 6c20 3d20 6261  ms[1].local = ba
-0001be40: 7369 6332 6c6f 6361 6c20 4020 2878 797a  sic2local @ (xyz
-0001be50: 5b31 5d20 2d20 6365 6e74 6572 292e 540a  [1] - center).T.
-0001be60: 0a20 2020 2023 2074 6865 2063 656e 7465  .    # the cente
-0001be70: 7220 706f 696e 7420 7769 6c6c 206f 6674  r point will oft
-0001be80: 656e 2068 6176 6520 6e65 6172 2d7a 6572  en have near-zer
-0001be90: 6f73 2062 7574 2062 6520 6e75 6d65 7269  os but be numeri
-0001bea0: 6361 6c6c 790a 2020 2020 2320 6f66 6620  cally.    # off 
-0001beb0: 2e2e 2e20 6368 6563 6b20 666f 7220 7468  ... check for th
-0001bec0: 6973 2061 6e64 2061 646a 7573 7420 6966  is and adjust if
-0001bed0: 2074 6861 7427 7320 7468 6520 6361 7365   that's the case
-0001bee0: 3a0a 2020 2020 7261 6469 7573 203d 2063  :.    radius = c
-0001bef0: 6972 635f 7061 726d 735b 305d 2e72 6164  irc_parms[0].rad
-0001bf00: 6975 730a 2020 2020 666f 7220 692c 2076  ius.    for i, v
-0001bf10: 616c 7565 2069 6e20 656e 756d 6572 6174  alue in enumerat
-0001bf20: 6528 6365 6e74 6572 293a 0a20 2020 2020  e(center):.     
-0001bf30: 2020 2069 6620 6162 7328 7661 6c75 6529     if abs(value)
-0001bf40: 203c 2031 652d 3720 2a20 7261 6469 7573   < 1e-7 * radius
-0001bf50: 3a0a 2020 2020 2020 2020 2020 2020 6365  :.            ce
-0001bf60: 6e74 6572 5b69 5d20 3d20 302e 300a 0a20  nter[i] = 0.0.. 
-0001bf70: 2020 2040 6775 6974 6f6f 6c73 2e77 7269     @guitools.wri
-0001bf80: 7465 5f74 6578 745f 6669 6c65 0a20 2020  te_text_file.   
-0001bf90: 2064 6566 205f 7772 6974 655f 6669 6c65   def _write_file
-0001bfa0: 2866 293a 0a20 2020 2020 2020 2023 2077  (f):.        # w
-0001bfb0: 7269 7465 2063 6972 636c 6520 696e 666f  rite circle info
-0001bfc0: 2066 6f72 2072 6566 6572 656e 6365 3a0a   for reference:.
-0001bfd0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0001bfe0: 2072 616e 6765 2832 293a 0a20 2020 2020   range(2):.     
-0001bff0: 2020 2020 2020 2063 7472 203d 2063 6972         ctr = cir
-0001c000: 635f 7061 726d 735b 695d 2e63 656e 7465  c_parms[i].cente
-0001c010: 720a 2020 2020 2020 2020 2020 2020 6374  r.            ct
-0001c020: 725f 7374 7269 6e67 203d 2066 225b 7b63  r_string = f"[{c
-0001c030: 7472 5b30 5d3a 232e 3467 7d2c 207b 6374  tr[0]:#.4g}, {ct
-0001c040: 725b 315d 3a23 2e34 677d 2c20 7b63 7472  r[1]:#.4g}, {ctr
-0001c050: 5b32 5d3a 232e 3467 7d5d 220a 2020 2020  [2]:#.4g}]".    
-0001c060: 2020 2020 2020 2020 636f 6d6d 656e 7420          comment 
-0001c070: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001c080: 2020 2020 2224 5c6e 220a 2020 2020 2020      "$\n".      
-0001c090: 2020 2020 2020 2020 2020 6622 2420 4669            f"$ Fi
-0001c0a0: 7420 6f66 207b 6e61 6d65 735b 695d 7d20  t of {names[i]} 
-0001c0b0: 6772 6964 733a 5c6e 220a 2020 2020 2020  grids:\n".      
-0001c0c0: 2020 2020 2020 2020 2020 6622 2420 2020            f"$   
-0001c0d0: 2020 4365 6e74 6572 3a20 7b63 7472 5f73    Center: {ctr_s
-0001c0e0: 7472 696e 677d 2028 696e 2062 6173 6963  tring} (in basic
-0001c0f0: 295c 6e22 0a20 2020 2020 2020 2020 2020  )\n".           
-0001c100: 2020 2020 2066 2224 2020 2020 2052 6164       f"$     Rad
-0001c110: 6975 733a 207b 6369 7263 5f70 6172 6d73  ius: {circ_parms
-0001c120: 5b69 5d2e 7261 6469 7573 7d5c 6e22 0a20  [i].radius}\n". 
-0001c130: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001c140: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-0001c150: 2863 6f6d 6d65 6e74 290a 0a20 2020 2020  (comment)..     
-0001c160: 2020 2023 2077 7269 7465 206c 6f63 616c     # write local
-0001c170: 2063 6f6f 7264 696e 6174 6520 7379 7374   coordinate syst
-0001c180: 656d 2074 6f20 6669 6c65 3a0a 2020 2020  em to file:.    
-0001c190: 2020 2020 5f77 745f 6369 7263 6c65 315f      _wt_circle1_
-0001c1a0: 636f 6f72 6428 662c 2063 6f72 645f 6964  coord(f, cord_id
-0001c1b0: 2c20 6365 6e74 6572 2c20 6261 7369 6332  , center, basic2
-0001c1c0: 6c6f 6361 6c2c 2049 4473 5b30 5d5b 305d  local, IDs[0][0]
-0001c1d0: 2c20 6e6f 6465 5f69 6430 2c20 6e61 6d65  , node_id0, name
-0001c1e0: 7329 0a0a 2020 2020 2020 2020 2320 6372  s)..        # cr
-0001c1f0: 6561 7465 206e 6577 206e 6f64 6573 2074  eate new nodes t
-0001c200: 6861 7420 7769 6c6c 2062 6520 5242 4532  hat will be RBE2
-0001c210: 2764 2074 6f20 7269 6e67 2031 206e 6f64  'd to ring 1 nod
-0001c220: 6573 2c20 6275 740a 2020 2020 2020 2020  es, but.        
-0001c230: 2320 6c6f 6361 7465 6420 6f6e 2072 696e  # located on rin
-0001c240: 6720 3220 6369 7263 6c65 0a20 2020 2020  g 2 circle.     
-0001c250: 2020 2023 202d 2074 6865 7365 206e 6f64     # - these nod
-0001c260: 6573 2077 696c 6c20 6265 2064 6566 696e  es will be defin
-0001c270: 6564 2069 6e20 7468 6520 6c6f 6361 6c20  ed in the local 
-0001c280: 7379 7374 656d 2062 7574 206f 7574 7075  system but outpu
-0001c290: 740a 2020 2020 2020 2020 2320 2020 696e  t.        #   in
-0001c2a0: 2062 6173 6963 0a20 2020 2020 2020 206e   basic.        n
-0001c2b0: 6577 7074 732c 206e 6577 6964 7320 3d20  ewpts, newids = 
-0001c2c0: 5f77 7467 7269 6473 5f72 6265 3273 280a  _wtgrids_rbe2s(.
-0001c2d0: 2020 2020 2020 2020 2020 2020 662c 0a20              f,. 
-0001c2e0: 2020 2020 2020 2020 2020 2063 6972 635f             circ_
-0001c2f0: 7061 726d 732c 0a20 2020 2020 2020 2020  parms,.         
-0001c300: 2020 2063 656e 7465 722c 0a20 2020 2020     center,.     
-0001c310: 2020 2020 2020 2062 6173 6963 326c 6f63         basic2loc
-0001c320: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-0001c330: 636f 7264 5f69 642c 0a20 2020 2020 2020  cord_id,.       
-0001c340: 2020 2020 206e 6f64 655f 6964 302c 0a20       node_id0,. 
-0001c350: 2020 2020 2020 2020 2020 2072 6265 325f             rbe2_
-0001c360: 6964 302c 0a20 2020 2020 2020 2020 2020  id0,.           
-0001c370: 2049 4473 5b30 5d2c 0a20 2020 2020 2020   IDs[0],.       
-0001c380: 2020 2020 206e 616d 6573 2c0a 2020 2020       names,.    
-0001c390: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0001c3a0: 2072 7370 6c69 6e65 2077 696c 6c20 7469   rspline will ti
-0001c3b0: 6520 7468 6520 276e 6577 7074 7327 2061  e the 'newpts' a
-0001c3c0: 6e64 2074 6865 2072 696e 6720 3220 6e6f  nd the ring 2 no
-0001c3d0: 6465 7320 746f 6765 7468 6572 3a0a 2020  des together:.  
-0001c3e0: 2020 2020 2020 7273 706c 696e 655f 6e6f        rspline_no
-0001c3f0: 6465 7320 3d20 5f73 6f72 745f 6e5f 7772  des = _sort_n_wr
-0001c400: 6974 6528 0a20 2020 2020 2020 2020 2020  ite(.           
-0001c410: 2066 2c20 696e 6465 7065 6e64 656e 742c   f, independent,
-0001c420: 2063 6972 635f 7061 726d 732c 206e 6577   circ_parms, new
-0001c430: 7074 732c 206e 6577 6964 732c 2049 4473  pts, newids, IDs
-0001c440: 5b31 5d2c 2072 7370 6c69 6e65 5f69 6430  [1], rspline_id0
-0001c450: 2c20 446f 4c2c 206e 616d 6573 0a20 2020  , DoL, names.   
-0001c460: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001c470: 7265 7475 726e 206e 6577 7074 732c 206e  return newpts, n
-0001c480: 6577 6964 732c 2072 7370 6c69 6e65 5f6e  ewids, rspline_n
-0001c490: 6f64 6573 0a0a 2020 2020 2320 7772 6974  odes..    # writ
-0001c4a0: 6520 7468 6520 7273 706c 696e 653a 0a20  e the rspline:. 
-0001c4b0: 2020 206e 6577 7074 732c 206e 6577 6964     newpts, newid
-0001c4c0: 732c 2072 7370 6c69 6e65 5f6e 6f64 6573  s, rspline_nodes
-0001c4d0: 203d 205f 7772 6974 655f 6669 6c65 2866   = _write_file(f
-0001c4e0: 290a 0a20 2020 2061 7820 3d20 7974 6f6f  )..    ax = ytoo
-0001c4f0: 6c73 2e5f 6368 6563 6b5f 6d61 6b65 706c  ls._check_makepl
-0001c500: 6f74 286d 616b 6570 6c6f 742c 2066 6967  ot(makeplot, fig
-0001c510: 7369 7a65 3d5b 382c 2036 5d2c 206e 6565  size=[8, 6], nee
-0001c520: 6433 643d 5472 7565 290a 2020 2020 6966  d3d=True).    if
-0001c530: 2061 783a 0a20 2020 2020 2020 205f 706c   ax:.        _pl
-0001c540: 6f74 5f72 7370 6c69 6e65 280a 2020 2020  ot_rspline(.    
-0001c550: 2020 2020 2020 2020 6178 2c0a 2020 2020          ax,.    
-0001c560: 2020 2020 2020 2020 6369 7263 5f70 6172          circ_par
-0001c570: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-0001c580: 7879 7a2c 0a20 2020 2020 2020 2020 2020  xyz,.           
-0001c590: 206e 6577 7074 732c 0a20 2020 2020 2020   newpts,.       
-0001c5a0: 2020 2020 206e 6577 6964 732c 0a20 2020       newids,.   
-0001c5b0: 2020 2020 2020 2020 2062 6173 6963 326c           basic2l
-0001c5c0: 6f63 616c 2c0a 2020 2020 2020 2020 2020  ocal,.          
-0001c5d0: 2020 6365 6e74 6572 2c0a 2020 2020 2020    center,.      
-0001c5e0: 2020 2020 2020 7273 706c 696e 655f 6e6f        rspline_no
-0001c5f0: 6465 732c 0a20 2020 2020 2020 2020 2020  des,.           
-0001c600: 2049 4473 5b31 5d2c 0a20 2020 2020 2020   IDs[1],.       
-0001c610: 2020 2020 206e 616d 6573 2c0a 2020 2020       names,.    
-0001c620: 2020 2020 290a 0a0a 6465 6620 7774 636f      )...def wtco
-0001c630: 6f72 6463 6172 6473 2866 2c20 6369 293a  ordcards(f, ci):
-0001c640: 0a20 2020 2022 2222 0a20 2020 2057 7269  .    """.    Wri
-0001c650: 7465 204e 6173 7472 616e 2043 4f52 4432  te Nastran CORD2
-0001c660: 2a20 6361 7264 7320 746f 2061 2066 696c  * cards to a fil
-0001c670: 650a 0a20 2020 2050 6172 616d 6574 6572  e..    Parameter
-0001c680: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-0001c690: 0a20 2020 2066 203a 2073 7472 696e 6720  .    f : string 
-0001c6a0: 6f72 2066 696c 655f 6c69 6b65 206f 7220  or file_like or 
-0001c6b0: 3120 6f72 204e 6f6e 650a 2020 2020 2020  1 or None.      
-0001c6c0: 2020 4569 7468 6572 2061 206e 616d 6520    Either a name 
-0001c6d0: 6f66 2061 2066 696c 652c 206f 7220 6973  of a file, or is
-0001c6e0: 2061 2066 696c 655f 6c69 6b65 206f 626a   a file_like obj
-0001c6f0: 6563 7420 6173 2072 6574 7572 6e65 640a  ect as returned.
-0001c700: 2020 2020 2020 2020 6279 203a 6675 6e63          by :func
-0001c710: 3a60 6f70 656e 6020 6f72 203a 636c 6173  :`open` or :clas
-0001c720: 733a 6069 6f2e 5374 7269 6e67 494f 602e  s:`io.StringIO`.
-0001c730: 2049 6e70 7574 2061 7320 696e 7465 6765   Input as intege
-0001c740: 7220 3120 746f 0a20 2020 2020 2020 2077  r 1 to.        w
-0001c750: 7269 7465 2074 6f20 7374 646f 7574 2e20  rite to stdout. 
-0001c760: 4361 6e20 616c 736f 2062 6520 7468 6520  Can also be the 
-0001c770: 6e61 6d65 206f 6620 6120 6469 7265 6374  name of a direct
-0001c780: 6f72 7920 6f72 204e 6f6e 653b 0a20 2020  ory or None;.   
-0001c790: 2020 2020 2069 6e20 7468 6573 6520 6361       in these ca
-0001c7a0: 7365 732c 2061 2047 5549 2069 7320 6f70  ses, a GUI is op
-0001c7b0: 656e 6564 2066 6f72 2066 696c 6520 7365  ened for file se
-0001c7c0: 6c65 6374 696f 6e2e 0a20 2020 2063 6920  lection..    ci 
-0001c7d0: 3a20 6469 6374 696f 6e61 7279 206f 7220  : dictionary or 
-0001c7e0: 4e6f 6e65 0a20 2020 2020 2020 2044 6963  None.        Dic
-0001c7f0: 7469 6f6e 6172 7920 6f66 2063 6f6f 7264  tionary of coord
-0001c800: 696e 6174 6520 6361 7264 2069 6e66 6f20  inate card info 
-0001c810: 6173 2072 6574 7572 6e65 6420 6279 0a20  as returned by. 
-0001c820: 2020 2020 2020 203a 6675 6e63 3a60 7079         :func:`py
-0001c830: 7965 7469 2e6e 6173 7472 616e 2e6e 3270  yeti.nastran.n2p
-0001c840: 2e6d 6b63 6f72 6463 6172 6469 6e66 6f60  .mkcordcardinfo`
-0001c850: 2e20 4966 204e 6f6e 6520 6f72 2069 6620  . If None or if 
-0001c860: 6469 6374 0a20 2020 2020 2020 2069 7320  dict.        is 
-0001c870: 656d 7074 792c 2074 6869 7320 726f 7574  empty, this rout
-0001c880: 696e 6520 7175 6965 746c 7920 646f 6573  ine quietly does
-0001c890: 206e 6f74 6869 6e67 2e0a 0a20 2020 2052   nothing...    R
-0001c8a0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0001c8b0: 2d2d 0a20 2020 204e 6f6e 650a 0a20 2020  --.    None..   
-0001c8c0: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-0001c8d0: 0a20 2020 2054 7970 6963 616c 6c79 2063  .    Typically c
-0001c8e0: 616c 6c65 6420 6279 203a 6675 6e63 3a60  alled by :func:`
-0001c8f0: 7774 6578 7473 656f 7574 602e 0a0a 2020  wtextseout`...  
-0001c900: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-0001c910: 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20  -------.    >>> 
-0001c920: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-0001c930: 6e70 0a20 2020 203e 3e3e 2066 726f 6d20  np.    >>> from 
-0001c940: 7079 7965 7469 2069 6d70 6f72 7420 6e61  pyyeti import na
-0001c950: 7374 7261 6e0a 2020 2020 3e3e 3e20 6369  stran.    >>> ci
-0001c960: 203d 207b 3130 3a20 5b27 434f 5244 3252   = {10: ['CORD2R
-0001c970: 272c 206e 702e 6172 7261 7928 5b5b 3130  ', np.array([[10
-0001c980: 2c20 312c 2030 5d2c 0a20 2020 202e 2e2e  , 1, 0],.    ...
-0001c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9b0: 5b31 3030 2e2c 2030 2e2c 2030 2e5d 2c0a  [100., 0., 0.],.
-0001c9c0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
-0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9e0: 2020 2020 2020 205b 3130 302e 2c20 302e         [100., 0.
-0001c9f0: 2c20 3130 302e 5d2c 0a20 2020 202e 2e2e  , 100.],.    ...
-0001ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca20: 5b32 3030 2e2c 2030 2e2c 2030 2e5d 5d29  [200., 0., 0.]])
-0001ca30: 5d7d 0a20 2020 203e 3e3e 206e 6173 7472  ]}.    >>> nastr
-0001ca40: 616e 2e77 7463 6f6f 7264 6361 7264 7328  an.wtcoordcards(
-0001ca50: 312c 2063 6929 0a20 2020 2024 2043 6f6f  1, ci).    $ Coo
-0001ca60: 7264 696e 6174 6520 3130 3a0a 2020 2020  rdinate 10:.    
-0001ca70: 434f 5244 3252 2a20 2020 2020 2020 2020  CORD2R*         
-0001ca80: 2020 2020 2020 3130 2020 2020 2020 2020        10        
-0001ca90: 2020 2020 2020 2030 2020 312e 3030 3030         0  1.0000
-0001caa0: 3030 3030 652b 3032 2020 302e 3030 3030  0000e+02  0.0000
-0001cab0: 3030 3030 652b 3030 2a0a 2020 2020 2a20  0000e+00*.    * 
-0001cac0: 2020 2020 2020 2020 302e 3030 3030 3030          0.000000
-0001cad0: 3030 652b 3030 2020 312e 3030 3030 3030  00e+00  1.000000
-0001cae0: 3030 652b 3032 2020 302e 3030 3030 3030  00e+02  0.000000
-0001caf0: 3030 652b 3030 2020 312e 3030 3030 3030  00e+00  1.000000
-0001cb00: 3030 652b 3032 2a0a 2020 2020 2a20 2020  00e+02*.    *   
-0001cb10: 2020 2020 2020 322e 3030 3030 3030 3030        2.00000000
-0001cb20: 652b 3032 2020 302e 3030 3030 3030 3030  e+02  0.00000000
-0001cb30: 652b 3030 2020 302e 3030 3030 3030 3030  e+00  0.00000000
-0001cb40: 652b 3030 0a20 2020 2022 2222 0a20 2020  e+00.    """.   
-0001cb50: 2069 6620 6369 2069 7320 4e6f 6e65 206f   if ci is None o
-0001cb60: 7220 6c65 6e28 6369 2920 3d3d 2030 3a0a  r len(ci) == 0:.
-0001cb70: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-0001cb80: 2020 2020 4067 7569 746f 6f6c 732e 7772      @guitools.wr
-0001cb90: 6974 655f 7465 7874 5f66 696c 650a 2020  ite_text_file.  
-0001cba0: 2020 6465 6620 5f77 7463 6f6f 7264 7328    def _wtcoords(
-0001cbb0: 662c 2063 6929 3a0a 2020 2020 2020 2020  f, ci):.        
-0001cbc0: 666f 7220 6b20 696e 2063 693a 0a20 2020  for k in ci:.   
-0001cbd0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-0001cbe0: 6369 5b6b 5d20 2023 205b 6e61 6d65 2c20  ci[k]  # [name, 
-0001cbf0: 5b5b 6964 2c20 7479 7065 2c20 7265 665d  [[id, type, ref]
-0001cc00: 3b20 413b 2042 3b20 435d 5d0a 2020 2020  ; A; B; C]].    
-0001cc10: 2020 2020 2020 2020 636f 6f72 6420 3d20          coord = 
-0001cc20: 6461 7461 5b31 5d0a 2020 2020 2020 2020  data[1].        
-0001cc30: 2020 2020 6162 6320 3d20 2b63 6f6f 7264      abc = +coord
-0001cc40: 5b31 3a5d 0a20 2020 2020 2020 2020 2020  [1:].           
-0001cc50: 2061 6263 5b61 6273 2861 6263 2920 3c20   abc[abs(abc) < 
-0001cc60: 6162 7328 6162 6329 2e6d 6178 2829 202a  abs(abc).max() *
-0001cc70: 2031 652d 3135 5d20 3d20 302e 300a 2020   1e-15] = 0.0.  
-0001cc80: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-0001cc90: 6528 6622 2420 436f 6f72 6469 6e61 7465  e(f"$ Coordinate
-0001cca0: 207b 6b7d 3a5c 6e22 290a 2020 2020 2020   {k}:\n").      
-0001ccb0: 2020 2020 2020 662e 7772 6974 6528 0a20        f.write(. 
-0001ccc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001ccd0: 7b3a 3c38 737d 7b3a 3136 647d 7b3a 3136  {:<8s}{:16d}{:16
-0001cce0: 647d 7b3a 3136 2e38 657d 7b3a 3136 2e38  d}{:16.8e}{:16.8
-0001ccf0: 657d 2a5c 6e22 2e66 6f72 6d61 7428 0a20  e}*\n".format(. 
-0001cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd10: 2020 2064 6174 615b 305d 202b 2022 2a22     data[0] + "*"
-0001cd20: 2c20 6b2c 2069 6e74 2863 6f6f 7264 5b30  , k, int(coord[0
-0001cd30: 2c20 325d 292c 202a 6162 635b 302c 203a  , 2]), *abc[0, :
-0001cd40: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
-0001cd50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001cd60: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
-0001cd70: 2e77 7269 7465 2828 227b 3a3c 3873 7d22  .write(("{:<8s}"
-0001cd80: 202b 2022 7b3a 3136 2e38 657d 2220 2a20   + "{:16.8e}" * 
-0001cd90: 3420 2b20 222a 5c6e 2229 2e66 6f72 6d61  4 + "*\n").forma
-0001cda0: 7428 222a 222c 2061 6263 5b30 2c20 325d  t("*", abc[0, 2]
-0001cdb0: 2c20 2a61 6263 5b31 5d29 290a 2020 2020  , *abc[1])).    
-0001cdc0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001cdd0: 2822 7b3a 3c38 737d 2220 2b20 227b 3a31  ("{:<8s}" + "{:1
-0001cde0: 362e 3865 7d22 202a 2033 202b 2022 5c6e  6.8e}" * 3 + "\n
-0001cdf0: 2229 2e66 6f72 6d61 7428 222a 222c 202a  ").format("*", *
-0001ce00: 6162 635b 325d 2929 0a0a 2020 2020 5f77  abc[2]))..    _w
-0001ce10: 7463 6f6f 7264 7328 662c 2063 6929 0a0a  tcoords(f, ci)..
-0001ce20: 0a40 6775 6974 6f6f 6c73 2e77 7269 7465  .@guitools.write
-0001ce30: 5f74 6578 745f 6669 6c65 0a64 6566 2077  _text_file.def w
-0001ce40: 7465 7874 726e 2866 2c20 6964 732c 2064  textrn(f, ids, d
-0001ce50: 6f66 293a 0a20 2020 2022 2222 0a20 2020  of):.    """.   
-0001ce60: 2057 7269 7465 7320 6120 4e61 7374 7261   Writes a Nastra
-0001ce70: 6e20 4558 5452 4e20 6361 7264 2074 6f20  n EXTRN card to 
-0001ce80: 6120 6669 6c65 2e0a 0a20 2020 2050 6172  a file...    Par
-0001ce90: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0001cea0: 2d2d 2d2d 2d2d 0a20 2020 2066 203a 2073  ------.    f : s
-0001ceb0: 7472 696e 6720 6f72 2066 696c 655f 6c69  tring or file_li
-0001cec0: 6b65 206f 7220 3120 6f72 204e 6f6e 650a  ke or 1 or None.
-0001ced0: 2020 2020 2020 2020 4569 7468 6572 2061          Either a
-0001cee0: 206e 616d 6520 6f66 2061 2066 696c 652c   name of a file,
-0001cef0: 206f 7220 6973 2061 2066 696c 655f 6c69   or is a file_li
-0001cf00: 6b65 206f 626a 6563 7420 6173 2072 6574  ke object as ret
-0001cf10: 7572 6e65 640a 2020 2020 2020 2020 6279  urned.        by
-0001cf20: 203a 6675 6e63 3a60 6f70 656e 6020 6f72   :func:`open` or
-0001cf30: 203a 636c 6173 733a 6069 6f2e 5374 7269   :class:`io.Stri
-0001cf40: 6e67 494f 602e 2049 6e70 7574 2061 7320  ngIO`. Input as 
-0001cf50: 696e 7465 6765 7220 3120 746f 0a20 2020  integer 1 to.   
-0001cf60: 2020 2020 2077 7269 7465 2074 6f20 7374       write to st
-0001cf70: 646f 7574 2e20 4361 6e20 616c 736f 2062  dout. Can also b
-0001cf80: 6520 7468 6520 6e61 6d65 206f 6620 6120  e the name of a 
-0001cf90: 6469 7265 6374 6f72 7920 6f72 204e 6f6e  directory or Non
-0001cfa0: 653b 0a20 2020 2020 2020 2069 6e20 7468  e;.        in th
-0001cfb0: 6573 6520 6361 7365 732c 2061 2047 5549  ese cases, a GUI
-0001cfc0: 2069 7320 6f70 656e 6564 2066 6f72 2066   is opened for f
-0001cfd0: 696c 6520 7365 6c65 6374 696f 6e2e 0a20  ile selection.. 
-0001cfe0: 2020 2069 6473 203a 2031 6420 6172 7261     ids : 1d arra
-0001cff0: 795f 6c69 6b65 0a20 2020 2020 2020 2056  y_like.        V
-0001d000: 6563 746f 7220 6f66 206e 6f64 6520 6964  ector of node id
-0001d010: 730a 2020 2020 646f 6620 3a20 3164 2061  s.    dof : 1d a
-0001d020: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
-0001d030: 2020 5665 6374 6f72 206f 6620 444f 460a    Vector of DOF.
-0001d040: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-0001d050: 202d 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e   -------.    Non
-0001d060: 650a 0a20 2020 204e 6f74 6573 0a20 2020  e..    Notes.   
-0001d070: 202d 2d2d 2d2d 0a20 2020 2054 7970 6963   -----.    Typic
-0001d080: 616c 6c79 2063 616c 6c65 6420 6279 203a  ally called by :
-0001d090: 6675 6e63 3a60 7774 6578 7473 656f 7574  func:`wtextseout
-0001d0a0: 602e 0a0a 2020 2020 4578 616d 706c 6573  `...    Examples
-0001d0b0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001d0c0: 2020 3e3e 3e20 6672 6f6d 2070 7979 6574    >>> from pyyet
-0001d0d0: 6920 696d 706f 7274 206e 6173 7472 616e  i import nastran
-0001d0e0: 0a20 2020 203e 3e3e 206e 6173 7472 616e  .    >>> nastran
-0001d0f0: 2e77 7465 7874 726e 2831 2c20 5b39 3939  .wtextrn(1, [999
-0001d100: 2c20 3130 3030 312c 2031 3030 3032 2c20  , 10001, 10002, 
-0001d110: 3130 3030 332c 2031 3030 3034 2c20 3130  10003, 10004, 10
-0001d120: 3030 355d 2c0a 2020 2020 2e2e 2e20 2020  005],.    ...   
-0001d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d140: 205b 3132 3334 3536 2c20 302c 2030 2c20   [123456, 0, 0, 
-0001d150: 302c 2030 2c20 305d 290a 2020 2020 4558  0, 0, 0]).    EX
-0001d160: 5452 4e20 2020 2020 2020 2039 3939 2020  TRN        999  
-0001d170: 3132 3334 3536 2020 2031 3030 3031 2020  123456   10001  
-0001d180: 2020 2020 2030 2020 2031 3030 3032 2020       0   10002  
-0001d190: 2020 2020 2030 2020 2031 3030 3033 2020       0   10003  
-0001d1a0: 2020 2020 2030 0a20 2020 2020 2020 2020       0.         
-0001d1b0: 2020 2020 2020 3130 3030 3420 2020 2020        10004     
-0001d1c0: 2020 3020 2020 3130 3030 3520 2020 2020    0   10005     
-0001d1d0: 2020 300a 2020 2020 2222 220a 2020 2020    0.    """.    
-0001d1e0: 662e 7772 6974 6528 2245 5854 524e 2020  f.write("EXTRN  
-0001d1f0: 2022 290a 2020 2020 696e 7473 203d 206e   ").    ints = n
-0001d200: 702e 7a65 726f 7328 6c65 6e28 6964 7329  p.zeros(len(ids)
-0001d210: 202a 2032 2c20 6474 7970 653d 696e 7429   * 2, dtype=int)
-0001d220: 0a20 2020 2069 6e74 735b 3a3a 325d 203d  .    ints[::2] =
-0001d230: 2069 6473 0a20 2020 2069 6e74 735b 313a   ids.    ints[1:
-0001d240: 3a32 5d20 3d20 646f 660a 2020 2020 7774  :2] = dof.    wt
-0001d250: 6e61 7369 6e74 7328 662c 2032 2c20 696e  nasints(f, 2, in
-0001d260: 7473 290a 0a0a 6465 6620 7774 6578 7473  ts)...def wtexts
-0001d270: 656f 7574 280a 2020 2020 6e61 6d65 2c0a  eout(.    name,.
-0001d280: 2020 2020 2a2c 0a20 2020 2073 652c 0a20      *,.    se,. 
-0001d290: 2020 206d 6161 2c0a 2020 2020 6261 612c     maa,.    baa,
-0001d2a0: 0a20 2020 206b 6161 2c0a 2020 2020 6273  .    kaa,.    bs
-0001d2b0: 6574 2c0a 2020 2020 7573 6574 2c0a 2020  et,.    uset,.  
-0001d2c0: 2020 7370 6f69 6e74 312c 0a20 2020 2073    spoint1,.    s
-0001d2d0: 6564 6e3d 302c 0a20 2020 206e 616d 656c  edn=0,.    namel
-0001d2e0: 6973 743d 5b0a 2020 2020 2020 2020 226b  ist=[.        "k
-0001d2f0: 6161 222c 0a20 2020 2020 2020 2022 6d61  aa",.        "ma
-0001d300: 6122 2c0a 2020 2020 2020 2020 2262 6161  a",.        "baa
-0001d310: 222c 0a20 2020 2020 2020 2022 6b34 7878  ",.        "k4xx
-0001d320: 222c 0a20 2020 2020 2020 2022 7061 222c  ",.        "pa",
-0001d330: 0a20 2020 2020 2020 2022 6770 7878 222c  .        "gpxx",
-0001d340: 0a20 2020 2020 2020 2022 6764 7878 222c  .        "gdxx",
-0001d350: 0a20 2020 2020 2020 2022 7276 6178 222c  .        "rvax",
-0001d360: 0a20 2020 2020 2020 2022 7661 222c 0a20  .        "va",. 
-0001d370: 2020 2020 2020 2022 6d75 6731 222c 0a20         "mug1",. 
-0001d380: 2020 2020 2020 2022 6d75 6731 6f22 2c0a         "mug1o",.
-0001d390: 2020 2020 2020 2020 226d 6573 3122 2c0a          "mes1",.
-0001d3a0: 2020 2020 2020 2020 226d 6573 316f 222c          "mes1o",
-0001d3b0: 0a20 2020 2020 2020 2022 6d65 6531 222c  .        "mee1",
-0001d3c0: 0a20 2020 2020 2020 2022 6d65 6531 6f22  .        "mee1o"
-0001d3d0: 2c0a 2020 2020 2020 2020 226d 6770 6622  ,.        "mgpf"
-0001d3e0: 2c0a 2020 2020 2020 2020 226d 6770 666f  ,.        "mgpfo
-0001d3f0: 222c 0a20 2020 2020 2020 2022 6d65 6631  ",.        "mef1
-0001d400: 222c 0a20 2020 2020 2020 2022 6d65 6631  ",.        "mef1
-0001d410: 6f22 2c0a 2020 2020 2020 2020 226d 7167  o",.        "mqg
-0001d420: 3122 2c0a 2020 2020 2020 2020 226d 7167  1",.        "mqg
-0001d430: 316f 222c 0a20 2020 2020 2020 2022 6d71  1o",.        "mq
-0001d440: 6d67 3122 2c0a 2020 2020 2020 2020 226d  mg1",.        "m
-0001d450: 716d 6731 6f22 2c0a 2020 2020 5d2c 0a20  qmg1o",.    ],. 
-0001d460: 2020 202a 2a6b 7761 7267 732c 0a29 3a0a     **kwargs,.):.
-0001d470: 2020 2020 2222 220a 2020 2020 5772 6974      """.    Writ
-0001d480: 6520 2e6f 7034 2c20 2e61 736d 2c20 2e70  e .op4, .asm, .p
-0001d490: 6368 2061 6e64 2070 6f73 7369 626c 7920  ch and possibly 
-0001d4a0: 7468 6520 6461 6d70 696e 6720 444d 4947  the damping DMIG
-0001d4b0: 2066 696c 6520 666f 7220 616e 0a20 2020   file for an.   
-0001d4c0: 2065 7874 6572 6e61 6c20 5345 2e0a 0a20   external SE... 
-0001d4d0: 2020 204e 6f74 6520 7468 6174 2061 6c6c     Note that all
-0001d4e0: 2069 6e70 7574 7320 6578 6365 7074 2060   inputs except `
-0001d4f0: 6e61 6d65 6020 6d75 7374 2062 6520 6e61  name` must be na
-0001d500: 6d65 6420 616e 6420 6361 6e20 6265 2069  med and can be i
-0001d510: 6e70 7574 0a20 2020 2069 6e20 616e 7920  nput.    in any 
-0001d520: 6f72 6465 722e 0a0a 2020 2020 5061 7261  order...    Para
-0001d530: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-0001d540: 2d2d 2d2d 2d0a 2020 2020 6e61 6d65 203a  -----.    name :
-0001d550: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0001d560: 4261 7365 6e61 6d65 2066 6f72 2066 696c  Basename for fil
-0001d570: 6573 3b20 6567 3a20 2773 7061 6365 6372  es; eg: 'spacecr
-0001d580: 6166 7427 2e20 4669 6c65 7320 7769 7468  aft'. Files with
-0001d590: 2074 6865 0a20 2020 2020 2020 2065 7874   the.        ext
-0001d5a0: 656e 7369 6f6e 7320 272e 6f70 3427 2c20  ensions '.op4', 
-0001d5b0: 272e 6173 6d27 2c20 616e 6420 272e 7063  '.asm', and '.pc
-0001d5c0: 6827 2077 696c 6c20 6265 2063 7265 6174  h' will be creat
-0001d5d0: 6564 2e20 4966 2060 6268 600a 2020 2020  ed. If `bh`.    
-0001d5e0: 2020 2020 6973 2054 7275 652c 2061 2027      is True, a '
-0001d5f0: 2e62 6161 5f64 6d69 6727 2066 696c 6520  .baa_dmig' file 
-0001d600: 7769 6c6c 2061 6c73 6f20 6265 2063 7265  will also be cre
-0001d610: 6174 6564 2e0a 2020 2020 7365 203a 2069  ated..    se : i
-0001d620: 6e74 6567 6572 0a20 2020 2020 2020 2053  nteger.        S
-0001d630: 7570 6572 656c 656d 656e 7420 6964 3b20  uperelement id; 
-0001d640: 616c 736f 2075 7365 6420 6173 2074 6865  also used as the
-0001d650: 2046 6f72 7472 616e 2075 6e69 7420 6e75   Fortran unit nu
-0001d660: 6d62 6572 206f 6e20 7468 650a 2020 2020  mber on the.    
-0001d670: 2020 2020 5345 4255 4c4b 2065 6e74 7279      SEBULK entry
-0001d680: 2e0a 2020 2020 6d61 612c 2062 6161 2c20  ..    maa, baa, 
-0001d690: 6b61 6120 3a20 3264 2061 7272 6179 5f6c  kaa : 2d array_l
-0001d6a0: 696b 650a 2020 2020 2020 2020 5468 6573  ike.        Thes
-0001d6b0: 6520 6172 6520 7468 6520 4372 6169 672d  e are the Craig-
-0001d6c0: 4261 6d70 746f 6e20 6d61 7373 2c20 6461  Bampton mass, da
-0001d6d0: 6d70 696e 6720 616e 6420 7374 6966 666e  mping and stiffn
-0001d6e0: 6573 730a 2020 2020 2020 2020 6d61 7472  ess.        matr
-0001d6f0: 6963 6573 2072 6573 7065 6374 6976 656c  ices respectivel
-0001d700: 792e 0a20 2020 2062 7365 7420 3a20 3164  y..    bset : 1d
-0001d710: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
-0001d720: 2020 2020 496e 6465 7820 7061 7274 6974      Index partit
-0001d730: 696f 6e20 7665 6374 6f72 2066 6f72 2074  ion vector for t
-0001d740: 6865 2062 7365 740a 2020 2020 7573 6574  he bset.    uset
-0001d750: 203a 2070 616e 6461 7320 4461 7461 4672   : pandas DataFr
-0001d760: 616d 650a 2020 2020 2020 2020 4120 4461  ame.        A Da
-0001d770: 7461 4672 616d 6520 6173 206f 7574 7075  taFrame as outpu
-0001d780: 7420 6279 0a20 2020 2020 2020 203a 6675  t by.        :fu
-0001d790: 6e63 3a60 7079 7965 7469 2e6e 6173 7472  nc:`pyyeti.nastr
-0001d7a0: 616e 2e6f 7032 2e4f 5032 2e72 646e 3263  an.op2.OP2.rdn2c
-0001d7b0: 6f70 3260 2e0a 0a20 2020 2020 2020 202e  op2`...        .
-0001d7c0: 2e20 7761 726e 696e 673a 3a0a 2020 2020  . warning::.    
-0001d7d0: 2020 2020 2020 2020 556e 6c69 6b65 203a          Unlike :
-0001d7e0: 6675 6e63 3a60 7079 7965 7469 2e63 622e  func:`pyyeti.cb.
-0001d7f0: 6d6b 5f6e 6574 5f64 726d 7360 2c20 7468  mk_net_drms`, th
-0001d800: 6973 2055 5345 5420 7461 626c 650a 2020  is USET table.  
-0001d810: 2020 2020 2020 2020 2020 6465 6669 6e65            define
-0001d820: 7320 7468 6520 622d 7365 7420 6e6f 6465  s the b-set node
-0001d830: 7320 7265 6c61 7469 7665 2074 6f20 7468  s relative to th
-0001d840: 6520 6261 7369 6320 636f 6f72 6469 6e61  e basic coordina
-0001d850: 7465 0a20 2020 2020 2020 2020 2020 2073  te.            s
-0001d860: 7973 7465 6d20 6f66 2073 7570 6572 656c  ystem of superel
-0001d870: 656d 656e 7420 302e 2054 6869 7320 6973  ement 0. This is
-0001d880: 2073 6f20 7468 6520 6578 7465 726e 616c   so the external
-0001d890: 0a20 2020 2020 2020 2020 2020 2073 7570  .            sup
-0001d8a0: 6572 656c 656d 656e 7420 6973 2070 6f73  erelement is pos
-0001d8b0: 6974 696f 6e65 6420 7072 6f70 6572 6c79  itioned properly
-0001d8c0: 2e20 4e6f 7465 2068 6f77 6576 6572 2074  . Note however t
-0001d8d0: 6861 7420 7468 650a 2020 2020 2020 2020  hat the.        
-0001d8e0: 2020 2020 2264 6973 706c 6163 656d 656e      "displacemen
-0001d8f0: 7422 2063 6f6f 7264 696e 6174 6520 7379  t" coordinate sy
-0001d900: 7374 656d 2873 2920 2873 7065 6369 6669  stem(s) (specifi
-0001d910: 6564 2061 6674 6572 2074 6865 0a20 2020  ed after the.   
-0001d920: 2020 2020 2020 2020 2063 6f6f 7264 696e           coordin
-0001d930: 6174 6573 206f 6e20 7468 6520 2247 5249  ates on the "GRI
-0001d940: 4422 2063 6172 6429 206d 7573 7420 6d61  D" card) must ma
-0001d950: 7463 6820 7768 6174 6576 6572 2074 6865  tch whatever the
-0001d960: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-0001d970: 706c 6163 656d 656e 7420 636f 6f72 6469  placement coordi
-0001d980: 6e61 7465 2073 7973 7465 6d28 7329 2061  nate system(s) a
-0001d990: 7265 2066 6f72 2074 6865 0a20 2020 2020  re for the.     
-0001d9a0: 2020 2020 2020 2043 7261 6967 2d42 616d         Craig-Bam
-0001d9b0: 7074 6f6e 2063 6f6d 706f 6e65 6e74 2e0a  pton component..
-0001d9c0: 0a20 2020 2073 706f 696e 7431 203a 2069  .    spoint1 : i
-0001d9d0: 6e74 6567 6572 0a20 2020 2020 2020 2053  nteger.        S
-0001d9e0: 7461 7274 696e 6720 7661 6c75 6520 666f  tarting value fo
-0001d9f0: 7220 7468 6520 5350 4f49 4e54 7320 2866  r the SPOINTs (f
-0001da00: 6f72 206d 6f64 616c 2044 4f46 290a 2020  or modal DOF).  
-0001da10: 2020 7365 646e 203a 2069 6e74 6567 6572    sedn : integer
-0001da20: 3b20 6f70 7469 6f6e 616c 0a20 2020 2020  ; optional.     
-0001da30: 2020 2044 6f77 6e73 7472 6561 6d20 7375     Downstream su
-0001da40: 7065 7265 6c65 6d65 6e74 2069 640a 2020  perelement id.  
-0001da50: 2020 6e61 6d65 6c69 7374 203a 206c 6973    namelist : lis
-0001da60: 743b 206f 7074 696f 6e61 6c0a 2020 2020  t; optional.    
-0001da70: 2020 2020 4c69 7374 2c20 696e 206f 7264      List, in ord
-0001da80: 6572 2c20 6f66 206e 616d 6573 2074 6f20  er, of names to 
-0001da90: 7772 6974 6520 746f 2074 6865 206f 7034  write to the op4
-0001daa0: 2066 696c 652e 2056 616c 7565 730a 2020   file. Values.  
-0001dab0: 2020 2020 2020 6465 6661 756c 7420 746f        default to
-0001dac0: 2031 7831 207a 6572 6f20 6d61 7472 6963   1x1 zero matric
-0001dad0: 6573 2077 6974 6820 7468 6573 6520 6578  es with these ex
-0001dae0: 6365 7074 696f 6e73 3a20 226d 6161 222c  ceptions: "maa",
-0001daf0: 0a20 2020 2020 2020 2022 6b61 6122 2c20  .        "kaa", 
-0001db00: 2262 6161 222c 2061 7265 2061 7320 696e  "baa", are as in
-0001db10: 7075 7420 6162 6f76 652c 2022 7061 2220  put above, "pa" 
-0001db20: 6973 2061 2076 6563 746f 7220 6f66 207a  is a vector of z
-0001db30: 6572 6f73 0a20 2020 2020 2020 2061 6e64  eros.        and
-0001db40: 2022 7661 2220 6973 2061 2076 6563 746f   "va" is a vecto
-0001db50: 7220 6f66 206f 6e65 732e 2054 6865 2064  r of ones. The d
-0001db60: 6566 6175 6c74 7320 6361 6e20 6265 206f  efaults can be o
-0001db70: 7665 7272 6964 6465 6e0a 2020 2020 2020  verridden.      
-0001db80: 2020 696e 2060 6b77 6172 6773 602e 0a20    in `kwargs`.. 
-0001db90: 2020 202a 2a6b 7761 7267 7320 3a20 6f70     **kwargs : op
-0001dba0: 7469 6f6e 616c 0a20 2020 2020 2020 2041  tional.        A
-0001dbb0: 6c6c 6f77 7320 7573 6572 2074 6f20 696e  llows user to in
-0001dbc0: 7075 7420 6f74 6865 7220 6d61 7472 6963  put other matric
-0001dbd0: 6573 2074 6f20 6265 2077 7269 7474 656e  es to be written
-0001dbe0: 2074 6f20 7468 6520 6f70 340a 2020 2020   to the op4.    
-0001dbf0: 2020 2020 6669 6c65 2e20 4e61 6d65 206d      file. Name m
-0001dc00: 7573 7420 696e 2060 6e61 6d65 6c69 7374  ust in `namelist
-0001dc10: 6020 746f 2062 6520 7772 6974 7465 6e2e  ` to be written.
-0001dc20: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0001dc30: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f    -------.    No
-0001dc40: 6e65 0a20 2020 2022 2222 0a20 2020 206d  ne.    """.    m
-0001dc50: 6161 2c20 6261 612c 206b 6161 203d 206e  aa, baa, kaa = n
-0001dc60: 702e 6174 6c65 6173 745f 3264 286d 6161  p.atleast_2d(maa
-0001dc70: 2c20 6261 612c 206b 6161 290a 2020 2020  , baa, kaa).    
-0001dc80: 6273 6574 203d 206e 702e 6174 6c65 6173  bset = np.atleas
-0001dc90: 745f 3164 2862 7365 7429 0a20 2020 206e  t_1d(bset).    n
-0001dca0: 203d 206d 6161 2e73 6861 7065 5b30 5d0a   = maa.shape[0].
-0001dcb0: 2020 2020 6e71 203d 206e 202d 206c 656e      nq = n - len
-0001dcc0: 2862 7365 7429 0a0a 2020 2020 2320 7072  (bset)..    # pr
-0001dcd0: 6570 6172 6520 7374 616e 6461 7264 204e  epare standard N
-0001dce0: 6173 7472 616e 206f 7034 2066 696c 653a  astran op4 file:
-0001dcf0: 0a20 2020 2070 6120 3d20 6e70 2e7a 6572  .    pa = np.zer
-0001dd00: 6f73 2828 6e2c 2031 2929 0a20 2020 2076  os((n, 1)).    v
-0001dd10: 6120 3d20 6e70 2e6f 6e65 7328 286e 2c20  a = np.ones((n, 
-0001dd20: 3129 290a 2020 2020 6463 7420 3d20 7b2a  1)).    dct = {*
-0001dd30: 2a6c 6f63 616c 7328 292c 202a 2a6b 7761  *locals(), **kwa
-0001dd40: 7267 737d 0a20 2020 2076 6172 6c69 7374  rgs}.    varlist
-0001dd50: 203d 205b 6463 742e 6765 7428 692c 2030   = [dct.get(i, 0
-0001dd60: 2e30 2920 666f 7220 6920 696e 206e 616d  .0) for i in nam
-0001dd70: 656c 6973 745d 0a20 2020 206f 7034 2e77  elist].    op4.w
-0001dd80: 7269 7465 286e 616d 6520 2b20 222e 6f70  rite(name + ".op
-0001dd90: 3422 2c20 6e61 6d65 6c69 7374 2c20 7661  4", namelist, va
-0001dda0: 726c 6973 7429 0a0a 2020 2020 2320 4765  rlist)..    # Ge
-0001ddb0: 7420 736f 6d65 2064 6174 6120 6672 6f6d  t some data from
-0001ddc0: 2074 6865 2075 7365 7420 7461 626c 653a   the uset table:
-0001ddd0: 0a20 2020 2063 6920 3d20 6e32 702e 6d6b  .    ci = n2p.mk
-0001dde0: 636f 7264 6361 7264 696e 666f 2875 7365  cordcardinfo(use
-0001ddf0: 7429 0a20 2020 2067 7269 6473 203d 2075  t).    grids = u
-0001de00: 7365 742e 696e 6465 782e 6765 745f 6c65  set.index.get_le
-0001de10: 7665 6c5f 7661 6c75 6573 2822 6964 2229  vel_values("id")
-0001de20: 0a20 2020 2064 6f66 203d 2075 7365 742e  .    dof = uset.
-0001de30: 696e 6465 782e 6765 745f 6c65 7665 6c5f  index.get_level_
-0001de40: 7661 6c75 6573 2822 646f 6622 290a 2020  values("dof").  
-0001de50: 2020 7076 203d 2064 6f66 203d 3d20 310a    pv = dof == 1.
-0001de60: 2020 2020 6772 6964 7320 3d20 6772 6964      grids = grid
-0001de70: 735b 7076 5d0a 2020 2020 7879 7a20 3d20  s[pv].    xyz = 
-0001de80: 7573 6574 2e6c 6f63 5b70 762c 2022 7822  uset.loc[pv, "x"
-0001de90: 3a22 7a22 5d2e 7661 6c75 6573 0a20 2020  :"z"].values.   
-0001dea0: 2070 7620 3d20 646f 6620 3d3d 2032 0a20   pv = dof == 2. 
-0001deb0: 2020 2063 6420 3d20 7573 6574 2e6c 6f63     cd = uset.loc
-0001dec0: 5b70 762c 2022 7822 5d2e 7661 6c75 6573  [pv, "x"].values
-0001ded0: 2e61 7374 7970 6528 696e 7429 0a0a 2020  .astype(int)..  
-0001dee0: 2020 2320 5772 6974 6520 6f75 7420 4153    # Write out AS
-0001def0: 4d20 6669 6c65 0a20 2020 2075 6e69 7420  M file.    unit 
-0001df00: 3d20 7365 0a20 2020 2073 706f 696e 746e  = se.    spointn
-0001df10: 203d 2073 706f 696e 7431 202b 206e 7120   = spoint1 + nq 
-0001df20: 2d20 310a 2020 2020 7769 7468 206f 7065  - 1.    with ope
-0001df30: 6e28 6e61 6d65 202b 2022 2e61 736d 222c  n(name + ".asm",
-0001df40: 2022 7722 2920 6173 2066 3a0a 2020 2020   "w") as f:.    
-0001df50: 2020 2020 662e 7772 6974 6528 0a20 2020      f.write(.   
-0001df60: 2020 2020 2020 2020 2066 2224 207b 6e61           f"$ {na
-0001df70: 6d65 2e75 7070 6572 2829 7d20 4153 5345  me.upper()} ASSE
-0001df80: 4d42 4c59 2046 494c 4520 464f 5220 5245  MBLY FILE FOR RE
-0001df90: 5349 4455 414c 2052 554e 2e2e 2e49 4e43  SIDUAL RUN...INC
-0001dfa0: 4c55 4445 2049 4e20 4255 4c4b 2044 4154  LUDE IN BULK DAT
-0001dfb0: 415c 6e22 0a20 2020 2020 2020 2029 0a20  A\n".        ). 
-0001dfc0: 2020 2020 2020 2066 2e77 7269 7465 2822         f.write("
-0001dfd0: 245c 6e22 290a 2020 2020 2020 2020 662e  $\n").        f.
-0001dfe0: 7772 6974 6528 6622 5345 4255 4c4b 2020  write(f"SEBULK  
-0001dff0: 7b73 653a 3864 7d20 2045 5854 4f50 3420  {se:8d}  EXTOP4 
-0001e000: 2020 2020 2020 2020 204d 414e 5541 4c20           MANUAL 
-0001e010: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0001e020: 756e 6974 3a38 647d 5c6e 2229 0a20 2020  unit:8d}\n").   
-0001e030: 2020 2020 2066 2e77 7269 7465 2866 2253       f.write(f"S
-0001e040: 4543 4f4e 4354 207b 7365 3a38 647d 7b73  ECONCT {se:8d}{s
-0001e050: 6564 6e3a 3864 7d20 2020 2020 2020 2020  edn:8d}         
-0001e060: 2020 2020 204e 4f5c 6e22 290a 2020 2020       NO\n").    
-0001e070: 2020 2020 662e 7772 6974 6528 2220 2020      f.write("   
-0001e080: 2020 2020 2022 290a 2020 2020 2020 2020       ").        
-0001e090: 6769 6473 203d 206e 702e 7673 7461 636b  gids = np.vstack
-0001e0a0: 2828 6772 6964 732c 2067 7269 6473 2929  ((grids, grids))
-0001e0b0: 2e54 0a20 2020 2020 2020 2077 746e 6173  .T.        wtnas
-0001e0c0: 696e 7473 2866 2c20 322c 2067 6964 732e  ints(f, 2, gids.
-0001e0d0: 7261 7665 6c28 2929 0a0a 2020 2020 2020  ravel())..      
-0001e0e0: 2020 2320 5772 6974 6520 636f 6f72 6469    # Write coordi
-0001e0f0: 6e61 7465 2073 7973 7465 6d20 6361 7264  nate system card
-0001e100: 7320 6966 206e 6565 6465 643a 0a20 2020  s if needed:.   
-0001e110: 2020 2020 2066 2e77 7269 7465 2822 245c       f.write("$\
-0001e120: 6e24 2043 4f4f 5244 494e 4154 4520 5359  n$ COORDINATE SY
-0001e130: 5354 454d 2044 4154 415c 6e24 5c6e 2229  STEM DATA\n$\n")
-0001e140: 0a20 2020 2020 2020 2077 7463 6f6f 7264  .        wtcoord
-0001e150: 6361 7264 7328 662c 2063 6929 0a0a 2020  cards(f, ci)..  
-0001e160: 2020 2020 2020 2320 5772 6974 6520 4772        # Write Gr
-0001e170: 6964 2064 6174 613a 0a20 2020 2020 2020  id data:.       
-0001e180: 2066 2e77 7269 7465 2822 245c 6e24 2042   f.write("$\n$ B
-0001e190: 4f55 4e44 4152 5920 4752 4944 2044 4154  OUNDARY GRID DAT
-0001e1a0: 415c 6e24 5c6e 2229 0a20 2020 2020 2020  A\n$\n").       
-0001e1b0: 2077 7467 7269 6473 2866 2c20 6772 6964   wtgrids(f, grid
-0001e1c0: 732c 2030 2c20 7879 7a2c 2063 6429 0a20  s, 0, xyz, cd). 
-0001e1d0: 2020 2020 2020 2069 6620 7370 6f69 6e74         if spoint
-0001e1e0: 6e20 3e3d 2073 706f 696e 7431 3a0a 2020  n >= spoint1:.  
-0001e1f0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-0001e200: 6528 2224 5c6e 2229 0a20 2020 2020 2020  e("$\n").       
-0001e210: 2020 2020 2066 2e77 7269 7465 2866 2253       f.write(f"S
-0001e220: 4543 4f4e 4354 207b 7365 3a38 647d 7b73  ECONCT {se:8d}{s
-0001e230: 6564 6e3a 3864 7d20 2020 2020 2020 2020  edn:8d}         
-0001e240: 2020 2020 204e 4f5c 6e22 290a 2020 2020       NO\n").    
-0001e250: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001e260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e270: 2066 2220 2020 2020 2020 207b 7370 6f69   f"        {spoi
-0001e280: 6e74 313a 3864 7d20 2020 2054 4852 557b  nt1:8d}    THRU{
-0001e290: 7370 6f69 6e74 6e3a 3864 7d22 0a20 2020  spointn:8d}".   
-0001e2a0: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-0001e2b0: 7370 6f69 6e74 313a 3864 7d20 2020 2054  spoint1:8d}    T
-0001e2c0: 4852 557b 7370 6f69 6e74 6e3a 3864 7d5c  HRU{spointn:8d}\
-0001e2d0: 6e22 0a20 2020 2020 2020 2020 2020 2029  n".            )
-0001e2e0: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-0001e2f0: 7269 7465 2822 245c 6e22 290a 2020 2020  rite("$\n").    
-0001e300: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001e310: 6622 5350 4f49 4e54 2020 7b73 706f 696e  f"SPOINT  {spoin
-0001e320: 7431 3a38 647d 2020 2020 5448 5255 7b73  t1:8d}    THRU{s
-0001e330: 706f 696e 746e 3a38 647d 5c6e 2229 0a0a  pointn:8d}\n")..
-0001e340: 2020 2020 2320 5772 6974 6520 6f75 7420      # Write out 
-0001e350: 5043 4820 6669 6c65 0a20 2020 2077 6974  PCH file.    wit
-0001e360: 6820 6f70 656e 286e 616d 6520 2b20 222e  h open(name + ".
-0001e370: 7063 6822 2c20 2277 2229 2061 7320 663a  pch", "w") as f:
-0001e380: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
-0001e390: 2866 2224 207b 6e61 6d65 2e75 7070 6572  (f"$ {name.upper
-0001e3a0: 2829 7d20 5055 4e43 4820 4649 4c45 2046  ()} PUNCH FILE F
-0001e3b0: 4f52 2052 4553 4944 5541 4c20 5255 4e2e  OR RESIDUAL RUN.
-0001e3c0: 2e2e 494e 434c 5544 4520 4154 2045 4e44  ..INCLUDE AT END
-0001e3d0: 5c6e 2229 0a20 2020 2020 2020 2066 2e77  \n").        f.w
-0001e3e0: 7269 7465 2822 245c 6e22 290a 2020 2020  rite("$\n").    
-0001e3f0: 2020 2020 662e 7772 6974 6528 6622 4245      f.write(f"BE
-0001e400: 4749 4e20 5355 5045 527b 7365 3a38 647d  GIN SUPER{se:8d}
-0001e410: 5c6e 245c 6e22 290a 2020 2020 2020 2020  \n$\n").        
-0001e420: 6964 7320 3d20 6e70 2e68 7374 6163 6b28  ids = np.hstack(
-0001e430: 2867 7269 6473 2c20 7370 6f69 6e74 3120  (grids, spoint1 
-0001e440: 2b20 6e70 2e61 7261 6e67 6528 6e71 2929  + np.arange(nq))
-0001e450: 290a 2020 2020 2020 2020 646f 6620 3d20  ).        dof = 
-0001e460: 6e70 2e7a 6572 6f73 5f6c 696b 6528 6964  np.zeros_like(id
-0001e470: 732c 2064 7479 7065 3d69 6e74 290a 2020  s, dtype=int).  
-0001e480: 2020 2020 2020 646f 665b 3a20 6c65 6e28        dof[: len(
-0001e490: 6772 6964 7329 5d20 3d20 3132 3334 3536  grids)] = 123456
-0001e4a0: 0a20 2020 2020 2020 2077 7465 7874 726e  .        wtextrn
-0001e4b0: 2866 2c20 6964 732c 2064 6f66 290a 2020  (f, ids, dof).  
-0001e4c0: 2020 2020 2020 662e 7772 6974 6528 2224        f.write("$
-0001e4d0: 5c6e 2229 0a20 2020 2020 2020 2066 2e77  \n").        f.w
-0001e4e0: 7269 7465 2822 2420 434f 4f52 4449 4e41  rite("$ COORDINA
-0001e4f0: 5445 2053 5953 5445 4d20 4441 5441 5c6e  TE SYSTEM DATA\n
-0001e500: 245c 6e22 290a 2020 2020 2020 2020 7774  $\n").        wt
-0001e510: 636f 6f72 6463 6172 6473 2866 2c20 6369  coordcards(f, ci
-0001e520: 290a 2020 2020 2020 2020 662e 7772 6974  ).        f.writ
-0001e530: 6528 2224 5c6e 2420 424f 554e 4441 5259  e("$\n$ BOUNDARY
-0001e540: 2047 5249 4420 4441 5441 5c6e 245c 6e22   GRID DATA\n$\n"
-0001e550: 290a 2020 2020 2020 2020 7774 6772 6964  ).        wtgrid
-0001e560: 7328 662c 2067 7269 6473 2c20 302c 2078  s(f, grids, 0, x
-0001e570: 797a 2c20 6364 290a 2020 2020 2020 2020  yz, cd).        
-0001e580: 662e 7772 6974 6528 2224 5c6e 2229 0a0a  f.write("$\n")..
-0001e590: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001e5a0: 2224 2042 5345 545c 6e24 5c6e 2229 0a20  "$ BSET\n$\n"). 
-0001e5b0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
-0001e5c0: 2241 5345 5431 2020 207b 3132 3334 3536  "ASET1   {123456
-0001e5d0: 3a38 647d 2229 0a20 2020 2020 2020 2077  :8d}").        w
-0001e5e0: 746e 6173 696e 7473 2866 2c20 332c 2067  tnasints(f, 3, g
-0001e5f0: 7269 6473 290a 2020 2020 2020 2020 6966  rids).        if
-0001e600: 2073 706f 696e 746e 203e 3d20 7370 6f69   spointn >= spoi
-0001e610: 6e74 313a 0a20 2020 2020 2020 2020 2020  nt1:.           
-0001e620: 2066 2e77 7269 7465 2822 245c 6e22 290a   f.write("$\n").
-0001e630: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-0001e640: 6974 6528 2224 2051 5345 545c 6e24 5c6e  ite("$ QSET\n$\n
-0001e650: 2229 0a20 2020 2020 2020 2020 2020 2066  ").            f
-0001e660: 2e77 7269 7465 2866 2251 5345 5431 2020  .write(f"QSET1  
-0001e670: 207b 303a 3864 7d7b 7370 6f69 6e74 313a   {0:8d}{spoint1:
-0001e680: 3864 7d20 2020 2054 4852 557b 7370 6f69  8d}    THRU{spoi
-0001e690: 6e74 6e3a 3864 7d5c 6e22 290a 2020 2020  ntn:8d}\n").    
-0001e6a0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001e6b0: 2224 5c6e 2229 0a20 2020 2020 2020 2020  "$\n").         
-0001e6c0: 2020 2066 2e77 7269 7465 2866 2253 504f     f.write(f"SPO
-0001e6d0: 494e 5420 207b 7370 6f69 6e74 313a 3864  INT  {spoint1:8d
-0001e6e0: 7d20 2020 2054 4852 557b 7370 6f69 6e74  }    THRU{spoint
-0001e6f0: 6e3a 3864 7d5c 6e22 290a 0a0a 6465 6620  n:8d}\n")...def 
-0001e700: 6d6b 6e61 7374 280a 2020 2020 7363 7269  mknast(.    scri
-0001e710: 7074 3d4e 6f6e 652c 0a20 2020 202a 2c0a  pt=None,.    *,.
-0001e720: 2020 2020 6e61 7363 6f6d 3d22 6e61 7374      nascom="nast
-0001e730: 3970 3122 2c0a 2020 2020 6e61 736f 7074  9p1",.    nasopt
-0001e740: 3d22 6261 7463 683d 6e6f 222c 0a20 2020  ="batch=no",.   
-0001e750: 2065 7874 3d22 6f75 7422 2c0a 2020 2020   ext="out",.    
-0001e760: 7374 6f70 6f6e 6661 7461 6c3d 4661 6c73  stoponfatal=Fals
-0001e770: 652c 0a20 2020 2073 6865 6c6c 3d22 2f62  e,.    shell="/b
-0001e780: 696e 2f73 6822 2c0a 2020 2020 6669 6c65  in/sh",.    file
-0001e790: 733d 4e6f 6e65 2c0a 2020 2020 6265 666f  s=None,.    befo
-0001e7a0: 7265 3d22 222c 0a20 2020 2061 6674 6572  re="",.    after
-0001e7b0: 3d22 222c 0a20 2020 2074 6f70 3d22 222c  ="",.    top="",
-0001e7c0: 0a20 2020 2062 6f74 746f 6d3d 2222 2c0a  .    bottom="",.
-0001e7d0: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
-0001e7e0: 7265 6174 6573 2061 2073 6865 6c6c 2073  reates a shell s
-0001e7f0: 6372 6970 7420 666f 7220 7275 6e6e 696e  cript for runnin
-0001e800: 6720 6120 6368 6169 6e20 6f66 204e 6173  g a chain of Nas
-0001e810: 7472 616e 2028 6f72 206f 7468 6572 290a  tran (or other).
-0001e820: 2020 2020 7275 6e73 2e0a 0a20 2020 204e      runs...    N
-0001e830: 6f74 6520 7468 6174 2061 6c6c 2069 6e70  ote that all inp
-0001e840: 7574 7320 6578 6365 7074 2060 7363 7269  uts except `scri
-0001e850: 7074 6020 6d75 7374 2062 6520 6e61 6d65  pt` must be name
-0001e860: 6420 616e 6420 6361 6e20 6265 0a20 2020  d and can be.   
-0001e870: 2069 6e70 7574 2069 6e20 616e 7920 6f72   input in any or
-0001e880: 6465 722e 0a0a 2020 2020 5061 7261 6d65  der...    Parame
-0001e890: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001e8a0: 2d2d 2d0a 2020 2020 7363 7269 7074 203a  ---.    script :
-0001e8b0: 2073 7472 696e 6720 6f72 204e 6f6e 653b   string or None;
-0001e8c0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0001e8d0: 2020 4e61 6d65 206f 6620 7368 656c 6c20    Name of shell 
-0001e8e0: 7363 7269 7074 2074 6f20 6372 6561 7465  script to create
-0001e8f0: 3b20 6966 204e 6f6e 652c 2075 7365 7220  ; if None, user 
-0001e900: 6973 2070 726f 6d70 7465 6420 666f 720a  is prompted for.
-0001e910: 2020 2020 2020 2020 6e61 6d65 2e0a 2020          name..  
-0001e920: 2020 6e61 7363 6f6d 203a 2073 7472 696e    nascom : strin
-0001e930: 673b 206f 7074 696f 6e61 6c0a 2020 2020  g; optional.    
-0001e940: 2020 2020 4e61 7374 7261 6e20 636f 6d6d      Nastran comm
-0001e950: 616e 643b 206e 6f74 653a 2074 6869 7320  and; note: this 
-0001e960: 6361 6e20 6163 7475 616c 6c79 2073 7065  can actually spe
-0001e970: 6369 6679 2061 6e79 2070 726f 6772 616d  cify any program
-0001e980: 2c0a 2020 2020 2020 2020 6275 7420 606e  ,.        but `n
-0001e990: 6173 6f70 7460 2077 6f75 6c64 206c 696b  asopt` would lik
-0001e9a0: 656c 7920 6e65 6564 2061 646a 7573 7469  ely need adjusti
-0001e9b0: 6e67 2074 6f6f 2e0a 2020 2020 6e61 736f  ng too..    naso
-0001e9c0: 7074 203a 2073 7472 696e 673b 206f 7074  pt : string; opt
-0001e9d0: 696f 6e61 6c0a 2020 2020 2020 2020 4f70  ional.        Op
-0001e9e0: 7469 6f6e 7320 666f 7220 6e61 7374 7261  tions for nastra
-0001e9f0: 6e20 636f 6d6d 616e 640a 2020 2020 6578  n command.    ex
-0001ea00: 7420 3a20 7374 7269 6e67 3b20 6f70 7469  t : string; opti
-0001ea10: 6f6e 616c 0a20 2020 2020 2020 2054 6865  onal.        The
-0001ea20: 2065 7874 656e 7369 6f6e 206f 6620 7468   extension of th
-0001ea30: 6520 4e61 7374 7261 6e20 6f75 7470 7574  e Nastran output
-0001ea40: 2028 6630 3629 2066 696c 653b 2075 7375   (f06) file; usu
-0001ea50: 616c 6c79 2027 6630 3627 0a20 2020 2020  ally 'f06'.     
-0001ea60: 2020 206f 7220 276f 7574 270a 2020 2020     or 'out'.    
-0001ea70: 7374 6f70 6f6e 6661 7461 6c20 3a20 626f  stoponfatal : bo
-0001ea80: 6f6c 3b20 6f70 7469 6f6e 616c 0a20 2020  ol; optional.   
-0001ea90: 2020 2020 2053 6574 2074 6f20 5472 7565       Set to True
-0001eaa0: 2069 6620 796f 7520 7761 6e74 2074 6865   if you want the
-0001eab0: 2073 6372 6970 7420 746f 2065 7869 7420   script to exit 
-0001eac0: 6f6e 2066 6972 7374 2046 4154 414c 0a20  on first FATAL. 
-0001ead0: 2020 2020 2020 2069 6e73 7465 6164 206f         instead o
-0001eae0: 6620 636f 6e74 696e 7569 6e67 206f 6e0a  f continuing on.
-0001eaf0: 2020 2020 7368 656c 6c20 3a20 7374 7269      shell : stri
-0001eb00: 6e67 3b20 6f70 7469 6f6e 616c 0a20 2020  ng; optional.   
-0001eb10: 2020 2020 2053 6865 6c6c 2070 726f 6772       Shell progr
-0001eb20: 616d 2074 6f20 7772 6974 6520 6174 2074  am to write at t
-0001eb30: 6f70 206f 6620 7363 7269 7074 2c20 6567  op of script, eg
-0001eb40: 3a20 2321 6073 6865 6c6c 600a 2020 2020  : #!`shell`.    
-0001eb50: 6669 6c65 7320 3a20 7374 7269 6e67 206f  files : string o
-0001eb60: 7220 4e6f 6e65 3b20 6f70 7469 6f6e 616c  r None; optional
-0001eb70: 0a20 2020 2020 2020 204c 6973 7420 6f66  .        List of
-0001eb80: 2066 696c 656e 616d 6573 2074 6f20 7275   filenames to ru
-0001eb90: 6e3b 2069 6620 4e6f 6e65 2c20 7573 6572  n; if None, user
-0001eba0: 2069 7320 7072 6f6d 7074 6564 2066 6f72   is prompted for
-0001ebb0: 206e 616d 6573 0a20 2020 2062 6566 6f72   names.    befor
-0001ebc0: 6520 3a20 7374 7269 6e67 3b20 6f70 7469  e : string; opti
-0001ebd0: 6f6e 616c 0a20 2020 2020 2020 2053 7472  onal.        Str
-0001ebe0: 696e 6720 746f 2070 7574 2069 6e20 7368  ing to put in sh
-0001ebf0: 656c 6c20 7363 7269 7074 2062 6566 6f72  ell script befor
-0001ec00: 6520 6561 6368 206e 6173 7472 616e 2063  e each nastran c
-0001ec10: 6f6d 6d61 6e64 0a20 2020 2061 6674 6572  ommand.    after
-0001ec20: 203a 2073 7472 696e 673b 206f 7074 696f   : string; optio
-0001ec30: 6e61 6c0a 2020 2020 2020 2020 5374 7269  nal.        Stri
-0001ec40: 6e67 2074 6f20 7075 7420 696e 2073 6865  ng to put in she
-0001ec50: 6c6c 2073 6372 6970 7420 6166 7465 7220  ll script after 
-0001ec60: 6561 6368 206e 6173 7472 616e 2063 6f6d  each nastran com
-0001ec70: 6d61 6e64 0a20 2020 2074 6f70 203a 2073  mand.    top : s
-0001ec80: 7472 696e 673b 206f 7074 696f 6e61 6c0a  tring; optional.
-0001ec90: 2020 2020 2020 2020 5374 7269 6e67 2074          String t
-0001eca0: 6f20 7075 7420 696e 2073 6865 6c6c 2073  o put in shell s
-0001ecb0: 6372 6970 7420 6174 2074 6865 2074 6f70  cript at the top
-0001ecc0: 0a20 2020 2062 6f74 746f 6d20 3a20 7374  .    bottom : st
-0001ecd0: 7269 6e67 3b20 6f70 7469 6f6e 616c 0a20  ring; optional. 
-0001ece0: 2020 2020 2020 2053 7472 696e 6720 746f         String to
-0001ecf0: 2070 7574 2069 6e20 7368 656c 6c20 7363   put in shell sc
-0001ed00: 7269 7074 2061 7420 7468 6520 626f 7474  ript at the bott
-0001ed10: 6f6d 0a0a 2020 2020 5265 7475 726e 730a  om..    Returns.
-0001ed20: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0001ed30: 4e6f 6e65 0a0a 2020 2020 4e6f 7465 730a  None..    Notes.
-0001ed40: 2020 2020 2d2d 2d2d 2d0a 2020 2020 4966      -----.    If
-0001ed50: 2079 6f75 2772 6520 696e 2074 6865 2027   you're in the '
-0001ed60: 6261 7368 2720 7368 656c 6c2c 2074 6865  bash' shell, the
-0001ed70: 2072 6573 756c 7469 6e67 2073 6372 6970   resulting scrip
-0001ed80: 7420 6361 6e20 6265 2072 756e 2069 6e0a  t can be run in.
-0001ed90: 2020 2020 7468 6520 6261 636b 6772 6f75      the backgrou
-0001eda0: 6e64 2077 6974 682c 2061 7373 756d 696e  nd with, assumin
-0001edb0: 6720 7468 6520 7363 7269 7074 206e 616d  g the script nam
-0001edc0: 6520 6973 2027 646f 7275 6e73 2e73 6827  e is 'doruns.sh'
-0001edd0: 3a3a 0a0a 2020 2020 2020 206e 6f68 7570  ::..       nohup
-0001ede0: 202e 2f64 6f72 756e 732e 7368 203e 2064   ./doruns.sh > d
-0001edf0: 6f72 756e 732e 6c6f 6720 323e 2631 2026  oruns.log 2>&1 &
-0001ee00: 0a0a 2020 2020 4578 616d 706c 6520 7573  ..    Example us
-0001ee10: 6167 653a 3a0a 0a20 2020 2020 2020 2066  age::..        f
-0001ee20: 726f 6d20 7079 7965 7469 2069 6d70 6f72  rom pyyeti impor
-0001ee30: 7420 6e61 7374 7261 6e0a 2020 2020 2020  t nastran.      
-0001ee40: 2020 6e61 7374 7261 6e2e 6d6b 6e61 7374    nastran.mknast
-0001ee50: 2827 646f 7275 6e73 2e73 6827 2c20 6669  ('doruns.sh', fi
-0001ee60: 6c65 733d 5b27 6669 6c65 312e 6461 7427  les=['file1.dat'
-0001ee70: 2c20 2766 696c 6532 2e64 6174 275d 290a  , 'file2.dat']).
-0001ee80: 2020 2020 2222 220a 2020 2020 2320 4e61      """.    # Na
-0001ee90: 6d65 206f 6620 7363 7269 7074 2074 6f20  me of script to 
-0001eea0: 6372 6561 7465 3a0a 2020 2020 6966 2073  create:.    if s
-0001eeb0: 6372 6970 7420 6973 204e 6f6e 653a 0a20  cript is None:. 
-0001eec0: 2020 2020 2020 2073 6372 6970 7420 3d20         script = 
-0001eed0: 696e 7075 7428 224e 616d 6520 6f66 2073  input("Name of s
-0001eee0: 6865 6c6c 2073 6372 6970 7420 746f 2063  hell script to c
-0001eef0: 7265 6174 6520 2864 6f72 756e 732e 7368  reate (doruns.sh
-0001ef00: 293a 2022 290a 2020 2020 2020 2020 6966  ): ").        if
-0001ef10: 206e 6f74 2073 6372 6970 743a 0a20 2020   not script:.   
-0001ef20: 2020 2020 2020 2020 2073 6372 6970 7420           script 
-0001ef30: 3d20 2264 6f72 756e 732e 7368 220a 0a20  = "doruns.sh".. 
-0001ef40: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
-0001ef50: 7368 656c 6c20 7363 7269 7074 0a20 2020  shell script.   
-0001ef60: 2047 5245 5020 3d20 2267 7265 7020 2d6c   GREP = "grep -l
-0001ef70: 2027 5b2a 5e5d 5b2a 5e5d 5b2a 5e5d 2e2a   '[*^][*^][*^].*
-0001ef80: 4641 5441 4c27 220a 2020 2020 7769 7468  FATAL'".    with
-0001ef90: 206f 7065 6e28 7363 7269 7074 2c20 2277   open(script, "w
-0001efa0: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
-0001efb0: 2066 2e77 7269 7465 2866 2223 217b 7368   f.write(f"#!{sh
-0001efc0: 656c 6c7d 5c6e 2229 0a20 2020 2020 2020  ell}\n").       
-0001efd0: 2063 7572 6469 7220 3d20 6f73 2e67 6574   curdir = os.get
-0001efe0: 6377 6428 290a 2020 2020 2020 2020 662e  cwd().        f.
-0001eff0: 7772 6974 6528 6622 6364 207b 6375 7264  write(f"cd {curd
-0001f000: 6972 7d5c 6e5c 6e22 290a 2020 2020 2020  ir}\n\n").      
-0001f010: 2020 6966 2074 6f70 3a0a 2020 2020 2020    if top:.      
-0001f020: 2020 2020 2020 662e 7772 6974 6528 6622        f.write(f"
-0001f030: 7b74 6f70 7d5c 6e22 290a 0a20 2020 2020  {top}\n")..     
-0001f040: 2020 2069 203d 202d 310a 2020 2020 2020     i = -1.      
-0001f050: 2020 7768 696c 6520 313a 2020 2320 6c6f    while 1:  # lo
-0001f060: 6f70 206f 7665 7220 6669 6c65 206e 616d  op over file nam
-0001f070: 6573 0a20 2020 2020 2020 2020 2020 2069  es.            i
-0001f080: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-0001f090: 2020 6966 2066 696c 6573 2069 7320 6e6f    if files is no
-0001f0a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0001f0b0: 2020 2020 2020 2020 6966 2069 203e 3d20          if i >= 
-0001f0c0: 6c65 6e28 6669 6c65 7329 3a0a 2020 2020  len(files):.    
-0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0e0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-0001f0f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f110: 6e61 7366 696c 6520 3d20 6669 6c65 735b  nasfile = files[
-0001f120: 695d 0a20 2020 2020 2020 2020 2020 2065  i].            e
-0001f130: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001f140: 2020 2020 2070 203d 2066 2246 696c 6520       p = f"File 
-0001f150: 237b 6920 2b20 313a 3264 7d20 2862 6c61  #{i + 1:2d} (bla
-0001f160: 6e6b 2074 6f20 7175 6974 293a 2022 0a20  nk to quit): ". 
-0001f170: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0001f180: 6173 6669 6c65 203d 2069 6e70 7574 2870  asfile = input(p
-0001f190: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001f1a0: 2020 6966 206e 6f74 206e 6173 6669 6c65    if not nasfile
-0001f1b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001f1c0: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
-0001f1d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0001f1e0: 6f73 2e70 6174 682e 6578 6973 7473 286e  os.path.exists(n
-0001f1f0: 6173 6669 6c65 293a 0a20 2020 2020 2020  asfile):.       
-0001f200: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-0001f210: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-0001f220: 2020 2020 2020 2020 2020 2020 6622 6669              f"fi
-0001f230: 6c65 2027 7b6e 6173 6669 6c65 7d27 206e  le '{nasfile}' n
-0001f240: 6f74 2066 6f75 6e64 222c 2052 756e 7469  ot found", Runti
-0001f250: 6d65 5761 726e 696e 672c 0a20 2020 2020  meWarning,.     
-0001f260: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0001f270: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-0001f280: 6528 6622 5c6e 2320 2a2a 2a2a 2a2a 2a2a  e(f"\n# ********
-0001f290: 2046 696c 6520 7b6e 6173 6669 6c65 7d20   File {nasfile} 
-0001f2a0: 2a2a 2a2a 2a2a 2a2a 5c6e 2229 0a20 2020  ********\n").   
-0001f2b0: 2020 2020 2020 2020 2070 203d 206e 6173           p = nas
-0001f2c0: 6669 6c65 2e72 6669 6e64 2822 2f22 290a  file.rfind("/").
-0001f2d0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-0001f2e0: 203e 202d 313a 0a20 2020 2020 2020 2020   > -1:.         
-0001f2f0: 2020 2020 2020 2066 696c 6570 6174 6820         filepath 
-0001f300: 3d20 6e61 7366 696c 655b 3a70 5d0a 2020  = nasfile[:p].  
-0001f310: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0001f320: 6c65 6e61 6d65 203d 206e 6173 6669 6c65  lename = nasfile
-0001f330: 5b70 202b 2031 203a 5d0a 2020 2020 2020  [p + 1 :].      
-0001f340: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-0001f350: 6528 6622 2020 6364 207b 6669 6c65 7061  e(f"  cd {filepa
-0001f360: 7468 7d5c 6e22 290a 2020 2020 2020 2020  th}\n").        
-0001f370: 2020 2020 2020 2020 646f 6364 203d 2031          docd = 1
-0001f380: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001f390: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001f3a0: 2020 2066 696c 656e 616d 6520 3d20 6e61     filename = na
-0001f3b0: 7366 696c 650a 2020 2020 2020 2020 2020  sfile.          
-0001f3c0: 2020 2020 2020 646f 6364 203d 2030 0a0a        docd = 0..
-0001f3d0: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0001f3e0: 6566 6f72 653a 0a20 2020 2020 2020 2020  efore:.         
-0001f3f0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
-0001f400: 227b 6265 666f 7265 7d5c 6e22 290a 2020  "{before}\n").  
-0001f410: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-0001f420: 6528 6622 2020 7b6e 6173 636f 6d7d 2027  e(f"  {nascom} '
-0001f430: 7b6e 6173 6f70 747d 2720 277b 6669 6c65  {nasopt}' '{file
-0001f440: 6e61 6d65 7d27 5c6e 2229 0a0a 2020 2020  name}'\n")..    
-0001f450: 2020 2020 2020 2020 6966 2073 746f 706f          if stopo
-0001f460: 6e66 6174 616c 3a0a 2020 2020 2020 2020  nfatal:.        
-0001f470: 2020 2020 2020 2020 7020 3d20 6669 6c65          p = file
-0001f480: 6e61 6d65 2e72 6669 6e64 2822 2e22 290a  name.rfind(".").
-0001f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f4a0: 6966 2070 203e 202d 313a 0a20 2020 2020  if p > -1:.     
-0001f4b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001f4c0: 3036 6669 6c65 203d 2066 696c 656e 616d  06file = filenam
-0001f4d0: 655b 3a20 7020 2b20 315d 202b 2065 7874  e[: p + 1] + ext
-0001f4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f4f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001f500: 2020 2020 2020 2020 2020 2066 3036 6669             f06fi
-0001f510: 6c65 203d 2066 696c 656e 616d 6520 2b20  le = filename + 
-0001f520: 222e 2220 2b20 6578 740a 0a20 2020 2020  "." + ext..     
-0001f530: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-0001f540: 7465 2866 2220 2069 6620 5b20 5820 213d  te(f"  if [ X !=
-0001f550: 2058 607b 4752 4550 7d20 7b66 3036 6669   X`{GREP} {f06fi
-0001f560: 6c65 7d60 205d 203b 2074 6865 6e5c 6e22  le}` ] ; then\n"
-0001f570: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001f580: 2020 662e 7772 6974 6528 2220 2020 2065    f.write("    e
-0001f590: 7869 745c 6e22 290a 2020 2020 2020 2020  xit\n").        
-0001f5a0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001f5b0: 2220 2066 695c 6e22 290a 2020 2020 2020  "  fi\n").      
-0001f5c0: 2020 2020 2020 6966 2061 6674 6572 3a0a        if after:.
-0001f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f5e0: 662e 7772 6974 6528 6622 7b61 6674 6572  f.write(f"{after
-0001f5f0: 7d5c 6e22 290a 0a20 2020 2020 2020 2020  }\n")..         
-0001f600: 2020 2069 6620 646f 6364 3a0a 2020 2020     if docd:.    
-0001f610: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-0001f620: 6974 6528 6622 2020 6364 207b 6375 7264  ite(f"  cd {curd
-0001f630: 6972 7d5c 6e22 290a 0a20 2020 2020 2020  ir}\n")..       
-0001f640: 2069 6620 626f 7474 6f6d 3a0a 2020 2020   if bottom:.    
-0001f650: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-0001f660: 6622 7b62 6f74 746f 6d7d 5c6e 2229 0a20  f"{bottom}\n"). 
-0001f670: 2020 206f 732e 7379 7374 656d 2866 2263     os.system(f"c
-0001f680: 686d 6f64 2061 2b72 7820 277b 7363 7269  hmod a+rx '{scri
-0001f690: 7074 7d27 2229 0a0a 0a64 6566 2072 6464  pt}'")...def rdd
-0001f6a0: 7469 7063 6828 662c 206e 616d 653d 2254  tipch(f, name="T
-0001f6b0: 5547 3122 293a 0a20 2020 2022 2222 0a20  UG1"):.    """. 
-0001f6c0: 2020 2052 6561 6420 7468 6520 326e 6420     Read the 2nd 
-0001f6d0: 7265 636f 7264 206f 6620 7370 6563 6966  record of specif
-0001f6e0: 6963 2044 5449 7320 6672 6f6d 2061 202e  ic DTIs from a .
-0001f6f0: 7063 6820 6669 6c65 2e0a 0a20 2020 2050  pch file...    P
-0001f700: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0001f710: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 203a  --------.    f :
-0001f720: 2073 7472 696e 6720 6f72 2066 696c 655f   string or file_
-0001f730: 6c69 6b65 206f 7220 4e6f 6e65 0a20 2020  like or None.   
-0001f740: 2020 2020 2045 6974 6865 7220 6120 6e61       Either a na
-0001f750: 6d65 206f 6620 6120 6669 6c65 2c20 6f72  me of a file, or
-0001f760: 2069 7320 6120 6669 6c65 5f6c 696b 6520   is a file_like 
-0001f770: 6f62 6a65 6374 2061 7320 7265 7475 726e  object as return
-0001f780: 6564 0a20 2020 2020 2020 2062 7920 3a66  ed.        by :f
-0001f790: 756e 633a 606f 7065 6e60 2e20 4966 2066  unc:`open`. If f
-0001f7a0: 696c 655f 6c69 6b65 206f 626a 6563 742c  ile_like object,
-0001f7b0: 2069 7420 6973 2072 6577 6f75 6e64 2066   it is rewound f
-0001f7c0: 6972 7374 2e20 4361 6e0a 2020 2020 2020  irst. Can.      
-0001f7d0: 2020 616c 736f 2062 6520 7468 6520 6e61    also be the na
-0001f7e0: 6d65 206f 6620 6120 6469 7265 6374 6f72  me of a director
-0001f7f0: 7920 6f72 204e 6f6e 653b 2069 6e20 7468  y or None; in th
-0001f800: 6573 6520 6361 7365 732c 2061 2047 5549  ese cases, a GUI
-0001f810: 0a20 2020 2020 2020 2069 7320 6f70 656e  .        is open
-0001f820: 6564 2066 6f72 2066 696c 6520 7365 6c65  ed for file sele
-0001f830: 6374 696f 6e2e 0a20 2020 206e 616d 6520  ction..    name 
-0001f840: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-0001f850: 204e 616d 6520 6f66 2044 5449 2074 6162   Name of DTI tab
-0001f860: 6c65 2074 6f20 7265 6164 2066 726f 6d20  le to read from 
-0001f870: 7468 6520 2e70 6368 2066 696c 650a 0a20  the .pch file.. 
-0001f880: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-0001f890: 2d2d 2d2d 2d2d 0a20 2020 2069 645f 646f  ------.    id_do
-0001f8a0: 6620 3a20 6e64 6172 7261 790a 2020 2020  f : ndarray.    
-0001f8b0: 2020 2020 322d 636f 6c75 6d6e 206d 6174      2-column mat
-0001f8c0: 7269 7820 6f66 2074 6865 2066 6f72 6d3a  rix of the form:
-0001f8d0: 2060 605b 6964 2c20 646f 665d 6060 2e20   ``[id, dof]``. 
-0001f8e0: 5468 6520 6e75 6d62 6572 206f 6620 726f  The number of ro
-0001f8f0: 7773 0a20 2020 2020 2020 2069 6e20 6069  ws.        in `i
-0001f900: 645f 646f 6660 2063 6f72 7265 7370 6f6e  d_dof` correspon
-0001f910: 6473 2074 6f20 7468 6520 6d61 7463 6869  ds to the matchi
-0001f920: 6e67 206d 6174 7269 7820 696e 202e 6f70  ng matrix in .op
-0001f930: 3420 6669 6c65 0a20 2020 2020 2020 2028  4 file.        (
-0001f940: 7365 6520 4e6f 7465 7329 2e0a 0a20 2020  see Notes)...   
-0001f950: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-0001f960: 0a20 2020 2054 6869 7320 726f 7574 696e  .    This routin
-0001f970: 6520 6973 2075 7365 6675 6c20 666f 7220  e is useful for 
-0001f980: 7265 6164 696e 6720 6461 7461 2066 726f  reading data fro
-0001f990: 6d20 2e70 6368 2066 696c 6573 2077 7269  m .pch files wri
-0001f9a0: 7474 656e 2062 790a 2020 2020 7468 6520  tten by.    the 
-0001f9b0: 4558 5453 454f 5554 2063 6f6d 6d61 6e64  EXTSEOUT command
-0001f9c0: 2e20 5468 6520 326e 6420 7265 636f 7264  . The 2nd record
-0001f9d0: 206f 6620 2254 5547 3122 2028 666f 7220   of "TUG1" (for 
-0001f9e0: 6578 616d 706c 6529 0a20 2020 2063 6f6e  example).    con
-0001f9f0: 7461 696e 7320 7468 6520 444f 4620 7468  tains the DOF th
-0001fa00: 6174 2063 6f72 7265 7370 6f6e 6420 746f  at correspond to
-0001fa10: 2074 6865 2072 6f77 7320 6f66 2074 6865   the rows of the
-0001fa20: 2022 4d55 4731 2220 6d61 7472 6978 0a20   "MUG1" matrix. 
-0001fa30: 2020 2069 6e20 7468 6520 2e6f 7034 2066     in the .op4 f
-0001fa40: 696c 652e 2054 6861 7420 6d61 7472 6978  ile. That matrix
-0001fa50: 2063 616e 2062 6520 7265 6164 2062 7920   can be read by 
-0001fa60: 7468 650a 2020 2020 3a6d 6f64 3a60 7079  the.    :mod:`py
-0001fa70: 7965 7469 2e6e 6173 7472 616e 2e6f 7034  yeti.nastran.op4
-0001fa80: 6020 6d6f 6475 6c65 2e0a 0a20 2020 2045  ` module...    E
-0001fa90: 7861 6d70 6c65 2075 7361 6765 3a3a 0a0a  xample usage::..
-0001faa0: 2020 2020 2020 2020 2320 7265 6164 206d          # read m
-0001fab0: 7567 3120 616e 6420 7475 6731 2028 6372  ug1 and tug1 (cr
-0001fac0: 6561 7465 6420 6672 6f6d 2045 5854 5345  eated from EXTSE
-0001fad0: 4f55 5429 3a0a 2020 2020 2020 2020 6672  OUT):.        fr
-0001fae0: 6f6d 2070 7979 6574 6920 696d 706f 7274  om pyyeti import
-0001faf0: 206e 6173 7472 616e 0a20 2020 2020 2020   nastran.       
-0001fb00: 2066 726f 6d20 7079 7965 7469 2e6e 6173   from pyyeti.nas
-0001fb10: 7472 616e 2069 6d70 6f72 7420 6f70 340a  tran import op4.
-0001fb20: 2020 2020 2020 2020 6d75 6731 203d 206f          mug1 = o
-0001fb30: 7034 2e72 6561 6428 2764 6174 612e 6f70  p4.read('data.op
-0001fb40: 3427 2c20 276d 7567 3127 295b 276d 7567  4', 'mug1')['mug
-0001fb50: 3127 5d0a 2020 2020 2020 2020 7475 6731  1'].        tug1
-0001fb60: 203d 206e 6173 7472 616e 2e72 6464 7469   = nastran.rddti
-0001fb70: 7063 6828 2764 6174 612e 7063 6827 290a  pch('data.pch').
-0001fb80: 0a20 2020 2020 2020 2023 2066 6f72 6d20  .        # form 
-0001fb90: 4452 4d20 746f 2072 6563 6f76 6572 7920  DRM to recovery 
-0001fba0: 6772 6964 2031 3030 2c20 646f 6620 343a  grid 100, dof 4:
-0001fbb0: 0a20 2020 2020 2020 2066 726f 6d20 7079  .        from py
-0001fbc0: 7965 7469 2069 6d70 6f72 7420 6c6f 6361  yeti import loca
-0001fbd0: 7465 0a20 2020 2020 2020 2072 6f77 203d  te.        row =
-0001fbe0: 206c 6f63 6174 652e 6669 6e64 5f72 6f77   locate.find_row
-0001fbf0: 7328 7475 6731 2c20 5b31 3030 2c20 345d  s(tug1, [100, 4]
-0001fc00: 290a 2020 2020 2020 2020 6472 6d20 3d20  ).        drm = 
-0001fc10: 6d75 6731 5b72 6f77 2c20 3a5d 0a20 2020  mug1[row, :].   
-0001fc20: 2022 2222 0a20 2020 2073 7472 696e 6720   """.    string 
-0001fc30: 3d20 6622 4454 4920 2020 2020 7b6e 616d  = f"DTI     {nam
-0001fc40: 653a 3c38 737d 3222 0a20 2020 2063 203d  e:<8s}2".    c =
-0001fc50: 2072 6463 6172 6473 2866 2c20 7374 7269   rdcards(f, stri
-0001fc60: 6e67 290a 2020 2020 6320 3d20 635b 302c  ng).    c = c[0,
-0001fc70: 2031 363a 2d31 5d2e 7265 7368 6170 6528   16:-1].reshape(
-0001fc80: 2d31 2c20 3429 2e61 7374 7970 6528 6e70  -1, 4).astype(np
-0001fc90: 2e69 6e74 3634 290a 2020 2020 6d20 3d20  .int64).    m = 
-0001fca0: 635b 3a2c 2031 3a5d 0a0a 2020 2020 2320  c[:, 1:]..    # 
-0001fcb0: 6172 7261 7928 5b5b 2020 2020 2020 332c  array([[      3,
-0001fcc0: 2020 2020 2020 2036 2c20 2020 2020 2020         6,       
-0001fcd0: 315d 2c0a 2020 2020 2320 2020 2020 2020  1],.    #       
-0001fce0: 205b 2020 2020 2031 312c 2020 2020 2020   [     11,      
-0001fcf0: 2036 2c20 2020 2020 2020 375d 2c0a 2020   6,       7],.  
-0001fd00: 2020 2320 2020 2020 2020 205b 2020 2020    #        [    
-0001fd10: 2031 392c 2020 2020 2020 2036 2c20 2020   19,       6,   
-0001fd20: 2020 2031 335d 2c0a 2020 2020 2320 2020     13],.    #   
-0001fd30: 2020 2020 205b 2020 2020 2032 372c 2020       [     27,  
-0001fd40: 2020 2020 2036 2c20 2020 2020 2031 395d       6,      19]
-0001fd50: 2c0a 2020 2020 2320 2020 2020 2020 205b  ,.    #        [
-0001fd60: 2020 2020 2034 352c 2020 2020 2020 2036       45,       6
-0001fd70: 2c20 2020 2020 2032 355d 2c0a 2020 2020  ,      25],.    
-0001fd80: 2320 2020 2020 2020 205b 2020 2020 2036  #        [     6
-0001fd90: 302c 2020 2020 2020 2036 2c20 2020 2020  0,       6,     
-0001fda0: 2033 315d 2c0a 2020 2020 2320 2020 2020   31],.    #     
-0001fdb0: 2020 205b 3139 3935 3030 322c 2020 2020     [1995002,    
-0001fdc0: 2020 2036 2c20 2020 2020 2033 375d 5d29     6,      37]])
-0001fdd0: 0a0a 2020 2020 6966 206e 702e 616c 6c28  ..    if np.all(
-0001fde0: 6d5b 3a2c 2031 5d20 3d3d 206d 5b30 2c20  m[:, 1] == m[0, 
-0001fdf0: 315d 293a 0a20 2020 2020 2020 2023 2061  1]):.        # a
-0001fe00: 6c6c 2069 6473 2068 6176 6520 7361 6d65  ll ids have same
-0001fe10: 206e 756d 6265 7220 6f66 2063 6f6d 706f   number of compo
-0001fe20: 6e65 6e74 732c 2073 6f20 7461 6b65 2073  nents, so take s
-0001fe30: 686f 7274 6375 743a 0a20 2020 2020 2020  hortcut:.       
-0001fe40: 2063 203d 206d 5b30 2c20 315d 0a20 2020   c = m[0, 1].   
-0001fe50: 2020 2020 2069 6473 203d 206e 702e 646f       ids = np.do
-0001fe60: 7428 6d5b 3a2c 2030 3a31 5d2c 206e 702e  t(m[:, 0:1], np.
-0001fe70: 6f6e 6573 2828 312c 2063 292c 206e 702e  ones((1, c), np.
-0001fe80: 696e 7436 3429 290a 2020 2020 2020 2020  int64)).        
-0001fe90: 6964 7320 3d20 6964 732e 7265 7368 6170  ids = ids.reshap
-0001fea0: 6528 282d 312c 2031 2929 0a20 2020 2020  e((-1, 1)).     
-0001feb0: 2020 2064 6f66 203d 206e 702e 6172 616e     dof = np.aran
-0001fec0: 6765 2831 2c20 6320 2b20 312c 2064 7479  ge(1, c + 1, dty
-0001fed0: 7065 3d6e 702e 696e 7436 3429 2e72 6573  pe=np.int64).res
-0001fee0: 6861 7065 2831 2c20 2d31 290a 2020 2020  hape(1, -1).    
-0001fef0: 2020 2020 646f 6673 203d 206e 702e 646f      dofs = np.do
-0001ff00: 7428 6e70 2e6f 6e65 7328 286e 702e 7369  t(np.ones((np.si
-0001ff10: 7a65 286d 2c20 3029 2c20 3129 2c20 6e70  ze(m, 0), 1), np
-0001ff20: 2e69 6e74 3634 292c 2064 6f66 290a 2020  .int64), dof).  
-0001ff30: 2020 2020 2020 646f 6673 203d 2064 6f66        dofs = dof
-0001ff40: 732e 7265 7368 6170 6528 282d 312c 2031  s.reshape((-1, 1
-0001ff50: 2929 0a20 2020 2020 2020 2069 6464 6f66  )).        iddof
-0001ff60: 203d 206e 702e 6873 7461 636b 2828 6964   = np.hstack((id
-0001ff70: 732c 2064 6f66 7329 290a 2020 2020 656c  s, dofs)).    el
-0001ff80: 7365 3a0a 2020 2020 2020 2020 6e72 6f77  se:.        nrow
-0001ff90: 7320 3d20 6d5b 2d31 2c20 325d 202b 206d  s = m[-1, 2] + m
-0001ffa0: 5b2d 312c 2031 5d20 2d20 310a 2020 2020  [-1, 1] - 1.    
-0001ffb0: 2020 2020 6964 646f 6620 3d20 6e70 2e7a      iddof = np.z
-0001ffc0: 6572 6f73 2828 6e72 6f77 732c 2032 292c  eros((nrows, 2),
-0001ffd0: 206e 702e 696e 7436 3429 0a20 2020 2020   np.int64).     
-0001ffe0: 2020 206a 203d 2030 0a20 2020 2020 2020     j = 0.       
-0001fff0: 2066 6f72 204a 2069 6e20 7261 6e67 6528   for J in range(
-00020000: 6e70 2e73 697a 6528 6d2c 2030 2929 3a0a  np.size(m, 0)):.
-00020010: 2020 2020 2020 2020 2020 2020 7076 203d              pv =
-00020020: 206e 702e 6172 616e 6765 2830 2c20 6d5b   np.arange(0, m[
-00020030: 4a2c 2031 5d2c 2064 7479 7065 3d6e 702e  J, 1], dtype=np.
-00020040: 696e 7436 3429 0a20 2020 2020 2020 2020  int64).         
-00020050: 2020 2069 6464 6f66 5b70 7620 2b20 6a2c     iddof[pv + j,
-00020060: 2030 5d20 3d20 6d5b 4a2c 2030 5d0a 2020   0] = m[J, 0].  
-00020070: 2020 2020 2020 2020 2020 6964 646f 665b            iddof[
-00020080: 7076 202b 206a 2c20 315d 203d 2070 7620  pv + j, 1] = pv 
-00020090: 2b20 310a 2020 2020 2020 2020 2020 2020  + 1.            
-000200a0: 6a20 2b3d 206d 5b4a 2c20 315d 0a20 2020  j += m[J, 1].   
-000200b0: 2072 6574 7572 6e20 6964 646f 660a        return iddof.
+00010dc0: 2020 2020 454e 4444 4154 4122 293a 0a20      ENDDATA"):. 
+00010dd0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00010de0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+00010df0: 206d 203d 2070 726f 672e 6d61 7463 6828   m = prog.match(
+00010e00: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
+00010e10: 2020 6966 206d 3a0a 2020 2020 2020 2020    if m:.        
+00010e20: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
+00010e30: 6d2e 6772 6f75 7028 3129 2e73 7472 6970  m.group(1).strip
+00010e40: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00010e50: 2020 2069 6620 6d61 7463 685b 305d 203d     if match[0] =
+00010e60: 3d20 222b 2220 6f72 206d 6174 6368 5b30  = "+" or match[0
+00010e70: 5d20 3d3d 2022 2a22 3a0a 2020 2020 2020  ] == "*":.      
+00010e80: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010e90: 206c 656e 286d 6174 6368 2920 3e20 383a   len(match) > 8:
+00010ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010eb0: 2020 2020 2020 2020 206d 6174 6368 203d           match =
+00010ec0: 206d 6174 6368 5b30 5d20 2b20 2220 2020   match[0] + "   
+00010ed0: 2020 2020 2220 2b20 6d61 7463 685b 383a      " + match[8:
+00010ee0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00010ef0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 2020 2020 6d61 7463 6820 3d20 6d61 7463      match = matc
+00010f20: 685b 305d 0a20 2020 2020 2020 2020 2020  h[0].           
+00010f30: 2020 2020 2073 2e61 7070 656e 6428 6d61       s.append(ma
+00010f40: 7463 6829 0a20 2020 2020 2020 2072 6574  tch).        ret
+00010f50: 7572 6e20 225c 6e22 2e6a 6f69 6e28 7329  urn "\n".join(s)
+00010f60: 202b 2022 5c6e 220a 0a20 2020 2040 6775   + "\n"..    @gu
+00010f70: 6974 6f6f 6c73 2e77 7269 7465 5f74 6578  itools.write_tex
+00010f80: 745f 6669 6c65 0a20 2020 2064 6566 205f  t_file.    def _
+00010f90: 7774 6275 6c6b 2866 2c20 626c 6b29 3a0a  wtbulk(f, blk):.
+00010fa0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00010fb0: 626c 6b29 0a0a 2020 2020 5f77 7462 756c  blk)..    _wtbul
+00010fc0: 6b28 666f 7574 2c20 5f72 6462 756c 6b28  k(fout, _rdbulk(
+00010fd0: 6669 6e29 290a 0a0a 4067 7569 746f 6f6c  fin))...@guitool
+00010fe0: 732e 7265 6164 5f74 6578 745f 6669 6c65  s.read_text_file
+00010ff0: 0a64 6566 2072 6465 6967 656e 2866 2c20  .def rdeigen(f, 
+00011000: 7573 655f 7061 6e64 6173 3d54 7275 6529  use_pandas=True)
+00011010: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+00011020: 6164 2065 6967 656e 7661 6c75 6520 7461  ad eigenvalue ta
+00011030: 626c 6573 2066 726f 6d20 6120 4e61 7374  bles from a Nast
+00011040: 7261 6e20 6630 3620 6669 6c65 2e0a 0a20  ran f06 file... 
+00011050: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00011060: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00011070: 2066 203a 2073 7472 696e 6720 6f72 2066   f : string or f
+00011080: 696c 655f 6c69 6b65 206f 7220 4e6f 6e65  ile_like or None
+00011090: 0a20 2020 2020 2020 2045 6974 6865 7220  .        Either 
+000110a0: 6120 6e61 6d65 206f 6620 6120 6669 6c65  a name of a file
+000110b0: 2c20 6f72 2069 7320 6120 6669 6c65 5f6c  , or is a file_l
+000110c0: 696b 6520 6f62 6a65 6374 2061 7320 7265  ike object as re
+000110d0: 7475 726e 6564 0a20 2020 2020 2020 2062  turned.        b
+000110e0: 7920 3a66 756e 633a 606f 7065 6e60 2e20  y :func:`open`. 
+000110f0: 4966 2066 696c 655f 6c69 6b65 206f 626a  If file_like obj
+00011100: 6563 742c 2069 7420 6973 2072 6577 6f75  ect, it is rewou
+00011110: 6e64 2066 6972 7374 2e20 4361 6e0a 2020  nd first. Can.  
+00011120: 2020 2020 2020 616c 736f 2062 6520 7468        also be th
+00011130: 6520 6e61 6d65 206f 6620 6120 6469 7265  e name of a dire
+00011140: 6374 6f72 7920 6f72 204e 6f6e 653b 2069  ctory or None; i
+00011150: 6e20 7468 6573 6520 6361 7365 732c 2061  n these cases, a
+00011160: 2047 5549 0a20 2020 2020 2020 2069 7320   GUI.        is 
+00011170: 6f70 656e 6564 2066 6f72 2066 696c 6520  opened for file 
+00011180: 7365 6c65 6374 696f 6e2e 0a20 2020 2075  selection..    u
+00011190: 7365 5f70 616e 6461 7320 3a20 626f 6f6c  se_pandas : bool
+000111a0: 3b20 6f70 7469 6f6e 616c 0a20 2020 2020  ; optional.     
+000111b0: 2020 2049 6620 5472 7565 2c20 7468 6520     If True, the 
+000111c0: 7661 6c75 6573 2072 6574 7572 6e65 6420  values returned 
+000111d0: 696e 2074 6865 2064 6963 7469 6f6e 6172  in the dictionar
+000111e0: 7920 7769 6c6c 2062 6520 7061 6e64 6173  y will be pandas
+000111f0: 0a20 2020 2020 2020 2044 6174 6146 7261  .        DataFra
+00011200: 6d65 730a 0a20 2020 2052 6574 7572 6e73  mes..    Returns
+00011210: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00011220: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
+00011230: 2020 2020 5468 6520 6b65 7973 2061 7265      The keys are
+00011240: 2074 6865 2073 7570 6572 656c 656d 656e   the superelemen
+00011250: 7420 4944 7320 616e 6420 7468 6520 7661  t IDs and the va
+00011260: 6c75 6573 2069 7320 7468 6520 370a 2020  lues is the 7.  
+00011270: 2020 2020 2020 636f 6c75 6d6e 2065 6967        column eig
+00011280: 656e 7661 6c75 6520 7461 626c 653a 205b  envalue table: [
+00011290: 6d6f 6465 206e 756d 6265 722c 2065 7874  mode number, ext
+000112a0: 7261 6374 696f 6e20 6f72 6465 722c 0a20  raction order,. 
+000112b0: 2020 2020 2020 2065 6967 656e 7661 6c75         eigenvalu
+000112c0: 652c 2072 6164 6961 6e73 2c20 6379 636c  e, radians, cycl
+000112d0: 6573 2c20 6765 6e65 7261 6c69 7a65 6420  es, generalized 
+000112e0: 6d61 7373 2c20 6765 6e65 7261 6c69 7a65  mass, generalize
+000112f0: 640a 2020 2020 2020 2020 7374 6966 666e  d.        stiffn
+00011300: 6573 735d 0a0a 2020 2020 4e6f 7465 730a  ess]..    Notes.
+00011310: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
+00011320: 6520 6c61 7374 2074 6162 6c65 2072 6561  e last table rea
+00011330: 6420 666f 7220 6120 7375 7065 7265 6c65  d for a superele
+00011340: 6d65 6e74 2072 6570 6c61 6365 7320 7461  ment replaces ta
+00011350: 626c 6573 2070 7265 7669 6f75 736c 790a  bles previously.
+00011360: 2020 2020 7265 6164 2069 6e2e 0a0a 2020      read in...  
+00011370: 2020 4966 2074 6865 2070 616e 6461 7320    If the pandas 
+00011380: 6f75 7470 7574 2069 7320 6368 6f73 656e  output is chosen
+00011390: 2028 7468 6520 6465 6661 756c 7429 2074   (the default) t
+000113a0: 6865 206d 6f64 6520 6e75 6d62 6572 2069  he mode number i
+000113b0: 730a 2020 2020 7573 6564 2061 7320 7468  s.    used as th
+000113c0: 6520 6069 6e64 6578 6020 616e 6420 6063  e `index` and `c
+000113d0: 6f6c 756d 6e73 6020 6973 3a3a 0a0a 2020  olumns` is::..  
+000113e0: 2020 2020 2020 6320 3d20 5b27 4d6f 6465        c = ['Mode
+000113f0: 2023 272c 2027 6578 7420 2327 2c20 2765   #', 'ext #', 'e
+00011400: 6967 656e 7661 6c75 6527 2c20 2772 6164  igenvalue', 'rad
+00011410: 6961 6e73 272c 0a20 2020 2020 2020 2020  ians',.         
+00011420: 2020 2020 2763 7963 6c65 7327 2c20 2767      'cycles', 'g
+00011430: 656e 6d61 7373 272c 2027 6765 6e73 7469  enmass', 'gensti
+00011440: 6627 5d0a 2020 2020 2222 220a 0a20 2020  f'].    """..   
+00011450: 2064 6566 205f 6669 6e64 5f65 6967 656e   def _find_eigen
+00011460: 2866 293a 0a20 2020 2020 2020 2053 4520  (f):.        SE 
+00011470: 3d20 2253 5550 4552 454c 454d 454e 5420  = "SUPERELEMENT 
+00011480: 220a 2020 2020 2020 2020 4549 4720 3d20  ".        EIG = 
+00011490: 2252 2045 2041 204c 2020 2045 2049 2047  "R E A L   E I G
+000114a0: 2045 204e 2056 2041 204c 2055 2045 2053   E N V A L U E S
+000114b0: 220a 2020 2020 2020 2020 7365 203d 2030  ".        se = 0
+000114c0: 0a20 2020 2020 2020 2066 6f72 206c 696e  .        for lin
+000114d0: 6520 696e 2066 3a0a 2020 2020 2020 2020  e in f:.        
+000114e0: 2020 2020 6966 206c 656e 286c 696e 6529      if len(line)
+000114f0: 203e 2031 3136 2061 6e64 206c 696e 655b   > 116 and line[
+00011500: 3130 343a 5d2e 7374 6172 7473 7769 7468  104:].startswith
+00011510: 2853 4529 3a0a 2020 2020 2020 2020 2020  (SE):.          
+00011520: 2020 2020 2020 7365 203d 2069 6e74 286c        se = int(l
+00011530: 696e 655b 3131 363a 5d29 0a20 2020 2020  ine[116:]).     
+00011540: 2020 2020 2020 2069 6620 6c65 6e28 6c69         if len(li
+00011550: 6e65 2920 3e20 3736 2061 6e64 206c 696e  ne) > 76 and lin
+00011560: 655b 3436 3a5d 2e73 7461 7274 7377 6974  e[46:].startswit
+00011570: 6828 4549 4729 3a0a 2020 2020 2020 2020  h(EIG):.        
+00011580: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011590: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+000115a0: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
+000115b0: 7264 5f65 6967 656e 5f74 6162 6c65 2866  rd_eigen_table(f
+000115c0: 293a 0a20 2020 2020 2020 2022 2222 4569  ):.        """Ei
+000115d0: 6765 6e76 616c 7565 2074 6162 6c65 2066  genvalue table f
+000115e0: 6f75 6e64 2c20 7265 6164 2069 742e 2222  ound, read it.""
+000115f0: 220a 2020 2020 2020 2020 666f 7220 6c69  ".        for li
+00011600: 6e65 2069 6e20 663a 0a20 2020 2020 2020  ne in f:.       
+00011610: 2020 2020 2069 6620 6c69 6e65 2e73 7461       if line.sta
+00011620: 7274 7377 6974 6828 2220 2020 204e 4f2e  rtswith("    NO.
+00011630: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00011640: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00011650: 2020 7461 626c 6520 3d20 5b5d 0a20 2020    table = [].   
+00011660: 2020 2020 2063 6f6e 7469 6e75 6564 203d       continued =
+00011670: 2054 7275 650a 2020 2020 2020 2020 7768   True.        wh
+00011680: 696c 6520 636f 6e74 696e 7565 643a 0a20  ile continued:. 
+00011690: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
+000116a0: 696e 6520 696e 2066 3a0a 2020 2020 2020  ine in f:.      
+000116b0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116d0: 2020 2072 6f77 203d 205b 666c 6f61 7428     row = [float(
+000116e0: 6929 2066 6f72 2069 2069 6e20 6c69 6e65  i) for i in line
+000116f0: 2e73 706c 6974 2829 5d0a 2020 2020 2020  .split()].      
+00011700: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00011710: 2056 616c 7565 4572 726f 723a 0a20 2020   ValueError:.   
+00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011730: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+00011740: 2020 2020 2020 2069 6620 6c65 6e28 726f         if len(ro
+00011750: 7729 203d 3d20 373a 0a20 2020 2020 2020  w) == 7:.       
+00011760: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+00011770: 6c65 2e61 7070 656e 6428 726f 7729 0a20  le.append(row). 
+00011780: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
+00011790: 2069 6e20 7261 6e67 6528 3829 3a0a 2020   in range(8):.  
+000117a0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+000117b0: 6e65 203d 2066 2e72 6561 646c 696e 6528  ne = f.readline(
+000117c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000117d0: 2020 6966 206c 696e 652e 7374 6172 7473    if line.starts
+000117e0: 7769 7468 2822 3120 2229 3a0a 2020 2020  with("1 "):.    
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 636f 6e74 696e 7565 6420 3d20 4661 6c73  continued = Fals
+00011810: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00011820: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+00011830: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00011840: 696e 652e 7374 6172 7473 7769 7468 2822  ine.startswith("
+00011850: 2020 2020 4e4f 2e22 293a 0a20 2020 2020      NO."):.     
+00011860: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00011870: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+00011880: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00011890: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+000118a0: 2020 2020 2072 6574 7572 6e20 6e70 2e61       return np.a
+000118b0: 7272 6179 2874 6162 6c65 290a 0a20 2020  rray(table)..   
+000118c0: 2064 6374 203d 207b 7d0a 2020 2020 662e   dct = {}.    f.
+000118d0: 7365 656b 2830 2c20 3029 0a20 2020 2077  seek(0, 0).    w
+000118e0: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
+000118f0: 2020 2073 6520 3d20 5f66 696e 645f 6569     se = _find_ei
+00011900: 6765 6e28 6629 0a20 2020 2020 2020 2069  gen(f).        i
+00011910: 6620 7365 2069 7320 4e6f 6e65 3a0a 2020  f se is None:.  
+00011920: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011930: 2064 6374 0a20 2020 2020 2020 2074 6162   dct.        tab
+00011940: 6c65 203d 205f 7264 5f65 6967 656e 5f74  le = _rd_eigen_t
+00011950: 6162 6c65 2866 290a 2020 2020 2020 2020  able(f).        
+00011960: 6966 2075 7365 5f70 616e 6461 733a 0a20  if use_pandas:. 
+00011970: 2020 2020 2020 2020 2020 2069 203d 2074             i = t
+00011980: 6162 6c65 5b3a 2c20 305d 2e61 7374 7970  able[:, 0].astyp
+00011990: 6528 696e 7429 0a20 2020 2020 2020 2020  e(int).         
+000119a0: 2020 2063 203d 205b 0a20 2020 2020 2020     c = [.       
+000119b0: 2020 2020 2020 2020 2022 6d6f 6465 2023           "mode #
+000119c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000119d0: 2020 2022 6578 7420 2322 2c0a 2020 2020     "ext #",.    
+000119e0: 2020 2020 2020 2020 2020 2020 2265 6967              "eig
+000119f0: 656e 7661 6c75 6522 2c0a 2020 2020 2020  envalue",.      
+00011a00: 2020 2020 2020 2020 2020 2272 6164 6961            "radia
+00011a10: 6e73 222c 0a20 2020 2020 2020 2020 2020  ns",.           
+00011a20: 2020 2020 2022 6379 636c 6573 222c 0a20       "cycles",. 
+00011a30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011a40: 6765 6e6d 6173 7322 2c0a 2020 2020 2020  genmass",.      
+00011a50: 2020 2020 2020 2020 2020 2267 656e 7374            "genst
+00011a60: 6966 222c 0a20 2020 2020 2020 2020 2020  if",.           
+00011a70: 205d 0a20 2020 2020 2020 2020 2020 2074   ].            t
+00011a80: 6162 6c65 203d 2070 642e 4461 7461 4672  able = pd.DataFr
+00011a90: 616d 6528 7461 626c 652c 2069 6e64 6578  ame(table, index
+00011aa0: 3d69 2c20 636f 6c75 6d6e 733d 6329 0a20  =i, columns=c). 
+00011ab0: 2020 2020 2020 2064 6374 5b73 655d 203d         dct[se] =
+00011ac0: 2074 6162 6c65 0a0a 0a40 6775 6974 6f6f   table...@guitoo
+00011ad0: 6c73 2e77 7269 7465 5f74 6578 745f 6669  ls.write_text_fi
+00011ae0: 6c65 0a64 6566 2077 746e 6173 696e 7473  le.def wtnasints
+00011af0: 2866 2c20 7374 6172 742c 2069 6e74 7329  (f, start, ints)
+00011b00: 3a0a 2020 2020 2222 220a 2020 2020 5574  :.    """.    Ut
+00011b10: 696c 6974 7920 726f 7574 696e 6520 666f  ility routine fo
+00011b20: 7220 7468 6520 6e61 7374 7261 6e20 2777  r the nastran 'w
+00011b30: 742a 2720 726f 7574 696e 6573 2e0a 0a20  t*' routines... 
+00011b40: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00011b50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00011b60: 2066 203a 2073 7472 696e 6720 6f72 2066   f : string or f
+00011b70: 696c 655f 6c69 6b65 206f 7220 3120 6f72  ile_like or 1 or
+00011b80: 204e 6f6e 650a 2020 2020 2020 2020 4569   None.        Ei
+00011b90: 7468 6572 2061 206e 616d 6520 6f66 2061  ther a name of a
+00011ba0: 2066 696c 652c 206f 7220 6973 2061 2066   file, or is a f
+00011bb0: 696c 655f 6c69 6b65 206f 626a 6563 7420  ile_like object 
+00011bc0: 6173 2072 6574 7572 6e65 640a 2020 2020  as returned.    
+00011bd0: 2020 2020 6279 203a 6675 6e63 3a60 6f70      by :func:`op
+00011be0: 656e 6020 6f72 203a 636c 6173 733a 6069  en` or :class:`i
+00011bf0: 6f2e 5374 7269 6e67 494f 602e 2049 6e70  o.StringIO`. Inp
+00011c00: 7574 2061 7320 696e 7465 6765 7220 3120  ut as integer 1 
+00011c10: 746f 0a20 2020 2020 2020 2077 7269 7465  to.        write
+00011c20: 2074 6f20 7374 646f 7574 2e20 4361 6e20   to stdout. Can 
+00011c30: 616c 736f 2062 6520 7468 6520 6e61 6d65  also be the name
+00011c40: 206f 6620 6120 6469 7265 6374 6f72 7920   of a directory 
+00011c50: 6f72 204e 6f6e 653b 0a20 2020 2020 2020  or None;.       
+00011c60: 2069 6e20 7468 6573 6520 6361 7365 732c   in these cases,
+00011c70: 2061 2047 5549 2069 7320 6f70 656e 6564   a GUI is opened
+00011c80: 2066 6f72 2066 696c 6520 7365 6c65 6374   for file select
+00011c90: 696f 6e2e 0a20 2020 2073 7461 7274 203a  ion..    start :
+00011ca0: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
+00011cb0: 2042 6567 696e 6e69 6e67 2066 6965 6c64   Beginning field
+00011cc0: 2066 6f72 2074 6865 2069 6e74 6567 6572   for the integer
+00011cd0: 733b 2063 6172 6420 6e61 6d65 2069 7320  s; card name is 
+00011ce0: 696e 2066 6965 6c64 2031 2c20 736f 0a20  in field 1, so. 
+00011cf0: 2020 2020 2020 2073 7461 7274 2073 686f         start sho
+00011d00: 756c 6420 6265 203e 3d20 322e 0a20 2020  uld be >= 2..   
+00011d10: 2069 6e74 7320 3a20 3164 2061 7272 6179   ints : 1d array
+00011d20: 5f6c 696b 650a 2020 2020 2020 2020 5665  _like.        Ve
+00011d30: 6374 6f72 206f 6620 696e 7465 6765 7273  ctor of integers
+00011d40: 2074 6f20 7772 6974 650a 0a20 2020 2052   to write..    R
+00011d50: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00011d60: 2d2d 0a20 2020 204e 6f6e 650a 0a20 2020  --.    None..   
+00011d70: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
+00011d80: 0a0a 2020 2020 5468 6973 2072 6f75 7469  ..    This routi
+00011d90: 6e65 2069 7320 7479 7069 6361 6c6c 7920  ne is typically 
+00011da0: 6e6f 7420 6361 6c6c 6564 2064 6972 6563  not called direc
+00011db0: 746c 792c 2062 7574 2063 6f75 6c64 2062  tly, but could b
+00011dc0: 6520 7573 6566 756c 0a20 2020 2074 6f20  e useful.    to 
+00011dd0: 7772 6974 6520 6361 7264 7320 7468 6174  write cards that
+00011de0: 2061 7265 206e 6f74 2061 6c72 6561 6479   are not already
+00011df0: 2061 6363 6f75 6e74 6564 2066 6f72 2069   accounted for i
+00011e00: 6e20 7468 6973 0a20 2020 206d 6f64 756c  n this.    modul
+00011e10: 652e 2041 7320 616e 2065 7861 6d70 6c65  e. As an example
+00011e20: 2075 7361 6765 2c20 6865 7265 2069 7320   usage, here is 
+00011e30: 7468 6520 636f 6465 2069 6e73 6964 650a  the code inside.
+00011e40: 2020 2020 3a66 756e 633a 6077 7463 7375      :func:`wtcsu
+00011e50: 7065 7260 3a3a 0a0a 2020 2020 2020 2020  per`::..        
+00011e60: 662e 7772 6974 6528 6622 4353 5550 4552  f.write(f"CSUPER
+00011e70: 2020 7b73 7570 6572 6964 3a38 647d 7b30    {superid:8d}{0
+00011e80: 3a38 647d 2229 0a20 2020 2020 2020 2077  :8d}").        w
+00011e90: 746e 6173 696e 7473 2866 2c20 342c 2067  tnasints(f, 4, g
+00011ea0: 7269 6473 290a 0a20 2020 2045 7861 6d70  rids)..    Examp
+00011eb0: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
+00011ec0: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
+00011ed0: 6e75 6d70 7920 6173 206e 700a 2020 2020  numpy as np.    
+00011ee0: 3e3e 3e20 6672 6f6d 2070 7979 6574 6920  >>> from pyyeti 
+00011ef0: 696d 706f 7274 206e 6173 7472 616e 0a20  import nastran. 
+00011f00: 2020 203e 3e3e 206e 6173 7472 616e 2e77     >>> nastran.w
+00011f10: 746e 6173 696e 7473 2831 2c20 322c 206e  tnasints(1, 2, n
+00011f20: 702e 6172 616e 6765 2832 3829 290a 2020  p.arange(28)).  
+00011f30: 2020 2020 2020 2020 2030 2020 2020 2020           0      
+00011f40: 2031 2020 2020 2020 2032 2020 2020 2020   1       2      
+00011f50: 2033 2020 2020 2020 2034 2020 2020 2020   3       4      
+00011f60: 2035 2020 2020 2020 2036 2020 2020 2020   5       6      
+00011f70: 2037 0a20 2020 2020 2020 2020 2020 2020   7.             
+00011f80: 2020 2020 2020 3820 2020 2020 2020 3920        8       9 
+00011f90: 2020 2020 2031 3020 2020 2020 2031 3120       10      11 
+00011fa0: 2020 2020 2031 3220 2020 2020 2031 3320       12      13 
+00011fb0: 2020 2020 2031 3420 2020 2020 2031 350a       14      15.
+00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fd0: 2020 3136 2020 2020 2020 3137 2020 2020    16      17    
+00011fe0: 2020 3138 2020 2020 2020 3139 2020 2020    18      19    
+00011ff0: 2020 3230 2020 2020 2020 3231 2020 2020    20      21    
+00012000: 2020 3232 2020 2020 2020 3233 0a20 2020    22      23.   
+00012010: 2020 2020 2020 2020 2020 2020 2020 2032                 2
+00012020: 3420 2020 2020 2032 3520 2020 2020 2032  4      25      2
+00012030: 3620 2020 2020 2032 370a 2020 2020 2222  6      27.    ""
+00012040: 220a 2020 2020 6e20 3d20 6c65 6e28 696e  ".    n = len(in
+00012050: 7473 290a 2020 2020 6669 7273 746c 696e  ts).    firstlin
+00012060: 6520 3d20 3130 202d 2073 7461 7274 0a20  e = 10 - start. 
+00012070: 2020 2069 6620 6e20 3e3d 2066 6972 7374     if n >= first
+00012080: 6c69 6e65 3a0a 2020 2020 2020 2020 6920  line:.        i 
+00012090: 3d20 6669 7273 746c 696e 650a 2020 2020  = firstline.    
+000120a0: 2020 2020 662e 7772 6974 6528 2822 7b3a      f.write(("{:
+000120b0: 3864 7d22 202a 2069 202b 2022 5c6e 2229  8d}" * i + "\n")
+000120c0: 2e66 6f72 6d61 7428 2a69 6e74 735b 3a69  .format(*ints[:i
+000120d0: 5d29 290a 2020 2020 2020 2020 7768 696c  ])).        whil
+000120e0: 6520 6e20 3e3d 2069 202b 2038 3a0a 2020  e n >= i + 8:.  
+000120f0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00012100: 6528 2822 7b3a 3873 7d22 202b 2022 7b3a  e(("{:8s}" + "{:
+00012110: 3864 7d22 202a 2038 202b 2022 5c6e 2229  8d}" * 8 + "\n")
+00012120: 2e66 6f72 6d61 7428 2222 2c20 2a69 6e74  .format("", *int
+00012130: 735b 6920 3a20 6920 2b20 385d 2929 0a20  s[i : i + 8])). 
+00012140: 2020 2020 2020 2020 2020 2069 202b 3d20             i += 
+00012150: 380a 2020 2020 2020 2020 6966 206e 203e  8.        if n >
+00012160: 2069 3a0a 2020 2020 2020 2020 2020 2020   i:.            
+00012170: 6e20 2d3d 2069 0a20 2020 2020 2020 2020  n -= i.         
+00012180: 2020 2066 2e77 7269 7465 2828 227b 3a38     f.write(("{:8
+00012190: 737d 2220 2b20 227b 3a38 647d 2220 2a20  s}" + "{:8d}" * 
+000121a0: 6e20 2b20 225c 6e22 292e 666f 726d 6174  n + "\n").format
+000121b0: 2822 222c 202a 696e 7473 5b69 3a5d 2929  ("", *ints[i:]))
+000121c0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000121d0: 2020 2066 2e77 7269 7465 2828 227b 3a38     f.write(("{:8
+000121e0: 647d 2220 2a20 6e20 2b20 225c 6e22 292e  d}" * n + "\n").
+000121f0: 666f 726d 6174 282a 696e 7473 2929 0a0a  format(*ints))..
+00012200: 0a64 6566 2072 6463 7375 7065 7273 2866  .def rdcsupers(f
+00012210: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
+00012220: 5265 6164 2043 5355 5045 5220 656e 7472  Read CSUPER entr
+00012230: 6965 730a 0a20 2020 2050 6172 616d 6574  ies..    Paramet
+00012240: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00012250: 2d2d 0a20 2020 2066 203a 2073 7472 696e  --.    f : strin
+00012260: 6720 6f72 2066 696c 655f 6c69 6b65 206f  g or file_like o
+00012270: 7220 4e6f 6e65 0a20 2020 2020 2020 2045  r None.        E
+00012280: 6974 6865 7220 6120 6669 6c65 6e61 6d65  ither a filename
+00012290: 2c20 6f72 2069 7320 6120 6669 6c65 5f6c  , or is a file_l
+000122a0: 696b 6520 6f62 6a65 6374 2061 7320 7265  ike object as re
+000122b0: 7475 726e 6564 0a20 2020 2020 2020 2062  turned.        b
+000122c0: 7920 3a66 756e 633a 606f 7065 6e60 2e20  y :func:`open`. 
+000122d0: 4966 2066 696c 655f 6c69 6b65 206f 626a  If file_like obj
+000122e0: 6563 742c 2069 7420 6973 2072 6577 6f75  ect, it is rewou
+000122f0: 6e64 2066 6972 7374 2e20 4361 6e0a 2020  nd first. Can.  
+00012300: 2020 2020 2020 616c 736f 2062 6520 7468        also be th
+00012310: 6520 6e61 6d65 206f 6620 6120 6469 7265  e name of a dire
+00012320: 6374 6f72 7920 6f72 204e 6f6e 653b 2069  ctory or None; i
+00012330: 6e20 7468 6573 6520 6361 7365 732c 2061  n these cases, a
+00012340: 2047 5549 0a20 2020 2020 2020 2069 7320   GUI.        is 
+00012350: 6f70 656e 6564 2066 6f72 2066 696c 6520  opened for file 
+00012360: 7365 6c65 6374 696f 6e2e 0a0a 2020 2020  selection...    
+00012370: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00012380: 2d2d 2d0a 2020 2020 6469 6374 696f 6e61  ---.    dictiona
+00012390: 7279 0a20 2020 2020 2020 2054 6865 2064  ry.        The d
+000123a0: 6963 7469 6f6e 6172 7920 6b65 7973 2061  ictionary keys a
+000123b0: 7265 2074 6865 2043 5355 5045 5220 4944  re the CSUPER ID
+000123c0: 732e 2054 6865 2064 6963 7469 6f6e 6172  s. The dictionar
+000123d0: 7920 7661 6c75 6573 0a20 2020 2020 2020  y values.       
+000123e0: 2061 7265 2061 6c6c 2074 6865 2069 6473   are all the ids
+000123f0: 2066 726f 6d20 7468 6520 4353 5550 4552   from the CSUPER
+00012400: 2063 6172 6420 696e 2074 6865 2066 6f72   card in the for
+00012410: 6d3a 205b 6373 7570 6572 5f69 642c 2030  m: [csuper_id, 0
+00012420: 2c0a 2020 2020 2020 2020 6e6f 6465 5f69  ,.        node_i
+00012430: 645f 312c 206e 6f64 655f 6964 5f32 2c20  d_1, node_id_2, 
+00012440: e280 a620 6e6f 6465 5f69 645f 6e5d 0a0a  ... node_id_n]..
+00012450: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
+00012460: 2d2d 2d0a 2020 2020 416e 7920 2254 4852  ---.    Any "THR
+00012470: 5522 2066 6965 6c64 7320 7769 6c6c 2062  U" fields will b
+00012480: 6520 7365 7420 746f 202d 312e 2054 6869  e set to -1. Thi
+00012490: 7320 726f 7574 696e 6520 7369 6d70 6c79  s routine simply
+000124a0: 2063 616c 6c73 2074 6865 0a20 2020 206d   calls the.    m
+000124b0: 6f72 6520 6765 6e65 7261 6c20 726f 7574  ore general rout
+000124c0: 696e 6520 3a66 756e 633a 6072 6463 6172  ine :func:`rdcar
+000124d0: 6473 603a 3a0a 0a20 2020 2020 2020 2072  ds`::..        r
+000124e0: 6463 6172 6473 2866 2c20 2763 7375 7065  dcards(f, 'csupe
+000124f0: 7227 2c20 7265 7475 726e 5f76 6172 3d27  r', return_var='
+00012500: 6469 6374 272c 2064 7479 7065 3d6e 702e  dict', dtype=np.
+00012510: 696e 7436 342c 2062 6c61 6e6b 3d2d 3129  int64, blank=-1)
+00012520: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
+00012530: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00012540: 3e3e 3e20 696d 706f 7274 206e 756d 7079  >>> import numpy
+00012550: 2061 7320 6e70 0a20 2020 203e 3e3e 2066   as np.    >>> f
+00012560: 726f 6d20 7079 7965 7469 2069 6d70 6f72  rom pyyeti impor
+00012570: 7420 6e61 7374 7261 6e0a 2020 2020 3e3e  t nastran.    >>
+00012580: 3e20 6672 6f6d 2069 6f20 696d 706f 7274  > from io import
+00012590: 2053 7472 696e 6749 4f0a 2020 2020 3e3e   StringIO.    >>
+000125a0: 3e20 6e70 2e73 6574 5f70 7269 6e74 6f70  > np.set_printop
+000125b0: 7469 6f6e 7328 6c69 6e65 7769 6474 683d  tions(linewidth=
+000125c0: 3630 290a 2020 2020 3e3e 3e20 6620 3d20  60).    >>> f = 
+000125d0: 5374 7269 6e67 494f 2822 4353 5550 4552  StringIO("CSUPER
+000125e0: 2c31 3031 2c30 2c33 2c31 312c 3139 2c32  ,101,0,3,11,19,2
+000125f0: 372c 3139 3935 3030 312c 3139 3935 3030  7,1995001,199500
+00012600: 325c 6e22 0a20 2020 202e 2e2e 2020 2020  2\n".    ...    
+00012610: 2020 2020 2020 2020 2020 222c 3139 3935            ",1995
+00012620: 3030 332c 7468 7275 2c31 3939 3530 3130  003,thru,1995010
+00012630: 2020 2420 636f 6d6d 656e 7422 290a 2020    $ comment").  
+00012640: 2020 3e3e 3e20 6e61 7374 7261 6e2e 7264    >>> nastran.rd
+00012650: 6373 7570 6572 7328 6629 2020 2020 2020  csupers(f)      
+00012660: 2020 2020 2020 2023 2064 6f63 7465 7374         # doctest
+00012670: 3a20 2b45 4c4c 4950 5349 530a 2020 2020  : +ELLIPSIS.    
+00012680: 7b31 3031 3a20 6172 7261 7928 5b20 2020  {101: array([   
+00012690: 2031 3031 2c20 2020 2020 2020 302c 2020   101,       0,  
+000126a0: 2020 2020 2033 2c20 2020 2020 2031 312c       3,      11,
+000126b0: 2020 2020 2020 3139 2c20 2020 2020 2032        19,      2
+000126c0: 372c 0a20 2020 2020 2020 2020 2020 3139  7,.           19
+000126d0: 3935 3030 312c 2031 3939 3530 3032 2c20  95001, 1995002, 
+000126e0: 3139 3935 3030 332c 2020 2020 2020 2d31  1995003,      -1
+000126f0: 2c20 3139 3935 3031 305d 2e2e 2e29 7d0a  , 1995010]...)}.
+00012700: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+00012710: 726e 2072 6463 6172 6473 2866 2c20 2263  rn rdcards(f, "c
+00012720: 7375 7065 7222 2c20 7265 7475 726e 5f76  super", return_v
+00012730: 6172 3d22 6469 6374 222c 2064 7479 7065  ar="dict", dtype
+00012740: 3d6e 702e 696e 7436 342c 2062 6c61 6e6b  =np.int64, blank
+00012750: 3d2d 3129 0a0a 0a64 6566 2072 6465 7874  =-1)...def rdext
+00012760: 726e 2866 2c20 6578 7061 6e64 3d54 7275  rn(f, expand=Tru
+00012770: 6529 3a0a 2020 2020 7222 2222 0a20 2020  e):.    r""".   
+00012780: 2052 6561 6420 4558 5452 4e20 656e 7472   Read EXTRN entr
+00012790: 7920 6672 6f6d 202e 7063 6820 6669 6c65  y from .pch file
+000127a0: 2063 7265 6174 6564 2062 7920 4e61 7374   created by Nast
+000127b0: 7261 6e0a 0a20 2020 2050 6172 616d 6574  ran..    Paramet
+000127c0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000127d0: 2d2d 0a20 2020 2066 203a 2073 7472 696e  --.    f : strin
+000127e0: 6720 6f72 2066 696c 655f 6c69 6b65 206f  g or file_like o
+000127f0: 7220 4e6f 6e65 0a20 2020 2020 2020 2045  r None.        E
+00012800: 6974 6865 7220 6120 6e61 6d65 206f 6620  ither a name of 
+00012810: 6120 6669 6c65 2c20 6f72 2069 7320 6120  a file, or is a 
+00012820: 6669 6c65 5f6c 696b 6520 6f62 6a65 6374  file_like object
+00012830: 2061 7320 7265 7475 726e 6564 0a20 2020   as returned.   
+00012840: 2020 2020 2062 7920 3a66 756e 633a 606f       by :func:`o
+00012850: 7065 6e60 2e20 4966 2066 696c 655f 6c69  pen`. If file_li
+00012860: 6b65 206f 626a 6563 742c 2069 7420 6973  ke object, it is
+00012870: 2072 6577 6f75 6e64 2066 6972 7374 2e20   rewound first. 
+00012880: 4361 6e0a 2020 2020 2020 2020 616c 736f  Can.        also
+00012890: 2062 6520 7468 6520 6e61 6d65 206f 6620   be the name of 
+000128a0: 6120 6469 7265 6374 6f72 7920 6f72 204e  a directory or N
+000128b0: 6f6e 653b 2069 6e20 7468 6573 6520 6361  one; in these ca
+000128c0: 7365 732c 2061 2047 5549 0a20 2020 2020  ses, a GUI.     
+000128d0: 2020 2069 7320 6f70 656e 6564 2066 6f72     is opened for
+000128e0: 2066 696c 6520 7365 6c65 6374 696f 6e2e   file selection.
+000128f0: 0a20 2020 2065 7870 616e 6420 3a20 626f  .    expand : bo
+00012900: 6f6c 3b20 6f70 7469 6f6e 616c 0a20 2020  ol; optional.   
+00012910: 2020 2020 2049 6620 5472 7565 2c20 6578       If True, ex
+00012920: 7061 6e64 2072 6f77 7320 6c69 6b65 2074  pand rows like t
+00012930: 6869 733a 3a0a 0a20 2020 2020 2020 2020  his::..         
+00012940: 2020 205b 3130 302c 2031 3233 3435 365d     [100, 123456]
+00012950: 0a0a 2020 2020 2020 2020 696e 746f 2036  ..        into 6
+00012960: 2073 6570 6172 6174 6520 726f 7773 206c   separate rows l
+00012970: 696b 6520 7468 6973 3a3a 0a0a 2020 2020  ike this::..    
+00012980: 2020 2020 2020 2020 5b31 3030 2c20 315d          [100, 1]
+00012990: 2c0a 2020 2020 2020 2020 2020 2020 5b31  ,.            [1
+000129a0: 3030 2c20 325d 2c0a 2020 2020 2020 2020  00, 2],.        
+000129b0: 2020 2020 5b31 3030 2c20 335d 2c0a 2020      [100, 3],.  
+000129c0: 2020 2020 2020 2020 2020 5b31 3030 2c20            [100, 
+000129d0: 345d 2c0a 2020 2020 2020 2020 2020 2020  4],.            
+000129e0: 5b31 3030 2c20 355d 2c0a 2020 2020 2020  [100, 5],.      
+000129f0: 2020 2020 2020 5b31 3030 2c20 365d 2c0a        [100, 6],.
+00012a00: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00012a10: 202d 2d2d 2d2d 2d2d 0a20 2020 2032 6420   -------.    2d 
+00012a20: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+00012a30: 5477 6f20 636f 6c75 6d6e 2061 7272 6179  Two column array
+00012a40: 3a20 5b49 442c 2044 4f46 5d0a 0a20 2020  : [ID, DOF]..   
+00012a50: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
+00012a60: 0a20 2020 2054 6865 2065 7870 616e 7369  .    The expansi
+00012a70: 6f6e 2069 7320 646f 6e65 2062 7920 3a66  on is done by :f
+00012a80: 756e 633a 6070 7979 6574 692e 6e61 7374  unc:`pyyeti.nast
+00012a90: 7261 6e2e 6e32 702e 6578 7061 6e64 646f  ran.n2p.expanddo
+00012aa0: 6660 2e0a 0a20 2020 2045 7861 6d70 6c65  f`...    Example
+00012ab0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
+00012ac0: 2020 203e 3e3e 2066 726f 6d20 7079 7965     >>> from pyye
+00012ad0: 7469 2069 6d70 6f72 7420 6e61 7374 7261  ti import nastra
+00012ae0: 6e0a 2020 2020 3e3e 3e20 6672 6f6d 2069  n.    >>> from i
+00012af0: 6f20 696d 706f 7274 2053 7472 696e 6749  o import StringI
+00012b00: 4f0a 2020 2020 3e3e 3e20 6620 3d20 5374  O.    >>> f = St
+00012b10: 7269 6e67 494f 2827 4558 5452 4e2c 332c  ringIO('EXTRN,3,
+00012b20: 3132 3334 3536 2c31 312c 3132 3334 3536  123456,11,123456
+00012b30: 2c31 392c 3132 3334 3536 2c32 372c 3132  ,19,123456,27,12
+00012b40: 3334 3536 5c6e 270a 2020 2020 2e2e 2e20  3456\n'.    ... 
+00012b50: 2020 2020 2020 2020 2020 2020 2027 2c32               ',2
+00012b60: 3939 3530 3031 2c30 2c32 3939 3530 3032  995001,0,2995002
+00012b70: 2c30 2c32 3939 3530 3033 2c30 2c32 3939  ,0,2995003,0,299
+00012b80: 3530 3034 2c30 5c6e 270a 2020 2020 2e2e  5004,0\n'.    ..
+00012b90: 2e20 2020 2020 2020 2020 2020 2020 2027  .              '
+00012ba0: 2c32 3939 3530 3035 2c30 2c32 3939 3530  ,2995005,0,29950
+00012bb0: 3036 2c30 2c32 3939 3530 3037 2c30 2c32  06,0,2995007,0,2
+00012bc0: 3939 3530 3038 2c30 5c6e 2729 0a20 2020  995008,0\n').   
+00012bd0: 203e 3e3e 206e 6173 7472 616e 2e72 6465   >>> nastran.rde
+00012be0: 7874 726e 2866 2c20 6578 7061 6e64 3d46  xtrn(f, expand=F
+00012bf0: 616c 7365 2920 2020 2320 646f 6374 6573  alse)   # doctes
+00012c00: 743a 202b 454c 4c49 5053 4953 0a20 2020  t: +ELLIPSIS.   
+00012c10: 2061 7272 6179 285b 5b20 2020 2020 2033   array([[      3
+00012c20: 2c20 2031 3233 3435 365d 2c0a 2020 2020  ,  123456],.    
+00012c30: 2020 2020 2020 205b 2020 2020 2031 312c         [     11,
+00012c40: 2020 3132 3334 3536 5d2c 0a20 2020 2020    123456],.     
+00012c50: 2020 2020 2020 5b20 2020 2020 3139 2c20        [     19, 
+00012c60: 2031 3233 3435 365d 2c0a 2020 2020 2020   123456],.      
+00012c70: 2020 2020 205b 2020 2020 2032 372c 2020       [     27,  
+00012c80: 3132 3334 3536 5d2c 0a20 2020 2020 2020  123456],.       
+00012c90: 2020 2020 5b32 3939 3530 3031 2c20 2020      [2995001,   
+00012ca0: 2020 2020 305d 2c0a 2020 2020 2020 2020      0],.        
+00012cb0: 2020 205b 3239 3935 3030 322c 2020 2020     [2995002,    
+00012cc0: 2020 2030 5d2c 0a20 2020 2020 2020 2020     0],.         
+00012cd0: 2020 5b32 3939 3530 3033 2c20 2020 2020    [2995003,     
+00012ce0: 2020 305d 2c0a 2020 2020 2020 2020 2020    0],.          
+00012cf0: 205b 3239 3935 3030 342c 2020 2020 2020   [2995004,      
+00012d00: 2030 5d2c 0a20 2020 2020 2020 2020 2020   0],.           
+00012d10: 5b32 3939 3530 3035 2c20 2020 2020 2020  [2995005,       
+00012d20: 305d 2c0a 2020 2020 2020 2020 2020 205b  0],.           [
+00012d30: 3239 3935 3030 362c 2020 2020 2020 2030  2995006,       0
+00012d40: 5d2c 0a20 2020 2020 2020 2020 2020 5b32  ],.           [2
+00012d50: 3939 3530 3037 2c20 2020 2020 2020 305d  995007,       0]
+00012d60: 2c0a 2020 2020 2020 2020 2020 205b 3239  ,.           [29
+00012d70: 3935 3030 382c 2020 2020 2020 2030 5d5d  95008,       0]]
+00012d80: 2e2e 2e29 0a20 2020 203e 3e3e 2066 203d  ...).    >>> f =
+00012d90: 2053 7472 696e 6749 4f28 2745 5854 524e   StringIO('EXTRN
+00012da0: 2c33 2c31 3233 3435 362c 3239 3935 3030  ,3,123456,299500
+00012db0: 312c 3027 290a 2020 2020 3e3e 3e20 6e61  1,0').    >>> na
+00012dc0: 7374 7261 6e2e 7264 6578 7472 6e28 6629  stran.rdextrn(f)
+00012dd0: 2020 2020 2020 2020 2020 2020 2023 2064               # d
+00012de0: 6f63 7465 7374 3a20 2b45 4c4c 4950 5349  octest: +ELLIPSI
+00012df0: 530a 2020 2020 6172 7261 7928 5b5b 2020  S.    array([[  
+00012e00: 2020 2020 332c 2020 2020 2020 2031 5d2c      3,       1],
+00012e10: 0a20 2020 2020 2020 2020 2020 5b20 2020  .           [   
+00012e20: 2020 2033 2c20 2020 2020 2020 325d 2c0a     3,       2],.
+00012e30: 2020 2020 2020 2020 2020 205b 2020 2020             [    
+00012e40: 2020 332c 2020 2020 2020 2033 5d2c 0a20    3,       3],. 
+00012e50: 2020 2020 2020 2020 2020 5b20 2020 2020            [     
+00012e60: 2033 2c20 2020 2020 2020 345d 2c0a 2020   3,       4],.  
+00012e70: 2020 2020 2020 2020 205b 2020 2020 2020           [      
+00012e80: 332c 2020 2020 2020 2035 5d2c 0a20 2020  3,       5],.   
+00012e90: 2020 2020 2020 2020 5b20 2020 2020 2033          [      3
+00012ea0: 2c20 2020 2020 2020 365d 2c0a 2020 2020  ,       6],.    
+00012eb0: 2020 2020 2020 205b 3239 3935 3030 312c         [2995001,
+00012ec0: 2020 2020 2020 2030 5d5d 2e2e 2e29 0a20         0]]...). 
+00012ed0: 2020 2022 2222 0a20 2020 2065 7874 726e     """.    extrn
+00012ee0: 203d 2072 6463 6172 6473 2866 2c20 2265   = rdcards(f, "e
+00012ef0: 7874 726e 222c 2064 7479 7065 3d6e 702e  xtrn", dtype=np.
+00012f00: 696e 7436 3429 2e72 6573 6861 7065 282d  int64).reshape(-
+00012f10: 312c 2032 290a 2020 2020 6966 2065 7870  1, 2).    if exp
+00012f20: 616e 643a 0a20 2020 2020 2020 2065 7874  and:.        ext
+00012f30: 726e 203d 206e 3270 2e65 7870 616e 6464  rn = n2p.expandd
+00012f40: 6f66 2865 7874 726e 290a 2020 2020 7265  of(extrn).    re
+00012f50: 7475 726e 2065 7874 726e 0a0a 0a40 6775  turn extrn...@gu
+00012f60: 6974 6f6f 6c73 2e77 7269 7465 5f74 6578  itools.write_tex
+00012f70: 745f 6669 6c65 0a64 6566 2077 7463 7375  t_file.def wtcsu
+00012f80: 7065 7228 662c 2073 7570 6572 6964 2c20  per(f, superid, 
+00012f90: 6772 6964 7329 3a0a 2020 2020 2222 220a  grids):.    """.
+00012fa0: 2020 2020 5772 6974 6573 2061 204e 6173      Writes a Nas
+00012fb0: 7472 616e 2043 5355 5045 5220 6361 7264  tran CSUPER card
+00012fc0: 2074 6f20 6120 6669 6c65 2e0a 0a20 2020   to a file...   
+00012fd0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00012fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066  ----------.    f
+00012ff0: 203a 2073 7472 696e 6720 6f72 2066 696c   : string or fil
+00013000: 655f 6c69 6b65 206f 7220 3120 6f72 204e  e_like or 1 or N
+00013010: 6f6e 650a 2020 2020 2020 2020 4569 7468  one.        Eith
+00013020: 6572 2061 206e 616d 6520 6f66 2061 2066  er a name of a f
+00013030: 696c 652c 206f 7220 6973 2061 2066 696c  ile, or is a fil
+00013040: 655f 6c69 6b65 206f 626a 6563 7420 6173  e_like object as
+00013050: 2072 6574 7572 6e65 640a 2020 2020 2020   returned.      
+00013060: 2020 6279 203a 6675 6e63 3a60 6f70 656e    by :func:`open
+00013070: 6020 6f72 203a 636c 6173 733a 6069 6f2e  ` or :class:`io.
+00013080: 5374 7269 6e67 494f 602e 2049 6e70 7574  StringIO`. Input
+00013090: 2061 7320 696e 7465 6765 7220 3120 746f   as integer 1 to
+000130a0: 0a20 2020 2020 2020 2077 7269 7465 2074  .        write t
+000130b0: 6f20 7374 646f 7574 2e20 4361 6e20 616c  o stdout. Can al
+000130c0: 736f 2062 6520 7468 6520 6e61 6d65 206f  so be the name o
+000130d0: 6620 6120 6469 7265 6374 6f72 7920 6f72  f a directory or
+000130e0: 204e 6f6e 653b 0a20 2020 2020 2020 2069   None;.        i
+000130f0: 6e20 7468 6573 6520 6361 7365 732c 2061  n these cases, a
+00013100: 2047 5549 2069 7320 6f70 656e 6564 2066   GUI is opened f
+00013110: 6f72 2066 696c 6520 7365 6c65 6374 696f  or file selectio
+00013120: 6e2e 0a20 2020 2073 7570 6572 6964 203a  n..    superid :
+00013130: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
+00013140: 2053 7570 6572 656c 656d 656e 7420 4944   Superelement ID
+00013150: 0a20 2020 2067 7269 6473 203a 2031 6420  .    grids : 1d 
+00013160: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+00013170: 2020 2056 6563 746f 7220 6f66 2067 7269     Vector of gri
+00013180: 6420 6964 732e 0a0a 2020 2020 5265 7475  d ids...    Retu
+00013190: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+000131a0: 2020 2020 4e6f 6e65 0a0a 2020 2020 4578      None..    Ex
+000131b0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+000131c0: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
+000131d0: 2070 7979 6574 6920 696d 706f 7274 206e   pyyeti import n
+000131e0: 6173 7472 616e 0a20 2020 203e 3e3e 2069  astran.    >>> i
+000131f0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+00013200: 700a 2020 2020 3e3e 3e20 6e61 7374 7261  p.    >>> nastra
+00013210: 6e2e 7774 6373 7570 6572 2831 2c20 3130  n.wtcsuper(1, 10
+00013220: 302c 206e 702e 6172 616e 6765 2831 2c20  0, np.arange(1, 
+00013230: 3130 2929 0a20 2020 2043 5355 5045 5220  10)).    CSUPER 
+00013240: 2020 2020 2020 3130 3020 2020 2020 2020        100       
+00013250: 3020 2020 2020 2020 3120 2020 2020 2020  0       1       
+00013260: 3220 2020 2020 2020 3320 2020 2020 2020  2       3       
+00013270: 3420 2020 2020 2020 3520 2020 2020 2020  4       5       
+00013280: 360a 2020 2020 2020 2020 2020 2020 2020  6.              
+00013290: 2020 2020 2037 2020 2020 2020 2038 2020       7       8  
+000132a0: 2020 2020 2039 0a20 2020 2022 2222 0a20       9.    """. 
+000132b0: 2020 2066 2e77 7269 7465 2866 2243 5355     f.write(f"CSU
+000132c0: 5045 5220 207b 7375 7065 7269 643a 3864  PER  {superid:8d
+000132d0: 7d7b 303a 3864 7d22 290a 2020 2020 7774  }{0:8d}").    wt
+000132e0: 6e61 7369 6e74 7328 662c 2034 2c20 6772  nasints(f, 4, gr
+000132f0: 6964 7329 0a0a 0a40 6775 6974 6f6f 6c73  ids)...@guitools
+00013300: 2e77 7269 7465 5f74 6578 745f 6669 6c65  .write_text_file
+00013310: 0a64 6566 2077 7473 7063 3128 662c 2065  .def wtspc1(f, e
+00013320: 6964 2c20 646f 662c 2067 7269 6473 2c20  id, dof, grids, 
+00013330: 6e61 6d65 3d22 5350 4331 2229 3a0a 2020  name="SPC1"):.  
+00013340: 2020 2222 220a 2020 2020 5772 6974 6573    """.    Writes
+00013350: 2061 204e 6173 7472 616e 2053 5043 3120   a Nastran SPC1 
+00013360: 286f 7220 7369 6d69 6c61 7229 2063 6172  (or similar) car
+00013370: 6420 746f 2061 2066 696c 652e 0a0a 2020  d to a file...  
+00013380: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00013390: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000133a0: 6620 3a20 7374 7269 6e67 206f 7220 6669  f : string or fi
+000133b0: 6c65 5f6c 696b 6520 6f72 2031 206f 7220  le_like or 1 or 
+000133c0: 4e6f 6e65 0a20 2020 2020 2020 2045 6974  None.        Eit
+000133d0: 6865 7220 6120 6e61 6d65 206f 6620 6120  her a name of a 
+000133e0: 6669 6c65 2c20 6f72 2069 7320 6120 6669  file, or is a fi
+000133f0: 6c65 5f6c 696b 6520 6f62 6a65 6374 2061  le_like object a
+00013400: 7320 7265 7475 726e 6564 0a20 2020 2020  s returned.     
+00013410: 2020 2062 7920 3a66 756e 633a 606f 7065     by :func:`ope
+00013420: 6e60 206f 7220 3a63 6c61 7373 3a60 696f  n` or :class:`io
+00013430: 2e53 7472 696e 6749 4f60 2e20 496e 7075  .StringIO`. Inpu
+00013440: 7420 6173 2069 6e74 6567 6572 2031 2074  t as integer 1 t
+00013450: 6f0a 2020 2020 2020 2020 7772 6974 6520  o.        write 
+00013460: 746f 2073 7464 6f75 742e 2043 616e 2061  to stdout. Can a
+00013470: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
+00013480: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
+00013490: 7220 4e6f 6e65 3b0a 2020 2020 2020 2020  r None;.        
+000134a0: 696e 2074 6865 7365 2063 6173 6573 2c20  in these cases, 
+000134b0: 6120 4755 4920 6973 206f 7065 6e65 6420  a GUI is opened 
+000134c0: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
+000134d0: 6f6e 2e0a 2020 2020 6569 6420 3a20 696e  on..    eid : in
+000134e0: 7465 6765 720a 2020 2020 2020 2020 456c  teger.        El
+000134f0: 656d 656e 7420 4944 0a20 2020 2064 6f66  ement ID.    dof
+00013500: 203a 2069 6e74 6567 6572 0a20 2020 2020   : integer.     
+00013510: 2020 2041 6e20 696e 7465 6765 7220 636f     An integer co
+00013520: 6e63 6174 656e 6174 696f 6e20 6f66 2074  ncatenation of t
+00013530: 6865 2044 4f46 2028 6578 3a20 3132 3334  he DOF (ex: 1234
+00013540: 3536 290a 2020 2020 6772 6964 7320 3a20  56).    grids : 
+00013550: 3164 2061 7272 6179 5f6c 696b 650a 2020  1d array_like.  
+00013560: 2020 2020 2020 5665 6374 6f72 206f 6620        Vector of 
+00013570: 6772 6964 2069 6473 2e0a 2020 2020 6e61  grid ids..    na
+00013580: 6d65 203a 2073 7472 696e 673b 206f 7074  me : string; opt
+00013590: 696f 6e61 6c0a 2020 2020 2020 2020 4e61  ional.        Na
+000135a0: 6d65 206f 6620 4e41 5354 5241 4e20 6361  me of NASTRAN ca
+000135b0: 7264 2074 6f20 7772 6974 653b 2063 6172  rd to write; car
+000135c0: 6420 6d75 7374 2062 6520 696e 2073 616d  d must be in sam
+000135d0: 6520 666f 726d 6174 2061 730a 2020 2020  e format as.    
+000135e0: 2020 2020 7468 6520 5350 4331 2063 6172      the SPC1 car
+000135f0: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+00013600: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00013610: 4e6f 6e65 0a0a 2020 2020 4578 616d 706c  None..    Exampl
+00013620: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+00013630: 2020 2020 3e3e 3e20 6672 6f6d 2070 7979      >>> from pyy
+00013640: 6574 6920 696d 706f 7274 206e 6173 7472  eti import nastr
+00013650: 616e 0a20 2020 203e 3e3e 2069 6d70 6f72  an.    >>> impor
+00013660: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
+00013670: 2020 3e3e 3e20 6e61 7374 7261 6e2e 7774    >>> nastran.wt
+00013680: 7370 6331 2831 2c20 312c 2031 3233 3435  spc1(1, 1, 12345
+00013690: 362c 206e 702e 6172 616e 6765 2831 2c20  6, np.arange(1, 
+000136a0: 3130 2929 0a20 2020 2053 5043 3120 2020  10)).    SPC1   
+000136b0: 2020 2020 2020 2020 3120 2031 3233 3435          1  12345
+000136c0: 3620 2020 2020 2020 3120 2020 2020 2020  6       1       
+000136d0: 3220 2020 2020 2020 3320 2020 2020 2020  2       3       
+000136e0: 3420 2020 2020 2020 3520 2020 2020 2020  4       5       
+000136f0: 360a 2020 2020 2020 2020 2020 2020 2020  6.              
+00013700: 2020 2020 2037 2020 2020 2020 2038 2020       7       8  
+00013710: 2020 2020 2039 0a20 2020 203e 3e3e 206e       9.    >>> n
+00013720: 6173 7472 616e 2e77 7473 7063 3128 312c  astran.wtspc1(1,
+00013730: 2032 3030 2c20 3132 3334 3536 2c20 6e70   200, 123456, np
+00013740: 2e61 7261 6e67 6528 3230 3031 2c20 3230  .arange(2001, 20
+00013750: 3331 292c 0a20 2020 202e 2e2e 2020 2020  31),.    ...    
+00013760: 2020 2020 2020 2020 2020 2020 2753 4551              'SEQ
+00013770: 5345 5431 2729 0a20 2020 2053 4551 5345  SET1').    SEQSE
+00013780: 5431 2020 2020 2020 3230 3020 2031 3233  T1      200  123
+00013790: 3435 3620 2020 2032 3030 3120 2020 2032  456    2001    2
+000137a0: 3030 3220 2020 2032 3030 3320 2020 2032  002    2003    2
+000137b0: 3030 3420 2020 2032 3030 3520 2020 2032  004    2005    2
+000137c0: 3030 360a 2020 2020 2020 2020 2020 2020  006.            
+000137d0: 2020 2020 3230 3037 2020 2020 3230 3038      2007    2008
+000137e0: 2020 2020 3230 3039 2020 2020 3230 3130      2009    2010
+000137f0: 2020 2020 3230 3131 2020 2020 3230 3132      2011    2012
+00013800: 2020 2020 3230 3133 2020 2020 3230 3134      2013    2014
+00013810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013820: 2032 3031 3520 2020 2032 3031 3620 2020   2015    2016   
+00013830: 2032 3031 3720 2020 2032 3031 3820 2020   2017    2018   
+00013840: 2032 3031 3920 2020 2032 3032 3020 2020   2019    2020   
+00013850: 2032 3032 3120 2020 2032 3032 320a 2020   2021    2022.  
+00013860: 2020 2020 2020 2020 2020 2020 2020 3230                20
+00013870: 3233 2020 2020 3230 3234 2020 2020 3230  23    2024    20
+00013880: 3235 2020 2020 3230 3236 2020 2020 3230  25    2026    20
+00013890: 3237 2020 2020 3230 3238 2020 2020 3230  27    2028    20
+000138a0: 3239 2020 2020 3230 3330 0a20 2020 2022  29    2030.    "
+000138b0: 2222 0a20 2020 2066 2e77 7269 7465 2866  "".    f.write(f
+000138c0: 227b 6e61 6d65 3a3c 3873 7d7b 6569 643a  "{name:<8s}{eid:
+000138d0: 3864 7d7b 646f 663a 3864 7d22 290a 2020  8d}{dof:8d}").  
+000138e0: 2020 7774 6e61 7369 6e74 7328 662c 2034    wtnasints(f, 4
+000138f0: 2c20 6772 6964 7329 0a0a 0a40 6775 6974  , grids)...@guit
+00013900: 6f6f 6c73 2e77 7269 7465 5f74 6578 745f  ools.write_text_
+00013910: 6669 6c65 0a64 6566 2077 7478 7365 7431  file.def wtxset1
+00013920: 2866 2c20 646f 662c 2067 7269 6473 2c20  (f, dof, grids, 
+00013930: 6e61 6d65 3d22 4253 4554 3122 293a 0a20  name="BSET1"):. 
+00013940: 2020 2022 2222 0a20 2020 2057 7269 7465     """.    Write
+00013950: 7320 6120 4e61 7374 7261 6e20 4253 4554  s a Nastran BSET
+00013960: 312c 2051 5345 5431 2028 6f72 2073 696d  1, QSET1 (or sim
+00013970: 696c 6172 2920 6361 7264 2074 6f20 6120  ilar) card to a 
+00013980: 6669 6c65 2e0a 0a20 2020 2050 6172 616d  file...    Param
+00013990: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000139a0: 2d2d 2d2d 0a20 2020 2066 203a 2073 7472  ----.    f : str
+000139b0: 696e 6720 6f72 2066 696c 655f 6c69 6b65  ing or file_like
+000139c0: 206f 7220 3120 6f72 204e 6f6e 650a 2020   or 1 or None.  
+000139d0: 2020 2020 2020 4569 7468 6572 2061 206e        Either a n
+000139e0: 616d 6520 6f66 2061 2066 696c 652c 206f  ame of a file, o
+000139f0: 7220 6973 2061 2066 696c 655f 6c69 6b65  r is a file_like
+00013a00: 206f 626a 6563 7420 6173 2072 6574 7572   object as retur
+00013a10: 6e65 640a 2020 2020 2020 2020 6279 203a  ned.        by :
+00013a20: 6675 6e63 3a60 6f70 656e 6020 6f72 203a  func:`open` or :
+00013a30: 636c 6173 733a 6069 6f2e 5374 7269 6e67  class:`io.String
+00013a40: 494f 602e 2049 6e70 7574 2061 7320 696e  IO`. Input as in
+00013a50: 7465 6765 7220 3120 746f 0a20 2020 2020  teger 1 to.     
+00013a60: 2020 2077 7269 7465 2074 6f20 7374 646f     write to stdo
+00013a70: 7574 2e20 4361 6e20 616c 736f 2062 6520  ut. Can also be 
+00013a80: 7468 6520 6e61 6d65 206f 6620 6120 6469  the name of a di
+00013a90: 7265 6374 6f72 7920 6f72 204e 6f6e 653b  rectory or None;
+00013aa0: 0a20 2020 2020 2020 2069 6e20 7468 6573  .        in thes
+00013ab0: 6520 6361 7365 732c 2061 2047 5549 2069  e cases, a GUI i
+00013ac0: 7320 6f70 656e 6564 2066 6f72 2066 696c  s opened for fil
+00013ad0: 6520 7365 6c65 6374 696f 6e2e 0a20 2020  e selection..   
+00013ae0: 2064 6f66 203a 2069 6e74 6567 6572 0a20   dof : integer. 
+00013af0: 2020 2020 2020 2041 6e20 696e 7465 6765         An intege
+00013b00: 7220 636f 6e63 6174 656e 6174 696f 6e20  r concatenation 
+00013b10: 6f66 2074 6865 2044 4f46 2028 6578 3a20  of the DOF (ex: 
+00013b20: 3132 3334 3536 290a 2020 2020 6772 6964  123456).    grid
+00013b30: 7320 3a20 3164 2061 7272 6179 5f6c 696b  s : 1d array_lik
+00013b40: 650a 2020 2020 2020 2020 5665 6374 6f72  e.        Vector
+00013b50: 206f 6620 6772 6964 2069 6473 2e0a 2020   of grid ids..  
+00013b60: 2020 6e61 6d65 203a 2073 7472 696e 673b    name : string;
+00013b70: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00013b80: 2020 4e61 6d65 206f 6620 4e41 5354 5241    Name of NASTRA
+00013b90: 4e20 6361 7264 2074 6f20 7772 6974 653b  N card to write;
+00013ba0: 2063 6172 6420 6d75 7374 2062 6520 696e   card must be in
+00013bb0: 2073 616d 6520 666f 726d 6174 2061 730a   same format as.
+00013bc0: 2020 2020 2020 2020 7468 6520 5350 4331          the SPC1
+00013bd0: 2063 6172 642e 0a0a 2020 2020 5265 7475   card...    Retu
+00013be0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00013bf0: 2020 2020 4e6f 6e65 0a0a 2020 2020 4578      None..    Ex
+00013c00: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00013c10: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
+00013c20: 2070 7979 6574 6920 696d 706f 7274 206e   pyyeti import n
+00013c30: 6173 7472 616e 0a20 2020 203e 3e3e 2069  astran.    >>> i
+00013c40: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+00013c50: 700a 2020 2020 3e3e 3e20 6e61 7374 7261  p.    >>> nastra
+00013c60: 6e2e 7774 7873 6574 3128 312c 2031 3233  n.wtxset1(1, 123
+00013c70: 3435 362c 206e 702e 6172 616e 6765 2831  456, np.arange(1
+00013c80: 2c20 3131 2929 0a20 2020 2042 5345 5431  , 11)).    BSET1
+00013c90: 2020 2020 2031 3233 3435 3620 2020 2020       123456     
+00013ca0: 2020 3120 2020 2020 2020 3220 2020 2020    1       2     
+00013cb0: 2020 3320 2020 2020 2020 3420 2020 2020    3       4     
+00013cc0: 2020 3520 2020 2020 2020 3620 2020 2020    5       6     
+00013cd0: 2020 370a 2020 2020 2020 2020 2020 2020    7.            
+00013ce0: 2020 2020 2020 2038 2020 2020 2020 2039         8       9
+00013cf0: 2020 2020 2020 3130 0a20 2020 203e 3e3e        10.    >>>
+00013d00: 206e 6173 7472 616e 2e77 7478 7365 7431   nastran.wtxset1
+00013d10: 2831 2c20 302c 206e 702e 6172 616e 6765  (1, 0, np.arange
+00013d20: 2832 3030 312c 2032 3031 3329 2c20 2751  (2001, 2013), 'Q
+00013d30: 5345 5431 2729 0a20 2020 2051 5345 5431  SET1').    QSET1
+00013d40: 2020 2020 2020 2020 2020 3020 2020 2032            0    2
+00013d50: 3030 3120 2020 2032 3030 3220 2020 2032  001    2002    2
+00013d60: 3030 3320 2020 2032 3030 3420 2020 2032  003    2004    2
+00013d70: 3030 3520 2020 2032 3030 3620 2020 2032  005    2006    2
+00013d80: 3030 370a 2020 2020 2020 2020 2020 2020  007.            
+00013d90: 2020 2020 3230 3038 2020 2020 3230 3039      2008    2009
+00013da0: 2020 2020 3230 3130 2020 2020 3230 3131      2010    2011
+00013db0: 2020 2020 3230 3132 0a20 2020 2022 2222      2012.    """
+00013dc0: 0a20 2020 2066 2e77 7269 7465 2866 227b  .    f.write(f"{
+00013dd0: 6e61 6d65 3a3c 3873 7d7b 646f 663a 3864  name:<8s}{dof:8d
+00013de0: 7d22 290a 2020 2020 7774 6e61 7369 6e74  }").    wtnasint
+00013df0: 7328 662c 2033 2c20 6772 6964 7329 0a0a  s(f, 3, grids)..
+00013e00: 0a40 6775 6974 6f6f 6c73 2e77 7269 7465  .@guitools.write
+00013e10: 5f74 6578 745f 6669 6c65 0a64 6566 2077  _text_file.def w
+00013e20: 7471 6373 6574 2866 2c20 7374 6172 7467  tqcset(f, startg
+00013e30: 7269 642c 206e 7129 3a0a 2020 2020 2222  rid, nq):.    ""
+00013e40: 220a 2020 2020 5772 6974 6573 204e 6173  ".    Writes Nas
+00013e50: 7472 616e 2051 5345 5431 2061 6e64 2043  tran QSET1 and C
+00013e60: 5345 5431 2063 6172 6473 2066 6f72 2047  SET1 cards for G
+00013e70: 5249 4420 6d6f 6461 6c20 444f 4620 666f  RID modal DOF fo
+00013e80: 7220 7573 6520 696e 0a20 2020 2074 6865  r use in.    the
+00013e90: 2044 4d41 5020 2278 746d 6174 7269 7822   DMAP "xtmatrix"
+00013ea0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+00013eb0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00013ec0: 0a20 2020 2066 203a 2073 7472 696e 6720  .    f : string 
+00013ed0: 6f72 2066 696c 655f 6c69 6b65 206f 7220  or file_like or 
+00013ee0: 3120 6f72 204e 6f6e 650a 2020 2020 2020  1 or None.      
+00013ef0: 2020 4569 7468 6572 2061 206e 616d 6520    Either a name 
+00013f00: 6f66 2061 2066 696c 652c 206f 7220 6973  of a file, or is
+00013f10: 2061 2066 696c 655f 6c69 6b65 206f 626a   a file_like obj
+00013f20: 6563 7420 6173 2072 6574 7572 6e65 640a  ect as returned.
+00013f30: 2020 2020 2020 2020 6279 203a 6675 6e63          by :func
+00013f40: 3a60 6f70 656e 6020 6f72 203a 636c 6173  :`open` or :clas
+00013f50: 733a 6069 6f2e 5374 7269 6e67 494f 602e  s:`io.StringIO`.
+00013f60: 2049 6e70 7574 2061 7320 696e 7465 6765   Input as intege
+00013f70: 7220 3120 746f 0a20 2020 2020 2020 2077  r 1 to.        w
+00013f80: 7269 7465 2074 6f20 7374 646f 7574 2e20  rite to stdout. 
+00013f90: 4361 6e20 616c 736f 2062 6520 7468 6520  Can also be the 
+00013fa0: 6e61 6d65 206f 6620 6120 6469 7265 6374  name of a direct
+00013fb0: 6f72 7920 6f72 204e 6f6e 653b 0a20 2020  ory or None;.   
+00013fc0: 2020 2020 2069 6e20 7468 6573 6520 6361       in these ca
+00013fd0: 7365 732c 2061 2047 5549 2069 7320 6f70  ses, a GUI is op
+00013fe0: 656e 6564 2066 6f72 2066 696c 6520 7365  ened for file se
+00013ff0: 6c65 6374 696f 6e2e 0a20 2020 2073 7461  lection..    sta
+00014000: 7274 6772 6964 203a 2069 6e74 6567 6572  rtgrid : integer
+00014010: 0a20 2020 2020 2020 2054 6865 2073 7461  .        The sta
+00014020: 7274 2049 4420 666f 7220 7468 6520 6d6f  rt ID for the mo
+00014030: 6461 6c20 6772 6964 7320 7468 6174 206e  dal grids that n
+00014040: 6565 6420 746f 2062 6520 6173 7369 676e  eed to be assign
+00014050: 6564 2074 6f0a 2020 2020 2020 2020 7468  ed to.        th
+00014060: 6520 512d 7365 7420 616e 6420 432d 7365  e Q-set and C-se
+00014070: 742e 2041 6e79 2065 7874 7261 2044 4f46  t. Any extra DOF
+00014080: 2061 7265 2061 7373 6967 6e65 6420 746f   are assigned to
+00014090: 2074 6865 2043 2d73 6574 2e0a 2020 2020   the C-set..    
+000140a0: 2020 2020 4372 6561 7465 6420 6772 6964      Created grid
+000140b0: 2049 4473 2077 696c 6c20 6265 2073 6571   IDs will be seq
+000140c0: 7565 6e74 6961 6c2e 0a20 2020 206e 7120  uential..    nq 
+000140d0: 3a20 696e 7465 6765 720a 2020 2020 2020  : integer.      
+000140e0: 2020 4e75 6d62 6572 206f 6620 6d6f 6461    Number of moda
+000140f0: 6c20 444f 460a 0a20 2020 2052 6574 7572  l DOF..    Retur
+00014100: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00014110: 2020 204e 6f6e 650a 0a20 2020 2045 7861     None..    Exa
+00014120: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00014130: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
+00014140: 7079 7965 7469 2069 6d70 6f72 7420 6e61  pyyeti import na
+00014150: 7374 7261 6e0a 2020 2020 3e3e 3e20 696d  stran.    >>> im
+00014160: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+00014170: 0a20 2020 203e 3e3e 206e 6173 7472 616e  .    >>> nastran
+00014180: 2e77 7471 6373 6574 2831 2c20 3939 3030  .wtqcset(1, 9900
+00014190: 3031 2c20 3134 290a 2020 2020 5153 4554  01, 14).    QSET
+000141a0: 3120 2020 2020 3132 3334 3536 2020 3939  1     123456  99
+000141b0: 3030 3031 2054 4852 5520 2020 2020 3939  0001 THRU     99
+000141c0: 3030 3032 0a20 2020 2051 5345 5431 2020  0002.    QSET1  
+000141d0: 2020 2020 2020 2031 3220 2039 3930 3030         12  99000
+000141e0: 330a 2020 2020 4353 4554 3120 2020 2020  3.    CSET1     
+000141f0: 2020 3334 3536 2020 3939 3030 3033 0a20    3456  990003. 
+00014200: 2020 2022 2222 0a20 2020 206e 6772 6964     """.    ngrid
+00014210: 7320 3d20 286e 7120 2b20 3529 202f 2f20  s = (nq + 5) // 
+00014220: 360a 2020 2020 656e 6467 7269 6420 3d20  6.    endgrid = 
+00014230: 7374 6172 7467 7269 6420 2b20 6e67 7269  startgrid + ngri
+00014240: 6473 202d 2031 0a20 2020 2078 646f 6620  ds - 1.    xdof 
+00014250: 3d20 6e71 202d 2036 202a 2028 6e67 7269  = nq - 6 * (ngri
+00014260: 6473 202d 2031 290a 2020 2020 7864 6f66  ds - 1).    xdof
+00014270: 7320 3d20 2231 3233 3435 3622 5b3a 7864  s = "123456"[:xd
+00014280: 6f66 5d0a 2020 2020 6364 6f66 7320 3d20  of].    cdofs = 
+00014290: 2231 3233 3435 3622 5b78 646f 663a 5d0a  "123456"[xdof:].
+000142a0: 2020 2020 2320 7772 6974 6520 7173 6574      # write qset
+000142b0: 2061 6e64 2063 7365 7420 6361 7264 733a   and cset cards:
+000142c0: 0a20 2020 2069 6620 7864 6f66 203d 3d20  .    if xdof == 
+000142d0: 363a 0a20 2020 2020 2020 2069 6620 6e67  6:.        if ng
+000142e0: 7269 6473 203e 2031 3a0a 2020 2020 2020  rids > 1:.      
+000142f0: 2020 2020 2020 662e 7772 6974 6528 0a20        f.write(. 
+00014300: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014310: 227b 2751 5345 5431 273a 3c38 737d 7b31  "{'QSET1':<8s}{1
+00014320: 3233 3435 363a 3864 7d7b 7374 6172 7467  23456:8d}{startg
+00014330: 7269 643a 3864 7d7b 2720 5448 5255 2027  rid:8d}{' THRU '
+00014340: 3a3c 3873 7d7b 656e 6467 7269 643a 3864  :<8s}{endgrid:8d
+00014350: 7d5c 6e22 0a20 2020 2020 2020 2020 2020  }\n".           
+00014360: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+00014370: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+00014380: 7269 7465 2866 227b 2751 5345 5431 273a  rite(f"{'QSET1':
+00014390: 3c38 737d 7b31 3233 3435 363a 3864 7d7b  <8s}{123456:8d}{
+000143a0: 7374 6172 7467 7269 643a 3864 7d5c 6e22  startgrid:8d}\n"
+000143b0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+000143c0: 2020 2020 6966 206e 6772 6964 7320 3e20      if ngrids > 
+000143d0: 323a 0a20 2020 2020 2020 2020 2020 2066  2:.            f
+000143e0: 2e77 7269 7465 280a 2020 2020 2020 2020  .write(.        
+000143f0: 2020 2020 2020 2020 6622 7b27 5153 4554          f"{'QSET
+00014400: 3127 3a3c 3873 7d7b 3132 3334 3536 3a38  1':<8s}{123456:8
+00014410: 647d 7b73 7461 7274 6772 6964 3a38 647d  d}{startgrid:8d}
+00014420: 7b27 2054 4852 5520 273a 3c38 737d 220a  {' THRU ':<8s}".
+00014430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014440: 6622 7b65 6e64 6772 6964 202d 2031 3a38  f"{endgrid - 1:8
+00014450: 647d 5c6e 220a 2020 2020 2020 2020 2020  d}\n".          
+00014460: 2020 290a 2020 2020 2020 2020 656c 6966    ).        elif
+00014470: 206e 6772 6964 7320 3d3d 2032 3a0a 2020   ngrids == 2:.  
+00014480: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00014490: 6528 6622 7b27 5153 4554 3127 3a3c 3873  e(f"{'QSET1':<8s
+000144a0: 7d7b 3132 3334 3536 3a38 647d 7b73 7461  }{123456:8d}{sta
+000144b0: 7274 6772 6964 3a38 647d 5c6e 2229 0a20  rtgrid:8d}\n"). 
+000144c0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+000144d0: 227b 2751 5345 5431 273a 3c38 737d 7b78  "{'QSET1':<8s}{x
+000144e0: 646f 6673 3a3e 3873 7d7b 656e 6467 7269  dofs:>8s}{endgri
+000144f0: 643a 3864 7d5c 6e22 290a 2020 2020 2020  d:8d}\n").      
+00014500: 2020 662e 7772 6974 6528 6622 7b27 4353    f.write(f"{'CS
+00014510: 4554 3127 3a3c 3873 7d7b 6364 6f66 733a  ET1':<8s}{cdofs:
+00014520: 3e38 737d 7b65 6e64 6772 6964 3a38 647d  >8s}{endgrid:8d}
+00014530: 5c6e 2229 0a0a 0a40 6775 6974 6f6f 6c73  \n")...@guitools
+00014540: 2e77 7269 7465 5f74 6578 745f 6669 6c65  .write_text_file
+00014550: 0a64 6566 2077 7472 6265 3228 662c 2065  .def wtrbe2(f, e
+00014560: 6964 2c20 696e 6465 702c 2064 6f66 2c20  id, indep, dof, 
+00014570: 6465 7029 3a0a 2020 2020 2222 220a 2020  dep):.    """.  
+00014580: 2020 5772 6974 6573 2061 204e 6173 7472    Writes a Nastr
+00014590: 616e 2052 4245 3220 6361 7264 2074 6f20  an RBE2 card to 
+000145a0: 6120 6669 6c65 2e0a 0a20 2020 2050 6172  a file...    Par
+000145b0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+000145c0: 2d2d 2d2d 2d2d 0a20 2020 2066 203a 2073  ------.    f : s
+000145d0: 7472 696e 6720 6f72 2066 696c 655f 6c69  tring or file_li
+000145e0: 6b65 206f 7220 3120 6f72 204e 6f6e 650a  ke or 1 or None.
+000145f0: 2020 2020 2020 2020 4569 7468 6572 2061          Either a
+00014600: 206e 616d 6520 6f66 2061 2066 696c 652c   name of a file,
+00014610: 206f 7220 6973 2061 2066 696c 655f 6c69   or is a file_li
+00014620: 6b65 206f 626a 6563 7420 6173 2072 6574  ke object as ret
+00014630: 7572 6e65 640a 2020 2020 2020 2020 6279  urned.        by
+00014640: 203a 6675 6e63 3a60 6f70 656e 6020 6f72   :func:`open` or
+00014650: 203a 636c 6173 733a 6069 6f2e 5374 7269   :class:`io.Stri
+00014660: 6e67 494f 602e 2049 6e70 7574 2061 7320  ngIO`. Input as 
+00014670: 696e 7465 6765 7220 3120 746f 0a20 2020  integer 1 to.   
+00014680: 2020 2020 2077 7269 7465 2074 6f20 7374       write to st
+00014690: 646f 7574 2e20 4361 6e20 616c 736f 2062  dout. Can also b
+000146a0: 6520 7468 6520 6e61 6d65 206f 6620 6120  e the name of a 
+000146b0: 6469 7265 6374 6f72 7920 6f72 204e 6f6e  directory or Non
+000146c0: 653b 0a20 2020 2020 2020 2069 6e20 7468  e;.        in th
+000146d0: 6573 6520 6361 7365 732c 2061 2047 5549  ese cases, a GUI
+000146e0: 2069 7320 6f70 656e 6564 2066 6f72 2066   is opened for f
+000146f0: 696c 6520 7365 6c65 6374 696f 6e2e 0a20  ile selection.. 
+00014700: 2020 2065 6964 203a 2069 6e74 6567 6572     eid : integer
+00014710: 0a20 2020 2020 2020 2045 6c65 6d65 6e74  .        Element
+00014720: 2049 440a 2020 2020 696e 6465 7020 3a20   ID.    indep : 
+00014730: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
+00014740: 496e 6465 7065 6e64 656e 7420 6772 6964  Independent grid
+00014750: 2049 442e 2041 6c6c 2036 2044 4f46 2061   ID. All 6 DOF a
+00014760: 7265 2061 7574 6f6d 6174 6963 616c 6c79  re automatically
+00014770: 2069 6e64 6570 656e 6465 6e74 0a20 2020   independent.   
+00014780: 2020 2020 2061 6e64 2061 7265 206e 6f74       and are not
+00014790: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
+000147a0: 646f 6620 3a20 696e 7465 6765 720a 2020  dof : integer.  
+000147b0: 2020 2020 2020 416e 2069 6e74 6567 6572        An integer
+000147c0: 2063 6f6e 6361 7465 6e61 7469 6f6e 206f   concatenation o
+000147d0: 6620 7468 6520 444f 4620 2865 783a 2031  f the DOF (ex: 1
+000147e0: 3233 3435 3629 2074 6861 7420 6170 706c  23456) that appl
+000147f0: 6965 730a 2020 2020 2020 2020 666f 7220  ies.        for 
+00014800: 616c 6c20 7468 6520 6465 7065 6e64 656e  all the dependen
+00014810: 7420 444f 462e 0a20 2020 2064 6570 203a  t DOF..    dep :
+00014820: 2031 6420 6172 7261 795f 6c69 6b65 0a20   1d array_like. 
+00014830: 2020 2020 2020 2056 6563 746f 7220 6f66         Vector of
+00014840: 2064 6570 656e 6465 6e74 2067 7269 6420   dependent grid 
+00014850: 4944 730a 0a20 2020 2052 6574 7572 6e73  IDs..    Returns
+00014860: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00014870: 204e 6f6e 650a 0a20 2020 2045 7861 6d70   None..    Examp
+00014880: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
+00014890: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
+000148a0: 7965 7469 2069 6d70 6f72 7420 6e61 7374  yeti import nast
+000148b0: 7261 6e0a 2020 2020 3e3e 3e20 696d 706f  ran.    >>> impo
+000148c0: 7274 206e 756d 7079 2061 7320 6e70 0a20  rt numpy as np. 
+000148d0: 2020 203e 3e3e 206e 6173 7472 616e 2e77     >>> nastran.w
+000148e0: 7472 6265 3228 312c 2031 2c20 3130 302c  trbe2(1, 1, 100,
+000148f0: 2031 3233 3435 362c 206e 702e 6172 616e   123456, np.aran
+00014900: 6765 2831 3031 2c20 3131 3129 290a 2020  ge(101, 111)).  
+00014910: 2020 5242 4532 2020 2020 2020 2020 2020    RBE2          
+00014920: 2031 2020 2020 2031 3030 2020 3132 3334   1     100  1234
+00014930: 3536 2020 2020 2031 3031 2020 2020 2031  56     101     1
+00014940: 3032 2020 2020 2031 3033 2020 2020 2031  02     103     1
+00014950: 3034 2020 2020 2031 3035 0a20 2020 2020  04     105.     
+00014960: 2020 2020 2020 2020 2020 2020 3130 3620              106 
+00014970: 2020 2020 3130 3720 2020 2020 3130 3820      107     108 
+00014980: 2020 2020 3130 3920 2020 2020 3131 300a      109     110.
+00014990: 2020 2020 2222 220a 2020 2020 662e 7772      """.    f.wr
+000149a0: 6974 6528 6622 5242 4532 2020 2020 7b65  ite(f"RBE2    {e
+000149b0: 6964 3a38 647d 7b69 6e64 6570 3a38 647d  id:8d}{indep:8d}
+000149c0: 7b64 6f66 3a38 647d 2229 0a20 2020 2077  {dof:8d}").    w
+000149d0: 746e 6173 696e 7473 2866 2c20 352c 2064  tnasints(f, 5, d
+000149e0: 6570 290a 0a0a 4067 7569 746f 6f6c 732e  ep)...@guitools.
+000149f0: 7772 6974 655f 7465 7874 5f66 696c 650a  write_text_file.
+00014a00: 6465 6620 7774 7262 6533 2866 2c20 6569  def wtrbe3(f, ei
+00014a10: 642c 2047 5249 445f 6465 702c 2044 4f46  d, GRID_dep, DOF
+00014a20: 5f64 6570 2c20 496e 645f 4c69 7374 2c20  _dep, Ind_List, 
+00014a30: 554d 5f4c 6973 743d 4e6f 6e65 2c20 616c  UM_List=None, al
+00014a40: 7068 613d 4e6f 6e65 293a 0a20 2020 2022  pha=None):.    "
+00014a50: 2222 0a20 2020 2057 7269 7465 7320 6120  "".    Writes a 
+00014a60: 4e61 7374 7261 6e20 5242 4533 2063 6172  Nastran RBE3 car
+00014a70: 6420 746f 2061 2066 696c 652e 0a0a 2020  d to a file...  
+00014a80: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00014a90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00014aa0: 6620 3a20 7374 7269 6e67 206f 7220 6669  f : string or fi
+00014ab0: 6c65 5f6c 696b 6520 6f72 2031 206f 7220  le_like or 1 or 
+00014ac0: 4e6f 6e65 0a20 2020 2020 2020 2045 6974  None.        Eit
+00014ad0: 6865 7220 6120 6e61 6d65 206f 6620 6120  her a name of a 
+00014ae0: 6669 6c65 2c20 6f72 2069 7320 6120 6669  file, or is a fi
+00014af0: 6c65 5f6c 696b 6520 6f62 6a65 6374 2061  le_like object a
+00014b00: 7320 7265 7475 726e 6564 0a20 2020 2020  s returned.     
+00014b10: 2020 2062 7920 3a66 756e 633a 606f 7065     by :func:`ope
+00014b20: 6e60 206f 7220 3a63 6c61 7373 3a60 696f  n` or :class:`io
+00014b30: 2e53 7472 696e 6749 4f60 2e20 496e 7075  .StringIO`. Inpu
+00014b40: 7420 6173 2069 6e74 6567 6572 2031 2074  t as integer 1 t
+00014b50: 6f0a 2020 2020 2020 2020 7772 6974 6520  o.        write 
+00014b60: 746f 2073 7464 6f75 742e 2043 616e 2061  to stdout. Can a
+00014b70: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
+00014b80: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
+00014b90: 7220 4e6f 6e65 3b0a 2020 2020 2020 2020  r None;.        
+00014ba0: 696e 2074 6865 7365 2063 6173 6573 2c20  in these cases, 
+00014bb0: 6120 4755 4920 6973 206f 7065 6e65 6420  a GUI is opened 
+00014bc0: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
+00014bd0: 6f6e 2e0a 2020 2020 6569 6420 3a20 696e  on..    eid : in
+00014be0: 7465 6765 720a 2020 2020 2020 2020 456c  teger.        El
+00014bf0: 656d 656e 7420 4944 0a20 2020 2047 5249  ement ID.    GRI
+00014c00: 445f 6465 7020 3a20 696e 7465 6765 720a  D_dep : integer.
+00014c10: 2020 2020 2020 2020 4465 7065 6e64 656e          Dependen
+00014c20: 7420 6772 6964 2049 440a 2020 2020 444f  t grid ID.    DO
+00014c30: 465f 6465 7020 3a20 696e 7465 6765 720a  F_dep : integer.
+00014c40: 2020 2020 2020 2020 416e 2069 6e74 6567          An integ
+00014c50: 6572 2063 6f6e 6361 7465 6e61 7469 6f6e  er concatenation
+00014c60: 206f 6620 7468 6520 444f 4620 2865 783a   of the DOF (ex:
+00014c70: 2031 3233 3435 3629 0a20 2020 2049 6e64   123456).    Ind
+00014c80: 5f4c 6973 7420 3a20 6c69 7374 0a20 2020  _List : list.   
+00014c90: 2020 2020 205b 2044 4f46 5f49 6e64 312c       [ DOF_Ind1,
+00014ca0: 2047 5249 4453 5f49 6e64 312c 2044 4f46   GRIDS_Ind1, DOF
+00014cb0: 5f49 6e64 322c 2047 5249 4453 5f49 6e64  _Ind2, GRIDS_Ind
+00014cc0: 322c 202e 2e2e 205d 2c20 7768 6572 653a  2, ... ], where:
+00014cd0: 3a0a 0a20 2020 2020 2020 2020 2020 2044  :..            D
+00014ce0: 4f46 5f49 6e64 3120 2020 3a20 3120 6f72  OF_Ind1   : 1 or
+00014cf0: 2032 2065 6c65 6d65 6e74 2061 7272 6179   2 element array
+00014d00: 5f6c 696b 6520 636f 6e74 6169 6e69 6e67  _like containing
+00014d10: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00014d20: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00014d30: 6d70 6f6e 656e 7420 444f 4620 2869 652c  mponent DOF (ie,
+00014d40: 2031 3233 3435 3629 206f 6620 7468 6520   123456) of the 
+00014d50: 6e6f 6465 7320 696e 0a20 2020 2020 2020  nodes in.       
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d70: 2020 4752 4944 535f 496e 6431 2061 6e64    GRIDS_Ind1 and
+00014d80: 2c20 6f70 7469 6f6e 616c 6c79 2c20 7468  , optionally, th
+00014d90: 6520 7765 6967 6874 696e 670a 2020 2020  e weighting.    
+00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014db0: 2020 2020 2066 6163 746f 7220 666f 7220       factor for 
+00014dc0: 7468 6573 6520 444f 462e 2049 6620 6e6f  these DOF. If no
+00014dd0: 7420 696e 7075 742c 2074 6865 0a20 2020  t input, the.   
+00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014df0: 2020 2020 2020 7765 6967 6874 696e 6720        weighting 
+00014e00: 6661 6374 6f72 2064 6566 6175 6c74 7320  factor defaults 
+00014e10: 746f 2031 2e30 2e0a 2020 2020 2020 2020  to 1.0..        
+00014e20: 2020 2020 4752 4944 535f 496e 6431 203a      GRIDS_Ind1 :
+00014e30: 2061 7272 6179 5f6c 696b 6520 6f66 206e   array_like of n
+00014e40: 6f64 6520 6964 7320 636f 7272 6573 706f  ode ids correspo
+00014e50: 6e64 696e 6720 746f 0a20 2020 2020 2020  nding to.       
+00014e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e70: 2020 444f 465f 496e 6431 0a20 2020 2020    DOF_Ind1.     
+00014e80: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+00014e90: 2020 2020 2020 2065 673a 2020 5b20 5b31         eg:  [ [1
+00014ea0: 3233 2c20 312e 325d 2c20 5b39 352c 2031  23, 1.2], [95, 1
+00014eb0: 3935 2c20 3130 3030 5d2c 2031 3233 3435  95, 1000], 12345
+00014ec0: 362c 2039 355d 0a0a 2020 2020 2020 2020  6, 95]..        
+00014ed0: 6049 6e64 5f4c 6973 7460 206d 7573 7420  `Ind_List` must 
+00014ee0: 6265 2065 7665 6e20 6c65 6e67 7468 2e0a  be even length..
+00014ef0: 0a20 2020 2055 4d5f 4c69 7374 203a 204e  .    UM_List : N
+00014f00: 6f6e 6520 6f72 206c 6973 743b 206f 7074  one or list; opt
+00014f10: 696f 6e61 6c0a 2020 2020 2020 2020 5b20  ional.        [ 
+00014f20: 4752 4944 5f4d 5345 5431 2c20 444f 465f  GRID_MSET1, DOF_
+00014f30: 4d53 4554 312c 2047 5249 445f 4d53 4554  MSET1, GRID_MSET
+00014f40: 322c 2044 4f46 5f4d 5345 5432 2c20 2e2e  2, DOF_MSET2, ..
+00014f50: 2e20 5d20 7768 6572 653a 3a0a 0a20 2020  . ] where::..   
+00014f60: 2020 2020 2020 2020 2020 2047 5249 445f             GRID_
+00014f70: 4d53 4554 3120 3a20 6669 7273 7420 6772  MSET1 : first gr
+00014f80: 6964 2069 6e20 7468 6520 4d2d 7365 740a  id in the M-set.
+00014f90: 2020 2020 2020 2020 2020 2020 2020 444f                DO
+00014fa0: 465f 4d53 4554 3120 203a 2044 4f46 206f  F_MSET1  : DOF o
+00014fb0: 6620 6669 7273 7420 6772 6964 2069 6e20  f first grid in 
+00014fc0: 4d2d 7365 7420 2869 6e74 6567 6572 2073  M-set (integer s
+00014fd0: 7562 7365 740a 2020 2020 2020 2020 2020  ubset.          
+00014fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ff0: 206f 6620 3132 3334 3536 292e 204e 6f20   of 123456). No 
+00015000: 7765 6967 6874 696e 6720 6661 6374 6f72  weighting factor
+00015010: 7320 6172 650a 2020 2020 2020 2020 2020  s are.          
+00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015030: 2061 6c6c 6f77 6564 2068 6572 652e 0a20   allowed here.. 
+00015040: 2020 2020 2020 2020 2020 2020 2047 5249               GRI
+00015050: 445f 4d53 4554 3220 3a20 7365 636f 6e64  D_MSET2 : second
+00015060: 2067 7269 6420 696e 2074 6865 204d 2d73   grid in the M-s
+00015070: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
+00015080: 2044 4f46 5f4d 5345 5432 2020 3a20 444f   DOF_MSET2  : DO
+00015090: 4620 6f66 2073 6563 6f6e 6420 6772 6964  F of second grid
+000150a0: 2069 6e20 4d2d 7365 740a 2020 2020 2020   in M-set.      
+000150b0: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+000150c0: 2061 6c70 6861 203a 204e 6f6e 6520 6f72   alpha : None or
+000150d0: 2073 7472 696e 673b 206f 7074 696f 6e61   string; optiona
+000150e0: 6c0a 2020 2020 2020 2020 5468 6572 6d61  l.        Therma
+000150f0: 6c20 6578 7061 6e73 696f 6e20 636f 6566  l expansion coef
+00015100: 6669 6369 656e 7420 696e 2061 2038 2d63  ficient in a 8-c
+00015110: 6861 7220 7374 7269 6e67 2028 6f72 206c  har string (or l
+00015120: 6573 7329 2e0a 0a20 2020 2052 6574 7572  ess)...    Retur
+00015130: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00015140: 2020 204e 6f6e 650a 0a20 2020 2045 7861     None..    Exa
+00015150: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00015160: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
+00015170: 7079 7965 7469 2069 6d70 6f72 7420 6e61  pyyeti import na
+00015180: 7374 7261 6e0a 2020 2020 3e3e 3e20 6e61  stran.    >>> na
+00015190: 7374 7261 6e2e 7774 7262 6533 2831 2c20  stran.wtrbe3(1, 
+000151a0: 3130 302c 2039 3930 302c 2031 3233 3435  100, 9900, 12345
+000151b0: 362c 0a20 2020 202e 2e2e 2020 2020 2020  6,.    ...      
+000151c0: 2020 2020 2020 2020 2020 5b31 3233 2c20            [123, 
+000151d0: 5b39 3930 312c 2039 3930 322c 2039 3930  [9901, 9902, 990
+000151e0: 332c 2039 3930 345d 2c0a 2020 2020 2e2e  3, 9904],.    ..
+000151f0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00015200: 2020 3132 3334 3536 2c20 5b34 3530 3030    123456, [45000
+00015210: 312c 2032 3030 5d5d 290a 2020 2020 5242  1, 200]]).    RB
+00015220: 4533 2020 2020 2020 2020 2031 3030 2020  E3         100  
+00015230: 2020 2020 2020 2020 2020 3939 3030 2020            9900  
+00015240: 3132 3334 3536 2020 2031 2e30 3030 2020  123456   1.000  
+00015250: 2020 2031 3233 2020 2020 3939 3031 2020     123    9901  
+00015260: 2020 3939 3032 0a20 2020 2020 2020 2020    9902.         
+00015270: 2020 2020 2020 2039 3930 3320 2020 2039         9903    9
+00015280: 3930 3420 2020 312e 3030 3020 2031 3233  904   1.000  123
+00015290: 3435 3620 2034 3530 3030 3120 2020 2020  456  450001     
+000152a0: 3230 300a 2020 2020 3e3e 3e20 6e61 7374  200.    >>> nast
+000152b0: 7261 6e2e 7774 7262 6533 2831 2c20 3130  ran.wtrbe3(1, 10
+000152c0: 302c 2039 3930 302c 2031 3233 3435 362c  0, 9900, 123456,
+000152d0: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+000152e0: 2020 2020 2020 2020 5b31 3233 2c20 5b39          [123, [9
+000152f0: 3930 312c 2039 3930 322c 2039 3930 332c  901, 9902, 9903,
+00015300: 2039 3930 345d 2c0a 2020 2020 2e2e 2e20   9904],.    ... 
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 5b31 3233 3435 362c 2031 2e32 5d2c 205b  [123456, 1.2], [
+00015330: 3435 3030 3031 2c20 3230 305d 5d2c 0a20  450001, 200]],. 
+00015340: 2020 202e 2e2e 2020 2020 2020 2020 2020     ...          
+00015350: 2020 2020 2020 554d 5f4c 6973 743d 5b39        UM_List=[9
+00015360: 3930 312c 2031 322c 2039 3930 322c 2033  901, 12, 9902, 3
+00015370: 2c20 3939 3033 2c20 3132 2c20 3939 3034  , 9903, 12, 9904
+00015380: 2c20 335d 2c0a 2020 2020 2e2e 2e20 2020  , 3],.    ...   
+00015390: 2020 2020 2020 2020 2020 2020 2061 6c70               alp
+000153a0: 6861 3d27 362e 3565 2d36 2729 0a20 2020  ha='6.5e-6').   
+000153b0: 2052 4245 3320 2020 2020 2020 2020 3130   RBE3         10
+000153c0: 3020 2020 2020 2020 2020 2020 2039 3930  0            990
+000153d0: 3020 2031 3233 3435 3620 2020 312e 3030  0  123456   1.00
+000153e0: 3020 2020 2020 3132 3320 2020 2039 3930  0     123    990
+000153f0: 3120 2020 2039 3930 320a 2020 2020 2020  1    9902.      
+00015400: 2020 2020 2020 2020 2020 3939 3033 2020            9903  
+00015410: 2020 3939 3034 2020 2031 2e32 3030 2020    9904   1.200  
+00015420: 3132 3334 3536 2020 3435 3030 3031 2020  123456  450001  
+00015430: 2020 2032 3030 0a20 2020 2020 2020 2020     200.         
+00015440: 2020 2055 4d20 2020 2020 2020 2020 2039     UM          9
+00015450: 3930 3120 2020 2020 2031 3220 2020 2039  901      12    9
+00015460: 3930 3220 2020 2020 2020 3320 2020 2039  902       3    9
+00015470: 3930 3320 2020 2020 2031 320a 2020 2020  903      12.    
+00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015490: 2020 2020 3939 3034 2020 2020 2020 2033      9904       3
+000154a0: 0a20 2020 2020 2020 2020 2020 2041 4c50  .            ALP
+000154b0: 4841 2020 2020 2036 2e35 652d 360a 2020  HA     6.5e-6.  
+000154c0: 2020 2222 220a 2020 2020 6966 206c 656e    """.    if len
+000154d0: 2849 6e64 5f4c 6973 7429 2026 2031 3a0a  (Ind_List) & 1:.
+000154e0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+000154f0: 6c75 6545 7272 6f72 2866 2260 496e 645f  lueError(f"`Ind_
+00015500: 4c69 7374 6020 6d75 7374 2068 6176 6520  List` must have 
+00015510: 6576 656e 206c 656e 6774 6820 2869 7420  even length (it 
+00015520: 6973 207b 6c65 6e28 496e 645f 4c69 7374  is {len(Ind_List
+00015530: 297d 2922 290a 0a20 2020 2066 2e77 7269  )})")..    f.wri
+00015540: 7465 2866 2252 4245 3320 2020 207b 6569  te(f"RBE3    {ei
+00015550: 643a 3864 7d20 2020 2020 2020 207b 4752  d:8d}        {GR
+00015560: 4944 5f64 6570 3a38 647d 7b44 4f46 5f64  ID_dep:8d}{DOF_d
+00015570: 6570 3a38 647d 2229 0a20 2020 2066 6965  ep:8d}").    fie
+00015580: 6c64 203d 2035 0a0a 2020 2020 6465 6620  ld = 5..    def 
+00015590: 5f49 6e63 5f46 6965 6c64 2866 2c20 6669  _Inc_Field(f, fi
+000155a0: 656c 6429 3a0a 2020 2020 2020 2020 6669  eld):.        fi
+000155b0: 656c 6420 2b3d 2031 0a20 2020 2020 2020  eld += 1.       
+000155c0: 2069 6620 6669 656c 6420 3d3d 2031 303a   if field == 10:
+000155d0: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+000155e0: 7269 7465 2822 5c6e 2020 2020 2020 2020  rite("\n        
+000155f0: 2229 0a20 2020 2020 2020 2020 2020 2066  ").            f
+00015600: 6965 6c64 203d 2032 0a20 2020 2020 2020  ield = 2.       
+00015610: 2072 6574 7572 6e20 6669 656c 640a 0a20   return field.. 
+00015620: 2020 2023 206c 6f6f 7020 6f76 6572 2069     # loop over i
+00015630: 6e64 6570 656e 6465 6e74 730a 2020 2020  ndependents.    
+00015640: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+00015650: 2c20 6c65 6e28 496e 645f 4c69 7374 292c  , len(Ind_List),
+00015660: 2032 293a 0a20 2020 2020 2020 2044 4f46   2):.        DOF
+00015670: 5f69 6e64 203d 206e 702e 6174 6c65 6173  _ind = np.atleas
+00015680: 745f 3164 2849 6e64 5f4c 6973 745b 6a5d  t_1d(Ind_List[j]
+00015690: 290a 2020 2020 2020 2020 4752 4944 535f  ).        GRIDS_
+000156a0: 696e 6420 3d20 6e70 2e61 746c 6561 7374  ind = np.atleast
+000156b0: 5f31 6428 496e 645f 4c69 7374 5b6a 202b  _1d(Ind_List[j +
+000156c0: 2031 5d29 0a20 2020 2020 2020 2064 6f66   1]).        dof
+000156d0: 203d 2069 6e74 2844 4f46 5f69 6e64 5b30   = int(DOF_ind[0
+000156e0: 5d29 0a20 2020 2020 2020 2069 6620 6c65  ]).        if le
+000156f0: 6e28 444f 465f 696e 6429 203d 3d20 323a  n(DOF_ind) == 2:
+00015700: 0a20 2020 2020 2020 2020 2020 2077 7420  .            wt 
+00015710: 3d20 666c 6f61 7428 444f 465f 696e 645b  = float(DOF_ind[
+00015720: 315d 290a 2020 2020 2020 2020 656c 7365  1]).        else
+00015730: 3a0a 2020 2020 2020 2020 2020 2020 7774  :.            wt
+00015740: 203d 2031 2e30 0a20 2020 2020 2020 2066   = 1.0.        f
+00015750: 6965 6c64 203d 205f 496e 635f 4669 656c  ield = _Inc_Fiel
+00015760: 6428 662c 2066 6965 6c64 290a 2020 2020  d(f, field).    
+00015770: 2020 2020 662e 7772 6974 6528 6622 7b77      f.write(f"{w
+00015780: 743a 382e 3366 7d22 290a 2020 2020 2020  t:8.3f}").      
+00015790: 2020 6669 656c 6420 3d20 5f49 6e63 5f46    field = _Inc_F
+000157a0: 6965 6c64 2866 2c20 6669 656c 6429 0a20  ield(f, field). 
+000157b0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+000157c0: 227b 646f 663a 3864 7d22 290a 2020 2020  "{dof:8d}").    
+000157d0: 2020 2020 666f 7220 6720 696e 2047 5249      for g in GRI
+000157e0: 4453 5f69 6e64 3a0a 2020 2020 2020 2020  DS_ind:.        
+000157f0: 2020 2020 6669 656c 6420 3d20 5f49 6e63      field = _Inc
+00015800: 5f46 6965 6c64 2866 2c20 6669 656c 6429  _Field(f, field)
+00015810: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
+00015820: 7269 7465 2866 227b 673a 3864 7d22 290a  rite(f"{g:8d}").
+00015830: 2020 2020 662e 7772 6974 6528 225c 6e22      f.write("\n"
+00015840: 290a 0a20 2020 2064 6566 205f 496e 635f  )..    def _Inc_
+00015850: 554d 5f46 6965 6c64 2866 2c20 6669 656c  UM_Field(f, fiel
+00015860: 6429 3a0a 2020 2020 2020 2020 6669 656c  d):.        fiel
+00015870: 6420 2b3d 2031 0a20 2020 2020 2020 2069  d += 1.        i
+00015880: 6620 6669 656c 6420 3d3d 2039 3a0a 2020  f field == 9:.  
+00015890: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+000158a0: 6528 225c 6e20 2020 2020 2020 2020 2020  e("\n           
+000158b0: 2020 2020 2022 290a 2020 2020 2020 2020       ").        
+000158c0: 2020 2020 6669 656c 6420 3d20 330a 2020      field = 3.  
+000158d0: 2020 2020 2020 7265 7475 726e 2066 6965        return fie
+000158e0: 6c64 0a0a 2020 2020 6966 2055 4d5f 4c69  ld..    if UM_Li
+000158f0: 7374 2069 7320 6e6f 7420 4e6f 6e65 3a0a  st is not None:.
+00015900: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00015910: 2220 2020 2020 2020 2055 4d20 2020 2020  "        UM     
+00015920: 2022 290a 2020 2020 2020 2020 6669 656c   ").        fiel
+00015930: 6420 3d20 320a 2020 2020 2020 2020 666f  d = 2.        fo
+00015940: 7220 6a20 696e 2055 4d5f 4c69 7374 3a0a  r j in UM_List:.
+00015950: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
+00015960: 6420 3d20 5f49 6e63 5f55 4d5f 4669 656c  d = _Inc_UM_Fiel
+00015970: 6428 662c 2066 6965 6c64 290a 2020 2020  d(f, field).    
+00015980: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00015990: 227b 3a38 647d 222e 666f 726d 6174 286a  "{:8d}".format(j
+000159a0: 2929 0a20 2020 2020 2020 2066 2e77 7269  )).        f.wri
+000159b0: 7465 2822 5c6e 2229 0a0a 2020 2020 6966  te("\n")..    if
+000159c0: 2061 6c70 6861 2069 7320 6e6f 7420 4e6f   alpha is not No
+000159d0: 6e65 3a0a 2020 2020 2020 2020 662e 7772  ne:.        f.wr
+000159e0: 6974 6528 6622 2020 2020 2020 2020 414c  ite(f"        AL
+000159f0: 5048 4120 2020 7b61 6c70 6861 3a3e 3873  PHA   {alpha:>8s
+00015a00: 7d5c 6e22 290a 0a0a 4067 7569 746f 6f6c  }\n")...@guitool
+00015a10: 732e 7772 6974 655f 7465 7874 5f66 696c  s.write_text_fil
+00015a20: 650a 6465 6620 7774 7365 7365 7428 662c  e.def wtseset(f,
+00015a30: 2073 7570 6572 6964 2c20 6772 6964 7329   superid, grids)
+00015a40: 3a0a 2020 2020 2222 220a 2020 2020 5772  :.    """.    Wr
+00015a50: 6974 6573 2061 204e 6173 7472 616e 2053  ites a Nastran S
+00015a60: 4553 4554 2063 6172 6420 746f 2061 2066  ESET card to a f
+00015a70: 696c 652e 0a0a 2020 2020 5061 7261 6d65  ile...    Parame
+00015a80: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00015a90: 2d2d 2d0a 2020 2020 6620 3a20 7374 7269  ---.    f : stri
+00015aa0: 6e67 206f 7220 6669 6c65 5f6c 696b 6520  ng or file_like 
+00015ab0: 6f72 2031 206f 7220 4e6f 6e65 0a20 2020  or 1 or None.   
+00015ac0: 2020 2020 2045 6974 6865 7220 6120 6e61       Either a na
+00015ad0: 6d65 206f 6620 6120 6669 6c65 2c20 6f72  me of a file, or
+00015ae0: 2069 7320 6120 6669 6c65 5f6c 696b 6520   is a file_like 
+00015af0: 6f62 6a65 6374 2061 7320 7265 7475 726e  object as return
+00015b00: 6564 0a20 2020 2020 2020 2062 7920 3a66  ed.        by :f
+00015b10: 756e 633a 606f 7065 6e60 206f 7220 3a63  unc:`open` or :c
+00015b20: 6c61 7373 3a60 696f 2e53 7472 696e 6749  lass:`io.StringI
+00015b30: 4f60 2e20 496e 7075 7420 6173 2069 6e74  O`. Input as int
+00015b40: 6567 6572 2031 2074 6f0a 2020 2020 2020  eger 1 to.      
+00015b50: 2020 7772 6974 6520 746f 2073 7464 6f75    write to stdou
+00015b60: 742e 2043 616e 2061 6c73 6f20 6265 2074  t. Can also be t
+00015b70: 6865 206e 616d 6520 6f66 2061 2064 6972  he name of a dir
+00015b80: 6563 746f 7279 206f 7220 4e6f 6e65 3b0a  ectory or None;.
+00015b90: 2020 2020 2020 2020 696e 2074 6865 7365          in these
+00015ba0: 2063 6173 6573 2c20 6120 4755 4920 6973   cases, a GUI is
+00015bb0: 206f 7065 6e65 6420 666f 7220 6669 6c65   opened for file
+00015bc0: 2073 656c 6563 7469 6f6e 2e0a 2020 2020   selection..    
+00015bd0: 7375 7065 7269 643a 2069 6e74 6567 6572  superid: integer
+00015be0: 0a20 2020 2020 2020 2053 7570 6572 656c  .        Superel
+00015bf0: 656d 656e 7420 4944 0a20 2020 2067 7269  ement ID.    gri
+00015c00: 6473 203a 2031 6420 6172 7261 795f 6c69  ds : 1d array_li
+00015c10: 6b65 0a20 2020 2020 2020 2056 6563 746f  ke.        Vecto
+00015c20: 7220 6f66 2067 7269 6420 6964 732e 0a0a  r of grid ids...
+00015c30: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00015c40: 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65  -------.    None
+00015c50: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
+00015c60: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00015c70: 3e3e 3e20 6672 6f6d 2070 7979 6574 6920  >>> from pyyeti 
+00015c80: 696d 706f 7274 206e 6173 7472 616e 0a20  import nastran. 
+00015c90: 2020 203e 3e3e 2069 6d70 6f72 7420 6e75     >>> import nu
+00015ca0: 6d70 7920 6173 206e 700a 2020 2020 3e3e  mpy as np.    >>
+00015cb0: 3e20 6e61 7374 7261 6e2e 7774 7365 7365  > nastran.wtsese
+00015cc0: 7428 312c 2031 3030 2c20 6e70 2e61 7261  t(1, 100, np.ara
+00015cd0: 6e67 6528 312c 2032 3629 290a 2020 2020  nge(1, 26)).    
+00015ce0: 5345 5345 5420 2020 2020 2020 2031 3030  SESET        100
+00015cf0: 2020 2020 2020 2031 2020 2020 2020 2032         1       2
+00015d00: 2020 2020 2020 2033 2020 2020 2020 2034         3       4
+00015d10: 2020 2020 2020 2035 2020 2020 2020 2036         5       6
+00015d20: 2020 2020 2020 2037 0a20 2020 2053 4553         7.    SES
+00015d30: 4554 2020 2020 2020 2020 3130 3020 2020  ET        100   
+00015d40: 2020 2020 3820 2020 2020 2020 3920 2020      8       9   
+00015d50: 2020 2031 3020 2020 2020 2031 3120 2020     10      11   
+00015d60: 2020 2031 3220 2020 2020 2031 3320 2020     12      13   
+00015d70: 2020 2031 340a 2020 2020 5345 5345 5420     14.    SESET 
+00015d80: 2020 2020 2020 2031 3030 2020 2020 2020         100      
+00015d90: 3135 2020 2020 2020 3136 2020 2020 2020  15      16      
+00015da0: 3137 2020 2020 2020 3138 2020 2020 2020  17      18      
+00015db0: 3139 2020 2020 2020 3230 2020 2020 2020  19      20      
+00015dc0: 3231 0a20 2020 2053 4553 4554 2020 2020  21.    SESET    
+00015dd0: 2020 2020 3130 3020 2020 2020 2032 3220      100      22 
+00015de0: 2020 2020 2032 3320 2020 2020 2032 3420       23      24 
+00015df0: 2020 2020 2032 350a 2020 2020 2222 220a       25.    """.
+00015e00: 2020 2020 6e20 3d20 6c65 6e28 6772 6964      n = len(grid
+00015e10: 7329 0a20 2020 2023 2037 2067 7269 6473  s).    # 7 grids
+00015e20: 2070 6572 2053 4553 4554 3a0a 2020 2020   per SESET:.    
+00015e30: 6672 6d20 3d20 2253 4553 4554 2020 207b  frm = "SESET   {
+00015e40: 3a38 647d 2220 2b20 227b 3a38 647d 2220  :8d}" + "{:8d}" 
+00015e50: 2a20 3720 2b20 225c 6e22 0a20 2020 2069  * 7 + "\n".    i
+00015e60: 203d 2030 0a20 2020 2077 6869 6c65 2069   = 0.    while i
+00015e70: 202b 2037 203c 3d20 6e3a 0a20 2020 2020   + 7 <= n:.     
+00015e80: 2020 2066 2e77 7269 7465 2866 726d 2e66     f.write(frm.f
+00015e90: 6f72 6d61 7428 7375 7065 7269 642c 202a  ormat(superid, *
+00015ea0: 6772 6964 735b 6920 3a20 6920 2b20 375d  grids[i : i + 7]
+00015eb0: 2929 0a20 2020 2020 2020 2069 202b 3d20  )).        i += 
+00015ec0: 370a 2020 2020 6966 2069 203c 206e 3a0a  7.    if i < n:.
+00015ed0: 2020 2020 2020 2020 6672 6d20 3d20 2253          frm = "S
+00015ee0: 4553 4554 2020 207b 3a38 647d 2220 2b20  ESET   {:8d}" + 
+00015ef0: 227b 3a38 647d 2220 2a20 286e 202d 2069  "{:8d}" * (n - i
+00015f00: 2920 2b20 225c 6e22 0a20 2020 2020 2020  ) + "\n".       
+00015f10: 2066 2e77 7269 7465 2866 726d 2e66 6f72   f.write(frm.for
+00015f20: 6d61 7428 7375 7065 7269 642c 202a 6772  mat(superid, *gr
+00015f30: 6964 735b 693a 5d29 290a 0a0a 4067 7569  ids[i:]))...@gui
+00015f40: 746f 6f6c 732e 7772 6974 655f 7465 7874  tools.write_text
+00015f50: 5f66 696c 650a 6465 6620 7774 7365 7428  _file.def wtset(
+00015f60: 662c 2073 6574 6964 2c20 6964 7329 3a0a  f, setid, ids):.
+00015f70: 2020 2020 2222 220a 2020 2020 5772 6974      """.    Writ
+00015f80: 6573 2061 204e 6173 7472 616e 2063 6173  es a Nastran cas
+00015f90: 652d 636f 6e74 726f 6c20 5345 5420 6361  e-control SET ca
+00015fa0: 7264 2074 6f20 6120 6669 6c65 2e0a 0a20  rd to a file... 
+00015fb0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00015fc0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00015fd0: 2066 203a 2073 7472 696e 6720 6f72 2066   f : string or f
+00015fe0: 696c 655f 6c69 6b65 206f 7220 3120 6f72  ile_like or 1 or
+00015ff0: 204e 6f6e 650a 2020 2020 2020 2020 4569   None.        Ei
+00016000: 7468 6572 2061 206e 616d 6520 6f66 2061  ther a name of a
+00016010: 2066 696c 652c 206f 7220 6973 2061 2066   file, or is a f
+00016020: 696c 655f 6c69 6b65 206f 626a 6563 7420  ile_like object 
+00016030: 6173 2072 6574 7572 6e65 640a 2020 2020  as returned.    
+00016040: 2020 2020 6279 203a 6675 6e63 3a60 6f70      by :func:`op
+00016050: 656e 6020 6f72 203a 636c 6173 733a 6069  en` or :class:`i
+00016060: 6f2e 5374 7269 6e67 494f 602e 2049 6e70  o.StringIO`. Inp
+00016070: 7574 2061 7320 696e 7465 6765 7220 3120  ut as integer 1 
+00016080: 746f 0a20 2020 2020 2020 2077 7269 7465  to.        write
+00016090: 2074 6f20 7374 646f 7574 2e20 4361 6e20   to stdout. Can 
+000160a0: 616c 736f 2062 6520 7468 6520 6e61 6d65  also be the name
+000160b0: 206f 6620 6120 6469 7265 6374 6f72 7920   of a directory 
+000160c0: 6f72 204e 6f6e 653b 0a20 2020 2020 2020  or None;.       
+000160d0: 2069 6e20 7468 6573 6520 6361 7365 732c   in these cases,
+000160e0: 2061 2047 5549 2069 7320 6f70 656e 6564   a GUI is opened
+000160f0: 2066 6f72 2066 696c 6520 7365 6c65 6374   for file select
+00016100: 696f 6e2e 0a20 2020 2073 6574 6964 3a20  ion..    setid: 
+00016110: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
+00016120: 5365 7420 4944 0a20 2020 2069 6473 203a  Set ID.    ids :
+00016130: 2031 6420 6172 7261 795f 6c69 6b65 0a20   1d array_like. 
+00016140: 2020 2020 2020 2056 6563 746f 7220 6f66         Vector of
+00016150: 2049 4473 0a0a 2020 2020 5265 7475 726e   IDs..    Return
+00016160: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00016170: 2020 4e6f 6e65 0a0a 2020 2020 4578 616d    None..    Exam
+00016180: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+00016190: 2d0a 2020 2020 3e3e 3e20 6672 6f6d 2070  -.    >>> from p
+000161a0: 7979 6574 6920 696d 706f 7274 206e 6173  yyeti import nas
+000161b0: 7472 616e 0a20 2020 203e 3e3e 2069 6d70  tran.    >>> imp
+000161c0: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+000161d0: 2020 2020 3e3e 3e20 6e61 7374 7261 6e2e      >>> nastran.
+000161e0: 7774 7365 7428 312c 2031 3030 2c20 6e70  wtset(1, 100, np
+000161f0: 2e61 7261 6e67 6528 312c 2032 3629 290a  .arange(1, 26)).
+00016200: 2020 2020 5345 5420 3130 3020 3d20 312c      SET 100 = 1,
+00016210: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
+00016220: 372c 0a20 2020 2020 382c 2039 2c20 3130  7,.     8, 9, 10
+00016230: 2c20 3131 2c20 3132 2c20 3133 2c20 3134  , 11, 12, 13, 14
+00016240: 2c0a 2020 2020 2031 352c 2031 362c 2031  ,.     15, 16, 1
+00016250: 372c 2031 382c 2031 392c 2032 302c 2032  7, 18, 19, 20, 2
+00016260: 312c 0a20 2020 2020 3232 2c20 3233 2c20  1,.     22, 23, 
+00016270: 3234 2c20 3235 0a20 2020 2022 2222 0a20  24, 25.    """. 
+00016280: 2020 2066 2e77 7269 7465 2866 2253 4554     f.write(f"SET
+00016290: 207b 7365 7469 647d 203d 2229 0a20 2020   {setid} =").   
+000162a0: 206e 203d 206c 656e 2869 6473 290a 2020   n = len(ids).  
+000162b0: 2020 2320 3720 6964 7320 7065 7220 6c69    # 7 ids per li
+000162c0: 6e65 3a0a 2020 2020 6672 6d20 3d20 2220  ne:.    frm = " 
+000162d0: 7b3a 647d 2c22 202a 2037 202b 2022 5c6e  {:d}," * 7 + "\n
+000162e0: 220a 2020 2020 6920 3d20 300a 2020 2020  ".    i = 0.    
+000162f0: 7768 696c 6520 6920 2b20 3720 3c20 6e3a  while i + 7 < n:
+00016300: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+00016310: 2866 726d 2e66 6f72 6d61 7428 2a69 6473  (frm.format(*ids
+00016320: 5b69 203a 2069 202b 2037 5d29 290a 2020  [i : i + 7])).  
+00016330: 2020 2020 2020 6920 2b3d 2037 0a20 2020        i += 7.   
+00016340: 2066 726d 203d 2022 207b 3a64 7d2c 2220   frm = " {:d}," 
+00016350: 2a20 286e 202d 2069 202d 2031 2920 2b20  * (n - i - 1) + 
+00016360: 2220 7b3a 647d 5c6e 220a 2020 2020 662e  " {:d}\n".    f.
+00016370: 7772 6974 6528 6672 6d2e 666f 726d 6174  write(frm.format
+00016380: 282a 6964 735b 693a 5d29 290a 0a0a 4067  (*ids[i:]))...@g
+00016390: 7569 746f 6f6c 732e 7772 6974 655f 7465  uitools.write_te
+000163a0: 7874 5f66 696c 650a 6465 6620 7774 7273  xt_file.def wtrs
+000163b0: 706c 696e 6528 662c 2072 6964 2c20 6964  pline(f, rid, id
+000163c0: 732c 2044 6f4c 3d22 302e 3122 293a 0a20  s, DoL="0.1"):. 
+000163d0: 2020 2022 2222 0a20 2020 2057 7269 7465     """.    Write
+000163e0: 204e 6173 7472 616e 2052 5350 4c49 4e45   Nastran RSPLINE
+000163f0: 2063 6172 6428 7329 2e0a 0a20 2020 2050   card(s)...    P
+00016400: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00016410: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 203a  --------.    f :
+00016420: 2073 7472 696e 6720 6f72 2066 696c 655f   string or file_
+00016430: 6c69 6b65 206f 7220 3120 6f72 204e 6f6e  like or 1 or Non
+00016440: 650a 2020 2020 2020 2020 4569 7468 6572  e.        Either
+00016450: 2061 206e 616d 6520 6f66 2061 2066 696c   a name of a fil
+00016460: 652c 206f 7220 6973 2061 2066 696c 655f  e, or is a file_
+00016470: 6c69 6b65 206f 626a 6563 7420 6173 2072  like object as r
+00016480: 6574 7572 6e65 640a 2020 2020 2020 2020  eturned.        
+00016490: 6279 203a 6675 6e63 3a60 6f70 656e 6020  by :func:`open` 
+000164a0: 6f72 203a 636c 6173 733a 6069 6f2e 5374  or :class:`io.St
+000164b0: 7269 6e67 494f 602e 2049 6e70 7574 2061  ringIO`. Input a
+000164c0: 7320 696e 7465 6765 7220 3120 746f 0a20  s integer 1 to. 
+000164d0: 2020 2020 2020 2077 7269 7465 2074 6f20         write to 
+000164e0: 7374 646f 7574 2e20 4361 6e20 616c 736f  stdout. Can also
+000164f0: 2062 6520 7468 6520 6e61 6d65 206f 6620   be the name of 
+00016500: 6120 6469 7265 6374 6f72 7920 6f72 204e  a directory or N
+00016510: 6f6e 653b 0a20 2020 2020 2020 2069 6e20  one;.        in 
+00016520: 7468 6573 6520 6361 7365 732c 2061 2047  these cases, a G
+00016530: 5549 2069 7320 6f70 656e 6564 2066 6f72  UI is opened for
+00016540: 2066 696c 6520 7365 6c65 6374 696f 6e2e   file selection.
+00016550: 0a20 2020 2072 6964 203a 2069 6e74 6567  .    rid : integ
+00016560: 6572 0a20 2020 2020 2020 2049 4420 666f  er.        ID fo
+00016570: 7220 3173 7420 5253 504c 494e 453b 2067  r 1st RSPLINE; g
+00016580: 6574 7320 696e 6372 656d 656e 7465 6420  ets incremented 
+00016590: 6279 2031 2066 6f72 2065 6163 6820 5253  by 1 for each RS
+000165a0: 504c 494e 450a 2020 2020 6964 7320 3a20  PLINE.    ids : 
+000165b0: 3264 2061 7272 6179 5f6c 696b 650a 2020  2d array_like.  
+000165c0: 2020 2020 2020 3220 636f 6c75 6d6e 206d        2 column m
+000165d0: 6174 7269 783a 205b 6772 6964 5f69 6473  atrix: [grid_ids
+000165e0: 2c20 696e 6465 7065 6e64 656e 745f 666c  , independent_fl
+000165f0: 6167 5d3b 2068 6173 2067 7269 6473 2066  ag]; has grids f
+00016600: 6f72 0a20 2020 2020 2020 2052 5350 4c49  or.        RSPLI
+00016610: 4e45 2069 6e20 6465 7369 7265 6420 6f72  NE in desired or
+00016620: 6465 7220 616e 6420 6120 3020 6f72 2031  der and a 0 or 1
+00016630: 2066 6c61 6720 666f 7220 6561 6368 2077   flag for each w
+00016640: 6865 7265 2031 0a20 2020 2020 2020 206d  here 1.        m
+00016650: 6561 6e73 2074 6865 2067 7269 6420 6973  eans the grid is
+00016660: 2069 6e64 6570 656e 6465 6e74 2e20 4e6f   independent. No
+00016670: 7465 3a20 7468 6520 3173 7420 616e 6420  te: the 1st and 
+00016680: 6c61 7374 2067 7269 6473 0a20 2020 2020  last grids.     
+00016690: 2020 206d 7573 7420 6265 2069 6e64 6570     must be indep
+000166a0: 656e 6465 6e74 2e0a 2020 2020 446f 4c20  endent..    DoL 
+000166b0: 3a20 7374 7269 6e67 206f 7220 7265 616c  : string or real
+000166c0: 2073 6361 6c61 720a 2020 2020 2020 2020   scalar.        
+000166d0: 5370 6563 6966 6965 7320 7261 7469 6f20  Specifies ratio 
+000166e0: 6f66 2064 6961 6d65 7465 7220 6f66 2065  of diameter of e
+000166f0: 6c61 7374 6963 2074 7562 6520 746f 2074  lastic tube to t
+00016700: 6865 2073 756d 206f 6620 7468 650a 2020  he sum of the.  
+00016710: 2020 2020 2020 6c65 6e67 7468 7320 6f66        lengths of
+00016720: 2061 6c6c 2073 6567 6d65 6e74 732e 2057   all segments. W
+00016730: 7269 7474 656e 2077 6974 683a 2060 6066  ritten with: ``f
+00016740: 277b 446f 4c3a 3c38 7d27 6060 0a0a 2020  '{DoL:<8}'``..  
+00016750: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00016760: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a0a  -----.    None..
+00016770: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
+00016780: 2d2d 2d0a 2020 2020 5468 6520 5253 504c  ---.    The RSPL
+00016790: 494e 4573 2077 696c 6c20 666f 6c6c 6f77  INEs will follow
+000167a0: 2074 6869 7320 7061 7474 6572 6e3a 3a0a   this pattern::.
+000167b0: 0a20 2020 2020 2020 2052 5350 4c49 4e45  .        RSPLINE
+000167c0: 3120 2069 6e64 6570 656e 6465 6e74 3120  1  independent1 
+000167d0: 2d20 6465 7065 6e64 656e 7473 3120 2d20  - dependents1 - 
+000167e0: 696e 6465 7065 6e64 656e 7432 0a20 2020  independent2.   
+000167f0: 2020 2020 2052 5350 4c49 4e45 3220 2069       RSPLINE2  i
+00016800: 6e64 6570 656e 6465 6e74 3220 2d20 6465  ndependent2 - de
+00016810: 7065 6e64 656e 7473 3220 2d20 696e 6465  pendents2 - inde
+00016820: 7065 6e64 656e 7433 0a20 2020 2020 2020  pendent3.       
+00016830: 202e 2e2e 0a0a 2020 2020 4e6f 7465 2074   .....    Note t
+00016840: 6861 7420 7468 6572 6520 6361 6e20 6265  hat there can be
+00016850: 206d 756c 7469 706c 6520 6465 7065 6e64   multiple depend
+00016860: 656e 7473 2073 616e 6477 6963 6865 6420  ents sandwiched 
+00016870: 6265 7477 6565 6e20 7468 650a 2020 2020  between the.    
+00016880: 7477 6f20 6f75 7473 6964 6520 696e 6465  two outside inde
+00016890: 7065 6e64 656e 7420 6e6f 6465 7320 7065  pendent nodes pe
+000168a0: 7220 5253 504c 494e 452e 0a0a 2020 2020  r RSPLINE...    
+000168b0: 5468 6520 7370 6c69 6e65 2065 6c65 6d65  The spline eleme
+000168c0: 6e74 2061 7373 756d 6573 2061 206c 696e  nt assumes a lin
+000168d0: 6561 7220 696e 7465 7270 6f6c 6174 696f  ear interpolatio
+000168e0: 6e20 666f 7220 6469 7370 6c61 6365 6d65  n for displaceme
+000168f0: 6e74 0a20 2020 2061 6e64 2074 6f72 7369  nt.    and torsi
+00016900: 6f6e 2061 6c6f 6e67 2074 6865 2061 7869  on along the axi
+00016910: 7320 6f66 2074 6865 2073 706c 696e 652c  s of the spline,
+00016920: 2061 2071 7561 6472 6174 6963 0a20 2020   a quadratic.   
+00016930: 2069 6e74 6572 706f 6c61 7469 6f6e 2066   interpolation f
+00016940: 6f72 2072 6f74 6174 696f 6e73 206e 6f72  or rotations nor
+00016950: 6d61 6c20 746f 2074 6865 2061 7869 7320  mal to the axis 
+00016960: 6f66 2074 6865 2073 706c 696e 652c 2061  of the spline, a
+00016970: 6e64 0a20 2020 2061 2063 7562 6963 2069  nd.    a cubic i
+00016980: 6e74 6572 706f 6c61 7469 6f6e 2066 6f72  nterpolation for
+00016990: 2064 6973 706c 6163 656d 656e 7473 206e   displacements n
+000169a0: 6f72 6d61 6c20 746f 2074 6865 2061 7869  ormal to the axi
+000169b0: 7320 6f66 2074 6865 0a20 2020 2073 706c  s of the.    spl
+000169c0: 696e 652e 0a0a 2020 2020 5365 6520 616c  ine...    See al
+000169d0: 736f 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  so.    --------.
+000169e0: 2020 2020 3a66 756e 633a 6077 7472 7370      :func:`wtrsp
+000169f0: 6c69 6e65 5f72 696e 6773 600a 0a20 2020  line_rings`..   
+00016a00: 2052 6169 7365 730a 2020 2020 2d2d 2d2d   Raises.    ----
+00016a10: 2d2d 0a20 2020 2056 616c 7565 4572 726f  --.    ValueErro
+00016a20: 720a 0a20 2020 2020 2020 2049 6620 7468  r..        If th
+00016a30: 6572 6520 6172 6520 6c65 7373 2074 6861  ere are less tha
+00016a40: 6e20 3320 6772 6964 7320 666f 7220 5253  n 3 grids for RS
+00016a50: 504c 494e 452e 0a0a 2020 2020 2020 2020  PLINE...        
+00016a60: 4966 2065 6974 6865 7220 7468 6520 6669  If either the fi
+00016a70: 7273 7420 6f72 206c 6173 7420 6772 6964  rst or last grid
+00016a80: 7320 6973 2064 6570 656e 6465 6e74 2e0a  s is dependent..
+00016a90: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
+00016aa0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e    --------.    >
+00016ab0: 3e3e 2069 6d70 6f72 7420 6e75 6d70 7920  >> import numpy 
+00016ac0: 6173 206e 700a 2020 2020 3e3e 3e20 6672  as np.    >>> fr
+00016ad0: 6f6d 2070 7979 6574 6920 696d 706f 7274  om pyyeti import
+00016ae0: 206e 6173 7472 616e 0a20 2020 203e 3e3e   nastran.    >>>
+00016af0: 2069 6473 203d 206e 702e 6172 7261 7928   ids = np.array(
+00016b00: 5b5b 3130 302c 2031 5d2c 0a20 2020 202e  [[100, 1],.    .
+00016b10: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
+00016b20: 2020 205b 3130 312c 2030 5d2c 0a20 2020     [101, 0],.   
+00016b30: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
+00016b40: 2020 2020 205b 3130 322c 2030 5d2c 0a20       [102, 0],. 
+00016b50: 2020 202e 2e2e 2020 2020 2020 2020 2020     ...          
+00016b60: 2020 2020 2020 205b 3130 332c 2031 5d2c         [103, 1],
+00016b70: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+00016b80: 2020 2020 2020 2020 205b 3130 342c 2030           [104, 0
+00016b90: 5d2c 0a20 2020 202e 2e2e 2020 2020 2020  ],.    ...      
+00016ba0: 2020 2020 2020 2020 2020 205b 3130 352c             [105,
+00016bb0: 2031 5d5d 290a 2020 2020 3e3e 3e20 6e61   1]]).    >>> na
+00016bc0: 7374 7261 6e2e 7774 7273 706c 696e 6528  stran.wtrspline(
+00016bd0: 312c 2031 302c 2069 6473 290a 2020 2020  1, 10, ids).    
+00016be0: 5253 504c 494e 4520 2020 2020 2020 3130  RSPLINE       10
+00016bf0: 2020 2020 2030 2e31 2020 2020 2031 3030       0.1     100
+00016c00: 2020 2020 2031 3031 2020 3132 3334 3536       101  123456
+00016c10: 2020 2020 2031 3032 2020 3132 3334 3536       102  123456
+00016c20: 2020 2020 2031 3033 0a20 2020 2052 5350       103.    RSP
+00016c30: 4c49 4e45 2020 2020 2020 2031 3120 2020  LINE       11   
+00016c40: 2020 302e 3120 2020 2020 3130 3320 2020    0.1     103   
+00016c50: 2020 3130 3420 2031 3233 3435 3620 2020    104  123456   
+00016c60: 2020 3130 350a 2020 2020 2222 220a 2020    105.    """.  
+00016c70: 2020 6964 7320 3d20 6e70 2e61 746c 6561    ids = np.atlea
+00016c80: 7374 5f32 6428 6964 7329 2e61 7374 7970  st_2d(ids).astyp
+00016c90: 6528 6e70 2e69 6e74 3634 290a 2020 2020  e(np.int64).    
+00016ca0: 4e20 3d20 6964 732e 7368 6170 655b 305d  N = ids.shape[0]
+00016cb0: 0a20 2020 2069 6620 4e20 3c20 333a 0a20  .    if N < 3:. 
+00016cc0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00016cd0: 7565 4572 726f 7228 226e 6f74 2065 6e6f  ueError("not eno
+00016ce0: 7567 6820 6772 6964 7320 666f 7220 5253  ugh grids for RS
+00016cf0: 504c 494e 4522 290a 0a20 2020 2069 6473  PLINE")..    ids
+00016d00: 2c20 696e 6420 3d20 6964 732e 540a 2020  , ind = ids.T.  
+00016d10: 2020 6966 2069 6e64 2e61 6c6c 2829 3a0a    if ind.all():.
+00016d20: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00016d30: 6c75 6545 7272 6f72 2822 7468 6572 6520  lueError("there 
+00016d40: 6172 6520 6e6f 2064 6570 656e 6465 6e74  are no dependent
+00016d50: 2044 4f46 2066 6f72 2052 5350 4c49 4e45   DOF for RSPLINE
+00016d60: 2229 0a0a 2020 2020 6966 206e 6f74 2069  ")..    if not i
+00016d70: 6e64 5b30 5d20 3d3d 2069 6e64 5b2d 315d  nd[0] == ind[-1]
+00016d80: 203d 3d20 313a 0a20 2020 2020 2020 2072   == 1:.        r
+00016d90: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00016da0: 2274 6865 2066 6972 7374 2061 6e64 206c  "the first and l
+00016db0: 6173 7420 6772 6964 7320 6d75 7374 2062  ast grids must b
+00016dc0: 6520 696e 6465 7065 6e64 656e 7422 290a  e independent").
+00016dd0: 0a20 2020 2023 2066 696e 6420 696e 6469  .    # find indi
+00016de0: 6365 7320 6f66 2061 6c6c 2064 6570 656e  ces of all depen
+00016df0: 6465 6e74 733a 0a20 2020 2064 6570 7320  dents:.    deps 
+00016e00: 3d20 2869 6e64 203d 3d20 3029 2e6e 6f6e  = (ind == 0).non
+00016e10: 7a65 726f 2829 5b30 5d0a 0a20 2020 2023  zero()[0]..    #
+00016e20: 2066 696e 6420 6761 7073 2069 6e20 696e   find gaps in in
+00016e30: 6469 6365 7320 6f66 2064 6570 656e 6465  dices of depende
+00016e40: 6e74 7320 6c69 7374 3a0a 2020 2020 6761  nts list:.    ga
+00016e50: 7073 203d 2028 6e70 2e64 6966 6628 6465  ps = (np.diff(de
+00016e60: 7073 2920 213d 2031 292e 6e6f 6e7a 6572  ps) != 1).nonzer
+00016e70: 6f28 295b 305d 0a0a 2020 2020 2320 7374  o()[0]..    # st
+00016e80: 6172 7469 6e67 2069 6e64 6963 6573 206f  arting indices o
+00016e90: 6620 6465 7065 6e64 656e 7473 3a0a 2020  f dependents:.  
+00016ea0: 2020 6669 7273 7473 203d 2064 6570 735b    firsts = deps[
+00016eb0: 6e70 2e68 7374 6163 6b28 2830 2c20 6761  np.hstack((0, ga
+00016ec0: 7073 202b 2031 2929 5d0a 0a20 2020 2023  ps + 1))]..    #
+00016ed0: 2065 6e64 696e 6720 696e 6469 6365 7320   ending indices 
+00016ee0: 6f66 2064 6570 656e 6465 6e74 733a 0a20  of dependents:. 
+00016ef0: 2020 206c 6173 7473 203d 2064 6570 735b     lasts = deps[
+00016f00: 6e70 2e68 7374 6163 6b28 2867 6170 732c  np.hstack((gaps,
+00016f10: 206c 656e 2864 6570 7329 202d 2031 2929   len(deps) - 1))
+00016f20: 5d0a 0a20 2020 2023 2077 7269 7465 206f  ]..    # write o
+00016f30: 6e65 2052 5350 4c49 4e45 2070 6572 2073  ne RSPLINE per s
+00016f40: 6572 6965 7320 6f66 2064 6570 656e 6465  eries of depende
+00016f50: 6e74 733a 0a20 2020 2066 6f72 2064 302c  nts:.    for d0,
+00016f60: 2064 3120 696e 207a 6970 2866 6972 7374   d1 in zip(first
+00016f70: 732c 206c 6173 7473 293a 0a20 2020 2020  s, lasts):.     
+00016f80: 2020 2066 2e77 7269 7465 2866 2252 5350     f.write(f"RSP
+00016f90: 4c49 4e45 207b 7269 643a 387d 7b44 6f4c  LINE {rid:8}{DoL
+00016fa0: 3a3e 387d 7b69 6473 5b64 3020 2d20 315d  :>8}{ids[d0 - 1]
+00016fb0: 3a38 7d22 290a 2020 2020 2020 2020 7269  :8}").        ri
+00016fc0: 6420 2b3d 2031 0a20 2020 2020 2020 2066  d += 1.        f
+00016fd0: 6965 6c64 203d 2035 2020 2320 6e65 7874  ield = 5  # next
+00016fe0: 206e 6173 7472 616e 2066 6965 6c64 2028   nastran field (
+00016ff0: 3120 746f 2031 3029 0a0a 2020 2020 2020  1 to 10)..      
+00017000: 2020 2320 7772 6974 6520 616c 6c20 6275    # write all bu
+00017010: 7420 6c61 7374 2067 7269 6420 6f66 2063  t last grid of c
+00017020: 7572 7265 6e74 2073 6567 6d65 6e74 3a0a  urrent segment:.
+00017030: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+00017040: 2072 616e 6765 2864 302c 2064 3120 2b20   range(d0, d1 + 
+00017050: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+00017060: 662e 7772 6974 6528 6622 7b69 6473 5b6a  f.write(f"{ids[j
+00017070: 5d3a 387d 2229 0a20 2020 2020 2020 2020  ]:8}").         
+00017080: 2020 2066 6965 6c64 202b 3d20 310a 2020     field += 1.  
+00017090: 2020 2020 2020 2020 2020 6966 2066 6965            if fie
+000170a0: 6c64 203d 3d20 3130 3a0a 2020 2020 2020  ld == 10:.      
+000170b0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+000170c0: 6528 225c 6e20 2020 2020 2020 2022 290a  e("\n        ").
+000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170e0: 6669 656c 6420 3d20 320a 2020 2020 2020  field = 2.      
+000170f0: 2020 2020 2020 662e 7772 6974 6528 2220        f.write(" 
+00017100: 2031 3233 3435 3622 290a 2020 2020 2020   123456").      
+00017110: 2020 2020 2020 6669 656c 6420 2b3d 2031        field += 1
+00017120: 0a0a 2020 2020 2020 2020 2320 7772 6974  ..        # writ
+00017130: 6520 636c 6f73 696e 6720 696e 6465 7065  e closing indepe
+00017140: 6e64 656e 743a 0a20 2020 2020 2020 2066  ndent:.        f
+00017150: 2e77 7269 7465 2866 227b 6964 735b 6431  .write(f"{ids[d1
+00017160: 202b 2031 5d3a 387d 5c6e 2229 0a0a 0a64   + 1]:8}\n")...d
+00017170: 6566 205f 696e 7465 7273 6563 7428 6369  ef _intersect(ci
+00017180: 7263 412c 2063 6972 6342 2c20 7879 412c  rcA, circB, xyA,
+00017190: 2064 7261 773d 4661 6c73 6529 3a0a 2020   draw=False):.  
+000171a0: 2020 2222 220a 2020 2020 4669 6e64 2077    """.    Find w
+000171b0: 6865 7265 2061 206c 696e 6520 7468 6174  here a line that
+000171c0: 2070 6173 7365 7320 7468 726f 7567 6820   passes through 
+000171d0: 7468 6520 6365 6e74 6572 206f 6620 6369  the center of ci
+000171e0: 7263 4120 616e 640a 2020 2020 706f 696e  rcA and.    poin
+000171f0: 7420 7879 4120 696e 7465 7273 6563 7473  t xyA intersects
+00017200: 2063 6972 6342 2e0a 0a20 2020 2050 6172   circB...    Par
+00017210: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00017220: 2d2d 2d2d 2d2d 0a20 2020 2063 6972 6341  ------.    circA
+00017230: 203a 2033 2d65 6c65 6d65 6e74 2061 7272   : 3-element arr
+00017240: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
+00017250: 5b78 632c 2079 632c 2052 5d20 666f 7220  [xc, yc, R] for 
+00017260: 6369 7263 6c65 2041 0a20 2020 2063 6972  circle A.    cir
+00017270: 6342 203a 2033 2d65 6c65 6d65 6e74 2061  cB : 3-element a
+00017280: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
+00017290: 2020 5b78 632c 2079 632c 2052 5d20 666f    [xc, yc, R] fo
+000172a0: 7220 6369 7263 6c65 2042 0a20 2020 2078  r circle B.    x
+000172b0: 7941 203a 2032 2d65 6c65 6d65 6e74 2061  yA : 2-element a
+000172c0: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
+000172d0: 2020 5b78 2c20 795d 2070 6f69 6e74 2028    [x, y] point (
+000172e0: 7072 6f62 6162 6c79 206f 6e20 6369 7263  probably on circ
+000172f0: 6c65 2041 290a 2020 2020 6472 6177 203a  le A).    draw :
+00017300: 2062 6f6f 6c3b 206f 7074 696f 6e61 6c0a   bool; optional.
+00017310: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+00017320: 2070 6c6f 7420 6369 7263 6c65 7320 616e   plot circles an
+00017330: 6420 706f 696e 7473 2066 6f72 2076 6973  d points for vis
+00017340: 7561 6c20 696e 7370 6563 7469 6f6e 2069  ual inspection i
+00017350: 6e0a 2020 2020 2020 2020 6669 6775 7265  n.        figure
+00017360: 2027 696e 7465 7273 6563 7427 0a0a 2020   'intersect'..  
+00017370: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00017380: 2d2d 2d2d 2d0a 2020 2020 7074 203a 2031  -----.    pt : 1
+00017390: 6420 6e64 6172 7261 790a 2020 2020 2020  d ndarray.      
+000173a0: 2020 5b78 2c20 795d 206c 6f63 6174 696f    [x, y] locatio
+000173b0: 6e20 6f66 2069 6e74 6572 7365 6374 696f  n of intersectio
+000173c0: 6e20 706f 696e 7420 636c 6f73 6573 7420  n point closest 
+000173d0: 746f 2078 7941 0a0a 2020 2020 4578 616d  to xyA..    Exam
+000173e0: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+000173f0: 2d0a 2020 2020 2e2e 2070 6c6f 743a 3a0a  -.    .. plot::.
+00017400: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
+00017410: 3a20 636c 6f73 652d 6669 6773 0a0a 2020  : close-figs..  
+00017420: 2020 2020 2020 3e3e 3e20 6672 6f6d 2070        >>> from p
+00017430: 7979 6574 692e 6e61 7374 7261 6e2e 6275  yyeti.nastran.bu
+00017440: 6c6b 2069 6d70 6f72 7420 5f69 6e74 6572  lk import _inter
+00017450: 7365 6374 0a20 2020 2020 2020 203e 3e3e  sect.        >>>
+00017460: 2063 6972 6341 203d 2028 302e 2c20 302e   circA = (0., 0.
+00017470: 2c20 3130 2e29 0a20 2020 2020 2020 203e  , 10.).        >
+00017480: 3e3e 2063 6972 6342 203d 2028 302e 2c20  >> circB = (0., 
+00017490: 302e 2c20 3135 2e29 0a20 2020 2020 2020  0., 15.).       
+000174a0: 203e 3e3e 2078 7941 203d 2028 302e 2c20   >>> xyA = (0., 
+000174b0: 352e 290a 2020 2020 2020 2020 3e3e 3e20  5.).        >>> 
+000174c0: 5f69 6e74 6572 7365 6374 2863 6972 6341  _intersect(circA
+000174d0: 2c20 6369 7263 422c 205b 302e 2c20 312e  , circB, [0., 1.
+000174e0: 5d2c 2064 7261 773d 3129 0a20 2020 2020  ], draw=1).     
+000174f0: 2020 2061 7272 6179 285b 2020 302e 2c20     array([  0., 
+00017500: 2031 352e 5d29 0a20 2020 2020 2020 203e   15.]).        >
+00017510: 3e3e 205f 696e 7465 7273 6563 7428 6369  >> _intersect(ci
+00017520: 7263 412c 2063 6972 6342 2c20 5b30 2e2c  rcA, circB, [0.,
+00017530: 202d 312e 5d29 0a20 2020 2020 2020 2061   -1.]).        a
+00017540: 7272 6179 285b 2020 302e 2c20 2d31 352e  rray([  0., -15.
+00017550: 5d29 0a20 2020 2020 2020 203e 3e3e 205f  ]).        >>> _
+00017560: 696e 7465 7273 6563 7428 6369 7263 412c  intersect(circA,
+00017570: 2063 6972 6342 2c20 5b31 2e2c 2030 2e5d   circB, [1., 0.]
+00017580: 290a 2020 2020 2020 2020 6172 7261 7928  ).        array(
+00017590: 5b20 3135 2e2c 2020 2030 2e5d 290a 2020  [ 15.,   0.]).  
+000175a0: 2020 2020 2020 3e3e 3e20 5f69 6e74 6572        >>> _inter
+000175b0: 7365 6374 2863 6972 6341 2c20 6369 7263  sect(circA, circ
+000175c0: 422c 205b 2d31 2e2c 2030 2e5d 290a 2020  B, [-1., 0.]).  
+000175d0: 2020 2020 2020 6172 7261 7928 5b2d 3135        array([-15
+000175e0: 2e2c 2020 2030 2e5d 290a 2020 2020 2222  .,   0.]).    ""
+000175f0: 220a 2020 2020 2878 312c 2079 312c 2052  ".    (x1, y1, R
+00017600: 3129 203d 2063 6972 6341 0a20 2020 2028  1) = circA.    (
+00017610: 7832 2c20 7932 2920 3d20 7879 410a 2020  x2, y2) = xyA.  
+00017620: 2020 2878 332c 2079 332c 2052 3329 203d    (x3, y3, R3) =
+00017630: 2063 6972 6342 0a20 2020 2069 6620 6162   circB.    if ab
+00017640: 7328 7832 202d 2078 3129 203e 2031 3030  s(x2 - x1) > 100
+00017650: 202a 206e 702e 6669 6e66 6f28 666c 6f61   * np.finfo(floa
+00017660: 7429 2e65 7073 3a0a 2020 2020 2020 2020  t).eps:.        
+00017670: 6d20 3d20 2879 3220 2d20 7931 2920 2f20  m = (y2 - y1) / 
+00017680: 2878 3220 2d20 7831 290a 2020 2020 2020  (x2 - x1).      
+00017690: 2020 6220 3d20 2878 3220 2a20 7931 202d    b = (x2 * y1 -
+000176a0: 2078 3120 2a20 7932 2920 2f20 2878 3220   x1 * y2) / (x2 
+000176b0: 2d20 7831 290a 2020 2020 2020 2020 2320  - x1).        # 
+000176c0: 286d 782b 622d 7933 292a 2a32 202b 2028  (mx+b-y3)**2 + (
+000176d0: 782d 7833 292a 2a32 203d 2052 332a 2a32  x-x3)**2 = R3**2
+000176e0: 0a20 2020 2020 2020 2061 3220 3d20 6d20  .        a2 = m 
+000176f0: 2a20 6d20 2b20 310a 2020 2020 2020 2020  * m + 1.        
+00017700: 6131 203d 2032 202a 2028 6d20 2a20 2862  a1 = 2 * (m * (b
+00017710: 202d 2079 3329 202d 2078 3329 202f 2061   - y3) - x3) / a
+00017720: 320a 2020 2020 2020 2020 6130 203d 2028  2.        a0 = (
+00017730: 2862 202d 2079 3329 202a 2a20 3220 2b20  (b - y3) ** 2 + 
+00017740: 7833 2a2a 3220 2d20 5233 2a2a 3229 202f  x3**2 - R3**2) /
+00017750: 2061 320a 2020 2020 2020 2020 7831 203d   a2.        x1 =
+00017760: 202d 6131 202f 2032 202b 206e 702e 7371   -a1 / 2 + np.sq
+00017770: 7274 2828 6131 202f 2032 2920 2a2a 2032  rt((a1 / 2) ** 2
+00017780: 202d 2061 3029 0a20 2020 2020 2020 2078   - a0).        x
+00017790: 3220 3d20 2d61 3120 2f20 3220 2d20 6e70  2 = -a1 / 2 - np
+000177a0: 2e73 7172 7428 2861 3120 2f20 3229 202a  .sqrt((a1 / 2) *
+000177b0: 2a20 3220 2d20 6130 290a 2020 2020 2020  * 2 - a0).      
+000177c0: 2020 7931 203d 206d 202a 2078 3120 2b20    y1 = m * x1 + 
+000177d0: 620a 2020 2020 2020 2020 7932 203d 206d  b.        y2 = m
+000177e0: 202a 2078 3220 2b20 620a 2020 2020 656c   * x2 + b.    el
+000177f0: 7365 3a0a 2020 2020 2020 2020 2320 6c69  se:.        # li
+00017800: 6e65 2069 7320 7665 7274 6963 616c 2028  ne is vertical (
+00017810: 7831 2026 2078 3220 6172 6520 756e 6368  x1 & x2 are unch
+00017820: 616e 6765 6429 0a20 2020 2020 2020 2023  anged).        #
+00017830: 2020 2020 2879 2d79 3329 2a2a 3220 2b20      (y-y3)**2 + 
+00017840: 2878 312d 7833 292a 2a32 203d 2052 332a  (x1-x3)**2 = R3*
+00017850: 2a32 0a20 2020 2020 2020 2023 2020 2020  *2.        #    
+00017860: 792d 7933 203d 202b 2d20 6e70 2e73 7172  y-y3 = +- np.sqr
+00017870: 7428 5233 2a2a 3220 2d20 2878 312d 7833  t(R3**2 - (x1-x3
+00017880: 292a 2a32 290a 2020 2020 2020 2020 7931  )**2).        y1
+00017890: 203d 2079 3320 2b20 6e70 2e73 7172 7428   = y3 + np.sqrt(
+000178a0: 5233 2a2a 3220 2d20 2878 3120 2d20 7833  R3**2 - (x1 - x3
+000178b0: 2920 2a2a 2032 290a 2020 2020 2020 2020  ) ** 2).        
+000178c0: 7932 203d 2079 3320 2d20 6e70 2e73 7172  y2 = y3 - np.sqr
+000178d0: 7428 5233 2a2a 3220 2d20 2878 3120 2d20  t(R3**2 - (x1 - 
+000178e0: 7833 2920 2a2a 2032 290a 2020 2020 6572  x3) ** 2).    er
+000178f0: 7231 203d 2061 6273 2878 7941 5b30 5d20  r1 = abs(xyA[0] 
+00017900: 2d20 7831 2920 2b20 6162 7328 7879 415b  - x1) + abs(xyA[
+00017910: 315d 202d 2079 3129 0a20 2020 2065 7272  1] - y1).    err
+00017920: 3220 3d20 6162 7328 7879 415b 305d 202d  2 = abs(xyA[0] -
+00017930: 2078 3229 202b 2061 6273 2878 7941 5b31   x2) + abs(xyA[1
+00017940: 5d20 2d20 7932 290a 2020 2020 6966 2065  ] - y2).    if e
+00017950: 7272 3120 3c20 6572 7232 3a0a 2020 2020  rr1 < err2:.    
+00017960: 2020 2020 7074 203d 206e 702e 6172 7261      pt = np.arra
+00017970: 7928 5b78 312c 2079 315d 290a 2020 2020  y([x1, y1]).    
+00017980: 656c 7365 3a0a 2020 2020 2020 2020 7074  else:.        pt
+00017990: 203d 206e 702e 6172 7261 7928 5b78 322c   = np.array([x2,
+000179a0: 2079 325d 290a 2020 2020 6966 2064 7261   y2]).    if dra
+000179b0: 773a 0a20 2020 2020 2020 2070 6c74 2e66  w:.        plt.f
+000179c0: 6967 7572 6528 2269 6e74 6572 7365 6374  igure("intersect
+000179d0: 2229 0a20 2020 2020 2020 2070 6c74 2e63  ").        plt.c
+000179e0: 6c66 2829 0a20 2020 2020 2020 2074 6820  lf().        th 
+000179f0: 3d20 6e70 2e61 7261 6e67 6528 302c 2033  = np.arange(0, 3
+00017a00: 3631 2920 2a20 6e70 2e70 6920 2f20 3138  61) * np.pi / 18
+00017a10: 302e 300a 2020 2020 2020 2020 2878 312c  0.0.        (x1,
+00017a20: 2079 312c 2052 3129 203d 2063 6972 6341   y1, R1) = circA
+00017a30: 0a20 2020 2020 2020 2070 6c74 2e70 6c6f  .        plt.plo
+00017a40: 7428 7831 202b 2052 3120 2a20 6e70 2e63  t(x1 + R1 * np.c
+00017a50: 6f73 2874 6829 2c20 7931 202b 2052 3120  os(th), y1 + R1 
+00017a60: 2a20 6e70 2e73 696e 2874 6829 2c20 6c61  * np.sin(th), la
+00017a70: 6265 6c3d 2243 6972 6341 2229 0a20 2020  bel="CircA").   
+00017a80: 2020 2020 2070 6c74 2e70 6c6f 7428 7833       plt.plot(x3
+00017a90: 202b 2052 3320 2a20 6e70 2e63 6f73 2874   + R3 * np.cos(t
+00017aa0: 6829 2c20 7933 202b 2052 3320 2a20 6e70  h), y3 + R3 * np
+00017ab0: 2e73 696e 2874 6829 2c20 6c61 6265 6c3d  .sin(th), label=
+00017ac0: 2243 6972 6342 2229 0a20 2020 2020 2020  "CircB").       
+00017ad0: 2070 6c74 2e73 6361 7474 6572 282a 7879   plt.scatter(*xy
+00017ae0: 412c 2063 3d22 6722 2c20 6d61 726b 6572  A, c="g", marker
+00017af0: 3d22 6f22 2c20 733d 3630 2c20 6c61 6265  ="o", s=60, labe
+00017b00: 6c3d 2278 7941 2229 0a20 2020 2020 2020  l="xyA").       
+00017b10: 2070 6c74 2e73 6361 7474 6572 282a 7074   plt.scatter(*pt
+00017b20: 2c20 633d 2262 222c 206d 6172 6b65 723d  , c="b", marker=
+00017b30: 2276 222c 2073 3d36 302c 206c 6162 656c  "v", s=60, label
+00017b40: 3d22 696e 7465 7273 6563 7469 6f6e 206f  ="intersection o
+00017b50: 6e20 4369 7263 4222 290a 2020 2020 2020  n CircB").      
+00017b60: 2020 706c 742e 6178 6973 2822 6571 7561    plt.axis("equa
+00017b70: 6c22 290a 2020 2020 2020 2020 706c 742e  l").        plt.
+00017b80: 6c65 6765 6e64 286c 6f63 3d22 6265 7374  legend(loc="best
+00017b90: 222c 2073 6361 7474 6572 706f 696e 7473  ", scatterpoints
+00017ba0: 3d31 290a 2020 2020 7265 7475 726e 2070  =1).    return p
+00017bb0: 740a 0a0a 6465 6620 5f63 6865 636b 5f7a  t...def _check_z
+00017bc0: 5f61 6c69 676e 6d65 6e74 2863 6972 635f  _alignment(circ_
+00017bd0: 7061 726d 732c 2074 6f6c 293a 0a20 2020  parms, tol):.   
+00017be0: 2023 2048 6176 6520 7477 6f20 6469 6666   # Have two diff
+00017bf0: 6572 656e 7420 7472 616e 7366 6f72 6d73  erent transforms
+00017c00: 2074 6f20 6120 6c6f 6361 6c20 7379 7374   to a local syst
+00017c10: 656d 202e 2e2e 2068 6176 6520 746f 2075  em ... have to u
+00017c20: 7365 0a20 2020 2023 2073 616d 6520 6f6e  se.    # same on
+00017c30: 6520 746f 2067 6574 2070 726f 7065 7220  e to get proper 
+00017c40: 6e6f 6465 2061 6c69 676e 696e 6720 746f  node aligning to
+00017c50: 206f 6363 7572 2066 6f72 2052 5350 4c49   occur for RSPLI
+00017c60: 4e45 2e20 4275 742c 0a20 2020 2023 2074  NE. But,.    # t
+00017c70: 6865 207a 2d61 7869 7320 666f 7220 626f  he z-axis for bo
+00017c80: 7468 2062 6574 7465 7220 6d61 7463 6820  th better match 
+00017c90: 7570 202e 2e2e 2063 6f6d 7075 7465 2063  up ... compute c
+00017ca0: 6f73 696e 6520 6f66 2061 6e67 6c65 0a20  osine of angle. 
+00017cb0: 2020 2023 2062 6574 7765 656e 2074 6865     # between the
+00017cc0: 2074 776f 207a 2d61 7865 7320 2e2e 2e20   two z-axes ... 
+00017cd0: 7368 6f75 6c64 2062 6520 7665 7279 2063  should be very c
+00017ce0: 6c6f 7365 2074 6f20 312e 303a 0a20 2020  lose to 1.0:.   
+00017cf0: 207a 3120 3d20 6369 7263 5f70 6172 6d73   z1 = circ_parms
+00017d00: 5b30 5d2e 6261 7369 6332 6c6f 6361 6c5b  [0].basic2local[
+00017d10: 325d 0a20 2020 207a 3220 3d20 6369 7263  2].    z2 = circ
+00017d20: 5f70 6172 6d73 5b31 5d2e 6261 7369 6332  _parms[1].basic2
+00017d30: 6c6f 6361 6c5b 325d 0a20 2020 2023 2074  local[2].    # t
+00017d40: 6865 7365 2061 7265 2075 6e69 7420 7665  hese are unit ve
+00017d50: 6374 6f72 733b 206e 6f20 6e65 6564 2074  ctors; no need t
+00017d60: 6f20 6469 7669 6465 2062 7920 6d61 676e  o divide by magn
+00017d70: 6974 7564 6573 3a0a 2020 2020 636f 7369  itudes:.    cosi
+00017d80: 6e65 203d 207a 312e 646f 7428 7a32 290a  ne = z1.dot(z2).
+00017d90: 2020 2020 6966 2061 6273 2863 6f73 696e      if abs(cosin
+00017da0: 6529 203c 2074 6f6c 3a0a 2020 2020 2020  e) < tol:.      
+00017db0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00017dc0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00017dd0: 2270 6572 7065 6e64 6963 756c 6172 2064  "perpendicular d
+00017de0: 6972 6563 7469 6f6e 7320 6f66 2060 7231  irections of `r1
+00017df0: 6772 6964 7360 2061 6e64 2022 0a20 2020  grids` and ".   
+00017e00: 2020 2020 2020 2020 2066 2260 7232 6772           f"`r2gr
+00017e10: 6964 7360 2064 6f20 6e6f 7420 6d61 7463  ids` do not matc
+00017e20: 683a 207b 7a31 7d20 7673 2e20 7b7a 327d  h: {z1} vs. {z2}
+00017e30: 3b20 7468 6520 220a 2020 2020 2020 2020  ; the ".        
+00017e40: 2020 2020 6622 636f 7369 6e65 206f 6620      f"cosine of 
+00017e50: 7468 6520 616e 676c 6520 6265 7477 6565  the angle betwee
+00017e60: 6e20 7468 656d 2069 7320 7b63 6f73 696e  n them is {cosin
+00017e70: 657d 220a 2020 2020 2020 2020 290a 0a0a  e}".        )...
+00017e80: 6465 6620 5f77 745f 6369 7263 6c65 315f  def _wt_circle1_
+00017e90: 636f 6f72 6428 662c 2063 6f72 645f 6964  coord(f, cord_id
+00017ea0: 2c20 6365 6e74 6572 2c20 6261 7369 6332  , center, basic2
+00017eb0: 6c6f 6361 6c2c 206e 6f64 6530 2c20 6e6f  local, node0, no
+00017ec0: 6465 5f69 6430 2c20 6e61 6d65 7329 3a0a  de_id0, names):.
+00017ed0: 2020 2020 7265 665f 636f 7264 5f69 6420      ref_cord_id 
+00017ee0: 3d20 300a 2020 2020 6469 7374 203d 206d  = 0.    dist = m
+00017ef0: 6178 2831 2e30 2c20 6e70 2e6c 696e 616c  ax(1.0, np.linal
+00017f00: 672e 6e6f 726d 2863 656e 7465 7229 290a  g.norm(center)).
+00017f10: 2020 2020 7020 3d20 3130 202a 2a20 6e70      p = 10 ** np
+00017f20: 2e66 6c6f 6f72 286e 702e 6c6f 6731 3028  .floor(np.log10(
+00017f30: 6469 7374 2929 0a20 2020 2064 6973 7420  dist)).    dist 
+00017f40: 3d20 726f 756e 6428 6469 7374 202f 2070  = round(dist / p
+00017f50: 2920 2a20 700a 2020 2020 6c6f 6361 6c5f  ) * p.    local_
+00017f60: 636f 7264 203d 207b 0a20 2020 2020 2020  cord = {.       
+00017f70: 2063 6f72 645f 6964 3a20 5b0a 2020 2020   cord_id: [.    
+00017f80: 2020 2020 2020 2020 2243 4f52 4432 5222          "CORD2R"
+00017f90: 2c0a 2020 2020 2020 2020 2020 2020 6e70  ,.            np
+00017fa0: 2e76 7374 6163 6b28 0a20 2020 2020 2020  .vstack(.       
+00017fb0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+00017fc0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00017fd0: 636f 7264 5f69 642c 2031 2c20 7265 665f  cord_id, 1, ref_
+00017fe0: 636f 7264 5f69 645d 2c0a 2020 2020 2020  cord_id],.      
+00017ff0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00018000: 6e74 6572 2c0a 2020 2020 2020 2020 2020  nter,.          
+00018010: 2020 2020 2020 2020 2020 6365 6e74 6572            center
+00018020: 202b 2064 6973 7420 2a20 6261 7369 6332   + dist * basic2
+00018030: 6c6f 6361 6c5b 325d 2c0a 2020 2020 2020  local[2],.      
+00018040: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00018050: 6e74 6572 202b 2064 6973 7420 2a20 6261  nter + dist * ba
+00018060: 7369 6332 6c6f 6361 6c5b 305d 2c0a 2020  sic2local[0],.  
+00018070: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00018080: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00018090: 2020 2020 2020 205d 0a20 2020 207d 0a20         ].    }. 
+000180a0: 2020 2063 6f6d 6d65 6e74 203d 2028 0a20     comment = (. 
+000180b0: 2020 2020 2020 2066 224f 7269 6769 6e20         f"Origin 
+000180c0: 6f66 206c 6f63 616c 2043 4f52 4432 5220  of local CORD2R 
+000180d0: 7b63 6f72 645f 6964 7d20 6973 2061 7420  {cord_id} is at 
+000180e0: 6365 6e74 6572 206f 6620 7b6e 616d 6573  center of {names
+000180f0: 5b30 5d7d 2072 696e 673b 220a 2020 2020  [0]} ring;".    
+00018100: 2020 2020 2220 7a20 6973 2070 6572 7065      " z is perpe
+00018110: 6e64 6963 756c 6172 2074 6f20 706c 616e  ndicular to plan
+00018120: 6520 6f66 2063 6972 636c 652c 2061 6e64  e of circle, and
+00018130: 2078 2069 7320 616c 6967 6e65 6420 7769   x is aligned wi
+00018140: 7468 2022 0a20 2020 2020 2020 2066 226e  th ".        f"n
+00018150: 6f64 6520 7b6e 6f64 6530 7d20 2861 6e64  ode {node0} (and
+00018160: 206e 6577 206e 6f64 6520 7b6e 6f64 655f   new node {node_
+00018170: 6964 307d 292e 220a 2020 2020 290a 2020  id0}).".    ).  
+00018180: 2020 662e 7772 6974 6528 6d6b 636f 6d6d    f.write(mkcomm
+00018190: 656e 7428 636f 6d6d 656e 7429 290a 2020  ent(comment)).  
+000181a0: 2020 7774 636f 6f72 6463 6172 6473 2866    wtcoordcards(f
+000181b0: 2c20 6c6f 6361 6c5f 636f 7264 290a 0a0a  , local_cord)...
+000181c0: 6465 6620 5f77 7467 7269 6473 5f72 6265  def _wtgrids_rbe
+000181d0: 3273 280a 2020 2020 662c 2063 6972 635f  2s(.    f, circ_
+000181e0: 7061 726d 732c 2063 656e 7465 722c 2062  parms, center, b
+000181f0: 6173 6963 326c 6f63 616c 2c20 636f 7264  asic2local, cord
+00018200: 5f69 642c 206e 6f64 655f 6964 302c 2072  _id, node_id0, r
+00018210: 6265 325f 6964 302c 2072 696e 6731 5f69  be2_id0, ring1_i
+00018220: 6473 2c20 6e61 6d65 730a 293a 0a20 2020  ds, names.):.   
+00018230: 206e 3120 3d20 6369 7263 5f70 6172 6d73   n1 = circ_parms
+00018240: 5b30 5d2e 6c6f 6361 6c2e 7368 6170 655b  [0].local.shape[
+00018250: 315d 0a20 2020 206e 6577 7074 7320 3d20  1].    newpts = 
+00018260: 6e70 2e7a 6572 6f73 2828 6e31 2c20 3329  np.zeros((n1, 3)
+00018270: 290a 0a20 2020 2023 2064 6566 696e 6520  )..    # define 
+00018280: 7a20 6c6f 6361 7469 6f6e 206f 6620 6e65  z location of ne
+00018290: 7770 7473 3a0a 2020 2020 6e65 7770 7473  wpts:.    newpts
+000182a0: 5b3a 2c20 325d 203d 2063 6972 635f 7061  [:, 2] = circ_pa
+000182b0: 726d 735b 315d 2e6c 6f63 616c 5b32 5d2e  rms[1].local[2].
+000182c0: 6d65 616e 2829 0a0a 2020 2020 2320 636f  mean()..    # co
+000182d0: 6d70 7574 6520 6365 6e74 6572 206f 6620  mpute center of 
+000182e0: 6369 7263 6c65 2032 2069 6e20 6c6f 6361  circle 2 in loca
+000182f0: 6c20 3120 636f 6f72 6469 6e61 7465 733a  l 1 coordinates:
+00018300: 0a20 2020 2063 656e 7465 7232 203d 2062  .    center2 = b
+00018310: 6173 6963 326c 6f63 616c 2040 2028 6369  asic2local @ (ci
+00018320: 7263 5f70 6172 6d73 5b31 5d2e 6365 6e74  rc_parms[1].cent
+00018330: 6572 202d 2063 656e 7465 7229 0a20 2020  er - center).   
+00018340: 2072 6164 6975 7320 3d20 6369 7263 5f70   radius = circ_p
+00018350: 6172 6d73 5b30 5d2e 7261 6469 7573 0a20  arms[0].radius. 
+00018360: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+00018370: 6528 6e31 293a 0a20 2020 2020 2020 206e  e(n1):.        n
+00018380: 6577 7074 735b 6a2c 203a 325d 203d 205f  ewpts[j, :2] = _
+00018390: 696e 7465 7273 6563 7428 0a20 2020 2020  intersect(.     
+000183a0: 2020 2020 2020 205b 302e 302c 2030 2e30         [0.0, 0.0
+000183b0: 2c20 7261 6469 7573 5d2c 0a20 2020 2020  , radius],.     
+000183c0: 2020 2020 2020 205b 6365 6e74 6572 325b         [center2[
+000183d0: 305d 2c20 6365 6e74 6572 325b 315d 2c20  0], center2[1], 
+000183e0: 6369 7263 5f70 6172 6d73 5b31 5d2e 7261  circ_parms[1].ra
+000183f0: 6469 7573 5d2c 0a20 2020 2020 2020 2020  dius],.         
+00018400: 2020 2063 6972 635f 7061 726d 735b 305d     circ_parms[0]
+00018410: 2e6c 6f63 616c 5b3a 322c 206a 5d2c 0a20  .local[:2, j],. 
+00018420: 2020 2020 2020 2029 0a0a 2020 2020 2320         )..    # 
+00018430: 7772 6974 6520 6e65 7720 6772 6964 730a  write new grids.
+00018440: 2020 2020 636f 6d6d 656e 7420 3d20 280a      comment = (.
+00018450: 2020 2020 2020 2020 6622 4772 6964 7320          f"Grids 
+00018460: 746f 2052 4245 3220 746f 2074 6865 207b  to RBE2 to the {
+00018470: 6e61 6d65 735b 305d 7d20 6772 6964 732e  names[0]} grids.
+00018480: 2054 6865 7365 2067 7269 6473 206c 696e   These grids lin
+00018490: 6520 220a 2020 2020 2020 2020 6622 7570  e ".        f"up
+000184a0: 2077 6974 6820 7468 6520 7b6e 616d 6573   with the {names
+000184b0: 5b31 5d7d 2063 6972 636c 6520 736f 2074  [1]} circle so t
+000184c0: 6861 7420 7468 6520 5253 504c 494e 4520  hat the RSPLINE 
+000184d0: 2877 6869 6368 2022 0a20 2020 2020 2020  (which ".       
+000184e0: 2066 2274 6965 7320 746f 6765 7468 6572   f"ties together
+000184f0: 2074 6865 7365 206e 6577 2067 7269 6473   these new grids
+00018500: 2061 6e64 2074 6865 207b 6e61 6d65 735b   and the {names[
+00018510: 315d 7d20 6772 6964 7329 2077 696c 6c20  1]} grids) will 
+00018520: 220a 2020 2020 2020 2020 2262 6520 736d  ".        "be sm
+00018530: 6f6f 7468 2e22 0a20 2020 2029 0a20 2020  ooth.".    ).   
+00018540: 2066 2e77 7269 7465 286d 6b63 6f6d 6d65   f.write(mkcomme
+00018550: 6e74 2863 6f6d 6d65 6e74 2929 0a20 2020  nt(comment)).   
+00018560: 2076 6563 203d 206e 702e 6172 616e 6765   vec = np.arange
+00018570: 286e 3129 0a20 2020 206e 6577 6964 7320  (n1).    newids 
+00018580: 3d20 6e6f 6465 5f69 6430 202b 2076 6563  = node_id0 + vec
+00018590: 0a20 2020 2072 6265 3269 6473 203d 2072  .    rbe2ids = r
+000185a0: 6265 325f 6964 3020 2b20 7665 630a 2020  be2_id0 + vec.  
+000185b0: 2020 7774 6772 6964 7328 662c 206e 6577    wtgrids(f, new
+000185c0: 6964 732c 2078 797a 3d6e 6577 7074 732c  ids, xyz=newpts,
+000185d0: 2063 703d 636f 7264 5f69 6429 0a0a 2020   cp=cord_id)..  
+000185e0: 2020 636f 6d6d 656e 7420 3d20 280a 2020    comment = (.  
+000185f0: 2020 2020 2020 6622 5242 4532 2074 6865        f"RBE2 the
+00018600: 207b 6e61 6d65 735b 305d 7d20 6e6f 6465   {names[0]} node
+00018610: 7320 746f 206e 6577 206e 6f64 6573 2063  s to new nodes c
+00018620: 7265 6174 6564 2061 626f 7665 2022 0a20  reated above ". 
+00018630: 2020 2020 2020 2022 2874 6865 206e 6577         "(the new
+00018640: 206e 6f64 6573 2061 7265 2069 6e64 6570   nodes are indep
+00018650: 656e 6465 6e74 293a 220a 2020 2020 290a  endent):".    ).
+00018660: 2020 2020 662e 7772 6974 6528 6d6b 636f      f.write(mkco
+00018670: 6d6d 656e 7428 636f 6d6d 656e 7429 290a  mment(comment)).
+00018680: 2020 2020 7772 6974 6572 2e76 6563 7772      writer.vecwr
+00018690: 6974 6528 662c 2022 5242 4532 2c7b 7d2c  ite(f, "RBE2,{},
+000186a0: 7b7d 2c31 3233 3435 362c 7b7d 5c6e 222c  {},123456,{}\n",
+000186b0: 2072 6265 3269 6473 2c20 6e65 7769 6473   rbe2ids, newids
+000186c0: 2c20 7269 6e67 315f 6964 7329 0a20 2020  , ring1_ids).   
+000186d0: 2072 6574 7572 6e20 6e65 7770 7473 2c20   return newpts, 
+000186e0: 6e65 7769 6473 0a0a 0a64 6566 205f 736f  newids...def _so
+000186f0: 7274 5f6e 5f77 7269 7465 280a 2020 2020  rt_n_write(.    
+00018700: 662c 2069 6e64 6570 656e 6465 6e74 2c20  f, independent, 
+00018710: 6369 7263 5f70 6172 6d73 2c20 6e65 7770  circ_parms, newp
+00018720: 7473 2c20 6e65 7769 6473 2c20 7269 6e67  ts, newids, ring
+00018730: 325f 6964 732c 2072 7370 6c69 6e65 5f69  2_ids, rspline_i
+00018740: 6430 2c20 446f 4c2c 206e 616d 6573 0a29  d0, DoL, names.)
+00018750: 3a0a 2020 2020 6e31 203d 2063 6972 635f  :.    n1 = circ_
+00018760: 7061 726d 735b 305d 2e6c 6f63 616c 2e73  parms[0].local.s
+00018770: 6861 7065 5b31 5d0a 2020 2020 6e32 203d  hape[1].    n2 =
+00018780: 2063 6972 635f 7061 726d 735b 315d 2e6c   circ_parms[1].l
+00018790: 6f63 616c 2e73 6861 7065 5b31 5d0a 0a20  ocal.shape[1].. 
+000187a0: 2020 2023 202d 2074 6f20 646f 2074 6869     # - to do thi
+000187b0: 7320 696e 206f 7264 6572 2c20 7765 206e  s in order, we n
+000187c0: 6565 6420 746f 2063 6f6d 7075 7465 2074  eed to compute t
+000187d0: 6865 6972 2061 6e67 6c65 730a 2020 2020  heir angles.    
+000187e0: 7468 5f31 203d 206e 702e 6172 6374 616e  th_1 = np.arctan
+000187f0: 3228 6e65 7770 7473 5b3a 2c20 315d 2c20  2(newpts[:, 1], 
+00018800: 6e65 7770 7473 5b3a 2c20 305d 290a 2020  newpts[:, 0]).  
+00018810: 2020 7232 5f6c 6f63 616c 203d 2063 6972    r2_local = cir
+00018820: 635f 7061 726d 735b 315d 2e6c 6f63 616c  c_parms[1].local
+00018830: 2e54 0a20 2020 2074 685f 3220 3d20 6e70  .T.    th_2 = np
+00018840: 2e61 7263 7461 6e32 2872 325f 6c6f 6361  .arctan2(r2_loca
+00018850: 6c5b 3a2c 2031 5d2c 2072 325f 6c6f 6361  l[:, 1], r2_loca
+00018860: 6c5b 3a2c 2030 5d29 0a20 2020 2074 6820  l[:, 0]).    th 
+00018870: 3d20 6e70 2e68 7374 6163 6b28 2874 685f  = np.hstack((th_
+00018880: 312c 2074 685f 3229 290a 2020 2020 7468  1, th_2)).    th
+00018890: 5b74 6820 3c20 2d31 652d 385d 202b 3d20  [th < -1e-8] += 
+000188a0: 3220 2a20 6e70 2e70 690a 0a20 2020 2069  2 * np.pi..    i
+000188b0: 6473 5f31 203d 206e 702e 636f 6c75 6d6e  ds_1 = np.column
+000188c0: 5f73 7461 636b 2828 6e65 7769 6473 2c20  _stack((newids, 
+000188d0: 6e70 2e7a 6572 6f73 286e 312c 206e 702e  np.zeros(n1, np.
+000188e0: 696e 7436 3429 2929 0a20 2020 2069 6473  int64))).    ids
+000188f0: 5f32 203d 206e 702e 636f 6c75 6d6e 5f73  _2 = np.column_s
+00018900: 7461 636b 2828 7269 6e67 325f 6964 732c  tack((ring2_ids,
+00018910: 206e 702e 7a65 726f 7328 6e32 2c20 6e70   np.zeros(n2, np
+00018920: 2e69 6e74 3634 2929 290a 0a20 2020 2069  .int64)))..    i
+00018930: 6620 696e 6465 7065 6e64 656e 7420 3d3d  f independent ==
+00018940: 2022 7269 6e67 3122 3a0a 2020 2020 2020   "ring1":.      
+00018950: 2020 636f 6d6d 656e 7420 3d20 280a 2020    comment = (.  
+00018960: 2020 2020 2020 2020 2020 6622 5253 504c            f"RSPL
+00018970: 494e 4520 7468 6520 7b6e 616d 6573 5b31  INE the {names[1
+00018980: 5d7d 206e 6f64 6573 2074 6f20 7468 6520  ]} nodes to the 
+00018990: 6e65 7720 6e6f 6465 7320 6372 6561 7465  new nodes create
+000189a0: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
+000189b0: 2261 626f 7665 2c20 7769 7468 2074 6865  "above, with the
+000189c0: 206e 6577 206e 6f64 6573 2062 6569 6e67   new nodes being
+000189d0: 2069 6e64 6570 656e 6465 6e74 2e22 0a20   independent.". 
+000189e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000189f0: 2069 6473 5f31 5b3a 2c20 315d 203d 2031   ids_1[:, 1] = 1
+00018a00: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00018a10: 2020 2063 6f6d 6d65 6e74 203d 2028 0a20     comment = (. 
+00018a20: 2020 2020 2020 2020 2020 2066 2252 5350             f"RSP
+00018a30: 4c49 4e45 2074 6865 206e 6577 206e 6f64  LINE the new nod
+00018a40: 6573 2063 7265 6174 6564 2061 626f 7665  es created above
+00018a50: 2074 6f20 7468 6520 7b6e 616d 6573 5b31   to the {names[1
+00018a60: 5d7d 2022 0a20 2020 2020 2020 2020 2020  ]} ".           
+00018a70: 2066 226e 6f64 6573 2c20 7769 7468 2074   f"nodes, with t
+00018a80: 6865 207b 6e61 6d65 735b 315d 7d20 6e6f  he {names[1]} no
+00018a90: 6465 7320 6265 696e 6720 696e 6465 7065  des being indepe
+00018aa0: 6e64 656e 742e 220a 2020 2020 2020 2020  ndent.".        
+00018ab0: 290a 2020 2020 2020 2020 6964 735f 325b  ).        ids_2[
+00018ac0: 3a2c 2031 5d20 3d20 310a 0a20 2020 2066  :, 1] = 1..    f
+00018ad0: 2e77 7269 7465 286d 6b63 6f6d 6d65 6e74  .write(mkcomment
+00018ae0: 2863 6f6d 6d65 6e74 2929 0a20 2020 2069  (comment)).    i
+00018af0: 6473 203d 206e 702e 7673 7461 636b 2828  ds = np.vstack((
+00018b00: 6964 735f 312c 2069 6473 5f32 2929 0a0a  ids_1, ids_2))..
+00018b10: 2020 2020 2320 736f 7274 2062 7920 616e      # sort by an
+00018b20: 6775 6c61 7220 6c6f 6361 7469 6f6e 3a0a  gular location:.
+00018b30: 2020 2020 6920 3d20 6e70 2e61 7267 736f      i = np.argso
+00018b40: 7274 2874 6829 0a20 2020 2069 6473 203d  rt(th).    ids =
+00018b50: 2069 6473 5b69 5d0a 2020 2020 6920 3d20   ids[i].    i = 
+00018b60: 300a 2020 2020 7768 696c 6520 6964 735b  0.    while ids[
+00018b70: 692c 2031 5d20 3d3d 2030 3a0a 2020 2020  i, 1] == 0:.    
+00018b80: 2020 2020 6920 2b3d 2031 0a20 2020 2023      i += 1.    #
+00018b90: 2073 7461 636b 2069 6473 2c20 656e 7375   stack ids, ensu
+00018ba0: 7269 6e67 2073 7461 7274 696e 6720 616e  ring starting an
+00018bb0: 6420 656e 6469 6e67 206e 6f64 6520 6973  d ending node is
+00018bc0: 2069 6e64 6570 656e 6465 6e74 3a0a 2020   independent:.  
+00018bd0: 2020 6964 7320 3d20 6e70 2e76 7374 6163    ids = np.vstac
+00018be0: 6b28 2869 6473 5b69 3a5d 2c20 6964 735b  k((ids[i:], ids[
+00018bf0: 3a69 5d2c 2069 6473 5b69 5d29 290a 2020  :i], ids[i])).  
+00018c00: 2020 7774 7273 706c 696e 6528 662c 2072    wtrspline(f, r
+00018c10: 7370 6c69 6e65 5f69 6430 2c20 6964 732c  spline_id0, ids,
+00018c20: 2044 6f4c 3d44 6f4c 290a 2020 2020 7265   DoL=DoL).    re
+00018c30: 7475 726e 2069 6473 0a0a 0a64 6566 205f  turn ids...def _
+00018c40: 706c 6f74 5f72 7370 6c69 6e65 280a 2020  plot_rspline(.  
+00018c50: 2020 6178 2c0a 2020 2020 6369 7263 5f70    ax,.    circ_p
+00018c60: 6172 6d73 2c0a 2020 2020 7879 7a2c 0a20  arms,.    xyz,. 
+00018c70: 2020 206e 6577 7074 732c 0a20 2020 206e     newpts,.    n
+00018c80: 6577 6964 732c 0a20 2020 2062 6173 6963  ewids,.    basic
+00018c90: 326c 6f63 616c 2c0a 2020 2020 6365 6e74  2local,.    cent
+00018ca0: 6572 2c0a 2020 2020 7273 706c 696e 655f  er,.    rspline_
+00018cb0: 6e6f 6465 732c 0a20 2020 2072 696e 6732  nodes,.    ring2
+00018cc0: 5f69 6473 2c0a 2020 2020 6e61 6d65 732c  _ids,.    names,
+00018cd0: 0a29 3a0a 2020 2020 666f 7220 6974 656d  .):.    for item
+00018ce0: 2069 6e20 2278 797a 223a 0a20 2020 2020   in "xyz":.     
+00018cf0: 2020 2067 6574 5f66 756e 6320 3d20 6765     get_func = ge
+00018d00: 7461 7474 7228 6178 2c20 6622 6765 745f  tattr(ax, f"get_
+00018d10: 7b69 7465 6d7d 6c61 6265 6c22 290a 2020  {item}label").  
+00018d20: 2020 2020 2020 6966 206e 6f74 2067 6574        if not get
+00018d30: 5f66 756e 6328 293a 0a20 2020 2020 2020  _func():.       
+00018d40: 2020 2020 2073 6574 5f66 756e 6320 3d20       set_func = 
+00018d50: 6765 7461 7474 7228 6178 2c20 6622 7365  getattr(ax, f"se
+00018d60: 745f 7b69 7465 6d7d 6c61 6265 6c22 290a  t_{item}label").
+00018d70: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+00018d80: 6675 6e63 2869 7465 6d2e 7570 7065 7228  func(item.upper(
+00018d90: 2929 0a0a 2020 2020 2320 6472 6177 2074  ))..    # draw t
+00018da0: 6865 2066 6974 2066 6f72 2063 6972 636c  he fit for circl
+00018db0: 6573 3a0a 2020 2020 7468 203d 206e 702e  es:.    th = np.
+00018dc0: 6465 6732 7261 6428 6e70 2e61 7261 6e67  deg2rad(np.arang
+00018dd0: 6528 302e 302c 2033 3631 2929 0a20 2020  e(0.0, 361)).   
+00018de0: 2066 6f72 206e 756d 2c20 2870 6172 6d73   for num, (parms
+00018df0: 2c20 6c69 6e65 2920 696e 2065 6e75 6d65  , line) in enume
+00018e00: 7261 7465 287a 6970 2863 6972 635f 7061  rate(zip(circ_pa
+00018e10: 726d 732c 2028 222b 222c 2022 7822 2929  rms, ("+", "x"))
+00018e20: 293a 0a20 2020 2020 2020 2078 203d 2070  ):.        x = p
+00018e30: 6172 6d73 2e72 6164 6975 7320 2a20 6e70  arms.radius * np
+00018e40: 2e63 6f73 2874 6829 0a20 2020 2020 2020  .cos(th).       
+00018e50: 2079 203d 2070 6172 6d73 2e72 6164 6975   y = parms.radiu
+00018e60: 7320 2a20 6e70 2e73 696e 2874 6829 0a20  s * np.sin(th). 
+00018e70: 2020 2020 2020 207a 203d 2030 202a 2078         z = 0 * x
+00018e80: 0a20 2020 2020 2020 2023 2074 7261 6e73  .        # trans
+00018e90: 666f 726d 2074 6f20 6261 7369 6320 636f  form to basic co
+00018ea0: 6f72 6469 6e61 7465 7320 616e 6420 706c  ordinates and pl
+00018eb0: 6f74 3a0a 2020 2020 2020 2020 6369 7263  ot:.        circ
+00018ec0: 6c65 5f62 6173 6963 203d 2028 0a20 2020  le_basic = (.   
+00018ed0: 2020 2020 2020 2020 2070 6172 6d73 2e63           parms.c
+00018ee0: 656e 7465 7220 2b20 286e 702e 636f 6c75  enter + (np.colu
+00018ef0: 6d6e 5f73 7461 636b 2828 782c 2079 2c20  mn_stack((x, y, 
+00018f00: 7a29 2920 4020 7061 726d 732e 6261 7369  z)) @ parms.basi
+00018f10: 6332 6c6f 6361 6c29 0a20 2020 2020 2020  c2local).       
+00018f20: 2029 2e54 0a20 2020 2020 2020 2068 203d   ).T.        h =
+00018f30: 2061 782e 706c 6f74 280a 2020 2020 2020   ax.plot(.      
+00018f40: 2020 2020 2020 2a78 797a 5b6e 756d 5d2e        *xyz[num].
+00018f50: 542c 0a20 2020 2020 2020 2020 2020 206c  T,.            l
+00018f60: 696e 652c 0a20 2020 2020 2020 2020 2020  ine,.           
+00018f70: 206d 6172 6b65 7273 697a 653d 382e 302c   markersize=8.0,
+00018f80: 0a20 2020 2020 2020 2020 2020 206d 6172  .            mar
+00018f90: 6b65 7265 6467 6577 6964 7468 3d32 2e30  keredgewidth=2.0
+00018fa0: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+00018fb0: 6265 6c3d 6622 7b6e 616d 6573 5b6e 756d  bel=f"{names[num
+00018fc0: 5d7d 206e 6f64 6573 222c 0a20 2020 2020  ]} nodes",.     
+00018fd0: 2020 2029 5b30 5d0a 2020 2020 2020 2020     )[0].        
+00018fe0: 6178 2e70 6c6f 7428 2a63 6972 636c 655f  ax.plot(*circle_
+00018ff0: 6261 7369 632c 2068 2e67 6574 5f63 6f6c  basic, h.get_col
+00019000: 6f72 2829 2c20 6c61 6265 6c3d 6622 7b6e  or(), label=f"{n
+00019010: 616d 6573 5b6e 756d 5d7d 2062 6573 742d  ames[num]} best-
+00019020: 6669 7420 6369 7263 6c65 2229 0a0a 2020  fit circle")..  
+00019030: 2020 2320 6765 7420 6261 7369 6320 636f    # get basic co
+00019040: 6f72 6469 6e61 7465 7320 6f66 206e 6577  ordinates of new
+00019050: 7074 733a 0a20 2020 206e 6577 7074 735f  pts:.    newpts_
+00019060: 6261 7369 6320 3d20 6e65 7770 7473 2040  basic = newpts @
+00019070: 2062 6173 6963 326c 6f63 616c 202b 2063   basic2local + c
+00019080: 656e 7465 720a 0a20 2020 2073 6567 6d65  enter..    segme
+00019090: 6e74 7320 3d20 6e70 2e65 6d70 7479 2828  nts = np.empty((
+000190a0: 3320 2a20 6e65 7770 7473 2e73 6861 7065  3 * newpts.shape
+000190b0: 5b30 5d2c 2033 2929 0a20 2020 2073 6567  [0], 3)).    seg
+000190c0: 6d65 6e74 735b 3a3a 335d 203d 206e 6577  ments[::3] = new
+000190d0: 7074 735f 6261 7369 630a 2020 2020 7365  pts_basic.    se
+000190e0: 676d 656e 7473 5b31 3a3a 335d 203d 2078  gments[1::3] = x
+000190f0: 797a 5b30 5d0a 2020 2020 7365 676d 656e  yz[0].    segmen
+00019100: 7473 5b32 3a3a 335d 203d 206e 702e 6e61  ts[2::3] = np.na
+00019110: 6e0a 0a20 2020 2068 203d 2061 782e 706c  n..    h = ax.pl
+00019120: 6f74 280a 2020 2020 2020 2020 2a6e 6577  ot(.        *new
+00019130: 7074 735f 6261 7369 632e 542c 0a20 2020  pts_basic.T,.   
+00019140: 2020 2020 2022 6f22 2c0a 2020 2020 2020       "o",.      
+00019150: 2020 6d61 726b 6572 7369 7a65 3d35 2e30    markersize=5.0
+00019160: 2c0a 2020 2020 2020 2020 6d61 726b 6572  ,.        marker
+00019170: 6564 6765 7769 6474 683d 322e 302c 0a20  edgewidth=2.0,. 
+00019180: 2020 2020 2020 206c 6162 656c 3d28 224e         label=("N
+00019190: 6577 207b 7d20 6e6f 6465 735c 6e20 2d20  ew {} nodes\n - 
+000191a0: 7368 6f75 6c64 2062 6520 6f6e 207b 7d20  should be on {} 
+000191b0: 6369 7263 6c65 2229 2e66 6f72 6d61 7428  circle").format(
+000191c0: 2a6e 616d 6573 292c 0a20 2020 2029 5b30  *names),.    )[0
+000191d0: 5d0a 2020 2020 6178 2e70 6c6f 7428 0a20  ].    ax.plot(. 
+000191e0: 2020 2020 2020 202a 7365 676d 656e 7473         *segments
+000191f0: 2e54 2c0a 2020 2020 2020 2020 222d 222c  .T,.        "-",
+00019200: 0a20 2020 2020 2020 2063 6f6c 6f72 3d68  .        color=h
+00019210: 2e67 6574 5f63 6f6c 6f72 2829 2c0a 2020  .get_color(),.  
+00019220: 2020 2020 2020 6c61 6265 6c3d 6622 5242        label=f"RB
+00019230: 4532 7320 2d20 7368 6f75 6c64 2062 6520  E2s - should be 
+00019240: 7b6e 616d 6573 5b30 5d7d 2072 6164 6961  {names[0]} radia
+00019250: 6c22 2c0a 2020 2020 290a 0a20 2020 2023  l",.    )..    #
+00019260: 2070 6c6f 7420 7468 6520 7273 706c 696e   plot the rsplin
+00019270: 653a 0a20 2020 2075 6e73 6f72 7465 645f  e:.    unsorted_
+00019280: 7273 706c 696e 655f 6e6f 6465 7320 3d20  rspline_nodes = 
+00019290: 6e70 2e68 7374 6163 6b28 286e 6577 6964  np.hstack((newid
+000192a0: 732c 2072 696e 6732 5f69 6473 2929 0a20  s, ring2_ids)). 
+000192b0: 2020 2070 7620 3d20 6c6f 6361 7465 2e6d     pv = locate.m
+000192c0: 6174 5f69 6e74 6572 7365 6374 2875 6e73  at_intersect(uns
+000192d0: 6f72 7465 645f 7273 706c 696e 655f 6e6f  orted_rspline_no
+000192e0: 6465 732c 2072 7370 6c69 6e65 5f6e 6f64  des, rspline_nod
+000192f0: 6573 5b3a 2c20 305d 2c20 3229 0a0a 2020  es[:, 0], 2)..  
+00019300: 2020 7273 706c 696e 655f 7879 7a20 3d20    rspline_xyz = 
+00019310: 6e70 2e76 7374 6163 6b28 286e 6577 7074  np.vstack((newpt
+00019320: 735f 6261 7369 632c 2078 797a 5b31 5d29  s_basic, xyz[1])
+00019330: 295b 7076 5b30 5d5d 0a20 2020 2061 782e  )[pv[0]].    ax.
+00019340: 706c 6f74 282a 7273 706c 696e 655f 7879  plot(*rspline_xy
+00019350: 7a2e 542c 2022 2d2d 222c 2061 6c70 6861  z.T, "--", alpha
+00019360: 3d30 2e37 2c20 6c69 6e65 7769 6474 683d  =0.7, linewidth=
+00019370: 332e 302c 206c 6162 656c 3d22 4669 6e61  3.0, label="Fina
+00019380: 6c20 5253 504c 494e 4522 290a 0a20 2020  l RSPLINE")..   
+00019390: 2079 746f 6f6c 732e 6178 6973 5f65 7175   ytools.axis_equ
+000193a0: 616c 5f33 6428 6178 290a 2020 2020 6178  al_3d(ax).    ax
+000193b0: 2e6c 6567 656e 6428 6c6f 633d 2275 7070  .legend(loc="upp
+000193c0: 6572 206c 6566 7422 2c20 6262 6f78 5f74  er left", bbox_t
+000193d0: 6f5f 616e 6368 6f72 3d28 312e 302c 2031  o_anchor=(1.0, 1
+000193e0: 2e30 2929 0a20 2020 2061 782e 6765 745f  .0)).    ax.get_
+000193f0: 6669 6775 7265 2829 2e74 6967 6874 5f6c  figure().tight_l
+00019400: 6179 6f75 7428 290a 0a0a 6465 6620 7774  ayout()...def wt
+00019410: 7273 706c 696e 655f 7269 6e67 7328 0a20  rspline_rings(. 
+00019420: 2020 2066 2c0a 2020 2020 7231 6772 6964     f,.    r1grid
+00019430: 732c 0a20 2020 2072 3267 7269 6473 2c0a  s,.    r2grids,.
+00019440: 2020 2020 6e6f 6465 5f69 6430 2c0a 2020      node_id0,.  
+00019450: 2020 7273 706c 696e 655f 6964 302c 0a20    rspline_id0,. 
+00019460: 2020 2072 6265 325f 6964 303d 4e6f 6e65     rbe2_id0=None
+00019470: 2c0a 2020 2020 636f 7264 5f69 643d 4e6f  ,.    cord_id=No
+00019480: 6e65 2c0a 2020 2020 6d61 6b65 706c 6f74  ne,.    makeplot
+00019490: 3d22 6e65 7722 2c0a 2020 2020 446f 4c3d  ="new",.    DoL=
+000194a0: 2230 2e31 222c 0a20 2020 2069 6e64 6570  "0.1",.    indep
+000194b0: 656e 6465 6e74 3d22 7269 6e67 3122 2c0a  endent="ring1",.
+000194c0: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
+000194d0: 7265 6174 6573 2061 2073 6d6f 6f74 6820  reates a smooth 
+000194e0: 5253 504c 494e 4520 746f 2063 6f6e 6e65  RSPLINE to conne
+000194f0: 6374 2074 776f 2072 696e 6773 206f 6620  ct two rings of 
+00019500: 6772 6964 730a 0a20 2020 2050 6172 616d  grids..    Param
+00019510: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00019520: 2d2d 2d2d 0a20 2020 2066 203a 2073 7472  ----.    f : str
+00019530: 696e 6720 6f72 2066 696c 655f 6c69 6b65  ing or file_like
+00019540: 206f 7220 3120 6f72 204e 6f6e 650a 2020   or 1 or None.  
+00019550: 2020 2020 2020 4569 7468 6572 2061 206e        Either a n
+00019560: 616d 6520 6f66 2061 2066 696c 652c 206f  ame of a file, o
+00019570: 7220 6973 2061 2066 696c 655f 6c69 6b65  r is a file_like
+00019580: 206f 626a 6563 7420 6173 2072 6574 7572   object as retur
+00019590: 6e65 640a 2020 2020 2020 2020 6279 203a  ned.        by :
+000195a0: 6675 6e63 3a60 6f70 656e 6020 6f72 203a  func:`open` or :
+000195b0: 636c 6173 733a 6069 6f2e 5374 7269 6e67  class:`io.String
+000195c0: 494f 602e 2049 6e70 7574 2061 7320 696e  IO`. Input as in
+000195d0: 7465 6765 7220 3120 746f 0a20 2020 2020  teger 1 to.     
+000195e0: 2020 2077 7269 7465 2074 6f20 7374 646f     write to stdo
+000195f0: 7574 2e20 4361 6e20 616c 736f 2062 6520  ut. Can also be 
+00019600: 7468 6520 6e61 6d65 206f 6620 6120 6469  the name of a di
+00019610: 7265 6374 6f72 7920 6f72 204e 6f6e 653b  rectory or None;
+00019620: 0a20 2020 2020 2020 2069 6e20 7468 6573  .        in thes
+00019630: 6520 6361 7365 732c 2061 2047 5549 2069  e cases, a GUI i
+00019640: 7320 6f70 656e 6564 2066 6f72 2066 696c  s opened for fil
+00019650: 6520 7365 6c65 6374 696f 6e2e 0a20 2020  e selection..   
+00019660: 2072 3167 7269 6473 203a 2032 6420 6172   r1grids : 2d ar
+00019670: 7261 795f 6c69 6b65 206f 7220 4461 7461  ray_like or Data
+00019680: 4672 616d 6520 6f72 2074 7570 6c65 0a20  Frame or tuple. 
+00019690: 2020 2020 2020 2049 676e 6f72 696e 6720         Ignoring 
+000196a0: 7468 6520 7475 706c 6520 696e 7075 7420  the tuple input 
+000196b0: 6f70 7469 6f6e 2066 6f72 206e 6f77 2c20  option for now, 
+000196c0: 6072 3167 7269 6473 6020 636f 6e74 6169  `r1grids` contai
+000196d0: 6e73 0a20 2020 2020 2020 2074 6865 2069  ns.        the i
+000196e0: 6473 2061 6e64 206c 6f63 6174 696f 6e73  ds and locations
+000196f0: 206f 6620 7468 6520 7269 6e67 2031 2067   of the ring 1 g
+00019700: 7269 6473 2069 6e20 6261 7369 630a 2020  rids in basic.  
+00019710: 2020 2020 2020 636f 6f72 6469 6e61 7465        coordinate
+00019720: 732e 2049 6620 3264 2061 7272 6179 5f6c  s. If 2d array_l
+00019730: 696b 652c 2069 7420 6861 7320 3420 636f  ike, it has 4 co
+00019740: 6c75 6d6e 7320 6465 7363 7269 6269 6e67  lumns describing
+00019750: 2074 6865 0a20 2020 2020 2020 2072 696e   the.        rin
+00019760: 6720 3120 6772 6964 733a 3a0a 0a20 2020  g 1 grids::..   
+00019770: 2020 2020 2020 2020 2020 5b69 642c 2078            [id, x
+00019780: 2c20 792c 207a 5d20 3c20 2d2d 2062 6173  , y, z] < -- bas
+00019790: 6963 2063 6f6f 7264 696e 6174 6573 0a0a  ic coordinates..
+000197a0: 2020 2020 2020 2020 4966 2044 6174 6146          If DataF
+000197b0: 7261 6d65 2c20 6974 2069 7320 6173 7375  rame, it is assu
+000197c0: 6d65 6420 746f 2062 6520 7468 6520 5553  med to be the US
+000197d0: 4554 2044 6174 6146 7261 6d65 0a20 2020  ET DataFrame.   
+000197e0: 2020 2020 2063 6f6e 7461 696e 696e 6720       containing 
+000197f0: 6a75 7374 2074 6865 2072 696e 6720 3120  just the ring 1 
+00019800: 6772 6964 732e 2054 6865 2066 6f72 6d61  grids. The forma
+00019810: 7420 6f66 2074 6869 730a 2020 2020 2020  t of this.      
+00019820: 2020 4461 7461 4672 616d 6520 6973 2064    DataFrame is d
+00019830: 6573 6372 6962 6564 2069 6e0a 2020 2020  escribed in.    
+00019840: 2020 2020 3a66 756e 633a 6070 7979 6574      :func:`pyyet
+00019850: 692e 6e61 7374 7261 6e2e 6f70 322e 4f50  i.nastran.op2.OP
+00019860: 322e 7264 6e32 636f 7032 602e 0a0a 2020  2.rdn2cop2`...  
+00019870: 2020 2020 2020 5468 6520 6465 6661 756c        The defaul
+00019880: 7420 6e61 6d65 2069 6e20 7468 6520 6f75  t name in the ou
+00019890: 7470 7574 2063 6f6d 6d65 6e74 7320 666f  tput comments fo
+000198a0: 7220 7269 6e67 2031 2069 7320 2752 696e  r ring 1 is 'Rin
+000198b0: 670a 2020 2020 2020 2020 3127 2e20 4279  g.        1'. By
+000198c0: 2075 7369 6e67 2074 6865 2074 7570 6c65   using the tuple
+000198d0: 2069 6e70 7574 206f 7074 696f 6e2c 2079   input option, y
+000198e0: 6f75 2063 616e 2070 726f 7669 6465 2061  ou can provide a
+000198f0: 0a20 2020 2020 2020 206e 616d 652e 2046  .        name. F
+00019900: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
+00019910: 6465 6661 756c 7420 6973 2065 7175 6976  default is equiv
+00019920: 616c 656e 7420 746f 3a3a 0a0a 2020 2020  alent to::..    
+00019930: 2020 2020 2020 2020 2827 5269 6e67 2031          ('Ring 1
+00019940: 272c 2072 3167 7269 6473 290a 0a20 2020  ', r1grids)..   
+00019950: 2020 2020 202e 2e20 6e6f 7465 3a3a 0a20       .. note::. 
+00019960: 2020 2020 2020 2020 2020 2020 4e6f 7465              Note
+00019970: 2074 6861 7420 7768 656e 2075 7369 6e67   that when using
+00019980: 2061 2055 5345 5420 7461 626c 652c 2074   a USET table, t
+00019990: 6865 2067 7269 6473 2063 616e 2062 650a  he grids can be.
+000199a0: 2020 2020 2020 2020 2020 2020 2064 6566               def
+000199b0: 696e 6564 2069 6e20 616e 7920 6c6f 6361  ined in any loca
+000199c0: 6c20 636f 6f72 6469 6e61 7465 2073 7973  l coordinate sys
+000199d0: 7465 6d28 7329 2e20 486f 7765 7665 722c  tem(s). However,
+000199e0: 2062 6f74 680a 2020 2020 2020 2020 2020   both.          
+000199f0: 2020 2060 7231 6772 6964 7360 2061 6e64     `r1grids` and
+00019a00: 2060 7232 6772 6964 7360 206d 7573 7420   `r2grids` must 
+00019a10: 7573 6520 7468 6520 7361 6d65 2062 6173  use the same bas
+00019a20: 6963 0a20 2020 2020 2020 2020 2020 2020  ic.             
+00019a30: 636f 6f72 6469 6e61 7465 2073 7973 7465  coordinate syste
+00019a40: 6d2e 0a0a 2020 2020 7232 6772 6964 7320  m...    r2grids 
+00019a50: 3a20 3264 2061 7272 6179 5f6c 696b 6520  : 2d array_like 
+00019a60: 6f72 2044 6174 6146 7261 6d65 206f 7220  or DataFrame or 
+00019a70: 7475 706c 650a 2020 2020 2020 2020 436f  tuple.        Co
+00019a80: 6e74 6169 6e73 2074 6865 2069 6473 2061  ntains the ids a
+00019a90: 6e64 206c 6f63 6174 696f 6e73 2028 616e  nd locations (an
+00019aa0: 6420 6f70 7469 6f6e 616c 6c79 2c20 7468  d optionally, th
+00019ab0: 6520 6e61 6d65 2920 6f66 0a20 2020 2020  e name) of.     
+00019ac0: 2020 2074 6865 2072 696e 6720 3220 6772     the ring 2 gr
+00019ad0: 6964 7320 696e 2062 6173 6963 2063 6f6f  ids in basic coo
+00019ae0: 7264 696e 6174 6573 2e20 5365 6520 6072  rdinates. See `r
+00019af0: 3167 7269 6473 6020 666f 720a 2020 2020  1grids` for.    
+00019b00: 2020 2020 6465 7363 7269 7074 696f 6e20      description 
+00019b10: 6f66 2066 6f72 6d61 742e 2054 6865 2064  of format. The d
+00019b20: 6566 6175 6c74 206e 616d 6520 666f 7220  efault name for 
+00019b30: 7269 6e67 2032 2069 7320 2752 696e 670a  ring 2 is 'Ring.
+00019b40: 2020 2020 2020 2020 3227 2e0a 2020 2020          2'..    
+00019b50: 6e6f 6465 5f69 6430 203a 2069 6e74 6567  node_id0 : integ
+00019b60: 6572 0a20 2020 2020 2020 2031 7374 2069  er.        1st i
+00019b70: 6420 6f66 206e 6577 206e 6f64 6573 2063  d of new nodes c
+00019b80: 7265 6174 6564 2074 6f20 276d 6f76 6527  reated to 'move'
+00019b90: 2072 696e 6720 3120 6e6f 6465 730a 2020   ring 1 nodes.  
+00019ba0: 2020 7273 706c 696e 655f 6964 3020 3a20    rspline_id0 : 
+00019bb0: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
+00019bc0: 3173 7420 6964 206f 6620 5253 504c 494e  1st id of RSPLIN
+00019bd0: 4573 0a20 2020 2072 6265 325f 6964 3020  Es.    rbe2_id0 
+00019be0: 3a20 696e 7465 6765 7220 6f72 204e 6f6e  : integer or Non
+00019bf0: 653b 206f 7074 696f 6e61 6c0a 2020 2020  e; optional.    
+00019c00: 2020 2020 3173 7420 6964 206f 6620 5242      1st id of RB
+00019c10: 4532 2065 6c65 6d65 6e74 7320 7468 6174  E2 elements that
+00019c20: 2077 696c 6c20 636f 6e6e 6563 7420 6f6c   will connect ol
+00019c30: 6420 7269 6e67 2031 206e 6f64 6573 2074  d ring 1 nodes t
+00019c40: 6f0a 2020 2020 2020 2020 6e65 7720 6f6e  o.        new on
+00019c50: 6573 2e20 4966 204e 6f6e 652c 2060 6072  es. If None, ``r
+00019c60: 6265 325f 6964 3020 3d20 6e6f 6465 5f69  be2_id0 = node_i
+00019c70: 6430 6060 2e0a 2020 2020 636f 7264 5f69  d0``..    cord_i
+00019c80: 6420 3a20 696e 7465 6765 7220 6f72 204e  d : integer or N
+00019c90: 6f6e 653b 206f 7074 696f 6e61 6c0a 2020  one; optional.  
+00019ca0: 2020 2020 2020 4944 2066 6f72 2074 6865        ID for the
+00019cb0: 206c 6f63 616c 2063 6f6f 7264 696e 6174   local coordinat
+00019cc0: 6520 7379 7374 656d 2066 6f72 2074 6865  e system for the
+00019cd0: 2060 7231 6772 6964 7360 2e20 4966 204e   `r1grids`. If N
+00019ce0: 6f6e 652c 0a20 2020 2020 2020 2069 7420  one,.        it 
+00019cf0: 6973 2073 6574 2074 6f20 6060 6e6f 6465  is set to ``node
+00019d00: 5f69 6430 202a 2031 3060 602e 0a20 2020  _id0 * 10``..   
+00019d10: 206d 616b 6570 6c6f 7420 3a20 7374 7269   makeplot : stri
+00019d20: 6e67 206f 7220 6178 6573 206f 626a 6563  ng or axes objec
+00019d30: 743b 206f 7074 696f 6e61 6c0a 2020 2020  t; optional.    
+00019d40: 2020 2020 5370 6563 6966 6965 7320 6966      Specifies if
+00019d50: 2061 6e64 2068 6f77 2074 6f20 706c 6f74   and how to plot
+00019d60: 2064 6174 6120 7368 6f77 696e 6720 7468   data showing th
+00019d70: 6520 5253 504c 494e 452e 0a0a 2020 2020  e RSPLINE...    
+00019d80: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d20      =========== 
+00019d90: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
+00019da0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019db0: 3d0a 2020 2020 2020 2020 606d 616b 6570  =.        `makep
+00019dc0: 6c6f 7460 2020 2020 4465 7363 7269 7074  lot`    Descript
+00019dd0: 696f 6e0a 2020 2020 2020 2020 3d3d 3d3d  ion.        ====
+00019de0: 3d3d 3d3d 3d3d 3d20 2020 3d3d 3d3d 3d3d  =======   ======
+00019df0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019e00: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2020  =========.      
+00019e10: 2020 2020 2020 276e 6f27 2020 2020 2020        'no'      
+00019e20: 646f 206e 6f74 2070 6c6f 740a 2020 2020  do not plot.    
+00019e30: 2020 2020 2027 636c 6561 7227 2020 2020       'clear'    
+00019e40: 2020 706c 6f74 2061 6674 6572 2063 6c65    plot after cle
+00019e50: 6172 696e 6720 6669 6775 7265 0a20 2020  aring figure.   
+00019e60: 2020 2020 2020 2020 2761 6464 2720 2020          'add'   
+00019e70: 2020 2070 6c6f 7420 7769 7468 6f75 7420     plot without 
+00019e80: 636c 6561 7269 6e67 2066 6967 7572 650a  clearing figure.
+00019e90: 2020 2020 2020 2020 2020 2027 6e65 7727             'new'
+00019ea0: 2020 2020 2020 706c 6f74 2069 6e20 6e65        plot in ne
+00019eb0: 7720 6669 6775 7265 0a20 2020 2020 2020  w figure.       
+00019ec0: 2061 7865 7320 6f62 6a65 6374 2020 2070   axes object   p
+00019ed0: 6c6f 7420 696e 2067 6976 656e 2061 7865  lot in given axe
+00019ee0: 7320 286c 696b 6520 2761 6464 2729 0a20  s (like 'add'). 
+00019ef0: 2020 2020 2020 203d 3d3d 3d3d 3d3d 3d3d         =========
+00019f00: 3d3d 2020 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ==   ===========
+00019f10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019f20: 3d3d 3d3d 0a0a 2020 2020 2020 2020 4e6f  ====..        No
+00019f30: 7465 2074 6861 7420 6966 2060 6d61 6b65  te that if `make
+00019f40: 706c 6f74 6020 6973 2027 6164 6427 206f  plot` is 'add' o
+00019f50: 7220 616e 2061 7865 7320 6f62 6a65 6374  r an axes object
+00019f60: 2c20 6974 206d 7573 7420 6265 0a20 2020  , it must be.   
+00019f70: 2020 2020 2033 643b 206f 7468 6572 7769       3d; otherwi
+00019f80: 7365 2061 2056 616c 7565 4572 726f 7220  se a ValueError 
+00019f90: 6578 6365 7074 696f 6e20 6973 2072 6169  exception is rai
+00019fa0: 7365 642e 0a0a 2020 2020 446f 4c20 3a20  sed...    DoL : 
+00019fb0: 7374 7269 6e67 206f 7220 7265 616c 2073  string or real s
+00019fc0: 6361 6c61 723b 206f 7074 696f 6e61 6c0a  calar; optional.
+00019fd0: 2020 2020 2020 2020 5370 6563 6966 6965          Specifie
+00019fe0: 7320 7261 7469 6f20 6f66 2064 6961 6d65  s ratio of diame
+00019ff0: 7465 7220 6f66 2065 6c61 7374 6963 2074  ter of elastic t
+0001a000: 7962 6520 746f 2074 6865 2073 756d 206f  ybe to the sum o
+0001a010: 6620 7468 650a 2020 2020 2020 2020 6c65  f the.        le
+0001a020: 6e67 7468 7320 6f66 2061 6c6c 2073 6567  ngths of all seg
+0001a030: 6d65 6e74 732e 2057 7269 7474 656e 2077  ments. Written w
+0001a040: 6974 683a 2060 6066 277b 446f 4c3a 3c38  ith: ``f'{DoL:<8
+0001a050: 7d27 6060 0a20 2020 2069 6e64 6570 656e  }'``.    indepen
+0001a060: 6465 6e74 203a 2073 7472 3b20 6f70 7469  dent : str; opti
+0001a070: 6f6e 616c 0a20 2020 2020 2020 2045 6974  onal.        Eit
+0001a080: 6865 7220 2772 696e 6731 2720 6f72 2027  her 'ring1' or '
+0001a090: 7269 6e67 3227 206f 7220 7468 6520 6173  ring2' or the as
+0001a0a0: 7369 676e 6564 206e 616d 6520 6966 206f  signed name if o
+0001a0b0: 6e65 2077 6173 0a20 2020 2020 2020 2070  ne was.        p
+0001a0c0: 726f 7669 6465 6420 696e 2074 6865 2060  rovided in the `
+0001a0d0: 7231 6772 6964 7360 206f 7220 6072 3267  r1grids` or `r2g
+0001a0e0: 7269 6473 6020 696e 7075 742e 2054 6869  rids` input. Thi
+0001a0f0: 7320 696e 7075 7420 6973 0a20 2020 2020  s input is.     
+0001a100: 2020 2063 6173 652d 696e 7365 6e73 6974     case-insensit
+0001a110: 6976 6520 616e 6420 616c 6c20 7370 6163  ive and all spac
+0001a120: 6573 2061 7265 2069 676e 6f72 6564 2c20  es are ignored, 
+0001a130: 736f 2027 5269 6e67 2031 2720 6973 0a20  so 'Ring 1' is. 
+0001a140: 2020 2020 2020 2074 6865 2073 616d 6520         the same 
+0001a150: 6173 2027 7269 6e67 3127 2e20 5370 6563  as 'ring1'. Spec
+0001a160: 6966 6965 7320 7768 6963 6820 7269 6e67  ifies which ring
+0001a170: 2077 696c 6c20 6265 2069 6e64 6570 656e   will be indepen
+0001a180: 6465 6e74 0a20 2020 2020 2020 206f 6e20  dent.        on 
+0001a190: 7468 6520 5253 504c 494e 4573 2e20 4e6f  the RSPLINEs. No
+0001a1a0: 7465 2074 6861 7420 6973 2064 6966 6665  te that is diffe
+0001a1b0: 7265 6e74 2074 6861 6e20 6a75 7374 2073  rent than just s
+0001a1c0: 7769 7463 6869 6e67 0a20 2020 2020 2020  witching.       
+0001a1d0: 2074 6865 206f 7264 6572 206f 6620 6072   the order of `r
+0001a1e0: 3167 7269 6473 6020 616e 6420 6072 3267  1grids` and `r2g
+0001a1f0: 7269 6473 602e 2054 6869 7320 6f70 7469  rids`. This opti
+0001a200: 6f6e 206d 6f64 6966 6965 730a 2020 2020  on modifies.    
+0001a210: 2020 2020 7374 6570 2034 2062 656c 6f77      step 4 below
+0001a220: 2077 6869 6c65 2073 7769 7463 6869 6e67   while switching
+0001a230: 2060 7231 6772 6964 7360 2061 6e64 2060   `r1grids` and `
+0001a240: 7232 6772 6964 7360 206d 6f64 6966 6965  r2grids` modifie
+0001a250: 730a 2020 2020 2020 2020 616c 6c20 7468  s.        all th
+0001a260: 6520 7374 6570 732e 0a0a 2020 2020 5265  e steps...    Re
+0001a270: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0001a280: 2d0a 2020 2020 4e6f 6e65 0a0a 2020 2020  -.    None..    
+0001a290: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+0001a2a0: 2020 2020 5468 6973 2072 6f75 7469 6e65      This routine
+0001a2b0: 2077 7269 7465 7320 4752 4944 2c20 5242   writes GRID, RB
+0001a2c0: 4532 2061 6e64 2052 5350 4c49 4e45 206c  E2 and RSPLINE l
+0001a2d0: 696e 6573 2074 6f20 7468 6520 6f75 7470  ines to the outp
+0001a2e0: 7574 0a20 2020 2066 696c 652e 0a0a 2020  ut.    file...  
+0001a2f0: 2020 5468 6520 6170 7072 6f61 6368 2069    The approach i
+0001a300: 7320 6173 2066 6f6c 6c6f 7773 2028 4e20  s as follows (N 
+0001a310: 3d20 6e75 6d62 6572 206f 6620 7269 6e67  = number of ring
+0001a320: 2031 2067 7269 6473 293a 0a0a 2020 2020   1 grids):..    
+0001a330: 2020 312e 2046 6974 2061 2063 6972 636c    1. Fit a circl
+0001a340: 6520 7468 726f 7567 6820 626f 7468 2074  e through both t
+0001a350: 6865 2072 696e 6720 3120 6e6f 6465 7320  he ring 1 nodes 
+0001a360: 616e 6420 7468 6520 7269 6e67 2032 0a20  and the ring 2. 
+0001a370: 2020 2020 2020 2020 6e6f 6465 732e 2041          nodes. A
+0001a380: 206e 6577 2022 7269 6e67 2031 2220 6c6f   new "ring 1" lo
+0001a390: 6361 6c20 636f 6f72 6469 6e61 7465 2073  cal coordinate s
+0001a3a0: 7973 7465 6d20 6973 2064 6566 696e 6564  ystem is defined
+0001a3b0: 2028 7365 650a 2020 2020 2020 2020 203a   (see.         :
+0001a3c0: 6675 6e63 3a60 7079 7965 7469 2e79 746f  func:`pyyeti.yto
+0001a3d0: 6f6c 732e 6669 745f 6369 7263 6c65 5f33  ols.fit_circle_3
+0001a3e0: 6460 2920 746f 2073 696d 706c 6966 7920  d`) to simplify 
+0001a3f0: 7468 6520 6372 6561 7469 6f6e 0a20 2020  the creation.   
+0001a400: 2020 2020 2020 6f66 2074 6865 206e 6577        of the new
+0001a410: 2052 5350 4c49 4e45 2e20 496e 2074 6865   RSPLINE. In the
+0001a420: 206c 6f63 616c 2073 7973 7465 6d2c 207a   local system, z
+0001a430: 2069 7320 7065 7270 656e 6469 6375 6c61   is perpendicula
+0001a440: 720a 2020 2020 2020 2020 2074 6f20 7468  r.         to th
+0001a450: 6520 706c 616e 6520 6f66 2074 6865 2063  e plane of the c
+0001a460: 6972 636c 6520 616e 6420 7820 6973 2061  ircle and x is a
+0001a470: 6c69 676e 6564 2077 6974 6820 6e6f 6465  ligned with node
+0001a480: 2031 206f 660a 2020 2020 2020 2020 2072   1 of.         r
+0001a490: 696e 6720 312e 0a20 2020 2020 2032 2e20  ing 1..      2. 
+0001a4a0: 4372 6561 7465 204e 206e 6577 2072 696e  Create N new rin
+0001a4b0: 6720 3120 6772 6964 7320 6174 2073 7461  g 1 grids at sta
+0001a4c0: 7469 6f6e 2061 6e64 2072 6164 6975 7320  tion and radius 
+0001a4d0: 6f66 2072 696e 6720 320a 2020 2020 2020  of ring 2.      
+0001a4e0: 2020 2067 7269 6473 2c20 6275 7420 6174     grids, but at
+0001a4f0: 2074 6865 2073 616d 6520 616e 6775 6c61   the same angula
+0001a500: 7220 6c6f 6361 7469 6f6e 2061 7320 6f72  r location as or
+0001a510: 6967 696e 616c 204e 2e0a 2020 2020 2020  iginal N..      
+0001a520: 332e 2052 4245 3220 7468 6573 6520 6e65  3. RBE2 these ne
+0001a530: 7720 6772 6964 7320 746f 2074 6865 204e  w grids to the N
+0001a540: 206f 7269 6769 6e61 6c20 6772 6964 732e   original grids.
+0001a550: 2054 6865 206e 6577 2067 7269 6473 0a20   The new grids. 
+0001a560: 2020 2020 2020 2020 6172 6520 696e 6465          are inde
+0001a570: 7065 6e64 656e 742e 0a20 2020 2020 2034  pendent..      4
+0001a580: 2e20 5772 6974 6520 5253 504c 494e 4520  . Write RSPLINE 
+0001a590: 6361 7264 7320 7573 696e 6720 3a66 756e  cards using :fun
+0001a5a0: 633a 6077 7472 7370 6c69 6e65 602e 2054  c:`wtrspline`. T
+0001a5b0: 6865 2066 6972 7374 0a20 2020 2020 2020  he first.       
+0001a5c0: 2020 5253 504c 494e 4520 7374 6172 7473    RSPLINE starts
+0001a5d0: 2061 7420 7468 6520 696e 6465 7065 6e64   at the independ
+0001a5e0: 656e 7420 6772 6964 2028 6f6e 2072 696e  ent grid (on rin
+0001a5f0: 6720 3120 6f72 2072 696e 6720 320a 2020  g 1 or ring 2.  
+0001a600: 2020 2020 2020 2061 6363 6f72 6469 6e67         according
+0001a610: 2074 6f20 6069 6e64 6570 656e 6465 6e74   to `independent
+0001a620: 6029 2077 6974 6820 7468 6520 6c6f 7765  `) with the lowe
+0001a630: 7374 2061 6e67 756c 6172 0a20 2020 2020  st angular.     
+0001a640: 2020 2020 6c6f 6361 7469 6f6e 2e20 5468      location. Th
+0001a650: 6520 616e 6775 6c61 7220 6c6f 6361 7469  e angular locati
+0001a660: 6f6e 7320 7261 6e67 6520 6672 6f6d 2030  ons range from 0
+0001a670: 2074 6f20 3336 3020 6465 6772 6565 732c   to 360 degrees,
+0001a680: 0a20 2020 2020 2020 2020 636f 756e 7465  .         counte
+0001a690: 722d 636c 6f63 6b77 6973 652e 2054 6865  r-clockwise. The
+0001a6a0: 2052 5350 4c49 4e45 7320 7072 6f63 6565   RSPLINEs procee
+0001a6b0: 6420 636f 756e 7465 722d 636c 6f63 6b77  d counter-clockw
+0001a6c0: 6973 650a 2020 2020 2020 2020 2061 726f  ise.         aro
+0001a6d0: 756e 6420 7468 6520 6369 7263 6c65 2e0a  und the circle..
+0001a6e0: 0a20 2020 2053 6565 2061 6c73 6f0a 2020  .    See also.  
+0001a6f0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203a    --------.    :
+0001a700: 6675 6e63 3a60 7774 7273 706c 696e 6560  func:`wtrspline`
+0001a710: 0a0a 2020 2020 5261 6973 6573 0a20 2020  ..    Raises.   
+0001a720: 202d 2d2d 2d2d 2d0a 2020 2020 5661 6c75   ------.    Valu
+0001a730: 6545 7272 6f72 0a0a 2020 2020 2020 2020  eError..        
+0001a740: 5768 656e 2074 6865 2070 6572 7065 6e64  When the perpend
+0001a750: 6963 756c 6172 2064 6972 6563 7469 6f6e  icular direction
+0001a760: 7320 6f66 2060 7231 6772 6964 7360 2061  s of `r1grids` a
+0001a770: 6e64 2060 7232 6772 6964 7360 0a20 2020  nd `r2grids`.   
+0001a780: 2020 2020 2064 6f20 6e6f 7420 6d61 7463       do not matc
+0001a790: 6820 7769 7468 696e 2074 6f6c 6572 616e  h within toleran
+0001a7a0: 6365 3a20 6162 736f 6c75 7465 2076 616c  ce: absolute val
+0001a7b0: 7565 206f 6620 7468 6520 636f 7369 6e65  ue of the cosine
+0001a7c0: 206f 660a 2020 2020 2020 2020 7468 6520   of.        the 
+0001a7d0: 616e 676c 6520 6265 7477 6565 6e20 7468  angle between th
+0001a7e0: 6520 7477 6f20 7065 7270 656e 6469 6375  e two perpendicu
+0001a7f0: 6c61 7220 6469 7265 6374 696f 6e73 206d  lar directions m
+0001a800: 7573 7420 6265 203e 0a20 2020 2020 2020  ust be >.       
+0001a810: 2030 2e39 392e 0a0a 2020 2020 2020 2020   0.99...        
+0001a820: 5768 656e 2061 2060 7231 6772 6964 7360  When a `r1grids`
+0001a830: 206f 7220 6072 3267 7269 6473 6020 4461   or `r2grids` Da
+0001a840: 7461 4672 616d 6520 646f 6573 206e 6f74  taFrame does not
+0001a850: 2068 6176 6520 610a 2020 2020 2020 2020   have a.        
+0001a860: 6d75 6c74 6970 6c65 206f 6620 3620 726f  multiple of 6 ro
+0001a870: 7773 2e0a 0a20 2020 2020 2020 2057 6865  ws...        Whe
+0001a880: 6e20 7468 6520 606d 616b 6570 6c6f 7460  n the `makeplot`
+0001a890: 206f 7074 696f 6e20 7472 6965 7320 746f   option tries to
+0001a8a0: 2061 6464 2074 6f20 616e 2061 7865 7320   add to an axes 
+0001a8b0: 6f62 6a65 6374 2074 6861 740a 2020 2020  object that.    
+0001a8c0: 2020 2020 6973 206e 6f74 2075 7369 6e67      is not using
+0001a8d0: 2061 2033 6420 7072 6f6a 6563 7469 6f6e   a 3d projection
+0001a8e0: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+0001a8f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001a900: 2044 6566 696e 6520 7477 6f20 7269 6e67   Define two ring
+0001a910: 7320 6f66 2067 7269 6473 3a0a 0a20 2020  s of grids:..   
+0001a920: 2031 2e20 5269 6e67 2031 2077 696c 6c20   1. Ring 1 will 
+0001a930: 6265 2061 7420 7374 6174 696f 6e20 302e  be at station 0.
+0001a940: 3020 7769 7468 2035 206e 6f64 6573 206f  0 with 5 nodes o
+0001a950: 6e20 7269 6e67 206f 6620 7261 6469 7573  n ring of radius
+0001a960: 0a20 2020 2020 2020 3530 2e20 4944 7320  .       50. IDs 
+0001a970: 7769 6c6c 2062 6520 3120 746f 2035 2e0a  will be 1 to 5..
+0001a980: 0a20 2020 2032 2e20 5269 6e67 2032 2077  .    2. Ring 2 w
+0001a990: 696c 6c20 6265 2061 7420 7374 6174 696f  ill be at statio
+0001a9a0: 6e20 312e 3020 7769 7468 2037 206e 6f64  n 1.0 with 7 nod
+0001a9b0: 6573 206f 6e20 7269 6e67 206f 6620 7261  es on ring of ra
+0001a9c0: 6469 7573 0a20 2020 2020 2020 3435 2e20  dius.       45. 
+0001a9d0: 4944 7320 7769 6c6c 2062 6520 3130 3120  IDs will be 101 
+0001a9e0: 746f 2031 3037 2e0a 0a20 2020 2046 6f72  to 107...    For
+0001a9f0: 2064 656d 6f6e 7374 7261 7469 6f6e 2c20   demonstration, 
+0001aa00: 7269 6e67 2031 2077 696c 6c20 6265 206e  ring 1 will be n
+0001aa10: 616d 6564 2027 5370 6163 6563 7261 6674  amed 'Spacecraft
+0001aa20: 2720 7768 696c 6520 7468 650a 2020 2020  ' while the.    
+0001aa30: 6465 6661 756c 7420 7769 6c6c 2062 6520  default will be 
+0001aa40: 6163 6365 7074 6564 2066 6f72 2072 696e  accepted for rin
+0001aa50: 6720 3220 2877 6869 6368 2069 7320 2752  g 2 (which is 'R
+0001aa60: 696e 6720 3227 292e 0a0a 2020 2020 2e2e  ing 2')...    ..
+0001aa70: 2070 6c6f 743a 3a0a 2020 2020 2020 2020   plot::.        
+0001aa80: 3a63 6f6e 7465 7874 3a20 636c 6f73 652d  :context: close-
+0001aa90: 6669 6773 0a0a 2020 2020 2020 2020 3e3e  figs..        >>
+0001aaa0: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
+0001aab0: 7320 6e70 0a20 2020 2020 2020 203e 3e3e  s np.        >>>
+0001aac0: 2069 6d70 6f72 7420 6d61 7470 6c6f 746c   import matplotl
+0001aad0: 6962 2e70 7970 6c6f 7420 6173 2070 6c74  ib.pyplot as plt
+0001aae0: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
+0001aaf0: 6d20 7079 7965 7469 2069 6d70 6f72 7420  m pyyeti import 
+0001ab00: 6e61 7374 7261 6e0a 2020 2020 2020 2020  nastran.        
+0001ab10: 3e3e 3e20 7468 6574 6131 203d 206e 702e  >>> theta1 = np.
+0001ab20: 6172 616e 6765 2830 2c20 3335 392c 2033  arange(0, 359, 3
+0001ab30: 3630 2f35 292a 6e70 2e70 692f 3138 300a  60/5)*np.pi/180.
+0001ab40: 2020 2020 2020 2020 3e3e 3e20 7261 6431          >>> rad1
+0001ab50: 203d 2035 302e 0a20 2020 2020 2020 203e   = 50..        >
+0001ab60: 3e3e 2073 7461 3120 3d20 302e 0a20 2020  >> sta1 = 0..   
+0001ab70: 2020 2020 203e 3e3e 206e 3120 3d20 6c65       >>> n1 = le
+0001ab80: 6e28 7468 6574 6131 290a 2020 2020 2020  n(theta1).      
+0001ab90: 2020 3e3e 3e20 7269 6e67 3120 3d20 6e70    >>> ring1 = np
+0001aba0: 2e76 7374 6163 6b28 286e 702e 6172 616e  .vstack((np.aran
+0001abb0: 6765 2831 2c20 6e31 2b31 292c 2020 2020  ge(1, n1+1),    
+0001abc0: 2020 2320 4944 0a20 2020 2020 2020 202e    # ID.        .
+0001abd0: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
+0001abe0: 2020 2020 2020 7374 6131 2a6e 702e 6f6e        sta1*np.on
+0001abf0: 6573 286e 3129 2c20 2020 2020 2020 2023  es(n1),        #
+0001ac00: 2078 0a20 2020 2020 2020 202e 2e2e 2020   x.        ...  
+0001ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac20: 2020 7261 6431 2a6e 702e 636f 7328 7468    rad1*np.cos(th
+0001ac30: 6574 6131 292c 2020 2020 2023 2079 0a20  eta1),     # y. 
+0001ac40: 2020 2020 2020 202e 2e2e 2020 2020 2020         ...      
+0001ac50: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0001ac60: 6431 2a6e 702e 7369 6e28 7468 6574 6131  d1*np.sin(theta1
+0001ac70: 2929 292e 5420 2023 207a 0a20 2020 2020  ))).T  # z.     
+0001ac80: 2020 203e 3e3e 2023 2050 726f 7669 6465     >>> # Provide
+0001ac90: 2061 206e 616d 6520 666f 7220 7269 6e67   a name for ring
+0001aca0: 2031 3a0a 2020 2020 2020 2020 3e3e 3e20   1:.        >>> 
+0001acb0: 7269 6e67 3120 3d20 2827 5370 6163 6563  ring1 = ('Spacec
+0001acc0: 7261 6674 272c 2072 696e 6731 290a 2020  raft', ring1).  
+0001acd0: 2020 2020 2020 3e3e 3e20 7468 6574 6132        >>> theta2
+0001ace0: 203d 206e 702e 6172 616e 6765 2831 302c   = np.arange(10,
+0001acf0: 2033 3539 2c20 3336 302f 3729 2a6e 702e   359, 360/7)*np.
+0001ad00: 7069 2f31 3830 0a20 2020 2020 2020 203e  pi/180.        >
+0001ad10: 3e3e 2072 6164 3220 3d20 3435 2e0a 2020  >> rad2 = 45..  
+0001ad20: 2020 2020 2020 3e3e 3e20 7374 6132 203d        >>> sta2 =
+0001ad30: 2031 2e0a 2020 2020 2020 2020 3e3e 3e20   1..        >>> 
+0001ad40: 6e32 203d 206c 656e 2874 6865 7461 3229  n2 = len(theta2)
+0001ad50: 0a20 2020 2020 2020 203e 3e3e 2072 696e  .        >>> rin
+0001ad60: 6732 203d 206e 702e 7673 7461 636b 2828  g2 = np.vstack((
+0001ad70: 6e70 2e61 7261 6e67 6528 312c 206e 322b  np.arange(1, n2+
+0001ad80: 3129 2b31 3030 2c20 2023 2049 440a 2020  1)+100,  # ID.  
+0001ad90: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+0001ada0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0001adb0: 322a 6e70 2e6f 6e65 7328 6e32 292c 2020  2*np.ones(n2),  
+0001adc0: 2020 2020 2020 2320 780a 2020 2020 2020        # x.      
+0001add0: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
+0001ade0: 2020 2020 2020 2020 2072 6164 322a 6e70           rad2*np
+0001adf0: 2e63 6f73 2874 6865 7461 3229 2c20 2020  .cos(theta2),   
+0001ae00: 2020 2320 790a 2020 2020 2020 2020 2e2e    # y.        ..
+0001ae10: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ae20: 2020 2020 2072 6164 322a 6e70 2e73 696e       rad2*np.sin
+0001ae30: 2874 6865 7461 3229 2929 2e54 2020 2320  (theta2))).T  # 
+0001ae40: 7a0a 2020 2020 2020 2020 3e3e 3e20 6669  z.        >>> fi
+0001ae50: 6720 3d20 706c 742e 6669 6775 7265 2827  g = plt.figure('
+0001ae60: 4578 616d 706c 6527 2c20 6669 6773 697a  Example', figsiz
+0001ae70: 653d 2838 2c20 3629 290a 2020 2020 2020  e=(8, 6)).      
+0001ae80: 2020 3e3e 3e20 6669 672e 636c 6628 290a    >>> fig.clf().
+0001ae90: 2020 2020 2020 2020 3e3e 3e20 6178 203d          >>> ax =
+0001aea0: 2066 6967 2e61 6464 5f73 7562 706c 6f74   fig.add_subplot
+0001aeb0: 2831 2c20 312c 2031 2c20 7072 6f6a 6563  (1, 1, 1, projec
+0001aec0: 7469 6f6e 3d27 3364 2729 0a20 2020 2020  tion='3d').     
+0001aed0: 2020 203e 3e3e 206e 6173 7472 616e 2e77     >>> nastran.w
+0001aee0: 7472 7370 6c69 6e65 5f72 696e 6773 280a  trspline_rings(.
+0001aef0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+0001af00: 312c 2072 696e 6731 2c20 7269 6e67 322c  1, ring1, ring2,
+0001af10: 2031 3030 312c 2032 3030 312c 0a20 2020   1001, 2001,.   
+0001af20: 2020 2020 202e 2e2e 2020 2020 206d 616b       ...     mak
+0001af30: 6570 6c6f 743d 6178 2920 2020 2320 646f  eplot=ax)   # do
+0001af40: 6374 6573 743a 202b 534b 4950 0a20 2020  ctest: +SKIP.   
+0001af50: 2020 2020 2024 0a20 2020 2020 2020 2024       $.        $
+0001af60: 2046 6974 206f 6620 5370 6163 6563 7261   Fit of Spacecra
+0001af70: 6674 2067 7269 6473 3a0a 2020 2020 2020  ft grids:.      
+0001af80: 2020 2420 2020 2020 4365 6e74 6572 3a20    $     Center: 
+0001af90: 5b30 2e30 3030 2c20 302e 3030 302c 2030  [0.000, 0.000, 0
+0001afa0: 2e30 3030 5d20 2869 6e20 6261 7369 6329  .000] (in basic)
+0001afb0: 0a20 2020 2020 2020 2024 2020 2020 2052  .        $     R
+0001afc0: 6164 6975 733a 2035 302e 300a 2020 2020  adius: 50.0.    
+0001afd0: 2020 2020 240a 2020 2020 2020 2020 2420      $.        $ 
+0001afe0: 4669 7420 6f66 2052 696e 6720 3220 6772  Fit of Ring 2 gr
+0001aff0: 6964 733a 0a20 2020 2020 2020 2024 2020  ids:.        $  
+0001b000: 2020 2043 656e 7465 723a 205b 312e 3030     Center: [1.00
+0001b010: 302c 202d 312e 3737 3665 2d31 352c 202d  0, -1.776e-15, -
+0001b020: 332e 3535 3365 2d31 355d 2028 696e 2062  3.553e-15] (in b
+0001b030: 6173 6963 290a 2020 2020 2020 2020 2420  asic).        $ 
+0001b040: 2020 2020 5261 6469 7573 3a20 3435 2e30      Radius: 45.0
+0001b050: 0a20 2020 2020 2020 2024 0a20 2020 2020  .        $.     
+0001b060: 2020 2024 204f 7269 6769 6e20 6f66 206c     $ Origin of l
+0001b070: 6f63 616c 2043 4f52 4432 5220 3130 3031  ocal CORD2R 1001
+0001b080: 3020 6973 2061 7420 6365 6e74 6572 206f  0 is at center o
+0001b090: 6620 5370 6163 6563 7261 6674 3b20 7a20  f Spacecraft; z 
+0001b0a0: 6973 0a20 2020 2020 2020 2024 2070 6572  is.        $ per
+0001b0b0: 7065 6e64 6963 756c 6172 2074 6f20 706c  pendicular to pl
+0001b0c0: 616e 6520 6f66 2063 6972 636c 652c 2061  ane of circle, a
+0001b0d0: 6e64 2078 2069 7320 616c 6967 6e65 6420  nd x is aligned 
+0001b0e0: 7769 7468 206e 6f64 6520 3120 2861 6e64  with node 1 (and
+0001b0f0: 0a20 2020 2020 2020 2024 206e 6577 206e  .        $ new n
+0001b100: 6f64 6520 3130 3031 292e 0a20 2020 2020  ode 1001)..     
+0001b110: 2020 2024 0a20 2020 2020 2020 2024 2043     $.        $ C
+0001b120: 6f6f 7264 696e 6174 6520 3130 3031 303a  oordinate 10010:
+0001b130: 0a20 2020 2020 2020 2043 4f52 4432 522a  .        CORD2R*
+0001b140: 2020 2020 2020 2020 2020 2020 3130 3031              1001
+0001b150: 3020 2020 2020 2020 2020 2020 2020 2020  0               
+0001b160: 3020 2030 2e30 3030 3030 3030 3065 2b30  0  0.00000000e+0
+0001b170: 3020 2030 2e30 3030 3030 3030 3065 2b30  0  0.00000000e+0
+0001b180: 302a 0a20 2020 2020 2020 202a 2020 2020  0*.        *    
+0001b190: 2020 2020 2030 2e30 3030 3030 3030 3065       0.00000000e
+0001b1a0: 2b30 3020 2031 2e30 3030 3030 3030 3065  +00  1.00000000e
+0001b1b0: 2b30 3020 2030 2e30 3030 3030 3030 3065  +00  0.00000000e
+0001b1c0: 2b30 3020 2030 2e30 3030 3030 3030 3065  +00  0.00000000e
+0001b1d0: 2b30 302a 0a20 2020 2020 2020 202a 2020  +00*.        *  
+0001b1e0: 2020 2020 2020 2030 2e30 3030 3030 3030         0.0000000
+0001b1f0: 3065 2b30 3020 2031 2e30 3030 3030 3030  0e+00  1.0000000
+0001b200: 3065 2b30 3020 2030 2e30 3030 3030 3030  0e+00  0.0000000
+0001b210: 3065 2b30 300a 2020 2020 2020 2020 240a  0e+00.        $.
+0001b220: 2020 2020 2020 2020 2420 4772 6964 7320          $ Grids 
+0001b230: 746f 2052 4245 3220 746f 2074 6865 2053  to RBE2 to the S
+0001b240: 7061 6365 6372 6166 7420 6772 6964 732e  pacecraft grids.
+0001b250: 2054 6865 7365 2067 7269 6473 206c 696e   These grids lin
+0001b260: 6520 7570 2077 6974 6820 7468 650a 2020  e up with the.  
+0001b270: 2020 2020 2020 2420 5269 6e67 2032 2063        $ Ring 2 c
+0001b280: 6972 636c 6520 736f 2074 6861 7420 7468  ircle so that th
+0001b290: 6520 5253 504c 494e 4520 2877 6869 6368  e RSPLINE (which
+0001b2a0: 2074 6965 7320 746f 6765 7468 6572 2074   ties together t
+0001b2b0: 6865 7365 206e 6577 2067 7269 6473 0a20  hese new grids. 
+0001b2c0: 2020 2020 2020 2024 2061 6e64 2074 6865         $ and the
+0001b2d0: 2052 696e 6720 3220 6772 6964 7329 2077   Ring 2 grids) w
+0001b2e0: 696c 6c20 6265 2073 6d6f 6f74 682e 0a20  ill be smooth.. 
+0001b2f0: 2020 2020 2020 2024 0a20 2020 2020 2020         $.       
+0001b300: 2047 5249 442a 2020 2020 2020 2020 2020   GRID*          
+0001b310: 2020 2020 2031 3030 3120 2020 2020 2020       1001       
+0001b320: 2020 2020 3130 3031 3020 2020 2020 3435      10010     45
+0001b330: 2e30 3030 3030 3030 3020 2020 2020 2d30  .00000000     -0
+0001b340: 2e30 3030 3030 3030 300a 2020 2020 2020  .00000000.      
+0001b350: 2020 2a20 2020 2020 2020 2020 2020 2020    *             
+0001b360: 312e 3030 3030 3030 3030 2020 2020 2020  1.00000000      
+0001b370: 2020 2020 2020 2020 2030 0a20 2020 2020           0.     
+0001b380: 2020 2047 5249 442a 2020 2020 2020 2020     GRID*        
+0001b390: 2020 2020 2020 2031 3030 3220 2020 2020         1002     
+0001b3a0: 2020 2020 2020 3130 3031 3020 2020 2020        10010     
+0001b3b0: 3133 2e39 3035 3736 3437 3520 2020 2020  13.90576475     
+0001b3c0: 3432 2e37 3937 3534 3332 330a 2020 2020  42.79754323.    
+0001b3d0: 2020 2020 2a20 2020 2020 2020 2020 2020      *           
+0001b3e0: 2020 312e 3030 3030 3030 3030 2020 2020    1.00000000    
+0001b3f0: 2020 2020 2020 2020 2020 2030 0a20 2020             0.   
+0001b400: 2020 2020 2047 5249 442a 2020 2020 2020       GRID*      
+0001b410: 2020 2020 2020 2020 2031 3030 3320 2020           1003   
+0001b420: 2020 2020 2020 2020 3130 3031 3020 2020          10010   
+0001b430: 202d 3336 2e34 3035 3736 3437 3520 2020   -36.40576475   
+0001b440: 2020 3236 2e34 3530 3333 3633 350a 2020    26.45033635.  
+0001b450: 2020 2020 2020 2a20 2020 2020 2020 2020        *         
+0001b460: 2020 2020 312e 3030 3030 3030 3030 2020      1.00000000  
+0001b470: 2020 2020 2020 2020 2020 2020 2030 0a20               0. 
+0001b480: 2020 2020 2020 2047 5249 442a 2020 2020         GRID*    
+0001b490: 2020 2020 2020 2020 2020 2031 3030 3420             1004 
+0001b4a0: 2020 2020 2020 2020 2020 3130 3031 3020            10010 
+0001b4b0: 2020 202d 3336 2e34 3035 3736 3437 3520     -36.40576475 
+0001b4c0: 2020 202d 3236 2e34 3530 3333 3633 350a     -26.45033635.
+0001b4d0: 2020 2020 2020 2020 2a20 2020 2020 2020          *       
+0001b4e0: 2020 2020 2020 312e 3030 3030 3030 3030        1.00000000
+0001b4f0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0001b500: 0a20 2020 2020 2020 2047 5249 442a 2020  .        GRID*  
+0001b510: 2020 2020 2020 2020 2020 2020 2031 3030               100
+0001b520: 3520 2020 2020 2020 2020 2020 3130 3031  5           1001
+0001b530: 3020 2020 2020 3133 2e39 3035 3736 3437  0     13.9057647
+0001b540: 3520 2020 202d 3432 2e37 3937 3534 3332  5    -42.7975432
+0001b550: 330a 2020 2020 2020 2020 2a20 2020 2020  3.        *     
+0001b560: 2020 2020 2020 2020 312e 3030 3030 3030          1.000000
+0001b570: 3030 2020 2020 2020 2020 2020 2020 2020  00              
+0001b580: 2030 0a20 2020 2020 2020 2024 0a20 2020   0.        $.   
+0001b590: 2020 2020 2024 2052 4245 3220 7468 6520       $ RBE2 the 
+0001b5a0: 5370 6163 6563 7261 6674 206e 6f64 6573  Spacecraft nodes
+0001b5b0: 2074 6f20 6e65 7720 6e6f 6465 7320 6372   to new nodes cr
+0001b5c0: 6561 7465 6420 6162 6f76 6520 2874 6865  eated above (the
+0001b5d0: 206e 6577 206e 6f64 6573 0a20 2020 2020   new nodes.     
+0001b5e0: 2020 2024 2061 7265 2069 6e64 6570 656e     $ are indepen
+0001b5f0: 6465 6e74 293a 0a20 2020 2020 2020 2024  dent):.        $
+0001b600: 0a20 2020 2020 2020 2052 4245 322c 3130  .        RBE2,10
+0001b610: 3031 2c31 3030 312c 3132 3334 3536 2c31  01,1001,123456,1
+0001b620: 0a20 2020 2020 2020 2052 4245 322c 3130  .        RBE2,10
+0001b630: 3032 2c31 3030 322c 3132 3334 3536 2c32  02,1002,123456,2
+0001b640: 0a20 2020 2020 2020 2052 4245 322c 3130  .        RBE2,10
+0001b650: 3033 2c31 3030 332c 3132 3334 3536 2c33  03,1003,123456,3
+0001b660: 0a20 2020 2020 2020 2052 4245 322c 3130  .        RBE2,10
+0001b670: 3034 2c31 3030 342c 3132 3334 3536 2c34  04,1004,123456,4
+0001b680: 0a20 2020 2020 2020 2052 4245 322c 3130  .        RBE2,10
+0001b690: 3035 2c31 3030 352c 3132 3334 3536 2c35  05,1005,123456,5
+0001b6a0: 0a20 2020 2020 2020 2024 0a20 2020 2020  .        $.     
+0001b6b0: 2020 2024 2052 5350 4c49 4e45 2074 6865     $ RSPLINE the
+0001b6c0: 2052 696e 6720 3220 6e6f 6465 7320 746f   Ring 2 nodes to
+0001b6d0: 2074 6865 206e 6577 206e 6f64 6573 2063   the new nodes c
+0001b6e0: 7265 6174 6564 2061 626f 7665 2c20 7769  reated above, wi
+0001b6f0: 7468 2074 6865 206e 6577 0a20 2020 2020  th the new.     
+0001b700: 2020 2024 206e 6f64 6573 2062 6569 6e67     $ nodes being
+0001b710: 2069 6e64 6570 656e 6465 6e74 2e0a 2020   independent..  
+0001b720: 2020 2020 2020 240a 2020 2020 2020 2020        $.        
+0001b730: 5253 504c 494e 4520 2020 2020 3230 3031  RSPLINE     2001
+0001b740: 2020 2020 2030 2e31 2020 2020 3130 3031       0.1    1001
+0001b750: 2020 2020 2031 3031 2020 3132 3334 3536       101  123456
+0001b760: 2020 2020 2031 3032 2020 3132 3334 3536       102  123456
+0001b770: 2020 2020 3130 3032 0a20 2020 2020 2020      1002.       
+0001b780: 2052 5350 4c49 4e45 2020 2020 2032 3030   RSPLINE     200
+0001b790: 3220 2020 2020 302e 3120 2020 2031 3030  2     0.1    100
+0001b7a0: 3220 2020 2020 3130 3320 2031 3233 3435  2     103  12345
+0001b7b0: 3620 2020 2031 3030 330a 2020 2020 2020  6    1003.      
+0001b7c0: 2020 5253 504c 494e 4520 2020 2020 3230    RSPLINE     20
+0001b7d0: 3033 2020 2020 2030 2e31 2020 2020 3130  03     0.1    10
+0001b7e0: 3033 2020 2020 2031 3034 2020 3132 3334  03     104  1234
+0001b7f0: 3536 2020 2020 2031 3035 2020 3132 3334  56     105  1234
+0001b800: 3536 2020 2020 3130 3034 0a20 2020 2020  56    1004.     
+0001b810: 2020 2052 5350 4c49 4e45 2020 2020 2032     RSPLINE     2
+0001b820: 3030 3420 2020 2020 302e 3120 2020 2031  004     0.1    1
+0001b830: 3030 3420 2020 2020 3130 3620 2031 3233  004     106  123
+0001b840: 3435 3620 2020 2031 3030 350a 2020 2020  456    1005.    
+0001b850: 2020 2020 5253 504c 494e 4520 2020 2020      RSPLINE     
+0001b860: 3230 3035 2020 2020 2030 2e31 2020 2020  2005     0.1    
+0001b870: 3130 3035 2020 2020 2031 3037 2020 3132  1005     107  12
+0001b880: 3334 3536 2020 2020 3130 3031 0a20 2020  3456    1001.   
+0001b890: 2022 2222 0a0a 2020 2020 6465 6620 5f63   """..    def _c
+0001b8a0: 6865 636b 5f67 7269 6473 2867 7269 6473  heck_grids(grids
+0001b8b0: 2c20 6e61 6d65 293a 0a20 2020 2020 2020  , name):.       
+0001b8c0: 2069 6620 6973 696e 7374 616e 6365 2867   if isinstance(g
+0001b8d0: 7269 6473 2c20 7475 706c 6529 2061 6e64  rids, tuple) and
+0001b8e0: 206c 656e 2867 7269 6473 2920 3d3d 2032   len(grids) == 2
+0001b8f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0001b900: 7475 726e 2067 7269 6473 0a20 2020 2020  turn grids.     
+0001b910: 2020 2072 6574 7572 6e20 6e61 6d65 2c20     return name, 
+0001b920: 6772 6964 730a 0a20 2020 2064 6566 205f  grids..    def _
+0001b930: 6465 7370 6163 6528 7329 3a0a 2020 2020  despace(s):.    
+0001b940: 2020 2020 7265 7475 726e 2028 2222 2e6a      return ("".j
+0001b950: 6f69 6e28 732e 7370 6c69 7428 2929 292e  oin(s.split())).
+0001b960: 6c6f 7765 7228 290a 0a20 2020 2072 316e  lower()..    r1n
+0001b970: 616d 652c 2072 3167 7269 6473 203d 205f  ame, r1grids = _
+0001b980: 6368 6563 6b5f 6772 6964 7328 7231 6772  check_grids(r1gr
+0001b990: 6964 732c 2022 5269 6e67 2031 2229 0a20  ids, "Ring 1"). 
+0001b9a0: 2020 2072 326e 616d 652c 2072 3267 7269     r2name, r2gri
+0001b9b0: 6473 203d 205f 6368 6563 6b5f 6772 6964  ds = _check_grid
+0001b9c0: 7328 7232 6772 6964 732c 2022 5269 6e67  s(r2grids, "Ring
+0001b9d0: 2032 2229 0a0a 2020 2020 2320 656e 7375   2")..    # ensu
+0001b9e0: 7265 2074 6861 7420 696e 6465 7065 6e64  re that independ
+0001b9f0: 656e 7420 6973 2065 6974 6865 7220 2772  ent is either 'r
+0001ba00: 696e 6731 2720 6f72 2027 7269 6e67 3227  ing1' or 'ring2'
+0001ba10: 3a0a 2020 2020 696e 6465 7065 6e64 656e  :.    independen
+0001ba20: 7420 3d20 5f64 6573 7061 6365 2869 6e64  t = _despace(ind
+0001ba30: 6570 656e 6465 6e74 290a 2020 2020 6966  ependent).    if
+0001ba40: 2069 6e64 6570 656e 6465 6e74 203d 3d20   independent == 
+0001ba50: 5f64 6573 7061 6365 2872 316e 616d 6529  _despace(r1name)
+0001ba60: 3a0a 2020 2020 2020 2020 696e 6465 7065  :.        indepe
+0001ba70: 6e64 656e 7420 3d20 2272 696e 6731 220a  ndent = "ring1".
+0001ba80: 2020 2020 656c 6966 2069 6e64 6570 656e      elif indepen
+0001ba90: 6465 6e74 203d 3d20 5f64 6573 7061 6365  dent == _despace
+0001baa0: 2872 326e 616d 6529 3a0a 2020 2020 2020  (r2name):.      
+0001bab0: 2020 696e 6465 7065 6e64 656e 7420 3d20    independent = 
+0001bac0: 2272 696e 6732 220a 2020 2020 6966 2069  "ring2".    if i
+0001bad0: 6e64 6570 656e 6465 6e74 206e 6f74 2069  ndependent not i
+0001bae0: 6e20 2822 7269 6e67 3122 2c20 2272 696e  n ("ring1", "rin
+0001baf0: 6732 2229 3a0a 2020 2020 2020 2020 7261  g2"):.        ra
+0001bb00: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+0001bb10: 696e 7661 6c69 6420 6069 6e64 6570 656e  invalid `indepen
+0001bb20: 6465 6e74 6020 6f70 7469 6f6e 2229 0a0a  dent` option")..
+0001bb30: 2020 2020 6966 2072 6265 325f 6964 3020      if rbe2_id0 
+0001bb40: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0001bb50: 2072 6265 325f 6964 3020 3d20 6e6f 6465   rbe2_id0 = node
+0001bb60: 5f69 6430 0a20 2020 2069 6620 636f 7264  _id0.    if cord
+0001bb70: 5f69 6420 6973 204e 6f6e 653a 0a20 2020  _id is None:.   
+0001bb80: 2020 2020 2063 6f72 645f 6964 203d 206e       cord_id = n
+0001bb90: 6f64 655f 6964 3020 2a20 3130 0a0a 2020  ode_id0 * 10..  
+0001bba0: 2020 6e61 6d65 7320 3d20 2872 316e 616d    names = (r1nam
+0001bbb0: 652c 2072 326e 616d 6529 0a20 2020 2049  e, r2name).    I
+0001bbc0: 4473 203d 205b 5d0a 2020 2020 7879 7a20  Ds = [].    xyz 
+0001bbd0: 3d20 5b5d 0a20 2020 2066 6f72 2072 696e  = [].    for rin
+0001bbe0: 672c 206e 616d 6520 696e 2028 2872 3167  g, name in ((r1g
+0001bbf0: 7269 6473 2c20 2272 3167 7269 6473 2229  rids, "r1grids")
+0001bc00: 2c20 2872 3267 7269 6473 2c20 2272 3267  , (r2grids, "r2g
+0001bc10: 7269 6473 2229 293a 0a20 2020 2020 2020  rids")):.       
+0001bc20: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+0001bc30: 696e 672c 2070 642e 4461 7461 4672 616d  ing, pd.DataFram
+0001bc40: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0001bc50: 7220 3d20 7269 6e67 2e73 6861 7065 5b30  r = ring.shape[0
+0001bc60: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+0001bc70: 2028 7220 2f2f 2036 2920 2a20 3620 213d   (r // 6) * 6 !=
+0001bc80: 2072 3a0a 2020 2020 2020 2020 2020 2020   r:.            
+0001bc90: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0001bca0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0001bcb0: 2020 2020 2020 2020 2020 6622 6e75 6d62            f"numb
+0001bcc0: 6572 206f 6620 726f 7773 2060 7b6e 616d  er of rows `{nam
+0001bcd0: 657d 6020 6973 206e 6f74 2022 2022 6d75  e}` is not " "mu
+0001bce0: 6c74 6970 6c65 206f 6620 3620 666f 7220  ltiple of 6 for 
+0001bcf0: 5553 4554 2069 6e70 7574 220a 2020 2020  USET input".    
+0001bd00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001bd10: 2020 2020 2020 2020 2020 4944 732e 6170            IDs.ap
+0001bd20: 7065 6e64 2872 696e 672e 696e 6465 782e  pend(ring.index.
+0001bd30: 6765 745f 6c65 7665 6c5f 7661 6c75 6573  get_level_values
+0001bd40: 2822 6964 2229 5b3a 3a36 5d29 0a20 2020  ("id")[::6]).   
+0001bd50: 2020 2020 2020 2020 2078 797a 2e61 7070           xyz.app
+0001bd60: 656e 6428 7269 6e67 2e69 6c6f 635b 3a3a  end(ring.iloc[::
+0001bd70: 362c 2031 3a5d 2e76 616c 7565 7329 0a20  6, 1:].values). 
+0001bd80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001bd90: 2020 2020 2020 2020 2072 696e 6720 3d20           ring = 
+0001bda0: 6e70 2e61 746c 6561 7374 5f32 6428 7269  np.atleast_2d(ri
+0001bdb0: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
+0001bdc0: 4944 732e 6170 7065 6e64 2872 696e 675b  IDs.append(ring[
+0001bdd0: 3a2c 2030 5d2e 6173 7479 7065 286e 702e  :, 0].astype(np.
+0001bde0: 696e 7436 3429 290a 2020 2020 2020 2020  int64)).        
+0001bdf0: 2020 2020 7879 7a2e 6170 7065 6e64 2872      xyz.append(r
+0001be00: 696e 675b 3a2c 2031 3a5d 290a 0a20 2020  ing[:, 1:])..   
+0001be10: 2023 2066 6974 2062 6f74 6820 6369 7263   # fit both circ
+0001be20: 6c65 733a 0a20 2020 2063 6972 635f 7061  les:.    circ_pa
+0001be30: 726d 7320 3d20 5b79 746f 6f6c 732e 6669  rms = [ytools.fi
+0001be40: 745f 6369 7263 6c65 5f33 6428 7879 7a5b  t_circle_3d(xyz[
+0001be50: 695d 2e54 2920 666f 7220 6920 696e 2028  i].T) for i in (
+0001be60: 302c 2031 295d 0a0a 2020 2020 2320 7a20  0, 1)]..    # z 
+0001be70: 6178 6573 2062 6574 7465 7220 6265 2061  axes better be a
+0001be80: 6c69 676e 6564 3a0a 2020 2020 5f63 6865  ligned:.    _che
+0001be90: 636b 5f7a 5f61 6c69 676e 6d65 6e74 2863  ck_z_alignment(c
+0001bea0: 6972 635f 7061 726d 732c 2030 2e39 3929  irc_parms, 0.99)
+0001beb0: 0a0a 2020 2020 2320 7573 6520 3173 7420  ..    # use 1st 
+0001bec0: 6261 7369 6332 6c6f 6361 6c20 7472 616e  basic2local tran
+0001bed0: 7366 6f72 6d20 6f6e 2073 6563 6f6e 6420  sform on second 
+0001bee0: 7365 7420 6f66 2064 6174 6120 746f 2067  set of data to g
+0001bef0: 6574 2061 6c6c 0a20 2020 2023 2063 6f6f  et all.    # coo
+0001bf00: 7264 696e 6174 6573 2069 6e20 7361 6d65  rdinates in same
+0001bf10: 206c 6f63 616c 2073 7973 7465 6d3a 0a20   local system:. 
+0001bf20: 2020 2062 6173 6963 326c 6f63 616c 203d     basic2local =
+0001bf30: 2063 6972 635f 7061 726d 735b 305d 2e62   circ_parms[0].b
+0001bf40: 6173 6963 326c 6f63 616c 0a20 2020 2063  asic2local.    c
+0001bf50: 656e 7465 7220 3d20 6369 7263 5f70 6172  enter = circ_par
+0001bf60: 6d73 5b30 5d2e 6365 6e74 6572 0a20 2020  ms[0].center.   
+0001bf70: 2063 6972 635f 7061 726d 735b 315d 2e6c   circ_parms[1].l
+0001bf80: 6f63 616c 203d 2062 6173 6963 326c 6f63  ocal = basic2loc
+0001bf90: 616c 2040 2028 7879 7a5b 315d 202d 2063  al @ (xyz[1] - c
+0001bfa0: 656e 7465 7229 2e54 0a0a 2020 2020 2320  enter).T..    # 
+0001bfb0: 7468 6520 6365 6e74 6572 2070 6f69 6e74  the center point
+0001bfc0: 2077 696c 6c20 6f66 7465 6e20 6861 7665   will often have
+0001bfd0: 206e 6561 722d 7a65 726f 7320 6275 7420   near-zeros but 
+0001bfe0: 6265 206e 756d 6572 6963 616c 6c79 0a20  be numerically. 
+0001bff0: 2020 2023 206f 6666 202e 2e2e 2063 6865     # off ... che
+0001c000: 636b 2066 6f72 2074 6869 7320 616e 6420  ck for this and 
+0001c010: 6164 6a75 7374 2069 6620 7468 6174 2773  adjust if that's
+0001c020: 2074 6865 2063 6173 653a 0a20 2020 2072   the case:.    r
+0001c030: 6164 6975 7320 3d20 6369 7263 5f70 6172  adius = circ_par
+0001c040: 6d73 5b30 5d2e 7261 6469 7573 0a20 2020  ms[0].radius.   
+0001c050: 2066 6f72 2069 2c20 7661 6c75 6520 696e   for i, value in
+0001c060: 2065 6e75 6d65 7261 7465 2863 656e 7465   enumerate(cente
+0001c070: 7229 3a0a 2020 2020 2020 2020 6966 2061  r):.        if a
+0001c080: 6273 2876 616c 7565 2920 3c20 3165 2d37  bs(value) < 1e-7
+0001c090: 202a 2072 6164 6975 733a 0a20 2020 2020   * radius:.     
+0001c0a0: 2020 2020 2020 2063 656e 7465 725b 695d         center[i]
+0001c0b0: 203d 2030 2e30 0a0a 2020 2020 4067 7569   = 0.0..    @gui
+0001c0c0: 746f 6f6c 732e 7772 6974 655f 7465 7874  tools.write_text
+0001c0d0: 5f66 696c 650a 2020 2020 6465 6620 5f77  _file.    def _w
+0001c0e0: 7269 7465 5f66 696c 6528 6629 3a0a 2020  rite_file(f):.  
+0001c0f0: 2020 2020 2020 2320 7772 6974 6520 6369        # write ci
+0001c100: 7263 6c65 2069 6e66 6f20 666f 7220 7265  rcle info for re
+0001c110: 6665 7265 6e63 653a 0a20 2020 2020 2020  ference:.       
+0001c120: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0001c130: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
+0001c140: 6374 7220 3d20 6369 7263 5f70 6172 6d73  ctr = circ_parms
+0001c150: 5b69 5d2e 6365 6e74 6572 0a20 2020 2020  [i].center.     
+0001c160: 2020 2020 2020 2063 7472 5f73 7472 696e         ctr_strin
+0001c170: 6720 3d20 6622 5b7b 6374 725b 305d 3a23  g = f"[{ctr[0]:#
+0001c180: 2e34 677d 2c20 7b63 7472 5b31 5d3a 232e  .4g}, {ctr[1]:#.
+0001c190: 3467 7d2c 207b 6374 725b 325d 3a23 2e34  4g}, {ctr[2]:#.4
+0001c1a0: 677d 5d22 0a20 2020 2020 2020 2020 2020  g}]".           
+0001c1b0: 2063 6f6d 6d65 6e74 203d 2028 0a20 2020   comment = (.   
+0001c1c0: 2020 2020 2020 2020 2020 2020 2022 245c               "$\
+0001c1d0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+0001c1e0: 2020 2066 2224 2046 6974 206f 6620 7b6e     f"$ Fit of {n
+0001c1f0: 616d 6573 5b69 5d7d 2067 7269 6473 3a5c  ames[i]} grids:\
+0001c200: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+0001c210: 2020 2066 2224 2020 2020 2043 656e 7465     f"$     Cente
+0001c220: 723a 207b 6374 725f 7374 7269 6e67 7d20  r: {ctr_string} 
+0001c230: 2869 6e20 6261 7369 6329 5c6e 220a 2020  (in basic)\n".  
+0001c240: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0001c250: 2420 2020 2020 5261 6469 7573 3a20 7b63  $     Radius: {c
+0001c260: 6972 635f 7061 726d 735b 695d 2e72 6164  irc_parms[i].rad
+0001c270: 6975 737d 5c6e 220a 2020 2020 2020 2020  ius}\n".        
+0001c280: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001c290: 2020 662e 7772 6974 6528 636f 6d6d 656e    f.write(commen
+0001c2a0: 7429 0a0a 2020 2020 2020 2020 2320 7772  t)..        # wr
+0001c2b0: 6974 6520 6c6f 6361 6c20 636f 6f72 6469  ite local coordi
+0001c2c0: 6e61 7465 2073 7973 7465 6d20 746f 2066  nate system to f
+0001c2d0: 696c 653a 0a20 2020 2020 2020 205f 7774  ile:.        _wt
+0001c2e0: 5f63 6972 636c 6531 5f63 6f6f 7264 2866  _circle1_coord(f
+0001c2f0: 2c20 636f 7264 5f69 642c 2063 656e 7465  , cord_id, cente
+0001c300: 722c 2062 6173 6963 326c 6f63 616c 2c20  r, basic2local, 
+0001c310: 4944 735b 305d 5b30 5d2c 206e 6f64 655f  IDs[0][0], node_
+0001c320: 6964 302c 206e 616d 6573 290a 0a20 2020  id0, names)..   
+0001c330: 2020 2020 2023 2063 7265 6174 6520 6e65       # create ne
+0001c340: 7720 6e6f 6465 7320 7468 6174 2077 696c  w nodes that wil
+0001c350: 6c20 6265 2052 4245 3227 6420 746f 2072  l be RBE2'd to r
+0001c360: 696e 6720 3120 6e6f 6465 732c 2062 7574  ing 1 nodes, but
+0001c370: 0a20 2020 2020 2020 2023 206c 6f63 6174  .        # locat
+0001c380: 6564 206f 6e20 7269 6e67 2032 2063 6972  ed on ring 2 cir
+0001c390: 636c 650a 2020 2020 2020 2020 2320 2d20  cle.        # - 
+0001c3a0: 7468 6573 6520 6e6f 6465 7320 7769 6c6c  these nodes will
+0001c3b0: 2062 6520 6465 6669 6e65 6420 696e 2074   be defined in t
+0001c3c0: 6865 206c 6f63 616c 2073 7973 7465 6d20  he local system 
+0001c3d0: 6275 7420 6f75 7470 7574 0a20 2020 2020  but output.     
+0001c3e0: 2020 2023 2020 2069 6e20 6261 7369 630a     #   in basic.
+0001c3f0: 2020 2020 2020 2020 6e65 7770 7473 2c20          newpts, 
+0001c400: 6e65 7769 6473 203d 205f 7774 6772 6964  newids = _wtgrid
+0001c410: 735f 7262 6532 7328 0a20 2020 2020 2020  s_rbe2s(.       
+0001c420: 2020 2020 2066 2c0a 2020 2020 2020 2020       f,.        
+0001c430: 2020 2020 6369 7263 5f70 6172 6d73 2c0a      circ_parms,.
+0001c440: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
+0001c450: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0001c460: 6261 7369 6332 6c6f 6361 6c2c 0a20 2020  basic2local,.   
+0001c470: 2020 2020 2020 2020 2063 6f72 645f 6964           cord_id
+0001c480: 2c0a 2020 2020 2020 2020 2020 2020 6e6f  ,.            no
+0001c490: 6465 5f69 6430 2c0a 2020 2020 2020 2020  de_id0,.        
+0001c4a0: 2020 2020 7262 6532 5f69 6430 2c0a 2020      rbe2_id0,.  
+0001c4b0: 2020 2020 2020 2020 2020 4944 735b 305d            IDs[0]
+0001c4c0: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
+0001c4d0: 6d65 732c 0a20 2020 2020 2020 2029 0a0a  mes,.        )..
+0001c4e0: 2020 2020 2020 2020 2320 7273 706c 696e          # rsplin
+0001c4f0: 6520 7769 6c6c 2074 6965 2074 6865 2027  e will tie the '
+0001c500: 6e65 7770 7473 2720 616e 6420 7468 6520  newpts' and the 
+0001c510: 7269 6e67 2032 206e 6f64 6573 2074 6f67  ring 2 nodes tog
+0001c520: 6574 6865 723a 0a20 2020 2020 2020 2072  ether:.        r
+0001c530: 7370 6c69 6e65 5f6e 6f64 6573 203d 205f  spline_nodes = _
+0001c540: 736f 7274 5f6e 5f77 7269 7465 280a 2020  sort_n_write(.  
+0001c550: 2020 2020 2020 2020 2020 662c 2069 6e64            f, ind
+0001c560: 6570 656e 6465 6e74 2c20 6369 7263 5f70  ependent, circ_p
+0001c570: 6172 6d73 2c20 6e65 7770 7473 2c20 6e65  arms, newpts, ne
+0001c580: 7769 6473 2c20 4944 735b 315d 2c20 7273  wids, IDs[1], rs
+0001c590: 706c 696e 655f 6964 302c 2044 6f4c 2c20  pline_id0, DoL, 
+0001c5a0: 6e61 6d65 730a 2020 2020 2020 2020 290a  names.        ).
+0001c5b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001c5c0: 6e65 7770 7473 2c20 6e65 7769 6473 2c20  newpts, newids, 
+0001c5d0: 7273 706c 696e 655f 6e6f 6465 730a 0a20  rspline_nodes.. 
+0001c5e0: 2020 2023 2077 7269 7465 2074 6865 2072     # write the r
+0001c5f0: 7370 6c69 6e65 3a0a 2020 2020 6e65 7770  spline:.    newp
+0001c600: 7473 2c20 6e65 7769 6473 2c20 7273 706c  ts, newids, rspl
+0001c610: 696e 655f 6e6f 6465 7320 3d20 5f77 7269  ine_nodes = _wri
+0001c620: 7465 5f66 696c 6528 6629 0a0a 2020 2020  te_file(f)..    
+0001c630: 6178 203d 2079 746f 6f6c 732e 5f63 6865  ax = ytools._che
+0001c640: 636b 5f6d 616b 6570 6c6f 7428 6d61 6b65  ck_makeplot(make
+0001c650: 706c 6f74 2c20 6669 6773 697a 653d 5b38  plot, figsize=[8
+0001c660: 2c20 365d 2c20 6e65 6564 3364 3d54 7275  , 6], need3d=Tru
+0001c670: 6529 0a20 2020 2069 6620 6178 3a0a 2020  e).    if ax:.  
+0001c680: 2020 2020 2020 5f70 6c6f 745f 7273 706c        _plot_rspl
+0001c690: 696e 6528 0a20 2020 2020 2020 2020 2020  ine(.           
+0001c6a0: 2061 782c 0a20 2020 2020 2020 2020 2020   ax,.           
+0001c6b0: 2063 6972 635f 7061 726d 732c 0a20 2020   circ_parms,.   
+0001c6c0: 2020 2020 2020 2020 2078 797a 2c0a 2020           xyz,.  
+0001c6d0: 2020 2020 2020 2020 2020 6e65 7770 7473            newpts
+0001c6e0: 2c0a 2020 2020 2020 2020 2020 2020 6e65  ,.            ne
+0001c6f0: 7769 6473 2c0a 2020 2020 2020 2020 2020  wids,.          
+0001c700: 2020 6261 7369 6332 6c6f 6361 6c2c 0a20    basic2local,. 
+0001c710: 2020 2020 2020 2020 2020 2063 656e 7465             cente
+0001c720: 722c 0a20 2020 2020 2020 2020 2020 2072  r,.            r
+0001c730: 7370 6c69 6e65 5f6e 6f64 6573 2c0a 2020  spline_nodes,.  
+0001c740: 2020 2020 2020 2020 2020 4944 735b 315d            IDs[1]
+0001c750: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
+0001c760: 6d65 732c 0a20 2020 2020 2020 2029 0a0a  mes,.        )..
+0001c770: 0a64 6566 2077 7463 6f6f 7264 6361 7264  .def wtcoordcard
+0001c780: 7328 662c 2063 6929 3a0a 2020 2020 2222  s(f, ci):.    ""
+0001c790: 220a 2020 2020 5772 6974 6520 4e61 7374  ".    Write Nast
+0001c7a0: 7261 6e20 434f 5244 322a 2063 6172 6473  ran CORD2* cards
+0001c7b0: 2074 6f20 6120 6669 6c65 0a0a 2020 2020   to a file..    
+0001c7c0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0001c7d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6620  ---------.    f 
+0001c7e0: 3a20 7374 7269 6e67 206f 7220 6669 6c65  : string or file
+0001c7f0: 5f6c 696b 6520 6f72 2031 206f 7220 4e6f  _like or 1 or No
+0001c800: 6e65 0a20 2020 2020 2020 2045 6974 6865  ne.        Eithe
+0001c810: 7220 6120 6e61 6d65 206f 6620 6120 6669  r a name of a fi
+0001c820: 6c65 2c20 6f72 2069 7320 6120 6669 6c65  le, or is a file
+0001c830: 5f6c 696b 6520 6f62 6a65 6374 2061 7320  _like object as 
+0001c840: 7265 7475 726e 6564 0a20 2020 2020 2020  returned.       
+0001c850: 2062 7920 3a66 756e 633a 606f 7065 6e60   by :func:`open`
+0001c860: 206f 7220 3a63 6c61 7373 3a60 696f 2e53   or :class:`io.S
+0001c870: 7472 696e 6749 4f60 2e20 496e 7075 7420  tringIO`. Input 
+0001c880: 6173 2069 6e74 6567 6572 2031 2074 6f0a  as integer 1 to.
+0001c890: 2020 2020 2020 2020 7772 6974 6520 746f          write to
+0001c8a0: 2073 7464 6f75 742e 2043 616e 2061 6c73   stdout. Can als
+0001c8b0: 6f20 6265 2074 6865 206e 616d 6520 6f66  o be the name of
+0001c8c0: 2061 2064 6972 6563 746f 7279 206f 7220   a directory or 
+0001c8d0: 4e6f 6e65 3b0a 2020 2020 2020 2020 696e  None;.        in
+0001c8e0: 2074 6865 7365 2063 6173 6573 2c20 6120   these cases, a 
+0001c8f0: 4755 4920 6973 206f 7065 6e65 6420 666f  GUI is opened fo
+0001c900: 7220 6669 6c65 2073 656c 6563 7469 6f6e  r file selection
+0001c910: 2e0a 2020 2020 6369 203a 2064 6963 7469  ..    ci : dicti
+0001c920: 6f6e 6172 7920 6f72 204e 6f6e 650a 2020  onary or None.  
+0001c930: 2020 2020 2020 4469 6374 696f 6e61 7279        Dictionary
+0001c940: 206f 6620 636f 6f72 6469 6e61 7465 2063   of coordinate c
+0001c950: 6172 6420 696e 666f 2061 7320 7265 7475  ard info as retu
+0001c960: 726e 6564 2062 790a 2020 2020 2020 2020  rned by.        
+0001c970: 3a66 756e 633a 6070 7979 6574 692e 6e61  :func:`pyyeti.na
+0001c980: 7374 7261 6e2e 6e32 702e 6d6b 636f 7264  stran.n2p.mkcord
+0001c990: 6361 7264 696e 666f 602e 2049 6620 4e6f  cardinfo`. If No
+0001c9a0: 6e65 206f 7220 6966 2064 6963 740a 2020  ne or if dict.  
+0001c9b0: 2020 2020 2020 6973 2065 6d70 7479 2c20        is empty, 
+0001c9c0: 7468 6973 2072 6f75 7469 6e65 2071 7569  this routine qui
+0001c9d0: 6574 6c79 2064 6f65 7320 6e6f 7468 696e  etly does nothin
+0001c9e0: 672e 0a0a 2020 2020 5265 7475 726e 730a  g...    Returns.
+0001c9f0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001ca00: 4e6f 6e65 0a0a 2020 2020 4e6f 7465 730a  None..    Notes.
+0001ca10: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5479      -----.    Ty
+0001ca20: 7069 6361 6c6c 7920 6361 6c6c 6564 2062  pically called b
+0001ca30: 7920 3a66 756e 633a 6077 7465 7874 7365  y :func:`wtextse
+0001ca40: 6f75 7460 2e0a 0a20 2020 2045 7861 6d70  out`...    Examp
+0001ca50: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
+0001ca60: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
+0001ca70: 6e75 6d70 7920 6173 206e 700a 2020 2020  numpy as np.    
+0001ca80: 3e3e 3e20 6672 6f6d 2070 7979 6574 6920  >>> from pyyeti 
+0001ca90: 696d 706f 7274 206e 6173 7472 616e 0a20  import nastran. 
+0001caa0: 2020 203e 3e3e 2063 6920 3d20 7b31 303a     >>> ci = {10:
+0001cab0: 205b 2743 4f52 4432 5227 2c20 6e70 2e61   ['CORD2R', np.a
+0001cac0: 7272 6179 285b 5b31 302c 2031 2c20 305d  rray([[10, 1, 0]
+0001cad0: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
+0001cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001caf0: 2020 2020 2020 2020 205b 3130 302e 2c20           [100., 
+0001cb00: 302e 2c20 302e 5d2c 0a20 2020 202e 2e2e  0., 0.],.    ...
+0001cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb30: 5b31 3030 2e2c 2030 2e2c 2031 3030 2e5d  [100., 0., 100.]
+0001cb40: 2c0a 2020 2020 2e2e 2e20 2020 2020 2020  ,.    ...       
+0001cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb60: 2020 2020 2020 2020 205b 3230 302e 2c20           [200., 
+0001cb70: 302e 2c20 302e 5d5d 295d 7d0a 2020 2020  0., 0.]])]}.    
+0001cb80: 3e3e 3e20 6e61 7374 7261 6e2e 7774 636f  >>> nastran.wtco
+0001cb90: 6f72 6463 6172 6473 2831 2c20 6369 290a  ordcards(1, ci).
+0001cba0: 2020 2020 2420 436f 6f72 6469 6e61 7465      $ Coordinate
+0001cbb0: 2031 303a 0a20 2020 2043 4f52 4432 522a   10:.    CORD2R*
+0001cbc0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
+0001cbd0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
+0001cbe0: 3020 2031 2e30 3030 3030 3030 3065 2b30  0  1.00000000e+0
+0001cbf0: 3220 2030 2e30 3030 3030 3030 3065 2b30  2  0.00000000e+0
+0001cc00: 302a 0a20 2020 202a 2020 2020 2020 2020  0*.    *        
+0001cc10: 2030 2e30 3030 3030 3030 3065 2b30 3020   0.00000000e+00 
+0001cc20: 2031 2e30 3030 3030 3030 3065 2b30 3220   1.00000000e+02 
+0001cc30: 2030 2e30 3030 3030 3030 3065 2b30 3020   0.00000000e+00 
+0001cc40: 2031 2e30 3030 3030 3030 3065 2b30 322a   1.00000000e+02*
+0001cc50: 0a20 2020 202a 2020 2020 2020 2020 2032  .    *         2
+0001cc60: 2e30 3030 3030 3030 3065 2b30 3220 2030  .00000000e+02  0
+0001cc70: 2e30 3030 3030 3030 3065 2b30 3020 2030  .00000000e+00  0
+0001cc80: 2e30 3030 3030 3030 3065 2b30 300a 2020  .00000000e+00.  
+0001cc90: 2020 2222 220a 2020 2020 6966 2063 6920    """.    if ci 
+0001cca0: 6973 204e 6f6e 6520 6f72 206c 656e 2863  is None or len(c
+0001ccb0: 6929 203d 3d20 303a 0a20 2020 2020 2020  i) == 0:.       
+0001ccc0: 2072 6574 7572 6e0a 0a20 2020 2040 6775   return..    @gu
+0001ccd0: 6974 6f6f 6c73 2e77 7269 7465 5f74 6578  itools.write_tex
+0001cce0: 745f 6669 6c65 0a20 2020 2064 6566 205f  t_file.    def _
+0001ccf0: 7774 636f 6f72 6473 2866 2c20 6369 293a  wtcoords(f, ci):
+0001cd00: 0a20 2020 2020 2020 2066 6f72 206b 2069  .        for k i
+0001cd10: 6e20 6369 3a0a 2020 2020 2020 2020 2020  n ci:.          
+0001cd20: 2020 6461 7461 203d 2063 695b 6b5d 2020    data = ci[k]  
+0001cd30: 2320 5b6e 616d 652c 205b 5b69 642c 2074  # [name, [[id, t
+0001cd40: 7970 652c 2072 6566 5d3b 2041 3b20 423b  ype, ref]; A; B;
+0001cd50: 2043 5d5d 0a20 2020 2020 2020 2020 2020   C]].           
+0001cd60: 2063 6f6f 7264 203d 2064 6174 615b 315d   coord = data[1]
+0001cd70: 0a20 2020 2020 2020 2020 2020 2061 6263  .            abc
+0001cd80: 203d 202b 636f 6f72 645b 313a 5d0a 2020   = +coord[1:].  
+0001cd90: 2020 2020 2020 2020 2020 6162 635b 6162            abc[ab
+0001cda0: 7328 6162 6329 203c 2061 6273 2861 6263  s(abc) < abs(abc
+0001cdb0: 292e 6d61 7828 2920 2a20 3165 2d31 355d  ).max() * 1e-15]
+0001cdc0: 203d 2030 2e30 0a20 2020 2020 2020 2020   = 0.0.         
+0001cdd0: 2020 2066 2e77 7269 7465 2866 2224 2043     f.write(f"$ C
+0001cde0: 6f6f 7264 696e 6174 6520 7b6b 7d3a 5c6e  oordinate {k}:\n
+0001cdf0: 2229 0a20 2020 2020 2020 2020 2020 2066  ").            f
+0001ce00: 2e77 7269 7465 280a 2020 2020 2020 2020  .write(.        
+0001ce10: 2020 2020 2020 2020 227b 3a3c 3873 7d7b          "{:<8s}{
+0001ce20: 3a31 3664 7d7b 3a31 3664 7d7b 3a31 362e  :16d}{:16d}{:16.
+0001ce30: 3865 7d7b 3a31 362e 3865 7d2a 5c6e 222e  8e}{:16.8e}*\n".
+0001ce40: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+0001ce50: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0001ce60: 5b30 5d20 2b20 222a 222c 206b 2c20 696e  [0] + "*", k, in
+0001ce70: 7428 636f 6f72 645b 302c 2032 5d29 2c20  t(coord[0, 2]), 
+0001ce80: 2a61 6263 5b30 2c20 3a32 5d0a 2020 2020  *abc[0, :2].    
+0001ce90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001cea0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001ceb0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+0001cec0: 2822 7b3a 3c38 737d 2220 2b20 227b 3a31  ("{:<8s}" + "{:1
+0001ced0: 362e 3865 7d22 202a 2034 202b 2022 2a5c  6.8e}" * 4 + "*\
+0001cee0: 6e22 292e 666f 726d 6174 2822 2a22 2c20  n").format("*", 
+0001cef0: 6162 635b 302c 2032 5d2c 202a 6162 635b  abc[0, 2], *abc[
+0001cf00: 315d 2929 0a20 2020 2020 2020 2020 2020  1])).           
+0001cf10: 2066 2e77 7269 7465 2828 227b 3a3c 3873   f.write(("{:<8s
+0001cf20: 7d22 202b 2022 7b3a 3136 2e38 657d 2220  }" + "{:16.8e}" 
+0001cf30: 2a20 3320 2b20 225c 6e22 292e 666f 726d  * 3 + "\n").form
+0001cf40: 6174 2822 2a22 2c20 2a61 6263 5b32 5d29  at("*", *abc[2])
+0001cf50: 290a 0a20 2020 205f 7774 636f 6f72 6473  )..    _wtcoords
+0001cf60: 2866 2c20 6369 290a 0a0a 4067 7569 746f  (f, ci)...@guito
+0001cf70: 6f6c 732e 7772 6974 655f 7465 7874 5f66  ols.write_text_f
+0001cf80: 696c 650a 6465 6620 7774 6578 7472 6e28  ile.def wtextrn(
+0001cf90: 662c 2069 6473 2c20 646f 6629 3a0a 2020  f, ids, dof):.  
+0001cfa0: 2020 2222 220a 2020 2020 5772 6974 6573    """.    Writes
+0001cfb0: 2061 204e 6173 7472 616e 2045 5854 524e   a Nastran EXTRN
+0001cfc0: 2063 6172 6420 746f 2061 2066 696c 652e   card to a file.
+0001cfd0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0001cfe0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001cff0: 2020 2020 6620 3a20 7374 7269 6e67 206f      f : string o
+0001d000: 7220 6669 6c65 5f6c 696b 6520 6f72 2031  r file_like or 1
+0001d010: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+0001d020: 2045 6974 6865 7220 6120 6e61 6d65 206f   Either a name o
+0001d030: 6620 6120 6669 6c65 2c20 6f72 2069 7320  f a file, or is 
+0001d040: 6120 6669 6c65 5f6c 696b 6520 6f62 6a65  a file_like obje
+0001d050: 6374 2061 7320 7265 7475 726e 6564 0a20  ct as returned. 
+0001d060: 2020 2020 2020 2062 7920 3a66 756e 633a         by :func:
+0001d070: 606f 7065 6e60 206f 7220 3a63 6c61 7373  `open` or :class
+0001d080: 3a60 696f 2e53 7472 696e 6749 4f60 2e20  :`io.StringIO`. 
+0001d090: 496e 7075 7420 6173 2069 6e74 6567 6572  Input as integer
+0001d0a0: 2031 2074 6f0a 2020 2020 2020 2020 7772   1 to.        wr
+0001d0b0: 6974 6520 746f 2073 7464 6f75 742e 2043  ite to stdout. C
+0001d0c0: 616e 2061 6c73 6f20 6265 2074 6865 206e  an also be the n
+0001d0d0: 616d 6520 6f66 2061 2064 6972 6563 746f  ame of a directo
+0001d0e0: 7279 206f 7220 4e6f 6e65 3b0a 2020 2020  ry or None;.    
+0001d0f0: 2020 2020 696e 2074 6865 7365 2063 6173      in these cas
+0001d100: 6573 2c20 6120 4755 4920 6973 206f 7065  es, a GUI is ope
+0001d110: 6e65 6420 666f 7220 6669 6c65 2073 656c  ned for file sel
+0001d120: 6563 7469 6f6e 2e0a 2020 2020 6964 7320  ection..    ids 
+0001d130: 3a20 3164 2061 7272 6179 5f6c 696b 650a  : 1d array_like.
+0001d140: 2020 2020 2020 2020 5665 6374 6f72 206f          Vector o
+0001d150: 6620 6e6f 6465 2069 6473 0a20 2020 2064  f node ids.    d
+0001d160: 6f66 203a 2031 6420 6172 7261 795f 6c69  of : 1d array_li
+0001d170: 6b65 0a20 2020 2020 2020 2056 6563 746f  ke.        Vecto
+0001d180: 7220 6f66 2044 4f46 0a0a 2020 2020 5265  r of DOF..    Re
+0001d190: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0001d1a0: 2d0a 2020 2020 4e6f 6e65 0a0a 2020 2020  -.    None..    
+0001d1b0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+0001d1c0: 2020 2020 5479 7069 6361 6c6c 7920 6361      Typically ca
+0001d1d0: 6c6c 6564 2062 7920 3a66 756e 633a 6077  lled by :func:`w
+0001d1e0: 7465 7874 7365 6f75 7460 2e0a 0a20 2020  textseout`...   
+0001d1f0: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
+0001d200: 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e 2066  ------.    >>> f
+0001d210: 726f 6d20 7079 7965 7469 2069 6d70 6f72  rom pyyeti impor
+0001d220: 7420 6e61 7374 7261 6e0a 2020 2020 3e3e  t nastran.    >>
+0001d230: 3e20 6e61 7374 7261 6e2e 7774 6578 7472  > nastran.wtextr
+0001d240: 6e28 312c 205b 3939 392c 2031 3030 3031  n(1, [999, 10001
+0001d250: 2c20 3130 3030 322c 2031 3030 3033 2c20  , 10002, 10003, 
+0001d260: 3130 3030 342c 2031 3030 3035 5d2c 0a20  10004, 10005],. 
+0001d270: 2020 202e 2e2e 2020 2020 2020 2020 2020     ...          
+0001d280: 2020 2020 2020 2020 2020 5b31 3233 3435            [12345
+0001d290: 362c 2030 2c20 302c 2030 2c20 302c 2030  6, 0, 0, 0, 0, 0
+0001d2a0: 5d29 0a20 2020 2045 5854 524e 2020 2020  ]).    EXTRN    
+0001d2b0: 2020 2020 3939 3920 2031 3233 3435 3620      999  123456 
+0001d2c0: 2020 3130 3030 3120 2020 2020 2020 3020    10001       0 
+0001d2d0: 2020 3130 3030 3220 2020 2020 2020 3020    10002       0 
+0001d2e0: 2020 3130 3030 3320 2020 2020 2020 300a    10003       0.
+0001d2f0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
+0001d300: 3030 3034 2020 2020 2020 2030 2020 2031  0004       0   1
+0001d310: 3030 3035 2020 2020 2020 2030 0a20 2020  0005       0.   
+0001d320: 2022 2222 0a20 2020 2066 2e77 7269 7465   """.    f.write
+0001d330: 2822 4558 5452 4e20 2020 2229 0a20 2020  ("EXTRN   ").   
+0001d340: 2069 6e74 7320 3d20 6e70 2e7a 6572 6f73   ints = np.zeros
+0001d350: 286c 656e 2869 6473 2920 2a20 322c 2064  (len(ids) * 2, d
+0001d360: 7479 7065 3d69 6e74 290a 2020 2020 696e  type=int).    in
+0001d370: 7473 5b3a 3a32 5d20 3d20 6964 730a 2020  ts[::2] = ids.  
+0001d380: 2020 696e 7473 5b31 3a3a 325d 203d 2064    ints[1::2] = d
+0001d390: 6f66 0a20 2020 2077 746e 6173 696e 7473  of.    wtnasints
+0001d3a0: 2866 2c20 322c 2069 6e74 7329 0a0a 0a64  (f, 2, ints)...d
+0001d3b0: 6566 2077 7465 7874 7365 6f75 7428 0a20  ef wtextseout(. 
+0001d3c0: 2020 206e 616d 652c 0a20 2020 202a 2c0a     name,.    *,.
+0001d3d0: 2020 2020 7365 2c0a 2020 2020 6d61 612c      se,.    maa,
+0001d3e0: 0a20 2020 2062 6161 2c0a 2020 2020 6b61  .    baa,.    ka
+0001d3f0: 612c 0a20 2020 2062 7365 742c 0a20 2020  a,.    bset,.   
+0001d400: 2075 7365 742c 0a20 2020 2073 706f 696e   uset,.    spoin
+0001d410: 7431 2c0a 2020 2020 7365 646e 3d30 2c0a  t1,.    sedn=0,.
+0001d420: 2020 2020 6e61 6d65 6c69 7374 3d5b 0a20      namelist=[. 
+0001d430: 2020 2020 2020 2022 6b61 6122 2c0a 2020         "kaa",.  
+0001d440: 2020 2020 2020 226d 6161 222c 0a20 2020        "maa",.   
+0001d450: 2020 2020 2022 6261 6122 2c0a 2020 2020       "baa",.    
+0001d460: 2020 2020 226b 3478 7822 2c0a 2020 2020      "k4xx",.    
+0001d470: 2020 2020 2270 6122 2c0a 2020 2020 2020      "pa",.      
+0001d480: 2020 2267 7078 7822 2c0a 2020 2020 2020    "gpxx",.      
+0001d490: 2020 2267 6478 7822 2c0a 2020 2020 2020    "gdxx",.      
+0001d4a0: 2020 2272 7661 7822 2c0a 2020 2020 2020    "rvax",.      
+0001d4b0: 2020 2276 6122 2c0a 2020 2020 2020 2020    "va",.        
+0001d4c0: 226d 7567 3122 2c0a 2020 2020 2020 2020  "mug1",.        
+0001d4d0: 226d 7567 316f 222c 0a20 2020 2020 2020  "mug1o",.       
+0001d4e0: 2022 6d65 7331 222c 0a20 2020 2020 2020   "mes1",.       
+0001d4f0: 2022 6d65 7331 6f22 2c0a 2020 2020 2020   "mes1o",.      
+0001d500: 2020 226d 6565 3122 2c0a 2020 2020 2020    "mee1",.      
+0001d510: 2020 226d 6565 316f 222c 0a20 2020 2020    "mee1o",.     
+0001d520: 2020 2022 6d67 7066 222c 0a20 2020 2020     "mgpf",.     
+0001d530: 2020 2022 6d67 7066 6f22 2c0a 2020 2020     "mgpfo",.    
+0001d540: 2020 2020 226d 6566 3122 2c0a 2020 2020      "mef1",.    
+0001d550: 2020 2020 226d 6566 316f 222c 0a20 2020      "mef1o",.   
+0001d560: 2020 2020 2022 6d71 6731 222c 0a20 2020       "mqg1",.   
+0001d570: 2020 2020 2022 6d71 6731 6f22 2c0a 2020       "mqg1o",.  
+0001d580: 2020 2020 2020 226d 716d 6731 222c 0a20        "mqmg1",. 
+0001d590: 2020 2020 2020 2022 6d71 6d67 316f 222c         "mqmg1o",
+0001d5a0: 0a20 2020 205d 2c0a 2020 2020 2a2a 6b77  .    ],.    **kw
+0001d5b0: 6172 6773 2c0a 293a 0a20 2020 2022 2222  args,.):.    """
+0001d5c0: 0a20 2020 2057 7269 7465 202e 6f70 342c  .    Write .op4,
+0001d5d0: 202e 6173 6d2c 202e 7063 6820 616e 6420   .asm, .pch and 
+0001d5e0: 706f 7373 6962 6c79 2074 6865 2064 616d  possibly the dam
+0001d5f0: 7069 6e67 2044 4d49 4720 6669 6c65 2066  ping DMIG file f
+0001d600: 6f72 2061 6e0a 2020 2020 6578 7465 726e  or an.    extern
+0001d610: 616c 2053 452e 0a0a 2020 2020 4e6f 7465  al SE...    Note
+0001d620: 2074 6861 7420 616c 6c20 696e 7075 7473   that all inputs
+0001d630: 2065 7863 6570 7420 606e 616d 6560 206d   except `name` m
+0001d640: 7573 7420 6265 206e 616d 6564 2061 6e64  ust be named and
+0001d650: 2063 616e 2062 6520 696e 7075 740a 2020   can be input.  
+0001d660: 2020 696e 2061 6e79 206f 7264 6572 2e0a    in any order..
+0001d670: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0001d680: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001d690: 2020 206e 616d 6520 3a20 7374 7269 6e67     name : string
+0001d6a0: 0a20 2020 2020 2020 2042 6173 656e 616d  .        Basenam
+0001d6b0: 6520 666f 7220 6669 6c65 733b 2065 673a  e for files; eg:
+0001d6c0: 2027 7370 6163 6563 7261 6674 272e 2046   'spacecraft'. F
+0001d6d0: 696c 6573 2077 6974 6820 7468 650a 2020  iles with the.  
+0001d6e0: 2020 2020 2020 6578 7465 6e73 696f 6e73        extensions
+0001d6f0: 2027 2e6f 7034 272c 2027 2e61 736d 272c   '.op4', '.asm',
+0001d700: 2061 6e64 2027 2e70 6368 2720 7769 6c6c   and '.pch' will
+0001d710: 2062 6520 6372 6561 7465 642e 2049 6620   be created. If 
+0001d720: 6062 6860 0a20 2020 2020 2020 2069 7320  `bh`.        is 
+0001d730: 5472 7565 2c20 6120 272e 6261 615f 646d  True, a '.baa_dm
+0001d740: 6967 2720 6669 6c65 2077 696c 6c20 616c  ig' file will al
+0001d750: 736f 2062 6520 6372 6561 7465 642e 0a20  so be created.. 
+0001d760: 2020 2073 6520 3a20 696e 7465 6765 720a     se : integer.
+0001d770: 2020 2020 2020 2020 5375 7065 7265 6c65          Superele
+0001d780: 6d65 6e74 2069 643b 2061 6c73 6f20 7573  ment id; also us
+0001d790: 6564 2061 7320 7468 6520 466f 7274 7261  ed as the Fortra
+0001d7a0: 6e20 756e 6974 206e 756d 6265 7220 6f6e  n unit number on
+0001d7b0: 2074 6865 0a20 2020 2020 2020 2053 4542   the.        SEB
+0001d7c0: 554c 4b20 656e 7472 792e 0a20 2020 206d  ULK entry..    m
+0001d7d0: 6161 2c20 6261 612c 206b 6161 203a 2032  aa, baa, kaa : 2
+0001d7e0: 6420 6172 7261 795f 6c69 6b65 0a20 2020  d array_like.   
+0001d7f0: 2020 2020 2054 6865 7365 2061 7265 2074       These are t
+0001d800: 6865 2043 7261 6967 2d42 616d 7074 6f6e  he Craig-Bampton
+0001d810: 206d 6173 732c 2064 616d 7069 6e67 2061   mass, damping a
+0001d820: 6e64 2073 7469 6666 6e65 7373 0a20 2020  nd stiffness.   
+0001d830: 2020 2020 206d 6174 7269 6365 7320 7265       matrices re
+0001d840: 7370 6563 7469 7665 6c79 2e0a 2020 2020  spectively..    
+0001d850: 6273 6574 203a 2031 6420 6172 7261 795f  bset : 1d array_
+0001d860: 6c69 6b65 0a20 2020 2020 2020 2049 6e64  like.        Ind
+0001d870: 6578 2070 6172 7469 7469 6f6e 2076 6563  ex partition vec
+0001d880: 746f 7220 666f 7220 7468 6520 6273 6574  tor for the bset
+0001d890: 0a20 2020 2075 7365 7420 3a20 7061 6e64  .    uset : pand
+0001d8a0: 6173 2044 6174 6146 7261 6d65 0a20 2020  as DataFrame.   
+0001d8b0: 2020 2020 2041 2044 6174 6146 7261 6d65       A DataFrame
+0001d8c0: 2061 7320 6f75 7470 7574 2062 790a 2020   as output by.  
+0001d8d0: 2020 2020 2020 3a66 756e 633a 6070 7979        :func:`pyy
+0001d8e0: 6574 692e 6e61 7374 7261 6e2e 6f70 322e  eti.nastran.op2.
+0001d8f0: 4f50 322e 7264 6e32 636f 7032 602e 0a0a  OP2.rdn2cop2`...
+0001d900: 2020 2020 2020 2020 2e2e 2077 6172 6e69          .. warni
+0001d910: 6e67 3a3a 0a20 2020 2020 2020 2020 2020  ng::.           
+0001d920: 2055 6e6c 696b 6520 3a66 756e 633a 6070   Unlike :func:`p
+0001d930: 7979 6574 692e 6362 2e6d 6b5f 6e65 745f  yyeti.cb.mk_net_
+0001d940: 6472 6d73 602c 2074 6869 7320 5553 4554  drms`, this USET
+0001d950: 2074 6162 6c65 0a20 2020 2020 2020 2020   table.         
+0001d960: 2020 2064 6566 696e 6573 2074 6865 2062     defines the b
+0001d970: 2d73 6574 206e 6f64 6573 2072 656c 6174  -set nodes relat
+0001d980: 6976 6520 746f 2074 6865 2062 6173 6963  ive to the basic
+0001d990: 2063 6f6f 7264 696e 6174 650a 2020 2020   coordinate.    
+0001d9a0: 2020 2020 2020 2020 7379 7374 656d 206f          system o
+0001d9b0: 6620 7375 7065 7265 6c65 6d65 6e74 2030  f superelement 0
+0001d9c0: 2e20 5468 6973 2069 7320 736f 2074 6865  . This is so the
+0001d9d0: 2065 7874 6572 6e61 6c0a 2020 2020 2020   external.      
+0001d9e0: 2020 2020 2020 7375 7065 7265 6c65 6d65        supereleme
+0001d9f0: 6e74 2069 7320 706f 7369 7469 6f6e 6564  nt is positioned
+0001da00: 2070 726f 7065 726c 792e 204e 6f74 6520   properly. Note 
+0001da10: 686f 7765 7665 7220 7468 6174 2074 6865  however that the
+0001da20: 0a20 2020 2020 2020 2020 2020 2022 6469  .            "di
+0001da30: 7370 6c61 6365 6d65 6e74 2220 636f 6f72  splacement" coor
+0001da40: 6469 6e61 7465 2073 7973 7465 6d28 7329  dinate system(s)
+0001da50: 2028 7370 6563 6966 6965 6420 6166 7465   (specified afte
+0001da60: 7220 7468 650a 2020 2020 2020 2020 2020  r the.          
+0001da70: 2020 636f 6f72 6469 6e61 7465 7320 6f6e    coordinates on
+0001da80: 2074 6865 2022 4752 4944 2220 6361 7264   the "GRID" card
+0001da90: 2920 6d75 7374 206d 6174 6368 2077 6861  ) must match wha
+0001daa0: 7465 7665 7220 7468 650a 2020 2020 2020  tever the.      
+0001dab0: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
+0001dac0: 6e74 2063 6f6f 7264 696e 6174 6520 7379  nt coordinate sy
+0001dad0: 7374 656d 2873 2920 6172 6520 666f 7220  stem(s) are for 
+0001dae0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0001daf0: 4372 6169 672d 4261 6d70 746f 6e20 636f  Craig-Bampton co
+0001db00: 6d70 6f6e 656e 742e 0a0a 2020 2020 7370  mponent...    sp
+0001db10: 6f69 6e74 3120 3a20 696e 7465 6765 720a  oint1 : integer.
+0001db20: 2020 2020 2020 2020 5374 6172 7469 6e67          Starting
+0001db30: 2076 616c 7565 2066 6f72 2074 6865 2053   value for the S
+0001db40: 504f 494e 5473 2028 666f 7220 6d6f 6461  POINTs (for moda
+0001db50: 6c20 444f 4629 0a20 2020 2073 6564 6e20  l DOF).    sedn 
+0001db60: 3a20 696e 7465 6765 723b 206f 7074 696f  : integer; optio
+0001db70: 6e61 6c0a 2020 2020 2020 2020 446f 776e  nal.        Down
+0001db80: 7374 7265 616d 2073 7570 6572 656c 656d  stream superelem
+0001db90: 656e 7420 6964 0a20 2020 206e 616d 656c  ent id.    namel
+0001dba0: 6973 7420 3a20 6c69 7374 3b20 6f70 7469  ist : list; opti
+0001dbb0: 6f6e 616c 0a20 2020 2020 2020 204c 6973  onal.        Lis
+0001dbc0: 742c 2069 6e20 6f72 6465 722c 206f 6620  t, in order, of 
+0001dbd0: 6e61 6d65 7320 746f 2077 7269 7465 2074  names to write t
+0001dbe0: 6f20 7468 6520 6f70 3420 6669 6c65 2e20  o the op4 file. 
+0001dbf0: 5661 6c75 6573 0a20 2020 2020 2020 2064  Values.        d
+0001dc00: 6566 6175 6c74 2074 6f20 3178 3120 7a65  efault to 1x1 ze
+0001dc10: 726f 206d 6174 7269 6365 7320 7769 7468  ro matrices with
+0001dc20: 2074 6865 7365 2065 7863 6570 7469 6f6e   these exception
+0001dc30: 733a 2022 6d61 6122 2c0a 2020 2020 2020  s: "maa",.      
+0001dc40: 2020 226b 6161 222c 2022 6261 6122 2c20    "kaa", "baa", 
+0001dc50: 6172 6520 6173 2069 6e70 7574 2061 626f  are as input abo
+0001dc60: 7665 2c20 2270 6122 2069 7320 6120 7665  ve, "pa" is a ve
+0001dc70: 6374 6f72 206f 6620 7a65 726f 730a 2020  ctor of zeros.  
+0001dc80: 2020 2020 2020 616e 6420 2276 6122 2069        and "va" i
+0001dc90: 7320 6120 7665 6374 6f72 206f 6620 6f6e  s a vector of on
+0001dca0: 6573 2e20 5468 6520 6465 6661 756c 7473  es. The defaults
+0001dcb0: 2063 616e 2062 6520 6f76 6572 7269 6464   can be overridd
+0001dcc0: 656e 0a20 2020 2020 2020 2069 6e20 606b  en.        in `k
+0001dcd0: 7761 7267 7360 2e0a 2020 2020 2a2a 6b77  wargs`..    **kw
+0001dce0: 6172 6773 203a 206f 7074 696f 6e61 6c0a  args : optional.
+0001dcf0: 2020 2020 2020 2020 416c 6c6f 7773 2075          Allows u
+0001dd00: 7365 7220 746f 2069 6e70 7574 206f 7468  ser to input oth
+0001dd10: 6572 206d 6174 7269 6365 7320 746f 2062  er matrices to b
+0001dd20: 6520 7772 6974 7465 6e20 746f 2074 6865  e written to the
+0001dd30: 206f 7034 0a20 2020 2020 2020 2066 696c   op4.        fil
+0001dd40: 652e 204e 616d 6520 6d75 7374 2069 6e20  e. Name must in 
+0001dd50: 606e 616d 656c 6973 7460 2074 6f20 6265  `namelist` to be
+0001dd60: 2077 7269 7474 656e 2e0a 0a20 2020 2052   written...    R
+0001dd70: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0001dd80: 2d2d 0a20 2020 204e 6f6e 650a 2020 2020  --.    None.    
+0001dd90: 2222 220a 2020 2020 6d61 612c 2062 6161  """.    maa, baa
+0001dda0: 2c20 6b61 6120 3d20 6e70 2e61 746c 6561  , kaa = np.atlea
+0001ddb0: 7374 5f32 6428 6d61 612c 2062 6161 2c20  st_2d(maa, baa, 
+0001ddc0: 6b61 6129 0a20 2020 2062 7365 7420 3d20  kaa).    bset = 
+0001ddd0: 6e70 2e61 746c 6561 7374 5f31 6428 6273  np.atleast_1d(bs
+0001dde0: 6574 290a 2020 2020 6e20 3d20 6d61 612e  et).    n = maa.
+0001ddf0: 7368 6170 655b 305d 0a20 2020 206e 7120  shape[0].    nq 
+0001de00: 3d20 6e20 2d20 6c65 6e28 6273 6574 290a  = n - len(bset).
+0001de10: 0a20 2020 2023 2070 7265 7061 7265 2073  .    # prepare s
+0001de20: 7461 6e64 6172 6420 4e61 7374 7261 6e20  tandard Nastran 
+0001de30: 6f70 3420 6669 6c65 3a0a 2020 2020 7061  op4 file:.    pa
+0001de40: 203d 206e 702e 7a65 726f 7328 286e 2c20   = np.zeros((n, 
+0001de50: 3129 290a 2020 2020 7661 203d 206e 702e  1)).    va = np.
+0001de60: 6f6e 6573 2828 6e2c 2031 2929 0a20 2020  ones((n, 1)).   
+0001de70: 2064 6374 203d 207b 2a2a 6c6f 6361 6c73   dct = {**locals
+0001de80: 2829 2c20 2a2a 6b77 6172 6773 7d0a 2020  (), **kwargs}.  
+0001de90: 2020 7661 726c 6973 7420 3d20 5b64 6374    varlist = [dct
+0001dea0: 2e67 6574 2869 2c20 302e 3029 2066 6f72  .get(i, 0.0) for
+0001deb0: 2069 2069 6e20 6e61 6d65 6c69 7374 5d0a   i in namelist].
+0001dec0: 2020 2020 6f70 342e 7772 6974 6528 6e61      op4.write(na
+0001ded0: 6d65 202b 2022 2e6f 7034 222c 206e 616d  me + ".op4", nam
+0001dee0: 656c 6973 742c 2076 6172 6c69 7374 290a  elist, varlist).
+0001def0: 0a20 2020 2023 2047 6574 2073 6f6d 6520  .    # Get some 
+0001df00: 6461 7461 2066 726f 6d20 7468 6520 7573  data from the us
+0001df10: 6574 2074 6162 6c65 3a0a 2020 2020 6369  et table:.    ci
+0001df20: 203d 206e 3270 2e6d 6b63 6f72 6463 6172   = n2p.mkcordcar
+0001df30: 6469 6e66 6f28 7573 6574 290a 2020 2020  dinfo(uset).    
+0001df40: 6772 6964 7320 3d20 7573 6574 2e69 6e64  grids = uset.ind
+0001df50: 6578 2e67 6574 5f6c 6576 656c 5f76 616c  ex.get_level_val
+0001df60: 7565 7328 2269 6422 290a 2020 2020 646f  ues("id").    do
+0001df70: 6620 3d20 7573 6574 2e69 6e64 6578 2e67  f = uset.index.g
+0001df80: 6574 5f6c 6576 656c 5f76 616c 7565 7328  et_level_values(
+0001df90: 2264 6f66 2229 0a20 2020 2070 7620 3d20  "dof").    pv = 
+0001dfa0: 646f 6620 3d3d 2031 0a20 2020 2067 7269  dof == 1.    gri
+0001dfb0: 6473 203d 2067 7269 6473 5b70 765d 0a20  ds = grids[pv]. 
+0001dfc0: 2020 2078 797a 203d 2075 7365 742e 6c6f     xyz = uset.lo
+0001dfd0: 635b 7076 2c20 2278 223a 227a 225d 2e76  c[pv, "x":"z"].v
+0001dfe0: 616c 7565 730a 2020 2020 7076 203d 2064  alues.    pv = d
+0001dff0: 6f66 203d 3d20 320a 2020 2020 6364 203d  of == 2.    cd =
+0001e000: 2075 7365 742e 6c6f 635b 7076 2c20 2278   uset.loc[pv, "x
+0001e010: 225d 2e76 616c 7565 732e 6173 7479 7065  "].values.astype
+0001e020: 2869 6e74 290a 0a20 2020 2023 2057 7269  (int)..    # Wri
+0001e030: 7465 206f 7574 2041 534d 2066 696c 650a  te out ASM file.
+0001e040: 2020 2020 756e 6974 203d 2073 650a 2020      unit = se.  
+0001e050: 2020 7370 6f69 6e74 6e20 3d20 7370 6f69    spointn = spoi
+0001e060: 6e74 3120 2b20 6e71 202d 2031 0a20 2020  nt1 + nq - 1.   
+0001e070: 2077 6974 6820 6f70 656e 286e 616d 6520   with open(name 
+0001e080: 2b20 222e 6173 6d22 2c20 2277 2229 2061  + ".asm", "w") a
+0001e090: 7320 663a 0a20 2020 2020 2020 2066 2e77  s f:.        f.w
+0001e0a0: 7269 7465 280a 2020 2020 2020 2020 2020  rite(.          
+0001e0b0: 2020 6622 2420 7b6e 616d 652e 7570 7065    f"$ {name.uppe
+0001e0c0: 7228 297d 2041 5353 454d 424c 5920 4649  r()} ASSEMBLY FI
+0001e0d0: 4c45 2046 4f52 2052 4553 4944 5541 4c20  LE FOR RESIDUAL 
+0001e0e0: 5255 4e2e 2e2e 494e 434c 5544 4520 494e  RUN...INCLUDE IN
+0001e0f0: 2042 554c 4b20 4441 5441 5c6e 220a 2020   BULK DATA\n".  
+0001e100: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001e110: 662e 7772 6974 6528 2224 5c6e 2229 0a20  f.write("$\n"). 
+0001e120: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+0001e130: 2253 4542 554c 4b20 207b 7365 3a38 647d  "SEBULK  {se:8d}
+0001e140: 2020 4558 544f 5034 2020 2020 2020 2020    EXTOP4        
+0001e150: 2020 4d41 4e55 414c 2020 2020 2020 2020    MANUAL        
+0001e160: 2020 2020 2020 2020 7b75 6e69 743a 3864          {unit:8d
+0001e170: 7d5c 6e22 290a 2020 2020 2020 2020 662e  }\n").        f.
+0001e180: 7772 6974 6528 6622 5345 434f 4e43 5420  write(f"SECONCT 
+0001e190: 7b73 653a 3864 7d7b 7365 646e 3a38 647d  {se:8d}{sedn:8d}
+0001e1a0: 2020 2020 2020 2020 2020 2020 2020 4e4f                NO
+0001e1b0: 5c6e 2229 0a20 2020 2020 2020 2066 2e77  \n").        f.w
+0001e1c0: 7269 7465 2822 2020 2020 2020 2020 2229  rite("        ")
+0001e1d0: 0a20 2020 2020 2020 2067 6964 7320 3d20  .        gids = 
+0001e1e0: 6e70 2e76 7374 6163 6b28 2867 7269 6473  np.vstack((grids
+0001e1f0: 2c20 6772 6964 7329 292e 540a 2020 2020  , grids)).T.    
+0001e200: 2020 2020 7774 6e61 7369 6e74 7328 662c      wtnasints(f,
+0001e210: 2032 2c20 6769 6473 2e72 6176 656c 2829   2, gids.ravel()
+0001e220: 290a 0a20 2020 2020 2020 2023 2057 7269  )..        # Wri
+0001e230: 7465 2063 6f6f 7264 696e 6174 6520 7379  te coordinate sy
+0001e240: 7374 656d 2063 6172 6473 2069 6620 6e65  stem cards if ne
+0001e250: 6564 6564 3a0a 2020 2020 2020 2020 662e  eded:.        f.
+0001e260: 7772 6974 6528 2224 5c6e 2420 434f 4f52  write("$\n$ COOR
+0001e270: 4449 4e41 5445 2053 5953 5445 4d20 4441  DINATE SYSTEM DA
+0001e280: 5441 5c6e 245c 6e22 290a 2020 2020 2020  TA\n$\n").      
+0001e290: 2020 7774 636f 6f72 6463 6172 6473 2866    wtcoordcards(f
+0001e2a0: 2c20 6369 290a 0a20 2020 2020 2020 2023  , ci)..        #
+0001e2b0: 2057 7269 7465 2047 7269 6420 6461 7461   Write Grid data
+0001e2c0: 3a0a 2020 2020 2020 2020 662e 7772 6974  :.        f.writ
+0001e2d0: 6528 2224 5c6e 2420 424f 554e 4441 5259  e("$\n$ BOUNDARY
+0001e2e0: 2047 5249 4420 4441 5441 5c6e 245c 6e22   GRID DATA\n$\n"
+0001e2f0: 290a 2020 2020 2020 2020 7774 6772 6964  ).        wtgrid
+0001e300: 7328 662c 2067 7269 6473 2c20 302c 2078  s(f, grids, 0, x
+0001e310: 797a 2c20 6364 290a 2020 2020 2020 2020  yz, cd).        
+0001e320: 6966 2073 706f 696e 746e 203e 3d20 7370  if spointn >= sp
+0001e330: 6f69 6e74 313a 0a20 2020 2020 2020 2020  oint1:.         
+0001e340: 2020 2066 2e77 7269 7465 2822 245c 6e22     f.write("$\n"
+0001e350: 290a 2020 2020 2020 2020 2020 2020 662e  ).            f.
+0001e360: 7772 6974 6528 6622 5345 434f 4e43 5420  write(f"SECONCT 
+0001e370: 7b73 653a 3864 7d7b 7365 646e 3a38 647d  {se:8d}{sedn:8d}
+0001e380: 2020 2020 2020 2020 2020 2020 2020 4e4f                NO
+0001e390: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+0001e3a0: 2066 2e77 7269 7465 280a 2020 2020 2020   f.write(.      
+0001e3b0: 2020 2020 2020 2020 2020 6622 2020 2020            f"    
+0001e3c0: 2020 2020 7b73 706f 696e 7431 3a38 647d      {spoint1:8d}
+0001e3d0: 2020 2020 5448 5255 7b73 706f 696e 746e      THRU{spointn
+0001e3e0: 3a38 647d 220a 2020 2020 2020 2020 2020  :8d}".          
+0001e3f0: 2020 2020 2020 6622 7b73 706f 696e 7431        f"{spoint1
+0001e400: 3a38 647d 2020 2020 5448 5255 7b73 706f  :8d}    THRU{spo
+0001e410: 696e 746e 3a38 647d 5c6e 220a 2020 2020  intn:8d}\n".    
+0001e420: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001e430: 2020 2020 2020 662e 7772 6974 6528 2224        f.write("$
+0001e440: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+0001e450: 2066 2e77 7269 7465 2866 2253 504f 494e   f.write(f"SPOIN
+0001e460: 5420 207b 7370 6f69 6e74 313a 3864 7d20  T  {spoint1:8d} 
+0001e470: 2020 2054 4852 557b 7370 6f69 6e74 6e3a     THRU{spointn:
+0001e480: 3864 7d5c 6e22 290a 0a20 2020 2023 2057  8d}\n")..    # W
+0001e490: 7269 7465 206f 7574 2050 4348 2066 696c  rite out PCH fil
+0001e4a0: 650a 2020 2020 7769 7468 206f 7065 6e28  e.    with open(
+0001e4b0: 6e61 6d65 202b 2022 2e70 6368 222c 2022  name + ".pch", "
+0001e4c0: 7722 2920 6173 2066 3a0a 2020 2020 2020  w") as f:.      
+0001e4d0: 2020 662e 7772 6974 6528 6622 2420 7b6e    f.write(f"$ {n
+0001e4e0: 616d 652e 7570 7065 7228 297d 2050 554e  ame.upper()} PUN
+0001e4f0: 4348 2046 494c 4520 464f 5220 5245 5349  CH FILE FOR RESI
+0001e500: 4455 414c 2052 554e 2e2e 2e49 4e43 4c55  DUAL RUN...INCLU
+0001e510: 4445 2041 5420 454e 445c 6e22 290a 2020  DE AT END\n").  
+0001e520: 2020 2020 2020 662e 7772 6974 6528 2224        f.write("$
+0001e530: 5c6e 2229 0a20 2020 2020 2020 2066 2e77  \n").        f.w
+0001e540: 7269 7465 2866 2242 4547 494e 2053 5550  rite(f"BEGIN SUP
+0001e550: 4552 7b73 653a 3864 7d5c 6e24 5c6e 2229  ER{se:8d}\n$\n")
+0001e560: 0a20 2020 2020 2020 2069 6473 203d 206e  .        ids = n
+0001e570: 702e 6873 7461 636b 2828 6772 6964 732c  p.hstack((grids,
+0001e580: 2073 706f 696e 7431 202b 206e 702e 6172   spoint1 + np.ar
+0001e590: 616e 6765 286e 7129 2929 0a20 2020 2020  ange(nq))).     
+0001e5a0: 2020 2064 6f66 203d 206e 702e 7a65 726f     dof = np.zero
+0001e5b0: 735f 6c69 6b65 2869 6473 2c20 6474 7970  s_like(ids, dtyp
+0001e5c0: 653d 696e 7429 0a20 2020 2020 2020 2064  e=int).        d
+0001e5d0: 6f66 5b3a 206c 656e 2867 7269 6473 295d  of[: len(grids)]
+0001e5e0: 203d 2031 3233 3435 360a 2020 2020 2020   = 123456.      
+0001e5f0: 2020 7774 6578 7472 6e28 662c 2069 6473    wtextrn(f, ids
+0001e600: 2c20 646f 6629 0a20 2020 2020 2020 2066  , dof).        f
+0001e610: 2e77 7269 7465 2822 245c 6e22 290a 2020  .write("$\n").  
+0001e620: 2020 2020 2020 662e 7772 6974 6528 2224        f.write("$
+0001e630: 2043 4f4f 5244 494e 4154 4520 5359 5354   COORDINATE SYST
+0001e640: 454d 2044 4154 415c 6e24 5c6e 2229 0a20  EM DATA\n$\n"). 
+0001e650: 2020 2020 2020 2077 7463 6f6f 7264 6361         wtcoordca
+0001e660: 7264 7328 662c 2063 6929 0a20 2020 2020  rds(f, ci).     
+0001e670: 2020 2066 2e77 7269 7465 2822 245c 6e24     f.write("$\n$
+0001e680: 2042 4f55 4e44 4152 5920 4752 4944 2044   BOUNDARY GRID D
+0001e690: 4154 415c 6e24 5c6e 2229 0a20 2020 2020  ATA\n$\n").     
+0001e6a0: 2020 2077 7467 7269 6473 2866 2c20 6772     wtgrids(f, gr
+0001e6b0: 6964 732c 2030 2c20 7879 7a2c 2063 6429  ids, 0, xyz, cd)
+0001e6c0: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+0001e6d0: 2822 245c 6e22 290a 0a20 2020 2020 2020  ("$\n")..       
+0001e6e0: 2066 2e77 7269 7465 2822 2420 4253 4554   f.write("$ BSET
+0001e6f0: 5c6e 245c 6e22 290a 2020 2020 2020 2020  \n$\n").        
+0001e700: 662e 7772 6974 6528 6622 4153 4554 3120  f.write(f"ASET1 
+0001e710: 2020 7b31 3233 3435 363a 3864 7d22 290a    {123456:8d}").
+0001e720: 2020 2020 2020 2020 7774 6e61 7369 6e74          wtnasint
+0001e730: 7328 662c 2033 2c20 6772 6964 7329 0a20  s(f, 3, grids). 
+0001e740: 2020 2020 2020 2069 6620 7370 6f69 6e74         if spoint
+0001e750: 6e20 3e3d 2073 706f 696e 7431 3a0a 2020  n >= spoint1:.  
+0001e760: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+0001e770: 6528 2224 5c6e 2229 0a20 2020 2020 2020  e("$\n").       
+0001e780: 2020 2020 2066 2e77 7269 7465 2822 2420       f.write("$ 
+0001e790: 5153 4554 5c6e 245c 6e22 290a 2020 2020  QSET\n$\n").    
+0001e7a0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+0001e7b0: 6622 5153 4554 3120 2020 7b30 3a38 647d  f"QSET1   {0:8d}
+0001e7c0: 7b73 706f 696e 7431 3a38 647d 2020 2020  {spoint1:8d}    
+0001e7d0: 5448 5255 7b73 706f 696e 746e 3a38 647d  THRU{spointn:8d}
+0001e7e0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+0001e7f0: 2066 2e77 7269 7465 2822 245c 6e22 290a   f.write("$\n").
+0001e800: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+0001e810: 6974 6528 6622 5350 4f49 4e54 2020 7b73  ite(f"SPOINT  {s
+0001e820: 706f 696e 7431 3a38 647d 2020 2020 5448  point1:8d}    TH
+0001e830: 5255 7b73 706f 696e 746e 3a38 647d 5c6e  RU{spointn:8d}\n
+0001e840: 2229 0a0a 0a64 6566 206d 6b6e 6173 7428  ")...def mknast(
+0001e850: 0a20 2020 2073 6372 6970 743d 4e6f 6e65  .    script=None
+0001e860: 2c0a 2020 2020 2a2c 0a20 2020 206e 6173  ,.    *,.    nas
+0001e870: 636f 6d3d 226e 6173 7439 7031 222c 0a20  com="nast9p1",. 
+0001e880: 2020 206e 6173 6f70 743d 2262 6174 6368     nasopt="batch
+0001e890: 3d6e 6f22 2c0a 2020 2020 6578 743d 226f  =no",.    ext="o
+0001e8a0: 7574 222c 0a20 2020 2073 746f 706f 6e66  ut",.    stoponf
+0001e8b0: 6174 616c 3d46 616c 7365 2c0a 2020 2020  atal=False,.    
+0001e8c0: 7368 656c 6c3d 222f 6269 6e2f 7368 222c  shell="/bin/sh",
+0001e8d0: 0a20 2020 2066 696c 6573 3d4e 6f6e 652c  .    files=None,
+0001e8e0: 0a20 2020 2062 6566 6f72 653d 2222 2c0a  .    before="",.
+0001e8f0: 2020 2020 6166 7465 723d 2222 2c0a 2020      after="",.  
+0001e900: 2020 746f 703d 2222 2c0a 2020 2020 626f    top="",.    bo
+0001e910: 7474 6f6d 3d22 222c 0a29 3a0a 2020 2020  ttom="",.):.    
+0001e920: 2222 220a 2020 2020 4372 6561 7465 7320  """.    Creates 
+0001e930: 6120 7368 656c 6c20 7363 7269 7074 2066  a shell script f
+0001e940: 6f72 2072 756e 6e69 6e67 2061 2063 6861  or running a cha
+0001e950: 696e 206f 6620 4e61 7374 7261 6e20 286f  in of Nastran (o
+0001e960: 7220 6f74 6865 7229 0a20 2020 2072 756e  r other).    run
+0001e970: 732e 0a0a 2020 2020 4e6f 7465 2074 6861  s...    Note tha
+0001e980: 7420 616c 6c20 696e 7075 7473 2065 7863  t all inputs exc
+0001e990: 6570 7420 6073 6372 6970 7460 206d 7573  ept `script` mus
+0001e9a0: 7420 6265 206e 616d 6564 2061 6e64 2063  t be named and c
+0001e9b0: 616e 2062 650a 2020 2020 696e 7075 7420  an be.    input 
+0001e9c0: 696e 2061 6e79 206f 7264 6572 2e0a 0a20  in any order... 
+0001e9d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001e9e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001e9f0: 2073 6372 6970 7420 3a20 7374 7269 6e67   script : string
+0001ea00: 206f 7220 4e6f 6e65 3b20 6f70 7469 6f6e   or None; option
+0001ea10: 616c 0a20 2020 2020 2020 204e 616d 6520  al.        Name 
+0001ea20: 6f66 2073 6865 6c6c 2073 6372 6970 7420  of shell script 
+0001ea30: 746f 2063 7265 6174 653b 2069 6620 4e6f  to create; if No
+0001ea40: 6e65 2c20 7573 6572 2069 7320 7072 6f6d  ne, user is prom
+0001ea50: 7074 6564 2066 6f72 0a20 2020 2020 2020  pted for.       
+0001ea60: 206e 616d 652e 0a20 2020 206e 6173 636f   name..    nasco
+0001ea70: 6d20 3a20 7374 7269 6e67 3b20 6f70 7469  m : string; opti
+0001ea80: 6f6e 616c 0a20 2020 2020 2020 204e 6173  onal.        Nas
+0001ea90: 7472 616e 2063 6f6d 6d61 6e64 3b20 6e6f  tran command; no
+0001eaa0: 7465 3a20 7468 6973 2063 616e 2061 6374  te: this can act
+0001eab0: 7561 6c6c 7920 7370 6563 6966 7920 616e  ually specify an
+0001eac0: 7920 7072 6f67 7261 6d2c 0a20 2020 2020  y program,.     
+0001ead0: 2020 2062 7574 2060 6e61 736f 7074 6020     but `nasopt` 
+0001eae0: 776f 756c 6420 6c69 6b65 6c79 206e 6565  would likely nee
+0001eaf0: 6420 6164 6a75 7374 696e 6720 746f 6f2e  d adjusting too.
+0001eb00: 0a20 2020 206e 6173 6f70 7420 3a20 7374  .    nasopt : st
+0001eb10: 7269 6e67 3b20 6f70 7469 6f6e 616c 0a20  ring; optional. 
+0001eb20: 2020 2020 2020 204f 7074 696f 6e73 2066         Options f
+0001eb30: 6f72 206e 6173 7472 616e 2063 6f6d 6d61  or nastran comma
+0001eb40: 6e64 0a20 2020 2065 7874 203a 2073 7472  nd.    ext : str
+0001eb50: 696e 673b 206f 7074 696f 6e61 6c0a 2020  ing; optional.  
+0001eb60: 2020 2020 2020 5468 6520 6578 7465 6e73        The extens
+0001eb70: 696f 6e20 6f66 2074 6865 204e 6173 7472  ion of the Nastr
+0001eb80: 616e 206f 7574 7075 7420 2866 3036 2920  an output (f06) 
+0001eb90: 6669 6c65 3b20 7573 7561 6c6c 7920 2766  file; usually 'f
+0001eba0: 3036 270a 2020 2020 2020 2020 6f72 2027  06'.        or '
+0001ebb0: 6f75 7427 0a20 2020 2073 746f 706f 6e66  out'.    stoponf
+0001ebc0: 6174 616c 203a 2062 6f6f 6c3b 206f 7074  atal : bool; opt
+0001ebd0: 696f 6e61 6c0a 2020 2020 2020 2020 5365  ional.        Se
+0001ebe0: 7420 746f 2054 7275 6520 6966 2079 6f75  t to True if you
+0001ebf0: 2077 616e 7420 7468 6520 7363 7269 7074   want the script
+0001ec00: 2074 6f20 6578 6974 206f 6e20 6669 7273   to exit on firs
+0001ec10: 7420 4641 5441 4c0a 2020 2020 2020 2020  t FATAL.        
+0001ec20: 696e 7374 6561 6420 6f66 2063 6f6e 7469  instead of conti
+0001ec30: 6e75 696e 6720 6f6e 0a20 2020 2073 6865  nuing on.    she
+0001ec40: 6c6c 203a 2073 7472 696e 673b 206f 7074  ll : string; opt
+0001ec50: 696f 6e61 6c0a 2020 2020 2020 2020 5368  ional.        Sh
+0001ec60: 656c 6c20 7072 6f67 7261 6d20 746f 2077  ell program to w
+0001ec70: 7269 7465 2061 7420 746f 7020 6f66 2073  rite at top of s
+0001ec80: 6372 6970 742c 2065 673a 2023 2160 7368  cript, eg: #!`sh
+0001ec90: 656c 6c60 0a20 2020 2066 696c 6573 203a  ell`.    files :
+0001eca0: 2073 7472 696e 6720 6f72 204e 6f6e 653b   string or None;
+0001ecb0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0001ecc0: 2020 4c69 7374 206f 6620 6669 6c65 6e61    List of filena
+0001ecd0: 6d65 7320 746f 2072 756e 3b20 6966 204e  mes to run; if N
+0001ece0: 6f6e 652c 2075 7365 7220 6973 2070 726f  one, user is pro
+0001ecf0: 6d70 7465 6420 666f 7220 6e61 6d65 730a  mpted for names.
+0001ed00: 2020 2020 6265 666f 7265 203a 2073 7472      before : str
+0001ed10: 696e 673b 206f 7074 696f 6e61 6c0a 2020  ing; optional.  
+0001ed20: 2020 2020 2020 5374 7269 6e67 2074 6f20        String to 
+0001ed30: 7075 7420 696e 2073 6865 6c6c 2073 6372  put in shell scr
+0001ed40: 6970 7420 6265 666f 7265 2065 6163 6820  ipt before each 
+0001ed50: 6e61 7374 7261 6e20 636f 6d6d 616e 640a  nastran command.
+0001ed60: 2020 2020 6166 7465 7220 3a20 7374 7269      after : stri
+0001ed70: 6e67 3b20 6f70 7469 6f6e 616c 0a20 2020  ng; optional.   
+0001ed80: 2020 2020 2053 7472 696e 6720 746f 2070       String to p
+0001ed90: 7574 2069 6e20 7368 656c 6c20 7363 7269  ut in shell scri
+0001eda0: 7074 2061 6674 6572 2065 6163 6820 6e61  pt after each na
+0001edb0: 7374 7261 6e20 636f 6d6d 616e 640a 2020  stran command.  
+0001edc0: 2020 746f 7020 3a20 7374 7269 6e67 3b20    top : string; 
+0001edd0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0001ede0: 2053 7472 696e 6720 746f 2070 7574 2069   String to put i
+0001edf0: 6e20 7368 656c 6c20 7363 7269 7074 2061  n shell script a
+0001ee00: 7420 7468 6520 746f 700a 2020 2020 626f  t the top.    bo
+0001ee10: 7474 6f6d 203a 2073 7472 696e 673b 206f  ttom : string; o
+0001ee20: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0001ee30: 5374 7269 6e67 2074 6f20 7075 7420 696e  String to put in
+0001ee40: 2073 6865 6c6c 2073 6372 6970 7420 6174   shell script at
+0001ee50: 2074 6865 2062 6f74 746f 6d0a 0a20 2020   the bottom..   
+0001ee60: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+0001ee70: 2d2d 2d2d 0a20 2020 204e 6f6e 650a 0a20  ----.    None.. 
+0001ee80: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+0001ee90: 2d2d 0a20 2020 2049 6620 796f 7527 7265  --.    If you're
+0001eea0: 2069 6e20 7468 6520 2762 6173 6827 2073   in the 'bash' s
+0001eeb0: 6865 6c6c 2c20 7468 6520 7265 7375 6c74  hell, the result
+0001eec0: 696e 6720 7363 7269 7074 2063 616e 2062  ing script can b
+0001eed0: 6520 7275 6e20 696e 0a20 2020 2074 6865  e run in.    the
+0001eee0: 2062 6163 6b67 726f 756e 6420 7769 7468   background with
+0001eef0: 2c20 6173 7375 6d69 6e67 2074 6865 2073  , assuming the s
+0001ef00: 6372 6970 7420 6e61 6d65 2069 7320 2764  cript name is 'd
+0001ef10: 6f72 756e 732e 7368 273a 3a0a 0a20 2020  oruns.sh'::..   
+0001ef20: 2020 2020 6e6f 6875 7020 2e2f 646f 7275      nohup ./doru
+0001ef30: 6e73 2e73 6820 3e20 646f 7275 6e73 2e6c  ns.sh > doruns.l
+0001ef40: 6f67 2032 3e26 3120 260a 0a20 2020 2045  og 2>&1 &..    E
+0001ef50: 7861 6d70 6c65 2075 7361 6765 3a3a 0a0a  xample usage::..
+0001ef60: 2020 2020 2020 2020 6672 6f6d 2070 7979          from pyy
+0001ef70: 6574 6920 696d 706f 7274 206e 6173 7472  eti import nastr
+0001ef80: 616e 0a20 2020 2020 2020 206e 6173 7472  an.        nastr
+0001ef90: 616e 2e6d 6b6e 6173 7428 2764 6f72 756e  an.mknast('dorun
+0001efa0: 732e 7368 272c 2066 696c 6573 3d5b 2766  s.sh', files=['f
+0001efb0: 696c 6531 2e64 6174 272c 2027 6669 6c65  ile1.dat', 'file
+0001efc0: 322e 6461 7427 5d29 0a20 2020 2022 2222  2.dat']).    """
+0001efd0: 0a20 2020 2023 204e 616d 6520 6f66 2073  .    # Name of s
+0001efe0: 6372 6970 7420 746f 2063 7265 6174 653a  cript to create:
+0001eff0: 0a20 2020 2069 6620 7363 7269 7074 2069  .    if script i
+0001f000: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0001f010: 7363 7269 7074 203d 2069 6e70 7574 2822  script = input("
+0001f020: 4e61 6d65 206f 6620 7368 656c 6c20 7363  Name of shell sc
+0001f030: 7269 7074 2074 6f20 6372 6561 7465 2028  ript to create (
+0001f040: 646f 7275 6e73 2e73 6829 3a20 2229 0a20  doruns.sh): "). 
+0001f050: 2020 2020 2020 2069 6620 6e6f 7420 7363         if not sc
+0001f060: 7269 7074 3a0a 2020 2020 2020 2020 2020  ript:.          
+0001f070: 2020 7363 7269 7074 203d 2022 646f 7275    script = "doru
+0001f080: 6e73 2e73 6822 0a0a 2020 2020 2320 696e  ns.sh"..    # in
+0001f090: 6974 6961 6c69 7a65 2073 6865 6c6c 2073  itialize shell s
+0001f0a0: 6372 6970 740a 2020 2020 4752 4550 203d  cript.    GREP =
+0001f0b0: 2022 6772 6570 202d 6c20 275b 2a5e 5d5b   "grep -l '[*^][
+0001f0c0: 2a5e 5d5b 2a5e 5d2e 2a46 4154 414c 2722  *^][*^].*FATAL'"
+0001f0d0: 0a20 2020 2077 6974 6820 6f70 656e 2873  .    with open(s
+0001f0e0: 6372 6970 742c 2022 7722 2920 6173 2066  cript, "w") as f
+0001f0f0: 3a0a 2020 2020 2020 2020 662e 7772 6974  :.        f.writ
+0001f100: 6528 6622 2321 7b73 6865 6c6c 7d5c 6e22  e(f"#!{shell}\n"
+0001f110: 290a 2020 2020 2020 2020 6375 7264 6972  ).        curdir
+0001f120: 203d 206f 732e 6765 7463 7764 2829 0a20   = os.getcwd(). 
+0001f130: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+0001f140: 2263 6420 7b63 7572 6469 727d 5c6e 5c6e  "cd {curdir}\n\n
+0001f150: 2229 0a20 2020 2020 2020 2069 6620 746f  ").        if to
+0001f160: 703a 0a20 2020 2020 2020 2020 2020 2066  p:.            f
+0001f170: 2e77 7269 7465 2866 227b 746f 707d 5c6e  .write(f"{top}\n
+0001f180: 2229 0a0a 2020 2020 2020 2020 6920 3d20  ")..        i = 
+0001f190: 2d31 0a20 2020 2020 2020 2077 6869 6c65  -1.        while
+0001f1a0: 2031 3a20 2023 206c 6f6f 7020 6f76 6572   1:  # loop over
+0001f1b0: 2066 696c 6520 6e61 6d65 730a 2020 2020   file names.    
+0001f1c0: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
+0001f1d0: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
+0001f1e0: 6c65 7320 6973 206e 6f74 204e 6f6e 653a  les is not None:
+0001f1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f200: 2069 6620 6920 3e3d 206c 656e 2866 696c   if i >= len(fil
+0001f210: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+0001f220: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+0001f230: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001f240: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001f250: 2020 2020 2020 2020 206e 6173 6669 6c65           nasfile
+0001f260: 203d 2066 696c 6573 5b69 5d0a 2020 2020   = files[i].    
+0001f270: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001f280: 2020 2020 2020 2020 2020 2020 2020 7020                p 
+0001f290: 3d20 6622 4669 6c65 2023 7b69 202b 2031  = f"File #{i + 1
+0001f2a0: 3a32 647d 2028 626c 616e 6b20 746f 2071  :2d} (blank to q
+0001f2b0: 7569 7429 3a20 220a 2020 2020 2020 2020  uit): ".        
+0001f2c0: 2020 2020 2020 2020 6e61 7366 696c 6520          nasfile 
+0001f2d0: 3d20 696e 7075 7428 7029 0a20 2020 2020  = input(p).     
+0001f2e0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0001f2f0: 7420 6e61 7366 696c 653a 0a20 2020 2020  t nasfile:.     
+0001f300: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001f310: 7265 616b 0a0a 2020 2020 2020 2020 2020  reak..          
+0001f320: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+0001f330: 2e65 7869 7374 7328 6e61 7366 696c 6529  .exists(nasfile)
+0001f340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001f350: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+0001f360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f370: 2020 2020 2066 2266 696c 6520 277b 6e61       f"file '{na
+0001f380: 7366 696c 657d 2720 6e6f 7420 666f 756e  sfile}' not foun
+0001f390: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0001f3a0: 2020 2020 2020 2020 5275 6e74 696d 6557          RuntimeW
+0001f3b0: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
+0001f3c0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001f3d0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+0001f3e0: 225c 6e23 202a 2a2a 2a2a 2a2a 2a20 4669  "\n# ******** Fi
+0001f3f0: 6c65 207b 6e61 7366 696c 657d 202a 2a2a  le {nasfile} ***
+0001f400: 2a2a 2a2a 2a5c 6e22 290a 2020 2020 2020  *****\n").      
+0001f410: 2020 2020 2020 7020 3d20 6e61 7366 696c        p = nasfil
+0001f420: 652e 7266 696e 6428 222f 2229 0a20 2020  e.rfind("/").   
+0001f430: 2020 2020 2020 2020 2069 6620 7020 3e20           if p > 
+0001f440: 2d31 3a0a 2020 2020 2020 2020 2020 2020  -1:.            
+0001f450: 2020 2020 6669 6c65 7061 7468 203d 206e      filepath = n
+0001f460: 6173 6669 6c65 5b3a 705d 0a20 2020 2020  asfile[:p].     
+0001f470: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+0001f480: 616d 6520 3d20 6e61 7366 696c 655b 7020  ame = nasfile[p 
+0001f490: 2b20 3120 3a5d 0a20 2020 2020 2020 2020  + 1 :].         
+0001f4a0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+0001f4b0: 2220 2063 6420 7b66 696c 6570 6174 687d  "  cd {filepath}
+0001f4c0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+0001f4d0: 2020 2020 2064 6f63 6420 3d20 310a 2020       docd = 1.  
+0001f4e0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f500: 6669 6c65 6e61 6d65 203d 206e 6173 6669  filename = nasfi
+0001f510: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
+0001f520: 2020 2064 6f63 6420 3d20 300a 0a20 2020     docd = 0..   
+0001f530: 2020 2020 2020 2020 2069 6620 6265 666f           if befo
+0001f540: 7265 3a0a 2020 2020 2020 2020 2020 2020  re:.            
+0001f550: 2020 2020 662e 7772 6974 6528 6622 7b62      f.write(f"{b
+0001f560: 6566 6f72 657d 5c6e 2229 0a20 2020 2020  efore}\n").     
+0001f570: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+0001f580: 2220 207b 6e61 7363 6f6d 7d20 277b 6e61  "  {nascom} '{na
+0001f590: 736f 7074 7d27 2027 7b66 696c 656e 616d  sopt}' '{filenam
+0001f5a0: 657d 275c 6e22 290a 0a20 2020 2020 2020  e}'\n")..       
+0001f5b0: 2020 2020 2069 6620 7374 6f70 6f6e 6661       if stoponfa
+0001f5c0: 7461 6c3a 0a20 2020 2020 2020 2020 2020  tal:.           
+0001f5d0: 2020 2020 2070 203d 2066 696c 656e 616d       p = filenam
+0001f5e0: 652e 7266 696e 6428 222e 2229 0a20 2020  e.rfind(".").   
+0001f5f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001f600: 7020 3e20 2d31 3a0a 2020 2020 2020 2020  p > -1:.        
+0001f610: 2020 2020 2020 2020 2020 2020 6630 3666              f06f
+0001f620: 696c 6520 3d20 6669 6c65 6e61 6d65 5b3a  ile = filename[:
+0001f630: 2070 202b 2031 5d20 2b20 6578 740a 2020   p + 1] + ext.  
+0001f640: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0001f650: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001f660: 2020 2020 2020 2020 6630 3666 696c 6520          f06file 
+0001f670: 3d20 6669 6c65 6e61 6d65 202b 2022 2e22  = filename + "."
+0001f680: 202b 2065 7874 0a0a 2020 2020 2020 2020   + ext..        
+0001f690: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+0001f6a0: 6622 2020 6966 205b 2058 2021 3d20 5860  f"  if [ X != X`
+0001f6b0: 7b47 5245 507d 207b 6630 3666 696c 657d  {GREP} {f06file}
+0001f6c0: 6020 5d20 3b20 7468 656e 5c6e 2229 0a20  ` ] ; then\n"). 
+0001f6d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001f6e0: 2e77 7269 7465 2822 2020 2020 6578 6974  .write("    exit
+0001f6f0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+0001f700: 2020 2020 2066 2e77 7269 7465 2822 2020       f.write("  
+0001f710: 6669 5c6e 2229 0a20 2020 2020 2020 2020  fi\n").         
+0001f720: 2020 2069 6620 6166 7465 723a 0a20 2020     if after:.   
+0001f730: 2020 2020 2020 2020 2020 2020 2066 2e77               f.w
+0001f740: 7269 7465 2866 227b 6166 7465 727d 5c6e  rite(f"{after}\n
+0001f750: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+0001f760: 6966 2064 6f63 643a 0a20 2020 2020 2020  if docd:.       
+0001f770: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+0001f780: 2866 2220 2063 6420 7b63 7572 6469 727d  (f"  cd {curdir}
+0001f790: 5c6e 2229 0a0a 2020 2020 2020 2020 6966  \n")..        if
+0001f7a0: 2062 6f74 746f 6d3a 0a20 2020 2020 2020   bottom:.       
+0001f7b0: 2020 2020 2066 2e77 7269 7465 2866 227b       f.write(f"{
+0001f7c0: 626f 7474 6f6d 7d5c 6e22 290a 2020 2020  bottom}\n").    
+0001f7d0: 6f73 2e73 7973 7465 6d28 6622 6368 6d6f  os.system(f"chmo
+0001f7e0: 6420 612b 7278 2027 7b73 6372 6970 747d  d a+rx '{script}
+0001f7f0: 2722 290a 0a0a 6465 6620 7264 6474 6970  '")...def rddtip
+0001f800: 6368 2866 2c20 6e61 6d65 3d22 5455 4731  ch(f, name="TUG1
+0001f810: 2229 3a0a 2020 2020 2222 220a 2020 2020  "):.    """.    
+0001f820: 5265 6164 2074 6865 2032 6e64 2072 6563  Read the 2nd rec
+0001f830: 6f72 6420 6f66 2073 7065 6369 6669 6320  ord of specific 
+0001f840: 4454 4973 2066 726f 6d20 6120 2e70 6368  DTIs from a .pch
+0001f850: 2066 696c 652e 0a0a 2020 2020 5061 7261   file...    Para
+0001f860: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0001f870: 2d2d 2d2d 2d0a 2020 2020 6620 3a20 7374  -----.    f : st
+0001f880: 7269 6e67 206f 7220 6669 6c65 5f6c 696b  ring or file_lik
+0001f890: 6520 6f72 204e 6f6e 650a 2020 2020 2020  e or None.      
+0001f8a0: 2020 4569 7468 6572 2061 206e 616d 6520    Either a name 
+0001f8b0: 6f66 2061 2066 696c 652c 206f 7220 6973  of a file, or is
+0001f8c0: 2061 2066 696c 655f 6c69 6b65 206f 626a   a file_like obj
+0001f8d0: 6563 7420 6173 2072 6574 7572 6e65 640a  ect as returned.
+0001f8e0: 2020 2020 2020 2020 6279 203a 6675 6e63          by :func
+0001f8f0: 3a60 6f70 656e 602e 2049 6620 6669 6c65  :`open`. If file
+0001f900: 5f6c 696b 6520 6f62 6a65 6374 2c20 6974  _like object, it
+0001f910: 2069 7320 7265 776f 756e 6420 6669 7273   is rewound firs
+0001f920: 742e 2043 616e 0a20 2020 2020 2020 2061  t. Can.        a
+0001f930: 6c73 6f20 6265 2074 6865 206e 616d 6520  lso be the name 
+0001f940: 6f66 2061 2064 6972 6563 746f 7279 206f  of a directory o
+0001f950: 7220 4e6f 6e65 3b20 696e 2074 6865 7365  r None; in these
+0001f960: 2063 6173 6573 2c20 6120 4755 490a 2020   cases, a GUI.  
+0001f970: 2020 2020 2020 6973 206f 7065 6e65 6420        is opened 
+0001f980: 666f 7220 6669 6c65 2073 656c 6563 7469  for file selecti
+0001f990: 6f6e 2e0a 2020 2020 6e61 6d65 203a 2073  on..    name : s
+0001f9a0: 7472 696e 670a 2020 2020 2020 2020 4e61  tring.        Na
+0001f9b0: 6d65 206f 6620 4454 4920 7461 626c 6520  me of DTI table 
+0001f9c0: 746f 2072 6561 6420 6672 6f6d 2074 6865  to read from the
+0001f9d0: 202e 7063 6820 6669 6c65 0a0a 2020 2020   .pch file..    
+0001f9e0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+0001f9f0: 2d2d 2d0a 2020 2020 6964 5f64 6f66 203a  ---.    id_dof :
+0001fa00: 206e 6461 7272 6179 0a20 2020 2020 2020   ndarray.       
+0001fa10: 2032 2d63 6f6c 756d 6e20 6d61 7472 6978   2-column matrix
+0001fa20: 206f 6620 7468 6520 666f 726d 3a20 6060   of the form: ``
+0001fa30: 5b69 642c 2064 6f66 5d60 602e 2054 6865  [id, dof]``. The
+0001fa40: 206e 756d 6265 7220 6f66 2072 6f77 730a   number of rows.
+0001fa50: 2020 2020 2020 2020 696e 2060 6964 5f64          in `id_d
+0001fa60: 6f66 6020 636f 7272 6573 706f 6e64 7320  of` corresponds 
+0001fa70: 746f 2074 6865 206d 6174 6368 696e 6720  to the matching 
+0001fa80: 6d61 7472 6978 2069 6e20 2e6f 7034 2066  matrix in .op4 f
+0001fa90: 696c 650a 2020 2020 2020 2020 2873 6565  ile.        (see
+0001faa0: 204e 6f74 6573 292e 0a0a 2020 2020 4e6f   Notes)...    No
+0001fab0: 7465 730a 2020 2020 2d2d 2d2d 2d0a 2020  tes.    -----.  
+0001fac0: 2020 5468 6973 2072 6f75 7469 6e65 2069    This routine i
+0001fad0: 7320 7573 6566 756c 2066 6f72 2072 6561  s useful for rea
+0001fae0: 6469 6e67 2064 6174 6120 6672 6f6d 202e  ding data from .
+0001faf0: 7063 6820 6669 6c65 7320 7772 6974 7465  pch files writte
+0001fb00: 6e20 6279 0a20 2020 2074 6865 2045 5854  n by.    the EXT
+0001fb10: 5345 4f55 5420 636f 6d6d 616e 642e 2054  SEOUT command. T
+0001fb20: 6865 2032 6e64 2072 6563 6f72 6420 6f66  he 2nd record of
+0001fb30: 2022 5455 4731 2220 2866 6f72 2065 7861   "TUG1" (for exa
+0001fb40: 6d70 6c65 290a 2020 2020 636f 6e74 6169  mple).    contai
+0001fb50: 6e73 2074 6865 2044 4f46 2074 6861 7420  ns the DOF that 
+0001fb60: 636f 7272 6573 706f 6e64 2074 6f20 7468  correspond to th
+0001fb70: 6520 726f 7773 206f 6620 7468 6520 224d  e rows of the "M
+0001fb80: 5547 3122 206d 6174 7269 780a 2020 2020  UG1" matrix.    
+0001fb90: 696e 2074 6865 202e 6f70 3420 6669 6c65  in the .op4 file
+0001fba0: 2e20 5468 6174 206d 6174 7269 7820 6361  . That matrix ca
+0001fbb0: 6e20 6265 2072 6561 6420 6279 2074 6865  n be read by the
+0001fbc0: 0a20 2020 203a 6d6f 643a 6070 7979 6574  .    :mod:`pyyet
+0001fbd0: 692e 6e61 7374 7261 6e2e 6f70 3460 206d  i.nastran.op4` m
+0001fbe0: 6f64 756c 652e 0a0a 2020 2020 4578 616d  odule...    Exam
+0001fbf0: 706c 6520 7573 6167 653a 3a0a 0a20 2020  ple usage::..   
+0001fc00: 2020 2020 2023 2072 6561 6420 6d75 6731       # read mug1
+0001fc10: 2061 6e64 2074 7567 3120 2863 7265 6174   and tug1 (creat
+0001fc20: 6564 2066 726f 6d20 4558 5453 454f 5554  ed from EXTSEOUT
+0001fc30: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
+0001fc40: 7079 7965 7469 2069 6d70 6f72 7420 6e61  pyyeti import na
+0001fc50: 7374 7261 6e0a 2020 2020 2020 2020 6672  stran.        fr
+0001fc60: 6f6d 2070 7979 6574 692e 6e61 7374 7261  om pyyeti.nastra
+0001fc70: 6e20 696d 706f 7274 206f 7034 0a20 2020  n import op4.   
+0001fc80: 2020 2020 206d 7567 3120 3d20 6f70 342e       mug1 = op4.
+0001fc90: 7265 6164 2827 6461 7461 2e6f 7034 272c  read('data.op4',
+0001fca0: 2027 6d75 6731 2729 5b27 6d75 6731 275d   'mug1')['mug1']
+0001fcb0: 0a20 2020 2020 2020 2074 7567 3120 3d20  .        tug1 = 
+0001fcc0: 6e61 7374 7261 6e2e 7264 6474 6970 6368  nastran.rddtipch
+0001fcd0: 2827 6461 7461 2e70 6368 2729 0a0a 2020  ('data.pch')..  
+0001fce0: 2020 2020 2020 2320 666f 726d 2044 524d        # form DRM
+0001fcf0: 2074 6f20 7265 636f 7665 7279 2067 7269   to recovery gri
+0001fd00: 6420 3130 302c 2064 6f66 2034 3a0a 2020  d 100, dof 4:.  
+0001fd10: 2020 2020 2020 6672 6f6d 2070 7979 6574        from pyyet
+0001fd20: 6920 696d 706f 7274 206c 6f63 6174 650a  i import locate.
+0001fd30: 2020 2020 2020 2020 726f 7720 3d20 6c6f          row = lo
+0001fd40: 6361 7465 2e66 696e 645f 726f 7773 2874  cate.find_rows(t
+0001fd50: 7567 312c 205b 3130 302c 2034 5d29 0a20  ug1, [100, 4]). 
+0001fd60: 2020 2020 2020 2064 726d 203d 206d 7567         drm = mug
+0001fd70: 315b 726f 772c 203a 5d0a 2020 2020 2222  1[row, :].    ""
+0001fd80: 220a 2020 2020 7374 7269 6e67 203d 2066  ".    string = f
+0001fd90: 2244 5449 2020 2020 207b 6e61 6d65 3a3c  "DTI     {name:<
+0001fda0: 3873 7d32 220a 2020 2020 6320 3d20 7264  8s}2".    c = rd
+0001fdb0: 6361 7264 7328 662c 2073 7472 696e 6729  cards(f, string)
+0001fdc0: 0a20 2020 2063 203d 2063 5b30 2c20 3136  .    c = c[0, 16
+0001fdd0: 3a2d 315d 2e72 6573 6861 7065 282d 312c  :-1].reshape(-1,
+0001fde0: 2034 292e 6173 7479 7065 286e 702e 696e   4).astype(np.in
+0001fdf0: 7436 3429 0a20 2020 206d 203d 2063 5b3a  t64).    m = c[:
+0001fe00: 2c20 313a 5d0a 0a20 2020 2023 2061 7272  , 1:]..    # arr
+0001fe10: 6179 285b 5b20 2020 2020 2033 2c20 2020  ay([[      3,   
+0001fe20: 2020 2020 362c 2020 2020 2020 2031 5d2c      6,       1],
+0001fe30: 0a20 2020 2023 2020 2020 2020 2020 5b20  .    #        [ 
+0001fe40: 2020 2020 3131 2c20 2020 2020 2020 362c      11,       6,
+0001fe50: 2020 2020 2020 2037 5d2c 0a20 2020 2023         7],.    #
+0001fe60: 2020 2020 2020 2020 5b20 2020 2020 3139          [     19
+0001fe70: 2c20 2020 2020 2020 362c 2020 2020 2020  ,       6,      
+0001fe80: 3133 5d2c 0a20 2020 2023 2020 2020 2020  13],.    #      
+0001fe90: 2020 5b20 2020 2020 3237 2c20 2020 2020    [     27,     
+0001fea0: 2020 362c 2020 2020 2020 3139 5d2c 0a20    6,      19],. 
+0001feb0: 2020 2023 2020 2020 2020 2020 5b20 2020     #        [   
+0001fec0: 2020 3435 2c20 2020 2020 2020 362c 2020    45,       6,  
+0001fed0: 2020 2020 3235 5d2c 0a20 2020 2023 2020      25],.    #  
+0001fee0: 2020 2020 2020 5b20 2020 2020 3630 2c20        [     60, 
+0001fef0: 2020 2020 2020 362c 2020 2020 2020 3331        6,      31
+0001ff00: 5d2c 0a20 2020 2023 2020 2020 2020 2020  ],.    #        
+0001ff10: 5b31 3939 3530 3032 2c20 2020 2020 2020  [1995002,       
+0001ff20: 362c 2020 2020 2020 3337 5d5d 290a 0a20  6,      37]]).. 
+0001ff30: 2020 2069 6620 6e70 2e61 6c6c 286d 5b3a     if np.all(m[:
+0001ff40: 2c20 315d 203d 3d20 6d5b 302c 2031 5d29  , 1] == m[0, 1])
+0001ff50: 3a0a 2020 2020 2020 2020 2320 616c 6c20  :.        # all 
+0001ff60: 6964 7320 6861 7665 2073 616d 6520 6e75  ids have same nu
+0001ff70: 6d62 6572 206f 6620 636f 6d70 6f6e 656e  mber of componen
+0001ff80: 7473 2c20 736f 2074 616b 6520 7368 6f72  ts, so take shor
+0001ff90: 7463 7574 3a0a 2020 2020 2020 2020 6320  tcut:.        c 
+0001ffa0: 3d20 6d5b 302c 2031 5d0a 2020 2020 2020  = m[0, 1].      
+0001ffb0: 2020 6964 7320 3d20 6e70 2e64 6f74 286d    ids = np.dot(m
+0001ffc0: 5b3a 2c20 303a 315d 2c20 6e70 2e6f 6e65  [:, 0:1], np.one
+0001ffd0: 7328 2831 2c20 6329 2c20 6e70 2e69 6e74  s((1, c), np.int
+0001ffe0: 3634 2929 0a20 2020 2020 2020 2069 6473  64)).        ids
+0001fff0: 203d 2069 6473 2e72 6573 6861 7065 2828   = ids.reshape((
+00020000: 2d31 2c20 3129 290a 2020 2020 2020 2020  -1, 1)).        
+00020010: 646f 6620 3d20 6e70 2e61 7261 6e67 6528  dof = np.arange(
+00020020: 312c 2063 202b 2031 2c20 6474 7970 653d  1, c + 1, dtype=
+00020030: 6e70 2e69 6e74 3634 292e 7265 7368 6170  np.int64).reshap
+00020040: 6528 312c 202d 3129 0a20 2020 2020 2020  e(1, -1).       
+00020050: 2064 6f66 7320 3d20 6e70 2e64 6f74 286e   dofs = np.dot(n
+00020060: 702e 6f6e 6573 2828 6e70 2e73 697a 6528  p.ones((np.size(
+00020070: 6d2c 2030 292c 2031 292c 206e 702e 696e  m, 0), 1), np.in
+00020080: 7436 3429 2c20 646f 6629 0a20 2020 2020  t64), dof).     
+00020090: 2020 2064 6f66 7320 3d20 646f 6673 2e72     dofs = dofs.r
+000200a0: 6573 6861 7065 2828 2d31 2c20 3129 290a  eshape((-1, 1)).
+000200b0: 2020 2020 2020 2020 6964 646f 6620 3d20          iddof = 
+000200c0: 6e70 2e68 7374 6163 6b28 2869 6473 2c20  np.hstack((ids, 
+000200d0: 646f 6673 2929 0a20 2020 2065 6c73 653a  dofs)).    else:
+000200e0: 0a20 2020 2020 2020 206e 726f 7773 203d  .        nrows =
+000200f0: 206d 5b2d 312c 2032 5d20 2b20 6d5b 2d31   m[-1, 2] + m[-1
+00020100: 2c20 315d 202d 2031 0a20 2020 2020 2020  , 1] - 1.       
+00020110: 2069 6464 6f66 203d 206e 702e 7a65 726f   iddof = np.zero
+00020120: 7328 286e 726f 7773 2c20 3229 2c20 6e70  s((nrows, 2), np
+00020130: 2e69 6e74 3634 290a 2020 2020 2020 2020  .int64).        
+00020140: 6a20 3d20 300a 2020 2020 2020 2020 666f  j = 0.        fo
+00020150: 7220 4a20 696e 2072 616e 6765 286e 702e  r J in range(np.
+00020160: 7369 7a65 286d 2c20 3029 293a 0a20 2020  size(m, 0)):.   
+00020170: 2020 2020 2020 2020 2070 7620 3d20 6e70           pv = np
+00020180: 2e61 7261 6e67 6528 302c 206d 5b4a 2c20  .arange(0, m[J, 
+00020190: 315d 2c20 6474 7970 653d 6e70 2e69 6e74  1], dtype=np.int
+000201a0: 3634 290a 2020 2020 2020 2020 2020 2020  64).            
+000201b0: 6964 646f 665b 7076 202b 206a 2c20 305d  iddof[pv + j, 0]
+000201c0: 203d 206d 5b4a 2c20 305d 0a20 2020 2020   = m[J, 0].     
+000201d0: 2020 2020 2020 2069 6464 6f66 5b70 7620         iddof[pv 
+000201e0: 2b20 6a2c 2031 5d20 3d20 7076 202b 2031  + j, 1] = pv + 1
+000201f0: 0a20 2020 2020 2020 2020 2020 206a 202b  .            j +
+00020200: 3d20 6d5b 4a2c 2031 5d0a 2020 2020 7265  = m[J, 1].    re
+00020210: 7475 726e 2069 6464 6f66 0a              turn iddof.
```

### Comparing `pyyeti-1.2.4/pyyeti/nastran/n2p.py` & `pyyeti-1.2.5/pyyeti/nastran/n2p.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/nastran/op2.py` & `pyyeti-1.2.5/pyyeti/nastran/op2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/nastran/op4.py` & `pyyeti-1.2.5/pyyeti/nastran/op4.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/__init__.py` & `pyyeti-1.2.5/pyyeti/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/_base_ode_class.py` & `pyyeti-1.2.5/pyyeti/ode/_base_ode_class.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/_utilities.py` & `pyyeti-1.2.5/pyyeti/ode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/freqdirect.py` & `pyyeti-1.2.5/pyyeti/ode/freqdirect.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/frf_mode_participation.py` & `pyyeti-1.2.5/pyyeti/ode/frf_mode_participation.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/solvecdf.py` & `pyyeti-1.2.5/pyyeti/ode/solvecdf.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/solveexp1.py` & `pyyeti-1.2.5/pyyeti/ode/solveexp1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/solveexp2.py` & `pyyeti-1.2.5/pyyeti/ode/solveexp2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/solvenewmark.py` & `pyyeti-1.2.5/pyyeti/ode/solvenewmark.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ode/solveunc.py` & `pyyeti-1.2.5/pyyeti/ode/solveunc.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/pp.py` & `pyyeti-1.2.5/pyyeti/pp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/psd.py` & `pyyeti-1.2.5/pyyeti/psd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/rainflow/c_rain.c` & `pyyeti-1.2.5/pyyeti/rainflow/c_rain.c`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/rainflow/py_rain.py` & `pyyeti-1.2.5/pyyeti/rainflow/py_rain.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/srs.py` & `pyyeti-1.2.5/pyyeti/srs.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ssmodel.py` & `pyyeti-1.2.5/pyyeti/ssmodel.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/stats.py` & `pyyeti-1.2.5/pyyeti/stats.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/writer.py` & `pyyeti-1.2.5/pyyeti/writer.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti/ytools.py` & `pyyeti-1.2.5/pyyeti/ytools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/pyyeti.egg-info/PKG-INFO` & `pyyeti-1.2.5/pyyeti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.2.4
+Version: 1.2.5
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.2.4 Summary: Tools mostly related
+Metadata-Version: 2.1 Name: pyyeti Version: 1.2.5 Summary: Tools mostly related
 to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
 Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: C
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `pyyeti-1.2.4/pyyeti.egg-info/SOURCES.txt` & `pyyeti-1.2.5/pyyeti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/scripts/lsop2` & `pyyeti-1.2.5/scripts/lsop2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/setup.py` & `pyyeti-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         )
     else:
         kw = {}
 
     install_requires = check_dependencies()
     setup(
         name="pyyeti",
-        version="1.2.4",
+        version="1.2.5",
         url="http://github.com/twmacro/pyyeti/",
         license="BSD",
         author="Tim Widrick",
         install_requires=install_requires,
         author_email="twmacro@gmail.com",
         description=("Tools mostly related to structural dynamics"),
         long_description=long_description,
```

### Comparing `pyyeti-1.2.4/tests/nas2cam_csuper/inboard.asm` & `pyyeti-1.2.5/tests/nas2cam_csuper/inboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nas2cam_csuper/inboard.op4` & `pyyeti-1.2.5/tests/nas2cam_csuper/inboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nas2cam_csuper/inboard.pch` & `pyyeti-1.2.5/tests/nas2cam_csuper/inboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nas2cam_csuper/nas2cam.op2` & `pyyeti-1.2.5/tests/nas2cam_csuper/nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nas2cam_csuper/nas2cam.op4` & `pyyeti-1.2.5/tests/nas2cam_csuper/nas2cam.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nastran_drm12/drm12.op2` & `pyyeti-1.2.5/tests/nastran_drm12/drm12.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nastran_drm12/drm12.op4` & `pyyeti-1.2.5/tests/nastran_drm12/drm12.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nastran_drm12/inboard_nas2cam.op2` & `pyyeti-1.2.5/tests/nastran_drm12/inboard_nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.4/tests/nastran_drm12/inboard_nas2cam.op4` & `pyyeti-1.2.5/tests/nastran_drm12/inboard_nas2cam.op4`

 * *Files identical despite different names*

