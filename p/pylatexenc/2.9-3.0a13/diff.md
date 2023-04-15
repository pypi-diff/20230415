# Comparing `tmp/pylatexenc-2.9.tar.gz` & `tmp/pylatexenc-3.0a13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylatexenc-2.9.tar", last modified: Wed Mar  3 09:52:04 2021, max compression
+gzip compressed data, was "pylatexenc-3.0a13.tar", max compression
```

## Comparing `pylatexenc-2.9.tar` & `pylatexenc-3.0a13.tar`

### file list

```diff
@@ -1,43 +1,59 @@
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/
--rw-r--r--   0 philippe   (501) staff       (20)     1086 2019-07-27 15:08:32.000000 pylatexenc-2.9/LICENSE.txt
--rw-r--r--   0 philippe   (501) staff       (20)      105 2020-04-18 11:54:48.000000 pylatexenc-2.9/MANIFEST.in
--rw-r--r--   0 philippe   (501) staff       (20)     4277 2021-03-03 09:52:04.000000 pylatexenc-2.9/PKG-INFO
--rw-r--r--   0 philippe   (501) staff       (20)     2730 2020-04-18 11:52:40.000000 pylatexenc-2.9/README.rst
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc/
--rw-r--r--   0 philippe   (501) staff       (20)     1326 2019-07-25 20:20:56.000000 pylatexenc-2.9/pylatexenc/__init__.py
--rw-r--r--   0 philippe   (501) staff       (20)     5256 2019-08-19 21:09:13.000000 pylatexenc-2.9/pylatexenc/_util.py
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc/latex2text/
--rw-r--r--   0 philippe   (501) staff       (20)    59832 2020-10-29 21:43:44.000000 pylatexenc-2.9/pylatexenc/latex2text/__init__.py
--rw-r--r--   0 philippe   (501) staff       (20)     9480 2020-04-18 11:45:07.000000 pylatexenc-2.9/pylatexenc/latex2text/__main__.py
--rw-r--r--   0 philippe   (501) staff       (20)    92533 2021-02-26 15:05:37.000000 pylatexenc-2.9/pylatexenc/latex2text/_defaultspecs.py
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc/latexencode/
--rw-r--r--   0 philippe   (501) staff       (20)    34510 2020-09-09 22:08:35.000000 pylatexenc-2.9/pylatexenc/latexencode/__init__.py
--rw-r--r--   0 philippe   (501) staff       (20)     4426 2019-08-25 13:06:29.000000 pylatexenc-2.9/pylatexenc/latexencode/__main__.py
--rw-r--r--   0 philippe   (501) staff       (20)    99772 2021-01-06 14:31:48.000000 pylatexenc-2.9/pylatexenc/latexencode/_uni2latexmap.py
--rw-r--r--   0 philippe   (501) staff       (20)    55947 2019-07-27 15:08:32.000000 pylatexenc-2.9/pylatexenc/latexencode/_uni2latexmap_xml.py
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc/latexwalker/
--rw-r--r--   0 philippe   (501) staff       (20)   106850 2021-03-01 22:35:09.000000 pylatexenc-2.9/pylatexenc/latexwalker/__init__.py
--rw-r--r--   0 philippe   (501) staff       (20)     6213 2020-11-18 11:17:52.000000 pylatexenc-2.9/pylatexenc/latexwalker/__main__.py
--rw-r--r--   0 philippe   (501) staff       (20)    14955 2021-02-03 21:15:42.000000 pylatexenc-2.9/pylatexenc/latexwalker/_defaultspecs.py
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc/macrospec/
--rw-r--r--   0 philippe   (501) staff       (20)    31011 2019-08-19 10:02:58.000000 pylatexenc-2.9/pylatexenc/macrospec/__init__.py
--rw-r--r--   0 philippe   (501) staff       (20)    19210 2021-01-06 15:27:39.000000 pylatexenc-2.9/pylatexenc/macrospec/_argparsers.py
--rw-r--r--   0 philippe   (501) staff       (20)     2043 2021-03-03 09:45:19.000000 pylatexenc-2.9/pylatexenc/version.py
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc.egg-info/
--rw-r--r--   0 philippe   (501) staff       (20)     4277 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc.egg-info/PKG-INFO
--rw-r--r--   0 philippe   (501) staff       (20)      924 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc.egg-info/SOURCES.txt
--rw-r--r--   0 philippe   (501) staff       (20)        1 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc.egg-info/dependency_links.txt
--rw-r--r--   0 philippe   (501) staff       (20)      170 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc.egg-info/entry_points.txt
--rw-r--r--   0 philippe   (501) staff       (20)       11 2021-03-03 09:52:04.000000 pylatexenc-2.9/pylatexenc.egg-info/top_level.txt
--rw-r--r--   0 philippe   (501) staff       (20)       38 2021-03-03 09:52:04.000000 pylatexenc-2.9/setup.cfg
--rw-r--r--   0 philippe   (501) staff       (20)     2869 2019-08-22 14:28:39.000000 pylatexenc-2.9/setup.py
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/test/
-drwxr-xr-x   0 philippe   (501) staff       (20)        0 2021-03-03 09:52:04.000000 pylatexenc-2.9/test/dummy/
--rw-r--r--   0 philippe   (501) staff       (20)      108 2017-04-24 20:37:45.000000 pylatexenc-2.9/test/dummy/readme.txt
--rw-r--r--   0 philippe   (501) staff       (20)      128 2017-04-24 20:37:45.000000 pylatexenc-2.9/test/test_input_1.tex
--rw-r--r--   0 philippe   (501) staff       (20)    20423 2020-10-29 16:32:28.000000 pylatexenc-2.9/test/test_latex2text.py
--rw-r--r--   0 philippe   (501) staff       (20)    13075 2020-09-09 22:15:16.000000 pylatexenc-2.9/test/test_latexencode.py
--rw-r--r--   0 philippe   (501) staff       (20)     3173 2020-07-04 21:17:45.000000 pylatexenc-2.9/test/test_latexencode_all.py
--rw-r--r--   0 philippe   (501) staff       (20)    67196 2021-03-01 22:38:07.000000 pylatexenc-2.9/test/test_latexwalker.py
--rw-r--r--   0 philippe   (501) staff       (20)    24001 2019-08-06 18:40:55.000000 pylatexenc-2.9/test/test_macrospec.py
--rw-r--r--   0 philippe   (501) staff       (20)   131010 2021-01-06 14:54:51.000000 pylatexenc-2.9/test/uni_chars_test_previous.txt
+-rw-r--r--   0        0        0     1086 2023-04-15 13:24:30.143033 pylatexenc-3.0a13/LICENSE.txt
+-rw-r--r--   0        0        0     2830 2023-04-15 11:30:13.187333 pylatexenc-3.0a13/README.rst
+-rw-r--r--   0        0        0     1326 2019-07-25 20:20:56.000000 pylatexenc-3.0a13/pylatexenc/__init__.py
+-rw-r--r--   0        0        0     5162 2023-04-15 11:29:53.841130 pylatexenc-3.0a13/pylatexenc/_util.py
+-rw-r--r--   0        0        0     3766 2023-04-15 11:29:53.841423 pylatexenc-3.0a13/pylatexenc/_util_support.py
+-rw-r--r--   0        0        0    59269 2023-04-15 11:57:13.282343 pylatexenc-3.0a13/pylatexenc/latex2text/__init__.py
+-rw-r--r--   0        0        0    10011 2023-04-15 11:55:00.471421 pylatexenc-3.0a13/pylatexenc/latex2text/__main__.py
+-rw-r--r--   0        0        0    94342 2023-04-15 11:29:53.843500 pylatexenc-3.0a13/pylatexenc/latex2text/_defaultspecs.py
+-rw-r--r--   0        0        0     2526 2021-12-17 19:22:56.000000 pylatexenc-3.0a13/pylatexenc/latex2text/_inputlatexfile.py
+-rw-r--r--   0        0        0    12944 2021-03-31 23:28:40.000000 pylatexenc-3.0a13/pylatexenc/latexencode/__init__.py
+-rw-r--r--   0        0        0     4426 2019-08-25 13:06:29.000000 pylatexenc-3.0a13/pylatexenc/latexencode/__main__.py
+-rw-r--r--   0        0        0     4404 2023-04-15 12:03:11.103995 pylatexenc-3.0a13/pylatexenc/latexencode/_partial_latex_encoder.py
+-rw-r--r--   0        0        0    99833 2021-09-15 19:08:59.000000 pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap.py
+-rw-r--r--   0        0        0    55947 2019-07-27 15:08:32.000000 pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap_xml.py
+-rw-r--r--   0        0        0    26209 2021-04-01 11:51:30.000000 pylatexenc-3.0a13/pylatexenc/latexencode/_unicode_to_latex_encoder.py
+-rw-r--r--   0        0        0     2179 2023-04-15 11:29:53.843788 pylatexenc-3.0a13/pylatexenc/latexnodes/__init__.py
+-rw-r--r--   0        0        0     2088 2023-04-15 11:29:53.844020 pylatexenc-3.0a13/pylatexenc/latexnodes/_callablespecbase.py
+-rw-r--r--   0        0        0    10957 2023-04-15 11:29:53.844375 pylatexenc-3.0a13/pylatexenc/latexnodes/_exctypes.py
+-rw-r--r--   0        0        0     6203 2023-04-15 11:29:53.844620 pylatexenc-3.0a13/pylatexenc/latexnodes/_latexcontextdbbase.py
+-rw-r--r--   0        0        0    36350 2023-04-15 11:29:53.845057 pylatexenc-3.0a13/pylatexenc/latexnodes/_nodescollector.py
+-rw-r--r--   0        0        0    10124 2023-04-15 11:29:53.845301 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsedargs.py
+-rw-r--r--   0        0        0    11877 2023-04-15 11:29:53.845584 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsedargsinfo.py
+-rw-r--r--   0        0        0    17301 2023-04-15 11:29:53.845881 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsingstate.py
+-rw-r--r--   0        0        0     7109 2023-04-15 11:29:53.846228 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsingstatedelta.py
+-rw-r--r--   0        0        0     8145 2023-04-15 11:29:53.846477 pylatexenc-3.0a13/pylatexenc/latexnodes/_token.py
+-rw-r--r--   0        0        0    27323 2023-04-15 11:29:53.846903 pylatexenc-3.0a13/pylatexenc/latexnodes/_tokenreader.py
+-rw-r--r--   0        0        0     9984 2023-04-15 11:29:53.847231 pylatexenc-3.0a13/pylatexenc/latexnodes/_tokenreaderbase.py
+-rw-r--r--   0        0        0     3711 2023-04-15 11:29:53.847509 pylatexenc-3.0a13/pylatexenc/latexnodes/_walkerbase.py
+-rw-r--r--   0        0        0    41971 2023-04-15 11:29:53.847946 pylatexenc-3.0a13/pylatexenc/latexnodes/nodes.py
+-rw-r--r--   0        0        0     2141 2023-04-15 11:29:53.848262 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/__init__.py
+-rw-r--r--   0        0        0     5285 2023-04-15 11:29:53.848639 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_base.py
+-rw-r--r--   0        0        0    41018 2023-04-15 11:29:53.849003 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_delimited.py
+-rw-r--r--   0        0        0    18288 2023-04-15 11:29:53.849524 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_expression.py
+-rw-r--r--   0        0        0    12896 2023-04-15 11:29:53.849773 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_generalnodes.py
+-rw-r--r--   0        0        0     5658 2023-04-15 11:29:53.849985 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_math.py
+-rw-r--r--   0        0        0     6180 2023-04-15 11:29:53.850252 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_optionals.py
+-rw-r--r--   0        0        0    22366 2023-04-15 11:29:53.850621 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_stdarg.py
+-rw-r--r--   0        0        0    11290 2023-04-15 11:29:53.850847 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_verbatim.py
+-rw-r--r--   0        0        0     4520 2023-04-15 11:29:53.851132 pylatexenc-3.0a13/pylatexenc/latexwalker/__init__.py
+-rw-r--r--   0        0        0     6214 2023-04-15 11:29:53.851406 pylatexenc-3.0a13/pylatexenc/latexwalker/__main__.py
+-rw-r--r--   0        0        0    17383 2023-04-15 11:29:53.851774 pylatexenc-3.0a13/pylatexenc/latexwalker/_defaultspecs.py
+-rw-r--r--   0        0        0     2937 2023-04-15 11:29:53.852111 pylatexenc-3.0a13/pylatexenc/latexwalker/_get_defaultspecs.py
+-rw-r--r--   0        0        0     7833 2023-04-15 11:29:53.852354 pylatexenc-3.0a13/pylatexenc/latexwalker/_helpers.py
+-rw-r--r--   0        0        0     7487 2023-04-15 11:29:53.852626 pylatexenc-3.0a13/pylatexenc/latexwalker/_legacy_py1x.py
+-rw-r--r--   0        0        0    52642 2023-04-15 11:37:07.707893 pylatexenc-3.0a13/pylatexenc/latexwalker/_walker.py
+-rw-r--r--   0        0        0     2341 2023-04-15 11:29:53.853314 pylatexenc-3.0a13/pylatexenc/macrospec/__init__.py
+-rw-r--r--   0        0        0     8525 2023-04-15 11:29:53.853602 pylatexenc-3.0a13/pylatexenc/macrospec/_argumentsparser.py
+-rw-r--r--   0        0        0     7372 2023-04-15 11:29:53.853904 pylatexenc-3.0a13/pylatexenc/macrospec/_environmentbodyparser.py
+-rw-r--r--   0        0        0    29706 2023-04-15 11:29:53.854223 pylatexenc-3.0a13/pylatexenc/macrospec/_latexcontextdb.py
+-rw-r--r--   0        0        0    10045 2023-04-15 11:29:53.854565 pylatexenc-3.0a13/pylatexenc/macrospec/_macrocallparser.py
+-rw-r--r--   0        0        0     1535 2023-04-15 11:29:53.854841 pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
+-rw-r--r--   0        0        0     8866 2023-04-15 11:29:53.855062 pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
+-rw-r--r--   0        0        0    16112 2023-04-15 11:29:53.855268 pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
+-rw-r--r--   0        0        0    15650 2023-04-15 11:29:53.855594 pylatexenc-3.0a13/pylatexenc/macrospec/_specclasses.py
+-rw-r--r--   0        0        0     8951 2023-04-15 11:29:53.855874 pylatexenc-3.0a13/pylatexenc/macrospec/_spechelpers.py
+-rw-r--r--   0        0        0     2054 2023-04-15 13:21:15.064333 pylatexenc-3.0a13/pylatexenc/version.py
+-rw-r--r--   0        0        0     1091 2023-04-15 13:21:32.120070 pylatexenc-3.0a13/pyproject.toml
+-rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 pylatexenc-3.0a13/setup.py
+-rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 pylatexenc-3.0a13/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylatexenc-2.9/LICENSE.txt` & `pylatexenc-3.0a13/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2015-2019 Philippe Faist
+Copyright (c) 2015-2023 Philippe Faist
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pylatexenc-2.9/PKG-INFO` & `pylatexenc-3.0a13/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,39 @@
-Metadata-Version: 1.1
-Name: pylatexenc
-Version: 2.9
-Summary: Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
-Home-page: https://github.com/phfaist/pylatexenc
-Author: Philippe Faist
-Author-email: philippe.faist@bluewin.ch
-License: MIT
-Description: pylatexenc
-        ==========
-        
-        Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
-        
-        .. image:: https://img.shields.io/github/license/phfaist/pylatexenc.svg?style=flat
-           :target: https://github.com/phfaist/pylatexenc/blob/master/LICENSE.txt
-        
-        .. image:: https://img.shields.io/travis/phfaist/pylatexenc.svg?style=flat
-           :target: https://travis-ci.org/phfaist/pylatexenc
-           
-        .. image:: https://img.shields.io/pypi/v/pylatexenc.svg?style=flat
-           :target: https://pypi.org/project/pylatexenc/
-        
-        .. image:: https://img.shields.io/lgtm/alerts/g/phfaist/pylatexenc.svg?logo=lgtm&logoWidth=18&style=flat
-           :target: https://lgtm.com/projects/g/phfaist/pylatexenc/alerts/
-        
-        
-        Unicode Text to LaTeX code
-        --------------------------
-        
-        The ``pylatexenc.latexencode`` module provides a function ``unicode_to_latex()``
-        which converts a unicode string into LaTeX text and escape sequences. It should
-        recognize accented characters and most math symbols. A couple of switches allow
-        you to alter how this function behaves.
-        
-        You can also run ``latexencode`` in command-line to convert plain unicode text
-        (from the standard input or from files given on the command line) into LaTeX
-        code, written on to the standard output.
-        
-        A third party plug-in for Vim
-        `vim-latexencode <https://github.com/Konfekt/vim-latexencode>`_
-        by `@Konfekt <https://github.com/Konfekt>`_
-        provides a corresponding command to operate on a given range.
-        
-        
-        Parsing LaTeX code & converting to plain text (unicode)
-        -------------------------------------------------------
-        
-        The ``pylatexenc.latexwalker`` module provides a series of routines that parse
-        the LaTeX structure of given LaTeX code and returns a logical structure of
-        objects, which can then be used to produce output in another format such as
-        plain text.  This is not a replacement for a full (La)TeX engine, rather, this
-        module provides a way to parse a chunk of LaTeX code as mark-up code.
-        
-        The ``pylatexenc.latex2text`` module builds up on top of
-        ``pylatexenc.latexwalker`` and provides functions to convert given LaTeX code to
-        plain text with unicode characters.
-        
-        You can also run ``latex2text`` in command-line to convert LaTeX input (either
-        from the standard input, or from files given on the command line) into plain
-        text written on the standard output.
-        
-        
-        Documentation
-        -------------
-        
-        Full documentation is available at https://pylatexenc.readthedocs.io/.
-        
-        
-        License
-        -------
-        
-        See LICENSE.txt (MIT License).
-        
-        NOTE: See copyright notice and license information for file
-        ``tools/unicode.xml`` provided in ``tools/unicode.xml.LICENSE``.  (The file
-        ``tools/unicode.xml`` was downloaded from
-        https://www.w3.org/2003/entities/2007xml/unicode.xml as linked from
-        https://www.w3.org/TR/xml-entity-names/#source.)
-        
-Keywords: latex text unicode encode parse expression
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Markup :: LaTeX
+# -*- coding: utf-8 -*-
+from setuptools import setup
+
+packages = \
+['pylatexenc',
+ 'pylatexenc.latex2text',
+ 'pylatexenc.latexencode',
+ 'pylatexenc.latexnodes',
+ 'pylatexenc.latexnodes.parsers',
+ 'pylatexenc.latexwalker',
+ 'pylatexenc.macrospec',
+ 'pylatexenc.macrospec._pyltxenc2_argparsers']
+
+package_data = \
+{'': ['*']}
+
+entry_points = \
+{'console_scripts': ['latex2text = pylatexenc.latex2text.__main__:main',
+                     'latexencode = pylatexenc.latexencode.__main__:main',
+                     'latexwalker = pylatexenc.latexwalker.__main__:main']}
+
+setup_kwargs = {
+    'name': 'pylatexenc',
+    'version': '3.0a13',
+    'description': 'Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion',
+    'long_description': "pylatexenc\n==========\n\nSimple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion\n\n.. image:: https://img.shields.io/github/license/phfaist/pylatexenc.svg?style=flat\n   :target: https://github.com/phfaist/pylatexenc/blob/master/LICENSE.txt\n\n.. image:: https://img.shields.io/pypi/v/pylatexenc.svg?style=flat\n   :target: https://pypi.org/project/pylatexenc/\n\nPython: ≥ 3.4 or ≥ 2.7. The library is designed to be as backwards-compatible as\nreasonably possible and is able to run on old python verisons should it be\nnecessary. (Use the setup.py script directly if you have python<3.7, poetry\ndoesn't seem to work with old python versions.)\n\n\nUnicode Text to LaTeX code\n--------------------------\n\nThe ``pylatexenc.latexencode`` module provides a function ``unicode_to_latex()``\nwhich converts a unicode string into LaTeX text and escape sequences. It should\nrecognize accented characters and most math symbols. A couple of switches allow\nyou to alter how this function behaves.\n\nYou can also run ``latexencode`` in command-line to convert plain unicode text\n(from the standard input or from files given on the command line) into LaTeX\ncode, written on to the standard output.\n\nA third party plug-in for Vim\n`vim-latexencode <https://github.com/Konfekt/vim-latexencode>`_\nby `@Konfekt <https://github.com/Konfekt>`_\nprovides a corresponding command to operate on a given range.\n\n\nParsing LaTeX code & converting to plain text (unicode)\n-------------------------------------------------------\n\nThe ``pylatexenc.latexwalker`` module provides a series of routines that parse\nthe LaTeX structure of given LaTeX code and returns a logical structure of\nobjects, which can then be used to produce output in another format such as\nplain text.  This is not a replacement for a full (La)TeX engine, rather, this\nmodule provides a way to parse a chunk of LaTeX code as mark-up code.\n\nThe ``pylatexenc.latex2text`` module builds up on top of\n``pylatexenc.latexwalker`` and provides functions to convert given LaTeX code to\nplain text with unicode characters.\n\nYou can also run ``latex2text`` in command-line to convert LaTeX input (either\nfrom the standard input, or from files given on the command line) into plain\ntext written on the standard output.\n\n\nDocumentation\n-------------\n\nFull documentation is available at https://pylatexenc.readthedocs.io/.\n\nTo build the documentation manually, run::\n\n  > poetry install --with=builddoc\n  > cd doc/\n  doc> poetry run make html\n\n\nLicense\n-------\n\nSee LICENSE.txt (MIT License).\n\nNOTE: See copyright notice and license information for file\n``tools/unicode.xml`` provided in ``tools/unicode.xml.LICENSE``.  (The file\n``tools/unicode.xml`` was downloaded from\nhttps://www.w3.org/2003/entities/2007xml/unicode.xml as linked from\nhttps://www.w3.org/TR/xml-entity-names/#source.)\n",
+    'author': 'Philippe Faist',
+    'author_email': 'philippe.faist@bluewin.ch',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'packages': packages,
+    'package_data': package_data,
+    'entry_points': entry_points,
+    'python_requires': '>=3.7,<4.0',
+}
+
+
+setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pylatexenc-2.9/README.rst` & `pylatexenc-3.0a13/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 ==========
 
 Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
 
 .. image:: https://img.shields.io/github/license/phfaist/pylatexenc.svg?style=flat
    :target: https://github.com/phfaist/pylatexenc/blob/master/LICENSE.txt
 
-.. image:: https://img.shields.io/travis/phfaist/pylatexenc.svg?style=flat
-   :target: https://travis-ci.org/phfaist/pylatexenc
-   
 .. image:: https://img.shields.io/pypi/v/pylatexenc.svg?style=flat
    :target: https://pypi.org/project/pylatexenc/
 
-.. image:: https://img.shields.io/lgtm/alerts/g/phfaist/pylatexenc.svg?logo=lgtm&logoWidth=18&style=flat
-   :target: https://lgtm.com/projects/g/phfaist/pylatexenc/alerts/
+Python: ≥ 3.4 or ≥ 2.7. The library is designed to be as backwards-compatible as
+reasonably possible and is able to run on old python verisons should it be
+necessary. (Use the setup.py script directly if you have python<3.7, poetry
+doesn't seem to work with old python versions.)
 
 
 Unicode Text to LaTeX code
 --------------------------
 
 The ``pylatexenc.latexencode`` module provides a function ``unicode_to_latex()``
 which converts a unicode string into LaTeX text and escape sequences. It should
@@ -53,14 +52,20 @@
 
 
 Documentation
 -------------
 
 Full documentation is available at https://pylatexenc.readthedocs.io/.
 
+To build the documentation manually, run::
+
+  > poetry install --with=builddoc
+  > cd doc/
+  doc> poetry run make html
+
 
 License
 -------
 
 See LICENSE.txt (MIT License).
 
 NOTE: See copyright notice and license information for file
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pylatexenc-2.9/pylatexenc/__init__.py` & `pylatexenc-3.0a13/pylatexenc/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-2.9/pylatexenc/_util.py` & `pylatexenc-3.0a13/pylatexenc/_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,116 +24,33 @@
 #
 
 
 # Internal module. Internal API may move, disappear or otherwise change at any
 # time and without notice.
 
 
-try:
-    # Python >= 3.3
-    from collections.abc import MutableMapping
-except ImportError:
-    from collections import MutableMapping
-
-import warnings
 import bisect
+bisect_right = bisect.bisect_right
 
 
 # ------------------------------------------------------------------------------
 
 
-
-def pylatexenc_deprecated_ver(ver, msg, stacklevel=2):
-    warnings.warn(
-        "Deprecated (pylatexenc {}): {} ".format(ver, msg.strip()),
-        DeprecationWarning,
-        stacklevel=stacklevel+1
-    )
-
-
-def pylatexenc_deprecated_2(msg, stacklevel=2):
-    warnings.warn(
-        ( "Deprecated (pylatexenc 2.0): {} "
-          "[see https://pylatexenc.readthedocs.io/en/latest/new-in-pylatexenc-2/]" )
-        .format(msg.strip()),
-        DeprecationWarning,
-        stacklevel=stacklevel+1
-    )
-
-
-
-# ------------------------------------------------------------------------------
-
-
-
-
-
-class LazyDict(MutableMapping):
-    r"""
-    A lazy dictionary that loads its data when it is first queried.
-
-    This is used to store the legacy
-    :py:data:`pylatexenc.latexwalker.default_macro_dict` as well as
-    :py:data:`pylatexenc.latex2text.default_macro_dict` etc.  Such that these
-    "dictionaries" are still exposed at the module-level, but the data is loaded
-    only if they are actually queried.
-    """
-    def __init__(self, generate_dict_fn):
-        self._full_dict = None
-        self._generate_dict_fn = generate_dict_fn
-
-    def _ensure_instance(self):
-        if self._full_dict is not None:
-            return
-        self._full_dict = self._generate_dict_fn()
-
-    def __getitem__(self, key):
-        self._ensure_instance()
-        return self._full_dict.__getitem__(key)
-
-    def __setitem__(self, key, val):
-        self._ensure_instance()
-        return self._full_dict.__setitem__(key, val)
-
-    def __delitem__(self, key):
-        self._ensure_instance()
-        return self._full_dict.__delitem__(key)
-
-    def __iter__(self):
-        self._ensure_instance()
-        return iter(self._full_dict)
-
-    def __len__(self):
-        self._ensure_instance()
-        return len(self._full_dict)
-
-    def copy(self):
-        self._ensure_instance()
-        return self._full_dict.copy()
-
-    def clear(self):
-        self._ensure_instance()
-        return self._full_dict.clear()
-
-
-
-
-
-# ------------------------------------------------------------------------------
-
-
-
-
 class LineNumbersCalculator(object):
     r"""
     Utility to calculate line numbers.
     """
-    def __init__(self, s):
+    def __init__(self, s,
+                 line_number_offset=1, first_line_column_offset=0, column_offset=0):
         super(LineNumbersCalculator, self).__init__()
 
+        self.line_number_offset = line_number_offset
+        self.first_line_column_offset = first_line_column_offset
+        self.column_offset = column_offset
+
         def find_all_new_lines(x):
             # first line starts at the beginning of the string
             yield 0
             k = 0
             while k < len(x):
                 k = x.find('\n', k)
                 if k == -1:
@@ -153,20 +70,87 @@
         Return a tuple `(lineno, colno)` giving line number and column number.
         Line numbers start at 1 and column number start at zero, i.e., the
         beginning of the document (`pos=0`) has line and column number `(1,0)`.
         If `as_dict=True`, then a dictionary with keys 'lineno', 'colno' is
         returned instead of a tuple.
         """
 
+        if pos is None:
+            if as_dict:
+                return {'lineno': None, 'colno': None}
+            return (None, None)
+
         # find line number in list
 
         # line_no is the index of the last item in self._pos_new_lines that is <= pos.
-        line_no = bisect.bisect_right(self._pos_new_lines, pos)-1
+        line_no = bisect_right(self._pos_new_lines, pos)-1
         assert line_no >= 0 and line_no < len(self._pos_new_lines)
 
         col_no = pos - self._pos_new_lines[line_no]
-        # 1+... so that line and column numbers start at 1
+
+        if line_no == 0:
+            col_no += self.first_line_column_offset
+        else:
+            col_no += self.column_offset
+        line_no += self.line_number_offset
+
         if as_dict:
-            return {'lineno': 1 + line_no, 'colno': col_no}
-        return (1 + line_no, col_no)
+            return {'lineno': line_no, 'colno': col_no}
+        return (line_no, col_no)
+
+
+
+# ------------------------------------------------------------------------------
+
+
+class PushPropOverride(object):
+    def __init__(self, obj, propname, new_value):
+        super(PushPropOverride, self).__init__()
+        self.obj = obj
+        self.propname = propname
+        self.new_value = new_value
+
+    def __enter__(self):
+        if self.new_value is not None:
+            self.initval = getattr(self.obj, self.propname)
+            setattr(self.obj, self.propname, self.new_value)
+        return self
+
+    def __exit__(self, type, value, traceback):
+        # clean-up
+        if self.new_value is not None:
+            setattr(self.obj, self.propname, self.initval)
+
+
+# ------------------------------------------------------------------------------
+
+
+try:
+    from collections import ChainMap #lgtm [py/unused-import]
+except ImportError:
+    pass  #lgtm [py/unnecessary-pass]
+### BEGIN_PYTHON2_SUPPORT_CODE
+    from chainmap import ChainMap #lgtm [py/unused-import]
+### END_PYTHON2_SUPPORT_CODE
+
+
+
+# ------------------------------------------------------------------------------
+
+
 
+pylatexenc_deprecated_ver = lambda *args: None  #lgtm [py/multiple-definition]
+pylatexenc_deprecated_2 = lambda *args: None  #lgtm [py/multiple-definition]
+pylatexenc_deprecated_3 = lambda *args: None  #lgtm [py/multiple-definition]
+LazyDict = None  #lgtm [py/multiple-definition]
+
+### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
+
+from ._util_support import (   # lgtm [py/unused-import]
+    pylatexenc_deprecated_ver,
+    pylatexenc_deprecated_2,
+    pylatexenc_deprecated_3,
+    #
+    LazyDict
+)
 
+### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
```

### Comparing `pylatexenc-2.9/pylatexenc/latex2text/__init__.py` & `pylatexenc-3.0a13/pylatexenc/latex2text/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,36 +38,47 @@
 You may also use the command-line version of `latex2text`::
 
     $ echo '\textit{italic} \`acc\^ented text' | latex2text
     italic àccênted text
 
 """
 
-from __future__ import print_function, unicode_literals #, absolute_import
+from __future__ import print_function, unicode_literals
 
-import os
 import re
-import logging
-import sys
 import inspect
 import textwrap
 
-if sys.version_info.major >= 3:
-    def unicode(string): return string
-    basestring = str
-    getfullargspec = inspect.getfullargspec
-else:
-    getfullargspec = inspect.getargspec
+
+# for Py3
+_basestring = str
+_getfullargspec = getattr(inspect, 'getfullargspec', None)
+
+## Begin Py2 support code
+import sys
+if sys.version_info.major == 2:
+    # Py2
+    _basestring = basestring
+    _getfullargspec = inspect.getargspec
     chr = unichr
+#
+_python_is_narrow_build = (sys.maxunicode < 0x10FFFF)
+## End Py2 support code
+
+
 
-import pylatexenc
+
+#import pylatexenc
 from .. import latexwalker
+from ..latexnodes import nodes as latexnodes_nodes
+from ..latexnodes import parsers as latexnodes_parsers
 from .. import macrospec
 from .. import _util
 
+import logging
 logger = logging.getLogger(__name__)
 
 
 
 class MacroTextSpec(object):
     """
     A specification of how to obtain a textual representation of a macro.
@@ -261,19 +272,14 @@
 
     .. versionadded:: 2.0
 
        This function was introduced in `pylatexenc 2.0`.
     """
 
     return l2tobj.math_node_to_text(envnode)
-    # with _PushEquationContext(l2tobj):
-    #
-    #     contents = l2tobj.nodelist_to_text(envnode.nodelist).strip()
-    #     # indent equation, separate by newlines
-    #     return l2tobj._fmt_indented_block(contents)
 
 
 def fmt_input_macro(macronode, l2tobj):
     r"""
     This function can be used as callback in :py:class:`MacroTextSpec` for
     ``\input`` or ``\include`` macros.  The `macronode` must be a macro node
     with a single argument.  If :py:meth:`set_tex_input_directory()` was called
@@ -468,15 +474,15 @@
         return chr(offset_up + oc - _oA)
     if oc >= _oa and oc <= _oz:
         return chr(offset_lo + oc - _oa)
 
     # don't know how to handle this char
     return c
 
-if sys.maxunicode < 0x10FFFF:
+if _python_is_narrow_build:
     # narrow python build, disable math alphabets.
     _fmt_math_style_char = lambda c, style: c
 
 
 
 def fmt_math_text_style(text, style):
     r"""
@@ -637,15 +643,15 @@
         # "False" == the actual default for non-strict latex spaces == "macros"
         return _strict_latex_spaces_predef['macros']
     elif strict_latex_spaces is True:
         return dict([(k, True) for k in d.keys()])
     elif isinstance(strict_latex_spaces, dict):
         d.update(strict_latex_spaces)
         return d
-    elif isinstance(strict_latex_spaces, basestring):
+    elif isinstance(strict_latex_spaces, _basestring):
         if strict_latex_spaces == 'on':
             return _parse_strict_latex_spaces_dict(True)
         if strict_latex_spaces == 'off':
             return _parse_strict_latex_spaces_dict(False)
         if strict_latex_spaces not in _strict_latex_spaces_predef:
             raise ValueError("invalid value for strict_latex_spaces preset: {}"
                              .format(strict_latex_spaces))
@@ -662,14 +668,22 @@
             strict_latex_spaces = 'based-on-source'
 
         return _strict_latex_spaces_predef[strict_latex_spaces]
     else:
         raise ValueError("Invalid value for strict_latex_spaces: {!r}"
                          .format(strict_latex_spaces))
 
+#
+
+
+
+from ._inputlatexfile import read_latex_file
+
+
+
 
 class LatexNodes2Text(object):
     r"""
     Simplistic Latex-To-Text Converter.
 
     This class parses a nodes structure generated by the :py:mod:`latexwalker` module,
     and creates a text representation of the structure.
@@ -955,43 +969,15 @@
         the ``\\input`` macro), and should return a string with the file
         contents (or generate a warning or raise an error).
         """
 
         if self.tex_input_directory is None:
             return ''
 
-        fnfull = os.path.realpath(os.path.join(self.tex_input_directory, fn))
-        if self.strict_input:
-            # make sure that the input file is strictly within dirfull, and
-            # didn't escape with '../..' tricks or via symlinks.
-            dirfull = os.path.realpath(self.tex_input_directory)
-            if not fnfull.startswith(dirfull):
-                logger.warning(
-                    "Can't access path '%s' leading outside of mandated directory "
-                    "[strict input mode]",
-                    fn
-                )
-                return ''
-
-        if not os.path.exists(fnfull) and os.path.exists(fnfull + '.tex'):
-            fnfull = fnfull + '.tex'
-        if not os.path.exists(fnfull) and os.path.exists(fnfull + '.latex'):
-            fnfull = fnfull + '.latex'
-        if not os.path.isfile(fnfull):
-            logger.warning(u"Error, file doesn't exist: '%s'", fn)
-            return ''
-
-        logger.debug("Reading input file %r", fnfull)
-
-        try:
-            with open(fnfull) as f:
-                return f.read()
-        except IOError as e:
-            logger.warning(u"Error, can't access '%s': %s", fn, e)
-            return ''
+        return read_latex_file(self.tex_input_directory, self.strict_input, fn)
 
 
     def _input_node_simplify_repl(self, n):
         #
         # recurse into files upon '\input{}'
         #
 
@@ -1000,43 +986,48 @@
                            n.nodeargs)
 
         inputtex = self.read_input_file(self.nodelist_to_text([n.nodeargs[0]]).strip())
 
         if not inputtex:
             return ''
 
-        return self.nodelist_to_text(
-            latexwalker.LatexWalker(inputtex, **self.latex_walker_init_args)
-            .get_latex_nodes()[0]
-        )
+        lw = latexwalker.LatexWalker(inputtex, **self.latex_walker_init_args)
+
+        nodelist, _ = lw.parse_content(latexnodes_parsers.LatexGeneralNodesParser())
+
+        return self.nodelist_to_text(nodelist)
+
 
 
     def latex_to_text(self, latex, **parse_flags):
         """
         Parses the given `latex` code and returns its textual representation.
 
         This is equivalent to constructing a
         :py:class:`pylatexenc.latexwalker.LatexWalker` with the given `latex`
-        string, calling its method
-        :py:meth:`~pylatexenc.latexwalker.LatexWalker.get_latex_nodes()`, and
+        string, parsing the string into general nodes with a
+        :py:class:`~pylatexenc.latexnodes.parsers.LatexGeneralNodesParser` (see
+        :py:meth:`~pylatexenc.latexwalker.LatexWalker.parse_content()`), and
         providing the outcome to :py:meth:`nodelist_to_text()`.
 
         The `parse_flags` are keyword arguments to provide to the
         :py:class:`pylatexenc.latexwalker.LatexWalker` constructor.
         """
-        return self.nodelist_to_text(
-            latexwalker.LatexWalker(latex, **parse_flags).get_latex_nodes()[0]
-        )
+
+        lw = latexwalker.LatexWalker(latex, **parse_flags)
+        nodelist, _ = lw.parse_content(latexnodes_parsers.LatexGeneralNodesParser())
+        return self.nodelist_to_text( nodelist )
 
 
     def nodelist_to_text(self, nodelist):
         """
-        Extracts text from a node list. `nodelist` is a list of `latexwalker` nodes,
-        typically returned by
-        :py:meth:`pylatexenc.latexwalker.LatexWalker.get_latex_nodes()`.
+        Extracts text from a node list. `nodelist` is a list of
+        `latexwalker` nodes, typically parsed using a
+        :py:class:`~pylatexenc.latexnodes.parsers.LatexGeneralNodesParser` (see
+        :py:meth:`~pylatexenc.latexwalker.LatexWalker.parse_content()`).
 
         This function basically applies `node_to_text()` to each node and
         concatenates the results into one string.  (This is not quite actually
         the case, since we take some care as to where we add whitespace
         according to the class options.)
         """
 
@@ -1230,14 +1221,15 @@
 
         def get_specials_str_repl(node, specials_chars, spec):
             if spec.simplify_repl:
                 return self.apply_simplify_repl(node, spec.simplify_repl,
                                                 what="specials '%s'"%(specials_chars))
             if spec.discard:
                 return ""
+            a = []
             if node.nodeargd and node.nodeargd.argnlist:
                 a = node.nodeargd.argnlist
             return "".join([self._groupnodecontents_to_text(n) for n in a])
 
         s = get_specials_str_repl(node, specials_chars, sspec)
         return s
 
@@ -1249,38 +1241,42 @@
         :py:class:`~pylatexenc.latexwalker.LatexEnvironmentNode`.
 
         This method is responsible for honoring the `math_mode=...` option
         provided to the constructor.
         """
 
         if self.math_mode == 'verbatim':
-            if node.isNodeType(latexwalker.LatexEnvironmentNode) or node.displaytype == 'display':
+            if node.isNodeType(latexwalker.LatexEnvironmentNode) \
+               or node.displaytype == 'display':
                 return self._fmt_indented_block(node.latex_verbatim(), indent='')
             else:
                 return node.latex_verbatim()
 
         elif self.math_mode == 'remove':
             return ''
 
         elif self.math_mode == 'with-delimiters':
             with _PushEquationContext(self):
                 content = self.nodelist_to_text(node.nodelist).strip()
             if node.isNodeType(latexwalker.LatexMathNode):
                 delims = node.delimiters
             else: # environment node
-                delims = r'\begin{%s}'%(node.environmentname), r'\end{%s}'%(node.environmentname)
-            if node.isNodeType(latexwalker.LatexEnvironmentNode) or node.displaytype == 'display':
+                delims = (r'\begin{%s}'%(node.environmentname),
+                          r'\end{%s}'%(node.environmentname),)
+            if node.isNodeType(latexwalker.LatexEnvironmentNode) \
+               or node.displaytype == 'display':
                 return delims[0] + self._fmt_indented_block(content, indent='') + delims[1]
             else:
                 return delims[0] + content + delims[1]
 
         elif self.math_mode == 'text':
             with _PushEquationContext(self):
                 content = self.nodelist_to_text(node.nodelist).strip()
-            if node.isNodeType(latexwalker.LatexEnvironmentNode) or node.displaytype == 'display':
+            if node.isNodeType(latexwalker.LatexEnvironmentNode) \
+               or node.displaytype == 'display':
                 return self._fmt_indented_block(content)
             else:
                 return content
 
         else:
             raise RuntimeError("unknown math_mode={} !".format(self.math_mode))
 
@@ -1329,15 +1325,15 @@
         have a `simplify_repl` object (given by e.g. a MacroTextSpec or
         similar).
 
         The argument `what` is used in error messages.
         """
         if callable(simplify_repl):
             kwargs = {}
-            fn_args = getfullargspec(simplify_repl)[0]
+            fn_args = _getfullargspec(simplify_repl)[0]
             if 'l2tobj' in fn_args:
                 # callable accepts an argument named 'l2tobj', provide pointer to self
                 kwargs['l2tobj'] = self
             if node.isNodeType(latexwalker.LatexEnvironmentNode) and \
                'environmentname' in fn_args:
                 kwargs['environmentname'] = node.environmentname
             if node.isNodeType(latexwalker.LatexMacroNode) and \
@@ -1407,14 +1403,16 @@
                 node.isNodeType(latexwalker.LatexMacroNode) and
                 node.nodeoptarg is None and
                 len(node.nodeargs) == 0)
 
     def _groupnodecontents_to_text(self, groupnode):
         if groupnode is None:
             return ''
