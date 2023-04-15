# Comparing `tmp/opencmiss.exporter-0.3.5.tar.gz` & `tmp/opencmiss.exporter-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.exporter-0.3.5.tar", last modified: Thu Feb  9 02:33:27 2023, max compression
+gzip compressed data, was "opencmiss.exporter-0.3.6.tar", last modified: Sat Apr 15 01:38:48 2023, max compression
```

## Comparing `opencmiss.exporter-0.3.5.tar` & `opencmiss.exporter-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 02:33:27.681462 opencmiss.exporter-0.3.5/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2021-10-04 01:38:37.000000 opencmiss.exporter-0.3.5/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2476 2023-02-09 02:33:27.681207 opencmiss.exporter-0.3.5/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1081 2022-04-06 07:14:33.000000 opencmiss.exporter-0.3.5/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-02-09 02:33:27.681555 opencmiss.exporter-0.3.5/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1571 2023-01-31 01:21:27.000000 opencmiss.exporter-0.3.5/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 02:33:27.672805 opencmiss.exporter-0.3.5/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 02:33:27.673880 opencmiss.exporter-0.3.5/src/opencmiss/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      123 2021-09-29 23:38:45.000000 opencmiss.exporter-0.3.5/src/opencmiss/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 02:33:27.680476 opencmiss.exporter-0.3.5/src/opencmiss/exporter/
--rw-r--r--   0 hsor001  (1210695619) 1403514002       22 2023-02-09 02:32:10.000000 opencmiss.exporter-0.3.5/src/opencmiss/exporter/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2886 2022-05-26 03:56:28.000000 opencmiss.exporter-0.3.5/src/opencmiss/exporter/base.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6695 2023-01-31 01:21:27.000000 opencmiss.exporter-0.3.5/src/opencmiss/exporter/baseimage.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      181 2022-11-08 03:39:19.000000 opencmiss.exporter-0.3.5/src/opencmiss/exporter/errors.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      893 2022-11-09 21:30:45.000000 opencmiss.exporter-0.3.5/src/opencmiss/exporter/image.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      939 2022-11-09 21:30:45.000000 opencmiss.exporter-0.3.5/src/opencmiss/exporter/thumbnail.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6585 2022-08-16 04:30:48.000000 opencmiss.exporter-0.3.5/src/opencmiss/exporter/webgl.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 02:33:27.676293 opencmiss.exporter-0.3.5/src/opencmiss.exporter.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2476 2023-02-09 02:33:27.000000 opencmiss.exporter-0.3.5/src/opencmiss.exporter.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      562 2023-02-09 02:33:27.000000 opencmiss.exporter-0.3.5/src/opencmiss.exporter.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-02-09 02:33:27.000000 opencmiss.exporter-0.3.5/src/opencmiss.exporter.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-09-30 01:58:13.000000 opencmiss.exporter-0.3.5/src/opencmiss.exporter.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       99 2023-02-09 02:33:27.000000 opencmiss.exporter-0.3.5/src/opencmiss.exporter.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2023-02-09 02:33:27.000000 opencmiss.exporter-0.3.5/src/opencmiss.exporter.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 01:38:48.010183 opencmiss.exporter-0.3.6/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2023-04-14 23:52:14.000000 opencmiss.exporter-0.3.6/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      653 2023-04-15 01:38:48.009931 opencmiss.exporter-0.3.6/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      314 2023-04-15 01:37:27.000000 opencmiss.exporter-0.3.6/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 01:38:48.009584 opencmiss.exporter-0.3.6/opencmiss.exporter.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      653 2023-04-15 01:38:47.000000 opencmiss.exporter-0.3.6/opencmiss.exporter.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      236 2023-04-15 01:38:47.000000 opencmiss.exporter-0.3.6/opencmiss.exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-15 01:38:47.000000 opencmiss.exporter-0.3.6/opencmiss.exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       16 2023-04-15 01:38:47.000000 opencmiss.exporter-0.3.6/opencmiss.exporter.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-15 01:38:47.000000 opencmiss.exporter-0.3.6/opencmiss.exporter.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-15 01:38:48.010269 opencmiss.exporter-0.3.6/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      659 2023-04-15 01:36:56.000000 opencmiss.exporter-0.3.6/setup.py
```

### Comparing `opencmiss.exporter-0.3.5/LICENSE` & `opencmiss.exporter-0.3.6/LICENSE`

 * *Files identical despite different names*

