# Comparing `tmp/fio-plot-1.1.5.tar.gz` & `tmp/fio-plot-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio-plot-1.1.5.tar", last modified: Wed Apr 12 15:36:00 2023, max compression
+gzip compressed data, was "fio-plot-1.1.6.tar", last modified: Fri Apr 14 22:50:05 2023, max compression
```

## Comparing `fio-plot-1.1.5.tar` & `fio-plot-1.1.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.925628 fio-plot-1.1.5/
--rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.5/CHANGELOG.md
--rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.5/LICENSE
--rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.5/MANIFEST.in
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-12 15:36:00.925173 fio-plot-1.1.5/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-03-27 19:45:08.000000 fio-plot-1.1.5/README.md
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.873721 fio-plot-1.1.5/bench_fio/
--rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.881437 fio-plot-1.1.5/bench_fio/benchlib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/benchlib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    10583 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/checks.py
--rw-r--r--   0 nan03      (501) staff       (20)     2916 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     3295 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/display.py
--rw-r--r--   0 nan03      (501) staff       (20)     2338 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/generatefio.py
--rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/network.py
--rw-r--r--   0 nan03      (501) staff       (20)     1697 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/parseini.py
--rw-r--r--   0 nan03      (501) staff       (20)     6051 2023-04-10 23:24:41.000000 fio-plot-1.1.5/bench_fio/benchlib/runfio.py
--rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/supporting.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.882905 fio-plot-1.1.5/bench_fio/scripts/
--rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/scripts/bench-fio.sh
--rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/scripts/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.883790 fio-plot-1.1.5/bench_fio/templates/
--rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/templates/precondition.fio
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.886794 fio-plot-1.1.5/bin/
--rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bin/bench-fio
--rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bin/fio-plot
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.902758 fio-plot-1.1.5/docs/
--rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.5/docs/bench_fio_call_graph.png
--rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.5/docs/fio_plot_call_graph.png
--rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.5/docs/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.907239 fio-plot-1.1.5/fio_plot/
--rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.5/fio_plot/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.923275 fio-plot-1.1.5/fio_plot/fiolib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.5/fio_plot/fiolib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    11216 2023-04-12 15:29:01.000000 fio-plot-1.1.5/fio_plot/fiolib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     7815 2023-04-12 15:19:04.000000 fio-plot-1.1.5/fio_plot/fiolib/bar2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-04-12 15:00:11.000000 fio-plot-1.1.5/fio_plot/fiolib/bar3d.py
--rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/barhistogram.py
--rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/dataimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/dataimport_support.py
--rw-r--r--   0 nan03      (501) staff       (20)      781 2023-04-12 15:29:38.000000 fio-plot-1.1.5/fio_plot/fiolib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.5/fio_plot/fiolib/flightchecks.py
--rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/getdata.py
--rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/graph2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6278 2023-04-12 15:26:01.000000 fio-plot-1.1.5/fio_plot/fiolib/graph2dsupporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     2349 2023-04-12 15:30:20.000000 fio-plot-1.1.5/fio_plot/fiolib/iniparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-04-10 22:59:44.000000 fio-plot-1.1.5/fio_plot/fiolib/jsonimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     3265 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/jsonparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     5348 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/jsonparsing_support.py
--rw-r--r--   0 nan03      (501) staff       (20)    14738 2023-03-31 17:52:35.000000 fio-plot-1.1.5/fio_plot/fiolib/shared_chart.py
--rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-04-10 22:59:44.000000 fio-plot-1.1.5/fio_plot/fiolib/supporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     4021 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/table_support.py
--rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/tables.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.910659 fio-plot-1.1.5/fio_plot.egg-info/
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/SOURCES.txt
--rw-r--r--   0 nan03      (501) staff       (20)        1 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/dependency_links.txt
--rw-r--r--   0 nan03      (501) staff       (20)       70 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/entry_points.txt
--rw-r--r--   0 nan03      (501) staff       (20)       40 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/requires.txt
--rw-r--r--   0 nan03      (501) staff       (20)       19 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/top_level.txt
--rw-r--r--   0 nan03      (501) staff       (20)       38 2023-04-12 15:36:00.925722 fio-plot-1.1.5/setup.cfg
--rw-r--r--   0 nan03      (501) staff       (20)      909 2023-04-12 15:30:52.000000 fio-plot-1.1.5/setup.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.924396 fio-plot-1.1.5/tests/
--rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.5/tests/bench_fio_test.py
--rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.5/tests/test_3d.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.178011 fio-plot-1.1.6/
+-rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.6/CHANGELOG.md
+-rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.6/LICENSE
+-rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.6/MANIFEST.in
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-14 22:50:05.177539 fio-plot-1.1.6/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-03-27 19:45:08.000000 fio-plot-1.1.6/README.md
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.121284 fio-plot-1.1.6/bench_fio/
+-rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.128845 fio-plot-1.1.6/bench_fio/benchlib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/benchlib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10583 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/checks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2916 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3295 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/display.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2338 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/generatefio.py
+-rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/network.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1697 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/parseini.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6051 2023-04-10 23:24:41.000000 fio-plot-1.1.6/bench_fio/benchlib/runfio.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/supporting.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.130188 fio-plot-1.1.6/bench_fio/scripts/
+-rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/scripts/bench-fio.sh
+-rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/scripts/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.130941 fio-plot-1.1.6/bench_fio/templates/
+-rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/templates/precondition.fio
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.132554 fio-plot-1.1.6/bin/
+-rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bin/bench-fio
+-rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bin/fio-plot
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.148867 fio-plot-1.1.6/docs/
+-rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.6/docs/bench_fio_call_graph.png
+-rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.6/docs/fio_plot_call_graph.png
+-rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.6/docs/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.153430 fio-plot-1.1.6/fio_plot/
+-rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.6/fio_plot/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.173887 fio-plot-1.1.6/fio_plot/fiolib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.6/fio_plot/fiolib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    11216 2023-04-13 16:36:30.000000 fio-plot-1.1.6/fio_plot/fiolib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     7815 2023-04-13 14:07:16.000000 fio-plot-1.1.6/fio_plot/fiolib/bar2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-04-12 15:00:11.000000 fio-plot-1.1.6/fio_plot/fiolib/bar3d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-04-10 22:59:50.000000 fio-plot-1.1.6/fio_plot/fiolib/barhistogram.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/dataimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/dataimport_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)      781 2023-04-12 15:29:38.000000 fio-plot-1.1.6/fio_plot/fiolib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.6/fio_plot/fiolib/flightchecks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/getdata.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-04-13 16:47:00.000000 fio-plot-1.1.6/fio_plot/fiolib/graph2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6947 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/graph2dsupporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2349 2023-04-13 16:36:48.000000 fio-plot-1.1.6/fio_plot/fiolib/iniparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-04-10 22:59:44.000000 fio-plot-1.1.6/fio_plot/fiolib/jsonimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3275 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/jsonparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6298 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/jsonparsing_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)    14737 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/shared_chart.py
+-rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-04-13 15:02:14.000000 fio-plot-1.1.6/fio_plot/fiolib/supporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4018 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/table_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/tables.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.157043 fio-plot-1.1.6/fio_plot.egg-info/
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 nan03      (501) staff       (20)        1 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       70 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/entry_points.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       40 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/requires.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       19 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/top_level.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       38 2023-04-14 22:50:05.178103 fio-plot-1.1.6/setup.cfg
+-rw-r--r--   0 nan03      (501) staff       (20)      909 2023-04-14 22:48:06.000000 fio-plot-1.1.6/setup.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.175636 fio-plot-1.1.6/tests/
+-rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.6/tests/bench_fio_test.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.6/tests/test_3d.py
```

### Comparing `fio-plot-1.1.5/CHANGELOG.md` & `fio-plot-1.1.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/LICENSE` & `fio-plot-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/PKG-INFO` & `fio-plot-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.5
+Version: 1.1.6
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.5/README.md` & `fio-plot-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/__init__.py` & `fio-plot-1.1.6/bench_fio/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/argparsing.py` & `fio-plot-1.1.6/bench_fio/benchlib/argparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/checks.py` & `fio-plot-1.1.6/bench_fio/benchlib/checks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/defaultsettings.py` & `fio-plot-1.1.6/bench_fio/benchlib/defaultsettings.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/display.py` & `fio-plot-1.1.6/bench_fio/benchlib/display.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/generatefio.py` & `fio-plot-1.1.6/bench_fio/benchlib/generatefio.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/network.py` & `fio-plot-1.1.6/bench_fio/benchlib/network.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/parseini.py` & `fio-plot-1.1.6/bench_fio/benchlib/parseini.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/runfio.py` & `fio-plot-1.1.6/bench_fio/benchlib/runfio.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/benchlib/supporting.py` & `fio-plot-1.1.6/bench_fio/benchlib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/bench_fio/scripts/bench-fio.sh` & `fio-plot-1.1.6/bench_fio/scripts/bench-fio.sh`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/docs/bench_fio_call_graph.png` & `fio-plot-1.1.6/docs/bench_fio_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/docs/fio_plot_call_graph.png` & `fio-plot-1.1.6/docs/fio_plot_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/__init__.py` & `fio-plot-1.1.6/fio_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/argparsing.py` & `fio-plot-1.1.6/fio_plot/fiolib/argparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/bar2d.py` & `fio-plot-1.1.6/fio_plot/fiolib/bar2d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/bar3d.py` & `fio-plot-1.1.6/fio_plot/fiolib/bar3d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/barhistogram.py` & `fio-plot-1.1.6/fio_plot/fiolib/barhistogram.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/dataimport.py` & `fio-plot-1.1.6/fio_plot/fiolib/dataimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/dataimport_support.py` & `fio-plot-1.1.6/fio_plot/fiolib/dataimport_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/defaultsettings.py` & `fio-plot-1.1.6/fio_plot/fiolib/defaultsettings.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/flightchecks.py` & `fio-plot-1.1.6/fio_plot/fiolib/flightchecks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/getdata.py` & `fio-plot-1.1.6/fio_plot/fiolib/getdata.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/graph2d.py` & `fio-plot-1.1.6/fio_plot/fiolib/graph2d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/graph2dsupporting.py` & `fio-plot-1.1.6/fio_plot/fiolib/graph2dsupporting.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,28 +17,41 @@
         dataset = jsonimport.import_json_dataset(settings, list_of_json_files)
         parsed_data = jsonparsing.parse_json_data(settings, dataset)
         return parsed_data
     else:
         return None
 
 
-def create_label(item):
+def create_label(settings, item):
+    """
+    The label must be unique. With client/server data, when using
+    multiple source folders, the labels may not be unique by default.
+    """
     if item["hostname"]:
-        mydir = item["hostname"]
+        if len(settings["input_directory"]) > 1 and \
+        (settings["xlabel_parent"] == 1 and settings["xlabel_depth"] == 0):
+            print("WARNING: legend labels are not unique per input directory, use --xlabel-parent and --xlabel-depth to ajust.")
+
+        if len(settings["input_directory"]) > 1 and \
+            (settings["xlabel_parent"] != 1 \
+            or settings["xlabel_depth"] != 0):
+            mydir = f"{item['directory']}-{item['hostname']}"
+        else:
+            mydir = item["hostname"]
     else:
         mydir = f"{item['directory']}"
     return mydir
 
 
 def get_max_label_size(settings, data):
     labels = []
     for item in data["dataset"]:
         for rw in settings["filter"]:
             if rw in item.keys():
-                label = create_label(item)
+                label = create_label(settings, item)
                 labels.append(label)
 
     maxlabelsize = 0
     for label in labels:
         size = len(label)
         if size > maxlabelsize:
             maxlabelsize = size
@@ -154,15 +167,15 @@
     #
     supportdata["lines"].append(axes[dataplot])
     create_single_label(settings, item, rw, supportdata)
 
 
 def create_single_label(settings, item, rw, supportdata):
     # print(maxlabelsize)
-    mylabel = create_label(item)
+    mylabel = create_label(settings, item)
     mylabel = get_padding(mylabel, supportdata["maxlabelsize"])
     labelset = {
         "name": mylabel,
         "rw": rw,
         "type": item["type"],
         "qd": item["iodepth"],
         "nj": item["numjobs"],
```

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/iniparsing.py` & `fio-plot-1.1.6/fio_plot/fiolib/iniparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/jsonimport.py` & `fio-plot-1.1.6/fio_plot/fiolib/jsonimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/jsonparsing.py` & `fio-plot-1.1.6/fio_plot/fiolib/jsonparsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         row = jsonsupport.return_data_row(settings, job)  
         row["fio_version"] = record["fio version"]
         if hosts:
             hosts[hostname].append(row)
         else:
             jobs.append(row)
           
