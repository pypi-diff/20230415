# Comparing `tmp/iosense_connect-2.0.7.tar.gz` & `tmp/iosense_connect-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.0.7.tar", last modified: Thu Apr  6 10:20:25 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.0.8.tar", last modified: Sat Apr 15 12:10:58 2023, max compression
```

## Comparing `iosense_connect-2.0.7.tar` & `iosense_connect-2.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:20:25.467097 iosense_connect-2.0.7/
--rw-rw-rw-   0        0        0      117 2023-04-06 10:20:25.395080 iosense_connect-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-06 06:23:07.000000 iosense_connect-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 10:20:25.357221 iosense_connect-2.0.7/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.0.7/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    18996 2023-04-06 10:18:10.000000 iosense_connect-2.0.7/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:20:25.389912 iosense_connect-2.0.7/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0      117 2023-04-06 10:20:25.000000 iosense_connect-2.0.7/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-06 10:20:25.000000 iosense_connect-2.0.7/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:20:25.000000 iosense_connect-2.0.7/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-06 10:20:25.000000 iosense_connect-2.0.7/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 10:20:25.468100 iosense_connect-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0      207 2023-04-06 10:20:23.000000 iosense_connect-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:10:58.175881 iosense_connect-2.0.8/
+-rw-rw-rw-   0        0        0      117 2023-04-15 12:10:58.173475 iosense_connect-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-06 06:23:07.000000 iosense_connect-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 12:10:58.113609 iosense_connect-2.0.8/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.0.8/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    19421 2023-04-15 12:10:25.000000 iosense_connect-2.0.8/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:10:58.169022 iosense_connect-2.0.8/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0      117 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-15 12:10:57.000000 iosense_connect-2.0.8/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 12:10:58.175881 iosense_connect-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      207 2023-04-15 12:10:44.000000 iosense_connect-2.0.8/setup.py
```

### Comparing `iosense_connect-2.0.7/README.md` & `iosense_connect-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.0.7/iosense_connect/data_access.py` & `iosense_connect-2.0.8/iosense_connect/data_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,14 +217,21 @@
 
         Get Data Point fetches data containing values of last n data points of given sensor at given time.
 
         """
         try:
             metadata = {}
 
+            try:
+                end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
+                print(end_time)
+            except Exception as e:
+                end_time = end_time + " 23:59:59"
+                pass
+
             end_time = pd.to_datetime(end_time)
             if IST:
                 end_time = end_time - timedelta(hours=5, minutes=30)
             end_time = int(round(end_time.timestamp()))
             if type(sensors) == list:
                 len_sensors = len(sensors)
                 if len_sensors == 0:
@@ -282,14 +289,20 @@
             metadata = DataAccess.get_device_metadata(self, device_id)
             data_sensor = metadata['sensors']
             df_sensor = pd.DataFrame(data_sensor)
             sensor_id_list = list(df_sensor['sensorId'])
             sensors = sensor_id_list
         rawdata_res = []
         temp = ''
+        try:
+            end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
+        except Exception as e:
+            end_time = end_time + " 23:59:59"
+            pass
+
         s_time = pd.to_datetime(start_time)
         e_time = pd.to_datetime(end_time)
         if IST:
             s_time = s_time - timedelta(hours=5, minutes=30)
             e_time = e_time - timedelta(hours=5, minutes=30)
         st_time = int(round(s_time.timestamp())) * 10000
         en_time = int(round(e_time.timestamp())) * 10000
```

