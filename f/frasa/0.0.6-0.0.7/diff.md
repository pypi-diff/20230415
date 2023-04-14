# Comparing `tmp/frasa-0.0.6.tar.gz` & `tmp/frasa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasa-0.0.6.tar", last modified: Fri Apr 14 22:40:52 2023, max compression
+gzip compressed data, was "frasa-0.0.7.tar", last modified: Fri Apr 14 22:46:09 2023, max compression
```

## Comparing `frasa-0.0.6.tar` & `frasa-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,58 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.054056 frasa-0.0.6/
--rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.0.6/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 22:40:52.053887 frasa-0.0.6/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     1700 2023-04-12 08:34:25.000000 frasa-0.0.6/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.047802 frasa-0.0.6/frasa/
--rw-r--r--   0 novay      (501) staff       (20)      514 2023-04-14 22:39:17.000000 frasa-0.0.6/frasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.048746 frasa-0.0.6/frasa/deteksi/
--rw-r--r--   0 novay      (501) staff       (20)      980 2023-04-14 16:03:46.000000 frasa-0.0.6/frasa/deteksi/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.049261 frasa-0.0.6/frasa/deteksi/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.0.6/frasa/deteksi/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.050208 frasa-0.0.6/frasa/deteksi/gender/
--rw-r--r--   0 novay      (501) staff       (20)      596 2023-04-14 11:05:42.000000 frasa-0.0.6/frasa/deteksi/gender/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     2712 2023-04-14 11:07:12.000000 frasa-0.0.6/frasa/deteksi/gender/classify.py
--rw-r--r--   0 novay      (501) staff       (20)      789 2023-04-14 10:06:04.000000 frasa-0.0.6/frasa/deteksi/gender/utils.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.051051 frasa-0.0.6/frasa/deteksi/plagiat/
--rw-r--r--   0 novay      (501) staff       (20)       68 2023-04-12 08:57:39.000000 frasa-0.0.6/frasa/deteksi/plagiat/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     3708 2023-04-12 09:03:02.000000 frasa-0.0.6/frasa/deteksi/plagiat/plagiat.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.052482 frasa-0.0.6/frasa/sensor/
--rw-r--r--   0 novay      (501) staff       (20)       45 2023-04-14 16:27:02.000000 frasa-0.0.6/frasa/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      433 2023-04-11 19:58:03.000000 frasa-0.0.6/frasa/sensor/constants.py
--rw-r--r--   0 novay      (501) staff       (20)     9277 2023-04-14 16:25:42.000000 frasa-0.0.6/frasa/sensor/sensor.py
--rw-r--r--   0 novay      (501) staff       (20)     1572 2023-04-11 19:56:18.000000 frasa-0.0.6/frasa/sensor/utils.py
--rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.0.6/frasa/sensor/variasi.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.048578 frasa-0.0.6/frasa.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 22:40:52.000000 frasa-0.0.6/frasa.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)      738 2023-04-14 22:40:52.000000 frasa-0.0.6/frasa.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-14 22:40:52.000000 frasa-0.0.6/frasa.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)        5 2023-04-14 22:40:52.000000 frasa-0.0.6/frasa.egg-info/requires.txt
--rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-14 22:40:52.000000 frasa-0.0.6/frasa.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-14 22:40:52.054113 frasa-0.0.6/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1090 2023-04-14 22:38:46.000000 frasa-0.0.6/setup.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.052811 frasa-0.0.6/tests/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:39.000000 frasa-0.0.6/tests/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.053107 frasa-0.0.6/tests/lemmatisasi/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:52:26.000000 frasa-0.0.6/tests/lemmatisasi/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:41.000000 frasa-0.0.6/tests/lemmatisasi/test_lemmatizer.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.053382 frasa-0.0.6/tests/stopword/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:51:58.000000 frasa-0.0.6/tests/stopword/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:38.000000 frasa-0.0.6/tests/stopword/test_stopword.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:40:52.053617 frasa-0.0.6/tests/tokenisasi/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:53.000000 frasa-0.0.6/tests/tokenisasi/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:33.000000 frasa-0.0.6/tests/tokenisasi/test_tokenizer.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.094200 frasa-0.0.7/
+-rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.0.7/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 22:46:09.094030 frasa-0.0.7/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     1700 2023-04-12 08:34:25.000000 frasa-0.0.7/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.089007 frasa-0.0.7/frasa/
+-rw-r--r--   0 novay      (501) staff       (20)      514 2023-04-14 22:46:05.000000 frasa-0.0.7/frasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.090055 frasa-0.0.7/frasa/datasets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.0.7/frasa/datasets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.090192 frasa-0.0.7/frasa/datasets/corpus/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.0.7/frasa/datasets/corpus/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.090317 frasa-0.0.7/frasa/datasets/corpus/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.0.7/frasa/datasets/corpus/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.090447 frasa-0.0.7/frasa/datasets/corpus/indonesia/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.0.7/frasa/datasets/corpus/indonesia/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.090566 frasa-0.0.7/frasa/datasets/corpus/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.0.7/frasa/datasets/corpus/sensor/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.090678 frasa-0.0.7/frasa/datasets/corpus/tweets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.0.7/frasa/datasets/corpus/tweets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.090798 frasa-0.0.7/frasa/deteksi/
+-rw-r--r--   0 novay      (501) staff       (20)      980 2023-04-14 16:03:46.000000 frasa-0.0.7/frasa/deteksi/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.091038 frasa-0.0.7/frasa/deteksi/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.0.7/frasa/deteksi/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.091202 frasa-0.0.7/frasa/deteksi/bahasa/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.0.7/frasa/deteksi/bahasa/data/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.091650 frasa-0.0.7/frasa/deteksi/gender/
+-rw-r--r--   0 novay      (501) staff       (20)      596 2023-04-14 11:05:42.000000 frasa-0.0.7/frasa/deteksi/gender/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     2712 2023-04-14 11:07:12.000000 frasa-0.0.7/frasa/deteksi/gender/classify.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.091798 frasa-0.0.7/frasa/deteksi/gender/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:59.000000 frasa-0.0.7/frasa/deteksi/gender/data/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      789 2023-04-14 10:06:04.000000 frasa-0.0.7/frasa/deteksi/gender/utils.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.092059 frasa-0.0.7/frasa/deteksi/plagiat/
+-rw-r--r--   0 novay      (501) staff       (20)       68 2023-04-12 08:57:39.000000 frasa-0.0.7/frasa/deteksi/plagiat/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     3708 2023-04-12 09:03:02.000000 frasa-0.0.7/frasa/deteksi/plagiat/plagiat.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.092748 frasa-0.0.7/frasa/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)       45 2023-04-14 16:27:02.000000 frasa-0.0.7/frasa/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      433 2023-04-11 19:58:03.000000 frasa-0.0.7/frasa/sensor/constants.py
+-rw-r--r--   0 novay      (501) staff       (20)     9277 2023-04-14 16:25:42.000000 frasa-0.0.7/frasa/sensor/sensor.py
+-rw-r--r--   0 novay      (501) staff       (20)     1572 2023-04-11 19:56:18.000000 frasa-0.0.7/frasa/sensor/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.0.7/frasa/sensor/variasi.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.089866 frasa-0.0.7/frasa.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 22:46:09.000000 frasa-0.0.7/frasa.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     1042 2023-04-14 22:46:09.000000 frasa-0.0.7/frasa.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-14 22:46:09.000000 frasa-0.0.7/frasa.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)        5 2023-04-14 22:46:09.000000 frasa-0.0.7/frasa.egg-info/requires.txt
+-rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-14 22:46:09.000000 frasa-0.0.7/frasa.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-14 22:46:09.094256 frasa-0.0.7/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1090 2023-04-14 22:46:00.000000 frasa-0.0.7/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.092889 frasa-0.0.7/tests/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:39.000000 frasa-0.0.7/tests/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.093133 frasa-0.0.7/tests/lemmatisasi/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:52:26.000000 frasa-0.0.7/tests/lemmatisasi/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:41.000000 frasa-0.0.7/tests/lemmatisasi/test_lemmatizer.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.093420 frasa-0.0.7/tests/stopword/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:51:58.000000 frasa-0.0.7/tests/stopword/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:38.000000 frasa-0.0.7/tests/stopword/test_stopword.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 22:46:09.093793 frasa-0.0.7/tests/tokenisasi/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-04 17:50:53.000000 frasa-0.0.7/tests/tokenisasi/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-06 13:36:33.000000 frasa-0.0.7/tests/tokenisasi/test_tokenizer.py
```

### Comparing `frasa-0.0.6/LICENSE` & `frasa-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/PKG-INFO` & `frasa-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.0.6
+Version: 0.0.7
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/python/tree/main/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.0.6/README.md` & `frasa-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/__init__.py` & `frasa-0.0.7/frasa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 
 Kunjungi http://frasa.id untuk informasi selengkapnya.
 """
 
 import os
 
 __name__ = "frasa"
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __license__ = 'MIT'
 __author__ = 'Novianto Rahmadi'
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `frasa-0.0.6/frasa/deteksi/__init__.py` & `frasa-0.0.7/frasa/deteksi/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/deteksi/gender/__init__.py` & `frasa-0.0.7/frasa/deteksi/gender/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/deteksi/gender/classify.py` & `frasa-0.0.7/frasa/deteksi/gender/classify.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/deteksi/gender/utils.py` & `frasa-0.0.7/frasa/deteksi/gender/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/deteksi/plagiat/plagiat.py` & `frasa-0.0.7/frasa/deteksi/plagiat/plagiat.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/sensor/sensor.py` & `frasa-0.0.7/frasa/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/sensor/utils.py` & `frasa-0.0.7/frasa/sensor/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa/sensor/variasi.py` & `frasa-0.0.7/frasa/sensor/variasi.py`

 * *Files identical despite different names*

### Comparing `frasa-0.0.6/frasa.egg-info/PKG-INFO` & `frasa-0.0.7/frasa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.0.6
+Version: 0.0.7
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/python/tree/main/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.0.6/frasa.egg-info/SOURCES.txt` & `frasa-0.0.7/frasa.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,27 @@
 setup.py
 frasa/__init__.py
 frasa.egg-info/PKG-INFO
 frasa.egg-info/SOURCES.txt
 frasa.egg-info/dependency_links.txt
 frasa.egg-info/requires.txt
 frasa.egg-info/top_level.txt
+frasa/datasets/__init__.py
+frasa/datasets/corpus/__init__.py
+frasa/datasets/corpus/bahasa/__init__.py
+frasa/datasets/corpus/indonesia/__init__.py
+frasa/datasets/corpus/sensor/__init__.py
+frasa/datasets/corpus/tweets/__init__.py
 frasa/deteksi/__init__.py
 frasa/deteksi/bahasa/__init__.py
+frasa/deteksi/bahasa/data/__init__.py
 frasa/deteksi/gender/__init__.py
 frasa/deteksi/gender/classify.py
 frasa/deteksi/gender/utils.py
+frasa/deteksi/gender/data/__init__.py
 frasa/deteksi/plagiat/__init__.py
 frasa/deteksi/plagiat/plagiat.py
 frasa/sensor/__init__.py
 frasa/sensor/constants.py
 frasa/sensor/sensor.py
 frasa/sensor/utils.py
 frasa/sensor/variasi.py
```

### Comparing `frasa-0.0.6/setup.py` & `frasa-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="frasa",
-    version="0.0.6",
+    version="0.0.7",
     description="Koleksi NLP Pribadi untuk Bahasa Indonesia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/python/tree/main/frasa",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
```

