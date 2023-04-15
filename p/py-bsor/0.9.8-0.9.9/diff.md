# Comparing `tmp/py_bsor-0.9.8.tar.gz` & `tmp/py_bsor-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_bsor-0.9.8.tar", last modified: Mon Sep 12 23:05:19 2022, max compression
+gzip compressed data, was "py_bsor-0.9.9.tar", last modified: Fri Nov  4 21:04:02 2022, max compression
```

## Comparing `py_bsor-0.9.8.tar` & `py_bsor-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-12 23:05:19.479552 py_bsor-0.9.8/
--rw-rw-rw-   0        0        0     1095 2022-09-02 17:44:28.000000 py_bsor-0.9.8/LICENSE
--rw-rw-rw-   0        0        0     2379 2022-09-12 23:05:19.479052 py_bsor-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0      593 2022-09-04 22:10:18.000000 py_bsor-0.9.8/README.md
--rw-rw-rw-   0        0        0      620 2022-09-12 23:04:19.000000 py_bsor-0.9.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-12 23:05:19.480049 py_bsor-0.9.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-12 23:05:19.453048 py_bsor-0.9.8/src/
-drwxrwxrwx   0        0        0        0 2022-09-12 23:05:19.473049 py_bsor-0.9.8/src/bsor/
--rw-rw-rw-   0        0        0     9840 2022-09-12 23:04:06.000000 py_bsor-0.9.8/src/bsor/Bsor.py
--rw-rw-rw-   0        0        0     5132 2022-09-10 23:22:30.000000 py_bsor-0.9.8/src/bsor/Bsor_Main.py
--rw-rw-rw-   0        0        0     1391 2022-09-10 17:45:26.000000 py_bsor-0.9.8/src/bsor/Decoder.py
--rw-rw-rw-   0        0        0        0 2022-09-02 17:52:15.000000 py_bsor-0.9.8/src/bsor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 23:05:19.478048 py_bsor-0.9.8/src/py_bsor.egg-info/
--rw-rw-rw-   0        0        0     2379 2022-09-12 23:05:19.000000 py_bsor-0.9.8/src/py_bsor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2022-09-12 23:05:19.000000 py_bsor-0.9.8/src/py_bsor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-12 23:05:19.000000 py_bsor-0.9.8/src/py_bsor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-09-12 23:05:19.000000 py_bsor-0.9.8/src/py_bsor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-04 21:04:02.206847 py_bsor-0.9.9/
+-rw-rw-rw-   0        0        0     1095 2022-09-02 17:44:28.000000 py_bsor-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     2379 2022-11-04 21:04:02.205844 py_bsor-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2022-09-04 22:10:18.000000 py_bsor-0.9.9/README.md
+-rw-rw-rw-   0        0        0      620 2022-11-04 21:02:21.000000 py_bsor-0.9.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-11-04 21:04:02.206847 py_bsor-0.9.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-11-04 21:04:02.176298 py_bsor-0.9.9/src/
+drwxrwxrwx   0        0        0        0 2022-11-04 21:04:02.199830 py_bsor-0.9.9/src/bsor/
+-rw-rw-rw-   0        0        0     9927 2022-11-04 21:01:34.000000 py_bsor-0.9.9/src/bsor/Bsor.py
+-rw-rw-rw-   0        0        0     5271 2022-11-04 21:00:37.000000 py_bsor-0.9.9/src/bsor/Bsor_Main.py
+-rw-rw-rw-   0        0        0     1391 2022-09-10 17:45:26.000000 py_bsor-0.9.9/src/bsor/Decoder.py
+-rw-rw-rw-   0        0        0        0 2022-09-02 17:52:15.000000 py_bsor-0.9.9/src/bsor/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-04 21:04:02.204844 py_bsor-0.9.9/src/py_bsor.egg-info/
+-rw-rw-rw-   0        0        0     2379 2022-11-04 21:04:02.000000 py_bsor-0.9.9/src/py_bsor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2022-11-04 21:04:02.000000 py_bsor-0.9.9/src/py_bsor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-04 21:04:02.000000 py_bsor-0.9.9/src/py_bsor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2022-11-04 21:04:02.000000 py_bsor-0.9.9/src/py_bsor.egg-info/top_level.txt
```

### Comparing `py_bsor-0.9.8/LICENSE` & `py_bsor-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_bsor-0.9.8/PKG-INFO` & `py_bsor-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_bsor
-Version: 0.9.8
+Version: 0.9.9
 Summary: BS Open Replay Parser
 Author-email: Carsten Schipmann <theschippi+gh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carsten Schipmann
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `py_bsor-0.9.8/README.md` & `py_bsor-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `py_bsor-0.9.8/pyproject.toml` & `py_bsor-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "py_bsor"
-version = "0.9.8"
+version = "0.9.9"
 authors = [
   { name="Carsten Schipmann", email="theschippi+gh@gmail.com" },
 ]
 description = "BS Open Replay Parser"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `py_bsor-0.9.8/src/bsor/Bsor.py` & `py_bsor-0.9.9/src/bsor/Bsor.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,17 @@
         else:
             beforeCutRawScore = 70 * cut.beforeCutRating
             beforeCutRawScore = round_half_up(beforeCutRawScore)
             beforeCutRawScore = clamp(beforeCutRawScore, 0, 70)
 
     afterCutRawScore = 0
     if type != NOTE_SCORE_TYPE_BURSTSLIDERELEMENT:
-        if type == NOTE_SCORE_TYPE_SLIDERHEAD:
+        if type == NOTE_SCORE_TYPE_BURSTSLIDERHEAD:
+            afterCutRawScore = 0
+        elif type == NOTE_SCORE_TYPE_SLIDERHEAD:
             afterCutRawScore = 30
         else:
             afterCutRawScore = 30 * cut.afterCutRating
             afterCutRawScore = round_half_up(afterCutRawScore )
             afterCutRawScore = clamp(afterCutRawScore, 0, 30)
 
     cutDistanceRawScore = 0
@@ -356,15 +358,15 @@
     m.pauses = make_pauses(f)
 
     return m
 
 
 if __name__ == '__main__':
     import os
-    filename = 'D:/_TMP/Nutella.bsor'
+    filename = 'D:/_TMP/Burst.bsor'
     print('File name :    ', os.path.basename(filename))
     try:
         with open(filename, "rb") as f:
             m = make_bsor(f)
             print('BSOR Version: %d' % m.file_version)
             print('BSOR notes: %d' % len(m.notes))
     except BSException as e:
```

