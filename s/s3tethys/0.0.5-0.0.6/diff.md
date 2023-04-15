# Comparing `tmp/s3tethys-0.0.5.tar.gz` & `tmp/s3tethys-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3tethys-0.0.5.tar", last modified: Mon Nov  7 20:33:24 2022, max compression
+gzip compressed data, was "s3tethys-0.0.6.tar", last modified: Sat Apr 15 00:15:06 2023, max compression
```

## Comparing `s3tethys-0.0.5.tar` & `s3tethys-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-07 20:33:24.357874 s3tethys-0.0.5/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-11-04 04:20:46.000000 s3tethys-0.0.5/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      579 2022-11-07 20:33:24.357874 s3tethys-0.0.5/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      131 2022-11-04 04:20:46.000000 s3tethys-0.0.5/README.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2022-11-04 04:20:46.000000 s3tethys-0.0.5/pyproject.toml
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-07 20:33:24.357874 s3tethys-0.0.5/s3tethys/
--rw-rw-r--   0 mike      (1000) mike      (1000)      379 2022-11-04 04:20:46.000000 s3tethys-0.0.5/s3tethys/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-07 20:33:24.357874 s3tethys-0.0.5/s3tethys/datasets/
--rw-rw-r--   0 mike      (1000) mike      (1000)      906 2022-11-04 04:20:46.000000 s3tethys-0.0.5/s3tethys/datasets/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    21595 2022-11-07 18:52:52.000000 s3tethys-0.0.5/s3tethys/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-07 20:33:24.357874 s3tethys-0.0.5/s3tethys/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2022-11-04 04:20:46.000000 s3tethys-0.0.5/s3tethys/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1250 2022-11-04 04:20:46.000000 s3tethys-0.0.5/s3tethys/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-11-07 20:33:24.357874 s3tethys-0.0.5/s3tethys.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      579 2022-11-07 20:33:24.000000 s3tethys-0.0.5/s3tethys.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      324 2022-11-07 20:33:24.000000 s3tethys-0.0.5/s3tethys.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2022-11-07 20:33:24.000000 s3tethys-0.0.5/s3tethys.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       70 2022-11-07 20:33:24.000000 s3tethys-0.0.5/s3tethys.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        9 2022-11-07 20:33:24.000000 s3tethys-0.0.5/s3tethys.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2022-11-07 20:33:24.357874 s3tethys-0.0.5/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7261 2022-11-07 20:32:48.000000 s3tethys-0.0.5/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:15:06.868383 s3tethys-0.0.6/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-11-04 04:20:46.000000 s3tethys-0.0.6/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      579 2023-04-15 00:15:06.868383 s3tethys-0.0.6/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      131 2022-11-04 04:20:46.000000 s3tethys-0.0.6/README.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2022-11-04 04:20:46.000000 s3tethys-0.0.6/pyproject.toml
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:15:06.864383 s3tethys-0.0.6/s3tethys/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      379 2022-11-04 04:20:46.000000 s3tethys-0.0.6/s3tethys/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:15:06.868383 s3tethys-0.0.6/s3tethys/datasets/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      906 2022-11-04 04:20:46.000000 s3tethys-0.0.6/s3tethys/datasets/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    23325 2023-04-14 23:56:13.000000 s3tethys-0.0.6/s3tethys/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:15:06.868383 s3tethys-0.0.6/s3tethys/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2022-11-04 04:20:46.000000 s3tethys-0.0.6/s3tethys/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1433 2023-04-14 23:27:57.000000 s3tethys-0.0.6/s3tethys/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-04-15 00:15:06.868383 s3tethys-0.0.6/s3tethys.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      579 2023-04-15 00:15:06.000000 s3tethys-0.0.6/s3tethys.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      324 2023-04-15 00:15:06.000000 s3tethys-0.0.6/s3tethys.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-04-15 00:15:06.000000 s3tethys-0.0.6/s3tethys.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       43 2023-04-15 00:15:06.000000 s3tethys-0.0.6/s3tethys.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        9 2023-04-15 00:15:06.000000 s3tethys-0.0.6/s3tethys.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-04-15 00:15:06.868383 s3tethys-0.0.6/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7230 2023-04-15 00:01:29.000000 s3tethys-0.0.6/setup.py
```

### Comparing `s3tethys-0.0.5/LICENSE` & `s3tethys-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `s3tethys-0.0.5/PKG-INFO` & `s3tethys-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3tethys
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python S3 tools for tethys using smart_open
 Home-page: https://github.com/tethys-ts/s3tethys
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3tethys-0.0.5/s3tethys/datasets/__init__.py` & `s3tethys-0.0.6/s3tethys/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `s3tethys-0.0.5/s3tethys/main.py` & `s3tethys-0.0.6/s3tethys/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import pandas as pd
 import zstandard as zstd
 import copy
 import boto3
 import botocore
 from time import sleep
 from typing import Optional, List, Any, Union
