# Comparing `tmp/gwemopt-0.0.81.tar.gz` & `tmp/gwemopt-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwemopt-0.0.81.tar", last modified: Sat Apr 15 17:06:05 2023, max compression
+gzip compressed data, was "gwemopt-0.0.82.tar", last modified: Sat Apr 15 17:33:11 2023, max compression
```

## Comparing `gwemopt-0.0.81.tar` & `gwemopt-0.0.82.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.581353 gwemopt-0.0.81/
--rw-r--r--   0 mcoughlin   (501) staff       (20)    35147 2023-02-01 13:42:46.000000 gwemopt-0.0.81/LICENSE
--rw-r--r--   0 mcoughlin   (501) staff       (20)       50 2023-02-01 13:42:46.000000 gwemopt-0.0.81/MANIFEST.in
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1177 2023-04-15 17:06:05.581431 gwemopt-0.0.81/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1741 2023-02-01 13:42:46.000000 gwemopt-0.0.81/README.md
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.573227 gwemopt-0.0.81/bin/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6086 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/condor_gwemopt_run.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6184 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/efficiency_gwemopt_run.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13658 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_check_coverage
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1942 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_check_ref
--rw-r--r--   0 mcoughlin   (501) staff       (20)     7422 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_compute_overlap
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4669 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_crossmatch_catalog
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1503 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_download_ref
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1397 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_gen_queue
--rw-r--r--   0 mcoughlin   (501) staff       (20)    14662 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_gen_skymap
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3621 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_json_overlap
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5260 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_coverage_hist
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5049 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_coverage_int
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6714 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_ref
--rw-r--r--   0 mcoughlin   (501) staff       (20)    15337 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_plot_skymap
--rw-r--r--   0 mcoughlin   (501) staff       (20)    28801 2023-04-15 17:05:46.000000 gwemopt-0.0.81/bin/gwemopt_run
--rw-r--r--   0 mcoughlin   (501) staff       (20)    41793 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_serendipitous_schedule
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3819 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/gwemopt_skyvision_to_list
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2434 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/plot_telescope_comparison_S200115j.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2422 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/plot_telescope_comparison_S200213t.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1561 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_O2
--rw-r--r--   0 mcoughlin   (501) staff       (20)    14696 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gracedb.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1023 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GBM
--rw-r--r--   0 mcoughlin   (501) staff       (20)      665 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180523
--rw-r--r--   0 mcoughlin   (501) staff       (20)      798 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180626
--rw-r--r--   0 mcoughlin   (501) staff       (20)      666 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180715
--rw-r--r--   0 mcoughlin   (501) staff       (20)      807 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_GRB180728
--rw-r--r--   0 mcoughlin   (501) staff       (20)      430 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_TESS
--rw-r--r--   0 mcoughlin   (501) staff       (20)      727 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_run
--rw-r--r--   0 mcoughlin   (501) staff       (20)      359 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_run.pbs
--rw-r--r--   0 mcoughlin   (501) staff       (20)    17679 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_gwemopt_superscheduler
--rw-r--r--   0 mcoughlin   (501) staff       (20)    26105 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_skymaps.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    10081 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/run_skymaps_pproc.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2102 2023-02-01 13:42:47.000000 gwemopt-0.0.81/bin/slice_catalog.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.582189 gwemopt-0.0.81/gwemopt/
--rw-r--r--   0 mcoughlin   (501) staff       (20)      948 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)      498 2023-04-15 17:06:05.582231 gwemopt-0.0.81/gwemopt/_version.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    20739 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/catalog.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    35709 2023-04-15 17:05:46.000000 gwemopt-0.0.81/gwemopt/coverage.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13375 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/decam_tiling.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     9242 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/efficiency.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1566 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/flaskapp.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)      899 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/footprint.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1396 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/gracedb.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6490 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/lightcurve.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2685 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/mapsplit.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6093 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/moc.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2068 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/models.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    22116 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/pem.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    36994 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/plotting.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13976 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/quadrants.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    34491 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/rankedTilesGenerator.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12347 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/samplers.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    41865 2023-04-15 17:02:35.000000 gwemopt-0.0.81/gwemopt/scheduler.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    17763 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/segments.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12339 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/segments_astroplan.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12739 2023-04-15 17:05:46.000000 gwemopt-0.0.81/gwemopt/skyportal.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.580625 gwemopt-0.0.81/gwemopt/tests/
--rw-r--r--   0 mcoughlin   (501) staff       (20)        0 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/tests/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    10001 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/tests/test_schedule.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    29039 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/tiles.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4540 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/transients.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    53746 2023-04-15 17:05:46.000000 gwemopt-0.0.81/gwemopt/utils.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    16420 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/waw.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3751 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/ztf_coverage.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12447 2023-02-01 13:42:47.000000 gwemopt-0.0.81/gwemopt/ztf_tiling.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.580325 gwemopt-0.0.81/gwemopt.egg-info/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1177 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1730 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/SOURCES.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/dependency_links.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)      211 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/requires.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)       14 2023-04-15 17:06:05.000000 gwemopt-0.0.81/gwemopt.egg-info/top_level.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)      402 2023-04-15 17:06:05.581967 gwemopt-0.0.81/setup.cfg
--rwxr-xr-x   0 mcoughlin   (501) staff       (20)     3791 2023-04-15 17:05:46.000000 gwemopt-0.0.81/setup.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:06:05.581125 gwemopt-0.0.81/utils/
--rw-r--r--   0 mcoughlin   (501) staff       (20)      809 2023-02-01 13:42:48.000000 gwemopt-0.0.81/utils/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6213 2023-02-01 13:42:48.000000 gwemopt-0.0.81/utils/version.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    68611 2023-02-01 13:42:48.000000 gwemopt-0.0.81/versioneer.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:33:11.105258 gwemopt-0.0.82/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    35147 2023-02-01 13:42:46.000000 gwemopt-0.0.82/LICENSE
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       50 2023-02-01 13:42:46.000000 gwemopt-0.0.82/MANIFEST.in
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1158 2023-04-15 17:33:11.105338 gwemopt-0.0.82/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1741 2023-02-01 13:42:46.000000 gwemopt-0.0.82/README.md
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:33:11.099117 gwemopt-0.0.82/bin/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)  1586880 2023-04-15 02:30:49.000000 gwemopt-0.0.82/bin/2023-04-14T08-00-49_glg_healpix_all_bn230414334.fit.fits
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6086 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/condor_gwemopt_run.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6184 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/efficiency_gwemopt_run.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13658 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_check_coverage
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1942 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_check_ref
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     7422 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_compute_overlap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4669 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_crossmatch_catalog
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1503 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_download_ref
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1397 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_gen_queue
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    14662 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_gen_skymap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     3621 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_json_overlap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5260 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_plot_coverage_hist
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5049 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_plot_coverage_int
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6714 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_plot_ref
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    15337 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_plot_skymap
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    28801 2023-04-15 17:32:30.000000 gwemopt-0.0.82/bin/gwemopt_run
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    41793 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_serendipitous_schedule
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     3819 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/gwemopt_skyvision_to_list
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2434 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/plot_telescope_comparison_S200115j.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2422 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/plot_telescope_comparison_S200213t.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1561 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_O2
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    14696 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gracedb.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1023 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_GBM
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      665 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_GRB180523
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      798 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_GRB180626
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      666 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_GRB180715
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      807 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_GRB180728
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      430 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_TESS
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      727 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_run
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      359 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_run.pbs
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    17679 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_gwemopt_superscheduler
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    26105 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_skymaps.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    10081 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/run_skymaps_pproc.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2102 2023-02-01 13:42:47.000000 gwemopt-0.0.82/bin/slice_catalog.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:33:11.105890 gwemopt-0.0.82/gwemopt/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      948 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      498 2023-04-15 17:33:11.105925 gwemopt-0.0.82/gwemopt/_version.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    20739 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/catalog.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    35709 2023-04-15 17:05:46.000000 gwemopt-0.0.82/gwemopt/coverage.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13375 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/decam_tiling.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     9242 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/efficiency.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1566 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/flaskapp.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      899 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/footprint.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1396 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/gracedb.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6490 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/lightcurve.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2685 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/mapsplit.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6093 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/moc.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2068 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/models.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    22116 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/pem.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    36994 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/plotting.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13976 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/quadrants.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    34491 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/rankedTilesGenerator.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12347 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/samplers.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    41865 2023-04-15 17:02:35.000000 gwemopt-0.0.82/gwemopt/scheduler.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    17763 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/segments.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12339 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/segments_astroplan.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12723 2023-04-15 17:31:53.000000 gwemopt-0.0.82/gwemopt/skyportal.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:33:11.104873 gwemopt-0.0.82/gwemopt/tests/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        0 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/tests/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    10001 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/tests/test_schedule.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    29039 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/tiles.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4540 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/transients.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    53746 2023-04-15 17:05:46.000000 gwemopt-0.0.82/gwemopt/utils.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    16420 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/waw.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     3751 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/ztf_coverage.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12447 2023-02-01 13:42:47.000000 gwemopt-0.0.82/gwemopt/ztf_tiling.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:33:11.104633 gwemopt-0.0.82/gwemopt.egg-info/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1158 2023-04-15 17:33:10.000000 gwemopt-0.0.82/gwemopt.egg-info/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1791 2023-04-15 17:33:10.000000 gwemopt-0.0.82/gwemopt.egg-info/SOURCES.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2023-04-15 17:33:10.000000 gwemopt-0.0.82/gwemopt.egg-info/dependency_links.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      211 2023-04-15 17:33:10.000000 gwemopt-0.0.82/gwemopt.egg-info/requires.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       14 2023-04-15 17:33:10.000000 gwemopt-0.0.82/gwemopt.egg-info/top_level.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      402 2023-04-15 17:33:11.105708 gwemopt-0.0.82/setup.cfg
+-rwxr-xr-x   0 mcoughlin   (501) staff       (20)     3791 2023-04-15 17:05:46.000000 gwemopt-0.0.82/setup.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-15 17:33:11.105143 gwemopt-0.0.82/utils/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      809 2023-02-01 13:42:48.000000 gwemopt-0.0.82/utils/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6213 2023-02-01 13:42:48.000000 gwemopt-0.0.82/utils/version.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    68611 2023-02-01 13:42:48.000000 gwemopt-0.0.82/versioneer.py
```

### Comparing `gwemopt-0.0.81/LICENSE` & `gwemopt-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/PKG-INFO` & `gwemopt-0.0.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gwemopt
-Version: 0.0.81
+Version: 0.0.82
 Summary: A python package for GW-EM Followup Optimization
 Home-page: https://github.com/mcoughlin/gwemopt/
 Author: Michael Coughlin
 Author-email: michael.coughlin@ligo.org
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
@@ -24,8 +23,7 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides: gwemopt
 License-File: LICENSE
 
 gwemopt is a python package for GW-EM Followup Optimization 
