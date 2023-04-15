# Comparing `tmp/nlptoolssna-0.1.2.tar.gz` & `tmp/nlptoolssna-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.1.2.tar", last modified: Sat Apr 15 18:53:37 2023, max compression
+gzip compressed data, was "nlptoolssna-0.1.3.tar", last modified: Sat Apr 15 18:55:44 2023, max compression
```

## Comparing `nlptoolssna-0.1.2.tar` & `nlptoolssna-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:53:37.787810 nlptoolssna-0.1.2/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-15 18:53:37.788825 nlptoolssna-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 18:53:37.733628 nlptoolssna-0.1.2/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 18:53:37.740466 nlptoolssna-0.1.2/nlptools/
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:53:37.756827 nlptoolssna-0.1.2/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.1.2/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.1.2/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2465 2023-04-15 18:50:13.000000 nlptoolssna-0.1.2/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     8259 2023-04-15 18:51:38.000000 nlptoolssna-0.1.2/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.1.2/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.1.2/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:53:37.762631 nlptoolssna-0.1.2/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.1.2/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.1.2/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:53:37.782184 nlptoolssna-0.1.2/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-15 18:53:37.000000 nlptoolssna-0.1.2/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      835 2023-04-15 18:53:37.000000 nlptoolssna-0.1.2/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:53:37.000000 nlptoolssna-0.1.2/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-15 18:53:37.000000 nlptoolssna-0.1.2/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.1.2/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-04-15 18:53:37.000000 nlptoolssna-0.1.2/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 18:53:37.000000 nlptoolssna-0.1.2/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      403 2023-04-15 18:53:37.791174 nlptoolssna-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-04-15 18:53:02.000000 nlptoolssna-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:53:37.786846 nlptoolssna-0.1.2/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.1.2/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:55:44.430280 nlptoolssna-0.1.3/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-15 18:55:44.431257 nlptoolssna-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 18:55:44.385257 nlptoolssna-0.1.3/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 18:55:44.392628 nlptoolssna-0.1.3/nlptools/
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:55:44.404856 nlptoolssna-0.1.3/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.1.3/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.1.3/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.1.3/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     8259 2023-04-15 18:51:38.000000 nlptoolssna-0.1.3/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.1.3/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.1.3/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:55:44.409254 nlptoolssna-0.1.3/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.1.3/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.1.3/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:55:44.425307 nlptoolssna-0.1.3/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-15 18:55:44.000000 nlptoolssna-0.1.3/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2023-04-15 18:55:44.000000 nlptoolssna-0.1.3/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:55:44.000000 nlptoolssna-0.1.3/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-15 18:55:44.000000 nlptoolssna-0.1.3/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.1.3/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-04-15 18:55:44.000000 nlptoolssna-0.1.3/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 18:55:44.000000 nlptoolssna-0.1.3/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      403 2023-04-15 18:55:44.432232 nlptoolssna-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-04-15 18:55:40.000000 nlptoolssna-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:55:44.429355 nlptoolssna-0.1.3/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.1.3/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.1.2/CONTRIBUTING.rst` & `nlptoolssna-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/LICENSE` & `nlptoolssna-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/PKG-INFO` & `nlptoolssna-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.2/README.rst` & `nlptoolssna-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/docs/Makefile` & `nlptoolssna-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/docs/conf.py` & `nlptoolssna-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/docs/installation.rst` & `nlptoolssna-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/docs/make.bat` & `nlptoolssna-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/nlptools/morph/charsets.py` & `nlptoolssna-0.1.3/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.1.3/nlptools/morph/lemmatizeSentence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from tokenizers_words import simple_word_tokenize
-from morph import settings
+from nlptools.morph.tokenizers_words import simple_word_tokenize
+from nlptools.morph import settings
 import re
 
 def lemmatize_word(word):
    word = word.strip()
    solution = [word,word+"_0",""]
    # word_undiac = re.sub('[َّ؞ٝٞﱢۚۙ ۭ۠ﱠۡ ۦ ّْـ]+', '',word)
    word_undiac = re.sub(r'[\u064B-\u0650]+', '',word) # Remove all Arabic diacretics [ ًَ]
```

### Comparing `nlptoolssna-0.1.2/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.1.3/nlptools/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.1.3/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/nlptools/parse/parser.py` & `nlptoolssna-0.1.3/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.1.3/nlptoolssna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.2/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.1.3/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.2/setup.py` & `nlptoolssna-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     include_package_data=True,
     keywords='nlptools',
     name='nlptoolssna',
     packages=find_packages(include=['nlptools', 'nlptools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/nlptools',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

