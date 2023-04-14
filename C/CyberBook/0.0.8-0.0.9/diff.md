# Comparing `tmp/CyberBook-0.0.8.tar.gz` & `tmp/CyberBook-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CyberBook-0.0.8.tar", last modified: Wed Dec  7 17:17:55 2022, max compression
+gzip compressed data, was "CyberBook-0.0.9.tar", last modified: Wed Dec  7 17:58:19 2022, max compression
```

## Comparing `CyberBook-0.0.8.tar` & `CyberBook-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 17:17:55.404666 CyberBook-0.0.8/
-drwxrwxrwx   0        0        0        0 2022-12-07 17:17:55.388701 CyberBook-0.0.8/CyberBook/
-drwxrwxrwx   0        0        0        0 2022-12-07 17:17:55.399675 CyberBook-0.0.8/CyberBook/DecoderRing/
--rw-rw-rw-   0        0        0       31 2022-12-04 16:19:01.000000 CyberBook-0.0.8/CyberBook/DecoderRing/__init__.py
--rw-rw-rw-   0        0        0     2992 2022-12-07 17:16:29.000000 CyberBook-0.0.8/CyberBook/DecoderRing/main.py
--rw-rw-rw-   0        0        0      476 2022-12-04 14:40:56.000000 CyberBook-0.0.8/CyberBook/DecoderRing/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-07 17:17:55.400673 CyberBook-0.0.8/CyberBook/Identify/
--rw-rw-rw-   0        0        0       29 2022-12-04 16:23:42.000000 CyberBook-0.0.8/CyberBook/Identify/__init__.py
--rw-rw-rw-   0        0        0      616 2022-12-04 16:23:42.000000 CyberBook-0.0.8/CyberBook/Identify/os_specifics.py
-drwxrwxrwx   0        0        0        0 2022-12-07 17:17:55.402671 CyberBook-0.0.8/CyberBook/Misc/
--rw-rw-rw-   0        0        0       76 2022-12-04 16:28:34.000000 CyberBook-0.0.8/CyberBook/Misc/__init__.py
--rw-rw-rw-   0        0        0     1029 2022-12-04 16:20:00.000000 CyberBook-0.0.8/CyberBook/Misc/reverse_shell.py
--rw-rw-rw-   0        0        0      737 2022-12-04 14:40:56.000000 CyberBook-0.0.8/CyberBook/Misc/tools.py
-drwxrwxrwx   0        0        0        0 2022-12-07 17:17:55.402671 CyberBook-0.0.8/CyberBook/SummoningCircle/
--rw-rw-rw-   0        0        0       35 2022-12-07 16:47:10.000000 CyberBook-0.0.8/CyberBook/SummoningCircle/__init__.py
--rw-rw-rw-   0        0        0     3206 2022-12-07 17:03:11.000000 CyberBook-0.0.8/CyberBook/SummoningCircle/main.py
--rw-rw-rw-   0        0        0      105 2022-12-04 16:28:34.000000 CyberBook-0.0.8/CyberBook/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-07 17:17:55.398677 CyberBook-0.0.8/CyberBook.egg-info/
--rw-rw-rw-   0        0        0      814 2022-12-07 17:17:55.000000 CyberBook-0.0.8/CyberBook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2022-12-07 17:17:55.000000 CyberBook-0.0.8/CyberBook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 17:17:55.000000 CyberBook-0.0.8/CyberBook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-03 19:13:38.000000 CyberBook-0.0.8/CyberBook.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2022-12-07 17:17:55.000000 CyberBook-0.0.8/CyberBook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-07 17:17:55.000000 CyberBook-0.0.8/CyberBook.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-11-28 01:01:57.000000 CyberBook-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      814 2022-12-07 17:17:55.403664 CyberBook-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      406 2022-12-07 17:17:43.000000 CyberBook-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-12-07 17:17:55.404666 CyberBook-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      872 2022-12-07 17:17:43.000000 CyberBook-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-07 17:58:19.187441 CyberBook-0.0.9/
+drwxrwxrwx   0        0        0        0 2022-12-07 17:58:19.169641 CyberBook-0.0.9/CyberBook/
+drwxrwxrwx   0        0        0        0 2022-12-07 17:58:19.182605 CyberBook-0.0.9/CyberBook/DecoderRing/
+-rw-rw-rw-   0        0        0       31 2022-12-04 16:19:01.000000 CyberBook-0.0.9/CyberBook/DecoderRing/__init__.py
+-rw-rw-rw-   0        0        0     2992 2022-12-07 17:16:29.000000 CyberBook-0.0.9/CyberBook/DecoderRing/main.py
+-rw-rw-rw-   0        0        0      476 2022-12-04 14:40:56.000000 CyberBook-0.0.9/CyberBook/DecoderRing/utils.py
+drwxrwxrwx   0        0        0        0 2022-12-07 17:58:19.182605 CyberBook-0.0.9/CyberBook/Identify/
+-rw-rw-rw-   0        0        0       29 2022-12-04 16:23:42.000000 CyberBook-0.0.9/CyberBook/Identify/__init__.py
+-rw-rw-rw-   0        0        0      616 2022-12-04 16:23:42.000000 CyberBook-0.0.9/CyberBook/Identify/os_specifics.py
+drwxrwxrwx   0        0        0        0 2022-12-07 17:58:19.184600 CyberBook-0.0.9/CyberBook/Misc/
+-rw-rw-rw-   0        0        0       76 2022-12-04 16:28:34.000000 CyberBook-0.0.9/CyberBook/Misc/__init__.py
+-rw-rw-rw-   0        0        0     1029 2022-12-04 16:20:00.000000 CyberBook-0.0.9/CyberBook/Misc/reverse_shell.py
+-rw-rw-rw-   0        0        0      737 2022-12-04 14:40:56.000000 CyberBook-0.0.9/CyberBook/Misc/tools.py
+drwxrwxrwx   0        0        0        0 2022-12-07 17:58:19.185612 CyberBook-0.0.9/CyberBook/SummoningCircle/
+-rw-rw-rw-   0        0        0       35 2022-12-07 16:47:10.000000 CyberBook-0.0.9/CyberBook/SummoningCircle/__init__.py
+-rw-rw-rw-   0        0        0     3206 2022-12-07 17:03:11.000000 CyberBook-0.0.9/CyberBook/SummoningCircle/main.py
+-rw-rw-rw-   0        0        0      105 2022-12-04 16:28:34.000000 CyberBook-0.0.9/CyberBook/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-07 17:58:19.180611 CyberBook-0.0.9/CyberBook.egg-info/
+-rw-rw-rw-   0        0        0     1516 2022-12-07 17:58:19.000000 CyberBook-0.0.9/CyberBook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2022-12-07 17:58:19.000000 CyberBook-0.0.9/CyberBook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-07 17:58:19.000000 CyberBook-0.0.9/CyberBook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-03 19:13:38.000000 CyberBook-0.0.9/CyberBook.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2022-12-07 17:58:19.000000 CyberBook-0.0.9/CyberBook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-12-07 17:58:19.000000 CyberBook-0.0.9/CyberBook.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-11-28 01:01:57.000000 CyberBook-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1516 2022-12-07 17:58:19.186442 CyberBook-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1108 2022-12-07 17:39:53.000000 CyberBook-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-12-07 17:58:19.187441 CyberBook-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      872 2022-12-07 17:58:12.000000 CyberBook-0.0.9/setup.py
```

### Comparing `CyberBook-0.0.8/CyberBook/DecoderRing/main.py` & `CyberBook-0.0.9/CyberBook/DecoderRing/main.py`

 * *Files identical despite different names*

### Comparing `CyberBook-0.0.8/CyberBook/Identify/os_specifics.py` & `CyberBook-0.0.9/CyberBook/Identify/os_specifics.py`

 * *Files identical despite different names*

### Comparing `CyberBook-0.0.8/CyberBook/Misc/reverse_shell.py` & `CyberBook-0.0.9/CyberBook/Misc/reverse_shell.py`

 * *Files identical despite different names*

### Comparing `CyberBook-0.0.8/CyberBook/Misc/tools.py` & `CyberBook-0.0.9/CyberBook/Misc/tools.py`

 * *Files identical despite different names*

### Comparing `CyberBook-0.0.8/CyberBook/SummoningCircle/main.py` & `CyberBook-0.0.9/CyberBook/SummoningCircle/main.py`

 * *Files identical despite different names*

### Comparing `CyberBook-0.0.8/CyberBook.egg-info/SOURCES.txt` & `CyberBook-0.0.9/CyberBook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CyberBook-0.0.8/LICENSE` & `CyberBook-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CyberBook-0.0.8/setup.py` & `CyberBook-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='CyberBook',
-      version='0.0.8',
+      version='0.0.9',
       description='Cyber spellbook for developers.',
       url='https://github.com/ClutchTech/CyberBook',
       keywords='cyberbook DecoderRing tools',
       author='Clutch_Reboot',
       author_email='clutchshadow26@gmail.com',
       license='GNU General Public License v3.0',
       packages=[
```

