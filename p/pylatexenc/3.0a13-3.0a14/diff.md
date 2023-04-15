# Comparing `tmp/pylatexenc-3.0a13.tar.gz` & `tmp/pylatexenc-3.0a14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylatexenc-3.0a13.tar", max compression
+gzip compressed data, was "pylatexenc-3.0a14.tar", max compression
```

## Comparing `pylatexenc-3.0a13.tar` & `pylatexenc-3.0a14.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1086 2023-04-15 13:24:30.143033 pylatexenc-3.0a13/LICENSE.txt
--rw-r--r--   0        0        0     2830 2023-04-15 11:30:13.187333 pylatexenc-3.0a13/README.rst
--rw-r--r--   0        0        0     1326 2019-07-25 20:20:56.000000 pylatexenc-3.0a13/pylatexenc/__init__.py
--rw-r--r--   0        0        0     5162 2023-04-15 11:29:53.841130 pylatexenc-3.0a13/pylatexenc/_util.py
--rw-r--r--   0        0        0     3766 2023-04-15 11:29:53.841423 pylatexenc-3.0a13/pylatexenc/_util_support.py
--rw-r--r--   0        0        0    59269 2023-04-15 11:57:13.282343 pylatexenc-3.0a13/pylatexenc/latex2text/__init__.py
--rw-r--r--   0        0        0    10011 2023-04-15 11:55:00.471421 pylatexenc-3.0a13/pylatexenc/latex2text/__main__.py
--rw-r--r--   0        0        0    94342 2023-04-15 11:29:53.843500 pylatexenc-3.0a13/pylatexenc/latex2text/_defaultspecs.py
--rw-r--r--   0        0        0     2526 2021-12-17 19:22:56.000000 pylatexenc-3.0a13/pylatexenc/latex2text/_inputlatexfile.py
--rw-r--r--   0        0        0    12944 2021-03-31 23:28:40.000000 pylatexenc-3.0a13/pylatexenc/latexencode/__init__.py
--rw-r--r--   0        0        0     4426 2019-08-25 13:06:29.000000 pylatexenc-3.0a13/pylatexenc/latexencode/__main__.py
--rw-r--r--   0        0        0     4404 2023-04-15 12:03:11.103995 pylatexenc-3.0a13/pylatexenc/latexencode/_partial_latex_encoder.py
--rw-r--r--   0        0        0    99833 2021-09-15 19:08:59.000000 pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap.py
--rw-r--r--   0        0        0    55947 2019-07-27 15:08:32.000000 pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap_xml.py
--rw-r--r--   0        0        0    26209 2021-04-01 11:51:30.000000 pylatexenc-3.0a13/pylatexenc/latexencode/_unicode_to_latex_encoder.py
--rw-r--r--   0        0        0     2179 2023-04-15 11:29:53.843788 pylatexenc-3.0a13/pylatexenc/latexnodes/__init__.py
--rw-r--r--   0        0        0     2088 2023-04-15 11:29:53.844020 pylatexenc-3.0a13/pylatexenc/latexnodes/_callablespecbase.py
--rw-r--r--   0        0        0    10957 2023-04-15 11:29:53.844375 pylatexenc-3.0a13/pylatexenc/latexnodes/_exctypes.py
--rw-r--r--   0        0        0     6203 2023-04-15 11:29:53.844620 pylatexenc-3.0a13/pylatexenc/latexnodes/_latexcontextdbbase.py
--rw-r--r--   0        0        0    36350 2023-04-15 11:29:53.845057 pylatexenc-3.0a13/pylatexenc/latexnodes/_nodescollector.py
--rw-r--r--   0        0        0    10124 2023-04-15 11:29:53.845301 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsedargs.py
--rw-r--r--   0        0        0    11877 2023-04-15 11:29:53.845584 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsedargsinfo.py
--rw-r--r--   0        0        0    17301 2023-04-15 11:29:53.845881 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsingstate.py
--rw-r--r--   0        0        0     7109 2023-04-15 11:29:53.846228 pylatexenc-3.0a13/pylatexenc/latexnodes/_parsingstatedelta.py
--rw-r--r--   0        0        0     8145 2023-04-15 11:29:53.846477 pylatexenc-3.0a13/pylatexenc/latexnodes/_token.py
--rw-r--r--   0        0        0    27323 2023-04-15 11:29:53.846903 pylatexenc-3.0a13/pylatexenc/latexnodes/_tokenreader.py
--rw-r--r--   0        0        0     9984 2023-04-15 11:29:53.847231 pylatexenc-3.0a13/pylatexenc/latexnodes/_tokenreaderbase.py
--rw-r--r--   0        0        0     3711 2023-04-15 11:29:53.847509 pylatexenc-3.0a13/pylatexenc/latexnodes/_walkerbase.py
--rw-r--r--   0        0        0    41971 2023-04-15 11:29:53.847946 pylatexenc-3.0a13/pylatexenc/latexnodes/nodes.py
--rw-r--r--   0        0        0     2141 2023-04-15 11:29:53.848262 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/__init__.py
--rw-r--r--   0        0        0     5285 2023-04-15 11:29:53.848639 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_base.py
--rw-r--r--   0        0        0    41018 2023-04-15 11:29:53.849003 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_delimited.py
--rw-r--r--   0        0        0    18288 2023-04-15 11:29:53.849524 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_expression.py
--rw-r--r--   0        0        0    12896 2023-04-15 11:29:53.849773 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_generalnodes.py
--rw-r--r--   0        0        0     5658 2023-04-15 11:29:53.849985 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_math.py
--rw-r--r--   0        0        0     6180 2023-04-15 11:29:53.850252 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_optionals.py
--rw-r--r--   0        0        0    22366 2023-04-15 11:29:53.850621 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_stdarg.py
--rw-r--r--   0        0        0    11290 2023-04-15 11:29:53.850847 pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_verbatim.py
--rw-r--r--   0        0        0     4520 2023-04-15 11:29:53.851132 pylatexenc-3.0a13/pylatexenc/latexwalker/__init__.py
--rw-r--r--   0        0        0     6214 2023-04-15 11:29:53.851406 pylatexenc-3.0a13/pylatexenc/latexwalker/__main__.py
--rw-r--r--   0        0        0    17383 2023-04-15 11:29:53.851774 pylatexenc-3.0a13/pylatexenc/latexwalker/_defaultspecs.py
--rw-r--r--   0        0        0     2937 2023-04-15 11:29:53.852111 pylatexenc-3.0a13/pylatexenc/latexwalker/_get_defaultspecs.py
--rw-r--r--   0        0        0     7833 2023-04-15 11:29:53.852354 pylatexenc-3.0a13/pylatexenc/latexwalker/_helpers.py
--rw-r--r--   0        0        0     7487 2023-04-15 11:29:53.852626 pylatexenc-3.0a13/pylatexenc/latexwalker/_legacy_py1x.py
--rw-r--r--   0        0        0    52642 2023-04-15 11:37:07.707893 pylatexenc-3.0a13/pylatexenc/latexwalker/_walker.py
--rw-r--r--   0        0        0     2341 2023-04-15 11:29:53.853314 pylatexenc-3.0a13/pylatexenc/macrospec/__init__.py
--rw-r--r--   0        0        0     8525 2023-04-15 11:29:53.853602 pylatexenc-3.0a13/pylatexenc/macrospec/_argumentsparser.py
--rw-r--r--   0        0        0     7372 2023-04-15 11:29:53.853904 pylatexenc-3.0a13/pylatexenc/macrospec/_environmentbodyparser.py
--rw-r--r--   0        0        0    29706 2023-04-15 11:29:53.854223 pylatexenc-3.0a13/pylatexenc/macrospec/_latexcontextdb.py
--rw-r--r--   0        0        0    10045 2023-04-15 11:29:53.854565 pylatexenc-3.0a13/pylatexenc/macrospec/_macrocallparser.py
--rw-r--r--   0        0        0     1535 2023-04-15 11:29:53.854841 pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
--rw-r--r--   0        0        0     8866 2023-04-15 11:29:53.855062 pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
--rw-r--r--   0        0        0    16112 2023-04-15 11:29:53.855268 pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
--rw-r--r--   0        0        0    15650 2023-04-15 11:29:53.855594 pylatexenc-3.0a13/pylatexenc/macrospec/_specclasses.py
--rw-r--r--   0        0        0     8951 2023-04-15 11:29:53.855874 pylatexenc-3.0a13/pylatexenc/macrospec/_spechelpers.py
--rw-r--r--   0        0        0     2054 2023-04-15 13:21:15.064333 pylatexenc-3.0a13/pylatexenc/version.py
--rw-r--r--   0        0        0     1091 2023-04-15 13:21:32.120070 pylatexenc-3.0a13/pyproject.toml
--rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 pylatexenc-3.0a13/setup.py
--rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 pylatexenc-3.0a13/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-15 20:22:30.680495 pylatexenc-3.0a14/LICENSE.txt
+-rw-r--r--   0        0        0     2830 2023-04-15 20:22:30.680495 pylatexenc-3.0a14/README.rst
+-rw-r--r--   0        0        0     1326 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/__init__.py
+-rw-r--r--   0        0        0     5162 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/_util.py
+-rw-r--r--   0        0        0     3766 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/_util_support.py
+-rw-r--r--   0        0        0    59269 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/__init__.py
+-rw-r--r--   0        0        0    10011 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/__main__.py
+-rw-r--r--   0        0        0    94342 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/_defaultspecs.py
+-rw-r--r--   0        0        0     2526 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/_inputlatexfile.py
+-rw-r--r--   0        0        0    12944 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/__init__.py
+-rw-r--r--   0        0        0     4426 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/__main__.py
+-rw-r--r--   0        0        0     4404 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_partial_latex_encoder.py
+-rw-r--r--   0        0        0    99833 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap.py
+-rw-r--r--   0        0        0    55947 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap_xml.py
+-rw-r--r--   0        0        0    26209 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_unicode_to_latex_encoder.py
+-rw-r--r--   0        0        0     2179 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/__init__.py
+-rw-r--r--   0        0        0     2197 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/_callablespecbase.py
+-rw-r--r--   0        0        0    11001 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/_exctypes.py
+-rw-r--r--   0        0        0     6315 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/_latexcontextdbbase.py
+-rw-r--r--   0        0        0    36489 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_nodescollector.py
+-rw-r--r--   0        0        0    10124 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargs.py
+-rw-r--r--   0        0        0    11877 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargsinfo.py
+-rw-r--r--   0        0        0    17020 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstate.py
+-rw-r--r--   0        0        0     7109 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstatedelta.py
+-rw-r--r--   0        0        0     8446 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_token.py
+-rw-r--r--   0        0        0    27434 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreader.py
+-rw-r--r--   0        0        0    10098 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreaderbase.py
+-rw-r--r--   0        0        0     4841 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_walkerbase.py
+-rw-r--r--   0        0        0    42174 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/nodes.py
+-rw-r--r--   0        0        0     2141 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/__init__.py
+-rw-r--r--   0        0        0     5285 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_base.py
+-rw-r--r--   0        0        0    41024 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_delimited.py
+-rw-r--r--   0        0        0    18288 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_expression.py
+-rw-r--r--   0        0        0    12896 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_generalnodes.py
+-rw-r--r--   0        0        0     5658 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_math.py
+-rw-r--r--   0        0        0     6180 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_optionals.py
+-rw-r--r--   0        0        0    22370 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_stdarg.py
+-rw-r--r--   0        0        0    11301 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_verbatim.py
+-rw-r--r--   0        0        0     4520 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/__init__.py
+-rw-r--r--   0        0        0     6214 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/__main__.py
+-rw-r--r--   0        0        0    17383 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_defaultspecs.py
+-rw-r--r--   0        0        0     2937 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_get_defaultspecs.py
+-rw-r--r--   0        0        0     7833 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_helpers.py
+-rw-r--r--   0        0        0     7487 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_legacy_py1x.py
+-rw-r--r--   0        0        0    52642 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_walker.py
+-rw-r--r--   0        0        0     2341 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/__init__.py
+-rw-r--r--   0        0        0     8525 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_argumentsparser.py
+-rw-r--r--   0        0        0     7372 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_environmentbodyparser.py
+-rw-r--r--   0        0        0    29706 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_latexcontextdb.py
+-rw-r--r--   0        0        0    10045 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_macrocallparser.py
+-rw-r--r--   0        0        0     1535 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
+-rw-r--r--   0        0        0     8866 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
+-rw-r--r--   0        0        0    16110 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
+-rw-r--r--   0        0        0    15650 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_specclasses.py
+-rw-r--r--   0        0        0     8951 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_spechelpers.py
+-rw-r--r--   0        0        0     2115 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/version.py
+-rw-r--r--   0        0        0     1091 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pyproject.toml
+-rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 pylatexenc-3.0a14/setup.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 pylatexenc-3.0a14/PKG-INFO
```

### Comparing `pylatexenc-3.0a13/LICENSE.txt` & `pylatexenc-3.0a14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/README.rst` & `pylatexenc-3.0a14/README.rst`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/__init__.py` & `pylatexenc-3.0a14/pylatexenc/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/_util.py` & `pylatexenc-3.0a14/pylatexenc/_util.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/_util_support.py` & `pylatexenc-3.0a14/pylatexenc/_util_support.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latex2text/__init__.py` & `pylatexenc-3.0a14/pylatexenc/latex2text/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latex2text/__main__.py` & `pylatexenc-3.0a14/pylatexenc/latex2text/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latex2text/_defaultspecs.py` & `pylatexenc-3.0a14/pylatexenc/latex2text/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latex2text/_inputlatexfile.py` & `pylatexenc-3.0a14/pylatexenc/latex2text/_inputlatexfile.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexencode/__init__.py` & `pylatexenc-3.0a14/pylatexenc/latexencode/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexencode/__main__.py` & `pylatexenc-3.0a14/pylatexenc/latexencode/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexencode/_partial_latex_encoder.py` & `pylatexenc-3.0a14/pylatexenc/latexencode/_partial_latex_encoder.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap.py` & `pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexencode/_uni2latexmap_xml.py` & `pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap_xml.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexencode/_unicode_to_latex_encoder.py` & `pylatexenc-3.0a14/pylatexenc/latexencode/_unicode_to_latex_encoder.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/__init__.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_callablespecbase.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_callablespecbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,11 +41,15 @@
     construct (macro, environment, or specials).
 
     The spec object should implement :py:meth:`get_node_parser()`, and it should
     return a parser instance that can be used to parse the entire construct.
 
     See :py:class:`macrospec.MacroSpec` for how this is implemented in the
     :py:mod:`pylatexenc.macrospec` module.
+
+    .. versionadded:: 3.0
+    
+       The :py:class:`CallableSpecBase` class was added in `pylatexenc 3.0`.
     """
 
     def get_node_parser(self, token):
         raise RuntimeError("Subclasses must reimplement get_node_parser()")
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_exctypes.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_exctypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 # the other modules' namespaces, we define __all__ here.
 
 
 __all__ = [
     'LatexWalkerError',
     'LatexWalkerLocatedError',
     'LatexWalkerParseError',
-    'LatexWalkerParseErrorFormatter',
+    'LatexWalkerLocatedErrorFormatter',
     'LatexWalkerNodesParseError',
     'LatexWalkerTokenParseError',
     'LatexWalkerEndOfStream',
 ]
 
 
 
@@ -131,19 +131,19 @@
         self.open_contexts = kwargs.pop('open_contexts', [])
 
         if len(kwargs):
             raise ValueError("Unexpected keyword argument(s) to LatexWalkerParseError(): "
                              + repr(kwargs))
 
         super(LatexWalkerLocatedError, self).__init__(
-            LatexWalkerParseErrorFormatter(self).to_display_string()
+            LatexWalkerLocatedErrorFormatter(self).to_display_string()
         )
 
     def __str__(self):
-        return LatexWalkerParseErrorFormatter(self).to_display_string()
+        return LatexWalkerLocatedErrorFormatter(self).to_display_string()
 
     #
     # ### Problem: other_exception might have properties (e.g., from a
     # ### token-walker-parse-error) that are incompatible with the Cls class
     # ### (e.g. nodes-walker-parse-error)
     #
     # @classmethod
@@ -168,17 +168,21 @@
     Represents an error while LaTeX code, specifically while parsing the
     code into the nodes structure.
     """
     pass
 
 
 
-class LatexWalkerParseErrorFormatter(object):
+class LatexWalkerLocatedErrorFormatter(object):
+    r"""
+    Format the 
+    """
+
     def __init__(self, exc):
-        super(LatexWalkerParseErrorFormatter, self).__init__()
+        super(LatexWalkerLocatedErrorFormatter, self).__init__()
         self.exc = exc
         
     def format_open_blocks(self):
         exc = self.exc
         if not exc.open_contexts:
             return None
         disp = ''
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_latexcontextdbbase.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_latexcontextdbbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     object is simply an object that provides the :py:meth:`get_***_spec()`
     family of methods along with :py:meth:`test_for_specials()`, and they return
     relevant spec objects.
 
     The spec objects returned by :py:meth:`get_***_spec()` and
     :py:meth:`test_for_specials()` are subclasses of
     :py:class:`CallableSpecBase`.
+
+
+    .. versionadded:: 3.0
+    
+       The :py:class:`LatexContextDbBase` class was added in `pylatexenc 3.0`.
     """
 
     def get_macro_spec(self, macroname):
         r"""
         Return the macro spec to use to parse a macro named `macroname`.  The
         `macroname` does not contain the escape character (``\``) itself.
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_nodescollector.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_nodescollector.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,19 @@
     macros, environments, specials, etc. in the bulk that is being parsed.  The
     result is a node list containing a full tree of child nodes that represents
     the logical structure of the tokens that were encountered.
     
     The public API of this class resides essentially in the
     :py:meth:`process_tokens()`, as well as the :py:meth:`get_final_nodelist()`
     (and some other friends, see docs below).
