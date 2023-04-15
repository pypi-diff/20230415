# Comparing `tmp/nazo_rand-0.0.3.tar.gz` & `tmp/nazo_rand-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_rand-0.0.3.tar", last modified: Sat Apr 15 15:14:13 2023, max compression
+gzip compressed data, was "nazo_rand-0.0.5.tar", last modified: Sat Apr 15 15:37:14 2023, max compression
```

## Comparing `nazo_rand-0.0.3.tar` & `nazo_rand-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/nazo_rand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 15:14:13.000000 nazo_rand-0.0.3/nazo_rand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/rand/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   204018 2023-04-15 15:14:03.000000 nazo_rand-0.0.3/rand/nazo_rand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/rand/nazo_rand.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:14:13.815291 nazo_rand-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 15:13:49.000000 nazo_rand-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/nazo_rand/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   205123 2023-04-15 15:37:04.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/nazo_rand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/setup.py
```

### Comparing `nazo_rand-0.0.3/LICENSE` & `nazo_rand-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.3/PKG-INFO` & `nazo_rand-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nazo_rand
-Version: 0.0.3
+Version: 0.0.5
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# rand_int
+# nazo_rand
 
 Inspired to write from [Pyewacket](https://github.com/BrokenShell/Pyewacket)
 
 A fast random number generator for python
 
 `rand_int.choice(seq: list|Tuple) -> Any`
 example：
```

### Comparing `nazo_rand-0.0.3/README.md` & `nazo_rand-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# rand_int
+# nazo_rand
 
 Inspired to write from [Pyewacket](https://github.com/BrokenShell/Pyewacket)
 
 A fast random number generator for python
 
 `rand_int.choice(seq: list|Tuple) -> Any`
 example：
```

### Comparing `nazo_rand-0.0.3/nazo_rand.egg-info/PKG-INFO` & `nazo_rand-0.0.5/nazo_rand.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nazo-rand
-Version: 0.0.3
+Version: 0.0.5
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# rand_int
+# nazo_rand
 
 Inspired to write from [Pyewacket](https://github.com/BrokenShell/Pyewacket)
 
 A fast random number generator for python
 
 `rand_int.choice(seq: list|Tuple) -> Any`
 example：
```

### Comparing `nazo_rand-0.0.3/rand/nazo_rand.cpp` & `nazo_rand-0.0.5/nazo_rand/nazo_rand.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "rand/nazo_rand.hpp"
+            "nazo_rand/nazo_rand.hpp"
         ],
         "extra_compile_args": [
             "-std=c++17",
             "-O3"
         ],
         "extra_link_args": [
             "-O3"
         ],
         "include_dirs": [
-            "rand"
+            "nazo_rand"
         ],
         "language": "c++",
-        "name": "rand.nazo_rand",
+        "name": "nazo_rand.nazo_rand",
         "sources": [
-            "rand/nazo_rand.pyx"
+            "nazo_rand/nazo_rand.pyx"
         ]
     },
-    "module_name": "rand.nazo_rand"
+    "module_name": "nazo_rand.nazo_rand"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
@@ -774,16 +774,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__rand__nazo_rand
-#define __PYX_HAVE_API__rand__nazo_rand
+#define __PYX_HAVE__nazo_rand__nazo_rand
+#define __PYX_HAVE_API__nazo_rand__nazo_rand
 /* Early includes */
 #include <stdint.h>
 #include "nazo_rand.hpp"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
@@ -988,28 +988,28 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "rand/nazo_rand.pyx",
+  "nazo_rand/nazo_rand.pyx",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_opt_args_4rand_9nazo_rand_randrange;
+struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange;
 
-/* "rand/nazo_rand.pxd":10
+/* "nazo_rand/nazo_rand.pxd":10
  * cpdef int randbelow(int a)
  * cpdef int randint(int a,int b)
  * cpdef int randrange(int start,int stop=?,int step=?)             # <<<<<<<<<<<<<<
  * cpdef double random_double(double a, double b)
  * cpdef double random_double_noargs()
  */
-struct __pyx_opt_args_4rand_9nazo_rand_randrange {
+struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange {
   int __pyx_n;
   int stop;
   int step;
 };
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
@@ -1331,28 +1331,28 @@
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'libc.stdint' */
 
-/* Module declarations from 'rand.nazo_rand' */
-static void __pyx_f_4rand_9nazo_rand_shuffle(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_random_integer_noargs(int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_4rand_9nazo_rand_random_choice(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_randbelow(int, int __pyx_skip_dispatch); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_randint(int, int, int __pyx_skip_dispatch); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_randrange(int, int __pyx_skip_dispatch, struct __pyx_opt_args_4rand_9nazo_rand_randrange *__pyx_optional_args); /*proto*/
-static double __pyx_f_4rand_9nazo_rand_random_double(double, double, int __pyx_skip_dispatch); /*proto*/
-static double __pyx_f_4rand_9nazo_rand_random_double_noargs(int __pyx_skip_dispatch); /*proto*/
-#define __Pyx_MODULE_NAME "rand.nazo_rand"
-extern int __pyx_module_is_main_rand__nazo_rand;
-int __pyx_module_is_main_rand__nazo_rand = 0;
+/* Module declarations from 'nazo_rand.nazo_rand' */
+static void __pyx_f_9nazo_rand_9nazo_rand_shuffle(PyObject *, int __pyx_skip_dispatch); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *, int __pyx_skip_dispatch); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_randbelow(int, int __pyx_skip_dispatch); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_randint(int, int, int __pyx_skip_dispatch); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_randrange(int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args); /*proto*/
+static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double, double, int __pyx_skip_dispatch); /*proto*/
+static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(int __pyx_skip_dispatch); /*proto*/
+#define __Pyx_MODULE_NAME "nazo_rand.nazo_rand"
+extern int __pyx_module_is_main_nazo_rand__nazo_rand;
+int __pyx_module_is_main_nazo_rand__nazo_rand = 0;
 
-/* Implementation of 'rand.nazo_rand' */
+/* Implementation of 'nazo_rand.nazo_rand' */
 static PyObject *__pyx_builtin_reversed;
 static PyObject *__pyx_builtin_range;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_step[] = "step";
@@ -1365,50 +1365,50 @@
 static const char __pyx_k_shuffle[] = "shuffle";
 static const char __pyx_k_elements[] = "elements";
 static const char __pyx_k_reversed[] = "reversed";
 static const char __pyx_k_randbelow[] = "randbelow";
 static const char __pyx_k_randrange[] = "randrange";
 static const char __pyx_k_random_choice[] = "random_choice";
 static const char __pyx_k_random_double[] = "random_double";
-static const char __pyx_k_rand_nazo_rand[] = "rand.nazo_rand";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_rand_nazo_rand_pyx[] = "rand/nazo_rand.pyx";
+static const char __pyx_k_nazo_rand_nazo_rand[] = "nazo_rand.nazo_rand";
 static const char __pyx_k_random_double_noargs[] = "random_double_noargs";
 static const char __pyx_k_random_integer_noargs[] = "random_integer_noargs";
+static const char __pyx_k_nazo_rand_nazo_rand_pyx[] = "nazo_rand/nazo_rand.pyx";
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_b;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_elements;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_rand_nazo_rand;
-static PyObject *__pyx_kp_s_rand_nazo_rand_pyx;
+static PyObject *__pyx_n_s_nazo_rand_nazo_rand;
+static PyObject *__pyx_kp_s_nazo_rand_nazo_rand_pyx;
 static PyObject *__pyx_n_s_randbelow;
 static PyObject *__pyx_n_s_randint;
 static PyObject *__pyx_n_s_random_choice;
 static PyObject *__pyx_n_s_random_double;
 static PyObject *__pyx_n_s_random_double_noargs;
 static PyObject *__pyx_n_s_random_integer_noargs;
 static PyObject *__pyx_n_s_randrange;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reversed;
 static PyObject *__pyx_n_s_shuffle;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_pf_4rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_4rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array); /* proto */
-static PyObject *__pyx_pf_4rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a); /* proto */
-static PyObject *__pyx_pf_4rand_9nazo_rand_6random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_elements); /* proto */
-static PyObject *__pyx_pf_4rand_9nazo_rand_8randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b); /* proto */
-static PyObject *__pyx_pf_4rand_9nazo_rand_10randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step); /* proto */
-static PyObject *__pyx_pf_4rand_9nazo_rand_12random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b); /* proto */
-static PyObject *__pyx_pf_4rand_9nazo_rand_14random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_elements); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_8randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_10randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_12random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_14random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_codeobj_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__12;
@@ -1417,151 +1417,151 @@
 static PyObject *__pyx_codeobj__7;
 static PyObject *__pyx_codeobj__9;
 static PyObject *__pyx_codeobj__11;
 static PyObject *__pyx_codeobj__13;
 static PyObject *__pyx_codeobj__14;
 /* Late includes */
 
