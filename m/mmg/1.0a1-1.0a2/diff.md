# Comparing `tmp/mmg-1.0a1.tar.gz` & `tmp/mmg-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmg-1.0a1.tar", last modified: Thu Jun 17 00:06:06 2021, max compression
+gzip compressed data, was "/home/hr/git/multilingual-markdown/dist/tmpzvn4azvn/mmg-1.0a2.tar", last modified: Thu Jun 17 01:39:05 2021, max compression
```

## Comparing `mmg-1.0a1.tar` & `mmg-1.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 00:06:06.680966 mmg-1.0a1/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-06-17 00:05:53.000000 mmg-1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-06-17 00:05:53.000000 mmg-1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11897 2021-06-17 00:06:06.680966 mmg-1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    24534 2021-06-17 00:05:53.000000 mmg-1.0a1/README.base.md
--rw-r--r--   0 runner    (1001) docker     (121)    12391 2021-06-17 00:05:53.000000 mmg-1.0a1/README.fr.md
--rw-r--r--   0 runner    (1001) docker     (121)    11833 2021-06-17 00:05:53.000000 mmg-1.0a1/README.kr.md
--rw-r--r--   0 runner    (1001) docker     (121)    10938 2021-06-17 00:05:53.000000 mmg-1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 00:06:06.676965 mmg-1.0a1/bin/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-06-17 00:05:53.000000 mmg-1.0a1/bin/mmg
--rw-r--r--   0 runner    (1001) docker     (121)    62451 2021-06-17 00:05:53.000000 mmg-1.0a1/how-it-works.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 00:06:06.676965 mmg-1.0a1/mmg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11897 2021-06-17 00:06:06.000000 mmg-1.0a1/mmg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-06-17 00:06:06.000000 mmg-1.0a1/mmg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-17 00:06:06.000000 mmg-1.0a1/mmg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-06-17 00:06:06.000000 mmg-1.0a1/mmg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-17 00:06:06.000000 mmg-1.0a1/mmg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 00:06:06.680966 mmg-1.0a1/mmgcli/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-06-17 00:05:53.000000 mmg-1.0a1/mmgcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-06-17 00:05:53.000000 mmg-1.0a1/mmgcli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9933 2021-06-17 00:05:53.000000 mmg-1.0a1/mmgcli/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4326 2021-06-17 00:05:53.000000 mmg-1.0a1/mmgcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2021-06-17 00:05:53.000000 mmg-1.0a1/mmgcli/single_gen.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-06-17 00:05:53.000000 mmg-1.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-06-17 00:06:06.680966 mmg-1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2021-06-17 00:05:53.000000 mmg-1.0a1/setup.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2021-06-17 01:39:05.000000 mmg-1.0a2/
+-rw-rw-r--   0 hr        (1000) hr        (1000)    24534 2021-06-17 01:27:41.000000 mmg-1.0a2/README.base.md
+-rw-rw-r--   0 hr        (1000) hr        (1000)     2830 2021-06-17 01:21:06.000000 mmg-1.0a2/setup.py
+-rw-rw-r--   0 hr        (1000) hr        (1000)       25 2021-06-17 01:21:06.000000 mmg-1.0a2/requirements.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)    62451 2021-06-17 01:21:06.000000 mmg-1.0a2/how-it-works.png
+-rw-rw-r--   0 hr        (1000) hr        (1000)    10938 2021-06-17 01:27:41.000000 mmg-1.0a2/README.md
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2021-06-17 01:39:05.000000 mmg-1.0a2/mmgcli/
+-rw-rw-r--   0 hr        (1000) hr        (1000)     4330 2021-06-17 01:27:41.000000 mmg-1.0a2/mmgcli/cli.py
+-rw-rw-r--   0 hr        (1000) hr        (1000)       94 2021-06-17 01:27:41.000000 mmg-1.0a2/mmgcli/__init__.py
+-rw-rw-r--   0 hr        (1000) hr        (1000)     9933 2021-06-17 01:27:41.000000 mmg-1.0a2/mmgcli/base_parser.py
+-rw-rw-r--   0 hr        (1000) hr        (1000)     3846 2021-06-17 01:21:06.000000 mmg-1.0a2/mmgcli/single_gen.py
+-rw-rw-r--   0 hr        (1000) hr        (1000)      237 2021-06-17 01:21:06.000000 mmg-1.0a2/mmgcli/__main__.py
+-rw-rw-r--   0 hr        (1000) hr        (1000)    11897 2021-06-17 01:39:05.000000 mmg-1.0a2/PKG-INFO
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2021-06-17 01:39:05.000000 mmg-1.0a2/mmg.egg-info/
+-rw-rw-r--   0 hr        (1000) hr        (1000)    11897 2021-06-17 01:39:05.000000 mmg-1.0a2/mmg.egg-info/PKG-INFO
+-rw-rw-r--   0 hr        (1000) hr        (1000)        7 2021-06-17 01:39:05.000000 mmg-1.0a2/mmg.egg-info/top_level.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)        1 2021-06-17 01:39:05.000000 mmg-1.0a2/mmg.egg-info/dependency_links.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)       26 2021-06-17 01:39:05.000000 mmg-1.0a2/mmg.egg-info/requires.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)      360 2021-06-17 01:39:05.000000 mmg-1.0a2/mmg.egg-info/SOURCES.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)      103 2021-06-17 01:21:06.000000 mmg-1.0a2/MANIFEST.in
+-rw-rw-r--   0 hr        (1000) hr        (1000)    12391 2021-06-17 01:27:41.000000 mmg-1.0a2/README.fr.md
+-rw-rw-r--   0 hr        (1000) hr        (1000)    11833 2021-06-17 01:27:41.000000 mmg-1.0a2/README.kr.md
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2021-06-17 01:39:05.000000 mmg-1.0a2/bin/
+-rwxrwxr-x   0 hr        (1000) hr        (1000)      237 2021-06-17 01:27:41.000000 mmg-1.0a2/bin/mmg
+-rw-rw-r--   0 hr        (1000) hr        (1000)      179 2021-06-17 01:39:05.000000 mmg-1.0a2/setup.cfg
+-rw-rw-r--   0 hr        (1000) hr        (1000)     1072 2021-06-17 01:21:06.000000 mmg-1.0a2/LICENSE
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mmg-1.0a1/LICENSE` & `mmg-1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmg-1.0a1/PKG-INFO` & `mmg-1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmg
-Version: 1.0a1
+Version: 1.0a2
 Summary: Command Line Interface to Generate i18n Markdown
 Home-page: https://github.com/ryul1206/multilingual-markdown
 Author: Hong-ryul Jung
 Author-email: jung.hr.1206@gmail.com
 License: MIT
 Keywords: i18n,markdown,cli
 Platform: UNKNOWN
