# Comparing `tmp/duckduckgo_search-2.8.5.tar.gz` & `tmp/duckduckgo_search-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-2.8.5.tar", last modified: Sun Mar 12 12:07:07 2023, max compression
+gzip compressed data, was "duckduckgo_search-2.8.6.tar", last modified: Sat Apr 15 09:07:48 2023, max compression
```

## Comparing `duckduckgo_search-2.8.5.tar` & `duckduckgo_search-2.8.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:07:07.282963 duckduckgo_search-2.8.5/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-03-12 12:07:07.282963 duckduckgo_search-2.8.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:07:07.282963 duckduckgo_search-2.8.5/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:07:07.282963 duckduckgo_search-2.8.5/duckduckgo_search/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/cli/ddgs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5904 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6136 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1548 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/ddg_videos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3551 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:07:07.282963 duckduckgo_search-2.8.5/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-03-12 12:07:07.000000 duckduckgo_search-2.8.5/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-12 12:07:07.000000 duckduckgo_search-2.8.5/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 12:07:07.000000 duckduckgo_search-2.8.5/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-12 12:07:07.000000 duckduckgo_search-2.8.5/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-12 12:07:07.000000 duckduckgo_search-2.8.5/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-12 12:07:07.000000 duckduckgo_search-2.8.5/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 12:07:07.282963 duckduckgo_search-2.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 12:07:07.282963 duckduckgo_search-2.8.5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg_answers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg_news.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg_suggestions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-03-12 12:06:49.000000 duckduckgo_search-2.8.5/tests/test_ddg_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34567 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/duckduckgo_search/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10405 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/cli/ddgs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6014 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6246 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7090 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1548 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/ddg_videos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3570 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35682 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 09:07:48.000000 duckduckgo_search-2.8.6/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:07:48.312422 duckduckgo_search-2.8.6/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_answers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_news.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_suggestions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-15 09:07:34.000000 duckduckgo_search-2.8.6/tests/test_ddg_videos.py
```

### Comparing `duckduckgo_search-2.8.5/LICENSE.md` & `duckduckgo_search-2.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/PKG-INFO` & `duckduckgo_search-2.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 2.8.5
+Version: 2.8.6
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.8.5/README.md` & `duckduckgo_search-2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/__init__.py` & `duckduckgo_search-2.8.6/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/cli/ddgs.py` & `duckduckgo_search-2.8.6/duckduckgo_search/cli/ddgs.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from time import sleep
-from unicodedata import normalize
+from urllib.parse import unquote
 
 from click import progressbar
 
 from .utils import SESSION, _do_output, _download_file, _get_vqd, _normalize
 
 logger = logging.getLogger(__name__)
 
@@ -113,21 +113,26 @@
 
     # save to csv or json file
     if output:
         _do_output("ddg", keywords, output, results)
 
     # download documents
     if download:
-        keywords = keywords.replace('"', "'")
+        keywords = (
+            keywords.replace('"', "'")
+            .replace("site:", "")
+            .replace(" ", "_")
+            .replace("/", "_")
+        )
         path = f"ddg_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
         os.makedirs(path, exist_ok=True)
         futures = []
         with ThreadPoolExecutor(10) as executor:
             for i, res in enumerate(results, start=1):
