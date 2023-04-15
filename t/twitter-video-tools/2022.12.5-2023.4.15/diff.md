# Comparing `tmp/twitter_video_tools-2022.12.5.tar.gz` & `tmp/twitter_video_tools-2023.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_video_tools-2022.12.5.tar", max compression
+gzip compressed data, was "twitter_video_tools-2023.4.15.tar", max compression
```

## Comparing `twitter_video_tools-2022.12.5.tar` & `twitter_video_tools-2023.4.15.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1068 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/LICENSE
--rw-r--r--   0        0        0     4377 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/README.md
--rw-r--r--   0        0        0     2907 2022-12-05 14:03:32.305993 twitter_video_tools-2022.12.5/pyproject.toml
--rw-r--r--   0        0        0     1487 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/twitter_video_tools/__init__.py
--rw-r--r--   0        0        0       86 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/twitter_video_tools/__main__.py
--rw-r--r--   0        0        0     1422 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/twitter_video_tools/monsnode_parser.py
--rw-r--r--   0        0        0     2782 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/twitter_video_tools/platform_video_downloader.py
--rw-r--r--   0        0        0        0 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/twitter_video_tools/py.typed
--rw-r--r--   0        0        0        0 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/twitter_video_tools/tests/__init__.py
--rw-r--r--   0        0        0     1287 2022-12-05 14:03:06.490117 twitter_video_tools-2022.12.5/twitter_video_tools/tests/test_monsnode_parser.py
--rw-r--r--   0        0        0     7448 2022-12-05 14:03:06.494117 twitter_video_tools-2022.12.5/twitter_video_tools/twitter_crawler.py
--rw-r--r--   0        0        0     2549 2022-12-05 14:03:06.494117 twitter_video_tools-2022.12.5/twitter_video_tools/twitter_video_tools.py
--rw-r--r--   0        0        0      236 2022-12-05 14:03:06.494117 twitter_video_tools-2022.12.5/twitter_video_tools/utils/__init__.py
--rw-r--r--   0        0        0      300 2022-12-05 14:03:06.494117 twitter_video_tools-2022.12.5/twitter_video_tools/utils/execute_parallel.py
--rw-r--r--   0        0        0      676 2022-12-05 14:03:06.494117 twitter_video_tools-2022.12.5/twitter_video_tools/utils/url_validator.py
--rw-r--r--   0        0        0     1013 2022-12-05 14:03:06.494117 twitter_video_tools-2022.12.5/twitter_video_tools/utils/youtube_dl_wrapper.py
--rw-r--r--   0        0        0     1504 2022-12-05 14:03:06.494117 twitter_video_tools-2022.12.5/twitter_video_tools/video_downloader.py
--rw-r--r--   0        0        0     5455 1970-01-01 00:00:00.000000 twitter_video_tools-2022.12.5/setup.py
--rw-r--r--   0        0        0     5629 1970-01-01 00:00:00.000000 twitter_video_tools-2022.12.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/LICENSE
+-rw-r--r--   0        0        0     4484 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/README.md
+-rw-r--r--   0        0        0     2908 2023-04-15 09:21:07.237985 twitter_video_tools-2023.4.15/pyproject.toml
+-rw-r--r--   0        0        0     1769 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/__main__.py
+-rw-r--r--   0        0        0     1422 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/monsnode_parser.py
+-rw-r--r--   0        0        0     2782 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/platform_video_downloader.py
+-rw-r--r--   0        0        0        0 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/py.typed
+-rw-r--r--   0        0        0        0 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/tests/__init__.py
+-rw-r--r--   0        0        0     1287 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/tests/test_monsnode_parser.py
+-rw-r--r--   0        0        0     7448 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/twitter_crawler.py
+-rw-r--r--   0        0        0     2550 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/twitter_video_tools.py
+-rw-r--r--   0        0        0      236 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/utils/__init__.py
+-rw-r--r--   0        0        0      300 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/utils/execute_parallel.py
+-rw-r--r--   0        0        0      676 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/utils/url_validator.py
+-rw-r--r--   0        0        0     1013 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/utils/youtube_dl_wrapper.py
+-rw-r--r--   0        0        0     1504 2023-04-15 09:20:28.897750 twitter_video_tools-2023.4.15/twitter_video_tools/video_downloader.py
+-rw-r--r--   0        0        0     5736 1970-01-01 00:00:00.000000 twitter_video_tools-2023.4.15/PKG-INFO
```

### Comparing `twitter_video_tools-2022.12.5/LICENSE` & `twitter_video_tools-2023.4.15/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/README.md` & `twitter_video_tools-2023.4.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+**This project is deprecated. Please look at <https://github.com/code-yeongyu/twitter_video_tools_v2>** 
+
 # Twitter Video Tools
 
