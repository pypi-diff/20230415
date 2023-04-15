# Comparing `tmp/hackyargparser-0.11.tar.gz` & `tmp/hackyargparser-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackyargparser-0.11.tar", last modified: Fri Apr 14 05:51:15 2023, max compression
+gzip compressed data, was "hackyargparser-0.12.tar", last modified: Sat Apr 15 00:29:42 2023, max compression
```

## Comparing `hackyargparser-0.11.tar` & `hackyargparser-0.12.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 05:51:15.379812 hackyargparser-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-14 05:51:13.000000 hackyargparser-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      145 2023-04-14 05:51:12.000000 hackyargparser-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     4685 2023-04-14 05:51:15.379812 hackyargparser-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     3833 2023-04-14 04:52:15.000000 hackyargparser-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 05:51:15.372318 hackyargparser-0.11/hackyargparser/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 hackyargparser-0.11/hackyargparser/LICENSE
--rw-rw-rw-   0        0        0     3833 2023-04-14 04:52:15.000000 hackyargparser-0.11/hackyargparser/README.md
--rw-rw-rw-   0        0        0     4450 2023-04-14 05:48:51.000000 hackyargparser-0.11/hackyargparser/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-14 05:51:14.000000 hackyargparser-0.11/hackyargparser/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 05:51:14.000000 hackyargparser-0.11/hackyargparser/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-14 05:51:15.378302 hackyargparser-0.11/hackyargparser.egg-info/
--rw-rw-rw-   0        0        0     4685 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 05:51:15.381315 hackyargparser-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-04-14 05:51:14.000000 hackyargparser-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:29:42.674337 hackyargparser-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:29:36.000000 hackyargparser-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      113 2023-04-15 00:29:35.000000 hackyargparser-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     4477 2023-04-15 00:29:42.674337 hackyargparser-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     3833 2023-04-15 00:17:31.000000 hackyargparser-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 00:29:42.669350 hackyargparser-0.12/hackyargparser/
+-rw-rw-rw-   0        0        0     3833 2023-04-15 00:17:31.000000 hackyargparser-0.12/hackyargparser/README.md
+-rw-rw-rw-   0        0        0     4450 2023-04-15 00:17:31.000000 hackyargparser-0.12/hackyargparser/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-15 00:29:40.000000 hackyargparser-0.12/hackyargparser/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 00:29:40.000000 hackyargparser-0.12/hackyargparser/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 00:29:42.673340 hackyargparser-0.12/hackyargparser.egg-info/
+-rw-rw-rw-   0        0        0     4477 2023-04-15 00:29:42.000000 hackyargparser-0.12/hackyargparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-04-15 00:29:42.000000 hackyargparser-0.12/hackyargparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:29:42.000000 hackyargparser-0.12/hackyargparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-15 00:29:42.000000 hackyargparser-0.12/hackyargparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-15 00:29:42.675335 hackyargparser-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2023-04-15 00:29:40.000000 hackyargparser-0.12/setup.py
```

### Comparing `hackyargparser-0.11/LICENSE.rst` & `hackyargparser-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hackyargparser-0.11/PKG-INFO` & `hackyargparser-0.12/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,142 @@
-Metadata-Version: 2.1
-Name: hackyargparser
-Version: 0.11
-Summary: Hacky argparser - parses arguments and changes the defaults of functions
-Home-page: https://github.com/hansalemaos/hackyargparser
-Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
-License: MIT
-Keywords: argparser
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
-# Hacky argparser - parses arguments and changes the defaults of functions
-
-## pip install hackyargparser
-
-A decorator function that modifies the default arguments of a given function based on the values passed through command line arguments.
-The function first checks if the input function is callable or None. It then retrieves the global dictionary of the
-calling frame and defines a decorator function. The decorator function modifies the default arguments of the input
-function based on the values passed through command line arguments. It does this by retrieving the variable names
-and annotations of the input function and creating a dictionary of all the annotations. It then iterates through
-the default arguments of the input function and tries to convert them to the appropriate data type based on the
-annotations. If the conversion fails, it tries all possible data types until a successful conversion is made. The
-modified default arguments are then set and the input function is called with the modified arguments.
-
-
-## Create a py file 
-
-```python
-
-# "a2.py" in this example
-
-from hackyargparser import add_sysargv, config
-
-config.helptext = (
-    "Error! --f2_a, --f2_b, --f1_a are mandatory!"  # The help text to be printed
-)
-config.kill_when_not_there(
-    ("--f2_a", "--f2_b", "--f1_a")
-)  # If those arguments are not passed, config.helptext will be printed, and sys.exit will be called
-config.stop_after_kill = True  # Stop after printing config.helptext -> input()
-
-
-@add_sysargv
-def function1(
-    f1_a: int | float | None = None,
-    f1_b: int | float = 1,
-    mvar: int = 10,
-):
-    print(f1_b * f1_a * mvar)
-    return f1_a, f1_b, mvar
-
-
-@add_sysargv
-def function2(
-    f2_a: int | float | None = None,
-    f2_b: int | float | None = None,
-    mvar: int = 10,
-):
-    print(f2_a * f2_b * mvar)
-
-    return f2_a, f2_b, mvar
-
-
-@add_sysargv
-def function3(
-    f3_a: list | tuple = (),
-    f3_b: int | float = 1,
-):
-    for l in f3_a:
-        print(l + f3_b)
-
-    return set(f3_a)
-
-
-def function4(
-    f3_a: list | tuple = (),
-    f3_b: int | float = 1,
-):
-    print("i am not decorated")
-    print(f"{f3_a=}, {f3_b=}")
-
-    return set(f3_a)
-
-
-print(function2())
-
-print(function1())
-
-print(function3())
-
-print(function4())
-
-
-```
-
-
-# Execute the py file  with arguments from the command line
-
-```python
-####################################################################################################
-# use -- and the local variable name as arguments followed by the value you want to pass
-# Type hints are necessary as well as default values 
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60
-# 36000
-# (12, 300, 10)
-# 600
-# (60, 1, 10)
-# ...
-####################################################################################################
-
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300
-# Error! --f2_a, --f2_b, --f1_a are mandatory!
-####################################################################################################
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a [1,2,3,4,5,4,4] --f3_b 22
-
-
-# 36000
-# (12, 300, 10)
-# 600
-# (60, 1, 10)
-# 23
-# 24
-# 25
-# 26
-# 27
-# 26
-# 26
-# {1, 2, 3, 4, 5}
-# i am not decorated
-# f3_a=(), f3_b=1
-# set()
-
-####################################################################################################
-# If you get any errors, try using quotes  --f3_a "(1,2,3,4,5)"
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a "(1,2,3,4,5)" --f3_b 22
-
-# 36000
-# (12, 300, 10)
-# 600
-# (60, 1, 10)
-# 23
-# 24
-# 25
-# 26
-# 27
-# {1, 2, 3, 4, 5}
-# i am not decorated
-# f3_a=(), f3_b=1
-# set()
-
-
-####################################################################################################
-```
+# Hacky argparser - parses arguments and changes the defaults of functions
+
+## pip install hackyargparser
+
+A decorator function that modifies the default arguments of a given function based on the values passed through command line arguments.
+The function first checks if the input function is callable or None. It then retrieves the global dictionary of the
+calling frame and defines a decorator function. The decorator function modifies the default arguments of the input
+function based on the values passed through command line arguments. It does this by retrieving the variable names
+and annotations of the input function and creating a dictionary of all the annotations. It then iterates through
+the default arguments of the input function and tries to convert them to the appropriate data type based on the
+annotations. If the conversion fails, it tries all possible data types until a successful conversion is made. The
+modified default arguments are then set and the input function is called with the modified arguments.
+
+
+## Create a py file 
+
+```python
+
+# "a2.py" in this example
+
+from hackyargparser import add_sysargv, config
+
+config.helptext = (
+    "Error! --f2_a, --f2_b, --f1_a are mandatory!"  # The help text to be printed
+)
+config.kill_when_not_there(
+    ("--f2_a", "--f2_b", "--f1_a")
+)  # If those arguments are not passed, config.helptext will be printed, and sys.exit will be called
+config.stop_after_kill = True  # Stop after printing config.helptext -> input()
+
+
+@add_sysargv
+def function1(
+    f1_a: int | float | None = None,
+    f1_b: int | float = 1,
+    mvar: int = 10,
+):
+    print(f1_b * f1_a * mvar)
+    return f1_a, f1_b, mvar
+
+
+@add_sysargv
+def function2(
+    f2_a: int | float | None = None,
+    f2_b: int | float | None = None,
+    mvar: int = 10,
+):
+    print(f2_a * f2_b * mvar)
+
+    return f2_a, f2_b, mvar
+
+
+@add_sysargv
+def function3(
+    f3_a: list | tuple = (),
+    f3_b: int | float = 1,
+):
+    for l in f3_a:
+        print(l + f3_b)
+
+    return set(f3_a)
+
+
+def function4(
+    f3_a: list | tuple = (),
+    f3_b: int | float = 1,
+):
+    print("i am not decorated")
+    print(f"{f3_a=}, {f3_b=}")
+
+    return set(f3_a)
+
+
+print(function2())
+
+print(function1())
+
+print(function3())
+
+print(function4())
+
+
+```
+
+
+# Execute the py file  with arguments from the command line
+
+```python
+####################################################################################################
+# use -- and the local variable name as arguments followed by the value you want to pass
+# Type hints are necessary as well as default values 
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60
+# 36000
+# (12, 300, 10)
+# 600
+# (60, 1, 10)
+# ...
+####################################################################################################
+
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300
+# Error! --f2_a, --f2_b, --f1_a are mandatory!
+####################################################################################################
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a [1,2,3,4,5,4,4] --f3_b 22
+
+
+# 36000
+# (12, 300, 10)
+# 600
+# (60, 1, 10)
+# 23
+# 24
+# 25
+# 26
+# 27
+# 26
+# 26
+# {1, 2, 3, 4, 5}
+# i am not decorated
+# f3_a=(), f3_b=1
+# set()
+
+####################################################################################################
+# If you get any errors, try using quotes  --f3_a "(1,2,3,4,5)"
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a "(1,2,3,4,5)" --f3_b 22
+
+# 36000
+# (12, 300, 10)
+# 600
+# (60, 1, 10)
+# 23
+# 24
+# 25
+# 26
+# 27
+# {1, 2, 3, 4, 5}
+# i am not decorated
+# f3_a=(), f3_b=1
+# set()
+
+
+####################################################################################################
+```
```

### Comparing `hackyargparser-0.11/README.md` & `hackyargparser-0.12/hackyargparser/README.md`

 * *Files identical despite different names*

### Comparing `hackyargparser-0.11/hackyargparser/README.md` & `hackyargparser-0.12/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: hackyargparser
+Version: 0.12
+Summary: Hacky argparser - parses arguments and changes the defaults of functions
+Home-page: https://github.com/hansalemaos/hackyargparser
+Author: Johannes Fischer
+Author-email: aulasparticularesdealemaosp@gmail.com
+License: MIT
+Keywords: argparser
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE.rst
+
 # Hacky argparser - parses arguments and changes the defaults of functions
 
 ## pip install hackyargparser
 
 A decorator function that modifies the default arguments of a given function based on the values passed through command line arguments.
 The function first checks if the input function is callable or None. It then retrieves the global dictionary of the
 calling frame and defines a decorator function. The decorator function modifies the default arguments of the input