-import tethys_data_models as tdm
 import pathlib
 from pydantic import HttpUrl
 import shutil
 import gzip
 # import tethys_smart_open as smart_open
 import smart_open
 import smart_open.http as so_http
@@ -39,51 +38,57 @@
 s3_url_base = 's3://{bucket}/{key}'
 
 ##################################################
 ### Functions
 
 
 
-def s3_client(connection_config: dict, max_pool_connections: int = 30, max_attempts: int = 3):
+def s3_client(connection_config: dict, max_pool_connections: int = 30, max_attempts: int = 3, retry_mode: str='adaptive', read_timeout: int=120):
     """
-    Function to establish a client connection with an S3 account. This can use the legacy connect (signature_version s3) and the curent version.
+    Function to establish a client connection with an S3 account. This can use the legacy connect (signature_version s3) and the current version.
 
     Parameters
     ----------
     connection_config : dict
-        A dictionary of the connection info necessary to establish an S3 connection. It should contain service_name, endpoint_url, aws_access_key_id, and aws_secret_access_key. connection_config can also be a URL to a public S3 bucket.
+        A dictionary of the connection info necessary to establish an S3 connection. It should contain service_name, endpoint_url, aws_access_key_id, and aws_secret_access_key.
     max_pool_connections : int
         The number of simultaneous connections for the S3 connection.
+    max_attempts: int
+        The number of max attempts passed to the "retries" option in the S3 config.
+    retry_mode: str
+        The retry mode passed to the "retries" option in the S3 config.
+    read_timeout: int
+        The read timeout in seconds passed to the "retries" option in the S3 config.
 
     Returns
     -------
     S3 client object
     """
     ## Validate config
-    _ = tdm.base.ConnectionConfig(**connection_config)
+    _ = utils.ConnectionConfig(**connection_config)
 
     s3_config = copy.deepcopy(connection_config)
 
     if 'config' in s3_config:
         config0 = s3_config.pop('config')
-        config0.update({'max_pool_connections': max_pool_connections, 'retries': {'mode': 'adaptive', 'max_attempts': max_attempts}, 'read_timeout': 120})
+        config0.update({'max_pool_connections': max_pool_connections, 'retries': {'mode': retry_mode, 'max_attempts': max_attempts}, 'read_timeout': read_timeout})
         config1 = boto3.session.Config(**config0)
 
         s3_config1 = s3_config.copy()
         s3_config1.update({'config': config1})
 
         s3 = boto3.client(**s3_config1)
     else:
-        s3_config.update({'config': botocore.config.Config(max_pool_connections=max_pool_connections, retries={'mode': 'adaptive', 'max_attempts': max_attempts}, read_timeout=120)})
+        s3_config.update({'config': botocore.config.Config(max_pool_connections=max_pool_connections, retries={'mode': retry_mode, 'max_attempts': max_attempts}, read_timeout=read_timeout)})
         s3 = boto3.client(**s3_config)
 
     return s3
 
 
