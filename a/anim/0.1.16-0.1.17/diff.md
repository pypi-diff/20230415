# Comparing `tmp/anim-0.1.16-py3-none-any.whl.zip` & `tmp/anim-0.1.17-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9236 bytes, number of entries: 9
--rwxrwxrwx  2.0 unx        0 b- defN 23-Apr-15 05:40 src/__init__.py
+Zip file size: 9271 bytes, number of entries: 9
+-rwxrwxrwx  2.0 unx       60 b- defN 23-Apr-15 09:55 src/__init__.py
 -rwxrwxrwx  2.0 unx    10973 b- defN 23-Apr-15 05:40 src/body.py
 -rwxrwxrwx  2.0 unx     8745 b- defN 23-Apr-15 05:40 src/model.py
 -rwxrwxrwx  2.0 unx     8869 b- defN 23-Apr-15 09:25 src/util.py
--rwxrwxrwx  2.0 unx     1070 b- defN 23-Apr-15 09:48 anim-0.1.16.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     1021 b- defN 23-Apr-15 09:48 anim-0.1.16.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 09:48 anim-0.1.16.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        4 b- defN 23-Apr-15 09:48 anim-0.1.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-15 09:48 anim-0.1.16.dist-info/RECORD
-9 files, 31424 bytes uncompressed, 8134 bytes compressed:  74.1%
+-rwxrwxrwx  2.0 unx     1070 b- defN 23-Apr-15 09:56 anim-0.1.17.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx     1021 b- defN 23-Apr-15 09:56 anim-0.1.17.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 09:56 anim-0.1.17.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        4 b- defN 23-Apr-15 09:56 anim-0.1.17.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      651 b- defN 23-Apr-15 09:56 anim-0.1.17.dist-info/RECORD
+9 files, 31485 bytes uncompressed, 8169 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: src/model.py
 Comment: 
 
 Filename: src/util.py
 Comment: 
 
-Filename: anim-0.1.16.dist-info/LICENSE
+Filename: anim-0.1.17.dist-info/LICENSE
 Comment: 
 
-Filename: anim-0.1.16.dist-info/METADATA
+Filename: anim-0.1.17.dist-info/METADATA
 Comment: 
 
-Filename: anim-0.1.16.dist-info/WHEEL
+Filename: anim-0.1.17.dist-info/WHEEL
 Comment: 
 
-Filename: anim-0.1.16.dist-info/top_level.txt
+Filename: anim-0.1.17.dist-info/top_level.txt
 Comment: 
 
-Filename: anim-0.1.16.dist-info/RECORD
+Filename: anim-0.1.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 6672 6f6d 202e 626f 6479 2069 6d70 6f72  from .body impor
+00000010: 7420 2a0a 6672 6f6d 202e 6d6f 6465 6c20  t *.from .model 
+00000020: 696d 706f 7274 202a 0a66 726f 6d20 2e75  import *.from .u
+00000030: 7469 6c20 696d 706f 7274 202a            til import *
```

## Comparing `anim-0.1.16.dist-info/LICENSE` & `anim-0.1.17.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anim-0.1.16.dist-info/METADATA` & `anim-0.1.17.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anim
-Version: 0.1.16
+Version: 0.1.17
 Summary: Python package for anim
 Home-page: 
 Author: zhaoqyu
 Author-email: zhaoqyu@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

