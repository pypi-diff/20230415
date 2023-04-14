# Comparing `tmp/sopel_modules.twitter-0.4.1.tar.gz` & `tmp/sopel_modules.twitter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules.twitter-0.4.1.tar", last modified: Fri Mar  4 16:43:04 2022, max compression
+gzip compressed data, was "sopel_modules.twitter-1.0.0.tar", last modified: Fri Apr 14 22:00:33 2023, max compression
```

## Comparing `sopel_modules.twitter-0.4.1.tar` & `sopel_modules.twitter-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,18 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-03-04 16:43:04.544609 sopel_modules.twitter-0.4.1/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1746 2022-03-04 16:41:57.000000 sopel_modules.twitter-0.4.1/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     3977 2022-03-04 16:43:04.544109 sopel_modules.twitter-0.4.1/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1905 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/dev-requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       23 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       38 2022-03-04 16:43:04.544609 sopel_modules.twitter-0.4.1/setup.cfg
--rwxr-xr-x   0 dgw       (1000) dgw       (1000)     1408 2022-03-04 16:42:03.000000 sopel_modules.twitter-0.4.1/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-03-04 16:43:04.513608 sopel_modules.twitter-0.4.1/sopel_modules/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       56 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/sopel_modules/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-03-04 16:43:04.541108 sopel_modules.twitter-0.4.1/sopel_modules/twitter/
--rw-r--r--   0 dgw       (1000) dgw       (1000)      246 2022-03-04 16:42:10.000000 sopel_modules.twitter-0.4.1/sopel_modules/twitter/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)    10665 2022-03-04 16:39:39.000000 sopel_modules.twitter-0.4.1/sopel_modules/twitter/twitter.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-03-04 16:43:04.538608 sopel_modules.twitter-0.4.1/sopel_modules.twitter.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     3977 2022-03-04 16:43:03.000000 sopel_modules.twitter-0.4.1/sopel_modules.twitter.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      492 2022-03-04 16:43:03.000000 sopel_modules.twitter-0.4.1/sopel_modules.twitter.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2022-03-04 16:43:03.000000 sopel_modules.twitter-0.4.1/sopel_modules.twitter.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2022-03-04 16:43:03.000000 sopel_modules.twitter-0.4.1/sopel_modules.twitter.egg-info/namespace_packages.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       23 2022-03-04 16:43:03.000000 sopel_modules.twitter-0.4.1/sopel_modules.twitter.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2022-03-04 16:43:03.000000 sopel_modules.twitter-0.4.1/sopel_modules.twitter.egg-info/top_level.txt
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-03-04 16:43:04.543107 sopel_modules.twitter-0.4.1/tests/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/tests/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2022-03-02 18:17:04.000000 sopel_modules.twitter-0.4.1/tests/test_twitter.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 22:00:33.301056 sopel_modules.twitter-1.0.0/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel_modules.twitter-1.0.0/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      134 2023-04-14 21:53:42.000000 sopel_modules.twitter-1.0.0/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1874 2023-04-14 21:52:02.000000 sopel_modules.twitter-1.0.0/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     3155 2023-04-14 22:00:33.300056 sopel_modules.twitter-1.0.0/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      174 2023-04-14 21:50:42.000000 sopel_modules.twitter-1.0.0/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       21 2023-04-14 21:57:08.000000 sopel_modules.twitter-1.0.0/requirements.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       38 2023-04-14 22:00:33.301056 sopel_modules.twitter-1.0.0/setup.cfg
+-rwxr-xr-x   0 dgw       (1000) dgw       (1000)     1213 2023-04-14 21:52:19.000000 sopel_modules.twitter-1.0.0/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 22:00:33.287059 sopel_modules.twitter-1.0.0/sopel_modules/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       56 2023-04-14 21:48:28.000000 sopel_modules.twitter-1.0.0/sopel_modules/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-14 22:00:33.299064 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     3155 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      364 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/namespace_packages.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       21 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2023-04-14 22:00:33.000000 sopel_modules.twitter-1.0.0/sopel_modules.twitter.egg-info/top_level.txt
```

### Comparing `sopel_modules.twitter-0.4.1/COPYING` & `sopel_modules.twitter-1.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `sopel_modules.twitter-0.4.1/NEWS` & `sopel_modules.twitter-1.0.0/NEWS`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Changes between 0.4.1 and 1.0.0
+===============================
+
+**Package renamed. Please install `sopel-twitter` instead.**
+
+
 Changes between 0.4.0 and 0.4.1
 ===============================
 
 Fixed:
 * Detecting user profile links with trailing slash or query params (#28)
 * Error when quoted tweet has been deleted (#31)
```

### Comparing `sopel_modules.twitter-0.4.1/setup.py` & `sopel_modules.twitter-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,28 +17,23 @@
 
 with open('NEWS') as history_file:
     history = history_file.read()
 
 with open('requirements.txt') as requirements_file:
     requirements = [req for req in requirements_file.readlines()]
 
-with open('dev-requirements.txt') as dev_requirements_file:
-    dev_requirements = [req for req in dev_requirements_file.readlines()]
-
 
 setup(
     name='sopel_modules.twitter',
-    version='0.4.1',
+    version='1.0.0',
     description='A Twitter plugin for Sopel',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='dgw',
     author_email='dgw@technobabbl.es',
     url='https://github.com/sopel-irc/sopel-twitter',
     packages=find_packages('.'),
     namespace_packages=['sopel_modules'],
     include_package_data=True,
     install_requires=requirements,
-    tests_require=dev_requirements,
-    test_suite='tests',
     license='Eiffel Forum License, version 2',
 )
```

