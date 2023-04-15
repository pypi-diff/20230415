# Comparing `tmp/algo900-0.253.tar.gz` & `tmp/algo900-0.254.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\algo900-0.253.tar", last modified: Sat Apr 15 19:19:32 2023, max compression
+gzip compressed data, was "dist\algo900-0.254.tar", last modified: Sat Apr 15 19:38:27 2023, max compression
```

## Comparing `algo900-0.253.tar` & `algo900-0.254.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 19:19:32.593369 algo900-0.253/
--rw-rw-rw-   0        0        0      267 2023-04-15 19:19:32.593369 algo900-0.253/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-15 00:18:17.000000 algo900-0.253/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 19:19:32.592365 algo900-0.253/algo900.egg-info/
--rw-rw-rw-   0        0        0      267 2023-04-15 19:19:32.000000 algo900-0.253/algo900.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-04-15 19:19:32.000000 algo900-0.253/algo900.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:19:32.000000 algo900-0.253/algo900.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:19:32.000000 algo900-0.253/algo900.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 19:19:32.593369 algo900-0.253/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-04-15 19:19:25.000000 algo900-0.253/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:38:27.198791 algo900-0.254/
+-rw-rw-rw-   0        0        0      267 2023-04-15 19:38:27.197791 algo900-0.254/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-15 00:18:17.000000 algo900-0.254/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:38:27.196791 algo900-0.254/algo900.egg-info/
+-rw-rw-rw-   0        0        0      267 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-15 19:38:27.000000 algo900-0.254/algo900.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 19:38:27.198791 algo900-0.254/setup.cfg
+-rw-rw-rw-   0        0        0      509 2023-04-15 19:38:07.000000 algo900-0.254/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:38:27.197791 algo900-0.254/src/
+-rw-rw-rw-   0        0        0        0 2023-04-15 19:37:07.000000 algo900-0.254/src/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-04-15 19:36:59.000000 algo900-0.254/src/hello.py
```