+        if isinstance(groupnode, latexnodes_nodes.LatexNodeList):
+            return self.nodelist_to_text(groupnode)
         if not groupnode.isNodeType(latexwalker.LatexGroupNode):
             return self.node_to_text(groupnode)
         return self.nodelist_to_text(groupnode.nodelist)
 
     def node_arg_to_text(self, node, k):
         r"""
         Return the textual representation of the `k`\ -th argument of the given
@@ -1470,15 +1468,15 @@
 
         return s
 
 
 
 
 
-class _PushEquationContext(latexwalker._PushPropOverride):
+class _PushEquationContext(_util.PushPropOverride):
     def __init__(self, l2t):
 
         new_strict_latex_spaces = None
         if l2t.strict_latex_spaces['in-equations'] is not None:
             new_strict_latex_spaces = _parse_strict_latex_spaces_dict(
                 l2t.strict_latex_spaces['in-equations']
             )
```

### Comparing `pylatexenc-2.9/pylatexenc/latex2text/__main__.py` & `pylatexenc-3.0a13/pylatexenc/latex2text/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,43 +19,52 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
+from __future__ import print_function, unicode_literals
+
 import sys
 import fileinput
 import argparse
 import logging
 
 
 from .. import latexwalker
+from ..latexnodes import parsers as latexnodes_parsers
 from ..latex2text import LatexNodes2Text, _strict_latex_spaces_predef
 from ..version import version_str
 
 
 def main(argv=None):
 
     if argv is None:
         argv = sys.argv[1:]
 
     parser = argparse.ArgumentParser(prog='latex2text', add_help=False)
 
     codegroup = parser.add_argument_group("Input options")
 
     codegroup.add_argument('--code', '-c', action='store', default=None, metavar="LATEX_CODE",
-                           help="Convert the given LATEX_CODE to unicode text instead of reading "
-                           "from FILE or standard input.  You cannot specify FILEs if you use this "
-                           "option, and any standard input is ignored.")
+                           help="Convert the given LATEX_CODE to unicode text instead "
+                           "of reading from FILE or standard input.  You cannot specify "
+                           "FILEs if you use this option, and any standard input is ignored.")
+
+
+    codegroup.add_argument('--no-final-newline', '-n',
+                           action='store_true', default=False,
+                           help="Do not print a newline after the converted text.")
 
 
     codegroup.add_argument('files', metavar="FILE", nargs='*',
-                           help="Input files to read LaTeX code from. If no FILE(s) is/are specified, "
-                           "LaTeX code is read from standard input unless --code is specified")
+                           help="Input files to read LaTeX code from. If no FILE(s) "
+                           "is/are specified, LaTeX code is read from standard input "
+                           "unless --code is specified")
 
 
 
     group = parser.add_argument_group("LatexWalker options")
 
     group.add_argument('--parser-keep-inline-math', action='store_const', const=True,
                        dest='parser_keep_inline_math', default=None,
@@ -183,24 +192,30 @@
     else:
         fill_text = None
 
     lw = latexwalker.LatexWalker(latex,
                                  tolerant_parsing=args.tolerant_parsing,
                                  strict_braces=args.strict_braces)
 
-    (nodelist, pos, len_) = lw.get_latex_nodes()
+    nodelist, _ = lw.parse_content(latexnodes_parsers.LatexGeneralNodesParser())
+
+    #(nodelist, pos, len_) = lw.get_latex_nodes()
 
     ln2t = LatexNodes2Text(math_mode=args.math_mode,
                            keep_comments=args.keep_comments,
                            strict_latex_spaces=args.strict_latex_spaces,
                            keep_braced_groups=args.keep_braced_groups,
                            keep_braced_groups_minlen=args.keep_braced_groups_minlen,
                            fill_text=fill_text)
 
-    print(ln2t.nodelist_to_text(nodelist))
+    print_kwargs = {}
+    if args.no_final_newline:
+        print_kwargs['end'] = ''
+
+    print(ln2t.nodelist_to_text(nodelist), **print_kwargs)
 
 
 
 def run_main():
 
     try:
```

### Comparing `pylatexenc-2.9/pylatexenc/latex2text/_defaultspecs.py` & `pylatexenc-3.0a13/pylatexenc/latex2text/_defaultspecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,31 +80,14 @@
 
 # ==============================================================================
 
 
 
 _latex_specs_placeholders = {
     'environments': [
-        EnvironmentTextSpec('equation', simplify_repl=fmt_equation_environment),
-        # note {equation*} is actually defined by amsmath
-        EnvironmentTextSpec('equation*', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('eqnarray', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('eqnarray*', simplify_repl=fmt_equation_environment),
-
-        EnvironmentTextSpec('align', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('multline', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('gather', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('align*', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('multline*', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('gather*', simplify_repl=fmt_equation_environment),
-
-        # breqn math
-        EnvironmentTextSpec('dmath', simplify_repl=fmt_equation_environment),
-        EnvironmentTextSpec('dmath*', simplify_repl=fmt_equation_environment),
-
 #  --- as of pylatexenc 2.8, these are now approximated ---
 #        EnvironmentTextSpec('array', simplify_repl=fmt_placeholder_node),
 #        EnvironmentTextSpec('pmatrix', simplify_repl=fmt_placeholder_node),
 #        EnvironmentTextSpec('bmatrix', simplify_repl=fmt_placeholder_node),
 #        EnvironmentTextSpec('smallmatrix', simplify_repl=fmt_placeholder_node),
 #        EnvironmentTextSpec('psmallmatrix', simplify_repl=fmt_placeholder_node),
 #        EnvironmentTextSpec('bsmallmatrix', simplify_repl=fmt_placeholder_node),
@@ -117,14 +100,18 @@
         ('includegraphics', placeholder_node_formatter('graphics')),
 
         ('ref', '<ref>'),
         ('autoref', '<ref>'),
         ('cref', '<ref>'),
         ('Cref', '<Ref>'),
         ('eqref', '(<ref>)'),
+
+        ('cite', '<cit.>'),
+        ('citet', '<cit.>'),
+        ('citep', '<cit.>'),
     )],
 }
 
 _latex_specs_approximations = {
     'environments': [
         EnvironmentTextSpec('center', simplify_repl='\n%s\n'),
         EnvironmentTextSpec('flushleft', simplify_repl='\n%s\n'),
@@ -140,14 +127,36 @@
 
         EnvironmentTextSpec('array', simplify_repl=fmt_matrix_environment_node),
         EnvironmentTextSpec('pmatrix', simplify_repl=fmt_matrix_environment_node),
         EnvironmentTextSpec('bmatrix', simplify_repl=fmt_matrix_environment_node),
         EnvironmentTextSpec('smallmatrix', simplify_repl=fmt_matrix_environment_node),
         EnvironmentTextSpec('psmallmatrix', simplify_repl=fmt_matrix_environment_node),
         EnvironmentTextSpec('bsmallmatrix', simplify_repl=fmt_matrix_environment_node),
+
+        #
+        # math environments used to be categorized as 'placeholders' in
+        # pylatexenc <= 2.9, but I think it's more accurate to have them in
+        # 'approximations'.
+        #
+        EnvironmentTextSpec('equation', simplify_repl=fmt_equation_environment),
+        # note {equation*} is actually defined by amsmath
+        EnvironmentTextSpec('equation*', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('eqnarray', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('eqnarray*', simplify_repl=fmt_equation_environment),
+        #
+        EnvironmentTextSpec('align', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('multline', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('gather', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('align*', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('multline*', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('gather*', simplify_repl=fmt_equation_environment),
+        #
+        # breqn math
+        EnvironmentTextSpec('dmath', simplify_repl=fmt_equation_environment),
+        EnvironmentTextSpec('dmath*', simplify_repl=fmt_equation_environment),
     ],
     'specials': [
         SpecialsTextSpec('&', '   '), # ignore tabular alignments, just add a little space
     ],
     'macros': [
         # NOTE: macro will only be assigned arguments if they are explicitly
         #       defined as accepting arguments in the `LatexWalker` (see
@@ -181,51 +190,75 @@
          )
         ) ,
         ('footnote', '[%(2)s]'), # \footnote[optional mark]{footnote text}
         ('href', lambda n, l2tobj:  \
          '{} <{}>'.format(l2tobj.nodelist_to_text([n.nodeargd.argnlist[1]]), 
                           l2tobj.nodelist_to_text([n.nodeargd.argnlist[0]]))),
 
-        ('cite', '<cit.>'),
-        ('citet', '<cit.>'),
-        ('citep', '<cit.>'),
-
         ('part',
          lambda n, l2tobj: u'\n\nPART: {}\n'.format(
              l2tobj.node_arg_to_text(n, 2).upper())),
         ('chapter',
          lambda n, l2tobj: u'\n\nCHAPTER: {}\n'.format(
              l2tobj.node_arg_to_text(n, 2).upper())),
         ('section',
          lambda n, l2tobj: u'\n\n\N{SECTION SIGN} {}\n'.format(
              l2tobj.node_arg_to_text(n, 2).upper())),
         ('subsection',
          lambda n, l2tobj: u'\n\n \N{SECTION SIGN}.\N{SECTION SIGN} {}\n'.format(
              l2tobj.node_arg_to_text(n, 2))),
         ('subsubsection',
-         lambda n, l2tobj: u'\n\n  \N{SECTION SIGN}.\N{SECTION SIGN}.\N{SECTION SIGN} {}\n'.format(
-             l2tobj.node_arg_to_text(n, 2))),
+         lambda n, l2tobj: \
+             u'\n\n  \N{SECTION SIGN}.\N{SECTION SIGN}.\N{SECTION SIGN} {}\n'.format(
+                 l2tobj.node_arg_to_text(n, 2))),
         ('paragraph',
          lambda n, l2tobj: u'\n\n  {}\n'.format(l2tobj.node_arg_to_text(n, 2))),
         ('subparagraph',
          lambda n, l2tobj: u'\n\n    {}\n'.format(
              l2tobj.node_arg_to_text(n, 2))),
 
+        ('textcolor', '%(3)s'),
+        ('colorbox', '%(3)s'),
+        ('fcolorbox', '%(5)s'),
+
         ('hspace', ''),
         ('vspace', '\n'),
 
         # \\ is treated as an "approximation" because a good text renderer would
         # have to actually note that this is a end-of-line marker which is not
         # to be confused with other newlines in the paragraph (which can be
         # reflowed)
         ("\\", '\n'),
 
         ('frac', '%s/%s'),
         ('nicefrac', '%s/%s'),
         ('textfrac', '%s/%s'),
+
+        ('overline', '%s'),
+        ('underline', '%s'),
+        ('widehat', '%s'),
+        ('widetilde', '%s'),
+        ('wideparen', '%s'),
+        ('overleftarrow', '%s'),
+        ('overrightarrow', '%s'),
+        ('overleftrightarrow', '%s'),
+        ('underleftarrow', '%s'),
+        ('underrightarrow', '%s'),
+        ('underleftrightarrow', '%s'),
+        ('overbrace', '%s'),
+        ('underbrace', '%s'),
+        ('overgroup', '%s'),
+        ('undergroup', '%s'),
+        ('overbracket', '%s'),
+        ('underbracket', '%s'),
+        ('overlinesegment', '%s'),
+        ('underlinesegment', '%s'),
+        ('overleftharpoon', '%s'),
+        ('overrightharpoon', '%s'),
+
     )],
 }
 
 _latex_specs_base = {
     
     'environments': [
     ],
@@ -289,14 +322,16 @@
         ("texteuro", u"\N{EURO SIGN}"),
 
         ("backslash", "\\"),
         ("textbackslash", "\\"),
 
         # math stuff
 
+        ("ensuremath", "%s"),
+
         ("hbar", u"\N{LATIN SMALL LETTER H WITH STROKE}"),
         ("ell", u"\N{SCRIPT SMALL L}"),
 
         ('forall', u"\N{FOR ALL}"),
         ('complement', u"\N{COMPLEMENT}"),
         ('partial', u"\N{PARTIAL DIFFERENTIAL}"),
         ('exists', u"\N{THERE EXISTS}"),
@@ -443,16 +478,18 @@
         ('rVert', u'\N{DOUBLE VERTICAL LINE}'),
         ('Vert', u'\N{DOUBLE VERTICAL LINE}'),
         ('mid', u'|'),
         ('nmid', u'\N{DOES NOT DIVIDE}'),
 
         ('ket', u'|%s\N{MATHEMATICAL RIGHT ANGLE BRACKET}'),
         ('bra', u'\N{MATHEMATICAL LEFT ANGLE BRACKET}%s|'),
-        ('braket', u'\N{MATHEMATICAL LEFT ANGLE BRACKET}%s|%s\N{MATHEMATICAL RIGHT ANGLE BRACKET}'),
-        ('ketbra', u'|%s\N{MATHEMATICAL RIGHT ANGLE BRACKET}\N{MATHEMATICAL LEFT ANGLE BRACKET}%s|'),
+        ('braket',
+         u'\N{MATHEMATICAL LEFT ANGLE BRACKET}%s|%s\N{MATHEMATICAL RIGHT ANGLE BRACKET}'),
+        ('ketbra',
+         u'|%s\N{MATHEMATICAL RIGHT ANGLE BRACKET}\N{MATHEMATICAL LEFT ANGLE BRACKET}%s|'),
         ('uparrow', u'\N{UPWARDS ARROW}'),
         ('downarrow', u'\N{DOWNWARDS ARROW}'),
         ('rightarrow', u'\N{RIGHTWARDS ARROW}'),
         ('to', u'\N{RIGHTWARDS ARROW}'),
         ('leftarrow', u'\N{LEFTWARDS ARROW}'),
         ('longrightarrow', u'\N{LONG RIGHTWARDS ARROW}'),
         ('longleftarrow', u'\N{LONG LEFTWARDS ARROW}'),
@@ -1456,29 +1493,46 @@
             smallname = "GREEK LUNATE EPSILON SYMBOL"
         if ucharname == 'PHI':
             smallname = "GREEK PHI SYMBOL"
         _latex_specs_base['macros'].append(
             MacroTextSpec(l, unicodedata.lookup(smallname))
         )
         _latex_specs_base['macros'].append(
-            MacroTextSpec(l[0].upper()+l[1:], unicodedata.lookup("GREEK CAPITAL LETTER "+ucharname))
-            )
+            MacroTextSpec(l[0].upper()+l[1:],
+                          unicodedata.lookup("GREEK CAPITAL LETTER "+ucharname))
+        )
+        # up-greek version (from packages such as upgreek or newtxmath)
+        _latex_specs_base['macros'].append(
+            MacroTextSpec("up"+l, unicodedata.lookup(smallname))
+        )
+        _latex_specs_base['macros'].append(
+            MacroTextSpec("Up"+l, unicodedata.lookup("GREEK CAPITAL LETTER "+ucharname))
+        )
+
 _greekletters(
     ('alpha', 'beta', 'gamma', 'delta', 'epsilon', 'zeta', 'eta', 'theta', 'iota', 'kappa',
      'lambda', 'mu', 'nu', 'xi', 'omicron', 'pi', 'rho', 'sigma', 'tau', 'upsilon', 'phi',
      'chi', 'psi', 'omega')
 )
 _latex_specs_base['macros'] += [
     MacroTextSpec('varepsilon', u'\N{GREEK SMALL LETTER EPSILON}'),
     MacroTextSpec('vartheta', u'\N{GREEK THETA SYMBOL}'),
     MacroTextSpec('varpi', u'\N{GREEK PI SYMBOL}'),
     MacroTextSpec('varrho', u'\N{GREEK RHO SYMBOL}'),
     MacroTextSpec('varsigma', u'\N{GREEK SMALL LETTER FINAL SIGMA}'),
     MacroTextSpec('varphi', u'\N{GREEK SMALL LETTER PHI}'),
-    ]
+
+    # up-greek version
+    MacroTextSpec('upvarepsilon', u'\N{GREEK SMALL LETTER EPSILON}'),
+    MacroTextSpec('upvartheta', u'\N{GREEK THETA SYMBOL}'),
+    MacroTextSpec('upvarpi', u'\N{GREEK PI SYMBOL}'),
+    MacroTextSpec('upvarrho', u'\N{GREEK RHO SYMBOL}'),
+    MacroTextSpec('upvarsigma', u'\N{GREEK SMALL LETTER FINAL SIGMA}'),
+    MacroTextSpec('upvarphi', u'\N{GREEK SMALL LETTER PHI}'),
+]
 
 
 unicode_accents_list = (
     # see http://en.wikibooks.org/wiki/LaTeX/Special_Characters for a list
     ("'", u"\N{COMBINING ACUTE ACCENT}"),
     ("`", u"\N{COMBINING GRAVE ACCENT}"),
     ('"', u"\N{COMBINING DIAERESIS}"),
```

### Comparing `pylatexenc-2.9/pylatexenc/latexencode/__main__.py` & `pylatexenc-3.0a13/pylatexenc/latexencode/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-2.9/pylatexenc/latexencode/_uni2latexmap.py` & `pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,17 +290,18 @@
 0x0179: "\\'Z",
 0x017A: "\\'z",
 0x017B: r'\.Z',
 0x017C: r'\.z',
 0x017D: r'\v{Z}',
 0x017E: r'\v{z}',
 0x0192: r'\textflorin',                          # 0x0192
-0x0195: r'\texthvlig',                            # LATIN SMALL LETTER HV [ƕ]
-0x019E: r'\textnrleg',                            # LATIN SMALL LETTER N WITH LONG RIGHT LEG [ƞ]
-0x01F5: r"\'{g}",                                 # LATIN SMALL LETTER G WITH ACUTE [ǵ]
+0x0195: r'\texthvlig',                           # LATIN SMALL LETTER HV [ƕ]
+0x019E: r'\textnrleg',                           # LATIN SMALL LETTER N WITH LONG RIGHT LEG [ƞ]
+0x01E7: r'\v{g}',                                # character ǧ
+0x01F5: r"\'{g}",                                # LATIN SMALL LETTER G WITH ACUTE [ǵ]
 
 
 0x0228: r'\c{E}',
 0x0229: r'\c{e}',
 
 # chars in linguistics, thanks @roedoejet (https://github.com/roedoejet/pylatexenc)
 0x0259: r'\textschwa',
```

### Comparing `pylatexenc-2.9/pylatexenc/latexencode/_uni2latexmap_xml.py` & `pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap_xml.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-2.9/pylatexenc/latexwalker/__main__.py` & `pylatexenc-3.0a13/pylatexenc/latexwalker/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     
     latexwalker = LatexWalker(latex,
                               tolerant_parsing=args.tolerant_parsing,
                               strict_braces=args.strict_braces)
 
     (nodelist, pos, len_) = latexwalker.get_latex_nodes()
 
+
     if args.output_format == 'human':
         print('\n--- NODES ---\n')
         for n in nodelist:
             disp_node(n)
         print('\n-------------\n')
         return
 
@@ -153,9 +154,9 @@
         traceback.print_exc()
         pdb.post_mortem()
 
 
 
 if __name__ == '__main__':
 
-    #run_main() # debug
-    main()
+    run_main() # debug
+    #main()
```

### Comparing `pylatexenc-2.9/pylatexenc/latexwalker/_defaultspecs.py` & `pylatexenc-3.0a13/pylatexenc/latexwalker/_defaultspecs.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,26 +23,33 @@
 # THE SOFTWARE.
 #
 
 
 # Internal module. May change without notice.
 
 
-from ..macrospec import std_macro, std_environment, std_specials, \
-    MacroSpec, EnvironmentSpec, MacroStandardArgsParser, VerbatimArgsParser
+from ..macrospec import (
+    std_macro,
+    std_environment,
+    std_specials,
+    MacroSpec, EnvironmentSpec, MacroStandardArgsParser,
+    VerbatimArgsParser, LstListingArgsParser,
+)
+
 
 specs = [
     #
     # CATEGORY: latex-base
     #
     ('latex-base', {
         'macros': [
 
             std_macro('documentclass', True, 1),
             std_macro('usepackage', True, 1),
+            std_macro('RequirePackage', True, 1),
             std_macro('selectlanguage', True, 1),
             std_macro('setlength', True, 2),
             std_macro('addlength', True, 2),
             std_macro('setcounter', True, 2),
             std_macro('addcounter', True, 2),
             std_macro('newcommand', "*{[[{"),
             std_macro('renewcommand', "*{[[{"),
@@ -52,28 +59,32 @@
             std_macro('provideenvironment', "*{[[{{"),
 
             std_macro('DeclareMathOperator', '*{{'),
 
             std_macro('hspace', '*{'),
             std_macro('vspace', '*{'),
 
-            MacroSpec('mbox', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('mbox',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
 
             # \title, \author, \date
             MacroSpec('title', '{'),
             MacroSpec('author', '{'),
             MacroSpec('date', '{'),
 
             # (Note: single backslash) end of line with optional no-break ('*') and
             # additional vertical spacing, e.g. \\*[2mm]
             #
             # Special for this command: don't allow an optional spacing argument
-            # to be on a new line.  This emulates the behavior in AMS
-            # environments.
-            MacroSpec('\\', args_parser=MacroStandardArgsParser('*[', optional_arg_no_space=True)),
+            # [2mm] to be separated by spaces from the rest of the macro.  This
+            # emulates the behavior in AMS environments, and avoids some errors;
+            # e.g. in "\begin{align} A=0 \\ [C,D]=0 \end{align}" the "[C,D]"
+            # does not get captured as an optional macro argument.
+            MacroSpec('\\',
+                      args_parser=MacroStandardArgsParser('*[', optional_arg_no_space=True)),
 
             std_macro('item', True, 0),
 
             # \input{someotherfile}
             std_macro('input', False, 1),
             std_macro('include', False, 1),
 
@@ -86,36 +97,44 @@
             std_macro('pagagraph', '*[{'),
             std_macro('subparagraph', '*[{'),
 
             std_macro('bibliography', '{'),
 
 
             std_macro('emph', False, 1),
-            std_macro('underline', False, 1),
-            MacroSpec('textrm', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('textit', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('textbf', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('textmd', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('textsc', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('textsf', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('textsl', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('texttt', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('textup', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
-            MacroSpec('text', args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textrm',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textit',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textbf',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textmd',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textsc',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textsf',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textsl',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('texttt',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('textup',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
+            MacroSpec('text',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[False])),
             std_macro('mathrm', False, 1), # only allowed in math mode anyway
             std_macro('mathbb', False, 1), # only allowed in math mode anyway
             std_macro('mathbf', False, 1),
             std_macro('mathit', False, 1),
             std_macro('mathsf', False, 1),
             std_macro('mathtt', False, 1),
             std_macro('mathcal', False, 1),
             std_macro('mathscr', False, 1),
             std_macro('mathfrak', False, 1),
 
-
             std_macro('label', False, 1),
             std_macro('ref', False, 1),
             std_macro('autoref', False, 1),
             std_macro('cref', False, 1),
             std_macro('Cref', False, 1),
             std_macro('eqref', False, 1),
             std_macro('url', False, 1),
@@ -139,15 +158,16 @@
             std_macro("b", False, 1),
             std_macro(".", False, 1),
             std_macro("d", False, 1),
             std_macro("r", False, 1),
             std_macro("u", False, 1),
             std_macro("v", False, 1),
 
-            MacroSpec('ensuremath', args_parser=MacroStandardArgsParser('{', args_math_mode=[True])),
+            MacroSpec('ensuremath',
+                      args_parser=MacroStandardArgsParser('{', args_math_mode=[True])),
 
             std_macro("not", False, 1),
 
             std_macro("vec", False, 1),
             std_macro("dot", False, 1),
             std_macro("hat", False, 1),
             std_macro("check", False, 1),
@@ -159,20 +179,58 @@
             std_macro("ddot", False, 1),
 
             std_macro('frac', False, 2),
             std_macro('nicefrac', False, 2),
 
             std_macro('sqrt', True, 1),
 
+            MacroSpec('overline', '{'),
+            MacroSpec('underline', '{'),
+            MacroSpec('widehat', '{'),
+            MacroSpec('widetilde', '{'),
+            MacroSpec('wideparen', '{'),
+            MacroSpec('overleftarrow', '{'),
+            MacroSpec('overrightarrow', '{'),
+            MacroSpec('overleftrightarrow', '{'),
+            MacroSpec('underleftarrow', '{'),
+            MacroSpec('underrightarrow', '{'),
+            MacroSpec('underleftrightarrow', '{'),
+            MacroSpec('overbrace', '{'),
+            MacroSpec('underbrace', '{'),
+            MacroSpec('overgroup', '{'),
+            MacroSpec('undergroup', '{'),
+            MacroSpec('overbracket', '{'),
+            MacroSpec('underbracket', '{'),
+            MacroSpec('overlinesegment', '{'),
+            MacroSpec('underlinesegment', '{'),
+            MacroSpec('overleftharpoon', '{'),
+            MacroSpec('overrightharpoon', '{'),
+
+            MacroSpec('xleftarrow', '[{'),
+            MacroSpec('xrightarrow', '[{'),
+
             std_macro('ket', False, 1),
             std_macro('bra', False, 1),
             std_macro('braket', False, 2),
             std_macro('ketbra', False, 2),
 
             std_macro('texorpdfstring', False, 2),
+
+            # xcolor commands
+            MacroSpec('definecolor', '[{{{'),
+            MacroSpec('providecolor', '[{{{'),
+            MacroSpec('colorlet', '[{[{'),
+            MacroSpec('color', '[{'),
+            MacroSpec('textcolor', '[{{'),
+            MacroSpec('pagecolor', '[{'),
+            MacroSpec('nopagecolor', ''),
+            MacroSpec('colorbox', '[{{'),
+            MacroSpec('fcolorbox', '[{[{{'),
+            MacroSpec('boxframe', '{{{'),
+            MacroSpec('rowcolors', '*[{{{'),
         ],
         'environments': [
             # NOTE: Starred variants (as in \begin{equation*}) are not specified as
             # for macros with an argspec='*'.  Rather, we need to define a separate
             # spec for the starred variant as the star really is part of the
             # environment name.  If you specify argspec='*', the parser will try to
             # look for an expression of the form '\begin{equation}*'
@@ -253,14 +311,27 @@
         ],
         'specials': [
             # optionally users could include the specials "|" like in latex-doc
             # for verbatim |\like \this|...
         ]}),
 
     #
+    # CATEGORY: lstlisting
+    #
+    ('lstlisting', {
+        'macros': [],
+        'environments': [
+            EnvironmentSpec('lstlisting', args_parser=LstListingArgsParser()),
+        ],
+        'specials': [
+            # optionally users could include the specials "|" like in latex-doc
+            # for lstlisting |\like \this|...
+        ]}),
+
+    #
     # CATEGORY: theorems
     #
     ('theorems', {
         'macros': [],
         'environments': [
             std_environment('theorem', '['),
             std_environment('proposition', '['),
@@ -385,7 +456,12 @@
         ],
         'environments': [
         ],
         'specials': [
         ]
     }),
 ]
+
+
+
+
+
```

### Comparing `pylatexenc-2.9/pylatexenc/macrospec/__init__.py` & `pylatexenc-3.0a13/pylatexenc/macrospec/_latexcontextdb.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,378 +19,36 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-r"""
-Provides classes and helper functions to describe a LaTeX context of known
-macros and environments, specifying how they should be parsed by
-:py:mod:`pylatexenc.latexwalker`.
+# Internal module. Internal API may move, disappear or otherwise change at any
+# time and without notice.
 
