# Comparing `tmp/burny_common-0.0.8.tar.gz` & `tmp/burny_common-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burny_common-0.0.8.tar", max compression
+gzip compressed data, was "burny_common-0.0.9.tar", max compression
```

## Comparing `burny_common-0.0.8.tar` & `burny_common-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0        0 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/__init__.py
--rw-r--r--   0        0        0     1889 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/behavior_tree.py
--rw-r--r--   0        0        0     3224 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/copy_file_to_server.py
--rw-r--r--   0        0        0     4170 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/copy_folder_to_server.py
--rw-r--r--   0        0        0     9763 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/integration_test_helper.py
--rw-r--r--   0        0        0      398 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/measure_time.py
--rw-r--r--   0        0        0     4305 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/min_heap.py
--rw-r--r--   0        0        0      917 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/path_manipulation.py
--rw-r--r--   0        0        0     1606 2022-06-30 21:12:56.693471 burny_common-0.0.8/burny_common/run_command_on_server.py
--rw-r--r--   0        0        0      677 2022-06-30 21:12:56.697471 burny_common-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      761 2022-06-30 21:13:22.406195 burny_common-0.0.8/setup.py
--rw-r--r--   0        0        0      639 2022-06-30 21:13:22.406522 burny_common-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/__init__.py
+-rw-r--r--   0        0        0     1889 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/behavior_tree.py
+-rw-r--r--   0        0        0     3224 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/copy_file_to_server.py
+-rw-r--r--   0        0        0     4138 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/copy_folder_to_server.py
+-rw-r--r--   0        0        0      398 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/measure_time.py
+-rw-r--r--   0        0        0     4323 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/min_heap.py
+-rw-r--r--   0        0        0      880 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/path_manipulation.py
+-rw-r--r--   0        0        0     1606 2023-02-18 17:57:37.051948 burny_common-0.0.9/burny_common/run_command_on_server.py
+-rw-r--r--   0        0        0     1193 2023-02-18 17:57:37.051948 burny_common-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 burny_common-0.0.9/setup.py
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 burny_common-0.0.9/PKG-INFO
```

### Comparing `burny_common-0.0.8/burny_common/behavior_tree.py` & `burny_common-0.0.9/burny_common/behavior_tree.py`

 * *Files identical despite different names*

### Comparing `burny_common-0.0.8/burny_common/copy_file_to_server.py` & `burny_common-0.0.9/burny_common/copy_file_to_server.py`

 * *Files identical despite different names*

### Comparing `burny_common-0.0.8/burny_common/copy_folder_to_server.py` & `burny_common-0.0.9/burny_common/copy_folder_to_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,14 @@
         pkey_loaded = paramiko.RSAKey.from_private_key(StringIO(pkey))
         client.connect(hostname=host, port=port, username=username, password=password, pkey=pkey_loaded)
 
         path_source_root_folder = Path(sourcepath)
         path_target_root_folder = generate_path(client, targetpath)
 
         allowed_files: Optional[Set] = None
-        # pylint: disable=R1732
         if respectgitignore:
             proc = subprocess.Popen(
                 ['git', 'ls-files'],
                 cwd=path_source_root_folder.absolute(),
                 stdout=subprocess.PIPE,
             )
             output = proc.stdout
```

### Comparing `burny_common-0.0.8/burny_common/min_heap.py` & `burny_common-0.0.9/burny_common/min_heap.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,13 +118,14 @@
     1
     2 3
     4 5 6 7
     """
     for i in build_list:
         assert not p.is_empty(), 'Min heap should be not empty, but is returned to be empty'
         value = p.get_min()
-        assert (
-            value == i
-        ), f"get_min or delete_min function not working as expected, received value '{value}' but should have been '{i}', heap:\n{p}"
+        assert (value == i), (
+            f"get_min or delete_min function not working as expected, received value '{value}' "
+            f"but should have been '{i}', heap:\n{p}"
+        )
         p.delete_min()
 
     assert p.is_empty(), "Min heap should be empty, but isn't"
```

### Comparing `burny_common-0.0.8/burny_common/path_manipulation.py` & `burny_common-0.0.9/burny_common/path_manipulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,9 +23,8 @@
     If depth == 1: if given a folder, return containing file paths
     Depth > 1 allow recursively to go through folders up to a given depth
     """
     if path.is_file():
         yield path
     elif path.is_dir() and depth > 0:
         for subfile_path in sorted(path.iterdir()):
-            for new_file in recurse_path(subfile_path, depth=depth - 1):
-                yield new_file
+            yield from recurse_path(subfile_path, depth=depth - 1)
```

### Comparing `burny_common-0.0.8/burny_common/run_command_on_server.py` & `burny_common-0.0.9/burny_common/run_command_on_server.py`

 * *Files identical despite different names*

### Comparing `burny_common-0.0.8/setup.py` & `burny_common-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,23 +14,23 @@
  'portpicker>=1.5.2,<2.0.0',
  'psutil>=5.9.1,<6.0.0',
  'requests>=2.28.0,<3.0.0',
  'types-requests>=2.27.31,<3.0.0']
 
 setup_kwargs = {
     'name': 'burny-common',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'BurnySc2',
     'author_email': 'gamingburny@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `burny_common-0.0.8/PKG-INFO` & `burny_common-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: burny-common
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: BurnySc2
 Author-email: gamingburny@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: paramiko (>=2.11.0,<3.0.0)
 Requires-Dist: portpicker (>=1.5.2,<2.0.0)
 Requires-Dist: psutil (>=5.9.1,<6.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: types-requests (>=2.27.31,<3.0.0)
```

