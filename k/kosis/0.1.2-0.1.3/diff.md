# Comparing `tmp/kosis-0.1.2.tar.gz` & `tmp/kosis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kosis-0.1.2.tar", last modified: Sat Apr 15 18:06:20 2023, max compression
+gzip compressed data, was "kosis-0.1.3.tar", last modified: Sat Apr 15 19:03:40 2023, max compression
```

## Comparing `kosis-0.1.2.tar` & `kosis-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-15 18:06:20.054452 kosis-0.1.2/
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)     1080 2023-04-15 17:00:21.000000 kosis-0.1.2/LICENSE
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      642 2023-04-15 18:06:20.054452 kosis-0.1.2/PKG-INFO
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      182 2023-04-15 16:43:13.000000 kosis-0.1.2/README.md
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      533 2023-04-15 18:04:51.000000 kosis-0.1.2/pyproject.toml
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)       38 2023-04-15 18:06:20.054452 kosis-0.1.2/setup.cfg
-drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-15 18:06:20.054452 kosis-0.1.2/src/
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)       24 2023-04-15 17:30:14.000000 kosis-0.1.2/src/__init__.py
-drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-15 18:06:20.054452 kosis-0.1.2/src/kosis.egg-info/
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      642 2023-04-15 18:06:20.000000 kosis-0.1.2/src/kosis.egg-info/PKG-INFO
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      193 2023-04-15 18:06:20.000000 kosis-0.1.2/src/kosis.egg-info/SOURCES.txt
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)        1 2023-04-15 18:06:20.000000 kosis-0.1.2/src/kosis.egg-info/dependency_links.txt
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)       15 2023-04-15 18:06:20.000000 kosis-0.1.2/src/kosis.egg-info/top_level.txt
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)     6461 2023-04-15 17:15:39.000000 kosis-0.1.2/src/kosis.py
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-15 19:03:40.084461 kosis-0.1.3/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)     1080 2023-04-15 17:00:21.000000 kosis-0.1.3/LICENSE
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      642 2023-04-15 19:03:40.084461 kosis-0.1.3/PKG-INFO
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      182 2023-04-15 16:43:13.000000 kosis-0.1.3/README.md
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      643 2023-04-15 19:02:36.000000 kosis-0.1.3/pyproject.toml
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)       38 2023-04-15 19:03:40.084461 kosis-0.1.3/setup.cfg
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-15 19:03:40.084461 kosis-0.1.3/src/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)       24 2023-04-15 18:51:15.000000 kosis-0.1.3/src/__init__.py
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-15 19:03:40.084461 kosis-0.1.3/src/kosis.egg-info/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      642 2023-04-15 19:03:40.000000 kosis-0.1.3/src/kosis.egg-info/PKG-INFO
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      245 2023-04-15 19:03:40.000000 kosis-0.1.3/src/kosis.egg-info/SOURCES.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)        1 2023-04-15 19:03:40.000000 kosis-0.1.3/src/kosis.egg-info/dependency_links.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)       76 2023-04-15 19:03:40.000000 kosis-0.1.3/src/kosis.egg-info/requires.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)       15 2023-04-15 19:03:40.000000 kosis-0.1.3/src/kosis.egg-info/top_level.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)     6733 2023-04-15 19:01:19.000000 kosis-0.1.3/src/kosis.py
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-15 19:03:40.084461 kosis-0.1.3/tests/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      563 2023-04-15 18:52:05.000000 kosis-0.1.3/tests/test_kosis.py
```

### Comparing `kosis-0.1.2/LICENSE` & `kosis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kosis-0.1.2/PKG-INFO` & `kosis-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kosis
-Version: 0.1.2
+Version: 0.1.3
 Summary: KOSIS API
 Author-email: etinum <etinum@gmail.com>
 Project-URL: Homepage, https://github.com/etinum/kosis
 Project-URL: Bug Tracker, https://github.com/etinum/kosis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kosis-0.1.2/pyproject.toml` & `kosis-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kosis"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="etinum", email="etinum@gmail.com" },
 ]
 description = "KOSIS API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "pandas",
+  "plotly",
+  "django>2.1; os_name != 'nt'",
+  "django>2.0; os_name == 'nt'",
+]
+
 
 [project.urls]
 "Homepage" = "https://github.com/etinum/kosis"
 "Bug Tracker" = "https://github.com/etinum/kosis/issues"
```

### Comparing `kosis-0.1.2/src/kosis.egg-info/PKG-INFO` & `kosis-0.1.3/src/kosis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kosis
-Version: 0.1.2
+Version: 0.1.3
 Summary: KOSIS API
 Author-email: etinum <etinum@gmail.com>
 Project-URL: Homepage, https://github.com/etinum/kosis
 Project-URL: Bug Tracker, https://github.com/etinum/kosis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kosis-0.1.2/src/kosis.py` & `kosis-0.1.3/src/kosis.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,22 +24,29 @@
 
 def safe_classname(name):
     safe_name = name.strip()
     # add _ to a name if it starts with numbers
     safe_name = f'_{safe_name}' if safe_name[0].isdigit() else safe_name
 
     # replace all non alpha numeric characters
+    print('*before*', safe_name)
+    safe_name = safe_name.replace('ㆍ', '_')
     safe_name = re.sub('[\W_]+', '_', safe_name, flags=re.UNICODE)
-    if is_valid_class_name(safe_name):
+    print('*after*', safe_name)
+    if False: # is_valid_class_name() sometimes works and sometimes doesn't
+        if is_valid_class_name(safe_name):
+            return safe_name
+        raise Exception(f'Invalid class name : {safe_name}')
+    else:
         return safe_name
-    raise Exception(f'Invalid class name : {safe_name}')
 
 class KosisEntry:
     def __init__(self, kosis, name, attrs: dict):
         self.class_name = safe_classname(name)
+        print('@@@', self.class_name)
         self.__class__.__name__ = self.class_name
         self.kosis = kosis
         if 'LIST_NM' in attrs:
             self.id = attrs['LIST_ID']
             self.type = 'LIST_NM'
         elif 'TBL_NM' in attrs:
             self.id = attrs['TBL_ID']
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

