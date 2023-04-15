# Comparing `tmp/quorum_data_py-1.1.8.tar.gz` & `tmp/quorum_data_py-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.1.8.tar", last modified: Sat Apr 15 09:56:02 2023, max compression
+gzip compressed data, was "quorum_data_py-1.1.9.tar", last modified: Sat Apr 15 10:30:41 2023, max compression
```

## Comparing `quorum_data_py-1.1.8.tar` & `quorum_data_py-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 09:56:02.027665 quorum_data_py-1.1.8/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-15 09:56:02.026671 quorum_data_py-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.8/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-15 09:56:02.011890 quorum_data_py-1.1.8/quorum_data_py/
--rw-rw-rw-   0        0        0      349 2023-04-15 09:54:43.000000 quorum_data_py-1.1.8/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     5151 2023-04-15 09:53:48.000000 quorum_data_py-1.1.8/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.8/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.8/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.8/quorum_data_py/trx_type.py
-drwxrwxrwx   0        0        0        0 2023-04-15 09:56:02.024679 quorum_data_py-1.1.8/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 09:56:02.028662 quorum_data_py-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-15 09:54:43.000000 quorum_data_py-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:41.733122 quorum_data_py-1.1.9/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-15 10:30:41.702728 quorum_data_py-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.9/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:41.692767 quorum_data_py-1.1.9/quorum_data_py/
+-rw-rw-rw-   0        0        0      349 2023-04-15 10:29:48.000000 quorum_data_py-1.1.9/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.1.9/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.9/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.9/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.9/quorum_data_py/trx_type.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:30:41.700734 quorum_data_py-1.1.9/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 10:30:41.733122 quorum_data_py-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-15 10:29:48.000000 quorum_data_py-1.1.9/setup.py
```

### Comparing `quorum_data_py-1.1.8/LICENSE` & `quorum_data_py-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.8/PKG-INFO` & `quorum_data_py-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.8/README.md` & `quorum_data_py-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.8/quorum_data_py/_utils.py` & `quorum_data_py-1.1.9/quorum_data_py/_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import base64
-import datetime
 import io
 import json
 import logging
 import os
 import uuid
 import zipfile
 
@@ -14,28 +13,33 @@
 
 
 TRX_SIZE_LIMIT = 300  # kb, 每条trx的总大小上限，超出会被限制出块
 IMAGE_NUM_LIMIT = 4  # 单条 trx 最多4 张图片；此为 rum app 限定：第三方 app 可调整该限定
 CHUNK_SIZE = 280 * 1024  # bytes, 文件切割为多条trxs时，每条 trx 所包含的文件字节流上限
 
 
-def _filename_init(img):
-    file_bytes, is_file = _get_filebytes(img)
-    if is_file:
-        file_name = os.path.basename(img).encode().decode("utf-8")
-    else:
-        extension = filetype.guess(file_bytes).extension
-        name = f"{uuid.uuid4()}-{datetime.date.today()}"
-        file_name = ".".join([name, extension])
-    return file_name
+def read_file_to_bytes(file_path):
+    with open(file_path, "rb") as f:
+        bytes_data = f.read()
+    return bytes_data
 
 
-def _zip_image_bytes(img_bytes, kb=TRX_SIZE_LIMIT):
-    """zip image bytes and return bytes; default changed to .jpeg"""
+def zip_file(file_path, to_zipfile=None, mode="w"):
+    if not os.path.exists(file_path):
+        raise ValueError(f"{file_path} file is not exists.")
+    if not os.path.isfile(file_path):
+        raise ValueError(f"{file_path} is not a file.")
+    to_zipfile = to_zipfile or file_path + "_.zip"
+    with zipfile.ZipFile(to_zipfile, mode, zipfile.ZIP_DEFLATED) as zf:
+        zf.write(file_path, arcname=os.path.basename(file_path))
+    return to_zipfile
+
 
