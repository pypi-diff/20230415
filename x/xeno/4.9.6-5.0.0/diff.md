# Comparing `tmp/xeno-4.9.6.tar.gz` & `tmp/xeno-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeno-4.9.6.tar", last modified: Sun Mar 21 08:10:58 2021, max compression
+gzip compressed data, was "xeno-5.0.0.tar", last modified: Fri Apr 14 23:10:26 2023, max compression
```

## Comparing `xeno-4.9.6.tar` & `xeno-5.0.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-03-21 08:10:58.755592 xeno-4.9.6/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       52 2021-03-21 05:19:20.000000 xeno-4.9.6/.gitignore
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      143 2021-03-21 05:19:20.000000 xeno-4.9.6/.travis.yml
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2018-03-14 08:05:20.000000 xeno-4.9.6/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2021-03-21 05:19:20.000000 xeno-4.9.6/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11299 2021-03-21 08:10:58.755592 xeno-4.9.6/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8982 2021-03-21 05:19:20.000000 xeno-4.9.6/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2021-03-21 08:10:58.755592 xeno-4.9.6/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1159 2021-03-21 08:10:31.000000 xeno-4.9.6/setup.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    28426 2021-03-21 05:19:20.000000 xeno-4.9.6/test.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-03-21 08:10:58.755592 xeno-4.9.6/xeno/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1839 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9951 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/abstract.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13130 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/async_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6394 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/attributes.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    28130 2021-03-21 08:08:45.000000 xeno-4.9.6/xeno/build.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2778 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/color.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4172 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/decorators.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/errors.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/namespaces.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5729 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/shell.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7309 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/sync_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2744 2021-03-21 05:19:20.000000 xeno-4.9.6/xeno/utils.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-03-21 08:10:58.755592 xeno-4.9.6/xeno.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11299 2021-03-21 08:10:58.000000 xeno-4.9.6/xeno.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      419 2021-03-21 08:10:58.000000 xeno-4.9.6/xeno.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2021-03-21 08:10:58.000000 xeno-4.9.6/xeno.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       20 2021-03-21 08:10:58.000000 xeno-4.9.6/xeno.egg-info/entry_points.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2021-03-21 08:10:58.000000 xeno-4.9.6/xeno.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-14 23:10:26.244811 xeno-5.0.0/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-04-03 20:39:53.000000 xeno-5.0.0/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-04-03 20:39:53.000000 xeno-5.0.0/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-14 23:10:26.244811 xeno-5.0.0/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-04-03 20:39:53.000000 xeno-5.0.0/README.md
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-14 23:10:26.244811 xeno-5.0.0/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-14 23:10:04.000000 xeno-5.0.0/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-14 23:10:26.244811 xeno-5.0.0/xeno/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/abstract.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/async_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/attributes.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    14309 2023-04-14 23:07:26.000000 xeno-5.0.0/xeno/build.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2956 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/color.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9804 2023-04-14 22:17:15.000000 xeno-5.0.0/xeno/cookbook.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/decorators.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/errors.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5436 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/events.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/namespaces.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/pkg_config.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19116 2023-04-14 22:53:16.000000 xeno-5.0.0/xeno/recipe.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6738 2023-04-14 22:25:58.000000 xeno-5.0.0/xeno/shell.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1559 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/spinner.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/sync_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/testing.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2965 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/utils.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-14 23:10:26.244811 xeno-5.0.0/xeno.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/top_level.txt
```

### Comparing `xeno-4.9.6/LICENSE` & `xeno-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno-4.9.6/PKG-INFO` & `xeno-5.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,228 +1,218 @@
-Metadata-Version: 2.1
-Name: xeno
-Version: 4.9.6
-Summary: The Python dependency injector from outer space.
-Home-page: https://github.com/lainproliant/xeno
-Author: Lain Musgrove (lainproliant)
-Author-email: lainproliant@gmail.com
-License: BSD
-Description: # Xeno: The Python dependency injector from outer space. 
-        [![Build Status](https://travis-ci.org/lainproliant/xeno.svg?branch=master)](https://travis-ci.org/lainproliant/xeno)
-        
-        Xeno is a simple Python dependency injection framework. Use it when you
-        need to manage complex inter-object dependencies in a clean way. For the
-        merits of dependency injection and IOC, see
-        https://en.wikipedia.org/wiki/Dependency_injection.
-        
-        Xeno should feel pretty familiar to users of Google Guice in Java, as it
-        is somewhat similar, although it is less focused on type names and more
-        on named resources and parameter injection.
-        
-        # Installation
-        
-        Installation is simple. With python3-pip, do the following:
-        
-        ```
-        $ sudo pip install -e .
-        ```
-        
-        Or, to install the latest version available on PyPI:
-        
-        ```
-        $ sudo pip install xeno
-        ```
-        
-        # Usage
-        
-        To use Xeno as a dependency injection framework, you need to create a
-        xeno.Injector and provide it with modules. These modules are regular
-        Python objects with methods marked with the `@xeno.provider`
-        annotation. This annotation tells the `Injector` that this method
-        provides a named resource, the same name as the method marked with
-        `@provider`. These methods should either take no parameters (other
-        than `self`), or take named parameters which refer to other resources
-        by name, i.e. the providers can also be injected with other resources in
-        order to build a dependency chain.
-        
-        Once you have an `Injector` full of resources, you can use it to
-        inject instances, functions, or methods with resources.
-        
-        To create a new object instance by injecting resources into its
-        constructor, use `Injector.create(clazz)`, where `clazz` is the
-        class which you would like to instantiate. The constructor of this class
-        is called, and all named parameters in the constructor are treated as
-        resource references. Once the object is instantiated, any methods marked
-        with `@inject` are invoked with named resources provided.
-        
-        Resources can be injected into normal functions, bound methods, or
-        existing object instances via `Injector.inject(obj)`. If the parameter
-        is an object instance, it is scanned for methods marked with `@inject`
-        and these methods are invoked with named resources provided.
-        
-        ## Example
-        
-        In this simple example, we inject an output stream into an object.
-        
-        ```
-        import sys
-        from xeno import *
-        
-        class OutputStreamModule:
-           @provide
-           def output_stream(self):
-              return sys.stdout
-        
-        class VersionWriter:
-           def __init__(self, output_stream):
-              self.output_stream = output_stream
-        
-           def write_version(self):
-              print('The python version is %s' % sys.version_info,
-                    file=self.output_stream)
-        
-        injector = Injector(OutputStreamModule())
-        writer = injector.create(VersionWriter)
-        writer.write_version()
-        ```
-        
-        Checkout `test.py` in the git repo for more usage examples.
-        
-        ## Change Log
-        
-        ### Version 4.9.0: Jan 03 2020
-        - Deprecate `@recipe` factory decorator for `@factory`.
-        - Allow recipes to specify a `setup` recipe, which is not part
-          of the recipe inputs or outputs but is needed to fulfill the task.
-        ### Version 4.8.0: Dec 29 2020
-        - All recipe resources are loaded before targets are determined.
-        - Recipe names are now valid targets for a build.
-        
-        ### Version 4.7.0: Dec 16 2020
-        - Fixed a bug where build would continue resolving with outdated results.
-        - Added `@recipe` decorator to `xeno.build` to denote recipe functions.
-        
-        ### Version 4.4.0: Nov 2 2020
-        - Added experimental `xeno.build` module, a declarative build system driven by IOC.
-        - Added `xeno.color` offering basic ANSI color and terminal control.
-        
-        ### Version 4.3.0: May 9 2020
-        - Allow methods to be decorated with `@injector.provide`, eliminating the need for modules
-          in some simple usage scenarios.
-        
-        ### Version 4.2.0: May 8 2020
-        - Split `Injector` into `AsyncInjector` and `SyncInjector` to allow injection to be performed
-          in context of another event loop if async providers are not used.
-        - Fixed `AsyncInjector` to actually support asynchronous resolution of dependencies.
-        
-        ### Version 4.1.0: Feb 3 2020
-        - Added `Injector.get_ordered_dependencies` to get a breadth first list of
-          dependencies in the order they are built.
-        
-        ### Version 4.0.0: May 12 2019
-        ***BACKWARDS INCOMPATIBLE CHANGE***
-        - Removed support for parameter annotation aliases.  Use `@alias` on methods instead.
-          This was removed to allow Xeno code to play nicely with PEP 484 type hinting.
-        
-        ### Version 3.1.0: August 29 2018
-        - Add ClassAttributes.for_object convenience method
-        
-        ### Version 3.0.0: May 4 2018
-        ***BACKWARDS INCOMPATIBLE CHANGE***
-        - Provide injection interceptors with an alias map for the given param map.
-        - This change breaks all existing injection interceptors until the new param is added.
-        
-        ### Version 2.8.0: May 3 2018
-        - Allow decorated/wrapped methods to be properly injected if their `'params'` method attribute
-          is carried forward.
-        
-        ### Version 2.7.0: April 20 2018
-        - The `Injector` now adds a `'resource-name'` attribute to resource methods allowing
-          the inspection of a resource's full canonical name at runtime.
-        
-        ### Version 2.6.0: March 27 2018
-        - Bugfix release: Remove support for implicit asynchronous resolution of
-          dependencies.  Providers can still be async, in order to await some other
-          set of coroutines, but can no longer themselves be run in sync.  The
-          benefits do not outweigh the complexity of bugs and timing concerns
-          introduced by this approach.
-        
-        ### Version 2.5.0: March 2, 2018
-        - Added `Injector.provide_async()`.  Note that resource are always run within an
-          event loop and should not use `inject()`, `provide()`, or `require()`
-          directly, instead they should use `inject_async()`, `provide_async()`, and
-          `require_async()` to dynamically modify resources.
-        
-        ### Version 2.4.1: January 30, 2018
-        - Added `Injector.scan_resources()` to allow users to scan for resource names with the given attributes.
-        - Added `Attributes.merge()` to assist with passing attributes down to functions which are wrapped in a decorator.
-        - Added `MethodAttributes.wraps()` static decorator to summarize a common use case of attribute merging.
-        - Added `MethodAttributes.add()` as a simple static decorator to add attribute values to a method's attributes.
-        
-        ### Version 2.4.0: January 21, 2018
-        - Dropped support for deprecated `Namespace.enumerate()` in favor of `Namespace.get_leaves()`.
-        
-        ### Version 2.3.0: January 21, 2018
-        - Added support for asyncio-based concurrency and async provider coroutines with per-injector event loops (`injector.loop`).
-        
-        ### Version 2.2.0: September 19, 2017
-        - Expose the Injector's Namespace object via `Injector.get_namespace()`.  This is useful for users who want to list the contents of namespaces.
-        
-        ### Version 2.1.0: August 23rd, 2017
-        - Allow multiple resource names to be provided to `Injector.get_dependency_graph()`.
-        
-        ### Version 2.0.0: July 25th, 2017
-        ***BACKWARDS INCOMPATIBLE CHANGE***
-        - Change the default namespace separator and breakout symbol to '/'
-        
-        Code using the old namespace separator can be made to work by overriding the value of xeno.Namespace.SEP:
-        ```
-        import xeno
-        xeno.Namespace.SEP = '::'
-        ```
-        
-        ### Version 1.10: July 25th, 2017
-        - Allow names prefixed with `::` to escape their module's namespace, e.g. `::top_level_item`
-        
-        ### Version 1.9: May 23rd, 2017
-        - Add `@const()` module annotation for value-based resources
-        - Add `Injector.get_dependency_tree()` to fetch a tree of dependency names for a given resource name.
-        
-        ### Version 1.8: May 16th, 2017
-        - Add `MissingResourceError` and `MissingDependencyError` exception types.
-        
-        ### Version 1.7: May 16th, 2017
-        - Major update, adding support for namespaces, aliases, and inline resource parameter aliases.  See the unit tests in test.py for examples.
-          - Added `@namespace('Name')` decorator for modules to specify that all resources defined in the module should be scoped within 'Name::'.
-          - Added `@name('alt-name')` to allow resources to be named something other than the name of the function that defines them.
-          - Added `@alias('alt-name', 'name')` to allow a resource to be renamed within either the scope of a single resource or a whole module.
-          - Added `@using('NamespaceName')` to allow the contents of the given namespace
-            to be automatically aliases into either the scope of a single resource or
-            a whole module.
-          - Added support for resource function annotations via PEP 3107 to allow
-            inline aliases, e.g. `def my_resource(name: 'Name::something-important'):`
-        
-        ### Version 1.6: April 26th, 2017
-        - Changed how `xeno.MethodAttributes` works: it now holds a map of attributes
-          and provides methods `get()`, `put()`, and `check()`
-        
-        ### Version 1.5: April 26th, 2017
-        - Added injection interceptors
-        - Refactored method tagging to use `xeno.MethodAttributes` instead of named
-          object attributes to make attribute tagging more flexible and usable by
-          the outside world, e.g. for the new injectors.
-        
-        ### Version 1.4: August 30th, 2016
-        - Added cycle detection.
-        
-        ### Version 1.3: August 29th, 2016
-        - Have the injector offer itself as a named resource named 'injector'.
-        
-        
-Keywords: IOC dependency injector
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+# Xeno: The Python dependency injector from outer space. 
+[![Build Status](https://travis-ci.org/lainproliant/xeno.svg?branch=master)](https://travis-ci.org/lainproliant/xeno)
+
+Xeno is a simple Python dependency injection framework. Use it when you
+need to manage complex inter-object dependencies in a clean way. For the
+merits of dependency injection and IOC, see
+https://en.wikipedia.org/wiki/Dependency_injection.
+
+Xeno should feel pretty familiar to users of Google Guice in Java, as it
+is somewhat similar, although it is less focused on type names and more
+on named resources and parameter injection.
+
+# Installation
+
+Installation is simple. With python3-pip, do the following:
+
+```
+$ sudo pip install -e .
+```
+
+Or, to install the latest version available on PyPI:
+
+```
+$ sudo pip install xeno
+```
+
+# Usage
+
+To use Xeno as a dependency injection framework, you need to create a
+xeno.Injector and provide it with modules. These modules are regular
+Python objects with methods marked with the `@xeno.provider`
+annotation. This annotation tells the `Injector` that this method
+provides a named resource, the same name as the method marked with
+`@provider`. These methods should either take no parameters (other
+than `self`), or take named parameters which refer to other resources
+by name, i.e. the providers can also be injected with other resources in
+order to build a dependency chain.
+
+Once you have an `Injector` full of resources, you can use it to
+inject instances, functions, or methods with resources.
+
+To create a new object instance by injecting resources into its
+constructor, use `Injector.create(clazz)`, where `clazz` is the
+class which you would like to instantiate. The constructor of this class
+is called, and all named parameters in the constructor are treated as
+resource references. Once the object is instantiated, any methods marked
+with `@inject` are invoked with named resources provided.
+
+Resources can be injected into normal functions, bound methods, or
+existing object instances via `Injector.inject(obj)`. If the parameter
+is an object instance, it is scanned for methods marked with `@inject`
+and these methods are invoked with named resources provided.
+
+## Example
+
+In this simple example, we inject an output stream into an object.
+
+```
+import sys
+from xeno import *
+
+class OutputStreamModule:
+   @provide
+   def output_stream(self):
+      return sys.stdout
+
+class VersionWriter:
+   def __init__(self, output_stream):
+      self.output_stream = output_stream
+
+   def write_version(self):
+      print('The python version is %s' % sys.version_info,
+            file=self.output_stream)
+
+injector = Injector(OutputStreamModule())
+writer = injector.create(VersionWriter)
+writer.write_version()
+```
+
+Checkout `test.py` in the git repo for more usage examples.
+
+## Change Log
+
+### Version 4.12.0: Aug 07 2022
+- Changes to support Python 3.10, older versions are now deprecated.
+
+### Version 4.10.0: Oct 28 2021
+- Allow recipes to be specified with glob-style wildcards, as per `fnmatch`.
+
+### Version 4.9.0: Jan 03 2021
+- Deprecate `@recipe` factory decorator for `@factory`.
+- Allow recipes to specify a `setup` recipe, which is not part
+  of the recipe inputs or outputs but is needed to fulfill the task.
+
+### Version 4.8.0: Dec 29 2020
+- All recipe resources are loaded before targets are determined.
+- Recipe names are now valid targets for a build.
+
+### Version 4.7.0: Dec 16 2020
+- Fixed a bug where build would continue resolving with outdated results.
+- Added `@recipe` decorator to `xeno.build` to denote recipe functions.
+
+### Version 4.4.0: Nov 2 2020
+- Added experimental `xeno.build` module, a declarative build system driven by IOC.
+- Added `xeno.color` offering basic ANSI color and terminal control.
+
+### Version 4.3.0: May 9 2020
+- Allow methods to be decorated with `@injector.provide`, eliminating the need for modules
+  in some simple usage scenarios.
+
+### Version 4.2.0: May 8 2020
+- Split `Injector` into `AsyncInjector` and `SyncInjector` to allow injection to be performed
+  in context of another event loop if async providers are not used.
+- Fixed `AsyncInjector` to actually support asynchronous resolution of dependencies.
+
+### Version 4.1.0: Feb 3 2020
+- Added `Injector.get_ordered_dependencies` to get a breadth first list of
+  dependencies in the order they are built.
+
+### Version 4.0.0: May 12 2019
+***BACKWARDS INCOMPATIBLE CHANGE***
+- Removed support for parameter annotation aliases.  Use `@alias` on methods instead.
+  This was removed to allow Xeno code to play nicely with PEP 484 type hinting.
+
+### Version 3.1.0: August 29 2018
+- Add ClassAttributes.for_object convenience method
+
+### Version 3.0.0: May 4 2018
+***BACKWARDS INCOMPATIBLE CHANGE***
+- Provide injection interceptors with an alias map for the given param map.
+- This change breaks all existing injection interceptors until the new param is added.
+
+### Version 2.8.0: May 3 2018
+- Allow decorated/wrapped methods to be properly injected if their `'params'` method attribute
+  is carried forward.
+
+### Version 2.7.0: April 20 2018
+- The `Injector` now adds a `'resource-name'` attribute to resource methods allowing
+  the inspection of a resource's full canonical name at runtime.
+
+### Version 2.6.0: March 27 2018
+- Bugfix release: Remove support for implicit asynchronous resolution of
+  dependencies.  Providers can still be async, in order to await some other
+  set of coroutines, but can no longer themselves be run in sync.  The
+  benefits do not outweigh the complexity of bugs and timing concerns
+  introduced by this approach.
+
+### Version 2.5.0: March 2, 2018
+- Added `Injector.provide_async()`.  Note that resource are always run within an
+  event loop and should not use `inject()`, `provide()`, or `require()`
+  directly, instead they should use `inject_async()`, `provide_async()`, and
+  `require_async()` to dynamically modify resources.
+
+### Version 2.4.1: January 30, 2018
+- Added `Injector.scan_resources()` to allow users to scan for resource names with the given attributes.
+- Added `Attributes.merge()` to assist with passing attributes down to functions which are wrapped in a decorator.
+- Added `MethodAttributes.wraps()` static decorator to summarize a common use case of attribute merging.
+- Added `MethodAttributes.add()` as a simple static decorator to add attribute values to a method's attributes.
+
+### Version 2.4.0: January 21, 2018
+- Dropped support for deprecated `Namespace.enumerate()` in favor of `Namespace.get_leaves()`.
+
+### Version 2.3.0: January 21, 2018
+- Added support for asyncio-based concurrency and async provider coroutines with per-injector event loops (`injector.loop`).
+
+### Version 2.2.0: September 19, 2017
+- Expose the Injector's Namespace object via `Injector.get_namespace()`.  This is useful for users who want to list the contents of namespaces.
+
+### Version 2.1.0: August 23rd, 2017
+- Allow multiple resource names to be provided to `Injector.get_dependency_graph()`.
+
+### Version 2.0.0: July 25th, 2017
+***BACKWARDS INCOMPATIBLE CHANGE***
+- Change the default namespace separator and breakout symbol to '/'
+
+Code using the old namespace separator can be made to work by overriding the value of xeno.Namespace.SEP:
+```
+import xeno
+xeno.Namespace.SEP = '::'
+```
+
+### Version 1.10: July 25th, 2017
+- Allow names prefixed with `::` to escape their module's namespace, e.g. `::top_level_item`
+
+### Version 1.9: May 23rd, 2017
+- Add `@const()` module annotation for value-based resources
+- Add `Injector.get_dependency_tree()` to fetch a tree of dependency names for a given resource name.
+
+### Version 1.8: May 16th, 2017
+- Add `MissingResourceError` and `MissingDependencyError` exception types.
+
+### Version 1.7: May 16th, 2017
+- Major update, adding support for namespaces, aliases, and inline resource parameter aliases.  See the unit tests in test.py for examples.
+  - Added `@namespace('Name')` decorator for modules to specify that all resources defined in the module should be scoped within 'Name::'.
+  - Added `@name('alt-name')` to allow resources to be named something other than the name of the function that defines them.
+  - Added `@alias('alt-name', 'name')` to allow a resource to be renamed within either the scope of a single resource or a whole module.
+  - Added `@using('NamespaceName')` to allow the contents of the given namespace
+    to be automatically aliases into either the scope of a single resource or
+    a whole module.
+  - Added support for resource function annotations via PEP 3107 to allow
+    inline aliases, e.g. `def my_resource(name: 'Name::something-important'):`
+
+### Version 1.6: April 26th, 2017
+- Changed how `xeno.MethodAttributes` works: it now holds a map of attributes
+  and provides methods `get()`, `put()`, and `check()`
+
+### Version 1.5: April 26th, 2017
+- Added injection interceptors
+- Refactored method tagging to use `xeno.MethodAttributes` instead of named
+  object attributes to make attribute tagging more flexible and usable by
+  the outside world, e.g. for the new injectors.
+
+### Version 1.4: August 30th, 2016
+- Added cycle detection.
+
+### Version 1.3: August 29th, 2016
+- Have the injector offer itself as a named resource named 'injector'.
+
```

### Comparing `xeno-4.9.6/README.md` & `xeno-5.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: xeno
+Version: 5.0.0
+Summary: The Python dependency injector from outer space.
+Home-page: https://github.com/lainproliant/xeno
+Author: Lain Musgrove (lainproliant)
+Author-email: lainproliant@gmail.com
+License: BSD
+Keywords: IOC dependency injector
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Xeno: The Python dependency injector from outer space. 
 [![Build Status](https://travis-ci.org/lainproliant/xeno.svg?branch=master)](https://travis-ci.org/lainproliant/xeno)
 
 Xeno is a simple Python dependency injection framework. Use it when you
 need to manage complex inter-object dependencies in a clean way. For the
 merits of dependency injection and IOC, see
 https://en.wikipedia.org/wiki/Dependency_injection.
@@ -77,18 +94,25 @@
 writer.write_version()
 ```
 
 Checkout `test.py` in the git repo for more usage examples.
 
 ## Change Log
 
-### Version 4.9.0: Jan 03 2020
+### Version 4.12.0: Aug 07 2022
+- Changes to support Python 3.10, older versions are now deprecated.
+
+### Version 4.10.0: Oct 28 2021
+- Allow recipes to be specified with glob-style wildcards, as per `fnmatch`.
+
+### Version 4.9.0: Jan 03 2021
 - Deprecate `@recipe` factory decorator for `@factory`.
 - Allow recipes to specify a `setup` recipe, which is not part
   of the recipe inputs or outputs but is needed to fulfill the task.
+
 ### Version 4.8.0: Dec 29 2020
 - All recipe resources are loaded before targets are determined.
 - Recipe names are now valid targets for a build.
 
 ### Version 4.7.0: Dec 16 2020
 - Fixed a bug where build would continue resolving with outdated results.
 - Added `@recipe` decorator to `xeno.build` to denote recipe functions.
```

### Comparing `xeno-4.9.6/setup.py` & `xeno-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xeno",
-    version="4.9.6",
+    version="5.0.0",
     description="The Python dependency injector from outer space.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/xeno",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.10",
     ],
     keywords="IOC dependency injector",
     packages=find_packages(),
     install_requires=[],
     extras_require={},
     package_data={"xeno": ["LICENSE"]},
     data_files=[],
```

### Comparing `xeno-4.9.6/xeno/__init__.py` & `xeno-5.0.0/xeno/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "CircularDependencyError",
     "UndefinedNameError",
     "UnknownNamespaceError",
     "InvalidResourceError",
     "ClassAttributes",
     "MethodAttributes",
     "Namespace",
+    "Tags",
     "async_map",
     "async_wrap",
     "singleton",
     "provide",
     "inject",
     "named",
     "alias",
@@ -33,27 +34,48 @@
     "scan_methods",
     "get_injection_points",
     "get_providers",
     "get_injection_params",
     "Injector",
     "AsyncInjector",
     "SyncInjector",
-    "NOTHING"
+    "NOTHING",
 ]
 
-from .attributes import (ClassAttributes, MethodAttributes,
-                         get_injection_params, get_injection_points,
-                         get_providers, scan_methods, NOTHING)
-from .decorators import (alias, const, inject, named, namespace, provide,
-                         singleton, using)
-from .errors import (CircularDependencyError, ClassInjectionError,
-                     InjectionError, InvalidResourceError,
-                     MethodInjectionError, MissingDependencyError,
-                     MissingResourceError, UndefinedNameError,
-                     UnknownNamespaceError)
-from .namespaces import Namespace
-from .utils import async_map, async_wrap
 from .async_injector import AsyncInjector
+from .attributes import (
+    NOTHING,
+    ClassAttributes,
+    MethodAttributes,
+    get_injection_params,
+    get_injection_points,
+    get_providers,
+    scan_methods,
+)
+from .decorators import (
+    Tags,
+    alias,
+    const,
+    inject,
+    named,
+    namespace,
+    provide,
+    singleton,
+    using,
+)
+from .errors import (
+    CircularDependencyError,
+    ClassInjectionError,
+    InjectionError,
+    InvalidResourceError,
+    MethodInjectionError,
+    MissingDependencyError,
+    MissingResourceError,
+    UndefinedNameError,
+    UnknownNamespaceError,
+)
+from .namespaces import Namespace
 from .sync_injector import SyncInjector
+from .utils import async_map, async_wrap
 
 # For backwards compatibility with older versions of Xeno.
 Injector = AsyncInjector
```

### Comparing `xeno-4.9.6/xeno/abstract.py` & `xeno-5.0.0/xeno/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 # Date: Thursday May 7, 2020
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 
 from abc import ABCMeta, abstractmethod
-from typing import List, Set
+from typing import Any, List, Optional, Set
 
-from .attributes import ClassAttributes, NOTHING
+from .attributes import NOTHING, ClassAttributes, get_providers
+from .decorators import Tags
 from .errors import (
     CircularDependencyError,
     InjectionError,
     InvalidResourceError,
     MissingDependencyError,
     MissingResourceError,
 )
 from .namespaces import Namespace
-from .attributes import get_providers
 
 
 # --------------------------------------------------------------------
 class AbstractInjector(metaclass=ABCMeta):
     """
     This is the abstract base class for injectors.
 
@@ -47,15 +47,15 @@
         """
         Create an Injector object.
 
         *modules: A list of modules to include in the injector.
                   More modules can be added later by calling
                   Injector.add_module().
         """
-        self.resources = {"injector": lambda: self}
+        self.resources: dict[str, Any] = {"injector": lambda: self}
         self.singletons = {}
         self.dep_graph = {}
         self.injection_interceptors = []
         self.ns_index = Namespace.root()
         self.resource_attrs = {}
 
         for module in modules:
@@ -102,42 +102,45 @@
         requires the resource for injection, and causes this method to throw
         MethodInjectionError instead of InjectionError if the resource was
         not provided.
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def provide(self, name_or_method, value=NOTHING, is_singleton=False, namespace=None):
+    def provide(
+        self, name_or_method, value=NOTHING, is_singleton=False, namespace=None
+    ):
         raise NotImplementedError()
 
     @abstractmethod
     def _bind_resource(self, bound_method, module_aliases={}, namespace=None):
         raise NotImplementedError()
 
-    def get_namespace(self, name=None):
+    def get_namespace(self, name=None) -> Optional[Namespace]:
         if name is None or name == Namespace.SEP:
             return self.ns_index
         return self.ns_index.get_namespace(name)
 
     def add_module(self, module, skip_cycle_check=False):
         """
         Add a module to the injector.  The module is scanned for @provider
         annotated methods, and these methods are added as resources to
         the injector.
         """
         module_attrs = ClassAttributes.for_class(module.__class__)
-        namespace = module_attrs.get("namespace", None)
+        assert module_attrs is not None
+        namespace = module_attrs.get(Tags.NAMESPACE, None)
         using_namespaces = []
         if namespace is not None:
             using_namespaces.append(namespace)
             self.ns_index.add_namespace(namespace)
         module_aliases = self._get_aliases(module_attrs, using_namespaces)
-        for name, value in module_attrs.get("const_map", {}).items():
+        for name, value in module_attrs.get(Tags.CONST_MAP, {}).items():
             self.provide(name, value, is_singleton=True, namespace=namespace)
-        for attrs, provider in get_providers(module):
+        for _, provider in get_providers(module):
             self._bind_resource(provider, module_aliases, namespace)
 
         if not skip_cycle_check:
             self.check_for_cycles()
 
     def add_injection_interceptor(self, interceptor):
         """
@@ -213,15 +216,15 @@
 
     def unbind_singleton(self, resource_name=None, unbind_all=False):
         if unbind_all:
             self.singletons.clear()
         else:
             if resource_name not in self.resources:
                 raise MissingResourceError(resource_name)
-            if not self.get_resource_attributes(resource_name).check("singleton"):
+            if not self.get_resource_attributes(resource_name).check(Tags.SINGLETON):
                 raise InvalidResourceError(
                     'Resource "%s" is not a singleton.' % resource_name
                 )
             if resource_name in self.singletons:
                 del self.singletons[resource_name]
 
     def check_for_cycles(self):
@@ -234,28 +237,30 @@
                     raise CircularDependencyError(resource, dep)
                 visit(dep, set(visited))
 
         for resource in self.dep_graph:
             visit(resource)
 
     def _get_aliases(self, attrs, namespaces=[]):
-        aliases = attrs.get("aliases", {})
+        aliases = attrs.get(Tags.ALIASES, {})
         for alias in aliases.keys():
             if Namespace.SEP in alias:
                 raise InjectionError(
                     "Alias name may not contain the namespace "
                     'separator: "%s"' % alias
                 )
-        using_namespaces = namespaces + attrs.get("using-namespaces", [])
-        for namespace in using_namespaces:
+        using_namespaces = namespaces + attrs.get(Tags.USING_NAMESPACES, [])
+        for ns_name in using_namespaces:
+            namespace = self.get_namespace(ns_name)
+            assert namespace is not None
             aliases = {
                 **aliases,
                 **{
-                    Namespace.leaf_name(name): name
-                    for name in self.ns_index.get_leaves(recursive=True)
+                    Namespace.leaf_name(name): Namespace.join(ns_name, name)
+                    for name in namespace.get_leaves()
                 },
             }
         return aliases
 
     def _invoke_injection_interceptors(self, attrs, param_map, alias_map):
         for interceptor in self.injection_interceptors:
             param_map = interceptor(attrs, param_map, alias_map)
```

### Comparing `xeno-4.9.6/xeno/async_injector.py` & `xeno-5.0.0/xeno/async_injector.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,39 @@
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import asyncio
 import inspect
 from collections import defaultdict
+from typing import Optional, cast
 
 from .abstract import AbstractInjector
-from .attributes import (NOTHING, ClassAttributes, MethodAttributes,
-                         get_injection_params, get_injection_points)
-from .decorators import named, singleton
-from .errors import (ClassInjectionError, MethodInjectionError,
-                     MissingDependencyError, MissingResourceError)
+from .attributes import (
+    NOTHING,
+    ClassAttributes,
+    MethodAttributes,
+    get_injection_params,
+    get_injection_points,
+)
+from .decorators import Tags, named, singleton
+from .errors import (
+    ClassInjectionError,
+    MethodInjectionError,
+    MissingDependencyError,
+    MissingResourceError,
+)
 from .namespaces import Namespace
 from .utils import async_map, async_wrap, resolve_alias
 
 
 # --------------------------------------------------------------------
 class AsyncInjector(AbstractInjector):
     """
-    A specialization of AsyncInjector, and the classic Injector
+    A specialization of AbstractInjector, and the classic Injector
     which supports async providers and uses an asyncio event loop
     during dependency resolution.
 
     Use of this injector is preferred for flexibility if you know
     that it will not be run within an asyncio event loop.
 
     This form of Injector cannot be used within other event loops.
@@ -40,45 +50,45 @@
         """
         Create an Injector object.
 
         *modules: A list of modules to include in the injector.
                   More modules can be added later by calling
                   Injector.add_module().
         """
-        self.loop = asyncio.get_event_loop()
         self.async_injection_interceptors = []
         self.singleton_locks = defaultdict(asyncio.Lock)
         super().__init__(*modules)
 
     def add_async_injection_interceptor(self, interceptor):
         self.async_injection_interceptors.append(interceptor)
 
     def create(self, class_):
         """
         Overrides: AbstractInjector
 
+        This method creates a new event loop.  If running from an existing
+        event loop, await `create_async` instead.
+
         Create an instance of the specified class.  The class' constructor
         must follow the rules for @inject methods, such that all of its
         parameters refer to injectable resources or are optional.
 
         If the object needs to be constructed with objects not from the
         Injector, do not use this method.  Instead, instantiate the object
         with these parameters in the constructor, then mark one or more
         methods with @inject and pass the instance to Injector.inject().
         """
-        return self.loop.run_until_complete(self.create_async(class_))
+        return asyncio.run(self.create_async(class_))
 
     async def create_async(self, class_):
         """
         Create an instance of the specified class.  The class' constructor
         must follow the rules for @inject methods, such that all of its
         parameters refer to injectable resources or are optional.
 
-        This async method is meant to be awaited from another coroutine.
-
         If the object needs to be constructed with objects not from the
         Injector, do not use this method.  Instead, instantiate the object
         with these parameters in the constructor, then mark one or more
         methods with @inject and pass the instance to Injector.inject().
         """
         try:
             param_map, alias_map = await self._resolve_dependencies(
@@ -95,76 +105,93 @@
         await self._inject_instance(instance)
         return instance
 
     def inject(self, obj, aliases={}, namespace=""):
         """
         Overrides: AbstractInjector
 
+        This method creates a new event loop.  If running from an existing
+        event loop, await `inject_async` instead.
+
         Inject a method or object instance with resources from this Injector.
 
         obj: A method or object instance.  If this is a method, all named
              parameters are injected from the Injector.  If this is an
              instance, its methods are scanned for injection points and these
              methods are all invoked with resources from the Injector.
         aliases: An optional map from dependency alias to real dependency name.
         """
-        return self.loop.run_until_complete(self.inject_async(obj, aliases, namespace))
+        return asyncio.run(self.inject_async(obj, aliases, namespace))
 
-    async def inject_async(self, obj, aliases={}, namespace=""):
+    async def inject_async(self, obj, aliases={}, namespace: Optional[str] = None):
         """
         Inject a method or object instance with resources from this Injector.
 
-        This async method is meant to be awaited from another coroutine.
-
         obj: A method or object instance.  If this is a method, all named
              parameters are injected from the Injector.  If this is an
              instance, its methods are scanned for injection points and these
              methods are all invoked with resources from the Injector.
         aliases: An optional map from dependency alias to real dependency name.
         """
         if inspect.isfunction(obj) or inspect.ismethod(obj):
-            return await self._inject_method(obj, aliases, namespace)
-        return await self._inject_instance(obj, aliases, namespace)
+            return await self._inject_method(obj, aliases, namespace or "")
+        return await self._inject_instance(obj, aliases, namespace or "")
 
     def require(self, name, method=None):
         """
         Overrides: AbstractInjector
 
+        This method creates a new event loop.  If running from an existing
+        event loop, await `require_async` instead.
+
         Require a named resource from this Injector.  If it can't be provided,
         an InjectionError is raised.
 
-        This method should only be called from outside of the asyncio
-        event loop.
-
         Optionally, a method can be specified.  This indicates the method that
         requires the resource for injection, and causes this method to throw
         MethodInjectionError instead of InjectionError if the resource was
         not provided.
         """
-        return self.loop.run_until_complete(self.require_async(name, method))
+        return asyncio.run(self.require_async(name, method))
 
     async def require_async(self, name, method=None):
         """
         Require a named resource from this Injector.  If it can't be provided,
         an InjectionError is raised.
 
-        This async method is meant to be awaited from another coroutine.
-
         Optionally, a method can be specified.  This indicates the method that
         requires the resource for injection, and causes this method to throw
         MethodInjectionError instead of InjectionError if the resource was
         not provided.
         """
         return await self._require_coro(name, method)
 
-    async def provide_async(self, name_or_method, value=NOTHING, is_singleton=False, namespace=None):
+    def provide(
+        self, name_or_method, value=NOTHING, is_singleton=False, namespace=None
+    ):
+        """
+        Overrides: AbstractInjector
+
+        This method creates a new event loop.  If running from an existing
+        event loop, await `provide_async` instead.
+        """
+
+        return asyncio.run(
+            self.provide_async(name_or_method, value, is_singleton, namespace)
+        )
+
+    async def provide_async(
+        self, name_or_method, value=NOTHING, is_singleton=False, namespace=None
+    ):
 
         if inspect.ismethod(name_or_method) or inspect.isfunction(name_or_method):
             value = name_or_method
-            name = MethodAttributes.for_method(name_or_method).get('name')
+            attrs = MethodAttributes.for_method(name_or_method)
+            assert attrs is not None
+            name = attrs.get(Tags.NAME)
         elif value is NOTHING:
             raise ValueError("A name and value or just a method must be provided.")
         else:
             name = name_or_method
 
         if name in self.singletons:
             del self.singletons[name]
@@ -178,88 +205,78 @@
             def wrapper():
                 return value
 
             if is_singleton:
                 wrapper = singleton(wrapper)
             await self._bind_resource_async(wrapper, namespace=namespace)
 
-    def provide(self, name_or_method, value=NOTHING, is_singleton=False, namespace=None):
-        """
-        Overrides: AbstractInjector
-        """
-
-        return self.loop.run_until_complete(
-            self.provide_async(name_or_method, value, is_singleton, namespace)
-        )
-
     async def _bind_resource_async(
         self, bound_method, module_aliases={}, namespace=None
     ):
         params, _ = get_injection_params(bound_method)
         attrs = MethodAttributes.for_method(bound_method)
+        assert attrs is not None
 
         using_namespaces = []
-        name = attrs.get("name")
+        name = cast(str, attrs.get(Tags.NAME))
+        assert name is not None
         # Allow names that begin with the namespace separator
         # to be scoped outside of the specified namespace.
         if name.startswith(Namespace.SEP):
-            name = name[len(Namespace.SEP) :]
+            name = name[len(Namespace.SEP):]
         elif namespace is not None:
             name = Namespace.join(namespace, name)
             using_namespaces.append(namespace)
 
-        def get_aliases(name):
-            aliases = {
-                **(self._get_aliases(attrs, using_namespaces) or {}),
-                **module_aliases,
-            }
-            return aliases
+        aliases = {
+            **(self._get_aliases(attrs, using_namespaces) or {}),
+            **module_aliases,
+        }
 
-        aliases = get_aliases(name)
         injected_method = await self.inject_async(bound_method, aliases, namespace)
 
-        if attrs.check("singleton"):
+        if attrs.check(Tags.SINGLETON):
             async def wrapper():
                 async with self.singleton_locks[name]:
                     if name not in self.singletons:
                         singleton = await injected_method()
                         self.singletons[name] = singleton
                         return singleton
                     return self.singletons[name]
 
             resource = wrapper
         else:
             resource = injected_method
 
-        # Make the canonical full resource name available via 'resource-name'.
-        attrs.put("resource-name", name)
+        attrs.put(Tags.RESOURCE_FULL_NAME, name)
 
         self.ns_index.add(name)
         self.resources[name] = resource
         self.resource_attrs[name] = attrs
         self.dep_graph[name] = lambda: [
-            resolve_alias(x, get_aliases(x)) for x in params
+            resolve_alias(x, aliases) for x in params
         ]
 
     def _bind_resource(self, bound_method, module_aliases={}, namespace=None):
         """
         Overrides: AbstractInjector
         """
-        return self.loop.run_until_complete(
+        return asyncio.run(
             self._bind_resource_async(bound_method, module_aliases, namespace)
         )
 
     async def _resolve_dependencies(
         self, f, unbound_ctor=False, aliases={}, namespace=""
     ):
         params, default_set = get_injection_params(f, unbound_ctor=unbound_ctor)
         attrs = MethodAttributes.for_method(f)
+        assert attrs is not None
         param_map: dict = {}
         param_resource_map = {}
-        full_name = attrs.get("name")
+        full_name = attrs.get(Tags.NAME)
         if namespace:
             full_name = Namespace.join(namespace, full_name)
             aliases = {**aliases, **self._get_aliases(attrs, [namespace])}
 
         try:
             resource_async_map = {}
             for param in params:
@@ -268,37 +285,41 @@
                 resource_name = param
                 if resource_name.startswith(Namespace.SEP):
                     resource_name = resource_name[len(Namespace.SEP):]
                 resource_name = resolve_alias(resource_name, aliases)
                 resource_async_map[param] = self._require_coro(resource_name)
                 param_resource_map[param] = resource_name
 
-            param_map = dict(await asyncio.gather(
-                *(async_map(k, c) for k, c in resource_async_map.items())
-            ))
+            param_map = dict(
+                await asyncio.gather(
+                    *(async_map(k, c) for k, c in resource_async_map.items())
+                )
+            )
 
         except MissingResourceError as e:
             raise MissingDependencyError(full_name, e.name) from e
         return param_map, param_resource_map
 
     async def _inject_instance(self, instance, aliases={}, namespace=""):
         class_attributes = ClassAttributes.for_class(instance.__class__)
-        aliases = {**aliases, **class_attributes.get("aliases", {})}
-        for attrs, injection_point in get_injection_points(instance):
+        assert class_attributes is not None
+        aliases = {**aliases, **class_attributes.get(Tags.ALIASES, {})}
+        for _, injection_point in get_injection_points(instance):
             injected_method = await self.inject_async(
                 injection_point, aliases, namespace
             )
             await injected_method()
         return instance
 
     async def _inject_method(self, method, aliases_in={}, namespace=""):
         async def wrapper():
             aliases = {**aliases_in}
             attrs = MethodAttributes.for_method(method)
-            aliases = {**aliases, **attrs.get("aliases", {})}
+            assert attrs is not None
+            aliases = {**aliases, **attrs.get(Tags.ALIASES, {})}
             param_map, alias_map = await self._resolve_dependencies(
                 method, aliases=aliases, namespace=namespace
             )
             param_map = await self._async_invoke_injection_interceptors(
                 attrs, param_map, alias_map
             )
             return await async_wrap(method, **param_map)
```

### Comparing `xeno-4.9.6/xeno/color.py` & `xeno-5.0.0/xeno/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,31 @@
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 import os
 import sys
 from typing import List, Optional
 
 # --------------------------------------------------------------------
-_ansi_enabled = "NO_COLOR" not in os.environ and sys.stdout.isatty()
+_ansi_enabled = (
+    "NO_COLOR" not in os.environ and sys.stdout.isatty()
+) or "FORCE_COLOR" in os.environ
 
 # --------------------------------------------------------------------
 def disable():
     global _ansi_enabled
     _ansi_enabled = False
 
 
 # --------------------------------------------------------------------
+def enable():
+    global _ansi_enabled
+    _ansi_enabled = True
+
+
+# --------------------------------------------------------------------
 COLORS = ("black", "red", "green", "yellow", "blue", "magenta", "cyan", "white")
 RENDER_MODES = (
     "none",
     "bold",
     "dim",
     "italic",
     "underline",
@@ -56,19 +64,21 @@
 
 # --------------------------------------------------------------------
 def show_cursor():
     if sys.stdout.isatty():
         sys.stdout.write(seq("?25h"))
         sys.stdout.flush()
 
+
 # --------------------------------------------------------------------
 def hide_cursor():
     if sys.stdout.isatty():
         sys.stdout.write(seq("?25l"))
 
+
 # --------------------------------------------------------------------
 RESET = attr(0)
 
 # --------------------------------------------------------------------
 def style(
     fg: Optional[str] = None, bg: Optional[str] = None, render: Optional[str] = None
 ):
```

### Comparing `xeno-4.9.6/xeno/decorators.py` & `xeno-5.0.0/xeno/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,45 +5,46 @@
 # Date: Thursday May 7, 2020
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import inspect
 
-from .attributes import ClassAttributes, MethodAttributes
-
+from .attributes import ClassAttributes, MethodAttributes, Tags
 
 # --------------------------------------------------------------------
 def singleton(f):
     """
     Method annotation indicating a named singleton resource.
 
     The function will only ever be invoked on an instance of the
     module once, and the return value will be provided to all
     injected objects that require it.
     """
 
     attrs = MethodAttributes.for_method(f, write=True)
-    attrs.put("singleton")
-    attrs.put("provider")
+    assert attrs is not None
+    attrs.put(Tags.SINGLETON)
+    attrs.put(Tags.PROVIDER)
     return f
 
 
 # --------------------------------------------------------------------
 def provide(f):
     """
     Method annotation indicating a named resource.
 
     The function will be added to the Injector's resource map and
     called each time an injected instance is created that requires
     the resource.
     """
 
     attrs = MethodAttributes.for_method(f, write=True)
-    attrs.put("provider")
+    assert attrs is not None
+    attrs.put(Tags.PROVIDER)
     return f
 
 
 # --------------------------------------------------------------------
 def inject(f):
     """
     Method annotation indicating an injection point in an object.
@@ -53,28 +54,30 @@
     to Injector.inject().
 
     All of the parameters of a method marked with @inject must refer
     to named resources in the Injector, or must provide default values
     which can be overridden by resources in the injector.
     """
     attrs = MethodAttributes.for_method(f, write=True)
-    attrs.put("injection-point")
+    assert attrs is not None
+    attrs.put(Tags.INJECTION_POINT)
     return f
 
 
 # --------------------------------------------------------------------
 def named(name):
     """
     Method annotation indicating a name for the given resource other
     than the name of the method itself.
     """
 
     def impl(f):
         attrs = MethodAttributes.for_method(f, write=True)
-        attrs.put("name", name)
+        assert attrs is not None
+        attrs.put(Tags.NAME, name)
         return f
 
     return impl
 
 
 # --------------------------------------------------------------------
 def alias(alias, name):
@@ -85,17 +88,18 @@
 
     def impl(obj):
         attrs = None
         if inspect.isclass(obj):
             attrs = ClassAttributes.for_class(obj, write=True)
         else:
             attrs = MethodAttributes.for_method(obj, write=True)
-        aliases = attrs.get("aliases", {})
+        assert attrs is not None
+        aliases = attrs.get(Tags.ALIASES, {})
         aliases[alias] = name
-        attrs.put("aliases", aliases)
+        attrs.put(Tags.ALIASES, aliases)
         return obj
 
     return impl
 
 
 # --------------------------------------------------------------------
 def namespace(name):
@@ -103,44 +107,47 @@
     Module annotation indicating that the resources defined inside
     should be scoped into the given namespace, that is the given
     string is appended to all resource names followed by '/'.
     """
 
     def impl(class_):
         attrs = ClassAttributes.for_class(class_, write=True)
-        attrs.put("namespace", name)
+        assert attrs is not None
+        attrs.put(Tags.NAMESPACE, name)
         return class_
 
     return impl
 
 
 # --------------------------------------------------------------------
 def const(name, value):
     """
     Module annotation defining a constant resource scoped into the
     module's namespace.
     """
 
     def impl(class_):
         attrs = ClassAttributes.for_class(class_, write=True)
-        const_map = attrs.get("const_map", {})
+        assert attrs is not None
+        const_map = attrs.get(Tags.CONST_MAP, {})
         const_map[name] = value
-        attrs.put("const_map", const_map)
+        attrs.put(Tags.CONST_MAP, const_map)
         return class_
 
     return impl
 
 
 # --------------------------------------------------------------------
 def using(name):
     def impl(obj):
         attrs = None
         if inspect.isclass(obj):
             attrs = ClassAttributes.for_class(obj, write=True)
         else:
             attrs = MethodAttributes.for_method(obj, write=True)
-        namespaces = attrs.get("using-namespaces", [])
+        assert attrs is not None
+        namespaces = attrs.get(Tags.USING_NAMESPACES, [])
         namespaces.append(name)
-        attrs.put("using-namespaces", namespaces)
+        attrs.put(Tags.USING_NAMESPACES, namespaces)
         return obj
 
     return impl
```

### Comparing `xeno-4.9.6/xeno/errors.py` & `xeno-5.0.0/xeno/errors.py`

 * *Files identical despite different names*

### Comparing `xeno-4.9.6/xeno/namespaces.py` & `xeno-5.0.0/xeno/namespaces.py`

 * *Files identical despite different names*

### Comparing `xeno-4.9.6/xeno/shell.py` & `xeno-5.0.0/xeno/shell.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,45 @@
 import shlex
 import subprocess
 from pathlib import Path
 from typing import Any, Callable, Dict, Optional, Set, Tuple, Union, Iterable
 
 from xeno.utils import decode, is_iterable
 
+
+# --------------------------------------------------------------------
+class Environment(dict[str, Any]):
+    """
+    An environment dictionary that knows how to append shell
+    flag variables together when added to other dictionaries.
+    """
+
+    @staticmethod
+    def context():
+        return Environment(os.environ)
+
+    def __add__(self, rhs: Any) -> "Environment":
+        env = Environment()
+        for key, value in rhs.items():
+            if key in self:
+                if not is_iterable(value):
+                    value = shlex.split(value)
+                env[key] = shlex.join(shlex.split(self[key]) + value)
+            else:
+                env[key] = value
+        return env
+
+
 # --------------------------------------------------------------------
-EnvDict = Dict[str, Any]
+EnvDict = Environment | Dict[str, Any]
 InputSource = Callable[[], str]
 LineSink = Callable[[str, asyncio.StreamWriter], None]
 OutputTaskData = Tuple[asyncio.StreamReader, LineSink]
+PathSpec = Union[str | Path]
+
 
 # --------------------------------------------------------------------
 def digest_env(env: EnvDict):
     flat_env: Dict[str, str] = {}
     for key, value in env.items():
         if is_iterable(value):
             value = " ".join(shlex.quote(str(s)) for s in value)
@@ -49,17 +75,17 @@
     else:
         args = [*cmd]
     return subprocess.check_output(args).decode("utf-8").strip()
 
 
 # --------------------------------------------------------------------
 class Shell:
-    def __init__(self, env: EnvDict = dict(os.environ), cwd: Optional[Path] = None):
+    def __init__(self, env: EnvDict = dict(os.environ), cwd: Optional[PathSpec] = None):
         self._env = digest_env(env)
-        self._cwd = cwd or Path.cwd()
+        self._cwd = Path(cwd) if cwd is not None else Path.cwd()
 
     def env(self, new_env: EnvDict):
         return Shell({**self._env, **new_env}, self._cwd)
 
     def cd(self, new_cwd: Path):
         assert new_cwd.exists() and new_cwd.is_dir(), "Invalid directory provided."
         return Shell(self._env, new_cwd)
@@ -98,28 +124,31 @@
 
         redacted_params = {
             k: v if k not in redacted else "<redacted>"
             for k, v in digested_params.items()
         }
 
         if isinstance(cmd, str):
-            return cmd.format(**self._env, **redacted_params)
+            final_cmd = cmd.format(**self._env, **redacted_params)
         else:
-            return shlex.join([c.format(**self._env, **redacted_params) for c in cmd])
+            final_cmd = shlex.join(
+                [str(c).format(**self._env, **redacted_params) for c in cmd]
+            )
+
+        return final_cmd
 
     async def run(
         self,
         cmd: Union[str, Iterable[str]],
         stdin: Optional[InputSource] = None,
         stdout: Optional[LineSink] = None,
         stderr: Optional[LineSink] = None,
         check=False,
-        **params
+        **params,
     ) -> int:
-
         rl_tasks: Dict[asyncio.Future[Any], OutputTaskData] = {}
 
         def setup_rl_task(stream: asyncio.StreamReader, sink: LineSink):
             rl_tasks[asyncio.Task(stream.readline())] = (stream, sink)
 
         cmd = self.interpolate(cmd, params)
         proc = await self._create_proc(cmd)
@@ -130,17 +159,15 @@
             proc.stdin.write(stdin().encode("utf-8"))
         if stdout:
             setup_rl_task(proc.stdout, stdout)
         if stderr:
             setup_rl_task(proc.stderr, stderr)
 
         while rl_tasks:
-            done, pending = await asyncio.wait(
-                rl_tasks, return_when=asyncio.FIRST_COMPLETED
-            )
+            done, _ = await asyncio.wait(rl_tasks, return_when=asyncio.FIRST_COMPLETED)
 
             for future in done:
                 stream, sink = rl_tasks.pop(future)
                 line = future.result()
                 if line:
                     line = decode(line).rstrip()
                     assert proc.stdin is not None
@@ -155,17 +182,21 @@
     def sync(
         self,
         cmd: Union[str, Iterable[str]],
         stdin: Optional[InputSource] = None,
         stdout: Optional[LineSink] = None,
         stderr: Optional[LineSink] = None,
         check=False,
-        **params
+        **params,
     ) -> int:
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.run(cmd, stdin, stdout, stderr, check, **params)
-        )
+        return asyncio.run(self.run(cmd, stdin, stdout, stderr, check, **params))
 
     def interact(self, cmd: Union[str, Iterable[str]], check=False, **params) -> int:
         cmd = self.interpolate(cmd, params)
         return self._interact(cmd, check)
+
+    def interact_as(
+        self, as_user: str, cmd: Union[str, Iterable[str]], check=False, **params
+    ) -> int:
+        cmd = self.interpolate(cmd, params)
+        cmd = shlex.join(["sudo", "-u", as_user, "sh", "-c", cmd])
+        return self._interact(cmd, check)
```

### Comparing `xeno-4.9.6/xeno/sync_injector.py` & `xeno-5.0.0/xeno/sync_injector.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 # Author: Lain Musgrove (lain.proliant@gmail.com)
 # Date: Thursday May 7, 2020
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import inspect
+from typing import Optional, cast
 
 from .abstract import AbstractInjector
 from .attributes import (NOTHING, ClassAttributes, MethodAttributes,
                          get_injection_params, get_injection_points)
-from .decorators import named, singleton
+from .decorators import Tags, named, singleton
 from .errors import (ClassInjectionError, MethodInjectionError,
                      MissingDependencyError, MissingResourceError)
 from .namespaces import Namespace
 from .utils import resolve_alias
 
 
 # --------------------------------------------------------------------
@@ -39,36 +40,38 @@
         except MethodInjectionError as e:
             raise ClassInjectionError(class_, e.name)
 
         instance = class_(**param_map)
         self._inject_instance(instance)
         return instance
 
-    def inject(self, obj, aliases={}, namespace=""):
+    def inject(self, obj, aliases={}, namespace: Optional[str] = None):
         """
         Overrides: AbstractInjector
         """
         if inspect.isfunction(obj) or inspect.ismethod(obj):
-            return self._inject_method(obj, aliases, namespace)
-        return self._inject_instance(obj, aliases, namespace)
+            return self._inject_method(obj, aliases, namespace or "")
+        return self._inject_instance(obj, aliases, namespace or "")
 
     def require(self, name, method=None):
         """
         Overrides: AbstractInjector
         """
         return self._require(name, method)
 
     def provide(self, name_or_method, value=NOTHING, is_singleton=False, namespace=None):
         """
         Overrides: AbstractInjector
         """
 
         if inspect.ismethod(name_or_method) or inspect.isfunction(name_or_method):
             value = name_or_method
-            name = MethodAttributes.for_method(name_or_method).get('name')
+            attrs = MethodAttributes.for_method(name_or_method)
+            assert attrs is not None
+            name = attrs.get(Tags.NAME)
         elif value is NOTHING:
             raise ValueError("A name and value or just a method must be provided.")
         else:
             name = name_or_method
 
         if name in self.singletons:
             del self.singletons[name]
@@ -88,64 +91,62 @@
     def _bind_resource(self, bound_method, module_aliases={}, namespace=None):
         """
         Overrides: AbstractInjector
         """
 
         params, _ = get_injection_params(bound_method)
         attrs = MethodAttributes.for_method(bound_method)
+        assert attrs is not None
 
         using_namespaces = []
-        name = attrs.get("name")
+        name = cast(str, attrs.get(Tags.NAME))
         # Allow names that begin with the namespace separator
         # to be scoped outside of the specified namespace.
         if name.startswith(Namespace.SEP):
             name = name[len(Namespace.SEP):]
         elif namespace is not None:
             name = Namespace.join(namespace, name)
             using_namespaces.append(namespace)
 
-        def get_aliases(name):
-            aliases = {
-                **(self._get_aliases(attrs, using_namespaces) or {}),
-                **module_aliases,
-            }
-            return aliases
+        aliases = {
+            **(self._get_aliases(attrs, using_namespaces) or {}),
+            **module_aliases,
+        }
 
-        aliases = get_aliases(name)
         injected_method = self.inject(bound_method, aliases, namespace)
 
-        if attrs.check("singleton"):
-
+        if attrs.check(Tags.SINGLETON):
             def wrapper():
                 if name not in self.singletons:
                     singleton = injected_method()
                     self.singletons[name] = singleton
                     return singleton
                 return self.singletons[name]
 
             resource = wrapper
         else:
             resource = injected_method
 
         # Make the canonical full resource name available via 'resource-name'.
-        attrs.put("resource-name", name)
+        attrs.put(Tags.RESOURCE_FULL_NAME, name)
 
         self.ns_index.add(name)
         self.resources[name] = resource
         self.resource_attrs[name] = attrs
         self.dep_graph[name] = lambda: [
-            resolve_alias(x, get_aliases(x)) for x in params
+            resolve_alias(x, aliases) for x in params
         ]
 
     def _resolve_dependencies(self, f, unbound_ctor=False, aliases={}, namespace=""):
         params, default_set = get_injection_params(f, unbound_ctor=unbound_ctor)
         attrs = MethodAttributes.for_method(f)
+        assert attrs is not None
         param_map = {}
         param_resource_map = {}
-        full_name = attrs.get("name")
+        full_name = attrs.get(Tags.NAME)
         if namespace:
             full_name = Namespace.join(namespace, full_name)
             aliases = {**aliases, **self._get_aliases(attrs, [namespace])}
 
         try:
             resource_map = {}
             for param in params:
@@ -172,25 +173,27 @@
             raise MissingResourceError(name)
         if name in self.singletons:
             return self.singletons[name]
         return self.resources[name]()
 
     def _inject_instance(self, instance, aliases={}, namespace=""):
         class_attributes = ClassAttributes.for_class(instance.__class__)
-        aliases = {**aliases, **class_attributes.get("aliases", {})}
-        for attrs, injection_point in get_injection_points(instance):
+        assert class_attributes is not None
+        aliases = {**aliases, **class_attributes.get(Tags.ALIASES, {})}
+        for _, injection_point in get_injection_points(instance):
             injected_method = self.inject(injection_point, aliases, namespace)
             injected_method()
         return instance
 
     def _inject_method(self, method, aliases_in={}, namespace=""):
         def wrapper():
             aliases = {**aliases_in}
             attrs = MethodAttributes.for_method(method)
-            aliases = {**aliases, **attrs.get("aliases", {})}
+            assert attrs is not None
+            aliases = {**aliases, **attrs.get(Tags.ALIASES, {})}
             param_map, alias_map = self._resolve_dependencies(
                 method, aliases=aliases, namespace=namespace
             )
             param_map = self._invoke_injection_interceptors(
                 attrs, param_map, alias_map
             )
             return method(**param_map)
```

### Comparing `xeno-4.9.6/xeno/utils.py` & `xeno-5.0.0/xeno/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,22 @@
     """
     if not asyncio.iscoroutinefunction(f):
         return f(*args, **kwargs)
     return await f(*args, **kwargs)
 
 
 # --------------------------------------------------------------------
+async def async_vwrap(v):
+    """
+    Wraps a value in a coroutine for gathering.
+    """
+    return v
+
+
+# --------------------------------------------------------------------
 def bind_unbound_method(obj, method):
     return method.__get__(obj, obj.__class__)
 
 
 # --------------------------------------------------------------------
 def decode(b: bytes) -> str:
     try:
@@ -58,23 +66,26 @@
     """
     sig = inspect.signature(f)
     return list(sig.parameters.values())
 
 
 # --------------------------------------------------------------------
 def is_iterable(obj: Any) -> bool:
-    """ Determine if the given object is an iterable sequence other than a string or byte array. """
-    return isinstance(obj, Sequence) and not isinstance(obj, (str, bytes, bytearray))
+    """Determine if the given object is an iterable sequence other than a string or byte array."""
+    return (
+        isinstance(obj, Sequence)
+        and not isinstance(obj, (str, bytes, bytearray))
+        or inspect.isgenerator(obj)
+    )
 
 
 # --------------------------------------------------------------------
 def file_age(file: Path) -> timedelta:
-    return datetime.now() - datetime.fromtimestamp(
-        file.stat().st_mtime
-    )
+    return datetime.now() - datetime.fromtimestamp(file.stat().st_mtime)
+
 
 # --------------------------------------------------------------------
 def resolve_alias(name, aliases, visited=None):
     if visited is None:
         visited = set()
 
     if name in aliases:
```

### Comparing `xeno-4.9.6/xeno.egg-info/PKG-INFO` & `xeno-5.0.0/xeno.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,228 +1,235 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 4.9.6
+Version: 5.0.0
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
-Description: # Xeno: The Python dependency injector from outer space. 
-        [![Build Status](https://travis-ci.org/lainproliant/xeno.svg?branch=master)](https://travis-ci.org/lainproliant/xeno)
-        
-        Xeno is a simple Python dependency injection framework. Use it when you
-        need to manage complex inter-object dependencies in a clean way. For the
-        merits of dependency injection and IOC, see
-        https://en.wikipedia.org/wiki/Dependency_injection.
-        
-        Xeno should feel pretty familiar to users of Google Guice in Java, as it
-        is somewhat similar, although it is less focused on type names and more
-        on named resources and parameter injection.
-        
-        # Installation
-        
-        Installation is simple. With python3-pip, do the following:
-        
-        ```
-        $ sudo pip install -e .
-        ```
-        
-        Or, to install the latest version available on PyPI:
-        
-        ```
-        $ sudo pip install xeno
-        ```
-        
-        # Usage
-        
-        To use Xeno as a dependency injection framework, you need to create a
-        xeno.Injector and provide it with modules. These modules are regular
-        Python objects with methods marked with the `@xeno.provider`
-        annotation. This annotation tells the `Injector` that this method
-        provides a named resource, the same name as the method marked with
-        `@provider`. These methods should either take no parameters (other
-        than `self`), or take named parameters which refer to other resources
-        by name, i.e. the providers can also be injected with other resources in
-        order to build a dependency chain.
-        
-        Once you have an `Injector` full of resources, you can use it to
-        inject instances, functions, or methods with resources.
-        
-        To create a new object instance by injecting resources into its
-        constructor, use `Injector.create(clazz)`, where `clazz` is the
-        class which you would like to instantiate. The constructor of this class
-        is called, and all named parameters in the constructor are treated as
-        resource references. Once the object is instantiated, any methods marked
-        with `@inject` are invoked with named resources provided.
-        
-        Resources can be injected into normal functions, bound methods, or
-        existing object instances via `Injector.inject(obj)`. If the parameter
-        is an object instance, it is scanned for methods marked with `@inject`
-        and these methods are invoked with named resources provided.
-        
-        ## Example
-        
-        In this simple example, we inject an output stream into an object.
-        
-        ```
-        import sys
-        from xeno import *
-        
-        class OutputStreamModule:
-           @provide
-           def output_stream(self):
-              return sys.stdout
-        
-        class VersionWriter:
-           def __init__(self, output_stream):
-              self.output_stream = output_stream
-        
-           def write_version(self):
-              print('The python version is %s' % sys.version_info,
-                    file=self.output_stream)
-        
-        injector = Injector(OutputStreamModule())
-        writer = injector.create(VersionWriter)
-        writer.write_version()
-        ```
-        
-        Checkout `test.py` in the git repo for more usage examples.
-        
-        ## Change Log
-        
-        ### Version 4.9.0: Jan 03 2020
-        - Deprecate `@recipe` factory decorator for `@factory`.
-        - Allow recipes to specify a `setup` recipe, which is not part
-          of the recipe inputs or outputs but is needed to fulfill the task.
-        ### Version 4.8.0: Dec 29 2020
-        - All recipe resources are loaded before targets are determined.
-        - Recipe names are now valid targets for a build.
-        
-        ### Version 4.7.0: Dec 16 2020
-        - Fixed a bug where build would continue resolving with outdated results.
-        - Added `@recipe` decorator to `xeno.build` to denote recipe functions.
-        
-        ### Version 4.4.0: Nov 2 2020
-        - Added experimental `xeno.build` module, a declarative build system driven by IOC.
-        - Added `xeno.color` offering basic ANSI color and terminal control.
-        
-        ### Version 4.3.0: May 9 2020
-        - Allow methods to be decorated with `@injector.provide`, eliminating the need for modules
-          in some simple usage scenarios.
-        
-        ### Version 4.2.0: May 8 2020
-        - Split `Injector` into `AsyncInjector` and `SyncInjector` to allow injection to be performed
-          in context of another event loop if async providers are not used.
-        - Fixed `AsyncInjector` to actually support asynchronous resolution of dependencies.
-        
-        ### Version 4.1.0: Feb 3 2020
-        - Added `Injector.get_ordered_dependencies` to get a breadth first list of
-          dependencies in the order they are built.
-        
-        ### Version 4.0.0: May 12 2019
-        ***BACKWARDS INCOMPATIBLE CHANGE***
-        - Removed support for parameter annotation aliases.  Use `@alias` on methods instead.
-          This was removed to allow Xeno code to play nicely with PEP 484 type hinting.
-        
-        ### Version 3.1.0: August 29 2018
-        - Add ClassAttributes.for_object convenience method
-        
-        ### Version 3.0.0: May 4 2018
-        ***BACKWARDS INCOMPATIBLE CHANGE***
-        - Provide injection interceptors with an alias map for the given param map.
-        - This change breaks all existing injection interceptors until the new param is added.
-        
-        ### Version 2.8.0: May 3 2018
-        - Allow decorated/wrapped methods to be properly injected if their `'params'` method attribute
-          is carried forward.
-        
-        ### Version 2.7.0: April 20 2018
-        - The `Injector` now adds a `'resource-name'` attribute to resource methods allowing
-          the inspection of a resource's full canonical name at runtime.
-        
-        ### Version 2.6.0: March 27 2018
-        - Bugfix release: Remove support for implicit asynchronous resolution of
-          dependencies.  Providers can still be async, in order to await some other
-          set of coroutines, but can no longer themselves be run in sync.  The
-          benefits do not outweigh the complexity of bugs and timing concerns
-          introduced by this approach.
-        
-        ### Version 2.5.0: March 2, 2018
-        - Added `Injector.provide_async()`.  Note that resource are always run within an
-          event loop and should not use `inject()`, `provide()`, or `require()`
-          directly, instead they should use `inject_async()`, `provide_async()`, and
-          `require_async()` to dynamically modify resources.
-        
-        ### Version 2.4.1: January 30, 2018
-        - Added `Injector.scan_resources()` to allow users to scan for resource names with the given attributes.
-        - Added `Attributes.merge()` to assist with passing attributes down to functions which are wrapped in a decorator.
-        - Added `MethodAttributes.wraps()` static decorator to summarize a common use case of attribute merging.
-        - Added `MethodAttributes.add()` as a simple static decorator to add attribute values to a method's attributes.
-        
-        ### Version 2.4.0: January 21, 2018
-        - Dropped support for deprecated `Namespace.enumerate()` in favor of `Namespace.get_leaves()`.
-        
-        ### Version 2.3.0: January 21, 2018
-        - Added support for asyncio-based concurrency and async provider coroutines with per-injector event loops (`injector.loop`).
-        
-        ### Version 2.2.0: September 19, 2017
-        - Expose the Injector's Namespace object via `Injector.get_namespace()`.  This is useful for users who want to list the contents of namespaces.
-        
-        ### Version 2.1.0: August 23rd, 2017
-        - Allow multiple resource names to be provided to `Injector.get_dependency_graph()`.
-        
-        ### Version 2.0.0: July 25th, 2017
-        ***BACKWARDS INCOMPATIBLE CHANGE***
-        - Change the default namespace separator and breakout symbol to '/'
-        
-        Code using the old namespace separator can be made to work by overriding the value of xeno.Namespace.SEP:
-        ```
-        import xeno
-        xeno.Namespace.SEP = '::'
-        ```
-        
-        ### Version 1.10: July 25th, 2017
-        - Allow names prefixed with `::` to escape their module's namespace, e.g. `::top_level_item`
-        
-        ### Version 1.9: May 23rd, 2017
-        - Add `@const()` module annotation for value-based resources
-        - Add `Injector.get_dependency_tree()` to fetch a tree of dependency names for a given resource name.
-        
-        ### Version 1.8: May 16th, 2017
-        - Add `MissingResourceError` and `MissingDependencyError` exception types.
-        
-        ### Version 1.7: May 16th, 2017
-        - Major update, adding support for namespaces, aliases, and inline resource parameter aliases.  See the unit tests in test.py for examples.
-          - Added `@namespace('Name')` decorator for modules to specify that all resources defined in the module should be scoped within 'Name::'.
-          - Added `@name('alt-name')` to allow resources to be named something other than the name of the function that defines them.
-          - Added `@alias('alt-name', 'name')` to allow a resource to be renamed within either the scope of a single resource or a whole module.
-          - Added `@using('NamespaceName')` to allow the contents of the given namespace
-            to be automatically aliases into either the scope of a single resource or
-            a whole module.
-          - Added support for resource function annotations via PEP 3107 to allow
-            inline aliases, e.g. `def my_resource(name: 'Name::something-important'):`
-        
-        ### Version 1.6: April 26th, 2017
-        - Changed how `xeno.MethodAttributes` works: it now holds a map of attributes
-          and provides methods `get()`, `put()`, and `check()`
-        
-        ### Version 1.5: April 26th, 2017
-        - Added injection interceptors
-        - Refactored method tagging to use `xeno.MethodAttributes` instead of named
-          object attributes to make attribute tagging more flexible and usable by
-          the outside world, e.g. for the new injectors.
-        
-        ### Version 1.4: August 30th, 2016
-        - Added cycle detection.
-        
-        ### Version 1.3: August 29th, 2016
-        - Have the injector offer itself as a named resource named 'injector'.
-        
-        
 Keywords: IOC dependency injector
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Xeno: The Python dependency injector from outer space. 
+[![Build Status](https://travis-ci.org/lainproliant/xeno.svg?branch=master)](https://travis-ci.org/lainproliant/xeno)
+
+Xeno is a simple Python dependency injection framework. Use it when you
+need to manage complex inter-object dependencies in a clean way. For the
+merits of dependency injection and IOC, see
+https://en.wikipedia.org/wiki/Dependency_injection.
+
+Xeno should feel pretty familiar to users of Google Guice in Java, as it
+is somewhat similar, although it is less focused on type names and more
+on named resources and parameter injection.
+
+# Installation
+
+Installation is simple. With python3-pip, do the following:
+
+```
+$ sudo pip install -e .
+```
+
+Or, to install the latest version available on PyPI:
+
+```
+$ sudo pip install xeno
+```
+
+# Usage
+
+To use Xeno as a dependency injection framework, you need to create a
+xeno.Injector and provide it with modules. These modules are regular
+Python objects with methods marked with the `@xeno.provider`
+annotation. This annotation tells the `Injector` that this method
+provides a named resource, the same name as the method marked with
+`@provider`. These methods should either take no parameters (other
+than `self`), or take named parameters which refer to other resources
+by name, i.e. the providers can also be injected with other resources in
+order to build a dependency chain.
+
+Once you have an `Injector` full of resources, you can use it to
+inject instances, functions, or methods with resources.
+
+To create a new object instance by injecting resources into its
+constructor, use `Injector.create(clazz)`, where `clazz` is the
+class which you would like to instantiate. The constructor of this class
+is called, and all named parameters in the constructor are treated as
+resource references. Once the object is instantiated, any methods marked
+with `@inject` are invoked with named resources provided.
+
+Resources can be injected into normal functions, bound methods, or
+existing object instances via `Injector.inject(obj)`. If the parameter
+is an object instance, it is scanned for methods marked with `@inject`
+and these methods are invoked with named resources provided.
+
+## Example
+
+In this simple example, we inject an output stream into an object.
+
+```
+import sys
+from xeno import *
+
+class OutputStreamModule:
+   @provide
+   def output_stream(self):
+      return sys.stdout
+
+class VersionWriter:
+   def __init__(self, output_stream):
+      self.output_stream = output_stream
+
+   def write_version(self):
+      print('The python version is %s' % sys.version_info,
+            file=self.output_stream)
+
+injector = Injector(OutputStreamModule())
+writer = injector.create(VersionWriter)
+writer.write_version()
+```
+
+Checkout `test.py` in the git repo for more usage examples.
+
+## Change Log
+
+### Version 4.12.0: Aug 07 2022
+- Changes to support Python 3.10, older versions are now deprecated.
+
+### Version 4.10.0: Oct 28 2021
+- Allow recipes to be specified with glob-style wildcards, as per `fnmatch`.
+
+### Version 4.9.0: Jan 03 2021
+- Deprecate `@recipe` factory decorator for `@factory`.
+- Allow recipes to specify a `setup` recipe, which is not part
+  of the recipe inputs or outputs but is needed to fulfill the task.
+
+### Version 4.8.0: Dec 29 2020
+- All recipe resources are loaded before targets are determined.
+- Recipe names are now valid targets for a build.
+
+### Version 4.7.0: Dec 16 2020
+- Fixed a bug where build would continue resolving with outdated results.
+- Added `@recipe` decorator to `xeno.build` to denote recipe functions.
+
+### Version 4.4.0: Nov 2 2020
+- Added experimental `xeno.build` module, a declarative build system driven by IOC.
+- Added `xeno.color` offering basic ANSI color and terminal control.
+
+### Version 4.3.0: May 9 2020
+- Allow methods to be decorated with `@injector.provide`, eliminating the need for modules
+  in some simple usage scenarios.
+
+### Version 4.2.0: May 8 2020
+- Split `Injector` into `AsyncInjector` and `SyncInjector` to allow injection to be performed
+  in context of another event loop if async providers are not used.
+- Fixed `AsyncInjector` to actually support asynchronous resolution of dependencies.
+
+### Version 4.1.0: Feb 3 2020
+- Added `Injector.get_ordered_dependencies` to get a breadth first list of
+  dependencies in the order they are built.
+
+### Version 4.0.0: May 12 2019
+***BACKWARDS INCOMPATIBLE CHANGE***
+- Removed support for parameter annotation aliases.  Use `@alias` on methods instead.
+  This was removed to allow Xeno code to play nicely with PEP 484 type hinting.
+
+### Version 3.1.0: August 29 2018
+- Add ClassAttributes.for_object convenience method
+
+### Version 3.0.0: May 4 2018
+***BACKWARDS INCOMPATIBLE CHANGE***
+- Provide injection interceptors with an alias map for the given param map.
+- This change breaks all existing injection interceptors until the new param is added.
+
+### Version 2.8.0: May 3 2018
+- Allow decorated/wrapped methods to be properly injected if their `'params'` method attribute
+  is carried forward.
+
+### Version 2.7.0: April 20 2018
+- The `Injector` now adds a `'resource-name'` attribute to resource methods allowing
+  the inspection of a resource's full canonical name at runtime.
+
+### Version 2.6.0: March 27 2018
+- Bugfix release: Remove support for implicit asynchronous resolution of
+  dependencies.  Providers can still be async, in order to await some other
+  set of coroutines, but can no longer themselves be run in sync.  The
+  benefits do not outweigh the complexity of bugs and timing concerns
+  introduced by this approach.
+
+### Version 2.5.0: March 2, 2018
+- Added `Injector.provide_async()`.  Note that resource are always run within an
+  event loop and should not use `inject()`, `provide()`, or `require()`
+  directly, instead they should use `inject_async()`, `provide_async()`, and
+  `require_async()` to dynamically modify resources.
+
+### Version 2.4.1: January 30, 2018
+- Added `Injector.scan_resources()` to allow users to scan for resource names with the given attributes.
+- Added `Attributes.merge()` to assist with passing attributes down to functions which are wrapped in a decorator.
+- Added `MethodAttributes.wraps()` static decorator to summarize a common use case of attribute merging.
+- Added `MethodAttributes.add()` as a simple static decorator to add attribute values to a method's attributes.
+
+### Version 2.4.0: January 21, 2018
+- Dropped support for deprecated `Namespace.enumerate()` in favor of `Namespace.get_leaves()`.
+
+### Version 2.3.0: January 21, 2018
+- Added support for asyncio-based concurrency and async provider coroutines with per-injector event loops (`injector.loop`).
+
+### Version 2.2.0: September 19, 2017
+- Expose the Injector's Namespace object via `Injector.get_namespace()`.  This is useful for users who want to list the contents of namespaces.
+
+### Version 2.1.0: August 23rd, 2017
+- Allow multiple resource names to be provided to `Injector.get_dependency_graph()`.
+
+### Version 2.0.0: July 25th, 2017
+***BACKWARDS INCOMPATIBLE CHANGE***
+- Change the default namespace separator and breakout symbol to '/'
+
+Code using the old namespace separator can be made to work by overriding the value of xeno.Namespace.SEP:
+```
+import xeno
+xeno.Namespace.SEP = '::'
+```
+
+### Version 1.10: July 25th, 2017
+- Allow names prefixed with `::` to escape their module's namespace, e.g. `::top_level_item`
+
+### Version 1.9: May 23rd, 2017
+- Add `@const()` module annotation for value-based resources
+- Add `Injector.get_dependency_tree()` to fetch a tree of dependency names for a given resource name.
+
+### Version 1.8: May 16th, 2017
+- Add `MissingResourceError` and `MissingDependencyError` exception types.
+
+### Version 1.7: May 16th, 2017
+- Major update, adding support for namespaces, aliases, and inline resource parameter aliases.  See the unit tests in test.py for examples.
+  - Added `@namespace('Name')` decorator for modules to specify that all resources defined in the module should be scoped within 'Name::'.
+  - Added `@name('alt-name')` to allow resources to be named something other than the name of the function that defines them.
+  - Added `@alias('alt-name', 'name')` to allow a resource to be renamed within either the scope of a single resource or a whole module.
+  - Added `@using('NamespaceName')` to allow the contents of the given namespace
+    to be automatically aliases into either the scope of a single resource or
+    a whole module.
+  - Added support for resource function annotations via PEP 3107 to allow
+    inline aliases, e.g. `def my_resource(name: 'Name::something-important'):`
+
+### Version 1.6: April 26th, 2017
+- Changed how `xeno.MethodAttributes` works: it now holds a map of attributes
+  and provides methods `get()`, `put()`, and `check()`
+
+### Version 1.5: April 26th, 2017
+- Added injection interceptors
+- Refactored method tagging to use `xeno.MethodAttributes` instead of named
+  object attributes to make attribute tagging more flexible and usable by
+  the outside world, e.g. for the new injectors.
+
+### Version 1.4: August 30th, 2016
+- Added cycle detection.
+
+### Version 1.3: August 29th, 2016
+- Have the injector offer itself as a named resource named 'injector'.
+
```

