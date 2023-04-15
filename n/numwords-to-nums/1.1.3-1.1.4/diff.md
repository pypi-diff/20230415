# Comparing `tmp/numwords_to_nums-1.1.3.tar.gz` & `tmp/numwords_to_nums-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numwords_to_nums-1.1.3.tar", last modified: Sun Feb 19 19:36:26 2023, max compression
+gzip compressed data, was "numwords_to_nums-1.1.4.tar", last modified: Sat Apr 15 07:36:13 2023, max compression
```

## Comparing `numwords_to_nums-1.1.3.tar` & `numwords_to_nums-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-02-19 19:36:26.242076 numwords_to_nums-1.1.3/
--rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.3/LICENSE.md
--rw-rw-r--   0 user      (1000) user      (1000)     3537 2023-02-19 19:36:26.242076 numwords_to_nums-1.1.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2995 2023-02-19 19:34:30.000000 numwords_to_nums-1.1.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-02-19 19:36:26.242076 numwords_to_nums-1.1.3/numwords_to_nums/
--rw-rw-r--   0 user      (1000) user      (1000)       48 2023-02-19 19:30:01.000000 numwords_to_nums-1.1.3/numwords_to_nums/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.3/numwords_to_nums/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)     8414 2023-02-19 18:21:39.000000 numwords_to_nums-1.1.3/numwords_to_nums/numwords_to_nums.py
--rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-02-19 18:23:06.000000 numwords_to_nums-1.1.3/numwords_to_nums/rules.py
--rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.3/numwords_to_nums/text_processing_helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     8625 2023-02-19 18:23:06.000000 numwords_to_nums-1.1.3/numwords_to_nums/tokens_basic.py
--rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-02-19 18:23:06.000000 numwords_to_nums-1.1.3/numwords_to_nums/tokens_rules.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-02-19 19:36:26.242076 numwords_to_nums-1.1.3/numwords_to_nums.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3537 2023-02-19 19:36:26.000000 numwords_to_nums-1.1.3/numwords_to_nums.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      467 2023-02-19 19:36:26.000000 numwords_to_nums-1.1.3/numwords_to_nums.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-02-19 19:36:26.000000 numwords_to_nums-1.1.3/numwords_to_nums.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-02-19 19:36:26.000000 numwords_to_nums-1.1.3/numwords_to_nums.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      594 2023-02-19 19:30:01.000000 numwords_to_nums-1.1.3/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-02-19 19:36:26.242076 numwords_to_nums-1.1.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      571 2023-02-19 19:30:01.000000 numwords_to_nums-1.1.3/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-02-19 19:36:26.242076 numwords_to_nums-1.1.3/tests/
--rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.3/tests/test_numwords_to_nums.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/
+-rw-rw-r--   0 user      (1000) user      (1000)     1071 2023-02-19 15:09:25.000000 numwords_to_nums-1.1.4/LICENSE.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3790 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3248 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.097134 numwords_to_nums-1.1.4/numwords_to_nums/
+-rw-rw-r--   0 user      (1000) user      (1000)       48 2023-04-15 07:33:00.000000 numwords_to_nums-1.1.4/numwords_to_nums/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      610 2023-02-19 13:30:24.000000 numwords_to_nums-1.1.4/numwords_to_nums/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8871 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.4/numwords_to_nums/numwords_to_nums.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8023 2023-04-15 07:27:00.000000 numwords_to_nums-1.1.4/numwords_to_nums/rules.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2430 2023-02-18 13:04:36.000000 numwords_to_nums-1.1.4/numwords_to_nums/text_processing_helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8808 2023-04-15 07:31:47.000000 numwords_to_nums-1.1.4/numwords_to_nums/tokens_basic.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-04-15 07:27:13.000000 numwords_to_nums-1.1.4/numwords_to_nums/tokens_rules.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3790 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      467 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-15 07:36:13.000000 numwords_to_nums-1.1.4/numwords_to_nums.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      594 2023-04-15 07:32:18.000000 numwords_to_nums-1.1.4/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2023-04-15 07:32:09.000000 numwords_to_nums-1.1.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-15 07:36:13.101133 numwords_to_nums-1.1.4/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-02-19 18:33:42.000000 numwords_to_nums-1.1.4/tests/test_numwords_to_nums.py
```

### Comparing `numwords_to_nums-1.1.3/LICENSE.md` & `numwords_to_nums-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.3/PKG-INFO` & `numwords_to_nums-1.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords_to_nums
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -34,33 +34,36 @@
 num = NumWordsToNum()
 text = "one point two plus two"
 result = num.numerical_words_to_numbers(text, convert_operator = True)
 num.evaluate(result)
 > 3.2
 ```
 
-It can handle a variety of phrases. It also maintains ordinals such as first--> 1st:
+It can handle a variety of phrases. It also maintains ordinals such as first--> 1st and also supports negative numbers.
 
 ```
 "This is just a random sentence." -> 'This is just a random sentence.'
 "I am twenty five years old and my dad is 50 years old. I would like to get my father two cars!" -> 'I am 25 years old and my dad is 50 years old. I would like to get my father 2 cars!'
 "I was born in twenty ten" -> 'I was born in 1997'
