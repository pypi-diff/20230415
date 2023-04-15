# Comparing `tmp/interlinking-0.0.2.tar.gz` & `tmp/interlinking-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interlinking-0.0.2.tar", last modified: Sat Apr 15 11:11:54 2023, max compression
+gzip compressed data, was "interlinking-0.0.3.tar", last modified: Sat Apr 15 11:14:09 2023, max compression
```

## Comparing `interlinking-0.0.2.tar` & `interlinking-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:11:54.265336 interlinking-0.0.2/
--rw-rw-rw-   0        0        0      706 2023-04-15 11:11:54.264334 interlinking-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 11:11:54.249370 interlinking-0.0.2/interlinking/
--rw-rw-rw-   0        0        0       66 2023-04-15 11:10:19.000000 interlinking-0.0.2/interlinking/__init__.py
--rw-rw-rw-   0        0        0     7964 2023-04-15 10:20:31.000000 interlinking-0.0.2/interlinking/interlinking.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:11:54.262333 interlinking-0.0.2/interlinking.egg-info/
--rw-rw-rw-   0        0        0      706 2023-04-15 11:11:54.000000 interlinking-0.0.2/interlinking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-15 11:11:54.000000 interlinking-0.0.2/interlinking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:11:54.000000 interlinking-0.0.2/interlinking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 11:11:54.000000 interlinking-0.0.2/interlinking.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-15 11:11:54.000000 interlinking-0.0.2/interlinking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 11:11:54.266337 interlinking-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-04-15 11:11:38.000000 interlinking-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:14:09.640031 interlinking-0.0.3/
+-rw-rw-rw-   0        0        0      706 2023-04-15 11:14:09.639019 interlinking-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-15 11:14:09.622018 interlinking-0.0.3/interlinking/
+-rw-rw-rw-   0        0        0       66 2023-04-15 11:10:19.000000 interlinking-0.0.3/interlinking/__init__.py
+-rw-rw-rw-   0        0        0     7964 2023-04-15 10:20:31.000000 interlinking-0.0.3/interlinking/interlinking.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:14:09.635865 interlinking-0.0.3/interlinking.egg-info/
+-rw-rw-rw-   0        0        0      706 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-15 11:14:09.000000 interlinking-0.0.3/interlinking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 11:14:09.641033 interlinking-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-04-15 11:13:02.000000 interlinking-0.0.3/setup.py
```

### Comparing `interlinking-0.0.2/PKG-INFO` & `interlinking-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interlinking
-Version: 0.0.2
+Version: 0.0.3
 Summary: Send messages, files or raw data between python codes(servers, computers, ...).
 Author: AdioSs (Daniel Karlík)
 Author-email: <karlik.dan@gmail.com>
 Keywords: python,server,client,data sending,servers communication,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `interlinking-0.0.2/interlinking/interlinking.py` & `interlinking-0.0.3/interlinking/interlinking.py`

 * *Files identical despite different names*

### Comparing `interlinking-0.0.2/interlinking.egg-info/PKG-INFO` & `interlinking-0.0.3/interlinking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interlinking
-Version: 0.0.2
+Version: 0.0.3
 Summary: Send messages, files or raw data between python codes(servers, computers, ...).
 Author: AdioSs (Daniel Karlík)
 Author-email: <karlik.dan@gmail.com>
 Keywords: python,server,client,data sending,servers communication,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `interlinking-0.0.2/setup.py` & `interlinking-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Send messages, files or raw data between python codes(servers, computers, ...).'
 LONG_DESCRIPTION = 'A package that allows to build simple server with listening and handling all data.'
 
 # Setting up
 setup(
     name="interlinking",
     version=VERSION,
```

