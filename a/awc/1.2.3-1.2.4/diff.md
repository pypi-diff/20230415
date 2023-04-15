# Comparing `tmp/awc-1.2.3-py2.py3-none-any.whl.zip` & `tmp/awc-1.2.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23753 bytes, number of entries: 16
--rw-r--r--  2.0 unx     6843 b- defN 23-Apr-15 19:55 awc/__init__.py
+Zip file size: 23718 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     6843 b- defN 23-Apr-15 21:04 awc/__init__.py
 -rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
 -rw-r--r--  2.0 unx     5635 b- defN 23-Apr-15 16:25 awc/api.py
 -rw-r--r--  2.0 unx      305 b- defN 23-Apr-12 22:27 awc/const.py
--rw-r--r--  2.0 unx     1600 b- defN 23-Apr-13 14:32 awc/exc.py
+-rw-r--r--  2.0 unx     1479 b- defN 23-Apr-15 21:04 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
 -rw-r--r--  2.0 unx     1383 b- defN 23-Apr-13 14:54 awc/util.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 22:27 awc/wrn.py
 -rw-r--r--  2.0 unx     4429 b- defN 23-Apr-13 15:08 awc/sql/__init__.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Apr-13 15:11 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-Apr-15 19:56 awc-1.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3812 b- defN 23-Apr-15 19:56 awc-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-15 19:56 awc-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-15 19:56 awc-1.2.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.2.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-15 19:56 awc-1.2.3.dist-info/RECORD
-16 files, 64533 bytes uncompressed, 21917 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx     2867 b- defN 23-Apr-15 20:00 awc/sql/helpers.py
+-rw-------  2.0 unx    35107 b- defN 23-Apr-15 21:06 awc-1.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3812 b- defN 23-Apr-15 21:06 awc-1.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-15 21:06 awc-1.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-15 21:06 awc-1.2.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.2.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-15 21:06 awc-1.2.4.dist-info/RECORD
+16 files, 64412 bytes uncompressed, 21882 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-1.2.3.dist-info/LICENSE
+Filename: awc-1.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: awc-1.2.3.dist-info/METADATA
+Filename: awc-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: awc-1.2.3.dist-info/WHEEL
+Filename: awc-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: awc-1.2.3.dist-info/top_level.txt
+Filename: awc-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-1.2.3.dist-info/zip-safe
+Filename: awc-1.2.4.dist-info/zip-safe
 Comment: 
 
-Filename: awc-1.2.3.dist-info/RECORD
+Filename: awc-1.2.4.dist-info/RECORD
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
 
-__version__: typing.Final[str] = "1.2.3"
+__version__: typing.Final[str] = "1.2.4"
 
 
 class Awc:
     """ari-web comments interface
 
     this is where all API requests begin, you must
     pass an instance of this object to every api wrapper
```

## awc/exc.py

```diff
@@ -7,53 +7,53 @@
 import requests
 
 
 class AWCException(Exception):
     """base awc exception"""
 
 
-class InvalidInstanceURLError(AWCException, requests.exceptions.InvalidURL):
+class InvalidInstanceURLError(AWCException):
     """raised when an API instance URL isnt valid"""
 
     instance: str
 
     def __init__(self, instance: str) -> None:
         super().__init__(instance)  # type: ignore
         self.instance: str = instance
 
 
-class APIRequestFailedError(AWCException, requests.exceptions.HTTPError):
+class APIRequestFailedError(AWCException):
     """raised when a request to an API fails"""
 
     api: str
 
     def __init__(self, api: str, response: requests.Response) -> None:
         super().__init__(api)  # type: ignore
         self.api: str = api
         self.response: requests.Response = response
 
 
-class NoAPIKeyError(AWCException, PermissionError):
+class NoAPIKeyError(AWCException):
     """raised when no API key is provided"""
 
 
-class InvalidAPIKeyError(AWCException, PermissionError):
+class InvalidAPIKeyError(AWCException):
     """raised when the API key is invalid"""
 
 
-class UnexpectedResponseError(AWCException, ValueError):
+class UnexpectedResponseError(AWCException):
     """raised when the API returns an unexpected response"""
 
     def __init__(self, value: str, expected: type) -> None:
         super().__init__(
             f"got {value!r}, but we expected something of type {expected!r}"
         )
         self.value: str = value
         self.expected: type = expected
 
 
-class ResouceNotFoundError(AWCException, ValueError):
+class ResouceNotFoundError(AWCException):
     """raised when the API doesnt return the requested resource"""
 
     def __init__(self, value: typing.Any) -> None:
         super().__init__(value)
         self.value: typing.Any = value
```

## Comparing `awc-1.2.3.dist-info/LICENSE` & `awc-1.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc-1.2.3.dist-info/METADATA` & `awc-1.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc
-Version: 1.2.3
+Version: 1.2.4
 Summary: wrapper for ari-web comments API
 Home-page: https://ari-web.xyz/gh/awc
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,comments,api,wrapper,https
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `awc-1.2.3.dist-info/RECORD` & `awc-1.2.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-awc/__init__.py,sha256=2oFPKh7BO-N4xTpQ8GdMm-fjmxii_eDlJQ_avnza6V4,6843
+awc/__init__.py,sha256=LPXsXw7peC08WmuD055TyVkKkoDqorV_C0sdZ4BceXY,6843
 awc/__main__.py,sha256=d1UfoKcH5bl9qoqWowmcARIitWbbGsasAZfq8RHHsE4,678
 awc/api.py,sha256=I-SKlNj-AqVqmYjqkEct3WauCbQBYGYrGF1tYzHACK0,5635
 awc/const.py,sha256=0ctjO9muVRU7kBkqF9LjcgwvP4baLum63UUOxTE1oLw,305
-awc/exc.py,sha256=2tb9dhfT_0KNV0eNCm4RP5M_5s9i6cCxOq-PmbHzFbs,1600
+awc/exc.py,sha256=kGwH4_a8C1EpYx3PvoBXyWiiW451YbHsKi_JGtnsiuk,1479
 awc/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc/util.py,sha256=u9-_per8iyglLx9dVfQKJBdSEFZq2-5aymE7XDjoJ0o,1383
 awc/wrn.py,sha256=K84cpt9OdHQi76vhgMsWFbl8rIN_sH6EkOGptZOUWmQ,614
 awc/sql/__init__.py,sha256=y6htpvQk69bk_pVAoVXUKZkCHN8X2jzg_I9Wjf52bUY,4429
 awc/sql/helpers.py,sha256=4IiFOVP6wnrhKYb4GBaXX-SnIe7dD_JND8INkle9W0Y,2867
-awc-1.2.3.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
-awc-1.2.3.dist-info/METADATA,sha256=Q21vCJYWFdsa3TjGkJX4nPt7Nz85TNbfp6gExS18UOM,3812
-awc-1.2.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc-1.2.3.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
-awc-1.2.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc-1.2.3.dist-info/RECORD,,
+awc-1.2.4.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
+awc-1.2.4.dist-info/METADATA,sha256=jpLR34EbWCXFZuOdqIucxmazbY5rTQpHuM3k1ZoS3Rw,3812
+awc-1.2.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc-1.2.4.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
+awc-1.2.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc-1.2.4.dist-info/RECORD,,
```

