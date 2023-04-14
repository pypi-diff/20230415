# Comparing `tmp/st_text_annotator-0.1.0.tar.gz` & `tmp/st_text_annotator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_text_annotator-0.1.0.tar", last modified: Fri Apr 14 22:31:49 2023, max compression
+gzip compressed data, was "st_text_annotator-0.1.1.tar", last modified: Fri Apr 14 22:43:09 2023, max compression
```

## Comparing `st_text_annotator-0.1.0.tar` & `st_text_annotator-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:31:49.267725 st_text_annotator-0.1.0/
--rw-r--r--   0 robin      (501) staff       (20)     1075 2023-04-14 18:30:17.000000 st_text_annotator-0.1.0/LICENSE
--rw-r--r--   0 robin      (501) staff       (20)       53 2023-04-14 21:49:12.000000 st_text_annotator-0.1.0/MANIFEST.in
--rw-r--r--   0 robin      (501) staff       (20)     1630 2023-04-14 22:31:49.267425 st_text_annotator-0.1.0/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)      971 2023-04-14 22:26:10.000000 st_text_annotator-0.1.0/README.md
--rw-r--r--   0 robin      (501) staff       (20)      646 2023-04-14 22:31:12.000000 st_text_annotator-0.1.0/pyproject.toml
--rw-r--r--   0 robin      (501) staff       (20)       38 2023-04-14 22:31:49.267820 st_text_annotator-0.1.0/setup.cfg
--rw-r--r--   0 robin      (501) staff       (20)      806 2023-04-14 22:16:18.000000 st_text_annotator-0.1.0/setup.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:31:49.267015 st_text_annotator-0.1.0/st_text_annotator.egg-info/
--rw-r--r--   0 robin      (501) staff       (20)     1630 2023-04-14 22:31:49.000000 st_text_annotator-0.1.0/st_text_annotator.egg-info/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)      257 2023-04-14 22:31:49.000000 st_text_annotator-0.1.0/st_text_annotator.egg-info/SOURCES.txt
--rw-r--r--   0 robin      (501) staff       (20)        1 2023-04-14 22:31:49.000000 st_text_annotator-0.1.0/st_text_annotator.egg-info/dependency_links.txt
--rw-r--r--   0 robin      (501) staff       (20)       17 2023-04-14 22:31:49.000000 st_text_annotator-0.1.0/st_text_annotator.egg-info/requires.txt
--rw-r--r--   0 robin      (501) staff       (20)        1 2023-04-14 22:31:49.000000 st_text_annotator-0.1.0/st_text_annotator.egg-info/top_level.txt
+drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.255078 st_text_annotator-0.1.1/
+-rw-r--r--   0 robin      (501) staff       (20)     1075 2023-04-14 18:30:17.000000 st_text_annotator-0.1.1/LICENSE
+-rw-r--r--   0 robin      (501) staff       (20)       53 2023-04-14 21:49:12.000000 st_text_annotator-0.1.1/MANIFEST.in
+-rw-r--r--   0 robin      (501) staff       (20)     1630 2023-04-14 22:43:09.253256 st_text_annotator-0.1.1/PKG-INFO
+-rw-r--r--   0 robin      (501) staff       (20)      971 2023-04-14 22:26:10.000000 st_text_annotator-0.1.1/README.md
+-rw-r--r--   0 robin      (501) staff       (20)      646 2023-04-14 22:40:24.000000 st_text_annotator-0.1.1/pyproject.toml
+-rw-r--r--   0 robin      (501) staff       (20)       38 2023-04-14 22:43:09.255560 st_text_annotator-0.1.1/setup.cfg
+-rw-r--r--   0 robin      (501) staff       (20)      851 2023-04-14 22:42:20.000000 st_text_annotator-0.1.1/setup.py
+drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.245087 st_text_annotator-0.1.1/src/
+drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.248497 st_text_annotator-0.1.1/src/st_text_annotator/
+-rw-r--r--   0 robin      (501) staff       (20)     5238 2023-04-14 22:21:01.000000 st_text_annotator-0.1.1/src/st_text_annotator/__init__.py
+drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.252436 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/
+-rw-r--r--   0 robin      (501) staff       (20)     1630 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/PKG-INFO
+-rw-r--r--   0 robin      (501) staff       (20)      311 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/SOURCES.txt
+-rw-r--r--   0 robin      (501) staff       (20)        1 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/dependency_links.txt
+-rw-r--r--   0 robin      (501) staff       (20)       17 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/requires.txt
+-rw-r--r--   0 robin      (501) staff       (20)       18 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/top_level.txt
```

### Comparing `st_text_annotator-0.1.0/LICENSE` & `st_text_annotator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.0/PKG-INFO` & `st_text_annotator-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_text_annotator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Component for annotating text for NLP resolution
 Home-page: https://github.com/rmarquet21/steamlit-text-annotator
 Author: Robin Marquet
 Author-email: Robin Marquet <robin.marquet3@gmail.com>
 Project-URL: Homepage, https://github.com/rmarquet21/streamlit-text-annotator
 Project-URL: Bug Tracker, https://github.com/rmarquet21/streamlit-text-annotator/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `st_text_annotator-0.1.0/README.md` & `st_text_annotator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.0/pyproject.toml` & `st_text_annotator-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "st_text_annotator"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Robin Marquet", email="robin.marquet3@gmail.com" },
 ]
 description = "Component for annotating text for NLP resolution"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `st_text_annotator-0.1.0/setup.py` & `st_text_annotator-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 setuptools.setup(
     name="streamlit-text-annotator",
     version="0.1.1",
     author="Robin Marquet",
     author_email="robin.marquet3@gmail.com",
     description="Component for annotating text for NLP resolution",
     long_description=long_description,
-    long_description_content_type="text/plain",
+    long_description_content_type="text/markdown",
     url="https://github.com/rmarquet21/steamlit-text-annotator",
-    packages=setuptools.find_packages(),
+    package_dir = {"": "src"},
+    packages=setuptools.find_packages(where="src"),
     include_package_data=True,
     python_requires=">=3.8",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `st_text_annotator-0.1.0/st_text_annotator.egg-info/PKG-INFO` & `st_text_annotator-0.1.1/src/st_text_annotator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-text-annotator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Component for annotating text for NLP resolution
 Home-page: https://github.com/rmarquet21/steamlit-text-annotator
 Author: Robin Marquet
 Author-email: Robin Marquet <robin.marquet3@gmail.com>
 Project-URL: Homepage, https://github.com/rmarquet21/streamlit-text-annotator
 Project-URL: Bug Tracker, https://github.com/rmarquet21/streamlit-text-annotator/issues
 Classifier: Programming Language :: Python :: 3
```

