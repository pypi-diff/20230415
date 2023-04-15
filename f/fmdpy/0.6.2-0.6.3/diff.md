# Comparing `tmp/fmdpy-0.6.2.tar.gz` & `tmp/fmdpy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmdpy-0.6.2.tar", last modified: Mon Mar 20 11:50:26 2023, max compression
+gzip compressed data, was "fmdpy-0.6.3.tar", last modified: Sat Apr 15 06:51:56 2023, max compression
```

## Comparing `fmdpy-0.6.2.tar` & `fmdpy-0.6.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 11:50:25.994536 fmdpy-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-20 11:50:16.000000 fmdpy-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-03-20 11:50:25.994536 fmdpy-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-03-20 11:50:16.000000 fmdpy-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 11:50:25.990536 fmdpy-0.6.2/fmdpy/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/download.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/song.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/splist.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-20 11:50:16.000000 fmdpy-0.6.2/fmdpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 11:50:25.994536 fmdpy-0.6.2/fmdpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-03-20 11:50:25.000000 fmdpy-0.6.2/fmdpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-20 11:50:25.000000 fmdpy-0.6.2/fmdpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 11:50:25.000000 fmdpy-0.6.2/fmdpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 11:50:25.000000 fmdpy-0.6.2/fmdpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-20 11:50:25.000000 fmdpy-0.6.2/fmdpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-20 11:50:25.000000 fmdpy-0.6.2/fmdpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 11:50:25.994536 fmdpy-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-20 11:50:16.000000 fmdpy-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:56.100744 fmdpy-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 06:51:49.000000 fmdpy-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-04-15 06:51:56.100744 fmdpy-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-15 06:51:49.000000 fmdpy-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:56.096744 fmdpy-0.6.3/fmdpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/song.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/splist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-15 06:51:49.000000 fmdpy-0.6.3/fmdpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:56.096744 fmdpy-0.6.3/fmdpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-04-15 06:51:55.000000 fmdpy-0.6.3/fmdpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-15 06:51:56.000000 fmdpy-0.6.3/fmdpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 06:51:55.000000 fmdpy-0.6.3/fmdpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-15 06:51:55.000000 fmdpy-0.6.3/fmdpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 06:51:55.000000 fmdpy-0.6.3/fmdpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 06:51:55.000000 fmdpy-0.6.3/fmdpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 06:51:56.100744 fmdpy-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-15 06:51:49.000000 fmdpy-0.6.3/setup.py
```

### Comparing `fmdpy-0.6.2/LICENSE` & `fmdpy-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/PKG-INFO` & `fmdpy-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmdpy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Music Downloader
 Home-page: https://github.com/Liupold/fmdpy
 Author: Rohn Chatterjee
 Author-email: rohn.ch@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fmdpy-0.6.2/README.md` & `fmdpy-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/fmdpy/__init__.py` & `fmdpy-0.6.3/fmdpy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """fmdpy."""
 from . import conf
 
-VERSION = "0.6.2"
+VERSION = "0.6.3"
 install_requires = ['click', 'music-tag>=0.4.3', 'requests', 'pillow',
-                    'lyricsgenius', 'dataclasses', 'spotipy', 'tqdm', 'pydub']
+                    'lyricsgenius', 'dataclasses', 'spotipy', 'tqdm', 'pydub',
+                    'pycryptodome']
 
 headers = {
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 ' +
     '(KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36'
 }
 
 ART = fr'''
```

### Comparing `fmdpy-0.6.2/fmdpy/__main__.py` & `fmdpy-0.6.3/fmdpy/__main__.py`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/fmdpy/api.py` & `fmdpy-0.6.3/fmdpy/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """api for fetching song metadata and url."""
+import base64 as bs64
 import requests
+from Crypto.Cipher import DES
 from fmdpy import headers, ART
 from fmdpy.song import Song
 
 def get_song_urls(song_obj):
     """Fetch song download url."""
     req = requests.get(headers=headers,
-                       url="https://www.jiosaavn.com/api.php?__call=song.getDetails&cc=in" \
-                               + f"&_marker=0%3F_marker%3D0&_format=json&pids={song_obj.songid}")
-    raw_json = req.json()[song_obj.songid]
-    if 'media_preview_url' in raw_json.keys():
-        song_obj.url = raw_json['media_preview_url'].\
-            replace('https://preview.saavncdn.com/', 'https://aac.saavncdn.com/').\
-            replace('_96_p.mp4', '_320.mp4')
+                       url="https://www.jiosaavn.com/api.php?__call=song.getDetails" \
+                               + f"&ctx=web6dot0&_marker=0&_format=json&pids={song_obj.songid}")
+
+    raw_json = req.json()['songs'][0]
+    if 'encrypted_media_url' in raw_json.keys():
+        key = '38346591'.encode('utf-8')
+        dciper = DES.new(key, DES.MODE_ECB)
+        decrypted = dciper.decrypt(bs64.b64decode(raw_json['encrypted_media_url']))
+        song_obj.url = decrypted.replace(b'\x05', b'').decode().replace('_96', '_320')
         song_obj.thumb_url = raw_json['image'].replace(
             '-150x150.jpg', '-500x500.jpg')
 
 def parse_search_query(query_json):
     song_list = []
     for sng_raw in query_json['results']:
         song_id = sng_raw['id']
```

### Comparing `fmdpy-0.6.2/fmdpy/conf.py` & `fmdpy-0.6.3/fmdpy/conf.py`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/fmdpy/download.py` & `fmdpy-0.6.3/fmdpy/download.py`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/fmdpy/splist.py` & `fmdpy-0.6.3/fmdpy/splist.py`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/fmdpy/stream.py` & `fmdpy-0.6.3/fmdpy/stream.py`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/fmdpy/utils.py` & `fmdpy-0.6.3/fmdpy/utils.py`

 * *Files identical despite different names*

### Comparing `fmdpy-0.6.2/fmdpy.egg-info/PKG-INFO` & `fmdpy-0.6.3/fmdpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmdpy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Music Downloader
 Home-page: https://github.com/Liupold/fmdpy
 Author: Rohn Chatterjee
 Author-email: rohn.ch@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fmdpy-0.6.2/setup.py` & `fmdpy-0.6.3/setup.py`

 * *Files identical despite different names*

