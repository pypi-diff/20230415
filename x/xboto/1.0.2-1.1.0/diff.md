# Comparing `tmp/xboto-1.0.2.tar.gz` & `tmp/xboto-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xboto-1.0.2.tar", max compression
+gzip compressed data, was "xboto-1.1.0.tar", max compression
```

## Comparing `xboto-1.0.2.tar` & `xboto-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      907 2023-02-04 23:03:11.011861 xboto-1.0.2/LICENSE
--rw-r--r--   0        0        0     2552 2023-02-04 23:03:11.011861 xboto-1.0.2/README.md
--rw-r--r--   0        0        0     1929 2023-02-04 23:03:11.011861 xboto-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      175 2023-02-04 23:03:11.011861 xboto-1.0.2/xboto/__init__.py
--rw-r--r--   0        0        0     7913 2023-02-04 23:03:11.011861 xboto-1.0.2/xboto/client.py
--rw-r--r--   0        0        0    41378 2023-02-04 23:03:11.011861 xboto-1.0.2/xboto/dependencies.py
--rw-r--r--   0        0        0     1868 2023-02-04 23:03:11.011861 xboto-1.0.2/xboto/resource.py
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 xboto-1.0.2/setup.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 xboto-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 14:14:27.837397 xboto-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2552 2023-04-15 14:14:27.837397 xboto-1.1.0/README.md
+-rw-r--r--   0        0        0     1952 2023-04-15 14:14:27.841398 xboto-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/__init__.py
+-rw-r--r--   0        0        0     7913 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/client.py
+-rw-r--r--   0        0        0    41378 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/dependencies.py
+-rw-r--r--   0        0        0     1868 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/resource.py
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 xboto-1.1.0/PKG-INFO
```

### Comparing `xboto-1.0.2/README.md` & `xboto-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xboto-1.0.2/pyproject.toml` & `xboto-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 [tool.poetry]
 name = "xboto"
-version = "1.0.2"
+version = "1.1.0"
 description = "Easy lazy dependency injection for boto3 clients/resources."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xboto"}]
 readme = "README.md"
-license = "MIT"
 repository = "https://github.com/xyngular/py-xboto"
 keywords = ["boto", "boto client", "boto resource", "inject", "lazy", "dependency", "dependency injection", "aws"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-xinject = "^1.2.0"
+xinject = "^1.4.0"
 boto3 = "^1.26.64"
 botocore = "^1.29.64"
 xsentinels = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.9"
-pycodestyle = "^2.7.0"
 pdoc3 = "^0"
-pylint = "^2.9.6"
 pytest = "^7.1.3"
 pytest-mock = "^3.6.1"
 pytest-pycodestyle = "^2.3.0"
 black = { version = "*", allow-prereleases = true }
 moto = { version = "^4.0.3", extras = ["dynamodb2", "ssm"] }
 pyright = "^1.1.272"
 py = "^1.11.0"
 boto3-stubs = { extras = ["essential"], version = "^1.25.3" }
 mkdocstrings = { extras = ["python"], version = "^0" }
 mkdocs = "^1.4.1"
 mkdocs-material = "^8.5.7"
 mkdocs-autorefs = "^0"
 mike = "^1.1.2"
 mkdocs-git-revision-date-plugin = "^0.3.2"
+tomlkit = "^0.11.7"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.custom.xpublish]
```

### Comparing `xboto-1.0.2/xboto/client.py` & `xboto-1.1.0/xboto/client.py`

 * *Files identical despite different names*

### Comparing `xboto-1.0.2/xboto/dependencies.py` & `xboto-1.1.0/xboto/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,17 +476,17 @@
     Acm: Type[BotoClient]
     Acm_Pca: Type[BotoClient]
     AlexaForBusiness: Type[BotoClient]
     Amp: Type[BotoClient]
     Amplify: Type[BotoClient]
     AmplifyBackend: Type[BotoClient]
     AmplifyUiBuilder: Type[BotoClient]
