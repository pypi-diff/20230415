# Comparing `tmp/sabledocs-0.0.2.dev29.tar.gz` & `tmp/sabledocs-0.0.2.dev31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.0.2.dev29.tar", last modified: Sat Apr 15 13:02:27 2023, max compression
+gzip compressed data, was "sabledocs-0.0.2.dev31.tar", last modified: Sat Apr 15 13:20:27 2023, max compression
```

## Comparing `sabledocs-0.0.2.dev29.tar` & `sabledocs-0.0.2.dev31.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.885470 sabledocs-0.0.2.dev29/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:02:27.885470 sabledocs-0.0.2.dev29/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 13:02:27.885470 sabledocs-0.0.2.dev29/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2260 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13581 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2116 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 13:02:18.000000 sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:02:27.881471 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 13:02:27.000000 sabledocs-0.0.2.dev29/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.260520 sabledocs-0.0.2.dev31/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13581 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2235 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.260520 sabledocs-0.0.2.dev31/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.0.2.dev29/LICENSE` & `sabledocs-0.0.2.dev31/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/PKG-INFO` & `sabledocs-0.0.2.dev31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.2.dev29
+Version: 0.0.2.dev31
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.0.2.dev29/README.md` & `sabledocs-0.0.2.dev31/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/pyproject.toml` & `sabledocs-0.0.2.dev31/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/__main__.py` & `sabledocs-0.0.2.dev31/src/sabledocs/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import json
 import pprint
 import os
 from distutils.dir_util import copy_tree
 from re import template
 from sabledocs.proto_descriptor_parser import parse_proto_descriptor
 from sabledocs.sable_config import SableConfig
 from jinja2 import Environment, FileSystemLoader, select_autoescape
-from os import path
 
 
 def cli():
-    print(f"__file__ dirname: {path.dirname(__file__)}")
-    sable_config = SableConfig("sable.toml")
+    print("Starting documentation generation.")
+    sable_config = SableConfig("sabledocs.toml")
 
-    # sable_context = parse_proto_descriptor('descriptor.pb', sable_config)
-    # sable_context = parse_proto_descriptor('pubsub.pb', sable_config)
-    # sable_context = parse_proto_descriptor('sable-test.pb')
-    # sable_context = parse_proto_descriptor('datastore.pb', sable_config)
     sable_context = parse_proto_descriptor(sable_config)
 
-    template_base_dir = path.join(path.dirname(__file__), "templates", "_default") if sable_config.template == "_default" else f"templates/{sable_config.template}"
+    template_base_dir = os.path.join(os.path.dirname(__file__), "templates", "_default") if sable_config.template == "_default" else f"templates/{sable_config.template}"
 
     jinja_env = Environment(
         loader=FileSystemLoader(searchpath=template_base_dir),
         autoescape=select_autoescape()
     )
 
     package_template = jinja_env.get_template("package.html")
 
+    if not os.path.exists(sable_config.output_dir):
+        os.makedirs(sable_config.output_dir)
+
     for package in sable_context.packages:
-        with open(path.join(sable_config.output_dir, f'{package.name}.html'), 'wb') as fh:
+        with open(os.path.join(sable_config.output_dir, f'{package.name}.html'), 'wb') as fh:
             output = package_template.render(
                 sable_config=sable_config,
                 package=package,
                 packages=sable_context.packages,
                 all_messages=sable_context.all_messages,
                 all_enums=sable_context.all_enums).encode('utf-8') # Without encode('utf-8'), Unicode characters like © ended up garbled.
 
             fh.write(output)
 
-    with open(path.join(sable_config.output_dir, 'index.html'), 'wb') as fh:
+    with open(os.path.join(sable_config.output_dir, 'index.html'), 'wb') as fh:
         output = jinja_env.get_template("index.html").render(
             sable_config = sable_config,
             packages=sable_context.packages,
             all_messages=sable_context.all_messages,
             all_enums=sable_context.all_enums).encode('utf-8') # Without encode('utf-8'), Unicode characters like © ended up garbled.
 
         fh.write(output)
 
-    copy_tree(path.join(template_base_dir, "static"), path.join(sable_config.output_dir, "static"))
+    copy_tree(os.path.join(template_base_dir, "static"), os.path.join(sable_config.output_dir, "static"))
+
+    index_abs_path = os.path.abspath(os.path.join(sable_config.output_dir, "index.html"))
+    print(f"Building documentation done. It can be opened with {index_abs_path}")
 
 if __name__ == '__main__':  # pragma: no cover
     cli()
```

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.0.2.dev31/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/proto_model.py` & `sabledocs-0.0.2.dev31/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/sable_config.py` & `sabledocs-0.0.2.dev31/src/sabledocs/sable_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.repository_branch = ""
         self.repository_type = RepositoryType.GITHUB
         self.input_descriptor_file = "descriptor.pb"
         self.output_dir = "sabledocs_output"
         self.template = "_default"
 
         if path.exists(config_file_path):
-            print("Sable config found")
+            print(f"Configuration found in {config_file_path}")
             with open(config_file_path, mode='rb') as config_file:
                 print("TOML file parsed")
                 config_values = tomllib.load(config_file)
                 print(config_values)
                 if 'module-title' in config_values:
                     self.module_title = config_values['module-title']
 
@@ -49,7 +49,9 @@
                 if 'repository-type' in config_values:
                     print("repository-type found")
                     match config_values['repository-type']:
                         case 'github':
                             self.repository_type = RepositoryType.GITHUB
                         case 'bitbucket':
                             self.repository_type = RepositoryType.BITBUCKET
+        else:
+            print("sabledocs.toml file not found, using default configuration.")
```

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/base.html` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/index.html` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/message.html` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/package.html` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/service.html` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.0.2.dev31/src/sabledocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.2.dev29
+Version: 0.0.2.dev31
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.0.2.dev29/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.0.2.dev31/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

