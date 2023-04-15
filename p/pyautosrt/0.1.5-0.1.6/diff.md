# Comparing `tmp/pyautosrt-0.1.5.tar.gz` & `tmp/pyautosrt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.1.5.tar", last modified: Fri Apr 14 15:28:09 2023, max compression
+gzip compressed data, was "pyautosrt-0.1.6.tar", last modified: Sat Apr 15 02:00:02 2023, max compression
```

## Comparing `pyautosrt-0.1.5.tar` & `pyautosrt-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:28:09.808089 pyautosrt-0.1.5/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-04-14 15:28:09.811087 pyautosrt-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3061 2023-02-10 19:35:06.000000 pyautosrt-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 15:28:09.766133 pyautosrt-0.1.5/pyautosrt/
--rw-rw-rw-   0        0        0    40130 2023-04-14 15:18:14.000000 pyautosrt-0.1.5/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:28:09.805842 pyautosrt-0.1.5/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-04-14 15:28:08.000000 pyautosrt-0.1.5/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-14 15:28:09.000000 pyautosrt-0.1.5/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:28:08.000000 pyautosrt-0.1.5/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-14 15:28:08.000000 pyautosrt-0.1.5/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-14 15:28:08.000000 pyautosrt-0.1.5/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 15:28:08.000000 pyautosrt-0.1.5/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-14 15:28:09.839555 pyautosrt-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1512 2023-04-14 15:18:29.000000 pyautosrt-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:00:02.653945 pyautosrt-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-04-15 02:00:02.654695 pyautosrt-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3061 2023-02-10 19:35:06.000000 pyautosrt-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 02:00:02.633715 pyautosrt-0.1.6/pyautosrt/
+-rw-rw-rw-   0        0        0    40130 2023-04-15 01:59:25.000000 pyautosrt-0.1.6/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:00:02.651697 pyautosrt-0.1.6/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-04-15 02:00:02.000000 pyautosrt-0.1.6/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-15 02:00:02.000000 pyautosrt-0.1.6/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 02:00:02.000000 pyautosrt-0.1.6/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-15 02:00:02.000000 pyautosrt-0.1.6/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-15 02:00:02.000000 pyautosrt-0.1.6/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 02:00:02.000000 pyautosrt-0.1.6/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-15 02:00:02.656192 pyautosrt-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1512 2023-04-15 01:59:36.000000 pyautosrt-0.1.6/setup.py
```

### Comparing `pyautosrt-0.1.5/LICENSE` & `pyautosrt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.5/PKG-INFO` & `pyautosrt-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.5
+Version: 0.1.6
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.1.5/README.md` & `pyautosrt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.5/pyautosrt/__init__.py` & `pyautosrt-0.1.6/pyautosrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,15 +813,15 @@
     global all_threads, thread_transcribe, not_transcribing, pool
 
     parser = argparse.ArgumentParser()
     parser.add_argument('source_path', help="Path to the video or audio files to generate subtitle (use wildcard for multiple files or separate them with space eg. \"file 1.mp4\" \"file 2.mp4\")", nargs='*', default='')
     parser.add_argument('-S', '--src-language', help="Voice language", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired language for translation", default="en")
     parser.add_argument('-F', '--format', help="Destination subtitle format", default="srt")
-    parser.add_argument('-v', '--version', action='version', version='0.1.5')
+    parser.add_argument('-v', '--version', action='version', version='0.1.6')
     parser.add_argument('-lf', '--list-formats', help="List all available subtitle formats", action='store_true')
     parser.add_argument('-ll', '--list-languages', help="List all available source/translation languages", action='store_true')
 
     args = parser.parse_args()
 
     if args.list_formats:
         print("List of formats:")
```

### Comparing `pyautosrt-0.1.5/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.1.6/pyautosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.5
+Version: 0.1.6
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.1.5/setup.py` & `pyautosrt-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'them to a different language, and finally saves the resulting subtitles to disk.'
     'It supports  a variety of input and output languages  and can currently produce '
     'subtitles in SRT, VTT, JSON, and RAW format.'
 )
 
 setup(
     name="pyautosrt",
-    version="0.1.5",
+    version="0.1.6",
     description="pyautosrt is a python based desktop app to generate subtitle and translated subtitle file",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/pyautosrt",
     packages=[str("pyautosrt")],
     entry_points={
```

