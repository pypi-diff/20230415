# Comparing `tmp/snakeviz-2.1.1.tar.gz` & `tmp/snakeviz-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snakeviz-2.1.1.tar", last modified: Mon Oct 25 00:50:57 2021, max compression
+gzip compressed data, was "dist/snakeviz-2.1.2.tar", last modified: Sat Apr 15 20:22:14 2023, max compression
```

## Comparing `snakeviz-2.1.1.tar` & `snakeviz-2.1.2.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2021-10-25 00:50:57.000000 snakeviz-2.1.1/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     3552 2021-10-25 00:45:15.000000 snakeviz-2.1.1/CHANGES.rst
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1435 2014-11-30 22:30:22.000000 snakeviz-2.1.1/LICENSE.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)      155 2014-11-30 22:30:22.000000 snakeviz-2.1.1/MANIFEST.in
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1985 2021-10-25 00:50:57.000000 snakeviz-2.1.1/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)      901 2021-10-25 00:39:45.000000 snakeviz-2.1.1/README.rst
--rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2021-10-25 00:50:57.000000 snakeviz-2.1.1/setup.cfg
--rwxr-xr-x   0 jiffyclub   (501) staff       (20)     1933 2021-10-25 00:50:16.000000 snakeviz-2.1.1/setup.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       57 2014-10-14 05:02:54.000000 snakeviz-2.1.1/snakeviz/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      192 2018-08-04 21:39:42.000000 snakeviz-2.1.1/snakeviz/__main__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     5807 2020-04-26 23:02:31.000000 snakeviz-2.1.1/snakeviz/cli.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     5331 2020-04-26 23:59:59.000000 snakeviz-2.1.1/snakeviz/ipymagic.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2057 2020-04-26 23:53:30.000000 snakeviz-2.1.1/snakeviz/main.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz/static/
--rw-r--r--   0 jiffyclub   (501) staff       (20)    11428 2021-10-25 00:39:45.000000 snakeviz-2.1.1/snakeviz/static/drawsvg.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1406 2014-10-14 05:02:54.000000 snakeviz-2.1.1/snakeviz/static/favicon.ico
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz/static/images/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1118 2014-10-15 05:48:31.000000 snakeviz-2.1.1/snakeviz/static/images/sort_asc.png
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1136 2014-10-15 05:48:01.000000 snakeviz-2.1.1/snakeviz/static/images/sort_both.png
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1127 2014-10-15 05:48:40.000000 snakeviz-2.1.1/snakeviz/static/images/sort_desc.png
--rw-r--r--   0 jiffyclub   (501) staff       (20)     3533 2021-10-25 00:39:45.000000 snakeviz-2.1.1/snakeviz/static/snakeviz.css
--rw-r--r--   0 jiffyclub   (501) staff       (20)     6756 2017-09-24 04:26:04.000000 snakeviz-2.1.1/snakeviz/static/snakeviz.js
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz/static/vendor/
--rw-r--r--   0 jiffyclub   (501) staff       (20)   151725 2021-01-24 01:16:36.000000 snakeviz-2.1.1/snakeviz/static/vendor/d3.v3.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    57032 2016-06-22 20:04:09.000000 snakeviz-2.1.1/snakeviz/static/vendor/immutable.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    86659 2017-03-20 19:01:15.000000 snakeviz-2.1.1/snakeviz/static/vendor/jquery-3.2.1.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    14112 2017-04-18 08:46:44.000000 snakeviz-2.1.1/snakeviz/static/vendor/jquery.dataTables.min.css
--rw-r--r--   0 jiffyclub   (501) staff       (20)    83268 2017-04-18 08:46:44.000000 snakeviz-2.1.1/snakeviz/static/vendor/jquery.dataTables.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    71419 2016-12-31 17:47:51.000000 snakeviz-2.1.1/snakeviz/static/vendor/lodash.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2175 2017-09-24 04:26:04.000000 snakeviz-2.1.1/snakeviz/stats.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz/templates/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1757 2017-09-27 04:47:30.000000 snakeviz-2.1.1/snakeviz/templates/dir.html
--rw-r--r--   0 jiffyclub   (501) staff       (20)    11485 2021-10-25 00:39:45.000000 snakeviz-2.1.1/snakeviz/templates/viz.html
--rw-r--r--   0 jiffyclub   (501) staff       (20)       31 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz/version.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz.egg-info/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1985 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz.egg-info/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)      924 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz.egg-info/SOURCES.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz.egg-info/dependency_links.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       48 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz.egg-info/entry_points.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       13 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz.egg-info/requires.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)        9 2021-10-25 00:50:57.000000 snakeviz-2.1.1/snakeviz.egg-info/top_level.txt
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     3693 2023-04-15 20:20:00.000000 snakeviz-2.1.2/CHANGES.rst
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1435 2014-11-30 22:30:22.000000 snakeviz-2.1.2/LICENSE.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      155 2014-11-30 22:30:22.000000 snakeviz-2.1.2/MANIFEST.in
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2017 2023-04-15 20:22:14.000000 snakeviz-2.1.2/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      901 2021-10-25 00:39:45.000000 snakeviz-2.1.2/README.rst
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-15 20:22:14.000000 snakeviz-2.1.2/setup.cfg
+-rwxr-xr-x   0 jiffyclub   (501) staff       (20)     2008 2023-04-15 20:21:21.000000 snakeviz-2.1.2/setup.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       57 2014-10-14 05:02:54.000000 snakeviz-2.1.2/snakeviz/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      192 2018-08-04 21:39:42.000000 snakeviz-2.1.2/snakeviz/__main__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     5807 2020-04-26 22:58:54.000000 snakeviz-2.1.2/snakeviz/cli.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     5331 2020-04-26 23:59:59.000000 snakeviz-2.1.2/snakeviz/ipymagic.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2057 2020-04-26 23:53:30.000000 snakeviz-2.1.2/snakeviz/main.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/static/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    11369 2023-04-15 20:14:45.000000 snakeviz-2.1.2/snakeviz/static/drawsvg.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1406 2014-10-14 05:02:54.000000 snakeviz-2.1.2/snakeviz/static/favicon.ico
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/static/images/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1118 2014-10-15 05:48:31.000000 snakeviz-2.1.2/snakeviz/static/images/sort_asc.png
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1136 2014-10-15 05:48:01.000000 snakeviz-2.1.2/snakeviz/static/images/sort_both.png
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1127 2014-10-15 05:48:40.000000 snakeviz-2.1.2/snakeviz/static/images/sort_desc.png
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     5077 2023-04-15 20:14:45.000000 snakeviz-2.1.2/snakeviz/static/snakeviz.css
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     6756 2017-09-24 04:26:04.000000 snakeviz-2.1.2/snakeviz/static/snakeviz.js
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/static/vendor/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)   151725 2021-01-24 01:16:36.000000 snakeviz-2.1.2/snakeviz/static/vendor/d3.v3.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    57032 2016-06-22 20:04:09.000000 snakeviz-2.1.2/snakeviz/static/vendor/immutable.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    86659 2017-03-20 19:01:15.000000 snakeviz-2.1.2/snakeviz/static/vendor/jquery-3.2.1.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    14112 2017-04-18 08:46:44.000000 snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.css
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    83268 2017-04-18 08:46:44.000000 snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    71419 2016-12-31 17:47:51.000000 snakeviz-2.1.2/snakeviz/static/vendor/lodash.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2175 2017-09-24 04:26:04.000000 snakeviz-2.1.2/snakeviz/stats.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/templates/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1757 2017-09-27 04:47:30.000000 snakeviz-2.1.2/snakeviz/templates/dir.html
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    11485 2021-10-25 00:39:45.000000 snakeviz-2.1.2/snakeviz/templates/viz.html
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       31 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz/version.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz.egg-info/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2017 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      947 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       47 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/entry_points.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       13 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/requires.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)        9 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/top_level.txt
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/tests/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2031 2021-10-25 01:35:30.000000 snakeviz-2.1.2/tests/test_snakeviz.py
```

### Comparing `snakeviz-2.1.1/CHANGES.rst` & `snakeviz-2.1.2/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v2.1.2
+===================
+
+* Add dark theme (thanks @martinbagic in #173)
+* Add python-requires metadata (thanks @matthewfeickert in #188)
+
 v2.1.1
 ===================
 
 * Improved styling for snakeviz dropdowns (thanks @dannysepler in #166)
 * Improved performance of the icicle chart (thanks @dannysepler in #165)
 
 v2.1.0
```

### Comparing `snakeviz-2.1.1/LICENSE.txt` & `snakeviz-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/PKG-INFO` & `snakeviz-2.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: snakeviz
-Version: 2.1.1
+Version: 2.1.2
 Summary: A web-based viewer for Python profiler output
 Home-page: https://github.com/jiffyclub/snakeviz
 Author: Matt Davis
 Author-email: jiffyclub@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE.txt
 
 SnakeViz
 ========
 
 .. image:: https://github.com/jiffyclub/snakeviz/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/jiffyclub/snakeviz/actions/workflows/ci.yml
@@ -49,9 +48,7 @@
 -----
 
 SnakeViz is a viewer for Python profiling data that runs as a web
 application in your browser. It is inspired by the wxPython profile viewer
 `RunSnakeRun <http://www.vrplumber.com/programming/runsnakerun/>`_.
 
 View the docs at https://jiffyclub.github.io/snakeviz/.
-
-
```

### Comparing `snakeviz-2.1.1/README.rst` & `snakeviz-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/setup.py` & `snakeviz-2.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 
 import os
 
 
 NAME = 'snakeviz'
-VERSION = '2.1.1'
+VERSION = '2.1.2'
 
 
 # Create a simple version.py module; less trouble than hard-coding the version
 with open(os.path.join('snakeviz', 'version.py'), 'w') as f:
     f.write('__version__ = version = %r' % VERSION)
 
 # Load up the description from README.rst
@@ -33,31 +33,32 @@
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: JavaScript',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development'
     ],
     packages=['snakeviz'],
     package_data={
         'snakeviz': ['static/*.ico',
                      'static/*.js',
                      'static/*.css',
                      'static/vendor/*.js',
                      'static/vendor/*.css',
                      'static/images/*.png',
                      'templates/*.html']
     },
+    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
     install_requires=['tornado>=2.0'],
     entry_points={
         'console_scripts': ['snakeviz = snakeviz.cli:main']
     }
 )
```

### Comparing `snakeviz-2.1.1/snakeviz/cli.py` & `snakeviz-2.1.2/snakeviz/cli.py`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/ipymagic.py` & `snakeviz-2.1.2/snakeviz/ipymagic.py`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/main.py` & `snakeviz-2.1.2/snakeviz/main.py`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/drawsvg.js` & `snakeviz-2.1.2/snakeviz/static/drawsvg.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -250,15 +250,14 @@
         .enter().append("svg:path")
         .attr("id", function(d, i) {
             return "path-" + i;
         })
         .attr("d", params["arc"])
         .attr("fill-rule", "evenodd")
         .style("fill", color)
-        .style("stroke", "#fff")
         .on('click', click)
         .call(apply_mouseover);
 };
 
 var drawIcicle = function drawIcicle(json) {
     params = get_render_params("icicle");
     var nodes = params["partition"].nodes(json).filter(function(d) {
@@ -287,15 +286,14 @@
             return x(d.dx);
         })
         .attr("height", function(d) {
             return y(d.dy);
         })
         .attr("fill-rule", "evenodd")
         .attr("fill", color)
-        .attr("stroke", "#FFF")
         .on('click', click)
         .call(apply_mouseover);
 
     var labels = vis.data([json]).selectAll("text")
         .data(nodes)
         .enter().append("text")
         .attr("x", function(d) {
```

### Comparing `snakeviz-2.1.1/snakeviz/static/favicon.ico` & `snakeviz-2.1.2/snakeviz/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/images/sort_asc.png` & `snakeviz-2.1.2/snakeviz/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/images/sort_both.png` & `snakeviz-2.1.2/snakeviz/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/images/sort_desc.png` & `snakeviz-2.1.2/snakeviz/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/snakeviz.css` & `snakeviz-2.1.2/snakeviz/static/snakeviz.css`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+:root {
+  --dark-theme-white: rgb(200, 200, 200);
+  --dark-theme-gray: #444;
+  --dark-theme-black: #1c1c1c;
+}
+
 body {
   padding: 20px;
 }
 
 button {
   font-family: monospace;
   font-size: 20px;
@@ -222,7 +228,88 @@
     -webkit-transform: scale(1.0);
   }
 }
 
 .dir-listing {
   margin-top: 20px;
 }
