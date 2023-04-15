# Comparing `tmp/salmon-triplets-1.0.0rc8.tar.gz` & `tmp/salmon-triplets-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salmon-triplets-1.0.0rc8.tar", last modified: Sat Dec 31 02:11:05 2022, max compression
+gzip compressed data, was "salmon-triplets-1.0.0rc9.tar", last modified: Sun Feb  5 01:47:59 2023, max compression
```

## Comparing `salmon-triplets-1.0.0rc8.tar` & `salmon-triplets-1.0.0rc9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      686 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/salmon/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.875285 salmon-triplets-1.0.0rc8/salmon/_out/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/_out/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/salmon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.875285 salmon-triplets-1.0.0rc8/salmon/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/backend/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15547 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/backend/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.875285 salmon-triplets-1.0.0rc8/salmon/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/frontend/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    34081 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/frontend/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/frontend/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.875285 salmon-triplets-1.0.0rc8/salmon/frontend/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/frontend/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/frontend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.875285 salmon-triplets-1.0.0rc8/salmon/triplets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/offline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.875285 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20216 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_adaptive_runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_round_robin.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/_noise_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/__triplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/gram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)    19737 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/tests/test_rr.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/samplers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/triplets/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/salmon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2022-12-31 02:11:05.000000 salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2022-12-31 02:11:05.000000 salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 02:11:05.000000 salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2022-12-31 02:11:05.000000 salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-31 02:11:05.000000 salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:11:05.879285 salmon-triplets-1.0.0rc8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_active_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_allowabe_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13196 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_passive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2022-12-31 02:10:56.000000 salmon-triplets-1.0.0rc8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.037382 salmon-triplets-1.0.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-05 01:47:59.037382 salmon-triplets-1.0.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.037382 salmon-triplets-1.0.0rc9/salmon/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.029382 salmon-triplets-1.0.0rc9/salmon/_out/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/_out/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-05 01:47:59.037382 salmon-triplets-1.0.0rc9/salmon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.029382 salmon-triplets-1.0.0rc9/salmon/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/backend/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/backend/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.029382 salmon-triplets-1.0.0rc9/salmon/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/frontend/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34081 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/frontend/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/frontend/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.029382 salmon-triplets-1.0.0rc9/salmon/frontend/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/frontend/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/frontend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.029382 salmon-triplets-1.0.0rc9/salmon/triplets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/offline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.033382 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20216 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_adaptive_runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_round_robin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.033382 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/_noise_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.033382 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/__triplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/gram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.033382 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19737 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.033382 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/tests/test_rr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/samplers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/triplets/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/salmon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.037382 salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-05 01:47:59.000000 salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-02-05 01:47:59.000000 salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 01:47:59.000000 salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-05 01:47:59.000000 salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-05 01:47:59.000000 salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-02-05 01:47:59.037382 salmon-triplets-1.0.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:59.037382 salmon-triplets-1.0.0rc9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_active_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_allowabe_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13196 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_passive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-02-05 01:47:41.000000 salmon-triplets-1.0.0rc9/versioneer.py
```

### Comparing `salmon-triplets-1.0.0rc8/LICENSE.txt` & `salmon-triplets-1.0.0rc9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/PKG-INFO` & `salmon-triplets-1.0.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salmon-triplets
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Efficient crowdsourcing for ordinal embeddings
 Home-page: https://docs.stsievert.com/salmon
 Author: Scott Sievert
 Author-email: salmon@stsievert.com
 License: BSD 3-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `salmon-triplets-1.0.0rc8/README.md` & `salmon-triplets-1.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/backend/core.py` & `salmon-triplets-1.0.0rc9/salmon/backend/core.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/backend/sampler.py` & `salmon-triplets-1.0.0rc9/salmon/backend/sampler.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/frontend/plotting.py` & `salmon-triplets-1.0.0rc9/salmon/frontend/plotting.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/frontend/private.py` & `salmon-triplets-1.0.0rc9/salmon/frontend/private.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/frontend/public.py` & `salmon-triplets-1.0.0rc9/salmon/frontend/public.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/frontend/utils.py` & `salmon-triplets-1.0.0rc9/salmon/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/manager.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/manager.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/offline.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/offline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 from copy import copy, deepcopy
 from numbers import Number
 from time import time
-from typing import Dict, Union
+from typing import Dict, Union, List, Any
 
 import numpy as np
 import pandas as pd
 import torch
 import torch.optim as optim
 from sklearn.base import BaseEstimator
 from sklearn.exceptions import NotFittedError
@@ -30,14 +30,22 @@
     if isinstance(v, (str, int)):
         return v
     if isinstance(v, (float, np.floating)):
         return f"{v:0.3f}"
     return v
 
 
+def join(embedding: np.ndarray, targets: List[Any]) -> pd.DataFrame:
+    em_final = pd.DataFrame(embedding)
+    dims = {0: "x", 1: "y", 2: "z"}
+    em_final.columns = [dims.get(c, f"dim{c + 1}") for c in em_final.columns]
+    em_final["target"] = targets
+    return em_final
+
+
 class OfflineEmbedding(BaseEstimator):
     """
     Generate an embedding offline (after responses are downloaded from Salmon).
 
     Parameters
     ----------
     n : int
```

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_adaptive_runners.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_adaptive_runners.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_random_sampling.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_random_sampling.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_round_robin.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_round_robin.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/_validation.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/_validation.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/_embed.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/_embed.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/_noise_models.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/_noise_models.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/_score.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/_score.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/__triplets.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/__triplets.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/_search.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/_search.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/gram_utils.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/gram_utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/test_gram_utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/test_search_refactor.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/test_uncertainty.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/samplers/adaptive/search/tests/utilsSTE.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/triplets/test_config.py` & `salmon-triplets-1.0.0rc9/salmon/triplets/test_config.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon/utils.py` & `salmon-triplets-1.0.0rc9/salmon/utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/PKG-INFO` & `salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salmon-triplets
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Efficient crowdsourcing for ordinal embeddings
 Home-page: https://docs.stsievert.com/salmon
 Author: Scott Sievert
 Author-email: salmon@stsievert.com
 License: BSD 3-clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `salmon-triplets-1.0.0rc8/salmon_triplets.egg-info/SOURCES.txt` & `salmon-triplets-1.0.0rc9/salmon_triplets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/setup.cfg` & `salmon-triplets-1.0.0rc9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 	scipy
 	pandas>=1.0.1
 	Cython
 	scikit-learn
 	skorch>=0.8.0
 	torch
 	pydantic
+	PyYAML
 tests_require = pytest
 
 [options.extras_require]
 server = 
 	fastparquet
 	bokeh==2.0.1
 	jinja2<3.1.0
```

