# Comparing `tmp/LogicGateESO-0.1.0.tar.gz` & `tmp/LogicGateESO-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogicGateESO-0.1.0.tar", max compression
+gzip compressed data, was "LogicGateESO-0.1.1.tar", max compression
```

## Comparing `LogicGateESO-0.1.0.tar` & `LogicGateESO-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-04-15 10:26:11.945774 LogicGateESO-0.1.0/LICENSE
--rw-r--r--   0        0        0    10796 2023-04-15 10:26:48.361498 LogicGateESO-0.1.0/logicgateeso/LogicGate.py
--rw-r--r--   0        0        0       22 2023-04-15 10:25:20.557992 LogicGateESO-0.1.0/logicgateeso/__init__.py
--rw-r--r--   0        0        0      558 2023-04-15 10:28:15.805820 LogicGateESO-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      559 2023-04-15 10:28:42.314187 LogicGateESO-0.1.0/setup.py
--rw-r--r--   0        0        0      303 2023-04-15 10:28:42.314510 LogicGateESO-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 10:26:11.945774 LogicGateESO-0.1.1/LICENSE
+-rw-r--r--   0        0        0    10796 2023-04-15 10:26:48.361498 LogicGateESO-0.1.1/logicgateeso/LogicGate.py
+-rw-r--r--   0        0        0       22 2023-04-15 11:09:31.715399 LogicGateESO-0.1.1/logicgateeso/__init__.py
+-rw-r--r--   0        0        0      558 2023-04-15 11:09:18.491412 LogicGateESO-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      559 2023-04-15 11:09:46.042444 LogicGateESO-0.1.1/setup.py
+-rw-r--r--   0        0        0      303 2023-04-15 11:09:46.042860 LogicGateESO-0.1.1/PKG-INFO
```

### Comparing `LogicGateESO-0.1.0/LICENSE` & `LogicGateESO-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LogicGateESO-0.1.0/logicgateeso/LogicGate.py` & `LogicGateESO-0.1.1/logicgateeso/LogicGate.py`

 * *Files identical despite different names*

### Comparing `LogicGateESO-0.1.0/pyproject.toml` & `LogicGateESO-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LogicGateESO"
-version = "0.1.0"
+version = "0.1.1"
 description = "an esolang designed for manual encryption with logic gates"
 authors = ["Taokyle <taokyle415@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `LogicGateESO-0.1.0/setup.py` & `LogicGateESO-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['logicgateeso']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'logicgateeso',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'an esolang designed for manual encryption with logic gates',
     'long_description': None,
     'author': 'Taokyle',
     'author_email': 'taokyle415@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