```

### Comparing `hackyargparser-0.11/hackyargparser/__init__.py` & `hackyargparser-0.12/hackyargparser/__init__.py`

 * *Files identical despite different names*

### Comparing `hackyargparser-0.11/hackyargparser.egg-info/PKG-INFO` & `hackyargparser-0.12/hackyargparser.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,159 @@
 Metadata-Version: 2.1
 Name: hackyargparser
-Version: 0.11
+Version: 0.12
 Summary: Hacky argparser - parses arguments and changes the defaults of functions
 Home-page: https://github.com/hansalemaos/hackyargparser
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: argparser
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Hacky argparser - parses arguments and changes the defaults of functions
 
-# Hacky argparser - parses arguments and changes the defaults of functions
-
-## pip install hackyargparser
-
-A decorator function that modifies the default arguments of a given function based on the values passed through command line arguments.
-The function first checks if the input function is callable or None. It then retrieves the global dictionary of the
-calling frame and defines a decorator function. The decorator function modifies the default arguments of the input
-function based on the values passed through command line arguments. It does this by retrieving the variable names
-and annotations of the input function and creating a dictionary of all the annotations. It then iterates through
-the default arguments of the input function and tries to convert them to the appropriate data type based on the
-annotations. If the conversion fails, it tries all possible data types until a successful conversion is made. The
-modified default arguments are then set and the input function is called with the modified arguments.
-
-
-## Create a py file 
-
-```python
-
-# "a2.py" in this example
-
-from hackyargparser import add_sysargv, config
-
-config.helptext = (
-    "Error! --f2_a, --f2_b, --f1_a are mandatory!"  # The help text to be printed
-)
-config.kill_when_not_there(
-    ("--f2_a", "--f2_b", "--f1_a")
-)  # If those arguments are not passed, config.helptext will be printed, and sys.exit will be called
-config.stop_after_kill = True  # Stop after printing config.helptext -> input()
-
-
-@add_sysargv
-def function1(
-    f1_a: int | float | None = None,
-    f1_b: int | float = 1,
-    mvar: int = 10,
-):
-    print(f1_b * f1_a * mvar)
-    return f1_a, f1_b, mvar
-
-
-@add_sysargv
-def function2(
-    f2_a: int | float | None = None,
-    f2_b: int | float | None = None,
-    mvar: int = 10,
-):
-    print(f2_a * f2_b * mvar)
-
-    return f2_a, f2_b, mvar
-
-
-@add_sysargv
-def function3(
-    f3_a: list | tuple = (),
-    f3_b: int | float = 1,
-):
-    for l in f3_a:
-        print(l + f3_b)
-
-    return set(f3_a)
-
-
-def function4(
-    f3_a: list | tuple = (),
-    f3_b: int | float = 1,
-):
-    print("i am not decorated")
-    print(f"{f3_a=}, {f3_b=}")
-
-    return set(f3_a)
-
-
-print(function2())
-
-print(function1())
-
-print(function3())
-
-print(function4())
-
-
-```
-
-
-# Execute the py file  with arguments from the command line
-
-```python
-####################################################################################################
-# use -- and the local variable name as arguments followed by the value you want to pass
-# Type hints are necessary as well as default values 
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60
-# 36000
-# (12, 300, 10)
-# 600
-# (60, 1, 10)
-# ...
-####################################################################################################
-
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300
-# Error! --f2_a, --f2_b, --f1_a are mandatory!
-####################################################################################################
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a [1,2,3,4,5,4,4] --f3_b 22
-
-
-# 36000
-# (12, 300, 10)
-# 600
-# (60, 1, 10)
-# 23
-# 24
-# 25
-# 26
-# 27
-# 26
-# 26
-# {1, 2, 3, 4, 5}
-# i am not decorated
-# f3_a=(), f3_b=1
-# set()
-
-####################################################################################################
-# If you get any errors, try using quotes  --f3_a "(1,2,3,4,5)"
-# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a "(1,2,3,4,5)" --f3_b 22
-
-# 36000
-# (12, 300, 10)
-# 600
-# (60, 1, 10)
-# 23
-# 24
-# 25
-# 26
-# 27
-# {1, 2, 3, 4, 5}
-# i am not decorated
-# f3_a=(), f3_b=1
-# set()
-
-
-####################################################################################################
-```
+## pip install hackyargparser
+
+A decorator function that modifies the default arguments of a given function based on the values passed through command line arguments.
+The function first checks if the input function is callable or None. It then retrieves the global dictionary of the
+calling frame and defines a decorator function. The decorator function modifies the default arguments of the input
+function based on the values passed through command line arguments. It does this by retrieving the variable names
+and annotations of the input function and creating a dictionary of all the annotations. It then iterates through
+the default arguments of the input function and tries to convert them to the appropriate data type based on the
+annotations. If the conversion fails, it tries all possible data types until a successful conversion is made. The
+modified default arguments are then set and the input function is called with the modified arguments.
+
+
+## Create a py file 
+
+```python
+
+# "a2.py" in this example
+
+from hackyargparser import add_sysargv, config
+
+config.helptext = (
+    "Error! --f2_a, --f2_b, --f1_a are mandatory!"  # The help text to be printed
+)
+config.kill_when_not_there(
+    ("--f2_a", "--f2_b", "--f1_a")
+)  # If those arguments are not passed, config.helptext will be printed, and sys.exit will be called
+config.stop_after_kill = True  # Stop after printing config.helptext -> input()
+
+
+@add_sysargv
+def function1(
+    f1_a: int | float | None = None,
+    f1_b: int | float = 1,
+    mvar: int = 10,
+):
+    print(f1_b * f1_a * mvar)
+    return f1_a, f1_b, mvar
+
+
+@add_sysargv
+def function2(
+    f2_a: int | float | None = None,
+    f2_b: int | float | None = None,
+    mvar: int = 10,
+):
+    print(f2_a * f2_b * mvar)
+
+    return f2_a, f2_b, mvar
+
+
+@add_sysargv
+def function3(
+    f3_a: list | tuple = (),
+    f3_b: int | float = 1,
+):
+    for l in f3_a:
+        print(l + f3_b)
+
+    return set(f3_a)
+
+
+def function4(
+    f3_a: list | tuple = (),
+    f3_b: int | float = 1,
+):
+    print("i am not decorated")
+    print(f"{f3_a=}, {f3_b=}")
+
+    return set(f3_a)
+
+
+print(function2())
+
+print(function1())
+
+print(function3())
+
+print(function4())
+
+
+```
+
+
+# Execute the py file  with arguments from the command line
+
+```python
+####################################################################################################
+# use -- and the local variable name as arguments followed by the value you want to pass
+# Type hints are necessary as well as default values 
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60
+# 36000
+# (12, 300, 10)
+# 600
+# (60, 1, 10)
+# ...
+####################################################################################################
+
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300
+# Error! --f2_a, --f2_b, --f1_a are mandatory!
+####################################################################################################
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a [1,2,3,4,5,4,4] --f3_b 22
+
+
+# 36000
+# (12, 300, 10)
+# 600
+# (60, 1, 10)
+# 23
+# 24
+# 25
+# 26
+# 27
+# 26
+# 26
+# {1, 2, 3, 4, 5}
+# i am not decorated
+# f3_a=(), f3_b=1
+# set()
+
+####################################################################################################
+# If you get any errors, try using quotes  --f3_a "(1,2,3,4,5)"
+# .\python.exe .\a2.py --f2_a 12 --f2_b 300 --f1_a 60 --f3_a "(1,2,3,4,5)" --f3_b 22
+
+# 36000
+# (12, 300, 10)
+# 600
+# (60, 1, 10)
+# 23
+# 24
+# 25
+# 26
+# 27
+# {1, 2, 3, 4, 5}
+# i am not decorated
+# f3_a=(), f3_b=1
+# set()
+
+
+####################################################################################################
+```
```

### Comparing `hackyargparser-0.11/setup.py` & `hackyargparser-0.12/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
-import codecs
-import os
+# import codecs
+# import os
+# 
+# here = os.path.abspath(os.path.dirname(__file__))
+# 
+# with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+#     long_description = "\n" + fh.read()\
 
-#change to dict
-here = os.path.abspath(os.path.dirname(__file__))
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.11'
-DESCRIPTION = "Hacky argparser - parses arguments and changes the defaults of functions"
+VERSION = '''0.12'''
+DESCRIPTION = '''Hacky argparser - parses arguments and changes the defaults of functions'''
 
 # Setting up
 setup(
     name="hackyargparser",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/hackyargparser',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=[],
     keywords=['argparser'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=[],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

