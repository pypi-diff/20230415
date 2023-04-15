# Comparing `tmp/drf_pydantic-0.4.0.tar.gz` & `tmp/drf_pydantic-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic-0.4.0.tar", max compression
+gzip compressed data, was "drf_pydantic-0.4.1.tar", max compression
```

## Comparing `drf_pydantic-0.4.0.tar` & `drf_pydantic-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-07 02:15:45.269589 drf_pydantic-0.4.0/LICENSE
--rw-r--r--   0        0        0     3475 2023-04-07 02:15:45.269589 drf_pydantic-0.4.0/README.md
--rw-r--r--   0        0        0     2148 2023-04-07 02:15:45.273589 drf_pydantic-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       66 2023-04-07 02:15:45.273589 drf_pydantic-0.4.0/src/drf_pydantic/__init__.py
--rw-r--r--   0        0        0      626 2023-04-07 02:15:45.273589 drf_pydantic-0.4.0/src/drf_pydantic/base_model.py
--rw-r--r--   0        0        0     5637 2023-04-07 02:15:45.273589 drf_pydantic-0.4.0/src/drf_pydantic/parse.py
--rw-r--r--   0        0        0     4740 1970-01-01 00:00:00.000000 drf_pydantic-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3481 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/README.md
+-rw-r--r--   0        0        0     2148 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/src/drf_pydantic/__init__.py
+-rw-r--r--   0        0        0      626 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/src/drf_pydantic/base_model.py
+-rw-r--r--   0        0        0     6029 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/src/drf_pydantic/parse.py
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 drf_pydantic-0.4.1/PKG-INFO
```

### Comparing `drf_pydantic-0.4.0/LICENSE` & `drf_pydantic-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic-0.4.0/README.md` & `drf_pydantic-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
-  <a href="https://github.com/georgebv/drf-pydantic/actions/workflows/cicd.yml" target="_blank">
-    <img src="https://github.com/georgebv/drf-pydantic/actions/workflows/cicd.yml/badge.svg?branch=main" alt="CI/CD Status">
+  <a href="https://github.com/georgebv/drf-pydantic/actions/workflows/test.yml" target="_blank">
+    <img src="https://github.com/georgebv/drf-pydantic/actions/workflows/test.yml/badge.svg?event=pull_request" alt="Test Status">
   </a>
   <a href="https://codecov.io/gh/georgebv/drf-pydantic" target="_blank">
     <img src="https://codecov.io/gh/georgebv/drf-pydantic/branch/main/graph/badge.svg?token=GN9rxzIFMc" alt="Test Coverage"/>
   </a>
   <a href="https://badge.fury.io/py/drf-pydantic" target="_blank">
     <img src="https://badge.fury.io/py/drf-pydantic.svg" alt="PyPI version" height="20">
   </a>
