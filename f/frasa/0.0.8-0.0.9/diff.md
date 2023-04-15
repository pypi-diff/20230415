# Comparing `tmp/frasa-0.0.8.tar.gz` & `tmp/frasa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasa-0.0.8.tar", last modified: Fri Apr 14 22:53:09 2023, max compression
+gzip compressed data, was "frasa-0.0.9.tar", last modified: Sat Apr 15 19:28:24 2023, max compression
```

## Comparing `frasa-0.0.8.tar` & `frasa-0.0.9.tar`

### file list

```diff
@@ -1,62 +1,72 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.729555 frasa-0.0.8/
--rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.0.8/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 22:53:09.729382 frasa-0.0.8/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     1700 2023-04-12 08:34:25.000000 frasa-0.0.8/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.721151 frasa-0.0.8/frasa/
--rw-r--r--   0 novay      (501) staff       (20)      514 2023-04-14 22:48:21.000000 frasa-0.0.8/frasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.722451 frasa-0.0.8/frasa/datasets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.0.8/frasa/datasets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.722613 frasa-0.0.8/frasa/datasets/corpus/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.0.8/frasa/datasets/corpus/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.722799 frasa-0.0.8/frasa/datasets/corpus/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.0.8/frasa/datasets/corpus/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.722966 frasa-0.0.8/frasa/datasets/corpus/indonesia/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.0.8/frasa/datasets/corpus/indonesia/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.723097 frasa-0.0.8/frasa/datasets/corpus/sensor/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.0.8/frasa/datasets/corpus/sensor/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.723240 frasa-0.0.8/frasa/datasets/corpus/tweets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.0.8/frasa/datasets/corpus/tweets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.723384 frasa-0.0.8/frasa/datasets/models/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.0.8/frasa/datasets/models/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.723504 frasa-0.0.8/frasa/deteksi/
--rw-r--r--   0 novay      (501) staff       (20)      980 2023-04-14 16:03:46.000000 frasa-0.0.8/frasa/deteksi/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.723696 frasa-0.0.8/frasa/deteksi/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.0.8/frasa/deteksi/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.723838 frasa-0.0.8/frasa/deteksi/bahasa/data/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.0.8/frasa/deteksi/bahasa/data/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.724390 frasa-0.0.8/frasa/deteksi/gender/
--rw-r--r--   0 novay      (501) staff       (20)      596 2023-04-14 11:05:42.000000 frasa-0.0.8/frasa/deteksi/gender/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     2712 2023-04-14 11:07:12.000000 frasa-0.0.8/frasa/deteksi/gender/classify.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.724946 frasa-0.0.8/frasa/deteksi/gender/data/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:59.000000 frasa-0.0.8/frasa/deteksi/gender/data/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)   121063 2023-04-14 10:10:52.000000 frasa-0.0.8/frasa/deteksi/gender/data/frasa-gender.pickle
--rw-r--r--   0 novay      (501) staff       (20)  2815899 2023-04-13 22:34:54.000000 frasa-0.0.8/frasa/deteksi/gender/data/nama-gender-combined.csv
--rw-r--r--   0 novay      (501) staff       (20)      789 2023-04-14 10:06:04.000000 frasa-0.0.8/frasa/deteksi/gender/utils.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.727118 frasa-0.0.8/frasa/deteksi/plagiat/
--rw-r--r--   0 novay      (501) staff       (20)       68 2023-04-12 08:57:39.000000 frasa-0.0.8/frasa/deteksi/plagiat/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     3708 2023-04-12 09:03:02.000000 frasa-0.0.8/frasa/deteksi/plagiat/plagiat.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.728018 frasa-0.0.8/frasa/sensor/
--rw-r--r--   0 novay      (501) staff       (20)       45 2023-04-14 16:27:02.000000 frasa-0.0.8/frasa/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      433 2023-04-11 19:58:03.000000 frasa-0.0.8/frasa/sensor/constants.py
--rw-r--r--   0 novay      (501) staff       (20)     9277 2023-04-14 16:25:42.000000 frasa-0.0.8/frasa/sensor/sensor.py
--rw-r--r--   0 novay      (501) staff       (20)     1572 2023-04-11 19:56:18.000000 frasa-0.0.8/frasa/sensor/utils.py
--rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.0.8/frasa/sensor/variasi.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.722242 frasa-0.0.8/frasa.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 22:53:09.000000 frasa-0.0.8/frasa.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     1173 2023-04-14 22:53:09.000000 frasa-0.0.8/frasa.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-14 22:53:09.000000 frasa-0.0.8/frasa.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)        5 2023-04-14 22:53:09.000000 frasa-0.0.8/frasa.egg-info/requires.txt
--rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-14 22:53:09.000000 frasa-0.0.8/frasa.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-14 22:53:09.729604 frasa-0.0.8/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1145 2023-04-14 22:52:29.000000 frasa-0.0.8/setup.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.728187 frasa-0.0.8/tests/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:39.000000 frasa-0.0.8/tests/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.728426 frasa-0.0.8/tests/lemmatisasi/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:52:26.000000 frasa-0.0.8/tests/lemmatisasi/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:41.000000 frasa-0.0.8/tests/lemmatisasi/test_lemmatizer.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.728637 frasa-0.0.8/tests/stopword/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:51:58.000000 frasa-0.0.8/tests/stopword/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:38.000000 frasa-0.0.8/tests/stopword/test_stopword.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:53:09.728898 frasa-0.0.8/tests/tokenisasi/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:53.000000 frasa-0.0.8/tests/tokenisasi/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:33.000000 frasa-0.0.8/tests/tokenisasi/test_tokenizer.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.560121 frasa-0.0.9/
+-rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.0.9/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)     1064 2023-04-15 19:28:24.559959 frasa-0.0.9/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)      338 2023-04-14 23:09:29.000000 frasa-0.0.9/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.537397 frasa-0.0.9/frasa/
+-rw-r--r--   0 novay      (501) staff       (20)      535 2023-04-15 19:28:11.000000 frasa-0.0.9/frasa/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      364 2023-04-15 12:25:54.000000 frasa-0.0.9/frasa/base.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.538254 frasa-0.0.9/frasa/datasets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.0.9/frasa/datasets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.538827 frasa-0.0.9/frasa/datasets/corpus/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.0.9/frasa/datasets/corpus/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.538971 frasa-0.0.9/frasa/datasets/corpus/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.0.9/frasa/datasets/corpus/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.539098 frasa-0.0.9/frasa/datasets/corpus/indonesia/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.0.9/frasa/datasets/corpus/indonesia/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.539212 frasa-0.0.9/frasa/datasets/corpus/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.0.9/frasa/datasets/corpus/sensor/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.539330 frasa-0.0.9/frasa/datasets/corpus/tweets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.0.9/frasa/datasets/corpus/tweets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.539438 frasa-0.0.9/frasa/datasets/models/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.0.9/frasa/datasets/models/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.539545 frasa-0.0.9/frasa/deteksi/
+-rw-r--r--   0 novay      (501) staff       (20)      980 2023-04-14 16:03:46.000000 frasa-0.0.9/frasa/deteksi/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.539718 frasa-0.0.9/frasa/deteksi/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.0.9/frasa/deteksi/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.539865 frasa-0.0.9/frasa/deteksi/bahasa/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.0.9/frasa/deteksi/bahasa/data/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.540555 frasa-0.0.9/frasa/deteksi/gender/
+-rw-r--r--   0 novay      (501) staff       (20)      596 2023-04-14 11:05:42.000000 frasa-0.0.9/frasa/deteksi/gender/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     2712 2023-04-14 11:07:12.000000 frasa-0.0.9/frasa/deteksi/gender/classify.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.546294 frasa-0.0.9/frasa/deteksi/gender/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:59.000000 frasa-0.0.9/frasa/deteksi/gender/data/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)   121063 2023-04-14 10:10:52.000000 frasa-0.0.9/frasa/deteksi/gender/data/frasa-gender.pickle
+-rw-r--r--   0 novay      (501) staff       (20)   133974 2023-04-14 23:11:57.000000 frasa-0.0.9/frasa/deteksi/gender/data/frasa-gender.pkl
+-rw-r--r--   0 novay      (501) staff       (20)  2815899 2023-04-13 22:34:54.000000 frasa-0.0.9/frasa/deteksi/gender/data/nama-gender-combined.csv
+-rw-r--r--   0 novay      (501) staff       (20) 16459307 2023-04-14 23:11:57.000000 frasa-0.0.9/frasa/deteksi/gender/data/nama.csv
+-rw-r--r--   0 novay      (501) staff       (20)      789 2023-04-14 10:06:04.000000 frasa-0.0.9/frasa/deteksi/gender/utils.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.557598 frasa-0.0.9/frasa/deteksi/plagiat/
+-rw-r--r--   0 novay      (501) staff       (20)       68 2023-04-12 08:57:39.000000 frasa-0.0.9/frasa/deteksi/plagiat/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     3708 2023-04-12 09:03:02.000000 frasa-0.0.9/frasa/deteksi/plagiat/plagiat.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.558359 frasa-0.0.9/frasa/scrap/
+-rw-r--r--   0 novay      (501) staff       (20)       88 2023-04-15 12:14:39.000000 frasa-0.0.9/frasa/scrap/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:09.000000 frasa-0.0.9/frasa/scrap/cnn.py
+-rw-r--r--   0 novay      (501) staff       (20)     7923 2023-04-15 18:28:08.000000 frasa-0.0.9/frasa/scrap/detiknews.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:14.000000 frasa-0.0.9/frasa/scrap/liputan6.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:30.000000 frasa-0.0.9/frasa/scrap/tribun.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:21.000000 frasa-0.0.9/frasa/scrap/viva.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.558996 frasa-0.0.9/frasa/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)       45 2023-04-14 16:27:02.000000 frasa-0.0.9/frasa/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      433 2023-04-11 19:58:03.000000 frasa-0.0.9/frasa/sensor/constants.py
+-rw-r--r--   0 novay      (501) staff       (20)     9277 2023-04-14 16:25:42.000000 frasa-0.0.9/frasa/sensor/sensor.py
+-rw-r--r--   0 novay      (501) staff       (20)     1572 2023-04-11 19:56:18.000000 frasa-0.0.9/frasa/sensor/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.0.9/frasa/sensor/variasi.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.538089 frasa-0.0.9/frasa.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     1064 2023-04-15 19:28:24.000000 frasa-0.0.9/frasa.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     1399 2023-04-15 19:28:24.000000 frasa-0.0.9/frasa.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-15 19:28:24.000000 frasa-0.0.9/frasa.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)        5 2023-04-15 19:28:24.000000 frasa-0.0.9/frasa.egg-info/requires.txt
+-rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-15 19:28:24.000000 frasa-0.0.9/frasa.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-15 19:28:24.560168 frasa-0.0.9/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1145 2023-04-15 19:26:55.000000 frasa-0.0.9/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.559127 frasa-0.0.9/tests/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:39.000000 frasa-0.0.9/tests/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.559332 frasa-0.0.9/tests/lemmatisasi/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:52:26.000000 frasa-0.0.9/tests/lemmatisasi/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:41.000000 frasa-0.0.9/tests/lemmatisasi/test_lemmatizer.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.559537 frasa-0.0.9/tests/stopword/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:51:58.000000 frasa-0.0.9/tests/stopword/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:38.000000 frasa-0.0.9/tests/stopword/test_stopword.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-15 19:28:24.559755 frasa-0.0.9/tests/tokenisasi/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:53.000000 frasa-0.0.9/tests/tokenisasi/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:33.000000 frasa-0.0.9/tests/tokenisasi/test_tokenizer.py
```

### Comparing `frasa-0.0.8/LICENSE` & `frasa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/__init__.py` & `frasa-0.0.9/frasa/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,14 @@
 
 Kunjungi http://frasa.id untuk informasi selengkapnya.
 """
 
 import os
 
 __name__ = "frasa"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __license__ = 'MIT'
 __author__ = 'Novianto Rahmadi'
 
-PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
+PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
+
+from .base import *
```

### Comparing `frasa-0.0.8/frasa/deteksi/__init__.py` & `frasa-0.0.9/frasa/deteksi/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/deteksi/gender/__init__.py` & `frasa-0.0.9/frasa/deteksi/gender/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/deteksi/gender/classify.py` & `frasa-0.0.9/frasa/deteksi/gender/classify.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/deteksi/gender/data/frasa-gender.pickle` & `frasa-0.0.9/frasa/deteksi/gender/data/frasa-gender.pickle`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/deteksi/gender/data/nama-gender-combined.csv` & `frasa-0.0.9/frasa/deteksi/gender/data/nama-gender-combined.csv`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/deteksi/gender/utils.py` & `frasa-0.0.9/frasa/deteksi/gender/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/deteksi/plagiat/plagiat.py` & `frasa-0.0.9/frasa/deteksi/plagiat/plagiat.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/sensor/sensor.py` & `frasa-0.0.9/frasa/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/sensor/utils.py` & `frasa-0.0.9/frasa/sensor/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa/sensor/variasi.py` & `frasa-0.0.9/frasa/sensor/variasi.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.8/frasa.egg-info/SOURCES.txt` & `frasa-0.0.9/frasa.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 frasa/__init__.py
+frasa/base.py
 frasa.egg-info/PKG-INFO
 frasa.egg-info/SOURCES.txt
 frasa.egg-info/dependency_links.txt
 frasa.egg-info/requires.txt
 frasa.egg-info/top_level.txt
 frasa/datasets/__init__.py
 frasa/datasets/corpus/__init__.py
@@ -18,17 +19,25 @@
 frasa/deteksi/bahasa/__init__.py
 frasa/deteksi/bahasa/data/__init__.py
 frasa/deteksi/gender/__init__.py
 frasa/deteksi/gender/classify.py
 frasa/deteksi/gender/utils.py
 frasa/deteksi/gender/data/__init__.py
 frasa/deteksi/gender/data/frasa-gender.pickle
+frasa/deteksi/gender/data/frasa-gender.pkl
 frasa/deteksi/gender/data/nama-gender-combined.csv
+frasa/deteksi/gender/data/nama.csv
 frasa/deteksi/plagiat/__init__.py
 frasa/deteksi/plagiat/plagiat.py
+frasa/scrap/__init__.py
+frasa/scrap/cnn.py
+frasa/scrap/detiknews.py
+frasa/scrap/liputan6.py
+frasa/scrap/tribun.py
+frasa/scrap/viva.py
 frasa/sensor/__init__.py
 frasa/sensor/constants.py
 frasa/sensor/sensor.py
 frasa/sensor/utils.py
 frasa/sensor/variasi.py
 tests/__init__.py
 tests/lemmatisasi/__init__.py
```

### Comparing `frasa-0.0.8/setup.py` & `frasa-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="frasa",
-    version="0.0.8",
+    version="0.0.9",
     description="Koleksi NLP Pribadi untuk Bahasa Indonesia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/python/tree/main/frasa",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
```

