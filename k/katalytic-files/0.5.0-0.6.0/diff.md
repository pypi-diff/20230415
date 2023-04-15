# Comparing `tmp/katalytic-files-0.5.0.tar.gz` & `tmp/katalytic-files-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.5.0.tar", last modified: Sat Apr 15 06:25:26 2023, max compression
+gzip compressed data, was "katalytic-files-0.6.0.tar", last modified: Sat Apr 15 06:36:58 2023, max compression
```

## Comparing `katalytic-files-0.5.0.tar` & `katalytic-files-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       87 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/.gitignore
--rw-r--r--   0        0        0      841 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      542 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/.travis.yml
--rw-r--r--   0        0        0      915 2023-04-15 06:25:21.718625 katalytic-files-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2031 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/README.md
--rw-r--r--   0        0        0     1608 2023-04-15 06:25:21.258855 katalytic-files-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/pytest.sh
--rw-r--r--   0        0        0     3107 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/scripts/venv.sh
--rw-r--r--   0        0        0    12240 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/src/katalytic/files.py
--rw-r--r--   0        0        0    41944 2023-04-15 06:24:40.031477 katalytic-files-0.5.0/tests/test_files.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 katalytic-files-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      542 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/.travis.yml
+-rw-r--r--   0        0        0     1235 2023-04-15 06:36:54.312829 katalytic-files-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2031 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/README.md
+-rw-r--r--   0        0        0     1608 2023-04-15 06:36:53.869051 katalytic-files-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/pytest.sh
+-rw-r--r--   0        0        0     3107 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/scripts/venv.sh
+-rw-r--r--   0        0        0    12492 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/src/katalytic/files.py
+-rw-r--r--   0        0        0    42174 2023-04-15 06:36:16.103941 katalytic-files-0.6.0/tests/test_files.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 katalytic-files-0.6.0/PKG-INFO
```

### Comparing `katalytic-files-0.5.0/.gitignore` & `katalytic-files-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/.gitlab-ci.yml` & `katalytic-files-0.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/.travis.yml` & `katalytic-files-0.6.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/CHANGELOG.md` & `katalytic-files-0.6.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.6.0 (2023-04-15)
+### Feature
+* Add load_text() and save_text() ([`2283da7`](https://github.com/katalytic/katalytic-files/commit/2283da70eddcc90f3ff90f14f9c611ffb310adf6))
+* Add load_text() and save_text() ([`4eb85d6`](https://github.com/katalytic/katalytic-files/commit/4eb85d66245efad828f14b0ccd48858a473e9394))
+
+
 ## 0.5.0 (2023-04-15)
 ### Feature
 * **load_json:** Remove sort_keys parameter. I will add a function for that later, probably in katalytic-data ([`8e188c0`](https://github.com/katalytic/katalytic-files/commit/8e188c08fc22497090f8ca07d8aaa47aa1856dd4))
 
 
 ## 0.4.0 (2023-04-15)
 ### Feature
```

### Comparing `katalytic-files-0.5.0/LICENSE.txt` & `katalytic-files-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/README.md` & `katalytic-files-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/pyproject.toml` & `katalytic-files-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.5.0"
+version = "0.6.0"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-files-0.5.0/scripts/conda.sh` & `katalytic-files-0.6.0/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/scripts/find_requirements.py` & `katalytic-files-0.6.0/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/scripts/release.sh` & `katalytic-files-0.6.0/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/scripts/venv.sh` & `katalytic-files-0.6.0/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.5.0/src/katalytic/files.py` & `katalytic-files-0.6.0/src/katalytic/files.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 from pathlib import Path
 
 from katalytic.pkg import get_version
 
 __version__, __version_info__ = get_version(__name__)
 
 
+def load_text(path, *, encoding='utf-8', **kwargs):
+    with open(path, encoding=encoding) as f:
+        return f.read()
+
+
+def save_text(data, path, *, encoding='utf-8'):
+    with open(path, 'w', encoding=encoding) as f:
+        return f.write(data)
+
+
 def load_json(path, *, encoding='utf-8', **kwargs):
     with open(path, encoding=encoding) as f:
         return json.load(f, **kwargs)
 
 
 def save_json(data, path, *, encoding='utf-8', indent=4, **kwargs):
     if isinstance(indent, float) and indent.is_integer():
```

### Comparing `katalytic-files-0.5.0/tests/test_files.py` & `katalytic-files-0.6.0/tests/test_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import collections
 import shutil
 import tempfile
 from pathlib import Path
 
 import pytest
 
-from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, load_json, make_dir, move_dir, move_file, save_json
+from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, load_json, load_text, make_dir, move_dir, move_file, save_json, save_text
 
 
 class TestGroup_save_and_load:
     class Test_json:
         def test_indent_0(self):
             data = self.create_json_data()
             path = _setup_path()
@@ -65,14 +65,21 @@
             else:
                 return True
 
         def create_json_data(self):
             """The keys are not sorted on purpose."""
             return {'e': 0, 'a': 1, 'b': 2.0, 'c': 3.5, 'd': [{'y': None, 'f': True, 'g': {'x': 'i', 'j': [False]}}]}
 
+    class Test_text:
+        def test_basic(self):
+            data = 'some text\nwith newlines'
+            path = _setup_path()
+            save_text(data, path)
+            assert load_text(path) == data
+
 
 class TestGroup_copy:
     class Test_copy_dir:
         def test_dest_is_dir(self):
             src = Path(_setup_tree('{}_src'))
 
             dest = Path(get_unique_path('{}_dest'))
```

### Comparing `katalytic-files-0.5.0/PKG-INFO` & `katalytic-files-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.5.0
+Version: 0.6.0
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

