# Comparing `tmp/algoxyz-0.0.2.tar.gz` & `tmp/algoxyz-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\algoxyz-0.0.2.tar", last modified: Sat Apr 15 20:39:46 2023, max compression
+gzip compressed data, was "dist\algoxyz-0.31.tar", last modified: Sat Apr 15 20:33:23 2023, max compression
```

## Comparing `algoxyz-0.0.2.tar` & `algoxyz-0.31.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 20:39:46.695602 algoxyz-0.0.2/
--rw-rw-rw-   0        0        0       81 2023-04-15 20:39:26.000000 algoxyz-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1056 2020-04-19 15:03:38.000000 algoxyz-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 algoxyz-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      578 2023-04-15 20:39:46.695602 algoxyz-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-15 20:38:38.000000 algoxyz-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 20:39:46.683601 algoxyz-0.0.2/algo/
--rw-rw-rw-   0        0        0      233 2020-04-19 14:55:15.000000 algoxyz-0.0.2/algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:39:46.694603 algoxyz-0.0.2/algoxyz.egg-info/
--rw-rw-rw-   0        0        0      578 2023-04-15 20:39:46.000000 algoxyz-0.0.2/algoxyz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-15 20:39:46.000000 algoxyz-0.0.2/algoxyz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 20:39:46.000000 algoxyz-0.0.2/algoxyz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 20:39:46.000000 algoxyz-0.0.2/algoxyz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 20:39:46.695602 algoxyz-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-04-15 20:38:58.000000 algoxyz-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:33:23.163152 algoxyz-0.31/
+-rw-rw-rw-   0        0        0     1059 2023-04-15 20:28:36.000000 algoxyz-0.31/LICENSE.TXT
+-rw-rw-rw-   0        0        0       25 2023-04-15 20:27:05.000000 algoxyz-0.31/MANIFEST.in
+-rw-rw-rw-   0        0        0      139 2023-04-15 20:33:23.163152 algoxyz-0.31/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-15 20:25:43.000000 algoxyz-0.31/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 20:33:23.153153 algoxyz-0.31/algo/
+-rw-rw-rw-   0        0        0       27 2023-04-15 20:25:07.000000 algoxyz-0.31/algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:33:23.155151 algoxyz-0.31/algo900.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-04-15 20:30:39.000000 algoxyz-0.31/algo900.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 20:30:39.000000 algoxyz-0.31/algo900.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 20:30:39.000000 algoxyz-0.31/algo900.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 20:33:23.162151 algoxyz-0.31/algoxyz.egg-info/
+-rw-rw-rw-   0        0        0      139 2023-04-15 20:33:23.000000 algoxyz-0.31/algoxyz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-04-15 20:33:23.000000 algoxyz-0.31/algoxyz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 20:33:23.000000 algoxyz-0.31/algoxyz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 20:33:23.000000 algoxyz-0.31/algoxyz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 20:33:23.163152 algoxyz-0.31/setup.cfg
+-rw-rw-rw-   0        0        0      194 2023-04-15 20:33:15.000000 algoxyz-0.31/setup.py
```

