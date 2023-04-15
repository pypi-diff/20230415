# Comparing `tmp/pritunl_api-1.1.7.tar.gz` & `tmp/pritunl_api-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pritunl_api-1.1.7.tar", max compression
+gzip compressed data, was "pritunl_api-1.1.8.tar", max compression
```

## Comparing `pritunl_api-1.1.7.tar` & `pritunl_api-1.1.8.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1097 2023-03-20 04:19:29.857393 pritunl_api-1.1.7/LICENSE
--rw-r--r--   0        0        0     5539 2023-04-14 19:31:59.444906 pritunl_api-1.1.7/README.md
--rw-r--r--   0        0        0    15607 2023-04-14 16:33:56.576948 pritunl_api-1.1.7/pritunl_api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 16:22:56.215232 pritunl_api-1.1.7/pritunl_api/utils/__init__.py
--rw-r--r--   0        0        0      413 2023-03-27 16:22:56.215533 pritunl_api-1.1.7/pritunl_api/utils/genkey.py
--rw-r--r--   0        0        0      603 2023-03-27 16:22:56.215737 pritunl_api-1.1.7/pritunl_api/utils/query.py
--rw-r--r--   0        0        0     1079 2023-04-14 17:13:49.659799 pritunl_api-1.1.7/pritunl_api_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 07:11:20.907060 pritunl_api-1.1.7/pritunl_api_cli/commands/__init__.py
--rw-r--r--   0        0        0     7268 2023-04-14 19:31:59.445306 pritunl_api-1.1.7/pritunl_api_cli/commands/users.py
--rw-r--r--   0        0        0     1953 2023-04-14 19:32:45.517421 pritunl_api-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     7483 1970-01-01 00:00:00.000000 pritunl_api-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-03-20 04:19:29.857393 pritunl_api-1.1.8/LICENSE
+-rw-r--r--   0        0        0     5591 2023-04-15 05:35:33.875349 pritunl_api-1.1.8/README.md
+-rw-r--r--   0        0        0    16025 2023-04-15 05:35:33.875712 pritunl_api-1.1.8/pritunl_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 16:22:56.215232 pritunl_api-1.1.8/pritunl_api/utils/__init__.py
+-rw-r--r--   0        0        0      413 2023-03-27 16:22:56.215533 pritunl_api-1.1.8/pritunl_api/utils/genkey.py
+-rw-r--r--   0        0        0      603 2023-03-27 16:22:56.215737 pritunl_api-1.1.8/pritunl_api/utils/query.py
+-rw-r--r--   0        0        0     1166 2023-04-15 05:35:33.876034 pritunl_api-1.1.8/pritunl_api_cli/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-15 05:35:33.876314 pritunl_api-1.1.8/pritunl_api_cli/commands/__init__.py
+-rw-r--r--   0        0        0      193 2023-04-15 05:35:33.876532 pritunl_api-1.1.8/pritunl_api_cli/commands/connection.py
+-rw-r--r--   0        0        0     7238 2023-04-15 05:35:33.876867 pritunl_api-1.1.8/pritunl_api_cli/commands/users.py
+-rw-r--r--   0        0        0     1953 2023-04-15 05:35:33.877177 pritunl_api-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 pritunl_api-1.1.8/PKG-INFO
```

### Comparing `pritunl_api-1.1.7/LICENSE` & `pritunl_api-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pritunl_api-1.1.7/README.md` & `pritunl_api-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,22 @@
 pritunl-api-cli --help
 ```
 
 ```txt
 Usage: pritunl-api-cli [OPTIONS] COMMAND [ARGS]...
 
 Options:
-  --help  Show this message and exit.
+  --version  Show the version and exit.
+  --help     Show this message and exit.
 
 Commands:
   create-user
   delete-user
   get-user
+  status
   update-user
 ```
 
 For available command options and syntax, use the feature command help option.
 
 ```bash
 pritunl-api-cli create-user --help
```

### Comparing `pritunl_api-1.1.7/pritunl_api/__init__.py` & `pritunl_api-1.1.8/pritunl_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     def __init__(self, msg):
         log.error(msg)
         pass
 
 
 class Pritunl:
     def __init__(self, url=None, token=None, secret=None):
