# Comparing `tmp/numwords_to_nums-1.1.5.tar.gz` & `tmp/numwords_to_nums-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numwords_to_nums-1.1.5.tar", last modified: Sat Apr 15 09:05:39 2023, max compression
+gzip compressed data, was "numwords_to_nums-1.1.6.tar", last modified: Sat Apr 15 11:31:38 2023, max compression
```

## Comparing `numwords_to_nums-1.1.5.tar` & `numwords_to_nums-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/
--rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.5/LICENSE.md
--rw-rw-r--   0 user      (1000) user      (1000)     3800 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3258 2023-04-15 07:48:59.000000 numwords_to_nums-1.1.5/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/numwords_to_nums/
--rw-rw-r--   0 user      (1000) user      (1000)       48 2023-04-15 09:05:04.000000 numwords_to_nums-1.1.5/numwords_to_nums/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.5/numwords_to_nums/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)     8871 2023-04-15 09:03:37.000000 numwords_to_nums-1.1.5/numwords_to_nums/numwords_to_nums.py
--rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-04-15 09:02:47.000000 numwords_to_nums-1.1.5/numwords_to_nums/rules.py
--rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.5/numwords_to_nums/text_processing_helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     8808 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.5/numwords_to_nums/tokens_basic.py
--rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-04-15 09:02:38.000000 numwords_to_nums-1.1.5/numwords_to_nums/tokens_rules.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3800 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      467 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-15 09:05:39.000000 numwords_to_nums-1.1.5/numwords_to_nums.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      594 2023-04-15 09:04:49.000000 numwords_to_nums-1.1.5/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      571 2023-04-15 09:04:57.000000 numwords_to_nums-1.1.5/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 09:05:39.580671 numwords_to_nums-1.1.5/tests/
--rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.5/tests/test_numwords_to_nums.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/
+-rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.6/LICENSE.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3874 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3332 2023-04-15 11:25:28.000000 numwords_to_nums-1.1.6/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/numwords_to_nums/
+-rw-rw-r--   0 user      (1000) user      (1000)       48 2023-04-15 11:26:55.000000 numwords_to_nums-1.1.6/numwords_to_nums/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.6/numwords_to_nums/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8877 2023-04-15 11:25:28.000000 numwords_to_nums-1.1.6/numwords_to_nums/numwords_to_nums.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-04-15 11:21:14.000000 numwords_to_nums-1.1.6/numwords_to_nums/rules.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.6/numwords_to_nums/text_processing_helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8808 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.6/numwords_to_nums/tokens_basic.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-04-15 11:21:04.000000 numwords_to_nums-1.1.6/numwords_to_nums/tokens_rules.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3874 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      467 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      594 2023-04-15 11:28:30.000000 numwords_to_nums-1.1.6/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2023-04-15 11:28:15.000000 numwords_to_nums-1.1.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.6/tests/test_numwords_to_nums.py
```

### Comparing `numwords_to_nums-1.1.5/LICENSE.md` & `numwords_to_nums-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.5/PKG-INFO` & `numwords_to_nums-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords_to_nums
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -52,18 +52,20 @@
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
 "three forty five" -> '345'
 "one point two plus two" -> '1.2+2'  (To use this make sure to use flag (convert_operator = True))
 "one point two plus two" -> '3.2' (To use this make sure to use evaluate function)
 "zero point five plus zero point five" -> '0.5+0.5'
 "zero point five plus zero point five" -> '1.0'
+"Please calculate 24-34+50*70" -> '3490'
 ```
 
 I find this useful if converting audio to text and have to convert the text to digits, operators, numerical expressions as well as evaluating them.
 It also find it helpful when converting ordinals to numbers as it maintains the suffix.
 
 ## Improvements/Issues
+- Complex arithmetic operations.
 - Please email us if you find any issues.
 
 ## Acknowledgements
 I have heavily used code from the SO answers from here: https://stackoverflow.com/questions/493174/is-there-a-way-to-convert-number-words-to-integers
 and improved upon them
```

### Comparing `numwords_to_nums-1.1.5/README.md` & `numwords_to_nums-1.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,20 @@
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
 "three forty five" -> '345'
 "one point two plus two" -> '1.2+2'  (To use this make sure to use flag (convert_operator = True))
 "one point two plus two" -> '3.2' (To use this make sure to use evaluate function)
 "zero point five plus zero point five" -> '0.5+0.5'
 "zero point five plus zero point five" -> '1.0'
