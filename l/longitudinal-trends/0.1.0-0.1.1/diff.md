# Comparing `tmp/longitudinal_trends-0.1.0.tar.gz` & `tmp/longitudinal_trends-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longitudinal_trends-0.1.0.tar", last modified: Mon Apr 10 18:34:04 2023, max compression
+gzip compressed data, was "longitudinal_trends-0.1.1.tar", last modified: Sat Apr 15 12:33:04 2023, max compression
```

## Comparing `longitudinal_trends-0.1.0.tar` & `longitudinal_trends-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-10 18:34:04.310888 longitudinal_trends-0.1.0/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.0/LICENSE
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.0/MANIFEST.in
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9883 2023-04-10 18:34:04.310888 longitudinal_trends-0.1.0/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9349 2023-04-07 07:04:07.000000 longitudinal_trends-0.1.0/README.md
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-10 18:34:04.115846 longitudinal_trends-0.1.0/longitudinal_trends/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17412 2023-04-10 18:21:23.000000 longitudinal_trends-0.1.0/longitudinal_trends/__init__.py
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-10 18:34:04.262911 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9883 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/SOURCES.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/dependency_links.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/requires.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-04-10 18:34:03.000000 longitudinal_trends-0.1.0/longitudinal_trends.egg-info/top_level.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1097 2023-04-10 18:23:40.000000 longitudinal_trends-0.1.0/pyproject.toml
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      136 2023-04-03 18:57:25.000000 longitudinal_trends-0.1.0/requirements.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-04-10 18:34:04.315900 longitudinal_trends-0.1.0/setup.cfg
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-15 12:33:04.224443 longitudinal_trends-0.1.1/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.1/LICENSE
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9927 2023-04-15 12:33:04.213915 longitudinal_trends-0.1.1/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9349 2023-04-07 07:04:07.000000 longitudinal_trends-0.1.1/README.md
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-15 12:33:03.621832 longitudinal_trends-0.1.1/longitudinal_trends/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17412 2023-04-10 18:21:23.000000 longitudinal_trends-0.1.1/longitudinal_trends/__init__.py
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-04-15 12:33:04.122380 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9927 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-04-15 12:33:03.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/SOURCES.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/dependency_links.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/requires.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-04-15 12:33:02.000000 longitudinal_trends-0.1.1/longitudinal_trends.egg-info/top_level.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-04-15 12:27:49.000000 longitudinal_trends-0.1.1/pyproject.toml
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      136 2023-04-03 18:57:25.000000 longitudinal_trends-0.1.1/requirements.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-04-15 12:33:04.229457 longitudinal_trends-0.1.1/setup.cfg
```

### Comparing `longitudinal_trends-0.1.0/LICENSE` & `longitudinal_trends-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.0/PKG-INFO` & `longitudinal_trends-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: longitudinal_trends
-Version: 0.1.0
-Summary: Download long-term longitudinal Google Trends
+Version: 0.1.1
+Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
-Keywords: google trends api search longtrends cross section
+Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `longitudinal_trends-0.1.0/README.md` & `longitudinal_trends-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.0/longitudinal_trends/__init__.py` & `longitudinal_trends-0.1.1/longitudinal_trends/__init__.py`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.0/longitudinal_trends.egg-info/PKG-INFO` & `longitudinal_trends-0.1.1/longitudinal_trends.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: longitudinal-trends
-Version: 0.1.0
-Summary: Download long-term longitudinal Google Trends
+Version: 0.1.1
+Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
-Keywords: google trends api search longtrends cross section
+Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `longitudinal_trends-0.1.0/pyproject.toml` & `longitudinal_trends-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]#, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "longitudinal_trends"
-version='0.1.0'
-description="Download long-term longitudinal Google Trends"
+version='0.1.1'
+description="Generate long-term longitudinal Google Trends Data"
 urls = {homepage = "https://github.com/Mohammad-sakir/longitudinalTrends"}
 requires-python = ">=3.6"
 authors = [
     {name = "Mohammad Saleh Ahsan Sakir"},
     {name = "Taeyong Park"}, 
     {email="ahsansakir506@gmail.com"},    
     {email = "taeyongp@andrew.cmu.edu"}
@@ -20,15 +20,15 @@
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 keywords = [
-    "google trends api search longtrends cross section"
+    "longitudinal-trends longitudinal data python google-trends-api google-trends search-data"
 ]
 
 dynamic = ["readme", "dependencies"]
 
 [tool.setuptools]
 packages = ["longitudinal_trends"]
```