```

### Comparing `drf_pydantic-0.4.0/pyproject.toml` & `drf_pydantic-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pydantic"
-version = "0.4.0"
+version = "0.4.1"
 description = "Use pydantic with the Django REST framework"
 license = "MIT"
 authors = ["George Bocharov <bocharovgeorgii@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/georgebv/drf-pydantic"
 repository = "https://github.com/georgebv/drf-pydantic"
 keywords = ["django", "drf", "pydantic", "typing", "rest", "api"]
```

### Comparing `drf_pydantic-0.4.0/src/drf_pydantic/base_model.py` & `drf_pydantic-0.4.1/src/drf_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic-0.4.0/src/drf_pydantic/parse.py` & `drf_pydantic-0.4.1/src/drf_pydantic/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import decimal
 import inspect
 import types
 import typing
 import uuid
+import warnings
 
 import pydantic
 
 from rest_framework import serializers
 
 # Cache serializer classes to ensure that there is a one-to-one relationship
 # between pydantic models and serializer classes
@@ -90,46 +91,62 @@
     else:
         extra_kwargs["required"] = field.required
     if field.default is not None:
         extra_kwargs["default"] = field.default
     if field.allow_none:
         extra_kwargs["allow_null"] = True
         extra_kwargs["default"] = None
-    
-    #check if field._type is a subclass of ConstrainedNumberMeta
-    if issubclass(field.type_.__class__, pydantic.types.ConstrainedNumberMeta):
+
+    # Numeric field with constraints
+    if isinstance(field.type_, pydantic.types.ConstrainedNumberMeta):
         if field.type_.gt is not None:
-            extra_kwargs["min_value"] = field.type_.gt + 1
+            warnings.warn(
+                "gt (>) is not supported by DRF, using ge (>=) instead",
+                UserWarning,
+            )
+            extra_kwargs["min_value"] = field.type_.gt
         elif field.type_.ge is not None:
             extra_kwargs["min_value"] = field.type_.ge
         if field.type_.lt is not None:
-            extra_kwargs["max_value"] = field.type_.lt - 1
+            warnings.warn(
+                "lt (<) is not supported by DRF, using le (<=) instead",
+                UserWarning,
+            )
+            extra_kwargs["max_value"] = field.type_.lt
         elif field.type_.le is not None:
             extra_kwargs["max_value"] = field.type_.le
-    
-    #check if field._type is a subclass of ConstrainedStr
-    if inspect.isclass(field.type_) and issubclass(field.type_, pydantic.types.ConstrainedStr):
+
+    # String field with constraints
+    if inspect.isclass(field.type_) and issubclass(
+        field.type_, pydantic.types.ConstrainedStr
+    ):
         extra_kwargs["min_length"] = field.type_.min_length
         extra_kwargs["max_length"] = field.type_.max_length
-    
+
     # Scalar field
     if field.outer_type_ is field.type_:
         # Normal class
         if inspect.isclass(field.type_):
             return _convert_type(field.type_)(**extra_kwargs)
 
         # Alias
         if field.type_.__origin__ is typing.Literal:
             choices = field.type_.__args__
             assert all(isinstance(choice, str) for choice in choices)
             return serializers.ChoiceField(choices=choices, **extra_kwargs)
         raise NotImplementedError(f"{field.type_.__name__} is not yet supported")
 
     # Container field
-    assert isinstance(field.outer_type_, types.GenericAlias)
+    assert isinstance(
+        field.outer_type_,
+        (
+            types.GenericAlias,
+            getattr(typing, "_GenericAlias"),
+        ),
+    ), f"Unsupported container type '{field.outer_type_.__name__}'"
     if field.outer_type_.__origin__ is list or field.outer_type_.__origin__ is tuple:
         return serializers.ListField(child=_convert_type(field.type_)(**extra_kwargs))
     raise NotImplementedError(
         f"Container type '{field.outer_type_.__origin__.__name__}' is not yet supported"
     )
```

### Comparing `drf_pydantic-0.4.0/PKG-INFO` & `drf_pydantic-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pydantic
-Version: 0.4.0
+Version: 0.4.1
 Summary: Use pydantic with the Django REST framework
 Home-page: https://github.com/georgebv/drf-pydantic
 License: MIT
 Keywords: django,drf,pydantic,typing,rest,api
 Author: George Bocharov
 Author-email: bocharovgeorgii@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -25,16 +25,16 @@
 Classifier: Typing :: Typed
 Requires-Dist: djangorestframework (>=3.13.0,<4.0.0)
 Requires-Dist: pydantic[email] (>=1.9.0,<2.0.0)
 Project-URL: Repository, https://github.com/georgebv/drf-pydantic
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <a href="https://github.com/georgebv/drf-pydantic/actions/workflows/cicd.yml" target="_blank">
-    <img src="https://github.com/georgebv/drf-pydantic/actions/workflows/cicd.yml/badge.svg?branch=main" alt="CI/CD Status">
+  <a href="https://github.com/georgebv/drf-pydantic/actions/workflows/test.yml" target="_blank">
+    <img src="https://github.com/georgebv/drf-pydantic/actions/workflows/test.yml/badge.svg?event=pull_request" alt="Test Status">
   </a>
   <a href="https://codecov.io/gh/georgebv/drf-pydantic" target="_blank">
     <img src="https://codecov.io/gh/georgebv/drf-pydantic/branch/main/graph/badge.svg?token=GN9rxzIFMc" alt="Test Coverage"/>
   </a>
   <a href="https://badge.fury.io/py/drf-pydantic" target="_blank">
     <img src="https://badge.fury.io/py/drf-pydantic.svg" alt="PyPI version" height="20">
   </a>
```

