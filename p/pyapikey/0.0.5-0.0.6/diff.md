# Comparing `tmp/pyapikey-0.0.5.tar.gz` & `tmp/pyapikey-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapikey-0.0.5.tar", last modified: Sat Apr 15 11:47:24 2023, max compression
+gzip compressed data, was "pyapikey-0.0.6.tar", last modified: Sat Apr 15 11:51:55 2023, max compression
```

## Comparing `pyapikey-0.0.5.tar` & `pyapikey-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:47:24.615840 pyapikey-0.0.5/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-15 11:47:05.000000 pyapikey-0.0.5/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-15 11:47:24.615840 pyapikey-0.0.5/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      390 2023-04-15 11:47:05.000000 pyapikey-0.0.5/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:47:24.614840 pyapikey-0.0.5/pyapikey/
--rw-r--r--   0 mark      (1000) mark      (1000)       46 2020-10-02 10:21:11.000000 pyapikey-0.0.5/pyapikey/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1240 2023-04-15 11:43:04.000000 pyapikey-0.0.5/pyapikey/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)      172 2023-04-15 11:47:05.000000 pyapikey-0.0.5/pyapikey/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:47:24.615840 pyapikey-0.0.5/pyapikey.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-15 11:47:24.000000 pyapikey-0.0.5/pyapikey.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      222 2023-04-15 11:47:24.000000 pyapikey-0.0.5/pyapikey.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-15 11:47:24.000000 pyapikey-0.0.5/pyapikey.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-15 11:47:24.000000 pyapikey-0.0.5/pyapikey.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-15 11:47:24.615840 pyapikey-0.0.5/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1351 2023-04-15 11:47:05.000000 pyapikey-0.0.5/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:51:55.124305 pyapikey-0.0.6/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-15 11:51:37.000000 pyapikey-0.0.6/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-15 11:51:55.124305 pyapikey-0.0.6/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      390 2023-04-15 11:51:37.000000 pyapikey-0.0.6/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:51:55.124305 pyapikey-0.0.6/pyapikey/
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2020-10-02 10:21:11.000000 pyapikey-0.0.6/pyapikey/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1310 2023-04-15 11:51:26.000000 pyapikey-0.0.6/pyapikey/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      172 2023-04-15 11:51:37.000000 pyapikey-0.0.6/pyapikey/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:51:55.124305 pyapikey-0.0.6/pyapikey.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-15 11:51:55.000000 pyapikey-0.0.6/pyapikey.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      222 2023-04-15 11:51:55.000000 pyapikey-0.0.6/pyapikey.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-15 11:51:55.000000 pyapikey-0.0.6/pyapikey.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-15 11:51:55.000000 pyapikey-0.0.6/pyapikey.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-15 11:51:55.124305 pyapikey-0.0.6/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1351 2023-04-15 11:51:37.000000 pyapikey-0.0.6/setup.py
```

### Comparing `pyapikey-0.0.5/LICENSE` & `pyapikey-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyapikey-0.0.5/PKG-INFO` & `pyapikey-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyapikey
-Version: 0.0.5
+Version: 0.0.6
 Summary: access api keys from code
 Home-page: https://veltzer.github.io/pyapikey
 Download-URL: https://github.com/veltzer/pyapikey
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyapikey
 
 author: Mark Veltzer
 
-version: 0.0.5
+version: 0.0.6
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

### Comparing `pyapikey-0.0.5/pyapikey/core.py` & `pyapikey-0.0.6/pyapikey/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,11 +35,14 @@
 
     def get(self, key: str) -> Any:
         return self.data[key]
 
     def set(self, key: str, value: Any) -> None:
         self.data[key] = value
 
+    def has(self, key: str) -> bool:
+        return key in self.data
+
     def save(self):
         filename = os.path.expanduser("~/.config/pyapikey.temp.json")
         with open(filename, 'w') as file_handle:
             json.dump(fp=file_handle, obj=self.data, default=default)
```

### Comparing `pyapikey-0.0.5/pyapikey.egg-info/PKG-INFO` & `pyapikey-0.0.6/pyapikey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyapikey
-Version: 0.0.5
+Version: 0.0.6
 Summary: access api keys from code
 Home-page: https://veltzer.github.io/pyapikey
 Download-URL: https://github.com/veltzer/pyapikey
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyapikey
 
 author: Mark Veltzer
 
-version: 0.0.5
+version: 0.0.6
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

### Comparing `pyapikey-0.0.5/setup.py` & `pyapikey-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyapikey",
-    version="0.0.5",
+    version="0.0.6",
     packages=[
         "pyapikey",
     ],
     # from here all is optional
     description="access api keys from code",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
```

