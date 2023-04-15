# Comparing `tmp/revchatgptauth-2023.4.14.tar.gz` & `tmp/revchatgptauth-2023.4.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revchatgptauth-2023.4.14.tar", max compression
+gzip compressed data, was "revchatgptauth-2023.4.16.tar", max compression
```

## Comparing `revchatgptauth-2023.4.14.tar` & `revchatgptauth-2023.4.16.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1208 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/README.md
--rw-r--r--   0        0        0     1326 2023-04-13 06:25:54.753340 revchatgptauth-2023.4.14/pyproject.toml
--rw-r--r--   0        0        0      247 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/__init__.py
--rw-r--r--   0        0        0     1056 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/chatgpt_access_token_parser.py
--rw-r--r--   0        0        0     1561 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/openai_cookie_parser.py
--rw-r--r--   0        0        0        0 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/test/__init__.py
--rw-r--r--   0        0        0     1989 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/test/test_chatgpt_access_token_parser.py
--rw-r--r--   0        0        0     3124 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/test/test_openai_cookie_parser.py
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 revchatgptauth-2023.4.14/PKG-INFO
+-rw-r--r--   0        0        0     1208 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/README.md
+-rw-r--r--   0        0        0     1334 2023-04-15 15:13:18.688474 revchatgptauth-2023.4.16/pyproject.toml
+-rw-r--r--   0        0        0      421 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/__init__.py
+-rw-r--r--   0        0        0     1245 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/chatgpt_access_token_parser.py
+-rw-r--r--   0        0        0     1441 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/openai_cookie_parser.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/py.typed
+-rw-r--r--   0        0        0      308 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/supported_browser.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/test/__init__.py
+-rw-r--r--   0        0        0     2066 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/test/test_chatgpt_access_token_parser.py
+-rw-r--r--   0        0        0     3052 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/test/test_openai_cookie_parser.py
+-rw-r--r--   0        0        0     1357 2023-04-15 15:12:57.428270 revchatgptauth-2023.4.16/revChatGPTAuth/utils.py
+-rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 revchatgptauth-2023.4.16/PKG-INFO
```

### Comparing `revchatgptauth-2023.4.14/README.md` & `revchatgptauth-2023.4.16/README.md`

 * *Files identical despite different names*

### Comparing `revchatgptauth-2023.4.14/pyproject.toml` & `revchatgptauth-2023.4.16/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "revChatGPTAuth"
-version = "2023.04.14"
+version = "v2023.04.16"
 description = ""
 authors = []
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "revChatGPTAuth"
 
 [tool.pyright]
@@ -34,16 +34,16 @@
 [tool.ruff]
 line-length = 119
 select = [ "PLE", "PLW", "E", "W", "F", "I", "Q", "B",]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 poetry = "^1.4.2"
-yt-dlp = "^2023.3.4"
 httpx = "^0.24.0"
+browser-cookie3 = "^0.17.1"
 
 [tool.pyright.defineConstant]
 DEBUG = true
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 docstring-quotes = "single"
```

### Comparing `revchatgptauth-2023.4.14/revChatGPTAuth/chatgpt_access_token_parser.py` & `revchatgptauth-2023.4.16/revChatGPTAuth/chatgpt_access_token_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+from typing import Union
+
 import httpx
 
+from revChatGPTAuth.supported_browser import SupportedBrowser
+
 from .openai_cookie_parser import OpenAICookieParser
 
 
 class ChatGPTAccessTokenParser:
 
-    def __init__(self, browser_name: str):
+    def __init__(self, browser_name: SupportedBrowser):
         self.openai_cookie_parser = OpenAICookieParser(browser_name)
 
-    def get_openai_chatgpt_access_token(self) -> str:
+    def get_access_token(self) -> str:
         cookie = self._get_stringified_cookies()
         response = self._auth_openai(cookie)
         response.raise_for_status()
         return response.json()['accessToken']
 
     def _get_stringified_cookies(self) -> str:
         cookies = self.openai_cookie_parser.parse_cookie()