+"The temperature of the room was minus seven so I had to turn on the heater." -> 'The temperature of the room was -7 so I had to turn on the heater.'
 "In the year twenty twenty one, the forty sixth President of the United States was inaugurated." -> 'In the year 2021, the 46th President of the United States was inaugurated.'
-"Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 70 eight.'
+"Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 78.'
 "He was elected in November twenty twenty after defeating the incumbent, Donald Trump." -> 'He was elected in November 2020 after defeating the incumbent, Donald Trump.'
 "Bidens inauguration took place on January twentieth, which marked the fifty ninth quadrennial presidential inauguration." -> 'Bidens inauguration took place on January 20th, which marked the 59th quadrennial presidential inauguration.'
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
 "three forty five" -> '345'
 "one point two plus two" -> '1.2+2'  (To use this make sure to use flag (convert_operator = True))
 "one point two plus two" -> '3.2' (To use this make sure to use evaluate function)
+"zero point five plus zero point five" -> '0.5+0.5'
+"zero point five plus zero point five" -> '1.0'
 ```
 
 I find this useful if converting audio to text and have to convert the text to digits, operators, numerical expressions as well as evaluating them.
 It also find it helpful when converting ordinals to numbers as it maintains the suffix.
 
 ## Improvements/Issues
-- Need to add support for negative numbers example :- (minus seven)
+- Please email us if you find any issues.
 
 ## Acknowledgements
 I have heavily used code from the SO answers from here: https://stackoverflow.com/questions/493174/is-there-a-way-to-convert-number-words-to-integers
 and improved upon them
```

### Comparing `numwords_to_nums-1.1.3/README.md` & `numwords_to_nums-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,33 +21,36 @@
 num = NumWordsToNum()
 text = "one point two plus two"
 result = num.numerical_words_to_numbers(text, convert_operator = True)
 num.evaluate(result)
 > 3.2
 ```
 
-It can handle a variety of phrases. It also maintains ordinals such as first--> 1st:
+It can handle a variety of phrases. It also maintains ordinals such as first--> 1st and also supports negative numbers.
 
 ```
 "This is just a random sentence." -> 'This is just a random sentence.'
 "I am twenty five years old and my dad is 50 years old. I would like to get my father two cars!" -> 'I am 25 years old and my dad is 50 years old. I would like to get my father 2 cars!'
 "I was born in twenty ten" -> 'I was born in 1997'
+"The temperature of the room was minus seven so I had to turn on the heater." -> 'The temperature of the room was -7 so I had to turn on the heater.'
 "In the year twenty twenty one, the forty sixth President of the United States was inaugurated." -> 'In the year 2021, the 46th President of the United States was inaugurated.'
-"Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 70 eight.'
+"Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 78.'
 "He was elected in November twenty twenty after defeating the incumbent, Donald Trump." -> 'He was elected in November 2020 after defeating the incumbent, Donald Trump.'
 "Bidens inauguration took place on January twentieth, which marked the fifty ninth quadrennial presidential inauguration." -> 'Bidens inauguration took place on January 20th, which marked the 59th quadrennial presidential inauguration.'
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
 "three forty five" -> '345'
 "one point two plus two" -> '1.2+2'  (To use this make sure to use flag (convert_operator = True))
 "one point two plus two" -> '3.2' (To use this make sure to use evaluate function)
