# Comparing `tmp/py-senertec-0.4.0.tar.gz` & `tmp/py-senertec-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-senertec-0.4.0.tar", last modified: Mon Apr 10 19:39:48 2023, max compression
+gzip compressed data, was "py-senertec-0.5.0.tar", last modified: Sat Apr 15 13:17:38 2023, max compression
```

## Comparing `py-senertec-0.4.0.tar` & `py-senertec-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 19:39:38.000000 py-senertec-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-10 19:39:48.393090 py-senertec-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-10 19:39:38.000000 py-senertec-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 19:39:38.000000 py-senertec-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:39:48.393090 py-senertec-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-10 19:39:41.000000 py-senertec-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.389090 py-senertec-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/src/py_senertec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 19:39:48.000000 py-senertec-0.4.0/src/py_senertec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/src/senertec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/canipError.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/canipValue.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/energyUnit.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-10 19:39:38.000000 py-senertec-0.4.0/src/senertec/obdClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:39:48.393090 py-senertec-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-10 19:39:38.000000 py-senertec-0.4.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:17:38.943397 py-senertec-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 13:17:26.000000 py-senertec-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-15 13:17:38.943397 py-senertec-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-15 13:17:26.000000 py-senertec-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 13:17:26.000000 py-senertec-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:17:38.943397 py-senertec-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-15 13:17:32.000000 py-senertec-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:17:38.935397 py-senertec-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:17:38.939397 py-senertec-0.5.0/src/py_senertec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-15 13:17:38.000000 py-senertec-0.5.0/src/py_senertec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 13:17:38.000000 py-senertec-0.5.0/src/py_senertec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:17:38.000000 py-senertec-0.5.0/src/py_senertec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 13:17:38.000000 py-senertec-0.5.0/src/py_senertec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 13:17:38.000000 py-senertec-0.5.0/src/py_senertec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:17:38.943397 py-senertec-0.5.0/src/senertec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/canipError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/canipValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21128 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/energyUnit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-15 13:17:26.000000 py-senertec-0.5.0/src/senertec/obdClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:17:38.943397 py-senertec-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-15 13:17:26.000000 py-senertec-0.5.0/tests/test_base_test.py
```

### Comparing `py-senertec-0.4.0/LICENSE` & `py-senertec-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-senertec-0.4.0/PKG-INFO` & `py-senertec-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-senertec
-Version: 0.4.0
+Version: 0.5.0
 Summary: Senertec energy system gen2 interface.
 Home-page: https://github.com/Kleinrotti/py-senertec
 Author: Kleinrotti
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/Kleinrotti/py-senertec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -50,18 +50,18 @@
 ```python
 from senertec.client import senertec
 from senertec.canipValue import canipValue
 import json
 import os
 
 #this example uses no filtering, read below how to use a filter instead of None as first parameter.
-senertec = senertec(None, "username", "password")
+senertec = senertec(None)
 #set your callback function for messages
 senertec.messagecallback = self.output
-senertec.login()
+senertec.login("username", "password")
 senertec.init()
 ```
 
 ### Requesting data
 
 ```python
 units = senertec.getUnits()
```

### Comparing `py-senertec-0.4.0/README.md` & `py-senertec-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 ```python
 from senertec.client import senertec
 from senertec.canipValue import canipValue
 import json
 import os
 
 #this example uses no filtering, read below how to use a filter instead of None as first parameter.
-senertec = senertec(None, "username", "password")
+senertec = senertec(None)
 #set your callback function for messages
 senertec.messagecallback = self.output
-senertec.login()
+senertec.login("username", "password")
 senertec.init()
 ```
 
 ### Requesting data
 
 ```python
 units = senertec.getUnits()
```

### Comparing `py-senertec-0.4.0/setup.py` & `py-senertec-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py-senertec",
-    version="0.4.0",
+    version="0.5.0",
     author="Kleinrotti",
     author_email="",
     package_dir={"": "src"},
     packages=setuptools.find_packages("src"),
     description="Senertec energy system gen2 interface.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `py-senertec-0.4.0/src/py_senertec.egg-info/PKG-INFO` & `py-senertec-0.5.0/src/py_senertec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-senertec
-Version: 0.4.0
+Version: 0.5.0
 Summary: Senertec energy system gen2 interface.
 Home-page: https://github.com/Kleinrotti/py-senertec
 Author: Kleinrotti
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/Kleinrotti/py-senertec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -50,18 +50,18 @@
 ```python
 from senertec.client import senertec
 from senertec.canipValue import canipValue
 import json
 import os
 
 #this example uses no filtering, read below how to use a filter instead of None as first parameter.
-senertec = senertec(None, "username", "password")
+senertec = senertec(None)
 #set your callback function for messages
 senertec.messagecallback = self.output
-senertec.login()
+senertec.login("username", "password")
 senertec.init()
 ```
 
 ### Requesting data
 
 ```python
 units = senertec.getUnits()
```

