# Comparing `tmp/subaligner-0.3.0.tar.gz` & `tmp/subaligner-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/subaligner-0.3.0.tar", last modified: Fri Mar 10 19:53:30 2023, max compression
+gzip compressed data, was "dist/subaligner-0.3.1.tar", last modified: Sat Apr 15 17:24:02 2023, max compression
```

## Comparing `subaligner-0.3.0.tar` & `subaligner-0.3.1.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/
--rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.0/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.0/MANIFEST.in
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-03-10 19:53:30.000000 subaligner-0.3.0/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     9199 2023-03-07 23:41:55.000000 subaligner-0.3.0/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/bin/
--rwxr-xr-x   0 macbook    (501) staff       (20)    21172 2023-03-07 23:41:55.000000 subaligner-0.3.0/bin/subaligner
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-07 23:41:55.000000 subaligner-0.3.0/bin/subaligner_1pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-07 23:41:55.000000 subaligner-0.3.0/bin/subaligner_2pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    13332 2023-03-07 23:41:55.000000 subaligner-0.3.0/bin/subaligner_batch
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-07 23:41:55.000000 subaligner-0.3.0/bin/subaligner_convert
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.0/bin/subaligner_train
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.0/bin/subaligner_tune
--rw-r--r--   0 macbook    (501) staff       (20)     1229 2023-03-07 23:41:51.000000 subaligner-0.3.0/requirements.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-03-10 19:53:30.000000 subaligner-0.3.0/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     3728 2023-03-07 23:41:55.000000 subaligner-0.3.0/setup.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/
--rw-r--r--   0 macbook    (501) staff       (20)      174 2023-03-07 23:41:51.000000 subaligner-0.3.0/subaligner/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    21172 2023-03-07 23:41:55.000000 subaligner-0.3.0/subaligner/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)       64 2023-03-10 16:22:53.000000 subaligner-0.3.0/subaligner/_version.py
--rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/embedder.py
--rw-r--r--   0 macbook    (501) staff       (20)      410 2023-03-07 23:41:55.000000 subaligner-0.3.0/subaligner/exception.py
--rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/hparam_tuner.py
--rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/hyperparameters.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/lib/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/lib/language.py
--rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/lib/to_srt.py
--rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)    18067 2023-03-07 23:41:51.000000 subaligner-0.3.0/subaligner/media_helper.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/models/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/models/training/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/models/training/config/
--rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/models/training/config/hyperparameters.json
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/models/training/model/
--rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/models/training/model/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/models/training/model/model.hdf5
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/models/training/weights/
--rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/models/training/weights/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/models/training/weights/weights.hdf5
--rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/network.py
--rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 10:25:31.000000 subaligner-0.3.0/subaligner/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/singleton.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/subaligner_1pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/subaligner_1pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-07 23:41:55.000000 subaligner-0.3.0/subaligner/subaligner_1pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/subaligner_2pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/subaligner_2pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-07 23:41:55.000000 subaligner-0.3.0/subaligner/subaligner_2pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/subaligner_batch/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/subaligner_batch/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    13332 2023-03-07 23:41:55.000000 subaligner-0.3.0/subaligner/subaligner_batch/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/subaligner_convert/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/subaligner_convert/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-07 23:41:55.000000 subaligner-0.3.0/subaligner/subaligner_convert/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/subaligner_train/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/subaligner_train/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.0/subaligner/subaligner_train/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner/subaligner_tune/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/subaligner_tune/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.0/subaligner/subaligner_tune/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-03-07 23:41:55.000000 subaligner-0.3.0/subaligner/subtitle.py
--rw-r--r--   0 macbook    (501) staff       (20)    15843 2023-03-07 23:41:51.000000 subaligner-0.3.0/subaligner/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     5386 2023-03-07 11:48:49.000000 subaligner-0.3.0/subaligner/transcriber.py
--rw-r--r--   0 macbook    (501) staff       (20)     9711 2023-03-07 23:41:51.000000 subaligner-0.3.0/subaligner/translator.py
--rw-r--r--   0 macbook    (501) staff       (20)    32196 2022-05-10 00:20:59.000000 subaligner-0.3.0/subaligner/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     9974 2023-03-10 19:53:29.000000 subaligner-0.3.0/subaligner.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1610 2023-03-10 19:53:30.000000 subaligner-0.3.0/subaligner.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-03-10 19:53:29.000000 subaligner-0.3.0/subaligner.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      424 2023-03-10 19:53:29.000000 subaligner-0.3.0/subaligner.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)     2132 2023-03-10 19:53:29.000000 subaligner-0.3.0/subaligner.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-03-10 19:53:29.000000 subaligner-0.3.0/subaligner.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.488037 subaligner-0.3.1/
+-rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.1/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.1/MANIFEST.in
+-rw-r--r--   0 macbook    (501) staff       (20)    10178 2023-04-15 17:24:02.487525 subaligner-0.3.1/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     9403 2023-04-15 17:08:17.000000 subaligner-0.3.1/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.360554 subaligner-0.3.1/bin/
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.1/bin/subaligner
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.1/bin/subaligner_1pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.1/bin/subaligner_2pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    16659 2023-04-15 17:17:05.000000 subaligner-0.3.1/bin/subaligner_batch
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.1/bin/subaligner_convert
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.1/bin/subaligner_train
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.1/bin/subaligner_tune
+-rw-r--r--   0 macbook    (501) staff       (20)     1181 2023-03-29 00:31:58.000000 subaligner-0.3.1/requirements.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-04-15 17:24:02.488249 subaligner-0.3.1/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     3728 2023-03-10 19:10:53.000000 subaligner-0.3.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.446659 subaligner-0.3.1/subaligner/
+-rw-r--r--   0 macbook    (501) staff       (20)      258 2023-03-11 16:33:37.000000 subaligner-0.3.1/subaligner/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.1/subaligner/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)       64 2023-03-12 11:44:17.000000 subaligner-0.3.1/subaligner/_version.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/embedder.py
+-rw-r--r--   0 macbook    (501) staff       (20)      511 2023-03-11 23:58:14.000000 subaligner-0.3.1/subaligner/exception.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/hparam_tuner.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/hyperparameters.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.460981 subaligner-0.3.1/subaligner/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/lib/language.py
+-rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/lib/to_srt.py
+-rw-r--r--   0 macbook    (501) staff       (20)      709 2023-03-19 19:33:51.000000 subaligner-0.3.1/subaligner/llm.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)    18286 2023-03-17 01:31:21.000000 subaligner-0.3.1/subaligner/media_helper.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.351528 subaligner-0.3.1/subaligner/models/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.352181 subaligner-0.3.1/subaligner/models/training/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.462404 subaligner-0.3.1/subaligner/models/training/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/config/hyperparameters.json
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.464136 subaligner-0.3.1/subaligner/models/training/model/
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/model/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/model/model.hdf5
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.472381 subaligner-0.3.1/subaligner/models/training/weights/
+-rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/weights/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/weights/weights.hdf5
+-rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/network.py
+-rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/singleton.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.481047 subaligner-0.3.1/subaligner/subaligner_1pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_1pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/subaligner_1pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.482266 subaligner-0.3.1/subaligner/subaligner_2pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_2pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/subaligner_2pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.483305 subaligner-0.3.1/subaligner/subaligner_batch/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_batch/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    16659 2023-04-15 17:17:05.000000 subaligner-0.3.1/subaligner/subaligner_batch/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.484162 subaligner-0.3.1/subaligner/subaligner_convert/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_convert/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/subaligner_convert/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.485320 subaligner-0.3.1/subaligner/subaligner_train/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_train/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.1/subaligner/subaligner_train/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.486733 subaligner-0.3.1/subaligner/subaligner_tune/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_tune/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_tune/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-04-15 16:48:57.000000 subaligner-0.3.1/subaligner/subtitle.py
+-rw-r--r--   0 macbook    (501) staff       (20)    15843 2023-03-07 23:41:51.000000 subaligner-0.3.1/subaligner/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4695 2023-03-21 00:12:01.000000 subaligner-0.3.1/subaligner/transcriber.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12131 2023-03-28 22:20:16.000000 subaligner-0.3.1/subaligner/translator.py
+-rw-r--r--   0 macbook    (501) staff       (20)    33741 2023-03-17 02:05:09.000000 subaligner-0.3.1/subaligner/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.458857 subaligner-0.3.1/subaligner.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    10178 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1628 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      424 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)     2084 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `subaligner-0.3.0/LICENSE` & `subaligner-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/PKG-INFO` & `subaligner-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subaligner
-Version: 0.3.0
+Version: 0.3.1
 Summary: Automatically synchronize and translate subtitles with pretrained deep neural networks, forced alignments and transformers.
 Home-page: https://subaligner.readthedocs.io/en/latest/
 Author: Xi Bai
 Author-email: xi.bai.ed@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -22,42 +22,51 @@
 License-File: LICENSE
 
 <div align="center">
   <img src="./figures/subaligner.png" alt="subaligner" width="300" />
 </div>
 
 [![Build Status](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml/badge.svg?branch=master)](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml?query=branch%3Amaster) ![Codecov](https://img.shields.io/codecov/c/github/baxtree/subaligner)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/) [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/subaligner/badge/?version=latest)](https://subaligner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/baxtree/subaligner)](https://github.com/baxtree/subaligner/blob/master/LICENSE)
 [![PyPI](https://badge.fury.io/py/subaligner.svg)](https://badge.fury.io/py/subaligner)
 [![Docker Build](https://img.shields.io/docker/cloud/build/baxtree/subaligner?label=Docker&style=flat)](https://hub.docker.com/r/baxtree/subaligner/builds)
 [![Docker Pulls](https://img.shields.io/docker/pulls/baxtree/subaligner)](https://hub.docker.com/r/baxtree/subaligner)
 [![Citation](https://zenodo.org/badge/228440472.svg)](https://doi.org/10.5281/zenodo.5603083)
 
 ## Supported Formats
 Subtitle: SubRip, TTML, WebVTT, (Advanced) SubStation Alpha, MicroDVD, MPL2, TMP, EBU STL, SAMI, SCC and SBV.
 
 Video/Audio: MP4, WebM, Ogg, 3GP, FLV, MOV, Matroska, MPEG TS, WAV, MP3, AAC, FLAC, etc.
 
+:information_source: <small style="line-height: 1.2;">Subaligner relies on file extensions as default hints to process a wide range of audiovisual or subtitle formats. It is recommended to use extensions widely acceppted by the community to ensure compatibility.</small>
+
 ## Dependencies
 Required by basic: [FFmpeg](https://www.ffmpeg.org/)
 ```
 $ apt-get install ffmpeg
 ```
 or
 ```
 $ brew install ffmpeg
 ```
 
 ## Basic Installation
 ```
-$ pip install -U pip
+$ pip install -U pip && pip install -U setuptools
 $ pip install subaligner
 ```
+or install from source:
+```
+$ git clone git@github.com:baxtree/subaligner.git && cd subaligner
+$ pip install -U pip && pip install -U setuptools
+$ python setup.py install
+```
+:information_source: <small style="line-height: 1.2;">It is highly recommended creating a virtual environment prior to installation.</small>
 
 ## Installation with Optional Packages Supporting Additional Features
 ```
 # Install dependencies for enabling translation and transcription
 
 $ pip install 'subaligner[llm]'
 ```
@@ -80,73 +89,44 @@
 $ brew install espeak
 ```
 To install all supported features:
 ```
 $ pip install 'subaligner[harmony]'
 ```
 
