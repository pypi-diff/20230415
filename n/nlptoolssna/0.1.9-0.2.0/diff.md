# Comparing `tmp/nlptoolssna-0.1.9.tar.gz` & `tmp/nlptoolssna-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.1.9.tar", last modified: Sat Apr 15 20:12:28 2023, max compression
+gzip compressed data, was "nlptoolssna-0.2.0.tar", last modified: Sat Apr 15 20:15:14 2023, max compression
```

## Comparing `nlptoolssna-0.1.9.tar` & `nlptoolssna-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.938059 nlptoolssna-0.1.9/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-15 20:12:28.938059 nlptoolssna-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.886129 nlptoolssna-0.1.9/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.892030 nlptoolssna-0.1.9/nlptools/
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.894146 nlptoolssna-0.1.9/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.1.9/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.910213 nlptoolssna-0.1.9/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.1.9/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.1.9/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.1.9/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     9655 2023-04-15 20:11:05.000000 nlptoolssna-0.1.9/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.1.9/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.1.9/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.914106 nlptoolssna-0.1.9/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.1.9/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.1.9/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.931228 nlptoolssna-0.1.9/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-15 20:12:28.000000 nlptoolssna-0.1.9/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-04-15 20:12:28.000000 nlptoolssna-0.1.9/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 20:12:28.000000 nlptoolssna-0.1.9/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-15 20:12:28.000000 nlptoolssna-0.1.9/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.1.9/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-04-15 20:12:28.000000 nlptoolssna-0.1.9/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 20:12:28.000000 nlptoolssna-0.1.9/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      403 2023-04-15 20:12:28.940031 nlptoolssna-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-04-15 20:12:19.000000 nlptoolssna-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 20:12:28.936109 nlptoolssna-0.1.9/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.1.9/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.396304 nlptoolssna-0.2.0/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-15 20:15:14.396304 nlptoolssna-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.348726 nlptoolssna-0.2.0/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.354638 nlptoolssna-0.2.0/nlptools/
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.357120 nlptoolssna-0.2.0/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.2.0/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.374453 nlptoolssna-0.2.0/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.2.0/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.2.0/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.2.0/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     9701 2023-04-15 20:15:05.000000 nlptoolssna-0.2.0/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.2.0/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.2.0/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.378363 nlptoolssna-0.2.0/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.2.0/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.2.0/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.391193 nlptoolssna-0.2.0/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-15 20:15:14.000000 nlptoolssna-0.2.0/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-04-15 20:15:14.000000 nlptoolssna-0.2.0/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 20:15:14.000000 nlptoolssna-0.2.0/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-15 20:15:14.000000 nlptoolssna-0.2.0/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.2.0/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-04-15 20:15:14.000000 nlptoolssna-0.2.0/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 20:15:14.000000 nlptoolssna-0.2.0/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      403 2023-04-15 20:15:14.397298 nlptoolssna-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1583 2023-04-15 20:14:50.000000 nlptoolssna-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 20:15:14.394350 nlptoolssna-0.2.0/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.2.0/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.1.9/CONTRIBUTING.rst` & `nlptoolssna-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/LICENSE` & `nlptoolssna-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/PKG-INFO` & `nlptoolssna-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.9/README.rst` & `nlptoolssna-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/docs/Makefile` & `nlptoolssna-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/docs/conf.py` & `nlptoolssna-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/docs/installation.rst` & `nlptoolssna-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/docs/make.bat` & `nlptoolssna-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/nlptools/data/my_data.pickle` & `nlptoolssna-0.2.0/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/nlptools/morph/charsets.py` & `nlptoolssna-0.2.0/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.2.0/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.2.0/nlptools/morph/morph_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,49 +40,49 @@
 
     except FileNotFoundError as e:
         print(f"File not found: {url}")
         raise e
     except pickle.UnpicklingError as e:
         print("Error while unpickling the data.")
         raise e
