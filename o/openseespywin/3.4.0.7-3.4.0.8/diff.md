# Comparing `tmp/openseespywin-3.4.0.7-py3-none-any.whl.zip` & `tmp/openseespywin-3.4.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5940146 bytes, number of entries: 8
+Zip file size: 5808569 bytes, number of entries: 8
 -rw-rw----  2.0 unx     1073 b- defN 22-Jul-18 00:07 openseespywin/LICENSE.md
 -rw-r--r--  2.0 unx      762 b- defN 22-Nov-28 19:43 openseespywin/__init__.py
--rw-rw----  2.0 unx 14959104 b- defN 23-Apr-03 05:17 openseespywin/opensees.pyd
+-rw-rw----  2.0 unx 14628352 b- defN 23-Apr-03 20:30 openseespywin/opensees.pyd
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-18 00:07 openseespywin/lib/__init__.py
--rw-r--r--  2.0 unx     1014 b- defN 23-Apr-03 19:47 openseespywin-3.4.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 19:47 openseespywin-3.4.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-03 19:47 openseespywin-3.4.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      662 b- defN 23-Apr-03 19:47 openseespywin-3.4.0.7.dist-info/RECORD
-8 files, 14962721 bytes uncompressed, 5938988 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx     1014 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      662 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/RECORD
+8 files, 14631969 bytes uncompressed, 5807411 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: openseespywin/opensees.pyd
 Comment: 
 
 Filename: openseespywin/lib/__init__.py
 Comment: 
 
-Filename: openseespywin-3.4.0.7.dist-info/METADATA
+Filename: openseespywin-3.4.0.8.dist-info/METADATA
 Comment: 
 
-Filename: openseespywin-3.4.0.7.dist-info/WHEEL
+Filename: openseespywin-3.4.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: openseespywin-3.4.0.7.dist-info/top_level.txt
+Filename: openseespywin-3.4.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: openseespywin-3.4.0.7.dist-info/RECORD
+Filename: openseespywin-3.4.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `openseespywin-3.4.0.7.dist-info/METADATA` & `openseespywin-3.4.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseespywin
-Version: 3.4.0.7
+Version: 3.4.0.8
 Summary: A OpenSeesPy Windows package
 Home-page: https://github.com/zhuminjie/openseespy
 Author: Minjie Zhu
 Author-email: zhum@oregonstate.edu
 License: LICENSE.md
 Platform: Windows
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `openseespywin-3.4.0.7.dist-info/RECORD` & `openseespywin-3.4.0.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 openseespywin/LICENSE.md,sha256=OT3Bt-KttaggiLhu5ITmx9bhaS4xGih3JyHAhNUnfFc,1073
 openseespywin/__init__.py,sha256=FzBKKc8B5u48hxMol0XK2j-qL29R2iPXgXRXiHAtwe8,762
-openseespywin/opensees.pyd,sha256=d-jQBK7-PWKJuyluZC5tkyZ9oD9Gen67snlfYY1JV6M,14959104
+openseespywin/opensees.pyd,sha256=2yMaEmUbQ6FEWccdeR7aNRn9mO5oPAmRA20sambOCHo,14628352
 openseespywin/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-openseespywin-3.4.0.7.dist-info/METADATA,sha256=CD08eM_3MaZ_K-Pnpxd4edZXjHECLoCWHzj-FS4-3-I,1014
-openseespywin-3.4.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openseespywin-3.4.0.7.dist-info/top_level.txt,sha256=M-xKulaColQWDllAxMKDXCaVRxQxDyC-g0aTzQ6pmVY,14
-openseespywin-3.4.0.7.dist-info/RECORD,,
+openseespywin-3.4.0.8.dist-info/METADATA,sha256=Bdi0slve97hL96CvWpwr4vZyFV9rnrkpOD1FnhlYpfQ,1014
+openseespywin-3.4.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openseespywin-3.4.0.8.dist-info/top_level.txt,sha256=M-xKulaColQWDllAxMKDXCaVRxQxDyC-g0aTzQ6pmVY,14
+openseespywin-3.4.0.8.dist-info/RECORD,,
```

