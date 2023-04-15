# Comparing `tmp/algo900-0.254.tar.gz` & `tmp/algo900-0.255.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\algo900-0.254.tar", last modified: Sat Apr 15 19:38:27 2023, max compression
+gzip compressed data, was "dist\algo900-0.255.tar", last modified: Sat Apr 15 20:12:14 2023, max compression
```

## Comparing `algo900-0.254.tar` & `algo900-0.255.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 19:38:27.198791 algo900-0.254/
--rw-rw-rw-   0        0        0      267 2023-04-15 19:38:27.197791 algo900-0.254/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-15 00:18:17.000000 algo900-0.254/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 19:38:27.196791 algo900-0.254/algo900.egg-info/
--rw-rw-rw-   0        0        0      267 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 19:38:27.198791 algo900-0.254/setup.cfg
--rw-rw-rw-   0        0        0      509 2023-04-15 19:38:07.000000 algo900-0.254/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:38:27.197791 algo900-0.254/src/
--rw-rw-rw-   0        0        0        0 2023-04-15 19:37:07.000000 algo900-0.254/src/__init__.py
--rw-rw-rw-   0        0        0       29 2023-04-15 19:36:59.000000 algo900-0.254/src/hello.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:12:14.221450 algo900-0.255/
+-rw-rw-rw-   0        0        0      267 2023-04-15 20:12:14.221450 algo900-0.255/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-15 00:18:17.000000 algo900-0.255/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 20:12:14.219450 algo900-0.255/algo900.egg-info/
+-rw-rw-rw-   0        0        0      267 2023-04-15 20:12:14.000000 algo900-0.255/algo900.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-04-15 20:12:14.000000 algo900-0.255/algo900.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 20:12:14.000000 algo900-0.255/algo900.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 20:12:14.000000 algo900-0.255/algo900.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 20:12:14.221450 algo900-0.255/setup.cfg
+-rw-rw-rw-   0        0        0      502 2023-04-15 20:11:28.000000 algo900-0.255/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:12:14.220449 algo900-0.255/src/
+-rw-rw-rw-   0        0        0       23 2023-04-15 20:08:17.000000 algo900-0.255/src/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-04-15 19:36:59.000000 algo900-0.255/src/hello.py
```