-.. versionadded:: 2.0
+from __future__ import print_function, unicode_literals
 
-   The entire module :py:mod:`pylatexenc.macrospec` was introduced in
-   `pylatexenc 2.0`.
-"""
 
+from .. import _util
 
-import sys
+from ..latexnodes import ParsingStateDelta
 
 
-if sys.version_info.major > 2:
-    # Py3
-    def unicode(s): return s
-    _basestring = str
-    _str_from_unicode = lambda x: x
-    _unicode_from_str = lambda x: x
-else:
-    # Py2
-    _basestring = basestring
-    _str_from_unicode = lambda x: unicode(x).encode('utf-8')
-    _unicode_from_str = lambda x: x.decode('utf-8')
+import logging
+logger = logging.getLogger(__name__)
 
 
-# ------------------------------------------------------------------------------
 
-from ._argparsers import ParsedMacroArgs, MacroStandardArgsParser, \
-    ParsedVerbatimArgs, VerbatimArgsParser
+_autogen_category_prefix = '__lctxdb_cat_'
 
-# ------------------------------------------------------------------------------
-
-class MacroSpec(object):
-    r"""
-    Stores the specification of a macro.
-
-    This stores the macro name and instructions on how to parse the macro
-    arguments.
-
-    .. py:attribute:: macroname
-
-       The name of the macro, without the leading backslash.
-
-    .. py:attribute:: args_parser
-
-       The parser instance that can understand this macro's arguments.  For
-       standard LaTeX macros this is usually a
-       :py:class:`MacroStandardArgsParser` instance.
-
-       If you specify a string, then for convenience this is interpreted as an
-       argspec argument for :py:class:`MacroStandardArgsParser` and such an
-       instance is automatically created.
-    """
-    def __init__(self, macroname, args_parser=MacroStandardArgsParser(), **kwargs):
-        super(MacroSpec, self).__init__(**kwargs)
-        self.macroname = macroname
-        if isinstance(args_parser, _basestring):
-            self.args_parser = MacroStandardArgsParser(args_parser)
-        else:
-            self.args_parser = args_parser
-
-    def parse_args(self, *args, **kwargs):
-        r"""
-        Shorthand for calling the :py:attr:`args_parser`\ 's `parse_args()` method.
-        See :py:class:`MacroStandardArgsParser`.
-        """
-        return self.args_parser.parse_args(*args, **kwargs)
-
-    def __repr__(self):
-        return 'MacroSpec(macroname=%r, args_parser=%r)'%(self.macroname, self.args_parser)
-
-
-
-class EnvironmentSpec(object):
-    r"""
-    Stores the specification of a LaTeX environment.
-
-    This stores the environment name and instructions on how to parse any
-    arguments provided after ``\begin{environment}<args>``.
-
-    .. py:attribute:: environmentname
-
-       The name of the environment, i.e., the argument of ``\begin{...}`` and
-       ``\end{...}``.
-
-    .. py:attribute:: args_parser
-
-       The parser instance that can understand this environment's arguments.
-       For standard LaTeX environment this is usually a
-       :py:class:`MacroStandardArgsParser` instance.
-
-       If you specify a string, then for convenience this is interpreted as an
-       argspec argument for :py:class:`MacroStandardArgsParser` and such an
-       instance is automatically created.
-
-    .. py:attribute:: is_math_mode
-
-       A boolean that indicates whether or not the contents is to be interpreted
-       in Math Mode.  This would be True for environments like
-       ``\begin{equation}``, ``\begin{align}``, etc., but False for
-       ``\begin{figure}``, etc.
-
-    .. note::
-
-       Starred variants of environments (as in ``\begin{equation*}``) must not
-       be specified using an argspec as for macros (e.g., `argspec='*'`).
-       Rather, we need to define a separate environment spec for the starred
-       variant with the star in the name itself (``EnvironmentSpec('equation*',
-       None)``) because the star really is part of the environment name.  If you
-       happened to use ``EnvironmentSpec('equation', '*')``, then the parser
-       would recognize the expression ``\begin{equation}*`` but not
-       ``\begin{equation*}``.
-    """
-    def __init__(self, environmentname, args_parser=MacroStandardArgsParser(),
-                 is_math_mode=False, **kwargs):
-        super(EnvironmentSpec, self).__init__(**kwargs)
-        self.environmentname = environmentname
-        if isinstance(args_parser, _basestring):
-            self.args_parser = MacroStandardArgsParser(args_parser)
-        else:
-            self.args_parser = args_parser
-        self.is_math_mode = is_math_mode
-
-    def parse_args(self, *args, **kwargs):
-        r"""
-        Shorthand for calling the :py:attr:`args_parser`\ 's `parse_args()` method.
-        See :py:class:`MacroStandardArgsParser`.
-        """
-        return self.args_parser.parse_args(*args, **kwargs)
-
-    def __repr__(self):
-        return 'EnvironmentSpec(environmentname=%r, args_parser=%r, is_math_mode=%r)'%(
-            self.environmentname, self.args_parser, self.is_math_mode
-        )
-
-
-
-class SpecialsSpec(object):
-    r"""
-    Specification of a LaTeX "special char sequence": an active char, a
-    ligature, or some other non-macro char sequence that has a special meaning.
-
-    For instance, '&', '~', and '``' are considered as "specials".
-
-    .. py:attribute:: specials_chars
-    
-       The string (one or several characters) that has a special meaning. E.g.,
-       '&', '~', '``', etc.
-
-    .. py:attribute:: args_parser
-    
-       A parser (e.g. :py:class:`MacroStandardArgsParser`) that is invoked when
-       the specials is encountered.  Can/should be set to `None` if the specials
-       should not parse any arguments (e.g. '~').
-    """
-    def __init__(self, specials_chars,
-                 args_parser=None,
-                 **kwargs):
-        super(SpecialsSpec, self).__init__(**kwargs)
-        self.specials_chars = specials_chars
-        self.args_parser = args_parser
-
-    def parse_args(self, *args, **kwargs):
-        r"""
-        Basically a shorthand for calling the :py:attr:`args_parser`\ 's
-        `parse_args()` method.  See :py:class:`MacroStandardArgsParser`.
-        
-        If however the py:attr:`args_parser` attribute is `None`, then this
-        method returns `None`.
-        """
-        if self.args_parser is None:
-            return None
-        return self.args_parser.parse_args(*args, **kwargs)
-
-    def __repr__(self):
-        return 'SpecialsSpec(specials_chars=%r, args_parser=%r)'%(
-            self.specials_chars, self.args_parser
-        )
-
-
-# ------------------------------------------------------------------------------
-
-
-def std_macro(macname, *args, **kwargs):
-    r"""
-    Return a macro specification for the given macro.  Syntax::
-    
-      spec = std_macro(macname, argspec)
-      #  or
-      spec = std_macro(macname, optarg, numargs)
-      #  or
-      spec = std_macro( (macname, argspec), )
-      #  or
-      spec = std_macro( (macname, optarg, numargs), )
-      #  or
-      spec = std_macro( spec ) # spec is already a `MacroSpec` -- no-op
-
-    - `macname` is the name of the macro, without the leading backslash.
-
-    - `argspec` is a string either characters "\*", "{" or "[", in which star
-      indicates an optional asterisk character (e.g. starred macro variants),
-      each curly brace specifies a mandatory argument and each square bracket
-      specifies an optional argument in square brackets.  For example, "{{\*[{"
-      expects two mandatory arguments, then an optional star, an optional
-      argument in square brackets, and then another mandatory argument.
-
-      `argspec` may also be `None`, which is the same as ``argspec=''``.
-
-    - `optarg` may be one of `True`, `False`, or `None`, corresponding to these
-      possibilities:
-
-      + if `True`, the macro expects as first argument an optional argument in
-        square brackets. Then, `numargs` specifies the number of additional
-        mandatory arguments to the command, given in usual curly braces (or
-        simply as one TeX token like a single macro)
-
-      + if `False`, the macro only expects a number of mandatory arguments given
-        by `numargs`. The mandatory arguments are given in usual curly braces
-        (or simply as one TeX token like a single macro)
-
-      + if `None`, then `numargs` is a string like `argspec` above.  I.e.,
-        ``std_macro(macname, None, argspec)`` is the same as
-        ``std_macro(macname, argspec)``.
-
-    - `numargs`: depends on `optarg`, see above.
-    
-    To make environment specifications (:py:class:`EnvironmentSpec`) instead of
-    a macro specification, use the function :py:func:`std_environment()`
-    instead.
-
-    The helper function :py:func:`std_environment()` is a shorthand for calling
-    this function with additional keyword arguments.  An optional keyword
-    argument `make_environment_spec=True` to the present function may be
-    specified to return an `EnvironmentSpec` instead of a `MacroSpec`.  In this
-    case, you can further specify the `environment_is_math_mode=True|False` to
-    specify whether of not the environment represents a math mode.
-    """
-
-    if isinstance(macname, tuple):
-        if len(args) != 0:
-            raise TypeError("No positional arguments expected if first argument is a tuple")
-        args = tuple(macname[1:])
-        macname = macname[0]
-
-    if isinstance(macname, MacroSpec):
-        if len(args) != 0:
-            raise TypeError("No positional arguments expected if first argument is a MacroSpec")
-        return macname
-    
-    if isinstance(macname, EnvironmentSpec):
-        if len(args) != 0:
-            raise TypeError("No positional arguments expected if first argument is a EnvironmentSpec")
-        return macname
-
-    if len(args) == 1:
-        # std_macro(macname, argspec)
-        argspec = args[0]
-    elif len(args) != 2:
-        raise TypeError(
-            "Wrong number of arguments for std_macro, macname={!r}, args={!r}".format(
-                macname, args
-            ))
-    elif not args[0] and isinstance(args[1], _basestring):
-        # argspec given in numargs
-        argspec = args[1]
-    else:
-        argspec = ''
-        if args[0]:
-            argspec = '['
-        argspec += '{'*args[1]
-
-    if kwargs.get('make_environment_spec', False):
-        return EnvironmentSpec(macname, args_parser=MacroStandardArgsParser(argspec),
-                               is_math_mode=kwargs.get('environment_is_math_mode', False))
-    return MacroSpec(macname, args_parser=MacroStandardArgsParser(argspec))
-
-
-def std_environment(envname, *args, **kwargs):
-    r"""
-    Return an environment specification for the given environment.  Syntax::
-
-      spec = std_environment(envname, argspec, is_math_mode=True|False)
-      #  or
-      spec = std_environment(envname, optarg, numargs, is_math_mode=True|False)
-      #  or
-      spec = std_environment( (envname, argspec), is_math_mode=True|False)
-      #  or
-      spec = std_environment( (envname, optarg, numargs), is_math_mode=True|False)
-      #  or
-      spec = std_environment( spec ) # spec is already a `EnvironmentSpec` -- no-op
-
-    - `envname` is the name of the environment, i.e., the argument to
-      ``\begin{...}``.
-
-    - `argspec` is a string either characters "\*", "{" or "[", in which star
-      indicates an optional asterisk character (e.g. starred environment
-      variants), each curly brace specifies a mandatory argument and each square
-      bracket specifies an optional argument in square brackets.  For example,
-      "{{\*[{" expects two mandatory arguments, then an optional star, an
-      optional argument in square brackets, and then another mandatory argument.
-
-      `argspec` may also be `None`, which is the same as ``argspec=''``.
-
-    .. note::
-
-       See :py:class:`EnvironmentSpec` for an important remark about starred
-       variants for environments.  TL;DR: a starred verison of an environment is
-       defined as a separate `EnvironmentSpec` with the star in the name and
-       *not* using an ``argspec='*'``.
-
-    - `optarg` may be one of `True`, `False`, or `None`, corresponding to these
-      possibilities:
-
-      + if `True`, the environment expects as first argument an optional argument in
-        square brackets. Then, `numargs` specifies the number of additional
-        mandatory arguments to the command, given in usual curly braces (or
-        simply as one TeX token like a single environment)
-
-      + if `False`, the environment only expects a number of mandatory arguments given
-        by `numargs`. The mandatory arguments are given in usual curly braces
-        (or simply as one TeX token like a single environment)
-
-      + if `None`, then `numargs` is a string like `argspec` above.  I.e.,
-        ``std_environment(envname, None, argspec)`` is the same as
-        ``std_environment(envname, argspec)``.
-
-    - `numargs`: depends on `optarg`, see above.
-
-    - `is_math_mode`: if set to True, then the environment represents a math
-      mode environment (e.g., 'equation', 'align', 'gather', etc.), i.e., whose
-      contents should be parsed in an appropriate math mode.  Note that
-      `is_math_mode` *must* be given as a keyword argument, in contrast to all
-      other arguments which must be positional (non-keyword) arguments.
-    """
-    is_math_mode = kwargs.pop('is_math_mode', False)
-    kwargs2 = dict(kwargs)
-    kwargs2.update(make_environment_spec=True,
-                   environment_is_math_mode=is_math_mode)
-    return std_macro(envname, *args, **kwargs2)
-
-
-def std_specials(specials_chars):
-    r"""
-    Return a latex specials specification for the given character sequence.  Syntax::
-
-      spec = std_specials(specials_chars)
-
-    where `specials_chars` is the sequence of characters that has a special
-    LaTeX meaning, e.g. ``&`` or ``''``.
-
-    This helper function only allows to create specs for simple specials without
-    any argument parsing.  For more complicated specials, you can instantiate a
-    :py:class:`SpecialsSpec` directly.
-    """
-    return SpecialsSpec(specials_chars, args_parser=None)
-
-
-
-
-# ------------------------------------------------------------------------------
 
+### BEGINPATCH_UNIQUE_OBJECT_ID
+fn_unique_object_id = id
+### ENDPATCH_UNIQUE_OBJECT_ID
 
 
 
 class LatexContextDb(object):
     r"""
     Store a database of specifications of known macros, environments, and other
     latex specials.  This might be, e.g., how many arguments a macro accepts, or
