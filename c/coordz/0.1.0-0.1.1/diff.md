# Comparing `tmp/coordz-0.1.0.tar.gz` & `tmp/coordz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coordz-0.1.0.tar", max compression
+gzip compressed data, was "coordz-0.1.1.tar", max compression
```

## Comparing `coordz-0.1.0.tar` & `coordz-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       14 2023-04-14 23:54:41.149446 coordz-0.1.0/README.md
--rw-r--r--   0        0        0    16572 2023-04-15 00:00:23.979746 coordz-0.1.0/coordz/__init__.py
--rw-r--r--   0        0        0      266 2023-04-14 23:59:07.650624 coordz-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 coordz-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-04-14 23:54:41.149446 coordz-0.1.1/README.md
+-rw-r--r--   0        0        0    16572 2023-04-15 00:00:23.979746 coordz-0.1.1/coordz/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-15 00:04:57.798797 coordz-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 coordz-0.1.1/PKG-INFO
```

### Comparing `coordz-0.1.0/coordz/__init__.py` & `coordz-0.1.1/coordz/__init__.py`

 * *Files identical despite different names*