-def load_ALMA_dic(file):
-    """
-    Load the ALMA dictionary from a binary pickle file.
-
-    Args:
-    - file_path: str - The path of the binary pickle file containing the ALMA dictionary.
-
-    Returns:
-    - dict: A dictionary containing the ALMA dictionary data.
-
-    Raises:
-    - FileNotFoundError: If the file specified in file_path cannot be found.
-    - pickle.UnpicklingError: If an error occurred while unpickling the data.
-    """
-    # URL of the .pickle file on GitHub
-    #url = 'https://github.com/eng-aomar/ts/blob/main/my_data.pickle'
-    data_folder = os.path.join("nlptoos", "data")
-
-    file_to_open = os.path.join(data_folder, file)
-    try:
-        # Download the file from the URL
-        #response = requests.get(url)
-        #data = response.content
-        #Load the data from the file into a Python object
-        #data = pickle.loads(response.content)
-        with open(file_to_open, 'rb') as f:
-            ALMA_dic = pickle.load(f)
-        #my_dict = pickle.loads(data)
-        return ALMA_dic
-    except FileNotFoundError as e:
-        print(f"File not found: {file_to_open}")
-        raise e
-    except pickle.UnpicklingError as e:
-        print("Error while unpickling the data.")
-        raise e
+# def load_ALMA_dic(file):
+#     """
+#     Load the ALMA dictionary from a binary pickle file.
+
+#     Args:
+#     - file_path: str - The path of the binary pickle file containing the ALMA dictionary.
+
+#     Returns:
+#     - dict: A dictionary containing the ALMA dictionary data.
+
+#     Raises:
+#     - FileNotFoundError: If the file specified in file_path cannot be found.
+#     - pickle.UnpicklingError: If an error occurred while unpickling the data.
+#     """
+#     # URL of the .pickle file on GitHub
+#     #url = 'https://github.com/eng-aomar/ts/blob/main/my_data.pickle'
+#     data_folder = os.path.join("nlptoos", "data")
+
+#     file_to_open = os.path.join(data_folder, file)
+#     try:
+#         # Download the file from the URL
+#         #response = requests.get(url)
+#         #data = response.content
+#         #Load the data from the file into a Python object
+#         #data = pickle.loads(response.content)
+#         with open(file_to_open, 'rb') as f:
+#             ALMA_dic = pickle.load(f)
+#         #my_dict = pickle.loads(data)
+#         return ALMA_dic
+#     except FileNotFoundError as e:
+#         print(f"File not found: {file_to_open}")
+#         raise e
+#     except pickle.UnpicklingError as e:
+#         print("Error while unpickling the data.")
+#         raise e
 
 def tag(word, lang, task):
     """
     given a token, this method retrives the possible morphological solutions (lemma, pos, and frequency) filterd by spesific
     language and task.
      
        in a dictionary to find its lemma, part of speech, and frequency,
@@ -219,15 +219,15 @@
         list: A list of lists, where each sublist contains information about a word in the input sentence, including 
               the original word, its lemma, its part of speech (POS) tag, and its lemma frequency.
     """
     
     # Check if the ALMA dictionary has been loaded
     if settings.flag == True:
         settings.flag = False
-    settings.div_dic = load_ALMA_dic('my_data.pickle')
+    settings.div_dic = load_ALMA_dic()
    
     
     # Perform lemmatization on the input sentence
     output_list = lemmatize_sentence(text,lang, task)
     
     # Return the list of lemmatized words
     return output_list
```

### Comparing `nlptoolssna-0.1.9/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.2.0/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/nlptools/parse/parser.py` & `nlptoolssna-0.2.0/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.2.0/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.1.9/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.2.0/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.1.9/setup.py` & `nlptoolssna-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     include_package_data=True,
     keywords='nlptools',
     name='nlptoolssna',
     packages=find_packages(include=['nlptools', 'nlptools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/nlptools',
-    version='0.1.9',
+    version='0.2.0',
     zip_safe=False,
 )
```

