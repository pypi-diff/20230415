# Comparing `tmp/gwemopt-0.0.80.tar.gz` & `tmp/gwemopt-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwemopt-0.0.80.tar", last modified: Sat Mar  4 18:31:10 2023, max compression
+gzip compressed data, was "gwemopt-0.0.81.tar", last modified: Sat Apr 15 17:06:05 2023, max compression
```

## Comparing `gwemopt-0.0.80.tar` & `gwemopt-0.0.81.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-03-04 18:31:10.879682 gwemopt-0.0.80/
--rw-r--r--   0 mcoughlin   (501) staff       (20)    35147 2023-03-04 18:28:52.000000 gwemopt-0.0.80/LICENSE
--rw-r--r--   0 mcoughlin   (501) staff       (20)       50 2023-03-04 18:28:52.000000 gwemopt-0.0.80/MANIFEST.in
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1158 2023-03-04 18:31:10.879753 gwemopt-0.0.80/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1741 2023-03-04 18:28:52.000000 gwemopt-0.0.80/README.md
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-03-04 18:31:10.874187 gwemopt-0.0.80/bin/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6086 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/condor_gwemopt_run.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6184 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/efficiency_gwemopt_run.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13658 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_check_coverage
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1942 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_check_ref
--rw-r--r--   0 mcoughlin   (501) staff       (20)     7422 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_compute_overlap
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4669 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_crossmatch_catalog
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1503 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_download_ref
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1397 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_gen_queue
--rw-r--r--   0 mcoughlin   (501) staff       (20)    14662 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_gen_skymap
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3621 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_json_overlap
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5260 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_plot_coverage_hist
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5049 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_plot_coverage_int
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6714 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_plot_ref
--rw-r--r--   0 mcoughlin   (501) staff       (20)    15337 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_plot_skymap
--rw-r--r--   0 mcoughlin   (501) staff       (20)    28816 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_run
--rw-r--r--   0 mcoughlin   (501) staff       (20)    41793 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_serendipitous_schedule
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3819 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/gwemopt_skyvision_to_list
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2434 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/plot_telescope_comparison_S200115j.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2422 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/plot_telescope_comparison_S200213t.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1561 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_O2
--rw-r--r--   0 mcoughlin   (501) staff       (20)    14696 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gracedb.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1023 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_GBM
--rw-r--r--   0 mcoughlin   (501) staff       (20)      665 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_GRB180523
--rw-r--r--   0 mcoughlin   (501) staff       (20)      798 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_GRB180626
--rw-r--r--   0 mcoughlin   (501) staff       (20)      666 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_GRB180715
--rw-r--r--   0 mcoughlin   (501) staff       (20)      807 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_GRB180728
--rw-r--r--   0 mcoughlin   (501) staff       (20)      430 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_TESS
--rw-r--r--   0 mcoughlin   (501) staff       (20)      727 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_run
--rw-r--r--   0 mcoughlin   (501) staff       (20)      359 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_run.pbs
--rw-r--r--   0 mcoughlin   (501) staff       (20)    17679 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_gwemopt_superscheduler
--rw-r--r--   0 mcoughlin   (501) staff       (20)    26105 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_skymaps.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    10081 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/run_skymaps_pproc.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2102 2023-03-04 18:28:53.000000 gwemopt-0.0.80/bin/slice_catalog.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-03-04 18:31:10.880232 gwemopt-0.0.80/gwemopt/
--rw-r--r--   0 mcoughlin   (501) staff       (20)      948 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)      498 2023-03-04 18:31:10.880267 gwemopt-0.0.80/gwemopt/_version.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    20739 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/catalog.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    35715 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/coverage.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13375 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/decam_tiling.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     9242 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/efficiency.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1566 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/flaskapp.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)      899 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/footprint.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1396 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/gracedb.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6490 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/lightcurve.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2685 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/mapsplit.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6093 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/moc.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2068 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/models.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    22116 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/pem.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    36994 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/plotting.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13976 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/quadrants.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    34491 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/rankedTilesGenerator.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12347 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/samplers.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    41865 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/scheduler.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    17763 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/segments.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12339 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/segments_astroplan.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12757 2023-03-04 18:29:50.000000 gwemopt-0.0.80/gwemopt/skyportal.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-03-04 18:31:10.879297 gwemopt-0.0.80/gwemopt/tests/
--rw-r--r--   0 mcoughlin   (501) staff       (20)        0 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/tests/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    10001 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/tests/test_schedule.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    29039 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/tiles.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4540 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/transients.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    53758 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/utils.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    16420 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/waw.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3751 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/ztf_coverage.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12447 2023-03-04 18:28:53.000000 gwemopt-0.0.80/gwemopt/ztf_tiling.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-03-04 18:31:10.879039 gwemopt-0.0.80/gwemopt.egg-info/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1158 2023-03-04 18:31:10.000000 gwemopt-0.0.80/gwemopt.egg-info/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1730 2023-03-04 18:31:10.000000 gwemopt-0.0.80/gwemopt.egg-info/SOURCES.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2023-03-04 18:31:10.000000 gwemopt-0.0.80/gwemopt.egg-info/dependency_links.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)      211 2023-03-04 18:31:10.000000 gwemopt-0.0.80/gwemopt.egg-info/requires.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)       14 2023-03-04 18:31:10.000000 gwemopt-0.0.80/gwemopt.egg-info/top_level.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)      402 2023-03-04 18:31:10.880080 gwemopt-0.0.80/setup.cfg
--rwxr-xr-x   0 mcoughlin   (501) staff       (20)     3791 2023-03-04 18:30:34.000000 gwemopt-0.0.80/setup.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-03-04 18:31:10.879561 gwemopt-0.0.80/utils/
--rw-r--r--   0 mcoughlin   (501) staff       (20)      809 2023-03-04 18:28:54.000000 gwemopt-0.0.80/utils/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6213 2023-03-04 18:28:54.000000 gwemopt-0.0.80/utils/version.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    68611 2023-03-04 18:28:54.000000 gwemopt-0.0.80/versioneer.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.581353 gwemopt-0.0.81/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    35147 2023-02-01 13:42:46.000000 gwemopt-0.0.81/LICENSE
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       50 2023-02-01 13:42:46.000000 gwemopt-0.0.81/MANIFEST.in
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1177 2023-04-15 17:06:05.581431 gwemopt-0.0.81/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1741 2023-02-01 13:42:46.000000 gwemopt-0.0.81/README.md
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.573227 gwemopt-0.0.81/bin/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6086 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/condor_gwemopt_run.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6184 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/efficiency_gwemopt_run.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13658 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_check_coverage
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1942 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_check_ref
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     7422 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_compute_overlap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4669 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_crossmatch_catalog
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1503 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_download_ref
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1397 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_gen_queue
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    14662 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_gen_skymap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     3621 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_json_overlap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5260 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_coverage_hist
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5049 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_coverage_int
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6714 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_ref
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    15337 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_skymap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    28801 2023-04-15 17:05:46.000000 gwemopt-0.0.81/bin/gwemopt_run
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    41793 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_serendipitous_schedule
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     3819 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_skyvision_to_list
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2434 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/plot_telescope_comparison_S200115j.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2422 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/plot_telescope_comparison_S200213t.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1561 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_O2
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    14696 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gracedb.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1023 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GBM
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      665 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180523
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      798 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180626
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      666 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180715
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      807 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180728
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      430 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_TESS
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      727 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_run
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      359 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_run.pbs
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    17679 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_superscheduler
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    26105 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_skymaps.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    10081 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_skymaps_pproc.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2102 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/slice_catalog.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.582189 gwemopt-0.0.81/gwemopt/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      948 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      498 2023-04-15 17:06:05.582231 gwemopt-0.0.81/gwemopt/_version.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    20739 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/catalog.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    35709 2023-04-15 17:05:46.000000 gwemopt-0.0.81/gwemopt/coverage.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13375 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/decam_tiling.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     9242 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/efficiency.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1566 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/flaskapp.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      899 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/footprint.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1396 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/gracedb.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6490 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/lightcurve.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2685 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/mapsplit.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6093 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/moc.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2068 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/models.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    22116 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/pem.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    36994 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/plotting.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13976 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/quadrants.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    34491 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/rankedTilesGenerator.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12347 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/samplers.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    41865 2023-04-15 17:02:35.000000 gwemopt-0.0.81/gwemopt/scheduler.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    17763 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/segments.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12339 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/segments_astroplan.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12739 2023-04-15 17:05:46.000000 gwemopt-0.0.81/gwemopt/skyportal.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.580625 gwemopt-0.0.81/gwemopt/tests/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        0 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/tests/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    10001 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/tests/test_schedule.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    29039 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/tiles.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4540 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/transients.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    53746 2023-04-15 17:05:46.000000 gwemopt-0.0.81/gwemopt/utils.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    16420 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/waw.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     3751 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/ztf_coverage.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12447 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/ztf_tiling.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.580325 gwemopt-0.0.81/gwemopt.egg-info/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1177 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1730 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/SOURCES.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/dependency_links.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      211 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/requires.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       14 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/top_level.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      402 2023-04-15 17:06:05.581967 gwemopt-0.0.81/setup.cfg
+-rwxr-xr-x   0 mcoughlin   (501) staff       (20)     3791 2023-04-15 17:05:46.000000 gwemopt-0.0.81/setup.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.581125 gwemopt-0.0.81/utils/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      809 2023-02-01 13:42:48.000000 gwemopt-0.0.81/utils/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6213 2023-02-01 13:42:48.000000 gwemopt-0.0.81/utils/version.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    68611 2023-02-01 13:42:48.000000 gwemopt-0.0.81/versioneer.py
```

### Comparing `gwemopt-0.0.80/LICENSE` & `gwemopt-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/PKG-INFO` & `gwemopt-0.0.81/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: gwemopt
-Version: 0.0.80
+Version: 0.0.81
 Summary: A python package for GW-EM Followup Optimization
 Home-page: https://github.com/mcoughlin/gwemopt/
 Author: Michael Coughlin
 Author-email: michael.coughlin@ligo.org
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
@@ -23,7 +24,8 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides: gwemopt
 License-File: LICENSE
 
 gwemopt is a python package for GW-EM Followup Optimization 
