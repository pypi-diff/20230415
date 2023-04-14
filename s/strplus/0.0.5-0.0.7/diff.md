# Comparing `tmp/strplus-0.0.5.tar.gz` & `tmp/strplus-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-0.0.5.tar", max compression
+gzip compressed data, was "strplus-0.0.7.tar", max compression
```

## Comparing `strplus-0.0.5.tar` & `strplus-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-0.0.5/LICENSE
--rw-r--r--   0        0        0     2348 2023-04-14 19:36:57.172317 strplus-0.0.5/README.md
--rw-r--r--   0        0        0      672 2023-04-14 19:37:09.612313 strplus-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      160 2023-04-14 07:41:30.953611 strplus-0.0.5/strplus/__init__.py
--rw-r--r--   0        0        0     1773 2023-04-14 18:34:33.673438 strplus-0.0.5/strplus/cases.py
--rw-r--r--   0        0        0       27 2023-04-14 19:22:40.562574 strplus-0.0.5/strplus/functions.py
--rw-r--r--   0        0        0      807 2023-04-14 19:29:33.032449 strplus-0.0.5/strplus/strplus.py
--rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 strplus-0.0.5/setup.py
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 strplus-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2348 2023-04-14 19:36:57.172317 strplus-0.0.7/README.md
+-rw-r--r--   0        0        0      672 2023-04-14 23:02:53.571036 strplus-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-14 07:41:30.953611 strplus-0.0.7/strplus/__init__.py
+-rw-r--r--   0        0        0     2749 2023-04-14 19:54:07.942014 strplus-0.0.7/strplus/cases.py
+-rw-r--r--   0        0        0      548 2023-04-14 20:50:24.051003 strplus-0.0.7/strplus/functions.py
+-rw-r--r--   0        0        0     1137 2023-04-14 23:01:10.671058 strplus-0.0.7/strplus/strplus.py
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 strplus-0.0.7/setup.py
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 strplus-0.0.7/PKG-INFO
```

### Comparing `strplus-0.0.5/LICENSE` & `strplus-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-0.0.5/README.md` & `strplus-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `strplus-0.0.5/pyproject.toml` & `strplus-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "0.0.5"
+version = "0.0.7"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-0.0.5/setup.py` & `strplus-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '0.0.5',
+    'version': '0.0.7',
     'description': 'Python extra functions for strings',
     'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n```\nfrom strplus import Str\ns = Str("hello")\nassert s.upper() == "HELLO"\n```\n\n<br>\n<br>\n<br>\n<br>\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/under_construction.gif" width="300" />\n</a>\n\n<br>\n<br>\n<br>\n\n\n![](https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/20230414_203231_image.png)\n\n\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'0.0.5', 'description': 'Python extra functions for strings',
+'0.0.7', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n
 \n
 \n\n\n[img]\n\n\n
```

### Comparing `strplus-0.0.5/PKG-INFO` & `strplus-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 0.0.5
+Version: 0.0.7
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 0.0.5 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 0.0.7 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.9,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown [Wise_Up_Data's
```

