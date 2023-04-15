# Comparing `tmp/habmapslib-1.0.9.tar.gz` & `tmp/habmapslib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/habmapslib-1.0.9.tar", last modified: Sat Apr  3 15:44:04 2021, max compression
+gzip compressed data, was "habmapslib-2.0.0.tar", last modified: Sat Apr 15 18:14:44 2023, max compression
```

## Comparing `habmapslib-1.0.9.tar` & `habmapslib-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2021-04-03 15:44:04.664504 habmapslib-1.0.9/
--rw-r--r--   0 alvaroperis   (501) staff       (20)     4714 2021-04-03 15:44:04.664115 habmapslib-1.0.9/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2932 2021-04-03 15:44:03.000000 habmapslib-1.0.9/README.md
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2021-04-03 15:44:04.661364 habmapslib-1.0.9/habmapslib/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      489 2021-04-03 14:17:42.000000 habmapslib-1.0.9/habmapslib/ConfHandler.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2579 2021-04-03 10:17:05.000000 habmapslib-1.0.9/habmapslib/HMTail.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     3289 2021-04-03 12:42:22.000000 habmapslib-1.0.9/habmapslib/HabMapsMessage.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2602 2021-04-03 15:07:40.000000 habmapslib-1.0.9/habmapslib/MapTracker.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     3459 2021-04-03 15:20:34.000000 habmapslib-1.0.9/habmapslib/Parser.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)      104 2021-04-03 15:40:09.000000 habmapslib-1.0.9/habmapslib/__init__.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)        0 2021-04-02 12:05:39.000000 habmapslib-1.0.9/habmapslib/__main__.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     1006 2021-04-03 14:34:25.000000 habmapslib-1.0.9/habmapslib/cli.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)      698 2021-04-03 14:32:20.000000 habmapslib-1.0.9/habmapslib/confyaml.py
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2021-04-03 15:44:04.663611 habmapslib-1.0.9/habmapslib.egg-info/
--rw-r--r--   0 alvaroperis   (501) staff       (20)     4714 2021-04-03 15:44:04.000000 habmapslib-1.0.9/habmapslib.egg-info/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)      396 2021-04-03 15:44:04.000000 habmapslib-1.0.9/habmapslib.egg-info/SOURCES.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2021-04-03 15:44:04.000000 habmapslib-1.0.9/habmapslib.egg-info/dependency_links.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       43 2021-04-03 15:44:04.000000 habmapslib-1.0.9/habmapslib.egg-info/requires.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       11 2021-04-03 15:44:04.000000 habmapslib-1.0.9/habmapslib.egg-info/top_level.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2021-04-03 15:44:04.664634 habmapslib-1.0.9/setup.cfg
--rw-r--r--   0 alvaroperis   (501) staff       (20)     1326 2021-04-03 15:43:56.000000 habmapslib-1.0.9/setup.py
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-15 18:14:44.584937 habmapslib-2.0.0/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1072 2023-04-13 16:43:51.000000 habmapslib-2.0.0/LICENSE.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     8969 2023-04-15 18:14:44.573326 habmapslib-2.0.0/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     8025 2023-04-15 18:14:42.000000 habmapslib-2.0.0/README.md
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-15 18:14:44.563024 habmapslib-2.0.0/habmapslib/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      694 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/Appender.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      489 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/ConfHandler.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2116 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/GPSAppender.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2154 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/HMTail.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     3557 2023-04-15 18:10:37.000000 habmapslib-2.0.0/habmapslib/HabMapsMessage.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1694 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/InitChecks.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2660 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/MapTracker.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     3830 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/Parser.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      105 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/__init__.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        0 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/__main__.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1107 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/cli.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      862 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/confyaml.py
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-15 18:14:44.571431 habmapslib-2.0.0/habmapslib.egg-info/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     8969 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      482 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/SOURCES.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/dependency_links.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       43 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/requires.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       11 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/top_level.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-04-15 18:14:44.591460 habmapslib-2.0.0/setup.cfg
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1325 2023-04-15 18:14:36.000000 habmapslib-2.0.0/setup.py
```

### Comparing `habmapslib-1.0.9/habmapslib/HMTail.py` & `habmapslib-2.0.0/habmapslib/HMTail.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,44 @@
-#!/usr/bin/env python
-
-'''
-Python-Tail - Unix tail follow implementation in Python. 
-
-python-tail can be used to monitor changes to a file.
-
-Example:
-    import tail
-
-    # Create a tail instance
-    t = tail.Tail('file-to-be-followed')
-
-    # Register a callback function to be called when a new line is found in the followed file. 
-    # If no callback function is registerd, new lines would be printed to standard out.
-    t.register_callback(callback_function)
-
-    # Follow the file with 5 seconds as sleep time between iterations. 
-    # If sleep time is not provided 1 second is used as the default time.
-    t.follow(s=5) '''
-
-# Author - Kasun Herath <kasunh01 at gmail.com>
-# Source - https://github.com/kasun/python-tail
-
 import os
 import sys
 import time