-                filename = normalize("NFC", res["href"].split("/")[-1].split("?")[0])
+                filename = unquote(res["href"].split("/")[-1].split("?")[0])
                 future = executor.submit(
                     _download_file, res["href"], path, f"{i}_{filename}"
                 )
                 futures.append(future)
             with progressbar(
                 as_completed(futures),
                 label="Downloading documents",
```

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg_answers.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg_images.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from time import sleep
-from unicodedata import normalize
+from urllib.parse import unquote
 
 from click import progressbar
 
 from .utils import SESSION, _do_output, _download_file, _get_vqd
 
 logger = logging.getLogger(__name__)
 
@@ -134,21 +134,26 @@
 
     # save to csv or json file
     if output:
         _do_output("ddg_images", keywords, output, results)
 
     # download images
     if download:
-        keywords = keywords.replace('"', "'")
+        keywords = (
+            keywords.replace('"', "'")
+            .replace("site:", "")
+            .replace(" ", "_")
+            .replace("/", "_")
+        )
         path = f"ddg_images_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
         os.makedirs(path, exist_ok=True)
         futures = []
         with ThreadPoolExecutor(30) as executor:
             for i, res in enumerate(results, start=1):
-                filename = normalize("NFC", res["image"].split("/")[-1].split("?")[0])
+                filename = unquote(res["image"].split("/")[-1].split("?")[0])
                 future = executor.submit(
                     _download_file, res["image"], path, f"{i}_{filename}"
                 )
                 futures.append(future)
             with progressbar(
                 as_completed(futures),
                 label="Downloading images",
```

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg_maps.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg_maps.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg_news.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg_suggestions.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg_translate.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/ddg_videos.py` & `duckduckgo_search-2.8.6/duckduckgo_search/ddg_videos.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search/utils.py` & `duckduckgo_search-2.8.6/duckduckgo_search/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import csv
-import html
 import json
 import logging
 import os
 import re
-import shutil
 from datetime import datetime
+from html import unescape
+from shutil import copyfileobj
 from time import sleep
 
 import requests
 
 logger = logging.getLogger(__name__)
 
 HEADERS = {
@@ -85,24 +85,24 @@
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0"
     }
     try:
         with requests.get(url, headers=headers, stream=True, timeout=10) as resp:
             resp.raise_for_status()
             resp.raw.decode_content = True
             with open(os.path.join(dir_path, filename), "wb") as file:
-                shutil.copyfileobj(resp.raw, file)
+                copyfileobj(resp.raw, file)
             logger.info(f"File downloaded {url}")
     except Exception:
         logger.exception("")
 
 
 def _normalize(raw_html):
     """strip HTML tags"""
     if raw_html:
-        return html.unescape(re.sub(RE_STRIP_TAGS, "", raw_html))
+        return unescape(re.sub(RE_STRIP_TAGS, "", raw_html))
 
 
 def _do_output(module_name, keywords, output, results):
     keywords = keywords.replace('"', "'")
     if output == "csv":
         _save_csv(
             f"{module_name}_{keywords}_{datetime.now():%Y%m%d_%H%M%S}.csv", results
```

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-2.8.6/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 2.8.5
+Version: 2.8.6
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-2.8.5/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-2.8.6/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/pyproject.toml` & `duckduckgo_search-2.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/tests/test_ddg.py` & `duckduckgo_search-2.8.6/tests/test_ddg.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,14 +57,7 @@
         raise AssertionError("Files not found")
 
     # delete folder contains keyword in name
     for dir in os.listdir():
         if f"ddg_{keywords}" in dir:
             if os.path.isdir(dir):
                 shutil.rmtree(dir)
-
-
-# results not found
-def test_ddg_not_results():
-    random_chars = "".join(chr(randrange(65, 90)) for i in range(100))
-    results = ddg(random_chars, safesearch="Off", time="d")
-    assert results is None
```

### Comparing `duckduckgo_search-2.8.5/tests/test_ddg_answers.py` & `duckduckgo_search-2.8.6/tests/test_ddg_answers.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/tests/test_ddg_images.py` & `duckduckgo_search-2.8.6/tests/test_ddg_images.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/tests/test_ddg_news.py` & `duckduckgo_search-2.8.6/tests/test_ddg_news.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/tests/test_ddg_suggestions.py` & `duckduckgo_search-2.8.6/tests/test_ddg_suggestions.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/tests/test_ddg_translate.py` & `duckduckgo_search-2.8.6/tests/test_ddg_translate.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-2.8.5/tests/test_ddg_videos.py` & `duckduckgo_search-2.8.6/tests/test_ddg_videos.py`

 * *Files identical despite different names*

