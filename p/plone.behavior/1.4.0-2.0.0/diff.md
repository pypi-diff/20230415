# Comparing `tmp/plone.behavior-1.4.0.tar.gz` & `tmp/plone.behavior-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.behavior-1.4.0.tar", last modified: Mon Sep  7 11:13:45 2020, max compression
+gzip compressed data, was "plone.behavior-2.0.0.tar", last modified: Sat Apr 15 08:59:20 2023, max compression
```

## Comparing `plone.behavior-1.4.0.tar` & `plone.behavior-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/
--rw-r--r--   0 maurits    (501) staff       (20)    22007 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      150 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    22007 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      843 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)      116 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone.behavior.egg-info/dependency_links.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1222 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1480 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1655 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/plone/behavior/
--rw-r--r--   0 maurits    (501) staff       (20)     3447 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/registration.py
--rw-r--r--   0 maurits    (501) staff       (20)     3551 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      207 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2029 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/annotation.py
--rw-r--r--   0 maurits    (501) staff       (20)    12427 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      518 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/vocab.py
--rw-r--r--   0 maurits    (501) staff       (20)    14447 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/directives.rst
--rw-r--r--   0 maurits    (501) staff       (20)      172 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      830 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/factory.py
--rw-r--r--   0 maurits    (501) staff       (20)     4021 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/annotation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6704 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/metaconfigure.py
--rw-r--r--   0 maurits    (501) staff       (20)      482 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/markers.py
--rw-r--r--   0 maurits    (501) staff       (20)      359 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3282 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/behavior/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/plone/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      104 2020-09-07 11:13:45.000000 plone.behavior-1.4.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)    12176 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4604 2020-09-07 11:13:44.000000 plone.behavior-1.4.0/CHANGES.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:59:20.342325 plone.behavior-2.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4781 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      150 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    17894 2023-04-15 08:59:20.342325 plone.behavior-2.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)    12176 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:59:20.340325 plone.behavior-2.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1222 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/docs/INSTALL.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1480 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:59:20.340325 plone.behavior-2.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:59:20.342325 plone.behavior-2.0.0/plone/behavior/
+-rw-r--r--   0 gil       (1000) gil       (1000)      148 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1956 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/annotation.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4018 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/annotation.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)    12427 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/behaviors.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      204 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)    14448 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/directives.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      797 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/factory.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3444 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      458 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/markers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      340 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/meta.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     6534 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/metaconfigure.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3420 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/registration.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2693 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/tests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      480 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/plone/behavior/vocab.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:59:20.341325 plone.behavior-2.0.0/plone.behavior.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    17894 2023-04-15 08:59:20.000000 plone.behavior-2.0.0/plone.behavior.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      802 2023-04-15 08:59:20.000000 plone.behavior-2.0.0/plone.behavior.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:59:20.000000 plone.behavior-2.0.0/plone.behavior.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:59:20.000000 plone.behavior-2.0.0/plone.behavior.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:59:20.000000 plone.behavior-2.0.0/plone.behavior.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      116 2023-04-15 08:59:20.000000 plone.behavior-2.0.0/plone.behavior.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:59:20.000000 plone.behavior-2.0.0/plone.behavior.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2782 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 08:59:20.342325 plone.behavior-2.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1696 2023-04-15 08:59:19.000000 plone.behavior-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.behavior-1.4.0/PKG-INFO` & `plone.behavior-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,560 +1,577 @@
 Metadata-Version: 2.1
 Name: plone.behavior
-Version: 1.4.0
+Version: 2.0.0
 Summary: Infrastructure for maintaining a registry of available behaviors
-Home-page: https://pypi.org/project/plone.behavior
+Home-page: https://github.com/plone/plone.behavior
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
+Maintainer: Plone Foundation - Release Team
+Maintainer-email: releaseteam@plone.org
 License: BSD
