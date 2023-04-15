# Comparing `tmp/quorum_data_py-1.1.7.tar.gz` & `tmp/quorum_data_py-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.1.7.tar", last modified: Thu Apr 13 15:25:13 2023, max compression
+gzip compressed data, was "quorum_data_py-1.1.8.tar", last modified: Sat Apr 15 09:56:02 2023, max compression
```

## Comparing `quorum_data_py-1.1.7.tar` & `quorum_data_py-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 15:25:13.254452 quorum_data_py-1.1.7/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-13 15:25:13.253485 quorum_data_py-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.7/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-13 15:25:13.237881 quorum_data_py-1.1.7/quorum_data_py/
--rw-rw-rw-   0        0        0      349 2023-04-13 15:24:47.000000 quorum_data_py-1.1.7/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     6028 2023-04-13 15:24:01.000000 quorum_data_py-1.1.7/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.7/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.7/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.7/quorum_data_py/trx_type.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:25:13.251453 quorum_data_py-1.1.7/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 15:25:13.000000 quorum_data_py-1.1.7/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 15:25:13.255447 quorum_data_py-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1314 2023-04-13 15:24:47.000000 quorum_data_py-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:56:02.027665 quorum_data_py-1.1.8/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-15 09:56:02.026671 quorum_data_py-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.8/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-15 09:56:02.011890 quorum_data_py-1.1.8/quorum_data_py/
+-rw-rw-rw-   0        0        0      349 2023-04-15 09:54:43.000000 quorum_data_py-1.1.8/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     5151 2023-04-15 09:53:48.000000 quorum_data_py-1.1.8/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.8/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.8/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.8/quorum_data_py/trx_type.py
+drwxrwxrwx   0        0        0        0 2023-04-15 09:56:02.024679 quorum_data_py-1.1.8/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-15 09:56:01.000000 quorum_data_py-1.1.8/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 09:56:02.028662 quorum_data_py-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-15 09:54:43.000000 quorum_data_py-1.1.8/setup.py
```

### Comparing `quorum_data_py-1.1.7/LICENSE` & `quorum_data_py-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.7/PKG-INFO` & `quorum_data_py-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.7/README.md` & `quorum_data_py-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.7/quorum_data_py/_utils.py` & `quorum_data_py-1.1.8/quorum_data_py/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import logging
 import os
 import uuid
 import zipfile
 
 import filetype
 from PIL import Image
-from pygifsicle import gifsicle
 
 logger = logging.getLogger(__name__)
 
 
 TRX_SIZE_LIMIT = 300  # kb, 每条trx的总大小上限，超出会被限制出块
 IMAGE_NUM_LIMIT = 4  # 单条 trx 最多4 张图片；此为 rum app 限定：第三方 app 可调整该限定
 CHUNK_SIZE = 280 * 1024  # bytes, 文件切割为多条trxs时，每条 trx 所包含的文件字节流上限
@@ -72,63 +71,29 @@
     check_file(file_path)
     to_zipfile = to_zipfile or file_path + "_.zip"
     with zipfile.ZipFile(to_zipfile, mode, zipfile.ZIP_DEFLATED) as zf:
         zf.write(file_path, arcname=os.path.basename(file_path))
     return to_zipfile
 
 
-def zip_gif(gif, kb=TRX_SIZE_LIMIT, cover=False):
-    """压缩动图(gif)到指定大小(kb)以下
-
-    gif: gif 格式动图本地路径
-    kb: 指定压缩大小, 默认 200kb
-    cover: 是否覆盖原图, 默认不覆盖
-
-    返回压缩后图片字节. 该方法需要安装 gifsicle 软件和 pygifsicle 模块
-    """
-    size = os.path.getsize(gif) / 1024
-    if size < kb:
-        return read_file_to_bytes(gif)
-
-    destination = None
-    if not cover:
-        destination = f"{os.path.splitext(gif)[0]}-zip.gif"
-
-    n = 0.9
-    while size >= kb:
-        gifsicle(
-            gif,
-            destination=destination,
-            optimize=True,
-            options=["--lossy=80", "--scale", str(n)],
-        )
-        if not cover:
-            gif = destination
-        size = os.path.getsize(gif) / 1024
-        n -= 0.05
-
-    return read_file_to_bytes(gif)
-
-
-def _zip_image(img, kb=TRX_SIZE_LIMIT):
-    file_bytes, is_file = _get_filebytes(img)
+def zip_image(img_bytes, kb=TRX_SIZE_LIMIT):
+    if isinstance(img_bytes, str) and os.path.exists(img_bytes):
+        img_bytes = read_file_to_bytes(img_bytes)
+    if not isinstance(img_bytes, bytes):
+        raise TypeError("img_bytes must be bytes or file path.")
     try:
-        if filetype.guess(file_bytes).extension == "gif" and is_file:
-            img_bytes = zip_gif(img, kb=kb, cover=False)
-        else:
-            img_bytes = _zip_image_bytes(file_bytes, kb)
+        img_bytes = _zip_image_bytes(img_bytes, kb)
     except Exception as e:
         logger.warning("zip_image %s", e)
     return img_bytes
 
 
 def pack_icon(icon):
     """icon: one image as file path, or bytes, or bytes-string."""
-
-    img_bytes = _zip_image(icon)
+    img_bytes = zip_image(icon)
     icon = "".join(
         [
             "data:",
             filetype.guess(img_bytes).mime,
             ";base64,",
             base64.b64encode(img_bytes).decode("utf-8"),
         ]
@@ -170,15 +135,15 @@
     if total_size < bytes_limit:
         target_size = sizes
     else:
         target_size = [int(i * bytes_limit / total_size) for i in sizes]
 
     imgs = []
     for i, _img in enumerate(images):
-        _bytes = _zip_image(_img, target_size[i] // 1024)
+        _bytes = zip_image(_img, target_size[i] // 1024)
         imgs.append(
             {
                 "mediaType": filetype.guess(_bytes).mime,
                 "content": base64.b64encode(_bytes).decode("utf-8"),
                 "type": "Image",
             }
         )
```

### Comparing `quorum_data_py-1.1.7/quorum_data_py/converter.py` & `quorum_data_py-1.1.8/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.7/quorum_data_py/feed.py` & `quorum_data_py-1.1.8/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.7/quorum_data_py/trx_type.py` & `quorum_data_py-1.1.8/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.7/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.1.8/quorum_data_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.7/setup.py` & `quorum_data_py-1.1.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.1.7",
+    version="1.1.8",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
@@ -27,11 +27,10 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(exclude=["tests"]),
     python_requires=">=3.7",
     install_requires=[
         "pillow",
-        "pygifsicle",
         "filetype",
     ],
 )
```

