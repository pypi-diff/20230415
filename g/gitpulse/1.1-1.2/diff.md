# Comparing `tmp/gitpulse-1.1.tar.gz` & `tmp/gitpulse-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitpulse-1.1.tar", last modified: Sat Apr 15 13:35:24 2023, max compression
+gzip compressed data, was "gitpulse-1.2.tar", last modified: Sat Apr 15 13:42:35 2023, max compression
```

## Comparing `gitpulse-1.1.tar` & `gitpulse-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:24.144452 gitpulse-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 13:35:24.144452 gitpulse-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-15 13:35:13.000000 gitpulse-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:24.144452 gitpulse-1.1/gitpulse/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/DynamicHTMLReportGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/GitDiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/HTMLReportGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-15 13:35:13.000000 gitpulse-1.1/gitpulse/gitpulse_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:35:24.144452 gitpulse-1.1/gitpulse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 13:35:24.000000 gitpulse-1.1/gitpulse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:35:24.144452 gitpulse-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-15 13:35:13.000000 gitpulse-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:42:35.732838 gitpulse-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-15 13:42:35.732838 gitpulse-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-15 13:42:24.000000 gitpulse-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:42:35.732838 gitpulse-1.2/gitpulse/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-15 13:42:24.000000 gitpulse-1.2/gitpulse/DynamicHTMLReportGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-15 13:42:24.000000 gitpulse-1.2/gitpulse/GitDiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-15 13:42:24.000000 gitpulse-1.2/gitpulse/HTMLReportGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:42:24.000000 gitpulse-1.2/gitpulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-15 13:42:24.000000 gitpulse-1.2/gitpulse/gitpulse_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:42:35.732838 gitpulse-1.2/gitpulse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-15 13:42:35.000000 gitpulse-1.2/gitpulse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-15 13:42:35.000000 gitpulse-1.2/gitpulse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:42:35.000000 gitpulse-1.2/gitpulse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 13:42:35.000000 gitpulse-1.2/gitpulse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 13:42:35.000000 gitpulse-1.2/gitpulse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 13:42:35.000000 gitpulse-1.2/gitpulse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:42:35.732838 gitpulse-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-15 13:42:24.000000 gitpulse-1.2/setup.py
```

### Comparing `gitpulse-1.1/PKG-INFO` & `gitpulse-1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-Metadata-Version: 2.1
-Name: gitpulse
-Version: 1.1
-Description-Content-Type: text/markdown
-
 GitPulse
 ========
 ![image](https://user-images.githubusercontent.com/82222256/232227058-d90fe7c8-26cb-4d04-9d98-01aec5510a08.png)
 
 GitPulse is a Python-based command-line tool that generates an HTML report summarizing Git log data for a software development project. It provides insights into the number of commits and merges for each developer who has contributed to the project.
 
 Installation
 ------------
 
-To install GitPulse, you can use pip. Open a terminal window and enter the following command:
-
-bashCopy code
+To install GitPulse, you can use pip. Open a terminal window and enter the following command in adminstrator mode:
 
-`pip install gitpulse`
+```
+pip install gitpulse
+```
 
 Usage
 -----
 
-GitPulse can be run from the command line using the `gitpulse` command. The tool requires two inputs: the path to the Git repository and the output filename for the generated report.
+GitPulse can be run from the command line using the `gitpulse` command in the the Git repository.
 
 Here is the basic syntax for using GitPulse:
 
-bashCopy code
-
-`gitpulse `
+```
+gitpulse
+```
 
-The generated report will be saved in the current directory with name **gitpulse_report.html**.
+On success there will be clean exit to console. The generated report will be saved in the current directory with name **gitpulse_report.html**.
 
 Benefits
 --------
 ![image](https://user-images.githubusercontent.com/82222256/232167548-b4767c2e-737b-42cb-b66b-aad78ad29602.png)
 
 ![image](https://user-images.githubusercontent.com/82222256/232167592-62605251-8ec7-4f9e-a396-2c35beb83d71.png)
```

### Comparing `gitpulse-1.1/README.md` & `gitpulse-1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
+Metadata-Version: 2.1
+Name: gitpulse
+Version: 1.2
+Description-Content-Type: text/markdown
+
 GitPulse
 ========
 ![image](https://user-images.githubusercontent.com/82222256/232227058-d90fe7c8-26cb-4d04-9d98-01aec5510a08.png)
 
 GitPulse is a Python-based command-line tool that generates an HTML report summarizing Git log data for a software development project. It provides insights into the number of commits and merges for each developer who has contributed to the project.
 
 Installation
 ------------
 
-To install GitPulse, you can use pip. Open a terminal window and enter the following command:
-
-bashCopy code
+To install GitPulse, you can use pip. Open a terminal window and enter the following command in adminstrator mode:
 
-`pip install gitpulse`
+```
+pip install gitpulse
+```
 
 Usage
 -----
 
-GitPulse can be run from the command line using the `gitpulse` command. The tool requires two inputs: the path to the Git repository and the output filename for the generated report.
+GitPulse can be run from the command line using the `gitpulse` command in the the Git repository.
 
 Here is the basic syntax for using GitPulse:
 
-bashCopy code
-
-`gitpulse `
+```
+gitpulse
+```
 
-The generated report will be saved in the current directory with name **gitpulse_report.html**.
+On success there will be clean exit to console. The generated report will be saved in the current directory with name **gitpulse_report.html**.
 
 Benefits
 --------
 ![image](https://user-images.githubusercontent.com/82222256/232167548-b4767c2e-737b-42cb-b66b-aad78ad29602.png)
 
 ![image](https://user-images.githubusercontent.com/82222256/232167592-62605251-8ec7-4f9e-a396-2c35beb83d71.png)
```

### Comparing `gitpulse-1.1/gitpulse/DynamicHTMLReportGenerator.py` & `gitpulse-1.2/gitpulse/DynamicHTMLReportGenerator.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.1/gitpulse/GitDiff.py` & `gitpulse-1.2/gitpulse/GitDiff.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.1/gitpulse/HTMLReportGenerator.py` & `gitpulse-1.2/gitpulse/HTMLReportGenerator.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.1/gitpulse/gitpulse_cli.py` & `gitpulse-1.2/gitpulse/gitpulse_cli.py`

 * *Files identical despite different names*

### Comparing `gitpulse-1.1/gitpulse.egg-info/PKG-INFO` & `gitpulse-1.2/gitpulse.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: gitpulse
-Version: 1.1
+Version: 1.2
 Description-Content-Type: text/markdown
 
 GitPulse
 ========
 ![image](https://user-images.githubusercontent.com/82222256/232227058-d90fe7c8-26cb-4d04-9d98-01aec5510a08.png)
 
 GitPulse is a Python-based command-line tool that generates an HTML report summarizing Git log data for a software development project. It provides insights into the number of commits and merges for each developer who has contributed to the project.
 
 Installation
 ------------
 
-To install GitPulse, you can use pip. Open a terminal window and enter the following command:
+To install GitPulse, you can use pip. Open a terminal window and enter the following command in adminstrator mode:
 
-bashCopy code
-
-`pip install gitpulse`
+```
+pip install gitpulse
+```
 
 Usage
 -----
 
-GitPulse can be run from the command line using the `gitpulse` command. The tool requires two inputs: the path to the Git repository and the output filename for the generated report.
+GitPulse can be run from the command line using the `gitpulse` command in the the Git repository.
 
 Here is the basic syntax for using GitPulse:
 
-bashCopy code
-
-`gitpulse `
+```
+gitpulse
+```
 
-The generated report will be saved in the current directory with name **gitpulse_report.html**.
+On success there will be clean exit to console. The generated report will be saved in the current directory with name **gitpulse_report.html**.
 
 Benefits
 --------
 ![image](https://user-images.githubusercontent.com/82222256/232167548-b4767c2e-737b-42cb-b66b-aad78ad29602.png)
 
 ![image](https://user-images.githubusercontent.com/82222256/232167592-62605251-8ec7-4f9e-a396-2c35beb83d71.png)
```

### Comparing `gitpulse-1.1/setup.py` & `gitpulse-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the content of the README.md file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='gitpulse',
-    version='1.1',
+    version='1.2',
     packages=find_packages(),
     install_requires=[
         # Add your package dependencies here:
         'gitpython',
         'jinja2',
         'python-dateutil',
     ],
```

