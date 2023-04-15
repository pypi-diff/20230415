# Comparing `tmp/salix-containers-0.3.0.tar.gz` & `tmp/salix-containers-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salix-containers-0.3.0.tar", max compression
+gzip compressed data, was "salix-containers-0.3.1.tar", max compression
```

## Comparing `salix-containers-0.3.0.tar` & `salix-containers-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      331 2023-04-15 16:50:32.069609 salix-containers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      129 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/__init__.py
--rw-r--r--   0        0        0      763 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/caselessmapping.py
--rw-r--r--   0        0        0     1617 2022-04-16 20:28:31.676860 salix-containers-0.3.0/salix_containers/casttypes.py
--rw-r--r--   0        0        0        0 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/tests/__init__.py
--rw-r--r--   0        0        0     1450 2023-04-15 16:49:10.619609 salix-containers-0.3.0/salix_containers/tests/test_caselessdict.py
--rw-r--r--   0        0        0      561 2023-04-15 16:51:54.696066 salix-containers-0.3.0/setup.py
--rw-r--r--   0        0        0      489 2023-04-15 16:51:54.696210 salix-containers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      331 2023-04-15 17:31:43.159609 salix-containers-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-04-15 17:31:03.289609 salix-containers-0.3.1/salix_containers/__init__.py
+-rw-r--r--   0        0        0     1039 2023-04-15 17:31:03.289609 salix-containers-0.3.1/salix_containers/caselessmapping.py
+-rw-r--r--   0        0        0     1617 2022-04-16 20:28:31.676860 salix-containers-0.3.1/salix_containers/casttypes.py
+-rw-r--r--   0        0        0        0 2023-04-15 16:49:10.619609 salix-containers-0.3.1/salix_containers/tests/__init__.py
+-rw-r--r--   0        0        0     3537 2023-04-15 17:31:03.289609 salix-containers-0.3.1/salix_containers/tests/test_caselessmappings.py
+-rw-r--r--   0        0        0      561 2023-04-15 17:32:56.424143 salix-containers-0.3.1/setup.py
+-rw-r--r--   0        0        0      489 2023-04-15 17:32:56.424292 salix-containers-0.3.1/PKG-INFO
```

### Comparing `salix-containers-0.3.0/salix_containers/caselessmapping.py` & `salix-containers-0.3.1/salix_containers/caselessmapping.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
-from collections.abc import Mapping
+from collections.abc import Mapping, MutableMapping
 
 
 class CaselessMapping(Mapping):
 
     def __init__(self, init):
-        if not isinstance(init, Mapping):
-            raise ValueError('init argument must be a mapping')
-        self._data = {self.norm_key(key): (key, value) for key, value in init.items()}
+        init_dict = dict(init)
+        self._data = {self.norm_key(key): (key, value) for key, value in init_dict.items()}
 
     @staticmethod
     def norm_key(key):
         if isinstance(key, str):
             return key.lower()
         else:
             return key
@@ -25,7 +24,19 @@
     def __iter__(self):
         for key in self._data.keys():
             yield self._data[key][0]
 
     def get_raw_key_name(self, key):
         return self._data[self.norm_key(key)][0]
 
+
+class CaselessMutableMapping(MutableMapping, CaselessMapping):
+
+    def __init__(self, init=None):
+        super().__init__(init if init is not None else {})
+
+    def __setitem__(self, key, value):
+        self._data[self.norm_key(key)] = (key, value)
+
+    def __delitem__(self, key):
+        del self._data[self.norm_key(key)]
+
```

### Comparing `salix-containers-0.3.0/salix_containers/casttypes.py` & `salix-containers-0.3.1/salix_containers/casttypes.py`

 * *Files identical despite different names*

### Comparing `salix-containers-0.3.0/salix_containers/tests/test_caselessdict.py` & `salix-containers-0.3.1/salix_containers/tests/test_caselessmappings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 from unittest import TestCase
 
-from caselessmapping import CaselessMapping
+from caselessmapping import CaselessMapping, CaselessMutableMapping
+
 
 class TestCaselessMapping(TestCase):
 
     def test_null_init(self):
         self.assertRaises(TypeError, CaselessMapping)
 
     def test_int_keys(self):
@@ -42,7 +43,75 @@
         test_tups = list(cd.items())
         self.assertListEqual(orig_tups, test_tups)
 
     def test_raw_name(self):
         data = {'a': 'A', 'B': 'B', 'c': 'C'}
         cd = CaselessMapping(data)
         self.assertEqual(cd.get_raw_key_name('b'), 'B')
+
+
+class TestCaselessMutableMapping(TestCase):
+
+    def test_null_init(self):
+        cd = CaselessMutableMapping()
+        self.assertEqual(cd, {})
+
+    def test_int_keys(self):
+        data = {1: 10, 2: 20, 3:30}
+        cd = CaselessMutableMapping(data)
+        self.assertEqual(cd, data)
+
+    def test_str_keys(self):
+        data = {'a': 'A', 'b': 'B', 'c': 'C'}
+        cd = CaselessMutableMapping(data)
+        self.assertEqual(cd, data)
+
+    def test_matching_case_retreive(self):
+        data = {'a': 'A', 'B': 'B', 'c': 'C'}
+        cd = CaselessMutableMapping(data)
+        self.assertEqual(cd['a'], data['a'])
+        self.assertEqual(cd['B'], data['B'])
+
+    def test_caseless_retreive(self):
+        data = {'a': 'A', 'B': 'B', 'c': 'C'}
+        cd = CaselessMutableMapping(data)
+        self.assertEqual(cd['A'], data['a'])
+        self.assertEqual(cd['b'], data['B'])
+
+    def test_len(self):
+        data = {'a': 'A', 'B': 'B', 'c': 'C'}
+        cd = CaselessMutableMapping(data)
+        self.assertEqual(len(cd), 3)
+
+    def test_iter(self):
+        data = {'a': 'A', 'B': 'B', 'c': 'C'}
+        cd = CaselessMutableMapping(data)
+        orig_tups = list(data.items())
+        test_tups = list(cd.items())
+        self.assertListEqual(orig_tups, test_tups)
+
+    def test_raw_name(self):
+        data = {'a': 'A', 'B': 'B', 'c': 'C'}
+        cd = CaselessMutableMapping(data)
+        self.assertEqual(cd.get_raw_key_name('b'), 'B')
+
+    def test_add_item_str_key(self):
+       cd = CaselessMutableMapping()
+       cd['x'] = 'X'
+       self.assertEqual(cd, {'x': 'X'})
+
+    def test_add_item_int_key(self):
+       cd = CaselessMutableMapping()
+       cd[1] = 'X'
+       self.assertEqual(cd, {1: 'X'})
+
+    def test_del_item_str_key(self):
+        data = {'x': 'X', 'y': 'Y'}
+        cd = CaselessMutableMapping(data)
+        del cd['x']
+        self.assertEqual(cd, {'y': 'Y'})
+
+    def test_del_item_int_key(self):
+        data = {1: 'X', 2: 'Y'}
+        cd = CaselessMutableMapping(data)
+        del cd[1]
+        self.assertEqual(cd, {2: 'Y'})
```

### Comparing `salix-containers-0.3.0/setup.py` & `salix-containers-0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['salix_containers', 'salix_containers.tests']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'salix-containers',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Occasionally handy container types',
     'long_description': None,
     'author': 'Salix',
     'author_email': 'salix@pilae.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

