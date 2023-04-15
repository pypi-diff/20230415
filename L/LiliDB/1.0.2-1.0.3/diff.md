# Comparing `tmp/LiliDB-1.0.2.tar.gz` & `tmp/LiliDB-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiliDB-1.0.2.tar", last modified: Tue Feb 28 23:21:56 2023, max compression
+gzip compressed data, was "LiliDB-1.0.3.tar", last modified: Sat Apr 15 21:23:27 2023, max compression
```

## Comparing `LiliDB-1.0.2.tar` & `LiliDB-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 23:21:56.665479 LiliDB-1.0.2/
--rw-rw-rw-   0        0        0     1088 2023-01-14 07:40:06.000000 LiliDB-1.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-02-28 23:21:56.660493 LiliDB-1.0.2/LiliDB.egg-info/
--rw-rw-rw-   0        0        0      828 2023-02-28 23:21:56.000000 LiliDB-1.0.2/LiliDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-02-28 23:21:56.000000 LiliDB-1.0.2/LiliDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 23:21:56.000000 LiliDB-1.0.2/LiliDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-28 23:21:56.000000 LiliDB-1.0.2/LiliDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      828 2023-02-28 23:21:56.664481 LiliDB-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-02-28 23:13:22.000000 LiliDB-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 23:21:56.663484 LiliDB-1.0.2/lilidb/
--rw-rw-rw-   0        0        0       26 2022-12-25 08:21:00.000000 LiliDB-1.0.2/lilidb/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-02-26 03:37:28.000000 LiliDB-1.0.2/lilidb/db.py
--rw-rw-rw-   0        0        0       42 2023-02-28 23:21:56.665479 LiliDB-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      465 2023-02-28 23:13:12.000000 LiliDB-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 21:23:27.675463 LiliDB-1.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-01-14 07:40:06.000000 LiliDB-1.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-15 21:23:27.668189 LiliDB-1.0.3/LiliDB.egg-info/
+-rw-rw-rw-   0        0        0      828 2023-04-15 21:23:26.000000 LiliDB-1.0.3/LiliDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-15 21:23:26.000000 LiliDB-1.0.3/LiliDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 21:23:26.000000 LiliDB-1.0.3/LiliDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 21:23:26.000000 LiliDB-1.0.3/LiliDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      828 2023-04-15 21:23:27.675463 LiliDB-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-02-28 23:13:22.000000 LiliDB-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 21:23:27.672182 LiliDB-1.0.3/lilidb/
+-rw-rw-rw-   0        0        0      289 2023-03-22 16:19:06.000000 LiliDB-1.0.3/lilidb/__init__.py
+-rw-rw-rw-   0        0        0     3756 2023-04-15 21:21:49.000000 LiliDB-1.0.3/lilidb/db.py
+-rw-rw-rw-   0        0        0       42 2023-04-15 21:23:27.676463 LiliDB-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      465 2023-04-15 21:23:09.000000 LiliDB-1.0.3/setup.py
```

### Comparing `LiliDB-1.0.2/LICENSE` & `LiliDB-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LiliDB-1.0.2/LiliDB.egg-info/PKG-INFO` & `LiliDB-1.0.3/LiliDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiliDB
-Version: 1.0.2
+Version: 1.0.3
 Summary: Key-Value database library, small and easy to use.
 Home-page: https://github.com/ZSendokame/LiliDB
 Author: ZSendokame
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `LiliDB-1.0.2/PKG-INFO` & `LiliDB-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiliDB
-Version: 1.0.2
+Version: 1.0.3
 Summary: Key-Value database library, small and easy to use.
 Home-page: https://github.com/ZSendokame/LiliDB
 Author: ZSendokame
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `LiliDB-1.0.2/README.md` & `LiliDB-1.0.3/README.md`

 * *Files identical despite different names*

