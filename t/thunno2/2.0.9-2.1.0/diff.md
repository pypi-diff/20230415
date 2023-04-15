# Comparing `tmp/thunno2-2.0.9.tar.gz` & `tmp/thunno2-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.0.9.tar", last modified: Fri Apr 14 19:09:18 2023, max compression
+gzip compressed data, was "thunno2-2.1.0.tar", last modified: Sat Apr 15 17:56:38 2023, max compression
```

## Comparing `thunno2-2.0.9.tar` & `thunno2-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 19:09:18.595983 thunno2-2.0.9/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 19:09:18.595862 thunno2-2.0.9/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-14 19:09:18.596019 thunno2-2.0.9/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.9/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 19:09:18.595187 thunno2-2.0.9/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.9/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.9/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    46659 2023-04-14 08:28:09.000000 thunno2-2.0.9/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.9/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.0.9/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:07:56.000000 thunno2-2.0.9/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    47961 2023-04-13 17:15:28.000000 thunno2-2.0.9/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    25799 2023-04-14 16:37:26.000000 thunno2-2.0.9/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    22283 2023-04-14 16:37:26.000000 thunno2-2.0.9/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-14 19:08:45.000000 thunno2-2.0.9/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    62646 2023-04-14 08:28:09.000000 thunno2-2.0.9/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.9/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-14 19:09:07.000000 thunno2-2.0.9/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 19:09:18.595713 thunno2-2.0.9/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-14 19:09:18.000000 thunno2-2.0.9/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-15 17:56:38.680179 thunno2-2.1.0/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-15 17:56:38.680056 thunno2-2.1.0/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-15 17:56:38.680237 thunno2-2.1.0/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.1.0/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-15 17:56:38.679022 thunno2-2.1.0/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.0/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.1.0/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    46735 2023-04-15 17:10:04.000000 thunno2-2.1.0/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2971 2023-04-15 15:28:56.000000 thunno2-2.1.0/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.1.0/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:12:18.000000 thunno2-2.1.0/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    48088 2023-04-15 17:10:04.000000 thunno2-2.1.0/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25876 2023-04-15 15:28:56.000000 thunno2-2.1.0/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    22512 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    62680 2023-04-15 17:10:04.000000 thunno2-2.1.0/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3274 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-15 17:55:44.000000 thunno2-2.1.0/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-15 17:56:38.679848 thunno2-2.1.0/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-15 17:56:38.000000 thunno2-2.1.0/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.0.9/PKG-INFO` & `thunno2-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.9
+Version: 2.1.0
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.9.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.0.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.0.9/setup.py` & `thunno2-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.9/thunno2/codepage.py` & `thunno2-2.1.0/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.9/thunno2/commands.py` & `thunno2-2.1.0/thunno2/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,18 @@
                         break
                 else:
                     if ctx.warnings:
                         print('TRACEBACK: [UNEXPECTED TYPE]', file=sys.stderr)
                         print('Got', (type(x), type(i)), file=sys.stderr)
         yield r
     else:
-        if not x:
+        if not (x + y):
+            if main:
+                yield []
+        elif not x:
             yield from y
         elif not y:
             yield from x
         else:
             if main:
                 yield list(recursively_distribute(x[0], y[0], dct, 0)) + list(
                     recursively_distribute(x[1:], y[1:], dct, 0))
@@ -812,16 +815,16 @@
         (str, str): string_add
     }, 2, ('add', 'plus')),
 
     '-': Overload(2, {
         (Number[0], Number[0]): subtract,
         (str, Number[0]): slice_start,
         (Number[0], str): slice_end,
-        (str, str): strip
-    }, 2, ('subtract', 'minus', 'strip')),
+        (str, str): replace_with_nothing
+    }, 2, ('subtract', 'minus')),
 
     '×': Overload(2, {
         (Number[0], Number[0]): multiply,
         (str, Number[0]): multiply,
         (Number[0], str): multiply,
         (str, str): string_cartesian_product
     }, 2, ('multiply', 'times')),
@@ -854,16 +857,16 @@
         (str, str): first_split3
     }, 2, ('floor_divide', 'integer_divide')),
 
     '_': Overload(2, {
         (Number[0], Number[0]): swapped_subtract,
         (str, Number[0]): slice_end2,
         (Number[0], str): slice_start2,
-        (str, str): strip2
-    }, 2, ('swapped_subtract', 'swapped_minus', 'swapped_strip')),
+        (str, str): replace_with_nothing2
+    }, 2, ('swapped_subtract', 'swapped_minus')),
 
     '\\': Overload(2, {
         (Number[0], Number[0]): swapped_divide,
         (str, Number[0]): split1,
         (Number[0], str): split2,
         (str, str): split4
     }, 2, ('swapped_divide', 'swapped_split')),
