# Comparing `tmp/qemu-runner-1.2.0.tar.gz` & `tmp/qemu-runner-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qemu-runner-1.2.0.tar", last modified: Sun Feb 12 18:23:44 2023, max compression
+gzip compressed data, was "qemu-runner-1.3.0.tar", last modified: Sat Apr 15 08:40:20 2023, max compression
```

## Comparing `qemu-runner-1.2.0.tar` & `qemu-runner-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:23:44.478298 qemu-runner-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-02-12 18:23:44.478298 qemu-runner-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 18:23:44.478298 qemu-runner-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:23:44.466297 qemu-runner-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:23:44.470297 qemu-runner-1.2.0/src/qemu_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/layer_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:23:44.474297 qemu-runner-1.2.0/src/qemu_runner/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/layers/virt-cortex-m.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:23:44.474297 qemu-runner-1.2.0/src/qemu_runner/make_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/make_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/make_runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/make_runner/main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/make_runner/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/make_runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/src/qemu_runner/variable_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:23:44.474297 qemu-runner-1.2.0/src/qemu_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-02-12 18:23:44.000000 qemu-runner-1.2.0/src/qemu_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-12 18:23:44.000000 qemu-runner-1.2.0/src/qemu_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 18:23:44.000000 qemu-runner-1.2.0/src/qemu_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-12 18:23:44.000000 qemu-runner-1.2.0/src/qemu_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-12 18:23:44.000000 qemu-runner-1.2.0/src/qemu_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 18:23:44.478298 qemu-runner-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_find_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_layer_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_layer_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_layer_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_qemu_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_qemu_argument_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_runner_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_utllities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-02-12 18:23:32.000000 qemu-runner-1.2.0/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.828066 qemu-runner-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.832066 qemu-runner-1.3.0/src/qemu_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/layer_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.836066 qemu-runner-1.3.0/src/qemu_runner/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/layers/virt-cortex-m.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.836066 qemu-runner-1.3.0/src/qemu_runner/make_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/make_runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/src/qemu_runner/variable_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.836066 qemu-runner-1.3.0/src/qemu_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 08:40:20.000000 qemu-runner-1.3.0/src/qemu_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:40:20.840066 qemu-runner-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_find_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_layer_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_qemu_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_qemu_argument_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_runner_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_utllities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-15 08:40:07.000000 qemu-runner-1.3.0/tests/test_venv.py
```

### Comparing `qemu-runner-1.2.0/LICENSE.txt` & `qemu-runner-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/PKG-INFO` & `qemu-runner-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.2.0
+Version: 1.3.0
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
-Home-page: https://github.com/Novakov/qemu-runne
+Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -69,15 +69,16 @@
    1. `c:\dir1\dir2`
    2. `c:\dir1\dir2\qemu`
    3. `c:\dir1\`
    4. `c:\dir1\qemu`
    5. `c:\`
    6. `c:\qemu`
 4. Repeat step 2 with path of base runner in case of derived runners with `--tract-qemu` option.
-5. Directories in `PATH` environment variable.
+5. Repeat step 2 with path of passed as `--qemu-dir` when runner was derived.
+6. Directories in `PATH` environment variable.
 
 On Windows, `PATHEXT` variable is used to determine executable extension.
 
 # Environment variables
 Several environment variables influences the way QEMU command line is constructed:
 * `QEMU_FLAGS` - arguments to be added to the QEMU command line during execution 
 * `QEMU_RUNNER_FLAGS` - arguments will be interpreted exactly as if they were added to runner execution.
```

### Comparing `qemu-runner-1.2.0/README.md` & `qemu-runner-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,16 @@
    1. `c:\dir1\dir2`
    2. `c:\dir1\dir2\qemu`
    3. `c:\dir1\`
    4. `c:\dir1\qemu`
    5. `c:\`
    6. `c:\qemu`
 4. Repeat step 2 with path of base runner in case of derived runners with `--tract-qemu` option.
-5. Directories in `PATH` environment variable.
+5. Repeat step 2 with path of passed as `--qemu-dir` when runner was derived.
+6. Directories in `PATH` environment variable.
 
 On Windows, `PATHEXT` variable is used to determine executable extension.
 
 # Environment variables
 Several environment variables influences the way QEMU command line is constructed:
 * `QEMU_FLAGS` - arguments to be added to the QEMU command line during execution 
 * `QEMU_RUNNER_FLAGS` - arguments will be interpreted exactly as if they were added to runner execution.
```