-
 class Tail(object):
     ''' Represents a tail command. '''
     def __init__(self, tailed_file):
         ''' Initiate a Tail instance.
             Check for file validity, assigns callback function to standard out.
             
             Arguments:
                 tailed_file - File to be followed. '''
 
         self.check_file_validity(tailed_file)
         self.tailed_file = tailed_file
         self.callback = sys.stdout.write
 
+    def checkIfFileExists(self,file):
+        try:
+            with open(file) as f:
+                return True
+        except IOError as e:
+            return False
+
     def follow(self, s=1):
         ''' Do a tail follow. If a callback function is registered it is called with every new line. 
         Else printed to standard out.
     
         Arguments:
             s - Number of seconds to wait between each iteration; Defaults to 1. '''
 
         with open(self.tailed_file) as file_:
             # Go to the end of file
             file_.seek(0,2)
             while True:
+                if not self.checkIfFileExists(self.tailed_file):
+                    raise TailError("File '%s' does not exist" % (file_))
+
                 curr_position = file_.tell()
                 line = file_.readline()
                 if not line:
                     file_.seek(curr_position)
                     time.sleep(s)
                 else:
                     self.callback(line)
```

### Comparing `habmapslib-1.0.9/habmapslib/HabMapsMessage.py` & `habmapslib-2.0.0/habmapslib/HabMapsMessage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from datetime import datetime, timedelta
 import os
-import json,logging
+import json
+import logging
 LOGLEVEL = os.environ.get('HABLIB_LOGLEVEL', 'INFO').upper()
-FORMATTER = os.environ.get('HABLIB_FORMAT', '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+FORMATTER = os.environ.get(
+    'HABLIB_FORMAT', '[%(asctime)s] p%(process)s {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s')
 LOGFILE = os.environ.get('HABLIB_LOGFILE', '/tmp/hablibclient.log')
-logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[logging.FileHandler(LOGFILE),logging.StreamHandler()])
+logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[
+                    logging.FileHandler(LOGFILE), logging.StreamHandler()])
+
 
 class HabMapsMessage(object):
     def __init__(self,
                  TimeStamp='',
                  HabId='',
                  BasestationId='',
-                 HabPosition=[-1.0,-1.0],
+                 HabPosition=[-1.0, -1.0],
                  Signals={},
-                 BasestationPosition=[0.0,0.0]):
+                 BasestationPosition=[0.0, 0.0]):
         super(HabMapsMessage, self).__init__()
         self._track = {
             "type": "frame",
             "ftime": '',
             "hab": {
-                "id": '',
+                "hid": '',
                 "pos": {
                     "lat": -1.0,
                     "lon": -1.0
                 },
                 "payload": {}
             },
             "basestation": {
-                "id": '',
+                "bid": '',
                 "pos": {
                     "lat": 0.0,
                     "lon": 0.0
                 }
             }
         }
         if TimeStamp != '':
@@ -51,50 +55,53 @@
     def _setTS(self):
         self._track['ftime'] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
     def isValidMessage(self):
         valid = True
 
         if self._track['hab']['pos']['lat'] == -1.0 or self._track['hab']['pos']['lon'] == -1.0:
-            logging.error('Please set a valid hab pos with setHabPosition([<float : lat>, <float : lon>])')
+            logging.error(
+                'Please set a valid hab pos with setHabPosition([<float : lat>, <float : lon>])')
             valid = False
 
         if self._track['hab']['id'] == '':
             logging.error('Please set a habid with setHabId(<string : id>)')
             valid = False
 
         if self._track['basestation']['id'] == '':
-            logging.error('Please set a habid with setBasestationId(<string : id>)')
+            logging.error(
+                'Please set a habid with setBasestationId(<string : id>)')
             valid = False
 
         if self._track['ftime'] == '':
             self._setTS()
 
         return valid
 
     # SETTERS *******
     def setTimeStamp(self, ts):
         try:
             datetime.strptime(ts, "%Y-%m-%d %H:%M:%S")
             self._track['ftime'] = ts
         except ValueError:
             logging.error("Invalid date format")
-            raise ValueError("Incorrect data format, should be YYYY-mm-dd H:M:S")
-
+            raise ValueError(
+                "Incorrect data format, should be YYYY-mm-dd H:M:S")
 
     def setHabPosition(self, habpos):
-        self._track['hab']['pos']['lat'] = habpos[0]
-        self._track['hab']['pos']['lon'] = habpos[1]
+        self._track['hab']['pos']['lat'] = float(habpos[0])
+        self._track['hab']['pos']['lon'] = float(habpos[1])
 