### Comparing `salmon-triplets-1.0.0rc8/tests/test_active.py` & `salmon-triplets-1.0.0rc9/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/tests/test_active_search.py` & `salmon-triplets-1.0.0rc9/tests/test_active_search.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/tests/test_allowabe_targets.py` & `salmon-triplets-1.0.0rc9/tests/test_allowabe_targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 @pytest.mark.parametrize("sampler", ["RoundRobin", "Random"])
 def test_targets(sampler, server):
     samplers = {sampler: {"targets": [0, 2, 4]}, "Test": {"class": "Random"}}
     config = {"samplers": samplers, "targets": 5}
     server.authorize()
     server.post("/init_exp", data={"exp": config})
 
-    for k in range(20):
+    for k in range(30):
         q = server.get("/query").json()
         ans = {"winner": random.choice([q["left"], q["right"]]), "puid": "foo", **q}
         server.post("/answer", json=ans)
     r = server.get("/responses")
     df = pd.DataFrame(r.json())
 
     allow = df.loc[df.sampler == sampler, ["left", "right", "head"]].to_numpy()
```

### Comparing `salmon-triplets-1.0.0rc8/tests/test_backend.py` & `salmon-triplets-1.0.0rc9/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/tests/test_basic.py` & `salmon-triplets-1.0.0rc9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/tests/test_examples.py` & `salmon-triplets-1.0.0rc9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/tests/test_offline.py` & `salmon-triplets-1.0.0rc9/tests/test_offline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from pathlib import Path
+import yaml
 
 import numpy as np
 import numpy.linalg as LA
 import pandas as pd
 import pytest
 from sklearn.model_selection import train_test_split
 
 from salmon.triplets.offline import OfflineEmbedding
 from salmon.triplets.samplers import TSTE
+import salmon.triplets.offline
 
 
 def test_salmon_import():
-    """ This test makes sure that no errors are raised on import
+    """This test makes sure that no errors are raised on import
     (non-existant directories, etc)"""
     import salmon
 
     return True
 
 
 def test_score_predict_basic():
@@ -45,15 +47,15 @@
 
     # Make sure perfect accuracy if the output aligns with the embedding
     assert np.allclose(alg.score(X, y_hat), 1)
 
     # Make sure the score has the expected value (winner has minimum distance)
     embed = alg.opt.embedding() * 1e3
     y_hat2 = []
-    for (head, left, right) in X:
+    for head, left, right in X:
         ldist = LA.norm(embed[head] - embed[left])
         rdist = LA.norm(embed[head] - embed[right])
 
         left_wins = ldist <= rdist
         y_hat2.append(0 if left_wins else 1)
 
     assert y_hat.tolist() == y_hat2
@@ -104,11 +106,31 @@
     est.initialize(X, embedding=em)
 
     assert np.allclose(est.embedding_, em)
     est.partial_fit(X)
     assert not np.allclose(est.embedding_, em), "Embedding didn't change"
 
 
+def test_offline_names_correct():
+    DIR = Path(__file__).absolute().parent
+    _f = DIR / "data" / "active.yaml"
+    config = yaml.load(_f.read_text(), Loader=yaml.SafeLoader)
+    n = len(config["targets"])
+    d = config["sampling"]["common"]["d"]
+
+    X = np.random.choice(n, size=(100, 3))
+    est = OfflineEmbedding(n=n, d=d)
+    est.partial_fit(X)
+
+    import salmon.triplets.offline as offline
+
+    em = offline.join(est.embedding_, config["targets"])
+    assert isinstance(em, pd.DataFrame)
+    assert len(em) == len(config["targets"])
+    assert set(em.columns) == {"x", "y", "target"}
+    assert (em["target"] == config["targets"]).all()
+
+
 if __name__ == "__main__":
     test_offline_init()
     test_offline_embedding_random_state()
     test_offline_embedding()
```

### Comparing `salmon-triplets-1.0.0rc8/tests/test_passive.py` & `salmon-triplets-1.0.0rc9/tests/test_passive.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/tests/test_validation.py` & `salmon-triplets-1.0.0rc9/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/tests/utils.py` & `salmon-triplets-1.0.0rc9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `salmon-triplets-1.0.0rc8/versioneer.py` & `salmon-triplets-1.0.0rc9/versioneer.py`

 * *Files identical despite different names*

