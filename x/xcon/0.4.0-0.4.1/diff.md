# Comparing `tmp/xcon-0.4.0.tar.gz` & `tmp/xcon-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcon-0.4.0.tar", max compression
+gzip compressed data, was "xcon-0.4.1.tar", max compression
```

## Comparing `xcon-0.4.0.tar` & `xcon-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1211 2023-02-28 00:56:01.712690 xcon-0.4.0/LICENSE
--rw-r--r--   0        0        0     1311 2023-02-28 00:56:01.712690 xcon-0.4.0/Readme.md
--rw-r--r--   0        0        0     2442 2023-02-28 00:56:01.712690 xcon-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/__init__.py
--rw-r--r--   0        0        0     4379 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/conf.py
--rw-r--r--   0        0        0    68252 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/config.py
--rw-r--r--   0        0        0    27944 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/directory.py
--rw-r--r--   0        0        0       39 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/exceptions.py
--rw-r--r--   0        0        0       25 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/meta.json
--rw-r--r--   0        0        0    23815 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/provider.py
--rw-r--r--   0        0        0      201 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/providers/__init__.py
--rw-r--r--   0        0        0     4097 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/providers/common.py
--rw-r--r--   0        0        0    25159 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/providers/dynamo.py
--rw-r--r--   0        0        0     8233 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/providers/environmental.py
--rw-r--r--   0        0        0     9038 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/providers/secrets_manager.py
--rw-r--r--   0        0        0     3193 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/providers/ssm_param_store.py
--rw-r--r--   0        0        0     4202 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/__init__.py
--rw-r--r--   0        0        0     1755 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/cache-permissions.yml
--rw-r--r--   0        0        0     1785 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/config_manager/cache-table.yml
--rw-r--r--   0        0        0     3068 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/config_manager/change_handler.py
--rw-r--r--   0        0        0      746 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/config_manager/change_handler.yml
--rw-r--r--   0        0        0     1133 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/config_manager/config_cache_all_access.yml
--rw-r--r--   0        0        0     2134 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/secrets-permissions.yml
--rw-r--r--   0        0        0     1722 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/ssm-permissions.yml
--rw-r--r--   0        0        0      890 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/serverless_files/xcon-resources.js
--rw-r--r--   0        0        0      980 2023-02-28 00:56:01.716690 xcon-0.4.0/xcon/types.py
--rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 xcon-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 13:37:56.532281 xcon-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1306 2023-04-15 13:37:56.532281 xcon-0.4.1/Readme.md
+-rw-r--r--   0        0        0     2399 2023-04-15 13:37:56.536281 xcon-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1305 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/__init__.py
+-rw-r--r--   0        0        0     4379 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/conf.py
+-rw-r--r--   0        0        0    68252 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/config.py
+-rw-r--r--   0        0        0    27944 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/directory.py
+-rw-r--r--   0        0        0       39 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/exceptions.py
+-rw-r--r--   0        0        0       25 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/meta.json
+-rw-r--r--   0        0        0    23815 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/provider.py
+-rw-r--r--   0        0        0      201 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/providers/__init__.py
+-rw-r--r--   0        0        0     4097 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/providers/common.py
+-rw-r--r--   0        0        0    25159 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/providers/dynamo.py
+-rw-r--r--   0        0        0     8233 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/providers/environmental.py
+-rw-r--r--   0        0        0     9038 2023-04-15 13:37:56.536281 xcon-0.4.1/xcon/providers/secrets_manager.py
+-rw-r--r--   0        0        0     3193 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/providers/ssm_param_store.py
+-rw-r--r--   0        0        0     4202 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/__init__.py
+-rw-r--r--   0        0        0     1763 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/cache-permissions.yml
+-rw-r--r--   0        0        0     1785 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/config_manager/cache-table.yml
+-rw-r--r--   0        0        0     3068 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/config_manager/change_handler.py
+-rw-r--r--   0        0        0      746 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/config_manager/change_handler.yml
+-rw-r--r--   0        0        0     1133 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/config_manager/config_cache_all_access.yml
+-rw-r--r--   0        0        0     2134 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/secrets-permissions.yml
+-rw-r--r--   0        0        0     1722 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/ssm-permissions.yml
+-rw-r--r--   0        0        0      890 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/serverless_files/xcon-resources.js
+-rw-r--r--   0        0        0      980 2023-04-15 13:37:56.540281 xcon-0.4.1/xcon/types.py
+-rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 xcon-0.4.1/PKG-INFO
```

### Comparing `xcon-0.4.0/LICENSE` & `xcon-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/Readme.md` & `xcon-0.4.1/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Right now this is **pre-release software**, as the dynamo cache table and related need further documentation and testing.
 
 Retrieving values from Param Store and Secrets Manager should work and be relatively fast, as we bulk-grab values
 at the various directory-levels that are checked.
 
 **More documentation and testing will be coming soon, for a full 1.0.0 release sometime in the next month or so.**
 