@@ -21,10 +25,12 @@
     def _auth_openai(self, cookie: str) -> httpx.Response:
         URL = 'https://chat.openai.com/api/auth/session'
         headers = {'cookie': cookie}
         response = httpx.get(URL, headers=headers)
         return response
 
 
-def get_access_token(browser_name: str) -> str:
+def get_access_token(browser_name: Union[str, SupportedBrowser]) -> str:
+    if isinstance(browser_name, str):
+        browser_name = SupportedBrowser(browser_name)
     chatgpt_access_token_parser = ChatGPTAccessTokenParser(browser_name)
-    return chatgpt_access_token_parser.get_openai_chatgpt_access_token()
+    return chatgpt_access_token_parser.get_access_token()
```

### Comparing `revchatgptauth-2023.4.14/revChatGPTAuth/openai_cookie_parser.py` & `revchatgptauth-2023.4.16/revChatGPTAuth/openai_cookie_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from http.cookiejar import Cookie
 from typing import Any, Optional
 
-from yt_dlp.cookies import SUPPORTED_BROWSERS, extract_cookies_from_browser
-from yt_dlp.utils import YoutubeDLCookieJar
+from revChatGPTAuth.supported_browser import SupportedBrowser
+from revChatGPTAuth.utils import load_cookies
 
 
 class OpenAICookieParser:
 
-    def __init__(self, browser_name: str):
-        if browser_name not in SUPPORTED_BROWSERS:
-            raise ValueError(f'Browser {browser_name} is not supported. Supported browsers are: {SUPPORTED_BROWSERS}')
+    SUPPORTED_BROWSERS: list[str] = [browser.value for browser in SupportedBrowser]
+
+    def __init__(self, browser_name: SupportedBrowser):
         self.BROWSER_NAME = browser_name
 
     def parse_cookie(self):
-        all_cookies: YoutubeDLCookieJar = extract_cookies_from_browser(self.BROWSER_NAME)
+        all_cookies = load_cookies(self.BROWSER_NAME)
         openai_cookies = self._get_openai_cookies(all_cookies.__dict__)
         openai_cookies_dict: dict[str, Optional[str]] = {key: cookie.value for key, cookie in openai_cookies.items()}
         return openai_cookies_dict
 
     def _get_openai_cookies(self, all_cookies_dict: dict[str, Any]):
         try:
             chat_openai_cookies: dict[str, Cookie] = all_cookies_dict['_cookies']['chat.openai.com']['/']
```

### Comparing `revchatgptauth-2023.4.14/revChatGPTAuth/test/test_chatgpt_access_token_parser.py` & `revchatgptauth-2023.4.16/revChatGPTAuth/test/test_chatgpt_access_token_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest.mock import MagicMock, patch
 
 from revChatGPTAuth.chatgpt_access_token_parser import ChatGPTAccessTokenParser, get_access_token
