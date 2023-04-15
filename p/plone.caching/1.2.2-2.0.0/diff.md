# Comparing `tmp/plone.caching-1.2.2.tar.gz` & `tmp/plone.caching-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.caching-1.2.2.tar", last modified: Mon Apr 20 19:59:37 2020, max compression
+gzip compressed data, was "plone.caching-2.0.0.tar", last modified: Sat Apr 15 07:55:58 2023, max compression
```

## Comparing `plone.caching-1.2.2.tar` & `plone.caching-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 19:59:37.000000 plone.caching-1.2.2/
--rw-r--r--   0 maurits    (501) staff       (20)    22187 2020-04-20 19:59:37.000000 plone.caching-1.2.2/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    22187 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      840 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       37 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)      140 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone.caching.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-20 19:59:36.000000 plone.caching-1.2.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-04-20 19:59:36.000000 plone.caching-1.2.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      149 2020-04-20 19:59:36.000000 plone.caching-1.2.2/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 19:59:37.000000 plone.caching-1.2.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2020-04-20 19:59:36.000000 plone.caching-1.2.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     1214 2020-04-20 19:59:36.000000 plone.caching-1.2.2/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)      745 2020-04-20 19:59:36.000000 plone.caching-1.2.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1849 2020-04-20 19:59:36.000000 plone.caching-1.2.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone/caching/
--rw-r--r--   0 maurits    (501) staff       (20)     6232 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1307 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6766 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/hooks.py
--rw-r--r--   0 maurits    (501) staff       (20)      659 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/lookup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 19:59:37.000000 plone.caching-1.2.2/plone/caching/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     5544 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     6847 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/tests/test_operations.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    39355 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/tests/test_hooks.py
--rw-r--r--   0 maurits    (501) staff       (20)     1100 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/tests/test_lookup.py
--rw-r--r--   0 maurits    (501) staff       (20)       24 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2893 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/operations.py
--rw-r--r--   0 maurits    (501) staff       (20)     3425 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1416 2020-04-20 19:59:36.000000 plone.caching-1.2.2/plone/caching/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      299 2020-04-20 19:59:37.000000 plone.caching-1.2.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)    15697 2020-04-20 19:59:36.000000 plone.caching-1.2.2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1621 2020-04-20 19:59:36.000000 plone.caching-1.2.2/CHANGES.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.559595 plone.caching-2.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1795 2023-04-15 07:55:58.000000 plone.caching-2.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:55:58.000000 plone.caching-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      149 2023-04-15 07:55:58.000000 plone.caching-2.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    18364 2023-04-15 07:55:58.559595 plone.caching-2.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)    15697 2023-04-15 07:55:58.000000 plone.caching-2.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.557595 plone.caching-2.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1214 2023-04-15 07:55:58.000000 plone.caching-2.0.0/docs/INSTALL.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)    12282 2023-04-15 07:55:58.000000 plone.caching-2.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      745 2023-04-15 07:55:58.000000 plone.caching-2.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.557595 plone.caching-2.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.559595 plone.caching-2.0.0/plone/caching/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1340 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     6560 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/hooks.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6149 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      627 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/lookup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2750 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/operations.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1384 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.559595 plone.caching-2.0.0/plone/caching/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    39339 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/tests/test_hooks.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1066 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/tests/test_lookup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6686 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/tests/test_operations.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5302 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/tests/test_utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3501 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone/caching/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:55:58.558595 plone.caching-2.0.0/plone.caching.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    18364 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone.caching.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      800 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone.caching.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone.caching.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone.caching.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone.caching.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      148 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone.caching.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:55:58.000000 plone.caching-2.0.0/plone.caching.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1643 2023-04-15 07:55:58.000000 plone.caching-2.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:55:58.560595 plone.caching-2.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1779 2023-04-15 07:55:58.000000 plone.caching-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.caching-1.2.2/plone.caching.egg-info/SOURCES.txt` & `plone.caching-2.0.0/plone.caching.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.caching.egg-info/PKG-INFO
 plone.caching.egg-info/SOURCES.txt
 plone.caching.egg-info/dependency_links.txt
-plone.caching.egg-info/entry_points.txt
 plone.caching.egg-info/namespace_packages.txt
 plone.caching.egg-info/not-zip-safe
 plone.caching.egg-info/requires.txt
 plone.caching.egg-info/top_level.txt
 plone/caching/__init__.py
 plone/caching/configure.zcml
 plone/caching/hooks.py
```

### Comparing `plone.caching-1.2.2/docs/LICENSE.GPL` & `plone.caching-2.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.caching-1.2.2/docs/INSTALL.txt` & `plone.caching-2.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.caching-1.2.2/docs/LICENSE.txt` & `plone.caching-2.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.caching-1.2.2/plone/caching/interfaces.py` & `plone.caching-2.0.0/plone/caching/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# -*- coding: utf-8 -*-
 from zope import schema
 from zope.interface import Interface
 
 import zope.i18nmessageid
 
 
-_ = zope.i18nmessageid.MessageFactory('plone')
+_ = zope.i18nmessageid.MessageFactory("plone")
 
-X_CACHE_RULE_HEADER = 'X-Cache-Rule'
-X_CACHE_OPERATION_HEADER = 'X-Cache-Operation'
+X_CACHE_RULE_HEADER = "X-Cache-Rule"
+X_CACHE_OPERATION_HEADER = "X-Cache-Operation"
 
 
 class ICacheSettings(Interface):
-    """Settings expected to be found in plone.registry
-    """
+    """Settings expected to be found in plone.registry"""
 
     enabled = schema.Bool(
-        title=_(u'Globally enabled'),
-        description=_(u'If not set, no caching operations will be attempted'),
+        title=_("Globally enabled"),
+        description=_("If not set, no caching operations will be attempted"),
         default=False,
     )
 
     operationMapping = schema.Dict(
-        title=_(u'Rule set/operation mapping'),
-        description=_(u'Maps rule set names to operation names'),
-        key_type=schema.DottedName(title=_(u'Rule set name')),
-        value_type=schema.DottedName(title=_(u'Caching operation name')),
+        title=_("Rule set/operation mapping"),
+        description=_("Maps rule set names to operation names"),
+        key_type=schema.DottedName(title=_("Rule set name")),
+        value_type=schema.DottedName(title=_("Caching operation name")),
     )
 
+
 #
 #  Cache operations
 #
 
 
 class ICachingOperation(Interface):
     """Represents a caching operation, typically setting of response headers
@@ -67,14 +66,15 @@
         """
 
 
 #
 # Cache operation *types* (for UI support)
 #
 