-def get_object_s3(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, connection_config: dict = None, public_url: HttpUrl=None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, retries=3):
+def get_object_s3(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, connection_config: dict = None, public_url: HttpUrl=None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, retries: int=3, read_timeout: int=120):
     """
     General function to get an object from an S3 bucket. One of s3, connection_config, or public_url must be used.
 
     Parameters
     ----------
     obj_key : str
         The object key in the S3 bucket.
@@ -99,14 +104,18 @@
         The S3 version id associated with the object.
     range_start: int
         The byte range start for the file.
     range_end: int
         The byte range end for the file.
     chunk_size: int
         The amount of bytes to download as once.
+    retries: int
+        The number of url request retries to perform before failing. This shouldn't be necessary given the max_attempts parameter in the s3_client function...but I'll keep it around until it's clearly not needed.
+    read_timeout: int
+        The read timeout for the url request. This only applies if the public_url is set which consequently uses the url_to_stream function. The read_timeout for normal S3 requests are set in the s3_client function.
 
     Returns
     -------
     file object
         file object of the S3 object.
     """
     transport_params = {'buffer_size': chunk_size}
@@ -131,40 +140,22 @@
     else:
         range1 = None
 
     ## Get the object
     if isinstance(public_url, str) and (version_id is None):
         url = utils.create_public_s3_url(public_url, bucket, obj_key)
 
-        transport_params['timeout'] = 120
-
-        if range1 is not None:
-            transport_params['headers'] = {'Range': range1}
-
-        counter = retries
-        while True:
-            try:
-                file_obj = smart_open.open(url, 'rb', transport_params=transport_params, compression='disable')
-                break
-            except Exception as err:
-                counter = counter - 1
-                if counter > 0:
-                    sleep(3)
-                else:
-                    print('smart_open could not open url with the following error:')
-                    print(err)
-                    file_obj = None
-                    break
+        file_obj = url_to_stream(url, range_start, range_end, chunk_size, retries, read_timeout)
 
     elif isinstance(s3, botocore.client.BaseClient) or isinstance(connection_config, dict):
         if range1 is not None:
             transport_params.update({'client_kwargs': {'S3.Client.get_object': {'Range': range1}}})
 
         if s3 is None:
-            _ = tdm.base.ConnectionConfig(**connection_config)
+            _ = utils.ConnectionConfig(**connection_config)
 
             s3 = s3_client(connection_config)
 
         s3_url = s3_url_base.format(bucket=bucket, key=obj_key)
         transport_params['client'] = s3
 
         try:
@@ -176,35 +167,39 @@
 
     else:
         raise TypeError('One of s3, connection_config, or public_url needs to be correctly defined.')
 
     return file_obj
 
 
-def url_to_stream(url: HttpUrl, range_start: int=None, range_end: int=None, chunk_size: int=524288, retries=3):
+def url_to_stream(url: HttpUrl, range_start: int=None, range_end: int=None, chunk_size: int=524288, retries: int=3, read_timeout: int=120):
     """
-    General function to get an object from an S3 bucket. One of s3, connection_config, or public_url must be used.
+    Function to create a file object from a file stored via http(s).
 
     Parameters
     ----------
     url: http str
         The http url to the file.
     range_start: int
         The byte range start for the file.
     range_end: int
         The byte range end for the file.
     chunk_size: int
         The amount of bytes to download as once.
+    retries: int
+        The number of url request retries to perform before failing.
+    read_timeout: int
+        The read timeout for the url request.
 
     Returns
     -------
     file object
         file object of the S3 object.
     """
-    transport_params = {'buffer_size': chunk_size, 'timeout': 120}
+    transport_params = {'buffer_size': chunk_size, 'timeout': read_timeout}
 
     # Range
     if (range_start is not None) or (range_end is not None):
         range_dict = {}
         if range_start is not None:
             range_dict['start'] = str(range_start)
         else:
@@ -235,17 +230,17 @@
                 print(err)
                 file_obj = None
                 break
 
     return file_obj
 
 
