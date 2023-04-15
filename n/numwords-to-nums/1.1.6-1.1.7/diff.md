# Comparing `tmp/numwords_to_nums-1.1.6.tar.gz` & `tmp/numwords_to_nums-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numwords_to_nums-1.1.6.tar", last modified: Sat Apr 15 11:31:38 2023, max compression
+gzip compressed data, was "numwords_to_nums-1.1.7.tar", last modified: Sat Apr 15 12:12:54 2023, max compression
```

## Comparing `numwords_to_nums-1.1.6.tar` & `numwords_to_nums-1.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/
--rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.6/LICENSE.md
--rw-rw-r--   0 user      (1000) user      (1000)     3874 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3332 2023-04-15 11:25:28.000000 numwords_to_nums-1.1.6/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/numwords_to_nums/
--rw-rw-r--   0 user      (1000) user      (1000)       48 2023-04-15 11:26:55.000000 numwords_to_nums-1.1.6/numwords_to_nums/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.6/numwords_to_nums/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)     8877 2023-04-15 11:25:28.000000 numwords_to_nums-1.1.6/numwords_to_nums/numwords_to_nums.py
--rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-04-15 11:21:14.000000 numwords_to_nums-1.1.6/numwords_to_nums/rules.py
--rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.6/numwords_to_nums/text_processing_helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     8808 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.6/numwords_to_nums/tokens_basic.py
--rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-04-15 11:21:04.000000 numwords_to_nums-1.1.6/numwords_to_nums/tokens_rules.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3874 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      467 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-15 11:31:38.000000 numwords_to_nums-1.1.6/numwords_to_nums.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      594 2023-04-15 11:28:30.000000 numwords_to_nums-1.1.6/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      571 2023-04-15 11:28:15.000000 numwords_to_nums-1.1.6/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 11:31:38.768583 numwords_to_nums-1.1.6/tests/
--rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.6/tests/test_numwords_to_nums.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 12:12:54.892295 numwords_to_nums-1.1.7/
+-rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.7/LICENSE.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3884 2023-04-15 12:12:54.892295 numwords_to_nums-1.1.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3342 2023-04-15 12:11:51.000000 numwords_to_nums-1.1.7/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 12:12:54.892295 numwords_to_nums-1.1.7/numwords_to_nums/
+-rw-rw-r--   0 user      (1000) user      (1000)       48 2023-04-15 12:12:29.000000 numwords_to_nums-1.1.7/numwords_to_nums/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.7/numwords_to_nums/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8877 2023-04-15 11:25:28.000000 numwords_to_nums-1.1.7/numwords_to_nums/numwords_to_nums.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-04-15 11:21:14.000000 numwords_to_nums-1.1.7/numwords_to_nums/rules.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.7/numwords_to_nums/text_processing_helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8808 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.7/numwords_to_nums/tokens_basic.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-04-15 11:21:04.000000 numwords_to_nums-1.1.7/numwords_to_nums/tokens_rules.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 12:12:54.892295 numwords_to_nums-1.1.7/numwords_to_nums.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3884 2023-04-15 12:12:54.000000 numwords_to_nums-1.1.7/numwords_to_nums.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      467 2023-04-15 12:12:54.000000 numwords_to_nums-1.1.7/numwords_to_nums.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-15 12:12:54.000000 numwords_to_nums-1.1.7/numwords_to_nums.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-15 12:12:54.000000 numwords_to_nums-1.1.7/numwords_to_nums.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      594 2023-04-15 12:12:09.000000 numwords_to_nums-1.1.7/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-15 12:12:54.892295 numwords_to_nums-1.1.7/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2023-04-15 12:12:15.000000 numwords_to_nums-1.1.7/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 12:12:54.892295 numwords_to_nums-1.1.7/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.7/tests/test_numwords_to_nums.py
```

### Comparing `numwords_to_nums-1.1.6/LICENSE.md` & `numwords_to_nums-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.6/PKG-INFO` & `numwords_to_nums-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords_to_nums
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ```
 
 It can handle a variety of phrases. It also maintains ordinals such as first--> 1st and also supports negative numbers.
 
 ```
 "This is just a random sentence." -> 'This is just a random sentence.'
 "I am twenty five years old and my dad is 50 years old. I would like to get my father two cars!" -> 'I am 25 years old and my dad is 50 years old. I would like to get my father 2 cars!'