+
```

### Comparing `gwemopt-0.0.80/README.md` & `gwemopt-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/condor_gwemopt_run.py` & `gwemopt-0.0.81/bin/condor_gwemopt_run.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/efficiency_gwemopt_run.py` & `gwemopt-0.0.81/bin/efficiency_gwemopt_run.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_check_coverage` & `gwemopt-0.0.81/bin/gwemopt_check_coverage`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_check_ref` & `gwemopt-0.0.81/bin/gwemopt_check_ref`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_compute_overlap` & `gwemopt-0.0.81/bin/gwemopt_compute_overlap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_crossmatch_catalog` & `gwemopt-0.0.81/bin/gwemopt_crossmatch_catalog`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_download_ref` & `gwemopt-0.0.81/bin/gwemopt_download_ref`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_gen_queue` & `gwemopt-0.0.81/bin/gwemopt_gen_queue`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_gen_skymap` & `gwemopt-0.0.81/bin/gwemopt_gen_skymap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_json_overlap` & `gwemopt-0.0.81/bin/gwemopt_json_overlap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_plot_coverage_hist` & `gwemopt-0.0.81/bin/gwemopt_plot_coverage_hist`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_plot_coverage_int` & `gwemopt-0.0.81/bin/gwemopt_plot_coverage_int`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_plot_ref` & `gwemopt-0.0.81/bin/gwemopt_plot_ref`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_plot_skymap` & `gwemopt-0.0.81/bin/gwemopt_plot_skymap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_run` & `gwemopt-0.0.81/bin/gwemopt_run`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             if opts.doZTFCoverage and telescope == "ZTF":
                 pass
             else:
                 continue
         params["config"][telescope] = gwemopt.utils.readParamsFromFile(configFile)
         params["config"][telescope]["telescope"] = telescope
         if opts.doSingleExposure:
-            exposuretime = np.array(opts.exposuretimes.split(","),dtype=np.float)[0]
+            exposuretime = np.array(opts.exposuretimes.split(","),dtype=float)[0]
 
             params["config"][telescope]["magnitude_orig"] = params["config"][telescope]["magnitude"]
             params["config"][telescope]["exposuretime_orig"] = params["config"][telescope]["exposuretime"]
 
             nmag = -2.5*np.log10(np.sqrt(params["config"][telescope]["exposuretime"]/exposuretime))
             params["config"][telescope]["magnitude"] = params["config"][telescope]["magnitude"] + nmag
             params["config"][telescope]["exposuretime"] = exposuretime
@@ -319,15 +319,15 @@
     params["timeallocationType"] = opts.timeallocationType
     params["Ninj"] = opts.Ninj
     params["Ndet"] = opts.Ndet
     params["Ntiles"] = opts.Ntiles
     params["Ntiles_cr"] = opts.Ntiles_cr
     params["DScale"] = opts.DScale
     params["nside"] = opts.nside
-    params["Tobs"] = np.array(opts.Tobs.split(","),dtype=np.float)
+    params["Tobs"] = np.array(opts.Tobs.split(","),dtype=float)
     params["powerlaw_cl"] = opts.powerlaw_cl
     params["powerlaw_n"] = opts.powerlaw_n
     params["powerlaw_dist_exp"] = opts.powerlaw_dist_exp
     params["galaxies_FoV_sep"] = opts.galaxies_FoV_sep
     params["observedTiles"] = opts.observedTiles.split(",")
     params["doPlots"] = opts.doPlots
     params["doMovie"] = opts.doMovie
@@ -343,33 +343,33 @@
     params["doCalcTiles"] = opts.doCalcTiles
     params["doFootprint"] = opts.doFootprint
     params["footprint_ra"] = opts.footprint_ra
     params["footprint_dec"] = opts.footprint_dec
     params["footprint_radius"] = opts.footprint_radius
 
     params["doRASlice"] = opts.doRASlice
-    params["raslice"] = np.array(opts.raslice.split(","),dtype=np.float)
+    params["raslice"] = np.array(opts.raslice.split(","),dtype=float)
 
     params["doTransients"] = opts.doTransients
     params["transientsFile"] = opts.transientsFile
     params["transients_to_catalog"] = opts.transients_to_catalog
     params["dt"] = opts.dt
 
     params["galaxy_catalog"] = opts.galaxy_catalog
 
     params["doSingleExposure"] = opts.doSingleExposure
     params["doBalanceExposure"] = opts.doBalanceExposure
     params["unbalanced_tiles"] = None
     params["filters"] = opts.filters.split(",")
-    params["exposuretimes"] = np.array(opts.exposuretimes.split(","),dtype=np.float)
+    params["exposuretimes"] = np.array(opts.exposuretimes.split(","),dtype=float)
     params["doMovie_supersched"] = False
     params["doSuperSched"] = False
     params["doUpdateScheduler"] = False
     params["doMaxTiles"] = opts.doMaxTiles
-    params["max_nb_tiles"] = np.array(opts.max_nb_tiles.split(","),dtype=np.float)
+    params["max_nb_tiles"] = np.array(opts.max_nb_tiles.split(","),dtype=float)
     params["mindiff"] = opts.mindiff
     params["doAlternatingFilters"] = opts.doAlternatingFilters
     params["doReferences"] = opts.doReferences
 
     params["airmass"] = opts.airmass
 
     params["doIterativeTiling"] = opts.doIterativeTiling
```

