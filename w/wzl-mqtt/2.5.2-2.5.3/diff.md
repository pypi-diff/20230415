# Comparing `tmp/wzl-mqtt-2.5.2.tar.gz` & `tmp/wzl-mqtt-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wzl-mqtt-2.5.2.tar", last modified: Wed Mar 29 08:05:07 2023, max compression
+gzip compressed data, was "wzl-mqtt-2.5.3.tar", last modified: Sat Apr 15 07:29:11 2023, max compression
```

## Comparing `wzl-mqtt-2.5.2.tar` & `wzl-mqtt-2.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:05:07.360541 wzl-mqtt-2.5.2/
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4018 2023-03-29 08:05:07.359541 wzl-mqtt-2.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.2/PyPI-README.md
--rw-rw-rw-   0 root         (0) root         (0)     4102 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 08:05:07.360541 wzl-mqtt-2.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:05:07.355541 wzl-mqtt-2.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:05:07.358541 wzl-mqtt-2.5.2/src/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.2/src/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16330 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.2/src/mqtt/client.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.2/src/mqtt/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3868 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.2/src/mqtt/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:05:07.359541 wzl-mqtt-2.5.2/wzl_mqtt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4018 2023-03-29 08:05:07.000000 wzl-mqtt-2.5.2/wzl_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      340 2023-03-29 08:05:07.000000 wzl-mqtt-2.5.2/wzl_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 08:05:07.000000 wzl-mqtt-2.5.2/wzl_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 08:05:07.000000 wzl-mqtt-2.5.2/wzl_mqtt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-29 08:05:07.000000 wzl-mqtt-2.5.2/wzl_mqtt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-29 08:05:07.000000 wzl-mqtt-2.5.2/wzl_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.938241 wzl-mqtt-2.5.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-04-15 07:29:11.937241 wzl-mqtt-2.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/PyPI-README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4275 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 07:29:11.938241 wzl-mqtt-2.5.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.927241 wzl-mqtt-2.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.936241 wzl-mqtt-2.5.3/src/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/src/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17184 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/src/mqtt/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/src/mqtt/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3868 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/src/mqtt/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.937241 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      340 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/top_level.txt
```

### Comparing `wzl-mqtt-2.5.2/LICENSE` & `wzl-mqtt-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wzl-mqtt-2.5.2/PKG-INFO` & `wzl-mqtt-2.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-mqtt
-Version: 2.5.2
+Version: 2.5.3
 Summary: Small library containing an MQTT publisher and receiver.
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/
 Author: Matthias Bodenbenner, Benjamin Montavon
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WZL-MQTT
 
-Current stable version: 2.5.2
+Current stable version: 2.5.3
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 ## Installation
 Requires at least Python 3.6
@@ -90,14 +90,19 @@
     except KeyboardInterrupt:
         break
 
 ```
 
 ## Changelog
 
+**2.5.3** - 2023-04-15
+  - if the port is specified as string it is also correctly processed now
+  - improved user feedback in case of successful connection to the broker
+  - improved user feedback if the combination of port, ssl and websocket is invalid
+
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
 
 2.5.1
   - increased verbosity in case of errors by including the full stack trace
 
 2.5.0
```

### Comparing `wzl-mqtt-2.5.2/PyPI-README.md` & `wzl-mqtt-2.5.3/PyPI-README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # WZL-MQTT
 
-Current stable version: 2.5.2
+Current stable version: 2.5.3
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 ## Installation
 Requires at least Python 3.6
@@ -75,14 +75,19 @@
     except KeyboardInterrupt:
         break
 
 ```
 
 ## Changelog
 
+**2.5.3** - 2023-04-15
+  - if the port is specified as string it is also correctly processed now
+  - improved user feedback in case of successful connection to the broker
+  - improved user feedback if the combination of port, ssl and websocket is invalid
+
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
 
 2.5.1
   - increased verbosity in case of errors by including the full stack trace
 
 2.5.0
```

### Comparing `wzl-mqtt-2.5.2/README.md` & `wzl-mqtt-2.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # WZL-MQTT
 
