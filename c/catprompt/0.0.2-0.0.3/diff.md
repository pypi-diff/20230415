# Comparing `tmp/catprompt-0.0.2.tar.gz` & `tmp/catprompt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catprompt-0.0.2.tar", last modified: Fri Apr 14 09:32:06 2023, max compression
+gzip compressed data, was "catprompt-0.0.3.tar", last modified: Sat Apr 15 14:52:44 2023, max compression
```

## Comparing `catprompt-0.0.2.tar` & `catprompt-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.576426 catprompt-0.0.2/
--rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-14 07:06:27.000000 catprompt-0.0.2/LICENSE
--rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-14 09:32:06.575907 catprompt-0.0.2/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)     4141 2023-04-14 09:29:01.000000 catprompt-0.0.2/README.md
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.573114 catprompt-0.0.2/catprompt/
--rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-14 09:14:16.000000 catprompt-0.0.2/catprompt/__init__.py
--rw-r--r--   0 juanre     (501) staff       (20)     1619 2023-04-14 09:20:30.000000 catprompt-0.0.2/catprompt/prompter.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.574849 catprompt-0.0.2/catprompt.egg-info/
--rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)      307 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/SOURCES.txt
--rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/dependency_links.txt
--rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/entry_points.txt
--rw-r--r--   0 juanre     (501) staff       (20)       72 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/requires.txt
--rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/top_level.txt
--rw-r--r--   0 juanre     (501) staff       (20)      790 2023-04-14 09:31:11.000000 catprompt-0.0.2/pyproject.toml
--rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-14 09:32:06.576608 catprompt-0.0.2/setup.cfg
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-14 09:15:34.000000 catprompt-0.0.2/setup.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.575211 catprompt-0.0.2/test/
--rw-r--r--   0 juanre     (501) staff       (20)     1458 2023-04-14 09:14:49.000000 catprompt-0.0.2/test/test_prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.154076 catprompt-0.0.3/
+-rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.0.3/LICENSE
+-rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-15 14:52:44.153770 catprompt-0.0.3/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)     4141 2023-04-15 09:03:27.000000 catprompt-0.0.3/README.md
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.149858 catprompt-0.0.3/catprompt/
+-rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.0.3/catprompt/__init__.py
+-rw-r--r--   0 juanre     (501) staff       (20)     1967 2023-04-15 14:46:38.000000 catprompt-0.0.3/catprompt/prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.152243 catprompt-0.0.3/catprompt.egg-info/
+-rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)      307 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/entry_points.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/requires.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/top_level.txt
+-rw-r--r--   0 juanre     (501) staff       (20)      832 2023-04-15 14:51:03.000000 catprompt-0.0.3/pyproject.toml
+-rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-15 14:52:44.154163 catprompt-0.0.3/setup.cfg
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.0.3/setup.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.152766 catprompt-0.0.3/test/
+-rw-r--r--   0 juanre     (501) staff       (20)     1458 2023-04-15 09:03:27.000000 catprompt-0.0.3/test/test_prompter.py
```

### Comparing `catprompt-0.0.2/LICENSE` & `catprompt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `catprompt-0.0.2/PKG-INFO` & `catprompt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `catprompt-0.0.2/README.md` & `catprompt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `catprompt-0.0.2/catprompt/prompter.py` & `catprompt-0.0.3/catprompt/prompter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+# -*- coding: utf-8 -*-
+
 import sys
 from pathlib import Path
 import clipboard
+import tiktoken
 
 
 # pylint: disable=inconsistent-return-statements
 def process_line(line, base_dir, processed_lines):
     if line.startswith('++'):
         return
 
     if line.startswith('+='):
         file_to_include = line[2:].strip()
         file_path = base_dir / file_to_include
         if not file_path.is_file():
             file_path = Path(file_to_include)
         if file_path.is_file():
+            print(f'Including {str(file_path)}')
             process_file(file_path, processed_lines)
+        else:
+            raise RuntimeError(f'Cannot find {file_to_include}')
     elif line.startswith('+#'):
         return False
     else:
         processed_lines.append(line)
 
 
 def process_file(file_path, processed_lines=None):
@@ -49,13 +55,16 @@
     input_file = sys.argv[1]
     file_path = Path(input_file)
 
     if not file_path.is_file():
         print(f"Error: '{input_file}' not found.")
         sys.exit(1)
 
-    process_and_copy_to_clipboard(file_path)
-    print("Processed content copied to clipboard.")
+    processed_content = process_and_copy_to_clipboard(file_path)
+    encoding = 'cl100k_base'
+    tokenizer = tiktoken.get_encoding(encoding)
+    tokens = tokenizer.encode(processed_content)
+    print(f"Processed content copied to clipboard, {len(tokens)} {encoding} tokens")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `catprompt-0.0.2/catprompt.egg-info/PKG-INFO` & `catprompt-0.0.3/catprompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `catprompt-0.0.2/pyproject.toml` & `catprompt-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "catprompt"
-version = "0.0.2"
+version = "0.0.3"
 description = "Combine prompts for chatgpt."
 readme = "README.md"
 authors = [
     { name = "Juan Reyero", email="juan@juanreyero.com" }
 ]
 requires-python = ">=3.8"
 license = { file="LICENSE" }
 dependencies = [
-    "clipboard"
+    "clipboard",
+    "tiktoken"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
 dev = [
     "jedi >= 0.18.1",
     "pylint >= 2.13.9",
     "pytest >= 7.0.0",
-    "yapf >= 0.32.0"
+    "yapf >= 0.32.0",
+    "build",
+    "twine"
 ]
 
 [project.scripts]
 catprompt = "catprompt:prompter.main"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=build --ignore=doc --ignore=flymake"
```

### Comparing `catprompt-0.0.2/test/test_prompter.py` & `catprompt-0.0.3/test/test_prompter.py`

 * *Files identical despite different names*

