# Comparing `tmp/shreycriclivemac-0.3.tar.gz` & `tmp/shreycriclivemac-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shreycriclivemac-0.3.tar", last modified: Fri Apr 14 21:50:55 2023, max compression
+gzip compressed data, was "shreycriclivemac-0.4.tar", last modified: Fri Apr 14 22:01:03 2023, max compression
```

## Comparing `shreycriclivemac-0.3.tar` & `shreycriclivemac-0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 21:50:55.884143 shreycriclivemac-0.3/
--rw-r--r--   0 shreyansh   (501) staff       (20)       18 2023-04-14 21:32:35.000000 shreycriclivemac-0.3/MANIFEST.in
--rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 21:50:55.883657 shreycriclivemac-0.3/PKG-INFO
--rw-r--r--   0 shreyansh   (501) staff       (20)      103 2023-04-14 21:32:06.000000 shreycriclivemac-0.3/README.md
--rw-r--r--   0 shreyansh   (501) staff       (20)       38 2023-04-14 21:50:55.884336 shreycriclivemac-0.3/setup.cfg
--rw-r--r--   0 shreyansh   (501) staff       (20)      319 2023-04-14 21:50:44.000000 shreycriclivemac-0.3/setup.py
-drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 21:50:55.882932 shreycriclivemac-0.3/shreycriclivemac.egg-info/
--rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/PKG-INFO
--rw-r--r--   0 shreyansh   (501) staff       (20)      272 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/SOURCES.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)        1 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/dependency_links.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)       63 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/entry_points.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)       29 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/requires.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)       13 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/top_level.txt
+drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 22:01:03.289219 shreycriclivemac-0.4/
+-rw-r--r--   0 shreyansh   (501) staff       (20)       18 2023-04-14 21:32:35.000000 shreycriclivemac-0.4/MANIFEST.in
+-rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 22:01:03.288102 shreycriclivemac-0.4/PKG-INFO
+-rw-r--r--   0 shreyansh   (501) staff       (20)      103 2023-04-14 21:32:06.000000 shreycriclivemac-0.4/README.md
+-rw-r--r--   0 shreyansh   (501) staff       (20)       38 2023-04-14 22:01:03.289484 shreycriclivemac-0.4/setup.cfg
+-rw-r--r--   0 shreyansh   (501) staff       (20)      340 2023-04-14 21:59:48.000000 shreycriclivemac-0.4/setup.py
+drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 22:01:03.286682 shreycriclivemac-0.4/shreycriclivemac.egg-info/
+-rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 22:01:02.000000 shreycriclivemac-0.4/shreycriclivemac.egg-info/PKG-INFO
+-rw-r--r--   0 shreyansh   (501) staff       (20)      292 2023-04-14 22:01:03.000000 shreycriclivemac-0.4/shreycriclivemac.egg-info/SOURCES.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)        1 2023-04-14 22:01:02.000000 shreycriclivemac-0.4/shreycriclivemac.egg-info/dependency_links.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)       63 2023-04-14 22:01:02.000000 shreycriclivemac-0.4/shreycriclivemac.egg-info/entry_points.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)       29 2023-04-14 22:01:02.000000 shreycriclivemac-0.4/shreycriclivemac.egg-info/requires.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)       17 2023-04-14 22:01:02.000000 shreycriclivemac-0.4/shreycriclivemac.egg-info/top_level.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)     4158 2023-04-14 21:40:17.000000 shreycriclivemac-0.4/shreycriclivemac.py
```