### Comparing `gwemopt-0.0.80/bin/gwemopt_serendipitous_schedule` & `gwemopt-0.0.81/bin/gwemopt_serendipitous_schedule`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/gwemopt_skyvision_to_list` & `gwemopt-0.0.81/bin/gwemopt_skyvision_to_list`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/plot_telescope_comparison_S200115j.py` & `gwemopt-0.0.81/bin/plot_telescope_comparison_S200115j.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/plot_telescope_comparison_S200213t.py` & `gwemopt-0.0.81/bin/plot_telescope_comparison_S200213t.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_O2` & `gwemopt-0.0.81/bin/run_O2`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gracedb.py` & `gwemopt-0.0.81/bin/run_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gwemopt_GBM` & `gwemopt-0.0.81/bin/run_gwemopt_GBM`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gwemopt_GRB180523` & `gwemopt-0.0.81/bin/run_gwemopt_GRB180523`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gwemopt_GRB180626` & `gwemopt-0.0.81/bin/run_gwemopt_GRB180626`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gwemopt_GRB180715` & `gwemopt-0.0.81/bin/run_gwemopt_GRB180715`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gwemopt_GRB180728` & `gwemopt-0.0.81/bin/run_gwemopt_GRB180728`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gwemopt_run` & `gwemopt-0.0.81/bin/run_gwemopt_run`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_gwemopt_superscheduler` & `gwemopt-0.0.81/bin/run_gwemopt_superscheduler`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_skymaps.py` & `gwemopt-0.0.81/bin/run_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/run_skymaps_pproc.py` & `gwemopt-0.0.81/bin/run_skymaps_pproc.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/bin/slice_catalog.py` & `gwemopt-0.0.81/bin/slice_catalog.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/__init__.py` & `gwemopt-0.0.81/gwemopt/__init__.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/catalog.py` & `gwemopt-0.0.81/gwemopt/catalog.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/coverage.py` & `gwemopt-0.0.81/gwemopt/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
                 coverage_struct = gwemopt.scheduler.schedule_ra_splits(params,config_struct,
                                                                        map_struct_hold,tile_struct,
                                                                        telescope,previous_coverage_struct)
             elif params["doBalanceExposure"]:
                 if not params["doMaxTiles"]: #optimize max tiles (iff max tiles not already specified)
                     optimized_max,coverage_struct,tile_struct = gwemopt.utils.optimize_max_tiles(params,tile_struct,coverage_struct,config_struct,telescope,map_struct_hold)
