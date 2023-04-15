# Comparing `tmp/PhanMemMMN-0.0.3.tar.gz` & `tmp/PhanMemMMN-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhanMemMMN-0.0.3.tar", last modified: Sat Apr 15 06:42:02 2023, max compression
+gzip compressed data, was "PhanMemMMN-0.0.4.tar", last modified: Sat Apr 15 07:41:58 2023, max compression
```

## Comparing `PhanMemMMN-0.0.3.tar` & `PhanMemMMN-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 06:42:02.272745 PhanMemMMN-0.0.3/
--rw-rw-rw-   0        0        0       13 2023-03-19 12:46:25.000000 PhanMemMMN-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    10290 2023-04-13 03:55:17.000000 PhanMemMMN-0.0.3/MusicApp.py
--rw-rw-rw-   0        0        0      152 2023-04-15 06:42:02.271748 PhanMemMMN-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 06:42:02.261777 PhanMemMMN-0.0.3/PhanMemMMN.egg-info/
--rw-rw-rw-   0        0        0      152 2023-04-15 06:42:02.000000 PhanMemMMN-0.0.3/PhanMemMMN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-15 06:42:02.000000 PhanMemMMN-0.0.3/PhanMemMMN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 06:42:02.000000 PhanMemMMN-0.0.3/PhanMemMMN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-15 06:42:02.000000 PhanMemMMN-0.0.3/PhanMemMMN.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 06:42:02.000000 PhanMemMMN-0.0.3/PhanMemMMN.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 06:42:02.270752 PhanMemMMN-0.0.3/img/
--rw-rw-rw-   0        0        0     7219 2023-04-09 09:15:25.000000 PhanMemMMN-0.0.3/img/low-volume.png
--rw-rw-rw-   0        0        0     7641 2023-03-21 07:47:31.000000 PhanMemMMN-0.0.3/img/next-button.png
--rw-rw-rw-   0        0        0    10518 2023-03-21 07:46:44.000000 PhanMemMMN-0.0.3/img/pause.png
--rw-rw-rw-   0        0        0    12544 2023-03-20 12:41:41.000000 PhanMemMMN-0.0.3/img/play-button1.png
--rw-rw-rw-   0        0        0     7111 2023-03-21 07:47:51.000000 PhanMemMMN-0.0.3/img/previous.png
--rw-rw-rw-   0        0        0      443 2023-03-28 10:41:37.000000 PhanMemMMN-0.0.3/img/repeat-one.png
--rw-rw-rw-   0        0        0      415 2023-03-28 10:41:15.000000 PhanMemMMN-0.0.3/img/repeat.png
--rw-rw-rw-   0        0        0      691 2023-03-28 10:46:58.000000 PhanMemMMN-0.0.3/img/shuffle.png
--rw-rw-rw-   0        0        0       42 2023-04-15 06:42:02.272745 PhanMemMMN-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      457 2023-04-15 06:41:47.000000 PhanMemMMN-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 07:41:58.520573 PhanMemMMN-0.0.4/
+-rw-rw-rw-   0        0        0       65 2023-04-15 07:40:27.000000 PhanMemMMN-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    10290 2023-04-13 03:55:17.000000 PhanMemMMN-0.0.4/MusicApp.py
+-rw-rw-rw-   0        0        0      152 2023-04-15 07:41:58.520573 PhanMemMMN-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-15 07:41:58.508147 PhanMemMMN-0.0.4/PhanMemMMN.egg-info/
+-rw-rw-rw-   0        0        0      152 2023-04-15 07:41:58.000000 PhanMemMMN-0.0.4/PhanMemMMN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-15 07:41:58.000000 PhanMemMMN-0.0.4/PhanMemMMN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 07:41:58.000000 PhanMemMMN-0.0.4/PhanMemMMN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-15 07:41:58.000000 PhanMemMMN-0.0.4/PhanMemMMN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 07:41:58.000000 PhanMemMMN-0.0.4/PhanMemMMN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 07:41:58.518051 PhanMemMMN-0.0.4/img/
+-rw-rw-rw-   0        0        0     7219 2023-04-09 09:15:25.000000 PhanMemMMN-0.0.4/img/low-volume.png
+-rw-rw-rw-   0        0        0     7641 2023-03-21 07:47:31.000000 PhanMemMMN-0.0.4/img/next-button.png
+-rw-rw-rw-   0        0        0    10518 2023-03-21 07:46:44.000000 PhanMemMMN-0.0.4/img/pause.png
+-rw-rw-rw-   0        0        0    12544 2023-03-20 12:41:41.000000 PhanMemMMN-0.0.4/img/play-button1.png
+-rw-rw-rw-   0        0        0     7111 2023-03-21 07:47:51.000000 PhanMemMMN-0.0.4/img/previous.png
+-rw-rw-rw-   0        0        0      443 2023-03-28 10:41:37.000000 PhanMemMMN-0.0.4/img/repeat-one.png
+-rw-rw-rw-   0        0        0      415 2023-03-28 10:41:15.000000 PhanMemMMN-0.0.4/img/repeat.png
+-rw-rw-rw-   0        0        0      691 2023-03-28 10:46:58.000000 PhanMemMMN-0.0.4/img/shuffle.png
+-rw-rw-rw-   0        0        0       42 2023-04-15 07:41:58.521580 PhanMemMMN-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      365 2023-04-15 07:41:49.000000 PhanMemMMN-0.0.4/setup.py
```

### Comparing `PhanMemMMN-0.0.3/MusicApp.py` & `PhanMemMMN-0.0.4/MusicApp.py`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.3/img/low-volume.png` & `PhanMemMMN-0.0.4/img/low-volume.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.3/img/next-button.png` & `PhanMemMMN-0.0.4/img/next-button.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.3/img/pause.png` & `PhanMemMMN-0.0.4/img/pause.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.3/img/play-button1.png` & `PhanMemMMN-0.0.4/img/play-button1.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.3/img/previous.png` & `PhanMemMMN-0.0.4/img/previous.png`

 * *Files identical despite different names*

### Comparing `PhanMemMMN-0.0.3/img/shuffle.png` & `PhanMemMMN-0.0.4/img/shuffle.png`

 * *Files identical despite different names*