-
```

### Comparing `gwemopt-0.0.81/README.md` & `gwemopt-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/condor_gwemopt_run.py` & `gwemopt-0.0.82/bin/condor_gwemopt_run.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/efficiency_gwemopt_run.py` & `gwemopt-0.0.82/bin/efficiency_gwemopt_run.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_check_coverage` & `gwemopt-0.0.82/bin/gwemopt_check_coverage`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_check_ref` & `gwemopt-0.0.82/bin/gwemopt_check_ref`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_compute_overlap` & `gwemopt-0.0.82/bin/gwemopt_compute_overlap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_crossmatch_catalog` & `gwemopt-0.0.82/bin/gwemopt_crossmatch_catalog`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_download_ref` & `gwemopt-0.0.82/bin/gwemopt_download_ref`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_gen_queue` & `gwemopt-0.0.82/bin/gwemopt_gen_queue`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_gen_skymap` & `gwemopt-0.0.82/bin/gwemopt_gen_skymap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_json_overlap` & `gwemopt-0.0.82/bin/gwemopt_json_overlap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_plot_coverage_hist` & `gwemopt-0.0.82/bin/gwemopt_plot_coverage_hist`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_plot_coverage_int` & `gwemopt-0.0.82/bin/gwemopt_plot_coverage_int`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_plot_ref` & `gwemopt-0.0.82/bin/gwemopt_plot_ref`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_plot_skymap` & `gwemopt-0.0.82/bin/gwemopt_plot_skymap`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_run` & `gwemopt-0.0.82/bin/gwemopt_run`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_serendipitous_schedule` & `gwemopt-0.0.82/bin/gwemopt_serendipitous_schedule`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/gwemopt_skyvision_to_list` & `gwemopt-0.0.82/bin/gwemopt_skyvision_to_list`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/plot_telescope_comparison_S200115j.py` & `gwemopt-0.0.82/bin/plot_telescope_comparison_S200115j.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/plot_telescope_comparison_S200213t.py` & `gwemopt-0.0.82/bin/plot_telescope_comparison_S200213t.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_O2` & `gwemopt-0.0.82/bin/run_O2`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gracedb.py` & `gwemopt-0.0.82/bin/run_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gwemopt_GBM` & `gwemopt-0.0.82/bin/run_gwemopt_GBM`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gwemopt_GRB180523` & `gwemopt-0.0.82/bin/run_gwemopt_GRB180523`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gwemopt_GRB180626` & `gwemopt-0.0.82/bin/run_gwemopt_GRB180626`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gwemopt_GRB180715` & `gwemopt-0.0.82/bin/run_gwemopt_GRB180715`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gwemopt_GRB180728` & `gwemopt-0.0.82/bin/run_gwemopt_GRB180728`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gwemopt_run` & `gwemopt-0.0.82/bin/run_gwemopt_run`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_gwemopt_superscheduler` & `gwemopt-0.0.82/bin/run_gwemopt_superscheduler`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_skymaps.py` & `gwemopt-0.0.82/bin/run_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/run_skymaps_pproc.py` & `gwemopt-0.0.82/bin/run_skymaps_pproc.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/bin/slice_catalog.py` & `gwemopt-0.0.82/bin/slice_catalog.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/__init__.py` & `gwemopt-0.0.82/gwemopt/__init__.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/catalog.py` & `gwemopt-0.0.82/gwemopt/catalog.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/coverage.py` & `gwemopt-0.0.82/gwemopt/coverage.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/decam_tiling.py` & `gwemopt-0.0.82/gwemopt/decam_tiling.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/efficiency.py` & `gwemopt-0.0.82/gwemopt/efficiency.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/flaskapp.py` & `gwemopt-0.0.82/gwemopt/flaskapp.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/footprint.py` & `gwemopt-0.0.82/gwemopt/footprint.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/gracedb.py` & `gwemopt-0.0.82/gwemopt/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/lightcurve.py` & `gwemopt-0.0.82/gwemopt/lightcurve.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/mapsplit.py` & `gwemopt-0.0.82/gwemopt/mapsplit.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/moc.py` & `gwemopt-0.0.82/gwemopt/moc.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/models.py` & `gwemopt-0.0.82/gwemopt/models.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/pem.py` & `gwemopt-0.0.82/gwemopt/pem.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/plotting.py` & `gwemopt-0.0.82/gwemopt/plotting.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/quadrants.py` & `gwemopt-0.0.82/gwemopt/quadrants.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/rankedTilesGenerator.py` & `gwemopt-0.0.82/gwemopt/rankedTilesGenerator.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/samplers.py` & `gwemopt-0.0.82/gwemopt/samplers.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/scheduler.py` & `gwemopt-0.0.82/gwemopt/scheduler.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/segments.py` & `gwemopt-0.0.82/gwemopt/segments.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/segments_astroplan.py` & `gwemopt-0.0.82/gwemopt/segments_astroplan.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/skyportal.py` & `gwemopt-0.0.82/gwemopt/skyportal.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,14 @@
             for ii, key in enumerate(keys):
                 if ii in ipix_keep:
                     moc_struct[key] = moc_struct_new[key]
                     cnt = cnt + 1
 
         moc_structs[telescope] = moc_struct
 
