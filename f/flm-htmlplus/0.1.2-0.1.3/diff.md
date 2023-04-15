# Comparing `tmp/flm_htmlplus-0.1.2.tar.gz` & `tmp/flm_htmlplus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flm_htmlplus-0.1.2.tar", max compression
+gzip compressed data, was "flm_htmlplus-0.1.3.tar", max compression
```

## Comparing `flm_htmlplus-0.1.2.tar` & `flm_htmlplus-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      487 2023-04-14 20:55:00.059424 flm_htmlplus-0.1.2/README.md
--rw-r--r--   0        0        0      465 2023-04-14 20:52:23.428195 flm_htmlplus-0.1.2/flm_htmlplus/__init__.py
--rw-r--r--   0        0        0     6772 2023-04-14 20:52:23.418002 flm_htmlplus-0.1.2/flm_htmlplus/_fragmentrenderer.py
--rw-r--r--   0        0        0     4191 2023-04-11 15:24:31.553716 flm_htmlplus-0.1.2/flm_htmlplus/_selenium_driver.py
--rw-r--r--   0        0        0     6186 2023-04-14 20:52:23.396263 flm_htmlplus-0.1.2/flm_htmlplus/_workflow.py
--rw-r--r--   0        0        0  1815429 2023-04-01 11:21:45.601280 flm_htmlplus-0.1.2/flm_htmlplus/runmathjax_browser_dist.js
--rw-r--r--   0        0        0  1816360 2023-04-01 10:32:48.067688 flm_htmlplus-0.1.2/flm_htmlplus/runmathjax_script_dist.js
--rw-r--r--   0        0        0      555 2023-04-15 13:53:33.416286 flm_htmlplus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 flm_htmlplus-0.1.2/setup.py
--rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 flm_htmlplus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      487 2023-04-14 20:55:00.059424 flm_htmlplus-0.1.3/README.md
+-rw-r--r--   0        0        0      465 2023-04-14 20:52:23.428195 flm_htmlplus-0.1.3/flm_htmlplus/__init__.py
+-rw-r--r--   0        0        0     6772 2023-04-14 20:52:23.418002 flm_htmlplus-0.1.3/flm_htmlplus/_fragmentrenderer.py
+-rw-r--r--   0        0        0     4191 2023-04-11 15:24:31.553716 flm_htmlplus-0.1.3/flm_htmlplus/_selenium_driver.py
+-rw-r--r--   0        0        0     6186 2023-04-14 20:52:23.396263 flm_htmlplus-0.1.3/flm_htmlplus/_workflow.py
+-rw-r--r--   0        0        0  1815429 2023-04-01 11:21:45.601280 flm_htmlplus-0.1.3/flm_htmlplus/runmathjax_browser_dist.js
+-rw-r--r--   0        0        0  1816360 2023-04-01 10:32:48.067688 flm_htmlplus-0.1.3/flm_htmlplus/runmathjax_script_dist.js
+-rw-r--r--   0        0        0      555 2023-04-15 13:54:48.561041 flm_htmlplus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 flm_htmlplus-0.1.3/setup.py
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 flm_htmlplus-0.1.3/PKG-INFO
```

### Comparing `flm_htmlplus-0.1.2/flm_htmlplus/_fragmentrenderer.py` & `flm_htmlplus-0.1.3/flm_htmlplus/_fragmentrenderer.py`

 * *Files identical despite different names*

### Comparing `flm_htmlplus-0.1.2/flm_htmlplus/_selenium_driver.py` & `flm_htmlplus-0.1.3/flm_htmlplus/_selenium_driver.py`

 * *Files identical despite different names*

### Comparing `flm_htmlplus-0.1.2/flm_htmlplus/_workflow.py` & `flm_htmlplus-0.1.3/flm_htmlplus/_workflow.py`

 * *Files identical despite different names*

### Comparing `flm_htmlplus-0.1.2/flm_htmlplus/runmathjax_browser_dist.js` & `flm_htmlplus-0.1.3/flm_htmlplus/runmathjax_browser_dist.js`

 * *Files identical despite different names*

### Comparing `flm_htmlplus-0.1.2/flm_htmlplus/runmathjax_script_dist.js` & `flm_htmlplus-0.1.3/flm_htmlplus/runmathjax_script_dist.js`

 * *Files identical despite different names*

### Comparing `flm_htmlplus-0.1.2/pyproject.toml` & `flm_htmlplus-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flm-htmlplus"
-version = "0.1.2"
+version = "0.1.3"
 description = "Enhancements to LLM's HTML output (syntax highlighting, math equations, option for PDF output, etc.)"
 authors = ["Philippe Faist"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "flm_htmlplus"}]
 include = ["flm_htmlplus/runmathjax_browser_dist.js"]
```

### Comparing `flm_htmlplus-0.1.2/setup.py` & `flm_htmlplus-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['flm-core>=0.3.0a10',
  'pygments>=2.14.0,<3.0.0',
  'selenium>=4.7.2,<5.0.0',
  'webdriver-manager>=3.8.5,<4.0.0']
 
 setup_kwargs = {
     'name': 'flm-htmlplus',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': "Enhancements to LLM's HTML output (syntax highlighting, math equations, option for PDF output, etc.)",
     'long_description': "# Enhancements to LLM's HTML output, plus PDF via HTML\n\nInstallation:\n```\n> pip install git+https://github.com/phfaist/flm-htmlplus\n```\n\nThis LLM extension package provides the `flm_htmlplus` workflow\n(`--workflow=flm_htmlplus`) which adds some processing levels\nto LLM's default HTML output.  Mathematical equations can be\ncompiled into SVG elements.  You can also generate PDF output\n(internally, this uses an instance of Chrome to print the\ngenerated HTML content to a PDF document).\n",
     'author': 'Philippe Faist',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `flm_htmlplus-0.1.2/PKG-INFO` & `flm_htmlplus-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flm-htmlplus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Enhancements to LLM's HTML output (syntax highlighting, math equations, option for PDF output, etc.)
 License: MIT
 Author: Philippe Faist
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