-    def setBasestationPosition(self,bspos):
-        self._track['basestation']['pos']['lat'] = bspos[0]
-        self._track['basestation']['pos']['lon'] = bspos[1]
+    def setBasestationPosition(self, bspos):
+        self._track['basestation']['pos']['lat'] = float(bspos[0])
+        self._track['basestation']['pos']['lon'] = float(bspos[1])
+        if len(bspos) == 3 and float(bspos[2]) != 0.0:
+            self.addSignal('BStationHeight', float(bspos[2]))
 
-    def addSignal(self,key,value):
+    def addSignal(self, key, value):
         self._track['hab']['payload'][key] = value
 
-    def setHabId(self,id):
-        self._track['hab']['id'] = id.replace(" ","-")
-
-    def setBasestationId(self,id):
-        self._track['basestation']['id'] = id.replace(" ","-")
+    def setHabId(self, id):
+        self._track['hab']['id'] = id.replace(" ", "-")
 
+    def setBasestationId(self, id):
+        self._track['basestation']['id'] = id.replace(" ", "-")
```

### Comparing `habmapslib-1.0.9/habmapslib/MapTracker.py` & `habmapslib-2.0.0/habmapslib/MapTracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import paho.mqtt.client as mqtt
 import sched, time, threading,os
 import json,logging, traceback
 from datetime import datetime, timedelta
 LOGLEVEL = os.environ.get('HABLIB_LOGLEVEL', 'INFO').upper()
