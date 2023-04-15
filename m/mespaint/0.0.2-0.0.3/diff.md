# Comparing `tmp/mespaint-0.0.2.tar.gz` & `tmp/mespaint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mespaint-0.0.2.tar", last modified: Sat Apr 15 08:18:55 2023, max compression
+gzip compressed data, was "mespaint-0.0.3.tar", last modified: Sat Apr 15 08:20:54 2023, max compression
```

## Comparing `mespaint-0.0.2.tar` & `mespaint-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:18:55.001595 mespaint-0.0.2/
--rw-r--r--   0 vandi     (1000) vandi     (1000)     1067 2023-04-15 02:13:50.000000 mespaint-0.0.2/LICENSE
--rw-r--r--   0 vandi     (1000) vandi     (1000)      647 2023-04-15 08:18:55.001595 mespaint-0.0.2/PKG-INFO
--rw-r--r--   0 vandi     (1000) vandi     (1000)      369 2023-04-15 08:13:02.000000 mespaint-0.0.2/README.md
-drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:18:55.001595 mespaint-0.0.2/mespaint.egg-info/
--rw-r--r--   0 vandi     (1000) vandi     (1000)      647 2023-04-15 08:18:54.000000 mespaint-0.0.2/mespaint.egg-info/PKG-INFO
--rw-r--r--   0 vandi     (1000) vandi     (1000)      378 2023-04-15 08:18:54.000000 mespaint-0.0.2/mespaint.egg-info/SOURCES.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)        1 2023-04-15 08:18:54.000000 mespaint-0.0.2/mespaint.egg-info/dependency_links.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)       43 2023-04-15 08:18:54.000000 mespaint-0.0.2/mespaint.egg-info/entry_points.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)       26 2023-04-15 08:18:54.000000 mespaint-0.0.2/mespaint.egg-info/requires.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)        4 2023-04-15 08:18:54.000000 mespaint-0.0.2/mespaint.egg-info/top_level.txt
--rw-r--r--   0 vandi     (1000) vandi     (1000)       38 2023-04-15 08:18:55.001595 mespaint-0.0.2/setup.cfg
--rw-r--r--   0 vandi     (1000) vandi     (1000)      788 2023-04-15 07:51:14.000000 mespaint-0.0.2/setup.py
-drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:18:55.001595 mespaint-0.0.2/src/
--rw-r--r--   0 vandi     (1000) vandi     (1000)      237 2023-04-15 08:13:58.000000 mespaint-0.0.2/src/__init__.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     3047 2023-04-15 02:07:19.000000 mespaint-0.0.2/src/aboutdialog.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     5999 2023-04-15 02:02:01.000000 mespaint-0.0.2/src/canvas.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     1366 2023-04-15 02:02:49.000000 mespaint-0.0.2/src/inittab.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)      374 2023-04-15 07:44:51.000000 mespaint-0.0.2/src/main.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     6832 2023-04-15 07:44:51.000000 mespaint-0.0.2/src/mainwindow.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     3467 2023-04-15 07:44:51.000000 mespaint-0.0.2/src/menubar.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     2385 2023-04-15 00:35:35.000000 mespaint-0.0.2/src/palette.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     6576 2023-04-15 07:44:51.000000 mespaint-0.0.2/src/palettebutton.py
--rw-r--r--   0 vandi     (1000) vandi     (1000)     1093 2023-03-31 10:38:17.000000 mespaint-0.0.2/src/utils.py
+drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:20:54.495756 mespaint-0.0.3/
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1067 2023-04-15 02:13:50.000000 mespaint-0.0.3/LICENSE
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      647 2023-04-15 08:20:54.495756 mespaint-0.0.3/PKG-INFO
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      369 2023-04-15 08:13:02.000000 mespaint-0.0.3/README.md
+drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:20:54.492423 mespaint-0.0.3/mespaint.egg-info/
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      647 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/PKG-INFO
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      378 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/SOURCES.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)        1 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/dependency_links.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)       43 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/entry_points.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)       26 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/requires.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)        4 2023-04-15 08:20:54.000000 mespaint-0.0.3/mespaint.egg-info/top_level.txt
+-rw-r--r--   0 vandi     (1000) vandi     (1000)       38 2023-04-15 08:20:54.495756 mespaint-0.0.3/setup.cfg
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      788 2023-04-15 07:51:14.000000 mespaint-0.0.3/setup.py
+drwxr-xr-x   0 vandi     (1000) vandi     (1000)        0 2023-04-15 08:20:54.495756 mespaint-0.0.3/src/
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      237 2023-04-15 08:20:17.000000 mespaint-0.0.3/src/__init__.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     3047 2023-04-15 02:07:19.000000 mespaint-0.0.3/src/aboutdialog.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     5999 2023-04-15 02:02:01.000000 mespaint-0.0.3/src/canvas.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1366 2023-04-15 02:02:49.000000 mespaint-0.0.3/src/inittab.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)      374 2023-04-15 07:44:51.000000 mespaint-0.0.3/src/main.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     5608 2023-04-15 08:20:17.000000 mespaint-0.0.3/src/mainwindow.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     3467 2023-04-15 07:44:51.000000 mespaint-0.0.3/src/menubar.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     2385 2023-04-15 00:35:35.000000 mespaint-0.0.3/src/palette.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     6576 2023-04-15 07:44:51.000000 mespaint-0.0.3/src/palettebutton.py
+-rw-r--r--   0 vandi     (1000) vandi     (1000)     1093 2023-03-31 10:38:17.000000 mespaint-0.0.3/src/utils.py
```

### Comparing `mespaint-0.0.2/LICENSE` & `mespaint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/PKG-INFO` & `mespaint-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mespaint
-Version: 0.0.2
+Version: 0.0.3
 Summary: custom palette changer for indexed PNGs
 Home-page: https://github.com/menga-team/MESpaint
-Author: 0.0.2
+Author: 0.0.3
 Author-email: menga.team@yandex.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MES-Paint
 Application for editing indexed PNGs palettes. Mainly used for the creation of MES textures.
```

### Comparing `mespaint-0.0.2/mespaint.egg-info/PKG-INFO` & `mespaint-0.0.3/mespaint.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mespaint
-Version: 0.0.2
+Version: 0.0.3
 Summary: custom palette changer for indexed PNGs
 Home-page: https://github.com/menga-team/MESpaint
-Author: 0.0.2
+Author: 0.0.3
 Author-email: menga.team@yandex.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MES-Paint
 Application for editing indexed PNGs palettes. Mainly used for the creation of MES textures.
```

### Comparing `mespaint-0.0.2/setup.py` & `mespaint-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/src/aboutdialog.py` & `mespaint-0.0.3/src/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/src/canvas.py` & `mespaint-0.0.3/src/canvas.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/src/inittab.py` & `mespaint-0.0.3/src/inittab.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/src/menubar.py` & `mespaint-0.0.3/src/menubar.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/src/palette.py` & `mespaint-0.0.3/src/palette.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/src/palettebutton.py` & `mespaint-0.0.3/src/palettebutton.py`

 * *Files identical despite different names*

### Comparing `mespaint-0.0.2/src/utils.py` & `mespaint-0.0.3/src/utils.py`

 * *Files identical despite different names*

