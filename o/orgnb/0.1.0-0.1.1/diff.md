# Comparing `tmp/orgnb-0.1.0.tar.gz` & `tmp/orgnb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orgnb-0.1.0.tar", last modified: Sat Apr  1 16:25:45 2023, max compression
+gzip compressed data, was "orgnb-0.1.1.tar", last modified: Sat Apr 15 14:02:32 2023, max compression
```

## Comparing `orgnb-0.1.0.tar` & `orgnb-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-04-01 16:25:45.221878 orgnb-0.1.0/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        0 2019-05-09 15:14:08.000000 orgnb-0.1.0/LICENSE
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      927 2023-04-01 16:25:45.221878 orgnb-0.1.0/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      424 2023-04-01 16:13:01.000000 orgnb-0.1.0/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-04-01 16:25:45.221878 orgnb-0.1.0/orgnb.egg-info/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      927 2023-04-01 16:25:45.000000 orgnb-0.1.0/orgnb.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      217 2023-04-01 16:25:45.000000 orgnb-0.1.0/orgnb.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-04-01 16:25:45.000000 orgnb-0.1.0/orgnb.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       36 2023-04-01 16:25:45.000000 orgnb-0.1.0/orgnb.egg-info/entry_points.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       30 2023-04-01 16:25:45.000000 orgnb-0.1.0/orgnb.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        6 2023-04-01 16:25:45.000000 orgnb-0.1.0/orgnb.egg-info/top_level.txt
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)     6185 2023-04-01 16:02:09.000000 orgnb-0.1.0/orgnb.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1073 2023-04-01 16:25:12.000000 orgnb-0.1.0/pyproject.toml
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       38 2023-04-01 16:25:45.221878 orgnb-0.1.0/setup.cfg
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-04-15 14:02:32.877655 orgnb-0.1.1/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        0 2019-05-09 15:14:08.000000 orgnb-0.1.1/LICENSE
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      927 2023-04-15 14:02:32.877655 orgnb-0.1.1/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      424 2023-04-01 16:13:01.000000 orgnb-0.1.1/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-04-15 14:02:32.877655 orgnb-0.1.1/orgnb.egg-info/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      927 2023-04-15 14:02:32.000000 orgnb-0.1.1/orgnb.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      217 2023-04-15 14:02:32.000000 orgnb-0.1.1/orgnb.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-04-15 14:02:32.000000 orgnb-0.1.1/orgnb.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       36 2023-04-15 14:02:32.000000 orgnb-0.1.1/orgnb.egg-info/entry_points.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       30 2023-04-15 14:02:32.000000 orgnb-0.1.1/orgnb.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        6 2023-04-15 14:02:32.000000 orgnb-0.1.1/orgnb.egg-info/top_level.txt
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)     6253 2023-04-15 13:58:12.000000 orgnb-0.1.1/orgnb.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1145 2023-04-15 14:00:59.000000 orgnb-0.1.1/pyproject.toml
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       38 2023-04-15 14:02:32.877655 orgnb-0.1.1/setup.cfg
```

### Comparing `orgnb-0.1.0/PKG-INFO` & `orgnb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orgnb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convert org-mode files to jupyter notebooks
 Author-email: Daniele Coslovich <dcoslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/coslo/orgnb
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `orgnb-0.1.0/orgnb.egg-info/PKG-INFO` & `orgnb-0.1.1/orgnb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orgnb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convert org-mode files to jupyter notebooks
 Author-email: Daniele Coslovich <dcoslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/coslo/orgnb
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `orgnb-0.1.0/orgnb.py` & `orgnb-0.1.1/orgnb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python
 
-import base64, re, os
+import base64
+import re
+import os
 
 """
 Convert org mode file as jupyter notebook.
 """
 
 # The following does not transform code blocks into code cells
 # output = pypandoc.convert_file(sys.argv[1],
@@ -64,24 +66,24 @@
             # unless all lines are empty
             non_empty = sum([len(_) > 0 for _ in block])
             if non_empty > 0:
                 cells.append(block)
                 cells_type.append('text')
             # Reading a new code block
             if line.startswith('#+begin'):
-                state = line[8: ]  # strip #+begin
+                state = line[8:]  # strip #+begin
                 if len(line.split()) > 1:
                     state = line.split()[1]
-                
+
             block = []
 
         elif line.startswith('#+end'):
             # We store the current block as code
             assert state != 'text'
-            if state == 'example' or state == 'quote':
+            if state in ['example', 'quote']:
                 block.insert(0, '```')
                 block.append('```')
             cells.append(block)
             cells_type.append(state)
             # Reading a new text block. If there are consecutive code
             # blocks, empty text blocks are removed.
             state = 'text'
@@ -157,14 +159,16 @@
         if (include and t not in include) or (exclude and t in exclude):
             continue
         if t == 'text':
             # This is a text block
             from pypandoc import convert_text
             block = '\n'.join(e)
             block = convert_text(block, 'markdown-simple_tables+grid_tables', 'org')
+            # Fix generic verbatim code blocks
+            block = re.sub('\{.verbatim\}', '', block)
             block, attachments = attach_images(block, dir_inp)
             nb['cells'].append(nbformat.v4.new_markdown_cell(source=block, attachments=attachments))
         elif t == 'python':
             # This is a python code block
             block = '\n'.join(e)
             nb['cells'].append(nbformat.v4.new_code_cell(source=block))
         elif t == 'sh':
@@ -179,25 +183,25 @@
     nbformat.write(nb, file_out)
 
 
 def main(debug=False, include='', exclude='ditaa', *files):
     convert = convert_to_nb
     if debug:
         convert = convert_to_text
-        
+
     for file_inp in files:
         if debug:
             file_out = '/dev/stdout'
         else:
             file_out = file_inp[:-4] + '.ipynb'
         with open(file_inp) as fh:
             cells, cells_type = parse_org_file(fh)
             convert(cells, cells_type, file_out, os.path.dirname(fh.name), include, exclude)
 
 def cli():
     import argh
     argh.dispatch_command(main)
 
-            
+
 if __name__ == '__main__':
     import argh
     argh.dispatch_command(main)
```

### Comparing `orgnb-0.1.0/pyproject.toml` & `orgnb-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 # https://github.com/pypa/sampleproject/blob/main/pyproject.toml
 
 [project]
 name = "orgnb"
 description = "Convert org-mode files to jupyter notebooks"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Daniele Coslovich", email = "dcoslovich@umontpellier.fr"}
 ]
 requires-python = ">=3.6"
 license = {text = "GPLv3"}
 dependencies = [
     'pypandoc_binary',
@@ -32,8 +32,12 @@
 # The following would provide a command line executable called `mypackage`
 # which executes the function `cli.main` from this package when invoked.
 [project.scripts]
 orgnb = "orgnb:cli"
 
 # [build-system]
 # requires = ["setuptools>=61.0"]
-# build-backend = "setuptools.build_meta"
+# build-backend = "setuptools.build_meta"
+
+# pip install build
+# python -m build
+# python -m twine upload dist/*
```

