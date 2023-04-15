# Comparing `tmp/a_pandas_ex_easy_loc-0.14.tar.gz` & `tmp/a_pandas_ex_easy_loc-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_easy_loc-0.14.tar", last modified: Fri Apr 14 23:43:31 2023, max compression
+gzip compressed data, was "a_pandas_ex_easy_loc-0.15.tar", last modified: Sat Apr 15 00:24:07 2023, max compression
```

## Comparing `a_pandas_ex_easy_loc-0.14.tar` & `a_pandas_ex_easy_loc-0.15.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 23:43:31.825339 a_pandas_ex_easy_loc-0.14/
--rw-rw-rw-   0        0        0     1148 2023-04-14 23:43:27.000000 a_pandas_ex_easy_loc-0.14/LICENSE.rst
--rw-rw-rw-   0        0        0      131 2023-04-14 23:43:27.000000 a_pandas_ex_easy_loc-0.14/MANIFEST.in
--rw-rw-rw-   0        0        0    55124 2023-04-14 23:43:31.825339 a_pandas_ex_easy_loc-0.14/PKG-INFO
--rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 23:43:31.820352 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/
--rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/README.md
--rw-rw-rw-   0        0        0    22528 2023-04-14 23:17:13.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/__init__.py
--rw-rw-rw-   0        0        0      103 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/requirements.txt
--rw-rw-rw-   0        0        0     5332 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-14 23:43:31.824342 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/
--rw-rw-rw-   0        0        0    55124 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-14 23:43:31.826336 a_pandas_ex_easy_loc-0.14/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:24:07.296274 a_pandas_ex_easy_loc-0.15/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 a_pandas_ex_easy_loc-0.15/LICENSE.rst
+-rw-rw-rw-   0        0        0      131 2023-04-15 00:23:58.000000 a_pandas_ex_easy_loc-0.15/MANIFEST.in
+-rw-rw-rw-   0        0        0    55124 2023-04-15 00:24:07.297271 a_pandas_ex_easy_loc-0.15/PKG-INFO
+-rw-rw-rw-   0        0        0    54417 2023-04-15 00:18:47.000000 a_pandas_ex_easy_loc-0.15/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:24:07.292285 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/
+-rw-rw-rw-   0        0        0    54417 2023-04-15 00:18:47.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/README.md
+-rw-rw-rw-   0        0        0    22528 2023-04-15 00:18:47.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-04-15 00:24:06.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/requirements.txt
+-rw-rw-rw-   0        0        0     5332 2023-04-15 00:24:06.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 00:24:07.295276 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc.egg-info/
+-rw-rw-rw-   0        0        0    55124 2023-04-15 00:24:07.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-15 00:24:07.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:24:07.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-15 00:24:07.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-15 00:24:07.000000 a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:24:07.297271 a_pandas_ex_easy_loc-0.15/setup.cfg
+-rw-rw-rw-   0        0        0     1606 2023-04-15 00:24:06.000000 a_pandas_ex_easy_loc-0.15/setup.py
```

### Comparing `a_pandas_ex_easy_loc-0.14/LICENSE.rst` & `a_pandas_ex_easy_loc-0.15/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.14/PKG-INFO` & `a_pandas_ex_easy_loc-0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a_pandas_ex_easy_loc
-Version: 0.14
+Version: 0.15
 Summary: Search and replace values with df.loc without Exceptions due to dtype incompatibility
 Home-page: https://github.com/hansalemaos/a_pandas_ex_easy_loc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: loc,iloc,df.at,df.iat,pandas,DataFrame,Series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `a_pandas_ex_easy_loc-0.14/README.md` & `a_pandas_ex_easy_loc-0.15/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/README.md` & `a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/__init__.py` & `a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/__init__.py`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/thirdparty.json` & `a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc/thirdparty.json`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/PKG-INFO` & `a_pandas_ex_easy_loc-0.15/a_pandas_ex_easy_loc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a-pandas-ex-easy-loc
-Version: 0.14
+Version: 0.15
 Summary: Search and replace values with df.loc without Exceptions due to dtype incompatibility
 Home-page: https://github.com/hansalemaos/a_pandas_ex_easy_loc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: loc,iloc,df.at,df.iat,pandas,DataFrame,Series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `a_pandas_ex_easy_loc-0.14/setup.py` & `a_pandas_ex_easy_loc-0.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.14'''
+VERSION = '''0.15'''
 DESCRIPTION = '''Search and replace values with df.loc without Exceptions due to dtype incompatibility'''
 
 # Setting up
 setup(
     name="a_pandas_ex_easy_loc",
     version=VERSION,
     license='MIT',
```