-Description: ==============
-        plone.behavior
-        ==============
-        
-        .. contents:: Table of Contents
-           :depth: 2
-        
-        
-        Overview
-        ========
-        
-        This package provides support for **behaviors**.
-        
-            A behavior is a re-usable aspect of an object that can be enabled or disabled without changing the component registry.
-        
-        A behavior is described by an interface, and has metadata such as a title and a description.
-        The behavior can be looked up by a given short name or by the dotted name of the interface.
-        With this unique name behaviors metadata can be looked up.
-        When the behavior is enabled for an object, you will be able to adapt the object to the interface.
-        In some cases, the interface can be used as a marker interface as well.
-        
-        As an example, let's say that your application needs to support object-level locking.
-        This can be modeled via an adapter, but you want to leave it until runtime to determine whether locking is enabled for a particular object.
-        You could then register locking as a behavior.
-        
-        **Requirements and Limitations:**
-        
-        * This package comes with support for registering behaviors and factories.
-        
-        * It does not implement the policy for determining what behaviors are enabled on a particular object at a particular time.
-          That decision is deferred to an ``IBehaviorAssignable`` adapter, which must be implemented (``plone.dexterity`` implements this).
-        
-        * Like the ``IBehaviorAssignable`` plumbing, marker interface support needs to be enabled on a per-application basis.
-          This package also does not directly support the adding of marker interfaces to instances.
-          To do that, you can either use an event handler to mark an object when it is created, or a dynamic __providedBy__ descriptor that does the lookup on the fly (but you probably want some caching).
-          A sample event handler is provided with this package, but is not registered by default
-        
-        * The intention is that behavior assignment is generic across an application, used for multiple, optional behaviors.
-          It probably doesn't make much sense to use ``plone.behavior`` for a single type of object.
-          The means to keep track of which behaviors are enabled for what types of objects will be application specific.
-        
-        Usage
-        =====
-        
-        Explained
-        ---------
-        
-        A behavior is written much like an adapter, except that you don't specify the type of context being adapted directly.
-        For example::
-        
-            from zope.interface import Interface
-            from zope.interface import implementer
-        
-            class ILockingSupport(Interface):
-               """Support locking
-               """
-        
-               def lock():
-                   """Lock an object
-                   """
-        
-               def unlock():
-                   """Unlock an object
-                   """
-        
-            @implementer(ILockingSupport)
-            class LockingSupport(object):
-        
-                def __init__(self, context):
-                    self.context = context
-        
-                def lock(self):
-                    # do something
-        
-                def unlock(self):
-                    # do something
-        
-        This interface (which describes the type of behavior) and class (which describes the implementation of the behavior) then needs to be registered.
-        
-        The simplest way to do that is to load the ``meta.zcml`` file from this package and use ZCML::
-        
-            <configure
-              xmlns="http://namespaces.zope.org/zope"
-              xmlns:plone="http://namespaces.plone.org/plone"
-              i18n_domain="my.package">
-        
-              <include package="plone.behavior" file="meta.zcml" />
-        
-              <plone:behavior
-                  name="locking_support"
-                  title="Locking support"
-                  description="Optional object-level locking"
-                  provides=".interfaces.ILockingSupport"
-                  factory=".locking.LockingSupport"
-              />
-        
-            </configure>
-        
-        After this is done you can adapt a context to ``ILockingSupport`` as normal::
-        
-            locking = ILockingSupport(context, None)
-        
-            if locking is not None:
-                locking.lock()
-        
-        The ``name`` can be used for lookup instead of the full dotted name of the interface::
-        
-            from plone.behavior.interfaces import IBehavior
-            from zope.component import getUtility
-        
-            registration = getUtility(IBehavior, name='locking_support')
-        
-        We also have a helper function to achieve this::
-        
-            from plone.behavior.registration import lookup_behavior_registration
-        
-            registration = lookup_behavior_registration(name='locking_support')
-        
-        
-        You'll get an instance of ``LockingSupport`` if context can be adapted to ``IBehaviorAssignable`` (which, recall, is application specific),
-        and if the implementation of ``IBehaviorAssignable`` says that this context supports this particular behavior.
-        
-        It is also possible to let the provided interface act as a marker interface that is to be provided directly by the instance.
-        To achieve this, omit the ``factory`` argument.
-        This is useful if you need to register other adapters for instances providing a particular behavior.
-        
-        ZCML Reference
-        --------------
-        
-        The ``plone:behavior`` directive uses the namespace ``xmlns:plone="http://namespaces.plone.org/plone"``.
-        In order to enable it loading of its ``meta.zcml`` is needed, use::
-        
-            <include package="plone.behavior" file="meta.zcml" />
-        
-        The directive supports the attributes:
-        
-        ``title``
-            A user friendly title for this behavior (required).
-        
-        ``description``
-            A longer description for this behavior (optional).
-        
-        ``provides``
-            An interface to which the behavior can be adapted.
-            This is what the conditional adapter factory will be registered as providing (required).
-        
-        ``name``
-            Convenience lookup name for this behavior (optional).
-            The behavior will be always registered under the dotted name of ``provides`` attribute.
-            This are usally long names. ``name`` is a short name for this.
-            If ``name`` is given the behavior is registered additional under it.
-            Anyway using short namespaces in ``name`` is recommended.
-        
-        ``name_only``
-            If set to ``yes`` or ``true`` the behavior is registered only under the given name,
-            but not under the dotted path of the ``provides`` interface.
-            This makes ``name`` mandatory.
-        
-        ``marker``
-            A marker interface to be applied by the behavior.
-            If ``factory`` is not given, then this is optional and defaults to the value of ``provides``.
-            If factory is given ``marker`` is required and should be different from ``provides`` - even if its not enforced.
-        
-        ``factory``
-            The factory for this behavior (optional).
-            If no factory is given, the behavior context is assumed to provide the interface given by ``provides`` itself.
-        
-            If factory provides ``plone.behavior.interfaces.ISchemaAwareFactory`` the factory is assumed to be a callable.
-            ``ISchemaAwareFactory`` is an interface for factories that should be initialised with a schema.
-            It is called with the value given in ``provides`` as the only argument.
-            The value returned is then used as the factory, another callable that can create appropriate behavior factories on demand.
-        
-        ``for``
-            The type of object to register the conditional adapter factory for (optional).
-            Must be omitted is no ``factory`` is given.
-        
-            The default is either to auto-detect what the factory adapts (i.e. using the ``@adapter`` decorator) or to fall back to ``zope.interface.Interface`` (also written as ``*`` in ZCML).
-        
-            Must be one element (no multiadapters, applies also for auto-detection).
-        
-        ``former_dotted_names``
-            In case a behavior is modified so that its dotted name changes, this field can be used to register the old name(s). Therefore, it is possible to retrieve the name(s) under which a behavior was formerly registered under.
-        
-            If a call to ``lookup_behavior_registration`` does not find a behavior under the given name, it will look at the former dotted names to try and find the behavior.
-        
-        
-        ZCML Examples
-        -------------
-        
-        Example usage, given
-        
-        - some ``context`` (some arbitary object) which is ``IBehaviorAssignable``,
-        - an ``IMyBehavior`` interface intented to be used as ``provides``,
-        - an ``IMyMarker`` interface intented to be used as ``marker``,
-        - a ``MyFactory`` class implementing ``IMyBehavior`` ,
-        - a ``MySchemaAwareFactory`` class implementing ``IMyBehavior`` and ``plone.behavior.interfaces.ISchemaAwareFactory``,
-        - an ``IMyType`` intented to be used as ``for``.
-        - some ``typed_context`` (some arbitary object) which is ``IBehaviorAssignable`` and provides ``IMyType``,
-        - an ``MyTypedFactory`` class implementing ``IMyBehavior`` and adapting ``IMyType``,
-        
-        ``title`` and ``description`` is trivial, so we dont cover it here in the explanantion.
-        We dont cover ``name`` too, because it's not having any effect in this usage.
-        To simplify it, we assume ``context`` ``IBehaviorAssignable`` always supports the behavior.
-        Also for simplifications sake we assume some magic applies the marker interface to ``context``
-        I.e. both is done by ``plone.dexterity``.
-        
-        **Example 1** - only ``provides`` given::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-            />
-        
-        - ``marker`` defaults to ``provides``,
-        - with ``behavior = IMyBehavior(context)`` the ``context`` itself is returned,
-        - ``context`` provides ``IBehavior``,
-        
-        **Example 2** - also ``factory`` is given, so ``marker`` is required:
-        
-        .. warning::
-           Using the same Interface as marker and behavior works, but is not recommended and will be deprecated in future.
-           It is semantically wrong!
-           
-           Go for Example 3 instead!
-        
-        ::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyBehavior"
-                factory="MyFactory"
-            />
-        
-        - ``marker`` is the same as ``provides``,
-        - with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyBehavior``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        - having ``context`` and ``MyFactory`` providing both the same interface is ugly and not recommended!
-        
-        **Example 3** - in example 2 both, factory and context are providing the ``IMyBehavior``.
-        This may lead to confusion, so now better with a ``marker``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MyFactory"
-            />
-        
-        - with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        
-        **Example 4** - like example 3 but with an ``MySchemaAwareFactory``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MySchemaAwareFactory"
-            />
-        
-        - with ``behavior = IMyBehavior(context)`` some factory instance is returned as a result from calling a ``MySchemaAwareFactory`` instance with ``IMyBehavior`` as argument,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        
-        **Example 5** - the behavior should be restricted to the ``typed_context``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MyFactory"
-                for="IMyType"
-            />
-        
-        - with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
-        - with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` provides ``IMyBehavior``,
-        
-        **Example 6** - the behavior should be restricted to the ``typed_context`` by auto-detection.
-        The ``MyTypedFactory`` class adapts ``IMyType`` using a class decorator ``@adapter(IMyType)``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MyTypedFactory"
-            />
-        
-        - with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
-        - with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        
-        
-        Further Reading
-        ---------------
-        
-        For more details please read the doctests in the source code: ``behavior.rst``, ``directives.rst`` and ``annotation.rst``.
-        
-        
-        Source Code
-        ===========
-        
-        Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
-        
-        Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.behavior>`_.
-        
-        Changelog
-        =========
-        
-        .. You should *NOT* be adding new change log entries to this file.
-           You should create a file in the news directory instead.
-           For helpful instructions, please see:
-           https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
-        
-        .. towncrier release notes start
-        
-        1.4.0 (2020-09-07)
-        ------------------
-        
-        New features:
-        
-        
-        - Drop Plone 4.3 support.
-          [maurits] (#3130)
-        
-        
-        Bug fixes:
-        
-        
-        - Fixed deprecation warning for ComponentLookupError.
-          [maurits] (#3130)
-        
-        
-        1.3.2 (2020-04-20)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Minor packaging updates. (#1)
-        
-        
-        1.3.1 (2020-03-08)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Improved documentation.  [jensens] (#0)
-        
-        
-        1.3.0 (2019-02-13)
-        ------------------
-        
-        New features:
-        
-        
-        - New option ``former_dotted_names`` that allows to register the former name
-          under which a behavior used to be registerd. This can be useful to ensure a
-          smooth transition in case a behavior's dotted name is changed. [pysailor]
-          (#18)
-        
-        
-        1.2.1 (2018-01-17)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fixed import of dotted path in example.  [fulv]
-        
-        
-        1.2.0 (2017-03-23)
-        ------------------
-        
-        New features:
-        
-        - For zcml registration:
-          If both, no ``for`` and no ``@adapter`` is given,
-          fall first back to ``marker`` if given (new),
-          else to ``Interface`` (as it was already before).
-          [jensens]
-        
-        Bug fixes:
-        
-        - Cleanup: Make Jenkins CI code analysis silent by fixing the issues.
-          [jensens]
-        
-        
-        1.1.4 (2016-12-06)
-        ------------------
-        
-        Bug fixes:
-        
-        - Add already introduced attribute ``name`` to interface IBehavior.
-          This was missing.
-          Also modernized other IBehavior interface descriptions a bit.
-          [jensens]
-        
-        
-        1.1.3 (2016-11-09)
-        ------------------
-        
-        New features:
-        
-        - Support Python 3. [davisagli]
-        
-        
-        1.1.2 (2016-08-11)
-        ------------------
-        
-        New:
-        
-        - New option to register a behavior only by it's short name and not by it's dotted name.
-          This enables more advanced behavior subclassing capabilities.
-          [jensens]
-        
-        
-        1.1.1 (2016-02-25)
-        ------------------
-        
-        Fixes:
-        
-        - Make doctest comparison more robust against zope.component __repr__ changes.
-          [thet]
-        
-        
-        1.1 (2015-07-18)
-        ----------------
-        
-        - Corrected typo in warning.
-          [jensens]
-        
-        - Add name to behavior directive. This name can be used to lookup behavior
-          registrations by new plone.behaviors.registration.
-          lookup_behavior_registration function.
-          [rnixx]
-        
-        - Added more documentation, simplified code in directive, added a warning if
-          ``for`` is given w/o ``factory``.
-          [jensens]
-        
-        
-        1.0.3 (2015-04-29)
-        ------------------
-        
-        - Code modernization: utf-header, pep8, rst-files, adapter/implementer
-          decorators, ...
-          [jensens]
-        
-        
-        1.0.2 (2013-01-17)
-        ------------------
-        
-        - Remove dependence of tests on zope.app.testing.
-          [davisagli]
-        
-        
-        1.0.1 - 2011-05-20
-        ------------------
-        
-        - Relicense under BSD license.
-          See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
-          [davisagli]
-        
-        
-        1.0 - 2011-04-30
-        ----------------
-        
-        - Use stdlib doctest instead of the deprecated one in zope.testing.
-          [davisagli]
-        
-        - 'plone:behavior' zcml directive use now MessageID for title and description.
-          [sylvainb]
-        
-        
-        1.0b6 - 2009-11-17
-        ------------------
-        
-        - Fix tests for Zope 2.12
-          [optilude]
-        
-        
-        1.0b5 - 2009-07-12
-        ------------------
-        
-        - Changed API methods and arguments to mixedCase to be more consistent with
-          the rest of Zope. This is a non-backwards-compatible change. Our profuse
-          apologies, but it's now or never. :-/
-        
-          If you find that you get import errors or unknown keyword arguments in your
-          code, please change names from foo_bar too fooBar, e.g.
-          enumerate_behaviors() becomes enumerateBehaviors().
-          [optilude]
-        
-        
-        1.0b4 - 2009-06-07
-        ------------------
-        
-        - Allow a marker-interface-only behavior to be set by using the 'provides'
-          attribute (previously 'interface') in the <plone:behavior /> directive
-          without a 'factory' attribute. The 'marker' attribute (previously known as
-          'subtype') is now only required if there is a marker used in addition to
-          a behavior adapter with a separate interface ('provides') and factory.
-          [optilude]
-        
-        - Rename the 'interface' attribute of <plone:behavior /> to 'provides' to
-          be more consistent with the <adapter /> directive. This is a backwards
-          incompatible change!
-          [optilude]
-        
-        - Rename the 'subtype' attribute of <plone:behavior /> to 'marker' to
-          be more explicit about its purpose. This is a backwards
-          incompatible change!
-          [optilude]
-        
-        
-        1.0b3 - 2009-04-17
-        ------------------
-        
-        - Allow behaviors with no factory.
-          [alecm]
-        
-        - Provide a vocabulary of available behaviors.
-          [davisagli]
-        
-        
-        1.0b1 - 2008-04-27
-        ------------------
-        
-        - Initial release
-        
 Keywords: Plone behavior registry
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.8
 Provides-Extra: test
+
+==============
+plone.behavior
+==============
+
+.. contents:: Table of Contents
+   :depth: 2
+
+
+Overview
+========
+
+This package provides support for **behaviors**.
+
+    A behavior is a re-usable aspect of an object that can be enabled or disabled without changing the component registry.
+
+A behavior is described by an interface, and has metadata such as a title and a description.
+The behavior can be looked up by a given short name or by the dotted name of the interface.
+With this unique name behaviors metadata can be looked up.
+When the behavior is enabled for an object, you will be able to adapt the object to the interface.
+In some cases, the interface can be used as a marker interface as well.
+
+As an example, let's say that your application needs to support object-level locking.
+This can be modeled via an adapter, but you want to leave it until runtime to determine whether locking is enabled for a particular object.
+You could then register locking as a behavior.
+
+**Requirements and Limitations:**
+
+* This package comes with support for registering behaviors and factories.
+
+* It does not implement the policy for determining what behaviors are enabled on a particular object at a particular time.
+  That decision is deferred to an ``IBehaviorAssignable`` adapter, which must be implemented (``plone.dexterity`` implements this).
+
+* Like the ``IBehaviorAssignable`` plumbing, marker interface support needs to be enabled on a per-application basis.
+  This package also does not directly support the adding of marker interfaces to instances.
+  To do that, you can either use an event handler to mark an object when it is created, or a dynamic __providedBy__ descriptor that does the lookup on the fly (but you probably want some caching).
+  A sample event handler is provided with this package, but is not registered by default
+
+* The intention is that behavior assignment is generic across an application, used for multiple, optional behaviors.
+  It probably doesn't make much sense to use ``plone.behavior`` for a single type of object.
+  The means to keep track of which behaviors are enabled for what types of objects will be application specific.
+
+Usage
+=====
+
+Explained
+---------
+
+A behavior is written much like an adapter, except that you don't specify the type of context being adapted directly.
+For example::
+
+    from zope.interface import Interface
+    from zope.interface import implementer
+
+    class ILockingSupport(Interface):
+       """Support locking
+       """
+
+       def lock():
+           """Lock an object
+           """
+
+       def unlock():
+           """Unlock an object
+           """
+
+    @implementer(ILockingSupport)
+    class LockingSupport(object):
+
+        def __init__(self, context):
+            self.context = context
+
+        def lock(self):
+            # do something
+
+        def unlock(self):
+            # do something
+
+This interface (which describes the type of behavior) and class (which describes the implementation of the behavior) then needs to be registered.
+
+The simplest way to do that is to load the ``meta.zcml`` file from this package and use ZCML::
+
+    <configure
+      xmlns="http://namespaces.zope.org/zope"
+      xmlns:plone="http://namespaces.plone.org/plone"
+      i18n_domain="my.package">
+
+      <include package="plone.behavior" file="meta.zcml" />
+
+      <plone:behavior
+          name="locking_support"
+          title="Locking support"
+          description="Optional object-level locking"
+          provides=".interfaces.ILockingSupport"
+          factory=".locking.LockingSupport"
+      />
+
+    </configure>
+
+After this is done you can adapt a context to ``ILockingSupport`` as normal::
+
+    locking = ILockingSupport(context, None)
+
+    if locking is not None:
+        locking.lock()
+
+The ``name`` can be used for lookup instead of the full dotted name of the interface::
+
+    from plone.behavior.interfaces import IBehavior
+    from zope.component import getUtility
+
+    registration = getUtility(IBehavior, name='locking_support')
+
+We also have a helper function to achieve this::
+
+    from plone.behavior.registration import lookup_behavior_registration
+
+    registration = lookup_behavior_registration(name='locking_support')
+
+
+You'll get an instance of ``LockingSupport`` if context can be adapted to ``IBehaviorAssignable`` (which, recall, is application specific),
+and if the implementation of ``IBehaviorAssignable`` says that this context supports this particular behavior.
+
+It is also possible to let the provided interface act as a marker interface that is to be provided directly by the instance.
+To achieve this, omit the ``factory`` argument.
+This is useful if you need to register other adapters for instances providing a particular behavior.
+
+ZCML Reference
+--------------
+
+The ``plone:behavior`` directive uses the namespace ``xmlns:plone="http://namespaces.plone.org/plone"``.
+In order to enable it loading of its ``meta.zcml`` is needed, use::
+
+    <include package="plone.behavior" file="meta.zcml" />
+
+The directive supports the attributes:
+
+``title``
+    A user friendly title for this behavior (required).
+
+``description``
+    A longer description for this behavior (optional).
+
+``provides``
+    An interface to which the behavior can be adapted.
+    This is what the conditional adapter factory will be registered as providing (required).
+
+``name``
+    Convenience lookup name for this behavior (optional).
+    The behavior will be always registered under the dotted name of ``provides`` attribute.
+    This are usually long names. ``name`` is a short name for this.
+    If ``name`` is given the behavior is registered additional under it.
+    Anyway using short namespaces in ``name`` is recommended.
+
+``name_only``
+    If set to ``yes`` or ``true`` the behavior is registered only under the given name,
+    but not under the dotted path of the ``provides`` interface.
+    This makes ``name`` mandatory.
+
+``marker``
+    A marker interface to be applied by the behavior.
+    If ``factory`` is not given, then this is optional and defaults to the value of ``provides``.
+    If factory is given ``marker`` is required and should be different from ``provides`` - even if its not enforced.
+
+``factory``
+    The factory for this behavior (optional).
+    If no factory is given, the behavior context is assumed to provide the interface given by ``provides`` itself.
+
+    If factory provides ``plone.behavior.interfaces.ISchemaAwareFactory`` the factory is assumed to be a callable.
+    ``ISchemaAwareFactory`` is an interface for factories that should be initialised with a schema.
+    It is called with the value given in ``provides`` as the only argument.
+    The value returned is then used as the factory, another callable that can create appropriate behavior factories on demand.
+
+``for``
+    The type of object to register the conditional adapter factory for (optional).
+    Must be omitted is no ``factory`` is given.
+
+    The default is either to auto-detect what the factory adapts (i.e. using the ``@adapter`` decorator) or to fall back to ``zope.interface.Interface`` (also written as ``*`` in ZCML).
+
+    Must be one element (no multiadapters, applies also for auto-detection).
+
+``former_dotted_names``
+    In case a behavior is modified so that its dotted name changes, this field can be used to register the old name(s). Therefore, it is possible to retrieve the name(s) under which a behavior was formerly registered under.
+
+    If a call to ``lookup_behavior_registration`` does not find a behavior under the given name, it will look at the former dotted names to try and find the behavior.
+
+
+ZCML Examples
+-------------
+
+Example usage, given
+
+- some ``context`` (some arbitrary object) which is ``IBehaviorAssignable``,
+- an ``IMyBehavior`` interface intended to be used as ``provides``,
+- an ``IMyMarker`` interface intended to be used as ``marker``,
+- a ``MyFactory`` class implementing ``IMyBehavior`` ,
+- a ``MySchemaAwareFactory`` class implementing ``IMyBehavior`` and ``plone.behavior.interfaces.ISchemaAwareFactory``,
+- an ``IMyType`` intended to be used as ``for``.
+- some ``typed_context`` (some arbitrary object) which is ``IBehaviorAssignable`` and provides ``IMyType``,
+- an ``MyTypedFactory`` class implementing ``IMyBehavior`` and adapting ``IMyType``,
+
+``title`` and ``description`` is trivial, so we dont cover it here in the explanantion.
+We dont cover ``name`` too, because it's not having any effect in this usage.
+To simplify it, we assume ``context`` ``IBehaviorAssignable`` always supports the behavior.
+Also for simplifications sake we assume some magic applies the marker interface to ``context``
+I.e. both is done by ``plone.dexterity``.
+
+**Example 1** - only ``provides`` given::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+    />
+
+- ``marker`` defaults to ``provides``,
+- with ``behavior = IMyBehavior(context)`` the ``context`` itself is returned,
+- ``context`` provides ``IBehavior``,
+
+**Example 2** - also ``factory`` is given, so ``marker`` is required:
+
+.. warning::
+   Using the same Interface as marker and behavior works, but is not recommended and will be deprecated in future.
+   It is semantically wrong!
+
+   Go for Example 3 instead!
+
+::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyBehavior"
+        factory="MyFactory"
+    />
+
+- ``marker`` is the same as ``provides``,
+- with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyBehavior``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+- having ``context`` and ``MyFactory`` providing both the same interface is ugly and not recommended!
+
+**Example 3** - in example 2 both, factory and context are providing the ``IMyBehavior``.
+This may lead to confusion, so now better with a ``marker``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MyFactory"
+    />
+
+- with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+
+**Example 4** - like example 3 but with an ``MySchemaAwareFactory``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MySchemaAwareFactory"
+    />
+
+- with ``behavior = IMyBehavior(context)`` some factory instance is returned as a result from calling a ``MySchemaAwareFactory`` instance with ``IMyBehavior`` as argument,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+
+**Example 5** - the behavior should be restricted to the ``typed_context``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MyFactory"
+        for="IMyType"
+    />
+
+- with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
+- with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` provides ``IMyBehavior``,
+
+**Example 6** - the behavior should be restricted to the ``typed_context`` by auto-detection.
+The ``MyTypedFactory`` class adapts ``IMyType`` using a class decorator ``@adapter(IMyType)``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MyTypedFactory"
+    />
+
+- with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
+- with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+
+
+Further Reading
+---------------
+
+For more details please read the doctests in the source code: ``behavior.rst``, ``directives.rst`` and ``annotation.rst``.
+
+
+Source Code
+===========
+
+Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
+
+Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.behavior>`_.
+
+Changelog
+=========
+
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.0.0 (2023-04-15)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a9dd65cc)
+
+
+1.4.0 (2020-09-07)
+------------------
+
+New features:
+
+
+- Drop Plone 4.3 support.
+  [maurits] (#3130)
+
+
+Bug fixes:
+
+
+- Fixed deprecation warning for ComponentLookupError.
+  [maurits] (#3130)
+
+
+1.3.2 (2020-04-20)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+1.3.1 (2020-03-08)
+------------------
+
+Bug fixes:
+
+
+- Improved documentation.  [jensens] (#0)
+
+
+1.3.0 (2019-02-13)
+------------------
+
+New features:
+
+
+- New option ``former_dotted_names`` that allows to register the former name
+  under which a behavior used to be registered. This can be useful to ensure a
+  smooth transition in case a behavior's dotted name is changed. [pysailor]
+  (#18)
+
+
+1.2.1 (2018-01-17)
+------------------
+
+Bug fixes:
+
+- Fixed import of dotted path in example.  [fulv]
+
+
+1.2.0 (2017-03-23)
+------------------
+
+New features:
+
+- For zcml registration:
+  If both, no ``for`` and no ``@adapter`` is given,
+  fall first back to ``marker`` if given (new),
+  else to ``Interface`` (as it was already before).
+  [jensens]
+
+Bug fixes:
+
+- Cleanup: Make Jenkins CI code analysis silent by fixing the issues.
+  [jensens]
+
+
+1.1.4 (2016-12-06)
+------------------
+
+Bug fixes:
+
+- Add already introduced attribute ``name`` to interface IBehavior.
+  This was missing.
+  Also modernized other IBehavior interface descriptions a bit.
+  [jensens]
+
+
+1.1.3 (2016-11-09)
+------------------
+
+New features:
+
+- Support Python 3. [davisagli]
+
+
+1.1.2 (2016-08-11)
+------------------
+
+New:
+
+- New option to register a behavior only by it's short name and not by it's dotted name.
+  This enables more advanced behavior subclassing capabilities.
+  [jensens]
+
+
+1.1.1 (2016-02-25)
+------------------
+
+Fixes:
+
+- Make doctest comparison more robust against zope.component __repr__ changes.
+  [thet]
+
+
+1.1 (2015-07-18)
+----------------
+
+- Corrected typo in warning.
+  [jensens]
+
+- Add name to behavior directive. This name can be used to lookup behavior
+  registrations by new plone.behaviors.registration.
+  lookup_behavior_registration function.
+  [rnixx]
+
+- Added more documentation, simplified code in directive, added a warning if
+  ``for`` is given w/o ``factory``.
+  [jensens]
+
+
+1.0.3 (2015-04-29)
+------------------
+
+- Code modernization: utf-header, pep8, rst-files, adapter/implementer
+  decorators, ...
+  [jensens]
+
+
+1.0.2 (2013-01-17)
+------------------
+
+- Remove dependence of tests on zope.app.testing.
+  [davisagli]
+
+
+1.0.1 - 2011-05-20
+------------------
+
+- Relicense under BSD license.
+  See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
+  [davisagli]
+
+
+1.0 - 2011-04-30
+----------------
+
+- Use stdlib doctest instead of the deprecated one in zope.testing.
+  [davisagli]
+
+- 'plone:behavior' zcml directive use now MessageID for title and description.
+  [sylvainb]
+
+
+1.0b6 - 2009-11-17
+------------------
+
+- Fix tests for Zope 2.12
+  [optilude]
+
+
+1.0b5 - 2009-07-12
+------------------
+
+- Changed API methods and arguments to mixedCase to be more consistent with
+  the rest of Zope. This is a non-backwards-compatible change. Our profuse
+  apologies, but it's now or never. :-/
+
+  If you find that you get import errors or unknown keyword arguments in your
+  code, please change names from foo_bar too fooBar, e.g.
+  enumerate_behaviors() becomes enumerateBehaviors().
+  [optilude]
+
+
+1.0b4 - 2009-06-07
+------------------
+
+- Allow a marker-interface-only behavior to be set by using the 'provides'
+  attribute (previously 'interface') in the <plone:behavior /> directive
+  without a 'factory' attribute. The 'marker' attribute (previously known as
+  'subtype') is now only required if there is a marker used in addition to
+  a behavior adapter with a separate interface ('provides') and factory.
+  [optilude]
+
+- Rename the 'interface' attribute of <plone:behavior /> to 'provides' to
+  be more consistent with the <adapter /> directive. This is a backwards
+  incompatible change!
+  [optilude]
+
+- Rename the 'subtype' attribute of <plone:behavior /> to 'marker' to
+  be more explicit about its purpose. This is a backwards
+  incompatible change!
+  [optilude]
+
+
+1.0b3 - 2009-04-17
+------------------
+
+- Allow behaviors with no factory.
+  [alecm]
+
+- Provide a vocabulary of available behaviors.
+  [davisagli]
+
+
+1.0b1 - 2008-04-27
+------------------
+
+- Initial release
```

### Comparing `plone.behavior-1.4.0/plone.behavior.egg-info/PKG-INFO` & `plone.behavior-2.0.0/plone.behavior.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,560 +1,577 @@
 Metadata-Version: 2.1
 Name: plone.behavior
-Version: 1.4.0
+Version: 2.0.0
 Summary: Infrastructure for maintaining a registry of available behaviors
-Home-page: https://pypi.org/project/plone.behavior
+Home-page: https://github.com/plone/plone.behavior
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
+Maintainer: Plone Foundation - Release Team
+Maintainer-email: releaseteam@plone.org
 License: BSD
-Description: ==============
-        plone.behavior
-        ==============
-        
-        .. contents:: Table of Contents
-           :depth: 2
-        
-        
-        Overview
-        ========
-        
-        This package provides support for **behaviors**.
-        
-            A behavior is a re-usable aspect of an object that can be enabled or disabled without changing the component registry.
-        
-        A behavior is described by an interface, and has metadata such as a title and a description.
-        The behavior can be looked up by a given short name or by the dotted name of the interface.
-        With this unique name behaviors metadata can be looked up.
-        When the behavior is enabled for an object, you will be able to adapt the object to the interface.
-        In some cases, the interface can be used as a marker interface as well.
-        
-        As an example, let's say that your application needs to support object-level locking.
-        This can be modeled via an adapter, but you want to leave it until runtime to determine whether locking is enabled for a particular object.
-        You could then register locking as a behavior.
-        
-        **Requirements and Limitations:**
-        
-        * This package comes with support for registering behaviors and factories.
-        
-        * It does not implement the policy for determining what behaviors are enabled on a particular object at a particular time.
-          That decision is deferred to an ``IBehaviorAssignable`` adapter, which must be implemented (``plone.dexterity`` implements this).
-        
-        * Like the ``IBehaviorAssignable`` plumbing, marker interface support needs to be enabled on a per-application basis.
-          This package also does not directly support the adding of marker interfaces to instances.
-          To do that, you can either use an event handler to mark an object when it is created, or a dynamic __providedBy__ descriptor that does the lookup on the fly (but you probably want some caching).
-          A sample event handler is provided with this package, but is not registered by default
-        
-        * The intention is that behavior assignment is generic across an application, used for multiple, optional behaviors.
-          It probably doesn't make much sense to use ``plone.behavior`` for a single type of object.
-          The means to keep track of which behaviors are enabled for what types of objects will be application specific.
-        
-        Usage
-        =====
-        
-        Explained
-        ---------
-        
-        A behavior is written much like an adapter, except that you don't specify the type of context being adapted directly.
-        For example::
-        
-            from zope.interface import Interface
-            from zope.interface import implementer
-        
-            class ILockingSupport(Interface):
-               """Support locking
-               """
-        
-               def lock():
-                   """Lock an object
-                   """
-        
-               def unlock():
-                   """Unlock an object
-                   """
-        
-            @implementer(ILockingSupport)
-            class LockingSupport(object):
-        
-                def __init__(self, context):
-                    self.context = context
-        
-                def lock(self):
-                    # do something
-        
-                def unlock(self):
-                    # do something
-        
-        This interface (which describes the type of behavior) and class (which describes the implementation of the behavior) then needs to be registered.
-        
-        The simplest way to do that is to load the ``meta.zcml`` file from this package and use ZCML::
-        
-            <configure
-              xmlns="http://namespaces.zope.org/zope"
-              xmlns:plone="http://namespaces.plone.org/plone"
-              i18n_domain="my.package">
-        
-              <include package="plone.behavior" file="meta.zcml" />
-        
-              <plone:behavior
-                  name="locking_support"
-                  title="Locking support"
-                  description="Optional object-level locking"
-                  provides=".interfaces.ILockingSupport"
-                  factory=".locking.LockingSupport"
-              />
-        
-            </configure>
-        
-        After this is done you can adapt a context to ``ILockingSupport`` as normal::
-        
-            locking = ILockingSupport(context, None)
-        
-            if locking is not None:
-                locking.lock()
-        
-        The ``name`` can be used for lookup instead of the full dotted name of the interface::
-        
-            from plone.behavior.interfaces import IBehavior
-            from zope.component import getUtility
-        
-            registration = getUtility(IBehavior, name='locking_support')
-        
-        We also have a helper function to achieve this::
-        
-            from plone.behavior.registration import lookup_behavior_registration
-        
-            registration = lookup_behavior_registration(name='locking_support')
-        
-        
-        You'll get an instance of ``LockingSupport`` if context can be adapted to ``IBehaviorAssignable`` (which, recall, is application specific),
-        and if the implementation of ``IBehaviorAssignable`` says that this context supports this particular behavior.
-        
-        It is also possible to let the provided interface act as a marker interface that is to be provided directly by the instance.
-        To achieve this, omit the ``factory`` argument.
-        This is useful if you need to register other adapters for instances providing a particular behavior.
-        
-        ZCML Reference
-        --------------
-        
-        The ``plone:behavior`` directive uses the namespace ``xmlns:plone="http://namespaces.plone.org/plone"``.
-        In order to enable it loading of its ``meta.zcml`` is needed, use::
-        
-            <include package="plone.behavior" file="meta.zcml" />
-        
-        The directive supports the attributes:
-        
-        ``title``
-            A user friendly title for this behavior (required).
-        
-        ``description``
-            A longer description for this behavior (optional).
-        
-        ``provides``
-            An interface to which the behavior can be adapted.
-            This is what the conditional adapter factory will be registered as providing (required).
-        
-        ``name``
-            Convenience lookup name for this behavior (optional).
-            The behavior will be always registered under the dotted name of ``provides`` attribute.
-            This are usally long names. ``name`` is a short name for this.
-            If ``name`` is given the behavior is registered additional under it.
-            Anyway using short namespaces in ``name`` is recommended.
-        
-        ``name_only``
-            If set to ``yes`` or ``true`` the behavior is registered only under the given name,
-            but not under the dotted path of the ``provides`` interface.
-            This makes ``name`` mandatory.
-        
-        ``marker``
-            A marker interface to be applied by the behavior.
-            If ``factory`` is not given, then this is optional and defaults to the value of ``provides``.
-            If factory is given ``marker`` is required and should be different from ``provides`` - even if its not enforced.
-        
-        ``factory``
-            The factory for this behavior (optional).
-            If no factory is given, the behavior context is assumed to provide the interface given by ``provides`` itself.
-        
-            If factory provides ``plone.behavior.interfaces.ISchemaAwareFactory`` the factory is assumed to be a callable.
-            ``ISchemaAwareFactory`` is an interface for factories that should be initialised with a schema.
-            It is called with the value given in ``provides`` as the only argument.
-            The value returned is then used as the factory, another callable that can create appropriate behavior factories on demand.
-        
-        ``for``
-            The type of object to register the conditional adapter factory for (optional).
-            Must be omitted is no ``factory`` is given.
-        
-            The default is either to auto-detect what the factory adapts (i.e. using the ``@adapter`` decorator) or to fall back to ``zope.interface.Interface`` (also written as ``*`` in ZCML).
-        
-            Must be one element (no multiadapters, applies also for auto-detection).
-        
-        ``former_dotted_names``
-            In case a behavior is modified so that its dotted name changes, this field can be used to register the old name(s). Therefore, it is possible to retrieve the name(s) under which a behavior was formerly registered under.
-        
-            If a call to ``lookup_behavior_registration`` does not find a behavior under the given name, it will look at the former dotted names to try and find the behavior.
-        
-        
-        ZCML Examples
-        -------------
-        
-        Example usage, given
-        
-        - some ``context`` (some arbitary object) which is ``IBehaviorAssignable``,
-        - an ``IMyBehavior`` interface intented to be used as ``provides``,
-        - an ``IMyMarker`` interface intented to be used as ``marker``,
-        - a ``MyFactory`` class implementing ``IMyBehavior`` ,
-        - a ``MySchemaAwareFactory`` class implementing ``IMyBehavior`` and ``plone.behavior.interfaces.ISchemaAwareFactory``,
-        - an ``IMyType`` intented to be used as ``for``.
-        - some ``typed_context`` (some arbitary object) which is ``IBehaviorAssignable`` and provides ``IMyType``,
-        - an ``MyTypedFactory`` class implementing ``IMyBehavior`` and adapting ``IMyType``,
-        
-        ``title`` and ``description`` is trivial, so we dont cover it here in the explanantion.
-        We dont cover ``name`` too, because it's not having any effect in this usage.
-        To simplify it, we assume ``context`` ``IBehaviorAssignable`` always supports the behavior.
-        Also for simplifications sake we assume some magic applies the marker interface to ``context``
-        I.e. both is done by ``plone.dexterity``.
-        
-        **Example 1** - only ``provides`` given::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-            />
-        
-        - ``marker`` defaults to ``provides``,
-        - with ``behavior = IMyBehavior(context)`` the ``context`` itself is returned,
-        - ``context`` provides ``IBehavior``,
-        
-        **Example 2** - also ``factory`` is given, so ``marker`` is required:
-        
-        .. warning::
-           Using the same Interface as marker and behavior works, but is not recommended and will be deprecated in future.
-           It is semantically wrong!
-           
-           Go for Example 3 instead!
-        
-        ::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyBehavior"
-                factory="MyFactory"
-            />
-        
-        - ``marker`` is the same as ``provides``,
-        - with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyBehavior``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        - having ``context`` and ``MyFactory`` providing both the same interface is ugly and not recommended!
-        
-        **Example 3** - in example 2 both, factory and context are providing the ``IMyBehavior``.
-        This may lead to confusion, so now better with a ``marker``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MyFactory"
-            />
-        
-        - with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        
-        **Example 4** - like example 3 but with an ``MySchemaAwareFactory``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MySchemaAwareFactory"
-            />
-        
-        - with ``behavior = IMyBehavior(context)`` some factory instance is returned as a result from calling a ``MySchemaAwareFactory`` instance with ``IMyBehavior`` as argument,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        
-        **Example 5** - the behavior should be restricted to the ``typed_context``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MyFactory"
-                for="IMyType"
-            />
-        
-        - with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
-        - with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` provides ``IMyBehavior``,
-        
-        **Example 6** - the behavior should be restricted to the ``typed_context`` by auto-detection.
-        The ``MyTypedFactory`` class adapts ``IMyType`` using a class decorator ``@adapter(IMyType)``::
-        
-            <plone:behavior
-                title="Example 1"
-                provides="IMyBehavior"
-                marker="IMyMarker"
-                factory="MyTypedFactory"
-            />
-        
-        - with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
-        - with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
-        - ``context`` provides ``IMyMarker``,
-        - ``MyFactory`` instance provides ``IMyBehavior``,
-        
-        
-        Further Reading
-        ---------------
-        
-        For more details please read the doctests in the source code: ``behavior.rst``, ``directives.rst`` and ``annotation.rst``.
-        
-        
-        Source Code
-        ===========
-        
-        Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
-        
-        Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.behavior>`_.
-        
-        Changelog
-        =========
-        
-        .. You should *NOT* be adding new change log entries to this file.
-           You should create a file in the news directory instead.
-           For helpful instructions, please see:
-           https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
-        
-        .. towncrier release notes start
-        
-        1.4.0 (2020-09-07)
-        ------------------
-        
-        New features:
-        
-        
-        - Drop Plone 4.3 support.
-          [maurits] (#3130)
-        
-        
-        Bug fixes:
-        
-        
-        - Fixed deprecation warning for ComponentLookupError.
-          [maurits] (#3130)
-        
-        
-        1.3.2 (2020-04-20)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Minor packaging updates. (#1)
-        
-        
-        1.3.1 (2020-03-08)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Improved documentation.  [jensens] (#0)
-        
-        
-        1.3.0 (2019-02-13)
-        ------------------
-        
-        New features:
-        
-        
-        - New option ``former_dotted_names`` that allows to register the former name
-          under which a behavior used to be registerd. This can be useful to ensure a
-          smooth transition in case a behavior's dotted name is changed. [pysailor]
-          (#18)
-        
-        
-        1.2.1 (2018-01-17)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fixed import of dotted path in example.  [fulv]
-        
-        
-        1.2.0 (2017-03-23)
-        ------------------
-        
-        New features:
-        
-        - For zcml registration:
-          If both, no ``for`` and no ``@adapter`` is given,
-          fall first back to ``marker`` if given (new),
-          else to ``Interface`` (as it was already before).
-          [jensens]
-        
-        Bug fixes:
-        
-        - Cleanup: Make Jenkins CI code analysis silent by fixing the issues.
-          [jensens]
-        
-        
-        1.1.4 (2016-12-06)
-        ------------------
-        
-        Bug fixes:
-        
-        - Add already introduced attribute ``name`` to interface IBehavior.
-          This was missing.
-          Also modernized other IBehavior interface descriptions a bit.
-          [jensens]
-        
-        
-        1.1.3 (2016-11-09)
-        ------------------
-        
-        New features:
-        
-        - Support Python 3. [davisagli]
-        
-        
-        1.1.2 (2016-08-11)
-        ------------------
-        
-        New:
-        
-        - New option to register a behavior only by it's short name and not by it's dotted name.
-          This enables more advanced behavior subclassing capabilities.
-          [jensens]
-        
-        
-        1.1.1 (2016-02-25)
-        ------------------
-        
-        Fixes:
-        
-        - Make doctest comparison more robust against zope.component __repr__ changes.
-          [thet]
-        
-        
-        1.1 (2015-07-18)
-        ----------------
-        
-        - Corrected typo in warning.
-          [jensens]
-        
-        - Add name to behavior directive. This name can be used to lookup behavior
-          registrations by new plone.behaviors.registration.
-          lookup_behavior_registration function.
-          [rnixx]
-        
-        - Added more documentation, simplified code in directive, added a warning if
-          ``for`` is given w/o ``factory``.
-          [jensens]
-        
-        
-        1.0.3 (2015-04-29)
-        ------------------
-        
-        - Code modernization: utf-header, pep8, rst-files, adapter/implementer
-          decorators, ...
-          [jensens]
-        
-        
-        1.0.2 (2013-01-17)
-        ------------------
-        
-        - Remove dependence of tests on zope.app.testing.
-          [davisagli]
-        
-        
-        1.0.1 - 2011-05-20
-        ------------------
-        
-        - Relicense under BSD license.
-          See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
-          [davisagli]
-        
-        
-        1.0 - 2011-04-30
-        ----------------
-        
-        - Use stdlib doctest instead of the deprecated one in zope.testing.
-          [davisagli]
-        
-        - 'plone:behavior' zcml directive use now MessageID for title and description.
-          [sylvainb]
-        
-        
-        1.0b6 - 2009-11-17
-        ------------------
-        
-        - Fix tests for Zope 2.12
-          [optilude]
-        
-        
-        1.0b5 - 2009-07-12
-        ------------------
-        
-        - Changed API methods and arguments to mixedCase to be more consistent with
-          the rest of Zope. This is a non-backwards-compatible change. Our profuse
-          apologies, but it's now or never. :-/
-        
-          If you find that you get import errors or unknown keyword arguments in your
-          code, please change names from foo_bar too fooBar, e.g.
-          enumerate_behaviors() becomes enumerateBehaviors().
-          [optilude]
-        
-        
-        1.0b4 - 2009-06-07
-        ------------------
-        
-        - Allow a marker-interface-only behavior to be set by using the 'provides'
-          attribute (previously 'interface') in the <plone:behavior /> directive
-          without a 'factory' attribute. The 'marker' attribute (previously known as
-          'subtype') is now only required if there is a marker used in addition to
-          a behavior adapter with a separate interface ('provides') and factory.
-          [optilude]
-        
-        - Rename the 'interface' attribute of <plone:behavior /> to 'provides' to
-          be more consistent with the <adapter /> directive. This is a backwards
-          incompatible change!
-          [optilude]
-        
-        - Rename the 'subtype' attribute of <plone:behavior /> to 'marker' to
-          be more explicit about its purpose. This is a backwards
-          incompatible change!
-          [optilude]
-        
-        
-        1.0b3 - 2009-04-17
-        ------------------
-        
-        - Allow behaviors with no factory.
-          [alecm]
-        
-        - Provide a vocabulary of available behaviors.
-          [davisagli]
-        
-        
-        1.0b1 - 2008-04-27
-        ------------------
-        
-        - Initial release
-        
 Keywords: Plone behavior registry
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.8
 Provides-Extra: test
+
+==============
+plone.behavior
+==============
+
+.. contents:: Table of Contents
+   :depth: 2
+
+
+Overview
+========
+
+This package provides support for **behaviors**.
+
+    A behavior is a re-usable aspect of an object that can be enabled or disabled without changing the component registry.
+
+A behavior is described by an interface, and has metadata such as a title and a description.
+The behavior can be looked up by a given short name or by the dotted name of the interface.
+With this unique name behaviors metadata can be looked up.
+When the behavior is enabled for an object, you will be able to adapt the object to the interface.
+In some cases, the interface can be used as a marker interface as well.
+
+As an example, let's say that your application needs to support object-level locking.
+This can be modeled via an adapter, but you want to leave it until runtime to determine whether locking is enabled for a particular object.
+You could then register locking as a behavior.
+
+**Requirements and Limitations:**
+
+* This package comes with support for registering behaviors and factories.
+
+* It does not implement the policy for determining what behaviors are enabled on a particular object at a particular time.
+  That decision is deferred to an ``IBehaviorAssignable`` adapter, which must be implemented (``plone.dexterity`` implements this).
+
+* Like the ``IBehaviorAssignable`` plumbing, marker interface support needs to be enabled on a per-application basis.
+  This package also does not directly support the adding of marker interfaces to instances.
+  To do that, you can either use an event handler to mark an object when it is created, or a dynamic __providedBy__ descriptor that does the lookup on the fly (but you probably want some caching).
+  A sample event handler is provided with this package, but is not registered by default
+
+* The intention is that behavior assignment is generic across an application, used for multiple, optional behaviors.
+  It probably doesn't make much sense to use ``plone.behavior`` for a single type of object.
+  The means to keep track of which behaviors are enabled for what types of objects will be application specific.
+
+Usage
+=====
+
+Explained
+---------
+
+A behavior is written much like an adapter, except that you don't specify the type of context being adapted directly.
+For example::
+
+    from zope.interface import Interface
+    from zope.interface import implementer
+
+    class ILockingSupport(Interface):
+       """Support locking
+       """
+
+       def lock():
+           """Lock an object
+           """
+
+       def unlock():
+           """Unlock an object
+           """
+
+    @implementer(ILockingSupport)
+    class LockingSupport(object):
+
+        def __init__(self, context):
+            self.context = context
+
+        def lock(self):
+            # do something
+
+        def unlock(self):
+            # do something
+
+This interface (which describes the type of behavior) and class (which describes the implementation of the behavior) then needs to be registered.
+
+The simplest way to do that is to load the ``meta.zcml`` file from this package and use ZCML::
+
+    <configure
+      xmlns="http://namespaces.zope.org/zope"
+      xmlns:plone="http://namespaces.plone.org/plone"
+      i18n_domain="my.package">
+
+      <include package="plone.behavior" file="meta.zcml" />
+
+      <plone:behavior
+          name="locking_support"
+          title="Locking support"
+          description="Optional object-level locking"
+          provides=".interfaces.ILockingSupport"
+          factory=".locking.LockingSupport"
+      />
+
+    </configure>
+
+After this is done you can adapt a context to ``ILockingSupport`` as normal::
+
+    locking = ILockingSupport(context, None)
+
+    if locking is not None:
+        locking.lock()
+
+The ``name`` can be used for lookup instead of the full dotted name of the interface::
+
+    from plone.behavior.interfaces import IBehavior
+    from zope.component import getUtility
+
+    registration = getUtility(IBehavior, name='locking_support')
+
+We also have a helper function to achieve this::
+
+    from plone.behavior.registration import lookup_behavior_registration
+
+    registration = lookup_behavior_registration(name='locking_support')
+
+
+You'll get an instance of ``LockingSupport`` if context can be adapted to ``IBehaviorAssignable`` (which, recall, is application specific),
+and if the implementation of ``IBehaviorAssignable`` says that this context supports this particular behavior.
+
+It is also possible to let the provided interface act as a marker interface that is to be provided directly by the instance.
+To achieve this, omit the ``factory`` argument.
+This is useful if you need to register other adapters for instances providing a particular behavior.
+
+ZCML Reference
+--------------
+
+The ``plone:behavior`` directive uses the namespace ``xmlns:plone="http://namespaces.plone.org/plone"``.
+In order to enable it loading of its ``meta.zcml`` is needed, use::
+
+    <include package="plone.behavior" file="meta.zcml" />
+
+The directive supports the attributes:
+
+``title``
+    A user friendly title for this behavior (required).
+
+``description``
+    A longer description for this behavior (optional).
+
+``provides``
+    An interface to which the behavior can be adapted.
+    This is what the conditional adapter factory will be registered as providing (required).
+
+``name``
+    Convenience lookup name for this behavior (optional).
+    The behavior will be always registered under the dotted name of ``provides`` attribute.
+    This are usually long names. ``name`` is a short name for this.
+    If ``name`` is given the behavior is registered additional under it.
+    Anyway using short namespaces in ``name`` is recommended.
+
+``name_only``
+    If set to ``yes`` or ``true`` the behavior is registered only under the given name,
+    but not under the dotted path of the ``provides`` interface.
+    This makes ``name`` mandatory.
+
+``marker``
+    A marker interface to be applied by the behavior.
+    If ``factory`` is not given, then this is optional and defaults to the value of ``provides``.
+    If factory is given ``marker`` is required and should be different from ``provides`` - even if its not enforced.
+
+``factory``
+    The factory for this behavior (optional).
+    If no factory is given, the behavior context is assumed to provide the interface given by ``provides`` itself.
+
+    If factory provides ``plone.behavior.interfaces.ISchemaAwareFactory`` the factory is assumed to be a callable.
+    ``ISchemaAwareFactory`` is an interface for factories that should be initialised with a schema.
+    It is called with the value given in ``provides`` as the only argument.
+    The value returned is then used as the factory, another callable that can create appropriate behavior factories on demand.
+
+``for``
+    The type of object to register the conditional adapter factory for (optional).
+    Must be omitted is no ``factory`` is given.
+
+    The default is either to auto-detect what the factory adapts (i.e. using the ``@adapter`` decorator) or to fall back to ``zope.interface.Interface`` (also written as ``*`` in ZCML).
+
+    Must be one element (no multiadapters, applies also for auto-detection).
+
+``former_dotted_names``
+    In case a behavior is modified so that its dotted name changes, this field can be used to register the old name(s). Therefore, it is possible to retrieve the name(s) under which a behavior was formerly registered under.
+
+    If a call to ``lookup_behavior_registration`` does not find a behavior under the given name, it will look at the former dotted names to try and find the behavior.
+
+
+ZCML Examples
+-------------
+
+Example usage, given
+
+- some ``context`` (some arbitrary object) which is ``IBehaviorAssignable``,
+- an ``IMyBehavior`` interface intended to be used as ``provides``,
+- an ``IMyMarker`` interface intended to be used as ``marker``,
+- a ``MyFactory`` class implementing ``IMyBehavior`` ,
+- a ``MySchemaAwareFactory`` class implementing ``IMyBehavior`` and ``plone.behavior.interfaces.ISchemaAwareFactory``,
+- an ``IMyType`` intended to be used as ``for``.
+- some ``typed_context`` (some arbitrary object) which is ``IBehaviorAssignable`` and provides ``IMyType``,
+- an ``MyTypedFactory`` class implementing ``IMyBehavior`` and adapting ``IMyType``,
+
+``title`` and ``description`` is trivial, so we dont cover it here in the explanantion.
+We dont cover ``name`` too, because it's not having any effect in this usage.
+To simplify it, we assume ``context`` ``IBehaviorAssignable`` always supports the behavior.
+Also for simplifications sake we assume some magic applies the marker interface to ``context``
+I.e. both is done by ``plone.dexterity``.
+
+**Example 1** - only ``provides`` given::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+    />
+
+- ``marker`` defaults to ``provides``,
+- with ``behavior = IMyBehavior(context)`` the ``context`` itself is returned,
+- ``context`` provides ``IBehavior``,
+
+**Example 2** - also ``factory`` is given, so ``marker`` is required:
+
+.. warning::
+   Using the same Interface as marker and behavior works, but is not recommended and will be deprecated in future.
+   It is semantically wrong!
+
+   Go for Example 3 instead!
+
+::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyBehavior"
+        factory="MyFactory"
+    />
+
+- ``marker`` is the same as ``provides``,
+- with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyBehavior``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+- having ``context`` and ``MyFactory`` providing both the same interface is ugly and not recommended!
+
+**Example 3** - in example 2 both, factory and context are providing the ``IMyBehavior``.
+This may lead to confusion, so now better with a ``marker``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MyFactory"
+    />
+
+- with ``behavior = IMyBehavior(context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+
+**Example 4** - like example 3 but with an ``MySchemaAwareFactory``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MySchemaAwareFactory"
+    />
+
+- with ``behavior = IMyBehavior(context)`` some factory instance is returned as a result from calling a ``MySchemaAwareFactory`` instance with ``IMyBehavior`` as argument,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+
+**Example 5** - the behavior should be restricted to the ``typed_context``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MyFactory"
+        for="IMyType"
+    />
+
+- with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
+- with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` provides ``IMyBehavior``,
+
+**Example 6** - the behavior should be restricted to the ``typed_context`` by auto-detection.
+The ``MyTypedFactory`` class adapts ``IMyType`` using a class decorator ``@adapter(IMyType)``::
+
+    <plone:behavior
+        title="Example 1"
+        provides="IMyBehavior"
+        marker="IMyMarker"
+        factory="MyTypedFactory"
+    />
+
+- with ``behavior = IMyBehavior(context, None)`` it could not adapt and ``behavior`` is ``None``,
+- with ``behavior = IMyBehavior(typed_context)`` a ``MyFactory`` instance is returned,
+- ``context`` provides ``IMyMarker``,
+- ``MyFactory`` instance provides ``IMyBehavior``,
+
+
+Further Reading
+---------------
+
+For more details please read the doctests in the source code: ``behavior.rst``, ``directives.rst`` and ``annotation.rst``.
+
+
+Source Code
+===========
+
+Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
+
+Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.behavior>`_.
+
+Changelog
+=========
+
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.0.0 (2023-04-15)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a9dd65cc)
+
+
+1.4.0 (2020-09-07)
+------------------
+
+New features:
+
+
+- Drop Plone 4.3 support.
+  [maurits] (#3130)
+
+
+Bug fixes:
+
+
+- Fixed deprecation warning for ComponentLookupError.
+  [maurits] (#3130)
+
+
+1.3.2 (2020-04-20)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+1.3.1 (2020-03-08)
+------------------
+
+Bug fixes:
+
+
+- Improved documentation.  [jensens] (#0)
+
+
+1.3.0 (2019-02-13)
+------------------
+
+New features:
+
+
+- New option ``former_dotted_names`` that allows to register the former name
+  under which a behavior used to be registered. This can be useful to ensure a
+  smooth transition in case a behavior's dotted name is changed. [pysailor]
+  (#18)
+
+
+1.2.1 (2018-01-17)
+------------------
+
+Bug fixes:
+
+- Fixed import of dotted path in example.  [fulv]
+
+
+1.2.0 (2017-03-23)
+------------------
+
+New features:
+
+- For zcml registration:
+  If both, no ``for`` and no ``@adapter`` is given,
+  fall first back to ``marker`` if given (new),
+  else to ``Interface`` (as it was already before).
+  [jensens]
+
+Bug fixes:
+
+- Cleanup: Make Jenkins CI code analysis silent by fixing the issues.
+  [jensens]
+
+
+1.1.4 (2016-12-06)
+------------------
+
+Bug fixes:
+
+- Add already introduced attribute ``name`` to interface IBehavior.
+  This was missing.
+  Also modernized other IBehavior interface descriptions a bit.
+  [jensens]
+
+
+1.1.3 (2016-11-09)
+------------------
+
+New features:
+
+- Support Python 3. [davisagli]
+
+
+1.1.2 (2016-08-11)
+------------------
+
+New:
+
+- New option to register a behavior only by it's short name and not by it's dotted name.
+  This enables more advanced behavior subclassing capabilities.
+  [jensens]
+
+
+1.1.1 (2016-02-25)
+------------------
+
+Fixes:
+
+- Make doctest comparison more robust against zope.component __repr__ changes.
+  [thet]
+
+
+1.1 (2015-07-18)
+----------------
+
+- Corrected typo in warning.
+  [jensens]
+
+- Add name to behavior directive. This name can be used to lookup behavior
+  registrations by new plone.behaviors.registration.
+  lookup_behavior_registration function.
+  [rnixx]
+
+- Added more documentation, simplified code in directive, added a warning if
+  ``for`` is given w/o ``factory``.
+  [jensens]
+
+
+1.0.3 (2015-04-29)
+------------------
+
+- Code modernization: utf-header, pep8, rst-files, adapter/implementer
+  decorators, ...
+  [jensens]
+
+
+1.0.2 (2013-01-17)
+------------------
+
+- Remove dependence of tests on zope.app.testing.
+  [davisagli]
+
+
+1.0.1 - 2011-05-20
+------------------
+
+- Relicense under BSD license.
+  See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
+  [davisagli]
+
+
+1.0 - 2011-04-30
+----------------
+
+- Use stdlib doctest instead of the deprecated one in zope.testing.
+  [davisagli]
+
+- 'plone:behavior' zcml directive use now MessageID for title and description.
+  [sylvainb]
+
+
+1.0b6 - 2009-11-17
+------------------
+
+- Fix tests for Zope 2.12
+  [optilude]
+
+
+1.0b5 - 2009-07-12
+------------------
+
+- Changed API methods and arguments to mixedCase to be more consistent with
+  the rest of Zope. This is a non-backwards-compatible change. Our profuse
+  apologies, but it's now or never. :-/
+
+  If you find that you get import errors or unknown keyword arguments in your
+  code, please change names from foo_bar too fooBar, e.g.
+  enumerate_behaviors() becomes enumerateBehaviors().
+  [optilude]
+
+
+1.0b4 - 2009-06-07
+------------------
+
+- Allow a marker-interface-only behavior to be set by using the 'provides'
+  attribute (previously 'interface') in the <plone:behavior /> directive
+  without a 'factory' attribute. The 'marker' attribute (previously known as
+  'subtype') is now only required if there is a marker used in addition to
+  a behavior adapter with a separate interface ('provides') and factory.
+  [optilude]
+
+- Rename the 'interface' attribute of <plone:behavior /> to 'provides' to
+  be more consistent with the <adapter /> directive. This is a backwards
+  incompatible change!
+  [optilude]
+
+- Rename the 'subtype' attribute of <plone:behavior /> to 'marker' to
+  be more explicit about its purpose. This is a backwards
+  incompatible change!
+  [optilude]
+
+
+1.0b3 - 2009-04-17
+------------------
+
+- Allow behaviors with no factory.
+  [alecm]
+
+- Provide a vocabulary of available behaviors.
+  [davisagli]
+
+
+1.0b1 - 2008-04-27
+------------------
+
+- Initial release
```

### Comparing `plone.behavior-1.4.0/plone.behavior.egg-info/SOURCES.txt` & `plone.behavior-2.0.0/plone.behavior.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 setup.py
 docs/INSTALL.txt
 docs/LICENSE.txt
 plone/__init__.py
 plone.behavior.egg-info/PKG-INFO
 plone.behavior.egg-info/SOURCES.txt
 plone.behavior.egg-info/dependency_links.txt
-plone.behavior.egg-info/entry_points.txt
 plone.behavior.egg-info/namespace_packages.txt
 plone.behavior.egg-info/not-zip-safe
 plone.behavior.egg-info/requires.txt
 plone.behavior.egg-info/top_level.txt
 plone/behavior/__init__.py
 plone/behavior/annotation.py
 plone/behavior/annotation.rst
```

### Comparing `plone.behavior-1.4.0/docs/INSTALL.txt` & `plone.behavior-2.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.behavior-1.4.0/docs/LICENSE.txt` & `plone.behavior-2.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.behavior-1.4.0/plone/behavior/registration.py` & `plone.behavior-2.0.0/plone/behavior/registration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-# -*- coding: utf-8 -*-
 from plone.behavior import logger
 from plone.behavior.interfaces import IBehavior
 from zope.component import ComponentLookupError
 from zope.component import getUtilitiesFor
 from zope.component import getUtility
 from zope.interface import implementer
 
-import sys
 import textwrap
 
 
-if sys.version_info[0] >= 3:
-    text_type = str
-else:
-    text_type = unicode
-
-
 REGISTRATION_REPR = """\
 <{class} {name} at {id}
   schema: {identifier}
   marker: {marker}
   factory: {factory}
   title: {title}
   {description}{extra_info}
 >"""
 
 
 @implementer(IBehavior)
-class BehaviorRegistration(object):
-
-    def __init__(self, title, description, interface,
-                 marker, factory, name=None, former_dotted_names=''):
+class BehaviorRegistration:
+    def __init__(
+        self,
+        title,
+        description,
+        interface,
+        marker,
+        factory,
+        name=None,
+        former_dotted_names="",
+    ):
         self.title = title
         self.description = description
         self.interface = interface
         self.marker = marker
         self.factory = factory
         self.name = name
         self.former_dotted_names = former_dotted_names
 
     def __repr__(self):
         if self.marker is not None:
             marker_info = self.marker.__identifier__
         elif self.marker is not None and self.marker is not self.interface:
-            marker_info = '(uses schema as marker)'
+            marker_info = "(uses schema as marker)"
         else:
-            marker_info = '(no marker is set)'
+            marker_info = "(no marker is set)"
         info = {
-            'class': self.__class__.__name__,
-            'id': id(self),
-            'name': self.name or '(unique name not set)',
-            'identifier': self.interface.__identifier__,
-            'marker': marker_info,
-            'factory': text_type(self.factory),
-            'title': self.title or '(no title)',
-            'description': textwrap.fill(
-                self.description or '(no description)',
-                subsequent_indent='  ',
+            "class": self.__class__.__name__,
+            "id": id(self),
+            "name": self.name or "(unique name not set)",
+            "identifier": self.interface.__identifier__,
+            "marker": marker_info,
+            "factory": str(self.factory),
+            "title": self.title or "(no title)",
+            "description": textwrap.fill(
+                self.description or "(no description)",
+                subsequent_indent="  ",
             ),
-            'extra_info': (
-                self.former_dotted_names and
-                '\n  former dotted names: {0}'.format(self.former_dotted_names)
+            "extra_info": (
+                self.former_dotted_names
+                and f"\n  former dotted names: {self.former_dotted_names}"
             ),
         }
         return REGISTRATION_REPR.format(**info)
 
 
 class BehaviorRegistrationNotFound(Exception):
-    """Exception thrown if behavior registration lookup fails.
-    """
+    """Exception thrown if behavior registration lookup fails."""
 
 
-def lookup_behavior_registration(
-        name=None, identifier=None, warn_about_fallback=True):
+def lookup_behavior_registration(name=None, identifier=None, warn_about_fallback=True):
     """Look up behavior registration either by name or interface identifier.
        Fall back to checking the former_dotted_names if the lookup is not
        successful.
 
     ``ValueError`` is thrown if function call is incomplete.
     ``BehaviorRegistrationNotFound`` is thrown if lookup fails.
     """
     try:
-        assert(name or identifier)
+        assert name or identifier
     except AssertionError:
-        raise ValueError('Either ``name`` or ``identifier`` must be given')
+        raise ValueError("Either ``name`` or ``identifier`` must be given")
     # identifier rules if given
     if identifier:
         name = identifier
     try:
         return getUtility(IBehavior, name=name)
     except ComponentLookupError:
         for id_, behavior in getUtilitiesFor(IBehavior):
             # Before we raise an error, iterate over all behaviors and check
             # if the requested name is registered as a former dotted name.
             if name in behavior.former_dotted_names:
                 if warn_about_fallback:
-                    logger.warn(
-                        'The dotted name "{0}" is deprecated. It has been '
-                        'changed to "{1}"'.format(
-                            name, behavior.interface.__identifier__, ))
+                    logger.warning(
+                        'The dotted name "{}" is deprecated. It has been '
+                        'changed to "{}"'.format(
+                            name,
+                            behavior.interface.__identifier__,
+                        )
+                    )
                 return behavior
         raise BehaviorRegistrationNotFound(name)
```

### Comparing `plone.behavior-1.4.0/plone/behavior/interfaces.py` & `plone.behavior-2.0.0/plone/behavior/interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from zope import schema
 from zope.interface import Interface
 from zope.interface.interfaces import IInterface
 
 
 class IBehaviorAssignable(Interface):
     """An object will be adapted to this interface to determine if it supports
@@ -14,60 +13,59 @@
 
     def supports(behavior_interface):
         """Determine if the context supports the given behavior, returning
         True or False.
         """
 
     def enumerateBehaviors():
-        """Return an iterable of all the IBehaviors supported by the context.
-        """
+        """Return an iterable of all the IBehaviors supported by the context."""
 
 
 class IBehavior(Interface):
     """A description of a behavior. These should be registered as named
     utilities. There should also be an adapter factory registered, probably
     using IBehaviorAdapterFactory.
     """
 
     title = schema.TextLine(
-        title=u'Short title of the behavior',
+        title="Short title of the behavior",
         required=True,
     )
 
     description = schema.Text(
-        title=u'Longer description of the behavior',
+        title="Longer description of the behavior",
         required=False,
     )
 
     name = schema.TextLine(
-        title=u'Readable short name to be used for behavior lookup',
-        description=u'E.g. plone.somebehavior. If not given the full dotted '
-                    u'name of the interfaces is used for lookup instead.'
-                    u'Recommended, but due to BBB not required.',
+        title="Readable short name to be used for behavior lookup",
+        description="E.g. plone.somebehavior. If not given the full dotted "
+        "name of the interfaces is used for lookup instead."
+        "Recommended, but due to BBB not required.",
         required=False,
     )
 
     interface = schema.Object(
-        title=u'Interface describing this behavior',
+        title="Interface describing this behavior",
         required=True,
         schema=IInterface,
     )
 
     marker = schema.Object(
-        title=u'Marker interface for objects sporting this behavior',
-        description=u'Markers are persisted in the ZODB. '
-                    u'Required when a factory is given, because the factory '
-                    u'is an adapter adapting the the marker and providing the '
-                    u'"interface" of this behavior.',
+        title="Marker interface for objects sporting this behavior",
+        description="Markers are persisted in the ZODB. "
+        "Required when a factory is given, because the factory "
+        "is an adapter adapting the the marker and providing the "
+        '"interface" of this behavior.',
         required=False,
         schema=IInterface,
     )
 
     factory = schema.Object(
-        title=u'An adapter factory for the behavior',
+        title="An adapter factory for the behavior",
         required=True,
         schema=Interface,
     )
 
 
 class IBehaviorAdapterFactory(Interface):
     """An adapter factory that wraps a given behavior's own factory. By
@@ -81,15 +79,15 @@
      The ISomeBehavior adapter factory (i.e. the object providing
      IBehaviorAdapterFactory) will return None if
      IBehaviorAssignable(context).supports(ISomeBehavior) is False, or if
      the context cannot be adapted to IBehaviorAssignable at all.
     """
 
     behavior = schema.Object(
-        title=u'The behavior this is a factory for',
+        title="The behavior this is a factory for",
         schema=IBehavior,
     )
 
     def __call__(context):
         """Invoke the behavior-specific factory if the context can be adapted
         to IBehaviorAssignable and
         IBehaviorAssignable(context).supports(self.behavior.interface) returns
```

### Comparing `plone.behavior-1.4.0/plone/behavior/annotation.py` & `plone.behavior-2.0.0/plone/behavior/annotation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-# -*- coding: utf-8 -*-
 from plone.behavior.interfaces import ISchemaAwareFactory
 from zope.annotation.interfaces import IAnnotatable
 from zope.annotation.interfaces import IAnnotations
 from zope.component import adapter
 from zope.interface import alsoProvides
 from zope.interface import provider
 
 
 @adapter(IAnnotatable)
-class AnnotationsFactoryImpl(object):
+class AnnotationsFactoryImpl:
     """A factory that knows how to store data in annotations.
 
     Each value will be stored as a primitive in the annotations under a key
     that consists of the full dotted name to the field being stored.
 
     This class is not sufficient as an adapter factory on its own. It must
     be initialised with the schema interface in the first place. That is the
     role of the Annotations factory below.
     """
 
     def __init__(self, context, schema):
-        self.__dict__['schema'] = schema
-        self.__dict__['prefix'] = schema.__identifier__ + '.'
-        self.__dict__['annotations'] = IAnnotations(context)
+        self.__dict__["schema"] = schema
+        self.__dict__["prefix"] = schema.__identifier__ + "."
+        self.__dict__["annotations"] = IAnnotations(context)
         alsoProvides(self, schema)
 
     def __getattr__(self, name):
-        if name not in self.__dict__['schema']:
+        if name not in self.__dict__["schema"]:
             raise AttributeError(name)
 
-        annotations = self.__dict__['annotations']
-        key_name = self.__dict__['prefix'] + name
+        annotations = self.__dict__["annotations"]
+        key_name = self.__dict__["prefix"] + name
         if key_name not in annotations:
-            return self.__dict__['schema'][name].missing_value
+            return self.__dict__["schema"][name].missing_value
 
         return annotations[key_name]
 
     def __setattr__(self, name, value):
-        if name not in self.__dict__['schema']:
-            super(AnnotationsFactoryImpl, self).__setattr__(name, value)
+        if name not in self.__dict__["schema"]:
+            super().__setattr__(name, value)
         else:
-            prefixed_name = self.__dict__['prefix'] + name
-            self.__dict__['annotations'][prefixed_name] = value
+            prefixed_name = self.__dict__["prefix"] + name
+            self.__dict__["annotations"][prefixed_name] = value
 
 
 @provider(ISchemaAwareFactory)
-class AnnotationStorage(object):
-    """Behavior adapter factory class for storing data in annotations.
-    """
+class AnnotationStorage:
+    """Behavior adapter factory class for storing data in annotations."""
 
     def __init__(self, schema):
         self.schema = schema
         self.__component_adapts__ = (IAnnotatable,)
 
     def __call__(self, context):
         return AnnotationsFactoryImpl(context, self.schema)
```

### Comparing `plone.behavior-1.4.0/plone/behavior/behaviors.rst` & `plone.behavior-2.0.0/plone/behavior/behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.behavior-1.4.0/plone/behavior/directives.rst` & `plone.behavior-2.0.0/plone/behavior/directives.rst`

 * *Files 2% similar despite different names*

```diff
@@ -150,21 +150,21 @@
     >>> from plone.behavior.interfaces import IBehavior
 
 1) A standard behavior with an interface and a factory. It will be registered
 for any context.
 
     >>> dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IAdapterBehavior")
     >>> dummy.name
-    u'adapter_behavior'
+    'adapter_behavior'
 
     >>> dummy.title
-    u'Adapter behavior'
+    'Adapter behavior'
 
     >>> dummy.description
-    u'A basic adapter behavior'
+    'A basic adapter behavior'
 
     >>> dummy.interface
     <InterfaceClass plone.behavior.tests.IAdapterBehavior>
 
     >>> dummy.marker is None
     True
 
@@ -175,18 +175,18 @@
     >>> [a.required for a in sm.registeredAdapters() if a.provided == IAdapterBehavior][0]
     (<InterfaceClass zope.interface.Interface>,)
 
 2) An adapter behavior with a factory and an explicit context restriction.
 
     >>> dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IRestrictedAdapterBehavior")
     >>> dummy.name
-    u'context_restricted_behavior'
+    'context_restricted_behavior'
 
     >>> dummy.title
-    u'Context restricted behavior'
+    'Context restricted behavior'
 
     >>> dummy.description is None
     True
 
     >>> dummy.interface
     <InterfaceClass plone.behavior.tests.IRestrictedAdapterBehavior>
 
@@ -201,18 +201,18 @@
     (<InterfaceClass plone.behavior.tests.IMinimalContextRequirements>,)
 
 3) An adapter behavior where a context restriction is implied by the adapts()
 declaration on the factory.
 
     >>> dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IImpliedRestrictionAdapterBehavior")
     >>> dummy.name
-    u'factory_implied_context_restricted_behavior'
+    'factory_implied_context_restricted_behavior'
 
     >>> dummy.title
-    u'Factory-implied context restricted behavior'
+    'Factory-implied context restricted behavior'
 
     >>> dummy.description is None
     True
 
     >>> dummy.interface
     <InterfaceClass plone.behavior.tests.IImpliedRestrictionAdapterBehavior>
 
@@ -226,18 +226,18 @@
     >>> [a.required for a in sm.registeredAdapters() if a.provided == IImpliedRestrictionAdapterBehavior][0]
     (<InterfaceClass plone.behavior.tests.ISomeContext>,)
 
 4) A behavior with a marker marker interface.
 
     >>> dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IMarkerBehavior")
     >>> dummy.name
-    u'marker_interface_behavior'
+    'marker_interface_behavior'
 
     >>> dummy.title
-    u'Marker interface behavior'
+    'Marker interface behavior'
 
     >>> dummy.description is None
     True
 
     >>> dummy.interface
     <InterfaceClass plone.behavior.tests.IMarkerBehavior>
 
@@ -251,18 +251,18 @@
     >>> [a.required for a in sm.registeredAdapters() if a.provided == IMarkerBehavior]
     []
 
 5) A behavior using the standard annotation factory
 
     >>> dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IAnnotationStored")
     >>> dummy.name
-    u'annotation_storage_behavior'
+    'annotation_storage_behavior'
 
     >>> dummy.title
-    u'Annotation storage behavior'
+    'Annotation storage behavior'
 
     >>> dummy.description is None
     True
 
     >>> dummy.interface
     <InterfaceClass plone.behavior.tests.IAnnotationStored>
 
@@ -278,60 +278,60 @@
 
 6) A behavior providing a marker interface and using an adapter factory.
 
 6.1) ``@adapter`` decorated Behavior implementation.
 
     >>> dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IMarkerAndAdapterBehavior")
     >>> dummy.name
-    u'marker_and_adapter'
+    'marker_and_adapter'
 
     >>> dummy.title
-    u'Marker and adapter'
+    'Marker and adapter'
 
     >>> dummy.description is None
     True
 
     >>> dummy.interface
     <InterfaceClass plone.behavior.tests.IMarkerAndAdapterBehavior>
 
     >>> dummy.marker
     <InterfaceClass plone.behavior.tests.IMarkerAndAdapterMarker>
 
     >>> dummy.factory # doctest: +ELLIPSIS
     <plone.behavior.annotation.AnnotationStorage object at ...>
 
-    The factory has ist ``__component_adapts__`` (``@adapter``) in place, so the adapted Interface must be returned.
+    The factory has it's ``__component_adapts__`` (``@adapter``) in place, so the adapted Interface must be returned.
 
     >>> from plone.behavior.tests import IMarkerAndAdapterBehavior
     >>> [a.required for a in sm.registeredAdapters() if a.provided == IMarkerAndAdapterBehavior][0]
     (<InterfaceClass zope.annotation.interfaces.IAnnotatable>,)
 
 
 6.2) non ``@adapter`` decorated Behavior implementation.
 
     >>> dummy = getUtility(IBehavior, name=u"marker_and_adapter_no_atadapter")
     >>> dummy.name
-    u'marker_and_adapter_no_atadapter'
+    'marker_and_adapter_no_atadapter'
 
     >>> dummy.title
-    u'Marker and adapter no @adapter'
+    'Marker and adapter no @adapter'
 
     >>> dummy.description is None
     True
 
     >>> dummy.interface
     <InterfaceClass plone.behavior.tests.IMarkerAndAdapterBehavior2>
 
     >>> dummy.marker
     <InterfaceClass plone.behavior.tests.IMarkerAndAdapterMarker2>
 
     >>> dummy.factory # doctest: +ELLIPSIS
     <class 'plone.behavior.tests.DummyBehaviorImpl'>
 
-    The factory has ist ``__component_adapts__`` (``@adapter``) in place, so the adapted Interface must be returned.
+    The factory has it's ``__component_adapts__`` (``@adapter``) in place, so the adapted Interface must be returned.
 
     >>> from plone.behavior.tests import IMarkerAndAdapterBehavior2
     >>> [a.required for a in sm.registeredAdapters() if a.provided == IMarkerAndAdapterBehavior2][0]
     (<InterfaceClass plone.behavior.tests.IMarkerAndAdapterMarker2>,)
 
 
 7) A name only registered behavior
@@ -343,21 +343,21 @@
     ... except ComponentLookupError as e:
     ...     failed = True
     >>> failed
     True
 
     >>> dummy = getUtility(IBehavior, name=u"name_only")
     >>> dummy.name
-    u'name_only'
+    'name_only'
 
 8) A behavior that used to be known under a different dotted name
 
     A behavior that has been renamed, can of course be found under the new name.
     The representation tells us the former dotted name.
-    
+
     >>> dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IRenamedAdapterBehavior")
     >>> dummy  # doctest: +ELLIPSIS
     <BehaviorRegistration renamed_adapter_behavior at ...
       schema: plone.behavior.tests.IRenamedAdapterBehavior
       marker: (no marker is set)
       factory: <class 'plone.behavior.tests.RenamedAdapterBehavior'>
       title: Renamed Adapter behavior
@@ -372,15 +372,15 @@
     Traceback (most recent call last):
       ...
     ValueError: Either ``name`` or ``identifier`` must be given
 
     >>> lookup_behavior_registration('inexistent')
     Traceback (most recent call last):
       ...
-    BehaviorRegistrationNotFound: inexistent
+    plone.behavior.registration.BehaviorRegistrationNotFound: inexistent
 
     >>> lookup_behavior_registration('adapter_behavior')  # doctest: +ELLIPSIS
     <BehaviorRegistration adapter_behavior at ...
       schema: plone.behavior.tests.IAdapterBehavior
       marker: (no marker is set)
       factory: <class 'plone.behavior.tests.AdapterBehavior'>
       title: Adapter behavior
@@ -395,21 +395,21 @@
       marker: (no marker is set)
       factory: <class 'plone.behavior.tests.AdapterBehavior'>
       title: Adapter behavior
       A basic adapter behavior
     >
 
     A lookup via getUtility for a former behavior name fails.
-    
+
     >>> failed = False
     >>> try:
     ...     dummy = getUtility(IBehavior, name=u"plone.behavior.tests.IOriginalAdapterBehavior")
     ... except ComponentLookupError:
     ...     failed = True
     >>> failed
     True
 
     But the lookup helper still finds it under the former name.
-    
+
     >>> dummy = lookup_behavior_registration("plone.behavior.tests.IOriginalAdapterBehavior")
     >>> dummy.name
-    u'renamed_adapter_behavior'
+    'renamed_adapter_behavior'
```

### Comparing `plone.behavior-1.4.0/plone/behavior/factory.py` & `plone.behavior-2.0.0/plone/behavior/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# -*- coding: utf-8 -*-
 from plone.behavior.interfaces import IBehaviorAdapterFactory
 from plone.behavior.interfaces import IBehaviorAssignable
 from zope.interface import implementer
 
 
 @implementer(IBehaviorAdapterFactory)
-class BehaviorAdapterFactory(object):
-
+class BehaviorAdapterFactory:
     def __init__(self, behavior):
         self.behavior = behavior
 
     def __call__(self, context):
         assignable = IBehaviorAssignable(context, None)
         if assignable is None:
             return None
```

### Comparing `plone.behavior-1.4.0/plone/behavior/annotation.rst` & `plone.behavior-2.0.0/plone/behavior/annotation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -90,22 +90,22 @@
 Let's look at the annotations also::
 
     >>> sorted(IAnnotations(context).items())
     []
 
 If we now set the value, it will be stored in annotations::
 
-    >>> adapted.some_field = u'New value'
+    >>> adapted.some_field = 'New value'
     >>> sorted(IAnnotations(context).items())
-    [('plone.behavior.tests.IAnnotationStored.some_field', u'New value')]
+    [('plone.behavior.tests.IAnnotationStored.some_field', 'New value')]
 
 And of course we can get it back again::
 
     >>> adapted.some_field
-    u'New value'
+    'New value'
 
 If we try to get some other field, we get an AttributeError::
 
     >>> adapted.bogus_field #doctest: +ELLIPSIS
     Traceback (most recent call last):
     ...
     AttributeError: bogus_field
```

### Comparing `plone.behavior-1.4.0/plone/behavior/metaconfigure.py` & `plone.behavior-2.0.0/plone/behavior/metaconfigure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.behavior import logger
 from plone.behavior.factory import BehaviorAdapterFactory
 from plone.behavior.interfaces import IBehavior
 from plone.behavior.interfaces import ISchemaAwareFactory
 from plone.behavior.registration import BehaviorRegistration
 from zope.component.zcml import adapter
 from zope.component.zcml import utility
@@ -19,116 +18,122 @@
 
         * a global named utility registered by interface identifier
         * a global named utility registered by lookup name
         * an associated global and unnamed behavior adapter
     """
 
     name = TextLine(
-        title=u'Name',
-        description=u'Convenience lookup name for this behavior',
+        title="Name",
+        description="Convenience lookup name for this behavior",
         required=False,
     )
 
     title = configuration_fields.MessageID(
-        title=u'Title',
-        description=u'A user friendly title for this behavior',
+        title="Title",
+        description="A user friendly title for this behavior",
         required=True,
     )
 
     description = configuration_fields.MessageID(
-        title=u'Description',
-        description=u'A longer description for this behavior',
+        title="Description",
+        description="A longer description for this behavior",
         required=False,
     )
 
     provides = configuration_fields.GlobalInterface(
-        title=u'An interface to which the behavior can be adapted',
-        description=u'This is what the conditional adapter factory will '
-                    u'be registered as providing',
+        title="An interface to which the behavior can be adapted",
+        description="This is what the conditional adapter factory will "
+        "be registered as providing",
         required=True,
     )
 
     marker = configuration_fields.GlobalInterface(
-        title=u'A marker interface to be applied by the behavior',
-        description=u'If factory is not given, then this is optional',
+        title="A marker interface to be applied by the behavior",
+        description="If factory is not given, then this is optional",
         required=False,
     )
 
     factory = configuration_fields.GlobalObject(
-        title=u'The factory for this behavior',
-        description=u'If this is not given, the behavior is assumed to '
-                    u'provide a marker interface',
+        title="The factory for this behavior",
+        description="If this is not given, the behavior is assumed to "
+        "provide a marker interface",
         required=False,
     )
 
     for_ = configuration_fields.GlobalObject(
-        title=u'The type of object to register the conditional adapter '
-              u'factory for',
-        description=u'This is optional - the default is to register the '
-                    u'factory for zope.interface.Interface',
+        title="The type of object to register the conditional adapter " "factory for",
+        description="This is optional - the default is to register the "
+        "factory for zope.interface.Interface",
         required=False,
     )
 
     name_only = configuration_fields.Bool(
-        title=u'Do not register the behavior under the dotted path, but '
-              u'only under the given name',
-        description=u'Use this option to register a behavior for the same '
-                    u'provides under a different name.',
+        title="Do not register the behavior under the dotted path, but "
+        "only under the given name",
+        description="Use this option to register a behavior for the same "
+        "provides under a different name.",
         required=False,
     )
 
     former_dotted_names = TextLine(
-        title=u'Space-separated list of dotted names that this behavior was '
-              u'formerly registered under',
-        description=u'Use this field in case you change the dotted name, '
-                    u'so that the current behavior can be looked up under '
-                    u'its former name.',
+        title="Space-separated list of dotted names that this behavior was "
+        "formerly registered under",
+        description="Use this field in case you change the dotted name, "
+        "so that the current behavior can be looked up under "
+        "its former name.",
         required=False,
     )
 
 
 def _detect_for(factory, marker):
-    """if no explicit for is given we need to figure it out.
-    """
+    """if no explicit for is given we need to figure it out."""
     # Attempt to guess the factory's adapted interface and use it as
     # the 'for_'.
     # at last bastion fallback to '*' (=Interface).
-    adapts = getattr(factory, '__component_adapts__', [])
+    adapts = getattr(factory, "__component_adapts__", [])
     if len(adapts) == 1:
         return adapts[0]
     if len(adapts) > 1:
-        raise ConfigurationError(
-            u'The factory can not be declared as multi-adapter.')
+        raise ConfigurationError("The factory can not be declared as multi-adapter.")
     # down here it means len(adapts) < 1
     if marker is not None:
         # given we have a marker it is safe to register for the
         # marker, as the behavior context will always provides it
         return marker
     # fallback: for="*"
     return Interface
 
 
-def behaviorDirective(_context, title, provides, name=None, description=None,
-                      marker=None, factory=None, for_=None, name_only=False,
-                      former_dotted_names=''):
-
+def behaviorDirective(
+    _context,
+    title,
+    provides,
+    name=None,
+    description=None,
+    marker=None,
+    factory=None,
+    for_=None,
+    name_only=False,
+    former_dotted_names="",
+):
     if marker is None and factory is None:
         # a schema only behavior means usually direct attribute settings on the
         # object itself, so the object itself provides the interface.
         # so we mark with the provides.
         marker = provides
 
     if marker is not None and factory is None and marker is not provides:
         raise ConfigurationError(
-            u'You cannot specify a different \'marker\' and \'provides\' if '
-            u'there is no adapter factory for the provided interface.')
+            "You cannot specify a different 'marker' and 'provides' if "
+            "there is no adapter factory for the provided interface."
+        )
     if name_only and name is None:
         raise ConfigurationError(
-            u'If you decide to only register by \'name\', a name must '
-            u'be given.')
+            "If you decide to only register by 'name', a name must " "be given."
+        )
 
     # Instantiate the real factory if it's the schema-aware type. We do
     # this here so that the for_ interface may take this into account.
     if factory is not None and ISchemaAwareFactory.providedBy(factory):
         factory = factory(provides)
 
     # the behavior registration hold all information about the behavior.
@@ -164,16 +169,17 @@
             name=name,
             component=registration,
         )
 
     if factory is None:
         if for_ is not None:
             logger.warn(
-                u'Specifying \'for\' in behavior \'{0}\' if no \'factory\' is '
-                u'given has no effect and is superfluous.'.format(title))
+                "Specifying 'for' in behavior '{}' if no 'factory' is "
+                "given has no effect and is superfluous.".format(title)
+            )
         # w/o factory we're done here: schema only behavior
         return
 
     if for_ is None:
         for_ = _detect_for(factory, marker)
 
     adapter_factory = BehaviorAdapterFactory(registration)
```

### Comparing `plone.behavior-1.4.0/plone/behavior/tests.py` & `plone.behavior-2.0.0/plone/behavior/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-# -*- coding: utf-8 -*-
-from __future__ import print_function
 from zope import schema
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 import doctest
-import re
-import sys
 import unittest
 import zope.component.testing
 
 
 # Simple adapter behavior - no context restrictions
 class IAdapterBehavior(Interface):
     pass
 
 
 @implementer(IAdapterBehavior)
-class AdapterBehavior(object):
+class AdapterBehavior:
     def __init__(self, context):
         self.context = context
 
 
 # Simple adapter behavior that used to have a different name
 class IRenamedAdapterBehavior(Interface):
     pass
 
 
 @implementer(IRenamedAdapterBehavior)
-class RenamedAdapterBehavior(object):
+class RenamedAdapterBehavior:
     def __init__(self, context):
         self.context = context
 
 
 # Adapter behavior with explicit context restriction
 class IRestrictedAdapterBehavior(Interface):
     pass
 
 
 @implementer(IRestrictedAdapterBehavior)
-class RestrictedAdapterBehavior(object):
+class RestrictedAdapterBehavior:
     def __init__(self, context):
         self.context = context
 
 
 class IMinimalContextRequirements(Interface):
     pass
 
@@ -56,16 +52,15 @@
 
 class ISomeContext(Interface):
     pass
 
 
 @implementer(IImpliedRestrictionAdapterBehavior)
 @adapter(ISomeContext)
-class ImpliedRestrictionAdapterBehavior(object):
-
+class ImpliedRestrictionAdapterBehavior:
     def __init__(self, context):
         self.context = context
 
 
 # Behavior with marker
 class IMarkerBehavior(Interface):
     pass
@@ -74,15 +69,15 @@
 # Behavior to be registered with name only
 class INameOnlyBehavior(Interface):
     pass
 
 
 # For test of the annotation factory
 class IAnnotationStored(Interface):
-    some_field = schema.TextLine(title=u'Some field', default=u'default value')
+    some_field = schema.TextLine(title="Some field", default="default value")
 
 
 # Behavior and marker
 class IMarkerAndAdapterBehavior(Interface):
     pass
 
 
@@ -94,48 +89,35 @@
     pass
 
 
 class IMarkerAndAdapterMarker2(Interface):
     pass
 
 
-class DummyBehaviorImpl(object):
-
+class DummyBehaviorImpl:
     def __init__(self, context):
         self.context = context
 
 
-class Py23DocChecker(doctest.OutputChecker):
-    def check_output(self, want, got, optionflags):
-        if sys.version_info[0] > 2:
-            want = re.sub("u'(.*?)'", "'\\1'", want)
-            want = re.sub('u"(.*?)"', '"\\1"', want)
-            got = re.sub(
-                'plone.behavior.registration.BehaviorRegistrationNotFound',
-                'BehaviorRegistrationNotFound', got)
-        return doctest.OutputChecker.check_output(self, want, got, optionflags)
-
-
 def test_suite():
-    return unittest.TestSuite((
-
-        doctest.DocFileSuite(
-            'behaviors.rst',
-            tearDown=zope.component.testing.tearDown,
-            globs={
-                'print_function': print_function,
-            },
-            checker=Py23DocChecker(),
-        ),
-        doctest.DocFileSuite(
-            'directives.rst',
-            setUp=zope.component.testing.setUp,
-            tearDown=zope.component.testing.tearDown,
-            checker=Py23DocChecker(),
-        ),
-        doctest.DocFileSuite(
-            'annotation.rst',
-            setUp=zope.component.testing.setUp,
-            tearDown=zope.component.testing.tearDown,
-            checker=Py23DocChecker(),
-        ),
-    ))
+    return unittest.TestSuite(
+        (
+            doctest.DocFileSuite(
+                "behaviors.rst",
+                setUp=zope.component.testing.setUp,
+                tearDown=zope.component.testing.tearDown,
+                globs={
+                    "print_function": print,
+                },
+            ),
+            doctest.DocFileSuite(
+                "directives.rst",
+                setUp=zope.component.testing.setUp,
+                tearDown=zope.component.testing.tearDown,
+            ),
+            doctest.DocFileSuite(
+                "annotation.rst",
+                setUp=zope.component.testing.setUp,
+                tearDown=zope.component.testing.tearDown,
+            ),
+        )
+    )
```

### Comparing `plone.behavior-1.4.0/README.rst` & `plone.behavior-2.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 ``provides``
     An interface to which the behavior can be adapted.
     This is what the conditional adapter factory will be registered as providing (required).
 
 ``name``
     Convenience lookup name for this behavior (optional).
     The behavior will be always registered under the dotted name of ``provides`` attribute.
-    This are usally long names. ``name`` is a short name for this.
+    This are usually long names. ``name`` is a short name for this.
     If ``name`` is given the behavior is registered additional under it.
     Anyway using short namespaces in ``name`` is recommended.
 
 ``name_only``
     If set to ``yes`` or ``true`` the behavior is registered only under the given name,
     but not under the dotted path of the ``provides`` interface.
     This makes ``name`` mandatory.
@@ -185,21 +185,21 @@
 
 
 ZCML Examples
 -------------
 
 Example usage, given
 
-- some ``context`` (some arbitary object) which is ``IBehaviorAssignable``,
-- an ``IMyBehavior`` interface intented to be used as ``provides``,
-- an ``IMyMarker`` interface intented to be used as ``marker``,
+- some ``context`` (some arbitrary object) which is ``IBehaviorAssignable``,
+- an ``IMyBehavior`` interface intended to be used as ``provides``,
+- an ``IMyMarker`` interface intended to be used as ``marker``,
 - a ``MyFactory`` class implementing ``IMyBehavior`` ,
 - a ``MySchemaAwareFactory`` class implementing ``IMyBehavior`` and ``plone.behavior.interfaces.ISchemaAwareFactory``,
-- an ``IMyType`` intented to be used as ``for``.
-- some ``typed_context`` (some arbitary object) which is ``IBehaviorAssignable`` and provides ``IMyType``,
+- an ``IMyType`` intended to be used as ``for``.
+- some ``typed_context`` (some arbitrary object) which is ``IBehaviorAssignable`` and provides ``IMyType``,
 - an ``MyTypedFactory`` class implementing ``IMyBehavior`` and adapting ``IMyType``,
 
 ``title`` and ``description`` is trivial, so we dont cover it here in the explanantion.
 We dont cover ``name`` too, because it's not having any effect in this usage.
 To simplify it, we assume ``context`` ``IBehaviorAssignable`` always supports the behavior.
 Also for simplifications sake we assume some magic applies the marker interface to ``context``
 I.e. both is done by ``plone.dexterity``.
@@ -216,15 +216,15 @@
 - ``context`` provides ``IBehavior``,
 
 **Example 2** - also ``factory`` is given, so ``marker`` is required:
 
 .. warning::
    Using the same Interface as marker and behavior works, but is not recommended and will be deprecated in future.
    It is semantically wrong!
-   
+
    Go for Example 3 instead!
 
 ::
 
     <plone:behavior
         title="Example 1"
         provides="IMyBehavior"
```

### Comparing `plone.behavior-1.4.0/CHANGES.rst` & `plone.behavior-2.0.0/CHANGES.rst`

 * *Files 4% similar despite different names*

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
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a9dd65cc)
+
+
 1.4.0 (2020-09-07)
 ------------------
 
 New features:
 
 
 - Drop Plone 4.3 support.
@@ -46,15 +63,15 @@
 1.3.0 (2019-02-13)
 ------------------
 
 New features:
 
 
 - New option ``former_dotted_names`` that allows to register the former name
-  under which a behavior used to be registerd. This can be useful to ensure a
+  under which a behavior used to be registered. This can be useful to ensure a
   smooth transition in case a behavior's dotted name is changed. [pysailor]
   (#18)
 
 
 1.2.1 (2018-01-17)
 ------------------
```

