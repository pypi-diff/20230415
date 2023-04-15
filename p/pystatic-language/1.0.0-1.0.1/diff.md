# Comparing `tmp/pystatic-language-1.0.0.tar.gz` & `tmp/pystatic-language-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystatic-language-1.0.0.tar", last modified: Tue Mar 28 10:21:02 2023, max compression
+gzip compressed data, was "pystatic-language-1.0.1.tar", last modified: Sat Apr 15 12:25:21 2023, max compression
```

## Comparing `pystatic-language-1.0.0.tar` & `pystatic-language-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 10:21:02.421717 pystatic-language-1.0.0/
--rw-rw-rw-   0        0        0      115 2023-03-28 10:21:02.000000 pystatic-language-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8940 2023-03-28 10:21:02.420714 pystatic-language-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7852 2023-03-16 09:20:24.000000 pystatic-language-1.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.0.0/build.py
--rw-rw-rw-   0        0        0      925 2023-03-28 10:21:02.000000 pystatic-language-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-28 10:21:02.402576 pystatic-language-1.0.0/pystatic/
--rw-rw-rw-   0        0        0     4714 2023-03-10 17:43:12.000000 pystatic-language-1.0.0/pystatic/base.py
--rw-rw-rw-   0        0        0     8401 2023-03-20 21:44:09.000000 pystatic-language-1.0.0/pystatic/casting.py
--rw-rw-rw-   0        0        0     1315 2023-03-10 17:42:36.000000 pystatic-language-1.0.0/pystatic/clean.py
--rw-rw-rw-   0        0        0      489 2023-03-16 09:08:51.000000 pystatic-language-1.0.0/pystatic/document.py
--rw-rw-rw-   0        0        0     4178 2023-03-11 17:32:18.000000 pystatic-language-1.0.0/pystatic/overload.py
--rw-rw-rw-   0        0        0     5857 2023-03-12 10:31:25.000000 pystatic-language-1.0.0/pystatic/private.py
--rw-rw-rw-   0        0        0     8748 2023-03-10 17:45:57.000000 pystatic-language-1.0.0/pystatic/types.py
-drwxrwxrwx   0        0        0        0 2023-03-28 10:21:02.419738 pystatic-language-1.0.0/pystatic_language.egg-info/
--rw-rw-rw-   0        0        0     8940 2023-03-28 10:21:02.000000 pystatic-language-1.0.0/pystatic_language.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-03-28 10:21:02.000000 pystatic-language-1.0.0/pystatic_language.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 10:21:02.000000 pystatic-language-1.0.0/pystatic_language.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-03-28 10:21:02.000000 pystatic-language-1.0.0/pystatic_language.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-28 10:21:02.000000 pystatic-language-1.0.0/pystatic_language.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 10:21:02.421717 pystatic-language-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-03-28 10:20:53.000000 pystatic-language-1.0.0/setup.py
--rw-rw-rw-   0        0        0     2874 2023-03-16 09:19:38.000000 pystatic-language-1.0.0/test.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:25:21.632373 pystatic-language-1.0.1/
+-rw-rw-rw-   0        0        0      115 2023-04-15 12:25:21.000000 pystatic-language-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8940 2023-04-15 12:25:21.632373 pystatic-language-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7852 2023-03-16 09:20:24.000000 pystatic-language-1.0.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.0.1/build.py
+-rw-rw-rw-   0        0        0      925 2023-04-15 12:25:21.000000 pystatic-language-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-15 12:25:21.621371 pystatic-language-1.0.1/pystatic/
+-rw-rw-rw-   0        0        0     4714 2023-03-10 17:43:12.000000 pystatic-language-1.0.1/pystatic/base.py
+-rw-rw-rw-   0        0        0     8401 2023-03-20 21:44:09.000000 pystatic-language-1.0.1/pystatic/casting.py
+-rw-rw-rw-   0        0        0     1315 2023-03-10 17:42:36.000000 pystatic-language-1.0.1/pystatic/clean.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 09:08:51.000000 pystatic-language-1.0.1/pystatic/document.py
+-rw-rw-rw-   0        0        0     4178 2023-03-11 17:32:18.000000 pystatic-language-1.0.1/pystatic/overload.py
+-rw-rw-rw-   0        0        0     5874 2023-04-08 15:08:04.000000 pystatic-language-1.0.1/pystatic/private.py
+-rw-rw-rw-   0        0        0     8117 2023-04-15 12:24:30.000000 pystatic-language-1.0.1/pystatic/types.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:25:21.631372 pystatic-language-1.0.1/pystatic_language.egg-info/
+-rw-rw-rw-   0        0        0     8940 2023-04-15 12:25:21.000000 pystatic-language-1.0.1/pystatic_language.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-15 12:25:21.000000 pystatic-language-1.0.1/pystatic_language.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 12:25:21.000000 pystatic-language-1.0.1/pystatic_language.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-15 12:25:21.000000 pystatic-language-1.0.1/pystatic_language.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 12:25:21.000000 pystatic-language-1.0.1/pystatic_language.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.0.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 12:25:21.632373 pystatic-language-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-04-15 12:25:17.000000 pystatic-language-1.0.1/setup.py
+-rw-rw-rw-   0        0        0     2874 2023-04-08 15:05:57.000000 pystatic-language-1.0.1/test.py
```

### Comparing `pystatic-language-1.0.0/PKG-INFO` & `pystatic-language-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.0.0/README.md` & `pystatic-language-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.0/build.py` & `pystatic-language-1.0.1/build.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.0/pyproject.toml` & `pystatic-language-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pystatic-language'
-version = '1.0.0'
+version = '1.0.1'
 description = "This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and."
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pystatic-language-1.0.0/pystatic/base.py` & `pystatic-language-1.0.1/pystatic/base.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.0/pystatic/casting.py` & `pystatic-language-1.0.1/pystatic/casting.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.0/pystatic/clean.py` & `pystatic-language-1.0.1/pystatic/clean.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.0/pystatic/overload.py` & `pystatic-language-1.0.1/pystatic/overload.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.0/pystatic/private.py` & `pystatic-language-1.0.1/pystatic/private.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         :param instance: The instance of the class.
         :param owner: The class type of the instance.
 
         :return: The attribute's value.
         """
 
-        self.instance = instance
+        self.instance = instance or self.instance
 
         inside = in_scope(self.instance, levels=4)
 
         if not inside:
             raise AttributeError(
                 error_message(self.instance, self.name)
             )
```

### Comparing `pystatic-language-1.0.0/pystatic/types.py` & `pystatic-language-1.0.1/pystatic/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -93,21 +93,16 @@
     :returns: The inner wrapper function.
     """
 
     if crush is None:
         crush = Config.crush
     # end if
 
