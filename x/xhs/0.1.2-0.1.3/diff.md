# Comparing `tmp/xhs-0.1.2.tar.gz` & `tmp/xhs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.2.tar", last modified: Fri Apr 14 03:41:24 2023, max compression
+gzip compressed data, was "xhs-0.1.3.tar", last modified: Sat Apr 15 14:43:28 2023, max compression
```

## Comparing `xhs-0.1.2.tar` & `xhs-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 03:41:10.000000 xhs-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 03:41:10.000000 xhs-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 03:41:10.000000 xhs-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-14 03:41:24.414005 xhs-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-14 03:41:10.000000 xhs-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 03:41:10.000000 xhs-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 03:41:24.418005 xhs-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-14 03:41:10.000000 xhs-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-15 14:43:16.000000 xhs-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 14:43:16.000000 xhs-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 14:43:16.000000 xhs-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-15 14:43:28.262915 xhs-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-15 14:43:16.000000 xhs-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 14:43:16.000000 xhs-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-15 14:43:28.262915 xhs-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-15 14:43:16.000000 xhs-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 14:43:16.000000 xhs-0.1.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19541 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-15 14:43:16.000000 xhs-0.1.3/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:43:28.262915 xhs-0.1.3/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-15 14:43:28.000000 xhs-0.1.3/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.2/CHANGELOG.md` & `xhs-0.1.3/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.1.3
+
+### ADD
+
+- add get note comments
+- add get note sub comments
+- add get note all comments
+
 ## 0.1.2
 
 ### ADD
 
 - add get user all notes
 
 ### Changed
```

### Comparing `xhs-0.1.2/LICENSE` & `xhs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.2/PKG-INFO` & `xhs-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.2
+Version: 0.1.3
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xhs-0.1.2/README.md` & `xhs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xhs-0.1.2/setup.py` & `xhs-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.2/tests/test_help.py` & `xhs-0.1.3/tests/test_help.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 
 import pytest
 import requests
 
 from xhs import help
 
+from . import test_cookie
+
 
 @pytest.fixture
 def header():
     return {
-        "cookie": ('webId=e3455f4405340fc431af976dbf3de167;'
-                   "web_session=040069b253793fdd9ccd9a5f01364b856d4088"),
+        "cookie": test_cookie,
         "user-agent": ("Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
                        "AppleWebKit/537.36 (KHTML, like Gecko)"
                        "Chrome/111.0.0.0 Safari/537.36")
     }
 
 
 def test_sign_get(header):
```

### Comparing `xhs-0.1.2/tests/test_xhs.py` & `xhs-0.1.3/tests/test_xhs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pytest
 
 from xhs import FeedType, XhsClient
 
+from . import test_cookie
 from .utils import beauty_print
 
 
 @pytest.fixture
 def xhs_client():
-    return XhsClient(
-        cookie=("webId=3ceadc9abfc351b88b07b556afddab35;"
-                "web_session=040069b253793fdd9ccd9a5f01364b856d4088;"))
+    return XhsClient(cookie=test_cookie)
+
+
+def test_xhs_client_init():
+    xhs_client = XhsClient()
+    assert xhs_client
 
 
 def test_cookie_setter_getter():
     cookie = "web_session=123"
     xhs_client = XhsClient(cookie)
     assert xhs_client.cookie == cookie
     new_cookie = "web_session=456"
@@ -60,21 +64,47 @@
 def test_get_user_notes(xhs_client: XhsClient):
     user_id = "63273a77000000002303cc9b"
     data = xhs_client.get_user_notes(user_id)
     beauty_print(data)
     assert len(data["notes"]) > 0
 
 
-@pytest.mark.skip()
+@pytest.mark.skip(reason="it take much request and time")
 def test_get_user_all_notes(xhs_client: XhsClient):
     user_id = "5c2766b500000000050283f1"
     notes = xhs_client.get_user_all_notes(user_id, 0)
     beauty_print(notes)
 
 
+def test_get_note_comments(xhs_client: XhsClient):
+    note_id = "63db8819000000001a01ead1"
+    comments = xhs_client.get_note_comments(note_id)
+    beauty_print(comments)
+    assert len(comments["comments"]) > 0
+
+
+def test_get_note_sub_comments(xhs_client: XhsClient):
+    note_id = "63db8819000000001a01ead1"
+    root_comment_id = "63db8957000000001c03e5b5"
+    comments = xhs_client.get_note_sub_comments(note_id, root_comment_id)
+    beauty_print(comments)
+    assert len(comments["comments"]) > 0
+
+
+@pytest.mark.skip(reason="it take much request and time")
+def test_get_note_all_comments(xhs_client: XhsClient):
+    note_id = "63db8819000000001a01ead1"
+    note = xhs_client.get_note_by_id(note_id)
+    comments_count = int(note["interact_info"]["comment_count"])
+    print(comments_count)
+    comments = xhs_client.get_note_all_comments(note_id)
+    beauty_print(comments)
+    assert len(comments) == comments_count
+
+
 def test_get_qrcode(xhs_client: XhsClient):
     data = xhs_client.get_qrcode()
     beauty_print(data)
     assert data["url"].startswith("xhsdiscover://")
 
 
 @pytest.mark.skip()
```

### Comparing `xhs-0.1.2/xhs/help.py` & `xhs-0.1.3/xhs/help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.2/xhs.egg-info/PKG-INFO` & `xhs-0.1.3/xhs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.2
+Version: 0.1.3
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

