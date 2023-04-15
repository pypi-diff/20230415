# Comparing `tmp/awc-1.2.0-py2.py3-none-any.whl.zip` & `tmp/awc-1.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23683 bytes, number of entries: 16
--rw-r--r--  2.0 unx     6692 b- defN 23-Apr-13 15:09 awc/__init__.py
+Zip file size: 23717 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     6692 b- defN 23-Apr-15 17:02 awc/__init__.py
 -rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
--rw-r--r--  2.0 unx     5416 b- defN 23-Apr-13 15:09 awc/api.py
+-rw-r--r--  2.0 unx     5635 b- defN 23-Apr-15 16:25 awc/api.py
 -rw-r--r--  2.0 unx      305 b- defN 23-Apr-12 22:27 awc/const.py
 -rw-r--r--  2.0 unx     1600 b- defN 23-Apr-13 14:32 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
 -rw-r--r--  2.0 unx     1383 b- defN 23-Apr-13 14:54 awc/util.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 22:27 awc/wrn.py
 -rw-r--r--  2.0 unx     4429 b- defN 23-Apr-13 15:08 awc/sql/__init__.py
 -rw-r--r--  2.0 unx     2867 b- defN 23-Apr-13 15:11 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3780 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.2.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-13 15:14 awc-1.2.0.dist-info/RECORD
-16 files, 64131 bytes uncompressed, 21847 bytes compressed:  65.9%
+-rw-------  2.0 unx    35107 b- defN 23-Apr-15 17:14 awc-1.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3812 b- defN 23-Apr-15 17:14 awc-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-15 17:14 awc-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-15 17:14 awc-1.2.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.2.1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-15 17:14 awc-1.2.1.dist-info/RECORD
+16 files, 64382 bytes uncompressed, 21881 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-1.2.0.dist-info/LICENSE
+Filename: awc-1.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: awc-1.2.0.dist-info/METADATA
+Filename: awc-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: awc-1.2.0.dist-info/WHEEL
+Filename: awc-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: awc-1.2.0.dist-info/top_level.txt
+Filename: awc-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-1.2.0.dist-info/zip-safe
+Filename: awc-1.2.1.dist-info/zip-safe
 Comment: 
 
-Filename: awc-1.2.0.dist-info/RECORD
+Filename: awc-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc/__init__.py

```diff
@@ -7,15 +7,15 @@
 from functools import wraps
 
 import requests
 from furl import furl  # type: ignore
 
 from . import const, exc, util
 
-__version__: typing.Final[str] = "1.2.0"
+__version__: typing.Final[str] = "1.2.1"
 
 
 class Awc:
     """ari-web comments interface
 
     this is where all API requests begin, you must
     pass an instance of this object to every api wrapper
```

## awc/api.py

```diff
@@ -169,7 +169,14 @@
 
 
 def amiadmin(awc: Awc) -> bool:
     """returns your admin status ( `True` if API key is correct ( you are admin ) )
 
     awc: awc.Awc -- the awc.Awc instance to work on"""
     return util.resp_to_bool(awc.get(api="amiadmin").text)
+
+
+def applied(awc: Awc) -> bool:
+    """returns your application status ( `True` if applied / accepted )
+
+    awc: awc.Awc -- the awc.Awc instance to work on"""
+    return util.resp_to_bool(awc.get(api="applied").text)
```

## Comparing `awc-1.2.0.dist-info/LICENSE` & `awc-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc-1.2.0.dist-info/METADATA` & `awc-1.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc
-Version: 1.2.0
+Version: 1.2.1
 Summary: wrapper for ari-web comments API
 Home-page: https://ari-web.xyz/gh/awc
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,comments,api,wrapper,https
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: types-requests
+Requires-Dist: types-sqlalchemy
 Requires-Dist: furl
 Requires-Dist: pypika
 
 # awc
 
 > ari-web comments ( awc ) API wrapper
```

## Comparing `awc-1.2.0.dist-info/RECORD` & `awc-1.2.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-awc/__init__.py,sha256=_z-WGFsnNEQ-WoZvnJMBnJ_8kf6qvpZ4TXJGGrzPFys,6692
+awc/__init__.py,sha256=efTGZWwPWgrZogtaPWqJI_X4ulurVqJ6XxvSO_bMyeg,6692
 awc/__main__.py,sha256=d1UfoKcH5bl9qoqWowmcARIitWbbGsasAZfq8RHHsE4,678
-awc/api.py,sha256=qjOu6IBk1ULcnlzk7Ocehmu9YfBsBH8MJPOartBOQjs,5416
+awc/api.py,sha256=I-SKlNj-AqVqmYjqkEct3WauCbQBYGYrGF1tYzHACK0,5635
 awc/const.py,sha256=0ctjO9muVRU7kBkqF9LjcgwvP4baLum63UUOxTE1oLw,305
 awc/exc.py,sha256=2tb9dhfT_0KNV0eNCm4RP5M_5s9i6cCxOq-PmbHzFbs,1600
 awc/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc/util.py,sha256=u9-_per8iyglLx9dVfQKJBdSEFZq2-5aymE7XDjoJ0o,1383
 awc/wrn.py,sha256=K84cpt9OdHQi76vhgMsWFbl8rIN_sH6EkOGptZOUWmQ,614
 awc/sql/__init__.py,sha256=y6htpvQk69bk_pVAoVXUKZkCHN8X2jzg_I9Wjf52bUY,4429
 awc/sql/helpers.py,sha256=4IiFOVP6wnrhKYb4GBaXX-SnIe7dD_JND8INkle9W0Y,2867
-awc-1.2.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
-awc-1.2.0.dist-info/METADATA,sha256=BF4bF8Emy9aod2Z4vIcn6C_MDXBV5osVUpqxZqlBfXU,3780
-awc-1.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc-1.2.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
-awc-1.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc-1.2.0.dist-info/RECORD,,
+awc-1.2.1.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
+awc-1.2.1.dist-info/METADATA,sha256=KiWVgx8HJWKE8RtNC360amM7Fh-Ey_DaX4ZXy-LrHjI,3812
+awc-1.2.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc-1.2.1.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
+awc-1.2.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc-1.2.1.dist-info/RECORD,,
```

