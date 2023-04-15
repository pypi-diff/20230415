# Comparing `tmp/butler-connect-0.4.2.tar.gz` & `tmp/butler-connect-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.4.2.tar", last modified: Fri Apr 14 13:25:16 2023, max compression
+gzip compressed data, was "butler-connect-0.4.3.tar", last modified: Sat Apr 15 11:38:00 2023, max compression
```

## Comparing `butler-connect-0.4.2.tar` & `butler-connect-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.796179 butler-connect-0.4.2/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     1886 2023-04-14 13:25:16.795183 butler-connect-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      135 2023-03-22 08:42:33.000000 butler-connect-0.4.2/README.md
--rw-rw-rw-   0        0        0      738 2023-04-14 13:24:45.000000 butler-connect-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 13:25:16.796179 butler-connect-0.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.726553 butler-connect-0.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.754663 butler-connect-0.4.2/src/butlerConnect/
--rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.2/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    16359 2023-04-14 13:24:24.000000 butler-connect-0.4.2/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.762175 butler-connect-0.4.2/src/butlerDescription/
--rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.2/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.4.2/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.2/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.2/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:25:16.794180 butler-connect-0.4.2/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-14 13:25:16.000000 butler-connect-0.4.2/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.551450 butler-connect-0.4.3/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     1957 2023-04-15 11:38:00.549786 butler-connect-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-15 11:37:42.000000 butler-connect-0.4.3/README.md
+-rw-rw-rw-   0        0        0      738 2023-04-15 11:33:00.000000 butler-connect-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 11:38:00.551450 butler-connect-0.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.515910 butler-connect-0.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.519926 butler-connect-0.4.3/src/butlerConnect/
+-rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.3/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    16460 2023-04-15 11:32:35.000000 butler-connect-0.4.3/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.526701 butler-connect-0.4.3/src/butlerDescription/
+-rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.3/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.4.3/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.3/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.3/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.548695 butler-connect-0.4.3/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     1957 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.4.2/LICENSE` & `butler-connect-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.2/PKG-INFO` & `butler-connect-0.4.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.2
+Version: 0.4.3
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,8 +32,11 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Access libraries and data definitions for the Buttler project.
 For more information ask Oliver Birkholz.
 
-- 0.4.0: Adding vhost Support
+0.4.0:
+- Adding vhost Support
+0.4.3: 
+- Adding sending automatic heartbeats in publisher-function
```

### Comparing `butler-connect-0.4.2/pyproject.toml` & `butler-connect-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.4.2"
+version = "0.4.3"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.4.2/src/butlerConnect/pikaButler.py` & `butler-connect-0.4.3/src/butlerConnect/pikaButler.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,16 @@
             for topic in item.keys():
                 msg = item[topic]
                 LOG.info(f'publish data {topic}@{msg}')
                 self._channelPublish .basic_publish(exchange=topic,
                         routing_key='',
                         body=msg)
                 self.queSendData.task_done()
+            # sending heartbeat
+            self._connectionPublisher._send_frame(frame.Heartbeat())
      
                 
     def runConsumer(self):
         LOG.info(f'Create pika Consumer-Connection with: host={self.host}, post={self.port}')
         self._connectionConsumer = pika.BlockingConnection(self.ConnectionParameters())
         self._channelConsumer = self._connectionConsumer.channel()
         topicData = f'component.{self.component}.data.output'
```

### Comparing `butler-connect-0.4.2/src/butlerDescription/control.py` & `butler-connect-0.4.3/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.2/src/butlerDescription/signal.py` & `butler-connect-0.4.3/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.2/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.4.3/src/butler_connect.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.2
+Version: 0.4.3
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,8 +32,11 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Access libraries and data definitions for the Buttler project.
 For more information ask Oliver Birkholz.
 
-- 0.4.0: Adding vhost Support
+0.4.0:
+- Adding vhost Support
+0.4.3: 
+- Adding sending automatic heartbeats in publisher-function
```