@@ -417,41 +75,82 @@
     constructed and all the definitions added with
     :py:meth:`add_context_category()`, one should refrain from modifying it
     directly after providing it to, e.g., a
     :py:class:`~pylatexenc.latexwalker.LatexWalker` object.  The reason is that
     the latex walker keeps track of what the latex context was when parsing
     nodes, and modifying the context will modify that stored information, too.
     Instead of being tempted to modify the object, create a new one with
-    :py:meth:`filter_context()`.
+    :py:meth:`filtered_context()`.
+    
+    To (partially) ensure that the database isn't modified while it is being
+    used, it can be "frozen" with the method :py:meth:`freeze()`.  This method
+    simply sets a flag and will cause methods like `add_context_category()` to
+    raise an error.  You can always construct new context category instances
+    based on the present one by calling :py:meth:`filtered_context()` or
+    :py:meth:`extended_with()`.
 
     See :py:func:`pylatexenc.latexwalker.get_default_latex_context_db()` for the
     default latex context for `latexwalker` with a default collection of known
     latex macros and environments.
     See :py:func:`pylatexenc.latex2text.get_default_latex_context_db()` for the
     default latex context for `latex2text` with a set of text replacements for a
     collection of known macros and environments.
     """
     def __init__(self, **kwargs):
         super(LatexContextDb, self).__init__(**kwargs)
 
         self.category_list = []
         self.d = {}
 
+        self.frozen = False
+
+        # these chainmaps' list of maps mirror the category_list item for item.
+        self.lookup_chain_maps = {
+            'macros': _util.ChainMap({}),
+            'environments': _util.ChainMap({}),
+            'specials': _util.ChainMap({}),
+        }
+
         self.unknown_macro_spec = None
         self.unknown_environment_spec = None
         self.unknown_specials_spec = None
 
-        
+        self._autogen_category_counter = 0
+
+
+    def freeze(self):
+        r"""
+        Disable future changes to the information contained in this object.
+
+        LatexWalker objects expect that context category databases are
+        immutable, they don't change.  Building a context database object,
+        however, might require several calls to add_context_category, etc.
+
+        So what the latexwalker does is that it `freeze()`\ s the context db
+        object to prevent future changes.
+        """
+        self.frozen = True
+
+    
+    def __repr__(self):
+        return "<LatexContextDb {:#x}{}>".format(
+            fn_unique_object_id(self),
+            ("" if self.frozen else " unfrozen")
+        )
+
+
     def add_context_category(self, category, macros=[], environments=[], specials=[],
                              prepend=False, insert_before=None, insert_after=None):
         r"""
         Register a category of macro and environment specifications in the context
         database.
 