-See **[xsettings docs](https://xyngular.github.io/py-xcon/latest/)**.
+See **[xcon docs](https://xyngular.github.io/py-xcon/latest/)**.
 
 # Documentation
 
 **[📄 Detailed Documentation](https://xyngular.github.io/py-xcon/latest/)** | **[🐍 PyPi](https://pypi.org/project/xcon/)**
 
 # Install
```

### Comparing `xcon-0.4.0/pyproject.toml` & `xcon-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "xcon"
-version = "0.4.0"
+version = "0.4.1"
 description = "Dynamic configuration retreiver."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xcon"}]
 readme = "Readme.md"
-license = "The Unlicense (Unlicense)"
-repository = "https://github.com/xyngular/py-xsettings"
+repository = "https://github.com/xyngular/py-xcon"
 keywords = ["settings", "configuration", "lazy", "boto", "aws", "secrets manager", "param store", "ssm"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
```

### Comparing `xcon-0.4.0/xcon/__init__.py` & `xcon-0.4.1/xcon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 """
 from .config import Config
 from . import providers
 from .config import config
 from .config import ConfigSettings
 from .conf import xcon_settings
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

### Comparing `xcon-0.4.0/xcon/conf.py` & `xcon-0.4.1/xcon/conf.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/config.py` & `xcon-0.4.1/xcon/config.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/directory.py` & `xcon-0.4.1/xcon/directory.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/provider.py` & `xcon-0.4.1/xcon/provider.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/providers/common.py` & `xcon-0.4.1/xcon/providers/common.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/providers/dynamo.py` & `xcon-0.4.1/xcon/providers/dynamo.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/providers/environmental.py` & `xcon-0.4.1/xcon/providers/environmental.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/providers/secrets_manager.py` & `xcon-0.4.1/xcon/providers/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/providers/ssm_param_store.py` & `xcon-0.4.1/xcon/providers/ssm_param_store.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/pytest_plugin.py` & `xcon-0.4.1/xcon/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/serverless_files/cache-permissions.yml` & `xcon-0.4.1/xcon/serverless_files/cache-permissions.yml`

 * *Files 7% similar despite different names*

```diff
@@ -36,10 +36,10 @@
                     - Ref: "AWS::Region"
                     - Ref: "AWS::AccountId"
                     - "table/global-all-configCache"
             Condition:
               ForAllValues:StringEquals:
                 dynamodb:LeadingKeys:
                   - "/${self:service}/${self:provider.stage}"
-                  - "/${self:service}"
+                  - "/${self:service}/all"
                   - "/global/${self:provider.stage}"
-                  - "/global"
+                  - "/global/all"
```

### Comparing `xcon-0.4.0/xcon/serverless_files/config_manager/cache-table.yml` & `xcon-0.4.1/xcon/serverless_files/config_manager/cache-table.yml`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/serverless_files/config_manager/change_handler.py` & `xcon-0.4.1/xcon/serverless_files/config_manager/change_handler.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/serverless_files/config_manager/change_handler.yml` & `xcon-0.4.1/xcon/serverless_files/config_manager/change_handler.yml`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/serverless_files/config_manager/config_cache_all_access.yml` & `xcon-0.4.1/xcon/serverless_files/config_manager/config_cache_all_access.yml`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/serverless_files/secrets-permissions.yml` & `xcon-0.4.1/xcon/serverless_files/secrets-permissions.yml`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/serverless_files/ssm-permissions.yml` & `xcon-0.4.1/xcon/serverless_files/ssm-permissions.yml`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/serverless_files/xcon-resources.js` & `xcon-0.4.1/xcon/serverless_files/xcon-resources.js`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/xcon/types.py` & `xcon-0.4.1/xcon/types.py`

 * *Files identical despite different names*

### Comparing `xcon-0.4.0/PKG-INFO` & `xcon-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: xcon
-Version: 0.4.0
+Version: 0.4.1
 Summary: Dynamic configuration retreiver.
-Home-page: https://github.com/xyngular/py-xsettings
-License: The Unlicense (Unlicense)
+Home-page: https://github.com/xyngular/py-xcon
 Keywords: settings,configuration,lazy,boto,aws,secrets manager,param store,ssm
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ciso8601 (>=2.3.0,<3.0.0)
 Requires-Dist: xbool (>=1.0.0,<2.0.0)
 Requires-Dist: xboto (>=1.0.2,<2.0.0)
 Requires-Dist: xinject (>=1.3.0,<2.0.0)
 Requires-Dist: xloop (>=1.0.1,<2.0.0)
 Requires-Dist: xsentinels (>=1.2.1,<2.0.0)
 Requires-Dist: xsettings (>=1.1.2,<2.0.0)
-Project-URL: Repository, https://github.com/xyngular/py-xsettings
+Project-URL: Repository, https://github.com/xyngular/py-xcon
 Description-Content-Type: text/markdown
 
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8|%203.9|%203.10|%203.11|%203.12&color=blue?style=flat-square&logo=python)
 ![PyPI version](https://badge.fury.io/py/xcon.svg?)
 
 - [Introduction](#introduction)
 - [Documentation](#documentation)
@@ -42,15 +40,15 @@
 Right now this is **pre-release software**, as the dynamo cache table and related need further documentation and testing.
 
 Retrieving values from Param Store and Secrets Manager should work and be relatively fast, as we bulk-grab values
 at the various directory-levels that are checked.
 
 **More documentation and testing will be coming soon, for a full 1.0.0 release sometime in the next month or so.**
 
-See **[xsettings docs](https://xyngular.github.io/py-xcon/latest/)**.
+See **[xcon docs](https://xyngular.github.io/py-xcon/latest/)**.
 
 # Documentation
 
 **[📄 Detailed Documentation](https://xyngular.github.io/py-xcon/latest/)** | **[🐍 PyPi](https://pypi.org/project/xcon/)**
 
 # Install
```

