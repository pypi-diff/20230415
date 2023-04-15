# Comparing `tmp/xurls-0.2.0.tar.gz` & `tmp/xurls-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xurls-0.2.0.tar", max compression
+gzip compressed data, was "xurls-0.2.1.tar", max compression
```

## Comparing `xurls-0.2.0.tar` & `xurls-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-04-06 17:13:23.242882 xurls-0.2.0/LICENSE
--rw-r--r--   0        0        0      493 2023-04-06 17:13:23.242882 xurls-0.2.0/README.md
--rw-r--r--   0        0        0     1898 2023-04-06 17:13:23.246882 xurls-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      130 2023-04-06 17:13:23.246882 xurls-0.2.0/xurls/__init__.py
--rw-r--r--   0        0        0    56900 2023-04-06 17:13:23.246882 xurls-0.2.0/xurls/url.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 xurls-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:12:48.420120 xurls-0.2.1/LICENSE
+-rw-r--r--   0        0        0      839 2023-04-15 14:12:48.420120 xurls-0.2.1/README.md
+-rw-r--r--   0        0        0     2005 2023-04-15 14:12:48.424120 xurls-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-04-15 14:12:48.424120 xurls-0.2.1/xurls/__init__.py
+-rw-r--r--   0        0        0    56900 2023-04-15 14:12:48.424120 xurls-0.2.1/xurls/url.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 xurls-0.2.1/PKG-INFO
```

### Comparing `xurls-0.2.0/LICENSE` & `xurls-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xurls-0.2.0/pyproject.toml` & `xurls-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "xurls"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python URL Library"
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xurls"}]
 readme = "README.md"
-license = "The Unlicense (Unlicense)"
 repository = "https://github.com/xyngular/py-xurls"
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 xsentinels = "^1.2.1"
 xloop = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `xurls-0.2.0/xurls/url.py` & `xurls-0.2.1/xurls/url.py`

 * *Files identical despite different names*

