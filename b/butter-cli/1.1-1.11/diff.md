# Comparing `tmp/butter-cli-1.1.tar.gz` & `tmp/butter-cli-1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butter-cli-1.1.tar", last modified: Fri Apr 14 18:07:22 2023, max compression
+gzip compressed data, was "butter-cli-1.11.tar", last modified: Sat Apr 15 02:12:36 2023, max compression
```

## Comparing `butter-cli-1.1.tar` & `butter-cli-1.11.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.017002 butter-cli-1.1/
--rw-r--r--   0 michaelequi   (501) staff       (20)      195 2023-04-14 18:07:22.016690 butter-cli-1.1/PKG-INFO
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.012221 butter-cli-1.1/butter_cli.egg-info/
--rw-r--r--   0 michaelequi   (501) staff       (20)      145 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/PKG-INFO
--rw-r--r--   0 michaelequi   (501) staff       (20)      239 2023-04-14 01:28:01.000000 butter-cli-1.1/butter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/requires.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/top_level.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)       38 2023-04-14 18:07:22.017095 butter-cli-1.1/setup.cfg
--rw-r--r--   0 michaelequi   (501) staff       (20)      638 2023-04-14 18:07:04.000000 butter-cli-1.1/setup.py
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.009677 butter-cli-1.1/src/
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.014011 butter-cli-1.1/src/butter/
--rw-r--r--   0 michaelequi   (501) staff       (20)       51 2023-04-14 01:34:57.000000 butter-cli-1.1/src/butter/__init__.py
--rw-r--r--   0 michaelequi   (501) staff       (20)     3855 2023-04-14 07:32:50.000000 butter-cli-1.1/src/butter/butter.py
--rw-r--r--   0 michaelequi   (501) staff       (20)     1140 2023-01-29 05:31:52.000000 butter-cli-1.1/src/butter/cli.py
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.016325 butter-cli-1.1/src/butter_cli.egg-info/
--rw-r--r--   0 michaelequi   (501) staff       (20)      195 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/PKG-INFO
--rw-r--r--   0 michaelequi   (501) staff       (20)      469 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)       42 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/entry_points.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/requires.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/top_level.txt
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-15 02:12:36.649740 butter-cli-1.11/
+-rw-r--r--   0 michaelequi   (501) staff       (20)      196 2023-04-15 02:12:36.648788 butter-cli-1.11/PKG-INFO
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-15 02:12:36.642907 butter-cli-1.11/butter_cli.egg-info/
+-rw-r--r--   0 michaelequi   (501) staff       (20)      145 2023-04-14 01:30:14.000000 butter-cli-1.11/butter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 michaelequi   (501) staff       (20)      239 2023-04-14 01:28:01.000000 butter-cli-1.11/butter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-14 01:30:14.000000 butter-cli-1.11/butter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-14 01:30:14.000000 butter-cli-1.11/butter_cli.egg-info/requires.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-14 01:30:14.000000 butter-cli-1.11/butter_cli.egg-info/top_level.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       38 2023-04-15 02:12:36.650122 butter-cli-1.11/setup.cfg
+-rw-r--r--   0 michaelequi   (501) staff       (20)      639 2023-04-15 02:10:27.000000 butter-cli-1.11/setup.py
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-15 02:12:36.639829 butter-cli-1.11/src/
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-15 02:12:36.644794 butter-cli-1.11/src/butter/
+-rw-r--r--   0 michaelequi   (501) staff       (20)       51 2023-04-14 01:34:57.000000 butter-cli-1.11/src/butter/__init__.py
+-rw-r--r--   0 michaelequi   (501) staff       (20)     3796 2023-04-15 02:11:11.000000 butter-cli-1.11/src/butter/butter.py
+-rw-r--r--   0 michaelequi   (501) staff       (20)     1140 2023-01-29 05:31:52.000000 butter-cli-1.11/src/butter/cli.py
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-15 02:12:36.647649 butter-cli-1.11/src/butter_cli.egg-info/
+-rw-r--r--   0 michaelequi   (501) staff       (20)      196 2023-04-15 02:12:36.000000 butter-cli-1.11/src/butter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 michaelequi   (501) staff       (20)      469 2023-04-15 02:12:36.000000 butter-cli-1.11/src/butter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-15 02:12:36.000000 butter-cli-1.11/src/butter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       42 2023-04-15 02:12:36.000000 butter-cli-1.11/src/butter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-15 02:12:36.000000 butter-cli-1.11/src/butter_cli.egg-info/requires.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-15 02:12:36.000000 butter-cli-1.11/src/butter_cli.egg-info/top_level.txt
```

### Comparing `butter-cli-1.1/setup.py` & `butter-cli-1.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name='butter-cli',
-   version='1.1',
+   version='1.11',
    description='CI/CD for generative AI',
    author='Michael Equi',
    author_email='michaelequi@berkeley.edu',
    packages=find_packages('src'),  #same as name
    package_dir={'': 'src'},
    entry_points={
         'console_scripts': [
```

### Comparing `butter-cli-1.1/src/butter/butter.py` & `butter-cli-1.11/src/butter/butter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     return dec
 
 class Butter:
     tests = []
 
     def __init__(self) -> None:
         self.console = Console()
-        # self.url = "https://butter-production.up.railway.app/run_analytics"
-        self.url = "http://127.0.0.1:5000/run_analytics"
+        self.url = "https://butter-production.up.railway.app/run_analytics"
 
     def run_tests(self, path: Path, id, description: str, debug=False):
         self.console.print(f":sunglasses: Running tests...\n")
 
         tests = []
         json_files = set()
         for test, json_file, desc in Butter.tests:
```

### Comparing `butter-cli-1.1/src/butter/cli.py` & `butter-cli-1.11/src/butter/cli.py`

 * *Files identical despite different names*

