# Comparing `tmp/anachem-0.12.tar.gz` & `tmp/anachem-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anachem-0.12.tar", last modified: Sat Mar 18 06:58:44 2023, max compression
+gzip compressed data, was "anachem-0.20.tar", last modified: Sat Apr 15 04:55:29 2023, max compression
```

## Comparing `anachem-0.12.tar` & `anachem-0.20.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 06:58:44.239926 anachem-0.12/
--rw-rw-rw-   0        0        0      167 2023-03-18 06:58:44.236363 anachem-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-18 06:58:44.205773 anachem-0.12/anachem/
--rw-rw-rw-   0        0        0     9856 2023-03-18 06:41:24.000000 anachem-0.12/anachem/AnalyseChemistry.py
--rw-rw-rw-   0        0        0       60 2023-03-18 06:55:16.000000 anachem-0.12/anachem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-18 06:58:44.231920 anachem-0.12/anachem.egg-info/
--rw-rw-rw-   0        0        0      167 2023-03-18 06:58:43.000000 anachem-0.12/anachem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-03-18 06:58:43.000000 anachem-0.12/anachem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 06:58:43.000000 anachem-0.12/anachem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-18 06:58:43.000000 anachem-0.12/anachem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-18 06:58:44.239926 anachem-0.12/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-03-18 06:58:27.000000 anachem-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 04:55:29.708908 anachem-0.20/
+-rw-rw-rw-   0        0        0      131 2023-04-15 04:55:29.707905 anachem-0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-15 04:55:29.685900 anachem-0.20/anachem/
+-rw-rw-rw-   0        0        0    18500 2023-04-15 04:55:11.000000 anachem-0.20/anachem/AnaChem.py
+-rw-rw-rw-   0        0        0      853 2023-04-15 01:52:54.000000 anachem-0.20/anachem/__init__.py
+-rw-rw-rw-   0        0        0    24555 2023-04-15 03:00:35.000000 anachem-0.20/anachem/roundac.py
+-rw-rw-rw-   0        0        0    10710 2023-04-15 03:00:35.000000 anachem-0.20/anachem/roundbase.py
+drwxrwxrwx   0        0        0        0 2023-04-15 04:55:29.705909 anachem-0.20/anachem.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-04-15 04:55:29.000000 anachem-0.20/anachem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-15 04:55:29.000000 anachem-0.20/anachem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 04:55:29.000000 anachem-0.20/anachem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-15 04:55:29.000000 anachem-0.20/anachem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 04:55:29.708908 anachem-0.20/setup.cfg
+-rw-rw-rw-   0        0        0      227 2023-04-15 04:48:00.000000 anachem-0.20/setup.py
```

