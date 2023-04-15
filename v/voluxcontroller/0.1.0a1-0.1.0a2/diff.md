# Comparing `tmp/voluxcontroller-0.1.0a1.tar.gz` & `tmp/voluxcontroller-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voluxcontroller-0.1.0a1.tar", max compression
+gzip compressed data, was "voluxcontroller-0.1.0a2.tar", max compression
```

## Comparing `voluxcontroller-0.1.0a1.tar` & `voluxcontroller-0.1.0a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       25 2023-04-15 06:26:05.920860 voluxcontroller-0.1.0a1/README.md
--rw-r--r--   0        0        0      777 2023-04-15 08:02:14.129366 voluxcontroller-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     3536 2023-04-15 07:56:58.484774 voluxcontroller-0.1.0a1/voluxcontroller/__init__.py
--rw-r--r--   0        0        0      114 2023-04-15 08:03:17.481026 voluxcontroller-0.1.0a1/voluxcontroller/__version__.py
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 voluxcontroller-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1892 2023-04-15 08:27:57.092203 voluxcontroller-0.1.0a2/README.md
+-rw-r--r--   0        0        0      777 2023-04-15 08:29:32.158428 voluxcontroller-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3536 2023-04-15 07:56:58.484774 voluxcontroller-0.1.0a2/voluxcontroller/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-15 08:29:38.742321 voluxcontroller-0.1.0a2/voluxcontroller/__version__.py
+-rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 voluxcontroller-0.1.0a2/PKG-INFO
```

### Comparing `voluxcontroller-0.1.0a1/pyproject.toml` & `voluxcontroller-0.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voluxcontroller"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Controller/gamepad interface for Volux"
 authors = ["DrTexx <denver.opensource@tutanota.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://gitlab.com/volux/volux/"
 # TODO: add extra project details (e.g. keywords, classifiers, etc.)
```

### Comparing `voluxcontroller-0.1.0a1/voluxcontroller/__init__.py` & `voluxcontroller-0.1.0a2/voluxcontroller/__init__.py`

 * *Files identical despite different names*

