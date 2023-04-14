# Comparing `tmp/sspeedup-0.6.0.tar.gz` & `tmp/sspeedup-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspeedup-0.6.0.tar", max compression
+gzip compressed data, was "sspeedup-0.7.0.tar", max compression
```

## Comparing `sspeedup-0.6.0.tar` & `sspeedup-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.6.0/LICENSE
--rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.6.0/README.md
--rw-r--r--   0        0        0     1257 2023-04-08 23:07:04.719413 sspeedup-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2311 2023-04-08 23:07:04.719413 sspeedup-0.6.0/sspeedup/api.py
--rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.6.0/sspeedup/cache/timeout.py
--rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.6.0/sspeedup/colorful_print.py
--rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.6.0/sspeedup/dict_helper.py
--rw-r--r--   0        0        0    12985 2023-03-17 09:06:31.863741 sspeedup-0.6.0/sspeedup/logging/run_logger.py
--rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.6.0/sspeedup/make_qrcode.py
--rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.6.0/sspeedup/pywebio/callbacks.py
--rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/require.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.6.0/sspeedup/retry/__init__.py
--rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/retry/deco.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.6.0/sspeedup/retry/event.py
--rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/retry/policy.py
--rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/time_helper.py
--rw-r--r--   0        0        0     2332 2023-02-28 22:37:56.103296 sspeedup-0.6.0/sspeedup/word_split/_base.py
--rw-r--r--   0        0        0     5155 2023-02-28 22:37:56.109963 sspeedup-0.6.0/sspeedup/word_split/jieba.py
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 sspeedup-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.7.0/LICENSE
+-rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.7.0/README.md
+-rw-r--r--   0        0        0     1338 2023-04-14 22:27:40.256275 sspeedup-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      552 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/ability/exceptions.py
+-rw-r--r--   0        0        0     2031 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/ability/word_split/_base.py
+-rw-r--r--   0        0        0     7633 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/ability/word_split/jieba.py
+-rw-r--r--   0        0        0     2311 2023-04-14 22:08:58.626733 sspeedup-0.7.0/sspeedup/api.py
+-rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.7.0/sspeedup/cache/timeout.py
+-rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.7.0/sspeedup/colorful_print.py
+-rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.7.0/sspeedup/dict_helper.py
+-rw-r--r--   0        0        0    12985 2023-04-14 22:09:36.418433 sspeedup-0.7.0/sspeedup/logging/run_logger.py
+-rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.7.0/sspeedup/make_qrcode.py
+-rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.7.0/sspeedup/pywebio/callbacks.py
+-rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/require.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.7.0/sspeedup/retry/__init__.py
+-rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/retry/deco.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.7.0/sspeedup/retry/event.py
+-rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/retry/policy.py
+-rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.7.0/sspeedup/time_helper.py
+-rw-r--r--   0        0        0     2202 2023-04-14 22:27:40.256275 sspeedup-0.7.0/sspeedup/word_split/_base.py
+-rw-r--r--   0        0        0     4363 2023-04-14 22:27:40.259608 sspeedup-0.7.0/sspeedup/word_split/jieba.py
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 sspeedup-0.7.0/PKG-INFO
```

### Comparing `sspeedup-0.6.0/LICENSE` & `sspeedup-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/pyproject.toml` & `sspeedup-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sspeedup"
-version = "0.6.0"
+version = "0.7.0"
 description = "开发工具箱"
 authors = ["yezi <yehaowei20060411@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FHU-yezi/sspeedup"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -16,26 +16,28 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pymongo = { version = "^4.3.3", optional = true }
 jieba = { version = "^0.42.1", optional = true }
 qrcode = { version = "^7.4.2", optional = true }
 pywebio = { version = "^1.7.1", optional = true }
 sanic = { version = "^23.3.0", optional = true }
+httpx = { version = "^0.24.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.260"
 pyright = "^1.1.293"
 black = "^23.1.0"
 
 [tool.poetry.extras]
 logging = ["pymongo"]
 word-split-jieba = ["jieba"]
 qrcode = ["qrcode"]
 pywebio = ["pywebio"]
 api-response-sanic = ["sanic"]
+anbility-word-split = ["httpx"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `sspeedup-0.6.0/sspeedup/api.py` & `sspeedup-0.7.0/sspeedup/api.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/cache/timeout.py` & `sspeedup-0.7.0/sspeedup/cache/timeout.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/colorful_print.py` & `sspeedup-0.7.0/sspeedup/colorful_print.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/logging/run_logger.py` & `sspeedup-0.7.0/sspeedup/logging/run_logger.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/make_qrcode.py` & `sspeedup-0.7.0/sspeedup/make_qrcode.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/pywebio/callbacks.py` & `sspeedup-0.7.0/sspeedup/pywebio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/retry/deco.py` & `sspeedup-0.7.0/sspeedup/retry/deco.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/retry/policy.py` & `sspeedup-0.7.0/sspeedup/retry/policy.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/time_helper.py` & `sspeedup-0.7.0/sspeedup/time_helper.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.6.0/sspeedup/word_split/_base.py` & `sspeedup-0.7.0/sspeedup/word_split/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,20 +55,17 @@
     def add_hotwords_file(self, file_name: str) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def set_allowed_word_types_file(self, file_name: str) -> None:
         raise NotImplementedError
 
-    def _get_stopwords_need_to_process(self, word_list: Set[str]) -> Set[str]:
-        return word_list - self.stopwords
-
     def _get_hotwords_need_to_process(self, word_list: Set[str]) -> Set[str]:
         return word_list - self.hotwords
 
     @abstractmethod
-    def split(self, sentence: str) -> Generator[str, None, None]:
+    def split(self, text: str) -> Generator[str, None, None]:
         raise NotImplementedError
 
     @abstractmethod
-    def get_word_freq(self, sentence: str) -> Counter:
+    def get_word_freq(self, text: str) -> Counter:
         raise NotImplementedError
```

### Comparing `sspeedup-0.6.0/sspeedup/word_split/jieba.py` & `sspeedup-0.7.0/sspeedup/word_split/jieba.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,140 +11,125 @@
 
 
 class JiebaSplitter(WordSplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
-        word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
-        self.stopwords = self.stopwords.union(word_list_to_add)
+        self.stopwords = word_list
 
     def add_hotwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_hotwords_need_to_process(word_list)
         for word in word_list_to_add:
             add_word(word)
 
         self.hotwords = self.hotwords.union(word_list_to_add)
 
     def add_stopwords_file(self, file_name: str) -> None:
         with open(file_name, encoding="utf-8") as f:
-            word_list_to_add = self._get_stopwords_need_to_process(
-                {x.strip() for x in f.readlines()},
-            )
-
-        self.stopwords = self.stopwords.union(word_list_to_add)
+            self.stopwords = {x.strip() for x in f.readlines()}
 
     def set_allowed_word_type(self, types: Set[str]) -> None:
         del types
         raise NotImplementedError
 
     def add_hotwords_file(self, file_name: str) -> None:
         load_userdict(file_name)
 
     def set_allowed_word_types_file(self, file_name: str) -> None:
         del file_name
         raise NotImplementedError
 
-    def split(self, sentence: str) -> Generator[str, None, None]:
-        for word in cut(sentence):
+    def split(self, text: str) -> Generator[str, None, None]:
+        for word in cut(text):
             if word in self.stopwords:
                 continue
 
             yield word
 
-    def get_word_freq(self, sentence: str) -> Counter:
-        return Counter(x for x in cut(sentence) if x not in self.stopwords)
+    def get_word_freq(self, text: str) -> Counter:
+        return Counter(x for x in cut(text) if x not in self.stopwords)
 
 
 class JiebaSearchSplitter(WordSplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
-        word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
-        self.stopwords = self.stopwords.union(word_list_to_add)
+        self.stopwords = word_list
 
     def add_hotwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_hotwords_need_to_process(word_list)
         for word in word_list_to_add:
             add_word(word)
 
         self.hotwords = self.hotwords.union(word_list_to_add)
 
     def set_allowed_word_type(self, types_list: Set[str]) -> None:
         del types_list
         raise NotImplementedError
 
     def add_stopwords_file(self, file_name: str) -> None:
         with open(file_name, encoding="utf-8") as f:
-            word_list_to_add = self._get_stopwords_need_to_process(
-                {x.strip() for x in f.readlines()},
-            )
-
-        self.stopwords = self.stopwords.union(word_list_to_add)
+            self.stopwords = {x.strip() for x in f.readlines()}
 
     def add_hotwords_file(self, file_name: str) -> None:
         load_userdict(file_name)
 
     def set_allowed_word_types_file(self, file_name: str) -> None:
         del file_name
         raise NotImplementedError
 
-    def split(self, sentence: str) -> Generator[str, None, None]:
-        for word in cut_for_search(sentence):
+    def split(self, text: str) -> Generator[str, None, None]:
+        for word in cut_for_search(text):
             if word in self.stopwords:
                 continue
 
             yield word
 
-    def get_word_freq(self, sentence: str) -> Counter:
-        return Counter(x for x in cut_for_search(sentence) if x not in self.stopwords)
+    def get_word_freq(self, text: str) -> Counter:
+        return Counter(x for x in cut_for_search(text) if x not in self.stopwords)
 
 
 class JiebaPossegSplitter(WordSplitter):
     def init(self) -> None:
         pass
 
     def add_stopwords(self, word_list: Set[str]) -> None:
-        word_list_to_add: Set[str] = self._get_stopwords_need_to_process(word_list)
-        self.stopwords = self.stopwords.union(word_list_to_add)
+        self.stopwords = word_list
 
     def add_hotwords(self, word_list: Set[str]) -> None:
         word_list_to_add: Set[str] = self._get_hotwords_need_to_process(word_list)
         for word in word_list_to_add:
             add_word(word)
 
         self.hotwords = self.hotwords.union(word_list_to_add)
 
     def set_allowed_word_type(self, types: Set[str]) -> None:
         self.allowed_word_types = types
 
     def add_stopwords_file(self, file_name: str) -> None:
         with open(file_name, encoding="utf-8") as f:
-            word_list_to_add = self._get_stopwords_need_to_process(
-                {x.strip() for x in f.readlines()},
-            )
-
-        self.stopwords = self.stopwords.union(word_list_to_add)
+            self.stopwords = {x.strip() for x in f.readlines()}
 
     def add_hotwords_file(self, file_name: str) -> None:
         load_userdict(file_name)
 
     def set_allowed_word_types_file(self, file_name: str) -> None:
         with open(file_name, encoding="utf-8") as f:
             self.allowed_word_types = {x.strip() for x in f.readlines()}
 
-    def split(self, sentence: str) -> Generator[str, None, None]:
-        for pair in cut_poseg(sentence):
+    def split(self, text: str) -> Generator[str, None, None]:
+        for pair in cut_poseg(text):
             if pair.flag not in self.allowed_word_types:
                 continue
             if pair.word in self.stopwords:
                 continue
 
             yield pair.word
 
-    def get_word_freq(self, sentence: str) -> Counter:
+    def get_word_freq(self, text: str) -> Counter:
         return Counter(
             pair.word
-            for pair in cut_poseg(sentence)
+            for pair in cut_poseg(text)
             if pair.flag in self.allowed_word_types and pair.word not in self.stopwords
         )
```

### Comparing `sspeedup-0.6.0/PKG-INFO` & `sspeedup-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspeedup
-Version: 0.6.0
+Version: 0.7.0
 Summary: 开发工具箱
 Home-page: https://github.com/FHU-yezi/sspeedup
 License: MIT
 Author: yezi
 Author-email: yehaowei20060411@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,19 +12,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
+Provides-Extra: anbility-word-split
 Provides-Extra: api-response-sanic
 Provides-Extra: logging
 Provides-Extra: pywebio
 Provides-Extra: qrcode
 Provides-Extra: word-split-jieba
+Requires-Dist: httpx (>=0.24.0,<0.25.0) ; extra == "anbility-word-split"
 Requires-Dist: jieba (>=0.42.1,<0.43.0) ; extra == "word-split-jieba"
 Requires-Dist: pymongo (>=4.3.3,<5.0.0) ; extra == "logging"
 Requires-Dist: pywebio (>=1.7.1,<2.0.0) ; extra == "pywebio"
 Requires-Dist: qrcode (>=7.4.2,<8.0.0) ; extra == "qrcode"
 Requires-Dist: sanic (>=23.3.0,<24.0.0) ; extra == "api-response-sanic"
 Project-URL: Repository, https://github.com/FHU-yezi/sspeedup
 Description-Content-Type: text/markdown
```

