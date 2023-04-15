# Comparing `tmp/aioqzone-0.9.9.dev2.tar.gz` & `tmp/aioqzone-0.9.9.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqzone-0.9.9.dev2.tar", max compression
+gzip compressed data, was "aioqzone-0.9.9.dev3.tar", max compression
```

## Comparing `aioqzone-0.9.9.dev2.tar` & `aioqzone-0.9.9.dev3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    34523 2022-10-27 01:57:31.850216 aioqzone-0.9.9.dev2/LICENSE
--rw-r--r--   0        0        0     2932 2022-10-27 01:57:31.850216 aioqzone-0.9.9.dev2/README.md
--rw-r--r--   0        0        0     2208 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/__init__.py
--rw-r--r--   0        0        0     2776 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/api/__init__.py
--rw-r--r--   0        0        0     1028 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/api/constant.py
--rw-r--r--   0        0        0    10992 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/api/loginman.py
--rw-r--r--   0        0        0    24105 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/api/raw.py
--rw-r--r--   0        0        0       32 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/event/__init__.py
--rw-r--r--   0        0        0     2580 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/event/login.py
--rw-r--r--   0        0        0     1068 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/exception.py
--rw-r--r--   0        0        0        0 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/py.typed
--rw-r--r--   0        0        0      187 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/type/__init__.py
--rw-r--r--   0        0        0     1056 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/type/entity.py
--rw-r--r--   0        0        0     1451 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/type/internal.py
--rw-r--r--   0        0        0     5949 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/type/resp.py
--rw-r--r--   0        0        0       39 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/utils/__init__.py
--rw-r--r--   0        0        0     3859 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/utils/html.py
--rw-r--r--   0        0        0      297 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/utils/regex.py
--rw-r--r--   0        0        0     2623 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/aioqzone/utils/time.py
--rw-r--r--   0        0        0      133 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/jssupport/__init__.py
--rw-r--r--   0        0        0      625 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/jssupport/exception.py
--rw-r--r--   0        0        0     5878 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/jssupport/execjs.py
--rw-r--r--   0        0        0     2187 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/jssupport/jsdom.py
--rw-r--r--   0        0        0     3328 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/jssupport/jsjson.py
--rw-r--r--   0        0        0        0 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/jssupport/py.typed
--rw-r--r--   0        0        0      146 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/__init__.py
--rw-r--r--   0        0        0     3159 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/base.py
--rw-r--r--   0        0        0      816 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/constant.py
--rw-r--r--   0        0        0     5835 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/event/__init__.py
--rw-r--r--   0        0        0     1007 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/event/login.py
--rw-r--r--   0        0        0     1053 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/exception.py
--rw-r--r--   0        0        0        8 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/py.typed
--rw-r--r--   0        0        0     3917 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/qr/__init__.py
--rw-r--r--   0        0        0      198 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/qr/type.py
--rw-r--r--   0        0        0      583 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/ssl.py
--rw-r--r--   0        0        0      382 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/type.py
--rw-r--r--   0        0        0     8974 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/__init__.py
--rw-r--r--   0        0        0     8714 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/captcha/__init__.py
--rw-r--r--   0        0        0     5097 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/blob.js
--rw-r--r--   0        0        0     6773 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/decrypt.js
--rw-r--r--   0        0        0     5038 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/vdata.js
--rw-r--r--   0        0        0      541 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/window.tdc.js
--rw-r--r--   0        0        0     7327 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/captcha/jigsaw.py
--rw-r--r--   0        0        0     2529 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/captcha/vm.py
--rw-r--r--   0        0        0     6699 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/encrypt.py
--rw-r--r--   0        0        0    19455 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/rsa.py
--rw-r--r--   0        0        0     2674 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/up/type.py
--rw-r--r--   0        0        0      628 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/utils/daug.py
--rw-r--r--   0        0        0      204 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/utils/encrypt.py
--rw-r--r--   0        0        0      594 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/utils/iter.py
--rw-r--r--   0        0        0     2470 2022-10-27 01:57:31.854216 aioqzone-0.9.9.dev2/src/qqqr/utils/net.py
--rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 aioqzone-0.9.9.dev2/setup.py
--rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 aioqzone-0.9.9.dev2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-10-29 00:43:22.176285 aioqzone-0.9.9.dev3/LICENSE
+-rw-r--r--   0        0        0     2932 2022-10-29 00:43:22.176285 aioqzone-0.9.9.dev3/README.md
+-rw-r--r--   0        0        0     2208 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/__init__.py
+-rw-r--r--   0        0        0     2776 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/api/__init__.py
+-rw-r--r--   0        0        0     1028 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/api/constant.py
+-rw-r--r--   0        0        0    10992 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/api/loginman.py
+-rw-r--r--   0        0        0    23997 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/api/raw.py
+-rw-r--r--   0        0        0       32 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/event/__init__.py
+-rw-r--r--   0        0        0     2580 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/event/login.py
+-rw-r--r--   0        0        0     1068 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/exception.py
+-rw-r--r--   0        0        0        0 2022-10-29 00:43:22.180285 aioqzone-0.9.9.dev3/src/aioqzone/py.typed
+-rw-r--r--   0        0        0      187 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/type/__init__.py
+-rw-r--r--   0        0        0     1056 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/type/entity.py
+-rw-r--r--   0        0        0     1451 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/type/internal.py
+-rw-r--r--   0        0        0     5949 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/type/resp.py
+-rw-r--r--   0        0        0       39 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/utils/__init__.py
+-rw-r--r--   0        0        0     3859 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/utils/html.py
+-rw-r--r--   0        0        0      297 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/utils/regex.py
+-rw-r--r--   0        0        0     2623 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/aioqzone/utils/time.py
+-rw-r--r--   0        0        0      133 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/jssupport/__init__.py
+-rw-r--r--   0        0        0      625 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/jssupport/exception.py
+-rw-r--r--   0        0        0     5878 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/jssupport/execjs.py
+-rw-r--r--   0        0        0     2187 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/jssupport/jsdom.py
+-rw-r--r--   0        0        0     3328 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/jssupport/jsjson.py
+-rw-r--r--   0        0        0        0 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/jssupport/py.typed
+-rw-r--r--   0        0        0      146 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/__init__.py
+-rw-r--r--   0        0        0     3159 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/base.py
+-rw-r--r--   0        0        0      816 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/constant.py
+-rw-r--r--   0        0        0     5835 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/event/__init__.py
+-rw-r--r--   0        0        0     1007 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/event/login.py
+-rw-r--r--   0        0        0     1053 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/exception.py
+-rw-r--r--   0        0        0        8 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/py.typed
+-rw-r--r--   0        0        0     3917 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/qr/__init__.py
+-rw-r--r--   0        0        0      198 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/qr/type.py
+-rw-r--r--   0        0        0      583 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/ssl.py
+-rw-r--r--   0        0        0      382 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/type.py
+-rw-r--r--   0        0        0     8974 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/__init__.py
+-rw-r--r--   0        0        0     8643 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/captcha/__init__.py
+-rw-r--r--   0        0        0     5097 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/blob.js
+-rw-r--r--   0        0        0     6773 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/decrypt.js
+-rw-r--r--   0        0        0     5038 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/vdata.js
+-rw-r--r--   0        0        0      541 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/window.tdc.js
+-rw-r--r--   0        0        0     7327 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/captcha/jigsaw.py
+-rw-r--r--   0        0        0     2529 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/captcha/vm.py
+-rw-r--r--   0        0        0     6663 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/encrypt.py
+-rw-r--r--   0        0        0    19455 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/rsa.py
+-rw-r--r--   0        0        0     2674 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/up/type.py
+-rw-r--r--   0        0        0      628 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/utils/daug.py
+-rw-r--r--   0        0        0      204 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/utils/encrypt.py
+-rw-r--r--   0        0        0      594 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/utils/iter.py
+-rw-r--r--   0        0        0     2470 2022-10-29 00:43:22.184285 aioqzone-0.9.9.dev3/src/qqqr/utils/net.py
+-rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 aioqzone-0.9.9.dev3/setup.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 aioqzone-0.9.9.dev3/PKG-INFO
```

### Comparing `aioqzone-0.9.9.dev2/LICENSE` & `aioqzone-0.9.9.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/README.md` & `aioqzone-0.9.9.dev3/README.md`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/pyproject.toml` & `aioqzone-0.9.9.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioqzone"
-version = "0.9.9.dev2"
+version = "0.9.9.dev3"
 description = "Python wrapper for Qzone web login and Qzone http api."
 authors = ["aioqzone <zzzzss990315@gmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/aioqzone/aioqzone"
 repository = "https://github.com/aioqzone/aioqzone"
 documentation = "https://aioqzone.github.io/aioqzone"
```

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/api/__init__.py` & `aioqzone-0.9.9.dev3/src/aioqzone/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/api/constant.py` & `aioqzone-0.9.9.dev3/src/aioqzone/api/constant.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/api/loginman.py` & `aioqzone-0.9.9.dev3/src/aioqzone/api/loginman.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/api/raw.py` & `aioqzone-0.9.9.dev3/src/aioqzone/api/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
             "externparam": external,
         }
 
         @self._relogin_retry
         async def retry_closure():
             async with await self.aget(const.feeds3_html_more, du(default, query)) as r:
                 r.raise_for_status()
