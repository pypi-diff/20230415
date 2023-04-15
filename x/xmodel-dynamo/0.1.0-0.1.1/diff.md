# Comparing `tmp/xmodel_dynamo-0.1.0.tar.gz` & `tmp/xmodel_dynamo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmodel_dynamo-0.1.0.tar", max compression
+gzip compressed data, was "xmodel_dynamo-0.1.1.tar", max compression
```

## Comparing `xmodel_dynamo-0.1.0.tar` & `xmodel_dynamo-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      352 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/README.md
--rw-r--r--   0        0        0     1740 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    22428 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/__init__.py
--rw-r--r--   0        0        0     5425 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/api.py
--rw-r--r--   0        0        0    33004 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/client.py
--rw-r--r--   0        0        0    14373 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/common_types.py
--rw-r--r--   0        0        0     5722 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/db.py
--rw-r--r--   0        0        0       45 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/errors.py
--rw-r--r--   0        0        0     1058 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/fields.py
--rw-r--r--   0        0        0       25 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/meta.json
--rw-r--r--   0        0        0     2061 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/model.py
--rw-r--r--   0        0        0     5528 2023-04-15 03:33:20.024589 xmodel_dynamo-0.1.0/xmodel_dynamo/resources.py
--rw-r--r--   0        0        0     8678 2023-04-15 03:33:20.028589 xmodel_dynamo-0.1.0/xmodel_dynamo/structure.py
--rw-r--r--   0        0        0      161 2023-04-15 03:33:20.028589 xmodel_dynamo-0.1.0/xmodel_dynamo/utils.py
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 xmodel_dynamo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      722 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/README.md
+-rw-r--r--   0        0        0     1849 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    22428 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/__init__.py
+-rw-r--r--   0        0        0     5425 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/api.py
+-rw-r--r--   0        0        0    33004 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/client.py
+-rw-r--r--   0        0        0    14373 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/common_types.py
+-rw-r--r--   0        0        0     5722 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/db.py
+-rw-r--r--   0        0        0       45 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/errors.py
+-rw-r--r--   0        0        0     1058 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/fields.py
+-rw-r--r--   0        0        0       25 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/meta.json
+-rw-r--r--   0        0        0     2061 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/model.py
+-rw-r--r--   0        0        0     5528 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/resources.py
+-rw-r--r--   0        0        0     8678 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/structure.py
+-rw-r--r--   0        0        0      161 2023-04-15 14:12:47.946731 xmodel_dynamo-0.1.1/xmodel_dynamo/utils.py
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 xmodel_dynamo-0.1.1/PKG-INFO
```

### Comparing `xmodel_dynamo-0.1.0/pyproject.toml` & `xmodel_dynamo-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "xmodel_dynamo"
-version = "0.1.0"
+version = "0.1.1"
 description = "Use dynamo with xmodel objects."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xmodel_dynamo"}]
 readme = "README.md"
-license = "The Unlicense (Unlicense)"
-repository = "https://github.com/xyngular/py-xmodel-rest"
+repository = "https://github.com/xyngular/py-xmodel-dynamo"
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
+]
 
 [tool.poetry.dependencies]
 python = "~3.8"
 boto3 = "^1.17.54"
 #xyn-aws = "^1.1.1"
 #xyn-config = "^1.2.2"
 #xyn-model = "^1.1.0"
```

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/__init__.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/__init__.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/api.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/api.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/client.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/client.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/common_types.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/common_types.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/db.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/db.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/fields.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/fields.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/model.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/model.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/resources.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/resources.py`

 * *Files identical despite different names*

### Comparing `xmodel_dynamo-0.1.0/xmodel_dynamo/structure.py` & `xmodel_dynamo-0.1.1/xmodel_dynamo/structure.py`

 * *Files identical despite different names*

