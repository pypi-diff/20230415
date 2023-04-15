# Comparing `tmp/learning-apis-0.1.tar.gz` & `tmp/learning-apis-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning-apis-0.1.tar", last modified: Sat Apr 15 00:32:08 2023, max compression
+gzip compressed data, was "learning-apis-0.2.tar", last modified: Sat Apr 15 00:56:16 2023, max compression
```

## Comparing `learning-apis-0.1.tar` & `learning-apis-0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 joaopaulo   (501) staff       (20)        0 2023-04-15 00:32:08.352397 learning-apis-0.1/
--rw-r--r--   0 joaopaulo   (501) staff       (20)       77 2023-04-15 00:32:08.352262 learning-apis-0.1/PKG-INFO
-drwxr-xr-x   0 joaopaulo   (501) staff       (20)        0 2023-04-15 00:32:08.352071 learning-apis-0.1/learning_apis.egg-info/
--rw-r--r--   0 joaopaulo   (501) staff       (20)       77 2023-04-15 00:32:08.000000 learning-apis-0.1/learning_apis.egg-info/PKG-INFO
--rw-r--r--   0 joaopaulo   (501) staff       (20)      192 2023-04-15 00:32:08.000000 learning-apis-0.1/learning_apis.egg-info/SOURCES.txt
--rw-r--r--   0 joaopaulo   (501) staff       (20)        1 2023-04-15 00:32:08.000000 learning-apis-0.1/learning_apis.egg-info/dependency_links.txt
--rw-r--r--   0 joaopaulo   (501) staff       (20)       18 2023-04-15 00:32:08.000000 learning-apis-0.1/learning_apis.egg-info/requires.txt
--rw-r--r--   0 joaopaulo   (501) staff       (20)        1 2023-04-15 00:32:08.000000 learning-apis-0.1/learning_apis.egg-info/top_level.txt
--rw-r--r--   0 joaopaulo   (501) staff       (20)       38 2023-04-15 00:32:08.352436 learning-apis-0.1/setup.cfg
--rw-r--r--   0 joaopaulo   (501) staff       (20)      262 2023-04-15 00:21:39.000000 learning-apis-0.1/setup.py
+drwxr-xr-x   0 joaopaulo   (501) staff       (20)        0 2023-04-15 00:56:16.204797 learning-apis-0.2/
+-rw-r--r--   0 joaopaulo   (501) staff       (20)       77 2023-04-15 00:56:16.204664 learning-apis-0.2/PKG-INFO
+-rw-r--r--   0 joaopaulo   (501) staff       (20)       16 2023-03-03 17:39:56.000000 learning-apis-0.2/README.md
+drwxr-xr-x   0 joaopaulo   (501) staff       (20)        0 2023-04-15 00:56:16.204507 learning-apis-0.2/learning_apis.egg-info/
+-rw-r--r--   0 joaopaulo   (501) staff       (20)       77 2023-04-15 00:56:16.000000 learning-apis-0.2/learning_apis.egg-info/PKG-INFO
+-rw-r--r--   0 joaopaulo   (501) staff       (20)      208 2023-04-15 00:56:16.000000 learning-apis-0.2/learning_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 joaopaulo   (501) staff       (20)        1 2023-04-15 00:56:16.000000 learning-apis-0.2/learning_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 joaopaulo   (501) staff       (20)       18 2023-04-15 00:56:16.000000 learning-apis-0.2/learning_apis.egg-info/requires.txt
+-rw-r--r--   0 joaopaulo   (501) staff       (20)        1 2023-04-15 00:56:16.000000 learning-apis-0.2/learning_apis.egg-info/top_level.txt
+-rw-r--r--   0 joaopaulo   (501) staff       (20)      174 2023-03-03 17:35:02.000000 learning-apis-0.2/pyproject.toml
+-rw-r--r--   0 joaopaulo   (501) staff       (20)       38 2023-04-15 00:56:16.204834 learning-apis-0.2/setup.cfg
```

