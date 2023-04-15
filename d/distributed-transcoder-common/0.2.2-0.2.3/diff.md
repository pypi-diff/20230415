# Comparing `tmp/distributed-transcoder-common-0.2.2.tar.gz` & `tmp/distributed-transcoder-common-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributed-transcoder-common-0.2.2.tar", max compression
+gzip compressed data, was "distributed-transcoder-common-0.2.3.tar", max compression
```

## Comparing `distributed-transcoder-common-0.2.2.tar` & `distributed-transcoder-common-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.2/distributed_transcoder_common/__init__.py
--rw-r--r--   0        0        0      416 2023-04-04 05:06:21.155583 distributed-transcoder-common-0.2.2/distributed_transcoder_common/message_types.py
--rw-r--r--   0        0        0      365 2023-04-04 05:32:11.572320 distributed-transcoder-common-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      598 2023-04-04 05:32:18.624042 distributed-transcoder-common-0.2.2/setup.py
--rw-r--r--   0        0        0      375 2023-04-04 05:32:18.624272 distributed-transcoder-common-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.3/distributed_transcoder_common/__init__.py
+-rw-r--r--   0        0        0      416 2023-04-04 05:06:21.155583 distributed-transcoder-common-0.2.3/distributed_transcoder_common/message_types.py
+-rw-r--r--   0        0        0     1742 2023-04-15 06:23:13.897558 distributed-transcoder-common-0.2.3/distributed_transcoder_common/models.py
+-rw-r--r--   0        0        0      390 2023-04-15 06:23:45.593207 distributed-transcoder-common-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-04-15 06:23:48.866363 distributed-transcoder-common-0.2.3/setup.py
+-rw-r--r--   0        0        0      422 2023-04-15 06:23:48.866566 distributed-transcoder-common-0.2.3/PKG-INFO
```

### Comparing `distributed-transcoder-common-0.2.2/setup.py` & `distributed-transcoder-common-0.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 packages = \
 ['distributed_transcoder_common']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['tortoise-orm>=0.19.3,<0.20.0']
+
 setup_kwargs = {
     'name': 'distributed-transcoder-common',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'A common library for for the distributed transcoder project',
     'long_description': None,
     'author': 'Eric Volpert',
     'author_email': 'ericvolp12@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

