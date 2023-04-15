# Comparing `tmp/timeeval-gutenTAG-1.3.0.tar.gz` & `tmp/timeeval-gutenTAG-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/timeeval-gutenTAG-1.3.0.tar", last modified: Thu Feb  9 13:43:59 2023, max compression
+gzip compressed data, was "dist/timeeval-gutenTAG-1.4.0.tar", last modified: Sat Apr 15 11:32:18 2023, max compression
```

## Comparing `timeeval-gutenTAG-1.3.0.tar` & `timeeval-gutenTAG-1.4.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/addons/
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/addons/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/addons/timeeval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/extremum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/mode_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/pattern_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/trend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/variance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/api/bo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/base_oscillation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/cylinder_bell_funnel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/dirichlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/ecg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/formula.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/mls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/random_mode_jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/sawtooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/square.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/utils/math_func_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/anomaly-kind.guten-tag-generation-config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/anomaly.guten-tag-generation-config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/formula.guten-tag-generation-config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/guten-tag-generation-config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/oscillation.guten-tag-generation-config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/schema_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/config/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/consolidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/generator/overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/generator/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/gutenTAG.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/default_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/tqdm_joblib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/gutenTAG/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/logo_transparent.png
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-02-09 13:43:19.000000 timeeval-gutenTAG-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-09 13:43:59.000000 timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/addons/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/addons/timeeval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/extremum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/mode_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/pattern_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/variance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/api/bo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/base_oscillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/custom_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/cylinder_bell_funnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/dirichlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/mls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/random_mode_jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/sawtooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/square.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/utils/math_func_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/anomaly-kind.guten-tag-generation-config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/anomaly.guten-tag-generation-config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/formula.guten-tag-generation-config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/guten-tag-generation-config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/oscillation.guten-tag-generation-config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/schema_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/config/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/consolidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/generator/overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/generator/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/gutenTAG.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/tqdm_joblib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/gutenTAG/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/logo_transparent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-15 11:31:58.000000 timeeval-gutenTAG-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 11:32:18.000000 timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/top_level.txt
```

### Comparing `timeeval-gutenTAG-1.3.0/LICENSE` & `timeeval-gutenTAG-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/PKG-INFO` & `timeeval-gutenTAG-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeeval-gutenTAG
-Version: 1.3.0
+Version: 1.4.0
 Summary: A good Timeseries Anomaly Generator.
 Home-page: https://github.com/HPI-Information-Systems/gutentag
 Author: Phillip Wenig and Sebastian Schmidl
 Author-email: phillip.wenig@hpi.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `timeeval-gutenTAG-1.3.0/README.md` & `timeeval-gutenTAG-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/__main__.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/__main__.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/addons/__init__.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/addons/__init__.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/addons/timeeval.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/addons/timeeval.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,19 @@
             datasets.append(self._process_timeseries(config, ts, LearningType.SemiSupervised))
         return ctx.store_data(self.key, {
             "name": ts.dataset_name,
             "datasets": datasets
         })
 
     def finalize(self, ctx: AddOnFinalizeContext) -> None:
-        df = pd.DataFrame(columns=columns)
         # add metadata
+        metadata = []
         for ts_obj in ctx.get_data(self.key):
-            df = df.append(ts_obj["datasets"], ignore_index=True)
+            metadata += ts_obj["datasets"]
+        df = pd.DataFrame(metadata, columns=columns)
         self._set_global_vals(df)
         self.df = df
         if ctx.should_save and ctx.output_folder is not None:
             filename = os.path.join(ctx.output_folder, "datasets.csv")
             df.to_csv(filename, index=False)
 
     def _process_timeseries(self, config: Dict, generator: TimeSeries, tpe: LearningType) -> Dict[str, Any]:
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/__init__.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     while being injected to a BaseOscillation, performs the changes."""
 
     def __init__(self,
                  position: Position,
                  exact_position: Optional[int],
                  anomaly_length: int,
                  channel: int = 0,
-                 creep_length: int = 0):
+                 creeping_length: int = 0):
         self.position = position
         self.exact_position = exact_position
         self.anomaly_length = anomaly_length
         self.channel = channel
-        self.creep_length = creep_length
+        self.creeping_length = creeping_length
 
         self.anomaly_kinds: List[BaseAnomaly] = []
         self._requires_period_start_position: bool = False
 
     def set_anomaly(self, anomaly_kind: BaseAnomaly) -> Anomaly:
         self.anomaly_kinds.append(anomaly_kind)
         self._requires_period_start_position = self._requires_period_start_position or anomaly_kind.requires_period_start_position
@@ -55,15 +55,15 @@
         if self.exact_position is None:
             start, end = self._find_position(ctx)
         else:
             start, end = self.exact_position, self.exact_position + self.anomaly_length
 
         length = end - start
         label_range = LabelRange(start, length)
-        protocol = AnomalyProtocol(start, end, self.channel, ctx, label_range, creep_length=self.creep_length)
+        protocol = AnomalyProtocol(start, end, self.channel, ctx, label_range, creeping_length=self.creeping_length)
 
         for anomaly in self.anomaly_kinds:
             protocol = anomaly.generate(protocol)
 
         return protocol
 
     def _find_position(self, ctx: AnomalyGenerationContext, max_tries: int = 50) -> Tuple[int, int]:
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/__init__.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 @dataclass
 class AnomalyProtocol:
     start: int
     end: int
     channel: int
     ctx: AnomalyGenerationContext
     labels: LabelRange
-    creep_length: int = 0
+    creeping_length: int = 0
     subsequences: List[np.ndarray] = field(default_factory=lambda: [])
 
     @property
     def rng(self) -> np.random.Generator:
         return self.ctx.rng
 
     @property
@@ -37,16 +37,16 @@
         return self.ctx.base_oscillation_kind
 
     @property
     def length(self) -> int:
         return self.end - self.start
 
     @property
-    def length_without_creep(self) -> int:
-        return self.length - self.creep_length
+    def length_without_creeping(self) -> int:
+        return self.length - self.creeping_length
 
 
 class BaseAnomaly(ABC):
     def __init__(self):
         self.logger = GutenTagLogger()
 
     @abstractmethod
@@ -54,19 +54,19 @@
         return anomaly_protocol
 
     @property
     @abstractmethod
     def requires_period_start_position(self) -> bool:
         return False
 
-    def generate_creep(self, anomaly_protocol: AnomalyProtocol, custom_anomaly_length: Optional[int] = None) -> np.ndarray:
-        creep_length = anomaly_protocol.creep_length
-        anomaly_length = anomaly_protocol.length_without_creep if custom_anomaly_length is None else custom_anomaly_length
+    def generate_creeping(self, anomaly_protocol: AnomalyProtocol, custom_anomaly_length: Optional[int] = None) -> np.ndarray:
+        creeping_length = anomaly_protocol.creeping_length
+        anomaly_length = anomaly_protocol.length_without_creeping if custom_anomaly_length is None else custom_anomaly_length
         return np.concatenate([
-            np.linspace(0, 1, creep_length),  # creep
+            np.linspace(0, 1, creeping_length),  # creep
             np.ones(anomaly_length)           # anomaly
         ])
 
     def turn_off_trend(self, anomaly_protocol):
         anomaly_protocol.base_oscillation.trend_series[anomaly_protocol.start:anomaly_protocol.end] = 0
 
     @staticmethod
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/amplitude.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/amplitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
     def generate(self, anomaly_protocol: AnomalyProtocol) -> AnomalyProtocol:
         if anomaly_protocol.base_oscillation_kind in [Polynomial.KIND, Formula.KIND, RandomModeJump.KIND]:
             self.logger.warn_false_combination(self.__class__.__name__, anomaly_protocol.base_oscillation_kind)
             return anomaly_protocol
 
         length = anomaly_protocol.end - anomaly_protocol.start
-        if anomaly_protocol.creep_length == 0:
+        if anomaly_protocol.creeping_length == 0:
             transition_length = int(length * 0.2)
             plateau = np.ones(int(length * 0.6))
             start_transition = norm.pdf(np.linspace(-3, 0, transition_length), scale=1.05)
             end_transition = norm.pdf(np.linspace(0, 3, transition_length), scale=1.05)
             amplitude_bell = np.concatenate([start_transition / start_transition.max(), plateau, end_transition / end_transition.max()])
         else:
-            anomaly_length = length - anomaly_protocol.creep_length
-            creep = self.generate_creep(anomaly_protocol, custom_anomaly_length=int(anomaly_length * 0.8))
+            anomaly_length = length - anomaly_protocol.creeping_length
+            creeping = self.generate_creeping(anomaly_protocol, custom_anomaly_length=int(anomaly_length * 0.8))
             end_transition = norm.pdf(np.linspace(0, 3, int(anomaly_length * 0.2)), scale=1.05)
-            amplitude_bell = np.concatenate([creep, end_transition / end_transition.max()])
+            amplitude_bell = np.concatenate([creeping, end_transition / end_transition.max()])
         if self.amplitude_factor < 1.0:
             amplitude_bell = MinMaxScaler(feature_range=(1.0, 2.0 - self.amplitude_factor)).fit_transform(amplitude_bell.reshape(-1, 1)).reshape(-1)
             amplitude_bell = amplitude_bell * -1 + 2
         else:
             amplitude_bell = MinMaxScaler(feature_range=(1.0, self.amplitude_factor)).fit_transform(amplitude_bell.reshape(-1, 1)).reshape(-1)
 
         subsequence = anomaly_protocol.base_oscillation.timeseries[anomaly_protocol.start:anomaly_protocol.end] * amplitude_bell
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/extremum.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/extremum.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/frequency.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/frequency.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/kind.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/kind.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/mean.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/mean.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     def generate(self, anomaly_protocol: AnomalyProtocol) -> AnomalyProtocol:
         if anomaly_protocol.base_oscillation_kind == RandomModeJump.KIND:
             self.logger.warn_false_combination(self.__class__.__name__, anomaly_protocol.base_oscillation_kind)
             return anomaly_protocol
 
         base = anomaly_protocol.base_oscillation
         ts: np.ndarray = base.timeseries
-        creep = self.generate_creep(anomaly_protocol)
-        subsequence = ts[anomaly_protocol.start:anomaly_protocol.end] + self.offset * creep
+        creeping = self.generate_creeping(anomaly_protocol)
+        subsequence = ts[anomaly_protocol.start:anomaly_protocol.end] + self.offset * creeping
         anomaly_protocol.subsequences.append(subsequence)
         return anomaly_protocol
 
     @property
     def requires_period_start_position(self) -> bool:
         return False
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/mode_correlation.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/mode_correlation.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/pattern.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/pattern.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/pattern_shift.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/pattern_shift.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/platform.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/platform.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/trend.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/trend.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/anomalies/types/variance.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/anomalies/types/variance.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,18 @@
                 variance=self.variance
             )[anomaly_protocol.start:anomaly_protocol.end]
             anomaly_protocol.subsequences.append(subsequence)
 
         else:
             length = anomaly_protocol.end - anomaly_protocol.start
             variance_diff = self.variance - base.variance
-            creep = self.generate_creep(anomaly_protocol) * variance_diff + base.variance  # from 0 to variance_diff
-            creep /= self.variance * base.amplitude  # get relative transition from base variance to anomaly variance
+            creeping = self.generate_creeping(anomaly_protocol) * variance_diff + base.variance  # from 0 to variance_diff
+            creeping /= self.variance * base.amplitude  # get relative transition from base variance to anomaly variance
             subsequence_noise = base.generate_noise(anomaly_protocol.ctx.to_bo(), self.variance * base.amplitude, length)
-            base.noise[anomaly_protocol.start:anomaly_protocol.end] = subsequence_noise * creep
+            base.noise[anomaly_protocol.start:anomaly_protocol.end] = subsequence_noise * creeping
         return anomaly_protocol
 
     @property
     def requires_period_start_position(self) -> bool:
         return False
 
     @staticmethod
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/api/bo.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/api/bo.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/__init__.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .base_oscillation import BaseOscillation
 from .cosine import Cosine
+from .custom_input import CustomInput
 from .cylinder_bell_funnel import CylinderBellFunnel
 from .dirichlet import Dirichlet
 from .ecg import ECG
 from .formula import Formula  # type: ignore  # mypy ends up in recursion
 from .interface import BaseOscillationInterface
 from .mls import MLS
 from .polynomial import Polynomial
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/cosine.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/cosine.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/cylinder_bell_funnel.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/cylinder_bell_funnel.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/dirichlet.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/dirichlet.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/ecg.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/ecg.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/formula.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/formula.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/interface.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/interface.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         self.random_seed = kwargs.get(PARAMETERS.RANDOM_SEED, default_values[BASE_OSCILLATIONS][PARAMETERS.RANDOM_SEED])
         self.formula = kwargs.get(PARAMETERS.FORMULA, default_values[BASE_OSCILLATIONS][PARAMETERS.FORMULA])
         self.ecg_sim_method = kwargs.get(PARAMETERS.ECG_SIM_METHOD, default_values[BASE_OSCILLATIONS][PARAMETERS.ECG_SIM_METHOD])
         self.width = kwargs.get(PARAMETERS.WIDTH, default_values[BASE_OSCILLATIONS][PARAMETERS.WIDTH])
         self.duty = kwargs.get(PARAMETERS.DUTY, default_values[BASE_OSCILLATIONS][PARAMETERS.DUTY])
         self.periodicity = kwargs.get(PARAMETERS.PERIODICITY, default_values[BASE_OSCILLATIONS][PARAMETERS.PERIODICITY])
         self.complexity = kwargs.get(PARAMETERS.COMPLEXITY, default_values[BASE_OSCILLATIONS][PARAMETERS.COMPLEXITY])
+        self.input_timeseries_path_train = kwargs.get(PARAMETERS.INPUT_TIMESERIES_PATH_TRAIN, default_values[BASE_OSCILLATIONS][PARAMETERS.INPUT_TIMESERIES_PATH_TRAIN])
+        self.input_timeseries_path_test = kwargs.get(PARAMETERS.INPUT_TIMESERIES_PATH_TEST, default_values[BASE_OSCILLATIONS][PARAMETERS.INPUT_TIMESERIES_PATH_TEST])
+        self.use_column_train = kwargs.get(PARAMETERS.USE_COLUMN_TRAIN, default_values[BASE_OSCILLATIONS][PARAMETERS.USE_COLUMN_TRAIN])
+        self.use_column_test = kwargs.get(PARAMETERS.USE_COLUMN_TEST, default_values[BASE_OSCILLATIONS][PARAMETERS.USE_COLUMN_TEST])
 
         self.timeseries: Optional[np.ndarray] = None
         self.noise: Optional[np.ndarray] = None
         self.trend_series: Optional[np.ndarray] = None
 
     def generate_noise(self, ctx: BOGenerationContext, variance: float, length: int) -> np.ndarray:
         return ctx.rng.normal(0, variance, length)
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/mls.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/mls.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/polynomial.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/polynomial.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/random_mode_jump.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/random_mode_jump.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/random_walk.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/random_walk.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,8 @@
         ts = np.convolve(ts, ts_filter, "valid")
     else:
         ts = _gen_steps(rng, length)
 
     return MinMaxScaler(feature_range=(-amplitude, amplitude)).fit_transform(ts.reshape(-1, 1)).reshape(-1)
 
 
-BaseOscillation.register(RandomWalk.KIND, RandomWalk)
+BaseOscillation.register(RandomWalk.KIND, RandomWalk)
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/sawtooth.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/sawtooth.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/sine.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/sine.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/square.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/square.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/base_oscillations/utils/math_func_support.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/base_oscillations/utils/math_func_support.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/parser.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     def _build_single_anomaly(self, d: Dict) -> Anomaly:
         anomaly = Anomaly(
             Position(d.get(PARAMETERS.POSITION, default_values[ANOMALIES][PARAMETERS.POSITION])),
             d.get(PARAMETERS.EXACT_POSITION, None),
             d[PARAMETERS.LENGTH],
             d.get(PARAMETERS.CHANNEL, default_values[ANOMALIES][PARAMETERS.CHANNEL]),
-            d.get(PARAMETERS.CREEP_LENGTH, default_values[ANOMALIES][PARAMETERS.CREEP_LENGTH])
+            d.get(PARAMETERS.CREEPING_LENGTH, default_values[ANOMALIES][PARAMETERS.CREEPING_LENGTH])
         )
 
         anomaly_kinds = self._build_anomaly_kinds(d, anomaly.anomaly_length)
         for kind in anomaly_kinds:
             anomaly.set_anomaly(kind)
 
         return anomaly
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/anomaly-kind.guten-tag-generation-config.schema.yaml` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/anomaly-kind.guten-tag-generation-config.schema.yaml`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/anomaly.guten-tag-generation-config.schema.yaml` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/anomaly.guten-tag-generation-config.schema.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       Exact position of the anomaly.
       Starts at the given integer and ends at `exact-position + length`.
       Renders the 'position' parameter useless.
   length:
     type: integer
     minimum: 1
     description: Length of the anomaly region. For extrema, this must be 1.