-        The category name `category` must not already exist in the database.
+        The category name `category` must not already exist in the database.  If
+        `category` is `None`, then a unique automatically-generated and internal
+        category name is used.
 
         The argument `macros` is an iterable (e.g., a list) of macro
         specification objects.  The argument `environments` is an iterable
         (e.g., a list) of environment spec objects.  Similarly, the `specials`
         argument is an iterable of latex specials spec instances.
 
         If you specify `prepend=True`, then macro and environment lookups will
@@ -467,109 +166,147 @@
         be a string; the definitions are inserted in the category list
         immediately after the given category name, or at the end of the list if
         the given category doesn't exist.
 
         You may only specify one of `prepend=True`, `insert_before='...'` or
         `insert_after='...'`.
         """
-        
+
+        if self.frozen:
+            raise RuntimeError("You attempted to modify a frozen LatexContextDb object.")
+
+        if category is not None and category.startswith(_autogen_category_prefix):
+            raise ValueError("Category name {} is unfortunately reserved for internal use"
+                             .format(category))
+
+        if category is None:
+            _autogen_category_counter, category = self._get_new_autogen_category()
+            self._autogen_category_counter = _autogen_category_counter + 1
+
         if category in self.category_list:
             raise ValueError("Category {} is already registered in the context database"
                              .format(category))
 
         # ensure only one of these options is set
         if len([ x for x in (prepend, insert_before, insert_after) if x ]) > 1:
             raise TypeError("add_context_category(): You may only specify one of "
                             "prepend=True, insert_before=... or insert_after=...")
 
+        category_dicts = {
+            'macros': dict( (m.macroname, m) for m in macros ),
+            'environments': dict( (e.environmentname, e) for e in environments ),
+            'specials': dict( (s.specials_chars, s) for s in specials ),
+        }
+
+        logger.debug("Adding category context in db: %r", category_dicts)
+
         if prepend:
-            self.category_list.insert(0, category)
+            insert_fn = lambda listobj, item: listobj.insert(0, item)
         elif insert_before:
             if insert_before in self.category_list:
                 i = self.category_list.index(insert_before)
             else:
                 i = 0
-            self.category_list.insert(i, category)
+            insert_fn = lambda listobj, item: listobj.insert(i, item)
         elif insert_after:
             if insert_after in self.category_list:
                 i = self.category_list.index(insert_after) + 1 # insert after found category
             else:
                 i = len(self.category_list)
-            self.category_list.insert(i, category)
+            insert_fn = lambda listobj, item: listobj.insert(i, item)
         else:
-            self.category_list.append(category)
+            insert_fn = lambda listobj, item: listobj.append(item)
+
+        insert_fn(self.category_list, category)
+        for which in ('macros', 'environments', 'specials',):
+            insert_fn(self.lookup_chain_maps[which].maps, category_dicts[which])
+
+        self.d[category] = category_dicts
 
-        self.d[category] = {
-            'macros': dict( (m.macroname, m) for m in macros ),
-            'environments': dict( (e.environmentname, e) for e in environments ),
-            'specials': dict( (s.specials_chars, s) for s in specials ),
-        }
         
     def set_unknown_macro_spec(self, macrospec):
         r"""
         Set the macro spec to use when encountering a macro that is not in the
         database.
         """
+        if self.frozen:
+            raise RuntimeError("You attempted to modify a frozen LatexContextDb object.")
         self.unknown_macro_spec = macrospec
 
     def set_unknown_environment_spec(self, environmentspec):
         r"""
         Set the environment spec to use when encountering a LaTeX environment that
         is not in the database.
         """
+        if self.frozen:
+            raise RuntimeError("You attempted to modify a frozen LatexContextDb object.")
         self.unknown_environment_spec = environmentspec
 
     def set_unknown_specials_spec(self, specialsspec):
         r"""
         Set the latex specials spec to use when encountering a LaTeX environment
         that is not in the database.