-def stream_to_file(file_obj: io.BufferedIOBase, file_path: AnyPath, chunk_size=524288):
+def stream_to_file(file_obj: io.BufferedIOBase, file_path: AnyPath, chunk_size: int=524288):
     """
-    Convert a file object (stream) to a file on disk. no decompression will occur.
+    Convert a file object (stream) to a local file on disk. No decompression will occur.
 
     Parameters
     ----------
     file_obj : io.BytesIO or io.BufferedIOBase
         The file object to be saved to file.
     file_path: str or pathlib.Path
         The output file path. If you want the function to do decompression, make sure to include the appropriate compression extension.
@@ -262,31 +257,30 @@
     with open(file_path1, 'wb') as f:
         chunk = file_obj.read(chunk_size)
         while chunk:
             f.write(chunk)
             chunk = file_obj.read(chunk_size)
 
 
-def decompress_stream_to_file(file_obj: io.BufferedIOBase, file_path: AnyPath, chunk_size=524288):
+def decompress_stream_to_file(file_obj: io.BufferedIOBase, file_path: AnyPath, chunk_size: int=524288):
     """
-    Decompress a file object (stream) to a file on disk. Decompression will occur if the file_path has an extension of .zst or .gz, otherwise no decompression will occur. If decompression occurs, then the extension will be removed from the file_path.
+    Decompress a file object (stream) to a local file on disk. Decompression will occur if the file_path has an extension of .zst or .gz, otherwise no decompression will occur. If decompression occurs, then the extension will be removed from the file_path.
 
     Parameters
     ----------
     file_obj : io.BytesIO or io.BufferedIOBase
         The file object to be saved to file.
     file_path: str or pathlib.Path
         The output file path. If you want the function to do decompression, make sure to include the appropriate compression extension.
     chunk_size: int
         The amount of bytes to use in memory for processing the object.
 
     Returns
     -------
     str path
-
     """
     file_path1 = pathlib.Path(file_path)
     file_path1.parent.mkdir(parents=True, exist_ok=True)
 
     if file_path1.suffix == '.zst':
         file_path2 = file_path1.parent.joinpath(file_path1.stem)
         dctx = zstd.ZstdDecompressor()
@@ -303,15 +297,15 @@
     else:
         file_path2 = file_path1
         stream_to_file(file_obj, file_path2, chunk_size)
 
     return str(file_path2)
 
 
-def decompress_stream_to_object(file_obj: io.BufferedIOBase, compression=None, chunk_size=524288):
+def decompress_stream_to_object(file_obj: io.BufferedIOBase, compression: str=None, chunk_size: int=524288):
     """
     Decompress a file object (stream) to another file object. Decompression will occur only for compression options of zstd or gzip, otherwise no decompression will occur.
 
     Parameters
     ----------
     file_obj : io.BytesIO or io.BufferedIOBase
         The file object to be saved to file.
@@ -319,15 +313,14 @@
         The compression types. Options are zstd and gzip.
     chunk_size: int
         The amount of bytes to use in memory for processing the object.
 
     Returns
     -------
     file object
-
     """
     b1 = io.BytesIO()
 
     if compression.lower() == 'zstd':
         dctx = zstd.ZstdDecompressor()
 
         dctx.copy_stream(file_obj, b1, read_size=chunk_size, write_size=chunk_size)
@@ -345,15 +338,15 @@
                 chunk = file_obj.read(chunk_size)
 
     b1.seek(0)
 
     return b1
 
 
-def put_object_s3(s3: botocore.client.BaseClient, bucket: str, obj_key: str, file_obj: io.BufferedIOBase, metadata: dict=None, content_type: str=None, chunk_size=524288, retries=3):
+def put_object_s3(s3: botocore.client.BaseClient, bucket: str, obj_key: str, file_obj: io.BufferedIOBase, metadata: dict=None, content_type: str=None, chunk_size: int=524288, retries: int=3):
     """
     Function to upload data to an S3 bucket.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
@@ -363,14 +356,18 @@
         The key name for the uploaded object.
     file_obj : io.BytesIO or io.BufferedIOBase
         The file object to be uploaded.
     metadata : dict or None
         A dict of the metadata that should be saved along with the object.
     content_type : str
         The http content type to associate the object with.