### Comparing `qemu-runner-1.2.0/setup.py` & `qemu-runner-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 
 with open(os.path.dirname(os.path.abspath(__file__)) + '/README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='qemu-runner',
-    version='1.2.0',
+    version='1.3.0',
     description='Create self-contained wrappers around QEMU to hide & share long command-line invocations',
-    url='https://github.com/Novakov/qemu-runne',
+    url='https://github.com/Novakov/qemu-runner',
     long_description=description,
     long_description_content_type='text/markdown',
     author='Maciej Nowak',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
```

### Comparing `qemu-runner-1.2.0/src/qemu_runner/argument.py` & `qemu-runner-1.3.0/src/qemu_runner/argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/src/qemu_runner/find_qemu.py` & `qemu-runner-1.3.0/src/qemu_runner/find_qemu.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/src/qemu_runner/layer.py` & `qemu-runner-1.3.0/src/qemu_runner/layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/src/qemu_runner/layer_locator.py` & `qemu-runner-1.3.0/src/qemu_runner/layer_locator.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/src/qemu_runner/make_runner/__main__.py` & `qemu-runner-1.3.0/src/qemu_runner/make_runner/__main__.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/src/qemu_runner/make_runner/make.py` & `qemu-runner-1.3.0/src/qemu_runner/make_runner/make.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import importlib.resources
 import os
 import pkgutil
 import shutil
 import zipfile
 import zipimport
-from importlib import resources
-try:
-    from importlib.resources.abc import Traversable
-except ImportError:
-    try:
-        from importlib.abc import Traversable
-    except ImportError:
-        pass
 from pathlib import Path
 from typing import IO, List, Any
 import pkg_resources
 
 from qemu_runner.layer_locator import load_layer
 import qemu_runner
 
@@ -31,15 +23,15 @@
         ep: pkg_resources.EntryPoint
         packages.append(ep.module_name)
 
     return [load_layer(layer, packages=packages) for layer in layer_names]
 
 
 if hasattr(importlib.resources, 'files'):
-    def copy_directory_traversable(root: Traversable, archive: zipfile.ZipFile, subdir: Path) -> None:
+    def copy_directory_traversable(root: 'Traversable', archive: zipfile.ZipFile, subdir: Path) -> None:
         for item in root.iterdir():
             if item.name in ['__pycache__']:
                 continue
 
             if item.is_file():
                 with archive.open(str(subdir / item.name), 'w') as out_f:
                     with item.open('rb') as in_f:
@@ -76,14 +68,15 @@
             with source.open(f, 'r') as in_f:
                 with target_archive.open(str(target_sub_dir / rel_path), 'w') as out_f:
                     shutil.copyfileobj(in_f, out_f)
 
 
 def copy_package(package: Any, archive: zipfile.ZipFile) -> None:
     if hasattr(importlib.resources, 'files'):
+        from importlib import resources
         # Python 3.9+ has nice access to files in package using importlib.resources.file and Traversable
         copy_directory_traversable(resources.files(package), archive, Path(package.__name__))
     elif isinstance(package.__loader__, zipimport.zipimporter):
         # For older Python we need to treat packages from zip (runner) differently
         # zipimporter gives path to archive file, so we work how to open zip file
         # and extract package from it.
         # it's terrible
@@ -91,25 +84,25 @@
         copy_directory_from_zip(
             archive_file=Path(package.__loader__.archive),
             source_sub_dir=source_dir,
             target_archive=archive,
             target_sub_dir=Path(package.__name__)
         )
     else:
-        # No Python 3.9, not zipimproter, let's hope that importlib.resources.path will do the job
+        # No Python 3.9, not zipimporter, let's hope that importlib.resources.path will do the job
         with importlib.resources.path(qemu_runner, '') as p:
             copy_directory_path(p, archive, package.__name__)
 
 
 def make_runner(output: IO[bytes],
                 *,
                 layer_contents: List[str],
                 additional_script_bases: List[str]
                 ) -> None:
-    with zipfile.ZipFile(output, mode='w') as archive:
+    with zipfile.ZipFile(output, mode='w', compression=zipfile.ZIP_STORED) as archive:
         copy_package(qemu_runner, archive)
 
         with archive.open('embedded_layers/__init__.py', 'w'):
             pass
 
         for i, layer_content in enumerate(layer_contents):
             with archive.open(f'embedded_layers/layers/{i}.ini', 'w') as f1:
```

### Comparing `qemu-runner-1.2.0/src/qemu_runner/make_runner/runner.py` & `qemu-runner-1.3.0/src/qemu_runner/make_runner/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 import shlex
 import subprocess
 import sys
 from configparser import ConfigParser
 from pathlib import Path
 from typing import List, Optional
 
-from qemu_runner import find_qemu
-from qemu_runner.layer import Layer, parse_layer, build_command_line, GeneralSettings
-from qemu_runner.layer_locator import load_layer
-from qemu_runner.make_runner import make_runner, load_layers_from_all_search_paths
-
 
 def make_arg_parser():
     parser = argparse.ArgumentParser()
     parser.formatter_class = argparse.RawDescriptionHelpFormatter
 
     parser.description = '''QEMU runner wraps series of layers describing QEMU arguments as standalone executable file (ZIP file actually)
 requiring only Python 3.8+ standard library. 
@@ -30,15 +25,16 @@
 QEMU search precedence:
     1. QEMU_DEV environment variable, direct path to executable (currently: {qemu_dev})
     2. --qemu argument as direct path to executable (if specified)
     3. QEMU_DIR environment variable, path to directory containing QEMU executable (currently: {qemu_dir})
     4. --qemu-dir argument (if specified)
     5. Runner and it's ancestor directories and /qemu subdirectory on each level
     6. The same rule as (3) but for paths of base runners when derived with --track-qemu flag
-    7. Directories in PATH environment variable
+    7. The same rule as (3) but for paths added with --qemu-dir when derived
+    8. Directories in PATH environment variable
     
 Runtime QEMU flags
     1. Contents of QEMU_RUNNER_FLAGS (currently: {qemu_runner_flags}) are treated as runner arguments
     2. Contents of QEMU_FLAGS (currently: {qemu_flags}) are added as QEMU arguments without any interpretation 
 '''
 
     runner_args = parser.add_argument_group('Runner arguments')
@@ -67,15 +63,16 @@
     program_args.add_argument('--dry-run', action='store_true', help='Do not execute QEMU, just output command line')
     program_args.add_argument('kernel', help='Executable to run under QEMU', nargs='?')
     program_args.add_argument('arguments', nargs=argparse.REMAINDER, help='Arguments passed to executable', default=[])
 
     return parser
 
 
-def make_layer_from_args(args: argparse.Namespace) -> Layer:
+def make_layer_from_args(args: argparse.Namespace) -> 'Layer':
+    from qemu_runner.layer import GeneralSettings, Layer
     general = GeneralSettings(
         kernel=args.kernel,
         kernel_cmdline=' '.join(args.arguments),
         gdb=args.debug,
         gdb_dev=args.debug_listen,
         halted=args.halted,
     )
@@ -84,41 +81,46 @@
 
 def build_qemu_command_line(
         *,
         embedded_layers: List[str],
         additional_script_bases: List[str],
         args: argparse.Namespace,
         additional_qemu_args: str) -> List[str]:
+    from qemu_runner.layer_locator import load_layer
     layer_contents = [load_layer(
         layer,
         packages=['embedded_layers']
     ) for layer in embedded_layers]
 
+    from qemu_runner.layer import Layer
     combined_layer = Layer()
 
     for layer_content in layer_contents:
         parser = ConfigParser()
         parser.read_string(layer_content)
+        from qemu_runner.layer import parse_layer
         layer = parse_layer(parser)
         combined_layer = combined_layer.apply(layer)
 
     args_layer = make_layer_from_args(args)
 
     combined_layer = combined_layer.apply(args_layer)
 
     def do_find_qemu(engine: str) -> Optional[Path]:
         if args.qemu:
             return Path(args.qemu)
 
+        from qemu_runner import find_qemu
         return find_qemu(
             engine=engine,
             script_paths=[__file__] + additional_script_bases,
             search_paths=[args.qemu_dir] if args.qemu_dir else []
         )
 
+    from qemu_runner.layer import build_command_line
     full_cmdline = build_command_line(combined_layer, find_qemu_func=do_find_qemu)
 
     result = list(full_cmdline)
 
     if additional_qemu_args != '':
         user_qemu_args = shlex.split(additional_qemu_args, posix=sys.platform != 'win32')
         result = [result[0], *user_qemu_args, *result[1:]]
@@ -131,26 +133,31 @@
         cp = subprocess.run(command_line)
         sys.exit(cp.returncode)
     except FileNotFoundError:
         raise
 
 
 def make_derived_runner(embedded_layers: List[str], args: argparse.Namespace) -> None:
+    from qemu_runner.make_runner.make import make_runner, load_layers_from_all_search_paths
+    from qemu_runner.layer_locator import load_layer
     base_layers = [load_layer(
         layer,
         packages=['embedded_layers']
     ) for layer in embedded_layers]
 
     additional_layers = load_layers_from_all_search_paths(args.layers)
 
     if args.track_qemu:
         base_script_paths: List[str] = [__file__]
     else:
         base_script_paths = []
 
+    if args.qemu_dir:
+        base_script_paths.append(args.qemu_dir)
+
     make_runner(
         args.derive,
         layer_contents=base_layers + additional_layers,
         additional_script_bases=base_script_paths
     )
 
 
@@ -163,14 +170,15 @@
         formatter = TerminalFormatter()
         return lambda s: print(highlight(s, lexer, formatter).strip())
     except ImportError:
         return lambda s: print(s)
 
 
 def inspect_runner(embedded_layers: List[str]) -> None:
+    from qemu_runner.layer_locator import load_layer
     layers = [(layer, load_layer(
         layer,
         packages=['embedded_layers']
     )) for layer in embedded_layers]
 
     print_ini = make_layer_printer()
```

### Comparing `qemu-runner-1.2.0/src/qemu_runner/variable_resolution.py` & `qemu-runner-1.3.0/src/qemu_runner/variable_resolution.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/src/qemu_runner.egg-info/PKG-INFO` & `qemu-runner-1.3.0/src/qemu_runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.2.0
+Version: 1.3.0
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
-Home-page: https://github.com/Novakov/qemu-runne
+Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Embedded Systems
@@ -69,15 +69,16 @@
    1. `c:\dir1\dir2`
    2. `c:\dir1\dir2\qemu`
    3. `c:\dir1\`
    4. `c:\dir1\qemu`
    5. `c:\`
    6. `c:\qemu`
 4. Repeat step 2 with path of base runner in case of derived runners with `--tract-qemu` option.
-5. Directories in `PATH` environment variable.
+5. Repeat step 2 with path of passed as `--qemu-dir` when runner was derived.
+6. Directories in `PATH` environment variable.
 
 On Windows, `PATHEXT` variable is used to determine executable extension.
 
 # Environment variables
 Several environment variables influences the way QEMU command line is constructed:
 * `QEMU_FLAGS` - arguments to be added to the QEMU command line during execution 
 * `QEMU_RUNNER_FLAGS` - arguments will be interpreted exactly as if they were added to runner execution.
```

### Comparing `qemu-runner-1.2.0/src/qemu_runner.egg-info/SOURCES.txt` & `qemu-runner-1.3.0/src/qemu_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_find_layer.py` & `qemu-runner-1.3.0/tests/test_find_layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_find_qemu.py` & `qemu-runner-1.3.0/tests/test_find_qemu.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_layer.py` & `qemu-runner-1.3.0/tests/test_layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_layer_cmdline.py` & `qemu-runner-1.3.0/tests/test_layer_cmdline.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_layer_equality.py` & `qemu-runner-1.3.0/tests/test_layer_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_layer_parsing.py` & `qemu-runner-1.3.0/tests/test_layer_parsing.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_qemu_argument.py` & `qemu-runner-1.3.0/tests/test_qemu_argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_qemu_argument_equality.py` & `qemu-runner-1.3.0/tests/test_qemu_argument_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_runner_flow.py` & `qemu-runner-1.3.0/tests/test_runner_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     cp = subprocess.run(
         [sys.executable, '-m', 'qemu_runner.make_runner', *map(str, args)],
         cwd=cwd
     )
     assert cp.returncode == 0
 
 
