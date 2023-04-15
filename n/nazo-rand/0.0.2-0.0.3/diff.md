# Comparing `tmp/nazo_rand-0.0.2.tar.gz` & `tmp/nazo_rand-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_rand-0.0.2.tar", last modified: Sat Apr 15 15:04:30 2023, max compression
+gzip compressed data, was "nazo_rand-0.0.3.tar", last modified: Sat Apr 15 15:14:13 2023, max compression
```

## Comparing `nazo_rand-0.0.2.tar` & `nazo_rand-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:04:30.312901 nazo_rand-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-15 15:04:30.312901 nazo_rand-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:04:30.312901 nazo_rand-0.0.2/nazo_rand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-15 15:04:30.000000 nazo_rand-0.0.2/nazo_rand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-15 15:04:30.000000 nazo_rand-0.0.2/nazo_rand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:04:30.000000 nazo_rand-0.0.2/nazo_rand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 15:04:30.000000 nazo_rand-0.0.2/nazo_rand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:04:30.312901 nazo_rand-0.0.2/rand/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/rand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   204266 2023-04-15 15:04:15.000000 nazo_rand-0.0.2/rand/nazo_rand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/rand/nazo_rand.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/rand/nazo_rand.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/rand/nazo_rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/rand/nazo_rand.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:04:30.312901 nazo_rand-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 15:03:58.000000 nazo_rand-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/nazo_rand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/rand/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204018 2023-04-15 15:14:03.000000 nazo_rand-0.0.3/rand/nazo_rand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/setup.py
```

### Comparing `nazo_rand-0.0.2/LICENSE` & `nazo_rand-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.2/PKG-INFO` & `nazo_rand-0.0.3/nazo_rand.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nazo_rand
-Version: 0.0.2
+Name: nazo-rand
+Version: 0.0.3
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nazo_rand-0.0.2/README.md` & `nazo_rand-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.2/nazo_rand.egg-info/PKG-INFO` & `nazo_rand-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nazo-rand
-Version: 0.0.2
+Name: nazo_rand
+Version: 0.0.3
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nazo_rand-0.0.2/rand/nazo_rand.cpp` & `nazo_rand-0.0.3/rand/nazo_rand.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -991,27 +991,18 @@
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "rand/nazo_rand.pyx",
 };
 
-/* "rand/nazo_rand.pxd":6
- * 
- * #cpdef void seed(int rseed = ?)
- * ctypedef int64_t Integer             # <<<<<<<<<<<<<<
- * cpdef void shuffle(list array)
- * cpdef int random_integer_noargs()
- */
-typedef int64_t __pyx_t_4rand_9nazo_rand_Integer;
-
 /*--- Type declarations ---*/
 struct __pyx_opt_args_4rand_9nazo_rand_randrange;
 
