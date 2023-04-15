# Comparing `tmp/jinja2_orderblocks-0.1.0.tar.gz` & `tmp/jinja2_orderblocks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jinja2_orderblocks-0.1.0.tar", last modified: Sun Oct 30 17:58:42 2016, max compression
+gzip compressed data, was "dist/jinja2_orderblocks-0.1.1.tar", last modified: Sat Apr 15 21:18:23 2023, max compression
```

## Comparing `jinja2_orderblocks-0.1.0.tar` & `jinja2_orderblocks-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 graham    (1000) users      (100)        0 2016-10-30 17:58:42.000000 jinja2_orderblocks-0.1.0/
--rw-r--r--   0 graham    (1000) users      (100)      768 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/setup.py
--rw-r--r--   0 graham    (1000) users      (100)       41 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/CHANGES.txt
-drwxr-xr-x   0 graham    (1000) users      (100)        0 2016-10-30 17:58:42.000000 jinja2_orderblocks-0.1.0/lib/
-drwxr-xr-x   0 graham    (1000) users      (100)        0 2016-10-30 17:58:42.000000 jinja2_orderblocks-0.1.0/lib/jinja2_orderblocks/
--rw-r--r--   0 graham    (1000) users      (100)     3314 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/lib/jinja2_orderblocks/orderblocks.py
--rw-r--r--   0 graham    (1000) users      (100)       77 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/lib/jinja2_orderblocks/__init__.py
-drwxr-xr-x   0 graham    (1000) users      (100)        0 2016-10-30 17:58:42.000000 jinja2_orderblocks-0.1.0/test/
--rw-r--r--   0 graham    (1000) users      (100)     2167 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/test/test_orderblocks.py
--rw-r--r--   0 graham    (1000) users      (100)       98 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/MANIFEST.in
--rw-r--r--   0 graham    (1000) users      (100)    35147 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/COPYING
--rw-r--r--   0 graham    (1000) users      (100)     7407 2016-10-30 17:58:42.000000 jinja2_orderblocks-0.1.0/PKG-INFO
--rw-r--r--   0 graham    (1000) users      (100)     5416 2016-10-30 17:58:02.000000 jinja2_orderblocks-0.1.0/README.rst
+drwxr-xr-x   0 graham    (1000) users      (100)        0 2023-04-15 21:18:23.000000 jinja2_orderblocks-0.1.1/
+drwxr-xr-x   0 graham    (1000) users      (100)        0 2023-04-15 21:18:23.000000 jinja2_orderblocks-0.1.1/lib/
+drwxr-xr-x   0 graham    (1000) users      (100)        0 2023-04-15 21:18:23.000000 jinja2_orderblocks-0.1.1/lib/jinja2_orderblocks/
+-rw-r--r--   0 graham    (1000) users      (100)       77 2023-04-15 20:04:16.000000 jinja2_orderblocks-0.1.1/lib/jinja2_orderblocks/__init__.py
+-rw-r--r--   0 graham    (1000) users      (100)     3323 2023-04-15 21:13:52.000000 jinja2_orderblocks-0.1.1/lib/jinja2_orderblocks/orderblocks.py
+drwxr-xr-x   0 graham    (1000) users      (100)        0 2023-04-15 21:18:23.000000 jinja2_orderblocks-0.1.1/test/
+-rw-r--r--   0 graham    (1000) users      (100)     2167 2023-04-15 20:51:59.000000 jinja2_orderblocks-0.1.1/test/test_orderblocks.py
+-rw-r--r--   0 graham    (1000) users      (100)      108 2023-04-15 21:13:52.000000 jinja2_orderblocks-0.1.1/CHANGES.txt
+-rw-r--r--   0 graham    (1000) users      (100)    35147 2023-04-15 20:04:16.000000 jinja2_orderblocks-0.1.1/COPYING
+-rw-r--r--   0 graham    (1000) users      (100)       98 2023-04-15 20:04:16.000000 jinja2_orderblocks-0.1.1/MANIFEST.in
+-rw-r--r--   0 graham    (1000) users      (100)     5520 2023-04-15 21:13:52.000000 jinja2_orderblocks-0.1.1/README.rst
+-rw-r--r--   0 graham    (1000) users      (100)      768 2023-04-15 21:13:52.000000 jinja2_orderblocks-0.1.1/setup.py
+-rw-r--r--   0 graham    (1000) users      (100)     7527 2023-04-15 21:18:23.000000 jinja2_orderblocks-0.1.1/PKG-INFO
```

### Comparing `jinja2_orderblocks-0.1.0/lib/jinja2_orderblocks/orderblocks.py` & `jinja2_orderblocks-0.1.1/lib/jinja2_orderblocks/orderblocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # OrderBlocks extension for Jinja2
-# Copyright (C) 2016 Graham Bell
+# Copyright (C) 2016-2023 Graham Bell
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -59,15 +59,15 @@
         for node in parser.parse_statements(['name:endorderblocks'],
                                             drop_needle=True):
             if isinstance(node, nodes.Block):
                 blocks.append(nodes.If(
                     nodes.Compare(
                         block_name,
                         [nodes.Operand('eq', nodes.Const(node.name))]),
-                    [node], []))
+                    [node], [], []))
 
                 block_names.append(node.name)
 
         # Make a "For" node iterating over the given block selection.  If the
         # block selection is undefined or None then use the original ordering.
         return nodes.For(
             block_name,
```

### Comparing `jinja2_orderblocks-0.1.0/test/test_orderblocks.py` & `jinja2_orderblocks-0.1.1/test/test_orderblocks.py`

 * *Files identical despite different names*

### Comparing `jinja2_orderblocks-0.1.0/COPYING` & `jinja2_orderblocks-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `jinja2_orderblocks-0.1.0/PKG-INFO` & `jinja2_orderblocks-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 1.1
 Name: jinja2_orderblocks
-Version: 0.1.0
+Version: 0.1.1
 Summary: OrderBlocks Extension for Jinja2
 Home-page: http://github.com/grahambell/jinja2-orderblocks
 Author: Graham Bell
 Author-email: graham.s.bell@gmail.com
 License: UNKNOWN
 Description: OrderBlocks Extension for Jinja2
         ================================
         
         Introduction
         ------------
         
-        This is an extension for the `Jinja2 <http://jinja.pocoo.org/>`_
+        This is an extension for the `Jinja2 <https://palletsprojects.com/p/jinja/>`_
         template engine which allows you to select and reorder inheritance blocks.
         
         
         Example 1: Ordering Specified by Child Template
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         In this example, a website might wish to publish a number of articles.
@@ -81,14 +81,16 @@
         Here a page allows the user to specify which sections
         they wish to see, and their ordering, via a request argument::
         
             from flask import Flask, render_template, request
         
             app = Flask(__name__)
         
+            if 'extensions' not in app.jinja_options:
+                app.jinja_options['extensions'] = []
             app.jinja_options['extensions'].append(
                 'jinja2_orderblocks.OrderBlocks')
         
             @app.route('/example/')
             def example_page():
                 return render_template(
                     'example_template.html',
```

### Comparing `jinja2_orderblocks-0.1.0/README.rst` & `jinja2_orderblocks-0.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 OrderBlocks Extension for Jinja2
 ================================
 
 Introduction
 ------------
 
-This is an extension for the `Jinja2 <http://jinja.pocoo.org/>`_
+This is an extension for the `Jinja2 <https://palletsprojects.com/p/jinja/>`_
 template engine which allows you to select and reorder inheritance blocks.
 
 
 Example 1: Ordering Specified by Child Template
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 In this example, a website might wish to publish a number of articles.
@@ -73,14 +73,16 @@
 Here a page allows the user to specify which sections
 they wish to see, and their ordering, via a request argument::
 
     from flask import Flask, render_template, request
 
     app = Flask(__name__)
 
+    if 'extensions' not in app.jinja_options:
+        app.jinja_options['extensions'] = []
     app.jinja_options['extensions'].append(
         'jinja2_orderblocks.OrderBlocks')
 
     @app.route('/example/')
     def example_page():
         return render_template(
             'example_template.html',
```

