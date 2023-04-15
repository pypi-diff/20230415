# Comparing `tmp/pyhOn-0.7.4.tar.gz` & `tmp/pyhOn-0.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.7.4.tar", last modified: Fri Apr 14 22:37:24 2023, max compression
+gzip compressed data, was "pyhOn-0.8.0b2.tar", last modified: Sat Apr 15 02:19:58 2023, max compression
```

## Comparing `pyhOn-0.7.4.tar` & `pyhOn-0.8.0b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.693191 pyhOn-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 22:37:15.000000 pyhOn-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 22:37:24.693191 pyhOn-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-14 22:37:15.000000 pyhOn-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.689191 pyhOn-0.7.4/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.689191 pyhOn-0.7.4/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.689191 pyhOn-0.7.4/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.693191 pyhOn-0.7.4/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:37:24.693191 pyhOn-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-14 22:37:15.000000 pyhOn-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.273452 pyhOn-0.8.0b2/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 02:19:58.000000 pyhOn-0.8.0b2/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.273452 pyhOn-0.8.0b2/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3251 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.273452 pyhOn-0.8.0b2/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 02:19:58.277452 pyhOn-0.8.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 02:19:46.000000 pyhOn-0.8.0b2/setup.py
```

### Comparing `pyhOn-0.7.4/LICENSE` & `pyhOn-0.8.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/PKG-INFO` & `pyhOn-0.8.0b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.4
+Version: 0.8.0b2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -117,16 +117,14 @@
 ...
 ```
 This generates a huge output. It is recommended to pipe this into a file
 ```commandline
 $ pyhOn translate fr > hon_fr.yaml
 $ pyhOn translate en --json > hon_en.json
 ```
-## Tested devices
-- Haier Washing Machine HW90
 
 ## Usage example
 This library is used for the custom [HomeAssistant Integration "Haier hOn"](https://github.com/Andre0512/hOn).
 
 ## Contribution
 Any kind of contribution is welcome!
```

### Comparing `pyhOn-0.7.4/README.md` & `pyhOn-0.8.0b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,14 @@
 ...
 ```
 This generates a huge output. It is recommended to pipe this into a file
 ```commandline
 $ pyhOn translate fr > hon_fr.yaml
 $ pyhOn translate en --json > hon_en.json
 ```
-## Tested devices
-- Haier Washing Machine HW90
 
 ## Usage example
 This library is used for the custom [HomeAssistant Integration "Haier hOn"](https://github.com/Andre0512/hOn).
 
 ## Contribution
 Any kind of contribution is welcome!
```

### Comparing `pyhOn-0.7.4/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.8.0b2/pyhOn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.4
+Version: 0.8.0b2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -117,16 +117,14 @@
 ...
 ```
 This generates a huge output. It is recommended to pipe this into a file
 ```commandline
 $ pyhOn translate fr > hon_fr.yaml
 $ pyhOn translate en --json > hon_en.json
 ```
-## Tested devices
-- Haier Washing Machine HW90
 
 ## Usage example
 This library is used for the custom [HomeAssistant Integration "Haier hOn"](https://github.com/Andre0512/hOn).
 
 ## Contribution
 Any kind of contribution is welcome!
```

### Comparing `pyhOn-0.7.4/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.8.0b2/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/__main__.py` & `pyhOn-0.8.0b2/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/appliance.py` & `pyhOn-0.8.0b2/pyhon/appliance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,84 @@
 import importlib
 from contextlib import suppress
+from typing import Optional, Dict
 
 from pyhon import helper
 from pyhon.commands import HonCommand
 from pyhon.parameter import HonParameterFixed
 
 
 class HonAppliance:
-    def __init__(self, api, info):
+    def __init__(self, api, info: Dict, zone: int = 0) -> None:
         if attributes := info.get("attributes"):
             info["attributes"] = {v["parName"]: v["parValue"] for v in attributes}
         self._info = info
         self._api = api
         self._appliance_model = {}
 
         self._commands = {}
         self._statistics = {}
         self._attributes = {}
+        self._zone = zone
 
         try:
             self._extra = importlib.import_module(
                 f"pyhon.appliances.{self.appliance_type.lower()}"
             ).Appliance()
         except ModuleNotFoundError:
             self._extra = None
 
     def __getitem__(self, item):
+        if self._zone:
+            item += f"Z{self._zone}"
         if "." in item:
             result = self.data
             for key in item.split("."):
-                if all([k in "0123456789" for k in key]) and type(result) is list:
+                if all(k in "0123456789" for k in key) and isinstance(result, list):
                     result = result[int(key)]
                 else:
                     result = result[key]
             return result