-    directory["data"].extend(jsonsupport.merge_job_data_hosts_jobs(hosts, jobs))
+    directory["data"].extend(jsonsupport.merge_job_data_hosts_jobs(settings, hosts, jobs))
 
     
 def parse_json_data(settings, dataset):
     """
     This funcion traverses the relevant JSON structure to gather data
     and store it in a flat dictionary. We do this for each imported json file.
     """
```

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/shared_chart.py` & `fio-plot-1.1.6/fio_plot/fiolib/shared_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         for data in dataset:
             # pprint.pprint(data.keys())
             # pprint.pprint(data['directory'])
             for record in data["data"]:
                 #pprint.pprint(record.keys())
                 #pprint.pprint(f"-> {record['type']}")
                 #print(f"{depth} - {record['iodepth']} + {numjobs} - {record['numjobs']} + {record['rw']} + {record['type']}")
-                #print(f"{settings['filter']}") 
+                #print(f"{settings['filter']}")
                 if (
                     (int(record["iodepth"]) == int(depth))
                     and int(record["numjobs"]) == int(numjobs)
                     and record["rw"] == rw
                     and record["type"] in settings["filter"]
                 ):
                     datadict["fio_version"].append(record["fio_version"])
```

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/supporting.py` & `fio-plot-1.1.6/fio_plot/fiolib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/table_support.py` & `fio-plot-1.1.6/fio_plot/fiolib/table_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             scale = round((x/1000000),1)
             scaled.append(f"{scale}M")
         else:
             scaled.append(str(x))
     return scaled
 
 
