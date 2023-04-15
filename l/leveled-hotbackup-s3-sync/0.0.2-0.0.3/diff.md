# Comparing `tmp/leveled_hotbackup_s3_sync-0.0.2-py3-none-any.whl.zip` & `tmp/leveled_hotbackup_s3_sync-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11833 bytes, number of entries: 11
+Zip file size: 11889 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      273 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/__init__.py
 -rw-r--r--  2.0 unx      273 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/__main__.py
 -rw-r--r--  2.0 unx     4054 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/app.py
 -rw-r--r--  2.0 unx     1029 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/hints.py
 -rw-r--r--  2.0 unx     2127 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/journal.py
 -rw-r--r--  2.0 unx     2221 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/manifest.py
 -rw-r--r--  2.0 unx     3801 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3169 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1011 b- defN 16-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.2.dist-info/RECORD
-11 files, 29403 bytes uncompressed, 10093 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3360 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1011 b- defN 16-Jan-01 00:00 leveled_hotbackup_s3_sync-0.0.3.dist-info/RECORD
+11 files, 29594 bytes uncompressed, 10149 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: leveled_hotbackup_s3_sync/manifest.py
 Comment: 
 
 Filename: leveled_hotbackup_s3_sync/utils.py
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.2.dist-info/LICENSE
+Filename: leveled_hotbackup_s3_sync-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.2.dist-info/METADATA
+Filename: leveled_hotbackup_s3_sync-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.2.dist-info/WHEEL
+Filename: leveled_hotbackup_s3_sync-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: leveled_hotbackup_s3_sync-0.0.2.dist-info/RECORD
+Filename: leveled_hotbackup_s3_sync-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `leveled_hotbackup_s3_sync-0.0.2.dist-info/LICENSE` & `leveled_hotbackup_s3_sync-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `leveled_hotbackup_s3_sync-0.0.2.dist-info/METADATA` & `leveled_hotbackup_s3_sync-0.0.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: leveled-hotbackup-s3-sync
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool to syncrhonise LevelEd hotbackup files to Amazon S3
+Home-page: https://github.com/yorkshire-steve/leveled-hotbackup-s3-sync
 License: Apache-2.0
+Keywords: riak,leveled,backup,s3
 Author: yorkshire-steve
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.114,<2.0.0)
 Requires-Dist: erlang-py (>=2.0.5,<3.0.0)
 Requires-Dist: pure-cdb (>=4.0.0,<5.0.0)
+Project-URL: Repository, https://github.com/yorkshire-steve/leveled-hotbackup-s3-sync
 Description-Content-Type: text/markdown
 
 # leveled-hotbackup-s3-sync
 A Python 3.8 tool which can backup and restore leveled hotbackups with Amazon S3
 
 ## Quick Start
 ```
```

## Comparing `leveled_hotbackup_s3_sync-0.0.2.dist-info/RECORD` & `leveled_hotbackup_s3_sync-0.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 leveled_hotbackup_s3_sync/__init__.py,sha256=Sa6E3LeYdkk0glQH1wRrrDQjRonVFno9rvrNqVrsUFA,273
 leveled_hotbackup_s3_sync/__main__.py,sha256=Sa6E3LeYdkk0glQH1wRrrDQjRonVFno9rvrNqVrsUFA,273
 leveled_hotbackup_s3_sync/app.py,sha256=jqwlCnbUGr17C7OKhdw4hR6MQdkqZbIUhlBP4sUGB4M,4054
 leveled_hotbackup_s3_sync/hints.py,sha256=gQyE-noNv6WHjKhBdn2CxasZ0kHFx5MrkQP-bWvOelU,1029
 leveled_hotbackup_s3_sync/journal.py,sha256=LGHiUc_r9VO_lQT42mYBUvoMHQ8sCwieD7mEGvl2Z10,2127
 leveled_hotbackup_s3_sync/manifest.py,sha256=ApJA7zEthxjemOtC4wR0zDIU-vEx5FpOQHFCxZYdI3A,2221
 leveled_hotbackup_s3_sync/utils.py,sha256=IfwpgQrGJq1zYbq0XF6Q361wNj6YmS64w_1Xa83PZ8Y,3801
-leveled_hotbackup_s3_sync-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-leveled_hotbackup_s3_sync-0.0.2.dist-info/METADATA,sha256=Ot78bbDNxfhFThAvtxvEdJoqKsbHMv1qITK6HkVXXdA,3169
-leveled_hotbackup_s3_sync-0.0.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-leveled_hotbackup_s3_sync-0.0.2.dist-info/RECORD,,
+leveled_hotbackup_s3_sync-0.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+leveled_hotbackup_s3_sync-0.0.3.dist-info/METADATA,sha256=GqEq6KhJutLFVTiQTEEPtLhAFHmin92GRQIoHDZBwXg,3360
+leveled_hotbackup_s3_sync-0.0.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+leveled_hotbackup_s3_sync-0.0.3.dist-info/RECORD,,
```

