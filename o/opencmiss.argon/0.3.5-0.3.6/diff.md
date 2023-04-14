# Comparing `tmp/opencmiss.argon-0.3.5.tar.gz` & `tmp/opencmiss.argon-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.argon-0.3.5.tar", last modified: Sun Sep  4 11:43:57 2022, max compression
+gzip compressed data, was "opencmiss.argon-0.3.6.tar", last modified: Fri Apr 14 22:56:35 2023, max compression
```

## Comparing `opencmiss.argon-0.3.5.tar` & `opencmiss.argon-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-04 11:43:57.415277 opencmiss.argon-0.3.5/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2021-06-16 01:34:31.000000 opencmiss.argon-0.3.5/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1121 2022-09-04 11:43:57.415008 opencmiss.argon-0.3.5/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      159 2021-06-16 01:34:31.000000 opencmiss.argon-0.3.5/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2022-09-04 11:43:57.415382 opencmiss.argon-0.3.5/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1450 2022-03-10 00:56:18.000000 opencmiss.argon-0.3.5/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-04 11:43:57.401733 opencmiss.argon-0.3.5/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-04 11:43:57.403139 opencmiss.argon-0.3.5/src/opencmiss/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      124 2021-06-16 00:43:37.000000 opencmiss.argon-0.3.5/src/opencmiss/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-04 11:43:57.413461 opencmiss.argon-0.3.5/src/opencmiss/argon/
--rw-r--r--   0 hsor001  (1210695619) 1403514002       22 2022-09-04 11:43:26.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     8835 2022-06-26 23:32:17.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argondocument.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      894 2022-06-26 23:19:25.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonerror.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5737 2022-06-26 23:19:25.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonlogger.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2069 2022-08-12 04:33:31.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonmaterials.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5839 2022-09-02 22:18:52.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonmodelsources.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    18417 2022-08-12 20:01:39.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonregion.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    11333 2022-06-26 23:19:25.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonsceneviewer.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7031 2022-08-12 04:33:37.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonspectrums.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2239 2022-08-12 04:33:44.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argontessellations.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     9255 2022-08-12 04:33:51.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/argonviews.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-04 11:43:57.414325 opencmiss.argon-0.3.5/src/opencmiss/argon/settings/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-06-16 00:43:37.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/settings/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      947 2021-09-30 23:24:46.000000 opencmiss.argon-0.3.5/src/opencmiss/argon/settings/mainsettings.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-04 11:43:57.406218 opencmiss.argon-0.3.5/src/opencmiss.argon.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1121 2022-09-04 11:43:57.000000 opencmiss.argon-0.3.5/src/opencmiss.argon.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      801 2022-09-04 11:43:57.000000 opencmiss.argon-0.3.5/src/opencmiss.argon.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-09-04 11:43:57.000000 opencmiss.argon-0.3.5/src/opencmiss.argon.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-06-16 01:36:09.000000 opencmiss.argon-0.3.5/src/opencmiss.argon.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       25 2022-09-04 11:43:57.000000 opencmiss.argon-0.3.5/src/opencmiss.argon.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2022-09-04 11:43:57.000000 opencmiss.argon-0.3.5/src/opencmiss.argon.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-14 22:56:35.147004 opencmiss.argon-0.3.6/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2023-04-14 22:47:04.000000 opencmiss.argon-0.3.6/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      660 2023-04-14 22:56:35.146751 opencmiss.argon-0.3.6/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      300 2023-04-14 22:53:15.000000 opencmiss.argon-0.3.6/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-14 22:56:35.146397 opencmiss.argon-0.3.6/opencmiss.argon.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      660 2023-04-14 22:56:35.000000 opencmiss.argon-0.3.6/opencmiss.argon.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      221 2023-04-14 22:56:35.000000 opencmiss.argon-0.3.6/opencmiss.argon.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-14 22:56:35.000000 opencmiss.argon-0.3.6/opencmiss.argon.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       13 2023-04-14 22:56:35.000000 opencmiss.argon-0.3.6/opencmiss.argon.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-14 22:56:35.000000 opencmiss.argon-0.3.6/opencmiss.argon.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-14 22:56:35.147096 opencmiss.argon-0.3.6/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      670 2023-04-14 22:55:39.000000 opencmiss.argon-0.3.6/setup.py
```

### Comparing `opencmiss.argon-0.3.5/LICENSE` & `opencmiss.argon-0.3.6/LICENSE`

 * *Files identical despite different names*