-        self.BASE_URL = self.clean_url(os.environ.get('PRITUNL_BASE_URL') if not url else url)
-        self.API_TOKEN = os.environ.get('PRITUNL_API_TOKEN') if not token else token
-        self.API_SECRET = os.environ.get('PRITUNL_API_SECRET') if not secret else secret
+        self.BASE_URL = self.clean_url(os.environ['PRITUNL_BASE_URL'] if not url else url)
+        self.API_TOKEN = os.environ['PRITUNL_API_TOKEN'] if not token else token
+        self.API_SECRET = os.environ['PRITUNL_API_SECRET'] if not secret else secret
 
         # Sub classes
         self.server = self.ServerClass(self)
         self.organization = self.OrganizationClass(self)
         self.user = self.UserClass(self)
         self.key = self.KeyClass(self)
 
@@ -305,14 +305,24 @@
             if self.r.status_code == 200:
                 return True
             else:
                 raise PritunlErr("{0}:{1}".format(sys._getframe().f_code.co_name, self.root.BASE_URL))
         except Exception:
             raise PritunlErr("{0}:{1}".format(sys._getframe().f_code.co_name, self.root.BASE_URL))
 
+    def status(self):
+        try:
+            self.r = self.auth_request(method="GET", path="/status")
+            if self.r.status_code == 200:
+                return self.r.json()
+            else:
+                raise PritunlErr("{0}:{1}".format(sys._getframe().f_code.co_name, self.root.BASE_URL))
+        except Exception:
+            raise PritunlErr("{0}:{1}".format(sys._getframe().f_code.co_name, self.root.BASE_URL))
+
     def setting(self):
         try:
             self.r = self.auth_request(method="GET", path="/settings")
             if self.r.status_code == 200:
                 return self.r.json()
             else:
                 raise PritunlErr("{0}:{1}".format(sys._getframe().f_code.co_name, self.root.BASE_URL))
```

### Comparing `pritunl_api-1.1.7/pritunl_api/utils/query.py` & `pritunl_api-1.1.8/pritunl_api/utils/query.py`

 * *Files identical despite different names*

### Comparing `pritunl_api-1.1.7/pritunl_api_cli/__init__.py` & `pritunl_api-1.1.8/pritunl_api_cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import click
 
 # Pritunl
+from .commands import connection
 from .commands import users
 
 @click.group()
 @click.version_option(package_name='pritunl-api')
 @click.pass_context
 def run(ctx):
     pass
 
+@run.command()
+def status():
+    connection.status()
+
 # Get User
 @run.command()
 @click.option('--org-name')
 @click.option('--user-name')
 @click.option('--show-advanced-details', is_flag=True)
 def get_user(**kwargs):
     users.get_user(**kwargs)
```

### Comparing `pritunl_api-1.1.7/pritunl_api_cli/commands/users.py` & `pritunl_api-1.1.8/pritunl_api_cli/commands/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import csv
 import json
 from urllib.parse import urlparse
 
-from pritunl_api import Pritunl
-pritunl = Pritunl()
+from . import pritunl
 
 from pritunl_api.utils.query import org_user
 from pritunl_api.utils.genkey import profile_key
 
 import click
 
 from rich import print_json
```

### Comparing `pritunl_api-1.1.7/pyproject.toml` & `pritunl_api-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pritunl-api"
-version = "1.1.7"
+version = "1.1.8"
 description = "Pritunl API Client for Python"
 authors = ["Nathaniel Varona <nathaniel.varona+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pritunl_api-1.1.7/PKG-INFO` & `pritunl_api-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pritunl-api
-Version: 1.1.7
+Version: 1.1.8
 Summary: Pritunl API Client for Python
 License: MIT
 Author: Nathaniel Varona
 Author-email: nathaniel.varona+pypi@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -159,20 +159,22 @@
 pritunl-api-cli --help
 ```
 
 ```txt
 Usage: pritunl-api-cli [OPTIONS] COMMAND [ARGS]...
 
 Options:
-  --help  Show this message and exit.
+  --version  Show the version and exit.
+  --help     Show this message and exit.
 
 Commands:
   create-user
   delete-user
   get-user
+  status
   update-user
 ```
 
 For available command options and syntax, use the feature command help option.
 
 ```bash
 pritunl-api-cli create-user --help
```

