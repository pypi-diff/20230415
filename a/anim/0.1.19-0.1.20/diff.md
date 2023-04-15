# Comparing `tmp/anim-0.1.19-py3-none-any.whl.zip` & `tmp/anim-0.1.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15911 bytes, number of entries: 13
--rwxrwxrwx  2.0 unx       59 b- defN 23-Apr-15 10:19 anim/__init__.py
+Zip file size: 15877 bytes, number of entries: 13
+-rwxrwxrwx  2.0 unx       60 b- defN 23-Apr-15 10:27 anim/__init__.py
 -rwxrwxrwx  2.0 unx    10555 b- defN 23-Apr-15 10:22 anim/body.py
 -rwxrwxrwx  2.0 unx     8745 b- defN 23-Apr-15 10:18 anim/model.py
 -rwxrwxrwx  2.0 unx     8078 b- defN 23-Apr-15 10:22 anim/util.py
 -rwxrwxrwx  2.0 unx       60 b- defN 23-Apr-15 09:55 src/__init__.py
 -rwxrwxrwx  2.0 unx    10973 b- defN 23-Apr-15 05:40 src/body.py
 -rwxrwxrwx  2.0 unx     8745 b- defN 23-Apr-15 05:40 src/model.py
 -rwxrwxrwx  2.0 unx     8869 b- defN 23-Apr-15 09:25 src/util.py
--rwxrwxrwx  2.0 unx     1070 b- defN 23-Apr-15 10:23 anim-0.1.19.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     1021 b- defN 23-Apr-15 10:23 anim-0.1.19.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 10:23 anim-0.1.19.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        5 b- defN 23-Apr-15 10:23 anim-0.1.19.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      931 b- defN 23-Apr-15 10:23 anim-0.1.19.dist-info/RECORD
-13 files, 59203 bytes uncompressed, 14399 bytes compressed:  75.7%
+-rwxrwxrwx  2.0 unx     1070 b- defN 23-Apr-15 10:27 anim-0.1.20.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx     1021 b- defN 23-Apr-15 10:27 anim-0.1.20.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 10:27 anim-0.1.20.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        5 b- defN 23-Apr-15 10:27 anim-0.1.20.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      931 b- defN 23-Apr-15 10:27 anim-0.1.20.dist-info/RECORD
+13 files, 59204 bytes uncompressed, 14365 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: src/model.py
 Comment: 
 
 Filename: src/util.py
 Comment: 
 
-Filename: anim-0.1.19.dist-info/LICENSE
+Filename: anim-0.1.20.dist-info/LICENSE
 Comment: 
 
-Filename: anim-0.1.19.dist-info/METADATA
+Filename: anim-0.1.20.dist-info/METADATA
 Comment: 
 
-Filename: anim-0.1.19.dist-info/WHEEL
+Filename: anim-0.1.20.dist-info/WHEEL
 Comment: 
 
-Filename: anim-0.1.19.dist-info/top_level.txt
+Filename: anim-0.1.20.dist-info/top_level.txt
 Comment: 
 
-Filename: anim-0.1.19.dist-info/RECORD
+Filename: anim-0.1.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anim/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .body import *
 from .model import *
-from util import *
+from .util import *
```

## Comparing `anim-0.1.19.dist-info/LICENSE` & `anim-0.1.20.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anim-0.1.19.dist-info/METADATA` & `anim-0.1.20.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anim
-Version: 0.1.19
+Version: 0.1.20
 Summary: Python package for anim
 Home-page: 
 Author: zhaoqyu
 Author-email: zhaoqyu@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

## Comparing `anim-0.1.19.dist-info/RECORD` & `anim-0.1.20.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-anim/__init__.py,sha256=Cy4IGLCfRzOBVw_2Q_BYCZlr9zuDe6QmsBVsiMqqK9I,59
+anim/__init__.py,sha256=wUkJtSJ_DWMbN2Pe4d4WA31P43CS9_H7uTW2ZoxaXVY,60
 anim/body.py,sha256=5VYD7CKV_He6xvj4RVKCgzCQByH-NAbfDBSZf7nxHJ4,10555
 anim/model.py,sha256=9Xc6-5jpbf9uW2-35wV08cEYBArDWQoiF0akLUV6FdM,8745
 anim/util.py,sha256=jXn7g98QJxWizoydD3Ous1ydDHX3WdJTm8B16VmIHV0,8078
 src/__init__.py,sha256=wUkJtSJ_DWMbN2Pe4d4WA31P43CS9_H7uTW2ZoxaXVY,60
 src/body.py,sha256=mjAWfe86Ur2eCwXwmRdfsprjqlty5HCFZ4vAorMQBbQ,10973
 src/model.py,sha256=9Xc6-5jpbf9uW2-35wV08cEYBArDWQoiF0akLUV6FdM,8745
 src/util.py,sha256=AAvC8IBxcmfXVoQscnenbNwLMOOwNnEEDR29phU8UhA,8869
-anim-0.1.19.dist-info/LICENSE,sha256=WsrxnSVZq3kchu3dO20NECj5Aw3tr-uqGB7qj548iXk,1070
-anim-0.1.19.dist-info/METADATA,sha256=SHeUmz1HTLzbwzIPbrTgQFk9zRp_N0iP4Ge01_Ux4n8,1021
-anim-0.1.19.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-anim-0.1.19.dist-info/top_level.txt,sha256=6EuFjP3SC8OdvBC_G4gGmy89cQIlpQuQNy5knCtvf2s,5
-anim-0.1.19.dist-info/RECORD,,
+anim-0.1.20.dist-info/LICENSE,sha256=WsrxnSVZq3kchu3dO20NECj5Aw3tr-uqGB7qj548iXk,1070
+anim-0.1.20.dist-info/METADATA,sha256=wMRyVF_jbUgpbpQUivRxaPpO2wvL0g-bgfHUThV3Uc4,1021
+anim-0.1.20.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+anim-0.1.20.dist-info/top_level.txt,sha256=6EuFjP3SC8OdvBC_G4gGmy89cQIlpQuQNy5knCtvf2s,5
+anim-0.1.20.dist-info/RECORD,,
```

