# Comparing `tmp/algo900-0.256.tar.gz` & `tmp/algo900-0.257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\algo900-0.256.tar", last modified: Sat Apr 15 20:18:39 2023, max compression
+gzip compressed data, was "dist\algo900-0.257.tar", last modified: Sat Apr 15 20:23:29 2023, max compression
```

## Comparing `algo900-0.256.tar` & `algo900-0.257.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 20:18:39.749360 algo900-0.256/
--rw-rw-rw-   0        0        0      267 2023-04-15 20:18:39.749360 algo900-0.256/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-15 00:18:17.000000 algo900-0.256/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 20:18:39.747361 algo900-0.256/algo900.egg-info/
--rw-rw-rw-   0        0        0      267 2023-04-15 20:18:39.000000 algo900-0.256/algo900.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-04-15 20:18:39.000000 algo900-0.256/algo900.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 20:18:39.000000 algo900-0.256/algo900.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-15 20:18:39.000000 algo900-0.256/algo900.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 20:18:39.749360 algo900-0.256/setup.cfg
--rw-rw-rw-   0        0        0      483 2023-04-15 20:18:12.000000 algo900-0.256/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:18:39.748360 algo900-0.256/src/
--rw-rw-rw-   0        0        0       23 2023-04-15 20:08:17.000000 algo900-0.256/src/__init__.py
--rw-rw-rw-   0        0        0       29 2023-04-15 19:36:59.000000 algo900-0.256/src/hello.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:23:29.771161 algo900-0.257/
+-rw-rw-rw-   0        0        0      267 2023-04-15 20:23:29.771161 algo900-0.257/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-15 00:18:17.000000 algo900-0.257/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 20:23:29.757161 algo900-0.257/algo/
+-rw-rw-rw-   0        0        0       29 2023-04-15 20:22:50.000000 algo900-0.257/algo/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-04-15 19:36:59.000000 algo900-0.257/algo/hello.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:23:29.770160 algo900-0.257/algo900.egg-info/
+-rw-rw-rw-   0        0        0      267 2023-04-15 20:23:29.000000 algo900-0.257/algo900.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-15 20:23:29.000000 algo900-0.257/algo900.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 20:23:29.000000 algo900-0.257/algo900.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 20:23:29.000000 algo900-0.257/algo900.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 20:23:29.771161 algo900-0.257/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-04-15 20:23:21.000000 algo900-0.257/setup.py
```

