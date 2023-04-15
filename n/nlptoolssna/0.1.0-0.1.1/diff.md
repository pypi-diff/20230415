# Comparing `tmp/nlptoolssna-0.1.0.tar.gz` & `tmp/nlptoolssna-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.1.0.tar", last modified: Sat Apr 15 18:40:32 2023, max compression
+gzip compressed data, was "nlptoolssna-0.1.1.tar", last modified: Sat Apr 15 18:46:46 2023, max compression
```

## Comparing `nlptoolssna-0.1.0.tar` & `nlptoolssna-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:40:32.619154 nlptoolssna-0.1.0/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-15 18:40:32.619154 nlptoolssna-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 18:40:32.584095 nlptoolssna-0.1.0/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 18:40:32.588941 nlptoolssna-0.1.0/nlptools/
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:40:32.599123 nlptoolssna-0.1.0/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.1.0/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.1.0/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2767 2023-04-15 18:33:54.000000 nlptoolssna-0.1.0/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     8217 2023-04-15 18:35:35.000000 nlptoolssna-0.1.0/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.1.0/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      574 2023-04-15 18:35:24.000000 nlptoolssna-0.1.0/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:40:32.603031 nlptoolssna-0.1.0/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.1.0/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.1.0/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:40:32.614269 nlptoolssna-0.1.0/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-15 18:40:32.000000 nlptoolssna-0.1.0/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      835 2023-04-15 18:40:32.000000 nlptoolssna-0.1.0/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:40:32.000000 nlptoolssna-0.1.0/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-15 18:40:32.000000 nlptoolssna-0.1.0/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.1.0/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-04-15 18:40:32.000000 nlptoolssna-0.1.0/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 18:40:32.000000 nlptoolssna-0.1.0/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      403 2023-04-15 18:40:32.621107 nlptoolssna-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-04-15 18:40:04.000000 nlptoolssna-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:40:32.618246 nlptoolssna-0.1.0/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.1.0/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:46:46.717627 nlptoolssna-0.1.1/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-15 18:46:46.718614 nlptoolssna-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 18:46:46.667442 nlptoolssna-0.1.1/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 18:46:46.674129 nlptoolssna-0.1.1/nlptools/
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:46:46.688434 nlptoolssna-0.1.1/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.1.1/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.1.1/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2767 2023-04-15 18:33:54.000000 nlptoolssna-0.1.1/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     8200 2023-04-15 18:46:15.000000 nlptoolssna-0.1.1/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.1.1/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      574 2023-04-15 18:35:24.000000 nlptoolssna-0.1.1/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:46:46.694328 nlptoolssna-0.1.1/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.1.1/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.1.1/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:46:46.712120 nlptoolssna-0.1.1/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-15 18:46:46.000000 nlptoolssna-0.1.1/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2023-04-15 18:46:46.000000 nlptoolssna-0.1.1/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:46:46.000000 nlptoolssna-0.1.1/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-15 18:46:46.000000 nlptoolssna-0.1.1/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.1.1/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-04-15 18:46:46.000000 nlptoolssna-0.1.1/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 18:46:46.000000 nlptoolssna-0.1.1/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      403 2023-04-15 18:46:46.720515 nlptoolssna-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-04-15 18:46:27.000000 nlptoolssna-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:46:46.716616 nlptoolssna-0.1.1/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.1.1/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.1.0/CONTRIBUTING.rst` & `nlptoolssna-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/LICENSE` & `nlptoolssna-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/PKG-INFO` & `nlptoolssna-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.0/README.rst` & `nlptoolssna-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/docs/Makefile` & `nlptoolssna-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/docs/conf.py` & `nlptoolssna-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/docs/installation.rst` & `nlptoolssna-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/docs/make.bat` & `nlptoolssna-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/nlptools/morph/charsets.py` & `nlptoolssna-0.1.1/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.1.1/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.1.1/nlptools/morph/morph_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
-from morph import settings 
+import settings 
 import re
 from lemmatizeSentence import lemmatize_sentence
-from morph.tokenizers_words import simple_word_tokenize
+from tokenizers_words import simple_word_tokenize
 from parse.parser import arStrip
 import requests
 
 def load_ALMA_dic():
     """
     Load the ALMA dictionary from a binary pickle file.
```

### Comparing `nlptoolssna-0.1.0/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.1.1/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/nlptools/parse/parser.py` & `nlptoolssna-0.1.1/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.1.1/nlptoolssna.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.0/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.1.1/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.0/setup.py` & `nlptoolssna-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     include_package_data=True,
     keywords='nlptools',
     name='nlptoolssna',
     packages=find_packages(include=['nlptools', 'nlptools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/nlptools',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

