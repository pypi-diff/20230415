# Comparing `tmp/witch_doctor-0.1.2.tar.gz` & `tmp/witch_doctor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "witch_doctor-0.1.2.tar", max compression
+gzip compressed data, was "witch_doctor-1.0.0.tar", max compression
```

## Comparing `witch_doctor-0.1.2.tar` & `witch_doctor-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-02-03 23:22:13.304775 witch_doctor-0.1.2/LICENSE
--rw-r--r--   0        0        0     2224 2023-02-04 12:42:34.580417 witch_doctor-0.1.2/README.md
--rw-r--r--   0        0        0      541 2023-04-02 10:11:40.094451 witch_doctor-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1739 2023-04-02 10:11:40.094451 witch_doctor-0.1.2/witch_doctor/__init__.py
--rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 witch_doctor-0.1.2/setup.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 witch_doctor-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-03 23:22:13.304775 witch_doctor-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4247 2023-04-15 15:01:21.141450 witch_doctor-1.0.0/README.md
+-rw-r--r--   0        0        0      563 2023-04-15 14:42:15.751707 witch_doctor-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4952 2023-04-15 14:41:43.848483 witch_doctor-1.0.0/witch_doctor/__init__.py
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 witch_doctor-1.0.0/setup.py
+-rw-r--r--   0        0        0     4725 1970-01-01 00:00:00.000000 witch_doctor-1.0.0/PKG-INFO
```

### Comparing `witch_doctor-0.1.2/LICENSE` & `witch_doctor-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `witch_doctor-0.1.2/pyproject.toml` & `witch_doctor-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "witch-doctor"
-version = "0.1.2"
+version = "1.0.0"
 description = "Dependency injection for python"
 authors = ["Marco Sievers de Almeida Ximit Gaia <im.ximit@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "witch_doctor"},
     { include = "witch_doctor/**/*.py" },
@@ -13,11 +13,12 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mutatest = "^3.1.0"
 pylint = "^2.15.10"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