+def zip_image(img, kb=TRX_SIZE_LIMIT):
+    img_bytes = _get_filebytes(img)
     guess_extension = filetype.guess(img_bytes).extension
 
     with io.BytesIO(img_bytes) as im:
         size = len(im.getvalue()) // 1024
         if size < kb:
             return img_bytes
         while size >= kb:
@@ -49,48 +53,14 @@
             except Exception as err:
                 logger.info(err)
                 out.save(im, guess_extension)
             size = len(im.getvalue()) // 1024
         return im.getvalue()
 
 
-def check_file(file_path):
-    if not os.path.exists(file_path):
-        raise ValueError(f"{file_path} file is not exists.")
-    if not os.path.isfile(file_path):
-        raise ValueError(f"{file_path} is not a file.")
-
-
-def read_file_to_bytes(file_path):
-    check_file(file_path)
-    with open(file_path, "rb") as f:
-        bytes_data = f.read()
-    return bytes_data
-
-
-def zip_file(file_path, to_zipfile=None, mode="w"):
-    check_file(file_path)
-    to_zipfile = to_zipfile or file_path + "_.zip"
-    with zipfile.ZipFile(to_zipfile, mode, zipfile.ZIP_DEFLATED) as zf:
-        zf.write(file_path, arcname=os.path.basename(file_path))
-    return to_zipfile
-
-
-def zip_image(img_bytes, kb=TRX_SIZE_LIMIT):
-    if isinstance(img_bytes, str) and os.path.exists(img_bytes):
-        img_bytes = read_file_to_bytes(img_bytes)
-    if not isinstance(img_bytes, bytes):
-        raise TypeError("img_bytes must be bytes or file path.")
-    try:
-        img_bytes = _zip_image_bytes(img_bytes, kb)
-    except Exception as e:
-        logger.warning("zip_image %s", e)
-    return img_bytes
-
-
 def pack_icon(icon):
     """icon: one image as file path, or bytes, or bytes-string."""
     img_bytes = zip_image(icon)
     icon = "".join(
         [
             "data:",
             filetype.guess(img_bytes).mime,
@@ -98,42 +68,39 @@
             base64.b64encode(img_bytes).decode("utf-8"),
         ]
     )
     return icon
 
 
 def _get_filebytes(img):
-    _size = len(img)
-    is_file = False
     if isinstance(img, str):
         if os.path.exists(img):
             file_bytes = read_file_to_bytes(img)
-            is_file = True
         else:
             file_bytes = base64.b64decode(img)
     elif isinstance(img, bytes):
         file_bytes = img
     else:
         raise TypeError(
-            f"not support for type: {type(img)} and length: {_size}"
+            f"not support for type: {type(img)} and length: {len(img)}"
         )
-    return file_bytes, is_file
+    return file_bytes
 
 
 def pack_imgs(images: list, kb: int = TRX_SIZE_LIMIT):
     """
     打包图片为 feed 所需的数据格式。
     由于每个 trx 限定了 300kb 的大小，图片的大小需要根据已有 content 计算得出余量。
     """
     # check images size
     if len(images) == 0:
         raise ValueError("images is empty.")
     # 从图片字节转换为 base64string 大小会膨胀 1.33 左右
     bytes_limit = int(1024 * kb / 1.34)
-    sizes = [len(read_file_to_bytes(i)) for i in images]
+    sizes = [len(_get_filebytes(i)) for i in images]
     total_size = sum(sizes)
 
     if total_size < bytes_limit:
         target_size = sizes
     else:
         target_size = [int(i * bytes_limit / total_size) for i in sizes]
```

### Comparing `quorum_data_py-1.1.8/quorum_data_py/converter.py` & `quorum_data_py-1.1.9/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.8/quorum_data_py/feed.py` & `quorum_data_py-1.1.9/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.8/quorum_data_py/trx_type.py` & `quorum_data_py-1.1.9/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.8/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.1.9/quorum_data_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.8/setup.py` & `quorum_data_py-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.1.8",
+    version="1.1.9",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

