# Comparing `tmp/vidya-0.1.0.tar.gz` & `tmp/vidya-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidya-0.1.0.tar", max compression
+gzip compressed data, was "vidya-0.1.1.tar", max compression
```

## Comparing `vidya-0.1.0.tar` & `vidya-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        5 2023-04-15 20:46:19.056343 vidya-0.1.0/README.md
--rw-r--r--   0        0        0      426 2023-04-15 21:12:59.383708 vidya-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-15 09:00:16.596670 vidya-0.1.0/vidya/__init__.py
--rw-r--r--   0        0        0       49 2023-04-15 21:12:59.653707 vidya-0.1.0/vidya/__main__.py
--rw-r--r--   0        0        0      113 2023-04-15 21:12:59.710663 vidya-0.1.0/vidya/main.py
--rw-r--r--   0        0        0      917 2023-04-15 21:12:59.609001 vidya-0.1.0/vidya/transform.py
--rw-r--r--   0        0        0        0 2023-04-15 17:36:03.668006 vidya-0.1.0/vidya/utils/__init__.py
--rw-r--r--   0        0        0      152 2023-04-15 18:42:33.311154 vidya-0.1.0/vidya/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3200 2023-04-15 20:07:29.361665 vidya-0.1.0/vidya/utils/__pycache__/css_to_csv.cpython-311.pyc
--rw-r--r--   0        0        0      764 2023-04-15 20:10:01.807589 vidya-0.1.0/vidya/utils/__pycache__/os.cpython-311.pyc
--rw-r--r--   0        0        0     1263 2023-04-15 20:07:28.750351 vidya-0.1.0/vidya/utils/css_to_csv.py
--rw-r--r--   0        0        0      172 2023-04-15 20:10:01.131696 vidya-0.1.0/vidya/utils/os.py
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 vidya-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2023-04-15 21:13:45.178792 vidya-0.1.1/README.md
+-rw-r--r--   0        0        0      476 2023-04-15 21:14:25.615088 vidya-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-15 09:00:16.596670 vidya-0.1.1/vidya/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-15 21:12:59.653707 vidya-0.1.1/vidya/__main__.py
+-rw-r--r--   0        0        0      113 2023-04-15 21:12:59.710663 vidya-0.1.1/vidya/main.py
+-rw-r--r--   0        0        0      917 2023-04-15 21:12:59.609001 vidya-0.1.1/vidya/transform.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:36:03.668006 vidya-0.1.1/vidya/utils/__init__.py
+-rw-r--r--   0        0        0      152 2023-04-15 18:42:33.311154 vidya-0.1.1/vidya/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3200 2023-04-15 20:07:29.361665 vidya-0.1.1/vidya/utils/__pycache__/css_to_csv.cpython-311.pyc
+-rw-r--r--   0        0        0      764 2023-04-15 20:10:01.807589 vidya-0.1.1/vidya/utils/__pycache__/os.cpython-311.pyc
+-rw-r--r--   0        0        0     1263 2023-04-15 20:07:28.750351 vidya-0.1.1/vidya/utils/css_to_csv.py
+-rw-r--r--   0        0        0      172 2023-04-15 20:10:01.131696 vidya-0.1.1/vidya/utils/os.py
+-rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 vidya-0.1.1/PKG-INFO
```

### Comparing `vidya-0.1.0/vidya/transform.py` & `vidya-0.1.1/vidya/transform.py`

 * *Files identical despite different names*

### Comparing `vidya-0.1.0/vidya/utils/__pycache__/css_to_csv.cpython-311.pyc` & `vidya-0.1.1/vidya/utils/__pycache__/css_to_csv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vidya-0.1.0/vidya/utils/__pycache__/os.cpython-311.pyc` & `vidya-0.1.1/vidya/utils/__pycache__/os.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vidya-0.1.0/vidya/utils/css_to_csv.py` & `vidya-0.1.1/vidya/utils/css_to_csv.py`

 * *Files identical despite different names*