+        
+        ### FIXME: When is an "unknown specials" encountered ??
         """
+        if self.frozen:
+            raise RuntimeError("You attempted to modify a frozen LatexContextDb object.")
         self.unknown_specials_spec = specialsspec
 
     def categories(self):
         r"""
         Return a list of valid category names that are registered in the current
         database context.
         """
         return list(self.category_list)
 
-    def get_macro_spec(self, macroname):
+    def get_macro_spec(self, macroname, raise_if_not_found=False):
         r"""
         Look up a macro specification by macro name.  The macro name is searched for
         in all categories one by one and the first match is returned.
 
         Returns a macro spec instance that matches the given `macroname`.  If
         the macro name was not found, we return the default macro specification
         set by :py:meth:`set_unknown_macro_spec()` or `None` if no such spec was
-        set.
+        set.  
         """
-        for cat in self.category_list:
-            # search categories in the given order
-            if macroname in self.d[cat]['macros']:
-                return self.d[cat]['macros'][macroname]
-        return self.unknown_macro_spec
+        # for cat in self.category_list:
+        #     # search categories in the given order
+        #     if macroname in self.d[cat]['macros']:
+        #         return self.d[cat]['macros'][macroname]
+        try:
+            return self.lookup_chain_maps['macros'][macroname]
+        except KeyError:
+            if raise_if_not_found:
+                raise
+            return self.unknown_macro_spec
     
-    def get_environment_spec(self, environmentname):
+    def get_environment_spec(self, environmentname, raise_if_not_found=False):
         r"""
         Look up an environment specification by environment name.  The environment
         name is searched for in all categories one by one and the first match is
         returned.
 
         Returns the environment spec.  If the environment name was not found, we
         return the default environment specification set by
         :py:meth:`set_unknown_environment_spec()` or `None` if no such spec was
         set.
         """
-        for cat in self.category_list:
-            # search categories in the given order
-            if environmentname in self.d[cat]['environments']:
-                return self.d[cat]['environments'][environmentname]
-        return self.unknown_environment_spec
+        # for cat in self.category_list:
+        #     # search categories in the given order
+        #     if environmentname in self.d[cat]['environments']:
+        #         return self.d[cat]['environments'][environmentname]
+        try:
+            return self.lookup_chain_maps['environments'][environmentname]
+        except KeyError:
+            if raise_if_not_found:
+                raise
+            return self.unknown_environment_spec
 
-    def get_specials_spec(self, specials_chars):
+    def get_specials_spec(self, specials_chars, raise_if_not_found=False):
         r"""
         Look up a "latex specials" specification by character sequence.  The
         sequence name is searched for in all categories one by one and the first
         match is returned.
 
         If you are parsing a chunk of LaTeX code, you should use
         :py:meth:`test_for_specials()` instead.  Unlike
