# Comparing `tmp/pure_safetensors-0.3.1.tar.gz` & `tmp/pure_safetensors-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_safetensors-0.3.1.tar", last modified: Wed Apr 12 08:48:52 2023, max compression
+gzip compressed data, was "pure_safetensors-0.3.2.tar", last modified: Sat Apr 15 06:53:10 2023, max compression
```

## Comparing `pure_safetensors-0.3.1.tar` & `pure_safetensors-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/
--rw-r--r--   0 user      (1000) user      (1000)      595 2023-04-12 08:48:07.000000 pure_safetensors-0.3.1/CHANGELOG.md
--rw-r--r--   0 user      (1000) user      (1000)       58 2023-04-12 08:46:43.000000 pure_safetensors-0.3.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     3174 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/README.md
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-12 08:48:24.000000 pure_safetensors-0.3.1/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.297149 pure_safetensors-0.3.1/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/src/pure_safetensors/
--rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/src/pure_safetensors/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2270 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     2329 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/adapter.py
--rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/src/pure_safetensors/exc.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/src/pure_safetensors/ext/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/ext/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3305 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/ext/torch.py
--rw-r--r--   0 user      (1000) user      (1000)     4194 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/mmap.py
--rw-r--r--   0 user      (1000) user      (1000)     1472 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/numpy.py
--rw-r--r--   0 user      (1000) user      (1000)    26018 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/safetensors.py
--rw-r--r--   0 user      (1000) user      (1000)     1159 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      714 2023-04-12 08:48:52.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      442 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/tests/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)       56 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/tests/test_errors.py
--rw-r--r--   0 user      (1000) user      (1000)     2113 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/tests/test_hypothesis.py
--rw-r--r--   0 user      (1000) user      (1000)     2127 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/tests/test_roundtrip.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:53:10.788496 pure_safetensors-0.3.2/
+-rw-r--r--   0 user      (1000) user      (1000)      808 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/CHANGELOG.md
+-rw-r--r--   0 user      (1000) user      (1000)       58 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     4838 2023-04-15 06:53:10.788496 pure_safetensors-0.3.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     3751 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-15 06:53:10.788496 pure_safetensors-0.3.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-15 06:52:37.000000 pure_safetensors-0.3.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:53:10.778496 pure_safetensors-0.3.2/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:53:10.788496 pure_safetensors-0.3.2/src/pure_safetensors/
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3006 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2329 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/adapter.py
+-rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/exc.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:53:10.788496 pure_safetensors-0.3.2/src/pure_safetensors/ext/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/ext/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     7251 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/ext/torch.py
+-rw-r--r--   0 user      (1000) user      (1000)     4194 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/mmap.py
+-rw-r--r--   0 user      (1000) user      (1000)     1472 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/numpy.py
+-rw-r--r--   0 user      (1000) user      (1000)    26782 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/safetensors.py
+-rw-r--r--   0 user      (1000) user      (1000)     1286 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/src/pure_safetensors/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:53:10.788496 pure_safetensors-0.3.2/src/pure_safetensors.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4838 2023-04-15 06:53:10.000000 pure_safetensors-0.3.2/src/pure_safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      714 2023-04-15 06:53:10.000000 pure_safetensors-0.3.2/src/pure_safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-15 06:53:10.000000 pure_safetensors-0.3.2/src/pure_safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-15 06:53:10.000000 pure_safetensors-0.3.2/src/pure_safetensors.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-15 06:53:10.000000 pure_safetensors-0.3.2/src/pure_safetensors.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:53:10.788496 pure_safetensors-0.3.2/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      442 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/tests/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)       56 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/tests/test_errors.py
+-rw-r--r--   0 user      (1000) user      (1000)     2113 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/tests/test_hypothesis.py
+-rw-r--r--   0 user      (1000) user      (1000)     2127 2023-04-15 06:44:12.000000 pure_safetensors-0.3.2/tests/test_roundtrip.py
```

### Comparing `pure_safetensors-0.3.1/PKG-INFO` & `pure_safetensors-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: pure_safetensors
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pure-Python safetensors
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # pure_safetensors
         
         [Safetensors](https://github.com/huggingface/safetensors) library but in pure clean Python. Run it on PyPy or IronPython or wherever.
         
-        # Dependencies
+        ## Dependencies
         
         We try to keep dependencies light:
         
         - [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
         - [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
         - [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
         - (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
         - (optional) [fickle](https://pypi.org/project/fickle/) whitelist-based firewall for safe pickle loading, used for PyTorch model conversion (926 LoC)
         
         Optionally, this library integrates with NumPy (if available). PyTorch integration is planned, someday.
         
         To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
         
-        # Examples
+        ## Examples
         
         ```python
         from pure_safetensors import SafeTensors
         
         with SafeTensors("/path/to/example.safetensors", "r+") as sf:
             arrays = sf.as_numpy()
             arrays["hello"][3, :] += 420.69
@@ -43,27 +43,39 @@
                 }
             )
         
             # delete arrays! such wonders!
             del arrays["v"]
         ```
         
-        Do you have an existing PyTorch checkpoint model that you would like to safetensors? Then try running:
+        ## Conversion
+        
+        Do you have an existing PyTorch checkpoint model that you would like to convert to safetensors? Then try running:
         
         ```sh
         python3 -m pure_safetensors import-pytorch /path/to/model.ckpt /path/to/model.safetensors
         ```
         
-        # Bugs
+        You may also be able to convert the model **in-place** without making an additional copy! Use this facility at your own risk (or make a zero-cost [copy-on-write](https://en.wikipedia.org/wiki/Copy-on-write) backup [copy](https://man.archlinux.org/man/cp.1.en#reflink) of your checkpoint file using `cp --reflink=always ...` if your filesystem [supports it](https://unix.stackexchange.com/a/631238)).
+        
+        ```sh
+        # convert it
+        python3 -m pure_safetensors import-pytorch-inplace /data/model.ckpt
+        
+        # rename
+        mv /data/model.ckpt /data/model.safetensors
+        ```
+        
+        ## Bugs
         
         The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
         
         PyTorch support isn't implemented yet.
         
-        # Alternatives
+        ## Alternatives
         
         - [safetensors](https://github.com/huggingface/safetensors/)
         - [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
         - [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
         
         |                                                 | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
         |-------------------------------------------------|------------------|-------------|---------------|-----------------|
```

### Comparing `pure_safetensors-0.3.1/README.md` & `pure_safetensors-0.3.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # pure_safetensors
 
 [Safetensors](https://github.com/huggingface/safetensors) library but in pure clean Python. Run it on PyPy or IronPython or wherever.
 
-# Dependencies
+## Dependencies
 
 We try to keep dependencies light:
 
 - [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
 - [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
 - [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
 - (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
 - (optional) [fickle](https://pypi.org/project/fickle/) whitelist-based firewall for safe pickle loading, used for PyTorch model conversion (926 LoC)
 
 Optionally, this library integrates with NumPy (if available). PyTorch integration is planned, someday.
 
 To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
 
-# Examples
+## Examples
 
 ```python
 from pure_safetensors import SafeTensors
 
 with SafeTensors("/path/to/example.safetensors", "r+") as sf:
     arrays = sf.as_numpy()
     arrays["hello"][3, :] += 420.69
@@ -35,27 +35,39 @@
         }
     )
 
     # delete arrays! such wonders!
     del arrays["v"]
 ```
 
-Do you have an existing PyTorch checkpoint model that you would like to safetensors? Then try running:
+## Conversion
+
+Do you have an existing PyTorch checkpoint model that you would like to convert to safetensors? Then try running:
 
 ```sh
 python3 -m pure_safetensors import-pytorch /path/to/model.ckpt /path/to/model.safetensors
 ```
 
-# Bugs
+You may also be able to convert the model **in-place** without making an additional copy! Use this facility at your own risk (or make a zero-cost [copy-on-write](https://en.wikipedia.org/wiki/Copy-on-write) backup [copy](https://man.archlinux.org/man/cp.1.en#reflink) of your checkpoint file using `cp --reflink=always ...` if your filesystem [supports it](https://unix.stackexchange.com/a/631238)).
+
+```sh
+# convert it
+python3 -m pure_safetensors import-pytorch-inplace /data/model.ckpt
+
+# rename
+mv /data/model.ckpt /data/model.safetensors
+```
+
+## Bugs
 
 The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
 
 PyTorch support isn't implemented yet.
 
-# Alternatives
+## Alternatives
 
 - [safetensors](https://github.com/huggingface/safetensors/)
 - [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
 - [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
 
 |                                                 | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
 |-------------------------------------------------|------------------|-------------|---------------|-----------------|
```

### Comparing `pure_safetensors-0.3.1/setup.py` & `pure_safetensors-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text("utf-8")
 
 setup(
     name="pure_safetensors",
     description="Pure-Python safetensors",
-    version="0.3.1",
+    version="0.3.2",
     author="Eduard Christian Dumitrescu",
     author_email="eduard.c.dumitrescu@gmail.com",
     install_requires=["attrs", "marshmallow", "sortedcollections"],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     license="MIT",
     classifiers=[
```

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors/__main__.py` & `pure_safetensors-0.3.2/src/pure_safetensors/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,18 +24,25 @@
                     f"  {t.start:>12d}-{t.end:<12d} "
                     f"{t.shape!r:>20s} {t.dtype.name:4s} {k!r:s}"
                 )
 
     def cmd_pytorch_import(self):
         from .ext.torch import PyTorchSafetensorsConverter
 
-        PyTorchSafetensorsConverter.convert(
+        PyTorchSafetensorsConverter.convert_file_to_file(
             torch_checkpoint=self.a.pytorch_file, safe_tensors=self.a.safetensors
         )
 
+    def cmd_pytorch_import_inplace(self):
+        from .ext.torch import PyTorchSafetensorsInplaceConverter
+
+        PyTorchSafetensorsInplaceConverter.convert_inplace(
+            torch_checkpoint=self.a.pytorch_file
+        )
+
     def init_argparser(self):
         parser = argparse.ArgumentParser()
         parser.set_defaults(callback=self.cmd_missing)
         subparsers = parser.add_subparsers()
 
         def _Path(x):
             return Path(x).resolve()
@@ -56,14 +63,26 @@
             "pytorch_file", type=_Path, help="PyTorch .ckpt checkpoint file (source)"
         )
         pytorch_import.add_argument(
             "safetensors", type=_Path, help="Safetensors file (destination)"
         )
         pytorch_import.set_defaults(callback=self.cmd_pytorch_import)
 
+        pytorch_import_inplace = subparsers.add_parser(
+            "import-pytorch-inplace",
+            help='Convert pytorch ".ckpt" file to safetensors by modifying it',
+        )
+        pytorch_import_inplace.add_argument(
+            "pytorch_file",
+            type=_Path,
+            help="PyTorch .ckpt checkpoint file that will be modified to become "
+            "a safetensors file",
+        )
+        pytorch_import_inplace.set_defaults(callback=self.cmd_pytorch_import_inplace)
+
         return parser
 
     def run(self):
         self.a.callback()
 
     @classmethod
     def main(cls, argv=None):
```

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors/adapter.py` & `pure_safetensors-0.3.2/src/pure_safetensors/adapter.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors/mmap.py` & `pure_safetensors-0.3.2/src/pure_safetensors/mmap.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors/numpy.py` & `pure_safetensors-0.3.2/src/pure_safetensors/numpy.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors/safetensors.py` & `pure_safetensors-0.3.2/src/pure_safetensors/safetensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import functools
 import json
-import operator
 import os
 import struct
 from typing import Dict, IO, Iterable, List, Optional, Tuple
 
 import attr
 import marshmallow
 from marshmallow import fields
@@ -15,15 +14,15 @@
     FakeMemoryMappingFactory,
     MemoryMapping,
     MemoryMappingFactory,
     RealMemoryMappingFactory,
     mmap,
 )
 from .exc import SafeTensorError, SafeTensorHeaderError, SafeTensorEmptyFileError
-from .util import align, samefile_copy
+from .util import align, prod, samefile_copy
 
 try:
     import sparsefile
 except ImportError:
     sparsefile = None
 
 
@@ -50,23 +49,30 @@
         w+: Create or overwrite existing file for reading and writing.
         c: Copy-on-write: assignments affect data in memory, but changes are
            not saved to disk. The file on disk is read-only.
     sparse: bool or None, optional
         If True, make the file sparse. If False, then don't. If None, then
         try to make it sparse but don't raise an exception if it's not possible
         to do so.
+    use_mmap: bool, optional
+        Use mmap? Default value depends on whether it is supported.
+    do_not_initialize_map: bool, optional
+        If True, do not read or write the file header on instance init. This is
+        used for PyTorch checkpoint in-place conversion, and I don't know
+        what else you could be using it for (default: False).
     """
 
     _valid_modes = frozenset(("r", "r+", "x+", "w+", "c"))
 
     file: IO = attr.ib()
     mode: str = attr.ib()
     sparse: bool = attr.ib(default=None)
     settings: "Settings" = attr.ib(factory=lambda: Settings(), kw_only=True)
     use_mmap: bool = attr.ib(factory=lambda: use_mmap)
+    do_not_initialize_map = attr.ib(default=False)
 
     mappings: Dict[str, MemoryMapping] = attr.ib(init=False, factory=dict)
 
     map: "FileMap"
     tensors: "Dict[str, SafeTensorInfo]"
     _memory_mapping_factory: MemoryMappingFactory
 
@@ -84,25 +90,33 @@
         # replace "x+" with "w+" since they are equivalent after the file is created
         if self.mode == "x+":
             self.mode = "w+"
 
         self._init_memory_mapping_factory()
 
         # load file or write empty header if creating new file
-        self._initialize_structure()
+        if not self.do_not_initialize_map:
+            self._initialize_structure()
 
     def _init_memory_mapping_factory(self):
         cls = RealMemoryMappingFactory if self.use_mmap else FakeMemoryMappingFactory
         self._memory_mapping_factory = cls(file=self.file, mode=self.mode)
 
     @mode.validator
     def check(self, attribute, value):
         if value not in self._valid_modes:
             raise ValueError(f"{value!r} not in {self._valid_modes!r}")
 
+    def assert_writable(self):
+        mode = self.mode
+        if mode == "c" or mode == "r":
+            raise AssertionError(
+                "operation not supported since file opened with mode={mode!r}"
+            )
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def close(self):
@@ -124,14 +138,15 @@
         else:
             self._write_empty_header()
 
     def _write_empty_header(self):
         self._write_header(FileMap(settings=self.settings))
 
     def _write_header(self, file_map):
+        self.assert_writable()
         # temporarily destroy the file header to prevent usage of a broken file
         # if the moves below fail
         self.file.seek(0)
         self.file.write(b"\0\0\0\0\0\0\0\0")
 
         for move in file_map.pending_moves:
             samefile_copy(self.file, src=move.src, dst=move.dst, length=move.len)
@@ -200,14 +215,15 @@
         move existing tensors to make way for a larger header. As such, it is NOT
         safe to use this method if you have existing memory mappings.
 
         If a tensor is ``None``, then it will be deleted.
 
         Existing tensors (with the same name) will be replaced/moved.
         """
+        self.assert_writable()
 
         file_map = self.map.copy()
         file_map.modify(
             create={
                 name: tensor for name, tensor in tensors.items() if tensor is not None
             },
             delete={name for name, tensor in tensors.items() if tensor is None},
@@ -220,24 +236,26 @@
         self.truncate()
         self.sparsify()
 
     def truncate(self):
         """
         Truncate file to its smallest possible size.
         """
+        self.assert_writable()
         n = self.map.minimum_file_size
         self.file.seek(n)
         self.file.write(b"\0")
         self.file.flush()
         self.file.truncate(n)
 
     def sparsify(self):
         """
         Make file sparse, depending on the value of :attr:`sparse`.
         """
+        self.assert_writable()
         if self.sparse is False:
             return
 
         if sparsefile is None:
             text = (
                 "module `sparsefile` not available, cannot "
                 "make file sparse to save space"
@@ -801,8 +819,8 @@
 
     @property
     def is_zero_length(self):
         return self.start == self.end
 
     @functools.cached_property
     def required_size(self):
-        return functools.reduce(operator.mul, self.shape, self.dtype.size_in_bytes)
+        return prod(self.shape, self.dtype.size_in_bytes)
```

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors/util.py` & `pure_safetensors-0.3.2/src/pure_safetensors/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+import functools
+import operator
 import os
 from typing import IO
 
 
+def prod(iterable, initial=1):
+    return functools.reduce(operator.mul, iterable, initial)
+
+
 def align(alignment: int, position: int) -> int:
     assert alignment & (alignment - 1) == 0
     mask = alignment - 1
     return (position + mask) & ~mask
 
 
 def align_down(alignment: int, position: int) -> int:
```

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors.egg-info/PKG-INFO` & `pure_safetensors-0.3.2/src/pure_safetensors.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: pure-safetensors
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pure-Python safetensors
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # pure_safetensors
         
         [Safetensors](https://github.com/huggingface/safetensors) library but in pure clean Python. Run it on PyPy or IronPython or wherever.
         
-        # Dependencies
+        ## Dependencies
         
         We try to keep dependencies light:
         
         - [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
         - [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
         - [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
         - (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
         - (optional) [fickle](https://pypi.org/project/fickle/) whitelist-based firewall for safe pickle loading, used for PyTorch model conversion (926 LoC)
         
         Optionally, this library integrates with NumPy (if available). PyTorch integration is planned, someday.
         
         To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
         
-        # Examples
+        ## Examples
         
         ```python
         from pure_safetensors import SafeTensors
         
         with SafeTensors("/path/to/example.safetensors", "r+") as sf:
             arrays = sf.as_numpy()
             arrays["hello"][3, :] += 420.69
@@ -43,27 +43,39 @@
                 }
             )
         
             # delete arrays! such wonders!
             del arrays["v"]
         ```
         
-        Do you have an existing PyTorch checkpoint model that you would like to safetensors? Then try running:
+        ## Conversion
+        
+        Do you have an existing PyTorch checkpoint model that you would like to convert to safetensors? Then try running:
         
         ```sh
         python3 -m pure_safetensors import-pytorch /path/to/model.ckpt /path/to/model.safetensors
         ```
         
-        # Bugs
+        You may also be able to convert the model **in-place** without making an additional copy! Use this facility at your own risk (or make a zero-cost [copy-on-write](https://en.wikipedia.org/wiki/Copy-on-write) backup [copy](https://man.archlinux.org/man/cp.1.en#reflink) of your checkpoint file using `cp --reflink=always ...` if your filesystem [supports it](https://unix.stackexchange.com/a/631238)).
+        
+        ```sh
+        # convert it
+        python3 -m pure_safetensors import-pytorch-inplace /data/model.ckpt
+        
+        # rename
+        mv /data/model.ckpt /data/model.safetensors
+        ```
+        
+        ## Bugs
         
         The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
         
         PyTorch support isn't implemented yet.
         
-        # Alternatives
+        ## Alternatives
         
         - [safetensors](https://github.com/huggingface/safetensors/)
         - [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
         - [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
         
         |                                                 | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
         |-------------------------------------------------|------------------|-------------|---------------|-----------------|
```

### Comparing `pure_safetensors-0.3.1/src/pure_safetensors.egg-info/SOURCES.txt` & `pure_safetensors-0.3.2/src/pure_safetensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.1/tests/test_hypothesis.py` & `pure_safetensors-0.3.2/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.1/tests/test_roundtrip.py` & `pure_safetensors-0.3.2/tests/test_roundtrip.py`

 * *Files identical despite different names*