-                    params["max_nb_tiles"] = np.array([optimized_max],dtype=np.float)
+                    params["max_nb_tiles"] = np.array([optimized_max],dtype=float)
                 else:
                     params_hold = copy.copy(params)
                     config_struct_hold = copy.copy(config_struct)
                     
                     coverage_struct,tile_struct = gwemopt.scheduler.schedule_alternating(params_hold, config_struct_hold, telescope, map_struct_hold, tile_struct,previous_coverage_struct)
                     doReschedule,balanced_fields = gwemopt.utils.balance_tiles(params_hold, tile_struct, coverage_struct)
 
@@ -423,15 +423,15 @@
             if params["doRASlices"]:
                 coverage_struct = gwemopt.scheduler.schedule_ra_splits(params,config_struct,
                                                                        map_struct_hold,tile_struct,
                                                                        telescope,previous_coverage_struct)
             elif params["doBalanceExposure"]:
                 if not params["doMaxTiles"]: #optimize max tiles (iff max tiles not already specified)
                     optimized_max,coverage_struct,tile_struct = gwemopt.utils.optimize_max_tiles(params,tile_struct,coverage_struct,config_struct,telescope,map_struct_hold)
-                    params["max_nb_tiles"] = np.array([optimized_max],dtype=np.float)
+                    params["max_nb_tiles"] = np.array([optimized_max],dtype=float)
 
                 else:
                     params_hold = copy.copy(params)
                     config_struct_hold = copy.copy(config_struct)
 
                     coverage_struct,tile_struct = gwemopt.scheduler.schedule_alternating(params_hold, config_struct_hold, telescope, map_struct_hold, tile_struct,previous_coverage_struct)
                     doReschedule,balanced_fields = gwemopt.utils.balance_tiles(params_hold, tile_struct, coverage_struct)