+"zero point five plus zero point five" -> '0.5+0.5'
+"zero point five plus zero point five" -> '1.0'
 ```
 
 I find this useful if converting audio to text and have to convert the text to digits, operators, numerical expressions as well as evaluating them.
 It also find it helpful when converting ordinals to numbers as it maintains the suffix.
 
 ## Improvements/Issues
-- Need to add support for negative numbers example :- (minus seven)
+- Please email us if you find any issues.
 
 ## Acknowledgements
 I have heavily used code from the SO answers from here: https://stackoverflow.com/questions/493174/is-there-a-way-to-convert-number-words-to-integers
 and improved upon them
```

### Comparing `numwords_to_nums-1.1.3/numwords_to_nums/constants.py` & `numwords_to_nums-1.1.4/numwords_to_nums/constants.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.3/numwords_to_nums/numwords_to_nums.py` & `numwords_to_nums-1.1.4/numwords_to_nums/numwords_to_nums.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,20 @@
                     if 'with' in expression_text:
                         expression_text = expression_text.replace(operator_word, '')
                         expression_text = expression_text.replace('with', operator_word)
 
                 valid_pattern = f'\d+ {operator_word} \d+'
                 operator_symbol = OPERATORS[operator_word]
 
-                if re.findall('(percent|square)', expression_text):
+                if (re.findall('minus', expression_text)) and (
+                re.findall(f' {operator_word} \d+', expression_text)) and not (
+                re.findall(valid_pattern, expression_text)):
+                    pattern = f'{operator_word}'
+                    expression_text = expression_text.replace(f'{pattern} ', operator_symbol)
+                elif re.findall('(percent|square)', expression_text):
                     pattern = f' {operator_word}' if 'percent' in expression_text else f'{operator_word} '
                     expression_text = expression_text.replace(pattern, operator_symbol)
                 elif re.findall(valid_pattern, expression_text):
                     expression_text = expression_text.replace(f' {operator_word} ', operator_symbol)
 
         return expression_text
 
@@ -157,14 +162,16 @@
 
     @staticmethod
     def evaluate(et):
         # Clean character other than numeric and math characters
         expr_text = ''.join(re.findall("[\d\W]", et))
         # Clean new line, tab and space characters
         expr_text = ''.join(re.findall("[\S]", expr_text))
+        # clean extra special character at the end
+        expr_text = re.sub(r'[^\w\s]+$', '', expr_text)
 
         result = None
         if re.compile(r'^\d*\s*[\+\-\*\/√%]\s*\d+$').match(expr_text) or re.compile(
                 r'^\d*[.]*\d*\s*[\+\-\*\/√%]\s*\d*[.]*\d+$').match(expr_text):
             try:
                 result = eval(expr_text)
             except Exception as e:
