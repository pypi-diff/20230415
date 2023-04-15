# Comparing `tmp/fibnumber-0.1.3.tar.gz` & `tmp/fibnumber-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibnumber-0.1.3.tar", max compression
+gzip compressed data, was "fibnumber-0.1.4.tar", max compression
```

## Comparing `fibnumber-0.1.3.tar` & `fibnumber-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-04-15 08:56:20.048290 fibnumber-0.1.3/LICENSE
--rw-r--r--   0        0        0       67 2023-04-15 08:39:32.833112 fibnumber-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-14 16:39:33.459711 fibnumber-0.1.3/fibnumber/__init__.py
--rw-r--r--   0        0        0      308 2023-04-14 17:16:42.488724 fibnumber-0.1.3/fibnumber/cmd/fib_numb.py
--rw-r--r--   0        0        0        0 2023-04-14 15:53:09.205136 fibnumber-0.1.3/fibnumber/fib_calcs/__init__.py
--rw-r--r--   0        0        0      302 2023-04-15 09:13:37.373469 fibnumber-0.1.3/fibnumber/fib_calcs/fib_number.py
--rw-r--r--   0        0        0      200 2023-04-15 09:14:11.777173 fibnumber-0.1.3/fibnumber/fib_calcs/fib_numbers.py
--rw-r--r--   0        0        0      555 2023-04-15 09:29:34.552811 fibnumber-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 fibnumber-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-15 08:56:20.048290 fibnumber-0.1.4/LICENSE
+-rw-r--r--   0        0        0       67 2023-04-15 08:39:32.833112 fibnumber-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 16:39:33.459711 fibnumber-0.1.4/fibnumber/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-14 17:16:42.488724 fibnumber-0.1.4/fibnumber/cmd/fib_numb.py
+-rw-r--r--   0        0        0        0 2023-04-14 15:53:09.205136 fibnumber-0.1.4/fibnumber/fib_calcs/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-15 09:13:37.373469 fibnumber-0.1.4/fibnumber/fib_calcs/fib_number.py
+-rw-r--r--   0        0        0      200 2023-04-15 09:14:11.777173 fibnumber-0.1.4/fibnumber/fib_calcs/fib_numbers.py
+-rw-r--r--   0        0        0      558 2023-04-15 13:04:29.268271 fibnumber-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 fibnumber-0.1.4/PKG-INFO
```

### Comparing `fibnumber-0.1.3/LICENSE` & `fibnumber-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fibnumber-0.1.3/pyproject.toml` & `fibnumber-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "fibnumber"
-version = "0.1.3"
+version = "0.1.4"
 description = "Calculate fibonacci using a simple program"
 authors = ["XettriSomeman <bsomeman326@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
 
 # optional package, used as `pip install fibnumber[server]'
-fastapi ={version = "^0.95.1", optional=true} 
+fastapi = {version = "^0.95.1", optional=true} 
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
 fib-number = "fibnumber.cmd.fib_numb:calculate_fib"
 
 [tool.poetry.extras]
-server=['fastapi']
+server = ["fastapi"]
```

### Comparing `fibnumber-0.1.3/PKG-INFO` & `fibnumber-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibnumber
-Version: 0.1.3
+Version: 0.1.4
 Summary: Calculate fibonacci using a simple program
 Author: XettriSomeman
 Author-email: bsomeman326@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