+
 class ICachingOperationType(Interface):
     """A named utility which is used to provide UI support for caching
     operations. The name should correspond to the operation adapter name.
 
     The usual pattern is::
 
         from plone.caching.interfaces import ICachingOperation
@@ -116,50 +116,55 @@
     adapter names must match. By convention, the option prefix should be the
     same as the adapter/utility name.
 
     You could also register an instance as a utility, of course.
     """
 
     title = schema.TextLine(
-        title=_(u'Title'),
-        description=_(u'A descriptive title for the operation'),
+        title=_("Title"),
+        description=_("A descriptive title for the operation"),
     )
 
     description = schema.Text(
-        title=_(u'Description'),
-        description=_(u'A longer description for the operaton'),
+        title=_("Description"),
+        description=_("A longer description for the operation"),
         required=False,
     )
 
     prefix = schema.DottedName(
-        title=_(u'Registry prefix'),
-        description=_(u'Prefix for records in the registry pertaining to '
-                      u'this operation. This, alongside the next '
-                      u'parameter, allows the user interface to present '
-                      u'relevant configuration options for this '
-                      u'operation.'),
+        title=_("Registry prefix"),
+        description=_(
+            "Prefix for records in the registry pertaining to "
+            "this operation. This, alongside the next "
+            "parameter, allows the user interface to present "
+            "relevant configuration options for this "
+            "operation."
+        ),
         required=False,
     )
 
     options = schema.Tuple(
-        title=_(u'Registry options'),
-        description=_(u'A tuple of options which can be used to '
-                      u'configure this operation. An option is looked '
-                      u'up in the registry by concatenating the prefix '
-                      u'with the option name, optionally preceded by '
-                      u'the rule set name, to allow per-rule overrides.'),
+        title=_("Registry options"),
+        description=_(
+            "A tuple of options which can be used to "
+            "configure this operation. An option is looked "
+            "up in the registry by concatenating the prefix "
+            "with the option name, optionally preceded by "
+            "the rule set name, to allow per-rule overrides."
+        ),
         value_type=schema.DottedName(),
         required=False,
     )
 
 
 #
 # Internal abstractions
 #
 
+
 class IRulesetLookup(Interface):
     """Abstraction for the lookup of response rulesets from published objects.
     This is an unnamed multi- adapter from (published, request).
 
     The main reason for needing this is that some publishable resources cannot
     be adequately mapped to a rule set by context type alone. In particular,
     Zope page templates in skin layers or created through the web can only be
```

### Comparing `plone.caching-1.2.2/plone/caching/configure.zcml` & `plone.caching-2.0.0/plone/caching/configure.zcml`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:zcml="http://namespaces.zope.org/zcml"
     xmlns:browser="http://namespaces.zope.org/browser"
-    i18n_domain="plone">
-
-    <include package="z3c.caching" file="meta.zcml" />
-    <include package="z3c.caching" />
-
-    <include package="plone.registry" />
-    <include package="plone.transformchain" />
-
-    <!-- Default lookup -->
-    <adapter factory=".lookup.DefaultRulesetLookup" />
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone"
+    >
 
-    <!-- The 'Chain' operation -->
-    <adapter factory=".operations.Chain"   name="plone.caching.operations.chain" />
-    <utility component=".operations.Chain" name="plone.caching.operations.chain" />
+  <include
+      package="z3c.caching"
+      file="meta.zcml"
+      />
+  <include package="z3c.caching" />
+
+  <include package="plone.registry" />
+  <include package="plone.transformchain" />
+
+  <!-- Default lookup -->
+  <adapter factory=".lookup.DefaultRulesetLookup" />
+
+  <!-- The 'Chain' operation -->
+  <adapter
+      factory=".operations.Chain"
+      name="plone.caching.operations.chain"
+      />
+  <utility
+      name="plone.caching.operations.chain"
+      component=".operations.Chain"
+      />
 
-    <!-- Intercepts are performed by raising an exception prior to view
+  <!-- Intercepts are performed by raising an exception prior to view
          invocation. There is a view on this exception which renders the
          intercepted response.
      -->
-    <subscriber handler=".hooks.intercept" />
-    <browser:page
-        name="index.html"
-        for=".hooks.Intercepted"
-        class=".hooks.InterceptorResponse"
-        permission="zope2.Public"
-        />
-
-    <!-- Mutator: plone.transformchain order 12000 -->
-    <adapter factory=".hooks.MutatorTransform" name="plone.caching.mutator" />
+  <subscriber handler=".hooks.intercept" />
+  <browser:page
+      name="index.html"
+      for=".hooks.Intercepted"
+      class=".hooks.InterceptorResponse"
+      permission="zope2.Public"
+      />
+
+  <!-- Mutator: plone.transformchain order 12000 -->
+  <adapter
+      factory=".hooks.MutatorTransform"
+      name="plone.caching.mutator"
+      />
 
-    <!-- Mutator for streaming responses -->
-    <subscriber handler=".hooks.modifyStreamingResponse" />
+  <!-- Mutator for streaming responses -->
+  <subscriber handler=".hooks.modifyStreamingResponse" />
 
 </configure>
```

### Comparing `plone.caching-1.2.2/plone/caching/hooks.py` & `plone.caching-2.0.0/plone/caching/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.caching.interfaces import X_CACHE_OPERATION_HEADER
 from plone.caching.interfaces import X_CACHE_RULE_HEADER
 from plone.caching.utils import findOperation
 from plone.transformchain.interfaces import DISABLE_TRANSFORM_REQUEST_KEY
 from plone.transformchain.interfaces import ITransform
 from ZODB.POSException import ConflictError
 from zope.component import adapter
@@ -12,15 +11,15 @@
 from zope.interface import Interface
 from ZPublisher.interfaces import IPubAfterTraversal
 from ZPublisher.interfaces import IPubBeforeStreaming
 
 import logging
 
 
-logger = logging.getLogger('plone.caching')
+logger = logging.getLogger("plone.caching")
 
 
 class IStreamedResponse(Interface):
     """Marker applied when we intercepted a streaming response. This allows
     us to avoid applying the same rules twice, since the normal hook may also
     be executed for streaming responses (albeit on a seemingly empty body,
     and after the response has been sent).
@@ -32,20 +31,20 @@
     published resource (e.g. a view) is called, and render a specific response
     body and status provided by an intercepting caching operation instead.
     """
 
     responseBody = None
     status = None
 
-    def __init__(self, status=304, responseBody=u""):
+    def __init__(self, status=304, responseBody=""):
         self.status = status
         self.responseBody = responseBody
 
 
-class InterceptorResponse(object):
+class InterceptorResponse:
     """View for the Intercepted exception, serving to return an empty
     response in the case of an intercepted response.
     """
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
@@ -63,38 +62,32 @@
     actual response (typically an empty response) is then set via a view on
     the exception. We set and lock the response status to avoid defaulting to
     a 404 exception.
     """
 
     try:
         request = event.request
-        published = request.get('PUBLISHED', None)
+        published = request.get("PUBLISHED", None)
         rule, operationName, operation = findOperation(request)
 
         if rule is None:
             return
 
         request.response.setHeader(X_CACHE_RULE_HEADER, rule)
         logger.debug(
-            'Published: %s Ruleset: %s Operation: %s',
-            repr(published),
-            rule,
-            operation
+            "Published: %s Ruleset: %s Operation: %s", repr(published), rule, operation
         )
 
         if operation is not None:
             responseBody = operation.interceptResponse(rule, request.response)
 
             if responseBody is not None:
                 # Only put this in the response if the operation actually
                 # intercepted something
