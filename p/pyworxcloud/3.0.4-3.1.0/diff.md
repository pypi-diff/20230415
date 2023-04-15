# Comparing `tmp/pyworxcloud-3.0.4.tar.gz` & `tmp/pyworxcloud-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.0.4.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.0.tar", max compression
```

## Comparing `pyworxcloud-3.0.4.tar` & `pyworxcloud-3.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-03-31 18:16:32.039904 pyworxcloud-3.0.4/LICENSE
--rw-r--r--   0        0        0      929 2023-03-31 18:16:32.039904 pyworxcloud-3.0.4/README.md
--rw-r--r--   0        0        0      627 2023-03-31 18:16:46.708138 pyworxcloud-3.0.4/pyproject.toml
--rw-r--r--   0        0        0    28586 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     3751 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/events.py
--rw-r--r--   0        0        0     1756 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3838 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     4793 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     2410 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6375 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1423 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 pyworxcloud-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/LICENSE
+-rw-r--r--   0        0        0      929 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/README.md
+-rw-r--r--   0        0        0      610 2023-04-15 21:26:50.221668 pyworxcloud-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    28745 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/events.py
+-rw-r--r--   0        0        0     1756 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3838 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-04-15 21:26:39.145454 pyworxcloud-3.1.0/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     6150 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     2410 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6375 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     1423 2023-04-15 21:26:39.149454 pyworxcloud-3.1.0/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.0/PKG-INFO
```

### Comparing `pyworxcloud-3.0.4/LICENSE` & `pyworxcloud-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/README.md` & `pyworxcloud-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/__init__.py` & `pyworxcloud-3.1.0/pyworxcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ScheduleType,
     Statistic,
     Weekdays,
 )
 from .utils.mqtt import Command
 from .utils.schedules import TYPE_TO_STRING
 
