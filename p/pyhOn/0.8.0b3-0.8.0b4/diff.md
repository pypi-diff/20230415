# Comparing `tmp/pyhOn-0.8.0b3.tar.gz` & `tmp/pyhOn-0.8.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.8.0b3.tar", last modified: Sat Apr 15 20:02:07 2023, max compression
+gzip compressed data, was "pyhOn-0.8.0b4.tar", last modified: Sat Apr 15 20:28:26 2023, max compression
```

## Comparing `pyhOn-0.8.0b3.tar` & `pyhOn-0.8.0b4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.586464 pyhOn-0.8.0b3/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 20:02:07.000000 pyhOn-0.8.0b3/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/pyhon/connection/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/anonym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/connection/handler/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:02:07.590464 pyhOn-0.8.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 20:01:56.000000 pyhOn-0.8.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.195605 pyhOn-0.8.0b4/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 20:28:26.000000 pyhOn-0.8.0b4/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.195605 pyhOn-0.8.0b4/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/pyhon/connection/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/anonym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/connection/handler/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:28:26.199605 pyhOn-0.8.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 20:28:10.000000 pyhOn-0.8.0b4/setup.py
```

### Comparing `pyhOn-0.8.0b3/LICENSE` & `pyhOn-0.8.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/PKG-INFO` & `pyhOn-0.8.0b4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b3
+Version: 0.8.0b4
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 
 # pyhOn
 [![PyPI - Status](https://img.shields.io/pypi/status/pyhOn)](https://pypi.org/project/pyhOn)
 [![PyPI](https://img.shields.io/pypi/v/pyhOn?color=blue)](https://pypi.org/project/pyhOn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyhOn)](https://www.python.org/)
 [![PyPI - License](https://img.shields.io/pypi/l/pyhOn)](https://github.com/Andre0512/pyhOn/blob/main/LICENSE)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyhOn)](https://pypistats.org/packages/pyhon)  
-Control your Haier appliances with python!
+Control your Haier, Candy and Hoover appliances with python!
 The idea behind this library is, to make the use of all available commands as simple as possible.
 
 ## Installation
 ```bash
 pip install pyhOn
 ```
```

### Comparing `pyhOn-0.8.0b3/README.md` & `pyhOn-0.8.0b4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # pyhOn
 [![PyPI - Status](https://img.shields.io/pypi/status/pyhOn)](https://pypi.org/project/pyhOn)
 [![PyPI](https://img.shields.io/pypi/v/pyhOn?color=blue)](https://pypi.org/project/pyhOn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyhOn)](https://www.python.org/)
 [![PyPI - License](https://img.shields.io/pypi/l/pyhOn)](https://github.com/Andre0512/pyhOn/blob/main/LICENSE)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyhOn)](https://pypistats.org/packages/pyhon)  
-Control your Haier appliances with python!
+Control your Haier, Candy and Hoover appliances with python!
 The idea behind this library is, to make the use of all available commands as simple as possible.
 
 ## Installation
 ```bash
 pip install pyhOn
 ```
```

### Comparing `pyhOn-0.8.0b3/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.0b4/pyhOn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.8.0b3
+Version: 0.8.0b4
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 
 # pyhOn
 [![PyPI - Status](https://img.shields.io/pypi/status/pyhOn)](https://pypi.org/project/pyhOn)
 [![PyPI](https://img.shields.io/pypi/v/pyhOn?color=blue)](https://pypi.org/project/pyhOn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyhOn)](https://www.python.org/)
 [![PyPI - License](https://img.shields.io/pypi/l/pyhOn)](https://github.com/Andre0512/pyhOn/blob/main/LICENSE)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyhOn)](https://pypistats.org/packages/pyhon)  
-Control your Haier appliances with python!
+Control your Haier, Candy and Hoover appliances with python!
 The idea behind this library is, to make the use of all available commands as simple as possible.
 
 ## Installation
 ```bash
 pip install pyhOn
 ```
```

### Comparing `pyhOn-0.8.0b3/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.8.0b4/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/__main__.py` & `pyhOn-0.8.0b4/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/appliance.py` & `pyhOn-0.8.0b4/pyhon/appliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._info: Dict = info
         self._api: Optional[HonAPI] = api
         self._appliance_model: Dict = {}
 
         self._commands: Dict = {}
         self._statistics: Dict = {}
         self._attributes: Dict = {}
-        self._zone = zone
+        self._zone: int = zone
 
         try:
             self._extra = importlib.import_module(
                 f"pyhon.appliances.{self.appliance_type.lower()}"
             ).Appliance()
         except ModuleNotFoundError:
             self._extra = None
@@ -102,14 +102,18 @@
     def statistics(self):
         return self._statistics
 
     @property
     def info(self):
         return self._info
 
+    @property
+    def zone(self) -> int:
+        return self._zone
+
     async def _recover_last_command_states(self, commands):
         command_history = await self._api.command_history(self)
         for name, command in commands.items():
             last = next(
                 (
                     index
                     for (index, d) in enumerate(command_history)
```

### Comparing `pyhOn-0.8.0b3/pyhon/appliances/ov.py` & `pyhOn-0.8.0b4/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/commands.py` & `pyhOn-0.8.0b4/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/connection/api.py` & `pyhOn-0.8.0b4/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/connection/auth.py` & `pyhOn-0.8.0b4/pyhon/connection/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/connection/device.py` & `pyhOn-0.8.0b4/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/connection/handler/anonym.py` & `pyhOn-0.8.0b4/pyhon/connection/handler/anonym.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/connection/handler/auth.py` & `pyhOn-0.8.0b4/pyhon/connection/handler/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/connection/handler/base.py` & `pyhOn-0.8.0b4/pyhon/connection/handler/base.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/connection/handler/hon.py` & `pyhOn-0.8.0b4/pyhon/connection/handler/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/helper.py` & `pyhOn-0.8.0b4/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/hon.py` & `pyhOn-0.8.0b4/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/pyhon/parameter.py` & `pyhOn-0.8.0b4/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.8.0b3/setup.py` & `pyhOn-0.8.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.8.0b3",
+    version="0.8.0b4",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

