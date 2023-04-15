# Comparing `tmp/ovos_listener-0.0.2a6-py3-none-any.whl.zip` & `tmp/ovos_listener-0.0.2a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5848 bytes, number of entries: 6
--rw-r--r--  2.0 unx    11423 b- defN 23-Apr-06 23:16 ovos_listener-0.0.2a6.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1066 b- defN 23-Apr-06 23:16 ovos_listener-0.0.2a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 23:16 ovos_listener-0.0.2a6.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Apr-06 23:16 ovos_listener-0.0.2a6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-06 23:16 ovos_listener-0.0.2a6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      532 b- defN 23-Apr-06 23:16 ovos_listener-0.0.2a6.dist-info/RECORD
-6 files, 13177 bytes uncompressed, 4870 bytes compressed:  63.0%
+Zip file size: 5850 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    11423 b- defN 23-Apr-15 02:04 ovos_listener-0.0.2a7.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-15 02:04 ovos_listener-0.0.2a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 02:04 ovos_listener-0.0.2a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Apr-15 02:04 ovos_listener-0.0.2a7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 02:04 ovos_listener-0.0.2a7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      532 b- defN 23-Apr-15 02:04 ovos_listener-0.0.2a7.dist-info/RECORD
+6 files, 13178 bytes uncompressed, 4872 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: ovos_listener-0.0.2a6.dist-info/LICENSE.md
+Filename: ovos_listener-0.0.2a7.dist-info/LICENSE.md
 Comment: 
 
-Filename: ovos_listener-0.0.2a6.dist-info/METADATA
+Filename: ovos_listener-0.0.2a7.dist-info/METADATA
 Comment: 
 
-Filename: ovos_listener-0.0.2a6.dist-info/WHEEL
+Filename: ovos_listener-0.0.2a7.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_listener-0.0.2a6.dist-info/entry_points.txt
+Filename: ovos_listener-0.0.2a7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_listener-0.0.2a6.dist-info/top_level.txt
+Filename: ovos_listener-0.0.2a7.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_listener-0.0.2a6.dist-info/RECORD
+Filename: ovos_listener-0.0.2a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ovos_listener-0.0.2a6.dist-info/LICENSE.md` & `ovos_listener-0.0.2a7.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `ovos_listener-0.0.2a6.dist-info/METADATA` & `ovos_listener-0.0.2a7.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-listener
-Version: 0.0.2a6
+Version: 0.0.2a7
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-listener
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Requires-Dist: ovos-ww-plugin-pocketsphinx (>=0.1.3,~=0.1)
 Requires-Dist: ovos-ww-plugin-precise-lite (>=0.1.2a3,~=0.1)
 Requires-Dist: ovos-ww-plugin-precise (>=0.1.1,~=0.1)
 Requires-Dist: ovos-ww-plugin-vosk
 Requires-Dist: ovos-stt-plugin-server (>=0.0.2,~=0.0)
 Requires-Dist: ovos-stt-plugin-vosk (~=0.1)
 Requires-Dist: ovos-utils (>=0.0.31a3,~=0.0)
-Requires-Dist: ovos-bus-client (>=0.0.3a4,~=0.0)
+Requires-Dist: ovos-bus-client (>=0.0.3a16,~=0.0)
 Requires-Dist: ovos-plugin-manager (>=0.0.23a5,~=0.0)
-Requires-Dist: ovos-config (>=0.0.8a2,~=0.0)
+Requires-Dist: ovos-config (>=0.0.8a3,~=0.0)
 Requires-Dist: ovos-backend-client (>=0.0.7a2,~=0.0)
 
 UNKNOWN
```

## Comparing `ovos_listener-0.0.2a6.dist-info/RECORD` & `ovos_listener-0.0.2a7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-ovos_listener-0.0.2a6.dist-info/LICENSE.md,sha256=HP46TQN2uSd_OW1lJPi1TJ-SVSgLJXixGmY9C16CQJQ,11423
-ovos_listener-0.0.2a6.dist-info/METADATA,sha256=6vQ_8SkijbX17a9XnSUYkakWCRtcHTmXLk6Vw4YY3zU,1066
-ovos_listener-0.0.2a6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_listener-0.0.2a6.dist-info/entry_points.txt,sha256=8tMSAxrLEn880nBqPzhc-m5nBAWp8UqLDMn_Kor3O6g,63
-ovos_listener-0.0.2a6.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_listener-0.0.2a6.dist-info/RECORD,,
+ovos_listener-0.0.2a7.dist-info/LICENSE.md,sha256=HP46TQN2uSd_OW1lJPi1TJ-SVSgLJXixGmY9C16CQJQ,11423
+ovos_listener-0.0.2a7.dist-info/METADATA,sha256=dX8jFJZlhOZRWwwVitX7Ry18OgvHqpXz5IkOUGYgMVk,1067
+ovos_listener-0.0.2a7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_listener-0.0.2a7.dist-info/entry_points.txt,sha256=8tMSAxrLEn880nBqPzhc-m5nBAWp8UqLDMn_Kor3O6g,63
+ovos_listener-0.0.2a7.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_listener-0.0.2a7.dist-info/RECORD,,
```

