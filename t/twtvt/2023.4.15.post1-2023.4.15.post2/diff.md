# Comparing `tmp/twtvt-2023.4.15.post1.tar.gz` & `tmp/twtvt-2023.4.15.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtvt-2023.4.15.post1.tar", max compression
+gzip compressed data, was "twtvt-2023.4.15.post2.tar", max compression
```

## Comparing `twtvt-2023.4.15.post1.tar` & `twtvt-2023.4.15.post2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1017 2023-04-15 09:42:21.736242 twtvt-2023.4.15.post1/README.md
--rw-r--r--   0        0        0     1445 2023-04-15 09:42:45.064562 twtvt-2023.4.15.post1/pyproject.toml
--rw-r--r--   0        0        0      120 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/__init__.py
--rw-r--r--   0        0        0      110 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/__main__.py
--rw-r--r--   0        0        0       41 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/cli/__init__.py
--rw-r--r--   0        0        0     1150 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/cli/commands.py
--rw-r--r--   0        0        0       79 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/main.py
--rw-r--r--   0        0        0        0 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/tests/sample_test.py
--rw-r--r--   0        0        0      238 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/__init__.py
--rw-r--r--   0        0        0     2017 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/download_video.py
--rw-r--r--   0        0        0      249 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/logger.py
--rw-r--r--   0        0        0     1353 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/monsnode_parser.py
--rw-r--r--   0        0        0     7831 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/twitter_parser.py
--rw-r--r--   0        0        0      676 2023-04-15 09:42:21.740243 twtvt-2023.4.15.post1/twtvt/utils/url_validator.py
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 twtvt-2023.4.15.post1/PKG-INFO
+-rw-r--r--   0        0        0     1017 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/README.md
+-rw-r--r--   0        0        0     1445 2023-04-15 11:36:32.093193 twtvt-2023.4.15.post2/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/__main__.py
+-rw-r--r--   0        0        0       41 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/cli/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/cli/commands.py
+-rw-r--r--   0        0        0       79 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/main.py
+-rw-r--r--   0        0        0        0 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/tests/sample_test.py
+-rw-r--r--   0        0        0      238 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/__init__.py
+-rw-r--r--   0        0        0     4014 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/download_video.py
+-rw-r--r--   0        0        0      249 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/logger.py
+-rw-r--r--   0        0        0     1354 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/monsnode_parser.py
+-rw-r--r--   0        0        0     7831 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/twitter_parser.py
+-rw-r--r--   0        0        0      566 2023-04-15 11:36:10.132994 twtvt-2023.4.15.post2/twtvt/utils/uri_validator.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 twtvt-2023.4.15.post2/PKG-INFO
```

### Comparing `twtvt-2023.4.15.post1/README.md` & `twtvt-2023.4.15.post2/README.md`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post1/pyproject.toml` & `twtvt-2023.4.15.post2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "twtvt"
-version = "2023.04.15-1"
+version = "2023.04.15-2"
 description = ""
 authors = []
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "twtvt"
 
 [tool.pyright]
```

### Comparing `twtvt-2023.4.15.post1/twtvt/cli/commands.py` & `twtvt-2023.4.15.post2/twtvt/cli/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from twtvt.utils import download_video
 
 cli_app = Typer()
 
 
 @cli_app.command()
 def twtvt(
-    target_links: list[str] = typer.Argument(..., help="Video tweet link or target user's likes or media."),
-    username: str = typer.Argument(..., help='Your twitter credentials username.'),
-    password: str = typer.Argument(..., help='Your twitter credentials password.'),
+    target_uris: list[str] = typer.Argument(..., help="Video tweet link, target user's likes or media, or file path."),
+    username: Optional[str] = typer.Option(None, help='Your twitter credentials username.'),
+    password: Optional[str] = typer.Option(None, help='Your twitter credentials password.'),
     cookies_from_browser: Optional[str] = typer.Option(None, help='Browser to get cookies from. '),
-    output: str = typer.Option('videos', help='Output path for downloaded videos.'),
+    output: str = typer.Option('.', help='Output path for downloaded videos.'),
     debug: bool = typer.Option(False, help='Enable debug mode. This disables headless mode of Browser.'),
     until_link: Optional[str] = typer.Option(
         None,
         help="Keeps finding videos until this link is found. None for no limit. Only for user's likes or media.",
     ),
 ):
     download_video(
-        target_links=target_links,
+        target_uris=target_uris,
         username=username,
         password=password,
         output=output,
         debug=debug,
         cookies_from_browser=cookies_from_browser,
         until_link=until_link,
     )
```

### Comparing `twtvt-2023.4.15.post1/twtvt/utils/monsnode_parser.py` & `twtvt-2023.4.15.post2/twtvt/utils/monsnode_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 
         video_name = self._parse_video_name(soup)
         link = self._parse_video_url(soup)
 
         return video_name, link
 
     def _parse_video_name(self, soup: BeautifulSoup) -> str:
-
         uploader_name = soup.select('body > div:nth-child(2) > div:nth-child(2) > div:nth-child(5) > b')[0].text
         title = soup.select('body > div:nth-child(2) > div:nth-child(2) > div:nth-child(2)')[0].text
         title = title.replace('/', '_')
         title = title.replace('\n', '')
         return f'{uploader_name} - {title}.mp4'
 
     def _parse_video_url(self, soup: BeautifulSoup) -> str:
-        video_path = typing.cast(str,
-                                 soup.select('body > div:nth-child(2) > div:nth-child(1) > a:nth-child(2)')[0]['href'])
+        video_path = typing.cast(
+            str,
+            soup.select('body > div:nth-child(2) > div:nth-child(1) > a:nth-child(2)')[0]['href'],
+        )
         return self.TARGET_URL + video_path
```

### Comparing `twtvt-2023.4.15.post1/twtvt/utils/twitter_parser.py` & `twtvt-2023.4.15.post2/twtvt/utils/twitter_parser.py`

 * *Files identical despite different names*

### Comparing `twtvt-2023.4.15.post1/PKG-INFO` & `twtvt-2023.4.15.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twtvt
-Version: 2023.4.15.post1
+Version: 2023.4.15.post2
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
```

