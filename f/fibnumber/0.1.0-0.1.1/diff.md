# Comparing `tmp/fibnumber-0.1.0.tar.gz` & `tmp/fibnumber-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibnumber-0.1.0.tar", max compression
+gzip compressed data, was "fibnumber-0.1.1.tar", max compression
```

## Comparing `fibnumber-0.1.0.tar` & `fibnumber-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-04-15 08:56:20.048290 fibnumber-0.1.0/LICENSE
--rw-r--r--   0        0        0       67 2023-04-15 08:39:32.833112 fibnumber-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-14 16:39:33.459711 fibnumber-0.1.0/fibnumber/__init__.py
--rw-r--r--   0        0        0      308 2023-04-14 17:16:42.488724 fibnumber-0.1.0/fibnumber/cmd/fib_numb.py
--rw-r--r--   0        0        0        0 2023-04-14 15:53:09.205136 fibnumber-0.1.0/fibnumber/fib_calcs/__init__.py
--rw-r--r--   0        0        0      302 2023-04-15 09:13:37.373469 fibnumber-0.1.0/fibnumber/fib_calcs/fib_number.py
--rw-r--r--   0        0        0      200 2023-04-15 09:14:11.777173 fibnumber-0.1.0/fibnumber/fib_calcs/fib_numbers.py
--rw-r--r--   0        0        0      406 2023-04-15 09:14:59.388761 fibnumber-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 fibnumber-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-15 08:56:20.048290 fibnumber-0.1.1/LICENSE
+-rw-r--r--   0        0        0       67 2023-04-15 08:39:32.833112 fibnumber-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 16:39:33.459711 fibnumber-0.1.1/fibnumber/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-14 17:16:42.488724 fibnumber-0.1.1/fibnumber/cmd/fib_numb.py
+-rw-r--r--   0        0        0        0 2023-04-14 15:53:09.205136 fibnumber-0.1.1/fibnumber/fib_calcs/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-15 09:13:37.373469 fibnumber-0.1.1/fibnumber/fib_calcs/fib_number.py
+-rw-r--r--   0        0        0      200 2023-04-15 09:14:11.777173 fibnumber-0.1.1/fibnumber/fib_calcs/fib_numbers.py
+-rw-r--r--   0        0        0      447 2023-04-15 09:20:32.265800 fibnumber-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 fibnumber-0.1.1/PKG-INFO
```

### Comparing `fibnumber-0.1.0/LICENSE` & `fibnumber-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fibnumber-0.1.0/PKG-INFO` & `fibnumber-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: fibnumber
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calculate fibonacci using a simple program
 Author: XettriSomeman
 Author-email: bsomeman326@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: server
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Description-Content-Type: text/markdown
 
 ## Beginner Python Pip Package
 
 ### To run type: fib-number --help
```

