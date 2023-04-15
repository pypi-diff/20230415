# Comparing `tmp/algoxyz-0.33.tar.gz` & `tmp/algoxyz-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\algoxyz-0.33.tar", last modified: Sat Apr 15 20:36:27 2023, max compression
+gzip compressed data, was "dist\algoxyz-0.34.tar", last modified: Sat Apr 15 20:39:34 2023, max compression
```

## Comparing `algoxyz-0.33.tar` & `algoxyz-0.34.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 20:36:27.457592 algoxyz-0.33/
--rw-rw-rw-   0        0        0       25 2023-04-15 20:27:05.000000 algoxyz-0.33/MANIFEST.in
--rw-rw-rw-   0        0        0      196 2023-04-15 20:36:27.457592 algoxyz-0.33/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-15 20:25:43.000000 algoxyz-0.33/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 20:36:27.441966 algoxyz-0.33/algo/
--rw-rw-rw-   0        0        0        0 2023-04-15 20:14:55.000000 algoxyz-0.33/algo/__init__.py
--rw-rw-rw-   0        0        0       27 2023-04-15 20:14:53.000000 algoxyz-0.33/algo/algo1.py
--rw-rw-rw-   0        0        0      109 2023-04-15 20:33:22.000000 algoxyz-0.33/algo/algo3.py
--rw-rw-rw-   0        0        0       61 2023-04-15 20:33:00.000000 algoxyz-0.33/algo/claseotra.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:36:27.457592 algoxyz-0.33/algoxyz.egg-info/
--rw-rw-rw-   0        0        0      196 2023-04-15 20:36:27.000000 algoxyz-0.33/algoxyz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-15 20:36:27.000000 algoxyz-0.33/algoxyz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 20:36:27.000000 algoxyz-0.33/algoxyz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 20:36:27.000000 algoxyz-0.33/algoxyz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 20:36:27.457592 algoxyz-0.33/setup.cfg
--rw-rw-rw-   0        0        0      194 2023-04-15 20:33:37.000000 algoxyz-0.33/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:39:34.479771 algoxyz-0.34/
+-rw-rw-rw-   0        0        0       25 2023-04-15 20:27:05.000000 algoxyz-0.34/MANIFEST.in
+-rw-rw-rw-   0        0        0      196 2023-04-15 20:39:34.479771 algoxyz-0.34/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-15 20:25:43.000000 algoxyz-0.34/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 20:39:34.479771 algoxyz-0.34/algo/
+-rw-rw-rw-   0        0        0        0 2023-04-15 20:14:55.000000 algoxyz-0.34/algo/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-04-15 20:14:53.000000 algoxyz-0.34/algo/algo1.py
+-rw-rw-rw-   0        0        0      114 2023-04-15 20:38:56.000000 algoxyz-0.34/algo/algo3.py
+-rw-rw-rw-   0        0        0       61 2023-04-15 20:33:00.000000 algoxyz-0.34/algo/claseotra.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:39:34.479771 algoxyz-0.34/algoxyz.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-04-15 20:39:34.000000 algoxyz-0.34/algoxyz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-15 20:39:34.000000 algoxyz-0.34/algoxyz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 20:39:34.000000 algoxyz-0.34/algoxyz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 20:39:34.000000 algoxyz-0.34/algoxyz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 20:39:34.479771 algoxyz-0.34/setup.cfg
+-rw-rw-rw-   0        0        0      194 2023-04-15 20:39:30.000000 algoxyz-0.34/setup.py
```