-## Alternative Installations
-```
-# Install via pipx
-$ pip install -U pip pipx
-$ pipx install subaligner
-```
-or
-```
-# Install from GitHub via Pipenv
-$ pipenv install subaligner
-$ pipenv install 'subaligner[stretch]'
-$ pipenv install 'subaligner[dev]'
-```
-or
-```
-# Install from source
+## Container Support
+If you prefer using a containerised environment over installing everything locally, run:
 
-$ git clone git@github.com:baxtree/subaligner.git
-$ cd subaligner
-$ python setup.py install
-```
-or
 ```
-# Use dockerised installation
-
 $ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner bash
 ```
 For users on Windows 10: [Docker Desktop](https://docs.docker.com/docker-for-windows/install/) is the only option at present.
 Assuming your media assets are stored under `d:\media`, open built-in command prompt, PowerShell, or Windows Terminal and run:
 ```
 docker pull baxtree/subaligner
 docker run -v "/d/media":/media -w "/media" -it baxtree/subaligner bash
 ```
 
 ## Usage
 ```
 # Single-stage alignment (high-level shift with lower latency)
 
-$ subaligner_1pass -v video.mp4 -s subtitle.srt
-$ subaligner_1pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ subaligner -m single -v video.mp4 -s subtitle.srt
+$ subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
 ```
 # Dual-stage alignment (low-level shift with higher latency)
 
-$ subaligner_2pass -v video.mp4 -s subtitle.srt
-$ subaligner_2pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
-```
-or
-```
-# Pass in single-stage or dual-stage as the alignment mode
-
-$ subaligner -m single -v video.mp4 -s subtitle.srt
 $ subaligner -m dual -v video.mp4 -s subtitle.srt
-$ subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 $ subaligner -m dual -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
 ```
 # Generate subtitles by transcribing audiovisual files
 $ subaligner -m transcribe -v video.mp4 -ml eng -mr whisper -mf small -o subtitle_aligned.srt
+$ subaligner -m transcribe -v video.mp4 -ml zho -mr whisper -mf medium -o subtitle_aligned.srt
 ```
 ```
 # Alignment on segmented plain texts (double newlines as the delimiter)
 
 $ subaligner -m script -v test.mp4 -s subtitle.txt -o subtitle_aligned.srt
 $ subaligner -m script -v https://example.com/video.mp4 -s https://example.com/subtitle.txt -o subtitle_aligned.srt
 ```
@@ -160,19 +140,27 @@
 # Alignment on embedded subtitles
 
 $ subaligner -m single -v video.mkv -s embedded:stream_index=0 -o subtitle_aligned.srt
 $ subaligner -m dual -v video.mkv -s embedded:stream_index=0 -o subtitle_aligned.srt
 ```
 ```
 # Translative alignment with the ISO 639-3 language code pair (src,tgt)
+
 $ subaligner --languages
 $ subaligner -m single -v video.mp4 -s subtitle.srt -t src,tgt
 $ subaligner -m dual -v video.mp4 -s subtitle.srt -t src,tgt
 $ subaligner -m script -v test.mp4 -s subtitle.txt -o subtitle_aligned.srt -t src,tgt
-$ subaligner -m transcribe -v video.mp4 -ml eng -mr whisper -mf small -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr helsinki-nlp -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr facebook-mbart -tf large -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr whisper -tf small -o subtitle_aligned.srt -t src,eng
+```
+```
+# Transcribe audiovisual files and generate translated subtitles
+
+$ subaligner -m transcribe -v video.mp4 -ml src -mr whisper -mf small -tr helsinki-nlp -o subtitle_aligned.srt -t src,tgt
 ```
 ```
 # Shift subtitle manually by offset in seconds
 
 $ subaligner -m shift --subtitle_path subtitle.srt -os 5.5
 $ subaligner -m shift --subtitle_path subtitle.srt -os -5.5 -o subtitle_shifted.srt
 ```
@@ -189,28 +177,25 @@
 $ pipx run subaligner -m single -v video.mp4 -s subtitle.srt
 $ pipx run subaligner -m dual -v video.mp4 -s subtitle.srt
 ```
 ```
 # Run the module as a script
 $ python -m subaligner -m single -v video.mp4 -s subtitle.srt
 $ python -m subaligner -m dual -v video.mp4 -s subtitle.srt
-$ python -m subaligner.subaligner_1pass -v video.mp4 -s subtitle.srt
-$ python -m subaligner.subaligner_2pass -v video.mp4 -s subtitle.srt
 ```
 ```
 # Run alignments with the docker image
 
 $ docker pull baxtree/subaligner
-$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner_1pass -v video.mp4 -s subtitle.srt
-$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner_2pass -v video.mp4 -s subtitle.srt
-$ docker run -it baxtree/subaligner subaligner_1pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
-$ docker run -it baxtree/subaligner subaligner_2pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner -m single -v video.mp4 -s subtitle.srt
+$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner -m dual -v video.mp4 -s subtitle.srt
+$ docker run -it baxtree/subaligner subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ docker run -it baxtree/subaligner subaligner -m dual -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
-The aligned subtitle will be saved at `subtitle_aligned.srt`. For details on CLI, run `subaligner_1pass -h`, `subaligner_2pass -h` or `subaligner -h`.
-Additional utilities can be used after consulting `subaligner_batch -h`, `subaligner_convert -h`, `subaligner_train -h` and `subaligner_tune -h`.
+The aligned subtitle will be saved at `subtitle_aligned.srt`. For details on CLIs, run `subaligner -h` or `subaligner_batch -h`, `subaligner_convert -h`, `subaligner_train -h` and `subaligner_tune -h` for additional utilities. `subaligner_1pass` and `subaligner_2pass` are shortcuts for running `subaligner` with `-m single` and `-m dual` options, respectively.
 
 ![](figures/screencast.gif)
 
 ## Advanced Usage
 You can train a new model with your own audiovisual files and subtitle files:
 ```
 $ subaligner_train -vd VIDEO_DIRECTORY -sd SUBTITLE_DIRECTORY -tod TRAINING_OUTPUT_DIRECTORY
```

### Comparing `subaligner-0.3.0/README.md` & `subaligner-0.3.1/subaligner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,72 @@
+Metadata-Version: 2.1
+Name: subaligner
+Version: 0.3.1
+Summary: Automatically synchronize and translate subtitles with pretrained deep neural networks, forced alignments and transformers.
+Home-page: https://subaligner.readthedocs.io/en/latest/
+Author: Xi Bai
+Author-email: xi.bai.ed@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: harmony
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: stretch
+Provides-Extra: translation
+Provides-Extra: llm
+License-File: LICENSE
+
 <div align="center">
   <img src="./figures/subaligner.png" alt="subaligner" width="300" />
 </div>
 
 [![Build Status](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml/badge.svg?branch=master)](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml?query=branch%3Amaster) ![Codecov](https://img.shields.io/codecov/c/github/baxtree/subaligner)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/) [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/subaligner/badge/?version=latest)](https://subaligner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/baxtree/subaligner)](https://github.com/baxtree/subaligner/blob/master/LICENSE)
 [![PyPI](https://badge.fury.io/py/subaligner.svg)](https://badge.fury.io/py/subaligner)
 [![Docker Build](https://img.shields.io/docker/cloud/build/baxtree/subaligner?label=Docker&style=flat)](https://hub.docker.com/r/baxtree/subaligner/builds)
 [![Docker Pulls](https://img.shields.io/docker/pulls/baxtree/subaligner)](https://hub.docker.com/r/baxtree/subaligner)
 [![Citation](https://zenodo.org/badge/228440472.svg)](https://doi.org/10.5281/zenodo.5603083)
 
 ## Supported Formats
 Subtitle: SubRip, TTML, WebVTT, (Advanced) SubStation Alpha, MicroDVD, MPL2, TMP, EBU STL, SAMI, SCC and SBV.
 
 Video/Audio: MP4, WebM, Ogg, 3GP, FLV, MOV, Matroska, MPEG TS, WAV, MP3, AAC, FLAC, etc.
 
+:information_source: <small style="line-height: 1.2;">Subaligner relies on file extensions as default hints to process a wide range of audiovisual or subtitle formats. It is recommended to use extensions widely acceppted by the community to ensure compatibility.</small>
+
 ## Dependencies
 Required by basic: [FFmpeg](https://www.ffmpeg.org/)
 ```
 $ apt-get install ffmpeg
 ```
 or
 ```
 $ brew install ffmpeg
 ```
 
 ## Basic Installation
 ```
-$ pip install -U pip
+$ pip install -U pip && pip install -U setuptools
 $ pip install subaligner
 ```
+or install from source:
+```
+$ git clone git@github.com:baxtree/subaligner.git && cd subaligner
+$ pip install -U pip && pip install -U setuptools
+$ python setup.py install
+```
+:information_source: <small style="line-height: 1.2;">It is highly recommended creating a virtual environment prior to installation.</small>
 
 ## Installation with Optional Packages Supporting Additional Features
 ```
 # Install dependencies for enabling translation and transcription
 
 $ pip install 'subaligner[llm]'
 ```
@@ -57,73 +89,44 @@
 $ brew install espeak
 ```
 To install all supported features:
 ```
 $ pip install 'subaligner[harmony]'
 ```
 
-## Alternative Installations
-```
-# Install via pipx
-$ pip install -U pip pipx
-$ pipx install subaligner
-```
-or
-```
-# Install from GitHub via Pipenv
-$ pipenv install subaligner
-$ pipenv install 'subaligner[stretch]'
-$ pipenv install 'subaligner[dev]'
-```
-or
-```
-# Install from source
+## Container Support
+If you prefer using a containerised environment over installing everything locally, run:
 
-$ git clone git@github.com:baxtree/subaligner.git
-$ cd subaligner
-$ python setup.py install
-```
-or
 ```
-# Use dockerised installation
-
 $ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner bash
 ```
 For users on Windows 10: [Docker Desktop](https://docs.docker.com/docker-for-windows/install/) is the only option at present.
 Assuming your media assets are stored under `d:\media`, open built-in command prompt, PowerShell, or Windows Terminal and run:
 ```
 docker pull baxtree/subaligner
 docker run -v "/d/media":/media -w "/media" -it baxtree/subaligner bash
 ```
 
 ## Usage
 ```
 # Single-stage alignment (high-level shift with lower latency)
 
-$ subaligner_1pass -v video.mp4 -s subtitle.srt
-$ subaligner_1pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ subaligner -m single -v video.mp4 -s subtitle.srt
+$ subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
 ```
 # Dual-stage alignment (low-level shift with higher latency)
 
-$ subaligner_2pass -v video.mp4 -s subtitle.srt
-$ subaligner_2pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
-```
-or
-```
-# Pass in single-stage or dual-stage as the alignment mode
-
-$ subaligner -m single -v video.mp4 -s subtitle.srt
 $ subaligner -m dual -v video.mp4 -s subtitle.srt
-$ subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 $ subaligner -m dual -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
 ```
 # Generate subtitles by transcribing audiovisual files
 $ subaligner -m transcribe -v video.mp4 -ml eng -mr whisper -mf small -o subtitle_aligned.srt
+$ subaligner -m transcribe -v video.mp4 -ml zho -mr whisper -mf medium -o subtitle_aligned.srt
 ```
 ```
 # Alignment on segmented plain texts (double newlines as the delimiter)
 
 $ subaligner -m script -v test.mp4 -s subtitle.txt -o subtitle_aligned.srt
 $ subaligner -m script -v https://example.com/video.mp4 -s https://example.com/subtitle.txt -o subtitle_aligned.srt
 ```
@@ -137,19 +140,27 @@
 # Alignment on embedded subtitles
 
 $ subaligner -m single -v video.mkv -s embedded:stream_index=0 -o subtitle_aligned.srt
 $ subaligner -m dual -v video.mkv -s embedded:stream_index=0 -o subtitle_aligned.srt
 ```
 ```
 # Translative alignment with the ISO 639-3 language code pair (src,tgt)
+
 $ subaligner --languages
 $ subaligner -m single -v video.mp4 -s subtitle.srt -t src,tgt
 $ subaligner -m dual -v video.mp4 -s subtitle.srt -t src,tgt
 $ subaligner -m script -v test.mp4 -s subtitle.txt -o subtitle_aligned.srt -t src,tgt
-$ subaligner -m transcribe -v video.mp4 -ml eng -mr whisper -mf small -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr helsinki-nlp -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr facebook-mbart -tf large -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr whisper -tf small -o subtitle_aligned.srt -t src,eng
+```
+```
+# Transcribe audiovisual files and generate translated subtitles
+
+$ subaligner -m transcribe -v video.mp4 -ml src -mr whisper -mf small -tr helsinki-nlp -o subtitle_aligned.srt -t src,tgt
 ```
 ```
 # Shift subtitle manually by offset in seconds
 
 $ subaligner -m shift --subtitle_path subtitle.srt -os 5.5
 $ subaligner -m shift --subtitle_path subtitle.srt -os -5.5 -o subtitle_shifted.srt
 ```
@@ -166,28 +177,25 @@
 $ pipx run subaligner -m single -v video.mp4 -s subtitle.srt
 $ pipx run subaligner -m dual -v video.mp4 -s subtitle.srt
 ```
 ```
 # Run the module as a script
 $ python -m subaligner -m single -v video.mp4 -s subtitle.srt
 $ python -m subaligner -m dual -v video.mp4 -s subtitle.srt
-$ python -m subaligner.subaligner_1pass -v video.mp4 -s subtitle.srt
-$ python -m subaligner.subaligner_2pass -v video.mp4 -s subtitle.srt
 ```
 ```
 # Run alignments with the docker image
 
 $ docker pull baxtree/subaligner
-$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner_1pass -v video.mp4 -s subtitle.srt
-$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner_2pass -v video.mp4 -s subtitle.srt
-$ docker run -it baxtree/subaligner subaligner_1pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
-$ docker run -it baxtree/subaligner subaligner_2pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner -m single -v video.mp4 -s subtitle.srt
+$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner -m dual -v video.mp4 -s subtitle.srt
+$ docker run -it baxtree/subaligner subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ docker run -it baxtree/subaligner subaligner -m dual -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
-The aligned subtitle will be saved at `subtitle_aligned.srt`. For details on CLI, run `subaligner_1pass -h`, `subaligner_2pass -h` or `subaligner -h`.
-Additional utilities can be used after consulting `subaligner_batch -h`, `subaligner_convert -h`, `subaligner_train -h` and `subaligner_tune -h`.
+The aligned subtitle will be saved at `subtitle_aligned.srt`. For details on CLIs, run `subaligner -h` or `subaligner_batch -h`, `subaligner_convert -h`, `subaligner_train -h` and `subaligner_tune -h` for additional utilities. `subaligner_1pass` and `subaligner_2pass` are shortcuts for running `subaligner` with `-m single` and `-m dual` options, respectively.
 
 ![](figures/screencast.gif)
 
 ## Advanced Usage
 You can train a new model with your own audiovisual files and subtitle files:
 ```
 $ subaligner_train -vd VIDEO_DIRECTORY -sd SUBTITLE_DIRECTORY -tod TRAINING_OUTPUT_DIRECTORY
@@ -214,7 +222,9 @@
 [pysrt](https://github.com/byroot/pysrt)
 [pysubs2](https://github.com/tkarabela/pysubs2)
 [aeneas](https://www.readbeyond.it/aeneas/)
 [transformers](https://huggingface.co/transformers/)
 [openai-whisper](https://github.com/openai/whisper).
 
 Thanks to Alan Robinson and Nigel Megitt for their invaluable feedback.
+
+
```

### Comparing `subaligner-0.3.0/bin/subaligner` & `subaligner-0.3.1/bin/subaligner`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 """
 usage: subaligner [-h] [-m {single,dual,script,shift,transcribe}] [-v VIDEO_PATH] [-s SUBTITLE_PATH [SUBTITLE_PATH ...]] [-l MAX_LOGLOSS] [-so]
                   [-sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
                   [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-o OUTPUT] [-t TRANSLATE] [-os OFFSET_SECONDS]
                   [-ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
-                  [-mr {whisper}] [-mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}] [-lgs] [-d] [-q] [-ver]
+                  [-mr {whisper}] [-mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}] [-tr {helsinki-nlp,whisper,facebook-mbart}]
+                  [-tf TRANSLATION_FLAVOUR] [-lgs] [-d] [-q] [-ver]
 
 Subaligner command line interface
 
 optional arguments:
   -h, --help            show this help message and exit
   -s SUBTITLE_PATH [SUBTITLE_PATH ...], --subtitle_path SUBTITLE_PATH [SUBTITLE_PATH ...]
-                        File path or URL to the subtitle file (Extensions of supported subtitles: .ssa, .vtt, .srt, .txt, .smi, .ytt, .sub, .xml, .sbv, .ass, .sami, .scc, .tmp, .stl, .ttml, .dfxp) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)
+                        File path or URL to the subtitle file (Extensions of supported subtitles: .ttml, .ssa, .stl, .sbv, .dfxp, .srt, .txt, .ytt, .vtt, .sub, .sami, .xml, .scc, .ass, .smi, .tmp) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)
   -l MAX_LOGLOSS, --max_logloss MAX_LOGLOSS
                         Max global log loss for alignment
   -so, --stretch_on     Switch on stretch on subtitles)
   -sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --stretch_in_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].
                         NB: This will be ignored if neither -so nor --stretch_on is present
   -fos, --exit_segfail  Exit on any segment alignment failures
@@ -25,18 +26,22 @@
                         Path to the output subtitle file
   -t TRANSLATE, --translate TRANSLATE
                         Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)
   -os OFFSET_SECONDS, --offset_seconds OFFSET_SECONDS
                         Offset by which the subtitle will be shifted
   -ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --main_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]
-  -mr {whisper}, --llm_recipe {whisper}
+  -mr {whisper}, --transcription_recipe {whisper}
                         LLM recipe used for transcribing video files
-  -mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}, --llm_flavour {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}
-                        Flavour variation for a specific LLM recipe
+  -mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}, --transcription_flavour {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}
+                        Flavour variation for a specific LLM recipe supporting transcription
+  -tr {helsinki-nlp,whisper,facebook-mbart}, --translation_recipe {helsinki-nlp,whisper,facebook-mbart}
+                        LLM recipe used for translating subtitles
+  -tf TRANSLATION_FLAVOUR, --translation_flavour TRANSLATION_FLAVOUR
+                        Flavour variation for a specific LLM recipe supporting translation
   -lgs, --languages     Print out language codes used for stretch and translation
   -d, --debug           Print out debugging information
   -q, --quiet           Switch off logging information
   -ver, --version       show program's version number and exit
 
 required arguments:
   -m {single,dual,script,shift,transcribe}, --mode {single,dual,script,shift,transcribe}
@@ -148,29 +153,48 @@
     parser.add_argument(
         "-ml",
         "--main_language",
         type=str.lower,
         choices=Utils.get_stretch_language_codes(),
         help="Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]",
     )
+    from subaligner.llm import TranscriptionRecipe
+    from subaligner.llm import WhisperFlavour
     parser.add_argument(
         "-mr",
-        "--llm_recipe",
+        "--transcription_recipe",
         type=str.lower,
-        default="whisper",
-        choices=["whisper"],
+        default=TranscriptionRecipe.WHISPER.value,
+        choices=[r.value for r in TranscriptionRecipe],
         help="LLM recipe used for transcribing video files"
     )
     parser.add_argument(
         "-mf",
-        "--llm_flavour",
+        "--transcription_flavour",
         type=str.lower,
-        default="small",
-        choices=["tiny", "tiny.en", "small", "medium", "medium.en", "base", "base.en", "large-v1", "large-v2", "large"],
-        help="Flavour variation for a specific LLM recipe"
+        default=WhisperFlavour.SMALL.value,
+        choices=[wf.value for wf in WhisperFlavour],
+        help="Flavour variation for a specific LLM recipe supporting transcription"
+    )
+    from subaligner.llm import TranslationRecipe
+    from subaligner.llm import HelsinkiNLPFlavour
+    parser.add_argument(
+        "-tr",
+        "--translation_recipe",
+        type=str.lower,
+        default=TranslationRecipe.HELSINKI_NLP.value,
+        choices=[r.value for r in TranslationRecipe],
+        help="LLM recipe used for translating subtitles"
+    )
+    parser.add_argument(
+        "-tf",
+        "--translation_flavour",
+        type=str.lower,
+        default=None,
+        help="Flavour variation for a specific LLM recipe supporting translation"
     )
     parser.add_argument("-lgs", "--languages", action="store_true",
                         help="Print out language codes used for stretch and translation")
     parser.add_argument("-d", "--debug", action="store_true",
                         help="Print out debugging information")
     parser.add_argument("-q", "--quiet", action="store_true",
                         help="Switch off logging information")
@@ -294,30 +318,30 @@
                     aligned_subs, _, voice_probabilities, frame_rate = predictor.predict_plain_text(
                         video_file_path=local_video_path,
                         subtitle_file_path=local_subtitle_path,
                         stretch_in_lang=stretch_in_lang,
                     )
                 elif FLAGS.mode == "transcribe":
                     from subaligner.transcriber import Transcriber
-                    transcriber = Transcriber(recipe=FLAGS.llm_recipe, flavour=FLAGS.llm_flavour)
+                    transcriber = Transcriber(recipe=FLAGS.transcription_recipe, flavour=FLAGS.transcription_flavour)
                     subtitle, frame_rate = transcriber.transcribe(local_video_path, stretch_in_lang)
                     aligned_subs = subtitle.subs
                 else:
                     print("ERROR: Unknown mode {}".format(FLAGS.mode))
                     parser.print_usage()
                     sys.exit(21)
 
                 aligned_subtitle_path = "_aligned.".join(
                     subtitle_path.rsplit(".", 1)).replace(".stl", ".srt") if FLAGS.output == "" else FLAGS.output
 
                 if FLAGS.translate is not None:
                     from subaligner.translator import Translator
                     source, target = FLAGS.translate.split(",")
-                    translator = Translator(source, target)
-                    aligned_subs = translator.translate(aligned_subs)
+                    translator = Translator(src_language=source, tgt_language=target, recipe=FLAGS.translation_recipe, flavour=FLAGS.translation_flavour)
+                    aligned_subs = translator.translate(aligned_subs, local_video_path, (source, target))
                     Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path,
                                                         frame_rate, "utf-8")
                 elif FLAGS.mode == "transcribe":
                     Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path,
                                                         frame_rate, "utf-8")
                 else:
                     Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path,
```

### Comparing `subaligner-0.3.0/bin/subaligner_1pass` & `subaligner-0.3.1/bin/subaligner_1pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/bin/subaligner_2pass` & `subaligner-0.3.1/bin/subaligner_2pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/bin/subaligner_batch` & `subaligner-0.3.1/subaligner/subaligner_2pass/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,92 @@
 #!/usr/bin/env python
 """
-usage: subaligner_batch [-h] [-m {single,dual}] [-vd VIDEO_DIRECTORY] [-sd SUBTITLE_DIRECTORY] [-l MAX_LOGLOSS] [-so]
+usage: subaligner_2pass [-h] [-v VIDEO_PATH] [-s SUBTITLE_PATH] [-l MAX_LOGLOSS] [-so]
                         [-sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
-                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-od OUTPUT_DIRECTORY] [-t TRANSLATE] [-lgs] [-d] [-q] [-ver]
+                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-o OUTPUT] [-t TRANSLATE] [-lgs] [-d] [-q] [-ver]
 
-Batch align multiple subtitle files and audiovisual files
-
-Subtitle files and their companion audiovisual files need to be stored in two separate directories.
-Each file pair needs to share the same base filename, the part before the extension.
+Run dual-stage alignment
 
 optional arguments:
   -h, --help            show this help message and exit
-  -vd VIDEO_DIRECTORY, --video_directory VIDEO_DIRECTORY
-                        Path to the video directory
-  -sd SUBTITLE_DIRECTORY, --subtitle_directory SUBTITLE_DIRECTORY
-                        Path to the subtitle directory
   -l MAX_LOGLOSS, --max_logloss MAX_LOGLOSS
                         Max global log loss for alignment
   -so, --stretch_on    Switch on stretch on subtitles
   -sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --stretch_in_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].
                         NB: This will be ignored if neither -so nor --stretch_on is present
   -fos, --exit_segfail  Exit on any segment alignment failures
   -tod TRAINING_OUTPUT_DIRECTORY, --training_output_directory TRAINING_OUTPUT_DIRECTORY
                         Path to the output directory containing training results
-  -od OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
-                        Path to the output subtitle directory
+  -o OUTPUT, --output OUTPUT
+                        Path to the output subtitle file
   -t TRANSLATE, --translate TRANSLATE
                         Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)
   -lgs, --languages     Print out language codes used for stretch and translation
   -d, --debug           Print out debugging information
   -q, --quiet           Switch off logging information
   -ver, --version       show program's version number and exit
 
 required arguments:
-  -m {single,dual}, --mode {single,dual}
-                        Alignment mode: either single or dual
+  -v VIDEO_PATH, --video_path VIDEO_PATH
+                        File path or URL to the video file
+  -s SUBTITLE_PATH, --subtitle_path SUBTITLE_PATH
+                        File path or URL to the subtitle file (Extensions of supported subtitles: .ass, .sbv, .srt, .vtt, .ttml, .dfxp, .scc, .txt, .tmp, .smi, .ssa, .sami, .xml, .sub, .stl, .ytt) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)
 """
 
 import argparse
 import sys
 import traceback
 import os
+import tempfile
 import pkg_resources
 
 
 def main():
     if sys.version_info.major != 3:
         print("ERROR: Cannot find Python 3")
         sys.exit(20)
     try:
         import subaligner
     except ModuleNotFoundError:
         print("ERROR: Subaligner is not installed")
         sys.exit(20)
 
     from subaligner._version import __version__
-    parser = argparse.ArgumentParser(description="""Batch align multiple subtitle files and audiovisual files (v%s)\n
-Subtitle files and their companion audiovisual files need to be stored in two separate directories.
-Each file pair needs to share the same base filename, the part before the extension.""" % __version__, formatter_class=argparse.RawTextHelpFormatter)
+    parser = argparse.ArgumentParser(description="Run dual-stage alignment (v%s)" % __version__, formatter_class=argparse.RawTextHelpFormatter)
     required_args = parser.add_argument_group("required arguments")
     required_args.add_argument(
-        "-m",
-        "--mode",
-        type=str,
-        default="",
-        choices=["single", "dual"],
-        help="Alignment mode: either single or dual",
-    )
-    parser.add_argument(
-        "-vd",
-        "--video_directory",
+        "-v",
+        "--video_path",
         type=str,
         default="",
-        help="Path to the video directory",
+        help="File path or URL to the video file",
     )
-    parser.add_argument(
-        "-sd",
-        "--subtitle_directory",
+    from subaligner.subtitle import Subtitle
+    required_args.add_argument(
+        "-s",
+        "--subtitle_path",
         type=str,
         default="",
-        help="Path to the subtitle directory",
+        help="File path or URL to the subtitle file (Extensions of supported subtitles: {}) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)".format(", ".join(Subtitle.subtitle_extensions())),
     )
     parser.add_argument(
         "-l",
         "--max_logloss",
         type=float,
         default=float("inf"),
         help="Max global log loss for alignment",
     )
     parser.add_argument(
         "-so",
         "--stretch_on",
         action="store_true",
-        help="Switch on stretch on subtitles)",
+        help="Switch on stretch on subtitles",
     )
     from subaligner.utils import Utils
-    from subaligner.subtitle import Subtitle
     parser.add_argument(
         "-sil",
         "--stretch_in_language",
         type=str,
         choices=Utils.get_stretch_language_codes(),
         default="eng",
         help="Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].\nNB: This will be ignored if neither -so nor --stretch_on is present",
@@ -115,27 +101,19 @@
         "-tod",
         "--training_output_directory",
         type=str,
         default=os.path.abspath(os.path.dirname(subaligner.__file__)),
         help="Path to the output directory containing training results",
     )
     parser.add_argument(
-        "-od",
-        "--output_directory",
-        type=str,
-        default="",
-        help="Path to the output subtitle directory",
-    )
-    parser.add_argument(
-        "-of",
-        "--output_format",
+        "-o",
+        "--output",
         type=str,
-        choices=list(map(lambda x: x[1:], Subtitle.subtitle_extensions())),
         default="",
-        help="File format of the output subtitles"
+        help="Path to the output subtitle file",
     )
     parser.add_argument(
         "-t",
         "--translate",
         type=str,
         help="Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)",
     )
@@ -147,136 +125,141 @@
                         help="Switch off logging information")
     parser.add_argument("-ver", "--version", action="version", version=__version__)
     FLAGS, unparsed = parser.parse_known_args()
 
     if FLAGS.languages:
         print("\n".join(Utils.get_language_table()))
         sys.exit(0)
-    if FLAGS.mode == "":
-        print("ERROR: --mode was not passed in")
-        parser.print_usage()
-        sys.exit(21)
-    if FLAGS.video_directory == "":
-        print("ERROR: --video_directory was not passed in")
+    if FLAGS.video_path == "":
+        print("ERROR: --video_path was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.subtitle_directory == "":
-        print("ERROR: --subtitle_directory was not passed in")
+    if FLAGS.subtitle_path == "":
+        print("ERROR: --subtitle_path was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.output_directory == "":
-        print("ERROR: --output_directory was not passed in")
+    if FLAGS.subtitle_path.lower().startswith("http") and FLAGS.output == "":
+        print("ERROR: --output was not passed in for alignment on a remote subtitle file")
         parser.print_usage()
         sys.exit(21)
-    if os.path.abspath(FLAGS.subtitle_directory) == os.path.abspath(FLAGS.output_directory):
-        print("ERROR: The output directory cannot be set to the same as the input subtitle directory")
+    if FLAGS.subtitle_path.lower().startswith("teletext:") and FLAGS.output == "":
+        print("ERROR: --output was not passed in for alignment on embedded subtitles")
         parser.print_usage()
         sys.exit(21)
     if FLAGS.translate is not None:
         if "transformers" not in {pkg.key for pkg in pkg_resources.working_set}:
             print('ERROR: Alignment has been configured to perform translation. Please install "subaligner[llm]" and run your command again.')
             sys.exit(21)
+    if FLAGS.stretch_on:
+        if "aeneas" not in {pkg.key for pkg in pkg_resources.working_set}:
+            print('ERROR: Alignment has been configured to use extra features. Please install "subaligner[stretch]" and run your command again.')
+            sys.exit(21)
 
-    video_file_paths = [os.path.abspath(os.path.join(path, p)) for path, _, files in
-                        os.walk(FLAGS.video_directory) for p in files if not p.startswith(".")]
-    subtitle_file_paths = [os.path.abspath(os.path.join(path, p)) for path, _, files in
-                           os.walk(FLAGS.subtitle_directory) for p in files if not p.startswith(".")]
-    if len(video_file_paths) != len(subtitle_file_paths):
-        print("ERROR: The numbers of input videos and subtitles do not match")
-        parser.print_usage()
-        sys.exit(21)
-
-    output_dir = os.path.abspath(FLAGS.output_directory)
-    os.makedirs(output_dir, exist_ok=True)
-    video_file_paths = sorted(video_file_paths, key=lambda x: os.path.splitext(os.path.basename(x))[0])
-    subtitle_file_paths = sorted(subtitle_file_paths, key=lambda x: os.path.splitext(os.path.basename(x))[0])
+    local_video_path = FLAGS.video_path
+    local_subtitle_path = FLAGS.subtitle_path
     exit_segfail = FLAGS.exit_segfail
     stretch = FLAGS.stretch_on
     stretch_in_lang = FLAGS.stretch_in_language
 
     from subaligner.logger import Logger
     Logger.VERBOSE = FLAGS.debug
     Logger.QUIET = FLAGS.quiet
     from subaligner.predictor import Predictor
-    from subaligner.subtitle import Subtitle
     from subaligner.exception import UnsupportedFormatException
     from subaligner.exception import TerminalException
 
-    predictor = Predictor()
-    failures = []
-    for index in range(len(video_file_paths)):
-        local_video_path = video_file_paths[index]
-        local_subtitle_path = subtitle_file_paths[index]
-        try:
-            if FLAGS.mode == "single":
-                aligned_subs, audio_file_path, voice_probabilities, frame_rate = predictor.predict_single_pass(
-                    video_file_path=local_video_path,
-                    subtitle_file_path=local_subtitle_path,
-                    weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights")
-                )
-            else:
-                aligned_subs, subs, voice_probabilities, frame_rate = predictor.predict_dual_pass(
-                    video_file_path=local_video_path,
-                    subtitle_file_path=local_subtitle_path,
-                    weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights"),
-                    stretch=stretch,
-                    stretch_in_lang=stretch_in_lang,
-                    exit_segfail=exit_segfail,
-                )
-
-            parent_dir = os.path.dirname(local_subtitle_path.replace(os.path.abspath(FLAGS.subtitle_directory), output_dir))
-            os.makedirs(parent_dir, exist_ok=True)
-            file_parts = os.path.basename(local_subtitle_path).rsplit(".", 1)
-            file_parts[1] = FLAGS.output_format if FLAGS.output_format != "" else file_parts[1]
-            aligned_subtitle_path = os.path.abspath(os.path.join(parent_dir, ".".join(file_parts).replace(".stl", ".srt")))
-
-            if FLAGS.translate is not None:
-                from subaligner.translator import Translator
-                source, target = FLAGS.translate.split(",")
-                translator = Translator(source, target)
-                aligned_subs = translator.translate(aligned_subs)
-                Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
+    try:
+        if FLAGS.video_path.lower().startswith("http"):
+            _, local_video_path = tempfile.mkstemp()
+            _, video_file_extension = os.path.splitext(FLAGS.video_path.lower())
+            local_video_path = "{}{}".format(local_video_path, video_file_extension)
+            Utils.download_file(FLAGS.video_path, local_video_path)
+
+        if FLAGS.subtitle_path.lower().startswith("http"):
+            _, local_subtitle_path = tempfile.mkstemp()
+            _, subtitle_file_extension = os.path.splitext(FLAGS.subtitle_path.lower())
+            local_subtitle_path = "{}{}".format(local_subtitle_path, subtitle_file_extension)
+            Utils.download_file(FLAGS.subtitle_path, local_subtitle_path)
+
+        if FLAGS.subtitle_path.lower().startswith("embedded:"):
+            _, local_subtitle_path = tempfile.mkstemp()
+            _, subtitle_file_extension = os.path.splitext(FLAGS.output)
+            local_subtitle_path = "{}{}".format(local_subtitle_path, subtitle_file_extension)
+            params = FLAGS.subtitle_path.lower().split(":")[1].split(",")
+            if params and "=" in params[0]:
+                params = {param.split("=")[0]: param.split("=")[1] for param in params}
+                if "page_num" in params:
+                    Utils.extract_teletext_as_subtitle(local_video_path, int(params["page_num"]), local_subtitle_path)
+                elif "stream_index" in params:
+                    Utils.extract_matroska_subtitle(local_video_path, int(params["stream_index"]), local_subtitle_path)
             else:
-                Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
+                print("ERROR: Embedded subtitle selector cannot be empty")
+                parser.print_usage()
+                sys.exit(21)
+
+        predictor = Predictor()
+        subs_list, subs, voice_probabilities, frame_rate = predictor.predict_dual_pass(
+            video_file_path=local_video_path,
+            subtitle_file_path=local_subtitle_path,
+            weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights"),
+            stretch=stretch,
+            stretch_in_lang=stretch_in_lang,
+            exit_segfail=exit_segfail,
+        )
+
+        aligned_subtitle_path = "_aligned.".join(
+            FLAGS.subtitle_path.rsplit(".", 1)).replace(".stl", ".srt") if FLAGS.output == "" else FLAGS.output
+
+        if FLAGS.translate is not None:
+            from subaligner.translator import Translator
+            source, target = FLAGS.translate.split(",")
+            translator = Translator(source, target)
+            subs_list = translator.translate(subs)
+            Subtitle.save_subs_as_target_format(subs_list, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
 
-            log_loss = predictor.get_log_loss(voice_probabilities, aligned_subs)
-            if log_loss is None or log_loss > FLAGS.max_logloss:
-                print(
-                    "ERROR: Alignment failed with a too high loss value: {} for {} and {}".format(log_loss, local_video_path, local_subtitle_path)
-                )
-                failures.append((local_video_path, local_subtitle_path))
-                continue
+        else:
+            Subtitle.save_subs_as_target_format(subs_list, local_subtitle_path, aligned_subtitle_path, frame_rate)
 
-            print("Aligned subtitle saved to: {}".format(aligned_subtitle_path))
-        except UnsupportedFormatException as e:
+        log_loss = predictor.get_log_loss(voice_probabilities, subs_list)
+        if log_loss is None or log_loss > FLAGS.max_logloss:
             print(
-                "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
+                "ERROR: Alignment failed with a too high loss value: {}".format(log_loss)
             )
-            traceback.print_tb(e.__traceback__)
-            failures.append((local_video_path, local_subtitle_path))
-            continue
-        except TerminalException as e:
-            print(
-                "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
-            )
-            traceback.print_tb(e.__traceback__)
-            failures.append((local_video_path, local_subtitle_path))
-            continue
-        except Exception as e:
-            print(
-                "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
-            )
-            traceback.print_tb(e.__traceback__)
-            failures.append((local_video_path, local_subtitle_path))
-            continue
-        else:
-            continue
+            _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
+            sys.exit(22)
+
+        print("Aligned subtitle saved to: {}".format(aligned_subtitle_path))
+    except UnsupportedFormatException as e:
+        print(
+            "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
+        )
+        traceback.print_tb(e.__traceback__)
+        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
+        sys.exit(23)
+    except TerminalException as e:
+        print(
+            "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
+        )
+        traceback.print_tb(e.__traceback__)
+        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
+        sys.exit(24)
+    except Exception as e:
+        print(
+            "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
+        )
+        traceback.print_tb(e.__traceback__)
+        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
+        sys.exit(1)
+    else:
+        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
+        sys.exit(0)
+
 
-    if len(failures) > 0:
-        print("WARNING: The following video and subtitle failed to align with each other:")
-        for failure in failures:
-            video_file_path, subtitle_file_path = failure
-            print("\t{}  {}".format(video_file_path, subtitle_file_path))
+def _remove_tmp_files(flags, local_video_path, local_subtitle_path):
+    if flags.video_path.lower().startswith("http") and os.path.exists(local_video_path):
+        os.remove(local_video_path)
+    if flags.subtitle_path.lower().startswith("http") and os.path.exists(local_subtitle_path):
+        os.remove(local_subtitle_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `subaligner-0.3.0/bin/subaligner_convert` & `subaligner-0.3.1/bin/subaligner_convert`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/bin/subaligner_train` & `subaligner-0.3.1/bin/subaligner_train`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/bin/subaligner_tune` & `subaligner-0.3.1/bin/subaligner_tune`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/requirements.txt` & `subaligner-0.3.1/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-absl-py~=0.10
 astor==0.7.1
-audioread==2.1.5
 beautifulsoup4<4.9.0
 bleach==3.3.0
 cachetools==3.1.1
 captionstransformer~=1.2.1
 cchardet==2.1.7
 certifi==2019.11.28
 chardet==3.0.4
 click==5.1
 cloudpickle~=1.6.0
 cycler==0.10.0
 Cython~=0.29.22
-dask<2022.1.0
+dask>=2021.10.0,<2022.1.0
 decorator==4.3.0
 distributed==1.13.0
 filelock<4.0.0
-google-auth==1.27.0
 google-auth-oauthlib==0.4.2
 google-pasta~=0.2
 graphviz==0.8.3
 HeapDict==1.0.0
 h5py<=3.6.0
 html5lib==1.0b9
 hyperopt==0.2.4
 idna==2.8
 isort==4.3.4
+joblib>=1.2.0
 Keras-Applications>=1.0.8
 Keras-Preprocessing>=1.0.9
 kiwisolver==1.0.1
 lazy-object-proxy==1.4.3
 le-pycaption==2.2.0a1
-librosa>=0.8.0
+librosa<0.10.0
 locket==0.2.0
 Markdown==2.6.11
 mccabe==0.6.1
 networkx>=2.5.1
-msgpack-python==0.5.6
 numba>=0.50.0
 numpy<1.24.0
 oauthlib==3.1.0
 pbr==4.0.2
 pluggy==0.13.1
 psutil==5.6.7
 py==1.10.0
@@ -55,19 +52,19 @@
 pystack-debugger==0.8.0
 pytz==2018.4
 PyYAML>=4.2b1
 requests~=2.25.1
 requests-oauthlib==1.3.0
 rsa==4.7
 scipy<=1.8.1
-scikit-learn~=0.24.2
+scikit-learn<1.2.0
 setuptools>=41.0.0
 six~=1.15.0
 tblib==1.3.2
-tensorflow>=1.15.5,<2.9
+tensorflow>=1.15.5,<2.12
 termcolor==1.1.0
 toml==0.10.0
 toolz==0.9.0
 tornado==5.1.0
 urllib3~=1.26.5
 Werkzeug>=0.15.3
 zict==0.1.3
```

### Comparing `subaligner-0.3.0/setup.py` & `subaligner-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/__main__.py` & `subaligner-0.3.1/subaligner/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 """
 usage: subaligner [-h] [-m {single,dual,script,shift,transcribe}] [-v VIDEO_PATH] [-s SUBTITLE_PATH [SUBTITLE_PATH ...]] [-l MAX_LOGLOSS] [-so]
                   [-sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
                   [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-o OUTPUT] [-t TRANSLATE] [-os OFFSET_SECONDS]
                   [-ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
-                  [-mr {whisper}] [-mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}] [-lgs] [-d] [-q] [-ver]
+                  [-mr {whisper}] [-mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}] [-tr {helsinki-nlp,whisper,facebook-mbart}]
+                  [-tf TRANSLATION_FLAVOUR] [-lgs] [-d] [-q] [-ver]
 
 Subaligner command line interface
 
 optional arguments:
   -h, --help            show this help message and exit
   -s SUBTITLE_PATH [SUBTITLE_PATH ...], --subtitle_path SUBTITLE_PATH [SUBTITLE_PATH ...]
-                        File path or URL to the subtitle file (Extensions of supported subtitles: .ssa, .vtt, .srt, .txt, .smi, .ytt, .sub, .xml, .sbv, .ass, .sami, .scc, .tmp, .stl, .ttml, .dfxp) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)
+                        File path or URL to the subtitle file (Extensions of supported subtitles: .ttml, .ssa, .stl, .sbv, .dfxp, .srt, .txt, .ytt, .vtt, .sub, .sami, .xml, .scc, .ass, .smi, .tmp) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)
   -l MAX_LOGLOSS, --max_logloss MAX_LOGLOSS
                         Max global log loss for alignment
   -so, --stretch_on     Switch on stretch on subtitles)
   -sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --stretch_in_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].
                         NB: This will be ignored if neither -so nor --stretch_on is present
   -fos, --exit_segfail  Exit on any segment alignment failures
@@ -25,18 +26,22 @@
                         Path to the output subtitle file
   -t TRANSLATE, --translate TRANSLATE
                         Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)
   -os OFFSET_SECONDS, --offset_seconds OFFSET_SECONDS
                         Offset by which the subtitle will be shifted
   -ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --main_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]
-  -mr {whisper}, --llm_recipe {whisper}
+  -mr {whisper}, --transcription_recipe {whisper}
                         LLM recipe used for transcribing video files
-  -mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}, --llm_flavour {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}
-                        Flavour variation for a specific LLM recipe
+  -mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}, --transcription_flavour {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}
+                        Flavour variation for a specific LLM recipe supporting transcription
+  -tr {helsinki-nlp,whisper,facebook-mbart}, --translation_recipe {helsinki-nlp,whisper,facebook-mbart}
+                        LLM recipe used for translating subtitles
+  -tf TRANSLATION_FLAVOUR, --translation_flavour TRANSLATION_FLAVOUR
+                        Flavour variation for a specific LLM recipe supporting translation
   -lgs, --languages     Print out language codes used for stretch and translation
   -d, --debug           Print out debugging information
   -q, --quiet           Switch off logging information
   -ver, --version       show program's version number and exit
 
 required arguments:
   -m {single,dual,script,shift,transcribe}, --mode {single,dual,script,shift,transcribe}
@@ -148,29 +153,48 @@
     parser.add_argument(
         "-ml",
         "--main_language",
         type=str.lower,
         choices=Utils.get_stretch_language_codes(),
         help="Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]",
     )
+    from subaligner.llm import TranscriptionRecipe
+    from subaligner.llm import WhisperFlavour
     parser.add_argument(
         "-mr",
-        "--llm_recipe",
+        "--transcription_recipe",
         type=str.lower,
-        default="whisper",
-        choices=["whisper"],
+        default=TranscriptionRecipe.WHISPER.value,
+        choices=[r.value for r in TranscriptionRecipe],
         help="LLM recipe used for transcribing video files"
     )
     parser.add_argument(
         "-mf",
-        "--llm_flavour",
+        "--transcription_flavour",
         type=str.lower,
-        default="small",
-        choices=["tiny", "tiny.en", "small", "medium", "medium.en", "base", "base.en", "large-v1", "large-v2", "large"],
-        help="Flavour variation for a specific LLM recipe"
+        default=WhisperFlavour.SMALL.value,
+        choices=[wf.value for wf in WhisperFlavour],
+        help="Flavour variation for a specific LLM recipe supporting transcription"
+    )
+    from subaligner.llm import TranslationRecipe
+    from subaligner.llm import HelsinkiNLPFlavour
+    parser.add_argument(
+        "-tr",
+        "--translation_recipe",
+        type=str.lower,
+        default=TranslationRecipe.HELSINKI_NLP.value,
+        choices=[r.value for r in TranslationRecipe],
+        help="LLM recipe used for translating subtitles"
+    )
+    parser.add_argument(
+        "-tf",
+        "--translation_flavour",
+        type=str.lower,
+        default=None,
+        help="Flavour variation for a specific LLM recipe supporting translation"
     )
     parser.add_argument("-lgs", "--languages", action="store_true",
                         help="Print out language codes used for stretch and translation")
     parser.add_argument("-d", "--debug", action="store_true",
                         help="Print out debugging information")
     parser.add_argument("-q", "--quiet", action="store_true",
                         help="Switch off logging information")
@@ -294,30 +318,30 @@
                     aligned_subs, _, voice_probabilities, frame_rate = predictor.predict_plain_text(
                         video_file_path=local_video_path,
                         subtitle_file_path=local_subtitle_path,
                         stretch_in_lang=stretch_in_lang,
                     )
                 elif FLAGS.mode == "transcribe":
                     from subaligner.transcriber import Transcriber
-                    transcriber = Transcriber(recipe=FLAGS.llm_recipe, flavour=FLAGS.llm_flavour)
+                    transcriber = Transcriber(recipe=FLAGS.transcription_recipe, flavour=FLAGS.transcription_flavour)
                     subtitle, frame_rate = transcriber.transcribe(local_video_path, stretch_in_lang)
                     aligned_subs = subtitle.subs
                 else:
                     print("ERROR: Unknown mode {}".format(FLAGS.mode))
                     parser.print_usage()
                     sys.exit(21)
 
                 aligned_subtitle_path = "_aligned.".join(
                     subtitle_path.rsplit(".", 1)).replace(".stl", ".srt") if FLAGS.output == "" else FLAGS.output
 
                 if FLAGS.translate is not None:
                     from subaligner.translator import Translator
                     source, target = FLAGS.translate.split(",")
-                    translator = Translator(source, target)
-                    aligned_subs = translator.translate(aligned_subs)
+                    translator = Translator(src_language=source, tgt_language=target, recipe=FLAGS.translation_recipe, flavour=FLAGS.translation_flavour)
+                    aligned_subs = translator.translate(aligned_subs, local_video_path, (source, target))
                     Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path,
                                                         frame_rate, "utf-8")
                 elif FLAGS.mode == "transcribe":
                     Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path,
                                                         frame_rate, "utf-8")
                 else:
                     Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path,
```

### Comparing `subaligner-0.3.0/subaligner/embedder.py` & `subaligner-0.3.1/subaligner/embedder.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/hparam_tuner.py` & `subaligner-0.3.1/subaligner/hparam_tuner.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/hyperparameters.py` & `subaligner-0.3.1/subaligner/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/lib/language.py` & `subaligner-0.3.1/subaligner/lib/language.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/lib/to_srt.py` & `subaligner-0.3.1/subaligner/lib/to_srt.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/logger.py` & `subaligner-0.3.1/subaligner/logger.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/media_helper.py` & `subaligner-0.3.1/subaligner/media_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from copy import deepcopy
 from pysrt import SubRipFile, SubRipItem
 from decimal import Decimal
 from .embedder import FeatureEmbedder
 from .exception import TerminalException
 from .exception import NoFrameRateException
 from .logger import Logger
+from .utils import Utils
 
 TEMP_DIR_PATH = tempfile.mkdtemp()
 
 
 def clear_temp(*_):
     if os.path.isdir(TEMP_DIR_PATH):
         shutil.rmtree(TEMP_DIR_PATH)
@@ -69,22 +70,23 @@
             )
         else:
             audio_file_path = os.path.join(
                 TEMP_DIR_PATH, f"{basename}{self.AUDIO_FILE_EXTENSION[1]}"
             )
 
         command = (
-            "{0} -y -xerror -i '{1}' -ac 2 -ar {2} -vn '{3}'".format(
-                self.FFMPEG_BIN, video_file_path, freq, audio_file_path
+            "{0} -y -xerror -i {1} -ac 2 -ar {2} -vn {3}".format(
+                self.FFMPEG_BIN, Utils.double_quoted(video_file_path), freq, Utils.double_quoted(audio_file_path)
             )
             if decompress
-            else "{0} -y -xerror -i '{1}' -vn -acodec copy '{2}'".format(
-                self.FFMPEG_BIN, video_file_path, audio_file_path
+            else "{0} -y -xerror -i {1} -vn -acodec copy {2}".format(
+                self.FFMPEG_BIN, Utils.double_quoted(video_file_path), Utils.double_quoted(audio_file_path)
             )
         )
+        print(command)
         with subprocess.Popen(
             shlex.split(command),
             shell=False,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             close_fds=True,
             universal_newlines=True,
@@ -178,20 +180,20 @@
         start = start.replace(",", ".")
         if end is not None:
             end = end.replace(",", ".")
         segment_path = os.path.join(TEMP_DIR_PATH, f"{filename}_{str(start)}_{str(end)}{extension}")
 
         if end is not None:
             duration = self.get_duration_in_seconds(start, end)
-            command = "{0} -y -xerror -i '{1}' -ss {2} -t {3} -acodec copy '{4}'".format(
-                self.FFMPEG_BIN, audio_file_path, start, duration, segment_path
+            command = "{0} -y -xerror -i {1} -ss {2} -t {3} -acodec copy {4}".format(
+                self.FFMPEG_BIN, Utils.double_quoted(audio_file_path), start, duration, Utils.double_quoted(segment_path)
             )
         else:
-            command = "{0} -y -xerror -i '{1}' -ss {2} -acodec copy '{3}'".format(
-                self.FFMPEG_BIN, audio_file_path, start, segment_path
+            command = "{0} -y -xerror -i {1} -ss {2} -acodec copy {3}".format(
+                self.FFMPEG_BIN, Utils.double_quoted(audio_file_path), start, Utils.double_quoted(segment_path)
             )
         with subprocess.Popen(
             shlex.split(command),
             shell=False,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             universal_newlines=True,
@@ -312,15 +314,15 @@
         Returns:
             float -- The frame rate
         """
 
         discarded = "NUL:" if os.name == "nt" else "/dev/null"
 
         with subprocess.Popen(
-                shlex.split("{0} -i '{1}' -t 00:00:10 -f null {2}".format(self.FFMPEG_BIN, file_path, discarded)),
+                shlex.split("{0} -i {1} -t 00:00:10 -f null {2}".format(self.FFMPEG_BIN, Utils.double_quoted(file_path), discarded)),
                 shell=False,
                 stderr=subprocess.PIPE,
                 close_fds=True,
                 universal_newlines=True,
                 bufsize=1,
         ) as proc:
             with subprocess.Popen(
```

### Comparing `subaligner-0.3.0/subaligner/models/training/config/hyperparameters.json` & `subaligner-0.3.1/subaligner/models/training/config/hyperparameters.json`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/models/training/model/model.hdf5` & `subaligner-0.3.1/subaligner/models/training/model/model.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/models/training/weights/weights.hdf5` & `subaligner-0.3.1/subaligner/models/training/weights/weights.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/network.py` & `subaligner-0.3.1/subaligner/network.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/predictor.py` & `subaligner-0.3.1/subaligner/predictor.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/subaligner_1pass/__main__.py` & `subaligner-0.3.1/subaligner/subaligner_1pass/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/subaligner_2pass/__main__.py` & `subaligner-0.3.1/bin/subaligner_batch`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,107 @@
 #!/usr/bin/env python
 """
-usage: subaligner_2pass [-h] [-v VIDEO_PATH] [-s SUBTITLE_PATH] [-l MAX_LOGLOSS] [-so]
+usage: subaligner_batch [-h] [-m {single,dual}] [-vd VIDEO_DIRECTORY] [-sd SUBTITLE_DIRECTORY] [-l MAX_LOGLOSS] [-so]
                         [-sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
-                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-o OUTPUT] [-t TRANSLATE] [-lgs] [-d] [-q] [-ver]
+                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-od OUTPUT_DIRECTORY] [-t TRANSLATE] [-lgs] [-d] [-q] [-ver]
 
-Run dual-stage alignment
+Batch align multiple subtitle files and audiovisual files
+
+Subtitle files and their companion audiovisual files need to be stored in two separate directories.
+Each file pair needs to share the same base filename, the part before the extension.
 
 optional arguments:
   -h, --help            show this help message and exit
+  -vd VIDEO_DIRECTORY, --video_directory VIDEO_DIRECTORY
+                        Path to the video directory
+  -sd SUBTITLE_DIRECTORY, --subtitle_directory SUBTITLE_DIRECTORY
+                        Path to the subtitle directory
   -l MAX_LOGLOSS, --max_logloss MAX_LOGLOSS
                         Max global log loss for alignment
   -so, --stretch_on    Switch on stretch on subtitles
   -sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --stretch_in_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].
                         NB: This will be ignored if neither -so nor --stretch_on is present
   -fos, --exit_segfail  Exit on any segment alignment failures
   -tod TRAINING_OUTPUT_DIRECTORY, --training_output_directory TRAINING_OUTPUT_DIRECTORY
                         Path to the output directory containing training results
-  -o OUTPUT, --output OUTPUT
-                        Path to the output subtitle file
+  -od OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
+                        Path to the output subtitle directory
   -t TRANSLATE, --translate TRANSLATE
                         Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)
   -lgs, --languages     Print out language codes used for stretch and translation
   -d, --debug           Print out debugging information
   -q, --quiet           Switch off logging information
   -ver, --version       show program's version number and exit
 
 required arguments:
-  -v VIDEO_PATH, --video_path VIDEO_PATH
-                        File path or URL to the video file
-  -s SUBTITLE_PATH, --subtitle_path SUBTITLE_PATH
-                        File path or URL to the subtitle file (Extensions of supported subtitles: .ass, .sbv, .srt, .vtt, .ttml, .dfxp, .scc, .txt, .tmp, .smi, .ssa, .sami, .xml, .sub, .stl, .ytt) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)
+  -m {single,dual}, --mode {single,dual}
+                        Alignment mode: either single or dual
 """
 
 import argparse
 import sys
 import traceback
 import os
-import tempfile
 import pkg_resources
+import tempfile
 
 
 def main():
     if sys.version_info.major != 3:
         print("ERROR: Cannot find Python 3")
         sys.exit(20)
     try:
         import subaligner
     except ModuleNotFoundError:
         print("ERROR: Subaligner is not installed")
         sys.exit(20)
 
     from subaligner._version import __version__
-    parser = argparse.ArgumentParser(description="Run dual-stage alignment (v%s)" % __version__, formatter_class=argparse.RawTextHelpFormatter)
+    parser = argparse.ArgumentParser(description="""Batch align multiple subtitle files and audiovisual files (v%s)\n
+Subtitle files and their companion audiovisual files need to be stored in two separate directories.
+Each file pair needs to share the same base filename, the part before the extension.""" % __version__, formatter_class=argparse.RawTextHelpFormatter)
     required_args = parser.add_argument_group("required arguments")
     required_args.add_argument(
-        "-v",
-        "--video_path",
+        "-m",
+        "--mode",
         type=str,
         default="",
-        help="File path or URL to the video file",
+        choices=["single", "dual", "script", "transcribe"],
+        help="Alignment mode: either single or dual",
     )
-    from subaligner.subtitle import Subtitle
-    required_args.add_argument(
-        "-s",
-        "--subtitle_path",
+    parser.add_argument(
+        "-sd",
+        "--subtitle_directory",
+        type=str,
+        default="",
+        help="Path to the subtitle directory",
+    )
+    parser.add_argument(
+        "-vd",
+        "--video_directory",
         type=str,
         default="",
-        help="File path or URL to the subtitle file (Extensions of supported subtitles: {}) or selector for the embedded subtitle (e.g., embedded:page_num=888 or embedded:stream_index=0)".format(", ".join(Subtitle.subtitle_extensions())),
+        help="Path to the video directory",
     )
     parser.add_argument(
         "-l",
         "--max_logloss",
         type=float,
         default=float("inf"),
         help="Max global log loss for alignment",
     )
     parser.add_argument(
         "-so",
         "--stretch_on",
         action="store_true",
-        help="Switch on stretch on subtitles",
+        help="Switch on stretch on subtitles)",
     )
     from subaligner.utils import Utils
+    from subaligner.subtitle import Subtitle
     parser.add_argument(
         "-sil",
         "--stretch_in_language",
         type=str,
         choices=Utils.get_stretch_language_codes(),
         default="eng",
         help="Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].\nNB: This will be ignored if neither -so nor --stretch_on is present",
@@ -101,165 +116,227 @@
         "-tod",
         "--training_output_directory",
         type=str,
         default=os.path.abspath(os.path.dirname(subaligner.__file__)),
         help="Path to the output directory containing training results",
     )
     parser.add_argument(
-        "-o",
-        "--output",
+        "-od",
+        "--output_directory",
+        type=str,
+        default="",
+        help="Path to the output subtitle directory",
+    )
+    parser.add_argument(
+        "-of",
+        "--output_format",
         type=str,
+        choices=list(map(lambda x: x[1:], Subtitle.subtitle_extensions())),
         default="",
-        help="Path to the output subtitle file",
+        help="File format of the output subtitles"
     )
     parser.add_argument(
         "-t",
         "--translate",
         type=str,
         help="Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)",
     )
+    parser.add_argument(
+        "-ml",
+        "--main_language",
+        type=str.lower,
+        choices=Utils.get_stretch_language_codes(),
+        help="Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]",
+    )
+    from subaligner.llm import TranscriptionRecipe
+    from subaligner.llm import WhisperFlavour
+    parser.add_argument(
+        "-mr",
+        "--transcription_recipe",
+        type=str.lower,
+        default=TranscriptionRecipe.WHISPER.value,
+        choices=[r.value for r in TranscriptionRecipe],
+        help="LLM recipe used for transcribing video files"
+    )
+    parser.add_argument(
+        "-mf",
+        "--transcription_flavour",
+        type=str.lower,
+        default=WhisperFlavour.SMALL.value,
+        choices=[wf.value for wf in WhisperFlavour],
+        help="Flavour variation for a specific LLM recipe supporting transcription"
+    )
     parser.add_argument("-lgs", "--languages", action="store_true",
                         help="Print out language codes used for stretch and translation")
     parser.add_argument("-d", "--debug", action="store_true",
                         help="Print out debugging information")
     parser.add_argument("-q", "--quiet", action="store_true",
                         help="Switch off logging information")
     parser.add_argument("-ver", "--version", action="version", version=__version__)
     FLAGS, unparsed = parser.parse_known_args()
 
     if FLAGS.languages:
         print("\n".join(Utils.get_language_table()))
         sys.exit(0)
-    if FLAGS.video_path == "":
-        print("ERROR: --video_path was not passed in")
+    if FLAGS.mode == "":
+        print("ERROR: --mode was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.subtitle_path == "":
-        print("ERROR: --subtitle_path was not passed in")
+    if FLAGS.video_directory == "":
+        print("ERROR: --video_directory was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.subtitle_path.lower().startswith("http") and FLAGS.output == "":
-        print("ERROR: --output was not passed in for alignment on a remote subtitle file")
+    if FLAGS.mode != "transcribe" and FLAGS.subtitle_directory == "":
+        print("ERROR: --subtitle_directory was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.subtitle_path.lower().startswith("teletext:") and FLAGS.output == "":
-        print("ERROR: --output was not passed in for alignment on embedded subtitles")
+    if FLAGS.output_directory == "":
+        print("ERROR: --output_directory was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.translate is not None:
+    if FLAGS.mode != "transcribe" and os.path.abspath(FLAGS.subtitle_directory) == os.path.abspath(FLAGS.output_directory):
+        print("ERROR: The output directory cannot be set to the same as the input subtitle directory")
+        parser.print_usage()
+        sys.exit(21)
+    if FLAGS.translate is not None or FLAGS.mode == "transcribe":
         if "transformers" not in {pkg.key for pkg in pkg_resources.working_set}:
-            print('ERROR: Alignment has been configured to perform translation. Please install "subaligner[llm]" and run your command again.')
+            print('ERROR: Alignment has been configured to use language models. Please install "subaligner[llm]" and run your command again.')
             sys.exit(21)
-    if FLAGS.stretch_on:
+    if FLAGS.stretch_on or FLAGS.mode == "script":
         if "aeneas" not in {pkg.key for pkg in pkg_resources.working_set}:
             print('ERROR: Alignment has been configured to use extra features. Please install "subaligner[stretch]" and run your command again.')
             sys.exit(21)
+    if FLAGS.mode == "transcribe":
+        if FLAGS.main_language is None:
+            print("ERROR: --main_language was not passed in but required by mode 'transcribe'")
+            parser.print_usage()
+            sys.exit(21)
 
-    local_video_path = FLAGS.video_path
-    local_subtitle_path = FLAGS.subtitle_path
+    video_file_paths = [os.path.abspath(os.path.join(path, p)) for path, _, files in
+                        os.walk(FLAGS.video_directory) for p in files if not p.startswith(".")]
+
+    if FLAGS.mode != "transcribe":
+        subtitle_file_paths = [os.path.abspath(os.path.join(path, p)) for path, _, files in
+                               os.walk(FLAGS.subtitle_directory) for p in files if not p.startswith(".")]
+        if len(video_file_paths) != len(subtitle_file_paths):
+            print("ERROR: The numbers of input videos and subtitles do not match")
+            parser.print_usage()
+            sys.exit(21)
+
+    output_dir = os.path.abspath(FLAGS.output_directory)
+    os.makedirs(output_dir, exist_ok=True)
+    video_file_paths = sorted(video_file_paths, key=lambda x: os.path.splitext(os.path.basename(x))[0])
+    if FLAGS.mode != "transcribe":
+        subtitle_file_paths = sorted(subtitle_file_paths, key=lambda x: os.path.splitext(os.path.basename(x))[0])
     exit_segfail = FLAGS.exit_segfail
     stretch = FLAGS.stretch_on
     stretch_in_lang = FLAGS.stretch_in_language
 
     from subaligner.logger import Logger
     Logger.VERBOSE = FLAGS.debug
     Logger.QUIET = FLAGS.quiet
     from subaligner.predictor import Predictor
+    from subaligner.subtitle import Subtitle
     from subaligner.exception import UnsupportedFormatException
     from subaligner.exception import TerminalException
 
-    try:
-        if FLAGS.video_path.lower().startswith("http"):
-            _, local_video_path = tempfile.mkstemp()
-            _, video_file_extension = os.path.splitext(FLAGS.video_path.lower())
-            local_video_path = "{}{}".format(local_video_path, video_file_extension)
-            Utils.download_file(FLAGS.video_path, local_video_path)
-
-        if FLAGS.subtitle_path.lower().startswith("http"):
-            _, local_subtitle_path = tempfile.mkstemp()
-            _, subtitle_file_extension = os.path.splitext(FLAGS.subtitle_path.lower())
-            local_subtitle_path = "{}{}".format(local_subtitle_path, subtitle_file_extension)
-            Utils.download_file(FLAGS.subtitle_path, local_subtitle_path)
-
-        if FLAGS.subtitle_path.lower().startswith("embedded:"):
-            _, local_subtitle_path = tempfile.mkstemp()
-            _, subtitle_file_extension = os.path.splitext(FLAGS.output)
-            local_subtitle_path = "{}{}".format(local_subtitle_path, subtitle_file_extension)
-            params = FLAGS.subtitle_path.lower().split(":")[1].split(",")
-            if params and "=" in params[0]:
-                params = {param.split("=")[0]: param.split("=")[1] for param in params}
-                if "page_num" in params:
-                    Utils.extract_teletext_as_subtitle(local_video_path, int(params["page_num"]), local_subtitle_path)
-                elif "stream_index" in params:
-                    Utils.extract_matroska_subtitle(local_video_path, int(params["stream_index"]), local_subtitle_path)
+    predictor = Predictor()
+    failures = []
+    for index in range(len(video_file_paths)):
+        local_video_path = video_file_paths[index]
+        local_subtitle_path = subtitle_file_paths[index] if FLAGS.mode != "transcribe" else "{}.srt".format(tempfile.mkstemp()[1])
+        try:
+            voice_probabilities = None
+            if FLAGS.mode == "single":
+                aligned_subs, audio_file_path, voice_probabilities, frame_rate = predictor.predict_single_pass(
+                    video_file_path=local_video_path,
+                    subtitle_file_path=local_subtitle_path,
+                    weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights")
+                )
+            elif FLAGS.mode == "dual":
+                aligned_subs, subs, voice_probabilities, frame_rate = predictor.predict_dual_pass(
+                    video_file_path=local_video_path,
+                    subtitle_file_path=local_subtitle_path,
+                    weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights"),
+                    stretch=stretch,
+                    stretch_in_lang=stretch_in_lang,
+                    exit_segfail=exit_segfail,
+                )
+            elif FLAGS.mode == "script":
+                aligned_subs, _, voice_probabilities, frame_rate = predictor.predict_plain_text(
+                    video_file_path=local_video_path,
+                    subtitle_file_path=local_subtitle_path,
+                    stretch_in_lang=stretch_in_lang,
+                )
+            elif FLAGS.mode == "transcribe":
+                from subaligner.transcriber import Transcriber
+                transcriber = Transcriber(recipe=FLAGS.transcription_recipe, flavour=FLAGS.transcription_flavour)
+                subtitle, frame_rate = transcriber.transcribe(local_video_path, stretch_in_lang)
+                aligned_subs = subtitle.subs
+
+            if FLAGS.mode == "transcribe":
+                parent_dir = os.path.dirname(video_file_paths[index].replace(os.path.abspath(FLAGS.video_directory), output_dir))
+                os.makedirs(parent_dir, exist_ok=True)
+                file_parts = os.path.basename(video_file_paths[index]).rsplit(".", 1)
+                file_parts[1] = FLAGS.output_format if FLAGS.output_format != "" else "srt"
+                aligned_subtitle_path = os.path.abspath(os.path.join(parent_dir, ".".join(file_parts).replace(".stl", ".srt")))
             else:
-                print("ERROR: Embedded subtitle selector cannot be empty")
-                parser.print_usage()
-                sys.exit(21)
-
-        predictor = Predictor()
-        subs_list, subs, voice_probabilities, frame_rate = predictor.predict_dual_pass(
-            video_file_path=local_video_path,
-            subtitle_file_path=local_subtitle_path,
-            weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights"),
-            stretch=stretch,
-            stretch_in_lang=stretch_in_lang,
-            exit_segfail=exit_segfail,
-        )
-
-        aligned_subtitle_path = "_aligned.".join(
-            FLAGS.subtitle_path.rsplit(".", 1)).replace(".stl", ".srt") if FLAGS.output == "" else FLAGS.output
-
-        if FLAGS.translate is not None:
-            from subaligner.translator import Translator
-            source, target = FLAGS.translate.split(",")
-            translator = Translator(source, target)
-            subs_list = translator.translate(subs)
-            Subtitle.save_subs_as_target_format(subs_list, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
+                parent_dir = os.path.dirname(local_subtitle_path.replace(os.path.abspath(FLAGS.subtitle_directory), output_dir))
+                os.makedirs(parent_dir, exist_ok=True)
+                file_parts = os.path.basename(local_subtitle_path).rsplit(".", 1)
+                file_parts[1] = FLAGS.output_format if FLAGS.output_format != "" else file_parts[1]
+                aligned_subtitle_path = os.path.abspath(os.path.join(parent_dir, ".".join(file_parts).replace(".stl", ".srt")))
+
+            if FLAGS.translate is not None:
+                from subaligner.translator import Translator
+                source, target = FLAGS.translate.split(",")
+                translator = Translator(source, target)
+                aligned_subs = translator.translate(aligned_subs)
+                Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
+            elif FLAGS.mode == "transcribe":
+                Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
+            else:
+                Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate)
 
-        else:
-            Subtitle.save_subs_as_target_format(subs_list, local_subtitle_path, aligned_subtitle_path, frame_rate)
+            if voice_probabilities is not None:
+                log_loss = predictor.get_log_loss(voice_probabilities, aligned_subs)
+                if log_loss is None or log_loss > FLAGS.max_logloss:
+                    print(
+                        "ERROR: Alignment failed with a too high loss value: {} for {} and {}".format(log_loss, local_video_path, local_subtitle_path)
+                    )
+                    failures.append((local_video_path, local_subtitle_path))
+                    continue
 
-        log_loss = predictor.get_log_loss(voice_probabilities, subs_list)
-        if log_loss is None or log_loss > FLAGS.max_logloss:
+            print("Aligned subtitle saved to: {}".format(aligned_subtitle_path))
+        except UnsupportedFormatException as e:
             print(
-                "ERROR: Alignment failed with a too high loss value: {}".format(log_loss)
+                "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
             )
-            _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
-            sys.exit(22)
-
-        print("Aligned subtitle saved to: {}".format(aligned_subtitle_path))
-    except UnsupportedFormatException as e:
-        print(
-            "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
-        )
-        traceback.print_tb(e.__traceback__)
-        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
-        sys.exit(23)
-    except TerminalException as e:
-        print(
-            "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
-        )
-        traceback.print_tb(e.__traceback__)
-        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
-        sys.exit(24)
-    except Exception as e:
-        print(
-            "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
-        )
-        traceback.print_tb(e.__traceback__)
-        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
-        sys.exit(1)
-    else:
-        _remove_tmp_files(FLAGS, local_video_path, local_subtitle_path)
-        sys.exit(0)
-
+            traceback.print_tb(e.__traceback__)
+            failures.append((local_video_path, local_subtitle_path))
+            continue
+        except TerminalException as e:
+            print(
+                "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
+            )
+            traceback.print_tb(e.__traceback__)
+            failures.append((local_video_path, local_subtitle_path))
+            continue
+        except Exception as e:
+            print(
+                "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
+            )
+            traceback.print_tb(e.__traceback__)
+            failures.append((local_video_path, local_subtitle_path))
+            continue
+        else:
+            continue
 
-def _remove_tmp_files(flags, local_video_path, local_subtitle_path):
-    if flags.video_path.lower().startswith("http") and os.path.exists(local_video_path):
-        os.remove(local_video_path)
-    if flags.subtitle_path.lower().startswith("http") and os.path.exists(local_subtitle_path):
-        os.remove(local_subtitle_path)
+    if len(failures) > 0:
+        print("WARNING: The following video and subtitle failed to align with each other:")
+        for failure in failures:
+            video_file_path, subtitle_file_path = failure
+            print("\t{}  {}".format(video_file_path, subtitle_file_path))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `subaligner-0.3.0/subaligner/subaligner_batch/__main__.py` & `subaligner-0.3.1/subaligner/subaligner_batch/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 """
 
 import argparse
 import sys
 import traceback
 import os
 import pkg_resources
+import tempfile
 
 
 def main():
     if sys.version_info.major != 3:
         print("ERROR: Cannot find Python 3")
         sys.exit(20)
     try:
@@ -61,30 +62,30 @@
 Each file pair needs to share the same base filename, the part before the extension.""" % __version__, formatter_class=argparse.RawTextHelpFormatter)
     required_args = parser.add_argument_group("required arguments")
     required_args.add_argument(
         "-m",
         "--mode",
         type=str,
         default="",
-        choices=["single", "dual"],
+        choices=["single", "dual", "script", "transcribe"],
         help="Alignment mode: either single or dual",
     )
     parser.add_argument(
-        "-vd",
-        "--video_directory",
+        "-sd",
+        "--subtitle_directory",
         type=str,
         default="",
-        help="Path to the video directory",
+        help="Path to the subtitle directory",
     )
     parser.add_argument(
-        "-sd",
-        "--subtitle_directory",
+        "-vd",
+        "--video_directory",
         type=str,
         default="",
-        help="Path to the subtitle directory",
+        help="Path to the video directory",
     )
     parser.add_argument(
         "-l",
         "--max_logloss",
         type=float,
         default=float("inf"),
         help="Max global log loss for alignment",
@@ -135,14 +136,39 @@
     )
     parser.add_argument(
         "-t",
         "--translate",
         type=str,
         help="Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)",
     )
+    parser.add_argument(
+        "-ml",
+        "--main_language",
+        type=str.lower,
+        choices=Utils.get_stretch_language_codes(),
+        help="Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]",
+    )
+    from subaligner.llm import TranscriptionRecipe
+    from subaligner.llm import WhisperFlavour
+    parser.add_argument(
+        "-mr",
+        "--transcription_recipe",
+        type=str.lower,
+        default=TranscriptionRecipe.WHISPER.value,
+        choices=[r.value for r in TranscriptionRecipe],
+        help="LLM recipe used for transcribing video files"
+    )
+    parser.add_argument(
+        "-mf",
+        "--transcription_flavour",
+        type=str.lower,
+        default=WhisperFlavour.SMALL.value,
+        choices=[wf.value for wf in WhisperFlavour],
+        help="Flavour variation for a specific LLM recipe supporting transcription"
+    )
     parser.add_argument("-lgs", "--languages", action="store_true",
                         help="Print out language codes used for stretch and translation")
     parser.add_argument("-d", "--debug", action="store_true",
                         help="Print out debugging information")
     parser.add_argument("-q", "--quiet", action="store_true",
                         help="Switch off logging information")
     parser.add_argument("-ver", "--version", action="version", version=__version__)
@@ -155,44 +181,56 @@
         print("ERROR: --mode was not passed in")
         parser.print_usage()
         sys.exit(21)
     if FLAGS.video_directory == "":
         print("ERROR: --video_directory was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.subtitle_directory == "":
+    if FLAGS.mode != "transcribe" and FLAGS.subtitle_directory == "":
         print("ERROR: --subtitle_directory was not passed in")
         parser.print_usage()
         sys.exit(21)
     if FLAGS.output_directory == "":
         print("ERROR: --output_directory was not passed in")
         parser.print_usage()
         sys.exit(21)
-    if os.path.abspath(FLAGS.subtitle_directory) == os.path.abspath(FLAGS.output_directory):
+    if FLAGS.mode != "transcribe" and os.path.abspath(FLAGS.subtitle_directory) == os.path.abspath(FLAGS.output_directory):
         print("ERROR: The output directory cannot be set to the same as the input subtitle directory")
         parser.print_usage()
         sys.exit(21)
-    if FLAGS.translate is not None:
+    if FLAGS.translate is not None or FLAGS.mode == "transcribe":
         if "transformers" not in {pkg.key for pkg in pkg_resources.working_set}:
-            print('ERROR: Alignment has been configured to perform translation. Please install "subaligner[llm]" and run your command again.')
+            print('ERROR: Alignment has been configured to use language models. Please install "subaligner[llm]" and run your command again.')
+            sys.exit(21)
+    if FLAGS.stretch_on or FLAGS.mode == "script":
+        if "aeneas" not in {pkg.key for pkg in pkg_resources.working_set}:
+            print('ERROR: Alignment has been configured to use extra features. Please install "subaligner[stretch]" and run your command again.')
+            sys.exit(21)
+    if FLAGS.mode == "transcribe":
+        if FLAGS.main_language is None:
+            print("ERROR: --main_language was not passed in but required by mode 'transcribe'")
+            parser.print_usage()
             sys.exit(21)
 
     video_file_paths = [os.path.abspath(os.path.join(path, p)) for path, _, files in
                         os.walk(FLAGS.video_directory) for p in files if not p.startswith(".")]
-    subtitle_file_paths = [os.path.abspath(os.path.join(path, p)) for path, _, files in
-                           os.walk(FLAGS.subtitle_directory) for p in files if not p.startswith(".")]
-    if len(video_file_paths) != len(subtitle_file_paths):
-        print("ERROR: The numbers of input videos and subtitles do not match")
-        parser.print_usage()
-        sys.exit(21)
+
+    if FLAGS.mode != "transcribe":
+        subtitle_file_paths = [os.path.abspath(os.path.join(path, p)) for path, _, files in
+                               os.walk(FLAGS.subtitle_directory) for p in files if not p.startswith(".")]
+        if len(video_file_paths) != len(subtitle_file_paths):
+            print("ERROR: The numbers of input videos and subtitles do not match")
+            parser.print_usage()
+            sys.exit(21)
 
     output_dir = os.path.abspath(FLAGS.output_directory)
     os.makedirs(output_dir, exist_ok=True)
     video_file_paths = sorted(video_file_paths, key=lambda x: os.path.splitext(os.path.basename(x))[0])
-    subtitle_file_paths = sorted(subtitle_file_paths, key=lambda x: os.path.splitext(os.path.basename(x))[0])
+    if FLAGS.mode != "transcribe":
+        subtitle_file_paths = sorted(subtitle_file_paths, key=lambda x: os.path.splitext(os.path.basename(x))[0])
     exit_segfail = FLAGS.exit_segfail
     stretch = FLAGS.stretch_on
     stretch_in_lang = FLAGS.stretch_in_language
 
     from subaligner.logger import Logger
     Logger.VERBOSE = FLAGS.debug
     Logger.QUIET = FLAGS.quiet
@@ -201,54 +239,76 @@
     from subaligner.exception import UnsupportedFormatException
     from subaligner.exception import TerminalException
 
     predictor = Predictor()
     failures = []
     for index in range(len(video_file_paths)):
         local_video_path = video_file_paths[index]
-        local_subtitle_path = subtitle_file_paths[index]
+        local_subtitle_path = subtitle_file_paths[index] if FLAGS.mode != "transcribe" else "{}.srt".format(tempfile.mkstemp()[1])
         try:
+            voice_probabilities = None
             if FLAGS.mode == "single":
                 aligned_subs, audio_file_path, voice_probabilities, frame_rate = predictor.predict_single_pass(
                     video_file_path=local_video_path,
                     subtitle_file_path=local_subtitle_path,
                     weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights")
                 )
-            else:
+            elif FLAGS.mode == "dual":
                 aligned_subs, subs, voice_probabilities, frame_rate = predictor.predict_dual_pass(
                     video_file_path=local_video_path,
                     subtitle_file_path=local_subtitle_path,
                     weights_dir=os.path.join(FLAGS.training_output_directory, "models", "training", "weights"),
                     stretch=stretch,
                     stretch_in_lang=stretch_in_lang,
                     exit_segfail=exit_segfail,
                 )
-
-            parent_dir = os.path.dirname(local_subtitle_path.replace(os.path.abspath(FLAGS.subtitle_directory), output_dir))
-            os.makedirs(parent_dir, exist_ok=True)
-            file_parts = os.path.basename(local_subtitle_path).rsplit(".", 1)
-            file_parts[1] = FLAGS.output_format if FLAGS.output_format != "" else file_parts[1]
-            aligned_subtitle_path = os.path.abspath(os.path.join(parent_dir, ".".join(file_parts).replace(".stl", ".srt")))
+            elif FLAGS.mode == "script":
+                aligned_subs, _, voice_probabilities, frame_rate = predictor.predict_plain_text(
+                    video_file_path=local_video_path,
+                    subtitle_file_path=local_subtitle_path,
+                    stretch_in_lang=stretch_in_lang,
+                )
+            elif FLAGS.mode == "transcribe":
+                from subaligner.transcriber import Transcriber
+                transcriber = Transcriber(recipe=FLAGS.transcription_recipe, flavour=FLAGS.transcription_flavour)
+                subtitle, frame_rate = transcriber.transcribe(local_video_path, stretch_in_lang)
+                aligned_subs = subtitle.subs
+
+            if FLAGS.mode == "transcribe":
+                parent_dir = os.path.dirname(video_file_paths[index].replace(os.path.abspath(FLAGS.video_directory), output_dir))
+                os.makedirs(parent_dir, exist_ok=True)
+                file_parts = os.path.basename(video_file_paths[index]).rsplit(".", 1)
+                file_parts[1] = FLAGS.output_format if FLAGS.output_format != "" else "srt"
+                aligned_subtitle_path = os.path.abspath(os.path.join(parent_dir, ".".join(file_parts).replace(".stl", ".srt")))
+            else:
+                parent_dir = os.path.dirname(local_subtitle_path.replace(os.path.abspath(FLAGS.subtitle_directory), output_dir))
+                os.makedirs(parent_dir, exist_ok=True)
+                file_parts = os.path.basename(local_subtitle_path).rsplit(".", 1)
+                file_parts[1] = FLAGS.output_format if FLAGS.output_format != "" else file_parts[1]
+                aligned_subtitle_path = os.path.abspath(os.path.join(parent_dir, ".".join(file_parts).replace(".stl", ".srt")))
 
             if FLAGS.translate is not None:
                 from subaligner.translator import Translator
                 source, target = FLAGS.translate.split(",")
                 translator = Translator(source, target)
                 aligned_subs = translator.translate(aligned_subs)
                 Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
-            else:
+            elif FLAGS.mode == "transcribe":
                 Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate, "utf-8")
+            else:
+                Subtitle.save_subs_as_target_format(aligned_subs, local_subtitle_path, aligned_subtitle_path, frame_rate)
 
-            log_loss = predictor.get_log_loss(voice_probabilities, aligned_subs)
-            if log_loss is None or log_loss > FLAGS.max_logloss:
-                print(
-                    "ERROR: Alignment failed with a too high loss value: {} for {} and {}".format(log_loss, local_video_path, local_subtitle_path)
-                )
-                failures.append((local_video_path, local_subtitle_path))
-                continue
+            if voice_probabilities is not None:
+                log_loss = predictor.get_log_loss(voice_probabilities, aligned_subs)
+                if log_loss is None or log_loss > FLAGS.max_logloss:
+                    print(
+                        "ERROR: Alignment failed with a too high loss value: {} for {} and {}".format(log_loss, local_video_path, local_subtitle_path)
+                    )
+                    failures.append((local_video_path, local_subtitle_path))
+                    continue
 
             print("Aligned subtitle saved to: {}".format(aligned_subtitle_path))
         except UnsupportedFormatException as e:
             print(
                 "ERROR: {}\n{}".format(str(e), "".join(traceback.format_stack()) if FLAGS.debug else "")
             )
             traceback.print_tb(e.__traceback__)
```

### Comparing `subaligner-0.3.0/subaligner/subaligner_convert/__main__.py` & `subaligner-0.3.1/subaligner/subaligner_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/subaligner_train/__main__.py` & `subaligner-0.3.1/subaligner/subaligner_train/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/subaligner_tune/__main__.py` & `subaligner-0.3.1/subaligner/subaligner_tune/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/subtitle.py` & `subaligner-0.3.1/subaligner/subtitle.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/trainer.py` & `subaligner-0.3.1/subaligner/trainer.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.0/subaligner/transcriber.py` & `subaligner-0.3.1/subaligner/transcriber.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,81 @@
 import os
 import whisper
-from enum import Enum
 from typing import Tuple, Optional
 from pysrt import SubRipTime
 from whisper.tokenizer import LANGUAGES
 from .translator import Translator
 from .subtitle import Subtitle
 from .media_helper import MediaHelper
+from .llm import TranscriptionRecipe, WhisperFlavour
+from .singleton import Singleton
 from .logger import Logger
+from .utils import Utils
 from .exception import NoFrameRateException, TranscriptionException
 
 
 class Transcriber(object):
     """Transcribe audiovisual content for subtitle generation.
     """
 
-    def __init__(self, recipe: str = "whisper", flavour: str = "small") -> None:
+    def __init__(self, recipe: str = TranscriptionRecipe.WHISPER.value, flavour: str = WhisperFlavour.SMALL.value) -> None:
         """Initialiser for the transcribing process.
 
         Arguments:
             recipe {string} -- the LLM recipe used for transcribing video files (default: "whisper").
             flavour {string} -- the flavour variation for a specific LLM recipe (default: "small").
         Raises:
             NotImplementedError -- Thrown when the LLM recipe is unknown.
         """
-        if recipe not in [r.value for r in Recipe]:
+        if recipe not in [r.value for r in TranscriptionRecipe]:
             raise NotImplementedError(f"Unknown recipe: {recipe}")
-        if recipe == Recipe.whisper.value:
+        if recipe == TranscriptionRecipe.WHISPER.value:
             if flavour not in [f.value for f in WhisperFlavour]:
                 raise NotImplementedError(f"Unknown {recipe} flavour: {flavour}")
             self.__model = whisper.load_model(flavour)
-        self.recipe = recipe
-        self.flavour = flavour
+        self.__recipe = recipe
+        self.__flavour = flavour
         self.__media_helper = MediaHelper()
         self.__LOGGER = Logger().get_logger(__name__)
 
     def transcribe(self, video_file_path: str, language_code: str) -> Tuple[Subtitle, Optional[float]]:
         """Transcribe an audiovisual file and generate subtitles.
 
         Arguments:
             video_file_path {string} -- The input video file path.
             language_code {string} -- An alpha 3 language code derived from ISO 639-3.
         Raises:
             TranscriptionException -- Thrown when transcription is failed.
             NotImplementedError -- Thrown when the LLM recipe is not supported.
         """
-        if self.recipe == "whisper":
-            lang = Translator.get_iso_639_alpha_2(language_code)
+        if self.__recipe == "whisper":
+            lang = Utils.get_iso_639_alpha_2(language_code)
             if lang not in LANGUAGES:
-                raise TranscriptionException(f'"{language_code}" is not supported by {self.recipe} ({self.flavour})')
+                raise TranscriptionException(f'"{language_code}" is not supported by {self.__recipe} ({self.__flavour})')
             audio_file_path = self.__media_helper.extract_audio(video_file_path, True, 16000)
             try:
                 audio = whisper.load_audio(audio_file_path)
                 self.__LOGGER.debug("Start transcribing the audio...")
                 result = self.__model.transcribe(audio, task="transcribe", language=LANGUAGES[lang])
                 self.__LOGGER.info("Finished transcribing the audio")
                 srt_str = ""
                 for i, segment in enumerate(result["segments"], start=1):
                     srt_str += f"{i}\n" \
-                               f"{self.__format_timestamp(segment['start'])} --> {self.__format_timestamp(segment['end'])}\n" \
+                               f"{Utils.format_timestamp(segment['start'])} --> {Utils.format_timestamp(segment['end'])}\n" \
                                f"{segment['text'].strip().replace('-->', '->')}\n" \
                                "\n"
                 subtitle = Subtitle.load_subrip_str(srt_str)
                 subtitle, frame_rate = self.__on_frame_timecodes(subtitle, video_file_path)
                 self.__LOGGER.debug("Generated the raw subtitle")
                 return subtitle, frame_rate
             finally:
                 if os.path.exists(audio_file_path):
                     os.remove(audio_file_path)
         else:
-            raise NotImplementedError(f"{self.recipe} ({self.flavour}) is not supported")
-
-    @staticmethod
-    def __format_timestamp(seconds: float) -> str:
-        assert seconds >= 0, "non-negative timestamp expected"
-        milliseconds = round(seconds * 1000.0)
-        hours = milliseconds // 3_600_000
-        milliseconds -= hours * 3_600_000
-        minutes = milliseconds // 60_000
-        milliseconds -= minutes * 60_000
-        seconds = milliseconds // 1_000
-        milliseconds -= seconds * 1_000
-        hours_marker = f"{hours:02d}:"
-        return f"{hours_marker}{minutes:02d}:{seconds:02d},{milliseconds:03d}"
+            raise NotImplementedError(f"{self.__recipe} ({self.__flavour}) is not supported")
 
     def __on_frame_timecodes(self, subtitle: Subtitle, video_file_path: str) -> Tuple[Subtitle, Optional[float]]:
         frame_rate = None
         try:
             frame_rate = self.__media_helper.get_frame_rate(video_file_path)
             frame_duration = 1.0 / frame_rate
             for sub in subtitle.subs:
@@ -95,24 +84,7 @@
                 start_frames = int(start_seconds / frame_duration)
                 end_frames = int(end_seconds / frame_duration)
                 sub.start = SubRipTime(seconds=start_frames * frame_duration)
                 sub.end = SubRipTime(seconds=end_frames * frame_duration)
         except NoFrameRateException:
             self.__LOGGER.warning("Cannot detect the frame rate for %s" % video_file_path)
         return subtitle, frame_rate
-
-
-class Recipe(str, Enum):
-    whisper = "whisper"
-
-
-class WhisperFlavour(str, Enum):
-    tiny = "tiny"
-    tiny_en = "tiny.en"
-    small = "small"
-    medium = "medium"
-    medium_en = "medium.en"
-    base = "base"
-    base_en = "base.en"
-    large_v1 = "large-v1"
-    large_v2 = "large-v2"
-    large = "large"
```

### Comparing `subaligner-0.3.0/subaligner/utils.py` & `subaligner-0.3.1/subaligner/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import subprocess
 import pysubs2
 import requests
 import shutil
 import cchardet
 import shlex
+import pycountry
 
 from pycaption import (
     CaptionConverter,
     SRTWriter,
     SRTReader,
     DFXPWriter,
     DFXPReader,
@@ -83,15 +84,15 @@
             srt_file_path {string} -- The path to the SubRip file.
             vtt_file_path {string} -- The path to the WebVTT file.
             timeout_secs {int} -- The timeout in seconds on conversion {default: 30}.
         """
 
         _vtt_file_path = srt_file_path.replace(".srt", ".vtt") if vtt_file_path is None else vtt_file_path
         encoding = Utils.detect_encoding(srt_file_path)
-        command = "{0} -y -sub_charenc {1} -i '{2}' -f webvtt '{3}'".format(Utils.FFMPEG_BIN, encoding, srt_file_path, _vtt_file_path)
+        command = "{0} -y -sub_charenc {1} -i {2} -f webvtt {3}".format(Utils.FFMPEG_BIN, encoding, Utils.double_quoted(srt_file_path), Utils.double_quoted(_vtt_file_path))
         timeout_msg = "Timeout on converting SubRip to WebVTT: {}".format(srt_file_path)
         error_msg = "Cannot convert SubRip to WebVTT: {}".format(srt_file_path)
 
         def _callback(returncode: int, std_err: str) -> None:
             if returncode != 0:
                 raise TerminalException(
                     "Cannot convert SubRip to WebVTT: {} with error {}".format(
@@ -110,15 +111,15 @@
             vtt_file_path {string} -- The path to the WebVTT file.
             srt_file_path {string} -- The path to the SubRip file.
             timeout_secs {int} -- The timeout in seconds on conversion {default: 30}.
         """
 
         _srt_file_path = vtt_file_path.replace(".vtt", ".srt") if srt_file_path is None else srt_file_path
         encoding = Utils.detect_encoding(vtt_file_path)
-        command = "{0} -y -sub_charenc {1} -i '{2}' -f srt '{3}'".format(Utils.FFMPEG_BIN, encoding, vtt_file_path, _srt_file_path)
+        command = "{0} -y -sub_charenc {1} -i {2} -f srt {3}".format(Utils.FFMPEG_BIN, encoding, Utils.double_quoted(vtt_file_path), Utils.double_quoted(_srt_file_path))
         timeout_msg = "Timeout on converting WebVTT to SubRip: {}".format(vtt_file_path)
         error_msg = "Cannot convert WebVTT to SubRip: {}".format(vtt_file_path)
 
         def _callback(returncode: int, std_err: str) -> None:
             if returncode != 0:
                 raise TerminalException(
                     "Cannot convert WebVTT to SubRip: {} with error {}".format(
@@ -487,15 +488,15 @@
         Arguments:
             ts_file_path {string} -- The path to the Transport Stream file.
             page_num {int} -- The page number for the Teletext
             output_file_path {string} -- The path to the output file.
             timeout_secs {int} -- The timeout in seconds on extraction {default: 30}.
         """
 
-        command = "{0} -y -fix_sub_duration -txt_page {1} -txt_format text -i '{2}' '{3}'".format(Utils.FFMPEG_BIN, page_num, ts_file_path, output_file_path)
+        command = "{0} -y -fix_sub_duration -txt_page {1} -txt_format text -i {2} {3}".format(Utils.FFMPEG_BIN, page_num, Utils.double_quoted(ts_file_path), Utils.double_quoted(output_file_path))
         timeout_msg = "Timeout on extracting Teletext from transport stream: {} on page: {}".format(ts_file_path, page_num)
         error_msg = "Cannot extract Teletext from transport stream: {} on page: {}".format(ts_file_path, page_num)
 
         def _callback(returncode: int, std_err: str) -> None:
             if returncode != 0:
                 raise TerminalException(
                     "Cannot extract Teletext from transport stream: {} on page: {} with error {}".format(
@@ -513,15 +514,15 @@
         Arguments:
             mkv_file_path {string} -- The path to the Matroska file.
             stream_index {int} -- The index of the subtitle stream
             output_file_path {string} -- The path to the output file.
             timeout_secs {int} -- The timeout in seconds on extraction {default: 30}.
         """
 
-        command = "{0} -y -i '{1}' -map 0:s:{2} '{3}'".format(Utils.FFMPEG_BIN, mkv_file_path, stream_index, output_file_path)
+        command = "{0} -y -i {1} -map 0:s:{2} {3}".format(Utils.FFMPEG_BIN, Utils.double_quoted(mkv_file_path), stream_index, Utils.double_quoted(output_file_path))
         timeout_msg = "Timeout on extracting the subtitle from file: {} with stream index: {}".format(mkv_file_path, stream_index)
         error_msg = "Cannot extract the subtitle from file: {} with stream index: {}".format(mkv_file_path, stream_index)
 
         def _callback(returncode: int, std_err: str) -> None:
             if returncode != 0:
                 raise TerminalException(
                     "Cannot extract the subtitle from file: {} with stream index: {} with error {}".format(
@@ -565,15 +566,15 @@
             video_file_path {string} -- The path to the video file.
             timeout_secs {int} -- The timeout in seconds on extraction {default: 30}.
 
         Returns:
             bool -- True if the video contains embedded subtitles or False otherwise.
         """
 
-        command = "{0} -y -i '{1}' -c copy -map 0:s -f null - -v 0 -hide_banner".format(Utils.FFMPEG_BIN, video_file_path)
+        command = "{0} -y -i {1} -c copy -map 0:s -f null - -v 0 -hide_banner".format(Utils.FFMPEG_BIN, Utils.double_quoted(video_file_path))
         timeout_msg = "Timeout on detecting embedded subtitles from file: {}".format(video_file_path)
         error_msg = "Embedded subtitle detection failed for file: {}".format(video_file_path)
 
         def _callback(returncode: int, std_err: str) -> bool:
             return returncode == 0
         return Utils._run_command(command, timeout_secs, timeout_msg, error_msg, _callback)
 
@@ -649,14 +650,53 @@
              'gil', 'gmq', 'gmw', 'grk', 'guw', 'hil', 'iir', 'ilo', 'inc', 'ine', 'iso', 'itc', 'jap', 'kab', 'kqn',
              'kwn', 'kwy', 'loz', 'lua', 'lue', 'lun', 'luo', 'lus', 'map', 'mfe', 'mfs', 'mkh', 'mos', 'mul', 'nic',
              'niu', 'nso', 'nyk', 'pag', 'phi', 'pis', 'pon', 'poz', 'pqe', 'pqw', 'prl', 'rnd', 'roa', 'run', 'sal',
              'sem', 'sit', 'sla', 'srn', 'ssp', 'swc', 'taw', 'tdt', 'tiv', 'tll', 'toi', 'tpi', 'trk', 'tum', 'tut',
              'tvl', 'tzo', 'umb', 'urj', 'vsl', 'wal', 'war', 'wls', 'yap', 'yua', 'zai', 'zle', 'zls', 'zlw', 'zne']
 
     @staticmethod
+    def get_iso_639_alpha_2(language_code: str) -> str:
+        """Find the alpha 2 language code based on an alpha 3 one.
+
+        Arguments:
+            language_code {string} -- An alpha 3 language code derived from ISO 639-3.
+
+        Returns:
+            string -- The alpha 2 language code if exists otherwise the alpha 3 one.
+
+        Raises:
+            ValueError -- Thrown when the input language code cannot be recognised.
+        """
+
+        lang = pycountry.languages.get(alpha_3=language_code)
+        if lang is None:
+            return language_code
+        elif hasattr(lang, "alpha_2"):
+            return lang.alpha_2
+        else:
+            return lang.alpha_3
+
+    @staticmethod
+    def format_timestamp(seconds: float) -> str:
+        assert seconds >= 0, "non-negative timestamp expected"
+        milliseconds = round(seconds * 1000.0)
+        hours = milliseconds // 3_600_000
+        milliseconds -= hours * 3_600_000
+        minutes = milliseconds // 60_000
+        milliseconds -= minutes * 60_000
+        seconds = milliseconds // 1_000
+        milliseconds -= seconds * 1_000
+        hours_marker = f"{hours:02d}:"
+        return f"{hours_marker}{minutes:02d}:{seconds:02d},{milliseconds:03d}"
+
+    @staticmethod
+    def double_quoted(s: str) -> str:
+        return "\"{}\"".format(s.replace('"', "\\\""))
+
+    @staticmethod
     def __convert_subtitle(source_file_path: str, source_ext: str, target_file_path: Optional[str], target_ext: str, format: str, frame_rate: Optional[float] = None) -> Tuple[str, str]:
         encoding = Utils.detect_encoding(source_file_path)
         subs = pysubs2.load(source_file_path, encoding=encoding)
         new_target_file_path = source_file_path.replace(".%s" % source_ext, ".%s" % target_ext) if target_file_path is None else target_file_path
         if frame_rate is None:
             subs.save(new_target_file_path, encoding=encoding, format_=format)
         else:
```

### Comparing `subaligner-0.3.0/subaligner.egg-info/PKG-INFO` & `subaligner-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,49 @@
-Metadata-Version: 2.1
-Name: subaligner
-Version: 0.3.0
-Summary: Automatically synchronize and translate subtitles with pretrained deep neural networks, forced alignments and transformers.
-Home-page: https://subaligner.readthedocs.io/en/latest/
-Author: Xi Bai
-Author-email: xi.bai.ed@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: harmony
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: stretch
-Provides-Extra: translation
-Provides-Extra: llm
-License-File: LICENSE
-
 <div align="center">
   <img src="./figures/subaligner.png" alt="subaligner" width="300" />
 </div>
 
 [![Build Status](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml/badge.svg?branch=master)](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml?query=branch%3Amaster) ![Codecov](https://img.shields.io/codecov/c/github/baxtree/subaligner)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/) [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/subaligner/badge/?version=latest)](https://subaligner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/baxtree/subaligner)](https://github.com/baxtree/subaligner/blob/master/LICENSE)
 [![PyPI](https://badge.fury.io/py/subaligner.svg)](https://badge.fury.io/py/subaligner)
 [![Docker Build](https://img.shields.io/docker/cloud/build/baxtree/subaligner?label=Docker&style=flat)](https://hub.docker.com/r/baxtree/subaligner/builds)
 [![Docker Pulls](https://img.shields.io/docker/pulls/baxtree/subaligner)](https://hub.docker.com/r/baxtree/subaligner)
 [![Citation](https://zenodo.org/badge/228440472.svg)](https://doi.org/10.5281/zenodo.5603083)
 
 ## Supported Formats
 Subtitle: SubRip, TTML, WebVTT, (Advanced) SubStation Alpha, MicroDVD, MPL2, TMP, EBU STL, SAMI, SCC and SBV.
 
 Video/Audio: MP4, WebM, Ogg, 3GP, FLV, MOV, Matroska, MPEG TS, WAV, MP3, AAC, FLAC, etc.
 
+:information_source: <small style="line-height: 1.2;">Subaligner relies on file extensions as default hints to process a wide range of audiovisual or subtitle formats. It is recommended to use extensions widely acceppted by the community to ensure compatibility.</small>
+
 ## Dependencies
 Required by basic: [FFmpeg](https://www.ffmpeg.org/)
 ```
 $ apt-get install ffmpeg
 ```
 or
 ```
 $ brew install ffmpeg
 ```
 
 ## Basic Installation
 ```
-$ pip install -U pip
+$ pip install -U pip && pip install -U setuptools
 $ pip install subaligner
 ```
+or install from source:
+```
+$ git clone git@github.com:baxtree/subaligner.git && cd subaligner
+$ pip install -U pip && pip install -U setuptools
+$ python setup.py install
+```
+:information_source: <small style="line-height: 1.2;">It is highly recommended creating a virtual environment prior to installation.</small>
 
 ## Installation with Optional Packages Supporting Additional Features
 ```
 # Install dependencies for enabling translation and transcription
 
 $ pip install 'subaligner[llm]'
 ```
@@ -80,73 +66,44 @@
 $ brew install espeak
 ```
 To install all supported features:
 ```
 $ pip install 'subaligner[harmony]'
 ```
 
-## Alternative Installations
-```
-# Install via pipx
-$ pip install -U pip pipx
-$ pipx install subaligner
-```
-or
-```
-# Install from GitHub via Pipenv
-$ pipenv install subaligner
-$ pipenv install 'subaligner[stretch]'
-$ pipenv install 'subaligner[dev]'
-```
-or
-```
-# Install from source
+## Container Support
+If you prefer using a containerised environment over installing everything locally, run:
 
-$ git clone git@github.com:baxtree/subaligner.git
-$ cd subaligner
-$ python setup.py install
-```
-or
 ```
-# Use dockerised installation
-
 $ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner bash
 ```
 For users on Windows 10: [Docker Desktop](https://docs.docker.com/docker-for-windows/install/) is the only option at present.
 Assuming your media assets are stored under `d:\media`, open built-in command prompt, PowerShell, or Windows Terminal and run:
 ```
 docker pull baxtree/subaligner
 docker run -v "/d/media":/media -w "/media" -it baxtree/subaligner bash
 ```
 
 ## Usage
 ```
 # Single-stage alignment (high-level shift with lower latency)
 
-$ subaligner_1pass -v video.mp4 -s subtitle.srt
-$ subaligner_1pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ subaligner -m single -v video.mp4 -s subtitle.srt
+$ subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
 ```
 # Dual-stage alignment (low-level shift with higher latency)
 
-$ subaligner_2pass -v video.mp4 -s subtitle.srt
-$ subaligner_2pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
-```
-or
-```
-# Pass in single-stage or dual-stage as the alignment mode
-
-$ subaligner -m single -v video.mp4 -s subtitle.srt
 $ subaligner -m dual -v video.mp4 -s subtitle.srt
-$ subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 $ subaligner -m dual -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
 ```
 # Generate subtitles by transcribing audiovisual files
 $ subaligner -m transcribe -v video.mp4 -ml eng -mr whisper -mf small -o subtitle_aligned.srt
+$ subaligner -m transcribe -v video.mp4 -ml zho -mr whisper -mf medium -o subtitle_aligned.srt
 ```
 ```
 # Alignment on segmented plain texts (double newlines as the delimiter)
 
 $ subaligner -m script -v test.mp4 -s subtitle.txt -o subtitle_aligned.srt
 $ subaligner -m script -v https://example.com/video.mp4 -s https://example.com/subtitle.txt -o subtitle_aligned.srt
 ```
@@ -160,19 +117,27 @@
 # Alignment on embedded subtitles
 
 $ subaligner -m single -v video.mkv -s embedded:stream_index=0 -o subtitle_aligned.srt
 $ subaligner -m dual -v video.mkv -s embedded:stream_index=0 -o subtitle_aligned.srt
 ```
 ```
 # Translative alignment with the ISO 639-3 language code pair (src,tgt)
+
 $ subaligner --languages
 $ subaligner -m single -v video.mp4 -s subtitle.srt -t src,tgt
 $ subaligner -m dual -v video.mp4 -s subtitle.srt -t src,tgt
 $ subaligner -m script -v test.mp4 -s subtitle.txt -o subtitle_aligned.srt -t src,tgt
-$ subaligner -m transcribe -v video.mp4 -ml eng -mr whisper -mf small -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr helsinki-nlp -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr facebook-mbart -tf large -o subtitle_aligned.srt -t src,tgt
+$ subaligner -m dual -v video.mp4 -tr whisper -tf small -o subtitle_aligned.srt -t src,eng
+```
+```
+# Transcribe audiovisual files and generate translated subtitles
+
+$ subaligner -m transcribe -v video.mp4 -ml src -mr whisper -mf small -tr helsinki-nlp -o subtitle_aligned.srt -t src,tgt
 ```
 ```
 # Shift subtitle manually by offset in seconds
 
 $ subaligner -m shift --subtitle_path subtitle.srt -os 5.5
 $ subaligner -m shift --subtitle_path subtitle.srt -os -5.5 -o subtitle_shifted.srt
 ```
@@ -189,28 +154,25 @@
 $ pipx run subaligner -m single -v video.mp4 -s subtitle.srt
 $ pipx run subaligner -m dual -v video.mp4 -s subtitle.srt
 ```
 ```
 # Run the module as a script
 $ python -m subaligner -m single -v video.mp4 -s subtitle.srt
 $ python -m subaligner -m dual -v video.mp4 -s subtitle.srt
-$ python -m subaligner.subaligner_1pass -v video.mp4 -s subtitle.srt
-$ python -m subaligner.subaligner_2pass -v video.mp4 -s subtitle.srt
 ```
 ```
 # Run alignments with the docker image
 
 $ docker pull baxtree/subaligner
-$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner_1pass -v video.mp4 -s subtitle.srt
-$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner_2pass -v video.mp4 -s subtitle.srt
-$ docker run -it baxtree/subaligner subaligner_1pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
-$ docker run -it baxtree/subaligner subaligner_2pass -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner -m single -v video.mp4 -s subtitle.srt
+$ docker run -v `pwd`:`pwd` -w `pwd` -it baxtree/subaligner subaligner -m dual -v video.mp4 -s subtitle.srt
+$ docker run -it baxtree/subaligner subaligner -m single -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
+$ docker run -it baxtree/subaligner subaligner -m dual -v https://example.com/video.mp4 -s https://example.com/subtitle.srt -o subtitle_aligned.srt
 ```
-The aligned subtitle will be saved at `subtitle_aligned.srt`. For details on CLI, run `subaligner_1pass -h`, `subaligner_2pass -h` or `subaligner -h`.
-Additional utilities can be used after consulting `subaligner_batch -h`, `subaligner_convert -h`, `subaligner_train -h` and `subaligner_tune -h`.
+The aligned subtitle will be saved at `subtitle_aligned.srt`. For details on CLIs, run `subaligner -h` or `subaligner_batch -h`, `subaligner_convert -h`, `subaligner_train -h` and `subaligner_tune -h` for additional utilities. `subaligner_1pass` and `subaligner_2pass` are shortcuts for running `subaligner` with `-m single` and `-m dual` options, respectively.
 
 ![](figures/screencast.gif)
 
 ## Advanced Usage
 You can train a new model with your own audiovisual files and subtitle files:
 ```
 $ subaligner_train -vd VIDEO_DIRECTORY -sd SUBTITLE_DIRECTORY -tod TRAINING_OUTPUT_DIRECTORY
@@ -237,9 +199,7 @@
 [pysrt](https://github.com/byroot/pysrt)
 [pysubs2](https://github.com/tkarabela/pysubs2)
 [aeneas](https://www.readbeyond.it/aeneas/)
 [transformers](https://huggingface.co/transformers/)
 [openai-whisper](https://github.com/openai/whisper).
 
 Thanks to Alan Robinson and Nigel Megitt for their invaluable feedback.
-
-
```

### Comparing `subaligner-0.3.0/subaligner.egg-info/SOURCES.txt` & `subaligner-0.3.1/subaligner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 subaligner/__init__.py
 subaligner/__main__.py
 subaligner/_version.py
 subaligner/embedder.py
 subaligner/exception.py
 subaligner/hparam_tuner.py
 subaligner/hyperparameters.py
+subaligner/llm.py
 subaligner/logger.py
 subaligner/media_helper.py
 subaligner/network.py
 subaligner/predictor.py
 subaligner/singleton.py
 subaligner/subtitle.py
 subaligner/trainer.py
```

### Comparing `subaligner-0.3.0/subaligner.egg-info/requires.txt` & `subaligner-0.3.1/subaligner.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 zict==0.1.3
 Werkzeug>=0.15.3
 urllib3~=1.26.5
 tornado==5.1.0
 toolz==0.9.0
 toml==0.10.0
 termcolor==1.1.0
-tensorflow<2.9,>=1.15.5
+tensorflow<2.12,>=1.15.5
 tblib==1.3.2
 six~=1.15.0
 setuptools>=41.0.0
-scikit-learn~=0.24.2
+scikit-learn<1.2.0
 scipy<=1.8.1
 rsa==4.7
 requests-oauthlib==1.3.0
 requests~=2.25.1
 PyYAML>=4.2b1
 pytz==2018.4
 pystack-debugger==0.8.0
@@ -29,53 +29,50 @@
 py==1.10.0
 psutil==5.6.7
 pluggy==0.13.1
 pbr==4.0.2
 oauthlib==3.1.0
 numpy<1.24.0
 numba>=0.50.0
-msgpack-python==0.5.6
 networkx>=2.5.1
 mccabe==0.6.1
 Markdown==2.6.11
 locket==0.2.0
-librosa>=0.8.0
+librosa<0.10.0
 le-pycaption==2.2.0a1
 lazy-object-proxy==1.4.3
 kiwisolver==1.0.1
 Keras-Preprocessing>=1.0.9
 Keras-Applications>=1.0.8
+joblib>=1.2.0
 isort==4.3.4
 idna==2.8
 hyperopt==0.2.4
 html5lib==1.0b9
 h5py<=3.6.0
 HeapDict==1.0.0
 graphviz==0.8.3
 google-pasta~=0.2
 google-auth-oauthlib==0.4.2
-google-auth==1.27.0
 filelock<4.0.0
 distributed==1.13.0
 decorator==4.3.0
-dask<2022.1.0
+dask<2022.1.0,>=2021.10.0
 Cython~=0.29.22
 cycler==0.10.0
 cloudpickle~=1.6.0
 click==5.1
 chardet==3.0.4
 certifi==2019.11.28
 cchardet==2.1.7
 captionstransformer~=1.2.1
 cachetools==3.1.1
 bleach==3.3.0
 beautifulsoup4<4.9.0
-audioread==2.1.5
 astor==0.7.1
-absl-py~=0.10
 
 [dev]
 pygments==2.7.4
 pylint~=2.8.2
 parameterized==0.8.1
 typing-extensions<4.0.0
 types-setuptools==57.4.9
```

