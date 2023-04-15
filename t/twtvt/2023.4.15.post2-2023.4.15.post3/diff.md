# Comparing `tmp/twtvt-2023.4.15.post2.tar.gz` & `tmp/twtvt-2023.4.15.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtvt-2023.4.15.post2.tar", max compression
+gzip compressed data, was "twtvt-2023.4.15.post3.tar", max compression
```

## Comparing `twtvt-2023.4.15.post2.tar` & `twtvt-2023.4.15.post3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1017 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/README.md
--rw-r--r--   0        0        0     1445 2023-04-15 11:36:32.093193 twtvt-2023.4.15.post2/pyproject.toml
--rw-r--r--   0        0        0      120 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/__init__.py
--rw-r--r--   0        0        0      110 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/__main__.py
--rw-r--r--   0        0        0       41 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/cli/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/cli/commands.py
--rw-r--r--   0        0        0       79 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/main.py
--rw-r--r--   0        0        0        0 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/tests/sample_test.py
--rw-r--r--   0        0        0      238 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/__init__.py
--rw-r--r--   0        0        0     4014 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/download_video.py
--rw-r--r--   0        0        0      249 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/logger.py
--rw-r--r--   0        0        0     1354 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/monsnode_parser.py
--rw-r--r--   0        0        0     7831 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/twitter_parser.py
--rw-r--r--   0        0        0      566 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/uri_validator.py
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 twtvt-2023.4.15.post2/PKG-INFO
+-rw-r--r--   0        0        0     1017 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/README.md
+-rw-r--r--   0        0        0     1465 2023-04-15 14:50:37.808502 twtvt-2023.4.15.post3/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/__main__.py
+-rw-r--r--   0        0        0       41 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/cli/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/cli/commands.py
+-rw-r--r--   0        0        0       79 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/main.py
+-rw-r--r--   0        0        0        0 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/tests/sample_test.py
+-rw-r--r--   0        0        0      238 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/__init__.py
+-rw-r--r--   0        0        0     4603 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/download_video.py
+-rw-r--r--   0        0        0      249 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/logger.py
+-rw-r--r--   0        0        0     1354 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/monsnode_parser.py
+-rw-r--r--   0        0        0     7831 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/twitter_parser.py
+-rw-r--r--   0        0        0      566 2023-04-15 14:50:13.568083 twtvt-2023.4.15.post3/twtvt/utils/uri_validator.py
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 twtvt-2023.4.15.post3/PKG-INFO
```

### Comparing `twtvt-2023.4.15.post2/README.md` & `twtvt-2023.4.15.post3/README.md`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post2/pyproject.toml` & `twtvt-2023.4.15.post3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "twtvt"
-version = "2023.04.15-2"
+version = "2023.04.15-3"
 description = ""
 authors = []
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "twtvt"
 
 [tool.pyright]
@@ -43,14 +43,15 @@
 poetry = "^1.4.0"
 playwright = "^1.32.1"
 beautifulsoup4 = "^4.12.2"
 httpx = "^0.24.0"
 typer = "^0.7.0"
 rich = "^13.3.4"
 yt-dlp = "^2023.3.4"
+tenacity = "^8.2.2"
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 docstring-quotes = "single"
 multiline-quotes = "single"
 
 [tool.pytest.ini_options]
```

### Comparing `twtvt-2023.4.15.post2/twtvt/cli/commands.py` & `twtvt-2023.4.15.post3/twtvt/cli/commands.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post2/twtvt/utils/download_video.py` & `twtvt-2023.4.15.post3/twtvt/utils/download_video.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import logging
 import time
 from typing import Iterable, Optional, Union
 
 import yt_dlp
 from playwright.sync_api import sync_playwright
+from tenacity import after_log, before_sleep_log, retry, stop_after_attempt, wait_fixed
 
 from .logger import logger
 from .twitter_parser import TwitterParser
 from .uri_validator import URIValidator
 
 
 def download_video(
@@ -92,17 +94,30 @@
 
 
 def _backup_links(links: tuple[str], output: str):
     with open(f'{output}/links-{int(time.time())}-{len(links)}_videos.txt', 'w') as f:
         f.write('\n'.join(links))
 
 
-def _download_videos(video_links: Iterable[str], output: str, cookies_from_browser: Optional[str]):
+def _download_videos(video_links: tuple[str], output: str, cookies_from_browser: Optional[str]):
+    for index, video_link in enumerate(video_links):
+        logger.info(f'Downloading video from {video_link} ({index + 1}/{len(video_links)})')
+        _download_video(video_link, output, cookies_from_browser)
+
+
+@retry(
+    reraise=True,
+    before_sleep=before_sleep_log(logger, logging.DEBUG),
+    after=after_log(logger, logging.INFO),
+    stop=stop_after_attempt(60),
+    wait=wait_fixed(5),
+)
+def _download_video(video_link: str, output: str, cookies_from_browser: Optional[str]):
     ydl_opts: dict[str, Union[str, bool, tuple[Optional[str]]]] = {
         'nocheckcertificate': True,
     }
     ydl_opts['outtmpl'] = f'{output}/%(title)s.%(upload_date>%Y-%m-%d)s.%(id)s.%(ext)s'
     if cookies_from_browser:
         ydl_opts['cookiesfrombrowser'] = (cookies_from_browser, )  # noqa
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-        ydl.download(video_links)
+        ydl.download([video_link])
```

### Comparing `twtvt-2023.4.15.post2/twtvt/utils/monsnode_parser.py` & `twtvt-2023.4.15.post3/twtvt/utils/monsnode_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post2/twtvt/utils/twitter_parser.py` & `twtvt-2023.4.15.post3/twtvt/utils/twitter_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post2/twtvt/utils/uri_validator.py` & `twtvt-2023.4.15.post3/twtvt/utils/uri_validator.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post2/PKG-INFO` & `twtvt-2023.4.15.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: twtvt
-Version: 2023.4.15.post2
+Version: 2023.4.15.post3
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: playwright (>=1.32.1,<2.0.0)
 Requires-Dist: poetry (>=1.4.0,<2.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # Twitter Video Tools V2
 
 - A Twitter video downloader
```

