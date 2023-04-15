# Comparing `tmp/fhnw_nlp_utils-0.6.5-py3-none-any.whl.zip` & `tmp/fhnw_nlp_utils-0.6.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 21902 bytes, number of entries: 17
+Zip file size: 23312 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/nlp/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/__init__.py
 -rw-r--r--  2.0 unx      144 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/colab.py
 -rw-r--r--  2.0 unx     2254 b- defN 22-Aug-14 09:43 fhnw/nlp/utils/defaults.py
 -rw-r--r--  2.0 unx     6880 b- defN 22-Aug-14 09:42 fhnw/nlp/utils/normalize.py
 -rw-r--r--  2.0 unx    37887 b- defN 23-Mar-12 20:31 fhnw/nlp/utils/params.py
 -rw-r--r--  2.0 unx     9537 b- defN 22-Dec-12 20:18 fhnw/nlp/utils/ploting.py
 -rw-r--r--  2.0 unx     2262 b- defN 22-Aug-25 17:41 fhnw/nlp/utils/preprocess.py
 -rw-r--r--  2.0 unx    10048 b- defN 21-Nov-14 18:34 fhnw/nlp/utils/processing.py
 -rw-r--r--  2.0 unx     6838 b- defN 21-Nov-03 20:09 fhnw/nlp/utils/storage.py
 -rw-r--r--  2.0 unx     3346 b- defN 22-Oct-05 05:11 fhnw/nlp/utils/system.py
 -rw-r--r--  2.0 unx     3212 b- defN 22-Aug-10 15:41 fhnw/nlp/utils/text.py
--rw-r--r--  2.0 unx     1298 b- defN 23-Mar-12 20:31 fhnw_nlp_utils-0.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-12 20:31 fhnw_nlp_utils-0.6.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-12 20:31 fhnw_nlp_utils-0.6.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1372 b- defN 23-Mar-12 20:31 fhnw_nlp_utils-0.6.5.dist-info/RECORD
-17 files, 85175 bytes uncompressed, 19648 bytes compressed:  76.9%
+-rw-r--r--  2.0 unx     4011 b- defN 23-Apr-15 14:21 fhnw/nlp/utils/transformers.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1459 b- defN 23-Apr-15 14:21 fhnw_nlp_utils-0.6.6.dist-info/RECORD
+18 files, 89273 bytes uncompressed, 20922 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -33,20 +33,23 @@
 
 Filename: fhnw/nlp/utils/system.py
 Comment: 
 
 Filename: fhnw/nlp/utils/text.py
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.5.dist-info/METADATA
+Filename: fhnw/nlp/utils/transformers.py
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.5.dist-info/WHEEL
+Filename: fhnw_nlp_utils-0.6.6.dist-info/METADATA
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.5.dist-info/top_level.txt
+Filename: fhnw_nlp_utils-0.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.5.dist-info/RECORD
+Filename: fhnw_nlp_utils-0.6.6.dist-info/top_level.txt
+Comment: 
+
+Filename: fhnw_nlp_utils-0.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fhnw_nlp_utils-0.6.5.dist-info/METADATA` & `fhnw_nlp_utils-0.6.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhnw-nlp-utils
-Version: 0.6.5
+Version: 0.6.6
 Summary: Utilities for NLP courses taught at FHNW.
 Home-page: http://github.com/markif/fhnw-nlp-utils
 Author: Fabian
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

## Comparing `fhnw_nlp_utils-0.6.5.dist-info/RECORD` & `fhnw_nlp_utils-0.6.6.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -7,11 +7,12 @@
 fhnw/nlp/utils/params.py,sha256=xavHoG_CMmygKGp3lwHqPbZUpfnrjdLjZPII2fiZPjE,37887
 fhnw/nlp/utils/ploting.py,sha256=8ya50BauVgWfRh7X7V9urU5SCvd7RSF7INhCgKHdzzc,9537
 fhnw/nlp/utils/preprocess.py,sha256=FDy6HAYS3OjKue9kVigh7Cg84gc3rju5Zu0WuOLVoq0,2262
 fhnw/nlp/utils/processing.py,sha256=73R2Vy4tMzXpbjSbck7xZFDigaA3cjuLxbe-ZXxs_uc,10048
 fhnw/nlp/utils/storage.py,sha256=F3C19qp9x2cGHnE0mdLVQxLLqBzgtFUCWZSGtzmk_yw,6838
 fhnw/nlp/utils/system.py,sha256=yRphzlhw34C8qyl-sgUSbz56_Ckr8G-tsRJkko-pv-U,3346
 fhnw/nlp/utils/text.py,sha256=ElaWYdl_7YkHc_IHJyEUZPvKgcADTcbEBEL1FO5emME,3212
-fhnw_nlp_utils-0.6.5.dist-info/METADATA,sha256=WixLGgigtxiBeZmmFDaQeMURIzgdPess1U3URQeYi6A,1298
-fhnw_nlp_utils-0.6.5.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-fhnw_nlp_utils-0.6.5.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
-fhnw_nlp_utils-0.6.5.dist-info/RECORD,,
+fhnw/nlp/utils/transformers.py,sha256=DnSQhF00EMDF_-8616BRI9X_iPHvGidP4AZkfoq0mis,4011
+fhnw_nlp_utils-0.6.6.dist-info/METADATA,sha256=McOy4MXZ6NLlCP-aEQ9GREJxMevyYbMXidyJaZJhArc,1298
+fhnw_nlp_utils-0.6.6.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+fhnw_nlp_utils-0.6.6.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
+fhnw_nlp_utils-0.6.6.dist-info/RECORD,,
```

