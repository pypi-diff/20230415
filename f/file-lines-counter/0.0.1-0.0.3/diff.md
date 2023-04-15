# Comparing `tmp/file lines counter-0.0.1.tar.gz` & `tmp/file lines counter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file lines counter-0.0.1.tar", last modified: Sat Apr 15 07:29:57 2023, max compression
+gzip compressed data, was "file lines counter-0.0.3.tar", last modified: Sat Apr 15 07:42:26 2023, max compression
```

## Comparing `file lines counter-0.0.1.tar` & `file lines counter-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2023-04-15 07:29:57.567438 file lines counter-0.0.1/
--rw-r--r--   0 makbuk     (501) staff       (20)      295 2023-04-15 07:29:57.567053 file lines counter-0.0.1/PKG-INFO
-drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2023-04-15 07:29:57.564975 file lines counter-0.0.1/file_lines_counter.egg-info/
--rw-r--r--   0 makbuk     (501) staff       (20)      295 2023-04-15 07:29:57.000000 file lines counter-0.0.1/file_lines_counter.egg-info/PKG-INFO
--rw-r--r--   0 makbuk     (501) staff       (20)      308 2023-04-15 07:29:57.000000 file lines counter-0.0.1/file_lines_counter.egg-info/SOURCES.txt
--rw-r--r--   0 makbuk     (501) staff       (20)        1 2023-04-15 07:29:57.000000 file lines counter-0.0.1/file_lines_counter.egg-info/dependency_links.txt
--rw-r--r--   0 makbuk     (501) staff       (20)       42 2023-04-15 07:29:57.000000 file lines counter-0.0.1/file_lines_counter.egg-info/entry_points.txt
--rw-r--r--   0 makbuk     (501) staff       (20)        6 2023-04-15 07:29:57.000000 file lines counter-0.0.1/file_lines_counter.egg-info/requires.txt
--rw-r--r--   0 makbuk     (501) staff       (20)        4 2023-04-15 07:29:57.000000 file lines counter-0.0.1/file_lines_counter.egg-info/top_level.txt
--rw-r--r--   0 makbuk     (501) staff       (20)       84 2023-04-15 07:24:20.000000 file lines counter-0.0.1/pyproject.toml
--rw-r--r--   0 makbuk     (501) staff       (20)       38 2023-04-15 07:29:57.567581 file lines counter-0.0.1/setup.cfg
--rw-r--r--   0 makbuk     (501) staff       (20)      554 2023-04-15 07:26:34.000000 file lines counter-0.0.1/setup.py
-drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2023-04-15 07:29:57.566038 file lines counter-0.0.1/src/
--rw-r--r--   0 makbuk     (501) staff       (20)        0 2023-04-15 07:22:47.000000 file lines counter-0.0.1/src/__init__.py
--rw-r--r--   0 makbuk     (501) staff       (20)      461 2023-04-15 06:46:07.000000 file lines counter-0.0.1/src/wc_util.py
+drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2023-04-15 07:42:26.857714 file lines counter-0.0.3/
+-rw-r--r--   0 makbuk     (501) staff       (20)      295 2023-04-15 07:42:26.857066 file lines counter-0.0.3/PKG-INFO
+drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2023-04-15 07:42:26.854918 file lines counter-0.0.3/file_lines_counter.egg-info/
+-rw-r--r--   0 makbuk     (501) staff       (20)      295 2023-04-15 07:42:26.000000 file lines counter-0.0.3/file_lines_counter.egg-info/PKG-INFO
+-rw-r--r--   0 makbuk     (501) staff       (20)      308 2023-04-15 07:42:26.000000 file lines counter-0.0.3/file_lines_counter.egg-info/SOURCES.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)        1 2023-04-15 07:42:26.000000 file lines counter-0.0.3/file_lines_counter.egg-info/dependency_links.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)       42 2023-04-15 07:42:26.000000 file lines counter-0.0.3/file_lines_counter.egg-info/entry_points.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)        6 2023-04-15 07:42:26.000000 file lines counter-0.0.3/file_lines_counter.egg-info/requires.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)        4 2023-04-15 07:42:26.000000 file lines counter-0.0.3/file_lines_counter.egg-info/top_level.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)       84 2023-04-15 07:24:20.000000 file lines counter-0.0.3/pyproject.toml
+-rw-r--r--   0 makbuk     (501) staff       (20)       38 2023-04-15 07:42:26.858040 file lines counter-0.0.3/setup.cfg
+-rw-r--r--   0 makbuk     (501) staff       (20)      554 2023-04-15 07:42:18.000000 file lines counter-0.0.3/setup.py
+drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2023-04-15 07:42:26.856124 file lines counter-0.0.3/src/
+-rw-r--r--   0 makbuk     (501) staff       (20)        0 2023-04-15 07:22:47.000000 file lines counter-0.0.3/src/__init__.py
+-rw-r--r--   0 makbuk     (501) staff       (20)      461 2023-04-15 06:46:07.000000 file lines counter-0.0.3/src/wc_util.py
```

### Comparing `file lines counter-0.0.1/setup.py` & `file lines counter-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 
 setuptools.setup(
     name="file lines counter",
-    version="0.0.1",
+    version="0.0.3",
     author="me",
     author_email="aa@example.com",
     description=("lines  counter"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["typer"],
     packages=setuptools.find_packages(),
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "count = src.wc_util:app",
         ]
     },
 )
```

