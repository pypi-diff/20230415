# Comparing `tmp/a_pandas_ex_easy_loc-0.11.tar.gz` & `tmp/a_pandas_ex_easy_loc-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_easy_loc-0.11.tar", last modified: Fri Apr 14 23:34:46 2023, max compression
+gzip compressed data, was "a_pandas_ex_easy_loc-0.13.tar", last modified: Fri Apr 14 23:38:45 2023, max compression
```

## Comparing `a_pandas_ex_easy_loc-0.11.tar` & `a_pandas_ex_easy_loc-0.13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 23:34:46.202157 a_pandas_ex_easy_loc-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-14 23:34:41.000000 a_pandas_ex_easy_loc-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      131 2023-04-14 23:34:41.000000 a_pandas_ex_easy_loc-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0    55576 2023-04-14 23:34:46.203154 a_pandas_ex_easy_loc-0.11/PKG-INFO
--rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 23:34:46.198167 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/
--rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/README.MD
--rw-rw-rw-   0        0        0    22528 2023-04-14 23:17:13.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/__init__.py
--rw-rw-rw-   0        0        0      103 2023-04-14 23:34:45.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/requirements.txt
--rw-rw-rw-   0        0        0     5332 2023-04-14 23:34:45.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-14 23:34:46.202157 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc.egg-info/
--rw-rw-rw-   0        0        0    55576 2023-04-14 23:34:45.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-14 23:34:46.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 23:34:45.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-14 23:34:45.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-14 23:34:45.000000 a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      168 2023-04-14 23:34:46.203154 a_pandas_ex_easy_loc-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-04-14 23:34:45.000000 a_pandas_ex_easy_loc-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 23:38:45.485807 a_pandas_ex_easy_loc-0.13/
+-rw-rw-rw-   0        0        0     1148 2023-04-14 23:38:41.000000 a_pandas_ex_easy_loc-0.13/LICENSE.rst
+-rw-rw-rw-   0        0        0      131 2023-04-14 23:38:41.000000 a_pandas_ex_easy_loc-0.13/MANIFEST.in
+-rw-rw-rw-   0        0        0    55576 2023-04-14 23:38:45.486805 a_pandas_ex_easy_loc-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 23:38:45.481817 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/
+-rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/README.md
+-rw-rw-rw-   0        0        0    22528 2023-04-14 23:17:13.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-04-14 23:38:44.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/requirements.txt
+-rw-rw-rw-   0        0        0     5332 2023-04-14 23:38:44.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-14 23:38:45.484810 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/
+-rw-rw-rw-   0        0        0    55576 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-14 23:38:45.486805 a_pandas_ex_easy_loc-0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-04-14 23:38:44.000000 a_pandas_ex_easy_loc-0.13/setup.py
```

### Comparing `a_pandas_ex_easy_loc-0.11/LICENSE.rst` & `a_pandas_ex_easy_loc-0.13/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.11/PKG-INFO` & `a_pandas_ex_easy_loc-0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a_pandas_ex_easy_loc
-Version: 0.11
+Version: 0.13
 Summary: Search and replace values with df.loc without Exceptions due to dtype incompatibility
 Home-page: https://github.com/hansalemaos/a_pandas_ex_easy_loc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: loc,iloc,df.at,df.iat,pandas,DataFrame,Series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `a_pandas_ex_easy_loc-0.11/README.md` & `a_pandas_ex_easy_loc-0.13/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/README.MD` & `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/__init__.py` & `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/__init__.py`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc/thirdparty.json` & `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/thirdparty.json`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.11/a_pandas_ex_easy_loc.egg-info/PKG-INFO` & `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a-pandas-ex-easy-loc
-Version: 0.11
+Version: 0.13
 Summary: Search and replace values with df.loc without Exceptions due to dtype incompatibility
 Home-page: https://github.com/hansalemaos/a_pandas_ex_easy_loc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: loc,iloc,df.at,df.iat,pandas,DataFrame,Series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `a_pandas_ex_easy_loc-0.11/setup.py` & `a_pandas_ex_easy_loc-0.13/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '''0.11'''
+VERSION = '''0.13'''
 DESCRIPTION = '''Search and replace values with df.loc without Exceptions due to dtype incompatibility'''
 
 # Setting up
 setup(
     name="a_pandas_ex_easy_loc",
     version=VERSION,
     license='MIT',
```

