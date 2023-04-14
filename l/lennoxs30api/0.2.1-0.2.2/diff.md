# Comparing `tmp/lennoxs30api-0.2.1.tar.gz` & `tmp/lennoxs30api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lennoxs30api-0.2.1.tar", last modified: Sun Jan 22 21:14:42 2023, max compression
+gzip compressed data, was "lennoxs30api-0.2.2.tar", last modified: Fri Apr 14 23:30:21 2023, max compression
```

## Comparing `lennoxs30api-0.2.1.tar` & `lennoxs30api-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-01-22 21:14:42.188187 lennoxs30api-0.2.1/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.1/LICENSE
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-01-22 21:14:42.186188 lennoxs30api-0.2.1/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.1/README.md
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-01-22 21:14:42.111178 lennoxs30api-0.2.1/lennoxs30api/
--rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-01-22 16:40:04.000000 lennoxs30api-0.2.1/lennoxs30api/__init__.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.1/lennoxs30api/lennox_equipment.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.1/lennoxs30api/lennox_errors.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.1/lennoxs30api/lennox_home.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.1/lennoxs30api/lennox_period.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.1/lennoxs30api/lennox_schedule.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.1/lennoxs30api/message_logger.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3973 2022-05-22 21:24:48.000000 lennoxs30api-0.2.1/lennoxs30api/metrics.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)   126107 2023-01-22 16:40:29.000000 lennoxs30api-0.2.1/lennoxs30api/s30api_async.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.1/lennoxs30api/s30exception.py
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-01-22 21:14:42.173030 lennoxs30api-0.2.1/lennoxs30api.egg-info/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-01-22 21:14:41.000000 lennoxs30api-0.2.1/lennoxs30api.egg-info/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)      496 2023-01-22 21:14:41.000000 lennoxs30api-0.2.1/lennoxs30api.egg-info/SOURCES.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-01-22 21:14:41.000000 lennoxs30api-0.2.1/lennoxs30api.egg-info/dependency_links.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-01-22 21:14:41.000000 lennoxs30api-0.2.1/lennoxs30api.egg-info/requires.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-01-22 21:14:41.000000 lennoxs30api-0.2.1/lennoxs30api.egg-info/top_level.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-01-22 21:14:42.189185 lennoxs30api-0.2.1/setup.cfg
--rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-01-22 16:39:56.000000 lennoxs30api-0.2.1/setup.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-14 23:30:21.036753 lennoxs30api-0.2.2/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.2/LICENSE
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-14 23:30:21.033755 lennoxs30api-0.2.2/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.2/README.md
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-14 23:30:20.942763 lennoxs30api-0.2.2/lennoxs30api/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-04-14 23:27:17.000000 lennoxs30api-0.2.2/lennoxs30api/__init__.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_equipment.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_errors.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_home.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_period.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.2/lennoxs30api/lennox_schedule.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.2/lennoxs30api/message_logger.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3973 2022-05-22 21:24:48.000000 lennoxs30api-0.2.2/lennoxs30api/metrics.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)   126146 2023-04-14 23:27:17.000000 lennoxs30api-0.2.2/lennoxs30api/s30api_async.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.2/lennoxs30api/s30exception.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-14 23:30:21.015753 lennoxs30api-0.2.2/lennoxs30api.egg-info/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      496 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/requires.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-04-14 23:30:20.000000 lennoxs30api-0.2.2/lennoxs30api.egg-info/top_level.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-04-14 23:30:21.038754 lennoxs30api-0.2.2/setup.cfg
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-04-14 23:27:17.000000 lennoxs30api-0.2.2/setup.py
```

### Comparing `lennoxs30api-0.2.1/LICENSE` & `lennoxs30api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/PKG-INFO` & `lennoxs30api-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.1
+Version: 0.2.2
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.1/README.md` & `lennoxs30api-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/lennox_equipment.py` & `lennoxs30api-0.2.2/lennoxs30api/lennox_equipment.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/lennox_errors.py` & `lennoxs30api-0.2.2/lennoxs30api/lennox_errors.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/lennox_home.py` & `lennoxs30api-0.2.2/lennoxs30api/lennox_home.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/lennox_period.py` & `lennoxs30api-0.2.2/lennoxs30api/lennox_period.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/lennox_schedule.py` & `lennoxs30api-0.2.2/lennoxs30api/lennox_schedule.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/message_logger.py` & `lennoxs30api-0.2.2/lennoxs30api/message_logger.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/metrics.py` & `lennoxs30api-0.2.2/lennoxs30api/metrics.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api/s30api_async.py` & `lennoxs30api-0.2.2/lennoxs30api/s30api_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,15 +592,15 @@
     async def subscribe(self, lennoxSystem: "lennox_system") -> None:
 
         if self.isLANConnection == True:
             ref: int = 1
             try:
                 await self.requestDataHelper(
                     lennoxSystem.sysId,
-                    '"AdditionalParameters":{"JSONPath":"1;/systemControl;/systemController;/reminderSensors;/reminders;/alerts/active;/alerts/meta;/fwm;/rgw;/devices;/zones;/equipments;/schedules;/occupancy;/system"}',
+                    '"AdditionalParameters":{"JSONPath":"1;/systemControl;/systemController;/reminderSensors;/reminders;/alerts/active;/alerts/meta;/bleProvisionDB;/ble;/indoorAirQuality;/fwm;/rgw;/devices;/zones;/equipments;/schedules;/occupancy;/system"}',
                 )
                 ref = 2
                 await self.requestDataHelper(
                     lennoxSystem.sysId,
                     '"AdditionalParameters":{"JSONPath":"1;/automatedTest;/zoneTestControl;/homes;/reminders;/algorithm;/historyReportFileDetails;/interfaces;/logs"}',
                 )
```

### Comparing `lennoxs30api-0.2.1/lennoxs30api/s30exception.py` & `lennoxs30api-0.2.2/lennoxs30api/s30exception.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.1/lennoxs30api.egg-info/PKG-INFO` & `lennoxs30api-0.2.2/lennoxs30api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.1
+Version: 0.2.2
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.1/setup.py` & `lennoxs30api-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lennoxs30api",
-    version="0.2.1",
+    version="0.2.2",
     description="API Wrapper for Lennox S30 Cloud and LAN API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PeteRager/lennoxs30api",
     author="Pete Rage",
     author_email="pete.rager@x.com",
     license="MIT",
```