@@ -28,15 +28,15 @@
 This package provides a command-line interface to manage multilingual contents and generate i18n markdown from a single base file.
 
 [![Multilingual Markdown Generator](https://img.shields.io/badge/markdown-multilingual%20🌐-ff69b4.svg)](https://github.com/ryul1206/multilingual-markdown)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ryul1206/multilingual-markdown.svg)
 ![GitHub](https://img.shields.io/github/license/ryul1206/multilingual-markdown.svg)
 [![CodeFactor](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/badge/master)](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/overview/master)
 
-🚀 **version 1.0-alpha.1** 🌏
+🚀 **version 1.0-alpha.2** 🌏
 [English](https://github.com/ryul1206/multilingual-markdown/blob/master/README.md),
 [Français](https://github.com/ryul1206/multilingual-markdown/blob/master/README.fr.md),
 [한국어](https://github.com/ryul1206/multilingual-markdown/blob/master/README.kr.md)
 
 ---
 
 **Table of Contents** ⚡
```

### Comparing `mmg-1.0a1/README.base.md` & `mmg-1.0a2/README.base.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 <!-- [common] -->
 
 [![Multilingual Markdown Generator](https://img.shields.io/badge/markdown-multilingual%20🌐-ff69b4.svg)](https://github.com/ryul1206/multilingual-markdown)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ryul1206/multilingual-markdown.svg)
 ![GitHub](https://img.shields.io/github/license/ryul1206/multilingual-markdown.svg)
 [![CodeFactor](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/badge/master)](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/overview/master)
 
-🚀 **version 1.0-alpha.1** 🌏
+🚀 **version 1.0-alpha.2** 🌏
 [English](https://github.com/ryul1206/multilingual-markdown/blob/master/README.md),
 [Français](https://github.com/ryul1206/multilingual-markdown/blob/master/README.fr.md),
 [한국어](https://github.com/ryul1206/multilingual-markdown/blob/master/README.kr.md)
 
 ---
 
 <!-- [en] -->
```

### Comparing `mmg-1.0a1/README.fr.md` & `mmg-1.0a2/README.fr.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Ce package fournit une interface de ligne de commande pour gérer les contenus multilingues et générer des démarques i18n à partir d'un seul fichier de base.
 
 [![Multilingual Markdown Generator](https://img.shields.io/badge/markdown-multilingual%20🌐-ff69b4.svg)](https://github.com/ryul1206/multilingual-markdown)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ryul1206/multilingual-markdown.svg)
 ![GitHub](https://img.shields.io/github/license/ryul1206/multilingual-markdown.svg)
 [![CodeFactor](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/badge/master)](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/overview/master)
 
-🚀 **version 1.0-alpha.1** 🌏
+🚀 **version 1.0-alpha.2** 🌏
 [English](https://github.com/ryul1206/multilingual-markdown/blob/master/README.md),
 [Français](https://github.com/ryul1206/multilingual-markdown/blob/master/README.fr.md),
 [한국어](https://github.com/ryul1206/multilingual-markdown/blob/master/README.kr.md)
 
 ---
 
 **Table des matières** ⚡
```

### Comparing `mmg-1.0a1/README.kr.md` & `mmg-1.0a2/README.kr.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 이 패키지는 다국어 콘텐츠를 관리하고, 단일 기본 파일로부터 i18n 마크 다운을 생성하는 명령 줄 인터페이스(CLI)를 제공합니다.
 
 [![Multilingual Markdown Generator](https://img.shields.io/badge/markdown-multilingual%20🌐-ff69b4.svg)](https://github.com/ryul1206/multilingual-markdown)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ryul1206/multilingual-markdown.svg)
 ![GitHub](https://img.shields.io/github/license/ryul1206/multilingual-markdown.svg)
 [![CodeFactor](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/badge/master)](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/overview/master)
 
-🚀 **version 1.0-alpha.1** 🌏
+🚀 **version 1.0-alpha.2** 🌏
 [English](https://github.com/ryul1206/multilingual-markdown/blob/master/README.md),
 [Français](https://github.com/ryul1206/multilingual-markdown/blob/master/README.fr.md),
 [한국어](https://github.com/ryul1206/multilingual-markdown/blob/master/README.kr.md)
 
 ---
 
 **목차** ⚡
```

### Comparing `mmg-1.0a1/README.md` & `mmg-1.0a2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package provides a command-line interface to manage multilingual contents and generate i18n markdown from a single base file.
 
 [![Multilingual Markdown Generator](https://img.shields.io/badge/markdown-multilingual%20🌐-ff69b4.svg)](https://github.com/ryul1206/multilingual-markdown)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ryul1206/multilingual-markdown.svg)
 ![GitHub](https://img.shields.io/github/license/ryul1206/multilingual-markdown.svg)
 [![CodeFactor](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/badge/master)](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/overview/master)
 
-🚀 **version 1.0-alpha.1** 🌏
+🚀 **version 1.0-alpha.2** 🌏
 [English](https://github.com/ryul1206/multilingual-markdown/blob/master/README.md),
 [Français](https://github.com/ryul1206/multilingual-markdown/blob/master/README.fr.md),
 [한국어](https://github.com/ryul1206/multilingual-markdown/blob/master/README.kr.md)
 
 ---
 
 **Table of Contents** ⚡
```

### Comparing `mmg-1.0a1/how-it-works.png` & `mmg-1.0a2/how-it-works.png`

 * *Files identical despite different names*

### Comparing `mmg-1.0a1/mmg.egg-info/PKG-INFO` & `mmg-1.0a2/mmg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmg
-Version: 1.0a1
+Version: 1.0a2
 Summary: Command Line Interface to Generate i18n Markdown
 Home-page: https://github.com/ryul1206/multilingual-markdown
 Author: Hong-ryul Jung
 Author-email: jung.hr.1206@gmail.com
 License: MIT
 Keywords: i18n,markdown,cli
 Platform: UNKNOWN
@@ -28,15 +28,15 @@
 This package provides a command-line interface to manage multilingual contents and generate i18n markdown from a single base file.
 
 [![Multilingual Markdown Generator](https://img.shields.io/badge/markdown-multilingual%20🌐-ff69b4.svg)](https://github.com/ryul1206/multilingual-markdown)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/ryul1206/multilingual-markdown.svg)
 ![GitHub](https://img.shields.io/github/license/ryul1206/multilingual-markdown.svg)
 [![CodeFactor](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/badge/master)](https://www.codefactor.io/repository/github/ryul1206/multilingual-markdown/overview/master)
 
-🚀 **version 1.0-alpha.1** 🌏
+🚀 **version 1.0-alpha.2** 🌏
 [English](https://github.com/ryul1206/multilingual-markdown/blob/master/README.md),
 [Français](https://github.com/ryul1206/multilingual-markdown/blob/master/README.fr.md),
 [한국어](https://github.com/ryul1206/multilingual-markdown/blob/master/README.kr.md)
 
 ---
 
 **Table of Contents** ⚡
```

### Comparing `mmg-1.0a1/mmgcli/base_parser.py` & `mmg-1.0a2/mmgcli/base_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         max_tag = max(suffix_counter.values())
         missing = sum(1 if max_tag != x else 0 for x in suffix_counter.values())
 
         color = "bright_red" if missing else "bright_green"
         message = ""
         if verbosity > 0:
-            message = f"\t[X] {missing} language(s) not translated.\n\t    " if missing else "\t[O] "
+            message = f"\t❌ {missing} language(s) not translated.\n\t    " if missing else "\t✅ "
             message += f"Tag count: {str(suffix_counter)}"
             message += buffer
         return message, color
 
     def run(self):
         # Main converting
         self._converting()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mmg-1.0a1/mmgcli/cli.py` & `mmg-1.0a2/mmgcli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     The "answer" return value is True for "yes" or False for "no".
     """
     valid = {"yes": True, "y": True, "ye": True, "no": False, "n": False}
     default = "no"
     prompt = " [y/N] "
 
     resp = None
-    while not resp:
+    while resp is None:
         sys.stdout.write(question + prompt)
         choice = input().lower()
         if choice == "":
             resp = valid[default]
         elif choice in valid:
             resp = valid[choice]
         sys.stdout.write("Please respond with 'yes' or 'no' " "(or 'y' or 'n').\n")
```

### Comparing `mmg-1.0a1/mmgcli/single_gen.py` & `mmg-1.0a2/mmgcli/single_gen.py`

 * *Files identical despite different names*

### Comparing `mmg-1.0a1/setup.py` & `mmg-1.0a2/setup.py`

 * *Files identical despite different names*