-def execute_runner(runner, args: Sequence[CmdlineArg], cwd: Optional[os.PathLike] = None, check: bool = True) -> subprocess.CompletedProcess:
+def execute_runner(runner, args: Sequence[CmdlineArg], cwd: Optional[os.PathLike] = None,
+                   check: bool = True) -> subprocess.CompletedProcess:
     cp = subprocess.run(
         [sys.executable, str(runner), *map(str, args)],
         cwd=cwd,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding='utf-8'
     )
@@ -134,16 +135,16 @@
 
     run_make_runner('-l', 'virt-cortex-m.ini', 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     with with_env({'QEMU_DEV': 'my-qemu'}):
         cp = execute_runner(tmp_path / 'test.pyz', ['--debug', '--dry-run', 'abc.elf', 'a', 'b', 'c'])
 
     assert cp.stdout.strip() == (
-                "my-qemu -machine virt_cortex_m,flash_kb=1024 -device test_device,id=test_id,addr=12 " +
-                "-s -kernel abc.elf -append 'a b c'")
+            "my-qemu -machine virt_cortex_m,flash_kb=1024 -device test_device,id=test_id,addr=12 " +
+            "-s -kernel abc.elf -append 'a b c'")
 
 
 def test_extract_base_command_line_no_kernel(tmp_path: Path):
     with open(tmp_path / 'my-layer.ini', 'w') as f:
         f.write("""
         [device:test_id]
         @=test_device
@@ -205,15 +206,43 @@
         @=test
         """)
 
     run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'dir1' / 'base_runner.pyz', cwd=tmp_path)
 
     (tmp_path / 'dir2').mkdir()
     execute_runner(
-        tmp_path / 'dir1' / 'base_runner.pyz', ['--layers', './layer1.ini', '--derive', './dir2/derived.pyz', '--track-qemu'],
+        tmp_path / 'dir1' / 'base_runner.pyz',
+        ['--layers', './layer1.ini', '--derive', './dir2/derived.pyz', '--track-qemu'],
+        cwd=tmp_path
+    )
+
+    cmdline = capture_runner_cmdline(tmp_path / 'dir2' / 'derived.pyz', 'abc.elf')
+
+    assert cmdline[0] == engine
+
+
+def test_derive_add_qemu_dir(tmp_path: Path):
+    engine = place_echo_args(tmp_path / 'dir1' / 'qemu' / 'my-qemu')
+
+    with open(tmp_path / 'layer1.ini', 'w') as f:
+        f.write("""
+        [general]
+        engine = my-qemu
+
+        [device:d1]
+        @=test
+        """)
+
+    (tmp_path / 'dir2').mkdir()
+
+    run_make_runner('-l', './layer1.ini', '-o', tmp_path / 'dir2' / 'base_runner.pyz', cwd=tmp_path)
+
+    execute_runner(
+        tmp_path / 'dir2' / 'base_runner.pyz',
+        ['--layers', './layer1.ini', '--derive', './dir2/derived.pyz', '--qemu-dir', tmp_path / 'dir1' / 'qemu'],
         cwd=tmp_path
     )
 
     cmdline = capture_runner_cmdline(tmp_path / 'dir2' / 'derived.pyz', 'abc.elf')
 
     assert cmdline[0] == engine
```

### Comparing `qemu-runner-1.2.0/tests/test_utllities.py` & `qemu-runner-1.3.0/tests/test_utllities.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.2.0/tests/test_venv.py` & `qemu-runner-1.3.0/tests/test_venv.py`

 * *Files identical despite different names*

