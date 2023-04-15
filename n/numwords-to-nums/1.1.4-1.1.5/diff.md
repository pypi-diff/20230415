# Comparing `tmp/numwords_to_nums-1.1.4.tar.gz` & `tmp/numwords_to_nums-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numwords_to_nums-1.1.4.tar", last modified: Sat Apr 15 07:36:13 2023, max compression
+gzip compressed data, was "numwords_to_nums-1.1.5.tar", last modified: Sat Apr 15 09:05:39 2023, max compression
```

## Comparing `numwords_to_nums-1.1.4.tar` & `numwords_to_nums-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/
--rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.4/LICENSE.md
--rw-rw-r--   0 user      (1000) user      (1000)     3790 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3248 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.4/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.097134 numwords_to_nums-1.1.4/numwords_to_nums/
--rw-rw-r--   0 user      (1000) user      (1000)       48 2023-04-15 07:33:00.000000 numwords_to_nums-1.1.4/numwords_to_nums/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.4/numwords_to_nums/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)     8871 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.4/numwords_to_nums/numwords_to_nums.py
--rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-04-15 07:27:00.000000 numwords_to_nums-1.1.4/numwords_to_nums/rules.py
--rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.4/numwords_to_nums/text_processing_helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     8808 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.4/numwords_to_nums/tokens_basic.py
--rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-04-15 07:27:13.000000 numwords_to_nums-1.1.4/numwords_to_nums/tokens_rules.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3790 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      467 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      594 2023-04-15 07:32:18.000000 numwords_to_nums-1.1.4/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      571 2023-04-15 07:32:09.000000 numwords_to_nums-1.1.4/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/tests/
--rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.4/tests/test_numwords_to_nums.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/
+-rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.5/LICENSE.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3800 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3258 2023-04-15 07:48:59.000000 numwords_to_nums-1.1.5/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/numwords_to_nums/
+-rw-rw-r--   0 user      (1000) user      (1000)       48 2023-04-15 09:05:04.000000 numwords_to_nums-1.1.5/numwords_to_nums/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.5/numwords_to_nums/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8871 2023-04-15 09:03:37.000000 numwords_to_nums-1.1.5/numwords_to_nums/numwords_to_nums.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-04-15 09:02:47.000000 numwords_to_nums-1.1.5/numwords_to_nums/rules.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.5/numwords_to_nums/text_processing_helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8808 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.5/numwords_to_nums/tokens_basic.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-04-15 09:02:38.000000 numwords_to_nums-1.1.5/numwords_to_nums/tokens_rules.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3800 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      467 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      594 2023-04-15 09:04:49.000000 numwords_to_nums-1.1.5/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2023-04-15 09:04:57.000000 numwords_to_nums-1.1.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.5/tests/test_numwords_to_nums.py
```

### Comparing `numwords_to_nums-1.1.4/LICENSE.md` & `numwords_to_nums-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.4/PKG-INFO` & `numwords_to_nums-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords_to_nums
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 ```
 
 ## Usage
 Python 3 only!
 ```
 from numwords_to_nums.numwords_to_nums import NumWordsToNum
 num = NumWordsToNum()
-num.numwords_to_nums("twenty ten and twenty one")
+num.numerical_words_to_numbers("twenty ten and twenty one")
 > 2010 and 21
 
 To use our operator converter 
 num = NumWordsToNum()
 text = "one point two plus two"
 num.numerical_words_to_numbers(text, convert_operator = True)
 > 1.2+2
```

### Comparing `numwords_to_nums-1.1.4/README.md` & `numwords_to_nums-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ```
 
 ## Usage
 Python 3 only!
 ```
 from numwords_to_nums.numwords_to_nums import NumWordsToNum
 num = NumWordsToNum()
-num.numwords_to_nums("twenty ten and twenty one")
+num.numerical_words_to_numbers("twenty ten and twenty one")
 > 2010 and 21
 
 To use our operator converter 
 num = NumWordsToNum()
 text = "one point two plus two"
 num.numerical_words_to_numbers(text, convert_operator = True)
 > 1.2+2
```

### Comparing `numwords_to_nums-1.1.4/numwords_to_nums/constants.py` & `numwords_to_nums-1.1.5/numwords_to_nums/constants.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.4/numwords_to_nums/numwords_to_nums.py` & `numwords_to_nums-1.1.5/numwords_to_nums/numwords_to_nums.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.4/numwords_to_nums/rules.py` & `numwords_to_nums-1.1.5/numwords_to_nums/rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.4/numwords_to_nums/text_processing_helpers.py` & `numwords_to_nums-1.1.5/numwords_to_nums/text_processing_helpers.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.4/numwords_to_nums/tokens_basic.py` & `numwords_to_nums-1.1.5/numwords_to_nums/tokens_basic.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.4/numwords_to_nums/tokens_rules.py` & `numwords_to_nums-1.1.5/numwords_to_nums/tokens_rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.4/numwords_to_nums.egg-info/PKG-INFO` & `numwords_to_nums-1.1.5/numwords_to_nums.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords-to-nums
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 ```
 
 ## Usage
 Python 3 only!
 ```
 from numwords_to_nums.numwords_to_nums import NumWordsToNum
 num = NumWordsToNum()
-num.numwords_to_nums("twenty ten and twenty one")
+num.numerical_words_to_numbers("twenty ten and twenty one")
 > 2010 and 21
 
 To use our operator converter 
 num = NumWordsToNum()
 text = "one point two plus two"
 num.numerical_words_to_numbers(text, convert_operator = True)
 > 1.2+2
```

### Comparing `numwords_to_nums-1.1.4/pyproject.toml` & `numwords_to_nums-1.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "numwords_to_nums"
-version = "1.1.4"
+version = "1.1.5"
 description = "Python library for converting numerical words (textual numbers) to numbers"
 readme = "README.md"
 authors = [{ name = "Sarthak", email = "sarthak6jan16@gmail.com" }, { name = "Arpit", email = "joshia296@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `numwords_to_nums-1.1.4/setup.py` & `numwords_to_nums-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='numwords_to_nums',
     packages=find_packages(include=['numwords_to_nums']),
-    version='1.1.4',
+    version='1.1.5',
     description='Python library for converting numerical words (textual numbers) to numbers',
     long_description="README.md",
     long_description_content_type="text/markdown",
     author='Sarthak, Arpit',
     author_email="sarthak6jan16@gmail.com , joshia296@gmail.com",
     license='MIT',
     install_requires=[],
```

### Comparing `numwords_to_nums-1.1.4/tests/test_numwords_to_nums.py` & `numwords_to_nums-1.1.5/tests/test_numwords_to_nums.py`

 * *Files identical despite different names*

