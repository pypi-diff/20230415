# Comparing `tmp/meroua-1.0.tar.gz` & `tmp/meroua-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meroua-1.0.tar", last modified: Sat Apr 15 04:29:46 2023, max compression
+gzip compressed data, was "meroua-1.1.tar", last modified: Sat Apr 15 17:35:50 2023, max compression
```

## Comparing `meroua-1.0.tar` & `meroua-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 04:29:46.042717 meroua-1.0/
--rw-rw-rw-   0        0        0       43 2023-04-15 04:03:09.000000 meroua-1.0/LICENCE.TXT
--rw-rw-rw-   0        0        0      213 2023-04-15 04:29:46.037720 meroua-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 04:29:46.023728 meroua-1.0/meroua.egg-info/
--rw-rw-rw-   0        0        0      213 2023-04-15 04:29:45.000000 meroua-1.0/meroua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-04-15 04:29:45.000000 meroua-1.0/meroua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 04:29:45.000000 meroua-1.0/meroua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-15 04:29:45.000000 meroua-1.0/meroua.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 04:29:46.031724 meroua-1.0/my_codes/
--rw-rw-rw-   0        0        0      212 2023-04-14 05:11:00.000000 meroua-1.0/my_codes/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-15 04:29:46.043717 meroua-1.0/setup.cfg
--rw-rw-rw-   0        0        0      314 2023-04-15 04:29:28.000000 meroua-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:35:50.183993 meroua-1.1/
+-rw-rw-rw-   0        0        0       43 2023-04-15 04:03:09.000000 meroua-1.1/LICENCE.TXT
+-rw-rw-rw-   0        0        0      213 2023-04-15 17:35:50.181994 meroua-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-15 17:35:50.159009 meroua-1.1/meroua.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:35:50.173999 meroua-1.1/my_codes/
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:31:34.000000 meroua-1.1/my_codes/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-04-15 17:26:50.000000 meroua-1.1/my_codes/mymod.py
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:35:50.184993 meroua-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      314 2023-04-15 17:34:57.000000 meroua-1.1/setup.py
```