+    chunk_size: int
+        The amount of bytes to use in memory for processing the object.
+    retries: int
+        The number of url request retries to perform before failing. This shouldn't be necessary given the max_attempts parameter in the s3_client function...but I'll keep it around until it's clearly not needed.
 
     Returns
     -------
     None
     """
     max_size = 1024*1024*5
     s3_url = s3_url_base.format(bucket=bucket, key=obj_key)
@@ -396,16 +393,14 @@
     while True:
         try:
             with smart_open.open(s3_url, 'wb', transport_params=transport_params, compression='disable') as f:
                 chunk = file_obj.read(chunk_size)
                 while chunk:
                     f.write(chunk)
                     chunk = file_obj.read(chunk_size)
-
-            # obj2 = s3.put_object(Bucket=bucket, Key=key, Body=obj, Metadata=metadata, ContentType=content_type)
             break
         except bc_exceptions.ConnectionClosedError as err:
             print(err)
             counter = counter - 1
             if counter == 0:
                 raise err
             print('...trying again...')
@@ -415,17 +410,17 @@
         #     counter = counter - 1
         #     if counter == 0:
         #         raise err
         #     print('...trying again...')
         #     sleep(3)
 
 
-def put_file_s3(s3: botocore.client.BaseClient, bucket: str, obj_key: str, file_path: AnyPath, metadata: dict=None, content_type: str=None, retries=3):
+def put_file_s3(s3: botocore.client.BaseClient, bucket: str, obj_key: str, file_path: AnyPath, metadata: dict=None, content_type: str=None, retries: int=3):
     """
-    Function to upload data to an S3 bucket.
+    Function to upload a local file to an S3 bucket.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
@@ -433,25 +428,26 @@
         The key name for the uploaded object.
     file_path : str or pathlib.Path
         The path to the file to be uploaded.
     metadata : dict or None
         A dict of the metadata that should be saved along with the object.
     content_type : str
         The http content type to associate the object with.
+    retries: int
+        The number of url request retries to perform before failing. This shouldn't be necessary given the max_attempts parameter in the s3_client function...but I'll keep it around until it's clearly not needed.
 
     Returns
     -------
     None
     """
     with open(file_path, 'rb') as f:
         put_object_s3(s3, bucket, obj_key, f, metadata, content_type, retries=retries)
 
 
-
-def copy_object_s3(s3: botocore.client.BaseClient, source_bucket: str, dest_bucket: str, source_key: str, dest_key: str, retries=3):
+def copy_object_s3(s3: botocore.client.BaseClient, source_bucket: str, dest_bucket: str, source_key: str, dest_key: str, retries: int=3):
     """
     Copies an object in an S3 database to another location in an S3 database. They must have the same fundemental connection_config. All metadata is copied to the new object.
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.copy_object
 
     Parameters
     ----------
     s3 : boto3.client
@@ -460,18 +456,20 @@
         The S3 source bucket.
     dest_bucket : str
         The S3 destination bucket.
     source_key : str
         The key name for the source object.
     dest_key : str
         The key name for the destination object.
+    retries: int
+        The number of url request retries to perform before failing. This shouldn't be necessary given the max_attempts parameter in the s3_client function...but I'll keep it around until it's clearly not needed.
 
     Returns
     -------
-    None
+    S3 response
     """
     source_dict = {'Bucket': source_bucket, 'Key': source_key}
 
     counter = retries
     while True:
         try:
             resp = s3.copy_object(Bucket=dest_bucket, Key=dest_key, CopySource=source_dict, MetadataDirective='COPY')
@@ -490,30 +488,36 @@
         #         raise err
         #     print('...trying again...')
         #     sleep(3)
 
     return resp
 
 
-def multi_copy_object_s3(s3: botocore.client.BaseClient, source_bucket: str, dest_bucket: str, source_dest_keys: list, retries=5, threads=30):
+def multi_copy_object_s3(s3: botocore.client.BaseClient, source_bucket: str, dest_bucket: str, source_dest_keys: list, retries: int=5, threads: int=30):
     """
     Same as the copy_object_s3 except with multi threading. The input source_dest_keys must be a list of dictionaries with keys named source_key and dest_key.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
     source_bucket : str
         The S3 source bucket.