+
+
+    .. versionadded:: 3.0
+    
+       The :py:class:`LatexNodesCollector` class was added in `pylatexenc 3.0`.
     """
 
     class ReachedEndOfStream(Exception):
         r"""
         Raised by the :py:meth:`process_one_token()` method if we reached the end of
         stream.
         
@@ -151,14 +156,15 @@
             nodelist=self._nodelist,
             parsing_state=self.start_parsing_state,
         )
 
 
     def get_parser_parsing_state_delta(self):
         r"""
+        Doc. ............
         """
         if not self._finalized:
             raise RuntimeError("Call to get_parser_parsing_state_delta() before finalize()")
 
         if self.start_parsing_state is self.parsing_state:
             # we ended with the same object as the initial parsing state
             return None
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_parsedargs.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_parsedargsinfo.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargsinfo.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_parsingstate.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstate.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,33 +42,14 @@
 import sys
 if sys.version_info.major == 2:
     _unisafe_arrow_s = '->'
 ### END_PYTHON2_SUPPORT_CODE
 
 
 
-# class _StrictAsciiAlphaChars(object):
-#     def __str__(self):
-#         return "".join([
-#             chr(ord('a')+j) for j in range(26)
-#         ]) + "".join([
-#             chr(ord('A')+j) for j in range(26)
-#         ])
-#     def __repr__(self):
-#         return repr(self.__str__())
-#     def __contains__(self, c):
-#         n = ord(c)
-#         return (
-#             (97 <= n <= 122)  # 97 == ord('a'), 122 == ord('z')
-#             or
-#             (65 <= n <= 90) # 65, 90 == ord('A'), ord('Z')
-#         )
-#     def to_json_object(self):
-#         return self.__str__()
-
 # allowed macro chars by default: [a-zA-Z]
 _default_macro_alpha_chars = (
     "".join([
         chr(ord('a')+j) for j in range(26)
     ]) + "".join([
         chr(ord('A')+j) for j in range(26)
     ])
@@ -204,14 +185,21 @@
     .. versionadded:: 3.0
 
        The attributes `latex_group_delimiters`, `latex_inline_math_delimiters`,
        `latex_display_math_delimiters`, `enable_double_newline_paragraphs`,
        `enable_environments`, `enable_comments`, `macro_alpha_chars`,
        `macro_escape_char`, and `forbidden_characters` were introduced in
        version 3.
+
+    .. versionadded:: 3.0
+
+       This class was moved to :py:class:`pylatexenc.latexnodes.ParsingState`
+       starting in `pylatexenc 3.0`.  In earlier versions, this class was
+       located in the :py:mod:`~pylatexenc.latexwalker` module, see
+       :py:class:`~pylatexenc.latexwalker.ParsingState`.
     """
 
     _fields = (
         's',
         'latex_context',
         'in_math_mode',
         'math_mode_delimiter',
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_parsingstatedelta.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstatedelta.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_token.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -142,14 +142,21 @@
 
     .. versionchanged:: 3.0
 
        Starting in `pylatexenc 3`, the `len` argument was replaced by `pos_end`.
        For backwards compatibility, `kwargs` arguments are inspected for a `len`
        argument.  If a `len` argument is provided and `pos_end` was left `None`,
        then `pos_end` is set to `pos+len`.
+
+    .. versionadded:: 3.0
+
+       This class was moved to :py:class:`pylatexenc.latexnodes.LatexToken`
+       starting in `pylatexenc 3.0`.  In earlier versions, this class was
+       located in the :py:mod:`~pylatexenc.latexwalker` module, see
+       :py:class:`~pylatexenc.latexwalker.LatexToken`.
     """
     def __init__(self, tok, arg, pos, pos_end=None, pre_space='', post_space='', **kwargs):
 
         len_ = kwargs.pop('len', None)
 
         self.tok = tok
         self.arg = arg
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_tokenreader.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,19 @@
     .. py::attribute:  tolerant_parsing
 
        Whether or not we are in tolerant parsing mode.  In tolerant parsing
        mode, we go out of our way to recover from errors to produce some kind of
        useful tokens.  If not in tolerant parsing mode, then parsing is strict
        and errors are raised immediately so that they can be traced down and
        debugged more easily.
+
+
+    .. versionadded:: 3.0
+
+       The :py:class:`LatexTokenReader` class was introduced in `pylatexenc 3.0`.
     """
     def __init__(self, s, **kwargs):
         super(LatexTokenReader, self).__init__()
         self.s = s
         
         self.tolerant_parsing = kwargs.pop('tolerant_parsing', False)
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_tokenreaderbase.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreaderbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     :py:meth:`move_past_token()`, and :py:meth:`cur_pos()`.
 
     A token reader can (but does not have to) also provide character-level
     access to the input.  This can be used by some special parsers like verbatim
     parsers.  In this case, the token reader should implement
     :py:class:`peek_chars()`, :py:class:`next_chars()`, and
     :py:meth:`move_to_pos_chars()`.
+
+    .. versionadded:: 3.0
+
+       The :py:class:`LatexTokenReaderBase` class was introduced in `pylatexenc 3.0`.
     """
 
     def __init__(self, **kwargs):
         super(LatexTokenReaderBase, self).__init__(**kwargs)
 
     def make_token(self, **kwargs):
         r"""
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/_walkerbase.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/_walkerbase.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,14 +30,32 @@
 from __future__ import print_function, unicode_literals
 
 from ._parsingstatedelta import ParsingStateDelta
 
 
 
 class LatexWalkerParsingStateEventHandler(object):
+    r"""
+    A LatexWalker parsing state event handler.
+
+    The LatexWalker instance will call methods on this object to determine how
+    to update the parsing state upon certain events, such as entering or exiting
+    math mode.
+
+    Events:
+
+    - enter math mode
+
+    - exit math mode
+
+    .. versionadded:: 3.0
+    
+       The :py:class:`LatexWalkerParsingStateEventHandler` class was added in
+       `pylatexenc 3.0`.
+    """
 
     def enter_math_mode(self, math_mode_delimiter=None, trigger_token=None):
         return ParsingStateDelta(
             set_attributes=dict(
                 in_math_mode=True,
                 math_mode_delimiter=math_mode_delimiter
             )
@@ -52,40 +70,72 @@
         )
 
 
 _default_parsing_state_event_handler = LatexWalkerParsingStateEventHandler()
 
 
 class LatexWalkerBase(object):
+    r"""
+    Base class for a latex-walker.  Essentially, this is all that the
+    classes and methods in the :py:mod:`latexnodes` module need to know about
+    what a LatexWalker does.
+
+    See also :py:class:`latexwalker.LatexWalker`.
+
+    .. versionadded:: 3.0
+    
+       The :py:class:`LatexWalkerBase` class was added in `pylatexenc 3.0`.
+    """
 
     def parsing_state_event_handler(self):
+        r"""
+        Doc......
+        """
         return _default_parsing_state_event_handler
 
     def parse_content(self, parser, token_reader=None, parsing_state=None,
                       open_context=None, **kwargs):
+        r"""
+        Doc......
+        """
         raise RuntimeError("LatexWalkerBase subclasses must reimplement parse_content()")
 
     def make_node(self, node_class, **kwargs):
+        r"""
+        Doc......
+        """
         raise RuntimeError("LatexWalkerBase subclasses must reimplement make_node()")
 
     def make_nodelist(self, nodelist, **kwargs):
+        r"""
+        Doc......
+        """
         raise RuntimeError("LatexWalkerBase subclasses must reimplement make_nodelist()")
 
     def make_nodes_collector(self,
                              token_reader,
                              parsing_state,
                              **kwargs):
+        r"""
+        Doc......
+        """
         raise RuntimeError(
             "LatexWalkerBase subclasses must reimplement make_nodes_collector()")
 
     def make_latex_group_parser(self, delimiters):
+        r"""
+        Doc......
+        """
         raise RuntimeError(
             "LatexWalkerBase subclasses must reimplement make_latex_group_parser()")
         
     def make_latex_math_parser(self, math_mode_delimiters):
+        r"""
+        Doc......
+        """
         raise RuntimeError(
             "LatexWalkerBase subclasses must reimplement make_latex_math_parser()")
 
 
     def check_tolerant_parsing_ignore_error(self, exc):
         r"""
         You can inspect the exception object `exc` and decide whether or not to
@@ -94,8 +144,11 @@
 
         Return the exception object if it should be raised, or return None if
         recovery should be attempted.
         """
         return exc
 
     def format_node_pos(self, node):
+        r"""
+        Doc......
+        """
         return 'character position '+repr(node.pos)
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/nodes.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
     .. py:attribute:: spec
 
        The specification object for this macro (a :py:class:`MacroSpec`
        instance).
 
        .. versionadded:: 3.0
 
-       The `spec` attribute was introduced in `pylatexenc 3`.
+          The `spec` attribute was introduced in `pylatexenc 3`.
 
     .. py:attribute:: nodeargd
 
        The :py:class:`pylatexenc.latexnodes.ParsedArguments` object that
        represents the macro arguments.
 
        For macros that do not accept any argument, this is an empty
@@ -708,14 +708,18 @@
 
 
     .. py:attribute:: len
 
        (Read-only attribute.)  The total length spanned by this node list,
        assuming that the `nodelist` represents a single continuous sequence of
        nodes in the latex string.
+
+    .. versionadded: 3.0
+
+       The `LatexNodeList` class was introduced in `pylatexenc 3.0`.
     """
     def __init__(self, nodelist, **kwargs):
 
         if isinstance(nodelist, LatexNodeList):
             obj = nodelist
             self.nodelist = obj.nodelist
             self.parsing_state = obj.parsing_state
@@ -1177,15 +1181,19 @@
 # ------------------------------------------------------------------------------
 
 
 class LatexNodesVisitor(object):
     r"""
     Implement a visitor pattern on a node structure.
 
-    ......................
+    Doc ......................
+
+    .. versionadded: 3.0
+
+       The `LatexNodesVisitor` class was introduced in `pylatexenc 3.0`.
     """
 
     def visit(self, node):
         r"""
         Fallback for visiting any type of node.  This is called by the `visit_XXX()`
         methods below.  In your subclass, you can reimplement a subset of the
         `visit_XXXX()` methods, and whichever objects you didn't reimplement the
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/__init__.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_base.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_delimited.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_delimited.py`

 * *Files 0% similar despite different names*

```diff
@@ -910,27 +910,27 @@
             )
             return True
         return False
 
 
     def get_matching_delimiter(self, opening_delimiter):
         r"""
-        ..............
+        Doc..............
 
         This method assumes that the delimiters are latex group type (e.g., curly
         brace chars).  If not, then you need to reimplement this function in a
         subclass.
         """
         return self.group_parsing_state._latex_group_delimchars_by_open[opening_delimiter]
 
 
 
 class LatexDelimitedGroupParser(LatexDelimitedExpressionParser):
     r"""
-    .........................
+    Doc.........................
 
     In all cases, the first token read (after possible whitespace) must be a
     'brace_open' type.  If `delimiters` is a pair of characters, the parsing
     state is inspected to ensure that these delimiters are recorded as latex
     group delimiters, and will add them if necessary for parsing the group
     contents (but not its parsed children).
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_expression.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_expression.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_generalnodes.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_generalnodes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_math.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_math.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_optionals.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_optionals.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_stdarg.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_stdarg.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 # --------------------------------------------------------------------
 
 
 
 
 class LatexCharsGroupParser(LatexDelimitedGroupParser):
     r"""
-    ....................
+    Doc ....................
 
     Very similar to a verbatim parser, but works with tokens instead of chars.
     You can use comments and recursive groups, too.
 
     Will result in a group node that contains one char node (and possibly a
     combination of group, chars, and comment nodes if those were enabled)
     """
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexnodes/parsers/_verbatim.py` & `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_verbatim.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         return self.read_verbatim_content(latex_walker, token_reader, parsing_state,
                                           verbatim_info=verbatim_info, **kwargs)
 
 
     def read_verbatim_content(self, latex_walker, token_reader, parsing_state,
                               verbatim_info, **kwargs):
         r"""
-        ....
+        Doc ...........
         
         The `token_reader` is left *after* the character that caused the
         processing to stop.
         """
 
         verbatim_string = ''
         stop_condition_met = False
```

### Comparing `pylatexenc-3.0a13/pylatexenc/latexwalker/__init__.py` & `pylatexenc-3.0a14/pylatexenc/latexwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexwalker/__main__.py` & `pylatexenc-3.0a14/pylatexenc/latexwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexwalker/_defaultspecs.py` & `pylatexenc-3.0a14/pylatexenc/latexwalker/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexwalker/_get_defaultspecs.py` & `pylatexenc-3.0a14/pylatexenc/latexwalker/_get_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexwalker/_helpers.py` & `pylatexenc-3.0a14/pylatexenc/latexwalker/_helpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexwalker/_legacy_py1x.py` & `pylatexenc-3.0a14/pylatexenc/latexwalker/_legacy_py1x.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/latexwalker/_walker.py` & `pylatexenc-3.0a14/pylatexenc/latexwalker/_walker.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/__init__.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_argumentsparser.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_argumentsparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_environmentbodyparser.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_environmentbodyparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_latexcontextdb.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_latexcontextdb.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_macrocallparser.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_macrocallparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             and self.verbatim_text == other.verbatim_text
             and self.verbatim_delimiters == other.verbatim_delimiters
         )
 
 
 class VerbatimArgsParser(MacroStandardArgsParser):
     r"""
-    Parses the arguments to various LaTeX "verbatim" constructs such as
+    Parses the arguments to various LaTeX verbatim constructs such as
     ``\begin{verbatim}...\end{verbatim}`` environment or ``\verb+...+``.
 
     This class also serves to illustrate how to write custom parsers for
     complicated macro arguments.  See also :py:class:`MacroStandardArgsParser`.
 
     Arguments:
 
@@ -175,19 +175,19 @@
       the verbatim construct.  By default this is
       :py:class:`ParsedVerbatimArgs`.  You can use another class that derives
       from :py:class:`ParsedVerbatimArgs` and that accepts the same keyword
       arguments.
 
     .. py:attribute:: specials_delimiters
 
-      When parsing a "specials" form of a verbatim construct (e.g. ``|\begin|
-      and |\end| are special \LaTeX\ commands''), specify the opening and
-      closing delimiter here.  When parsing the verbatim construct, the closing
-      delimiter is searched and its first occurence is used (there is no
-      brace/parenthesis matching or anything of the kind).
+      When parsing a "specials" form of a verbatim construct (e.g.
+      ``|\begin| and |\end| are special \LaTeX\ commands``), specify the
+      opening and closing delimiter here.  When parsing the verbatim construct,
+      the closing delimiter is searched and its first occurence is used (there
+      is no brace/parenthesis matching or anything of the kind).
     """
     def __init__(self,
                  verbatim_arg_type,
                  verbatim_environment_name="verbatim",
                  verbatim_argspec='',
                  verbatim_parsed_args_class=ParsedVerbatimArgs,
                  specials_delimiters=('|', '|'),
```

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_specclasses.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_specclasses.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/macrospec/_spechelpers.py` & `pylatexenc-3.0a14/pylatexenc/macrospec/_spechelpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a13/pylatexenc/version.py` & `pylatexenc-3.0a14/pylatexenc/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 
 #
-# Self-note: Checklist
+# Self-note: Checklist --- NOTE THESE ARE OLD INSTRUCTIONS DATING FROM 2.X VERSIONS
 #
 #   1) First some checks:
 #
 #       - Set below in this file ' version_str = "X.Xb" ' (beta version for next
 #         release) for the following tests.
 #
 #       - tests pass: https://travis-ci.org/github/phfaist/pylatexenc
@@ -51,8 +51,8 @@
 #   7) on github.com, fill in release details with a summary of changes etc.
 #
 #   8) create the source package for PyPI (" python3 setup.py sdist ")
 #   
 #   8) upload package to PyPI (twine upload dist/pylatexenc-X.X.tar.gz -r realpypi)
 #
 
-version_str = "3.0alpha000013"
+version_str = "3.0alpha000014"
```

### Comparing `pylatexenc-3.0a13/pyproject.toml` & `pylatexenc-3.0a14/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylatexenc"
-version = "3.0alpha000013" # ALSO BUMP IN pylatexenc/version.py
+version = "3.0alpha000014" # ALSO BUMP IN pylatexenc/version.py
 description = "Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion"
 authors = ["Philippe Faist <philippe.faist@bluewin.ch>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.scripts]
 latexwalker = 'pylatexenc.latexwalker.__main__:main'
```

### Comparing `pylatexenc-3.0a13/setup.py` & `pylatexenc-3.0a14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 entry_points = \
 {'console_scripts': ['latex2text = pylatexenc.latex2text.__main__:main',
                      'latexencode = pylatexenc.latexencode.__main__:main',
                      'latexwalker = pylatexenc.latexwalker.__main__:main']}
 
 setup_kwargs = {
     'name': 'pylatexenc',
-    'version': '3.0a13',
+    'version': '3.0a14',
     'description': 'Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion',
     'long_description': "pylatexenc\n==========\n\nSimple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion\n\n.. image:: https://img.shields.io/github/license/phfaist/pylatexenc.svg?style=flat\n   :target: https://github.com/phfaist/pylatexenc/blob/master/LICENSE.txt\n\n.. image:: https://img.shields.io/pypi/v/pylatexenc.svg?style=flat\n   :target: https://pypi.org/project/pylatexenc/\n\nPython: ≥ 3.4 or ≥ 2.7. The library is designed to be as backwards-compatible as\nreasonably possible and is able to run on old python verisons should it be\nnecessary. (Use the setup.py script directly if you have python<3.7, poetry\ndoesn't seem to work with old python versions.)\n\n\nUnicode Text to LaTeX code\n--------------------------\n\nThe ``pylatexenc.latexencode`` module provides a function ``unicode_to_latex()``\nwhich converts a unicode string into LaTeX text and escape sequences. It should\nrecognize accented characters and most math symbols. A couple of switches allow\nyou to alter how this function behaves.\n\nYou can also run ``latexencode`` in command-line to convert plain unicode text\n(from the standard input or from files given on the command line) into LaTeX\ncode, written on to the standard output.\n\nA third party plug-in for Vim\n`vim-latexencode <https://github.com/Konfekt/vim-latexencode>`_\nby `@Konfekt <https://github.com/Konfekt>`_\nprovides a corresponding command to operate on a given range.\n\n\nParsing LaTeX code & converting to plain text (unicode)\n-------------------------------------------------------\n\nThe ``pylatexenc.latexwalker`` module provides a series of routines that parse\nthe LaTeX structure of given LaTeX code and returns a logical structure of\nobjects, which can then be used to produce output in another format such as\nplain text.  This is not a replacement for a full (La)TeX engine, rather, this\nmodule provides a way to parse a chunk of LaTeX code as mark-up code.\n\nThe ``pylatexenc.latex2text`` module builds up on top of\n``pylatexenc.latexwalker`` and provides functions to convert given LaTeX code to\nplain text with unicode characters.\n\nYou can also run ``latex2text`` in command-line to convert LaTeX input (either\nfrom the standard input, or from files given on the command line) into plain\ntext written on the standard output.\n\n\nDocumentation\n-------------\n\nFull documentation is available at https://pylatexenc.readthedocs.io/.\n\nTo build the documentation manually, run::\n\n  > poetry install --with=builddoc\n  > cd doc/\n  doc> poetry run make html\n\n\nLicense\n-------\n\nSee LICENSE.txt (MIT License).\n\nNOTE: See copyright notice and license information for file\n``tools/unicode.xml`` provided in ``tools/unicode.xml.LICENSE``.  (The file\n``tools/unicode.xml`` was downloaded from\nhttps://www.w3.org/2003/entities/2007xml/unicode.xml as linked from\nhttps://www.w3.org/TR/xml-entity-names/#source.)\n",
     'author': 'Philippe Faist',
     'author_email': 'philippe.faist@bluewin.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pylatexenc-3.0a13/PKG-INFO` & `pylatexenc-3.0a14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pylatexenc
-Version: 3.0a13
+Version: 3.0a14
 Summary: Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
 License: MIT
 Author: Philippe Faist
 Author-email: philippe.faist@bluewin.ch
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 pylatexenc
 ==========
 
 Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
```

