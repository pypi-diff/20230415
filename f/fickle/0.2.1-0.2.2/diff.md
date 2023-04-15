# Comparing `tmp/fickle-0.2.1.tar.gz` & `tmp/fickle-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fickle-0.2.1.tar", last modified: Wed Apr 12 08:41:22 2023, max compression
+gzip compressed data, was "fickle-0.2.2.tar", last modified: Sat Apr 15 06:42:03 2023, max compression
```

## Comparing `fickle-0.2.1.tar` & `fickle-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/
--rw-r--r--   0 user      (1000) user      (1000)       37 2023-03-31 04:34:09.000000 fickle-0.2.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3364 2023-04-12 08:41:22.318241 fickle-0.2.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2511 2023-03-31 02:29:03.000000 fickle-0.2.1/README.md
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-03-31 02:29:03.000000 fickle-0.2.1/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      105 2023-04-12 08:41:22.318241 fickle-0.2.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      726 2023-04-12 08:41:14.000000 fickle-0.2.1/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/fickle/
--rw-r--r--   0 user      (1000) user      (1000)       92 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      189 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/exc.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/fickle/ext/
--rw-r--r--   0 user      (1000) user      (1000)      143 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/ext/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     6576 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/ext/marshmallow.py
--rw-r--r--   0 user      (1000) user      (1000)     5970 2023-04-12 08:41:14.000000 fickle-0.2.1/src/fickle/ext/pytorch.py
--rw-r--r--   0 user      (1000) user      (1000)    25680 2023-04-12 08:41:14.000000 fickle-0.2.1/src/fickle/firewall.py
--rw-r--r--   0 user      (1000) user      (1000)     8353 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/unpickler.py
--rw-r--r--   0 user      (1000) user      (1000)      788 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/fickle.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3364 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      495 2023-04-12 08:41:22.000000 fickle-0.2.1/src/fickle.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        6 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      337 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)     1550 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/test_danger.py
--rw-r--r--   0 user      (1000) user      (1000)     1725 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/test_roundtrip.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:42:03.455730 fickle-0.2.2/
+-rw-r--r--   0 user      (1000) user      (1000)      637 2023-04-15 06:41:56.000000 fickle-0.2.2/CHANGELOG.md
+-rw-r--r--   0 user      (1000) user      (1000)       58 2023-04-12 08:45:32.000000 fickle-0.2.2/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3366 2023-04-15 06:42:03.455730 fickle-0.2.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2513 2023-04-15 06:41:56.000000 fickle-0.2.2/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-03-31 02:29:03.000000 fickle-0.2.2/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      105 2023-04-15 06:42:03.455730 fickle-0.2.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      726 2023-04-15 06:41:56.000000 fickle-0.2.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:42:03.445730 fickle-0.2.2/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:42:03.445730 fickle-0.2.2/src/fickle/
+-rw-r--r--   0 user      (1000) user      (1000)       92 2023-03-31 02:29:03.000000 fickle-0.2.2/src/fickle/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      189 2023-03-31 02:29:03.000000 fickle-0.2.2/src/fickle/exc.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:42:03.455730 fickle-0.2.2/src/fickle/ext/
+-rw-r--r--   0 user      (1000) user      (1000)      143 2023-03-31 02:29:03.000000 fickle-0.2.2/src/fickle/ext/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     6576 2023-03-31 02:29:03.000000 fickle-0.2.2/src/fickle/ext/marshmallow.py
+-rw-r--r--   0 user      (1000) user      (1000)     6950 2023-04-15 06:41:56.000000 fickle-0.2.2/src/fickle/ext/pytorch.py
+-rw-r--r--   0 user      (1000) user      (1000)    25680 2023-04-12 08:41:14.000000 fickle-0.2.2/src/fickle/firewall.py
+-rw-r--r--   0 user      (1000) user      (1000)     8353 2023-03-31 02:29:03.000000 fickle-0.2.2/src/fickle/unpickler.py
+-rw-r--r--   0 user      (1000) user      (1000)      788 2023-03-31 02:29:03.000000 fickle-0.2.2/src/fickle/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:42:03.455730 fickle-0.2.2/src/fickle.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3366 2023-04-15 06:42:02.000000 fickle-0.2.2/src/fickle.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      508 2023-04-15 06:42:03.000000 fickle-0.2.2/src/fickle.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-15 06:42:02.000000 fickle-0.2.2/src/fickle.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        6 2023-04-15 06:42:02.000000 fickle-0.2.2/src/fickle.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-04-15 06:42:02.000000 fickle-0.2.2/src/fickle.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-15 06:42:03.455730 fickle-0.2.2/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-31 02:29:03.000000 fickle-0.2.2/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      337 2023-03-31 02:29:03.000000 fickle-0.2.2/tests/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)     1550 2023-03-31 02:29:03.000000 fickle-0.2.2/tests/test_danger.py
+-rw-r--r--   0 user      (1000) user      (1000)     1725 2023-03-31 02:29:03.000000 fickle-0.2.2/tests/test_roundtrip.py
```

### Comparing `fickle-0.2.1/PKG-INFO` & `fickle-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fickle
-Version: 0.2.1
+Version: 0.2.2
 Summary: load pickled data as safely as possible
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # Fickle: Firewalled Pickle
         
         People abuse pickle. Especially researchers. Pickle is [not secure](https://docs.python.org/3/library/pickle.html). Published datasets and ML training weights are often distributed as pickle files (or formats which use pickle files, such as [PyTorch checkpoint.ckpt files](https://pytorch.org/tutorials/beginner/saving_loading_models.html)). Sometimes it is the only format that they are available in.
         
-        # Examples
+        ## Examples
         
         Loading basic types is easy:
         
         ```python
         >>> from fickle import DefaultFirewall
         >>> import pickle
         >>>
@@ -37,15 +37,15 @@
         >>> tensor.array
         array([0.39097363, 0.3898967 , 0.35191917, ..., 0.41924757, 0.4031702 ,
                0.37156993], dtype=float32)
         ```
         
         You can, optionally, even use `marshmallow` for validation!
         
-        # Alternatives
+        ## Alternatives
         
         - [picklemagic](https://github.com/CensoredUsername/picklemagic)
         - [pikara](https://pypi.org/project/pikara)
         
         |                                                | fickle | picklemagic | pikara |
         |------------------------------------------------|--------|-------------|--------|
         | Does not rely on `pickle._Unpickler`?          | ✅      | ❌           | ✅      |
```

### Comparing `fickle-0.2.1/README.md` & `fickle-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Fickle: Firewalled Pickle
 
 People abuse pickle. Especially researchers. Pickle is [not secure](https://docs.python.org/3/library/pickle.html). Published datasets and ML training weights are often distributed as pickle files (or formats which use pickle files, such as [PyTorch checkpoint.ckpt files](https://pytorch.org/tutorials/beginner/saving_loading_models.html)). Sometimes it is the only format that they are available in.
 
-# Examples
+## Examples
 
 Loading basic types is easy:
 
 ```python
 >>> from fickle import DefaultFirewall
 >>> import pickle
 >>>
@@ -29,15 +29,15 @@
 >>> tensor.array
 array([0.39097363, 0.3898967 , 0.35191917, ..., 0.41924757, 0.4031702 ,
        0.37156993], dtype=float32)
 ```
 
 You can, optionally, even use `marshmallow` for validation!
 
-# Alternatives
+## Alternatives
 
 - [picklemagic](https://github.com/CensoredUsername/picklemagic)
 - [pikara](https://pypi.org/project/pikara)
 
 |                                                | fickle | picklemagic | pikara |
 |------------------------------------------------|--------|-------------|--------|
 | Does not rely on `pickle._Unpickler`?          | ✅      | ❌           | ✅      |
```

### Comparing `fickle-0.2.1/setup.py` & `fickle-0.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text("utf-8")
 
 setup(
     name="fickle",
     description="load pickled data as safely as possible",
-    version="0.2.1",
+    version="0.2.2",
     author="Eduard Christian Dumitrescu",
     author_email="eduard.c.dumitrescu@gmail.com",
     install_requires=["attrs"],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     license="MIT",
     classifiers=[
```

### Comparing `fickle-0.2.1/src/fickle/ext/marshmallow.py` & `fickle-0.2.2/src/fickle/ext/marshmallow.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.1/src/fickle/ext/pytorch.py` & `fickle-0.2.2/src/fickle/ext/pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,23 @@
         contextvar.reset(token)
 
 
 class InvalidDTypeWarning(UserWarning):
     pass
 
 
+def trivial_strides_for_tensor_shape(shape: Tuple[int, ...]) -> Tuple[int, ...]:
+    reversed_strides = []
+    current = 1
+    for dim in shape[::-1]:
+        reversed_strides.append(current)
+        current *= dim if dim else 1
+    return tuple(reversed_strides[::-1])
+
+
 @dataclasses.dataclass
 class StoredTensor:
     storage: "StorageInfo"
     storage_offset: int
     size: Tuple[int]
     stride: Tuple[int]
     requires_grad: bool
@@ -61,14 +70,31 @@
     def numpy_dtype(self):
         dtype = self.storage.dtype
         if dtype not in self.PYTORCH_DTYPE_TO_ITEMSIZE:
             raise ValueError("invalid dtype: {dtype!r}")
 
         return np.dtype(dtype).newbyteorder("<")
 
+    @functools.cached_property
+    def has_trivial_layout(self) -> bool:
+        """
+        Does this tensor do any funny stride (i.e. memory layout) tricks?
+        """
+        if 0 in self.size:
+            return True  # Empty tensors have no memory, so there's no memory layout.
+
+        # If a dimension has length 1, the stride won't matter for it because the only
+        # valid index is 0.
+        return all(
+            dim == 1 or trivial_stride == actual_stride
+            for dim, actual_stride, trivial_stride in zip(
+                self.size, self.stride, trivial_strides_for_tensor_shape(self.size)
+            )
+        )
+
     @property
     def size_in_bytes(self) -> int:
         itemsize = self.PYTORCH_DTYPE_TO_ITEMSIZE[self.storage.dtype]
         return functools.reduce(operator.mul, self.size, itemsize)
 
     def _load_from_file(self, fileobj):
         byte_size = self.size_in_bytes
@@ -77,16 +103,19 @@
         if len(buf) != byte_size:
             raise ValueError(f"expected {len(buf)} bytes, got {byte_size}")
         return buf
 
     def _buffer_to_numpy(self, buffer):
         return np.frombuffer(buffer, self.numpy_dtype).reshape(self.size)
 
+    def open_storage(self):
+        return self.storage_manager.open(f"data/{self.storage.key}")
+
     def _load_from_zipfile(self):
-        with self.storage_manager.open(f"data/{self.storage.key}") as f:
+        with self.open_storage() as f:
             return self._load_from_file(f)
 
     @property
     def array(self):
         if self.numpy_dtype is None:
             raise ValueError(f"invalid dtype {self.storage.dtype!r}")
```

### Comparing `fickle-0.2.1/src/fickle/firewall.py` & `fickle-0.2.2/src/fickle/firewall.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.1/src/fickle/unpickler.py` & `fickle-0.2.2/src/fickle/unpickler.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.1/src/fickle/util.py` & `fickle-0.2.2/src/fickle/util.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.1/src/fickle.egg-info/PKG-INFO` & `fickle-0.2.2/src/fickle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fickle
-Version: 0.2.1
+Version: 0.2.2
 Summary: load pickled data as safely as possible
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # Fickle: Firewalled Pickle
         
         People abuse pickle. Especially researchers. Pickle is [not secure](https://docs.python.org/3/library/pickle.html). Published datasets and ML training weights are often distributed as pickle files (or formats which use pickle files, such as [PyTorch checkpoint.ckpt files](https://pytorch.org/tutorials/beginner/saving_loading_models.html)). Sometimes it is the only format that they are available in.
         
-        # Examples
+        ## Examples
         
         Loading basic types is easy:
         
         ```python
         >>> from fickle import DefaultFirewall
         >>> import pickle
         >>>
@@ -37,15 +37,15 @@
         >>> tensor.array
         array([0.39097363, 0.3898967 , 0.35191917, ..., 0.41924757, 0.4031702 ,
                0.37156993], dtype=float32)
         ```
         
         You can, optionally, even use `marshmallow` for validation!
         
-        # Alternatives
+        ## Alternatives
         
         - [picklemagic](https://github.com/CensoredUsername/picklemagic)
         - [pikara](https://pypi.org/project/pikara)
         
         |                                                | fickle | picklemagic | pikara |
         |------------------------------------------------|--------|-------------|--------|
         | Does not rely on `pickle._Unpickler`?          | ✅      | ❌           | ✅      |
```

### Comparing `fickle-0.2.1/tests/test_danger.py` & `fickle-0.2.2/tests/test_danger.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.1/tests/test_roundtrip.py` & `fickle-0.2.2/tests/test_roundtrip.py`

 * *Files identical despite different names*

