# Comparing `tmp/clibrary-1.6.2.tar.gz` & `tmp/clibrary-1.7.0.tar.gz`

## Comparing `clibrary-1.6.2.tar` & `clibrary-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.6.2/Makefile
--rw-r--r--   0        0        0     9720 2020-02-02 00:00:00.000000 clibrary-1.6.2/docs.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.6.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.6.2/src/CLIbrary/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.6.2/src/CLIbrary/files.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 clibrary-1.6.2/src/CLIbrary/inputs.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 clibrary-1.6.2/src/CLIbrary/interface.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 clibrary-1.6.2/src/CLIbrary/outputs.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clibrary-1.6.2/src/CLIbrary/settings.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.6.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.6.2/LICENSE
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 clibrary-1.6.2/README.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 clibrary-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 clibrary-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.7.0/Makefile
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 clibrary-1.7.0/docs.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/__main__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/files.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/inputs.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/interface.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/outputs.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clibrary-1.7.0/src/CLIbrary/settings.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.7.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 clibrary-1.7.0/README.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 clibrary-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 clibrary-1.7.0/PKG-INFO
```

### Comparing `clibrary-1.6.2/docs.md` & `clibrary-1.7.0/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # CLIbrary's documentation
 
 ## Projects built with CLIbrary
 
 These projects have been built with **CLIbrary** and they should serve as examples for future **CLIbrary** projects.
 
 * [**openBriefcase**](https://github.com/diantonioandrea/openBriefcase), by [Andrea Di Antonio](https://github.com/diantonioandrea).
+* [**openTree**](https://github.com/diantonioandrea/openTree), by [Andrea Di Antonio](https://github.com/diantonioandrea).
 * [**NBody**](https://github.com/diantonioandrea/NBody), by [Andrea Di Antonio](https://github.com/diantonioandrea).
 
 ## Table of Contents
 
 0. [Projects built with CLIbrary](#projects-built-with-clibrary)
 1. [Introduction](#introduction)
 	1. [CLIbrary](#clibrary)
@@ -63,14 +64,18 @@
 3. `CLIbrary.data.setting_fileExtension`, str: Defines a file extension for *CLIbrary.aDump* and *CLIbrary.aLoad*. Default value based on Python's module *pickle*.
 
 ### Import CLIbrary
 
 **CLIbrary** can be installed by:
 
 	python3 -m pip install --upgrade CLIbrary
+
+verified by:
+
+	python3 -m CLIbrary
 	
 imported by:
 
 	import CLIbrary
 
 and all the functions can be accessed by:
```

### Comparing `clibrary-1.6.2/.github/workflows/python-publish.yml` & `clibrary-1.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `clibrary-1.6.2/src/CLIbrary/files.py` & `clibrary-1.7.0/src/CLIbrary/files.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.6.2/src/CLIbrary/inputs.py` & `clibrary-1.7.0/src/CLIbrary/inputs.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.6.2/src/CLIbrary/interface.py` & `clibrary-1.7.0/src/CLIbrary/interface.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.6.2/src/CLIbrary/outputs.py` & `clibrary-1.7.0/src/CLIbrary/outputs.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.6.2/LICENSE` & `clibrary-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clibrary-1.6.2/pyproject.toml` & `clibrary-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "colorama", "datetime"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CLIbrary"
-version = "1.6.2"
+version = "1.7.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "A standardized collection of CLI utilities written in Python to handle commands, I/O and files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `clibrary-1.6.2/PKG-INFO` & `clibrary-1.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLIbrary
-Version: 1.6.2
+Version: 1.7.0
 Summary: A standardized collection of CLI utilities written in Python to handle commands, I/O and files.
 Project-URL: Homepage, https://github.com/diantonioandrea/CLIbrary
 Project-URL: Documentation, https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/CLIbrary/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,14 +22,26 @@
 
 ### Installing CLIbrary
 
 **CLIbrary** can be installed from [PyPI](https://pypi.org) by:
 
 	python3 -m pip install --upgrade CLIbrary
 
+### Verify installation
+
+The installation of **CLIbrary** can be verified by:
+
+	python3 -m CLIbrary
+
+which would return something similar to:
+
+	 ●  CLIbrary v1.7.0 
+	A standardized collection of CLI utilities written in Python to handle commands, I/O and files.
+	Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/CLIbrary
+
 ### Importing CLIbrary
 
 **CLIbrary** can be imported by:
 
 	import CLIbrary
 
 ## Examples
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