-    ApiFateway: Type[BotoClient]
-    ApiFatewaymanagementapi: Type[BotoClient]
-    ApiFatewayv2: Type[BotoClient]
+    ApiGateway: Type[BotoClient]
+    ApiGatewayManagementApi: Type[BotoClient]
+    ApiGatewayV2: Type[BotoClient]
     AppConfig: Type[BotoClient]
     AppConfigData: Type[BotoClient]
     Appflow: Type[BotoClient]
     AppIntegrations: Type[BotoClient]
     Application_Autoscaling: Type[BotoClient]
     Application_Insights: Type[BotoClient]
     Applicationcostprofiler: Type[BotoClient]
```

### Comparing `xboto-1.0.2/xboto/resource.py` & `xboto-1.1.0/xboto/resource.py`

 * *Files identical despite different names*

### Comparing `xboto-1.0.2/setup.py` & `xboto-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: xboto
+Version: 1.1.0
+Summary: Easy lazy dependency injection for boto3 clients/resources.
+Home-page: https://github.com/xyngular/py-xboto
+Keywords: boto,boto client,boto resource,inject,lazy,dependency,dependency injection,aws
+Author: Josh Orr
+Author-email: josh@orr.blue
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: boto3 (>=1.26.64,<2.0.0)
+Requires-Dist: botocore (>=1.29.64,<2.0.0)
+Requires-Dist: xinject (>=1.4.0,<2.0.0)
+Requires-Dist: xsentinels (>=1.2.1,<2.0.0)
+Project-URL: Repository, https://github.com/xyngular/py-xboto
+Description-Content-Type: text/markdown
+
+![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)
+![PyPI version](https://badge.fury.io/py/xboto.svg?)
+
+## Documentation
+
+**[📄 Detailed Documentation](https://xyngular.github.io/py-xboto/latest/)** | **[🐍 PyPi](https://pypi.org/project/xboto/)**
+
+## Install
+
+```bash
+# via pip
+pip install xboto
+
+# via poetry
+poetry add xboto
+```
+
+## Quick Start
+
+### Import Boto Client/Resource
+
+```python
+
+# Use imported `dynamodb` just like dynamodb boto resource
+from xboto.resource import dynamodb
+
+# Use imported `ssm` just like ssm boto client
+from xboto.client import ssm
+
+# These are for overriding/injecting settings.
+from xboto import BotoResources, BotoClients, BotoSession
+
+# Can use them like normal:
+dynamodb.table(...)
+ssm.get_object(...)
+
+
+# Or you can override settings if you wish:
+with BotoResources.DynamoDB(region_name='us-west-2'):
+    # Use us-west-2 when using dynamodb boto resource:
+    dynamodb.table(...)
+
+with BotoClients.Ssm(region_name='us-west-2'):
+    # Use us-west-2 when using ssm boto client:
+    ssm.get_object(...)
+
+with BotoSession(region_name='us-west-3'):
+    # Use us-west-3 when using any client/resource
+    # we are setting it at the boto-session level;
+    # the session is used by all boto client/resources.
+    ssm.get_object(...)
+
+    
+# Can use them like decorators as well:
+@BotoClients.Ssm(region_name='us-west-2')
+def some_method():
+    ssm.get_object(...)
+
+```
+
+### Grab Any Client/Resource
+
+```python
+
+# Can easily ask these for any client/resource
+from xboto import boto_clients, boto_resources
+
+# These are for overriding/injecting settings.
+from xboto import BotoResources, BotoClients, BotoSession
+
+# Can use them like normal:
+boto_clients.dynamodb.table(...)
+boto_resources.ssm.get_object(...)
+
+
+# Or you can override settings if you wish:
+with BotoResources.DynamoDB(region_name='us-west-2'):
+    # Use us-west-2 when using dynamodb boto resource:
+    boto_resources.dynamodb.table(...)
+
+with BotoClients.Ssm(region_name='us-west-2'):
+    # Use us-west-2 when using ssm boto client:
+    boto_clients.ssm.get_object(...)
+
+with BotoSession(region_name='us-west-3'):
+    # Use us-west-3 when using any client/resource
+    # we are setting it at the boto-session level;
+    # the session is used by all boto client/resources.
+    boto_clients.ssm.get_object(...)
+
+    
+# Can use them like decorators as well:
+@BotoClients.Ssm(region_name='us-west-2')
+def some_method():
+    boto_clients.ssm.get_object(...)
 
-packages = \
-['xboto']
+```
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['boto3>=1.26.64,<2.0.0',
- 'botocore>=1.29.64,<2.0.0',
- 'xinject>=1.2.0,<2.0.0',
- 'xsentinels>=1.2.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'xboto',
-    'version': '1.0.2',
-    'description': 'Easy lazy dependency injection for boto3 clients/resources.',
-    'long_description': "![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)\n![PyPI version](https://badge.fury.io/py/xboto.svg?)\n\n## Documentation\n\n**[📄 Detailed Documentation](https://xyngular.github.io/py-xboto/latest/)** | **[🐍 PyPi](https://pypi.org/project/xboto/)**\n\n## Install\n\n```bash\n# via pip\npip install xboto\n\n# via poetry\npoetry add xboto\n```\n\n## Quick Start\n\n### Import Boto Client/Resource\n\n```python\n\n# Use imported `dynamodb` just like dynamodb boto resource\nfrom xboto.resource import dynamodb\n\n# Use imported `ssm` just like ssm boto client\nfrom xboto.client import ssm\n\n# These are for overriding/injecting settings.\nfrom xboto import BotoResources, BotoClients, BotoSession\n\n# Can use them like normal:\ndynamodb.table(...)\nssm.get_object(...)\n\n\n# Or you can override settings if you wish:\nwith BotoResources.DynamoDB(region_name='us-west-2'):\n    # Use us-west-2 when using dynamodb boto resource:\n    dynamodb.table(...)\n\nwith BotoClients.Ssm(region_name='us-west-2'):\n    # Use us-west-2 when using ssm boto client:\n    ssm.get_object(...)\n\nwith BotoSession(region_name='us-west-3'):\n    # Use us-west-3 when using any client/resource\n    # we are setting it at the boto-session level;\n    # the session is used by all boto client/resources.\n    ssm.get_object(...)\n\n    \n# Can use them like decorators as well:\n@BotoClients.Ssm(region_name='us-west-2')\ndef some_method():\n    ssm.get_object(...)\n\n```\n\n### Grab Any Client/Resource\n\n```python\n\n# Can easily ask these for any client/resource\nfrom xboto import boto_clients, boto_resources\n\n# These are for overriding/injecting settings.\nfrom xboto import BotoResources, BotoClients, BotoSession\n\n# Can use them like normal:\nboto_clients.dynamodb.table(...)\nboto_resources.ssm.get_object(...)\n\n\n# Or you can override settings if you wish:\nwith BotoResources.DynamoDB(region_name='us-west-2'):\n    # Use us-west-2 when using dynamodb boto resource:\n    boto_resources.dynamodb.table(...)\n\nwith BotoClients.Ssm(region_name='us-west-2'):\n    # Use us-west-2 when using ssm boto client:\n    boto_clients.ssm.get_object(...)\n\nwith BotoSession(region_name='us-west-3'):\n    # Use us-west-3 when using any client/resource\n    # we are setting it at the boto-session level;\n    # the session is used by all boto client/resources.\n    boto_clients.ssm.get_object(...)\n\n    \n# Can use them like decorators as well:\n@BotoClients.Ssm(region_name='us-west-2')\ndef some_method():\n    boto_clients.ssm.get_object(...)\n\n```\n",
-    'author': 'Josh Orr',
-    'author_email': 'josh@orr.blue',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/xyngular/py-xboto',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

