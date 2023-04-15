# Comparing `tmp/webp_support-0.2.5.tar.gz` & `tmp/webp_support-0.2.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webp_support-0.2.5.tar", last modified: Sat Apr 15 05:46:56 2023, max compression
+gzip compressed data, was "webp_support-0.2.5.post1.tar", last modified: Sat Apr 15 06:32:38 2023, max compression
```

## Comparing `webp_support-0.2.5.tar` & `webp_support-0.2.5.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:46:56.077395 webp_support-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 05:46:27.000000 webp_support-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 05:46:27.000000 webp_support-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 05:46:56.077395 webp_support-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 05:46:27.000000 webp_support-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 05:46:27.000000 webp_support-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 05:46:56.077395 webp_support-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-15 05:46:27.000000 webp_support-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:46:56.077395 webp_support-0.2.5/webp_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 05:46:27.000000 webp_support-0.2.5/webp_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113612 2023-04-15 05:46:45.000000 webp_support-0.2.5/webp_support/webp_support.c
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 05:46:27.000000 webp_support-0.2.5/webp_support/webp_support.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 05:46:27.000000 webp_support-0.2.5/webp_support/webp_support.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 05:46:27.000000 webp_support-0.2.5/webp_support/webp_support_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 05:46:27.000000 webp_support-0.2.5/webp_support/webp_support_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:46:56.077395 webp_support-0.2.5/webp_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 05:46:56.000000 webp_support-0.2.5/webp_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 05:46:56.000000 webp_support-0.2.5/webp_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:46:56.000000 webp_support-0.2.5/webp_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 05:46:56.000000 webp_support-0.2.5/webp_support.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:32:38.893319 webp_support-0.2.5.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-15 06:32:38.893319 webp_support-0.2.5.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 06:32:38.893319 webp_support-0.2.5.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:32:38.893319 webp_support-0.2.5.post1/webp_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/webp_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113197 2023-04-15 06:32:29.000000 webp_support-0.2.5.post1/webp_support/webp_support.c
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/webp_support/webp_support.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/webp_support/webp_support.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/webp_support/webp_support_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 06:32:18.000000 webp_support-0.2.5.post1/webp_support/webp_support_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:32:38.893319 webp_support-0.2.5.post1/webp_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-15 06:32:38.000000 webp_support-0.2.5.post1/webp_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 06:32:38.000000 webp_support-0.2.5.post1/webp_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 06:32:38.000000 webp_support-0.2.5.post1/webp_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 06:32:38.000000 webp_support-0.2.5.post1/webp_support.egg-info/top_level.txt
```

### Comparing `webp_support-0.2.5/LICENSE` & `webp_support-0.2.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.5/PKG-INFO` & `webp_support-0.2.5.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp_support
-Version: 0.2.5
+Version: 0.2.5.post1
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `webp_support-0.2.5/README.md` & `webp_support-0.2.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.5/setup.py` & `webp_support-0.2.5.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 ext_modules = [
     Extension(
-        "webp_support.webp_support",
+        "webp_support",
         sources=["webp_support/webp_support.pyx", "webp_support/webp_support_c.c"],
         extra_compile_args=["-O3"],
         extra_link_args=["-O3"],
     ),
 ]
 
 setup(
@@ -25,15 +25,15 @@
             "wraparound": False,
         },
     ),
     package_data={'': ['webp_support/*.pyi', "webp_support/*.pyx","webp_support/*.c","webp_support/*.h"]},
     include_package_data=True,
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.2.5",
+    version="0.2.5-1",
     url="https://github.com/bymoye/webp_support",
     description="A Quickly determine whether Webp is supported from UserAgent.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

### Comparing `webp_support-0.2.5/webp_support/webp_support.c` & `webp_support-0.2.5.post1/webp_support/webp_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,21 @@
         ],
         "extra_link_args": [
             "-O3"
         ],
         "include_dirs": [
             "webp_support"
         ],
-        "name": "webp_support.webp_support",
+        "name": "webp_support",
         "sources": [
             "webp_support/webp_support.pyx",
             "webp_support/webp_support_c.c"
         ]
     },
-    "module_name": "webp_support.webp_support"
+    "module_name": "webp_support"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
@@ -759,16 +759,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__webp_support__webp_support
-#define __PYX_HAVE_API__webp_support__webp_support
+#define __PYX_HAVE__webp_support
+#define __PYX_HAVE_API__webp_support
 /* Early includes */
 #include "webp_support_c.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
@@ -1183,127 +1183,127 @@
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'cython' */
 
-/* Module declarations from 'webp_support.webp_support' */
-static int __pyx_f_12webp_support_12webp_support_webp_supported(PyObject *, int __pyx_skip_dispatch); /*proto*/
-#define __Pyx_MODULE_NAME "webp_support.webp_support"
-extern int __pyx_module_is_main_webp_support__webp_support;
-int __pyx_module_is_main_webp_support__webp_support = 0;
+/* Module declarations from 'webp_support' */
+static int __pyx_f_12webp_support_webp_supported(PyObject *, int __pyx_skip_dispatch); /*proto*/
+#define __Pyx_MODULE_NAME "webp_support"
+extern int __pyx_module_is_main_webp_support;
+int __pyx_module_is_main_webp_support = 0;
 
