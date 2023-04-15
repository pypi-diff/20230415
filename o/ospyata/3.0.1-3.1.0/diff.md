# Comparing `tmp/ospyata-3.0.1.tar.gz` & `tmp/ospyata-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospyata-3.0.1.tar", last modified: Sun Apr  9 04:55:10 2023, max compression
+gzip compressed data, was "ospyata-3.1.0.tar", last modified: Sat Apr 15 08:14:05 2023, max compression
```

## Comparing `ospyata-3.0.1.tar` & `ospyata-3.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 04:55:00.000000 ospyata-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-09 04:55:10.065797 ospyata-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-09 04:55:00.000000 ospyata-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-09 04:55:10.065797 ospyata-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-09 04:55:00.000000 ospyata-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/src/ospyata/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-09 04:55:00.000000 ospyata-3.0.1/src/ospyata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-09 04:55:00.000000 ospyata-3.0.1/src/ospyata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-09 04:55:00.000000 ospyata-3.0.1/src/ospyata/osmata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/src/ospyata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 08:13:55.000000 ospyata-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-15 08:14:05.045255 ospyata-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-15 08:13:55.000000 ospyata-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 08:14:05.045255 ospyata-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-15 08:13:55.000000 ospyata-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/src/ospyata/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-15 08:13:55.000000 ospyata-3.1.0/src/ospyata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-15 08:13:55.000000 ospyata-3.1.0/src/ospyata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-15 08:13:55.000000 ospyata-3.1.0/src/ospyata/osmata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:14:05.045255 ospyata-3.1.0/src/ospyata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 08:14:05.000000 ospyata-3.1.0/src/ospyata.egg-info/top_level.txt
```

### Comparing `ospyata-3.0.1/LICENSE` & `ospyata-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ospyata-3.0.1/setup.py` & `ospyata-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='ospyata',
     license="MIT License",
-    version='3.0.1',
+    version='3.1.0',
     description='Python library for the open source bookmark app Osmata.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aerocyber/ospyata',
     author='aerocyber',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
-    keywords='osmata, development, osmata-bindings, osmata-python-bindings, bookmarks',
+    keywords='osmata, development, osmata-bindings, osmata-python-bindings, bookmarks, ospyata',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     python_requires='>=3.11, <4',
     install_requires=['validators'],
     project_urls={
         'Bug Reports': 'https://github.com/aerocyber/ospyata/issues',
         'Source': 'https://github.com/aerocyber/ospyata/',
```

### Comparing `ospyata-3.0.1/src/ospyata/osmata.py` & `ospyata-3.1.0/src/ospyata/osmata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Copyright (c) 2021-present aerocyber
 #
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 import json
 import validators
+from typing import List
+import pathlib
+from jsonschema import validate
 
 
 class OspyataException(Exception):
     pass
 
 
 class Osmata:
 
     def __init__(self):
-        db = {}  # Initialize the datastructure.
+        self.db = {}  # Initialize the datastructure.
 
-    def push(self, name: str, url: str, categories: str = []):
+    def push(self, name: str, url: str, categories: List[str] = []):
         """Push a record to the datastructure.
 
         Args:
             name (str): The name (key) of the record.
             url (str): The URL (value) associated with the name (key).
             categories (str, optional): Categories to which the keypair is assigned to. Defaults to [].
         """
@@ -55,14 +58,68 @@
         # First, check its existance.
         if self.check_existance(name=name):
             del self.db[name]  # Yup, as simple as that.
         else:
             _msg = name + " do not exist in db."
             raise OspyataException(_msg)  # Either success or failure.
 
+    def validate_omio(self, dat: str):
+        """Validate an omio file
+
+        Args:
+            dat (str): The omio string.
+        """
+        schema = {
+            "$schema": "https://json-schema.org/draft/2020-12/schema",
+            "$id": "https://example.com/product.schema.json",
+            "title": "Osmations",
+            "description": "A record of all bookmarks.",
+            "type": "object",
+            "properties": {
+                "Name": {
+                    "description": "The unique identifier for a record.",
+                    "type": "string"
+                },
+                "URL": {
+                    "description": "URL associated with the Name.",
+                    "type": "string"
+                },
+                "Categories": {
+                    "description": "Tags for the Record",
+                    "type": "array",
+                    "items": {
+                        "type": "string"
+                    }
+                }
+            },
+            "required": ["Name", "URL"]
+        }
+        try:
+            validate(instance=dat, schema=schema)
+        except Exception as e:
+            return False
+        else:
+            return True
+
+    def dumpOmio(self):
+        return json.dumps(self.db)
+
+    def loadOmio(self, omio_path):
+        if pathlib.Path(omio_path).exists():
+            f = open(omio_path, 'r')
+            data = f.read()
+            f.close()
+            if self.validate_omio(dat=data):
+                _json = json.loads(data)
+                return _json
+            else:
+                raise OspyataException("Invalid omio file.")
+        else:
+            raise FileNotFoundError("The file: " + omio_path + " was not found.")
+
     def check_existance(self, name=False, url=False):
         """Check if osmation exists in database.
 
         Args:
             name (str | False): Name associated. Defaults to False.
             url (str | False): Url associated. Defaults to False.
         """
```

