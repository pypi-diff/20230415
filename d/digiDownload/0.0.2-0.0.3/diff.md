# Comparing `tmp/digiDownload-0.0.2.tar.gz` & `tmp/digiDownload-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiDownload-0.0.2.tar", last modified: Sat Apr 15 18:43:47 2023, max compression
+gzip compressed data, was "digiDownload-0.0.3.tar", last modified: Sat Apr 15 18:47:50 2023, max compression
```

## Comparing `digiDownload-0.0.2.tar` & `digiDownload-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:43:47.870767 digiDownload-0.0.2/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-15 18:43:47.870767 digiDownload-0.0.2/PKG-INFO
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:43:47.870767 digiDownload-0.0.2/digiDownload/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      176 2023-04-15 14:38:11.000000 digiDownload-0.0.2/digiDownload/AdBlockCookiePolicy.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     2114 2023-04-15 16:18:10.000000 digiDownload-0.0.2/digiDownload/Book.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)      628 2023-04-15 16:01:32.000000 digiDownload-0.0.2/digiDownload/LTIParser.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1317 2023-04-15 18:37:34.000000 digiDownload-0.0.2/digiDownload/Session.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)       29 2023-04-15 17:22:08.000000 digiDownload-0.0.2/digiDownload/__init__.py
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:43:47.870767 digiDownload-0.0.2/digiDownload.egg-info/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-15 18:43:47.000000 digiDownload-0.0.2/digiDownload.egg-info/PKG-INFO
--rw-r--r--   0 notyou    (1000) notyou    (1000)      329 2023-04-15 18:43:47.000000 digiDownload-0.0.2/digiDownload.egg-info/SOURCES.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-15 18:43:47.000000 digiDownload-0.0.2/digiDownload.egg-info/dependency_links.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       24 2023-04-15 18:43:47.000000 digiDownload-0.0.2/digiDownload.egg-info/requires.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-15 18:43:47.000000 digiDownload-0.0.2/digiDownload.egg-info/top_level.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       79 2023-04-15 18:43:47.870767 digiDownload-0.0.2/setup.cfg
--rw-r--r--   0 notyou    (1000) notyou    (1000)      464 2023-04-15 18:40:02.000000 digiDownload-0.0.2/setup.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:47:50.516475 digiDownload-0.0.3/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-15 18:47:50.516475 digiDownload-0.0.3/PKG-INFO
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:47:50.516475 digiDownload-0.0.3/digiDownload/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      176 2023-04-15 14:38:11.000000 digiDownload-0.0.3/digiDownload/AdBlockCookiePolicy.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     2116 2023-04-15 18:46:06.000000 digiDownload-0.0.3/digiDownload/Book.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      628 2023-04-15 16:01:32.000000 digiDownload-0.0.3/digiDownload/LTIParser.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1293 2023-04-15 18:46:06.000000 digiDownload-0.0.3/digiDownload/Session.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       29 2023-04-15 17:22:08.000000 digiDownload-0.0.3/digiDownload/__init__.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-15 18:47:50.516475 digiDownload-0.0.3/digiDownload.egg-info/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      305 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      329 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/SOURCES.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/dependency_links.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       24 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/requires.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-15 18:47:50.000000 digiDownload-0.0.3/digiDownload.egg-info/top_level.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       79 2023-04-15 18:47:50.516475 digiDownload-0.0.3/setup.cfg
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      464 2023-04-15 18:46:06.000000 digiDownload-0.0.3/setup.py
```

### Comparing `digiDownload-0.0.2/digiDownload/Book.py` & `digiDownload-0.0.3/digiDownload/Book.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from LTIParser import LTIForm
+from .LTIParser import LTIForm
+
 from threading import Thread
 from time import sleep
 from sys import maxsize
 
 
 class Book:
     urls = {
```

### Comparing `digiDownload-0.0.2/digiDownload/LTIParser.py` & `digiDownload-0.0.3/digiDownload/LTIParser.py`

 * *Files identical despite different names*

### Comparing `digiDownload-0.0.2/digiDownload/Session.py` & `digiDownload-0.0.3/digiDownload/Session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from .AdBlockCookiePolicy import AdBlockPolicy
+from .Book import Book
+
 from requests import Session as rSession
 from bs4 import BeautifulSoup
-
-from digiDownload.AdBlockCookiePolicy import AdBlockPolicy
-from digiDownload.Book import Book
 from urllib.parse import quote
 
 
 class Session:
     def __init__(self, email, password, remember_login=False):
         self.client = rSession()
         self.client.cookies.set_policy(AdBlockPolicy())
```