-/* "rand/nazo_rand.pyx":15
+/* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
 
-  /* "rand/nazo_rand.pyx":16
+  /* "nazo_rand/nazo_rand.pyx":16
  * 
  * cpdef int random_integer_noargs():
  *     return uniform_int_variate_noargs()             # <<<<<<<<<<<<<<
  * 
  * cpdef void shuffle(list array):
  */
   __pyx_r = Storm::uniform_int_variate_noargs();
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":15
+  /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_1random_integer_noargs = {"random_integer_noargs", (PyCFunction)__pyx_pw_4rand_9nazo_rand_1random_integer_noargs, METH_NOARGS, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_1random_integer_noargs = {"random_integer_noargs", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_1random_integer_noargs, METH_NOARGS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_integer_noargs (wrapper)", 0);
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_random_integer_noargs(__pyx_self);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_random_integer_noargs(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_random_integer_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rand.nazo_rand.random_integer_noargs", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_integer_noargs", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":18
+/* "nazo_rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
-static void __pyx_f_4rand_9nazo_rand_shuffle(PyObject *__pyx_v_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
+static void __pyx_f_9nazo_rand_9nazo_rand_shuffle(PyObject *__pyx_v_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
   Py_ssize_t __pyx_v_i;
   int __pyx_v_j;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
-  struct __pyx_opt_args_4rand_9nazo_rand_randrange __pyx_t_5;
+  struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
 
-  /* "rand/nazo_rand.pyx":19
+  /* "nazo_rand/nazo_rand.pyx":19
  * 
  * cpdef void shuffle(list array):
  *     for i in reversed(range(len(array) - 1)):             # <<<<<<<<<<<<<<
  *         j = randrange(i, len(array), 1)
  *         array[i], array[j] = array[j], array[i]
  */
   if (unlikely(__pyx_v_array == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(0, 19, __pyx_L1_error)
   }
   __pyx_t_1 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 19, __pyx_L1_error)
   for (__pyx_t_2 = (__pyx_t_1 - 1)-1; __pyx_t_2 >= 0; __pyx_t_2-=1) {
     __pyx_v_i = __pyx_t_2;
 
-    /* "rand/nazo_rand.pyx":20
+    /* "nazo_rand/nazo_rand.pyx":20
  * cpdef void shuffle(list array):
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)             # <<<<<<<<<<<<<<
  *         array[i], array[j] = array[j], array[i]
  * 
  */
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
       __PYX_ERR(0, 20, __pyx_L1_error)
     }
     __pyx_t_3 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 20, __pyx_L1_error)
     __pyx_t_5.__pyx_n = 2;
     __pyx_t_5.stop = __pyx_t_3;
     __pyx_t_5.step = 1;
-    __pyx_t_4 = __pyx_f_4rand_9nazo_rand_randrange(__pyx_v_i, 0, &__pyx_t_5); 
+    __pyx_t_4 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_i, 0, &__pyx_t_5); 
     __pyx_v_j = __pyx_t_4;
 
-    /* "rand/nazo_rand.pyx":21
+    /* "nazo_rand/nazo_rand.pyx":21
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  *         array[i], array[j] = array[j], array[i]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     if (unlikely(__pyx_v_array == Py_None)) {
@@ -1586,316 +1586,316 @@
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 21, __pyx_L1_error)
     }
     if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_j, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
 
-  /* "rand/nazo_rand.pyx":18
+  /* "nazo_rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_WriteUnraisable("rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("nazo_rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_3shuffle = {"shuffle", (PyCFunction)__pyx_pw_4rand_9nazo_rand_3shuffle, METH_O, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_3shuffle = {"shuffle", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_3shuffle, METH_O, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shuffle (wrapper)", 0);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), (&PyList_Type), 1, "array", 1))) __PYX_ERR(0, 18, __pyx_L1_error)
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject*)__pyx_v_array));
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject*)__pyx_v_array));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4rand_9nazo_rand_shuffle(__pyx_v_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_9nazo_rand_9nazo_rand_shuffle(__pyx_v_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":24
+/* "nazo_rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_randbelow(int __pyx_v_a, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_randbelow(int __pyx_v_a, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randbelow", 0);
 
-  /* "rand/nazo_rand.pyx":25
+  /* "nazo_rand/nazo_rand.pyx":25
  * 
  * cpdef int randbelow(int a):
  *     return random_below(a)             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __pyx_r = Storm::random_below(__pyx_v_a);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":24
+  /* "nazo_rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_5randbelow = {"randbelow", (PyCFunction)__pyx_pw_4rand_9nazo_rand_5randbelow, METH_O, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_5randbelow = {"randbelow", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_5randbelow, METH_O, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a) {
   int __pyx_v_a;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randbelow (wrapper)", 0);
   assert(__pyx_arg_a); {
     __pyx_v_a = __Pyx_PyInt_As_int(__pyx_arg_a); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rand.nazo_rand.randbelow", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randbelow", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_4randbelow(__pyx_self, ((int)__pyx_v_a));
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_4randbelow(__pyx_self, ((int)__pyx_v_a));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randbelow", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_randbelow(__pyx_v_a, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_randbelow(__pyx_v_a, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rand.nazo_rand.randbelow", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randbelow", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":29
+/* "nazo_rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements); /*proto*/
-static PyObject *__pyx_f_4rand_9nazo_rand_random_choice(PyObject *__pyx_v_elements, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements); /*proto*/
+static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *__pyx_v_elements, CYTHON_UNUSED int __pyx_skip_dispatch) {
   Py_ssize_t __pyx_v_index;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
 
-  /* "rand/nazo_rand.pyx":30
+  /* "nazo_rand/nazo_rand.pyx":30
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):
  *     cdef Py_ssize_t index = randbelow(len(elements))             # <<<<<<<<<<<<<<
  *     return elements[index]
  * 
  */
   __pyx_t_1 = PyObject_Length(__pyx_v_elements); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_v_index = __pyx_f_4rand_9nazo_rand_randbelow(__pyx_t_1, 0);
+  __pyx_v_index = __pyx_f_9nazo_rand_9nazo_rand_randbelow(__pyx_t_1, 0);
 
-  /* "rand/nazo_rand.pyx":31
+  /* "nazo_rand/nazo_rand.pyx":31
  * cpdef object random_choice(object elements):
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_elements, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":29
+  /* "nazo_rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("rand.nazo_rand.random_choice", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_7random_choice = {"random_choice", (PyCFunction)__pyx_pw_4rand_9nazo_rand_7random_choice, METH_O, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_7random_choice = {"random_choice", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_7random_choice, METH_O, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_choice (wrapper)", 0);
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_6random_choice(__pyx_self, ((PyObject *)__pyx_v_elements));
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_6random_choice(__pyx_self, ((PyObject *)__pyx_v_elements));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_6random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_elements) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_elements) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_4rand_9nazo_rand_random_choice(__pyx_v_elements, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_elements, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rand.nazo_rand.random_choice", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":34
+/* "nazo_rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_randint(int __pyx_v_a, int __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_randint(int __pyx_v_a, int __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randint", 0);
 
-  /* "rand/nazo_rand.pyx":35
+  /* "nazo_rand/nazo_rand.pyx":35
  * 
  * cpdef int randint(int a, int b):
  *     return uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  */
   __pyx_r = Storm::uniform_int_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_9randint = {"randint", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4rand_9nazo_rand_9randint, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_9randint = {"randint", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_9randint, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_a;
   int __pyx_v_b;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -1938,61 +1938,61 @@
     __pyx_v_a = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
     __pyx_v_b = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_b == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 34, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_8randint(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_8randint(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_8randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_8randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randint", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4rand_9nazo_rand_randint(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_randint(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":37
+/* "nazo_rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_f_4rand_9nazo_rand_randrange(int __pyx_v_start, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_4rand_9nazo_rand_randrange *__pyx_optional_args) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_randrange(int __pyx_v_start, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args) {
   int __pyx_v_stop = ((int)0);
   int __pyx_v_step = ((int)1);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -2002,73 +2002,73 @@
       __pyx_v_stop = __pyx_optional_args->stop;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_step = __pyx_optional_args->step;
       }
     }
   }
 
-  /* "rand/nazo_rand.pyx":38
+  /* "nazo_rand/nazo_rand.pyx":38
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   __pyx_t_1 = ((__pyx_v_stop == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "rand/nazo_rand.pyx":39
+    /* "nazo_rand/nazo_rand.pyx":39
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
 
-    /* "rand/nazo_rand.pyx":38
+    /* "nazo_rand/nazo_rand.pyx":38
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   }
 
-  /* "rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":40
  *     if stop == 0:
  *         stop, start = start, 0
  *     return random_range(start, stop, step)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::random_range(__pyx_v_start, __pyx_v_stop, __pyx_v_step);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":37
+  /* "nazo_rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_11randrange = {"randrange", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4rand_9nazo_rand_11randrange, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_11randrange = {"randrange", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_11randrange, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_start;
   int __pyx_v_stop;
   int __pyx_v_step;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -2134,99 +2134,99 @@
       __pyx_v_step = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_10randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_10randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_10randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_10randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  struct __pyx_opt_args_4rand_9nazo_rand_randrange __pyx_t_2;
+  struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randrange", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.stop = __pyx_v_stop;
   __pyx_t_2.step = __pyx_v_step;
-  __pyx_t_1 = __pyx_f_4rand_9nazo_rand_randrange(__pyx_v_start, 0, &__pyx_t_2); 
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_start, 0, &__pyx_t_2); 
   __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":43
+/* "nazo_rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static double __pyx_f_4rand_9nazo_rand_random_double(double __pyx_v_a, double __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double __pyx_v_a, double __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double", 0);
 
-  /* "rand/nazo_rand.pyx":44
+  /* "nazo_rand/nazo_rand.pyx":44
  * 
  * cpdef double random_double(double a, double b):
  *     return uniform_real_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::uniform_real_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":43
+  /* "nazo_rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_13random_double = {"random_double", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4rand_9nazo_rand_13random_double, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_13random_double = {"random_double", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_13random_double, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   double __pyx_v_a;
   double __pyx_v_b;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2269,118 +2269,118 @@
     __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
     __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 43, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_12random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_12random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_12random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_12random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_4rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rand/nazo_rand.pyx":47
+/* "nazo_rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
-static PyObject *__pyx_pw_4rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static double __pyx_f_4rand_9nazo_rand_random_double_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
 
-  /* "rand/nazo_rand.pyx":48
+  /* "nazo_rand/nazo_rand.pyx":48
  * 
  * cpdef double random_double_noargs():
  *     return uniform_real_variate_noargs()             # <<<<<<<<<<<<<<
  */
   __pyx_r = Storm::uniform_real_variate_noargs();
   goto __pyx_L0;
 
-  /* "rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_4rand_9nazo_rand_15random_double_noargs = {"random_double_noargs", (PyCFunction)__pyx_pw_4rand_9nazo_rand_15random_double_noargs, METH_NOARGS, 0};
-static PyObject *__pyx_pw_4rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_15random_double_noargs = {"random_double_noargs", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs, METH_NOARGS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs (wrapper)", 0);
-  __pyx_r = __pyx_pf_4rand_9nazo_rand_14random_double_noargs(__pyx_self);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_14random_double_noargs(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4rand_9nazo_rand_14random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_14random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_4rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rand.nazo_rand.random_double_noargs", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_double_noargs", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -2433,16 +2433,16 @@
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_elements, __pyx_k_elements, sizeof(__pyx_k_elements), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_rand_nazo_rand, __pyx_k_rand_nazo_rand, sizeof(__pyx_k_rand_nazo_rand), 0, 0, 1, 1},
-  {&__pyx_kp_s_rand_nazo_rand_pyx, __pyx_k_rand_nazo_rand_pyx, sizeof(__pyx_k_rand_nazo_rand_pyx), 0, 0, 1, 0},
+  {&__pyx_n_s_nazo_rand_nazo_rand, __pyx_k_nazo_rand_nazo_rand, sizeof(__pyx_k_nazo_rand_nazo_rand), 0, 0, 1, 1},
+  {&__pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_k_nazo_rand_nazo_rand_pyx, sizeof(__pyx_k_nazo_rand_nazo_rand_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_randbelow, __pyx_k_randbelow, sizeof(__pyx_k_randbelow), 0, 0, 1, 1},
   {&__pyx_n_s_randint, __pyx_k_randint, sizeof(__pyx_k_randint), 0, 0, 1, 1},
   {&__pyx_n_s_random_choice, __pyx_k_random_choice, sizeof(__pyx_k_random_choice), 0, 0, 1, 1},
   {&__pyx_n_s_random_double, __pyx_k_random_double, sizeof(__pyx_k_random_double), 0, 0, 1, 1},
   {&__pyx_n_s_random_double_noargs, __pyx_k_random_double_noargs, sizeof(__pyx_k_random_double_noargs), 0, 0, 1, 1},
   {&__pyx_n_s_random_integer_noargs, __pyx_k_random_integer_noargs, sizeof(__pyx_k_random_integer_noargs), 0, 0, 1, 1},
   {&__pyx_n_s_randrange, __pyx_k_randrange, sizeof(__pyx_k_randrange), 0, 0, 1, 1},
@@ -2463,102 +2463,102 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "rand/nazo_rand.pyx":15
+  /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 15, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":18
+  /* "nazo_rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":24
+  /* "nazo_rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
   __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_a); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":29
+  /* "nazo_rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_s_elements); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 29, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
   __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randint, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 34, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":37
+  /* "nazo_rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
   __pyx_tuple__10 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_randrange, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 37, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":43
+  /* "nazo_rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
   __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_double, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 43, __pyx_L1_error)
 
-  /* "rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2596,22 +2596,22 @@
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
-  if (__Pyx_ExportFunction("shuffle", (void (*)(void))__pyx_f_4rand_9nazo_rand_shuffle, "void (PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("random_integer_noargs", (void (*)(void))__pyx_f_4rand_9nazo_rand_random_integer_noargs, "int (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("random_choice", (void (*)(void))__pyx_f_4rand_9nazo_rand_random_choice, "PyObject *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("randbelow", (void (*)(void))__pyx_f_4rand_9nazo_rand_randbelow, "int (int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("randint", (void (*)(void))__pyx_f_4rand_9nazo_rand_randint, "int (int, int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("randrange", (void (*)(void))__pyx_f_4rand_9nazo_rand_randrange, "int (int, int __pyx_skip_dispatch, struct __pyx_opt_args_4rand_9nazo_rand_randrange *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("random_double", (void (*)(void))__pyx_f_4rand_9nazo_rand_random_double, "double (double, double, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("random_double_noargs", (void (*)(void))__pyx_f_4rand_9nazo_rand_random_double_noargs, "double (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("shuffle", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_shuffle, "void (PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("random_integer_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs, "int (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("random_choice", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_choice, "PyObject *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("randbelow", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randbelow, "int (int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("randint", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randint, "int (int, int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("randrange", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randrange, "int (int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("random_double", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double, "double (double, double, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("random_double_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs, "double (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2815,22 +2815,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_rand__nazo_rand) {
+  if (__pyx_module_is_main_nazo_rand__nazo_rand) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "rand.nazo_rand")) {
-      if (unlikely(PyDict_SetItemString(modules, "rand.nazo_rand", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "nazo_rand.nazo_rand")) {
+      if (unlikely(PyDict_SetItemString(modules, "nazo_rand.nazo_rand", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2843,110 +2843,110 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "rand/nazo_rand.pyx":15
+  /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":18
+  /* "nazo_rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":24
+  /* "nazo_rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":29
+  /* "nazo_rand/nazo_rand.pyx":29
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = randbelow(len(elements))
  *     return elements[index]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_7random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":34
  * 
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_9randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":37
+  /* "nazo_rand/nazo_rand.pyx":37
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_11randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":43
+  /* "nazo_rand/nazo_rand.pyx":43
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_13random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":47
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_4rand_9nazo_rand_15random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rand/nazo_rand.pyx":1
+  /* "nazo_rand/nazo_rand.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * cimport cython
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2955,19 +2955,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init rand.nazo_rand", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init nazo_rand.nazo_rand", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init rand.nazo_rand");
+    PyErr_SetString(PyExc_ImportError, "init nazo_rand.nazo_rand");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `nazo_rand-0.0.3/rand/nazo_rand.hpp` & `nazo_rand-0.0.5/nazo_rand/nazo_rand.hpp`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.3/rand/nazo_rand.pyi` & `nazo_rand-0.0.5/nazo_rand/nazo_rand.pyi`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.3/rand/nazo_rand.pyx` & `nazo_rand-0.0.5/nazo_rand/nazo_rand.pyx`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.3/setup.py` & `nazo_rand-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 
 
 setup(
     name="nazo_rand",
     ext_modules=cythonize(
         Extension(
             name="",
-            sources=["rand/nazo_rand.pyx"],
+            sources=["nazo_rand/nazo_rand.pyx"],
             language=["c++"],
             extra_compile_args=["-std=c++17", "-O3"],
             extra_link_args=["-O3"],
         ),
         compiler_directives={
             "language_level": 3,
             "boundscheck": False,
             "wraparound": False,
             "binding": True,
             "cdivision": True,
         },
     ),
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.0.3",
+    version="0.0.5",
     description="A fast random number generator for python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="Free for non-commercial use",
     package_data={
         "": [
-            "rand/nazo_rand.pyi",
-            "rand/nazo_rand.pyx",
-            "rand/nazo_rand.hpp",
-            "rand/nazo_rand.pxd",
+            "nazo_rand/nazo_rand.pyi",
+            "nazo_rand/nazo_rand.pyx",
+            "nazo_rand/nazo_rand.hpp",
+            "nazo_rand/nazo_rand.pxd",
         ]
     },
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
@@ -50,9 +50,9 @@
         "Programming Language :: Cython",
         "Programming Language :: C++",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.8",
-    packages=["rand"],
+    packages=["nazo_rand"],
 )
```