-                request.response.setHeader(
-                    X_CACHE_OPERATION_HEADER,
-                    operationName
-                )
+                request.response.setHeader(X_CACHE_OPERATION_HEADER, operationName)
 
                 # Stop any post-processing, including the operation's response
                 # modification
                 if DISABLE_TRANSFORM_REQUEST_KEY not in request.environ:
                     request.environ[DISABLE_TRANSFORM_REQUEST_KEY] = True
 
                 # The view is liable to have set a response status. Lock it
@@ -107,22 +100,21 @@
 
     except ConflictError:
         raise
     except Intercepted:
         raise
     except Exception:
         logging.exception(
-            'Swallowed exception in plone.caching IPubAfterTraversal event '
-            'handler'
+            "Swallowed exception in plone.caching IPubAfterTraversal event " "handler"
         )
 
 
 @implementer(ITransform)
 @adapter(Interface, Interface)
-class MutatorTransform(object):
+class MutatorTransform:
     """Transformation using plone.transformchain.
 
     This is registered at order 12000, i.e. "late". A typical transform
     chain order may include:
 
     * lxml transforms (e.g. plone.app.blocks, collectivexdv) => 8000-8999
     * gzip => 10000
@@ -155,32 +147,30 @@
         request = self.request
 
         # Abort if this was a streamed request handled by our event handler
         # below
         if IStreamedResponse.providedBy(request):
             return
 
-        published = request.get('PUBLISHED', None)
+        published = request.get("PUBLISHED", None)
         rule, operationName, operation = findOperation(request)
 
         if rule is None:
             return
 
         request.response.setHeader(X_CACHE_RULE_HEADER, rule)
         logger.debug(
-            'Published: %s Ruleset: %s Operation: %s',
-            repr(published),
-            rule,
-            operation
+            "Published: %s Ruleset: %s Operation: %s", repr(published), rule, operation
         )
 
         if operation is not None:
             request.response.setHeader(X_CACHE_OPERATION_HEADER, operationName)
             operation.modifyResponse(rule, request.response)
 
+
 # Hook for streaming responses - does not use plone.transformchain, since
 # sequencing is less likely to be an issue here
 
 
 @adapter(IPubBeforeStreaming)
 def modifyStreamingResponse(event):
     """Invoke the modifyResponse() method of a caching operation, if one
@@ -195,25 +185,22 @@
     if request is None:
         return
 
     # Mark the response to allow us to avoid attempting a modify operation
     # again in the normal hook above
     alsoProvides(request, IStreamedResponse)
 
-    published = request.get('PUBLISHED', None)
+    published = request.get("PUBLISHED", None)
 
     rule, operationName, operation = findOperation(request)
 
     if rule is None:
         return
 
     response.setHeader(X_CACHE_RULE_HEADER, rule)
     logger.debug(
-        'Published: %s Ruleset: %s Operation: %s',
-        repr(published),
-        rule,
-        operation
+        "Published: %s Ruleset: %s Operation: %s", repr(published), rule, operation
     )
 
     if operation is not None:
         response.setHeader(X_CACHE_OPERATION_HEADER, operationName)
         operation.modifyResponse(rule, response)
```

### Comparing `plone.caching-1.2.2/plone/caching/lookup.py` & `plone.caching-2.0.0/plone/caching/lookup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 from plone.caching.interfaces import IRulesetLookup
 from z3c.caching.registry import lookup
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 @implementer(IRulesetLookup)
 @adapter(Interface, Interface)
-class DefaultRulesetLookup(object):
+class DefaultRulesetLookup:
     """Default ruleset lookup.
 
     Only override this if you have very special needs. The safest option is
     to use ``z3c.caching`` to set rulesets.
     """
 
     def __init__(self, published, request):
```

### Comparing `plone.caching-1.2.2/plone/caching/tests/test_utils.py` & `plone.caching-2.0.0/plone/caching/tests/test_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.caching.interfaces import ICachingOperationType
 from plone.caching.utils import lookupOption
 from plone.caching.utils import lookupOptions
 from plone.registry import field
 from plone.registry import FieldRef
 from plone.registry import Record
 from plone.registry import Registry
@@ -15,179 +14,154 @@
 import zope.component.testing
 
 
 _marker = object()
 
 
 class TestLookupOption(unittest.TestCase):
-
     def tearDown(self):
         zope.component.testing.tearDown()
 
     def test_lookupOption_no_registry(self):
         result = lookupOption(
-            'plone.caching.tests',
-            'testrule',
-            'test',
-            default=_marker
+            "plone.caching.tests", "testrule", "test", default=_marker
         )
         self.assertTrue(result is _marker)
 
     def test_lookupOption_no_record(self):
         provideUtility(Registry(), IRegistry)
 
         result = lookupOption(
-            'plone.caching.tests',
-            'testrule',
-            'test',
-            default=_marker
+            "plone.caching.tests", "testrule", "test", default=_marker
         )
         self.assertTrue(result is _marker)
 
     def test_lookupOption_default(self):
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
 