-        else:
-            if item in self.data:
-                return self.data[item]
-            if item in self.attributes["parameters"]:
-                return self.attributes["parameters"].get(item)
-            return self.info[item]
+        if item in self.data:
+            return self.data[item]
+        if item in self.attributes["parameters"]:
+            return self.attributes["parameters"].get(item)
+        return self.info[item]
 
     def get(self, item, default=None):
         try:
             return self[item]
         except (KeyError, IndexError):
             return default
 
+    def _check_name_zone(self, name: str, frontend: bool = True) -> str:
+        middle = " Z" if frontend else "_z"
+        if (attribute := self._info.get(name, "")) and self._zone:
+            return f"{attribute}{middle}{self._zone}"
+        return attribute
+
     @property
-    def appliance_model_id(self):
+    def appliance_model_id(self) -> str:
         return self._info.get("applianceModelId")
 
     @property
-    def appliance_type(self):
+    def appliance_type(self) -> str:
         return self._info.get("applianceTypeName")
 
     @property
-    def mac_address(self):
-        return self._info.get("macAddress")
+    def mac_address(self) -> str:
+        return self._check_name_zone("macAddress", frontend=False)
 
     @property
-    def model_name(self):
-        return self._info.get("modelName")
+    def model_name(self) -> str:
+        return self._check_name_zone("modelName")
 
     @property
-    def nick_name(self):
-        return self._info.get("nickName")
+    def nick_name(self) -> str:
+        return self._check_name_zone("nickName")
 
     @property
     def commands_options(self):
         return self._appliance_model.get("options")
 
     @property
     def commands(self):
```

### Comparing `pyhOn-0.7.4/pyhon/appliances/ov.py` & `pyhOn-0.8.0b2/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/commands.py` & `pyhOn-0.8.0b2/pyhon/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
     def __repr__(self):
         return f"{self._name} command"
 
     def _create_parameters(self, parameters):
         result = {}
         for parameter, attributes in parameters.items():
+            if parameter == "zoneMap" and self._device.zone:
+                attributes["default"] = self._device.zone
             match attributes.get("typology"):
                 case "range":
                     result[parameter] = HonParameterRange(parameter, attributes)
                 case "enum":
                     result[parameter] = HonParameterEnum(parameter, attributes)
                 case "fixed":
                     result[parameter] = HonParameterFixed(parameter, attributes)
```

### Comparing `pyhOn-0.7.4/pyhon/connection/api.py` & `pyhOn-0.8.0b2/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/connection/auth.py` & `pyhOn-0.8.0b2/pyhon/connection/auth.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/connection/device.py` & `pyhOn-0.8.0b2/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/connection/handler.py` & `pyhOn-0.8.0b2/pyhon/connection/handler.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/helper.py` & `pyhOn-0.8.0b2/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/pyhon/hon.py` & `pyhOn-0.8.0b2/pyhon/hon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import List, Optional
+from typing import List, Optional, Dict
 from typing_extensions import Self
 
 from aiohttp import ClientSession
 
 from pyhon import HonAPI, exceptions
 from pyhon.appliance import HonAppliance
 
@@ -35,23 +35,28 @@
         await self.setup()
         return self
 
     @property
     def appliances(self) -> List[HonAppliance]:
         return self._appliances
 
+    async def _create_appliance(self, appliance: Dict, zone=0) -> None:
+        appliance = HonAppliance(self._api, appliance, zone=zone)
+        if appliance.mac_address is None:
+            return
+        await asyncio.gather(
+            *[
+                appliance.load_attributes(),
+                appliance.load_commands(),
+                appliance.load_statistics(),
+            ]
+        )
+        self._appliances.append(appliance)
+
     async def setup(self):
         for appliance in (await self._api.load_appliances())["payload"]["appliances"]:
-            appliance = HonAppliance(self._api, appliance)
-            if appliance.mac_address is None:
-                continue
-            await asyncio.gather(
-                *[
-                    appliance.load_attributes(),
-                    appliance.load_commands(),
-                    appliance.load_statistics(),
-                ]
-            )
-            self._appliances.append(appliance)
+            for zone in range(int(appliance.get("zone", "0"))):
+                await self._create_appliance(appliance, zone=zone + 1)
+            await self._create_appliance(appliance)
 
     async def close(self):
         await self._api.close()
```

### Comparing `pyhOn-0.7.4/pyhon/parameter.py` & `pyhOn-0.8.0b2/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.4/setup.py` & `pyhOn-0.8.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.7.4",
+    version="0.8.0b2",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

