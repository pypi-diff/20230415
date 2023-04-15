# Comparing `tmp/search-algos-0.0.1.tar.gz` & `tmp/search-algos-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search-algos-0.0.1.tar", last modified: Sat Apr 15 19:31:50 2023, max compression
+gzip compressed data, was "search-algos-0.1.tar", last modified: Sat Apr 15 19:10:30 2023, max compression
```

## Comparing `search-algos-0.0.1.tar` & `search-algos-0.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:31:50.643161 search-algos-0.0.1/
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      624 2023-04-15 19:31:50.638233 search-algos-0.0.1/PKG-INFO
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      356 2023-04-15 19:30:47.000000 search-algos-0.0.1/README.md
-drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:31:50.620973 search-algos-0.0.1/algos/
--rw-r--r--   0 arpanadhikari   (501) staff       (20)       69 2023-04-15 19:09:48.000000 search-algos-0.0.1/algos/__init__.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      121 2023-04-15 19:09:12.000000 search-algos-0.0.1/algos/linear_search.py
-drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:31:50.637544 search-algos-0.0.1/search_algos.egg-info/
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      624 2023-04-15 19:31:49.000000 search-algos-0.0.1/search_algos.egg-info/PKG-INFO
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      203 2023-04-15 19:31:50.000000 search-algos-0.0.1/search_algos.egg-info/SOURCES.txt
--rw-r--r--   0 arpanadhikari   (501) staff       (20)        1 2023-04-15 19:31:49.000000 search-algos-0.0.1/search_algos.egg-info/dependency_links.txt
--rw-r--r--   0 arpanadhikari   (501) staff       (20)        6 2023-04-15 19:31:50.000000 search-algos-0.0.1/search_algos.egg-info/top_level.txt
--rw-r--r--   0 arpanadhikari   (501) staff       (20)       38 2023-04-15 19:31:50.643814 search-algos-0.0.1/setup.cfg
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      442 2023-04-15 19:31:43.000000 search-algos-0.0.1/setup.py
+drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:10:30.796857 search-algos-0.1/
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      233 2023-04-15 19:10:30.793833 search-algos-0.1/PKG-INFO
+drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:10:30.764984 search-algos-0.1/algos/
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)       69 2023-04-15 19:09:48.000000 search-algos-0.1/algos/__init__.py
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      121 2023-04-15 19:09:12.000000 search-algos-0.1/algos/linear_search.py
+drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:10:30.785784 search-algos-0.1/search_algos.egg-info/
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      233 2023-04-15 19:10:29.000000 search-algos-0.1/search_algos.egg-info/PKG-INFO
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      193 2023-04-15 19:10:30.000000 search-algos-0.1/search_algos.egg-info/SOURCES.txt
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)        1 2023-04-15 19:10:30.000000 search-algos-0.1/search_algos.egg-info/dependency_links.txt
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)        6 2023-04-15 19:10:30.000000 search-algos-0.1/search_algos.egg-info/top_level.txt
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)       38 2023-04-15 19:10:30.801192 search-algos-0.1/setup.cfg
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      283 2023-04-15 19:06:27.000000 search-algos-0.1/setup.py
```

