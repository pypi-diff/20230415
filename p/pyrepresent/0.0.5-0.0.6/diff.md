# Comparing `tmp/pyrepresent-0.0.5.tar.gz` & `tmp/pyrepresent-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.0.5.tar", last modified: Wed Apr  5 09:32:04 2023, max compression
+gzip compressed data, was "pyrepresent-0.0.6.tar", last modified: Sat Apr 15 12:29:33 2023, max compression
```

## Comparing `pyrepresent-0.0.5.tar` & `pyrepresent-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 09:32:04.690788 pyrepresent-0.0.5/
--rw-rw-rw-   0        0        0      115 2023-04-05 09:32:04.000000 pyrepresent-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-04-05 09:32:04.690788 pyrepresent-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.0.5/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.0.5/build.py
--rw-rw-rw-   0        0        0      715 2023-04-05 09:32:04.000000 pyrepresent-0.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-05 09:32:04.685714 pyrepresent-0.0.5/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-04-05 09:32:04.000000 pyrepresent-0.0.5/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-05 09:32:04.000000 pyrepresent-0.0.5/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 09:32:04.000000 pyrepresent-0.0.5/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-05 09:32:04.000000 pyrepresent-0.0.5/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-05 09:32:04.000000 pyrepresent-0.0.5/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 09:32:04.689788 pyrepresent-0.0.5/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.0.5/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.0.5/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.0.5/represent/document.py
--rw-rw-rw-   0        0        0     2121 2023-04-05 09:22:18.000000 pyrepresent-0.0.5/represent/indentation.py
--rw-rw-rw-   0        0        0    11801 2023-03-31 19:41:50.000000 pyrepresent-0.0.5/represent/object.py
--rw-rw-rw-   0        0        0    19611 2023-03-31 19:36:24.000000 pyrepresent-0.0.5/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.0.5/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 09:32:04.690788 pyrepresent-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-05 09:31:59.000000 pyrepresent-0.0.5/setup.py
--rw-rw-rw-   0        0        0      669 2023-03-28 10:53:06.000000 pyrepresent-0.0.5/test.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:33.668529 pyrepresent-0.0.6/
+-rw-rw-rw-   0        0        0      115 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-04-15 12:29:33.667530 pyrepresent-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.0.6/README.md
+-rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.0.6/build.py
+-rw-rw-rw-   0        0        0      715 2023-04-15 12:29:29.000000 pyrepresent-0.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:33.662564 pyrepresent-0.0.6/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:33.667530 pyrepresent-0.0.6/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.0.6/represent/__init__.py
+-rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.0.6/represent/base.py
+-rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.0.6/represent/document.py
+-rw-rw-rw-   0        0        0     2121 2023-04-05 09:22:18.000000 pyrepresent-0.0.6/represent/indentation.py
+-rw-rw-rw-   0        0        0    11524 2023-04-15 12:28:39.000000 pyrepresent-0.0.6/represent/object.py
+-rw-rw-rw-   0        0        0    19611 2023-04-09 18:51:47.000000 pyrepresent-0.0.6/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.0.6/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 12:29:33.668529 pyrepresent-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-15 12:29:26.000000 pyrepresent-0.0.6/setup.py
+-rw-rw-rw-   0        0        0      669 2023-03-28 10:53:06.000000 pyrepresent-0.0.6/test.py
```

### Comparing `pyrepresent-0.0.5/PKG-INFO` & `pyrepresent-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.5
+Version: 0.0.6
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.5/README.md` & `pyrepresent-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.5/build.py` & `pyrepresent-0.0.6/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.5/pyproject.toml` & `pyrepresent-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.0.5'
+version = '0.0.6'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.0.5/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.0.6/pyrepresent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.5
+Version: 0.0.6
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.5/represent/base.py` & `pyrepresent-0.0.6/represent/base.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.5/represent/indentation.py` & `pyrepresent-0.0.6/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.5/represent/object.py` & `pyrepresent-0.0.6/represent/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,49 +80,35 @@
             assign = True
         # end if
 
         if protected is None:
             protected = False
         # end if
 
-        if properties is None:
-            properties = []
-        # end if
-
         if legalize is None:
             legalize = False
         # end if
 
         if force is None:
             force = False
         # end if
 
         if defined is None:
             defined = True
         # end if
 
-        if excluded is None:
-            excluded = [
-                'modifiers'
-            ]
-        # end if
-
-        if hidden is None:
-            hidden = []
-        # end if
-
         self.assign = assign
         self.protected = protected
         self.legalize = legalize
         self.force = force
         self.defined = defined
 
-        self.properties = list(properties)
-        self.excluded = list(excluded)
-        self.hidden = list(hidden)
+        self.properties = list(properties or [])
+        self.excluded = list(excluded or ['modifiers'])
+        self.hidden = list(hidden or [])
     # end __init__
 # end Modifiers
 
 class BaseModel:
     """A class to represent a base model."""
 
     modifiers = Modifiers()
@@ -184,17 +170,15 @@
         properties = modifiers.properties
         protected = modifiers.protected
         hidden = modifiers.hidden
         legalize = modifiers.legalize
         defined = modifiers.defined
     # end if
 
-    if ids is None:
-        ids = {}
-    # end if
+    ids = ids or {}
 
     if (not isinstance(hidden, dict)) and (hidden is not None):
         hide = True
 
     elif hidden is None:
         hide = False
```

### Comparing `pyrepresent-0.0.5/represent/structures.py` & `pyrepresent-0.0.6/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.5/setup.py` & `pyrepresent-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.0.5',
+        version='0.0.6',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.0.5/test.py` & `pyrepresent-0.0.6/test.py`

 * *Files identical despite different names*