### Comparing `py_bsor-0.9.8/src/bsor/Bsor_Main.py` & `py_bsor-0.9.9/src/bsor/Bsor_Main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from Bsor import *
 
 if __name__ == '__main__':
     import os
-    filename = 'D:/_TMP/Nutella.bsor'
+    filename = 'D:/_TMP/Burst.bsor'
     print('File name :    ', os.path.basename(filename))
     try:
         with open(filename, "rb") as f:
             m = make_bsor(f)
             print('BSOR Version: %d' % m.file_version)
             print('BSOR notes: %d' % len(m.notes))
             bad,miss,bomb = [0,0],[0,0],[0,0]
@@ -57,14 +57,16 @@
             scores =[]
             for e in sorted_events:
                 if isinstance(e[1],Note):
                     note_cnt = note_cnt + 1
                     max_mul = 8 if note_cnt > 8+4+2 else 4 if note_cnt > 4+2 else 2 if note_cnt > 2 else 1
                     if e[1].scoringType == NOTE_SCORE_TYPE_BURSTSLIDERELEMENT:
                         max_score = max_score + max_mul * 20
+                    elif e[1].scoringType == NOTE_SCORE_TYPE_BURSTSLIDERHEAD:
+                        max_score = max_score + max_mul * 85
                     else:
                         max_score = max_score + max_mul * 115
                 if isinstance(e[1],Wall) or isinstance(e[1],Note) and e[1].score == 0:
                     multiplier,mul_progress,mul_max_progress = dec_mul(multiplier,mul_progress,mul_max_progress)
                     combo = 0
                 else:
                     multiplier,mul_progress,mul_max_progress = inc_mul(multiplier,mul_progress,mul_max_progress)
```

### Comparing `py_bsor-0.9.8/src/bsor/Decoder.py` & `py_bsor-0.9.9/src/bsor/Decoder.py`

 * *Files identical despite different names*

### Comparing `py_bsor-0.9.8/src/py_bsor.egg-info/PKG-INFO` & `py_bsor-0.9.9/src/py_bsor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-bsor
-Version: 0.9.8
+Version: 0.9.9
 Summary: BS Open Replay Parser
 Author-email: Carsten Schipmann <theschippi+gh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Carsten Schipmann
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

