# Comparing `tmp/planetai-1.1.tar.gz` & `tmp/planetai-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetai-1.1.tar", last modified: Sat Apr 15 11:24:22 2023, max compression
+gzip compressed data, was "planetai-1.2.tar", last modified: Sat Apr 15 11:32:25 2023, max compression
```

## Comparing `planetai-1.1.tar` & `planetai-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:24:21.983017 planetai-1.1/
--rw-rw-rw-   0        0        0      137 2023-04-15 11:24:21.983017 planetai-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.1/README.md
--rw-rw-rw-   0        0        0     1066 2023-04-15 10:41:38.000000 planetai-1.1/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 11:24:21.907203 planetai-1.1/planetai/
--rw-rw-rw-   0        0        0       29 2023-04-15 11:19:25.000000 planetai-1.1/planetai/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-15 11:10:33.000000 planetai-1.1/planetai/main.py
--rw-rw-rw-   0        0        0     3063 2023-04-15 11:03:10.000000 planetai-1.1/planetai/planet.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:24:21.981016 planetai-1.1/planetai.egg-info/
--rw-rw-rw-   0        0        0      137 2023-04-15 11:24:21.000000 planetai-1.1/planetai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-15 11:24:21.000000 planetai-1.1/planetai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:24:21.000000 planetai-1.1/planetai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 11:12:20.000000 planetai-1.1/planetai.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-15 11:24:21.000000 planetai-1.1/planetai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-15 11:24:21.984523 planetai-1.1/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-04-15 11:19:50.000000 planetai-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:32:25.450470 planetai-1.2/
+-rw-rw-rw-   0        0        0      137 2023-04-15 11:32:25.450470 planetai-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.2/README.md
+-rw-rw-rw-   0        0        0     1066 2023-04-15 10:41:38.000000 planetai-1.2/license.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 11:32:25.438737 planetai-1.2/planetai/
+-rw-rw-rw-   0        0        0       27 2023-04-15 11:31:24.000000 planetai-1.2/planetai/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-15 11:10:33.000000 planetai-1.2/planetai/main.py
+-rw-rw-rw-   0        0        0     3063 2023-04-15 11:03:10.000000 planetai-1.2/planetai/planet.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:32:25.448463 planetai-1.2/planetai.egg-info/
+-rw-rw-rw-   0        0        0      137 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-15 11:32:25.452756 planetai-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-04-15 11:31:35.000000 planetai-1.2/setup.py
```

### Comparing `planetai-1.1/license.txt` & `planetai-1.2/license.txt`

 * *Files identical despite different names*

### Comparing `planetai-1.1/planetai/planet.py` & `planetai-1.2/planetai/planet.py`

 * *Files identical despite different names*