-                rtext = "".join([i async for i in r.aiter_text()])
+                rtext = r.text
 
             return self._rtext_handler(rtext)
 
         r = await retry_closure()
         data = r["data"]
         assert isinstance(data, dict)
 
@@ -271,15 +271,15 @@
             "feedsType": feedstype,
         }
 
         @self._relogin_retry
         async def retry_closure():
             async with await self.apost(const.emotion_getcomments, data=du(default, body)) as r:
                 r.raise_for_status()
-                rtext = "".join([i async for i in r.aiter_text()])
+                rtext = r.text
 
             return self._rtext_handler(rtext)
 
         return await retry_closure()
 
     async def emotion_msgdetail(self, owner: int, fid: str) -> StrDict:
         """Get detail of a given msg.
@@ -501,15 +501,15 @@
 
         @self._relogin_retry
         async def retry_closure():
             async with await self.aget(
                 const.emotion_msglist, du(param, add) if pos else param
             ) as r:
                 r.raise_for_status()
-                rtext = "".join([i async for i in r.aiter_text()])
+                rtext = r.text
             return self._rtext_handler(rtext)
 
         data = await retry_closure()
         return data["msglist"]  # type: ignore
 
     async def emotion_publish(self, content: str, right: int = 0) -> StrDict:
         """Publish a feed. appid=311.