-if sys.version_info < (3, 10, 0):
+if sys.version_info < (3, 9, 0):
     sys.exit("The pyWorxcloud module requires Python 3.10.0 or later")
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class WorxCloud(dict):
     """
@@ -240,21 +240,25 @@
         self._log.debug("Setting up MQTT handler")
         # setup MQTT handler
         self.mqtt = MQTT(
             self._api.access_token,
             self._cloud.BRAND_PREFIX,
             self._endpoint,
             self._user_id,
+            self._log,
             self._on_update,
         )
 
+        self.mqtt.connect()
+        while isinstance(self.mqtt.connected, type(None)):
+            pass
+
         for mower in self._mowers:
             self.mqtt.subscribe(mower["mqtt_topics"]["command_out"])
 
-        self.mqtt.connect()
         self._log.debug("MQTT connect done")
 
         # Convert time strings to objects.
         self._log.debug("Converting date and time string")
         for name, device in self.devices.items():
             convert_to_time(
                 name, device, device.time_zone, callback=self.update_attribute
@@ -264,19 +268,20 @@
         return True
 
     @property
     def auth_result(self) -> bool:
         """Return current authentication result."""
         return self._auth_result
 
-    def _on_update(self, topic, payload, dup, qos, retain, **kwargs):
+    def _on_update(self, payload):  # , topic, payload, dup, qos, retain, **kwargs):
         """Triggered when a MQTT message was received."""
         data = json.loads(payload)
         logger = self._log.getChild("MQTT_data_in")
-        logger.debug("MQTT data received '%s' on topic '%s'", payload, topic)
+        logger.debug("MQTT data received")
+        # logger.debug("MQTT data received '%s' on topic '%s'", payload, topic)
 
         for mower in self._mowers:
             if mower["serial_number"] == data["cfg"]["sn"]:
                 break
 
         device: DeviceHandler = self.devices[mower["name"]]
```

### Comparing `pyworxcloud-3.0.4/pyworxcloud/api.py` & `pyworxcloud-3.1.0/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/clouds.py` & `pyworxcloud-3.1.0/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/const.py` & `pyworxcloud-3.1.0/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/events.py` & `pyworxcloud-3.1.0/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.0/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.0/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.0/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/devices.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/mqtt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """MQTT information class."""
 from __future__ import annotations
 
 import json
-import logging
 import random
-import time
+import ssl
 import urllib.parse
 from datetime import datetime
+from logging import Logger
 from typing import Any
 from uuid import uuid4
-from zoneinfo import ZoneInfo
 
-from awsiot import mqtt, mqtt_connection_builder
+import paho.mqtt.client as mqtt
+from paho.mqtt.client import connack_string
 
 from ..events import EventHandler
 from .landroid_class import LDict
 
-_LOGGER = logging.getLogger(__name__)
-
 
 class MQTTMsgType(LDict):
     """Define specific message type data."""
 
     def __init__(self) -> dict:
         super().__init__()
 
@@ -85,77 +83,116 @@
 
     def __init__(
         self,
         token: str,
         brandprefix: str,
         endpoint: str,
         user_id: int,
+        logger: Logger,
         callback: Any,
     ) -> dict:
         """Initialize AWSIoT MQTT handler."""
         super().__init__()
-        self.client = None
+        # self.client = None
         self._events = EventHandler()
         self._on_update = callback
+        self._endpoint = endpoint
+        self._log = logger.getChild("MQTT")
+
+        self.connected: bool | None = None
 
         accesstokenparts = token.replace("_", "/").replace("-", "+").split(".")
 
         self._uuid = uuid4()
 
-        self._configuration = mqtt_connection_builder.direct_with_custom_authorizer(
-            endpoint=endpoint,
-            auth_username=f"bot?jwt={urllib.parse.quote(accesstokenparts[0])}.{urllib.parse.quote(accesstokenparts[1])}",
-            auth_authorizer_name="",
-            auth_authorizer_signature=urllib.parse.quote(accesstokenparts[2]),
-            auth_password=None,
-            port=443,
+        self.client = mqtt.Client(
             client_id=f"{brandprefix}/USER/{user_id}/bot/{self._uuid}",
             clean_session=False,
+            userdata=None,
+        )
+        self.client.username_pw_set(
+            username=f"bot?jwt={urllib.parse.quote(accesstokenparts[0])}.{urllib.parse.quote(accesstokenparts[1])}&x-amz-customauthorizer-name=''&x-amz-customauthorizer-signature={urllib.parse.quote(accesstokenparts[2])}",
+            password=None,
         )
 
+        ssl_context = ssl.create_default_context()
+        ssl_context.set_alpn_protocols(["mqtt"])
+        self.client.tls_set_context(context=ssl_context)
+
+        self.client.on_connect = self._on_connect
+        self.client.on_message = self._forward_on_message
+
+    def _forward_on_message(
+        self,
+        client: mqtt.Client | None,
+        userdata: Any | None,
+        message: Any | None,
+        properties: Any | None = None,  # pylint: disable=unused-argument
+    ) -> None:
+        """MQTT callback method definition."""
+        msg = message.payload.decode("utf-8")
+        self._log.debug("Received MQTT message:\n%s", msg)
+        self._on_update(msg)
+
     def subscribe(self, topic: str) -> None:
         """Subscribe to MQTT updates."""
-        self._configuration.subscribe(
-            topic=topic,
-            qos=mqtt.QoS.AT_LEAST_ONCE,
-            callback=self._on_update,
-        )
+        self.client.subscribe(topic=topic)
 
     def connect(self) -> None:
         """Connect to the MQTT service."""
-        connect_future = self._configuration.connect()
-        self.client = connect_future.result()
+        self.client.connect(self._endpoint, 443, 45)
+        self.client.loop_start()
+
+    def _on_connect(
+        self,
+        client: mqtt.Client | None,
+        userdata: Any | None,
+        flags: Any | None,
+        rc: int | None,
+        properties: Any | None = None,  # pylint: disable=unused-argument,invalid-name
+    ) -> None:
+        """MQTT callback method."""
+        self._log.debug(connack_string(rc))
+        if rc == 0:
+            self.connected = True
+            self._log.debug("MQTT connected")
+        else:
+            self.connected = False
+            self._log.debug("MQTT connection failed")
 
     def disconnect(
         self, reasoncode=None, properties=None  # pylint: disable=unused-argument
     ):
         """Disconnect from AWSIoT MQTT server."""
-        self.client = None
-        self._configuration.disconnect()
+        self.client.disconnect()
+        # self._configuration.disconnect()
 
     def ping(self, serial_number: str, topic: str) -> None:
         """Ping (update) the mower."""
         cmd = self.format_message(serial_number, {"cmd": Command.FORCE_REFRESH})
-        _LOGGER.debug("Sending '%s' on topic '%s'", cmd, topic)
-        self._configuration.publish(topic, cmd, mqtt.QoS.AT_LEAST_ONCE)
+        self._log.debug("Sending '%s' on topic '%s'", cmd, topic)
+        self.client.publish(topic, cmd, 0)
+        # self._configuration.publish(topic, cmd, mqtt.QoS.AT_LEAST_ONCE)
 
     def command(self, serial_number: str, topic: str, action: Command) -> None:
         """Send a specific command to the mower."""
         cmd = self.format_message(serial_number, {"cmd": action})
-        _LOGGER.debug("Sending '%s' on topic '%s'", cmd, topic)
-        self._configuration.publish(topic, cmd, mqtt.QoS.AT_LEAST_ONCE)
+        self._log.debug("Sending '%s' on topic '%s'", cmd, topic)
+        self.client.publish(topic, cmd, 0)
+        # self._configuration.publish(topic, cmd, mqtt.QoS.AT_LEAST_ONCE)
 
     def publish(self, serial_number: str, topic: str, message: dict) -> None:
         """Publish message to the mower."""
-        _LOGGER.debug("Publishing message '%s'", message)
-        self._configuration.publish(
-            topic,
-            self.format_message(serial_number, message),
-            mqtt.QoS.AT_LEAST_ONCE,
-        )
+        self._log.debug("Publishing message '%s'", message)
+        self.client.publish(topic, self.format_message(serial_number, message), 0)
+        # self._configuration.publish(
+        #     topic,
+        #     self.format_message(serial_number, message),
+        #     mqtt.QoS.AT_LEAST_ONCE,
+        # )
 
     def format_message(self, serial_number: str, message: dict) -> str:
         """
         Format a message.
         Message is expected to be a dict like this: {"cmd": 1}
         """
         now = datetime.now()
@@ -163,10 +200,10 @@
             "id": random.randint(1024, 65535),
             "sn": serial_number,
             "tm": now.strftime("%H:%M:%S"),
             "dt": now.strftime("%d/%m/%Y"),
         }
 
         msg.update(message)
-        _LOGGER.debug("Formatting message '%s' to '%s'", message, msg)
+        self._log.debug("Formatting message '%s' to '%s'", message, msg)
 
         return json.dumps(msg)
```

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.0/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/PKG-INFO` & `pyworxcloud-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.0.4
+Version: 3.1.0
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: awsiot (==0.1.3)
-Requires-Dist: awsiotsdk (==1.12.6)
+Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mtrab/pyworxcloud/issues
 Project-URL: Documentation, https://github.com/mtrab/pyworxcloud
 Description-Content-Type: text/markdown
 
 <a href="https://www.buymeacoffee.com/mtrab" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.0.4 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.0 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Dist: awsiot (==0.1.3) Requires-Dist: awsiotsdk (==1.12.6)
-Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-Dist: urllib3
-(>=1.26.10,<2.0.0) Project-URL: Bug Tracker, https://github.com/mtrab/
-pyworxcloud/issues Project-URL: Documentation, https://github.com/mtrab/
-pyworxcloud Description-Content-Type: text/markdown [Buy_Me_A_Coffee] #
-pyWorxCloud This is a PyPI module for communicating with Worx Cloud mowers,
-primarily developed for use with [Home Assistant](https://home-assistant.io),
-but I try to keep it as widely usable as possible.
+Modules Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests
+(>=2.26.0,<3.0.0) Requires-Dist: urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug
+Tracker, https://github.com/mtrab/pyworxcloud/issues Project-URL:
+Documentation, https://github.com/mtrab/pyworxcloud Description-Content-Type:
+text/markdown [Buy_Me_A_Coffee] # pyWorxCloud This is a PyPI module for
+communicating with Worx Cloud mowers, primarily developed for use with [Home
+Assistant](https://home-assistant.io), but I try to keep it as widely usable as
+possible.
 
 The module are compatible with cloud enabled devices from [these vendors]
 (https://github.com/MTrab/pyworxcloud/wiki#current-supported-brands--vendors)
 ## Documentation The documentation have been moved to the [Wiki](https://
 github.com/MTrab/pyworxcloud/wiki)
 This is unfortunately a little out-of-date due to the huge changes in version
 3.
```