-"I was born in twenty ten" -> 'I was born in 1997'
+"I was born in nineteen ninety five" -> 'I was born in 1995'
 "The temperature of the room was minus seven so I had to turn on the heater." -> 'The temperature of the room was -7 so I had to turn on the heater.'
 "In the year twenty twenty one, the forty sixth President of the United States was inaugurated." -> 'In the year 2021, the 46th President of the United States was inaugurated.'
 "Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 78.'
 "He was elected in November twenty twenty after defeating the incumbent, Donald Trump." -> 'He was elected in November 2020 after defeating the incumbent, Donald Trump.'
 "Bidens inauguration took place on January twentieth, which marked the fifty ninth quadrennial presidential inauguration." -> 'Bidens inauguration took place on January 20th, which marked the 59th quadrennial presidential inauguration.'
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
```

### Comparing `numwords_to_nums-1.1.6/README.md` & `numwords_to_nums-1.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 
 It can handle a variety of phrases. It also maintains ordinals such as first--> 1st and also supports negative numbers.
 
 ```
 "This is just a random sentence." -> 'This is just a random sentence.'
 "I am twenty five years old and my dad is 50 years old. I would like to get my father two cars!" -> 'I am 25 years old and my dad is 50 years old. I would like to get my father 2 cars!'
-"I was born in twenty ten" -> 'I was born in 1997'
+"I was born in nineteen ninety five" -> 'I was born in 1995'
 "The temperature of the room was minus seven so I had to turn on the heater." -> 'The temperature of the room was -7 so I had to turn on the heater.'
 "In the year twenty twenty one, the forty sixth President of the United States was inaugurated." -> 'In the year 2021, the 46th President of the United States was inaugurated.'
 "Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 78.'
 "He was elected in November twenty twenty after defeating the incumbent, Donald Trump." -> 'He was elected in November 2020 after defeating the incumbent, Donald Trump.'
 "Bidens inauguration took place on January twentieth, which marked the fifty ninth quadrennial presidential inauguration." -> 'Bidens inauguration took place on January 20th, which marked the 59th quadrennial presidential inauguration.'
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
```

### Comparing `numwords_to_nums-1.1.6/numwords_to_nums/constants.py` & `numwords_to_nums-1.1.7/numwords_to_nums/constants.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.6/numwords_to_nums/numwords_to_nums.py` & `numwords_to_nums-1.1.7/numwords_to_nums/numwords_to_nums.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.6/numwords_to_nums/rules.py` & `numwords_to_nums-1.1.7/numwords_to_nums/rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.6/numwords_to_nums/text_processing_helpers.py` & `numwords_to_nums-1.1.7/numwords_to_nums/text_processing_helpers.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.6/numwords_to_nums/tokens_basic.py` & `numwords_to_nums-1.1.7/numwords_to_nums/tokens_basic.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.6/numwords_to_nums/tokens_rules.py` & `numwords_to_nums-1.1.7/numwords_to_nums/tokens_rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.6/numwords_to_nums.egg-info/PKG-INFO` & `numwords_to_nums-1.1.7/numwords_to_nums.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords-to-nums
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ```
 
 It can handle a variety of phrases. It also maintains ordinals such as first--> 1st and also supports negative numbers.
 
 ```
 "This is just a random sentence." -> 'This is just a random sentence.'
 "I am twenty five years old and my dad is 50 years old. I would like to get my father two cars!" -> 'I am 25 years old and my dad is 50 years old. I would like to get my father 2 cars!'
-"I was born in twenty ten" -> 'I was born in 1997'
+"I was born in nineteen ninety five" -> 'I was born in 1995'
 "The temperature of the room was minus seven so I had to turn on the heater." -> 'The temperature of the room was -7 so I had to turn on the heater.'
 "In the year twenty twenty one, the forty sixth President of the United States was inaugurated." -> 'In the year 2021, the 46th President of the United States was inaugurated.'
 "Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 78.'
 "He was elected in November twenty twenty after defeating the incumbent, Donald Trump." -> 'He was elected in November 2020 after defeating the incumbent, Donald Trump.'
 "Bidens inauguration took place on January twentieth, which marked the fifty ninth quadrennial presidential inauguration." -> 'Bidens inauguration took place on January 20th, which marked the 59th quadrennial presidential inauguration.'
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
```

### Comparing `numwords_to_nums-1.1.6/pyproject.toml` & `numwords_to_nums-1.1.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "numwords_to_nums"
-version = "1.1.6"
+version = "1.1.7"
 description = "Python library for converting numerical words (textual numbers) to numbers"
 readme = "README.md"
 authors = [{ name = "Sarthak", email = "sarthak6jan16@gmail.com" }, { name = "Arpit", email = "joshia296@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `numwords_to_nums-1.1.6/setup.py` & `numwords_to_nums-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='numwords_to_nums',
     packages=find_packages(include=['numwords_to_nums']),
-    version='1.1.6',
+    version='1.1.7',
     description='Python library for converting numerical words (textual numbers) to numbers',
     long_description="README.md",
     long_description_content_type="text/markdown",
     author='Sarthak, Arpit',
     author_email="sarthak6jan16@gmail.com , joshia296@gmail.com",
     license='MIT',
     install_requires=[],
```

### Comparing `numwords_to_nums-1.1.6/tests/test_numwords_to_nums.py` & `numwords_to_nums-1.1.7/tests/test_numwords_to_nums.py`

 * *Files identical despite different names*

