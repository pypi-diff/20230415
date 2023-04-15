# Comparing `tmp/meroua-1.1.tar.gz` & `tmp/meroua-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meroua-1.1.tar", last modified: Sat Apr 15 17:35:50 2023, max compression
+gzip compressed data, was "meroua-1.2.tar", last modified: Sat Apr 15 18:12:31 2023, max compression
```

## Comparing `meroua-1.1.tar` & `meroua-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 17:35:50.183993 meroua-1.1/
--rw-rw-rw-   0        0        0       43 2023-04-15 04:03:09.000000 meroua-1.1/LICENCE.TXT
--rw-rw-rw-   0        0        0      213 2023-04-15 17:35:50.181994 meroua-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 17:35:50.159009 meroua-1.1/meroua.egg-info/
--rw-rw-rw-   0        0        0      213 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-15 17:35:49.000000 meroua-1.1/meroua.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:35:50.173999 meroua-1.1/my_codes/
--rw-rw-rw-   0        0        0       42 2023-04-15 17:31:34.000000 meroua-1.1/my_codes/__init__.py
--rw-rw-rw-   0        0        0      210 2023-04-15 17:26:50.000000 meroua-1.1/my_codes/mymod.py
--rw-rw-rw-   0        0        0       42 2023-04-15 17:35:50.184993 meroua-1.1/setup.cfg
--rw-rw-rw-   0        0        0      314 2023-04-15 17:34:57.000000 meroua-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:12:31.667334 meroua-1.2/
+-rw-rw-rw-   0        0        0       43 2023-04-15 04:03:09.000000 meroua-1.2/LICENCE.TXT
+-rw-rw-rw-   0        0        0      213 2023-04-15 18:12:31.663335 meroua-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-15 18:12:31.617363 meroua-1.2/meroua/
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:31:34.000000 meroua-1.2/meroua/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-04-15 17:26:50.000000 meroua-1.2/meroua/mymod.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:12:31.650343 meroua-1.2/meroua.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-04-15 18:12:31.000000 meroua-1.2/meroua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-15 18:12:31.000000 meroua-1.2/meroua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:12:31.000000 meroua-1.2/meroua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 18:12:31.000000 meroua-1.2/meroua.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:12:31.667334 meroua-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-04-15 18:12:24.000000 meroua-1.2/setup.py
```