```

### Comparing `gwemopt-0.0.80/gwemopt/decam_tiling.py` & `gwemopt-0.0.81/gwemopt/decam_tiling.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/efficiency.py` & `gwemopt-0.0.81/gwemopt/efficiency.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/flaskapp.py` & `gwemopt-0.0.81/gwemopt/flaskapp.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/footprint.py` & `gwemopt-0.0.81/gwemopt/footprint.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/gracedb.py` & `gwemopt-0.0.81/gwemopt/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/lightcurve.py` & `gwemopt-0.0.81/gwemopt/lightcurve.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/mapsplit.py` & `gwemopt-0.0.81/gwemopt/mapsplit.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/moc.py` & `gwemopt-0.0.81/gwemopt/moc.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/models.py` & `gwemopt-0.0.81/gwemopt/models.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/pem.py` & `gwemopt-0.0.81/gwemopt/pem.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/plotting.py` & `gwemopt-0.0.81/gwemopt/plotting.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/quadrants.py` & `gwemopt-0.0.81/gwemopt/quadrants.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/rankedTilesGenerator.py` & `gwemopt-0.0.81/gwemopt/rankedTilesGenerator.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/samplers.py` & `gwemopt-0.0.81/gwemopt/samplers.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/scheduler.py` & `gwemopt-0.0.81/gwemopt/scheduler.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/segments.py` & `gwemopt-0.0.81/gwemopt/segments.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/segments_astroplan.py` & `gwemopt-0.0.81/gwemopt/segments_astroplan.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/skyportal.py` & `gwemopt-0.0.81/gwemopt/skyportal.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     else:
         doUseSecondary = False
 
     npix = hp.nside2npix(nside)
     pixarea = hp.nside2pixarea(nside)
 
     theta, phi = hp.pix2ang(nside, np.arange(npix))