```

### Comparing `thunno2-2.0.9/thunno2/constants.py` & `thunno2-2.1.0/thunno2/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     'B': 'Buzz',
     'C': CODEPAGE,
     'D': '0123456789',
     'E': math.e,
     'F': 'Fizz',
     'G': (1 + 5 ** 0.5) / 2,
     'H': 'Hello, World!',
-    'I': datetime.datetime.now().microsecond,
-    'J': datetime.datetime.now().second,
-    'K': datetime.datetime.now().minute,
-    'L': datetime.datetime.now().hour,
-    'M': datetime.datetime.now().day,
-    'N': datetime.datetime.now().month,
-    'O': datetime.datetime.now().year,
+    'I': (lambda: datetime.datetime.now().microsecond),
+    'J': (lambda: datetime.datetime.now().second),
+    'K': (lambda: datetime.datetime.now().minute),
+    'L': (lambda: datetime.datetime.now().hour),
+    'M': (lambda: datetime.datetime.now().day),
+    'N': (lambda: datetime.datetime.now().month),
+    'O': (lambda: datetime.datetime.now().year),
     'P': math.pi,
-    'Q': str(datetime.datetime.now()).split('.')[0],
+    'Q': (lambda: str(datetime.datetime.now()).split('.')[0]),
     'R': '()[]{}',
     'S': '([{',
     'T': ')]}',
     'U': '([{<',
     'V': ')]}>',
     'W': 'AEIOU',
     'X': 'BCDFGHJKLMNPQRSTVWXYZ',
```

### Comparing `thunno2-2.0.9/thunno2/dictionary.py` & `thunno2-2.1.0/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.9/thunno2/flags.py` & `thunno2-2.1.0/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.9/thunno2/helpers.py` & `thunno2-2.1.0/thunno2/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,15 +705,15 @@
                 l.append(int(i))
             except:
                 try:
                     l.append(float(i))
                 except:
                     pass
     if not l:
-        return 0
+        return 1
     return math.prod(l)
 
 
 def ord_product(s):
     return math.prod(list(map(ord, s)))
 
 
@@ -819,15 +819,15 @@
 
 
 def slice_end(n, s):
     return s[:-n]
 
 
 def strip(a, b):
-    return b.strip(a)
+    return b.strip([a])
 
 
 def multiply(x, y):
     if isinstance(x, (str, list)):
         return x * int(y)
     elif isinstance(y, (str, list)):
         return int(x) * y
@@ -2546,7 +2546,15 @@
     return r
 
 
 def listify(x):
     if isinstance(x, (list, str)):
         return list(copy.deepcopy(x))
     return one_range(x)
+
+
+def replace_with_nothing(x, y):
+    return y.replace(x, '')
+
+
+def replace_with_nothing2(x, y):
+    return x.replace(y, '')
```

### Comparing `thunno2-2.0.9/thunno2/interpreter.py` & `thunno2-2.1.0/thunno2/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,16 @@
             if not isinstance(ga, list):
                 vars_dict['ga'] = [ga, a]
             vars_dict['ga'] = ga + [a]
         elif desc == 'stack':
             ctx.stack.push(list(ctx.stack).copy())
         elif desc == 'constant':
             ctx.stack.push(info)
+        elif desc == 'callable constant':
+            ctx.stack.push(info())
         elif desc == 'codepage compression':
             ctx.stack.push(info)
         elif desc == 'quit':
             raise TerminateProgramException()  # This will hopefully get caught and ignored
         elif desc == 'next input':
             if ctx.other_il:
                 ctx.stack.push(ctx.other_il[0])
```

### Comparing `thunno2-2.0.9/thunno2/lexer.py` & `thunno2-2.1.0/thunno2/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from thunno2.commands import commands, DIGRAPHS, get_a_function, Void
 from thunno2.constants import CONSTANTS
 from thunno2.codepage import codepage_index
 from thunno2.dictionary import dictionary_codepage
 
