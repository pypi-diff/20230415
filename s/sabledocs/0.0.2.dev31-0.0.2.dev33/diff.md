# Comparing `tmp/sabledocs-0.0.2.dev31.tar.gz` & `tmp/sabledocs-0.0.2.dev33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.0.2.dev31.tar", last modified: Sat Apr 15 13:20:27 2023, max compression
+gzip compressed data, was "sabledocs-0.0.2.dev33.tar", last modified: Sat Apr 15 15:01:23 2023, max compression
```

## Comparing `sabledocs-0.0.2.dev31.tar` & `sabledocs-0.0.2.dev33.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.260520 sabledocs-0.0.2.dev31/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13581 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2235 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.260520 sabledocs-0.0.2.dev31/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 13:20:16.000000 sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 13:20:27.264520 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 13:20:27.000000 sabledocs-0.0.2.dev31/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3461 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2920 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.626925 sabledocs-0.0.2.dev33/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.626925 sabledocs-0.0.2.dev33/src/sabledocs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13639 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.626925 sabledocs-0.0.2.dev33/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1850 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3461 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.0.2.dev31/LICENSE` & `sabledocs-0.0.2.dev33/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/PKG-INFO` & `sabledocs-0.0.2.dev33/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sabledocs
-Version: 0.0.2.dev31
-Summary: Static documentation generator for Protobuf and gRPC
-Author-email: Mark Vincze <mrk.vincze@gmail.com>
-Project-URL: Homepage, https://github.com/markvincze/sabledocs
-Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
 
 A simple static documentation generator for Protobuf and gRPC contracts.
 
 ## How to use
@@ -46,14 +32,45 @@
 
 ```
 sabledocs
 ```
 
 The documentation will be generated into a folder `sabledocs_output`, its main page can be opened with `index.html`.
 
+### Customization
+
+For further customization, create a `sabledocs.toml` file in the folder where the Protobuf descriptor file is located and from which the `sabledocs` CLI is executed.
+You can customize the following options. Any omitted field will use its default value.
+
+```
+# Configures the main title of the documentation site.
+# Default value: "Protobuf module documentation"
+module-title = "My Awesome Module"
+
+# Specifies the name of the Protobuf descriptor file.
+# Default value: "descriptor.pb"
+input-descriptor-file = "myawesomemodule.pb"
+
+# The output folder to which the documentation is generated.
+# Default value: "sabledocs_output"
+output-dir = "docs"
+
+# Copyright message displayed in the footer.
+# Default value: ""
+footer-content = "© 2023 Jane Doe. All rights reserved."
+
+# The following 3 fields configure the source control repository of the project.
+# It is used to generate deeplink for the components of the Proto model pointing to the original source code.
+# By default these fields are not configured, and source code links are not included in the docs.
+# The repository-type field supports two possible values, "github" and "bitbucket", and repository-url and `repository-branch` should be configured accordingly.
+repository-type = "github"
+repository-url = "https://github.com/janedoe/myawesomeproject"
+repository-branch = "master"
+```
+
 ## For maintainers
 
 Build the Python package:
 
 ```
 python -m build
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sabledocs-0.0.2.dev31/pyproject.toml` & `sabledocs-0.0.2.dev33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/__main__.py` & `sabledocs-0.0.2.dev33/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.0.2.dev33/src/sabledocs/proto_descriptor_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 FIELD_TYPE_MESSAGE = 11
 FIELD_TYPE_ENUM = 14
 
 
 def build_source_code_url(repository_url, repository_type, repository_branch, file_path, line_number):
     match repository_type:
+        case RepositoryType.NONE:
+            return None
         case RepositoryType.GITHUB:
             return f"{repository_url.strip('/')}/blob/{repository_branch}/{file_path}#L{line_number}"
         case RepositoryType.BITBUCKET:
             return f"{repository_url.strip('/')}/src/{repository_branch}/{file_path}#lines-{line_number}"
     return ""
```

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/proto_model.py` & `sabledocs-0.0.2.dev33/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/sable_config.py` & `sabledocs-0.0.2.dev33/src/sabledocs/sable_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from enum import Enum
 from os import path
 import tomllib
 
 
 class RepositoryType(Enum):
-    GITHUB = 1
-    BITBUCKET = 2
+    NONE = 1
+    GITHUB = 2
+    BITBUCKET = 3
 
 
 class SableConfig:
     def __init__(self, config_file_path):
-        self.module_title = "Module"
+        self.module_title = "Protobuf module documentation"
         self.footer_content = ""
         self.repository_url = ""
         self.repository_branch = ""
-        self.repository_type = RepositoryType.GITHUB
+        self.repository_type = RepositoryType.NONE
         self.input_descriptor_file = "descriptor.pb"
         self.output_dir = "sabledocs_output"
         self.template = "_default"
 
         if path.exists(config_file_path):
             print(f"Configuration found in {config_file_path}")
             with open(config_file_path, mode='rb') as config_file:
```

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/base.html` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
-    <title>gRPC documentation</title>
+    <title>{{ sable_config.module_title }}</title>
     <link rel="stylesheet" href="static/mystyles.css" />
     <script
       src="https://kit.fontawesome.com/4d30d3d1aa.js"
       crossorigin="anonymous"
     ></script>
   </head>
   <body>
@@ -42,12 +42,12 @@
     <div class="container mb-6">{% block content %}{% endblock %}</div>
 
     <footer class="footer">
       <div class="content has-text-centered">
         {% if sable_config.footer_content %}
           <p>{{ sable_config.footer_content | safe }}</p>
         {% endif %}
-        <p>Built with <strong>Sable</strong>.</p>
+        <p>Built with <strong><a href="https://github.com/markvincze/sabledocs">sabledocs</a></strong>.</p>
       </div>
     </footer>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,8 +3,8 @@
 {%_if_sable_config.repository_type_|_string_==_"RepositoryType.GITHUB"_%}____{%
 elif_sable_config.repository_type_|_string_==_"RepositoryType.BITBUCKET"_%}
 {%_endif_%}_Source
 {% block content %}{% endblock %}
 {% if sable_config.footer_content %}
 {{ sable_config.footer_content | safe }}
 {% endif %}
-Built with Sable.
+Built with sabledocs.
```

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/index.html` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/message.html` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/package.html` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/service.html` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev31/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.0.2.dev33/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