-    if excluded_names is None:
-        excluded_names = ''
-    # end if
-
-    if excluded_hints is None:
-        excluded_hints = ''
-    # end if
+    excluded_names = excluded_names or ()
+    excluded_hints = excluded_hints or ()
 
     # noinspection PyShadowingNames
     def wrap_call(*args: Any, **kwargs: Any) -> Any:
         """
         Wraps a callable object with runtime type enforcement.
 
         :param args: Any positional argument.
@@ -120,30 +115,14 @@
 
         bound = signature.bind(*args, **kwargs)
         bound.apply_defaults()
 
         parameters = dict(zip(signature.parameters, bound.args))
         parameters.update(bound.kwargs)
 
-        try:
-            # noinspection PyUnresolvedReferences,PyUnboundLocalVariable
-            if excluded_hints is None:
-                excluded_hints = tuple()
-            # end if
-
-            # noinspection PyUnresolvedReferences,PyUnboundLocalVariable
-            if excluded_names is None:
-                excluded_names = tuple()
-            # end if
-        
-        except UnboundLocalError:
-            excluded_hints = tuple()
-            excluded_names = tuple()
-        # end try
-
         for key, value in obj.__annotations__.items():
             # noinspection PyUnboundLocalVariable
             if any(
                 [
                     (key == "return"),
                     (key in excluded_names),
                     (value in excluded_hints)
@@ -198,15 +177,15 @@
                 # end if
             # end try
         # end if
 
         return data
     # end wrap_call
 
-    if ((excluded_names, excluded_hints) == ('', '')) and obj is not None:
+    if obj is not None:
         return wrap_call
     
     else:
         # noinspection PyShadowingNames
         def wrap_wrapper(value: Union[Type, Callable]) -> Callable:
             """
             Wraps a callable object with runtime type enforcement.
```

### Comparing `pystatic-language-1.0.0/pystatic_language.egg-info/PKG-INFO` & `pystatic-language-1.0.1/pystatic_language.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.0.0/setup.py` & `pystatic-language-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pystatic-language',
-        version='1.0.0',
+        version='1.0.1',
         description=(
             "This package is a collection of methods and classes for "
             "making python more secure, robust, and reliable. "
             "This could be achieved through the simple usage of decorators, "
             "function calls and inheritance of base classes. "
             "Generally, this package can make python a programming language, "
             "closer to other static-typed languages, "
```

### Comparing `pystatic-language-1.0.0/test.py` & `pystatic-language-1.0.1/test.py`

 * *Files identical despite different names*