### Comparing `py-senertec-0.4.0/src/senertec/board.py` & `py-senertec-0.5.0/src/senertec/board.py`

 * *Files identical despite different names*

### Comparing `py-senertec-0.4.0/src/senertec/canipError.py` & `py-senertec-0.5.0/src/senertec/canipError.py`

 * *Files identical despite different names*

### Comparing `py-senertec-0.4.0/src/senertec/canipValue.py` & `py-senertec-0.5.0/src/senertec/canipValue.py`

 * *Files identical despite different names*

### Comparing `py-senertec-0.4.0/src/senertec/client.py` & `py-senertec-0.5.0/src/senertec/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,48 +2,47 @@
 import inspect
 import json
 import logging
 from threading import Thread
 import requests
 import websocket
 from bs4 import BeautifulSoup
-
 from .obdClass import obdClass
 from .energyUnit import energyUnit
 from .lang import lang
 from .canipError import canipError
 from .canipValue import canipValue
 from .board import board
 from .datapoint import datapoint
 
 
 class basesocketclient:
     """Base class which provides logic for a senertec websocket connection."""
 
     def __init__(self, level=logging.WARN):
-        self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(level)
-        self.WS_HOST = "wss://dachsconnect.senertec.com/ws"
+        self.__logger__ = logging.getLogger(__name__)
+        self.__logger__.setLevel(level)
+        self.__ws_host__ = "wss://dachsconnect.senertec.com/ws"
         self.__is_ws_connected__ = False
         self.__messages__ = [str()]
         self.__thread__ = None
-        self.ws = None
-        self.boards = [board()]
+        self.__ws__ = None
+        self.__boards__ = [board()]
         """All available boards with datapoints which can be used in request function"""
 
     def __on_message__(self, ws, message):
         j = json.loads(message)
         action = j["action"]
         data = j["data"]
         if action == "CanipValue":
-            self.logger.debug("Received new CanipValue from websocket.")
+            self.__logger__.debug("Received new CanipValue from websocket.")
             # skip old values and array size indicators
             if (data["age"] != 0 or data["size"] == True):
                 return
-            for b in self.boards:
+            for b in self.__boards__:
                 if b.boardName == data["boardName"]:
                     value = canipValue()
                     value.boardName = b.boardName
                     value.array = data["array"]
                     value.deviceSerial = data["sn"]
                     for point in b.datapoints:
                         if point.id == data["dataPointName"]:
@@ -59,15 +58,15 @@
                             tempValue = data["value"]
                             if point.enumName != None:
                                 for enum in self.__enumTranslations__:
                                     if point.enumName == enum["name"]:
                                         try:
                                             value.dataValue = enum["translations"][f"{tempValue}"]
                                         except KeyError:
