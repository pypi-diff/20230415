# Comparing `tmp/pyhOn-0.7.3.tar.gz` & `tmp/pyhOn-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.7.3.tar", last modified: Wed Apr 12 17:19:26 2023, max compression
+gzip compressed data, was "pyhOn-0.7.4.tar", last modified: Fri Apr 14 22:37:24 2023, max compression
```

## Comparing `pyhOn-0.7.3.tar` & `pyhOn-0.7.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 17:19:14.000000 pyhOn-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 17:19:26.305727 pyhOn-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-12 17:19:14.000000 pyhOn-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.301727 pyhOn-0.7.3/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:19:26.305727 pyhOn-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 17:19:14.000000 pyhOn-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.693191 pyhOn-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 22:37:15.000000 pyhOn-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 22:37:24.693191 pyhOn-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-14 22:37:15.000000 pyhOn-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.689191 pyhOn-0.7.4/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 22:37:24.000000 pyhOn-0.7.4/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.689191 pyhOn-0.7.4/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.689191 pyhOn-0.7.4/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:24.693191 pyhOn-0.7.4/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-14 22:37:15.000000 pyhOn-0.7.4/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:37:24.693191 pyhOn-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-14 22:37:15.000000 pyhOn-0.7.4/setup.py
```

### Comparing `pyhOn-0.7.3/LICENSE` & `pyhOn-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/PKG-INFO` & `pyhOn-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.3
+Version: 0.7.4
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.7.3/README.md` & `pyhOn-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.7.4/pyhOn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.3
+Version: 0.7.4
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.7.3/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.7.4/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/pyhon/__main__.py` & `pyhOn-0.7.4/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/pyhon/appliance.py` & `pyhOn-0.7.4/pyhon/appliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         if self._extra:
             return self._extra.data(result)
         return result
 
     @property
     def diagnose(self):
         data = self.data.copy()
-        for sensible in ["PK", "SK", "serialNumber", "code"]:
+        for sensible in ["PK", "SK", "serialNumber", "code", "coords"]:
             data["appliance"].pop(sensible, None)
         result = helper.pretty_print({"data": self.data}, whitespace="\u200B \u200B ")
         result += helper.pretty_print(
             {"commands": helper.create_command(self.commands)},
             whitespace="\u200B \u200B ",
         )
         return result.replace(self.mac_address, "12-34-56-78-90-ab")
```

### Comparing `pyhOn-0.7.3/pyhon/appliances/ov.py` & `pyhOn-0.7.4/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/pyhon/commands.py` & `pyhOn-0.7.4/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/pyhon/connection/api.py` & `pyhOn-0.7.4/pyhon/connection/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,156 +1,194 @@
 import json
 import logging
 from datetime import datetime
+from typing import Dict, Optional
+from typing_extensions import Self
 
-from pyhon import const
+from aiohttp import ClientSession
+
+from pyhon import const, exceptions
 from pyhon.appliance import HonAppliance
+from pyhon.connection.auth import HonAuth
 from pyhon.connection.handler import HonConnectionHandler, HonAnonymousConnectionHandler
 
 _LOGGER = logging.getLogger()
 
 
 class HonAPI:
-    def __init__(self, email="", password="", anonymous=False, session=None) -> None:
+    def __init__(
+        self,
+        email: str = "",
+        password: str = "",
+        anonymous: bool = False,
+        session: Optional[ClientSession] = None,
+    ) -> None:
         super().__init__()
-        self._email = email
-        self._password = password
-        self._anonymous = anonymous
-        self._hon = None
-        self._hon_anonymous = None
-        self._session = session
+        self._email: str = email
+        self._password: str = password
+        self._anonymous: bool = anonymous
+        self._hon_handler: Optional[HonConnectionHandler] = None
+        self._hon_anonymous_handler: Optional[HonAnonymousConnectionHandler] = None
+        self._session: Optional[ClientSession] = session
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> Self:
         return await self.create()
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await self.close()
 