-        registry.records['plone.caching.tests.test'] = Record(
-            field.TextLine(),
-            u'default'
+        registry.records["plone.caching.tests.test"] = Record(
+            field.TextLine(), "default"
         )
 
         result = lookupOption(
-            'plone.caching.tests',
-            'testrule',
-            'test',
-            default=_marker
+            "plone.caching.tests", "testrule", "test", default=_marker
         )
-        self.assertEqual(u'default', result)
+        self.assertEqual("default", result)
 
     def test_lookupOption_override(self):
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
 
-        registry.records['plone.caching.tests.test'] = r = Record(
-            field.TextLine(),
-            u'default'
-        )
-        registry.records['plone.caching.tests.testrule.test'] = Record(
-            FieldRef(r.__name__, r.field),
-            u'override'
+        registry.records["plone.caching.tests.test"] = r = Record(
+            field.TextLine(), "default"
+        )
+        registry.records["plone.caching.tests.testrule.test"] = Record(
+            FieldRef(r.__name__, r.field), "override"
         )
 
         result = lookupOption(
-            'plone.caching.tests',
-            'testrule',
-            'test',
-            default=_marker
+            "plone.caching.tests", "testrule", "test", default=_marker
         )
-        self.assertEqual(u'override', result)
+        self.assertEqual("override", result)
 
 
 class TestLookupOptions(unittest.TestCase):
-
     def tearDown(self):
         zope.component.testing.tearDown()
 
     def test_lookupOptions_no_registry(self):
-
         @provider(ICachingOperationType)
-        class DummyOperation(object):
-
-            title = u''
-            description = u''
-            prefix = 'plone.caching.tests'
-            options = ('test1', 'test2',)
+        class DummyOperation:
+            title = ""
+            description = ""
+            prefix = "plone.caching.tests"
+            options = (
+                "test1",
+                "test2",
+            )
 
-        result = lookupOptions(DummyOperation, 'testrule', default=_marker)
-        self.assertEqual({'test1': _marker, 'test2': _marker}, result)
+        result = lookupOptions(DummyOperation, "testrule", default=_marker)
+        self.assertEqual({"test1": _marker, "test2": _marker}, result)
 
     def test_lookupOptions_no_records(self):
         provideUtility(Registry(), IRegistry)
 
         @provider(ICachingOperationType)
-        class DummyOperation(object):
-
-            title = u''
-            description = u''
-            prefix = 'plone.caching.tests'
-            options = ('test1', 'test2',)
+        class DummyOperation:
+            title = ""
+            description = ""
+            prefix = "plone.caching.tests"
+            options = (
+                "test1",
+                "test2",
+            )
 
-        result = lookupOptions(DummyOperation, 'testrule', default=_marker)
-        self.assertEqual({'test1': _marker, 'test2': _marker}, result)
+        result = lookupOptions(DummyOperation, "testrule", default=_marker)
+        self.assertEqual({"test1": _marker, "test2": _marker}, result)
 
     def test_lookupOptions_default(self):
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
 
-        registry.records['plone.caching.tests.test2'] = Record(
-            field.TextLine(),
-            u'foo'
-        )
+        registry.records["plone.caching.tests.test2"] = Record(field.TextLine(), "foo")
 
         @provider(ICachingOperationType)
-        class DummyOperation(object):
-
-            title = u''
-            description = u''
-            prefix = 'plone.caching.tests'
-            options = ('test1', 'test2',)
+        class DummyOperation:
+            title = ""
+            description = ""
+            prefix = "plone.caching.tests"
+            options = (
+                "test1",
+                "test2",
+            )
 
-        result = lookupOptions(DummyOperation, 'testrule', default=_marker)
-        self.assertEqual({'test1': _marker, 'test2': u'foo'}, result)
+        result = lookupOptions(DummyOperation, "testrule", default=_marker)
+        self.assertEqual({"test1": _marker, "test2": "foo"}, result)
 
     def test_lookupOptions_override(self):
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
 
-        registry.records['plone.caching.tests.test1'] = Record(
-            field.TextLine(),
-            u'foo'
-        )
-        registry.records['plone.caching.tests.test2'] = Record(
-            field.TextLine(),
-            u'bar'
-        )
-        registry.records['plone.caching.tests.testrule.test2'] = Record(
-            field.TextLine(),
-            u'baz'
+        registry.records["plone.caching.tests.test1"] = Record(field.TextLine(), "foo")
+        registry.records["plone.caching.tests.test2"] = Record(field.TextLine(), "bar")
+        registry.records["plone.caching.tests.testrule.test2"] = Record(
+            field.TextLine(), "baz"
         )
 
         @provider(ICachingOperationType)
-        class DummyOperation(object):
-
-            title = u''
-            description = u''
-            prefix = 'plone.caching.tests'
-            options = ('test1', 'test2',)
+        class DummyOperation:
+            title = ""
+            description = ""
+            prefix = "plone.caching.tests"
+            options = (
+                "test1",
+                "test2",
+            )
 
-        result = lookupOptions(DummyOperation, 'testrule', default=_marker)
-        self.assertEqual({'test1': u'foo', 'test2': u'baz'}, result)
+        result = lookupOptions(DummyOperation, "testrule", default=_marker)
+        self.assertEqual({"test1": "foo", "test2": "baz"}, result)
 
     def test_lookupOptions_named(self):
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
 
-        registry.records['plone.caching.tests.test2'] = Record(
-            field.TextLine(),
-            u'foo'
-        )
+        registry.records["plone.caching.tests.test2"] = Record(field.TextLine(), "foo")
 
         @provider(ICachingOperationType)
-        class DummyOperation(object):
-
-            title = u''
-            description = u''
-            prefix = 'plone.caching.tests'
-            options = ('test1', 'test2',)
+        class DummyOperation:
+            title = ""
+            description = ""
+            prefix = "plone.caching.tests"
+            options = (
+                "test1",
+                "test2",
+            )
 
-        provideUtility(DummyOperation, name=u'plone.caching.tests')
+        provideUtility(DummyOperation, name="plone.caching.tests")
 
-        result = lookupOptions(
-            u'plone.caching.tests',
-            'testrule',
-            default=_marker
-        )
-        self.assertEqual({'test1': _marker, 'test2': u'foo'}, result)
+        result = lookupOptions("plone.caching.tests", "testrule", default=_marker)
+        self.assertEqual({"test1": _marker, "test2": "foo"}, result)
 
 
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `plone.caching-1.2.2/plone/caching/tests/test_operations.py` & `plone.caching-2.0.0/plone/caching/tests/test_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.caching.interfaces import ICachingOperation
 from plone.caching.operations import Chain
 from plone.caching.testing import IMPLICIT_RULESET_REGISTRY_UNIT_TESTING
 from plone.registry import field
 from plone.registry import Record
 from plone.registry import Registry
 from plone.registry.interfaces import IRegistry
@@ -14,205 +13,192 @@
 
 import unittest
 
 
 _marker = object()
 
 
-class DummyView(object):
+class DummyView:
     pass
 
 
 class DummyResponse(dict):
-
     def addHeader(self, name, value):
         self.setdefault(name, []).append(value)
 
     def setHeader(self, name, value):
         self[name] = value
 
 
 class DummyRequest(dict):
     def __init__(self, published, response):
-        self['PUBLISHED'] = published
+        self["PUBLISHED"] = published
         self.response = response
 
 
 class TestChain(unittest.TestCase):
-
     layer = IMPLICIT_RULESET_REGISTRY_UNIT_TESTING
 
     def setUp(self):
         self.registry = Registry()
         provideUtility(self.registry, IRegistry)
 
     def test_no_option(self):
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         chain = Chain(view, request)
-        ret = chain.interceptResponse('testrule', request.response)
-        chain.modifyResponse('testrule', request.response)
+        ret = chain.interceptResponse("testrule", request.response)
+        chain.modifyResponse("testrule", request.response)
 
         self.assertEqual(None, ret)
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_operations_list_not_set(self):
-
-        self.registry.records[
-            '{0}.operations'.format(Chain.prefix)
-        ] = Record(field.List(value_type=field.Text()))
+        self.registry.records[f"{Chain.prefix}.operations"] = Record(
+            field.List(value_type=field.Text())
+        )
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         chain = Chain(view, request)
-        ret = chain.interceptResponse('testrule', request.response)
-        chain.modifyResponse('testrule', request.response)
+        ret = chain.interceptResponse("testrule", request.response)
+        chain.modifyResponse("testrule", request.response)
 
         self.assertEqual(None, ret)
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_operations_empty(self):
-
-        self.registry.records[
-            '{0}.operations'.format(Chain.prefix)
-        ] = Record(field.List(value_type=field.Text()), [])
+        self.registry.records[f"{Chain.prefix}.operations"] = Record(
+            field.List(value_type=field.Text()), []
+        )
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         chain = Chain(view, request)
-        ret = chain.interceptResponse('testrule', request.response)
-        chain.modifyResponse('testrule', request.response)
+        ret = chain.interceptResponse("testrule", request.response)
+        chain.modifyResponse("testrule", request.response)
 
         self.assertEqual(None, ret)
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_chained_operations_not_found(self):
-
-        self.registry.records[
-            '{0}.operations'.format(Chain.prefix)
-        ] = Record(field.List(value_type=field.Text()), [u'op1'])
+        self.registry.records[f"{Chain.prefix}.operations"] = Record(
+            field.List(value_type=field.Text()), ["op1"]
+        )
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         chain = Chain(view, request)
-        chain.modifyResponse('testrule', request.response)
+        chain.modifyResponse("testrule", request.response)
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_multiple_operations_one_found(self):
-        self.registry.records[
-            '{0}.operations'.format(Chain.prefix)
-        ] = Record(field.List(value_type=field.Text()), [u'op1', u'op2'])
+        self.registry.records[f"{Chain.prefix}.operations"] = Record(
+            field.List(value_type=field.Text()), ["op1", "op2"]
+        )
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
-                return u'foo'
+                return "foo"
 
             def modifyResponse(self, rulename, response):
-                response['X-Mutated'] = rulename
+                response["X-Mutated"] = rulename
 
-        provideAdapter(DummyOperation, name='op2')
+        provideAdapter(DummyOperation, name="op2")
 
         chain = Chain(view, request)
-        ret = chain.interceptResponse('testrule', request.response)
+        ret = chain.interceptResponse("testrule", request.response)
 
-        self.assertEqual(u'foo', ret)
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'X-Cache-Chain-Operations': 'op2'},
-            dict(request.response)
-        )
+        self.assertEqual("foo", ret)
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"X-Cache-Chain-Operations": "op2"}, dict(request.response))
 
         request = DummyRequest(view, DummyResponse())
         chain = Chain(view, request)
-        chain.modifyResponse('testrule', request.response)
+        chain.modifyResponse("testrule", request.response)
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual(
-            {'X-Mutated': 'testrule',
-             'X-Cache-Chain-Operations': 'op2'},
-            dict(request.response)
+            {"X-Mutated": "testrule", "X-Cache-Chain-Operations": "op2"},
+            dict(request.response),
         )
 
     def test_multiple_operations_multiple_found(self):
-        self.registry.records[
-            '{0}.operations'.format(Chain.prefix)
-        ] = Record(field.List(value_type=field.Text()), [u'op1', u'op2'])
+        self.registry.records[f"{Chain.prefix}.operations"] = Record(
+            field.List(value_type=field.Text()), ["op1", "op2"]
+        )
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation1(object):
-
+        class DummyOperation1:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
-                return u'foo'
+                return "foo"
 
             def modifyResponse(self, rulename, response):
-                response['X-Mutated-1'] = rulename
+                response["X-Mutated-1"] = rulename
 
-        provideAdapter(DummyOperation1, name='op1')
+        provideAdapter(DummyOperation1, name="op1")
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation2(object):
-
+        class DummyOperation2:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
-                return u'bar'
+                return "bar"
 
             def modifyResponse(self, rulename, response):
-                response['X-Mutated-2'] = rulename
+                response["X-Mutated-2"] = rulename
 
-        provideAdapter(DummyOperation2, name='op2')
+        provideAdapter(DummyOperation2, name="op2")
 
         chain = Chain(view, request)
-        ret = chain.interceptResponse('testrule', request.response)
+        ret = chain.interceptResponse("testrule", request.response)
 
-        self.assertEqual(u'foo', ret)
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'X-Cache-Chain-Operations': 'op1'},
-            dict(request.response)
-        )
+        self.assertEqual("foo", ret)
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"X-Cache-Chain-Operations": "op1"}, dict(request.response))
 
         request = DummyRequest(view, DummyResponse())
         chain = Chain(view, request)
-        chain.modifyResponse('testrule', request.response)
+        chain.modifyResponse("testrule", request.response)
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual(
-            {'X-Mutated-1': 'testrule',
-             'X-Mutated-2': 'testrule',
-             'X-Cache-Chain-Operations': 'op1; op2'},
-            dict(request.response)
+            {
+                "X-Mutated-1": "testrule",
+                "X-Mutated-2": "testrule",
+                "X-Cache-Chain-Operations": "op1; op2",
+            },
+            dict(request.response),
         )
 
 
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `plone.caching-1.2.2/plone/caching/tests/test_hooks.py` & `plone.caching-2.0.0/plone/caching/tests/test_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.caching.hooks import intercept
 from plone.caching.hooks import Intercepted
 from plone.caching.hooks import InterceptorResponse
 from plone.caching.hooks import modifyStreamingResponse
 from plone.caching.hooks import MutatorTransform
 from plone.caching.interfaces import ICacheSettings
 from plone.caching.interfaces import ICachingOperation
@@ -22,25 +21,24 @@
 from zope.interface import implementer
 from zope.interface import Interface
 
 import unittest
 import z3c.caching.registry
 
 
-class DummyView(object):
+class DummyView:
     pass
 
 
-class DummyResource(object):
+class DummyResource:
     def index_html(self):
-        return b'binary data'
+        return b"binary data"
 
 
 class DummyResponse(dict):
-
     locked = None
 
     def addHeader(self, name, value):
         self.setdefault(name, []).append(value)
 
     def setHeader(self, name, value):
         self[name] = [value]
@@ -52,31 +50,30 @@
 
     def getStatus(self):
         return self.status
 
 
 class DummyRequest(dict):
     def __init__(self, published, response):
-        self['PUBLISHED'] = published
+        self["PUBLISHED"] = published
         self.response = response
         self.environ = {}
 
 
-class DummyEvent(object):
+class DummyEvent:
     def __init__(self, request):
         self.request = request
 
 
-class DummyStreamingEvent(object):
+class DummyStreamingEvent:
     def __init__(self, response):
         self.response = response
 
 
 class TestMutateResponse(unittest.TestCase):
-
     layer = IMPLICIT_RULESET_REGISTRY_UNIT_TESTING
 
     def setUp(self):
         provideAdapter(persistentFieldAdapter)
 
     def test_no_published_object(self):
         provideAdapter(DefaultRulesetLookup)
@@ -84,324 +81,332 @@
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
         request = DummyRequest(None, DummyResponse())
 
-        MutatorTransform(None, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(None, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': None}, dict(request))
+        self.assertEqual({"PUBLISHED": None}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_registry(self):
         provideAdapter(DefaultRulesetLookup)
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_records(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_mapping(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
+        z3c.caching.registry.register(DummyView, "testrule")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_cache_rule(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        settings.operationMapping = {'testrule': 'dummy'}
+        settings.operationMapping = {"testrule": "dummy"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_lookup_adapter(self):
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'dummy'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "dummy"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_operation_name_not_found(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'foo': 'bar'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"foo": "bar"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'X-Cache-Rule': ['testrule']},
-            dict(request.response)
-        )
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"X-Cache-Rule": ["testrule"]}, dict(request.response))
 
     def test_operation_not_found(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'notfound'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "notfound"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'X-Cache-Rule': ['testrule']},
-            dict(request.response)
-        )
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"X-Cache-Rule": ["testrule"]}, dict(request.response))
 
     def test_match_unicode(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_match_bytes(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformBytes('', 'utf-8')
+        MutatorTransform(view, request).transformBytes("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_match_iterable(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformIterable([''], 'utf-8')
+        MutatorTransform(view, request).transformIterable([""], "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_match_method(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyResource, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyResource, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         resource = DummyResource()
         request = DummyRequest(resource.index_html, DummyResponse())
 
-        MutatorTransform(resource, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(resource, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': resource.index_html}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": resource.index_html}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_off_switch(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = False
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response['X-Mutated'] = rulename
+                response["X-Mutated"] = rulename
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
-        MutatorTransform(view, request).transformUnicode(u'', 'utf-8')
+        MutatorTransform(view, request).transformUnicode("", "utf-8")
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
 
 class TestMutateResponseStreaming(unittest.TestCase):
-
     layer = IMPLICIT_RULESET_REGISTRY_UNIT_TESTING
 
     def setUp(self):
         provideAdapter(persistentFieldAdapter)
 
     def tearDown(self):
         clearRequest()
@@ -416,348 +421,356 @@
 
         response = DummyResponse()
         request = DummyRequest(None, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': None}, dict(request))
+        self.assertEqual({"PUBLISHED": None}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_registry(self):
         provideAdapter(DefaultRulesetLookup)
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_records(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_mapping(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
+        z3c.caching.registry.register(DummyView, "testrule")
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_cache_rule(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        settings.operationMapping = {'testrule': 'dummy'}
+        settings.operationMapping = {"testrule": "dummy"}
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_lookup_adapter(self):
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'dummy'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "dummy"}
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_operation_name_not_found(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'foo': 'bar'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"foo": "bar"}
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'X-Cache-Rule': ['testrule']},
-            dict(request.response)
-        )
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"X-Cache-Rule": ["testrule"]}, dict(request.response))
 
     def test_operation_not_found(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'notfound'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "notfound"}
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'X-Cache-Rule': ['testrule']},
-            dict(request.response)
-        )
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"X-Cache-Rule": ["testrule"]}, dict(request.response))
 
     def test_match_unicode(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_match_bytes(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_match_iterable(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_match_method(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyResource, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyResource, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         resource = DummyResource()
         response = DummyResponse()
         request = DummyRequest(resource.index_html, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': resource.index_html}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Operation': ['op1'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": resource.index_html}, dict(request))
+        self.assertEqual(
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
+        )
 
     def test_off_switch(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = False
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def interceptResponse(self, rulename, response):
                 return None
 
             def modifyResponse(self, rulename, response):
-                response['X-Mutated'] = rulename
+                response["X-Mutated"] = rulename
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         response = DummyResponse()
         request = DummyRequest(view, response)
         setRequest(request)
 
         modifyStreamingResponse(DummyStreamingEvent(response))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
 
 class TestIntercept(unittest.TestCase):
-
     layer = IMPLICIT_RULESET_REGISTRY_UNIT_TESTING
 
     def setUp(self):
         provideAdapter(persistentFieldAdapter)
 
     def test_no_published_object(self):
         provideAdapter(DefaultRulesetLookup)
@@ -766,388 +779,375 @@
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
         request = DummyRequest(None, DummyResponse())
 
         intercept(DummyEvent(request))
-        self.assertEqual({'PUBLISHED': None}, dict(request))
+        self.assertEqual({"PUBLISHED": None}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_registry(self):
         provideAdapter(DefaultRulesetLookup)
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         intercept(DummyEvent(request))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_records(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         intercept(DummyEvent(request))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_cache_rule(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        settings.operationMapping = {'testrule': 'dummy'}
+        settings.operationMapping = {"testrule": "dummy"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         intercept(DummyEvent(request))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_no_mapping(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
         settings.operationMapping = None
 
-        z3c.caching.registry.register(DummyView, 'testrule')
+        z3c.caching.registry.register(DummyView, "testrule")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         intercept(DummyEvent(request))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_operation_not_found(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'notfound'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "notfound"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         intercept(DummyEvent(request))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'X-Cache-Rule': ['testrule']},
-            dict(request.response)
-        )
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"X-Cache-Rule": ["testrule"]}, dict(request.response))
 
     def test_match_abort(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def modifyResponse(self, rulename, response):
                 pass
 
             def interceptResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
                 return None
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         intercept(DummyEvent(request))
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual({'X-Cache-Rule': ['testrule'],
-                          'X-Cache-Foo': ['test']}, dict(request.response))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual(
+            {"X-Cache-Rule": ["testrule"], "X-Cache-Foo": ["test"]},
+            dict(request.response),
+        )
 
     def test_match_body(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def modifyResponse(self, rulename, response):
                 pass
 
             def interceptResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
                 response.setStatus(304)
-                return u'dummy'
+                return "dummy"
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         try:
             intercept(DummyEvent(request))
             self.fail()
         except Intercepted as e:
-            self.assertEqual(u'dummy', e.responseBody)
+            self.assertEqual("dummy", e.responseBody)
             self.assertEqual(304, e.status)
             self.assertEqual(304, request.response.status)
             self.assertEqual(True, request.response.locked)
         except Exception as e:
             self.fail(str(e))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
-        self.assertEqual(
-            {'plone.transformchain.disable': True},
-            request.environ
-        )
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"plone.transformchain.disable": True}, request.environ)
         self.assertEqual(
-            {'X-Cache-Rule': ['testrule'],
-             'X-Cache-Operation': ['op1'],
-             'X-Cache-Foo': ['test']},
-            dict(request.response)
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
         )
 
     def test_match_body_explicitly_enable_transform_chain(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def modifyResponse(self, rulename, response):
                 pass
 
             def interceptResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
                 response.setStatus(304)
-                self.request.environ['plone.transformchain.disable'] = False
-                return u'dummy'
+                self.request.environ["plone.transformchain.disable"] = False
+                return "dummy"
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         try:
             intercept(DummyEvent(request))
             self.fail()
         except Intercepted as e:
-            self.assertEqual(u'dummy', e.responseBody)
+            self.assertEqual("dummy", e.responseBody)
             self.assertEqual(304, e.status)
             self.assertEqual(304, request.response.status)
             self.assertEqual(True, request.response.locked)
         except Exception as e:
             self.fail(str(e))
 
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
+        self.assertEqual({"plone.transformchain.disable": False}, request.environ)
         self.assertEqual(
-            {'plone.transformchain.disable': False},
-            request.environ
-        )
-        self.assertEqual(
-            {'X-Cache-Rule': ['testrule'],
-             'X-Cache-Operation': ['op1'],
-             'X-Cache-Foo': ['test']},
-            dict(request.response)
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
         )
 
     def test_match_body_method(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
 
-        z3c.caching.registry.register(DummyResource, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyResource, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def modifyResponse(self, rulename, response):
                 pass
 
             def interceptResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
+                response.addHeader("X-Cache-Foo", "test")
                 response.setStatus(200)
-                return u'dummy'
+                return "dummy"
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         resource = DummyResource()
         request = DummyRequest(resource.index_html, DummyResponse())
         try:
             intercept(DummyEvent(request))
             self.fail()
         except Intercepted as e:
-            self.assertEqual(u'dummy', e.responseBody)
+            self.assertEqual("dummy", e.responseBody)
             self.assertEqual(200, e.status)
             self.assertEqual(200, request.response.status)
             self.assertEqual(True, request.response.locked)
         except Exception as e:
             self.fail(str(e))
 
-        self.assertEqual({'PUBLISHED': resource.index_html}, dict(request))
+        self.assertEqual({"PUBLISHED": resource.index_html}, dict(request))
+        self.assertEqual({"plone.transformchain.disable": True}, request.environ)
         self.assertEqual(
-            {'plone.transformchain.disable': True},
-            request.environ
-        )
-        self.assertEqual(
-            {'X-Cache-Rule': ['testrule'],
-             'X-Cache-Operation': ['op1'],
-             'X-Cache-Foo': ['test']},
-            dict(request.response)
+            {
+                "X-Cache-Rule": ["testrule"],
+                "X-Cache-Operation": ["op1"],
+                "X-Cache-Foo": ["test"],
+            },
+            dict(request.response),
         )
 
     def test_off_switch(self):
         provideAdapter(DefaultRulesetLookup)
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = False
 
-        z3c.caching.registry.register(DummyView, 'testrule')
-        settings.operationMapping = {'testrule': 'op1'}
+        z3c.caching.registry.register(DummyView, "testrule")
+        settings.operationMapping = {"testrule": "op1"}
 
         @implementer(ICachingOperation)
         @adapter(Interface, Interface)
-        class DummyOperation(object):
-
+        class DummyOperation:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def modifyResponse(self, rulename, response):
                 pass
 
             def interceptResponse(self, rulename, response):
-                response.addHeader('X-Cache-Foo', 'test')
-                return u'dummy'
+                response.addHeader("X-Cache-Foo", "test")
+                return "dummy"
 
-        provideAdapter(DummyOperation, name='op1')
+        provideAdapter(DummyOperation, name="op1")
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         intercept(DummyEvent(request))
-        self.assertEqual({'PUBLISHED': view}, dict(request))
+        self.assertEqual({"PUBLISHED": view}, dict(request))
         self.assertEqual({}, dict(request.response))
 
     def test_dont_swallow_conflict_error(self):
-
         @implementer(IRulesetLookup)
         @adapter(Interface, Interface)
-        class DummyRulesetLookup(object):
-
+        class DummyRulesetLookup:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def __call__(self):
                 raise ConflictError()
 
         provideAdapter(DummyRulesetLookup)
 
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
-        settings.operationMapping = {'foo': 'bar'}
+        settings.operationMapping = {"foo": "bar"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         self.assertRaises(ConflictError, intercept, DummyEvent(request))
 
     def test_swallow_other_error(self):
-
         @implementer(IRulesetLookup)
         @adapter(Interface, Interface)
-        class DummyRulesetLookup(object):
-
+        class DummyRulesetLookup:
             def __init__(self, published, request):
                 self.published = published
                 self.request = request
 
             def __call__(self):
-                raise AttributeError('Should be swallowed and logged')
+                raise AttributeError("Should be swallowed and logged")
 
         provideAdapter(DummyRulesetLookup)
 
         provideUtility(Registry(), IRegistry)
         registry = getUtility(IRegistry)
         registry.registerInterface(ICacheSettings)
         settings = registry.forInterface(ICacheSettings)
         settings.enabled = True
-        settings.operationMapping = {'foo': 'bar'}
+        settings.operationMapping = {"foo": "bar"}
 
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
 
         try:
             intercept(DummyEvent(request))
         except Exception:
-            self.fail('Intercept should not raise')
+            self.fail("Intercept should not raise")
 
     def test_exception_view(self):
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
-        exc = Intercepted(status=200, responseBody=u'Test')
+        exc = Intercepted(status=200, responseBody="Test")
         excView = InterceptorResponse(exc, request)
-        self.assertEqual(u'Test', excView())
+        self.assertEqual("Test", excView())
 
 
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `plone.caching-1.2.2/plone/caching/tests/test_lookup.py` & `plone.caching-2.0.0/plone/caching/tests/test_lookup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-# -*- coding: utf-8 -*-
 from plone.caching.lookup import DefaultRulesetLookup
 from plone.caching.testing import IMPLICIT_RULESET_REGISTRY_UNIT_TESTING
 
 import unittest
 import z3c.caching.registry
 
 
-class DummyView(object):
+class DummyView:
     pass
 
 
 class DummyResponse(dict):
-
     def addHeader(self, name, value):
         self.setdefault(name, []).append(value)
 
 
 class DummyRequest(dict):
     def __init__(self, published, response):
-        self['PUBLISHED'] = published
+        self["PUBLISHED"] = published
         self.response = response
 
 
 class TestLookup(unittest.TestCase):
-
     layer = IMPLICIT_RULESET_REGISTRY_UNIT_TESTING
 
     def test_no_cache_rule(self):
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
         self.assertEqual(None, DefaultRulesetLookup(view, request)())
 
     def test_match(self):
-        z3c.caching.registry.register(DummyView, 'testrule')
+        z3c.caching.registry.register(DummyView, "testrule")
         view = DummyView()
         request = DummyRequest(view, DummyResponse())
-        self.assertEqual('testrule', DefaultRulesetLookup(view, request)())
+        self.assertEqual("testrule", DefaultRulesetLookup(view, request)())
 
 
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `plone.caching-1.2.2/plone/caching/operations.py` & `plone.caching-2.0.0/plone/caching/operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,76 @@
-# -*- coding: utf-8 -*-
 from plone.caching.interfaces import _
 from plone.caching.interfaces import ICachingOperation
 from plone.caching.interfaces import ICachingOperationType
 from plone.caching.utils import lookupOptions
 from zope.component import adapter
 from zope.component import queryMultiAdapter
 from zope.interface import implementer
 from zope.interface import Interface
 from zope.interface import provider
 
 
 @implementer(ICachingOperation)
 @provider(ICachingOperationType)
 @adapter(Interface, Interface)
-class Chain(object):
+class Chain:
     """Caching operation which chains together several other operations.
 
     When intercepting the response, the first chained operation to return a
     value will be used. Subsequent operations are ignored. When modifying the
     response, all operations will be called, in order.
 
     The names of the operations to execute are found in the ``plone.registry``
     option ``plone.caching.operations.chain.operations`` by default, and can
     be customised on a per-rule basis with
     ``plone.caching.operations.chain.${rulename}.chain``.
 
     The option must be a sequence type (e.g. a ``Tuple``).
     """
-    title = _(u"Chain")
-    description = _(u"Allows multiple operations to be chained together")
-    prefix = 'plone.caching.operations.chain'
-    options = ('operations',)
+
+    title = _("Chain")
+    description = _("Allows multiple operations to be chained together")
+    prefix = "plone.caching.operations.chain"
+    options = ("operations",)
 
     def __init__(self, published, request):
         self.published = published
         self.request = request
 
     def interceptResponse(self, rulename, response):
         options = lookupOptions(self.__class__, rulename)
 
         chained = []
 
-        if options['operations']:
-            for name in options['operations']:
-
+        if options["operations"]:
+            for name in options["operations"]:
                 operation = queryMultiAdapter(
-                    (self.published, self.request),
-                    ICachingOperation,
-                    name=name
+                    (self.published, self.request), ICachingOperation, name=name
                 )
 
                 if operation is not None:
                     chained.append(name)
 
                     value = operation.interceptResponse(rulename, response)
                     if value is not None:
                         response.setHeader(
-                            'X-Cache-Chain-Operations',
-                            '; '.join(chained)
+                            "X-Cache-Chain-Operations", "; ".join(chained)
                         )
                         return value
 
     def modifyResponse(self, rulename, response):
         options = lookupOptions(self.__class__, rulename)
 
         chained = []
 
-        if options['operations']:
-            for name in options['operations']:
-
+        if options["operations"]:
+            for name in options["operations"]:
                 operation = queryMultiAdapter(
-                    (self.published, self.request),
-                    ICachingOperation,
-                    name=name
+                    (self.published, self.request), ICachingOperation, name=name
                 )
 
                 if operation is not None:
                     chained.append(name)
                     operation.modifyResponse(rulename, response)
 
         if chained:
-            response.setHeader('X-Cache-Chain-Operations', '; '.join(chained))
+            response.setHeader("X-Cache-Chain-Operations", "; ".join(chained))
```

### Comparing `plone.caching-1.2.2/plone/caching/utils.py` & `plone.caching-2.0.0/plone/caching/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.caching.interfaces import ICacheSettings
 from plone.caching.interfaces import ICachingOperation
 from plone.caching.interfaces import ICachingOperationType
 from plone.caching.interfaces import IRulesetLookup
 from plone.registry.interfaces import IRegistry
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
@@ -26,21 +25,17 @@
 
     if not ICachingOperationType.providedBy(type_):
         type_ = getUtility(ICachingOperationType, name=type_)
 
     options = {}
     registry = queryUtility(IRegistry)
 
-    for option in getattr(type_, 'options', ()):
+    for option in getattr(type_, "options", ()):
         options[option] = lookupOption(
-            type_.prefix,
-            rulename,
-            option,
-            default,
-            registry
+            type_.prefix, rulename, option, default, registry
         )
 
     return options
 
 
 def lookupOption(prefix, rulename, option, default=None, _registry=None):
     """Look up an option for a particular caching operation.
@@ -62,59 +57,73 @@
 
     if registry is None:
         registry = queryUtility(IRegistry)
 
     if registry is None:
         return default
 
-    key = '.'.join((prefix, rulename, option,))
+    key = ".".join(
+        (
+            prefix,
+            rulename,
+            option,
+        )
+    )
     if key in registry:
         return registry[key]
 
-    key = '.'.join((prefix, option,))
+    key = ".".join(
+        (
+            prefix,
+            option,
+        )
+    )
     if key in registry:
         return registry[key]
 
     return default
 
 
 def findOperation(request):
-
-    published = request.get('PUBLISHED', None)
+    published = request.get("PUBLISHED", None)
     if published is None:
         return None, None, None
 
     # If we get a method, try to look up its class
     if isinstance(published, types.MethodType):
-        published = getattr(published, '__self__', published)
+        published = getattr(published, "__self__", published)
 
     registry = queryUtility(IRegistry)
     if registry is None:
         return None, None, None
 
     settings = registry.forInterface(ICacheSettings, check=False)
     if not settings.enabled:
         return None, None, None
 
     if settings.operationMapping is None:
         return None, None, None
 
-    lookup = queryMultiAdapter((published, request,), IRulesetLookup)
+    lookup = queryMultiAdapter(
+        (
+            published,
+            request,
+        ),
+        IRulesetLookup,
+    )
     if lookup is None:
         return None, None, None
 
     # From this point, we want to at least log
     rule = lookup()
 
     if rule is None:
         return None, None, None
 
     operationName = settings.operationMapping.get(rule, None)
     if operationName is None:
         return rule, None, None
 
     operation = queryMultiAdapter(
-        (published, request),
-        ICachingOperation,
-        name=operationName
+        (published, request), ICachingOperation, name=operationName
     )
     return rule, operationName, operation
```

### Comparing `plone.caching-1.2.2/plone/caching/testing.py` & `plone.caching-2.0.0/plone/caching/testing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.testing import Layer
 from plone.testing.zca import UNIT_TESTING
 from z3c.caching.registry import getGlobalRulesetRegistry
 from z3c.caching.registry import RulesetRegistry
 from zope.component import provideAdapter
 
 import zope.component.testing
@@ -16,15 +15,15 @@
     The plone.caching unit tests do not register utilities and therefore
     require the ruleset registry to be in non-explicit mode.
 
     See the plone.app.caching.setuphandlers.enableExplicitMode ZCML
     startup hook.
     """
 
-    defaultBases = (UNIT_TESTING, )
+    defaultBases = (UNIT_TESTING,)
 
     def testSetUp(self):
         provideAdapter(RulesetRegistry)
         self.disable_explicit_mode()
 
     def testTearDown(self):
         self.reset_explicit_mode()
@@ -37,9 +36,8 @@
 
     def reset_explicit_mode(self):
         registry = getGlobalRulesetRegistry()
         if registry is not None:
             registry.explicit = self._explicit_mode_cache
 
 
-IMPLICIT_RULESET_REGISTRY_UNIT_TESTING = (
-    ImplicitRulesetRegistryUnitTestingLayer())
+IMPLICIT_RULESET_REGISTRY_UNIT_TESTING = ImplicitRulesetRegistryUnitTestingLayer()
```

### Comparing `plone.caching-1.2.2/README.rst` & `plone.caching-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.caching-1.2.2/CHANGES.rst` & `plone.caching-2.0.0/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.0 (2023-04-15)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3b8337e6)
+
+
 1.2.2 (2020-04-20)
 ------------------
 
 Bug fixes:
 
 
 - Minor packaging updates. (#1)
```

