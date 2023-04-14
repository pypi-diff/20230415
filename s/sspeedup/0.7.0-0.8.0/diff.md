# Comparing `tmp/sspeedup-0.7.0.tar.gz` & `tmp/sspeedup-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspeedup-0.7.0.tar", max compression
+gzip compressed data, was "sspeedup-0.8.0.tar", max compression
```

## Comparing `sspeedup-0.7.0.tar` & `sspeedup-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.7.0/LICENSE
--rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.7.0/README.md
--rw-r--r--   0        0        0     1338 2023-04-14 22:27:40.256275 sspeedup-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      552 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/ability/exceptions.py
--rw-r--r--   0        0        0     2031 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/ability/word_split/_base.py
--rw-r--r--   0        0        0     7633 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/ability/word_split/jieba.py
--rw-r--r--   0        0        0     2311 2023-04-14 22:08:58.626733 sspeedup-0.7.0/sspeedup/api.py
--rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.7.0/sspeedup/cache/timeout.py
--rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.7.0/sspeedup/colorful_print.py
--rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.7.0/sspeedup/dict_helper.py
--rw-r--r--   0        0        0    12985 2023-04-14 22:09:36.418433 sspeedup-0.7.0/sspeedup/logging/run_logger.py
--rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.7.0/sspeedup/make_qrcode.py
--rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.7.0/sspeedup/pywebio/callbacks.py
--rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/require.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.7.0/sspeedup/retry/__init__.py
--rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/retry/deco.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.7.0/sspeedup/retry/event.py
--rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/retry/policy.py
--rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/time_helper.py
--rw-r--r--   0        0        0     2202 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/word_split/_base.py
--rw-r--r--   0        0        0     4363 2023-04-14 22:27:40.259608 sspeedup-0.7.0/sspeedup/word_split/jieba.py
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 sspeedup-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.8.0/LICENSE
+-rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.8.0/README.md
+-rw-r--r--   0        0        0     1337 2023-04-14 23:08:51.965326 sspeedup-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      552 2023-04-14 22:27:40.256275 sspeedup-0.8.0/sspeedup/ability/exceptions.py
+-rw-r--r--   0        0        0     2031 2023-04-14 22:27:40.256275 sspeedup-0.8.0/sspeedup/ability/word_split/_base.py
+-rw-r--r--   0        0        0     7639 2023-04-14 23:07:38.449428 sspeedup-0.8.0/sspeedup/ability/word_split/jieba.py
+-rw-r--r--   0        0        0     2311 2023-04-14 22:08:58.626733 sspeedup-0.8.0/sspeedup/api.py
+-rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.8.0/sspeedup/cache/timeout.py
+-rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.8.0/sspeedup/colorful_print.py
+-rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.8.0/sspeedup/dict_helper.py
+-rw-r--r--   0        0        0    12985 2023-04-14 22:09:36.418433 sspeedup-0.8.0/sspeedup/logging/run_logger.py
+-rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.8.0/sspeedup/make_qrcode.py
+-rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.8.0/sspeedup/pywebio/callbacks.py
+-rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/require.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.8.0/sspeedup/retry/__init__.py
+-rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/retry/deco.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.8.0/sspeedup/retry/event.py
+-rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/retry/policy.py
+-rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.8.0/sspeedup/time_helper.py
+-rw-r--r--   0        0        0     2202 2023-04-14 22:27:40.256275 sspeedup-0.8.0/sspeedup/word_split/_base.py
+-rw-r--r--   0        0        0     4363 2023-04-14 22:27:40.259608 sspeedup-0.8.0/sspeedup/word_split/jieba.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 sspeedup-0.8.0/PKG-INFO
```

### Comparing `sspeedup-0.7.0/LICENSE` & `sspeedup-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/pyproject.toml` & `sspeedup-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sspeedup"
-version = "0.7.0"
+version = "0.8.0"
 description = "开发工具箱"
 authors = ["yezi <yehaowei20060411@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FHU-yezi/sspeedup"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -29,15 +29,15 @@
 
 [tool.poetry.extras]
 logging = ["pymongo"]
 word-split-jieba = ["jieba"]
 qrcode = ["qrcode"]
 pywebio = ["pywebio"]
 api-response-sanic = ["sanic"]
-anbility-word-split = ["httpx"]
+ability-word-split = ["httpx"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `sspeedup-0.7.0/sspeedup/ability/exceptions.py` & `sspeedup-0.8.0/sspeedup/ability/exceptions.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/ability/word_split/_base.py` & `sspeedup-0.8.0/sspeedup/ability/word_split/_base.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/ability/word_split/jieba.py` & `sspeedup-0.8.0/sspeedup/ability/word_split/jieba.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from sspeedup.ability.exceptions import AbilityCallHTTPError, AbilityCallServiceError
 from sspeedup.ability.word_split._base import AbilitySplitter
 
 HTTPX_CLIENT = Client(timeout=20)
 
 
-class AbilityJiebaSplitter(AbilitySplitter):
+class AbilityJiebaSplitterV1(AbilitySplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
         self.stopwords = word_list_to_add
 
@@ -81,15 +81,15 @@
             {
                 key: value
                 for key, value in response_json["data"]["word_freq"].items()
                 if key not in self.stopwords
             }
         )
 
-class AbilityJiebaSearchSplitter(AbilitySplitter):
+class AbilityJiebaSearchSplitterV1(AbilitySplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
         self.stopwords = word_list_to_add
 
@@ -157,15 +157,15 @@
             {
                 key: value
                 for key, value in response_json["data"]["word_freq"].items()
                 if key not in self.stopwords
             }
         )
 
-class AbilityJiebaPossegSplitter(AbilitySplitter):
+class AbilityJiebaPossegSplitterV1(AbilitySplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
         self.stopwords = word_list_to_add
```

### Comparing `sspeedup-0.7.0/sspeedup/api.py` & `sspeedup-0.8.0/sspeedup/api.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/cache/timeout.py` & `sspeedup-0.8.0/sspeedup/cache/timeout.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/colorful_print.py` & `sspeedup-0.8.0/sspeedup/colorful_print.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/logging/run_logger.py` & `sspeedup-0.8.0/sspeedup/logging/run_logger.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/make_qrcode.py` & `sspeedup-0.8.0/sspeedup/make_qrcode.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/pywebio/callbacks.py` & `sspeedup-0.8.0/sspeedup/pywebio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/retry/deco.py` & `sspeedup-0.8.0/sspeedup/retry/deco.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/retry/policy.py` & `sspeedup-0.8.0/sspeedup/retry/policy.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/time_helper.py` & `sspeedup-0.8.0/sspeedup/time_helper.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/word_split/_base.py` & `sspeedup-0.8.0/sspeedup/word_split/_base.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/sspeedup/word_split/jieba.py` & `sspeedup-0.8.0/sspeedup/word_split/jieba.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.7.0/PKG-INFO` & `sspeedup-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspeedup
-Version: 0.7.0
+Version: 0.8.0
 Summary: 开发工具箱
 Home-page: https://github.com/FHU-yezi/sspeedup
 License: MIT
 Author: yezi
 Author-email: yehaowei20060411@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,21 +12,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Provides-Extra: anbility-word-split
+Provides-Extra: ability-word-split
 Provides-Extra: api-response-sanic
 Provides-Extra: logging
 Provides-Extra: pywebio
 Provides-Extra: qrcode
 Provides-Extra: word-split-jieba
-Requires-Dist: httpx (>=0.24.0,<0.25.0) ; extra == "anbility-word-split"
+Requires-Dist: httpx (>=0.24.0,<0.25.0) ; extra == "ability-word-split"
 Requires-Dist: jieba (>=0.42.1,<0.43.0) ; extra == "word-split-jieba"
 Requires-Dist: pymongo (>=4.3.3,<5.0.0) ; extra == "logging"
 Requires-Dist: pywebio (>=1.7.1,<2.0.0) ; extra == "pywebio"
 Requires-Dist: qrcode (>=7.4.2,<8.0.0) ; extra == "qrcode"
 Requires-Dist: sanic (>=23.3.0,<24.0.0) ; extra == "api-response-sanic"
 Project-URL: Repository, https://github.com/FHU-yezi/sspeedup
 Description-Content-Type: text/markdown
```