-
 """Splits Thunno 2 code into tokens to make it easier for the interpreter"""
 
 """Creative Commons Legal Code
 
 CC0 1.0 Universal
 
     CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -202,23 +201,23 @@
             index += 3
             x = code[index - 2: index + 1]
             try:
                 nxt = code[index + 1]
             except:
                 nxt = ''
             if (len(x) != 3) or (
-                (
-                    x[0] not in dictionary_codepage
-                ) or (
-                    x[1] not in dictionary_codepage
-                ) or (
-                    x[2] not in dictionary_codepage
-                ) or (
-                    nxt not in dictionary_codepage
-                )
+                    (
+                            x[0] not in dictionary_codepage
+                    ) or (
+                            x[1] not in dictionary_codepage
+                    ) or (
+                            x[2] not in dictionary_codepage
+                    ) or (
+                            nxt not in dictionary_codepage
+                    )
             ):
                 ret.append(('ʋ' + x, 'three characters', x))
             else:
                 index += 1
                 ret.append(('ʋ' + x + nxt, 'two words dictionary compression', x + nxt))
         elif char == '[':
             s = char
@@ -385,17 +384,17 @@
             ret.append((char, 'get x', 0))
         elif char == 'y':
             ret.append((char, 'get y', 0))
         elif char == 'X':
             ret.append((char, 'set x', 0))
         elif char == 'Y':
             ret.append((char, 'set y', 0))
-        elif char == 'ẋ':
+        elif char == 'Ẋ':
             ret.append((char, 'set x without popping', 0))
-        elif char == 'ẏ':
+        elif char == 'Ẏ':
             ret.append((char, 'set y without popping', 0))
         elif char == 'ẋ':
             ret.append((char, 'increment x', 0))
         elif char == 'ẏ':
             ret.append((char, 'increment y', 0))
         elif char == 'Ȥ':
             ret.append((char, 'get global array', 0))
@@ -404,15 +403,19 @@
         elif char == 'K':
             ret.append((char, 'stack', 0))
         elif char == 'k':
             index += 1
             try:
                 if code[index] in CONSTANTS:
                     x = code[index]
-                    ret.append((char + x, 'constant', CONSTANTS[x]))
+                    c = CONSTANTS[x]
+                    if type(c) == type(lambda: 0):
+                        ret.append((char + x, 'callable constant', c))
+                    else:
+                        ret.append((char + x, 'constant', c))
             except:
                 pass
         elif char == 'ṇ':
             index += 1
             try:
                 x = code[index]
                 ret.append((char + x, 'codepage compression', next(codepage_index(x)) + 101))
```

### Comparing `thunno2-2.0.9/thunno2/tests.py` & `thunno2-2.1.0/thunno2/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -829,15 +829,15 @@
 assert_eq(call('-', [1, 2, 3], [4, 5, 6]), [3, 3, 3])
 
 assert_eq(call('-', 2, 'abcde'), 'abc')
 assert_eq(call('-', [3, 4, 5], 'abcde'), ['ab', 'a', ''])
 assert_eq(call('-', 'abcde', 2), 'cde')
 assert_eq(call('-', 'abcde', [3, 4, 5]), ['de', 'e', ''])
 
-assert_eq(call('-', ['ab', 'bc'], 'abcbabc'), ['cbabc', 'abcba'])
+assert_eq(call('-', ['ab', 'bc'], 'abcbabc'), ['cbc', 'aba'])
 
 # ×
 
 assert_eq(call('×', 2.5, 2), 5.0)
 assert_eq(call('×', [1, 2, 3, 4, 5], 3), [3, 6, 9, 12, 15])
 
 assert_eq(call('×', 3, 'abc'), 'abcabcabc')
@@ -864,14 +864,16 @@
 assert_eq(call('*', [0.25, 0.5, 1, 2], 16), [2.0, 4.0, 16, 256])
 
 assert_eq(call('*', 5, 'abc'), 'abcaa')
 assert_eq(call('*', ['abc', 'defghi', ''], 4), ['abca', 'defghi', '    '])
 
 assert_eq(call('*', '\\d+', '123abcd7890'), ['123', '7890'])
 
+assert_eq(call('*', [], []), [])
+
 # %
 
 assert_eq(call('%', 3, 10), 1)
 assert_eq(call('%', [1, 2, 3, 4, 5], 13), [0, 1, 1, 1, 3])
 
 assert_eq(call('%', 123, 'abc%def'), 'abc123def')
 assert_eq(call('%', 'abc', ['123%456', '%%%', 'ab%c']), ['123abc456', 'abcabcabc', 'ababcc'])
@@ -894,15 +896,15 @@
 assert_eq(call('_', [1, 2, 3], [4, 5, 6]), [-3, -3, -3])
 
 assert_eq(call('_', 2, 'abcde'), 'cde')
 assert_eq(call('_', [3, 4, 5], 'abcde'), ['de', 'e', ''])
 assert_eq(call('_', 'abcde', 2), 'abc')
 assert_eq(call('_', 'abcde', [3, 4, 5]), ['ab', 'a', ''])
 
-assert_eq(call('_', ['ab', 'bc'], 'abcbabc'), ['', ''])
+assert_eq(call('_', ['ab', 'bc'], 'abcbabc'), ['ab', 'bc'])
 
 # \
 
 assert_eq(call('\\', 2, 1), 2.0)
 assert_eq(call('\\', [1, 2, 5, 10], 10), [0.1, 0.2, 0.5, 1.0])
 
 assert_eq(call('\\', 2, 'abcde'), ['abc', 'de'])
```

### Comparing `thunno2-2.0.9/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.0/thunno2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.9
+Version: 2.1.0
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.9.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.0.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

