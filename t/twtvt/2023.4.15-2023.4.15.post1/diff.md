# Comparing `tmp/twtvt-2023.4.15.tar.gz` & `tmp/twtvt-2023.4.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtvt-2023.4.15.tar", max compression
+gzip compressed data, was "twtvt-2023.4.15.post1.tar", max compression
```

## Comparing `twtvt-2023.4.15.tar` & `twtvt-2023.4.15.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1042 2023-04-15 09:29:29.829125 twtvt-2023.4.15/README.md
--rw-r--r--   0        0        0     1443 2023-04-15 09:29:50.669681 twtvt-2023.4.15/pyproject.toml
--rw-r--r--   0        0        0      120 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/__init__.py
--rw-r--r--   0        0        0      110 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/__main__.py
--rw-r--r--   0        0        0       41 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/cli/__init__.py
--rw-r--r--   0        0        0     1148 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/cli/commands.py
--rw-r--r--   0        0        0       79 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/main.py
--rw-r--r--   0        0        0        0 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/tests/sample_test.py
--rw-r--r--   0        0        0      238 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/utils/__init__.py
--rw-r--r--   0        0        0     2013 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/utils/download_video.py
--rw-r--r--   0        0        0      249 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/utils/logger.py
--rw-r--r--   0        0        0     1353 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/utils/monsnode_parser.py
--rw-r--r--   0        0        0     7831 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/utils/twitter_parser.py
--rw-r--r--   0        0        0      676 2023-04-15 09:29:29.833125 twtvt-2023.4.15/twtvt/utils/url_validator.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 twtvt-2023.4.15/PKG-INFO
+-rw-r--r--   0        0        0     1017 2023-04-15 09:42:21.736242 twtvt-2023.4.15.post1/README.md
+-rw-r--r--   0        0        0     1445 2023-04-15 09:42:45.064562 twtvt-2023.4.15.post1/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/__main__.py
+-rw-r--r--   0        0        0       41 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/cli/__init__.py
+-rw-r--r--   0        0        0     1150 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/cli/commands.py
+-rw-r--r--   0        0        0       79 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/main.py
+-rw-r--r--   0        0        0        0 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/tests/sample_test.py
+-rw-r--r--   0        0        0      238 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/__init__.py
+-rw-r--r--   0        0        0     2017 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/download_video.py
+-rw-r--r--   0        0        0      249 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/logger.py
+-rw-r--r--   0        0        0     1353 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/monsnode_parser.py
+-rw-r--r--   0        0        0     7831 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/twitter_parser.py
+-rw-r--r--   0        0        0      676 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/url_validator.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 twtvt-2023.4.15.post1/PKG-INFO
```

### Comparing `twtvt-2023.4.15/pyproject.toml` & `twtvt-2023.4.15.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "twtvt"
-version = "2023.04.15"
+version = "2023.04.15-1"
 description = ""
 authors = []
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "twtvt"
 
 [tool.pyright]
```

### Comparing `twtvt-2023.4.15/twtvt/cli/commands.py` & `twtvt-2023.4.15.post1/twtvt/cli/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 cli_app = Typer()
 
 
 @cli_app.command()
 def twtvt(
     target_links: list[str] = typer.Argument(..., help="Video tweet link or target user's likes or media."),
     username: str = typer.Argument(..., help='Your twitter credentials username.'),
-    password: str = typer.Option(..., help='Your twitter credentials password.'),
+    password: str = typer.Argument(..., help='Your twitter credentials password.'),
     cookies_from_browser: Optional[str] = typer.Option(None, help='Browser to get cookies from. '),
     output: str = typer.Option('videos', help='Output path for downloaded videos.'),
     debug: bool = typer.Option(False, help='Enable debug mode. This disables headless mode of Browser.'),
     until_link: Optional[str] = typer.Option(
         None,
         help="Keeps finding videos until this link is found. None for no limit. Only for user's likes or media.",
     ),
```

### Comparing `twtvt-2023.4.15/twtvt/utils/download_video.py` & `twtvt-2023.4.15.post1/twtvt/utils/download_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     debug: bool = False,
     cookies_from_browser: Optional[str] = None,
     until_link: Optional[str] = None,
 ):
 
     # load playwright
     with sync_playwright() as playwright_sync:
-        browser = playwright_sync.webkit.launch(headless=debug)
+        browser = playwright_sync.webkit.launch(headless=not debug)
         page = browser.new_page()
 
         # load parser
         parser = TwitterParser(page)
         parser.login(username, password)
 
         # extract video links
```

### Comparing `twtvt-2023.4.15/twtvt/utils/monsnode_parser.py` & `twtvt-2023.4.15.post1/twtvt/utils/monsnode_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15/twtvt/utils/twitter_parser.py` & `twtvt-2023.4.15.post1/twtvt/utils/twitter_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15/twtvt/utils/url_validator.py` & `twtvt-2023.4.15.post1/twtvt/utils/url_validator.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15/PKG-INFO` & `twtvt-2023.4.15.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twtvt
-Version: 2023.4.15
+Version: 2023.4.15.post1
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
@@ -36,15 +36,15 @@
 ```
 
 ## Usage
 
 ### Command line
 
 ```sh
-python3 -m twitter_video_tools --help
+twtvt --help
 ```
 
 Supported link types:
 
 - Video tweet: <https://twitter.com/twtvtOfficial/status/1599748329927499777>
 - Video from [monsnode](https://monsnode.com): <https://monsnode.com/v1506575871309589251>
 - Specific user's uploaded videos: <https://twitter.com/twtvtOfficial/media>
```