-                                            self.logger.warning(
+                                            self.__logger__.warning(
                                                 f"No enum translation found for datapoint '{point.friendlyName}'.")
                                             value.dataValue = "Unknown"
                             elif point.gain != 0:
                                 value.dataValue = round(tempValue *
                                                         point.gain, 2)
                             else:
                                 value.dataValue = tempValue
@@ -75,123 +74,135 @@
                                 value.dataUnit = point.unit
                             else:
                                 value.dataUnit = ""
                             self.messagecallback(value)
                             break
         elif action == "HkaStore" and data["updateType"] == "remove":
             sn = j["sn"]
-            self.logger.info(
+            self.__logger__.info(
                 f"Unit with serial {sn} got disconnected.")
         else:
-            self.logger.debug(f"Received new websocket message {action}.")
+            self.__logger__.debug(f"Received new websocket message {action}.")
             self.__messages__.append(message)
 
     def __on_error__(self, ws, error):
-        self.logger.error(f"error : {error}")
+        self.__logger__.error(f"error : {error}")
 
     def __on_close__(self, ws, close_status_code, close_msg):
-        self.logger.info(
+        self.__logger__.info(
             f"Senertec Websocket closed with code {close_status_code}")
         self.__is_ws_connected__ = False
 
     def __on_open__(self, ws):
-        self.logger.info("Connected to Senertec websocket")
+        self.__logger__.info("Connected to Senertec websocket")
         self.__is_ws_connected__ = True
 
     def __create_websocket__(self):
         cookies = self.__getCookies__(
             self.__session__.cookies, "dachsconnect.senertec.com")
-        self.logger.debug("Creating websocket connection..")
-        self.ws = websocket.WebSocketApp(self.WS_HOST,
+        self.__logger__.debug("Creating websocket connection..")
+        self.__ws__ = websocket.WebSocketApp(self.__ws_host__,
                                          on_message=self.__on_message__,
                                          on_error=self.__on_error__,
                                          on_close=self.__on_close__,
                                          on_open=self.__on_open__,
                                          cookie=cookies)
         self.__thread__ = Thread(
-            target=self.ws.run_forever, kwargs={
+            target=self.__ws__.run_forever, kwargs={
                 "ping_interval": 60, "ping_timeout": 5}
         )
         self.__thread__.daemon = True
         self.__thread__.setName("senertec-websocket")
         self.__thread__.start()
-        self.logger.debug("Websocket connection started.")
+        self.__logger__.debug("Websocket connection started.")
 
 
 class senertec(basesocketclient):
     """Class to communicate with Senertec and handle network calls"""
 
-    def __init__(self, datapointList=None, email: str = None, password: str = None, language=lang.English, level=logging.INFO):
+    def __init__(self, datapointList=None, language=lang.English, level=logging.INFO):
         """Constructor, create instance of senertec client.
 
         ``datapointList`` Json string to add only these datapoints instead of everything.
 
         ``language`` Set to your language.
         """
-        if email is None or password is None:
-            raise ValueError(
-                "Arguments 'email', 'passwords'"
-            )
         super().__init__(level)
         logging.basicConfig(
             level=level,
             format='py-senertec: %(asctime)s %(levelname)-8s %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S'
         )
-        self.AUTHENTICATION_HOST = "https://dachsconnect.senertec.com"
-        self.SSO_HOST = "https://sso-portal.senertec.com"
-        self.email = email
+        self.__authentication_host__ = "https://dachsconnect.senertec.com"
+        self.__sso_host__ = "https://sso-portal.senertec.com"
         self.__session__ = None
-        self.language = language
-        self.password = password
-        self.level = level
+        self.__language__ = language
         self.__filteredDatapoints__ = datapointList
         self.__enums__ = []
         self.__metaDataPoints__ = []
         self.__metaDataTranslations__ = []
         self.__enumTranslations__ = []
         self.__errorTranslations__ = []
         self.__connectedUnit__ = []
         self.__appVersion__ = ""
         self.messagecallback = (canipValue())
         """Set your callback function to get the data values. Function has to be overloaded with data type ``canipValue``"""
-        self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(level)
+        self.__logger__ = logging.getLogger(__name__)
+        self.__logger__.setLevel(level)
+
+    @property
+    def boards(self) -> list[board]:
+        """Return all boards."""
+        return self.__boards__
+    
+    @property
+    def loglevel(self):
+        """Return the log level."""
+        return self.__logger__.level
+    
+    @property
+    def language(self):
+        """Return or set the language used for sensor names."""
+        return self.__language__
+    
+    @language.setter
+    def language(self, value: lang):
+        self.__language__ = value
 
     def __create_headers__(self):
         headers = {"Content-Type": "application/json"}
         return headers
 
     def __getCookies__(self, cookie_jar, domain):
         cookie_dict = cookie_jar.get_dict(domain=domain)
         found = ['%s=%s' % (name, value)
                  for (name, value) in cookie_dict.items()]
         return ';'.join(found)
 
     def __post__(self, urlPath: str, payload: str):
-        url = self.AUTHENTICATION_HOST + urlPath
+        url = self.__authentication_host__ + urlPath
         response = self.__session__.post(
             url, data=payload, headers=self.__create_headers__())
         if (response.status_code >= 400 and response.status_code <= 599):
             logger.error("Error in post request by function: " + inspect.stack()
                          [1].function + " HTTP response: " + response.text)
         return response
 
     def __get__(self, urlPath: str):
-        url = self.AUTHENTICATION_HOST + urlPath
+        url = self.__authentication_host__ + urlPath
         response = self.__session__.get(
             url, headers=self.__create_headers__())
         if (response.status_code >= 400 and response.status_code <= 599):
             logger.error("Error in get request by function: {" + inspect.stack()
                          [1].function + "} HTTP response: " + response.text)
         return response
 
     def __parseDataPoints__(self):
         """Parse all available datapoints for connected unit."""
-        self.logger.debug("Starting to parse datapoints..")
+        self.__logger__.debug("Starting to parse datapoints..")
         dataPointCount = 0
         metaData = self.__metaDataPoints__
         allPoints = []
         boardList = []
 
         # first collect all available datapoints
         for point in metaData:
@@ -218,22 +229,22 @@
                     for at in b["attributes"]:
                         if at == datap.id:
                             for b1 in boardList:
                                 if b1.boardName == b["name"]:
                                     dataPointCount += 1
                                     b1.__datapoints__.append(datap)
                             break
-        self.logger.debug(
+        self.__logger__.debug(
             f"Finished datapoints parsing. Found {len(boardList)} boards with {dataPointCount} datapoints in total.")
-        self.boards = boardList
+        self.__boards__ = boardList
         return
 
     def __parseDataPointsFiltered__(self):
         """Use this function to include only datapoints of datapointList which was set in class constructor."""
-        self.logger.debug("Starting to parse datapoints..")
+        self.__logger__.debug("Starting to parse datapoints..")
         metaData = self.__metaDataPoints__
         blist = []
         dataPointCount = 0
         boardname = ""
         for a in metaData:
             for element in self.__filteredDatapoints__[self.__connectedUnit__["productGroup"]]:
                 if metaData[a]["friendlyName"] == element:
@@ -258,104 +269,108 @@
                         b.__boardName__ = boardname
                         b.__datapoints__.append(datap)
                         blist.append(b)
                     else:
                         for b in blist:
                             if b.boardName == boardname:
                                 b.__datapoints__.append(datap)
-        self.boards = blist
-        self.logger.debug(
+        self.__boards__ = blist
+        self.__logger__.debug(
             f"Finished datapoints parsing. Found {len(blist)} boards with {dataPointCount} datapoints in total.")
 
     @property
     def portalVersion(self) -> str:
         """Returns Senertec Dachsportal version.
 
         Init function has to be called first.
         """
         return self.__appVersion__
 
-    def login(self):
+    def login(self, email: str, password: str):
         """
-        Login.
+        Login to senertec platform.
+
+        ``email`` Your email your are registered with.
+
+        ``password`` Your password.
 
         This function needs to be called first.
 
         Returns True on success, False on failure.
         """
-        self.logger.info("Logging in..")
+        self.__logger__.info("Logging in..")
         self.__session__ = requests.Session()
         loginSSOResponse = self.__session__.get(
-            self.AUTHENTICATION_HOST + "/rest/saml2/login")
+            self.__authentication_host__ + "/rest/saml2/login")
 
         authState = loginSSOResponse.url.split("loginuserpass.php?")[1]
         head = {"Content-Type": "application/x-www-form-urlencoded"}
-        userData = f"username={self.email}&password={self.password}&{authState}"
+        userData = f"username={email}&password={password}&{authState}"
         # submit credentials
-        loginResponse = self.__session__.post(self.SSO_HOST + "/simplesaml/module.php/core/loginuserpass.php?",
+        loginResponse = self.__session__.post(self.__sso_host__ + "/simplesaml/module.php/core/loginuserpass.php?",
                                               data=userData, headers=head)
 
         # filter out samlresponse and relaystate for ACS request
         soup = BeautifulSoup(loginResponse.text, features="html.parser")
         try:
             samlResponse = soup.findAll(
                 "input", {"name": "SAMLResponse"})[0]["value"]
             relayState = soup.findAll(
                 "input", {"name": "RelayState"})[0]["value"]
         except IndexError:
-            self.logger.error("Login failed, username or password wrong.")
+            self.__logger__.error("Login failed, username or password wrong.")
             return False
         acsData = {'SAMLResponse': {samlResponse}, 'RelayState': {relayState}}
 
         # do assertion consumer service request with received saml response
         acs = self.__session__.post(
-            self.AUTHENTICATION_HOST + "/rest/saml2/acs", data=acsData, headers=head)
+            self.__authentication_host__ + "/rest/saml2/acs", data=acsData, headers=head)
 
         if acs.history[0].status_code != 302:
-            self.logger.error("Login failed at ACS request, got no redirect.")
+            self.__logger__.error("Login failed at ACS request, got no redirect.")
             return False
-        self.logger.info("Login was successful.")
+        self.__logger__.info("Login was successful.")
         return True
 
     def logout(self):
         """
         Logout from senertec.
 
         Returns True on success, False on failure.
         """
-        self.logger.info("Logging out..")
+        self.__logger__.info("Logging out..")
         response = self.__get__("/logout")
-        if self.ws:
-            self.ws.close()
+        if self.__ws__:
+            self.__ws__.close()
         self.__session__.close()
         if response.status_code == 200:
-            self.logger.debug("Logout was successful.")
+            self.__logger__.debug("Logout was successful.")
             return True
         else:
             return False
 
     def init(self):
         """
         Initialize Senertec platform and connect to websocket.
 
         This function needs to be called after login.
 
         Returns True on success, False on failure.
         """
-        self.logger.info("Initializing senertec platform...")
+        self.__logger__.info("Initializing senertec platform...")
         response = self.__get__("/rest/info/init")
         if response.status_code == 200:
             self.__create_websocket__()
             j = json.loads(response.text)
             self.__metaDataPoints__ = j["metaDataPoints"]
             self.__enums__ = j["enums"]
-            self.__enumTranslations__ = j["translations"][f"{self.language.value}"]["enums"]
+            self.__enumTranslations__ = j["translations"][f"{self.__language__.value}"]["enums"]
             self.__metaDataTranslations__ = j["translations"][
-                f"{self.language.value}"]["metaDataPoints"]["translations"]
-            self.__errorTranslations__ = j["translations"][f"{self.language.value}"]["errorCategories"]
+                f"{self.__language__.value}"]["metaDataPoints"]["translations"]
+            self.__errorTranslations__ = j["translations"][f"{self.__language__.value}"]["errorCategories"]
             self.__appVersion__ = j["app"]["version"]
             return True
         else:
             return False
 
     def getUnits(self) -> list[energyUnit]:
         """
@@ -378,15 +393,15 @@
                 unit.contact = x["standortAnsprech"]
                 unit.city = x["standortOrt"]
                 unit.locationName = x["standortName"]
                 unit.postalCode = x["standortPlz"]
                 unit.street = x["standortAdresse"]
                 unit.productGroup = x["productGroup"]
                 units.append(unit)
-            self.logger.debug(
+            self.__logger__.debug(
                 f"Successful received a list of {len(units)} units.")
             return units
         else:
             return None
 
     def connectUnit(self, serial: str):
         """
@@ -428,25 +443,27 @@
         sn = self.__connectedUnit__["seriennummer"]
         response = self.__post__(
             f"/rest/charts/{sn}/data", json.dumps(
                 {"start": 1641596400000, "end": None, "parameters": {}, "chartName": chartname, "sn": sn}))
         if response.status_code == 200:
             return json.loads(response.text)
 
-    def request(self, dataPoints: list):
+    def request(self, dataPoints: list | str):
         """
         Request data from specific datapoints of the connected unit.
 
-        Data wil be received through websocket.
+        Data will be received through websocket.
 
-        ``dataPoints`` List of datapoint strings
+        ``dataPoints`` List of datapoint strings or a single datapoint as string.
 
         Returns True on success, False on failure.
         """
         sn = self.__connectedUnit__["seriennummer"]
+        if(type(dataPoints) == str):
+            dataPoints = dataPoints.split()
         j = json.dumps(
             {"seriennummer": sn, "keys": dataPoints})
         response = self.__post__(
             f"/rest/canip/{sn}/request", j)
         result = json.loads(response.text)
         if response.status_code == 200 and result["success"] and not result["errorKeys"]:
             return True
```

### Comparing `py-senertec-0.4.0/src/senertec/datapoint.py` & `py-senertec-0.5.0/src/senertec/datapoint.py`

 * *Files identical despite different names*

### Comparing `py-senertec-0.4.0/src/senertec/energyUnit.py` & `py-senertec-0.5.0/src/senertec/energyUnit.py`

 * *Files identical despite different names*

### Comparing `py-senertec-0.4.0/tests/test_base.py` & `py-senertec-0.5.0/tests/test_base_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 
 class TestBase(unittest.TestCase):
     def __init__(self, methodName: str = ...) -> None:
         super().__init__(methodName=methodName)
 
     def setUp(self):
-        # file = open(os.getcwd() + "\\productGroups.json")
-        # supportedItems = json.load(file)
-        # file.close()
-        self.senertec = senertec(
-            None, os.environ['SENERTECUSER'], os.environ['SENERTECPW'])
-        self.senertec.login()
+        file = open(os.getcwd() + "\\examples\\datapointFilter.json")
+        supportedItems = json.load(file)
+        file.close()
+        self.senertec = senertec(supportedItems)
+        self.senertec.login(
+            os.environ['SENERTECUSER'], os.environ['SENERTECPW'])
         self.senertec.init()
         self.out = Mock()
         self.senertec.messagecallback = self.out
 
     def tearDown(self):
         self.senertec.logout()
```