-    ra = np.rad2deg(phi)*24.0/360.0
+    ra = np.rad2deg(phi)
     dec = np.rad2deg(0.5*np.pi - theta)
 
     moc_structs = {}
     for telescope in params["telescopes"]:
         config_struct = params["config"][telescope]
         tesselation = config_struct["tesselation"]
         moc_struct = {}
@@ -213,16 +213,17 @@
             if (telescope == "ZTF") and doUseSecondary and (index < 1000):
                 continue
 
             ipix = ipixs[ii]
             if len(ipix) == 0: continue
 
             moc_struct[index] = {}
-            moc_struct[index]["ra"] = np.median(ra[ipix])
-            moc_struct[index]["dec"] = np.median(dec[ipix])
+            moc_struct[index]["ra"] = tess.ra
+            moc_struct[index]["dec"] = tess.dec
+
             moc_struct[index]["ipix"] = ipix
             moc_struct[index]["corners"] = [[np.min(ra[ipix]), np.min(dec[ipix])],
                                             [np.min(ra[ipix]), np.max(dec[ipix])],
                                             [np.max(ra[ipix]), np.max(dec[ipix])],
                                             [np.max(ra[ipix]), np.min(dec[ipix])]]
             moc_struct[index]["patch"] = []
             moc_struct[index]["area"] = len(ipix)*pixarea
@@ -252,14 +253,15 @@
             for ii, key in enumerate(keys):
                 if ii in ipix_keep:
                     moc_struct[key] = moc_struct_new[key]
                     cnt = cnt + 1
 
         moc_structs[telescope] = moc_struct
 
+    print(stop)
     return moc_structs
 
 
 def skyportal2FOV(tess, nside):
 
     moc = moc_from_tiles([tile.healpix for tile in tess.tiles], 2**29)
     pix_id = moc.degrade_to_order(int(np.log2(nside))).flatten()
```

### Comparing `gwemopt-0.0.80/gwemopt/tests/test_schedule.py` & `gwemopt-0.0.81/gwemopt/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/tiles.py` & `gwemopt-0.0.81/gwemopt/tiles.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/transients.py` & `gwemopt-0.0.81/gwemopt/transients.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/utils.py` & `gwemopt-0.0.81/gwemopt/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         configFiles = glob.glob("%s/*.config"%params["configDirectory"])
         for configFile in configFiles:
             telescope = configFile.split("/")[-1].replace(".config","")
             if not telescope in params["telescopes"]: continue
             params["config"][telescope] = gwemopt.utils.readParamsFromFile(configFile)
             params["config"][telescope]["telescope"] = telescope
             if params["doSingleExposure"]:
-                exposuretime = np.array(opts.exposuretimes.split(","),dtype=np.float)[0]
+                exposuretime = np.array(opts.exposuretimes.split(","),dtype=float)[0]
            
                 nmag = -2.5*np.log10(np.sqrt(params["config"][telescope]["exposuretime"]/exposuretime))
                 params["config"][telescope]["magnitude"] = params["config"][telescope]["magnitude"] + nmag
                 params["config"][telescope]["exposuretime"] = exposuretime
             if "tesselationFile" in params["config"][telescope]:
                 if not os.path.isfile(params["config"][telescope]["tesselationFile"]):
                     if params["config"][telescope]["FOV_type"] == "circle":
@@ -1116,15 +1116,15 @@
         max_trials = np.linspace(10,200,20)
 
     for ii,max_trial in enumerate(max_trials):
         for key in tile_struct_hold.keys():
             tile_struct_hold[key]['prob'] = prob[key]
             if "epochs" in tile_struct_hold[key]:
                 tile_struct_hold[key]['epochs'] = np.empty((0,9))
