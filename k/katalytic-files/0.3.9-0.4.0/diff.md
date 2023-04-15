# Comparing `tmp/katalytic-files-0.3.9.tar.gz` & `tmp/katalytic-files-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.3.9.tar", last modified: Wed Apr 12 18:10:32 2023, max compression
+gzip compressed data, was "katalytic-files-0.4.0.tar", last modified: Sat Apr 15 05:56:43 2023, max compression
```

## Comparing `katalytic-files-0.3.9.tar` & `katalytic-files-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       87 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.gitignore
--rw-r--r--   0        0        0      841 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.gitlab-ci.yml
--rw-r--r--   0        0        0      399 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.travis.yml
--rw-r--r--   0        0        0      349 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/LICENSE.txt
--rw-r--r--   0        0        0     1905 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/README.md
--rw-r--r--   0        0        0     1609 2023-04-12 18:10:26.961470 katalytic-files-0.3.9/pyproject.toml
--rw-r--r--   0        0        0       14 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/requirements.txt
--rw-r--r--   0        0        0      234 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/cleanup.sh
--rw-r--r--   0        0        0     1270 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/pytest.sh
--rw-r--r--   0        0        0     2209 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/release.sh
--rw-r--r--   0        0        0      403 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/setup.sh
--rw-r--r--   0        0        0      233 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/should_skip.sh
--rw-r--r--   0        0        0     1707 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/venv.sh
--rw-r--r--   0        0        0    11060 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/src/katalytic/files.py
--rw-r--r--   0        0        0    39566 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/tests/test_files.py
--rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      542 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/.travis.yml
+-rw-r--r--   0        0        0      661 2023-04-15 05:56:39.002481 katalytic-files-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2031 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/README.md
+-rw-r--r--   0        0        0     1608 2023-04-15 05:56:38.562701 katalytic-files-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/pytest.sh
+-rw-r--r--   0        0        0     3107 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/scripts/venv.sh
+-rw-r--r--   0        0        0    12335 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/src/katalytic/files.py
+-rw-r--r--   0        0        0    42489 2023-04-15 05:56:00.653663 katalytic-files-0.4.0/tests/test_files.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 katalytic-files-0.4.0/PKG-INFO
```

### Comparing `katalytic-files-0.3.9/.gitignore` & `katalytic-files-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.9/.gitlab-ci.yml` & `katalytic-files-0.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.9/LICENSE.txt` & `katalytic-files-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.9/README.md` & `katalytic-files-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-files)](https://pypi.org/project/katalytic-files/)
 [![Build Status](https://app.travis-ci.com/katalytic/katalytic-files.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
 [![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-files?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
 [![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-files/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-files?branch=main)
+[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-files.svg)](https://katalytic-files.readthedocs.io/en/latest/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-files
 ```
```

### Comparing `katalytic-files-0.3.9/pyproject.toml` & `katalytic-files-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.3.9"
-
+version = "0.4.0"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-files-0.3.9/scripts/conda.sh` & `katalytic-files-0.4.0/scripts/conda.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if [[ -z $1 ]]; then
 	echo 'You must provide a conda env to use'
 else
-	_CONDA_PY=/home/wip/anaconda3/envs/$1/bin/python
+	_CONDA_PY=~/anaconda3/envs/$1/bin/python
 
 	$_CONDA_PY -m pip uninstall -y katalytic-pkg
 	$_CONDA_PY -m pip install --no-cache-dir /media/data/projects/active/kata/katalytic-pkg/dist/katalytic*-py3-none-any.whl
 	_v1=$($_CONDA_PY -c 'from katalytic.pkg import __version__; print(f"wheel = {__version__}")')
 
 	echo '---'
 	$_CONDA_PY -m pip uninstall -y katalytic-pkg
```

### Comparing `katalytic-files-0.3.9/scripts/find_requirements.py` & `katalytic-files-0.4.0/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.9/scripts/release.sh` & `katalytic-files-0.4.0/scripts/release.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,76 @@
-assert(){
-	if [[ "$1" != "$2" ]]; then
-		echo "Expected '$2'"
-		echo "Got '$1'"
-		if [[ "$3" ]]; then
-			echo "${@:3}"
-		fi
-		exit 1
+prepend(){
+	file="$1"
+	text="$2"
+	echo "$text"
+	echo "$2" | command cat - "$1" > "$1.tmp" && command mv "$1.tmp" "$1"
+}
+
+update_changelog(){
+	new_version="$1"
+	if [[ ! -f "CHANGELOG.md" ]]; then
+		touch CHANGELOG.md
 	fi
+
+	prepend CHANGELOG.md ""
+	prepend CHANGELOG.md ""
+	prepend CHANGELOG.md "$(semantic-release changelog)" > /dev/null
+	prepend CHANGELOG.md "## $new_version ($(date +%Y-%m-%d))" > /dev/null
 }
 
 create_env(){
 	if [[ $VIRTUAL_ENV ]]; then
 		deactivate
 	fi
 
 	command rm -rf **/*.egg-info
 	command rm -rf **/__pycache__
 	command rm -rf **/.pytest_cache
 	command rm -rf **/venv
 
-	python -m venv venv
-	source venv/bin/activate
-	python -m pip install --quiet --quiet twine flit packaging
-	python -m pip install --quiet --quiet python-semantic-release==7.29.0
+	pip install --upgrade pip
+	pip install twine flit packaging
+	pip install python-semantic-release==7.29.0
 }
 
 check_build(){
 	pkg="$1"
+
+	if [[ "$pkg" == "katalytic" ]]; then
+		# There's no way of importing the version of the "collection" as katalytic.__version__
+		# because this is a namespace package, which prevents me from using an __init__.py file
+		pkg="$pkg.$pkg"
+	fi
+
 	twine check dist/*
 	if [ $? -eq 0 ]; then
 		echo "[twine] ok"
 	else
-		echo "[twine] Check failed. Exiting."
+		echo "[twine] Check failed. Exiting ..."
+		sleep 2
 		exit 1
 	fi
 
-	python -m pip install --quiet --quiet dist/katalytic-files*.tar.gz
+	pip install dist/*.tar.gz
 	python -c "from $pkg import __version__; print(__version__)"
 	if [ $? -eq 0 ]; then
 		echo "[sdist] ok"
 	else
-		echo "[sdist] Import failed. Exiting."
+		echo "[sdist] Import failed. Exiting ..."
+		sleep 2
 		exit 1
 	fi
 
-	python -m pip install --quiet --quiet dist/katalytic_files-*-py3-none-any.whl
+	pip install --force-reinstall dist/*-py3-none-any.whl
 	python -c "from $pkg import __version__; print(__version__)"
 	if [ $? -eq 0 ]; then
 		echo "[wheel] ok"
 	else
-		echo "[wheel] Import failed. Exiting."
+		echo "[wheel] Import failed. Exiting ..."
+		sleep 2
 		exit 1
 	fi
 }
 
 
 create_pypirc(){
 	message=$(echo "
@@ -79,26 +96,45 @@
 	echo ""
 
 	rm -rf **/dist
 	rm -rf **/build
 	create_pypirc
 	create_env
 
-	# bump -> build -> check
-	semantic-release version
-	if [ $? -ne 0 ]; then
-		# this executes when none of the commits are prefixed with "fix" or "feat"
-		# or when something really bad happened
-		echo "No version bump. Exiting."
+	# git config and pull
+	export GIT_MERGE_AUTOEDIT=no
+	git config credential.helper "!f() { printf '%s\n' 'username=vali19th' 'password=$GITLAB_TOKEN'; };f"
+	git config pull.rebase false
+	git pull --no-edit
+
+	# bump version and update changelog
+	new_version="$(semantic-release print-version)"
+	if [[ "$new_version" != "" ]]; then
+		semantic-release version
+		update_changelog "$new_version"
+		command cat CHANGELOG.md
+	else
+		echo "No version bump. Exiting ..."
+		sleep 2
 		exit 0
 	fi
 
-	flit build
+	# without this, flit won't build the sdist
+	git update-index --assume-unchanged pyproject.toml
+	git update-index --assume-unchanged CHANGELOG.md
+
+	flit build --format sdist --setup-py
+	flit build --format wheel --setup-py
 	check_build "$pkg"
 
-	# release -> push
+	# release
 	flit publish --repository pypi
-	git config credential.helper '!f() { printf "%s\n" "username=vali19th" "password=$GITLAB_TOKEN"; };f'
-	git push --tags https://gitlab.com/katalytic/katalytic-files.git HEAD:refs/heads/main
+
+	# push
+	git update-index --no-assume-unchanged pyproject.toml
+	git update-index --no-assume-unchanged CHANGELOG.md
+	git add CHANGELOG.md && git commit -m "doc: update CHANGELOG.md"
+	git push --tags
+	git push origin HEAD:main
 }
 
 main
```

### Comparing `katalytic-files-0.3.9/scripts/venv.sh` & `katalytic-files-0.4.0/scripts/venv.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if [[ -z $1 ]]; then
 	echo 'You must provide a conda env to use as base for the venv'
 else
-	_CONDA_PY=/home/wip/anaconda3/envs/$1/bin/python
+	_CONDA_PY=~/anaconda3/envs/$1/bin/python
 
 	command rm -rf venv venv
 	$_CONDA_PY -m venv venv
 	venv/bin/python -m pip install --upgrade pip
 	venv/bin/python -m pip install --no-cache-dir /media/data/projects/active/katalytic/katalytic-pkg/dist/katalytic*-py3-none-any.whl
 	_v1=$(venv/bin/python -c 'from katalytic.pkg import __version__; print(f"wheel = {__version__}")')
```

### Comparing `katalytic-files-0.3.9/src/katalytic/files.py` & `katalytic-files-0.4.0/src/katalytic/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,44 @@
+import collections
+import copy
 import itertools
+import json
 import re
 import shutil
 import tempfile
+
 from pathlib import Path
 
 from katalytic.pkg import get_version
 
 __version__, __version_info__ = get_version(__name__)
 
 
+def load_json(path, *, encoding='utf-8', sort_keys=True, **kwargs):
+    with open(path, encoding=encoding) as f:
+        if sort_keys:
+            return _sort_dict_keys_recursive(json.load(f, **kwargs))
+        else:
+            return json.load(f, **kwargs)
+
+
+def save_json(data, path, *, encoding='utf-8', indent=4, sort_keys=True, **kwargs):
+    if isinstance(indent, float) and indent.is_integer():
+        indent = int(indent)
+    elif not isinstance(indent, int):
+        raise TypeError(f'<indent> expects a positive integer. Got {indent!r}')
+    elif isinstance(indent, bool):
+        raise TypeError(f'<indent> expects a positive integer. Got {indent!r}')
+    elif indent < 0:
+        raise ValueError(f'<indent> expects a positive integer. Got {indent!r}')
+
+    with open(path, 'w', encoding=encoding) as f:
+        json.dump(data, f, indent=indent, sort_keys=sort_keys, **kwargs)
+
+
 def clear_dir(path, *, create_missing=True):
     """This function is not named "empty_dir" to avoid confusing it with "is_dir_empty"."""
     if not isinstance(create_missing, bool):
         raise TypeError(f'<create_missing> expects False or True. Got {type(create_missing)}')
 
     path = Path(path)
     delete_dir(path, missing_ok=True, non_empty_dir=True)
@@ -281,7 +307,16 @@
 def _is_none_of(obj, options):
     """Required when you have singletons (None, False, True) in the options"""
     return not _is_any_of(obj, options)
 
 
 def _is_singleton(obj):
     return obj is None or isinstance(obj, bool)
+
+
+def _sort_dict_keys_recursive(data):
+    if isinstance(data, dict):
+        return {k: _sort_dict_keys_recursive(v) for k, v in sorted(data.items())}
+    elif isinstance(data, collections.Iterable) and not isinstance(data, str):
+        return type(data)(_sort_dict_keys_recursive(item) for item in data)
+    else:
+        return data
```

### Comparing `katalytic-files-0.3.9/tests/test_files.py` & `katalytic-files-0.4.0/tests/test_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,89 @@
 import collections
 import shutil
 import tempfile
 from pathlib import Path
 
 import pytest
 
-from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, make_dir, move_dir, move_file
+from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, load_json, make_dir, move_dir, move_file, save_json
+
+
+class TestGroup_save_and_load:
+    class Test_json:
+        def test_indent_0(self):
+            data = self.create_json_data()
+            path = _setup_path()
+            save_json(data, path, indent=0)
+            assert load_json(path) == data
+
+        def test_indent_positive(self):
+            data = self.create_json_data()
+            path = _setup_path()
+            save_json(data, path, indent=4)
+            assert load_json(path) == data
+
+        def test_indent_negative(self):
+            data = self.create_json_data()
+            path = _setup_path()
+            with pytest.raises(ValueError):
+                save_json(data, path, indent=-1)
+
+        def test_indent_as_float(self):
+            data = self.create_json_data()
+            path = _setup_path()
+
+            save_json(data, path, indent=1.0)
+            assert load_json(path) == data
+
+        @pytest.mark.parametrize('mistake', ['1', 1.1, True, False, None, [], {}, (), object()])
+        def test_indent_of_wrong_type(self, mistake):
+            data = self.create_json_data()
+            path = _setup_path()
+            with pytest.raises(TypeError):
+                save_json(data, path, indent=mistake)
+
+        def test_save_sort_keys(self):
+            data = self.create_json_data()
+            path = _setup_path()
+            save_json(data, path, sort_keys=True)
+            assert self.are_keys_sorted_recursive(load_json(path, sort_keys=False))
+
+        def test_save_sort_keys_False(self):
+            data = self.create_json_data()
+            path = _setup_path()
+            save_json(data, path, sort_keys=False)
+            assert not self.are_keys_sorted_recursive(load_json(path, sort_keys=False))
+
+        def test_load_sort_keys(self):
+            data = self.create_json_data()
+            path = _setup_path()
+            save_json(data, path, sort_keys=False)
+            assert self.are_keys_sorted_recursive(load_json(path, sort_keys=True))
+
+        def test_load_sort_keys_False(self):
+            data = self.create_json_data()
+            path = _setup_path()
+            save_json(data, path, sort_keys=False)
+            assert not self.are_keys_sorted_recursive(load_json(path, sort_keys=False))
+
+        def are_keys_sorted_recursive(self, data):
+            if isinstance(data, dict):
+                if list(data.keys()) != sorted(data.keys()):
+                    return False
+
+                return all(self.are_keys_sorted_recursive(v) for v in data.values())
+            elif isinstance(data, collections.Iterable) and not isinstance(data, str):
+                return all(self.are_keys_sorted_recursive(item) for item in data)
+            else:
+                return True
+
+        def create_json_data(self):
+            """The keys are not sorted on purpose."""
+            return {'e': 0, 'a': 1, 'b': 2.0, 'c': 3.5, 'd': [{'y': None, 'f': True, 'g': {'x': 'i', 'j': [False]}}]}
 
 
 class TestGroup_copy:
     class Test_copy_dir:
         def test_dest_is_dir(self):
             src = Path(_setup_tree('{}_src'))
 
@@ -350,15 +424,15 @@
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_all(get_unique_path())
 
         def test_iter(self):
             r = get_all('', iter_=True)
-            assert isinstance(r, collections.abc.Iterator)
+            assert isinstance(r, collections.Iterator)
 
         def test_glob(self):
             path = _setup_tree_2()
             assert get_all(f'{path}/*/a/*') == [f'{path}/a/a/6.py', f'{path}/b/a/5.py']
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
@@ -467,15 +541,15 @@
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_dirs(get_unique_path())
 
         def test_iter(self):
             r = get_dirs('', iter_=True)
-            assert isinstance(r, collections.abc.Iterator)
+            assert isinstance(r, collections.Iterator)
 
         def test_glob(self):
             path = _setup_tree_2()
             assert get_dirs(f'{path}/*/a') == [f'{path}/a/a', f'{path}/b/a']
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
@@ -552,15 +626,15 @@
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_files(get_unique_path())
 
         def test_iter(self):
             r = get_files('', iter_=True)
-            assert isinstance(r, collections.abc.Iterator)
+            assert isinstance(r, collections.Iterator)
 
         def test_glob(self):
             path = _setup_tree_2()
             assert get_files(f'{path}/*.py') == [f'{path}/1.py']
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
```

### Comparing `katalytic-files-0.3.9/PKG-INFO` & `katalytic-files-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.3.9
+Version: 0.4.0
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,15 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-files)](https://pypi.org/project/katalytic-files/)
 [![Build Status](https://app.travis-ci.com/katalytic/katalytic-files.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
 [![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-files?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
 [![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-files/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-files?branch=main)
+[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-files.svg)](https://katalytic-files.readthedocs.io/en/latest/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-files
 ```
```