+
 [![PyPI version](https://badge.fury.io/py/twitter-video-tools.svg)](https://badge.fury.io/py/twitter-video-tools)
 [![Test](https://github.com/code-yeongyu/twitter_video_tools/actions/workflows/test.yaml/badge.svg?branch=master)](https://github.com/code-yeongyu/twitter_video_tools/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/code-yeongyu/TwitterVideoTools/branch/master/graph/badge.svg?token=97K8BBWOH7)](https://codecov.io/gh/code-yeongyu/TwitterVideoTools)
 
 - A multi-processing supported video downloader
 - supports downloading videos from twitter (or specific user from twitter) && monsnode.
```

### Comparing `twitter_video_tools-2022.12.5/pyproject.toml` & `twitter_video_tools-2023.4.15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = []
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/code-yeongyu/twitter_video_tools"
 keywords = [ "crawler", "parser", "downloader", "monsnode", "twitter", "youtube_dl",]
 classifiers = [ "Environment :: Console", "Operating System :: OS Independent", "Topic :: Software Development :: Libraries :: Python Modules", "Topic :: Software Development :: Testing :: Unit", "Topic :: Software Development :: Version Control", "Topic :: Internet :: WWW/HTTP :: Browsers", "Typing :: Typed",]
 include = [ "LICENSE",]
-version = "2022.12.05"
+version = "v2023.04.15"
 
 [tool.mypy]
 disallow_untyped_defs = true
 disallow_any_unimported = true
 no_implicit_optional = true
 check_untyped_defs = true
 warn_return_any = true
```

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/__init__.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 import typer
 from rich import print as rich_print
 
 from .twitter_video_tools import TwitterVideoTools as TwitterVideoTools
 from .utils import URLValidator
 
 
-def _cli_main(
-    link: str = typer.Argument(..., help='Video tweet link or target user\'s likes or media.'),
-    username: Optional[str] = typer.Option(None, help='Your twitter credentials username.'),
-    password: Optional[str] = typer.Option(None, help='Your twitter credentials password.'),
-    until_link: Optional[str] = typer.Option(
-        None,
-        help='Keeps finding videos until this link is found. None for no limit. Only for user\'s likes or media.',
-    ),
+def _cli_main(    # pylint: disable=too-many-arguments
+        link: str = typer.Argument(..., help='Video tweet link or target user\'s likes or media.'),
+        username: Optional[str] = typer.Option(None, help='Your twitter credentials username.'),
+        password: Optional[str] = typer.Option(None, help='Your twitter credentials password.'),
+        until_link: Optional[str] = typer.Option(
+            None,
+            help='Keeps finding videos until this link is found. None for no limit. Only for user\'s likes or media.',
+        ),
+        output: str = typer.Option('videos', help='Output path for downloaded videos.'),
+        debug: bool = typer.Option(False, help='Enable debug mode. This disables headless mode of Browser.'),
 ) -> None:
     url_validator = URLValidator(link)
 
     if not url_validator.is_valid_link():
         rich_print(f'\'[underline]{link}[/underline]\' [bold red]is an invalid link.[/bold red]')
         return
-    twitter_video_tools = TwitterVideoTools(username, password)
+    twitter_video_tools = TwitterVideoTools(username, password, output, debug)
 
     if url_validator.is_valid_twitter_media_link():
         target_username = link.split('/')[3]
         twitter_video_tools.download_from_user(target_username, until_link)
     elif url_validator.is_valid_twitter_liked_link():
         target_username = link.split('/')[3]
         twitter_video_tools.download_from_liked_tweets(target_username, until_link)
```

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/monsnode_parser.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/monsnode_parser.py`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/platform_video_downloader.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/platform_video_downloader.py`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/tests/test_monsnode_parser.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/tests/test_monsnode_parser.py`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/twitter_crawler.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/twitter_crawler.py`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/twitter_video_tools.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/twitter_video_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ) -> None:
         self.username = username
         self.password = password
         self._debug = debug
         platform_video_downloader = PlatformVideoDownloader(video_output_path)
         self.video_downloader = VideoDownloader(username, password, platform_video_downloader)
 
-        self._browser = sync_playwright().start().webkit.launch(headless=True)
+        self._browser = sync_playwright().start().webkit.launch(headless=debug)
         page = self._browser.new_page()
         self.twitter_crawler = TwitterCrawler(page)
         if self.username and self.password:
             self.twitter_crawler.login(self.username, self.password)
 
     def __enter__(self) -> TwitterVideoTools:
         return self
```

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/utils/url_validator.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/utils/url_validator.py`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/utils/youtube_dl_wrapper.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/utils/youtube_dl_wrapper.py`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/twitter_video_tools/video_downloader.py` & `twitter_video_tools-2023.4.15/twitter_video_tools/video_downloader.py`

 * *Files identical despite different names*

### Comparing `twitter_video_tools-2022.12.5/PKG-INFO` & `twitter_video_tools-2023.4.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-video-tools
-Version: 2022.12.5
+Version: 2023.4.15
 Summary: Twitter Video Tools is a multi-processing supported video downloader, supports videos from twitter (or specific user from twitter) && monsnode.
 Home-page: https://github.com/code-yeongyu/twitter_video_tools
 License: MIT
 Keywords: crawler,parser,downloader,monsnode,twitter,youtube_dl
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -21,16 +21,19 @@
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: playwright (>=1.27.1,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: yt-dlp (>=2022.11.11,<2023.0.0)
 Description-Content-Type: text/markdown
 
+**This project is deprecated. Please look at <https://github.com/code-yeongyu/twitter_video_tools_v2>** 
+
 # Twitter Video Tools
 
+
 [![PyPI version](https://badge.fury.io/py/twitter-video-tools.svg)](https://badge.fury.io/py/twitter-video-tools)
 [![Test](https://github.com/code-yeongyu/twitter_video_tools/actions/workflows/test.yaml/badge.svg?branch=master)](https://github.com/code-yeongyu/twitter_video_tools/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/code-yeongyu/TwitterVideoTools/branch/master/graph/badge.svg?token=97K8BBWOH7)](https://codecov.io/gh/code-yeongyu/TwitterVideoTools)
 
 - A multi-processing supported video downloader
 - supports downloading videos from twitter (or specific user from twitter) && monsnode.
```

