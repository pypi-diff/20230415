# Comparing `tmp/tinote-0.3.0.tar.gz` & `tmp/tinote-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-0.3.0.tar", last modified: Sat Apr 15 14:50:55 2023, max compression
+gzip compressed data, was "tinote-0.3.1.tar", last modified: Sat Apr 15 14:52:21 2023, max compression
```

## Comparing `tinote-0.3.0.tar` & `tinote-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 14:50:55.166981 tinote-0.3.0/
--rw-rw-rw-   0        0        0     1830 2023-04-15 14:50:55.151320 tinote-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-04-15 14:49:31.000000 tinote-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 14:50:55.166981 tinote-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-04-15 14:50:10.000000 tinote-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:50:55.135770 tinote-0.3.0/tinote/
--rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-0.3.0/tinote/__init__.py
--rw-rw-rw-   0        0        0     6019 2023-04-15 14:47:26.000000 tinote-0.3.0/tinote/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:50:55.151320 tinote-0.3.0/tinote.egg-info/
--rw-rw-rw-   0        0        0     1830 2023-04-15 14:50:55.000000 tinote-0.3.0/tinote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-15 14:50:55.000000 tinote-0.3.0/tinote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 14:50:55.000000 tinote-0.3.0/tinote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-15 14:50:55.000000 tinote-0.3.0/tinote.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 14:50:55.000000 tinote-0.3.0/tinote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 14:52:21.297646 tinote-0.3.1/
+-rw-rw-rw-   0        0        0     1830 2023-04-15 14:52:21.297646 tinote-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-04-15 14:49:31.000000 tinote-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 14:52:21.297646 tinote-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-04-15 14:52:09.000000 tinote-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:52:21.266299 tinote-0.3.1/tinote/
+-rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-0.3.1/tinote/__init__.py
+-rw-rw-rw-   0        0        0     6022 2023-04-15 14:51:51.000000 tinote-0.3.1/tinote/main.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:52:21.282025 tinote-0.3.1/tinote.egg-info/
+-rw-rw-rw-   0        0        0     1830 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 14:52:21.000000 tinote-0.3.1/tinote.egg-info/top_level.txt
```

### Comparing `tinote-0.3.0/PKG-INFO` & `tinote-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 0.3.0
+Version: 0.3.1
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tinote-0.3.0/README.md` & `tinote-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tinote-0.3.0/setup.py` & `tinote-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tinote",
-    version="0.3.0",
+    version="0.3.1",
     packages=find_packages(),
     install_requires=[
         # Add your package dependencies here
     ],
     entry_points={
         "console_scripts": [
             "ti = tinote.main:main"
```

### Comparing `tinote-0.3.0/tinote/main.py` & `tinote-0.3.1/tinote/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         create_note(args.note, args.category, args.importance)
     elif args.subcommand == "list":
         list_notes(args.category, args.importance)
     elif args.subcommand == "mark":
         mark_note(args.id, not args.uncheck)
     elif args.subcommand == "delete":
         delete_note(args.id)
-    elif args.command == 'clear':
+    elif args.subcommand == 'clear':
         clear_notes(args.category)
     else:
         parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tinote-0.3.0/tinote.egg-info/PKG-INFO` & `tinote-0.3.1/tinote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 0.3.0
+Version: 0.3.1
 Summary: A command-line note-taking tool
 Home-page: https://github.com/yourusername/tinote
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