+"Please calculate 24-34+50*70" -> '3490'
 ```
 
 I find this useful if converting audio to text and have to convert the text to digits, operators, numerical expressions as well as evaluating them.
 It also find it helpful when converting ordinals to numbers as it maintains the suffix.
 
 ## Improvements/Issues
+- Complex arithmetic operations.
 - Please email us if you find any issues.
 
 ## Acknowledgements
 I have heavily used code from the SO answers from here: https://stackoverflow.com/questions/493174/is-there-a-way-to-convert-number-words-to-integers
 and improved upon them
```

### Comparing `numwords_to_nums-1.1.5/numwords_to_nums/constants.py` & `numwords_to_nums-1.1.6/numwords_to_nums/constants.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.5/numwords_to_nums/numwords_to_nums.py` & `numwords_to_nums-1.1.6/numwords_to_nums/numwords_to_nums.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,16 @@
         expr_text = ''.join(re.findall("[\d\W]", et))
         # Clean new line, tab and space characters
         expr_text = ''.join(re.findall("[\S]", expr_text))
         # clean extra special character at the end
         expr_text = re.sub(r'[^\w\s]+$', '', expr_text)
 
         result = None
-        if re.compile(r'^\d*\s*[\+\-\*\/√%]\s*\d+$').match(expr_text) or re.compile(
-                r'^\d*[.]*\d*\s*[\+\-\*\/√%]\s*\d*[.]*\d+$').match(expr_text):
+        if re.compile(r'^\d+(\s*[\+\-\*\/√%]\s*\d+)+$').match(expr_text) or re.compile(
+                r'^\d*[.]*\d+(\s*[\+\-\*\/√%]\s*\d*[.]*\d+)+$').match(expr_text):
             try:
                 result = eval(expr_text)
             except Exception as e:
                 result = f" The answer is undefined. Evaluation error: {e}"
         return str(result)
```

### Comparing `numwords_to_nums-1.1.5/numwords_to_nums/rules.py` & `numwords_to_nums-1.1.6/numwords_to_nums/rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.5/numwords_to_nums/text_processing_helpers.py` & `numwords_to_nums-1.1.6/numwords_to_nums/text_processing_helpers.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.5/numwords_to_nums/tokens_basic.py` & `numwords_to_nums-1.1.6/numwords_to_nums/tokens_basic.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.5/numwords_to_nums/tokens_rules.py` & `numwords_to_nums-1.1.6/numwords_to_nums/tokens_rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.5/numwords_to_nums.egg-info/PKG-INFO` & `numwords_to_nums-1.1.6/numwords_to_nums.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords-to-nums
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -52,18 +52,20 @@
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
 "three forty five" -> '345'
 "one point two plus two" -> '1.2+2'  (To use this make sure to use flag (convert_operator = True))
 "one point two plus two" -> '3.2' (To use this make sure to use evaluate function)
 "zero point five plus zero point five" -> '0.5+0.5'
 "zero point five plus zero point five" -> '1.0'
+"Please calculate 24-34+50*70" -> '3490'
 ```
 
 I find this useful if converting audio to text and have to convert the text to digits, operators, numerical expressions as well as evaluating them.
 It also find it helpful when converting ordinals to numbers as it maintains the suffix.
 
 ## Improvements/Issues
+- Complex arithmetic operations.
 - Please email us if you find any issues.
 
 ## Acknowledgements
 I have heavily used code from the SO answers from here: https://stackoverflow.com/questions/493174/is-there-a-way-to-convert-number-words-to-integers
 and improved upon them
```

### Comparing `numwords_to_nums-1.1.5/pyproject.toml` & `numwords_to_nums-1.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "numwords_to_nums"
-version = "1.1.5"
+version = "1.1.6"
 description = "Python library for converting numerical words (textual numbers) to numbers"
 readme = "README.md"
 authors = [{ name = "Sarthak", email = "sarthak6jan16@gmail.com" }, { name = "Arpit", email = "joshia296@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `numwords_to_nums-1.1.5/setup.py` & `numwords_to_nums-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='numwords_to_nums',
     packages=find_packages(include=['numwords_to_nums']),
-    version='1.1.5',
+    version='1.1.6',
     description='Python library for converting numerical words (textual numbers) to numbers',
     long_description="README.md",
     long_description_content_type="text/markdown",
     author='Sarthak, Arpit',
     author_email="sarthak6jan16@gmail.com , joshia296@gmail.com",
     license='MIT',
     install_requires=[],
```

### Comparing `numwords_to_nums-1.1.5/tests/test_numwords_to_nums.py` & `numwords_to_nums-1.1.6/tests/test_numwords_to_nums.py`

 * *Files identical despite different names*

