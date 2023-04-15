# Comparing `tmp/hlatypingtools-0.1.1.tar.gz` & `tmp/hlatypingtools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlatypingtools-0.1.1.tar", max compression
+gzip compressed data, was "hlatypingtools-1.0.0.tar", max compression
```

## Comparing `hlatypingtools-0.1.1.tar` & `hlatypingtools-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-14 14:02:29.564981 hlatypingtools-0.1.1/hlatypingtools/__init__.py
--rw-r--r--   0        0        0      558 2023-04-14 15:43:18.514188 hlatypingtools-0.1.1/hlatypingtools/decrypt_file.py
--rw-r--r--   0        0        0      529 2023-04-14 15:44:09.067655 hlatypingtools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1178 2023-04-14 15:43:57.953770 hlatypingtools-0.1.1/README.md
--rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 hlatypingtools-0.1.1/setup.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 hlatypingtools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 14:02:29.564981 hlatypingtools-1.0.0/hlatypingtools/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-14 16:08:15.663091 hlatypingtools-1.0.0/hlatypingtools/decrypt_file.py
+-rw-r--r--   0        0        0     2950 2023-04-14 16:51:00.238909 hlatypingtools-1.0.0/hlatypingtools/get_info.py
+-rw-r--r--   0        0        0      529 2023-04-14 16:58:58.541951 hlatypingtools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2721 2023-04-14 17:10:41.358676 hlatypingtools-1.0.0/README.md
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 hlatypingtools-1.0.0/setup.py
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 hlatypingtools-1.0.0/PKG-INFO
```

### Comparing `hlatypingtools-0.1.1/pyproject.toml` & `hlatypingtools-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hlatypingtools"
-version = "0.1.1"
+version = "1.0.0"
 description = ""
 authors = ["JasonMendoza2008 <lhotteromain@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.0"
```