-def alternate_cell_height(number=2,stepsize=14):
+def alternate_cell_height(number=2,stepsize=2):
     start = 5
     stop = start + (number * stepsize)
     while True:
         for x in range(start, stop, stepsize):
             yield x / 10
 
 
@@ -96,15 +96,15 @@
         alpha = 0
         linewidth = 0
     return linewidth, alpha
 
 def get_alternator_value(matrix):
     if max(matrix) <= 10:
         alternator = alternate_cell_height()
-    elif max(matrix) > 10:
+    if max(matrix) > 10:
         alternator = alternate_cell_height(3,14)
     else:
         alternator = alternate_cell_height(1,10)
     return alternator
 
 def format_table_cells(settings, table, fontsize, matrix, cols):
     linewidth, alpha = tablelines(settings)
```

### Comparing `fio-plot-1.1.5/fio_plot/fiolib/tables.py` & `fio-plot-1.1.6/fio_plot/fiolib/tables.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/fio_plot.egg-info/PKG-INFO` & `fio-plot-1.1.6/fio_plot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.5
+Version: 1.1.6
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.5/fio_plot.egg-info/SOURCES.txt` & `fio-plot-1.1.6/fio_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/setup.py` & `fio-plot-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name="fio-plot",
-        version="1.1.5",
+        version="1.1.6",
         author="louwrentius",
         description="Create charts from FIO storage benchmark tool output",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/louwrentius/fio-plot/", 
         packages=setuptools.find_packages(),
         install_requires=['numpy','matplotlib','Pillow', 'pyan3', 'pyparsing'],
```

### Comparing `fio-plot-1.1.5/tests/bench_fio_test.py` & `fio-plot-1.1.6/tests/bench_fio_test.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.5/tests/test_3d.py` & `fio-plot-1.1.6/tests/test_3d.py`

 * *Files identical despite different names*

