# Comparing `tmp/webp_support-0.2.5.post3.tar.gz` & `tmp/webp_support-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webp_support-0.2.5.post3.tar", last modified: Sat Apr 15 07:23:45 2023, max compression
+gzip compressed data, was "webp_support-0.2.6.tar", last modified: Sat Apr 15 07:41:56 2023, max compression
```

## Comparing `webp_support-0.2.5.post3.tar` & `webp_support-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:23:45.864604 webp_support-0.2.5.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-15 07:23:45.864604 webp_support-0.2.5.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:23:45.864604 webp_support-0.2.5.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:23:45.864604 webp_support-0.2.5.post3/webp_support/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/webp_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113612 2023-04-15 07:23:35.000000 webp_support-0.2.5.post3/webp_support/webp_support.c
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/webp_support/webp_support.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/webp_support/webp_support.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/webp_support/webp_support_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 07:23:25.000000 webp_support-0.2.5.post3/webp_support/webp_support_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:23:45.864604 webp_support-0.2.5.post3/webp_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-15 07:23:45.000000 webp_support-0.2.5.post3/webp_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 07:23:45.000000 webp_support-0.2.5.post3/webp_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:23:45.000000 webp_support-0.2.5.post3/webp_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 07:23:45.000000 webp_support-0.2.5.post3/webp_support.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:41:56.612640 webp_support-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 07:41:37.000000 webp_support-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 07:41:37.000000 webp_support-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:41:56.612640 webp_support-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-15 07:41:37.000000 webp_support-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 07:41:37.000000 webp_support-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:41:56.612640 webp_support-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-15 07:41:37.000000 webp_support-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:41:56.612640 webp_support-0.2.6/webp_support/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115007 2023-04-15 07:41:48.000000 webp_support-0.2.6/webp_support/webp_support.c
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 07:41:37.000000 webp_support-0.2.6/webp_support/webp_support_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:41:56.612640 webp_support-0.2.6/webp_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 07:41:56.000000 webp_support-0.2.6/webp_support.egg-info/top_level.txt
```

### Comparing `webp_support-0.2.5.post3/LICENSE` & `webp_support-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.5.post3/PKG-INFO` & `webp_support-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp_support
-Version: 0.2.5.post3
+Version: 0.2.6
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `webp_support-0.2.5.post3/README.md` & `webp_support-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.5.post3/webp_support/webp_support.c` & `webp_support-0.2.6/webp_support/webp_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1177,14 +1177,17 @@
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
+/* FunctionExport.proto */
+static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
+
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'webp_support.webp_support' */
@@ -1391,18 +1394,25 @@
   /*--- Variable export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
+  if (__Pyx_ExportFunction("webp_supported", (void (*)(void))__pyx_f_12webp_support_12webp_support_webp_supported, "int (PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __Pyx_RefNannyFinishContext();
@@ -1619,15 +1629,15 @@
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
-  (void)__Pyx_modinit_function_export_code();
+  if (unlikely(__Pyx_modinit_function_export_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_init_code();
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2625,14 +2635,51 @@
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
+/* FunctionExport */
+static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig) {
+    PyObject *d = 0;
+    PyObject *cobj = 0;
+    union {
+        void (*fp)(void);
+        void *p;
+    } tmp;
+    d = PyObject_GetAttrString(__pyx_m, (char *)"__pyx_capi__");
+    if (!d) {
+        PyErr_Clear();
+        d = PyDict_New();
+        if (!d)
+            goto bad;
+        Py_INCREF(d);
+        if (PyModule_AddObject(__pyx_m, (char *)"__pyx_capi__", d) < 0)
+            goto bad;
+    }
+    tmp.fp = f;
+#if PY_VERSION_HEX >= 0x02070000
+    cobj = PyCapsule_New(tmp.p, sig, 0);
+#else
+    cobj = PyCObject_FromVoidPtrAndDesc(tmp.p, (void *)sig, 0);
+#endif
+    if (!cobj)
+        goto bad;
+    if (PyDict_SetItemString(d, name, cobj) < 0)
+        goto bad;
+    Py_DECREF(cobj);
+    Py_DECREF(d);
+    return 0;
+bad:
+    Py_XDECREF(cobj);
+    Py_XDECREF(d);
+    return -1;
+}
+
 /* InitStrings */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
```

### Comparing `webp_support-0.2.5.post3/webp_support/webp_support_c.c` & `webp_support-0.2.6/webp_support/webp_support_c.c`

 * *Files identical despite different names*

### Comparing `webp_support-0.2.5.post3/webp_support.egg-info/PKG-INFO` & `webp_support-0.2.6/webp_support.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp-support
-Version: 0.2.5.post3
+Version: 0.2.6
 Summary: A Quickly determine whether Webp is supported from UserAgent.
 Home-page: https://github.com/bymoye/webp_support
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