-    source_dest_bucket : list of dict
+    dest_bucket : str
+        The S3 destination bucket.
+    source_dest_keys : list of dict
         A list of dictionaries with keys named source_key and dest_key. Similar to the copy_obect_s3 function.
+    retries: int
+        The number of url request retries to perform before failing. This shouldn't be necessary given the max_attempts parameter in the s3_client function...but I'll keep it around until it's clearly not needed.
+    threads: int
+        The number of simultaneous copy_object_s3 runs.
 
     Returns
     -------
-    None
+    list of S3 responses
     """
     keys = copy.deepcopy(source_dest_keys)
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=threads) as executor:
         futures = []
         for key in keys:
             key['s3'] = s3
@@ -542,14 +546,16 @@
         Limits the response to keys that begin with the specified prefix.
     start_after : str
         The S3 key to start after.
     delimiter : str
         A delimiter is a character you use to group keys.
     continuation_token : str
         ContinuationToken indicates to S3 that the list is being continued on this bucket with a token.
+    date_format : str
+        If the object key has a date in it, pass a date format string to parse and add a column called KeyDate.
 
     Returns
     -------
     DataFrame
     """
     if s3._endpoint.host == 'https://vault.revera.co.nz':
         js = []
@@ -606,14 +612,16 @@
         The S3 bucket.
     prefix : str
         Limits the response to keys that begin with the specified prefix.
     start_after : str
         The S3 key to start at.
     delimiter : str or None
         A delimiter is a character you use to group keys.
+    date_format : str
+        If the object key has a date in it, pass a date format string to parse and add a column called KeyDate.
 
     Returns
     -------
     DataFrame
     """
     js = []
     while True:
```

### Comparing `s3tethys-0.0.5/s3tethys/utils.py` & `s3tethys-0.0.6/s3tethys/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,26 +4,34 @@
 Created on Sat Oct  8 11:02:46 2022
 
 @author: mike
 """
 import io
 import os
 import pandas as pd
+from pydantic import BaseModel, HttpUrl
 
 #######################################################
 ### Parameters
 
 b2_public_key_pattern = '{base_url}/{bucket}/{obj_key}'
 contabo_public_key_pattern = '{base_url}:{bucket}/{obj_key}'
 
 
 #######################################################
 ### Functions
 
 
+class ConnectionConfig(BaseModel):
+    service_name: str
+    endpoint_url: HttpUrl
+    aws_access_key_id: str
+    aws_secret_access_key: str
+
+
 def create_public_s3_url(base_url, bucket, obj_key):
     """
     This should be updated as more S3 providers are added!
     """
     if 'contabo' in base_url:
         key = contabo_public_key_pattern.format(base_url=base_url.rstrip('/'), bucket=bucket, obj_key=obj_key)
     else:
```

### Comparing `s3tethys-0.0.5/s3tethys.egg-info/PKG-INFO` & `s3tethys-0.0.6/s3tethys.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3tethys
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python S3 tools for tethys using smart_open
 Home-page: https://github.com/tethys-ts/s3tethys
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: tethys s3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s3tethys-0.0.5/setup.py` & `s3tethys-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 's3tethys'
 main_package = 's3tethys'
 datasets = 'datasets'
-version = '0.0.5'
+version = '0.0.6'
 descrip = 'Python S3 tools for tethys using smart_open'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
 else:
-    INSTALL_REQUIRES = ['smart_open', 'boto3', 'requests', 'pandas', 'zstandard', 'tethys-data-models >=0.4.10']
+    INSTALL_REQUIRES = ['smart_open', 'boto3', 'pandas', 'zstandard', 'requests']
 
 # Get the long description from the README file
 with open(os.path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 # get all data dirs in the datasets module
 # data_files = []
```

