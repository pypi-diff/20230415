# Comparing `tmp/staticvar-0.0.5.tar.gz` & `tmp/staticvar-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticvar-0.0.5.tar", max compression
+gzip compressed data, was "staticvar-0.0.6.tar", max compression
```

## Comparing `staticvar-0.0.5.tar` & `staticvar-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1080 2023-04-14 22:15:59.466307 staticvar-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      696 2023-04-14 22:15:59.466307 staticvar-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3195 2023-04-14 22:15:59.466307 staticvar-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-04-14 22:15:59.476249 staticvar-0.0.5/staticvar/__init__.py
--rw-r--r--   0        0        0     2084 2023-04-14 22:15:59.476249 staticvar-0.0.5/staticvar/Static.py
--rw-r--r--   0        0        0     3907 1970-01-01 00:00:00.000000 staticvar-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-14 22:41:09.473574 staticvar-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      647 2023-04-14 22:41:09.473574 staticvar-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3195 2023-04-14 22:41:09.473574 staticvar-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 22:41:09.473574 staticvar-0.0.6/staticvar/__init__.py
+-rw-r--r--   0        0        0     2084 2023-04-14 22:41:09.473574 staticvar-0.0.6/staticvar/Static.py
+-rw-r--r--   0        0        0     3851 1970-01-01 00:00:00.000000 staticvar-0.0.6/PKG-INFO
```

### Comparing `staticvar-0.0.5/LICENSE.txt` & `staticvar-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `staticvar-0.0.5/README.md` & `staticvar-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# StaticVar
+# staticvar
  A module that adds the horrors of C Static variables to Python, with Python. <br><br>
 
 > In programming, a static variable is the one allocated “statically,” which means its lifetime is throughout the program run.
 
 [Learn About Static Variables in C](https://www.upgrad.com/blog/static-variable-in-c) <br><br>
 
 Python does not provide a quick native way to declare static variables. There are some *workarounds*, but they don't look very nice; so I made a module that does it for you. <br><br>
 
 Currently, this module only supports integer, float, string and boolean types. <br><br>
 
 #
-To get started, install StaticVar by typing the following in your command line:
+To get started, install staticvar by typing the following in your command line:
 
 ```
-pip install StaticVar
+pip install staticvar
 ```
 <br><br>
 
-In your project, import the StaticVar module as follows:
+In your project, import the staticvar module as follows:
 
 ```python
 from staticvar import Static
 ```
 <br>
 
 Next, declare the name of the static variable with its value and type as the arguments:
@@ -32,15 +32,15 @@
 ```
 Supported types include:
 - `"int"` for integer type variables
 - `"float"` for float type variables
 - `"str"` for string type variables
 - `"bool"` for boolean type variables
 
-Alternatively, if no type is passed, StaticVar will infer the type.
+Alternatively, if no type is passed, staticvar will infer the type.
 <br><br>
 
 To access the value of the variable, use the `get()` method:
 
 ```python
 print(foo.get())
 ```
@@ -73,15 +73,15 @@
 ```python
 print(foo.getType())
 ```
 Output:
 
 `> int`<br><br>
 
-Variables set using the StaticVar module are not dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
+Variables set using the staticvar module are not dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
 
 ```python
 foo.set(6.9) # A float value in an integer variable type will be casted as an integer
 print(foo.get())
 ```
 Output:
 
@@ -100,15 +100,15 @@
 ```python
 from staticvar import Static
 
 
 # Using recursion and static variables to find the factorial of a number
 def factorial(limit, reset = True):
 	count = Static(1, "int")
-	answer = Static(1) # If no type specified, StaticVar will infer the type
+	answer = Static(1) # If no type specified, staticvar will infer the type
 
 	if reset == True:
 		count.set(1)
 		answer.set(1)
 
 	if count.get() <= limit:
 		answer.set(answer.get() * (count.set(count.get() + 1) - 1))
```

### Comparing `staticvar-0.0.5/staticvar/Static.py` & `staticvar-0.0.6/staticvar/Static.py`

 * *Files identical despite different names*

### Comparing `staticvar-0.0.5/PKG-INFO` & `staticvar-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: staticvar
-Version: 0.0.5
+Version: 0.0.6
 Summary: The horrors of C Static variables for Python, with Python.
-Home-page: https://github.com/AbdelRahmanRahal/StaticVar
+Home-page: https://github.com/AbdelRahmanRahal/staticvar
 License: MIT
 Author: AbdelRahman
 Author-email: abdelrahman.rahal.mail@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: varname (>=0.11.0,<0.12.0)
-Project-URL: Repository, https://github.com/AbdelRahmanRahal/StaticVar
+Project-URL: Repository, https://github.com/AbdelRahmanRahal/staticvar
 Description-Content-Type: text/markdown
 
-# StaticVar
+# staticvar
  A module that adds the horrors of C Static variables to Python, with Python. <br><br>
 
 > In programming, a static variable is the one allocated “statically,” which means its lifetime is throughout the program run.
 
 [Learn About Static Variables in C](https://www.upgrad.com/blog/static-variable-in-c) <br><br>
 
 Python does not provide a quick native way to declare static variables. There are some *workarounds*, but they don't look very nice; so I made a module that does it for you. <br><br>
 
 Currently, this module only supports integer, float, string and boolean types. <br><br>
 
 #
-To get started, install StaticVar by typing the following in your command line:
+To get started, install staticvar by typing the following in your command line:
 
 ```
-pip install StaticVar
+pip install staticvar
 ```
 <br><br>
 
-In your project, import the StaticVar module as follows:
+In your project, import the staticvar module as follows:
 
 ```python
 from staticvar import Static
 ```
 <br>
 
 Next, declare the name of the static variable with its value and type as the arguments:
@@ -53,15 +52,15 @@
 ```
 Supported types include:
 - `"int"` for integer type variables
 - `"float"` for float type variables
 - `"str"` for string type variables
 - `"bool"` for boolean type variables
 
-Alternatively, if no type is passed, StaticVar will infer the type.
+Alternatively, if no type is passed, staticvar will infer the type.
 <br><br>
 
 To access the value of the variable, use the `get()` method:
 
 ```python
 print(foo.get())
 ```
@@ -94,15 +93,15 @@
 ```python
 print(foo.getType())
 ```
 Output:
 
 `> int`<br><br>
 
-Variables set using the StaticVar module are not dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
+Variables set using the staticvar module are not dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
 
 ```python
 foo.set(6.9) # A float value in an integer variable type will be casted as an integer
 print(foo.get())
 ```
 Output:
 
@@ -121,15 +120,15 @@
 ```python
 from staticvar import Static
 
 
 # Using recursion and static variables to find the factorial of a number
 def factorial(limit, reset = True):
 	count = Static(1, "int")
-	answer = Static(1) # If no type specified, StaticVar will infer the type
+	answer = Static(1) # If no type specified, staticvar will infer the type
 
 	if reset == True:
 		count.set(1)
 		answer.set(1)
 
 	if count.get() <= limit:
 		answer.set(answer.get() * (count.set(count.get() + 1) - 1))
```