-    print(stop)
     return moc_structs
 
 
 def skyportal2FOV(tess, nside):
 
     moc = moc_from_tiles([tile.healpix for tile in tess.tiles], 2**29)
     pix_id = moc.degrade_to_order(int(np.log2(nside))).flatten()
```

### Comparing `gwemopt-0.0.81/gwemopt/tests/test_schedule.py` & `gwemopt-0.0.82/gwemopt/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/tiles.py` & `gwemopt-0.0.82/gwemopt/tiles.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/transients.py` & `gwemopt-0.0.82/gwemopt/transients.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/utils.py` & `gwemopt-0.0.82/gwemopt/utils.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/waw.py` & `gwemopt-0.0.82/gwemopt/waw.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/ztf_coverage.py` & `gwemopt-0.0.82/gwemopt/ztf_coverage.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt/ztf_tiling.py` & `gwemopt-0.0.82/gwemopt/ztf_tiling.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/gwemopt.egg-info/PKG-INFO` & `gwemopt-0.0.82/gwemopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gwemopt
-Version: 0.0.81
+Version: 0.0.82
 Summary: A python package for GW-EM Followup Optimization
 Home-page: https://github.com/mcoughlin/gwemopt/
 Author: Michael Coughlin
 Author-email: michael.coughlin@ligo.org
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
@@ -24,8 +23,7 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides: gwemopt
 License-File: LICENSE
 
 gwemopt is a python package for GW-EM Followup Optimization 
-
```

### Comparing `gwemopt-0.0.81/gwemopt.egg-info/SOURCES.txt` & `gwemopt-0.0.82/gwemopt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
+bin/2023-04-14T08-00-49_glg_healpix_all_bn230414334.fit.fits
 bin/condor_gwemopt_run.py
 bin/efficiency_gwemopt_run.py
 bin/gwemopt_check_coverage
 bin/gwemopt_check_ref
 bin/gwemopt_compute_overlap
 bin/gwemopt_crossmatch_catalog
 bin/gwemopt_download_ref
```

### Comparing `gwemopt-0.0.81/setup.py` & `gwemopt-0.0.82/setup.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/utils/__init__.py` & `gwemopt-0.0.82/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/utils/version.py` & `gwemopt-0.0.82/utils/version.py`

 * *Files identical despite different names*

### Comparing `gwemopt-0.0.81/versioneer.py` & `gwemopt-0.0.82/versioneer.py`

 * *Files identical despite different names*

