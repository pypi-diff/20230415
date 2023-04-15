# Comparing `tmp/toolkit_lennart-0.0.2.tar.gz` & `tmp/toolkit_lennart-0.0.3.tar.gz`

## Comparing `toolkit_lennart-0.0.2.tar` & `toolkit_lennart-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/.DS_Store
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/main.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/setup.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/.idea/python_package.iml
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/build/lib/toolkit_lennart/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/build/lib/toolkit_lennart/plot.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/build/lib/toolkit_lennart/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/toolkit_lennart/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/toolkit_lennart/plot.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/toolkit_lennart/plot_help.txt
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/toolkit_lennart.egg-info/PKG-INFO
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/toolkit_lennart.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/toolkit_lennart.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/toolkit_lennart.egg-info/top_level.txt
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/LICENSE
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/.DS_Store
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/main.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/setup.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/.idea/python_package.iml
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/build/lib/toolkit_lennart/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/build/lib/toolkit_lennart/plot.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/build/lib/toolkit_lennart/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/toolkit_lennart/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/toolkit_lennart/plot.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/toolkit_lennart/plot_help.txt
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/toolkit_lennart.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/toolkit_lennart.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/toolkit_lennart.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/toolkit_lennart.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/LICENSE
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 toolkit_lennart-0.0.3/PKG-INFO
```

### Comparing `toolkit_lennart-0.0.2/.DS_Store` & `toolkit_lennart-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.2/.idea/workspace.xml` & `toolkit_lennart-0.0.3/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.2/build/lib/toolkit_lennart/plot.py` & `toolkit_lennart-0.0.3/build/lib/toolkit_lennart/plot.py`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.2/toolkit_lennart/plot.py` & `toolkit_lennart-0.0.3/toolkit_lennart/plot.py`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.2/toolkit_lennart.egg-info/PKG-INFO` & `toolkit_lennart-0.0.3/toolkit_lennart.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.2/LICENSE` & `toolkit_lennart-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.2/pyproject.toml` & `toolkit_lennart-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toolkit_lennart"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Lennart Rooden", email="lennart.rs@gmail.com" },
 ]
 description = "Toolkit for data analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `toolkit_lennart-0.0.2/PKG-INFO` & `toolkit_lennart-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolkit_lennart
-Version: 0.0.2
+Version: 0.0.3
 Summary: Toolkit for data analysis
 Author-email: Lennart Rooden <lennart.rs@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

