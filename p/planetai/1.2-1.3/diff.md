# Comparing `tmp/planetai-1.2.tar.gz` & `tmp/planetai-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetai-1.2.tar", last modified: Sat Apr 15 11:32:25 2023, max compression
+gzip compressed data, was "planetai-1.3.tar", last modified: Sat Apr 15 11:36:28 2023, max compression
```

## Comparing `planetai-1.2.tar` & `planetai-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:32:25.450470 planetai-1.2/
--rw-rw-rw-   0        0        0      137 2023-04-15 11:32:25.450470 planetai-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.2/README.md
--rw-rw-rw-   0        0        0     1066 2023-04-15 10:41:38.000000 planetai-1.2/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 11:32:25.438737 planetai-1.2/planetai/
--rw-rw-rw-   0        0        0       27 2023-04-15 11:31:24.000000 planetai-1.2/planetai/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-15 11:10:33.000000 planetai-1.2/planetai/main.py
--rw-rw-rw-   0        0        0     3063 2023-04-15 11:03:10.000000 planetai-1.2/planetai/planet.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:32:25.448463 planetai-1.2/planetai.egg-info/
--rw-rw-rw-   0        0        0      137 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-15 11:32:25.000000 planetai-1.2/planetai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-15 11:32:25.452756 planetai-1.2/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-04-15 11:31:35.000000 planetai-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:36:28.542544 planetai-1.3/
+-rw-rw-rw-   0        0        0      137 2023-04-15 11:36:28.542544 planetai-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.3/README.md
+-rw-rw-rw-   0        0        0     1066 2023-04-15 10:41:38.000000 planetai-1.3/license.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 11:36:28.432227 planetai-1.3/planetai/
+-rw-rw-rw-   0        0        0       27 2023-04-15 11:31:24.000000 planetai-1.3/planetai/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-15 11:10:33.000000 planetai-1.3/planetai/main.py
+-rw-rw-rw-   0        0        0     3047 2023-04-15 11:35:38.000000 planetai-1.3/planetai/planet.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:36:28.540545 planetai-1.3/planetai.egg-info/
+-rw-rw-rw-   0        0        0      137 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-15 11:36:28.543544 planetai-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-04-15 11:35:44.000000 planetai-1.3/setup.py
```

### Comparing `planetai-1.2/license.txt` & `planetai-1.3/license.txt`

 * *Files identical despite different names*

### Comparing `planetai-1.2/planetai/planet.py` & `planetai-1.3/planetai/planet.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         url = "https://farsight.org/sponsors/PoolA/t{}.html".format(targetnumber)
         webbrowser.open(url)
 
     def copyright():
         print("""Copyright (c) 2023 Aziz Brown
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files 'Planetary Guides Package', to deal
+of this software and associated documentation files 'planetAI', to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in
 all copies or substantial portions of the Software.
```