```

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/event/login.py` & `aioqzone-0.9.9.dev3/src/aioqzone/event/login.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/exception.py` & `aioqzone-0.9.9.dev3/src/aioqzone/exception.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/type/entity.py` & `aioqzone-0.9.9.dev3/src/aioqzone/type/entity.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/type/internal.py` & `aioqzone-0.9.9.dev3/src/aioqzone/type/internal.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/type/resp.py` & `aioqzone-0.9.9.dev3/src/aioqzone/type/resp.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/utils/html.py` & `aioqzone-0.9.9.dev3/src/aioqzone/utils/html.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/aioqzone/utils/time.py` & `aioqzone-0.9.9.dev3/src/aioqzone/utils/time.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/jssupport/exception.py` & `aioqzone-0.9.9.dev3/src/jssupport/exception.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/jssupport/execjs.py` & `aioqzone-0.9.9.dev3/src/jssupport/execjs.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/jssupport/jsdom.py` & `aioqzone-0.9.9.dev3/src/jssupport/jsdom.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/jssupport/jsjson.py` & `aioqzone-0.9.9.dev3/src/jssupport/jsjson.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/base.py` & `aioqzone-0.9.9.dev3/src/qqqr/base.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/constant.py` & `aioqzone-0.9.9.dev3/src/qqqr/constant.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/event/__init__.py` & `aioqzone-0.9.9.dev3/src/qqqr/event/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/event/login.py` & `aioqzone-0.9.9.dev3/src/qqqr/event/login.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/exception.py` & `aioqzone-0.9.9.dev3/src/qqqr/exception.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/qr/__init__.py` & `aioqzone-0.9.9.dev3/src/qqqr/qr/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/ssl.py` & `aioqzone-0.9.9.dev3/src/qqqr/ssl.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/__init__.py` & `aioqzone-0.9.9.dev3/src/qqqr/up/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/captcha/__init__.py` & `aioqzone-0.9.9.dev3/src/qqqr/up/captcha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         """
 
         js_url = sess.tdx_js_url()
         tdc = cls("", header=self.client.headers)
 
         async with await self.client.get(js_url) as r:
             r.raise_for_status()
-            tdc.load_vm("".join([i async for i in r.aiter_text()]))
+            tdc.load_vm(r.text)
 
         sess.set_js_env(tdc)
 
     async def get_captcha_problem(self, sess: TcaptchaSession):
         """
         The get_captcha_problem function is a coroutine that accepts a TcaptchaSession object as an argument.
         It then uses the session to make an HTTP GET request to the captcha images (the problem). The images
@@ -195,15 +195,15 @@
         :param sess: captcha session
         :return: None
         """
 
         async def r(url):
             async with await self.client.get(url) as r:
                 r.raise_for_status()
-                return b"".join([i async for i in r.aiter_bytes()])
+                return r.content
 
         for i in await asyncio.gather(*(r(i) for i in sess.cdn_urls)):
             sess.cdn_imgs.append(i)
 
     async def solve_captcha(self, sess: TcaptchaSession):
         """
         The solve_captcha function solves the captcha problem. If captcha images is not set,
```

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/blob.js` & `aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/blob.js`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/decrypt.js` & `aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/decrypt.js`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/vdata.js` & `aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/vdata.js`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/captcha/archive/window.tdc.js` & `aioqzone-0.9.9.dev3/src/qqqr/up/captcha/archive/window.tdc.js`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/captcha/jigsaw.py` & `aioqzone-0.9.9.dev3/src/qqqr/up/captcha/jigsaw.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/captcha/vm.py` & `aioqzone-0.9.9.dev3/src/qqqr/up/captcha/vm.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/encrypt.py` & `aioqzone-0.9.9.dev3/src/qqqr/up/encrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     async def encode(self, salt: str, verifycode: str) -> str:
         assert self._passwd, "password should not be empty"
         return await self.getEncryption(salt, verifycode)
 
     async def login_js(self):
         async with await self.client.get(LOGIN_JS) as r:
             r.raise_for_status()
