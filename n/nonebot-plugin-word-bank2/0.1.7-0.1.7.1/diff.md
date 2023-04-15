# Comparing `tmp/nonebot_plugin_word_bank2-0.1.7.tar.gz` & `tmp/nonebot_plugin_word_bank2-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_word_bank2-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_word_bank2-0.1.7.1.tar", max compression
```

## Comparing `nonebot_plugin_word_bank2-0.1.7.tar` & `nonebot_plugin_word_bank2-0.1.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/LICENSE
--rw-r--r--   0        0        0     3735 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/README.md
--rw-r--r--   0        0        0     8904 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/__init__.py
--rw-r--r--   0        0        0     9334 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/data_source.py
--rw-r--r--   0        0        0      225 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/models.py
--rw-r--r--   0        0        0     4438 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/util.py
--rw-r--r--   0        0        0     2303 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/word_entry.py
--rw-r--r--   0        0        0      543 2023-04-15 12:38:29.896196 nonebot_plugin_word_bank2-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4501 1970-01-01 00:00:00.000000 nonebot_plugin_word_bank2-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/LICENSE
+-rw-r--r--   0        0        0     3735 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/README.md
+-rw-r--r--   0        0        0     8904 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/__init__.py
+-rw-r--r--   0        0        0     9334 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/data_source.py
+-rw-r--r--   0        0        0      225 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/models.py
+-rw-r--r--   0        0        0     4438 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/util.py
+-rw-r--r--   0        0        0     2303 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/word_entry.py
+-rw-r--r--   0        0        0      547 2023-04-15 12:39:44.470098 nonebot_plugin_word_bank2-0.1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 nonebot_plugin_word_bank2-0.1.7.1/PKG-INFO
```

### Comparing `nonebot_plugin_word_bank2-0.1.7/LICENSE` & `nonebot_plugin_word_bank2-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7/README.md` & `nonebot_plugin_word_bank2-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/__init__.py` & `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/data_source.py` & `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/util.py` & `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7/nonebot_plugin_word_bank2/word_entry.py` & `nonebot_plugin_word_bank2-0.1.7.1/nonebot_plugin_word_bank2/word_entry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_word_bank2-0.1.7/pyproject.toml` & `nonebot_plugin_word_bank2-0.1.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 authors = ["kexue <x@kexue.io>"]
 description = "无数据问答插件"
 homepage = "https://github.com/kexue-z/nonebot-plugin-word-bank2"
 license = "GPL-3.0"
 name = "nonebot-plugin-word-bank2"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.7.1"
 
 [tool.poetry.dependencies]
 httpx = ">=0.18.0,<1.0.0"
-nonebot-adapter-onebot = "^2.0.0-beta.1"
-nonebot2 = "^2.0.0-beta.4"
+nonebot-adapter-onebot = ">=2.0.0-beta.1"
+nonebot2 = ">=2.0.0-beta.4"
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 flake8 = "^4.0.1"
 
 [build-system]
```

### Comparing `nonebot_plugin_word_bank2-0.1.7/PKG-INFO` & `nonebot_plugin_word_bank2-0.1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-word-bank2
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: 无数据问答插件
 Home-page: https://github.com/kexue-z/nonebot-plugin-word-bank2
 License: GPL-3.0
 Author: kexue
 Author-email: x@kexue.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.18.0,<1.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1)
+Requires-Dist: nonebot2 (>=2.0.0-beta.4)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # nonebot-plugin-word-bank2
 
 _✨ 无数据库的轻量问答插件 ✨_
```