-Current stable version: 2.5.2
+Current stable version: 2.5.3
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 For using the MQTT Broker of the chair and department specific features, refer to the [internal documention](https://iot.wzl-mq.rwth-aachen.de/documentation/mqtt.html).
 
@@ -86,14 +86,18 @@
 
 The authors acknowledge funding from the LaVA project (Large Volume Applications, contract 17IND03 of the
 European Metrology Programme for Innovation and Research EMPIR). The EMPIR initiative is co-funded by
 the European Union’s Horizon 2020 research and innovation programme and the EMPIR Participating States.
 
 ## Changelog
 
+**2.5.3** - 2023-04-15
+  - if the port is specified as string it is also correctly processed now
+  - improved logging output in case of successful connection to the broker
+
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
 
 2.5.1
   - increased verbosity in case of errors by including the full stack trace
 
 2.5.0
```

### Comparing `wzl-mqtt-2.5.2/setup.py` & `wzl-mqtt-2.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("PyPI-README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='wzl-mqtt',
-      version='2.5.2',
+      version='2.5.3',
       url='https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/',
       project_urls={
             "Bug Tracker": "https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/-/issues",
       },
       author='Matthias Bodenbenner, Benjamin Montavon',
       author_email='m.bodenbenner@wzl-mq.rwth-aachen.de',
       description='Small library containing an MQTT publisher and receiver.',
```

### Comparing `wzl-mqtt-2.5.2/src/mqtt/client.py` & `wzl-mqtt-2.5.3/src/mqtt/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,27 +93,43 @@
             websocket: If true MQTT messages are published/received over WebSockets. If false, the default transportation over raw TCP is used.
             ssl: If true a secured TLS connection is established.
             keep_alive: maximum period in seconds allowed between communications with the broker.
                 If no other messages are being exchanged, this controls the rate at which the client will send ping messages to the broker.
 
             If not given explicitly given, the port automatically resolved from the values of "websocket" and "ssl".
         """
+
+        address = broker
         try:
-            address = broker
+            if isinstance(port, str):
+                port = int(port)
+        except Exception as exception:
+            self._logger.error(f"Specified port \"{port}\" is invalid. Port must be of type string or integer. Exiting...")
+            exit()
 
+        try:
             if port == 0:
                 if ssl:
                     port = 443 if websocket else 8883
                 else:
                     port = 80 if websocket else 1883
 
+
             if ssl:
+                if port not in [8883, 443]:
+                    self._logger.error(
+                        f"Can not connect to the broker. If ssl is set, the port must be \"8883\" (or \"443\" in case websockets are used), but specified port is \"{port}\". Exiting...")
+                    exit()
                 self._client.tls_set()
 
             if websocket:
+                if port not in [80, 443]:
+                    self._logger.error(
+                        f"Can not connect to the broker. If websocket is set, the port must be \"80\" (or \"443\" in case ssl is used), but specified port is \"{port}\". Exiting...")
+                    exit()
                 self._client._transport = "websockets"
                 fields = address.split("/")
                 address = fields[0]
                 path = "/".join(fields[1:])
                 print(address, path)
                 self._client.ws_set_options(path=f'/{path}')
 
@@ -143,15 +159,15 @@
                                                                  str(exception)))
             tb = sys.exc_info()[2]
             raise ConnectionError(str(exception)).with_traceback(tb)
 
     def _on_connect(self, client, userdata, flags, rc):
         if rc == 0:
             self._logger.info(
-                "MQTT Client {} connect terminated with code {} ({}).".format(
+                "MQTT Client {} connected successfully (code {}: {}).".format(
                     self.name, rc, mqtt.error_string(rc)))
             self._connected = True
         else:
             self._logger.error(
                 "MQTT Client {} connect terminated with code {} ({}).".format(
                     self.name, rc, mqtt.error_string(rc)))
             self._connected = False
```

### Comparing `wzl-mqtt-2.5.2/src/mqtt/exceptions.py` & `wzl-mqtt-2.5.3/src/mqtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `wzl-mqtt-2.5.2/src/mqtt/logger.py` & `wzl-mqtt-2.5.3/src/mqtt/logger.py`

 * *Files identical despite different names*

### Comparing `wzl-mqtt-2.5.2/wzl_mqtt.egg-info/PKG-INFO` & `wzl-mqtt-2.5.3/wzl_mqtt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-mqtt
-Version: 2.5.2
+Version: 2.5.3
 Summary: Small library containing an MQTT publisher and receiver.
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/
 Author: Matthias Bodenbenner, Benjamin Montavon
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WZL-MQTT
 
-Current stable version: 2.5.2
+Current stable version: 2.5.3
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 ## Installation
 Requires at least Python 3.6
@@ -90,14 +90,19 @@
     except KeyboardInterrupt:
         break
 
 ```
 
 ## Changelog
 
+**2.5.3** - 2023-04-15
+  - if the port is specified as string it is also correctly processed now
+  - improved user feedback in case of successful connection to the broker
+  - improved user feedback if the combination of port, ssl and websocket is invalid
+
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
 
 2.5.1
   - increased verbosity in case of errors by including the full stack trace
 
 2.5.0
```

