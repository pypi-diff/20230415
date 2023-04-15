# Comparing `tmp/nlptoolssna-0.1.6.tar.gz` & `tmp/nlptoolssna-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.1.6.tar", last modified: Sat Apr 15 19:22:16 2023, max compression
+gzip compressed data, was "nlptoolssna-0.1.7.tar", last modified: Sat Apr 15 19:24:31 2023, max compression
```

## Comparing `nlptoolssna-0.1.6.tar` & `nlptoolssna-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.085019 nlptoolssna-0.1.6/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-15 19:22:16.085996 nlptoolssna-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.045650 nlptoolssna-0.1.6/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.049553 nlptoolssna-0.1.6/nlptools/
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.051507 nlptoolssna-0.1.6/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.1.6/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.063769 nlptoolssna-0.1.6/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.1.6/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.1.6/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.1.6/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     8400 2023-04-15 19:21:56.000000 nlptoolssna-0.1.6/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.1.6/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.1.6/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.066700 nlptoolssna-0.1.6/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.1.6/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.1.6/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.081113 nlptoolssna-0.1.6/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-15 19:22:15.000000 nlptoolssna-0.1.6/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-04-15 19:22:16.000000 nlptoolssna-0.1.6/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:22:15.000000 nlptoolssna-0.1.6/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-15 19:22:15.000000 nlptoolssna-0.1.6/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.1.6/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-04-15 19:22:15.000000 nlptoolssna-0.1.6/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 19:22:15.000000 nlptoolssna-0.1.6/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      403 2023-04-15 19:22:16.087182 nlptoolssna-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-04-15 19:22:04.000000 nlptoolssna-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:22:16.084062 nlptoolssna-0.1.6/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.1.6/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.694509 nlptoolssna-0.1.7/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-15 19:24:31.695009 nlptoolssna-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.650196 nlptoolssna-0.1.7/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.655640 nlptoolssna-0.1.7/nlptools/
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.657668 nlptoolssna-0.1.7/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.1.7/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.670524 nlptoolssna-0.1.7/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.1.7/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.1.7/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.1.7/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     8403 2023-04-15 19:24:15.000000 nlptoolssna-0.1.7/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.1.7/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.1.7/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.674432 nlptoolssna-0.1.7/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.1.7/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.1.7/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.689208 nlptoolssna-0.1.7/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-15 19:24:31.000000 nlptoolssna-0.1.7/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-04-15 19:24:31.000000 nlptoolssna-0.1.7/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:24:31.000000 nlptoolssna-0.1.7/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-15 19:24:31.000000 nlptoolssna-0.1.7/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.1.7/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-04-15 19:24:31.000000 nlptoolssna-0.1.7/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 19:24:31.000000 nlptoolssna-0.1.7/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      403 2023-04-15 19:24:31.696008 nlptoolssna-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1583 2023-04-15 19:24:26.000000 nlptoolssna-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:31.693113 nlptoolssna-0.1.7/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.1.7/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.1.6/CONTRIBUTING.rst` & `nlptoolssna-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/LICENSE` & `nlptoolssna-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/PKG-INFO` & `nlptoolssna-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.6/README.rst` & `nlptoolssna-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/docs/Makefile` & `nlptoolssna-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/docs/conf.py` & `nlptoolssna-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/docs/installation.rst` & `nlptoolssna-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/docs/make.bat` & `nlptoolssna-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/nlptools/data/my_data.pickle` & `nlptoolssna-0.1.7/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/nlptools/morph/charsets.py` & `nlptoolssna-0.1.7/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.1.7/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.1.7/nlptools/morph/morph_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         #Load the data from the file into a Python object
         #data = pickle.loads(response.content)
         with open(file_to_open, 'rb') as f:
             ALMA_dic = pickle.load(f)
         #my_dict = pickle.loads(data)
         return ALMA_dic
     except FileNotFoundError as e:
-        print(f"File not found: {file_path}")
+        print(f"File not found: {file_to_open}")
         raise e
     except pickle.UnpicklingError as e:
         print("Error while unpickling the data.")
         raise e
 
 def tag(word, lang, task):
     """
```

### Comparing `nlptoolssna-0.1.6/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.1.7/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/nlptools/parse/parser.py` & `nlptoolssna-0.1.7/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.1.7/nlptoolssna.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.6/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.1.7/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.6/setup.py` & `nlptoolssna-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     include_package_data=True,
     keywords='nlptools',
     name='nlptoolssna',
     packages=find_packages(include=['nlptools', 'nlptools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/nlptools',
-    version='0.1.6',
+    version='0.1.7',
     zip_safe=False,
 )
```

