# Comparing `tmp/gitpulse-1.0.tar.gz` & `tmp/gitpulse-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitpulse-1.0.tar", last modified: Sat Apr 15 10:04:22 2023, max compression
+gzip compressed data, was "gitpulse-1.1.tar", last modified: Sat Apr 15 13:35:24 2023, max compression
```

## Comparing `gitpulse-1.0.tar` & `gitpulse-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:04:22.705851 gitpulse-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 10:04:22.705851 gitpulse-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-15 10:04:10.000000 gitpulse-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:04:22.705851 gitpulse-1.0/gitpulse/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-15 10:04:10.000000 gitpulse-1.0/gitpulse/DynamicHTMLReportGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-15 10:04:10.000000 gitpulse-1.0/gitpulse/GitDiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-15 10:04:10.000000 gitpulse-1.0/gitpulse/HTMLReportGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:04:10.000000 gitpulse-1.0/gitpulse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-15 10:04:10.000000 gitpulse-1.0/gitpulse/gitpulse_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:04:22.705851 gitpulse-1.0/gitpulse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 10:04:22.000000 gitpulse-1.0/gitpulse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-15 10:04:22.000000 gitpulse-1.0/gitpulse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:04:22.000000 gitpulse-1.0/gitpulse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 10:04:22.000000 gitpulse-1.0/gitpulse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 10:04:22.000000 gitpulse-1.0/gitpulse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 10:04:22.000000 gitpulse-1.0/gitpulse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:04:22.705851 gitpulse-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-15 10:04:10.000000 gitpulse-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:24.144452 gitpulse-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 13:35:24.144452 gitpulse-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-15 13:35:13.000000 gitpulse-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:24.144452 gitpulse-1.1/gitpulse/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/DynamicHTMLReportGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/GitDiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/HTMLReportGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/gitpulse_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:24.144452 gitpulse-1.1/gitpulse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:35:24.144452 gitpulse-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-15 13:35:13.000000 gitpulse-1.1/setup.py
```

### Comparing `gitpulse-1.0/PKG-INFO` & `gitpulse-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gitpulse
-Version: 1.0
+Version: 1.1
 Description-Content-Type: text/markdown
 
 GitPulse
 ========
-![image](https://user-images.githubusercontent.com/82222256/232206399-417bab63-1420-466b-84f5-663f860331f3.png)
+![image](https://user-images.githubusercontent.com/82222256/232227058-d90fe7c8-26cb-4d04-9d98-01aec5510a08.png)
 
 GitPulse is a Python-based command-line tool that generates an HTML report summarizing Git log data for a software development project. It provides insights into the number of commits and merges for each developer who has contributed to the project.
 
 Installation
 ------------
 
 To install GitPulse, you can use pip. Open a terminal window and enter the following command:
```

### Comparing `gitpulse-1.0/README.md` & `gitpulse-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 GitPulse
 ========
-![image](https://user-images.githubusercontent.com/82222256/232206399-417bab63-1420-466b-84f5-663f860331f3.png)
+![image](https://user-images.githubusercontent.com/82222256/232227058-d90fe7c8-26cb-4d04-9d98-01aec5510a08.png)
 
 GitPulse is a Python-based command-line tool that generates an HTML report summarizing Git log data for a software development project. It provides insights into the number of commits and merges for each developer who has contributed to the project.
 
 Installation
 ------------
 
 To install GitPulse, you can use pip. Open a terminal window and enter the following command:
```

### Comparing `gitpulse-1.0/gitpulse/DynamicHTMLReportGenerator.py` & `gitpulse-1.1/gitpulse/DynamicHTMLReportGenerator.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.0/gitpulse/GitDiff.py` & `gitpulse-1.1/gitpulse/GitDiff.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.0/gitpulse/HTMLReportGenerator.py` & `gitpulse-1.1/gitpulse/HTMLReportGenerator.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.0/gitpulse/gitpulse_cli.py` & `gitpulse-1.1/gitpulse/gitpulse_cli.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.0/gitpulse.egg-info/PKG-INFO` & `gitpulse-1.1/gitpulse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gitpulse
-Version: 1.0
+Version: 1.1
 Description-Content-Type: text/markdown
 
 GitPulse
 ========
-![image](https://user-images.githubusercontent.com/82222256/232206399-417bab63-1420-466b-84f5-663f860331f3.png)
+![image](https://user-images.githubusercontent.com/82222256/232227058-d90fe7c8-26cb-4d04-9d98-01aec5510a08.png)
 
 GitPulse is a Python-based command-line tool that generates an HTML report summarizing Git log data for a software development project. It provides insights into the number of commits and merges for each developer who has contributed to the project.
 
 Installation
 ------------
 
 To install GitPulse, you can use pip. Open a terminal window and enter the following command:
```

### Comparing `gitpulse-1.0/setup.py` & `gitpulse-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the content of the README.md file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='gitpulse',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     install_requires=[
         # Add your package dependencies here:
         'gitpython',
         'jinja2',
         'python-dateutil',
     ],
```

