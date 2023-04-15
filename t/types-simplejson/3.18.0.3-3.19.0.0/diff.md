# Comparing `tmp/types-simplejson-3.18.0.3.tar.gz` & `tmp/types-simplejson-3.19.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-simplejson-3.18.0.3.tar", last modified: Wed Mar 29 12:34:49 2023, max compression
+gzip compressed data, was "types-simplejson-3.19.0.0.tar", last modified: Sat Apr 15 09:13:39 2023, max compression
```

## Comparing `types-simplejson-3.18.0.3.tar` & `types-simplejson-3.19.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:34:49.615064 types-simplejson-3.18.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-29 12:34:49.615064 types-simplejson-3.18.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 12:34:49.615064 types-simplejson-3.18.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:34:49.615064 types-simplejson-3.18.0.3/simplejson-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/simplejson-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-29 12:34:30.000000 types-simplejson-3.18.0.3/simplejson-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-29 12:34:30.000000 types-simplejson-3.18.0.3/simplejson-stubs/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-29 12:34:30.000000 types-simplejson-3.18.0.3/simplejson-stubs/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-29 12:34:30.000000 types-simplejson-3.18.0.3/simplejson-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-29 12:34:30.000000 types-simplejson-3.18.0.3/simplejson-stubs/raw_json.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-29 12:34:30.000000 types-simplejson-3.18.0.3/simplejson-stubs/scanner.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:34:49.615064 types-simplejson-3.18.0.3/types_simplejson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/types_simplejson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/types_simplejson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/types_simplejson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-29 12:34:49.000000 types-simplejson-3.18.0.3/types_simplejson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:13:39.284710 types-simplejson-3.19.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-15 09:13:38.000000 types-simplejson-3.19.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 09:13:38.000000 types-simplejson-3.19.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 09:13:39.284710 types-simplejson-3.19.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 09:13:39.284710 types-simplejson-3.19.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-15 09:13:38.000000 types-simplejson-3.19.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:13:39.284710 types-simplejson-3.19.0.0/simplejson-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-15 09:13:38.000000 types-simplejson-3.19.0.0/simplejson-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-15 09:13:27.000000 types-simplejson-3.19.0.0/simplejson-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-15 09:13:27.000000 types-simplejson-3.19.0.0/simplejson-stubs/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-15 09:13:27.000000 types-simplejson-3.19.0.0/simplejson-stubs/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-15 09:13:27.000000 types-simplejson-3.19.0.0/simplejson-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 09:13:27.000000 types-simplejson-3.19.0.0/simplejson-stubs/raw_json.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-15 09:13:27.000000 types-simplejson-3.19.0.0/simplejson-stubs/scanner.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:13:39.284710 types-simplejson-3.19.0.0/types_simplejson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 09:13:39.000000 types-simplejson-3.19.0.0/types_simplejson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-15 09:13:39.000000 types-simplejson-3.19.0.0/types_simplejson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 09:13:39.000000 types-simplejson-3.19.0.0/types_simplejson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 09:13:39.000000 types-simplejson-3.19.0.0/types_simplejson.egg-info/top_level.txt
```

### Comparing `types-simplejson-3.18.0.3/CHANGELOG.md` & `types-simplejson-3.19.0.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.19.0.0 (2023-04-15)
+
+Bump simplejson to 3.19.* (#10049)
+
 ## 3.18.0.3 (2023-03-29)
 
 Remove unnecessary ellipsis expressions (#9976)
 
 Ignore flake8 F821 warnings in stub files
 
 ## 3.18.0.2 (2023-03-28)
```

### Comparing `types-simplejson-3.18.0.3/PKG-INFO` & `types-simplejson-3.19.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-simplejson
-Version: 3.18.0.3
+Version: 3.19.0.0
 Summary: Typing stubs for simplejson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/simplejson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `simplejson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/simplejson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ed915c5cde48329e3d1e597e60c4baee27b7854a`.
+This package was generated from typeshed commit `7dcec5b3db887f518114486b3e4783dde244186d`.
```

### Comparing `types-simplejson-3.18.0.3/setup.py` & `types-simplejson-3.19.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `simplejson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/simplejson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ed915c5cde48329e3d1e597e60c4baee27b7854a`.
+This package was generated from typeshed commit `7dcec5b3db887f518114486b3e4783dde244186d`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.18.0.3",
+      version="3.19.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/simplejson.md",
```

### Comparing `types-simplejson-3.18.0.3/simplejson-stubs/__init__.pyi` & `types-simplejson-3.19.0.0/simplejson-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-simplejson-3.18.0.3/simplejson-stubs/errors.pyi` & `types-simplejson-3.19.0.0/simplejson-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-simplejson-3.18.0.3/types_simplejson.egg-info/PKG-INFO` & `types-simplejson-3.19.0.0/types_simplejson.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-simplejson
-Version: 3.18.0.3
+Version: 3.19.0.0
 Summary: Typing stubs for simplejson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/simplejson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `simplejson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/simplejson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ed915c5cde48329e3d1e597e60c4baee27b7854a`.
+This package was generated from typeshed commit `7dcec5b3db887f518114486b3e4783dde244186d`.
```