-/* Implementation of 'webp_support.webp_support' */
+/* Implementation of 'webp_support' */
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_pf_12webp_support_12webp_support_webp_supported(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_user_agent); /* proto */
+static PyObject *__pyx_pf_12webp_support_webp_supported(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_user_agent); /* proto */
 /* Late includes */
 
-/* "webp_support/webp_support.pyx":9
+/* "webp_support.pyx":9
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef bint webp_supported(bytes user_agent):             # <<<<<<<<<<<<<<
  *     return is_webp_supported(user_agent)
  */
 
-static PyObject *__pyx_pw_12webp_support_12webp_support_1webp_supported(PyObject *__pyx_self, PyObject *__pyx_v_user_agent); /*proto*/
-static int __pyx_f_12webp_support_12webp_support_webp_supported(PyObject *__pyx_v_user_agent, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_12webp_support_1webp_supported(PyObject *__pyx_self, PyObject *__pyx_v_user_agent); /*proto*/
+static int __pyx_f_12webp_support_webp_supported(PyObject *__pyx_v_user_agent, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   char const *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("webp_supported", 0);
 
-  /* "webp_support/webp_support.pyx":10
+  /* "webp_support.pyx":10
  * @cython.wraparound(False)
  * cpdef bint webp_supported(bytes user_agent):
  *     return is_webp_supported(user_agent)             # <<<<<<<<<<<<<<
  */
   if (unlikely(__pyx_v_user_agent == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
     __PYX_ERR(0, 10, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_PyBytes_AsString(__pyx_v_user_agent); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L1_error)
   __pyx_r = is_webp_supported(__pyx_t_1);
   goto __pyx_L0;
 
-  /* "webp_support/webp_support.pyx":9
+  /* "webp_support.pyx":9
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef bint webp_supported(bytes user_agent):             # <<<<<<<<<<<<<<
  *     return is_webp_supported(user_agent)
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_WriteUnraisable("webp_support.webp_support.webp_supported", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("webp_support.webp_supported", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12webp_support_12webp_support_1webp_supported(PyObject *__pyx_self, PyObject *__pyx_v_user_agent); /*proto*/
-static PyObject *__pyx_pw_12webp_support_12webp_support_1webp_supported(PyObject *__pyx_self, PyObject *__pyx_v_user_agent) {
+static PyObject *__pyx_pw_12webp_support_1webp_supported(PyObject *__pyx_self, PyObject *__pyx_v_user_agent); /*proto*/
+static PyObject *__pyx_pw_12webp_support_1webp_supported(PyObject *__pyx_self, PyObject *__pyx_v_user_agent) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("webp_supported (wrapper)", 0);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_user_agent), (&PyBytes_Type), 1, "user_agent", 1))) __PYX_ERR(0, 9, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12webp_support_12webp_support_webp_supported(__pyx_self, ((PyObject*)__pyx_v_user_agent));
+  __pyx_r = __pyx_pf_12webp_support_webp_supported(__pyx_self, ((PyObject*)__pyx_v_user_agent));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12webp_support_12webp_support_webp_supported(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_user_agent) {
+static PyObject *__pyx_pf_12webp_support_webp_supported(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_user_agent) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("webp_supported", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_12webp_support_12webp_support_webp_supported(__pyx_v_user_agent, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_12webp_support_webp_supported(__pyx_v_user_agent, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("webp_support.webp_support.webp_supported", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("webp_support.webp_supported", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyMethodDef __pyx_methods[] = {
-  {"webp_supported", (PyCFunction)__pyx_pw_12webp_support_12webp_support_1webp_supported, METH_O, 0},
+  {"webp_supported", (PyCFunction)__pyx_pw_12webp_support_1webp_supported, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
 static int __pyx_pymod_exec_webp_support(PyObject* module); /*proto*/
@@ -1601,22 +1601,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_webp_support__webp_support) {
+  if (__pyx_module_is_main_webp_support) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "webp_support.webp_support")) {
-      if (unlikely(PyDict_SetItemString(modules, "webp_support.webp_support", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "webp_support")) {
+      if (unlikely(PyDict_SetItemString(modules, "webp_support", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -1629,15 +1629,15 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "webp_support/webp_support.pyx":1
+  /* "webp_support.pyx":1
  * # webp_support.pyx             # <<<<<<<<<<<<<<
  * cimport cython
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -1646,19 +1646,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init webp_support.webp_support", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init webp_support", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init webp_support.webp_support");
+    PyErr_SetString(PyExc_ImportError, "init webp_support");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `webp_support-0.2.5/webp_support/webp_support_c.c` & `webp_support-0.2.5.post1/webp_support/webp_support_c.c`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.5/webp_support.egg-info/PKG-INFO` & `webp_support-0.2.5.post1/webp_support.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp-support
-Version: 0.2.5
+Version: 0.2.5.post1
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

