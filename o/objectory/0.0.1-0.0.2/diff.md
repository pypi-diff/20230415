# Comparing `tmp/objectory-0.0.1.tar.gz` & `tmp/objectory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectory-0.0.1.tar", max compression
+gzip compressed data, was "objectory-0.0.2.tar", max compression
```

## Comparing `objectory-0.0.1.tar` & `objectory-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1501 2023-01-02 06:47:45.108954 objectory-0.0.1/LICENSE
--rw-r--r--   0        0        0     4097 2023-01-02 06:47:45.108954 objectory-0.0.1/README.md
--rw-r--r--   0        0        0     2249 2023-01-02 06:47:45.108954 objectory-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      280 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/__init__.py
--rw-r--r--   0        0        0    12974 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/abstract_factory.py
--rw-r--r--   0        0        0      138 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/constants.py
--rw-r--r--   0        0        0     1471 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/errors.py
--rw-r--r--   0        0        0    15891 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/registry.py
--rw-r--r--   0        0        0     1255 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/universal.py
--rw-r--r--   0        0        0      373 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/utils/__init__.py
--rw-r--r--   0        0        0     3185 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/utils/name_resolution.py
--rw-r--r--   0        0        0     7397 2023-01-02 06:47:45.108954 objectory-0.0.1/src/objectory/utils/object_helpers.py
--rw-r--r--   0        0        0     5003 1970-01-01 00:00:00.000000 objectory-0.0.1/setup.py
--rw-r--r--   0        0        0     5309 1970-01-01 00:00:00.000000 objectory-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-04-15 03:59:42.869678 objectory-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3948 2023-04-15 03:59:42.869678 objectory-0.0.2/README.md
+-rw-r--r--   0        0        0     3888 2023-04-15 03:59:42.869678 objectory-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/__init__.py
+-rw-r--r--   0        0        0    12973 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/abstract_factory.py
+-rw-r--r--   0        0        0      138 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/constants.py
+-rw-r--r--   0        0        0     1471 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/errors.py
+-rw-r--r--   0        0        0    16025 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/registry.py
+-rw-r--r--   0        0        0     1255 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/universal.py
+-rw-r--r--   0        0        0      373 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/utils/__init__.py
+-rw-r--r--   0        0        0     3185 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/utils/name_resolution.py
+-rw-r--r--   0        0        0     7397 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/utils/object_helpers.py
+-rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 objectory-0.0.2/PKG-INFO
```

### Comparing `objectory-0.0.1/LICENSE` & `objectory-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `objectory-0.0.1/README.md` & `objectory-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # objectory = object + factory
 
 <p align="center">
-   <a href="https://github.com/durandtibo/objectory/actions">
-      <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/CI/badge.svg?event=push&branch=main">
-   </a>
+    <a href="https://github.com/durandtibo/objectory/actions">
+        <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/CI/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://pypi.org/project/objectory/">
+        <img alt="PYPI version" src="https://img.shields.io/pypi/v/objectory">
+    </a>
     <a href="https://pypi.org/project/objectory/">
-      <img alt="PYPI version" src="https://img.shields.io/pypi/v/objectory">
+        <img alt="Python" src="https://img.shields.io/pypi/pyversions/objectory.svg">
+    </a>
+    <a href="https://opensource.org/licenses/BSD-3-Clause">
+        <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/objectory">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/objectory">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://github.com/psf/black">
+        <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+    </a>
+    <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
+        <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
     </a>
-   <a href="https://pypi.org/project/objectory/">
-      <img alt="Python" src="https://img.shields.io/pypi/pyversions/objectory.svg">
-   </a>
-   <a href="https://opensource.org/licenses/BSD-3-Clause">
-      <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/objectory">
-   </a>
-   <a href="https://codecov.io/gh/durandtibo/objectory">
-      <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
-   </a>
-   <a href="https://github.com/psf/black">
-     <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
-   </a>
-   <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
-     <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
-   </a>
-   <br/>
+    <br/>
+    <a href="https://pepy.tech/project/objectory">
+        <img  alt="Downloads" src="https://static.pepy.tech/badge/objectory">
+    </a>
+    <a href="https://pepy.tech/project/objectory">
+        <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/objectory/month">
+    </a>
+    <br/>
 </p>
 
 ## Overview
 
 A light Python library for general purpose object factories.
 In particular, it focuses on dynamic object factory implementations where objects can be registered
 dynamically without changing the code of the factory.
@@ -112,25 +119,15 @@
 ```
 
 Please check the [get started page](https://durandtibo.github.io/objectory/get_started) to see other
 alternatives to install the library.
 
 ## Contributing
 
-Please let us know if you encounter a bug by filing an issue.
-
-We welcome contributions from anyone, even if you are new to open source.
-
-- If you are planning to contribute back bug-fixes, please do so without any further discussion.
-- If you plan to contribute new features, utility functions, or extensions to the core, please first
-  open an issue and discuss the feature with us.
-
-Once you implement and test your feature or bug-fix, please submit a Pull Request.
-
-Please feel free to open an issue to share your feedback or to request new features.
+Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
 
 ## API stability
 
 :warning: While `objectory` is in development stage, no API is guaranteed to be stable from one
 release to the next.
 In fact, it is very likely that the API will change multiple times before a stable 1.0.0 release.
 In practice, this means that upgrading `objectory` to a new version will possibly break any code
```

### Comparing `objectory-0.0.1/src/objectory/abstract_factory.py` & `objectory-0.0.2/src/objectory/abstract_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,30 +45,30 @@
             which the class inherits.
             This becomes the ``__bases__`` attribute of the class.
         dct (dict): Specifies a namespace dictionary containing
             definitions for the class body.
             This becomes the ``__dict__`` attribute of the class.
     """
 
-    def __init__(self, name: str, bases: tuple, dct: dict):
-        if not hasattr(self, "_abstractfactory_inheritors"):
-            self._abstractfactory_inheritors = {}
-        self.register_object(self)
+    def __init__(cls, name: str, bases: tuple, dct: dict) -> None:
+        if not hasattr(cls, "_abstractfactory_inheritors"):
+            cls._abstractfactory_inheritors = {}
+        cls.register_object(cls)
         super().__init__(name, bases, dct)
 
     @property
-    def inheritors(self) -> dict[str, Any]:
+    def inheritors(cls) -> dict[str, Any]:
         r"""Gets the inheritors.
 
         Returns:
             dict: The inheritors.
         """
-        return self._abstractfactory_inheritors
+        return cls._abstractfactory_inheritors
 
-    def factory(self, _target_: str, *args, _init_: str = "__init__", **kwargs) -> Any:
+    def factory(cls, _target_: str, *args, _init_: str = "__init__", **kwargs) -> Any:
         r"""Creates dynamically an object given its configuration.
 
         Please read the documentation for more information.
 
         Args:
             _target_ (str): Specifies the name of the object
                 (class or function) to instantiate.
@@ -97,18 +97,18 @@
             ...     pass
             >>> class MyClass(BaseClass):
             ...     pass
             >>> BaseClass.factory("MyClass")
             <__main__.MyClass object at 0x123456789>
         """
         return instantiate_object(
-            self._abstractfactory_get_target_from_name(_target_), *args, _init_=_init_, **kwargs
+            cls._abstractfactory_get_target_from_name(_target_), *args, _init_=_init_, **kwargs
         )
 
-    def register_object(self, obj: Union[type, Callable]) -> None:
+    def register_object(cls, obj: Union[type, Callable]) -> None:
         r"""Registers a class or function to the factory. It is useful if you
         are using a 3rd party library.
 
         For example, you use a 3rd party library, and you cannot
         modify the classes to add ``AbstractFactory``. You can use
         this function to register some classes or functions of a
         3rd party library.
@@ -131,25 +131,25 @@
             >>> class MyClass:
             ...     pass
             >>> BaseClass.register_object(MyClass)
             >>> BaseClass.inheritors
             {'__main__.BaseClass': <class '__main__.BaseClass'>,
              '__main__.MyClass': <class '__main__.MyClass'>}
         """
-        self._abstractfactory_check_object(obj)
+        cls._abstractfactory_check_object(obj)
         name = full_object_name(obj)
         if (
-            self._abstractfactory_is_name_registered(name)
-            and self._abstractfactory_inheritors[name] != obj
+            cls._abstractfactory_is_name_registered(name)
+            and cls._abstractfactory_inheritors[name] != obj
         ):
             logger.warning(f"The class {name} already exists. The new class replaces the old one")
 
-        self._abstractfactory_inheritors[name] = obj
+        cls._abstractfactory_inheritors[name] = obj
 
-    def unregister(self, name: str) -> None:
+    def unregister(cls, name: str) -> None:
         r"""Removes a registered object from the factory.
 
         This is an experimental function and may change in the future.
 
         Args:
             name (string): Specifies the name of the object to remove.
                 This function uses the name resolution mechanism to
@@ -165,45 +165,45 @@
             >>> class MyClass:
             ...     pass
             >>> BaseClass.register_object(MyClass)
             >>> BaseClass.unregister("MyClass")
             >>> BaseClass.inheritors
             {'__main__.BaseClass': <class '__main__.BaseClass'>}
         """
-        resolved_name = self._abstractfactory_resolve_name(name)
-        if resolved_name is None or not self._abstractfactory_is_name_registered(resolved_name):
+        resolved_name = cls._abstractfactory_resolve_name(name)
+        if resolved_name is None or not cls._abstractfactory_is_name_registered(resolved_name):
             raise UnregisteredObjectFactoryError(
                 f"It is not possible to remove an object which is not registered (received: {name})"
             )
-        self._abstractfactory_inheritors.pop(resolved_name)
+        cls._abstractfactory_inheritors.pop(resolved_name)
 
-    def _abstractfactory_get_target_from_name(self, name: str) -> Any:
+    def _abstractfactory_get_target_from_name(cls, name: str) -> Union[type, Callable]:
         """Gets the class or function to used given its name.
 
         Args:
             name (str): Specifies the name of the class or function.
 
         Returns:
             The class or function.
 
         Raises:
             ``UnregisteredObjectFactoryError`` if it is not possible
                 to find the target.
         """
-        resolved_name = self._abstractfactory_resolve_name(name)
+        resolved_name = cls._abstractfactory_resolve_name(name)
         if resolved_name is None:
             raise UnregisteredObjectFactoryError(
-                f"Unable to create the object {name}. Registered objects of {self.__qualname__} "
-                f"are {set(self._abstractfactory_inheritors.keys())}"
+                f"Unable to create the object {name}. Registered objects of {cls.__qualname__} "
+                f"are {set(cls._abstractfactory_inheritors.keys())}"
             )
-        if not self._abstractfactory_is_name_registered(resolved_name):
-            self.register_object(import_object(resolved_name))
-        return self._abstractfactory_inheritors[resolved_name]
+        if not cls._abstractfactory_is_name_registered(resolved_name):
+            cls.register_object(import_object(resolved_name))
+        return cls._abstractfactory_inheritors[resolved_name]
 
-    def _abstractfactory_resolve_name(self, name: str) -> Optional[str]:
+    def _abstractfactory_resolve_name(cls, name: str) -> Optional[str]:
         r"""Tries to resolve the name.
 
         This function will look at if it can find an object which
         match with the given name. It is quite useful because there
         are several ways to load an object but only one can be
         registered. If you specify a full name (module path +
         class/function name), it will try to import the module
@@ -214,28 +214,28 @@
                 to resolve.
 
         Returns:
             ``str`` or ``None``: It returns the name to use to get
                 the object if the resolution was successful,
                 otherwise ``None``.
         """
-        return resolve_name(name, set(self._abstractfactory_inheritors.keys()))
+        return resolve_name(name, set(cls._abstractfactory_inheritors.keys()))
 
-    def _abstractfactory_is_name_registered(self, name: str) -> bool:
+    def _abstractfactory_is_name_registered(cls, name: str) -> bool:
         r"""Indicates if the name exists or not in the factory .
 
         Args:
             name (str): Specifies the name to check.
 
         Returns:
             bool: ``True`` if the name exists otherwise ``False``.
         """
-        return name in self._abstractfactory_inheritors
+        return name in cls._abstractfactory_inheritors
 
-    def _abstractfactory_check_object(self, obj: type) -> None:  # pylint: disable=no-self-use
+    def _abstractfactory_check_object(cls, obj: type) -> None:
         r"""Checks if the object is valid for this factory before to register
         it.
 
         This function will raise an exception if the object is not
         valid.
 
         Args:
@@ -252,15 +252,15 @@
         if is_lambda_function(obj):
             raise IncorrectObjectFactoryError(
                 "It is not possible to register a lambda function. "
                 "Please use a regular function instead"
             )
 
 
-def register(cls: AbstractFactory):
+def register(cls: AbstractFactory) -> Callable:
     r"""Defines a decorator to register a function to a factory.
 
     This decorator is designed to register functions that returns
     an object of a class registered in the factory.
 
     Args:
         cls (``AbstractFactory``): Specifies the class where to
@@ -276,15 +276,15 @@
         >>> @register(BaseClass)
         ... def function_to_register(value: int) -> int:
         ...     return value + 2
         >>> BaseClass.factory('function_to_register', 40)
         42
     """
 
-    def wrapped(func):
+    def wrapped(func: Callable) -> Callable:
         cls.register_object(func)
         return func
 
     return wrapped
 
 
 def register_child_classes(
```

### Comparing `objectory-0.0.1/src/objectory/errors.py` & `objectory-0.0.2/src/objectory/errors.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.1/src/objectory/registry.py` & `objectory-0.0.2/src/objectory/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""This module implements a registry class."""
 
 __all__ = ["Registry"]
 
 import inspect
 import logging
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, TypeVar, Union
 
 from objectory.errors import (
     IncorrectObjectFactoryError,
     InvalidAttributeRegistryError,
     InvalidNameFactoryError,
     UnregisteredObjectFactoryError,
 )
@@ -19,29 +19,31 @@
     instantiate_object,
     is_lambda_function,
     resolve_name,
 )
 
 logger = logging.getLogger(__name__)
 
+T = TypeVar("T")
+
 
 class Registry:
     r"""Implementation of the registry class.
 
     This class can be used to register some objects and instantiate an
     object from its configuration.
     """
 
     _CLASS_FILTER = "class_filter"
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._state = {}
         self._filters = {}
 
-    def __getattr__(self, key):
+    def __getattr__(self, key: str) -> Union["Registry", type]:
         if key not in self._state:
             self._state[key] = Registry()
         if self._is_registry(key):
             return self._state[key]
         raise InvalidAttributeRegistryError(
             f"The attribute {key} is not a registry. You can use this function only to access "
             "a Registry object."
@@ -177,21 +179,21 @@
             >>> @registry.register()
             ... def function_to_register(*args, **kwargs):
             ...     ...
             >>> registry.registered_names()
             {'__main__.ClassToRegister', '__main__.function_to_register'}
         """
 
-        def function_wrapper(obj):
+        def function_wrapper(obj: T) -> T:
             self.register_object(obj=obj, name=name)
             return obj
 
         return function_wrapper
 
-    def register_child_classes(self, cls, ignore_abstract_class: bool = True) -> None:
+    def register_child_classes(self, cls: type, ignore_abstract_class: bool = True) -> None:
         r"""Registers a given class and its child classes of a given class.
 
         This function registers all the child classes including the
         child classes of the child classes, etc. If you use this
         function, you cannot choose the names used to register the
         objects. It will use the full name of each object.
 
@@ -214,15 +216,15 @@
              'collections.Counter', 'builtins.dict', 'collections.OrderedDict'}
         """
         for class_to_register in [cls] + list(all_child_classes(cls)):
             if ignore_abstract_class and inspect.isabstract(class_to_register):
                 continue
             self.register_object(class_to_register)
 
-    def register_object(self, obj, name: Optional[str] = None) -> None:
+    def register_object(self, obj: Union[type, Callable], name: Optional[str] = None) -> None:
         r"""Registers an object.
 
         Please read the documentation for more information.
 
         Args:
             obj: Specifies the object to register. The object is
                 expected to be a class or a function.
@@ -355,15 +357,15 @@
             self._filters.pop(self._CLASS_FILTER, None)
             return
 
         if not inspect.isclass(cls):
             raise TypeError(f"The class filter has to be a class (received: {cls})")
         self._filters[self._CLASS_FILTER] = cls
 
-    def _check_object(self, obj) -> None:
+    def _check_object(self, obj: Union[type, Callable]) -> None:
         r"""Checks if the object is valid for this registry before to register
         it.
 
         This function will raise an exception if the object is not
         valid.
 
         Args:
```

### Comparing `objectory-0.0.1/src/objectory/universal.py` & `objectory-0.0.2/src/objectory/universal.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.1/src/objectory/utils/name_resolution.py` & `objectory-0.0.2/src/objectory/utils/name_resolution.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.1/src/objectory/utils/object_helpers.py` & `objectory-0.0.2/src/objectory/utils/object_helpers.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.1/PKG-INFO` & `objectory-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: objectory
-Version: 0.0.1
+Version: 0.0.2
 Summary: A light library for general purpose object factories
 Home-page: https://github.com/durandtibo/objectory
 License: BSD-3-Clause
 Keywords: factory,abstract factory,registry
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -26,36 +26,43 @@
 Requires-Dist: tornado (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/durandtibo/objectory
 Description-Content-Type: text/markdown
 
 # objectory = object + factory
 
 <p align="center">
-   <a href="https://github.com/durandtibo/objectory/actions">
-      <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/CI/badge.svg?event=push&branch=main">
-   </a>
+    <a href="https://github.com/durandtibo/objectory/actions">
+        <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/CI/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://pypi.org/project/objectory/">
+        <img alt="PYPI version" src="https://img.shields.io/pypi/v/objectory">
+    </a>
     <a href="https://pypi.org/project/objectory/">
-      <img alt="PYPI version" src="https://img.shields.io/pypi/v/objectory">
+        <img alt="Python" src="https://img.shields.io/pypi/pyversions/objectory.svg">
+    </a>
+    <a href="https://opensource.org/licenses/BSD-3-Clause">
+        <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/objectory">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/objectory">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://github.com/psf/black">
+        <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+    </a>
+    <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
+        <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
     </a>
-   <a href="https://pypi.org/project/objectory/">
-      <img alt="Python" src="https://img.shields.io/pypi/pyversions/objectory.svg">
-   </a>
-   <a href="https://opensource.org/licenses/BSD-3-Clause">
-      <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/objectory">
-   </a>
-   <a href="https://codecov.io/gh/durandtibo/objectory">
-      <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
-   </a>
-   <a href="https://github.com/psf/black">
-     <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
-   </a>
-   <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
-     <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
-   </a>
-   <br/>
+    <br/>
+    <a href="https://pepy.tech/project/objectory">
+        <img  alt="Downloads" src="https://static.pepy.tech/badge/objectory">
+    </a>
+    <a href="https://pepy.tech/project/objectory">
+        <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/objectory/month">
+    </a>
+    <br/>
 </p>
 
 ## Overview
 
 A light Python library for general purpose object factories.
 In particular, it focuses on dynamic object factory implementations where objects can be registered
 dynamically without changing the code of the factory.
@@ -141,25 +148,15 @@
 ```
 
 Please check the [get started page](https://durandtibo.github.io/objectory/get_started) to see other
 alternatives to install the library.
 
 ## Contributing
 
-Please let us know if you encounter a bug by filing an issue.
-
-We welcome contributions from anyone, even if you are new to open source.
-
-- If you are planning to contribute back bug-fixes, please do so without any further discussion.
-- If you plan to contribute new features, utility functions, or extensions to the core, please first
-  open an issue and discuss the feature with us.
-
-Once you implement and test your feature or bug-fix, please submit a Pull Request.
-
-Please feel free to open an issue to share your feedback or to request new features.
+Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
 
 ## API stability
 
 :warning: While `objectory` is in development stage, no API is guaranteed to be stable from one
 release to the next.
 In fact, it is very likely that the API will change multiple times before a stable 1.0.0 release.
 In practice, this means that upgrading `objectory` to a new version will possibly break any code
```

