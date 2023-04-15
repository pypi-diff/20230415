# Comparing `tmp/arraymap-0.1.3.tar.gz` & `tmp/arraymap-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.3.tar", last modified: Fri Apr 14 17:57:47 2023, max compression
+gzip compressed data, was "arraymap-0.1.4.tar", last modified: Fri Apr 14 23:33:10 2023, max compression
```

## Comparing `arraymap-0.1.3.tar` & `arraymap-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:57:47.078973 arraymap-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 17:57:45.000000 arraymap-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:57:45.000000 arraymap-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-14 17:57:47.078973 arraymap-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 17:57:45.000000 arraymap-0.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    60830 2023-04-14 17:57:45.000000 arraymap-0.1.3/arraymap.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:57:47.074973 arraymap-0.1.3/arraymap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 17:57:47.078973 arraymap-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 17:57:45.000000 arraymap-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:57:47.078973 arraymap-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-14 17:57:45.000000 arraymap-0.1.3/test/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-04-14 17:57:45.000000 arraymap-0.1.3/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:33:10.091410 arraymap-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 23:33:05.000000 arraymap-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 23:33:05.000000 arraymap-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-14 23:33:10.091410 arraymap-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-14 23:33:05.000000 arraymap-0.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    60885 2023-04-14 23:33:05.000000 arraymap-0.1.4/arraymap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:33:10.091410 arraymap-0.1.4/arraymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-14 23:33:10.000000 arraymap-0.1.4/arraymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-14 23:33:10.000000 arraymap-0.1.4/arraymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:33:10.000000 arraymap-0.1.4/arraymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 23:33:10.000000 arraymap-0.1.4/arraymap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 23:33:10.000000 arraymap-0.1.4/arraymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 23:33:10.095410 arraymap-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 23:33:05.000000 arraymap-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:33:10.091410 arraymap-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-14 23:33:05.000000 arraymap-0.1.4/test/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-04-14 23:33:05.000000 arraymap-0.1.4/test/test_unit.py
```

### Comparing `arraymap-0.1.3/LICENSE.md` & `arraymap-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.3/PKG-INFO` & `arraymap-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -54,14 +54,20 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.4
+........
+
+Corrected comparison in lookup of Unicode elements.
+
+
 0.1.3
 ........
 
 Updated ``classifiers``, ``install_requires`` with ``setuptools``.
 
 
 0.1.2
```

### Comparing `arraymap-0.1.3/README.rst` & `arraymap-0.1.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.4
+........
+
+Corrected comparison in lookup of Unicode elements.
+
+
 0.1.3
 ........
 
 Updated ``classifiers``, ``install_requires`` with ``setuptools``.
 
 
 0.1.2
