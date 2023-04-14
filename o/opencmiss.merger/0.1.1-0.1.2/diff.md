# Comparing `tmp/opencmiss.merger-0.1.1.tar.gz` & `tmp/opencmiss.merger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.merger-0.1.1.tar", last modified: Tue Jul 26 04:42:48 2022, max compression
+gzip compressed data, was "opencmiss.merger-0.1.2.tar", last modified: Fri Apr 14 22:32:34 2023, max compression
```

## Comparing `opencmiss.merger-0.1.1.tar` & `opencmiss.merger-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:42:48.662540 opencmiss.merger-0.1.1/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2021-10-04 01:38:37.000000 opencmiss.merger-0.1.1/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1589 2022-07-26 04:42:48.662305 opencmiss.merger-0.1.1/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      380 2022-07-26 04:41:58.000000 opencmiss.merger-0.1.1/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2022-07-26 04:42:48.662620 opencmiss.merger-0.1.1/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1422 2022-03-25 08:41:18.000000 opencmiss.merger-0.1.1/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:42:48.658558 opencmiss.merger-0.1.1/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:42:48.659675 opencmiss.merger-0.1.1/src/opencmiss/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      123 2021-09-29 23:38:45.000000 opencmiss.merger-0.1.1/src/opencmiss/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:42:48.661941 opencmiss.merger-0.1.1/src/opencmiss/merger/
--rw-r--r--   0 hsor001  (1210695619) 1403514002       22 2022-07-26 04:42:32.000000 opencmiss.merger-0.1.1/src/opencmiss/merger/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      183 2022-03-27 04:45:47.000000 opencmiss.merger-0.1.1/src/opencmiss/merger/errors.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14069 2022-07-25 05:37:40.000000 opencmiss.merger-0.1.1/src/opencmiss/merger/points.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 04:42:48.661188 opencmiss.merger-0.1.1/src/opencmiss.merger.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1589 2022-07-26 04:42:48.000000 opencmiss.merger-0.1.1/src/opencmiss.merger.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      410 2022-07-26 04:42:48.000000 opencmiss.merger-0.1.1/src/opencmiss.merger.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-07-26 04:42:48.000000 opencmiss.merger-0.1.1/src/opencmiss.merger.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-03-27 04:12:48.000000 opencmiss.merger-0.1.1/src/opencmiss.merger.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       15 2022-07-26 04:42:48.000000 opencmiss.merger-0.1.1/src/opencmiss.merger.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2022-07-26 04:42:48.000000 opencmiss.merger-0.1.1/src/opencmiss.merger.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-14 22:32:34.550269 opencmiss.merger-0.1.2/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2023-04-14 21:41:53.000000 opencmiss.merger-0.1.2/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      641 2023-04-14 22:32:34.550036 opencmiss.merger-0.1.2/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      304 2023-04-14 22:30:12.000000 opencmiss.merger-0.1.2/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-14 22:32:34.549717 opencmiss.merger-0.1.2/opencmiss.merger.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      641 2023-04-14 22:32:34.000000 opencmiss.merger-0.1.2/opencmiss.merger.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      226 2023-04-14 22:32:34.000000 opencmiss.merger-0.1.2/opencmiss.merger.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-14 22:32:34.000000 opencmiss.merger-0.1.2/opencmiss.merger.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       14 2023-04-14 22:32:34.000000 opencmiss.merger-0.1.2/opencmiss.merger.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-14 22:32:34.000000 opencmiss.merger-0.1.2/opencmiss.merger.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-14 22:32:34.550347 opencmiss.merger-0.1.2/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      656 2023-04-14 22:31:37.000000 opencmiss.merger-0.1.2/setup.py
```

### Comparing `opencmiss.merger-0.1.1/LICENSE` & `opencmiss.merger-0.1.2/LICENSE`

 * *Files identical despite different names*

