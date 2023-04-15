# Comparing `tmp/frida-9.1.8.tar.gz` & `tmp/frida-9.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\frida-9.1.8.tar", last modified: Tue Feb 21 17:46:03 2017, max compression
+gzip compressed data, was "dist\frida-9.1.9.tar", last modified: Sat Feb 25 01:15:19 2017, max compression
```

## Comparing `frida-9.1.8.tar` & `frida-9.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2017-02-21 17:46:03.000000 frida-9.1.8/
-drwxrwxrwx   0        0        0        0 2017-02-21 17:46:03.000000 frida-9.1.8/frida/
--rw-rw-rw-   0        0        0    14378 2017-02-21 17:26:01.000000 frida-9.1.8/frida/application.py
--rw-rw-rw-   0        0        0    18734 2017-02-21 17:26:01.000000 frida-9.1.8/frida/core.py
--rw-rw-rw-   0        0        0     6537 2017-02-21 17:26:01.000000 frida-9.1.8/frida/discoverer.py
--rw-rw-rw-   0        0        0     2971 2017-02-21 17:26:01.000000 frida-9.1.8/frida/lsd.py
--rw-rw-rw-   0        0        0     5446 2017-02-21 17:26:01.000000 frida-9.1.8/frida/ps.py
--rw-rw-rw-   0        0        0    23012 2017-02-21 17:26:01.000000 frida-9.1.8/frida/repl.py
--rw-rw-rw-   0        0        0    32176 2017-02-21 17:26:01.000000 frida-9.1.8/frida/tracer.py
--rw-rw-rw-   0        0        0     3988 2017-02-21 17:26:01.000000 frida-9.1.8/frida/__init__.py
-drwxrwxrwx   0        0        0        0 2017-02-21 17:46:03.000000 frida-9.1.8/frida.egg-info/
--rw-rw-rw-   0        0        0        1 2017-02-21 17:46:02.000000 frida-9.1.8/frida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2017-02-21 17:46:02.000000 frida-9.1.8/frida.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1358 2017-02-21 17:46:02.000000 frida-9.1.8/frida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       59 2017-02-21 17:46:02.000000 frida-9.1.8/frida.egg-info/requires.txt
--rw-rw-rw-   0        0        0      336 2017-02-21 17:46:03.000000 frida-9.1.8/frida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2017-02-21 17:46:02.000000 frida-9.1.8/frida.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2017-02-21 17:45:04.000000 frida-9.1.8/frida.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1358 2017-02-21 17:46:03.000000 frida-9.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2017-02-21 17:46:03.000000 frida-9.1.8/setup.cfg
--rw-rw-rw-   0        0        0     6978 2017-02-21 17:26:01.000000 frida-9.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2017-02-25 01:15:19.000000 frida-9.1.9/
+drwxrwxrwx   0        0        0        0 2017-02-25 01:15:19.000000 frida-9.1.9/frida/
+-rw-rw-rw-   0        0        0    14378 2017-02-21 17:26:01.000000 frida-9.1.9/frida/application.py
+-rw-rw-rw-   0        0        0    18734 2017-02-21 17:26:01.000000 frida-9.1.9/frida/core.py
+-rw-rw-rw-   0        0        0     6537 2017-02-21 17:26:01.000000 frida-9.1.9/frida/discoverer.py
+-rw-rw-rw-   0        0        0     2971 2017-02-21 17:26:01.000000 frida-9.1.9/frida/lsd.py
+-rw-rw-rw-   0        0        0     5446 2017-02-21 17:26:01.000000 frida-9.1.9/frida/ps.py
+-rw-rw-rw-   0        0        0    23012 2017-02-21 17:26:01.000000 frida-9.1.9/frida/repl.py
+-rw-rw-rw-   0        0        0    32176 2017-02-21 17:26:01.000000 frida-9.1.9/frida/tracer.py
+-rw-rw-rw-   0        0        0     3988 2017-02-21 17:26:01.000000 frida-9.1.9/frida/__init__.py
+drwxrwxrwx   0        0        0        0 2017-02-25 01:15:19.000000 frida-9.1.9/frida.egg-info/
+-rw-rw-rw-   0        0        0        1 2017-02-25 01:15:18.000000 frida-9.1.9/frida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2017-02-25 01:15:18.000000 frida-9.1.9/frida.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1358 2017-02-25 01:15:18.000000 frida-9.1.9/frida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2017-02-25 01:15:18.000000 frida-9.1.9/frida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      336 2017-02-25 01:15:19.000000 frida-9.1.9/frida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       13 2017-02-25 01:15:18.000000 frida-9.1.9/frida.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2017-02-21 17:45:04.000000 frida-9.1.9/frida.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1358 2017-02-25 01:15:19.000000 frida-9.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2017-02-25 01:15:19.000000 frida-9.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     6978 2017-02-21 17:26:01.000000 frida-9.1.9/setup.py
```

### Comparing `frida-9.1.8/frida/application.py` & `frida-9.1.9/frida/application.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida/core.py` & `frida-9.1.9/frida/core.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida/discoverer.py` & `frida-9.1.9/frida/discoverer.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida/lsd.py` & `frida-9.1.9/frida/lsd.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida/ps.py` & `frida-9.1.9/frida/ps.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida/repl.py` & `frida-9.1.9/frida/repl.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida/tracer.py` & `frida-9.1.9/frida/tracer.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida/__init__.py` & `frida-9.1.9/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `frida-9.1.8/frida.egg-info/PKG-INFO` & `frida-9.1.9/frida.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: frida
-Version: 9.1.8
+Version: 9.1.9
 Summary: Inject JavaScript to explore native apps on Windows, macOS, Linux, iOS, Android, and QNX
 Home-page: http://www.frida.re
 Author: Frida Developers
 Author-email: oleavr@nowsecure.com
 License: wxWindows Library Licence, Version 3.1
 Description: # frida-python
```

### Comparing `frida-9.1.8/PKG-INFO` & `frida-9.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: frida
-Version: 9.1.8
+Version: 9.1.9
 Summary: Inject JavaScript to explore native apps on Windows, macOS, Linux, iOS, Android, and QNX
 Home-page: http://www.frida.re
 Author: Frida Developers
 Author-email: oleavr@nowsecure.com
 License: wxWindows Library Licence, Version 3.1
 Description: # frida-python
```

### Comparing `frida-9.1.8/setup.py` & `frida-9.1.9/setup.py`

 * *Files identical despite different names*