-  creep-length:
+  creeping-length:
     type: integer
     minimum: 0
     description: Length of the transition region before the anomaly.
   channel:
     type: integer
     description: Channel identifier, where this anomaly should be applied to.
   kinds:
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/formula.guten-tag-generation-config.schema.yaml` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/formula.guten-tag-generation-config.schema.yaml`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/guten-tag-generation-config.schema.yaml` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/guten-tag-generation-config.schema.yaml`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/schema/oscillation.guten-tag-generation-config.schema.yaml` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/schema/oscillation.guten-tag-generation-config.schema.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
       - polynomial
       - random-mode-jump
       - formula
       - sawtooth
       - square
       - dirichlet
       - mls
+      - custom-input
     description: Kind of the base oscillation.
 oneOf:
   - properties:
       trend:
         description: Trend to add to the base oscillation
         $ref: "#"
       offset:
@@ -377,7 +378,42 @@
           This controls the length of the repeating sequence and its complexity.
       smoothing:
         type: number
         description: |
           Smoothing factor for convolutional smoothing of the generated bit sequence (highly recommended).
           Default is 0.01.
     additionalProperties: false
+  - properties:
+      trend:
+        description: Trend to add to the base oscillation
+        $ref: "#"
+      offset:
+        type: number
+        description: Constant offset added to the base oscillation.
+      variance:
+        type: number
+        description: |
+          Variance of the signal relative to signal value.
+          This is also called white noise.
+          If set to 0, there is no noise.
+      kind:
+        const: custom-input
+      input-timeseries-path-train:
+        type: string
+        description: |
+          timeseries from input file path used for a (semi-)supevised training set.
+      input-timeseries-path-test:
+        type: string
+        description: |
+          timeseries from input file path used for a test set.
+      use-column-test:
+        type: [string, integer]
+        description: |
+          column of the test data input file(s) to use
+      use-column-train:
+        type: [string, integer]
+        description: |
+          column of the training data input file(s) to use
+      required:
+        - use-column-test
+        - input-timeseries-path-test
+    additionalProperties: false
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/schema_loader.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/schema_loader.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/config/validator.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/config/validator.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/consolidator.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/consolidator.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,32 +7,39 @@
 from gutenTAG.utils.types import GenerationContext
 
 
 class Consolidator:
     def __init__(self,
                  base_oscillations: List[BaseOscillationInterface],
                  anomalies: List[Anomaly],
-                 random_seed: Optional[int] = None):
+                 random_seed: Optional[int] = None,
+                 semi_supervised: Optional[bool] = None,
+                 supervised: Optional[bool] = None):
         self.consolidated_channels: List[BaseOscillationInterface] = base_oscillations
         self.anomalies: List[Anomaly] = anomalies
         self.generated_anomalies: List[Tuple[AnomalyProtocol, int]] = []
         self.timeseries: Optional[np.ndarray] = None
         self.labels: Optional[np.ndarray] = None
         self.random_seed: Optional[int] = random_seed
+        self.semi_supervised: Optional[bool] = semi_supervised
+        self.supervised: Optional[bool] =  supervised
 
     def add_channel(self, channel: BaseOscillationInterface):
         self.consolidated_channels.append(channel)
 
     def get_channel(self, channel: int) -> BaseOscillationInterface:
         return self.consolidated_channels[channel]
 
     def generate(self, ctx: GenerationContext) -> Tuple[np.ndarray, np.ndarray]:
         channels: List[np.ndarray] = []
         for c, bo in enumerate(self.consolidated_channels):
-            bo.generate_timeseries_and_variations(ctx.to_bo(c, channels))  # type: ignore  # timeseries gets set in generate_timeseries_and_variations()
+            bo.generate_timeseries_and_variations(ctx.to_bo(c, channels),
+                                                  semi_supervised=self.semi_supervised,
+                                                  supervised=self.supervised,
+                                                  )  # type: ignore  # timeseries gets set in generate_timeseries_and_variations()
             if bo.timeseries is not None:
                 channels.append(bo.timeseries)
         self.timeseries = self._stack_channels(channels)
         self.labels = np.zeros(self.timeseries.shape[0], dtype=np.int8)
         self.generate_anomalies(ctx)
 
         self.apply_anomalies()
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/generator/overview.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/generator/overview.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/generator/timeseries.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/generator/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,23 @@
         self._rng_counter = 0
 
     def generate(self, random_seed: Optional[int] = None) -> TimeSeries:
         consolidator = Consolidator(self.base_oscillations, self.anomalies)
         self.timeseries, self.labels = consolidator.generate(GenerationContext(seed=self._create_new_seed(random_seed)))
 
         if self.semi_supervised:
-            semi_supervised_consolidator = Consolidator(self.base_oscillations, [])
+            semi_supervised_consolidator = Consolidator(self.base_oscillations, [],
+                                                        semi_supervised=self.semi_supervised)
             self.semi_supervised_timeseries, self.semi_train_labels = semi_supervised_consolidator.generate(
                 GenerationContext(seed=self._create_new_seed(random_seed))
             )
 
         if self.supervised:
-            supervised_consolidator = Consolidator(self.base_oscillations, self.anomalies)
+            supervised_consolidator = Consolidator(self.base_oscillations, self.anomalies,
+                supervised=self.supervised)
             self.supervised_timeseries, self.train_labels = supervised_consolidator.generate(
                 GenerationContext(seed=self._create_new_seed(random_seed))
             )
 
         return self
 
     def generate_with_dataframe(self, random_seed: Optional[int] = None) -> pd.DataFrame:
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/gutenTAG.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/gutenTAG.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/utils/compatibility.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/utils/compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 from ..utils.global_variables import BASE_OSCILLATION_NAMES, ANOMALY_TYPE_NAMES
 
 
 class Compatibility:
     combinations = pd.DataFrame(
         [
-            [1, 1, 1, 1, 1, 1, 0, 0, 0, 1, 1, 1],  # amplitude
-            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1],  # extremum
-            [1, 1, 1, 0, 0, 1, 0, 0, 0, 1, 1, 0],  # frequency
-            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1],  # mean
-            [1, 1, 1, 0, 1, 1, 0, 0, 0, 1, 1, 1],  # pattern
-            [1, 1, 1, 0, 0, 1, 0, 0, 0, 1, 1, 0],  # pattern_shift
-            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1],  # platform
-            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1],  # trend
-            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1],  # variance
-            [0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0],  # mode_correlation
+            [1, 1, 1, 1, 1, 1, 0, 0, 0, 1, 1, 1, 1],  # amplitude
+            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1],  # extremum
+            [1, 1, 1, 0, 0, 1, 0, 0, 0, 1, 1, 0, 0],  # frequency
+            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1],  # mean
+            [1, 1, 1, 0, 1, 1, 0, 0, 0, 1, 1, 1, 0],  # pattern
+            [1, 1, 1, 0, 0, 1, 0, 0, 0, 1, 1, 0, 0],  # pattern_shift
+            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1],  # platform
+            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1],  # trend
+            [1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1],  # variance
+            [0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0],  # mode_correlation
         ],
         columns=[BASE_OSCILLATION_NAMES.SINE, BASE_OSCILLATION_NAMES.COSINE, BASE_OSCILLATION_NAMES.SQUARE,
                  BASE_OSCILLATION_NAMES.RANDOM_WALK, BASE_OSCILLATION_NAMES.CYLINDER_BELL_FUNNEL,
                  BASE_OSCILLATION_NAMES.ECG, BASE_OSCILLATION_NAMES.POLYNOMIAL, BASE_OSCILLATION_NAMES.RANDOM_MODE_JUMP,
                  BASE_OSCILLATION_NAMES.FORMULA, BASE_OSCILLATION_NAMES.SAWTOOTH, BASE_OSCILLATION_NAMES.DIRICHLET,
-                 BASE_OSCILLATION_NAMES.MLS],
+                 BASE_OSCILLATION_NAMES.MLS, BASE_OSCILLATION_NAMES.CUSTOM_INPUT],
         index=[ANOMALY_TYPE_NAMES.AMPLITUDE, ANOMALY_TYPE_NAMES.EXTREMUM, ANOMALY_TYPE_NAMES.FREQUENCY,
                ANOMALY_TYPE_NAMES.MEAN, ANOMALY_TYPE_NAMES.PATTERN, ANOMALY_TYPE_NAMES.PATTERN_SHIFT,
                ANOMALY_TYPE_NAMES.PLATFORM, ANOMALY_TYPE_NAMES.TREND, ANOMALY_TYPE_NAMES.VARIANCE,
                ANOMALY_TYPE_NAMES.MODE_CORRELATION],
         dtype=bool
     )
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/utils/default_values.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/utils/default_values.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,20 @@
         PARAMETERS.CHANNEL_OFFSET: 1.0,
         PARAMETERS.RANDOM_SEED: None,
         PARAMETERS.FORMULA: None,
         PARAMETERS.ECG_SIM_METHOD: "simple",
         PARAMETERS.WIDTH: 1.0,
         PARAMETERS.DUTY: 0.5,
         PARAMETERS.PERIODICITY: 6,
-        PARAMETERS.COMPLEXITY: 7
+        PARAMETERS.COMPLEXITY: 7,
+        PARAMETERS.INPUT_TIMESERIES_PATH_TRAIN: None,
+        PARAMETERS.INPUT_TIMESERIES_PATH_TEST: None,
+        PARAMETERS.USE_COLUMN_TRAIN: None,
+        PARAMETERS.USE_COLUMN_TEST: None
     },
     ANOMALIES: {
         PARAMETERS.LENGTH: 200,
         PARAMETERS.POSITION: "middle",
         PARAMETERS.CHANNEL: 0,
-        PARAMETERS.CREEP_LENGTH: 0
+        PARAMETERS.CREEPING_LENGTH: 0
     }
 }
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/utils/global_variables.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/utils/global_variables.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     ECG = "ecg"
     POLYNOMIAL = "polynomial"
     RANDOM_MODE_JUMP = "random-mode-jump"
     FORMULA = "formula"
     SQUARE = "square"
     SAWTOOTH = "sawtooth"
     DIRICHLET = "dirichlet"
+    CUSTOM_INPUT = "custom-input"
 
 
 class ANOMALY_TYPE_NAMES:
     AMPLITUDE = "amplitude"
     EXTREMUM = "extremum"
     FREQUENCY = "frequency"
     MEAN = "mean"
@@ -61,20 +62,24 @@
     KIND = "kind"
     KINDS = "kinds"
     NAME = "name"
     CHANNELS = "channels"
     CHANNEL = "channel"
     POSITION = "position"
     EXACT_POSITION = "exact-position"
-    CREEP_LENGTH = "creep-length"
+    CREEPING_LENGTH = "creeping-length"
     ECG_SIM_METHOD = "ecg-sim-method"
     DUTY = "duty"
     WIDTH = "width"
     PERIODICITY = "periodicity"
     COMPLEXITY = "complexity"
+    INPUT_TIMESERIES_PATH_TRAIN = "input-timeseries-path-train"
+    INPUT_TIMESERIES_PATH_TEST = "input-timeseries-path-test"
+    USE_COLUMN_TRAIN = "use-column-train"
+    USE_COLUMN_TEST = "use-column-test"
 
 
 class CONFIG_SCHEMA:
     BASE_ID = "guten-tag-generation-config.schema.yaml"
     SCHEMA_DOMAIN = "https://example.com"
     SCHEMA_FOLDER_PATH = Path("generation-config-schema")
```

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/utils/logger.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/utils/logger.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/utils/tqdm_joblib.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/utils/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/gutenTAG/utils/types.py` & `timeeval-gutenTAG-1.4.0/gutenTAG/utils/types.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/logo_transparent.png` & `timeeval-gutenTAG-1.4.0/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/setup.cfg` & `timeeval-gutenTAG-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/setup.py` & `timeeval-gutenTAG-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/PKG-INFO` & `timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeeval-gutenTAG
-Version: 1.3.0
+Version: 1.4.0
 Summary: A good Timeseries Anomaly Generator.
 Home-page: https://github.com/HPI-Information-Systems/gutentag
 Author: Phillip Wenig and Sebastian Schmidl
 Author-email: phillip.wenig@hpi.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `timeeval-gutenTAG-1.3.0/timeeval_gutenTAG.egg-info/SOURCES.txt` & `timeeval-gutenTAG-1.4.0/timeeval_gutenTAG.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 gutenTAG/anomalies/types/trend.py
 gutenTAG/anomalies/types/variance.py
 gutenTAG/api/__init__.py
 gutenTAG/api/bo.py
 gutenTAG/base_oscillations/__init__.py
 gutenTAG/base_oscillations/base_oscillation.py
 gutenTAG/base_oscillations/cosine.py
+gutenTAG/base_oscillations/custom_input.py
 gutenTAG/base_oscillations/cylinder_bell_funnel.py
 gutenTAG/base_oscillations/dirichlet.py
 gutenTAG/base_oscillations/ecg.py
 gutenTAG/base_oscillations/formula.py
 gutenTAG/base_oscillations/interface.py
 gutenTAG/base_oscillations/mls.py
 gutenTAG/base_oscillations/polynomial.py
```