-    async def create(self):
-        self._hon_anonymous = await HonAnonymousConnectionHandler(
+    @property
+    def auth(self) -> HonAuth:
+        if self._hon is None or self._hon.auth is None:
+            raise exceptions.NoAuthenticationException
+        return self._hon.auth
+
+    @property
+    def _hon(self):
+        if self._hon_handler is None:
+            raise exceptions.NoAuthenticationException
+        return self._hon_handler
+
+    @property
+    def _hon_anonymous(self):
+        if self._hon_anonymous_handler is None:
+            raise exceptions.NoAuthenticationException
+        return self._hon_anonymous_handler
+
+    async def create(self) -> Self:
+        self._hon_anonymous_handler = await HonAnonymousConnectionHandler(
             self._session
         ).create()
         if not self._anonymous:
-            self._hon = await HonConnectionHandler(
+            self._hon_handler = await HonConnectionHandler(
                 self._email, self._password, self._session
             ).create()
         return self
 
-    async def load_appliances(self):
+    async def load_appliances(self) -> Dict:
         async with self._hon.get(f"{const.API_URL}/commands/v1/appliance") as resp:
             return await resp.json()
 
-    async def load_commands(self, appliance: HonAppliance):
-        params = {
+    async def load_commands(self, appliance: HonAppliance) -> Dict:
+        params: Dict = {
             "applianceType": appliance.appliance_type,
             "code": appliance.info["code"],
             "applianceModelId": appliance.appliance_model_id,
             "firmwareId": appliance.info["eepromId"],
             "macAddress": appliance.mac_address,
             "fwVersion": appliance.info["fwVersion"],
             "os": const.OS,
             "appVersion": const.APP_VERSION,
             "series": appliance.info["series"],
         }
-        url = f"{const.API_URL}/commands/v1/retrieve"
+        url: str = f"{const.API_URL}/commands/v1/retrieve"
         async with self._hon.get(url, params=params) as response:
-            result = (await response.json()).get("payload", {})
+            result: Dict = (await response.json()).get("payload", {})
             if not result or result.pop("resultCode") != "0":
                 return {}
             return result
 
-    async def command_history(self, appliance: HonAppliance):
-        url = f"{const.API_URL}/commands/v1/appliance/{appliance.mac_address}/history"
+    async def command_history(self, appliance: HonAppliance) -> Dict:
+        url: str = (
+            f"{const.API_URL}/commands/v1/appliance/{appliance.mac_address}/history"
+        )
         async with self._hon.get(url) as response:
-            result = await response.json()
+            result: Dict = await response.json()
             if not result or not result.get("payload"):
                 return {}
             return result["payload"]["history"]
 
-    async def last_activity(self, appliance: HonAppliance):
-        url = f"{const.API_URL}/commands/v1/retrieve-last-activity"
-        params = {"macAddress": appliance.mac_address}
+    async def last_activity(self, appliance: HonAppliance) -> Dict:
+        url: str = f"{const.API_URL}/commands/v1/retrieve-last-activity"
+        params: Dict = {"macAddress": appliance.mac_address}
         async with self._hon.get(url, params=params) as response:
-            result = await response.json()
+            result: Dict = await response.json()
             if result and (activity := result.get("attributes")):
                 return activity
         return {}
 
-    async def load_attributes(self, appliance: HonAppliance):
-        params = {
+    async def load_attributes(self, appliance: HonAppliance) -> Dict:
+        params: Dict = {
             "macAddress": appliance.mac_address,
             "applianceType": appliance.appliance_type,
             "category": "CYCLE",
         }
-        url = f"{const.API_URL}/commands/v1/context"
+        url: str = f"{const.API_URL}/commands/v1/context"
         async with self._hon.get(url, params=params) as response:
             return (await response.json()).get("payload", {})
 
-    async def load_statistics(self, appliance: HonAppliance):
-        params = {
+    async def load_statistics(self, appliance: HonAppliance) -> Dict:
+        params: Dict = {
             "macAddress": appliance.mac_address,
             "applianceType": appliance.appliance_type,
         }
-        url = f"{const.API_URL}/commands/v1/statistics"
+        url: str = f"{const.API_URL}/commands/v1/statistics"
         async with self._hon.get(url, params=params) as response:
             return (await response.json()).get("payload", {})
 
-    async def send_command(self, appliance, command, parameters, ancillary_parameters):
-        now = datetime.utcnow().isoformat()
-        data = {
+    async def send_command(
+        self,
+        appliance: HonAppliance,
+        command: str,
+        parameters: Dict,
+        ancillary_parameters: Dict,
+    ) -> bool:
+        now: str = datetime.utcnow().isoformat()
+        data: Dict = {
             "macAddress": appliance.mac_address,
             "timestamp": f"{now[:-3]}Z",
             "commandName": command,
             "transactionId": f"{appliance.mac_address}_{now[:-3]}Z",
             "applianceOptions": appliance.commands_options,
-            "appliance": self._hon.device.get(),
+            "device": self._hon.device.get(mobile=True),
             "attributes": {
                 "channel": "mobileApp",
                 "origin": "standardProgram",
                 "energyLabel": "0",
             },
             "ancillaryParameters": ancillary_parameters,
             "parameters": parameters,
             "applianceType": appliance.appliance_type,
         }
-        url = f"{const.API_URL}/commands/v1/send"
-        async with self._hon.post(url, json=data) as resp:
-            json_data = await resp.json()
+        url: str = f"{const.API_URL}/commands/v1/send"
+        async with self._hon.post(url, json=data) as response:
+            json_data: Dict = await response.json()
             if json_data.get("payload", {}).get("resultCode") == "0":
                 return True
+            _LOGGER.error(await response.text())
         return False
 
-    async def appliance_configuration(self):
-        url = f"{const.API_URL}/config/v1/appliance-configuration"
+    async def appliance_configuration(self) -> Dict:
+        url: str = f"{const.API_URL}/config/v1/appliance-configuration"
         async with self._hon_anonymous.get(url) as response:
-            result = await response.json()
+            result: Dict = await response.json()
             if result and (data := result.get("payload")):
                 return data
         return {}
 
-    async def app_config(self, language="en", beta=True):
-        url = f"{const.API_URL}/app-config"
-        payload = {
+    async def app_config(self, language: str = "en", beta: bool = True) -> Dict:
+        url: str = f"{const.API_URL}/app-config"
+        payload_data: Dict = {
             "languageCode": language,
             "beta": beta,
             "appVersion": const.APP_VERSION,
             "os": const.OS,
         }
-        payload = json.dumps(payload, separators=(",", ":"))
+        payload: str = json.dumps(payload_data, separators=(",", ":"))
         async with self._hon_anonymous.post(url, data=payload) as response:
             if (result := await response.json()) and (data := result.get("payload")):
                 return data
         return {}
 
-    async def translation_keys(self, language="en"):
+    async def translation_keys(self, language: str = "en") -> Dict:
         config = await self.app_config(language=language)
         if url := config.get("language", {}).get("jsonPath"):
             async with self._hon_anonymous.get(url) as response:
                 if result := await response.json():
                     return result
         return {}
 
-    async def close(self):
-        if self._hon:
-            await self._hon.close()
-        if self._hon_anonymous:
-            await self._hon_anonymous.close()
+    async def close(self) -> None:
+        if self._hon_handler is not None:
+            await self._hon_handler.close()
+        if self._hon_anonymous_handler is not None:
+            await self._hon_anonymous_handler.close()
```

### Comparing `pyhOn-0.7.3/pyhon/connection/auth.py` & `pyhOn-0.7.4/pyhon/connection/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import json
 import logging
 import re
 import secrets
 import urllib
+from datetime import datetime, timedelta
 from pprint import pformat
+from typing import List, Tuple
 from urllib import parse
 from urllib.parse import quote
 
 from yarl import URL
 
 from pyhon import const, exceptions
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class HonAuth:
+    _TOKEN_EXPIRES_AFTER_HOURS = 8
+    _TOKEN_EXPIRE_WARNING_HOURS = 7
+
     def __init__(self, session, email, password, device) -> None:
         self._session = session
         self._email = email
         self._password = password
         self._access_token = ""
         self._refresh_token = ""
         self._cognito_token = ""
         self._id_token = ""
         self._device = device
-        self._called_urls = []
+        self._called_urls: List[Tuple[int, str]] = []
+        self._expires: datetime = datetime.utcnow()
 
     @property
     def cognito_token(self):
         return self._cognito_token
 
     @property
     def id_token(self):
@@ -38,14 +44,25 @@
     def access_token(self):
         return self._access_token
 
     @property
     def refresh_token(self):
         return self._refresh_token
 
+    def _check_token_expiration(self, hours):
+        return datetime.utcnow() >= self._expires + timedelta(hours=hours)
+
+    @property
+    def token_is_expired(self) -> bool:
+        return self._check_token_expiration(self._TOKEN_EXPIRES_AFTER_HOURS)
+
+    @property
+    def token_expires_soon(self) -> bool:
+        return self._check_token_expiration(self._TOKEN_EXPIRE_WARNING_HOURS)
+
     async def _error_logger(self, response, fail=True):
         result = "hOn Authentication Error\n"
         for i, (status, url) in enumerate(self._called_urls):
             result += f" {i + 1: 2d}     {status} - {url}\n"
         result += f"ERROR - {response.status} - {response.request_info.url}\n"
         result += f"{15 * '='} Response {15 * '='}\n{await response.text()}\n{40 * '='}"
         _LOGGER.error(result)
@@ -67,14 +84,15 @@
         }
         params = "&".join([f"{k}={v}" for k, v in params.items()])
         async with self._session.get(
             f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params}"
         ) as response:
             self._called_urls.append((response.status, response.request_info.url))
             text = await response.text()
+            self._expires = datetime.utcnow()
             if not (login_url := re.findall("url = '(.+?)'", text)):
                 if "oauth/done#access_token=" in text:
                     self._parse_token_data(text)
                     raise exceptions.HonNoAuthenticationNeeded()
                 await self._error_logger(response)
                 return False
         async with self._session.get(login_url[0], allow_redirects=False) as redirect1:
@@ -232,17 +250,19 @@
             f"{const.AUTH_API}/services/oauth2/token", params=params
         ) as response:
             self._called_urls.append((response.status, response.request_info.url))
             if response.status >= 400:
                 await self._error_logger(response, fail=False)
                 return False
             data = await response.json()
+        self._expires = datetime.utcnow()
         self._id_token = data["id_token"]
         self._access_token = data["access_token"]
         return await self._api_auth()
 
     def clear(self):
         self._session.cookie_jar.clear_domain(const.AUTH_API.split("/")[-2])
+        self._called_urls = []
         self._cognito_token = ""
         self._id_token = ""
         self._access_token = ""
         self._refresh_token = ""
```

### Comparing `pyhOn-0.7.3/pyhon/connection/device.py` & `pyhOn-0.7.4/pyhon/connection/device.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import secrets
+from typing import Dict
 
 from pyhon import const
 
 
 class HonDevice:
-    def __init__(self):
-        self._app_version = const.APP_VERSION
-        self._os_version = const.OS_VERSION
-        self._os = const.OS
-        self._device_model = const.DEVICE_MODEL
-        self._mobile_id = secrets.token_hex(8)
+    def __init__(self) -> None:
+        self._app_version: str = const.APP_VERSION
+        self._os_version: int = const.OS_VERSION
+        self._os: str = const.OS
+        self._device_model: str = const.DEVICE_MODEL
+        self._mobile_id: str = secrets.token_hex(8)
 
     @property
-    def app_version(self):
+    def app_version(self) -> str:
         return self._app_version
 
     @property
-    def os_version(self):
+    def os_version(self) -> int:
         return self._os_version
 
     @property
-    def os(self):
+    def os(self) -> str:
         return self._os
 
     @property
-    def device_model(self):
+    def device_model(self) -> str:
         return self._device_model
 
     @property
-    def mobile_id(self):
+    def mobile_id(self) -> str:
         return self._mobile_id
 
-    def get(self):
-        return {
+    def get(self, mobile: bool = False) -> Dict:
+        result = {
             "appVersion": self.app_version,
             "mobileId": self.mobile_id,
-            "osVersion": self.os_version,
             "os": self.os,
+            "osVersion": self.os_version,
             "deviceModel": self.device_model,
         }
+        return (result | {"mobileOs": result.pop("os")}) if mobile else result
```

### Comparing `pyhOn-0.7.3/pyhon/connection/handler.py` & `pyhOn-0.7.4/pyhon/connection/handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,121 @@
 import json
+from collections.abc import Generator, AsyncIterator, Coroutine
 from contextlib import asynccontextmanager
+from typing import Optional, Callable, Dict
+from typing_extensions import Self
 
 import aiohttp
 
-from pyhon import const
+from pyhon import const, exceptions
 from pyhon.connection.auth import HonAuth, _LOGGER
 from pyhon.connection.device import HonDevice
 from pyhon.exceptions import HonAuthenticationError
 
 
 class HonBaseConnectionHandler:
-    _HEADERS = {"user-agent": const.USER_AGENT, "Content-Type": "application/json"}
+    _HEADERS: Dict = {
+        "user-agent": const.USER_AGENT,
+        "Content-Type": "application/json",
+    }
+
+    def __init__(self, session: Optional[aiohttp.ClientSession] = None) -> None:
+        self._create_session: bool = session is None
+        self._session: Optional[aiohttp.ClientSession] = session
+        self._auth: Optional[HonAuth] = None
 
-    def __init__(self, session=None):
-        self._create_session = session is None
-        self._session = session
-        self._auth = None
-
-    async def __aenter__(self):
+    async def __aenter__(self) -> Self:
         return await self.create()
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await self.close()
 
-    async def create(self):
+    @property
+    def auth(self) -> Optional[HonAuth]:
+        return self._auth
+
+    async def create(self) -> Self:
         if self._create_session:
             self._session = aiohttp.ClientSession()
         return self
 
     @asynccontextmanager
-    async def _intercept(self, method, *args, loop=0, **kwargs):
+    def _intercept(self, method: Callable, *args, loop: int = 0, **kwargs):
         raise NotImplementedError
 
     @asynccontextmanager
-    async def get(self, *args, **kwargs):
+    async def get(self, *args, **kwargs) -> AsyncIterator[Callable]:
+        if self._session is None:
+            raise exceptions.NoSessionException()
+        response: Callable
         async with self._intercept(self._session.get, *args, **kwargs) as response:
             yield response
 
     @asynccontextmanager
-    async def post(self, *args, **kwargs):
+    async def post(self, *args, **kwargs) -> AsyncIterator[Callable]:
+        if self._session is None:
+            raise exceptions.NoSessionException()
+        response: Callable
         async with self._intercept(self._session.post, *args, **kwargs) as response:
             yield response
 
-    async def close(self):
-        if self._create_session:
+    async def close(self) -> None:
+        if self._create_session and self._session is not None:
             await self._session.close()
 
 
 class HonConnectionHandler(HonBaseConnectionHandler):
-    def __init__(self, email, password, session=None):
+    def __init__(
+        self, email: str, password: str, session: Optional[aiohttp.ClientSession] = None
+    ) -> None:
         super().__init__(session=session)
-        self._device = HonDevice()
-        self._email = email
-        self._password = password
+        self._device: HonDevice = HonDevice()
+        self._email: str = email
+        self._password: str = password
         if not self._email:
             raise HonAuthenticationError("An email address must be specified")
         if not self._password:
             raise HonAuthenticationError("A password address must be specified")
 
     @property
-    def device(self):
+    def device(self) -> HonDevice:
         return self._device
 
-    async def create(self):
+    async def create(self) -> Self:
         await super().create()
-        self._auth = HonAuth(self._session, self._email, self._password, self._device)
+        self._auth: HonAuth = HonAuth(
+            self._session, self._email, self._password, self._device
+        )
         return self
 
-    async def _check_headers(self, headers):
+    async def _check_headers(self, headers: Dict) -> Dict:
         if not (self._auth.cognito_token and self._auth.id_token):
             await self._auth.authenticate()
         headers["cognito-token"] = self._auth.cognito_token
         headers["id-token"] = self._auth.id_token
         return self._HEADERS | headers
 
     @asynccontextmanager
-    async def _intercept(self, method, *args, loop=0, **kwargs):
+    async def _intercept(
+        self, method: Callable, *args, loop: int = 0, **kwargs
+    ) -> AsyncIterator:
         kwargs["headers"] = await self._check_headers(kwargs.get("headers", {}))
         async with method(*args, **kwargs) as response:
-            if response.status in [401, 403] and loop == 0:
+            if (
+                self._auth.token_expires_soon or response.status in [401, 403]
+            ) and loop == 0:
                 _LOGGER.info("Try refreshing token...")
                 await self._auth.refresh()
                 async with self._intercept(
                     method, *args, loop=loop + 1, **kwargs
                 ) as result:
                     yield result
-            elif response.status in [401, 403] and loop == 1:
+            elif (
+                self._auth.token_is_expired or response.status in [401, 403]
+            ) and loop == 1:
                 _LOGGER.warning(
                     "%s - Error %s - %s",
                     response.request_info.url,
                     response.status,
                     await response.text(),
                 )
                 await self.create()
@@ -112,20 +138,22 @@
                 except json.JSONDecodeError:
                     _LOGGER.warning(
                         "%s - JsonDecodeError %s - %s",
                         response.request_info.url,
                         response.status,
                         await response.text(),
                     )
-                    yield {}
+                    raise HonAuthenticationError("Decode Error")
 
 
 class HonAnonymousConnectionHandler(HonBaseConnectionHandler):
-    _HEADERS = HonBaseConnectionHandler._HEADERS | {"x-api-key": const.API_KEY}
+    _HEADERS: Dict = HonBaseConnectionHandler._HEADERS | {"x-api-key": const.API_KEY}
 
     @asynccontextmanager
-    async def _intercept(self, method, *args, loop=0, **kwargs):
+    async def _intercept(
+        self, method: Callable, *args, loop: int = 0, **kwargs
+    ) -> AsyncIterator:
         kwargs["headers"] = kwargs.pop("headers", {}) | self._HEADERS
         async with method(*args, **kwargs) as response:
             if response.status == 403:
                 _LOGGER.error("Can't authenticate anymore")
             yield response
```

### Comparing `pyhOn-0.7.3/pyhon/helper.py` & `pyhOn-0.7.4/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/pyhon/hon.py` & `pyhOn-0.7.4/pyhon/hon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import asyncio
-from typing import List
+from typing import List, Optional
+from typing_extensions import Self
 
-from pyhon import HonAPI
+from aiohttp import ClientSession
+
+from pyhon import HonAPI, exceptions
 from pyhon.appliance import HonAppliance
 
 
 class Hon:
-    def __init__(self, email, password, session=None):
-        self._email = email
-        self._password = password
-        self._session = session
-        self._appliances = []
-        self._api = None
+    def __init__(self, email: str, password: str, session: ClientSession | None = None):
+        self._email: str = email
+        self._password: str = password
+        self._session: ClientSession | None = session
+        self._appliances: List[HonAppliance] = []
+        self._api: Optional[HonAPI] = None
 
     async def __aenter__(self):
         return await self.create()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
-    async def create(self):
+    @property
+    def api(self) -> HonAPI:
+        if self._api is None:
+            raise exceptions.NoAuthenticationException
+        return self._api
+
+    async def create(self) -> Self:
         self._api = await HonAPI(
             self._email, self._password, session=self._session
         ).create()
         await self.setup()
         return self
 
     @property
```

### Comparing `pyhOn-0.7.3/pyhon/parameter.py` & `pyhOn-0.7.4/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.3/setup.py` & `pyhOn-0.7.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.7.3",
+    version="0.7.4",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