-            return "".join([i async for i in r.aiter_text()])
+            return r.text
 
     @abstractmethod
     async def getEncryption(self, salt: str, verifycode: str) -> str:
         pass
 
 
 class NodeEncoder(PasswdEncoder):
```

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/rsa.py` & `aioqzone-0.9.9.dev3/src/qqqr/up/rsa.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/up/type.py` & `aioqzone-0.9.9.dev3/src/qqqr/up/type.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/utils/daug.py` & `aioqzone-0.9.9.dev3/src/qqqr/utils/daug.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/utils/iter.py` & `aioqzone-0.9.9.dev3/src/qqqr/utils/iter.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/src/qqqr/utils/net.py` & `aioqzone-0.9.9.dev3/src/qqqr/utils/net.py`

 * *Files identical despite different names*

### Comparing `aioqzone-0.9.9.dev2/setup.py` & `aioqzone-0.9.9.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 extras_require = \
 {':python_version >= "3.7" and python_version < "3.8"': ['numpy>=1.21.6,<1.22.0'],
  ':python_version >= "3.8" and python_version < "4.0"': ['numpy>=1.22.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'aioqzone',
-    'version': '0.9.9.dev2',
+    'version': '0.9.9.dev3',
     'description': 'Python wrapper for Qzone web login and Qzone http api.',
     'long_description': '# aioqzone\n\naioqzone封装了一些Qzone接口。\n\n[![python](https://img.shields.io/pypi/pyversions/aioqzone?logo=python&logoColor=white)][home]\n[![QQQR](https://github.com/aioqzone/aioqzone/actions/workflows/qqqr.yml/badge.svg?branch=beta&event=schedule)](https://github.com/aioqzone/aioqzone/actions/workflows/qqqr.yml)\n[![version](https://img.shields.io/pypi/v/aioqzone?logo=python)][pypi]\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n[English](README_en.md)\n\n## 功能和特点\n\n### Qzone 功能\n\n- [x] 二维码登录\n- [x] 密码登录 (受限)\n- [x] 计算验证码答案\n- [ ] 通过网络环境检测\n- [x] 爬取HTML说说\n- [x] 爬取说说详细内容\n- [x] 爬取空间相册\n- [x] 点赞/取消赞\n- [x] 发布/修改/删除说说\n- [ ] 评论相关\n\n### 为什么选择 aioqzone\n\n- [x] 完整的 IDE 类型支持 (typing)\n- [x] API 结果类型验证 (pydantic)\n- [x] 异步设计\n- [x] 易于二次开发\n- [x] [文档支持](https://aioqzone.github.io/aioqzone)\n\n__在做了:__\n\n- [ ] 完善的测试覆盖\n\n## node 依赖\n\n- `jssupport.jsjson.AstLoader` 不需要借助其他进程；\n- 要使用 `jssupport.execjs` 和 `jssupport.jsjson.NodeLoader`，您（至少）需要安装 `Node.js` >= v14；\n- 要使用 `jssupport.jsdom`，您需要安装 `jsdom` 和 `canvas` 两个 npm 包。\n- 验证码部分需要使用 `canvas`，因此您需要正确配置运行环境内的 font config ([#45](https://github.com/aioqzone/aioqzone/issues/45)).\n\n## 包描述\n\n|包名    |简述  |\n|-----------|-------------------|\n|aioqzone   |封装Qzone API  |\n|jssupport  |执行JS            |\n|qqqr       |网页登录    |\n\n## 例子\n\n这些仓库提供了一些 aioqzone 的实际使用示例。\n\n### aioqzone 的插件们\n\n- [aioqzone-feed][aioqzone-feed]: 提供了操作 feed 的简单接口\n\n## 许可证\n\n```\nCopyright (C) 2022 aioqzone.\n\nThis program is free software: you can redistribute it and/or modify\nit under the terms of the GNU Affero General Public License as published\nby the Free Software Foundation, either version 3 of the License, or\n(at your option) any later version.\n\nThis program is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\nGNU Affero General Public License for more details.\n\nYou should have received a copy of the GNU Affero General Public License\nalong with this program.  If not, see <https://www.gnu.org/licenses/>.\n```\n\n- aioqzone 以 [AGPL-3.0](LICENSE) 开源.\n- [免责声明](https://aioqzone.github.io/aioqzone/disclaimers.html)\n\n\n[home]: https://github.com/aioqzone/aioqzone "Python wrapper for Qzone web login and Qzone http api"\n[aioqzone-feed]: https://github.com/aioqzone/aioqzone-feed "aioqzone plugin providing higher level api for processing feed"\n[pypi]: https://pypi.org/project/aioqzone\n',
     'author': 'aioqzone',
     'author_email': 'zzzzss990315@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aioqzone/aioqzone',
```

### Comparing `aioqzone-0.9.9.dev2/PKG-INFO` & `aioqzone-0.9.9.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqzone
-Version: 0.9.9.dev2
+Version: 0.9.9.dev3
 Summary: Python wrapper for Qzone web login and Qzone http api.
 Home-page: https://github.com/aioqzone/aioqzone
 License: AGPL-3.0
 Keywords: qzone-api,autologin,asyncio-spider
 Author: aioqzone
 Author-email: zzzzss990315@gmail.com
 Requires-Python: >=3.7,<4.0
```