+
+g#container rect, g#container path {
+  stroke: #fff;
+}
+
+@media (prefers-color-scheme: dark) {
+  body {
+    background-color: var(--dark-theme-black);
+    color: var(--dark-theme-white);
+  }
+
+  g#container rect, g#container path {
+    stroke: var(--dark-theme-black);
+  }
+
+  #sv-call-stack-list {
+    background: var(--dark-theme-gray);
+  }
+
+  #sv-style-select, #sv-depth-select, #sv-cutoff-select {
+    background: var(--dark-theme-gray);
+    color: var(--dark-theme-white)
+  }
+
+  #sv-style-label {
+    color: var(--dark-theme-white)
+  }
+
+  button {
+    background: var(--dark-theme-gray);
+    border-color: var(--dark-theme-white);
+    color: var(--dark-theme-white);
+  }
+
+  button:hover {
+    background: #555;
+    cursor: pointer;
+  }
+
+  button:disabled {
+    color: rgb(110, 110, 110);
+    border-color: rgb(110, 110, 110);
+  }
+
+  button:disabled:hover {
+    background: #555;
+    cursor: default;
+  }
+
+  #table_div label {
+    color: var(--dark-theme-white);
+  }
+
+  #table_div input {
+    background-color: #666;
+    color: var(--dark-theme-white);
+  }
+
+  #table_div tr {
+    background-color: var(--dark-theme-black);
+  }
+
+  #table_div td.data-table-hover {
+    background-color: #222;
+  }
+
+  #table_div td.sorting_1 {
+    background-color: #282828;
+  }
+
+  #table_div th.sorting {
+    background-color: #333;
+
+  }
+
+  #table_div th.sorting_desc, #table_div th.sorting_asc {
+    background-color: var(--dark-theme-gray);
+
+  }
+
+}
```

### Comparing `snakeviz-2.1.1/snakeviz/static/snakeviz.js` & `snakeviz-2.1.2/snakeviz/static/snakeviz.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/vendor/d3.v3.min.js` & `snakeviz-2.1.2/snakeviz/static/vendor/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/vendor/immutable.min.js` & `snakeviz-2.1.2/snakeviz/static/vendor/immutable.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/vendor/jquery-3.2.1.min.js` & `snakeviz-2.1.2/snakeviz/static/vendor/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/vendor/jquery.dataTables.min.css` & `snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/vendor/jquery.dataTables.min.js` & `snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/static/vendor/lodash.min.js` & `snakeviz-2.1.2/snakeviz/static/vendor/lodash.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/stats.py` & `snakeviz-2.1.2/snakeviz/stats.py`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/templates/dir.html` & `snakeviz-2.1.2/snakeviz/templates/dir.html`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz/templates/viz.html` & `snakeviz-2.1.2/snakeviz/templates/viz.html`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.1/snakeviz.egg-info/PKG-INFO` & `snakeviz-2.1.2/snakeviz.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: snakeviz
-Version: 2.1.1
+Version: 2.1.2
 Summary: A web-based viewer for Python profiler output
 Home-page: https://github.com/jiffyclub/snakeviz
 Author: Matt Davis
 Author-email: jiffyclub@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE.txt
 
 SnakeViz
 ========
 
 .. image:: https://github.com/jiffyclub/snakeviz/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/jiffyclub/snakeviz/actions/workflows/ci.yml
@@ -49,9 +48,7 @@
 -----
 
 SnakeViz is a viewer for Python profiling data that runs as a web
 application in your browser. It is inspired by the wxPython profile viewer
 `RunSnakeRun <http://www.vrplumber.com/programming/runsnakerun/>`_.
 
 View the docs at https://jiffyclub.github.io/snakeviz/.
-
-
```

### Comparing `snakeviz-2.1.1/snakeviz.egg-info/SOURCES.txt` & `snakeviz-2.1.2/snakeviz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 snakeviz/static/vendor/d3.v3.min.js
 snakeviz/static/vendor/immutable.min.js
 snakeviz/static/vendor/jquery-3.2.1.min.js
 snakeviz/static/vendor/jquery.dataTables.min.css
 snakeviz/static/vendor/jquery.dataTables.min.js
 snakeviz/static/vendor/lodash.min.js
 snakeviz/templates/dir.html
-snakeviz/templates/viz.html
+snakeviz/templates/viz.html
+tests/test_snakeviz.py
```