-FORMATTER = os.environ.get('HABLIB_FORMAT', '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+FORMATTER = os.environ.get('HABLIB_FORMAT', '[%(asctime)s] p%(process)s {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s')
 LOGFILE = os.environ.get('HABLIB_LOGFILE', '/tmp/hablibclient.log')
 logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[logging.FileHandler(LOGFILE),logging.StreamHandler()])
 
 class MapTracker(object):
     """Cliente de MQTT para maptracker"""
     def __init__(self, id="default-station-id",
                  mqtt_url="localhost",
@@ -59,15 +59,16 @@
         logging.debug(json.dumps(message))
         try:
             self.client.connect(self.mqtt_url,self.mqtt_port,60)
             self.client.publish(self.topic, json.dumps(message));
             self.client.disconnect();
             return {"isOK": True, "reason": ""}
         except Exception as e:
-            logging.error(traceback.print_exc())
+            logging.error(e)
+            logging.error(traceback.format_exc())
             return {"isOK": False, "reason": str(e)}
 
     def sendHabMessage(self,hm):
         hm.setBasestationId(self.id)
         if hm.isValidMessage() == False:
             raise ValueError("Please inform all required data")
         return self.sendMessage(hm.getMessage())
```

### Comparing `habmapslib-1.0.9/habmapslib/Parser.py` & `habmapslib-2.0.0/habmapslib/Parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging, os
 from datetime import datetime
 from . import HMTail
 from . import HabMapsMessage
 from . import MapTracker
-
+from . import GPSAppender
 LOGLEVEL = os.environ.get('HABLIB_LOGLEVEL', 'INFO').upper()
 FORMATTER = os.environ.get('HABLIB_FORMAT', '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 LOGFILE = os.environ.get('HABLIB_LOGFILE', '/tmp/hablibclient.log')
 logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[logging.FileHandler(LOGFILE), logging.StreamHandler()])
-
+import traceback
 
 class Parser(object):
     """docstring for Parser."""
 
     def __init__(self, confHandler):
         super(Parser, self).__init__()
         self.ch = confHandler.getConfig()
@@ -20,14 +20,15 @@
                                         mqtt_url=self.ch['mqtt']['url'],
                                         mqtt_port=int(self.ch['mqtt']['port']),
                                         user=self.ch['mqtt']['user'],
                                         publish=self.ch['mqtt']['topic'],
                                         alive=int(self.ch['mqtt']['alive']),
                                         password=self.ch['mqtt']['password']
                                         )
+        self.gps_appender = GPSAppender.GPSAppender(self.ch)
         #self.mt.startAlive()
 
     def parseline(self, line, definition):
         """ Core de parseo, aqui realiza la serialización a json de la traza retornando un HabMapsMessage"""
         trace = line.split('|')
         definitions = definition.split('|')
         i = 0
@@ -58,24 +59,29 @@
                         logging.info("Not a float signal")
                         hm.addSignal(el, trace[i])
             i += 1
         return hm
 
     def _print_line(self, txt):
         """ Call back, funcion que se llama por cada linea que se lee"""
-        logging.debug(datetime.now().strftime("%Y-%m-%d %H:%M:%S") + "  --> Nueva linea:")
+        logging.debug(datetime.now().strftime("%Y-%m-%d %H:%M:%S") + "  --> New line in file:")
         logging.debug(txt)
         # 1.- Parseamos la traza que nos llega de lora
         try:
             hm = self.parseline(txt, self.ch['frame']['format'])
             if hm:
+                # 2.- Obtenemos la ultima traza de gps
+                pos_gps = self.gps_appender.getValueAsArray()
+                hm.setBasestationPosition(pos_gps)
+                # 3.- Transmitimos el mensaje
                 self.mt.sendHabMessage(hm)
         except Exception as e:
             logging.error("Something went wrong ...")
             logging.error(e)
+            logging.error(traceback.format_exc())
 
 
     def run(self):
         """ Función que lanza el parser """
         t = HMTail.Tail(self.ch['frame']['file'])
         t.register_callback(self._print_line)
         t.follow(s=float(self.ch['frame']['refresh']))
```

### Comparing `habmapslib-1.0.9/habmapslib/cli.py` & `habmapslib-2.0.0/habmapslib/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import click
 from . import confyaml
 from . import ConfHandler
 from . import Parser
+from . import InitChecks
 import logging,os
 LOGLEVEL = os.environ.get('HABLIB_LOGLEVEL', 'INFO').upper()
-FORMATTER = os.environ.get('HABLIB_FORMAT', '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+FORMATTER = os.environ.get('HABLIB_FORMAT', '[%(asctime)s] p%(process)s {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s')
 LOGFILE = os.environ.get('HABLIB_LOGFILE', '/tmp/hablibclient.log')
 logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[logging.FileHandler(LOGFILE),logging.StreamHandler()])
 
 
 @click.command()
 @click.option('--conffile', help='Fichero de configuración')
 @click.option('--genconffile', is_flag=True, help='Muestra un fichero de configuración de ejemplo')
@@ -16,13 +17,14 @@
     if genconffile:
         print(confyaml.conf)
         return 0
     elif conffile:
         ch = ConfHandler.ConfHandler(file=conffile)
         logging.info("Launching habmapslib parser with the next configuration:")
         logging.info(ch.getConfig())
+        InitChecks.checkConfigs(ch.getConfig())
         p = Parser.Parser(ch)
         p.run()
 
 
 if __name__ == '__main__':
     cline()
```

### Comparing `habmapslib-1.0.9/habmapslib/confyaml.py` & `habmapslib-2.0.0/habmapslib/confyaml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-conf='''
-basestation:
-  id: id-de-mi-estacion
+conf='''basestation:
+  id: "id-de-mi-estacion"
   appenders:
-    - name: gps
-      filepath: /fichero/con/tramas/gps.txt
+    gpsappender:
+      file: '/Users/alvaroperis/ArchLab/habmapsgateway/demotraces/gps.appender'
+      regexselect: '\[.*\]\|(.*)\|(.*),(.*)\|.*\|'
+      mapping:
+        - "height"
+        - "lat"
+        - "lon"
 mqtt:
-  url: localhost
-  topic: hablistener
+  url: "localhost"
+  topic: "hablistener"
   port: 1883
-  user: habmaps
-  password: root
+  user: "habmaps"
+  password: "root"
   alive: 60
 frame:
   # Definición de la trama donde
   # $time : Es la hora expresada en HHMMSS
   # $pos : Es la posición gps del hab expresada en lat,lon
   # $id  : Es el identificador del hab
-  format: "$time|AlturaGPS|$pos|VelocidadHorizontalGPS|Temperatura|Presion|AlturaBarometrica|$id"
+  format: "$time|AlturaGPS|$pos|VelocidadHorizontalGPS|Temperatura|Presion|AlturaBarometrica|$id|"
   # Fichero donde se van insertando las trazas de LoRa
   file: "/Users/alvaroperis/ArchLab/habmapsgateway/demotraces/out.log"
   # Cada cuantos segundos se mira el fichero de envio
   refresh: 1
 '''
```

### Comparing `habmapslib-1.0.9/setup.py` & `habmapslib-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="habmapslib",
     include_package_data=True,
-    version="1.0.9",
+    version="2.0.0",
     author="Alpeza",
     author_email="",
     description="Librería para el acceso a habmaps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alpeza/habmapsgateway",
     packages=setuptools.find_packages(),
@@ -33,8 +33,8 @@
     python_requires='>=3.6, <4',
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/alpeza/habmapsgateway/issues',
         'Funding': 'https://github.com/alpeza/habmapsgateway/issues',
         'Say Thanks!': 'https://github.com/alpeza/habmapsgateway/issues',
         'Source': 'https://github.com/alpeza/habmapsgateway',
     },
-) 
+)
```