@@ -580,39 +317,51 @@
         sequence and one is looking up additional specs on it.]
 
         Returns the specials spec.  If the latex specials was not found, we
         return the default latex specials specification set by
         :py:meth:`set_unknown_specials_spec()` or `None` if no such spec was
         set.
         """
-        for cat in self.category_list:
-            # search categories in the given order
-            if specials_chars in self.d[cat]['specials']:
-                return self.d[cat]['specials'][specials_chars]
-        return self.unknown_specials_spec
+        # for cat in self.category_list:
+        #     # search categories in the given order
+        #     if specials_chars in self.d[cat]['specials']:
+        #         return self.d[cat]['specials'][specials_chars]
+        try:
+            return self.lookup_chain_maps['specials'][specials_chars]
+        except KeyError:
+            if raise_if_not_found:
+                raise
+            return self.unknown_specials_spec
 
     def test_for_specials(self, s, pos, parsing_state=None):
         r"""
         Test the given position in the string for any LaTeX specials.  The lookup
         proceeds by searching for in all categories one by one and the first
         match is returned, except that the longest match accross all categories
         is returned.  For instance, a match of '``' in a later category will
         take precedence over a match of '`' in a earlier-searched category.
 
         Returns a specials spec instance, or `None` if no specials are detected
         at the position `pos`.
         """
         best_match_len = 0
         best_match_s = None
+
+        logger.debug("test_for_specials() category_list=%r", self.category_list)
+
         for cat in self.category_list:
             # search categories in the given order
             for specials_chars in self.d[cat]['specials'].keys():
+                logger.debug("test_for_specials() ‘%s...’ testing %r",
+                             s[pos:pos+4], specials_chars)
                 if len(specials_chars) > best_match_len and s.startswith(specials_chars, pos):
                     best_match_s = self.d[cat]['specials'][specials_chars]
                     best_match_len = len(specials_chars)
+                    # logger.debug("        -> best_match_s=%s, best_match_len=%s",
+                    #              best_match_s, best_match_len)
 
         return best_match_s # this is None if no match
 
     def iter_macro_specs(self, categories=None):
         r"""
         Yield the macro specs corresponding to all macros in the given categories.
 
