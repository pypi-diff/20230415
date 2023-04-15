# Comparing `tmp/PhanMemMMN-0.0.5.tar.gz` & `tmp/PhanMemMMN-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhanMemMMN-0.0.5.tar", last modified: Sat Apr 15 07:53:20 2023, max compression
+gzip compressed data, was "PhanMemMMN-0.0.6.tar", last modified: Sat Apr 15 07:55:54 2023, max compression
```

## Comparing `PhanMemMMN-0.0.5.tar` & `PhanMemMMN-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 07:53:20.691244 PhanMemMMN-0.0.5/
--rw-rw-rw-   0        0        0       65 2023-04-15 07:40:27.000000 PhanMemMMN-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    10290 2023-04-13 03:55:17.000000 PhanMemMMN-0.0.5/MusicApp.py
--rw-rw-rw-   0        0        0      152 2023-04-15 07:53:20.691244 PhanMemMMN-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 07:53:20.679277 PhanMemMMN-0.0.5/PhanMemMMN.egg-info/
--rw-rw-rw-   0        0        0      152 2023-04-15 07:53:20.000000 PhanMemMMN-0.0.5/PhanMemMMN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-15 07:53:20.000000 PhanMemMMN-0.0.5/PhanMemMMN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 07:53:20.000000 PhanMemMMN-0.0.5/PhanMemMMN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-15 07:53:20.000000 PhanMemMMN-0.0.5/PhanMemMMN.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 07:53:20.000000 PhanMemMMN-0.0.5/PhanMemMMN.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 07:53:20.689250 PhanMemMMN-0.0.5/img/
--rw-rw-rw-   0        0        0     7219 2023-04-09 09:15:25.000000 PhanMemMMN-0.0.5/img/low-volume.png
--rw-rw-rw-   0        0        0     7641 2023-03-21 07:47:31.000000 PhanMemMMN-0.0.5/img/next-button.png
--rw-rw-rw-   0        0        0    10518 2023-03-21 07:46:44.000000 PhanMemMMN-0.0.5/img/pause.png
--rw-rw-rw-   0        0        0    12544 2023-03-20 12:41:41.000000 PhanMemMMN-0.0.5/img/play-button1.png
--rw-rw-rw-   0        0        0     7111 2023-03-21 07:47:51.000000 PhanMemMMN-0.0.5/img/previous.png
--rw-rw-rw-   0        0        0      443 2023-03-28 10:41:37.000000 PhanMemMMN-0.0.5/img/repeat-one.png
--rw-rw-rw-   0        0        0      415 2023-03-28 10:41:15.000000 PhanMemMMN-0.0.5/img/repeat.png
--rw-rw-rw-   0        0        0      691 2023-03-28 10:46:58.000000 PhanMemMMN-0.0.5/img/shuffle.png
--rw-rw-rw-   0        0        0       42 2023-04-15 07:53:20.691244 PhanMemMMN-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      458 2023-04-15 07:53:07.000000 PhanMemMMN-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:55:54.863423 PhanMemMMN-0.0.6/
+-rw-rw-rw-   0        0        0       65 2023-04-15 07:40:27.000000 PhanMemMMN-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    10290 2023-04-13 03:55:17.000000 PhanMemMMN-0.0.6/MusicApp.py
+-rw-rw-rw-   0        0        0      152 2023-04-15 07:55:54.862428 PhanMemMMN-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-15 07:55:54.853449 PhanMemMMN-0.0.6/PhanMemMMN.egg-info/
+-rw-rw-rw-   0        0        0      152 2023-04-15 07:55:54.000000 PhanMemMMN-0.0.6/PhanMemMMN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-15 07:55:54.000000 PhanMemMMN-0.0.6/PhanMemMMN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 07:55:54.000000 PhanMemMMN-0.0.6/PhanMemMMN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-15 07:55:54.000000 PhanMemMMN-0.0.6/PhanMemMMN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 07:55:54.000000 PhanMemMMN-0.0.6/PhanMemMMN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 07:55:54.860434 PhanMemMMN-0.0.6/img/
+-rw-rw-rw-   0        0        0     7219 2023-04-09 09:15:25.000000 PhanMemMMN-0.0.6/img/low-volume.png
+-rw-rw-rw-   0        0        0     7641 2023-03-21 07:47:31.000000 PhanMemMMN-0.0.6/img/next-button.png
+-rw-rw-rw-   0        0        0    10518 2023-03-21 07:46:44.000000 PhanMemMMN-0.0.6/img/pause.png
+-rw-rw-rw-   0        0        0    12544 2023-03-20 12:41:41.000000 PhanMemMMN-0.0.6/img/play-button1.png
+-rw-rw-rw-   0        0        0     7111 2023-03-21 07:47:51.000000 PhanMemMMN-0.0.6/img/previous.png
+-rw-rw-rw-   0        0        0      443 2023-03-28 10:41:37.000000 PhanMemMMN-0.0.6/img/repeat-one.png
+-rw-rw-rw-   0        0        0      415 2023-03-28 10:41:15.000000 PhanMemMMN-0.0.6/img/repeat.png
+-rw-rw-rw-   0        0        0      691 2023-03-28 10:46:58.000000 PhanMemMMN-0.0.6/img/shuffle.png
+-rw-rw-rw-   0        0        0       42 2023-04-15 07:55:54.863423 PhanMemMMN-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      458 2023-04-15 07:55:52.000000 PhanMemMMN-0.0.6/setup.py
```

### Comparing `PhanMemMMN-0.0.5/MusicApp.py` & `PhanMemMMN-0.0.6/MusicApp.py`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.5/img/low-volume.png` & `PhanMemMMN-0.0.6/img/low-volume.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.5/img/next-button.png` & `PhanMemMMN-0.0.6/img/next-button.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.5/img/pause.png` & `PhanMemMMN-0.0.6/img/pause.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.5/img/play-button1.png` & `PhanMemMMN-0.0.6/img/play-button1.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.5/img/previous.png` & `PhanMemMMN-0.0.6/img/previous.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.5/img/shuffle.png` & `PhanMemMMN-0.0.6/img/shuffle.png`

 * *Files identical despite different names*

