# Comparing `tmp/sabledocs-0.0.2.dev33.tar.gz` & `tmp/sabledocs-0.0.2.dev39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.0.2.dev33.tar", last modified: Sat Apr 15 15:01:23 2023, max compression
+gzip compressed data, was "sabledocs-0.0.2.dev39.tar", last modified: Sat Apr 15 16:51:46 2023, max compression
```

## Comparing `sabledocs-0.0.2.dev33.tar` & `sabledocs-0.0.2.dev39.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3461 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2920 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.626925 sabledocs-0.0.2.dev33/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.626925 sabledocs-0.0.2.dev33/src/sabledocs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13639 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.626925 sabledocs-0.0.2.dev33/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1850 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 15:01:13.000000 sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 15:01:23.630925 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3461 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 15:01:23.000000 sabledocs-0.0.2.dev33/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:46.234999 sabledocs-0.0.2.dev39/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3491 2023-04-15 16:51:46.234999 sabledocs-0.0.2.dev39/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      778 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-04-15 16:51:46.234999 sabledocs-0.0.2.dev39/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:46.230999 sabledocs-0.0.2.dev39/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:46.230999 sabledocs-0.0.2.dev39/src/sabledocs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13639 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:46.230999 sabledocs-0.0.2.dev39/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:46.234999 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1850 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      826 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1399 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1889 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:46.234999 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   257737 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      560 2023-04-15 16:51:29.000000 sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-15 16:51:46.234999 sabledocs-0.0.2.dev39/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3491 2023-04-15 16:51:46.000000 sabledocs-0.0.2.dev39/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-04-15 16:51:46.000000 sabledocs-0.0.2.dev39/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-15 16:51:46.000000 sabledocs-0.0.2.dev39/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-04-15 16:51:46.000000 sabledocs-0.0.2.dev39/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-15 16:51:46.000000 sabledocs-0.0.2.dev39/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.0.2.dev33/LICENSE` & `sabledocs-0.0.2.dev39/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/PKG-INFO` & `sabledocs-0.0.2.dev39/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.2.dev33
+Version: 0.0.2.dev39
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -71,18 +71,19 @@
 # Copyright message displayed in the footer.
 # Default value: ""
 footer-content = "© 2023 Jane Doe. All rights reserved."
 
 # The following 3 fields configure the source control repository of the project.
 # It is used to generate deeplink for the components of the Proto model pointing to the original source code.
 # By default these fields are not configured, and source code links are not included in the docs.
-# The repository-type field supports two possible values, "github" and "bitbucket", and repository-url and `repository-branch` should be configured accordingly.
+# The repository-type field supports two possible values, "github" and "bitbucket".
+# The fields repository-url and `repository-branch` should be configured to point to the correct repository.
 repository-type = "github"
 repository-url = "https://github.com/janedoe/myawesomeproject"
-repository-branch = "master"
+repository-branch = "main"
 ```
 
 ## For maintainers
 
 Build the Python package:
 
 ```
```

### Comparing `sabledocs-0.0.2.dev33/README.md` & `sabledocs-0.0.2.dev39/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,18 +57,19 @@
 # Copyright message displayed in the footer.
 # Default value: ""
 footer-content = "© 2023 Jane Doe. All rights reserved."
 
 # The following 3 fields configure the source control repository of the project.
 # It is used to generate deeplink for the components of the Proto model pointing to the original source code.
 # By default these fields are not configured, and source code links are not included in the docs.
-# The repository-type field supports two possible values, "github" and "bitbucket", and repository-url and `repository-branch` should be configured accordingly.
+# The repository-type field supports two possible values, "github" and "bitbucket".
+# The fields repository-url and `repository-branch` should be configured to point to the correct repository.
 repository-type = "github"
 repository-url = "https://github.com/janedoe/myawesomeproject"
-repository-branch = "master"
+repository-branch = "main"
 ```
 
 ## For maintainers
 
 Build the Python package:
 
 ```
```

### Comparing `sabledocs-0.0.2.dev33/pyproject.toml` & `sabledocs-0.0.2.dev39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/__main__.py` & `sabledocs-0.0.2.dev39/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.0.2.dev39/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/proto_model.py` & `sabledocs-0.0.2.dev39/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/sable_config.py` & `sabledocs-0.0.2.dev39/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/base.html` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/index.html` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/message.html` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/package.html` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/service.html` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.0.2.dev39/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.0.2.dev39/src/sabledocs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.0.2.dev33
+Version: 0.0.2.dev39
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -71,18 +71,19 @@
 # Copyright message displayed in the footer.
 # Default value: ""
 footer-content = "© 2023 Jane Doe. All rights reserved."
 
 # The following 3 fields configure the source control repository of the project.
 # It is used to generate deeplink for the components of the Proto model pointing to the original source code.
 # By default these fields are not configured, and source code links are not included in the docs.
-# The repository-type field supports two possible values, "github" and "bitbucket", and repository-url and `repository-branch` should be configured accordingly.
+# The repository-type field supports two possible values, "github" and "bitbucket".
+# The fields repository-url and `repository-branch` should be configured to point to the correct repository.
 repository-type = "github"
 repository-url = "https://github.com/janedoe/myawesomeproject"
-repository-branch = "master"
+repository-branch = "main"
 ```
 
 ## For maintainers
 
 Build the Python package:
 
 ```
```

### Comparing `sabledocs-0.0.2.dev33/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.0.2.dev39/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