@@ -626,16 +375,18 @@
         """
 
         if categories is None:
             categories = self.category_list
 
         for c in categories:
             if c not in self.category_list:
-                raise ValueError("Invalid latex macro spec db category: {!r} (Expected one of {!r})"
-                                 .format(c, self.category_list))
+                raise ValueError(
+                    "Invalid latex macro spec db category: {!r} (Expected one of {!r})"
+                    .format(c, self.category_list)
+                )
             for spec in self.d[c]['macros'].values():
                 yield spec
 
     def iter_environment_specs(self, categories=None):
         r"""
         Yield the environment specs corresponding to all environments in the given
         categories.
@@ -676,22 +427,36 @@
         """
 
         if categories is None:
             categories = self.category_list
 
         for c in categories:
             if c not in self.category_list:
-                raise ValueError("Invalid latex environment spec db category: {!r} (Expected one of {!r})"
-                                 .format(c, self.category_list))
+                raise ValueError(
+                    "Invalid latex environment spec db category: {!r} (Expected one of {!r})"
+                    .format(c, self.category_list)
+                )
             for spec in self.d[c]['specials'].values():
                 yield spec
 
 
-    def filter_context(self, keep_categories=[], exclude_categories=[],
-                       keep_which=[]):
+    def filter_context(self, *args, **kwargs):
+        r"""
+        .. deprecated:: 3.0
+
+           The `filter_context()` method was renamed `filtered_context()`.  The
+           method signature is unchanged.
+        """
+        _util.pylatexenc_deprecated_3("`LatexContextDb.filter_context()` was renamed to "
+                                      "`filtered_context()`.")
+        return self.filtered_context(*args, **kwargs)
+
+
+    def filtered_context(self, keep_categories=[], exclude_categories=[],
+                         keep_which=[], create_class=None):
         r"""
         Return a new :py:class:`LatexContextDb` instance where we only keep
         certain categories of macro and environment specifications.
         
         If `keep_categories` is set to a nonempty list, then the returned
         context will not contain any definitions that do not correspond to the
         specified categories.
@@ -710,15 +475,18 @@
         
         The returned context will make a copy of the dictionaries that store the
         macro and environment specifications, but the specification classes (and
         corresponding argument parsers) might correspond to the same instances.
         I.e., the returned context is not a full deep copy.
         """
         
-        new_context = LatexContextDb()
+        if create_class is None:
+            create_class = self.__class__
+
+        new_context = create_class()
 
         new_context.unknown_macro_spec = self.unknown_macro_spec
         new_context.unknown_environment_spec = self.unknown_environment_spec
         new_context.unknown_specials_spec = self.unknown_specials_spec
 
         keep_macros = not keep_which or 'macros' in keep_which
         keep_environments = not keep_which or 'environments' in keep_which
@@ -736,8 +504,212 @@
                 macros=self.d[cat]['macros'].values() if keep_macros else [],
                 environments=self.d[cat]['environments'].values() if keep_environments else [],
                 specials=self.d[cat]['specials'].values() if keep_specials else [],
             )
 
         return new_context
 
+    def _get_new_autogen_category(self):
+        while True:
+            category = _autogen_category_prefix + str(self._autogen_category_counter)
+            if category not in self.category_list:
+                break
+            self._autogen_category_counter += 1
+            
+        return (self._autogen_category_counter, category)
+
+    def extended_with(self, category=None, macros=None, environments=None, specials=None,
+                      create_class=None, **kwargs):
+        r"""
+        Creates a new context category by adding a new category before all others.
+        (Behaves as you'd imagine immediately after issuing a
+        ``\newcommand\newmacro{...}``).
+
+        If `category` is `None`, then an internal category name is used.
+
+        (Note: If `category` is `None`, it might happen that a new category
+        isn't actually created; if the current object's first category is
+        already an internally-created one, that one is used.)
+        """
+
+        if category in self.category_list:
+            raise ValueError
+
+        if not self.frozen:
+            raise RuntimeError(
+                "You can only call extended_with() on frozen objects, because extended "
+                "objects keep references to the original objects' data"
+            )
+
+        if create_class is None:
+            create_class = self.__class__
+
+        new_context = create_class()
+
+        new_context.unknown_macro_spec = \
+            kwargs.pop('unknown_macro_spec', self.unknown_macro_spec)
+        new_context.unknown_environment_spec = \
+            kwargs.pop('unknown_environment_spec', self.unknown_environment_spec)
+        new_context.unknown_specials_spec = \
+            kwargs.pop('unknown_specials_spec', self.unknown_specials_spec)
+
+        if macros is None: macros = []
+        if environments is None: environments = []
+        if specials is None: specials = []
+
+        new_category_dicts = {
+            'macros': dict( (m.macroname, m) for m in macros ),
+            'environments': dict( (e.environmentname, e) for e in environments ),
+            'specials': dict( (s.specials_chars, s) for s in specials ),
+        }
+
+        new_context.category_list = self.category_list
+
+        # actual changes in macros/environments/specials, not only
+        # unknown_macro_spec=...
+
+        # logger.debug("extended_with() extending context, category=%r, category_list=%r",
+        #              category, self.category_list)
+
+        if category is None and len(self.category_list) > 0 \
+           and self.category_list[0].startswith(_autogen_category_prefix):
+            # no need to create new category, can merge with our current
+            # internally-named one.
+            cat = self.category_list[0]
+            dd = dict(self.d)
+            d_cat = dd[cat]
+            # logger.debug("extended_with() DEBUG: d_cat=%r, new_category_dicts=%r",
+            #              d_cat, new_category_dicts)
+            # Make copies of macros, environments, specials dicts to update them
+            # with the new definitions.  Avoid the construction dict(olddict,
+            # **new_stuff) because it doesn't seem to work with Transcrypt.
+            d_cat = dict(
+                macros=dict(d_cat['macros']),
+                environments=dict(d_cat['environments']),
+                specials=dict(d_cat['specials']),
+            )
+            d_cat['macros'].update(new_category_dicts['macros'])
+            d_cat['environments'].update(new_category_dicts['environments'])
+            d_cat['specials'].update(new_category_dicts['specials'])
+            # logger.debug("extended_with() DEBUG: updated d_cat is now = %r ; None is %r",
+            #              d_cat, None)
+            dd[cat] = d_cat
+            new_context.d = dd
+            new_context.lookup_chain_maps = {
+                'macros': _util.ChainMap(
+                    d_cat['macros'],
+                    *self.lookup_chain_maps['macros'].maps[1:]
+                ),
+                'environments': _util.ChainMap(
+                    d_cat['environments'],
+                    *self.lookup_chain_maps['environments'].maps[1:]
+                ),
+                'specials': _util.ChainMap(
+                    d_cat['specials'],
+                    *self.lookup_chain_maps['specials'].maps[1:]
+                ),
+            }
+            new_context._autogen_category_counter = self._autogen_category_counter
+
+            # need to be frozen to prevent edits here affecting edits in the original object
+            new_context.frozen = True
+            logger.debug(
+                "Latex Context DB %r ---> extended with %r [extend auto-cat %s] ---> %r",
+                self,
+                {k: list(v.keys()) for k, v in new_category_dicts.items()},
+                cat,
+                new_context
+            )
+            return new_context
+
+        if category is None:
+            a, category = self._get_new_autogen_category()
+            new_context._autogen_category_counter = a + 1
+        else:
+            new_context._autogen_category_counter = self._autogen_category_counter
+
+        # creating new category
+        dd = dict(self.d)
+        dd[category] = new_category_dicts
+
+        new_context.category_list = [category] + self.category_list
+
+        new_context.d = dd
+
+        # logger.debug('new context category_list = %r\n        d = %r',
+        #              new_context.category_list, new_context.d)
+
+        # these chainmaps' list of maps mirror the category_list item for item.
+        new_context.lookup_chain_maps = {
+            'macros':
+                self.lookup_chain_maps['macros']
+                .new_child(new_category_dicts['macros']),
+            'environments':
+                self.lookup_chain_maps['environments']
+                .new_child(new_category_dicts['environments']),
+            'specials':
+                self.lookup_chain_maps['specials']
+                .new_child(new_category_dicts['specials']),
+        }
+
+        new_context.frozen = True
+
+        logger.debug(
+            "Latex Context DB %r ---> extended with %r [new cat %s] ---> %r",
+            self,
+            {k: list(v.keys()) for k, v in new_category_dicts.items()},
+            category,
+            new_context
+        )
+
+        #logger.debug("extended_with(): new context is = %r", new_context)
+        return new_context
+
+
+
+
+
+class ParsingStateDeltaExtendLatexContextDb(ParsingStateDelta):
+    r"""
+    In addition to setting attributes, this parsing state delta object can also
+    extend the latex context.
+
+    .. py:attribute::  extend_latex_context
+
+       A dictionary with keys 'macros', 'environments', 'specials', as accepted
+       by :py:meth:`LatexContextDb.add_context_category()`.
+        
+       Can be used along with set_parsing_state; in which case definitions are
+       added on top of the parsing state change.
+    """
+    def __init__(self, extend_latex_context, **kwargs):
+        super(ParsingStateDeltaExtendLatexContextDb, self).__init__(
+            _fields=('extend_latex_context', 'set_attributes',),
+            **kwargs
+        )
+        self.extend_latex_context = extend_latex_context
+
+    def get_updated_parsing_state(self, parsing_state, latex_walker):
+
+        if self.extend_latex_context:
+
+            if self.set_attributes:
+                set_attributes = self.set_attributes
+            else:
+                set_attributes = {}
+
+            latex_context = parsing_state.latex_context.extended_with(
+                category=None,
+                **self.extend_latex_context
+            )
+
+            return parsing_state.sub_context(
+                latex_context=latex_context,
+                **set_attributes
+            )
+        elif self.set_attributes:
+            return parsing_state.sub_context(
+                **self.set_attributes
+            )
+
+        return parsing_state
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pylatexenc-2.9/pylatexenc/version.py` & `pylatexenc-3.0a13/pylatexenc/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 #   7) on github.com, fill in release details with a summary of changes etc.
 #
 #   8) create the source package for PyPI (" python3 setup.py sdist ")
 #   
 #   8) upload package to PyPI (twine upload dist/pylatexenc-X.X.tar.gz -r realpypi)
 #
 
-version_str = "2.9"
+version_str = "3.0alpha000013"
```

### Comparing `pylatexenc-2.9/setup.py` & `pylatexenc-3.0a13/pylatexenc/macrospec/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+# -*- coding: utf-8 -*-
 #
 # The MIT License (MIT)
 # 
-# Copyright (c) 2019 Philippe Faist
+# Copyright (c) 2022 Philippe Faist
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,61 +19,57 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-import os
-import os.path
-#import sys
-
-from setuptools import setup, find_packages
-
-from pylatexenc.version import version_str
-
-def read(*paths):
-    """Build a file path from *paths* and return the contents."""
-    with open(os.path.join(*paths), 'r') as f:
-        return f.read()
-
-setup(
-    name = "pylatexenc",
-    version = version_str,
-
-    # metadata for upload to PyPI
-    author = "Philippe Faist",
-    author_email = "philippe.faist@bluewin.ch",
-    description = "Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion",
-    long_description = read("README.rst"),
-    license = "MIT",
-    keywords = "latex text unicode encode parse expression",
-    url = "https://github.com/phfaist/pylatexenc",
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Microsoft :: Windows',
-        'Operating System :: POSIX :: Linux',
-        'Intended Audience :: Developers',
-        'Topic :: Scientific/Engineering',
-        'Topic :: Text Processing :: General',
-        'Topic :: Text Processing :: Markup :: LaTeX',
-    ],
-
-    # files
-    packages = find_packages(),
-    entry_points = {
-        'console_scripts': [
-            'latexwalker=pylatexenc.latexwalker.__main__:main',
-            'latex2text=pylatexenc.latex2text.__main__:main',
-            'latexencode=pylatexenc.latexencode.__main__:main',
-        ],
-    },
-    install_requires = [],
-    package_data = {
-    },
+r"""
+Provides classes and helper functions to describe a LaTeX context of known
+macros and environments, specifying how they should be parsed by
+:py:mod:`pylatexenc.latexwalker`.
+
+.. versionadded:: 2.0
+
+   The entire module :py:mod:`pylatexenc.macrospec` was introduced in
+   `pylatexenc 2.0`.
+"""
+
+
+from ._specclasses import MacroSpec, EnvironmentSpec, SpecialsSpec
+
+### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
+from ._spechelpers import std_macro, std_environment, std_specials
+### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
+
+
+from ._latexcontextdb import (
+    LatexContextDb,
+    ParsingStateDeltaExtendLatexContextDb,
+)
+
+from ._argumentsparser import (
+    LatexArgumentsParser
 )
+
+from ._environmentbodyparser import (
+    LatexEnvironmentBodyContentsParser
+)
+
+from ._macrocallparser import (
+    LatexMacroCallParser,
+    LatexEnvironmentCallParser,
+    LatexSpecialsCallParser
+)
+
+
+### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
+from ..latexnodes import ParsedArguments as ParsedMacroArgs
+from ._pyltxenc2_argparsers import (
+    MacroStandardArgsParser,
+    ParsedVerbatimArgs,
+    VerbatimArgsParser,
+    ParsedLstListingArgs,
+    LstListingArgsParser,
+)
+### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
+
```

