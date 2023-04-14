# Comparing `tmp/StaticVar-0.0.4.tar.gz` & `tmp/staticvar-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StaticVar-0.0.4.tar", last modified: Fri Apr 14 12:33:12 2023, max compression
+gzip compressed data, was "staticvar-0.0.5.tar", max compression
```

## Comparing `StaticVar-0.0.4.tar` & `staticvar-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:33:12.246792 StaticVar-0.0.4/
--rw-rw-rw-   0        0        0     1080 2023-04-14 12:04:40.000000 StaticVar-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      670 2023-04-14 12:33:12.246792 StaticVar-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3164 2023-04-14 12:32:53.000000 StaticVar-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 12:33:12.240179 StaticVar-0.0.4/StaticVar.egg-info/
--rw-rw-rw-   0        0        0      670 2023-04-14 12:33:12.000000 StaticVar-0.0.4/StaticVar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-04-14 12:33:12.000000 StaticVar-0.0.4/StaticVar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:33:12.000000 StaticVar-0.0.4/StaticVar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 12:33:12.000000 StaticVar-0.0.4/StaticVar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:33:12.000000 StaticVar-0.0.4/StaticVar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 12:33:12.246792 StaticVar-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-04-14 12:31:43.000000 StaticVar-0.0.4/setup.py
+-rw-r--r--   0        0        0     1080 2023-04-14 22:15:59.466307 staticvar-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      696 2023-04-14 22:15:59.466307 staticvar-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3195 2023-04-14 22:15:59.466307 staticvar-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 22:15:59.476249 staticvar-0.0.5/staticvar/__init__.py
+-rw-r--r--   0        0        0     2084 2023-04-14 22:15:59.476249 staticvar-0.0.5/staticvar/Static.py
+-rw-r--r--   0        0        0     3907 1970-01-01 00:00:00.000000 staticvar-0.0.5/PKG-INFO
```

### Comparing `StaticVar-0.0.4/LICENSE.txt` & `staticvar-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `StaticVar-0.0.4/README.md` & `staticvar-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # StaticVar
- A module that adds static variables to Python. <br><br>
+ A module that adds the horrors of C Static variables to Python, with Python. <br><br>
 
 > In programming, a static variable is the one allocated “statically,” which means its lifetime is throughout the program run.
 
-[Learn About Static Variable in C](https://www.upgrad.com/blog/static-variable-in-c) <br><br>
+[Learn About Static Variables in C](https://www.upgrad.com/blog/static-variable-in-c) <br><br>
 
 Python does not provide a quick native way to declare static variables. There are some *workarounds*, but they don't look very nice; so I made a module that does it for you. <br><br>
 
 Currently, this module only supports integer, float, string and boolean types. <br><br>
 
 #
 To get started, install StaticVar by typing the following in your command line:
@@ -16,15 +16,15 @@
 pip install StaticVar
 ```
 <br><br>
 
 In your project, import the StaticVar module as follows:
 
 ```python
-from StaticVar import Static
+from staticvar import Static
 ```
 <br>
 
 Next, declare the name of the static variable with its value and type as the arguments:
 
 ```python
 # Syntax: VARIABLE_NAME = Static(VALUE, "TYPE")
@@ -94,15 +94,15 @@
 Output:
 
 `> ValueError: invalid literal for int() with base 10: 'Hello, mum!'`<br><br><br>
 
 # An example on how to utilise static variables in a simple program
 Though there are better ways to do it, we can use static variables to find the factorial of a number.
 ```python
-from StaticVar import Static
+from staticvar import Static
 
 
 # Using recursion and static variables to find the factorial of a number
 def factorial(limit, reset = True):
 	count = Static(1, "int")
 	answer = Static(1) # If no type specified, StaticVar will infer the type
```