+from revChatGPTAuth.supported_browser import SupportedBrowser
 
 
 class TestChatGPTAccessTokenParser:
 
     @patch('revChatGPTAuth.chatgpt_access_token_parser.OpenAICookieParser')
     @patch('httpx.get')
     def test_get_openai_chatgpt_access_token(
@@ -20,18 +21,18 @@
 
         ## mock access token response
         expected_access_token = 'access_token'
         mock_response = MagicMock()
         mock_response.json.return_value = {'accessToken': expected_access_token}
         mock_httpx_get.return_value = mock_response
 
-        chatgpt_access_token_parser = ChatGPTAccessTokenParser('chrome')
+        chatgpt_access_token_parser = ChatGPTAccessTokenParser(SupportedBrowser.CHROME)
 
         # when
-        access_token = chatgpt_access_token_parser.get_openai_chatgpt_access_token()
+        access_token = chatgpt_access_token_parser.get_access_token()
 
         # then
         mock_cookie_parser.parse_cookie.assert_called_once()
         mock_httpx_get.assert_called_once_with(
             'https://chat.openai.com/api/auth/session',
             headers={'cookie': 'cookie_key=cookie_value'},
         )
@@ -39,15 +40,15 @@
         assert access_token == expected_access_token
 
 
 @patch('revChatGPTAuth.chatgpt_access_token_parser.ChatGPTAccessTokenParser')
 def test_get_access_token(mock_chatgpt_access_token_parser: MagicMock) -> None:
     # given
     expected_access_token = 'access_token'
-    mock_chatgpt_access_token_parser.return_value.get_openai_chatgpt_access_token.return_value = expected_access_token
+    mock_chatgpt_access_token_parser.return_value.get_access_token.return_value = expected_access_token
 
     # when
-    access_token = get_access_token('chrome')
+    access_token = get_access_token(SupportedBrowser.CHROME)
 
     # then
-    mock_chatgpt_access_token_parser.assert_called_once_with('chrome')
+    mock_chatgpt_access_token_parser.assert_called_once_with(SupportedBrowser.CHROME)
     assert access_token == expected_access_token
```

### Comparing `revchatgptauth-2023.4.14/revChatGPTAuth/test/test_openai_cookie_parser.py` & `revchatgptauth-2023.4.16/revChatGPTAuth/test/test_openai_cookie_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-from http.cookiejar import Cookie
+from http.cookiejar import Cookie, CookieJar
 from unittest.mock import MagicMock, patch
 
 import pytest
-from yt_dlp.cookies import SUPPORTED_BROWSERS
-from yt_dlp.utils import YoutubeDLCookieJar
 
 from revChatGPTAuth.openai_cookie_parser import OpenAICookieParser
+from revChatGPTAuth.supported_browser import SupportedBrowser
 
 
 class TestOpenAICookieParser:
-
-    def test_init_with_unsupported_browser(self):
-        with pytest.raises(ValueError):
-            OpenAICookieParser(browser_name='Internet Explorer Holy Shit')
+    SUPPORTED_BROWSERS = [SupportedBrowser(browser_name) for browser_name in OpenAICookieParser.SUPPORTED_BROWSERS]
 
     @pytest.mark.parametrize('supported_browser', SUPPORTED_BROWSERS)
-    def test_init_with_supported_browser(self, supported_browser: str):
+    def test_init_with_supported_browser(self, supported_browser: SupportedBrowser):
         parser = OpenAICookieParser(browser_name=supported_browser)
         assert parser.BROWSER_NAME == supported_browser
 
     @pytest.mark.parametrize('supported_browser', SUPPORTED_BROWSERS)
-    @patch('revChatGPTAuth.openai_cookie_parser.extract_cookies_from_browser')
+    @patch('revChatGPTAuth.openai_cookie_parser.load_cookies')
     def test_parse_cookie_with_supported_browser(
         self,
-        mock_extract_cookies: MagicMock,
-        supported_browser: str,
+        mock_load_cookies: MagicMock,
+        supported_browser: SupportedBrowser,
     ):
         # given
-        cookie_jar = YoutubeDLCookieJar()
+        cookie_jar = CookieJar()
         cookie_jar.set_cookie(
             Cookie(
                 version=0,
                 name='cookie1',
                 value='value1',
                 port=None,
                 port_specified=False,
@@ -81,15 +77,15 @@
                 secure=False,
                 expires=None,
                 discard=True,
                 comment=None,
                 comment_url=None,
                 rest={},
             ))
-        mock_extract_cookies.return_value = cookie_jar
+        mock_load_cookies.return_value = cookie_jar
         parser = OpenAICookieParser(browser_name=supported_browser)
 
         # when
         openai_cookies = parser.parse_cookie()
 
         # then
         assert openai_cookies == {'cookie1': 'value1', 'cookie2': 'value2', 'cookie3': 'value3'}
```

### Comparing `revchatgptauth-2023.4.14/PKG-INFO` & `revchatgptauth-2023.4.16/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: revchatgptauth
-Version: 2023.4.14
+Version: 2023.4.16
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: browser-cookie3 (>=0.17.1,<0.18.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: poetry (>=1.4.2,<2.0.0)
-Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # revChatGPTAuth
 
 Authenticate using your browser's cookies - no need to inconveniently copy and paste from your browser!
 
 ## Getting Started
```

