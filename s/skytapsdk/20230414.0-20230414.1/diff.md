# Comparing `tmp/skytapsdk-20230414.0.tar.gz` & `tmp/skytapsdk-20230414.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytapsdk-20230414.0.tar", last modified: Fri Apr 14 16:29:59 2023, max compression
+gzip compressed data, was "skytapsdk-20230414.1.tar", last modified: Sat Apr 15 01:28:55 2023, max compression
```

## Comparing `skytapsdk-20230414.0.tar` & `skytapsdk-20230414.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.835550 skytapsdk-20230414.0/
--rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:30.000000 skytapsdk-20230414.0/LICENSE.md
--rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-14 16:29:59.835615 skytapsdk-20230414.0/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-04-14 16:29:59.835822 skytapsdk-20230414.0/setup.cfg
--rw-r--r--   0 dmickelson   (503) staff       (20)     1389 2023-04-14 16:28:55.000000 skytapsdk-20230414.0/setup.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.833889 skytapsdk-20230414.0/skytapsdk/
--rw-r--r--   0 dmickelson   (503) staff       (20)      165 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/__init__.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1334 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.834722 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/
--rw-r--r--   0 dmickelson   (503) staff       (20)      116 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/__init__.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1277 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/events.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      374 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/self_learners.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1481 2023-02-07 15:11:48.000000 skytapsdk-20230414.0/skytapsdk/helpers.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     3204 2023-04-14 16:29:25.000000 skytapsdk-20230414.0/skytapsdk/skytap.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.835457 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/
--rw-r--r--   0 dmickelson   (503) staff       (20)      294 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/__init__.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1068 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/assets.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1141 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/environments.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1609 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/projects.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1138 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/reports.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1102 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/templates.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1316 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/users.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.834409 skytapsdk-20230414.0/skytapsdk.egg-info/
--rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)      700 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/SOURCES.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/dependency_links.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        8 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/requires.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)       10 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/top_level.txt
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-15 01:28:55.326878 skytapsdk-20230414.1/
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:30.000000 skytapsdk-20230414.1/LICENSE.md
+-rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-15 01:28:55.326944 skytapsdk-20230414.1/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-04-15 01:28:55.327138 skytapsdk-20230414.1/setup.cfg
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1389 2023-04-15 01:27:15.000000 skytapsdk-20230414.1/setup.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-15 01:28:55.324957 skytapsdk-20230414.1/skytapsdk/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      165 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1334 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/course_manager.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-15 01:28:55.325891 skytapsdk-20230414.1/skytapsdk/course_manager_endpoints/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      116 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/course_manager_endpoints/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1139 2023-04-15 01:24:40.000000 skytapsdk-20230414.1/skytapsdk/course_manager_endpoints/events.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      423 2023-04-15 01:26:09.000000 skytapsdk-20230414.1/skytapsdk/course_manager_endpoints/self_learners.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1481 2023-02-07 15:11:48.000000 skytapsdk-20230414.1/skytapsdk/helpers.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     3204 2023-04-15 01:27:17.000000 skytapsdk-20230414.1/skytapsdk/skytap.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-15 01:28:55.326778 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      294 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1068 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/assets.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1141 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/environments.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1609 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/projects.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1138 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/reports.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1102 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/templates.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1316 2023-04-14 16:28:41.000000 skytapsdk-20230414.1/skytapsdk/skytap_endpoints/users.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-15 01:28:55.325452 skytapsdk-20230414.1/skytapsdk.egg-info/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-15 01:28:55.000000 skytapsdk-20230414.1/skytapsdk.egg-info/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)      700 2023-04-15 01:28:55.000000 skytapsdk-20230414.1/skytapsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-04-15 01:28:55.000000 skytapsdk-20230414.1/skytapsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        8 2023-04-15 01:28:55.000000 skytapsdk-20230414.1/skytapsdk.egg-info/requires.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)       10 2023-04-15 01:28:55.000000 skytapsdk-20230414.1/skytapsdk.egg-info/top_level.txt
```

### Comparing `skytapsdk-20230414.0/LICENSE.md` & `skytapsdk-20230414.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/PKG-INFO` & `skytapsdk-20230414.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytapsdk
-Version: 20230414.0
+Version: 20230414.1
 Summary: SDK for interacting with Skytap's APIs.
 Home-page: 
 Author: Dax Mickelson
 Author-email: dmickelson@zscaler.com
 License: BSD
 Keywords: skytap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skytapsdk-20230414.0/setup.py` & `skytapsdk-20230414.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version = "20230414.0"
