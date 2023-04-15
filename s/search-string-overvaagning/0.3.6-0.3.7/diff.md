# Comparing `tmp/search_string_overvaagning-0.3.6-py3-none-any.whl.zip` & `tmp/search_string_overvaagning-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16358 bytes, number of entries: 11
--rw-r--r--  2.0 unx      239 b- defN 23-Apr-08 11:27 search_string/__init__.py
--rw-r--r--  2.0 unx      385 b- defN 23-Apr-08 11:27 search_string/constants.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-08 11:27 search_string/py.typed
--rw-r--r--  2.0 unx    21846 b- defN 23-Apr-08 11:27 search_string/search_string.py
--rw-r--r--  2.0 unx    12201 b- defN 23-Apr-08 11:27 search_string/search_string_collection.py
--rw-r--r--  2.0 unx       58 b- defN 23-Apr-08 11:27 search_string/version.py
--rw-r--r--  2.0 unx     4074 b- defN 23-Apr-08 11:27 search_string_overvaagning-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    10197 b- defN 23-Apr-08 11:27 search_string_overvaagning-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 11:27 search_string_overvaagning-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-08 11:27 search_string_overvaagning-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      987 b- defN 23-Apr-08 11:27 search_string_overvaagning-0.3.6.dist-info/RECORD
-11 files, 50093 bytes uncompressed, 14656 bytes compressed:  70.7%
+Zip file size: 16383 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      239 b- defN 23-Apr-15 05:59 search_string/__init__.py
+-rw-r--r--  2.0 unx      385 b- defN 23-Apr-15 05:59 search_string/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-15 05:59 search_string/py.typed
+-rw-r--r--  2.0 unx    21840 b- defN 23-Apr-15 05:59 search_string/search_string.py
+-rw-r--r--  2.0 unx    12295 b- defN 23-Apr-15 05:59 search_string/search_string_collection.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Apr-15 05:59 search_string/version.py
+-rw-r--r--  2.0 unx     4074 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10296 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      987 b- defN 23-Apr-15 06:00 search_string_overvaagning-0.3.7.dist-info/RECORD
+11 files, 50280 bytes uncompressed, 14681 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: search_string/search_string_collection.py
 Comment: 
 
 Filename: search_string/version.py
 Comment: 
 
-Filename: search_string_overvaagning-0.3.6.dist-info/LICENSE
+Filename: search_string_overvaagning-0.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: search_string_overvaagning-0.3.6.dist-info/METADATA
+Filename: search_string_overvaagning-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: search_string_overvaagning-0.3.6.dist-info/WHEEL
+Filename: search_string_overvaagning-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: search_string_overvaagning-0.3.6.dist-info/top_level.txt
+Filename: search_string_overvaagning-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: search_string_overvaagning-0.3.6.dist-info/RECORD
+Filename: search_string_overvaagning-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## search_string/search_string.py

```diff
@@ -225,15 +225,15 @@
                 f'Search strings must be strings, but received value {string} '
                 + f'of type {type(string)} for SS.data={self.data}',
             )
 
         is_global = False
         cleaned = string.strip(' ;').lower()
         if cleaned.endswith(const.GLOBAL):
-            cleaned = cleaned.removesuffix(const.GLOBAL)
+            cleaned = cleaned[:-len(const.GLOBAL)]
             is_global = True
 
         final_str = cleaned.rstrip(';')
         if not final_str:
             return None, is_global
 
         parts = final_str.split(';')
```

## search_string/search_string_collection.py

```diff
@@ -125,15 +125,19 @@
             sentence = sentences[sentence_index]
             matched_sentences.append(sentence[:const.MAX_SENTENCE_CHARS])
             last_idx = sentence_index
 
         return matched_sentences
 
     def _split_part(self, part: str) -> list[str]:
-        cleaned = part.strip(' ;').removesuffix(const.GLOBAL).strip(' ;')
+        cleaned = part.strip(' ;')
+        if cleaned.endswith(const.GLOBAL):
+            cleaned = cleaned[:-len(const.GLOBAL)]
+        cleaned = cleaned.strip(' ;')
+
         parts = [p.strip() for p in cleaned.split(';')]
         return [p for p in parts if p]
 
     def _build_trie(self) -> Trie[Data]:
         root_trie: Trie[Data] = Trie()
         for ss in self:
             for part_id, part_str in ss._raw_parts():
```

## search_string/version.py

```diff
@@ -1,3 +1,3 @@
 from __future__ import annotations
 
-__version__ = '0.3.6'
+__version__ = '0.3.7'
```

## Comparing `search_string_overvaagning-0.3.6.dist-info/LICENSE` & `search_string_overvaagning-0.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `search_string_overvaagning-0.3.6.dist-info/METADATA` & `search_string_overvaagning-0.3.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search-string-overvaagning
-Version: 0.3.6
+Version: 0.3.7
 Summary: SearchString is a custom implementation for searching strings for overvaagning.app.
 Home-page: https://github.com/kaas-mulvad/search-string
 Author: Søren Mulvad
 Author-email: Soeren Mulvad <post@kaasogmulvad.dk>
 License: End-User License Agreement (EULA) of SearchString
         
         This End-User License Agreement ("EULA") is a legal agreement between you and Kaas & Mulvad. Our EULA was created by EULA Template for SearchString.
@@ -51,19 +51,21 @@
 Project-URL: Documentation, https://github.com/kaas-mulvad/search-string/
 Project-URL: Changelog, https://github.com/kaas-mulvad/search-string/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://github.com/kaas-mulvad/search-string/
 Project-URL: Github, https://github.com/kaas-mulvad/search-string
 Project-URL: Source, https://github.com/kaas-mulvad/search-string
 Project-URL: Issues, https://github.com/kaas-mulvad/search-string/issues
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: >=3.10.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Search String
 
 ![GitHub Workflow Status (branch)](https://github.com/kaas-mulvad/search-string/workflows/CI/badge.svg)
 [![PyPI - Version](https://img.shields.io/pypi/v/search-string-overvaagning)][pypi]
```

