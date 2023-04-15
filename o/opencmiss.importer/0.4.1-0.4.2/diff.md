# Comparing `tmp/opencmiss.importer-0.4.1.tar.gz` & `tmp/opencmiss.importer-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.importer-0.4.1.tar", last modified: Wed Aug 31 03:15:47 2022, max compression
+gzip compressed data, was "opencmiss.importer-0.4.2.tar", last modified: Sat Apr 15 02:10:11 2023, max compression
```

## Comparing `opencmiss.importer-0.4.1.tar` & `opencmiss.importer-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-08-31 03:15:47.881752 opencmiss.importer-0.4.1/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2022-03-17 03:07:54.000000 opencmiss.importer-0.4.1/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2102 2022-08-31 03:15:47.881305 opencmiss.importer-0.4.1/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      723 2022-04-17 03:26:52.000000 opencmiss.importer-0.4.1/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2022-08-31 03:15:47.881880 opencmiss.importer-0.4.1/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1979 2022-04-17 03:25:04.000000 opencmiss.importer-0.4.1/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-08-31 03:15:47.864045 opencmiss.importer-0.4.1/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-08-31 03:15:47.865037 opencmiss.importer-0.4.1/src/opencmiss/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      124 2022-03-17 03:12:39.000000 opencmiss.importer-0.4.1/src/opencmiss/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-08-31 03:15:47.880210 opencmiss.importer-0.4.1/src/opencmiss/importer/
--rw-r--r--   0 hsor001  (1210695619) 1403514002       22 2022-08-31 03:15:11.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      534 2022-03-21 02:10:49.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/base.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5469 2022-08-30 01:36:23.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/celldensity.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5647 2022-03-24 03:43:15.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/colonhrm.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4622 2022-03-27 01:25:47.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/colonmanometry.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1317 2022-08-30 00:07:41.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/dxf.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      615 2022-08-30 00:20:15.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/errors.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4828 2022-08-31 03:14:42.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/main.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2423 2022-04-15 08:05:05.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/mbfxml.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1321 2022-08-30 00:07:41.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/obj.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1314 2022-08-30 00:07:41.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/ply.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4330 2022-03-24 03:44:49.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/ragpdata.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1328 2022-08-30 00:07:41.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/stl.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1305 2022-08-30 00:07:41.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/svg.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5933 2022-08-30 00:03:01.000000 opencmiss.importer-0.4.1/src/opencmiss/importer/trimesh.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-08-31 03:15:47.868083 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2102 2022-08-31 03:15:47.000000 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      872 2022-08-31 03:15:47.000000 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-08-31 03:15:47.000000 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       63 2022-08-31 03:15:47.000000 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/entry_points.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-03-17 03:46:11.000000 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002      137 2022-08-31 03:15:47.000000 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2022-08-31 03:15:47.000000 opencmiss.importer-0.4.1/src/opencmiss.importer.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 02:10:11.095919 opencmiss.importer-0.4.2/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      594 2023-04-15 02:05:53.000000 opencmiss.importer-0.4.2/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      654 2023-04-15 02:10:11.095691 opencmiss.importer-0.4.2/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      315 2023-04-15 02:07:13.000000 opencmiss.importer-0.4.2/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 02:10:11.095355 opencmiss.importer-0.4.2/opencmiss.importer.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      654 2023-04-15 02:10:10.000000 opencmiss.importer-0.4.2/opencmiss.importer.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      236 2023-04-15 02:10:10.000000 opencmiss.importer-0.4.2/opencmiss.importer.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-15 02:10:10.000000 opencmiss.importer-0.4.2/opencmiss.importer.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       16 2023-04-15 02:10:10.000000 opencmiss.importer-0.4.2/opencmiss.importer.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-15 02:10:10.000000 opencmiss.importer-0.4.2/opencmiss.importer.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-15 02:10:11.095999 opencmiss.importer-0.4.2/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      659 2023-04-15 02:08:03.000000 opencmiss.importer-0.4.2/setup.py
```

### Comparing `opencmiss.importer-0.4.1/LICENSE` & `opencmiss.importer-0.4.2/LICENSE`

 * *Files identical despite different names*

