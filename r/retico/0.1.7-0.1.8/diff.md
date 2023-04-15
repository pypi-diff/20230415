# Comparing `tmp/retico-0.1.7.tar.gz` & `tmp/retico-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retico-0.1.7.tar", last modified: Fri Oct 21 08:50:02 2022, max compression
+gzip compressed data, was "retico-0.1.8.tar", last modified: Sat Apr 15 16:43:50 2023, max compression
```

## Comparing `retico-0.1.7.tar` & `retico-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thilo      (501) staff       (20)        0 2022-10-21 08:50:02.585300 retico-0.1.7/
--rw-r--r--   0 thilo      (501) staff       (20)    11357 2022-08-12 20:05:29.000000 retico-0.1.7/LICENSE
--rw-r--r--   0 thilo      (501) staff       (20)     1338 2022-10-21 08:50:02.585416 retico-0.1.7/PKG-INFO
--rw-r--r--   0 thilo      (501) staff       (20)      709 2022-09-07 14:03:55.000000 retico-0.1.7/README.md
-drwxr-xr-x   0 thilo      (501) staff       (20)        0 2022-10-21 08:50:02.583829 retico-0.1.7/retico/
--rw-r--r--   0 thilo      (501) staff       (20)      199 2022-09-09 15:17:25.000000 retico-0.1.7/retico/__init__.py
--rw-r--r--   0 thilo      (501) staff       (20)      275 2022-10-21 08:49:19.000000 retico-0.1.7/retico/helper.py
--rw-r--r--   0 thilo      (501) staff       (20)      228 2022-08-13 12:31:14.000000 retico-0.1.7/retico/ius.py
--rw-r--r--   0 thilo      (501) staff       (20)      866 2022-09-07 14:05:02.000000 retico-0.1.7/retico/modules.py
--rw-r--r--   0 thilo      (501) staff       (20)       76 2022-10-21 08:49:33.000000 retico-0.1.7/retico/version.py
-drwxr-xr-x   0 thilo      (501) staff       (20)        0 2022-10-21 08:50:02.585081 retico-0.1.7/retico.egg-info/
--rw-r--r--   0 thilo      (501) staff       (20)     1338 2022-10-21 08:50:02.000000 retico-0.1.7/retico.egg-info/PKG-INFO
--rw-r--r--   0 thilo      (501) staff       (20)      271 2022-10-21 08:50:02.000000 retico-0.1.7/retico.egg-info/SOURCES.txt
--rw-r--r--   0 thilo      (501) staff       (20)        1 2022-10-21 08:50:02.000000 retico-0.1.7/retico.egg-info/dependency_links.txt
--rw-r--r--   0 thilo      (501) staff       (20)      148 2022-10-21 08:50:02.000000 retico-0.1.7/retico.egg-info/requires.txt
--rw-r--r--   0 thilo      (501) staff       (20)        7 2022-10-21 08:50:02.000000 retico-0.1.7/retico.egg-info/top_level.txt
--rw-r--r--   0 thilo      (501) staff       (20)      103 2022-10-21 08:50:02.585915 retico-0.1.7/setup.cfg
--rw-r--r--   0 thilo      (501) staff       (20)     1517 2022-10-21 08:48:12.000000 retico-0.1.7/setup.py
+drwxr-xr-x   0 thilo      (501) staff       (20)        0 2023-04-15 16:43:50.328079 retico-0.1.8/
+-rw-r--r--   0 thilo      (501) staff       (20)    11357 2023-04-15 16:42:04.000000 retico-0.1.8/LICENSE
+-rw-r--r--   0 thilo      (501) staff       (20)     1338 2023-04-15 16:43:50.328127 retico-0.1.8/PKG-INFO
+-rw-r--r--   0 thilo      (501) staff       (20)      709 2023-04-15 16:42:04.000000 retico-0.1.8/README.md
+drwxr-xr-x   0 thilo      (501) staff       (20)        0 2023-04-15 16:43:50.327420 retico-0.1.8/retico/
+-rw-r--r--   0 thilo      (501) staff       (20)      199 2023-04-15 16:42:04.000000 retico-0.1.8/retico/__init__.py
+-rw-r--r--   0 thilo      (501) staff       (20)      275 2023-04-15 16:42:05.000000 retico-0.1.8/retico/helper.py
+-rw-r--r--   0 thilo      (501) staff       (20)      228 2023-04-15 16:42:05.000000 retico-0.1.8/retico/ius.py
+-rw-r--r--   0 thilo      (501) staff       (20)      916 2023-04-15 16:43:33.000000 retico-0.1.8/retico/modules.py
+-rw-r--r--   0 thilo      (501) staff       (20)       76 2023-04-15 16:42:48.000000 retico-0.1.8/retico/version.py
+drwxr-xr-x   0 thilo      (501) staff       (20)        0 2023-04-15 16:43:50.327968 retico-0.1.8/retico.egg-info/
+-rw-r--r--   0 thilo      (501) staff       (20)     1338 2023-04-15 16:43:50.000000 retico-0.1.8/retico.egg-info/PKG-INFO
+-rw-r--r--   0 thilo      (501) staff       (20)      271 2023-04-15 16:43:50.000000 retico-0.1.8/retico.egg-info/SOURCES.txt
+-rw-r--r--   0 thilo      (501) staff       (20)        1 2023-04-15 16:43:50.000000 retico-0.1.8/retico.egg-info/dependency_links.txt
+-rw-r--r--   0 thilo      (501) staff       (20)      170 2023-04-15 16:43:50.000000 retico-0.1.8/retico.egg-info/requires.txt
+-rw-r--r--   0 thilo      (501) staff       (20)        7 2023-04-15 16:43:50.000000 retico-0.1.8/retico.egg-info/top_level.txt
+-rw-r--r--   0 thilo      (501) staff       (20)      103 2023-04-15 16:43:50.328312 retico-0.1.8/setup.cfg
+-rw-r--r--   0 thilo      (501) staff       (20)     1550 2023-04-15 16:43:39.000000 retico-0.1.8/setup.py
```

### Comparing `retico-0.1.7/LICENSE` & `retico-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `retico-0.1.7/PKG-INFO` & `retico-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retico
-Version: 0.1.7
+Version: 0.1.8
 Summary: Retico is an open source framework for building state-of-the-art incremental processing systems.
 Home-page: https://github.com/retico-team/retico
 Download-URL: https://github.com/retico-team/retico
 Author: Thilo Michael
 Author-email: uhlomuhlo@gmail.com
 Keywords: retico,framework,incremental,dialogue,dialog,asr,speech
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `retico-0.1.7/README.md` & `retico-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `retico-0.1.7/retico/modules.py` & `retico-0.1.8/retico/modules.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,7 +26,9 @@
 from retico_googletts import GoogleTTSModule
 
 from retico_wav2vecasr import Wav2VecASRModule
 
 from retico_speechbraintts import SpeechBrainTTSModule
 
 from retico_hftranslate import HFTranslateModule
+
+from retico_chatgpt import ChatGPTDialogueModule
```

### Comparing `retico-0.1.7/retico.egg-info/PKG-INFO` & `retico-0.1.8/retico.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retico
-Version: 0.1.7
+Version: 0.1.8
 Summary: Retico is an open source framework for building state-of-the-art incremental processing systems.
 Home-page: https://github.com/retico-team/retico
 Download-URL: https://github.com/retico-team/retico
 Author: Thilo Michael
 Author-email: uhlomuhlo@gmail.com
 Keywords: retico,framework,incremental,dialogue,dialog,asr,speech
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `retico-0.1.7/setup.py` & `retico-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "install_requires": [
         "retico-core>=0.2.10",
         "retico-googleasr>=0.1.5",
         "retico-googletts>=0.1.3",
         "retico-hftranslate>=0.1.2",
         "retico-speechbraintts>=0.1.3",
         "retico-wav2vecasr>=0.1.6",
+        "retico-chatgpt>=0.0.1",
     ],
     "packages": find_packages(),
     "name": "retico",
     "keywords": "retico, framework, incremental, dialogue, dialog, asr, speech",
     "classifiers": [
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3",
```