```

### Comparing `arraymap-0.1.3/arraymap.c` & `arraymap-0.1.4/arraymap.c`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 } TableElement;
 
 
 // Table configuration; experimentation shows that these values work well:
 # define LOAD 0.9
 # define SCAN 16
 
+const static size_t UCS4_SIZE = sizeof(Py_UCS4);
 
 typedef enum KeysArrayType{
     KAT_LIST = 0, // must be falsy
 
     KAT_INT8, // order matters as ranges of size are used in selection
     KAT_INT16,
     KAT_INT32,
@@ -786,16 +787,16 @@
 {
     TableElement *table = self->table;
     Py_ssize_t mask = self->table_size - 1;
     Py_hash_t mixin = Py_ABS(hash);
     Py_ssize_t table_pos = hash & mask;
 
     PyArrayObject *a = (PyArrayObject *)self->keys;
-    // REVIEW: is this a new descr reference?
-    Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / sizeof(Py_UCS4);
+    Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / UCS4_SIZE;
+    Py_ssize_t cmp_bytes = Py_MIN(key_size, dt_size) * UCS4_SIZE;
 
     Py_hash_t h = 0;
     Py_UCS4* p_start = NULL;
 
     while (1) {
         for (Py_ssize_t i = 0; i < SCAN; i++) {
             h = table[table_pos].hash;
@@ -804,15 +805,15 @@
             }
             if (h != hash) {
                 table_pos++;
                 continue;
             }
             p_start = (Py_UCS4*)PyArray_GETPTR1(a, table[table_pos].keys_pos);
             // memcmp returns 0 on match
-            if (!memcmp(p_start, key, Py_MIN(key_size, dt_size))) {
+            if (!memcmp(p_start, key, cmp_bytes)) {
                 return table_pos;
             }
             table_pos++;
         }
         table_pos = (5 * (table_pos - SCAN) + (mixin >>= 1) + 1) & mask;
     }
 }
@@ -829,14 +830,15 @@
     TableElement *table = self->table;
     Py_ssize_t mask = self->table_size - 1;
     Py_hash_t mixin = Py_ABS(hash);
     Py_ssize_t table_pos = hash & mask;
 
     PyArrayObject *a = (PyArrayObject *)self->keys;
     Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / sizeof(char);
+    Py_ssize_t cmp_bytes = Py_MIN(key_size, dt_size);
 
     Py_hash_t h = 0;
     char* p_start = NULL;
 
     while (1) {
         for (Py_ssize_t i = 0; i < SCAN; i++) {
             h = table[table_pos].hash;
@@ -845,15 +847,15 @@
             }
             if (h != hash) {
                 table_pos++;
                 continue;
             }
             p_start = (char*)PyArray_GETPTR1(a, table[table_pos].keys_pos);
             // memcmp returns 0 on match
-            if (!memcmp(p_start, key, Py_MIN(key_size, dt_size))) {
+            if (!memcmp(p_start, key, cmp_bytes)) {
                 return table_pos;
             }
             table_pos++;
         }
         table_pos = (5 * (table_pos - SCAN) + (mixin >>= 1) + 1) & mask;
     }
 }
@@ -1106,15 +1108,15 @@
 static Py_ssize_t
 lookup_unicode(FAMObject *self, PyObject* key) {
     // NOTE: while we can identify and use PyArray_IsScalar(key, Unicode), this did not improve performance and fails on Windows.
     if (!PyUnicode_Check(key)) {
         return -1;
     }
     PyArrayObject *a = (PyArrayObject *)self->keys;
-    Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / sizeof(Py_UCS4);
+    Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / UCS4_SIZE;
     // if the key_size is greater than the dtype size of the array, we know there cannot be a match
     Py_ssize_t k_size = PyUnicode_GetLength(key);
     if (k_size > dt_size) {
         return -1;
     }
     // The buffer will have dt_size + 1 storage. We copy a NULL character so do not have to clear the buffer, but instead can reuse it and still discover the lookup
     if (!PyUnicode_AsUCS4(key, self->key_buffer, dt_size+1, 1)) {
@@ -1431,16 +1433,16 @@
     new->table_size = self->table_size;
     new->keys_array_type = self->keys_array_type;
     new->keys_size = self->keys_size;
 
     new->key_buffer = NULL;
     if (new->keys_array_type == KAT_UNICODE) {
         PyArrayObject *a = (PyArrayObject *)new->keys;
-        Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / sizeof(Py_UCS4);
-        new->key_buffer = (Py_UCS4*)PyMem_Malloc((dt_size+1) * sizeof(Py_UCS4));
+        Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / UCS4_SIZE;
+        new->key_buffer = (Py_UCS4*)PyMem_Malloc((dt_size+1) * UCS4_SIZE);
     }
 
     Py_ssize_t table_size_alloc = new->table_size + SCAN - 1;
     new->table = PyMem_New(TableElement, table_size_alloc);
     if (!new->table) {
         // Py_DECREF(new->keys); // assume this will get cleaned up
         return -1;
@@ -1918,16 +1920,16 @@
                 INSERT_SCALARS(npy_float, insert_double,);
                 break;
             case KAT_FLOAT16:
                 INSERT_SCALARS(npy_half, insert_double, npy_half_to_double);
                 break;
             case KAT_UNICODE: {
                 // Over allocate buffer by 1 so there is room for null at end. This buffer is only used in lookup();
-                Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / sizeof(Py_UCS4);
-                fam->key_buffer = (Py_UCS4*)PyMem_Malloc((dt_size+1) * sizeof(Py_UCS4));
+                Py_ssize_t dt_size = PyArray_DESCR(a)->elsize / UCS4_SIZE;
+                fam->key_buffer = (Py_UCS4*)PyMem_Malloc((dt_size+1) * UCS4_SIZE);
                 INSERT_FLEXIBLE(Py_UCS4, insert_unicode, ucs4_get_end_p);
                 break;
             }
             case KAT_STRING: {
                 Py_ssize_t dt_size = PyArray_DESCR(a)->elsize;
                 INSERT_FLEXIBLE(char, insert_string, char_get_end_p);
                 break;
```

### Comparing `arraymap-0.1.3/arraymap.egg-info/PKG-INFO` & `arraymap-0.1.4/arraymap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -54,14 +54,20 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.4
+........
+
+Corrected comparison in lookup of Unicode elements.
+
+
 0.1.3
 ........
 
 Updated ``classifiers``, ``install_requires`` with ``setuptools``.
 
 
 0.1.2
```

### Comparing `arraymap-0.1.3/setup.py` & `arraymap-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import typing as tp
 import site
 import os
 
 
-AM_VERSION = "0.1.3"
+AM_VERSION = "0.1.4"
 
 
 with open("README.rst") as file:
     LONG_DESCRIPTION = file.read()
 
 
 def get_ext_dir(*components: tp.Iterable[str]) -> tp.Sequence[str]:
```

### Comparing `arraymap-0.1.3/test/test_property.py` & `arraymap-0.1.4/test/test_property.py`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.3/test/test_unit.py` & `arraymap-0.1.4/test/test_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,20 @@
     a1 = np.array(("a", "bb", "ccc"))
     a1.flags.writeable = False
     fam = FrozenAutoMap(a1)
     for k in a1:
         assert k in fam
 
 
+def test_fam_constructor_array_unicode_c():
+    a1 = np.array(("z0Ct", "z0DS", "z0E9"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+
 def test_fam_copy_array_unicode_a():
     a1 = np.array(("a", "ccc", "bb"))
     a1.flags.writeable = False
     fam1 = FrozenAutoMap(a1)
     fam2 = FrozenAutoMap(fam1)
     assert fam2["a"] == 0
     assert fam2["ccc"] == 1
```

