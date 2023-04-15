# Comparing `tmp/json-replacer-1.0.0.tar.gz` & `tmp/json-replacer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-replacer-1.0.0.tar", last modified: Sun Mar 26 22:36:59 2023, max compression
+gzip compressed data, was "json-replacer-1.0.1.tar", last modified: Sat Apr 15 17:52:18 2023, max compression
```

## Comparing `json-replacer-1.0.0.tar` & `json-replacer-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 22:36:59.355048 json-replacer-1.0.0/
--rw-rw-rw-   0        0        0     1085 2023-03-25 09:35:12.000000 json-replacer-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      461 2023-03-26 22:36:59.355048 json-replacer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1146 2023-03-26 21:56:09.000000 json-replacer-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 22:36:59.323802 json-replacer-1.0.0/json_replacer/
--rw-rw-rw-   0        0        0       42 2023-03-26 21:40:17.000000 json-replacer-1.0.0/json_replacer/__init__.py
--rw-rw-rw-   0        0        0      954 2023-03-26 22:31:26.000000 json-replacer-1.0.0/json_replacer/json_replacer.py
--rw-rw-rw-   0        0        0     1083 2023-03-26 22:34:16.000000 json-replacer-1.0.0/json_replacer/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-26 22:36:59.339424 json-replacer-1.0.0/json_replacer.egg-info/
--rw-rw-rw-   0        0        0      461 2023-03-26 22:36:59.000000 json-replacer-1.0.0/json_replacer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-03-26 22:36:59.000000 json-replacer-1.0.0/json_replacer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 22:36:59.000000 json-replacer-1.0.0/json_replacer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-26 22:36:59.000000 json-replacer-1.0.0/json_replacer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 22:36:59.355048 json-replacer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-03-26 22:36:51.000000 json-replacer-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 22:36:59.339424 json-replacer-1.0.0/test/
--rw-rw-rw-   0        0        0     1880 2023-03-26 22:35:53.000000 json-replacer-1.0.0/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:52:18.465044 json-replacer-1.0.1/
+-rw-rw-rw-   0        0        0     1085 2023-03-25 09:35:12.000000 json-replacer-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-04-15 17:52:18.463041 json-replacer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1146 2023-03-26 21:56:09.000000 json-replacer-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 17:52:18.437368 json-replacer-1.0.1/json_replacer/
+-rw-rw-rw-   0        0        0       42 2023-03-26 21:40:17.000000 json-replacer-1.0.1/json_replacer/__init__.py
+-rw-rw-rw-   0        0        0      954 2023-03-26 22:31:26.000000 json-replacer-1.0.1/json_replacer/json_replacer.py
+-rw-rw-rw-   0        0        0      525 2023-04-15 17:28:11.000000 json-replacer-1.0.1/json_replacer/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:52:18.453896 json-replacer-1.0.1/json_replacer.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-04-15 17:52:18.000000 json-replacer-1.0.1/json_replacer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-15 17:52:18.000000 json-replacer-1.0.1/json_replacer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 17:52:18.000000 json-replacer-1.0.1/json_replacer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-15 17:52:18.000000 json-replacer-1.0.1/json_replacer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:52:18.465582 json-replacer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2023-04-15 17:52:10.000000 json-replacer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:52:18.459041 json-replacer-1.0.1/test/
+-rw-rw-rw-   0        0        0     1880 2023-03-26 22:35:53.000000 json-replacer-1.0.1/test/tests.py
```

### Comparing `json-replacer-1.0.0/LICENSE` & `json-replacer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json-replacer-1.0.0/README.md` & `json-replacer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `json-replacer-1.0.0/json_replacer/json_replacer.py` & `json-replacer-1.0.1/json_replacer/json_replacer.py`

 * *Files identical despite different names*

### Comparing `json-replacer-1.0.0/setup.py` & `json-replacer-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = 'JSON placeholder substitute tool'
-LONG_DESCRIPTION = 'Substitute the placeholder "{{name}}" in JSON with the corresponding value from another JSON such as {"name": "Lorenzo"}'
+LONG_DESCRIPTION = 'Substitute the placeholder "{{name}}" in JSON with the corresponding value from another JSON such as {"name": "Lorenzo"}. Project link: https://github.com/lorenzua02/json-replacer'
 
 setup(
     # python_requires=">3.10",
     name="json-replacer",
     version=VERSION,
     author="Lorenzo Mogicato",
     author_email="<lorenzo.mogicato@gmail.com>",
```

### Comparing `json-replacer-1.0.0/test/tests.py` & `json-replacer-1.0.1/test/tests.py`

 * *Files identical despite different names*

