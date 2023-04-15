# Comparing `tmp/paralleltd-0.0.0.tar.gz` & `tmp/paralleltd-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paralleltd-0.0.0.tar", last modified: Sat Apr 15 08:13:29 2023, max compression
+gzip compressed data, was "paralleltd-0.0.1.tar", last modified: Sat Apr 15 08:30:35 2023, max compression
```

## Comparing `paralleltd-0.0.0.tar` & `paralleltd-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 leslie_pun   (501) staff       (20)        0 2023-04-15 08:13:29.188318 paralleltd-0.0.0/
--rw-r--r--   0 leslie_pun   (501) staff       (20)      136 2023-04-15 08:13:29.188388 paralleltd-0.0.0/PKG-INFO
-drwxr-xr-x   0 leslie_pun   (501) staff       (20)        0 2023-04-15 08:13:29.187534 paralleltd-0.0.0/paralleltd/
--rw-r--r--   0 leslie_pun   (501) staff       (20)      819 2023-04-15 08:09:57.000000 paralleltd-0.0.0/paralleltd/Mps.py
--rw-r--r--   0 leslie_pun   (501) staff       (20)      166 2023-04-15 08:09:57.000000 paralleltd-0.0.0/paralleltd/__init__.py
-drwxr-xr-x   0 leslie_pun   (501) staff       (20)        0 2023-04-15 08:13:29.188191 paralleltd-0.0.0/paralleltd.egg-info/
--rw-r--r--   0 leslie_pun   (501) staff       (20)      136 2023-04-15 08:13:29.000000 paralleltd-0.0.0/paralleltd.egg-info/PKG-INFO
--rw-r--r--   0 leslie_pun   (501) staff       (20)      228 2023-04-15 08:13:29.000000 paralleltd-0.0.0/paralleltd.egg-info/SOURCES.txt
--rw-r--r--   0 leslie_pun   (501) staff       (20)        1 2023-04-15 08:13:29.000000 paralleltd-0.0.0/paralleltd.egg-info/dependency_links.txt
--rw-r--r--   0 leslie_pun   (501) staff       (20)        1 2023-04-15 08:13:29.000000 paralleltd-0.0.0/paralleltd.egg-info/not-zip-safe
--rw-r--r--   0 leslie_pun   (501) staff       (20)       11 2023-04-15 08:13:29.000000 paralleltd-0.0.0/paralleltd.egg-info/top_level.txt
--rw-r--r--   0 leslie_pun   (501) staff       (20)      225 2023-04-15 08:13:29.188761 paralleltd-0.0.0/setup.cfg
--rw-r--r--   0 leslie_pun   (501) staff       (20)      415 2023-04-15 04:00:34.000000 paralleltd-0.0.0/setup.py
+drwxr-xr-x   0 leslie_pun   (501) staff       (20)        0 2023-04-15 08:30:35.053449 paralleltd-0.0.1/
+-rw-r--r--   0 leslie_pun   (501) staff       (20)      136 2023-04-15 08:30:35.053518 paralleltd-0.0.1/PKG-INFO
+drwxr-xr-x   0 leslie_pun   (501) staff       (20)        0 2023-04-15 08:30:35.052680 paralleltd-0.0.1/paralleltd/
+-rw-r--r--   0 leslie_pun   (501) staff       (20)      823 2023-04-15 08:30:12.000000 paralleltd-0.0.1/paralleltd/Mps.py
+-rw-r--r--   0 leslie_pun   (501) staff       (20)      166 2023-04-15 08:09:57.000000 paralleltd-0.0.1/paralleltd/__init__.py
+drwxr-xr-x   0 leslie_pun   (501) staff       (20)        0 2023-04-15 08:30:35.053321 paralleltd-0.0.1/paralleltd.egg-info/
+-rw-r--r--   0 leslie_pun   (501) staff       (20)      136 2023-04-15 08:30:35.000000 paralleltd-0.0.1/paralleltd.egg-info/PKG-INFO
+-rw-r--r--   0 leslie_pun   (501) staff       (20)      228 2023-04-15 08:30:35.000000 paralleltd-0.0.1/paralleltd.egg-info/SOURCES.txt
+-rw-r--r--   0 leslie_pun   (501) staff       (20)        1 2023-04-15 08:30:35.000000 paralleltd-0.0.1/paralleltd.egg-info/dependency_links.txt
+-rw-r--r--   0 leslie_pun   (501) staff       (20)        1 2023-04-15 08:13:29.000000 paralleltd-0.0.1/paralleltd.egg-info/not-zip-safe
+-rw-r--r--   0 leslie_pun   (501) staff       (20)       11 2023-04-15 08:30:35.000000 paralleltd-0.0.1/paralleltd.egg-info/top_level.txt
+-rw-r--r--   0 leslie_pun   (501) staff       (20)      225 2023-04-15 08:30:35.053868 paralleltd-0.0.1/setup.cfg
+-rw-r--r--   0 leslie_pun   (501) staff       (20)      415 2023-04-15 04:00:34.000000 paralleltd-0.0.1/setup.py
```

