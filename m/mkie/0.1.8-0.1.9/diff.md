# Comparing `tmp/mkie-0.1.8.tar.gz` & `tmp/mkie-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkie-0.1.8.tar", max compression
+gzip compressed data, was "mkie-0.1.9.tar", max compression
```

## Comparing `mkie-0.1.8.tar` & `mkie-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1086 2023-03-21 08:09:20.020758 mkie-0.1.8/LICENSE
--rw-r--r--   0        0        0      655 2023-04-08 08:29:33.972716 mkie-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-21 08:09:20.021107 mkie-0.1.8/mkie/__init__.py
--rw-r--r--   0        0        0     4147 2023-04-08 08:25:24.196338 mkie-0.1.8/mkie/__main__.py
--rw-r--r--   0        0        0        0 2023-03-21 08:09:20.021483 mkie-0.1.8/mkie/core/__init__.py
--rw-r--r--   0        0        0     6295 2023-04-08 08:25:16.304737 mkie-0.1.8/mkie/core/mkdk.py
--rw-r--r--   0        0        0    10171 2023-04-04 16:05:56.243288 mkie-0.1.8/mkie/core/mkgit.py
--rw-r--r--   0        0        0     1515 2023-04-04 16:07:02.896812 mkie-0.1.8/mkie/core/toolkit.py
--rw-r--r--   0        0        0      635 2023-04-08 08:29:54.517783 mkie-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 mkie-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-03-21 08:09:20.020758 mkie-0.1.9/LICENSE
+-rw-r--r--   0        0        0      655 2023-04-08 08:35:24.483085 mkie-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-21 08:09:20.021107 mkie-0.1.9/mkie/__init__.py
+-rw-r--r--   0        0        0     4147 2023-04-08 08:35:24.483757 mkie-0.1.9/mkie/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-21 08:09:20.021483 mkie-0.1.9/mkie/core/__init__.py
+-rw-r--r--   0        0        0     6299 2023-04-15 06:22:36.756548 mkie-0.1.9/mkie/core/mkdk.py
+-rw-r--r--   0        0        0    10171 2023-04-08 08:35:24.485501 mkie-0.1.9/mkie/core/mkgit.py
+-rw-r--r--   0        0        0     1515 2023-04-04 16:07:02.896812 mkie-0.1.9/mkie/core/toolkit.py
+-rw-r--r--   0        0        0      635 2023-04-15 06:22:36.757076 mkie-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 mkie-0.1.9/PKG-INFO
```

### Comparing `mkie-0.1.8/LICENSE` & `mkie-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkie-0.1.8/README.md` & `mkie-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mkie-0.1.8/mkie/__main__.py` & `mkie-0.1.9/mkie/__main__.py`

 * *Files identical despite different names*

### Comparing `mkie-0.1.8/mkie/core/mkdk.py` & `mkie-0.1.9/mkie/core/mkdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 project_name=project_name,
                 subpath=subpath,
                 filepath=filepath,
             )
             _cmd.extend(['-f', str(_path)])
 
         _cmd.append('up')
-        if is_follow:
+        if not is_follow:
             _cmd.append('-d')
 
         # color log
         color_prefix = Style.RESET_ALL + Fore.BLACK
         prefix = Colored.get_color_prefix(color='LIGHTYELLOW_EX',
                                           color_prefix=color_prefix,
                                           prefix_msg='🐳 Docker ⬆ ',
```

### Comparing `mkie-0.1.8/mkie/core/mkgit.py` & `mkie-0.1.9/mkie/core/mkgit.py`

 * *Files identical despite different names*

### Comparing `mkie-0.1.8/mkie/core/toolkit.py` & `mkie-0.1.9/mkie/core/toolkit.py`

 * *Files identical despite different names*

### Comparing `mkie-0.1.8/pyproject.toml` & `mkie-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'mkie'
-version = '0.1.8'
+version = '0.1.9'
 description = 'A useful tool for control clis in terminal.'
 license = 'MIT'
 authors = ['Michael Chou <snoopy02m@gmail.com>']
 repository = 'https://github.com/cbb23021/mkie'
 readme = 'README.md'
 classifiers = [
   'Operating System :: MacOS',
```

### Comparing `mkie-0.1.8/PKG-INFO` & `mkie-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkie
-Version: 0.1.8
+Version: 0.1.9
 Summary: A useful tool for control clis in terminal.
 Home-page: https://github.com/cbb23021/mkie
 License: MIT
 Author: Michael Chou
 Author-email: snoopy02m@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