```

### Comparing `numwords_to_nums-1.1.3/numwords_to_nums/rules.py` & `numwords_to_nums-1.1.4/numwords_to_nums/rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.3/numwords_to_nums/text_processing_helpers.py` & `numwords_to_nums-1.1.4/numwords_to_nums/text_processing_helpers.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.3/numwords_to_nums/tokens_basic.py` & `numwords_to_nums-1.1.4/numwords_to_nums/tokens_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,17 @@
         """
 
         self.word_raw = word
         self.glue = glue
 
         # Basic preprocessing of the word to find the type
         self._word = word.lower().replace(',', '')
+        if re.match(r'^[^\w]+|\w+[^\w]+$', self._word):
+            # If there are special characters adjacent to the word
+            self._word = re.sub(r'[^\w\s]', '', self._word)
 
         # Try to match ordinal numbers and then treat them as cardinal ones
         self.ordinal_ending = None  # We need to keep a reference to the original ending in case the user wants to preserve it
         if self._word in Token.ORDINAL_WORDS:
             self.ordinal_ending = self._word[-2:]
             self._word = f'{Token.ORDINAL_WORDS[self._word]}_{self.ordinal_ending}'
```

### Comparing `numwords_to_nums-1.1.3/numwords_to_nums/tokens_rules.py` & `numwords_to_nums-1.1.4/numwords_to_nums/tokens_rules.py`

 * *Files identical despite different names*

### Comparing `numwords_to_nums-1.1.3/numwords_to_nums.egg-info/PKG-INFO` & `numwords_to_nums-1.1.4/numwords_to_nums.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numwords-to-nums
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python library for converting numerical words (textual numbers) to numbers
 Author: Sarthak, Arpit
 Author-email: Sarthak <sarthak6jan16@gmail.com>, Arpit <joshia296@gmail.com>
 Keywords: text2numbers,words2numbers,digits,numbers,ordinal numbers,evaluation,converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -34,33 +34,36 @@
 num = NumWordsToNum()
 text = "one point two plus two"
 result = num.numerical_words_to_numbers(text, convert_operator = True)
 num.evaluate(result)
 > 3.2
 ```
 
-It can handle a variety of phrases. It also maintains ordinals such as first--> 1st:
+It can handle a variety of phrases. It also maintains ordinals such as first--> 1st and also supports negative numbers.
 
 ```
 "This is just a random sentence." -> 'This is just a random sentence.'
 "I am twenty five years old and my dad is 50 years old. I would like to get my father two cars!" -> 'I am 25 years old and my dad is 50 years old. I would like to get my father 2 cars!'
 "I was born in twenty ten" -> 'I was born in 1997'
+"The temperature of the room was minus seven so I had to turn on the heater." -> 'The temperature of the room was -7 so I had to turn on the heater.'
 "In the year twenty twenty one, the forty sixth President of the United States was inaugurated." -> 'In the year 2021, the 46th President of the United States was inaugurated.'
-"Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 70 eight.'
+"Joe Biden became the oldest person to assume the presidency at the age of seventy eight." -> 'Joe Biden became the oldest person to assume the presidency at the age of 78.'
 "He was elected in November twenty twenty after defeating the incumbent, Donald Trump." -> 'He was elected in November 2020 after defeating the incumbent, Donald Trump.'
 "Bidens inauguration took place on January twentieth, which marked the fifty ninth quadrennial presidential inauguration." -> 'Bidens inauguration took place on January 20th, which marked the 59th quadrennial presidential inauguration.'
 "The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-nineteen pandemic." -> 'The event was held at the U.S. Capitol in Washington, D.C., and was attended by a limited number of people due to the COVID-19 pandemic.'
 "Despite the challenges, the fifty ninth presidential inauguration was a historic moment for the country." -> 'Despite the challenges, the 59th presidential inauguration was a historic moment for the country.'
 "three forty five" -> '345'
 "one point two plus two" -> '1.2+2'  (To use this make sure to use flag (convert_operator = True))
 "one point two plus two" -> '3.2' (To use this make sure to use evaluate function)
+"zero point five plus zero point five" -> '0.5+0.5'
+"zero point five plus zero point five" -> '1.0'
 ```
 
 I find this useful if converting audio to text and have to convert the text to digits, operators, numerical expressions as well as evaluating them.
 It also find it helpful when converting ordinals to numbers as it maintains the suffix.
 
 ## Improvements/Issues
-- Need to add support for negative numbers example :- (minus seven)
+- Please email us if you find any issues.
 
 ## Acknowledgements
 I have heavily used code from the SO answers from here: https://stackoverflow.com/questions/493174/is-there-a-way-to-convert-number-words-to-integers
 and improved upon them
```

### Comparing `numwords_to_nums-1.1.3/pyproject.toml` & `numwords_to_nums-1.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "numwords_to_nums"
-version = "1.1.3"
+version = "1.1.4"
 description = "Python library for converting numerical words (textual numbers) to numbers"
 readme = "README.md"
 authors = [{ name = "Sarthak", email = "sarthak6jan16@gmail.com" }, { name = "Arpit", email = "joshia296@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `numwords_to_nums-1.1.3/setup.py` & `numwords_to_nums-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='numwords_to_nums',
     packages=find_packages(include=['numwords_to_nums']),
-    version='1.1.3',
+    version='1.1.4',
     description='Python library for converting numerical words (textual numbers) to numbers',
     long_description="README.md",
     long_description_content_type="text/markdown",
     author='Sarthak, Arpit',
     author_email="sarthak6jan16@gmail.com , joshia296@gmail.com",
     license='MIT',
     install_requires=[],
```

### Comparing `numwords_to_nums-1.1.3/tests/test_numwords_to_nums.py` & `numwords_to_nums-1.1.4/tests/test_numwords_to_nums.py`

 * *Files identical despite different names*