-        params["max_nb_tiles"] = np.array([max_trial],dtype=np.float)
+        params["max_nb_tiles"] = np.array([max_trial],dtype=float)
         params_hold = copy.copy(params)
         config_struct_hold = copy.copy(config_struct)
         coverage_struct_hold,tile_struct_hold = gwemopt.scheduler.schedule_alternating(params_hold, config_struct_hold,
                                                                                   telescope, map_struct_hold, tile_struct_hold)
 
         keys_scheduled = coverage_struct_hold["data"][:,5]
         unique, freq = np.unique(keys_scheduled, return_counts=True)
@@ -1159,15 +1159,15 @@
     repeating = False
     for ii,max_trial in enumerate(max_trials):
         if optimized_max==-1: break #breaks if no max tiles restriction should be imposed
         for key in tile_struct_hold.keys():
             tile_struct_hold[key]['prob'] = prob[key]
             if "epochs" in tile_struct_hold[key]:
                 tile_struct_hold[key]['epochs'] = np.empty((0,9))
-        params["max_nb_tiles"] = np.array([max_trial],dtype=np.float)
+        params["max_nb_tiles"] = np.array([max_trial],dtype=float)
         params_hold = copy.copy(params)
         config_struct_hold = copy.copy(config_struct)
 
         coverage_struct_hold,tile_struct_hold = gwemopt.scheduler.schedule_alternating(params_hold, config_struct_hold,
                                                                                   telescope, map_struct_hold, tile_struct_hold)
 
         keys_scheduled = coverage_struct_hold["data"][:,5]
@@ -1203,15 +1203,15 @@
                 tile_struct_hold[key]['prob'] = prob[key]
                 if "epochs" in tile_struct_hold[key]:
                     tile_struct_hold[key]['epochs'] = np.empty((0,9))
             doReschedule,balanced_fields = balance_tiles(params_hold, opt_tile_struct, opt_coverage_struct)
             params_hold["unbalanced_tiles"] = unbalanced_tiles + params_hold["unbalanced_tiles"]
             if not doReschedule: break
             config_struct_hold = copy.copy(config_struct)
-            params_hold["max_nb_tiles"] = np.array([np.ceil(optimized_max)],dtype=np.float)
+            params_hold["max_nb_tiles"] = np.array([np.ceil(optimized_max)],dtype=float)
             coverage_struct,tile_struct_hold = gwemopt.scheduler.schedule_alternating(params_hold, config_struct_hold, telescope,
                                                                                     map_struct_hold, tile_struct_hold)
             keys_scheduled = coverage_struct["data"][:,5]
             unique, freq = np.unique(keys_scheduled, return_counts=True)
             n_equal = np.sum(freq==len(params["filters"]))
             n_dif = np.sum(freq!=len(params["filters"]))
             n_1 = n_equal
```

### Comparing `gwemopt-0.0.80/gwemopt/waw.py` & `gwemopt-0.0.81/gwemopt/waw.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/ztf_coverage.py` & `gwemopt-0.0.81/gwemopt/ztf_coverage.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt/ztf_tiling.py` & `gwemopt-0.0.81/gwemopt/ztf_tiling.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/gwemopt.egg-info/PKG-INFO` & `gwemopt-0.0.81/gwemopt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: gwemopt
-Version: 0.0.80
+Version: 0.0.81
 Summary: A python package for GW-EM Followup Optimization
 Home-page: https://github.com/mcoughlin/gwemopt/
 Author: Michael Coughlin
 Author-email: michael.coughlin@ligo.org
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
@@ -23,7 +24,8 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides: gwemopt
 License-File: LICENSE
 
 gwemopt is a python package for GW-EM Followup Optimization 
+
```

### Comparing `gwemopt-0.0.80/gwemopt.egg-info/SOURCES.txt` & `gwemopt-0.0.81/gwemopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/setup.py` & `gwemopt-0.0.81/setup.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/utils/__init__.py` & `gwemopt-0.0.81/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/utils/version.py` & `gwemopt-0.0.81/utils/version.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.80/versioneer.py` & `gwemopt-0.0.81/versioneer.py`

 * *Files identical despite different names*