+__version = "20230414.1"
 __author = "Dax Mickelson"
 __author_email = "dmickelson@zscaler.com"
 __license = "BSD"
 __name = "skytapsdk"
 __description = "SDK for interacting with Skytap's APIs."
 __long_description = __description
 __url = ""
```

### Comparing `skytapsdk-20230414.0/skytapsdk/course_manager.py` & `skytapsdk-20230414.1/skytapsdk/course_manager.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/events.py` & `skytapsdk-20230414.1/skytapsdk/course_manager_endpoints/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,40 +9,40 @@
     """
 
     _path = "events"
 
     def get(
         self,
         event_id: str = None,
+        **kwargs,
     ) -> requests.Response:
         if event_id:
             self._path = f"{self._path}/{event_id}"
-        return self._get(verify=False)
+        return self._get(**kwargs)
 
     def get_participants(
         self,
         event_id: str,
-        participant_id: str = None,
-    ) -> requests.Response:
-        pass  # FIXME: This doesn't work yet.
-        # self._path = f"{self._path}/{event_id}"
-        # parameters = {
-        #     "tab": "participants-tab",
-        # }
-        # return self._get(verify=False, params=parameters,)
-
-        # self._path = f"{self._path}/{event_id}/students"
-        # if participant_id:
-        #     self._path = f"{self._path}/{participant_id}"
-        # return self._get(verify=False)
+        **kwargs,
+    ) -> list:
+        """This uses the event.get() to get the events and then returns just the "students" list from the return."""
+        result = self.get(
+            event_id=event_id,
+            **kwargs,
+        )
+        return result.json().get(
+            "students",
+            [],
+        )
 
-    def update_participants(
+    def update_participant(
         self,
         event_id: str,
         participant_id: str,
         payload: dict,
+        **kwargs,
     ) -> requests.Response:
         self._path = f"{self._path}/{event_id}/event_participants/{participant_id}"
         return self._patch(
             json=payload,
-            verify=False,
+            **kwargs,
         )
```

### Comparing `skytapsdk-20230414.0/skytapsdk/helpers.py` & `skytapsdk-20230414.1/skytapsdk/helpers.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/skytap.py` & `skytapsdk-20230414.1/skytapsdk/skytap.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/assets.py` & `skytapsdk-20230414.1/skytapsdk/skytap_endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/environments.py` & `skytapsdk-20230414.1/skytapsdk/skytap_endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/projects.py` & `skytapsdk-20230414.1/skytapsdk/skytap_endpoints/projects.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/reports.py` & `skytapsdk-20230414.1/skytapsdk/skytap_endpoints/reports.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/templates.py` & `skytapsdk-20230414.1/skytapsdk/skytap_endpoints/templates.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/users.py` & `skytapsdk-20230414.1/skytapsdk/skytap_endpoints/users.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230414.0/skytapsdk.egg-info/PKG-INFO` & `skytapsdk-20230414.1/skytapsdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytapsdk
-Version: 20230414.0
+Version: 20230414.1
 Summary: SDK for interacting with Skytap's APIs.
 Home-page: 
 Author: Dax Mickelson
 Author-email: dmickelson@zscaler.com
 License: BSD
 Keywords: skytap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skytapsdk-20230414.0/skytapsdk.egg-info/SOURCES.txt` & `skytapsdk-20230414.1/skytapsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