-/* "rand/nazo_rand.pxd":12
+/* "rand/nazo_rand.pxd":10
  * cpdef int randbelow(int a)
  * cpdef int randint(int a,int b)
  * cpdef int randrange(int start,int stop=?,int step=?)             # <<<<<<<<<<<<<<
  * cpdef double random_double(double a, double b)
  * cpdef double random_double_noargs()
  */
 struct __pyx_opt_args_4rand_9nazo_rand_randrange {
@@ -1336,18 +1327,18 @@
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
-/* Module declarations from 'libc.stdint' */
-
 /* Module declarations from 'cython' */
 
+/* Module declarations from 'libc.stdint' */
+
 /* Module declarations from 'rand.nazo_rand' */
 static void __pyx_f_4rand_9nazo_rand_shuffle(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_4rand_9nazo_rand_random_integer_noargs(int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_4rand_9nazo_rand_random_choice(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_4rand_9nazo_rand_randbelow(int, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_4rand_9nazo_rand_randint(int, int, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_4rand_9nazo_rand_randrange(int, int __pyx_skip_dispatch, struct __pyx_opt_args_4rand_9nazo_rand_randrange *__pyx_optional_args); /*proto*/
@@ -1426,39 +1417,39 @@
 static PyObject *__pyx_codeobj__7;
 static PyObject *__pyx_codeobj__9;
 static PyObject *__pyx_codeobj__11;
 static PyObject *__pyx_codeobj__13;
 static PyObject *__pyx_codeobj__14;
 /* Late includes */
 
-/* "rand/nazo_rand.pyx":16
+/* "rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
 
 static PyObject *__pyx_pw_4rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static int __pyx_f_4rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
 
-  /* "rand/nazo_rand.pyx":17
+  /* "rand/nazo_rand.pyx":16
  * 
  * cpdef int random_integer_noargs():
  *     return uniform_int_variate_noargs()             # <<<<<<<<<<<<<<
  * 
  * cpdef void shuffle(list array):
  */
   __pyx_r = Storm::uniform_int_variate_noargs();
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":16
+  /* "rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
 
@@ -1487,15 +1478,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_random_integer_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_random_integer_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1504,15 +1495,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":19
+/* "rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
 
@@ -1529,81 +1520,81 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
 
-  /* "rand/nazo_rand.pyx":20
+  /* "rand/nazo_rand.pyx":19
  * 
  * cpdef void shuffle(list array):
  *     for i in reversed(range(len(array) - 1)):             # <<<<<<<<<<<<<<
  *         j = randrange(i, len(array), 1)
  *         array[i], array[j] = array[j], array[i]
  */
   if (unlikely(__pyx_v_array == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 20, __pyx_L1_error)
+    __PYX_ERR(0, 19, __pyx_L1_error)
   }
-  __pyx_t_1 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_1 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 19, __pyx_L1_error)
   for (__pyx_t_2 = (__pyx_t_1 - 1)-1; __pyx_t_2 >= 0; __pyx_t_2-=1) {
     __pyx_v_i = __pyx_t_2;
 
-    /* "rand/nazo_rand.pyx":21
+    /* "rand/nazo_rand.pyx":20
  * cpdef void shuffle(list array):
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)             # <<<<<<<<<<<<<<
  *         array[i], array[j] = array[j], array[i]
  * 
  */
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 21, __pyx_L1_error)
+      __PYX_ERR(0, 20, __pyx_L1_error)
     }
-    __pyx_t_3 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 20, __pyx_L1_error)
     __pyx_t_5.__pyx_n = 2;
     __pyx_t_5.stop = __pyx_t_3;
     __pyx_t_5.step = 1;
     __pyx_t_4 = __pyx_f_4rand_9nazo_rand_randrange(__pyx_v_i, 0, &__pyx_t_5); 
     __pyx_v_j = __pyx_t_4;
 
-    /* "rand/nazo_rand.pyx":22
+    /* "rand/nazo_rand.pyx":21
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  *         array[i], array[j] = array[j], array[i]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 22, __pyx_L1_error)
+      __PYX_ERR(0, 21, __pyx_L1_error)
     }
     __pyx_t_6 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_j);
     __Pyx_INCREF(__pyx_t_6);
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 22, __pyx_L1_error)
+      __PYX_ERR(0, 21, __pyx_L1_error)
     }
     __pyx_t_7 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_7);
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 22, __pyx_L1_error)
+      __PYX_ERR(0, 21, __pyx_L1_error)
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_6, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 22, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_6, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 22, __pyx_L1_error)
+      __PYX_ERR(0, 21, __pyx_L1_error)
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_j, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 22, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_j, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
 
-  /* "rand/nazo_rand.pyx":19
+  /* "rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
 
@@ -1623,15 +1614,15 @@
 static PyObject *__pyx_pw_4rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shuffle (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), (&PyList_Type), 1, "array", 1))) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), (&PyList_Type), 1, "array", 1))) __PYX_ERR(0, 18, __pyx_L1_error)
   __pyx_r = __pyx_pf_4rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject*)__pyx_v_array));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -1644,15 +1635,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4rand_9nazo_rand_shuffle(__pyx_v_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4rand_9nazo_rand_shuffle(__pyx_v_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1661,39 +1652,39 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":25
+/* "rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
 static PyObject *__pyx_pw_4rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a); /*proto*/
 static int __pyx_f_4rand_9nazo_rand_randbelow(int __pyx_v_a, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randbelow", 0);
 
-  /* "rand/nazo_rand.pyx":26
+  /* "rand/nazo_rand.pyx":25
  * 
  * cpdef int randbelow(int a):
  *     return random_below(a)             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __pyx_r = Storm::random_below(__pyx_v_a);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":25
+  /* "rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
@@ -1711,15 +1702,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randbelow (wrapper)", 0);
   assert(__pyx_arg_a); {
-    __pyx_v_a = __Pyx_PyInt_As_int(__pyx_arg_a); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyInt_As_int(__pyx_arg_a); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("rand.nazo_rand.randbelow", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -1735,15 +1726,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randbelow", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_randbelow(__pyx_v_a, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_randbelow(__pyx_v_a, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1752,15 +1743,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":30
+/* "rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
 
@@ -1772,39 +1763,39 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
 
-  /* "rand/nazo_rand.pyx":31
+  /* "rand/nazo_rand.pyx":30
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):
  *     cdef Py_ssize_t index = randbelow(len(elements))             # <<<<<<<<<<<<<<
  *     return elements[index]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_elements); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_elements); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 30, __pyx_L1_error)
   __pyx_v_index = __pyx_f_4rand_9nazo_rand_randbelow(__pyx_t_1, 0);
 
-  /* "rand/nazo_rand.pyx":32
+  /* "rand/nazo_rand.pyx":31
  * cpdef object random_choice(object elements):
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_elements, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_elements, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":30
+  /* "rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
 
@@ -1838,15 +1829,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_4rand_9nazo_rand_random_choice(__pyx_v_elements, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4rand_9nazo_rand_random_choice(__pyx_v_elements, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1855,39 +1846,39 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":35
+/* "rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
 
 static PyObject *__pyx_pw_4rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_f_4rand_9nazo_rand_randint(int __pyx_v_a, int __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randint", 0);
 
-  /* "rand/nazo_rand.pyx":36
+  /* "rand/nazo_rand.pyx":35
  * 
  * cpdef int randint(int a, int b):
  *     return uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  */
   __pyx_r = Storm::uniform_int_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":35
+  /* "rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
 
@@ -1928,32 +1919,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 35, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 34, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 35, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 34, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 35, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_b == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 35, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_b == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 35, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 34, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4rand_9nazo_rand_8randint(__pyx_self, __pyx_v_a, __pyx_v_b);
 
@@ -1967,15 +1958,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randint", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_randint(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_randint(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1984,15 +1975,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":38
+/* "rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2011,56 +2002,56 @@
       __pyx_v_stop = __pyx_optional_args->stop;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_step = __pyx_optional_args->step;
       }
     }
   }
 
-  /* "rand/nazo_rand.pyx":39
+  /* "rand/nazo_rand.pyx":38
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   __pyx_t_1 = ((__pyx_v_stop == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "rand/nazo_rand.pyx":40
+    /* "rand/nazo_rand.pyx":39
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:
  *         stop, start = start, 0             # <<<<<<<<<<<<<<
  *     return random_range(start, stop, step)
  * 
  */
     __pyx_t_2 = __pyx_v_start;
     __pyx_t_3 = 0;
     __pyx_v_stop = __pyx_t_2;
     __pyx_v_start = __pyx_t_3;
 
-    /* "rand/nazo_rand.pyx":39
+    /* "rand/nazo_rand.pyx":38
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   }
 
-  /* "rand/nazo_rand.pyx":41
+  /* "rand/nazo_rand.pyx":40
  *     if stop == 0:
  *         stop, start = start, 0
  *     return random_range(start, stop, step)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::random_range(__pyx_v_start, __pyx_v_stop, __pyx_v_step);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":38
+  /* "rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2114,42 +2105,42 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_step);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 38, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 37, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L3_error)
+      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 37, __pyx_L3_error)
     } else {
       __pyx_v_stop = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L3_error)
+      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 37, __pyx_L3_error)
     } else {
       __pyx_v_step = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 38, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4rand_9nazo_rand_10randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
 
@@ -2169,15 +2160,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randrange", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.stop = __pyx_v_stop;
   __pyx_t_2.step = __pyx_v_step;
   __pyx_t_1 = __pyx_f_4rand_9nazo_rand_randrange(__pyx_v_start, 0, &__pyx_t_2); 
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2186,39 +2177,39 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":44
+/* "rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
 static PyObject *__pyx_pw_4rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static double __pyx_f_4rand_9nazo_rand_random_double(double __pyx_v_a, double __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double", 0);
 
-  /* "rand/nazo_rand.pyx":45
+  /* "rand/nazo_rand.pyx":44
  * 
  * cpdef double random_double(double a, double b):
  *     return uniform_real_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::uniform_real_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":44
+  /* "rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
@@ -2259,32 +2250,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 44, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 43, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 44, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 43, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
-    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
+    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 44, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 43, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4rand_9nazo_rand_12random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
 
@@ -2298,15 +2289,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_4rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_4rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2315,36 +2306,36 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":48
+/* "rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
 static PyObject *__pyx_pw_4rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static double __pyx_f_4rand_9nazo_rand_random_double_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
 
-  /* "rand/nazo_rand.pyx":49
+  /* "rand/nazo_rand.pyx":48
  * 
  * cpdef double random_double_noargs():
  *     return uniform_real_variate_noargs()             # <<<<<<<<<<<<<<
  */
   __pyx_r = Storm::uniform_real_variate_noargs();
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":48
+  /* "rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
   /* function exit code */
@@ -2372,15 +2363,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_4rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_4rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2461,113 +2452,113 @@
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 20, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 19, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "rand/nazo_rand.pyx":16
+  /* "rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 15, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":19
+  /* "rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":25
+  /* "rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_a); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_a); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 25, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":30
+  /* "rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_s_elements); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_s_elements); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 29, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":35
+  /* "rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randint, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randint, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 34, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":38
+  /* "rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randrange, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randrange, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 37, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":44
+  /* "rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_double, 44, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_double, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 43, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":48
+  /* "rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2852,107 +2843,107 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "rand/nazo_rand.pyx":16
+  /* "rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":19
+  /* "rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":25
+  /* "rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":30
+  /* "rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_7random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_7random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":35
+  /* "rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_9randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_9randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":38
+  /* "rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_11randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_11randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":44
+  /* "rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_13random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_13random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":48
+  /* "rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_15random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_15random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "rand/nazo_rand.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * cimport cython
  */
```

### Comparing `nazo_rand-0.0.2/rand/nazo_rand.hpp` & `nazo_rand-0.0.3/rand/nazo_rand.hpp`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.2/rand/nazo_rand.pyi` & `nazo_rand-0.0.3/rand/nazo_rand.pyi`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.2/rand/nazo_rand.pyx` & `nazo_rand-0.0.3/rand/nazo_rand.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # cython: language_level=3
 # distutils: language = c++
 cimport cython
 from libc.stdint cimport int64_t, uint64_t
 
 cdef extern from "nazo_rand.hpp" namespace "Storm":
-    ctypedef int64_t Integer
     void seed(uint64_t seed)
-    Integer uniform_int_variate_noargs()
-    Integer random_range(Integer start, Integer stop, Integer step)
-    Integer random_below(Integer number)
-    Integer uniform_int_variate(Integer a, Integer b)
+    int64_t uniform_int_variate_noargs()
+    int64_t random_range(int64_t start, int64_t stop, int64_t step)
+    int64_t random_below(int64_t number)
+    int64_t uniform_int_variate(int64_t a, int64_t b)
     double uniform_real_variate_noargs()
     double uniform_real_variate(double a, double b)
 
 cpdef int random_integer_noargs():
     return uniform_int_variate_noargs()
 
 cpdef void shuffle(list array):
```

### Comparing `nazo_rand-0.0.2/setup.py` & `nazo_rand-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "wraparound": False,
             "binding": True,
             "cdivision": True,
         },
     ),
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.0.2",
+    version="0.0.3",
     description="A fast random number generator for python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="Free for non-commercial use",
     package_data={
         "": [
             "rand/nazo_rand.pyi",
```

