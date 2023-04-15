# Comparing `tmp/plone.protect-4.1.8.tar.gz` & `tmp/plone.protect-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.protect-4.1.8.tar", last modified: Fri Dec 16 10:24:46 2022, max compression
+gzip compressed data, was "plone.protect-5.0.0.tar", last modified: Sat Apr 15 08:11:10 2023, max compression
```

## Comparing `plone.protect-4.1.8.tar` & `plone.protect-5.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.408688 plone.protect-4.1.8/
--rw-r--r--   0 maurits    (501) staff       (20)    10853 2022-12-16 10:24:45.000000 plone.protect-4.1.8/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-12-16 10:24:45.000000 plone.protect-4.1.8/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      163 2022-12-16 10:24:45.000000 plone.protect-4.1.8/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    20580 2022-12-16 10:24:46.408831 plone.protect-4.1.8/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     8527 2022-12-16 10:24:45.000000 plone.protect-4.1.8/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)       93 2022-12-16 10:24:45.000000 plone.protect-4.1.8/TODO.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.398851 plone.protect-4.1.8/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1481 2022-12-16 10:24:45.000000 plone.protect-4.1.8/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.399153 plone.protect-4.1.8/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.405283 plone.protect-4.1.8/plone/protect/
--rw-r--r--   0 maurits    (501) staff       (20)      302 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3727 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/authenticator.py
--rw-r--r--   0 maurits    (501) staff       (20)    14400 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/auto.py
--rw-r--r--   0 maurits    (501) staff       (20)     2016 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1833 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/confirm.pt
--rw-r--r--   0 maurits    (501) staff       (20)      561 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2027 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/monkey.py
--rw-r--r--   0 maurits    (501) staff       (20)      287 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/postonly.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.395999 plone.protect-4.1.8/plone/protect/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.405572 plone.protect-4.1.8/plone/protect/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      181 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2896 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/protect.js
--rw-r--r--   0 maurits    (501) staff       (20)     1950 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2538 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.408441 plone.protect-4.1.8/plone/protect/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       24 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1276 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/case.py
--rw-r--r--   0 maurits    (501) staff       (20)      495 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/test.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4907 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/testAuthenticator.py
--rw-r--r--   0 maurits    (501) staff       (20)     8427 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/testAuto.py
--rw-r--r--   0 maurits    (501) staff       (20)     1358 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/testPatches.py
--rw-r--r--   0 maurits    (501) staff       (20)      902 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/testPostOnly.py
--rw-r--r--   0 maurits    (501) staff       (20)     2356 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/testUtils.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/tests/test_confirm_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     4854 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      620 2022-12-16 10:24:45.000000 plone.protect-4.1.8/plone/protect/views.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-12-16 10:24:46.401280 plone.protect-4.1.8/plone.protect.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    20580 2022-12-16 10:24:46.000000 plone.protect-4.1.8/plone.protect.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1083 2022-12-16 10:24:46.000000 plone.protect-4.1.8/plone.protect.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-12-16 10:24:46.000000 plone.protect-4.1.8/plone.protect.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-12-16 10:24:46.000000 plone.protect-4.1.8/plone.protect.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-12-16 10:24:46.000000 plone.protect-4.1.8/plone.protect.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      227 2022-12-16 10:24:46.000000 plone.protect-4.1.8/plone.protect.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-12-16 10:24:46.000000 plone.protect-4.1.8/plone.protect.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-12-16 10:24:45.000000 plone.protect-4.1.8/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2022-12-16 10:24:46.409289 plone.protect-4.1.8/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2034 2022-12-16 10:24:45.000000 plone.protect-4.1.8/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.284520 plone.protect-5.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)    11141 2023-04-15 08:11:09.000000 plone.protect-5.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:11:09.000000 plone.protect-5.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      163 2023-04-15 08:11:09.000000 plone.protect-5.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    20562 2023-04-15 08:11:10.284520 plone.protect-5.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     8527 2023-04-15 08:11:09.000000 plone.protect-5.0.0/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       93 2023-04-15 08:11:09.000000 plone.protect-5.0.0/TODO.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.281520 plone.protect-5.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1481 2023-04-15 08:11:09.000000 plone.protect-5.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.281520 plone.protect-5.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.283520 plone.protect-5.0.0/plone/protect/
+-rw-r--r--   0 gil       (1000) gil       (1000)      278 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3517 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/authenticator.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14289 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/auto.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1946 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2211 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/confirm.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      536 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2023 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/monkey.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      263 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/postonly.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.280520 plone.protect-5.0.0/plone/protect/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.283520 plone.protect-5.0.0/plone/protect/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)      181 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2896 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/protect.js
+-rw-r--r--   0 gil       (1000) gil       (1000)     1846 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/subscribers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2487 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.284520 plone.protect-5.0.0/plone/protect/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1201 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/case.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      532 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/test.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     4801 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/testAuthenticator.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8404 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/testAuto.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1271 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/testPatches.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      806 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/testPostOnly.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2301 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/testUtils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      824 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/tests/test_confirm_view.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4822 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      586 2023-04-15 08:11:09.000000 plone.protect-5.0.0/plone/protect/views.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:11:10.282520 plone.protect-5.0.0/plone.protect.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    20562 2023-04-15 08:11:10.000000 plone.protect-5.0.0/plone.protect.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     1083 2023-04-15 08:11:10.000000 plone.protect-5.0.0/plone.protect.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:11:10.000000 plone.protect-5.0.0/plone.protect.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:11:10.000000 plone.protect-5.0.0/plone.protect.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:11:10.000000 plone.protect-5.0.0/plone.protect.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      245 2023-04-15 08:11:10.000000 plone.protect-5.0.0/plone.protect.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:11:10.000000 plone.protect-5.0.0/plone.protect.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2903 2023-04-15 08:11:09.000000 plone.protect-5.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      269 2023-04-15 08:11:10.285520 plone.protect-5.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1728 2023-04-15 08:11:09.000000 plone.protect-5.0.0/setup.py
```

### Comparing `plone.protect-4.1.8/CHANGES.rst` & `plone.protect-5.0.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,44 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-4.1.8 (2022-12-16)
+5.0.0 (2023-04-15)
 ------------------
 
+New features:
+
+
+- Drop support for Python <3.8. (5390ebc6)
+
+
 Bug fixes:
 
 
+- Do not hard-depend on `plone.portlets`.
+  Prepare for Plone with portlets optional.
+  @jensens (#99)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a9dd65cc)
+
+
+4.1.8 (2022-12-16)
+------------------
+
+
+Bug fixes:
+
 - Testing: explicitly set response content type header to html.  [jeromeperrin] (#97)
 
 
 4.1.7 (2022-12-02)
 ------------------
 
 Bug fixes:
```

### Comparing `plone.protect-4.1.8/PKG-INFO` & `plone.protect-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.protect
-Version: 4.1.8
+Version: 5.0.0
 Summary: Security for browser forms
 Home-page: https://github.com/plone/plone.protect
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: zope security CSRF
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
-Classifier: Framework :: Zope :: 2
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 This package contains utilities that can help protect parts of Plone
 or applications build on top of the Plone framework.
@@ -320,20 +314,44 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-4.1.8 (2022-12-16)
+5.0.0 (2023-04-15)
 ------------------
 
+New features:
+
+
+- Drop support for Python <3.8. (5390ebc6)
+
+
 Bug fixes:
 
 
+- Do not hard-depend on `plone.portlets`.
+  Prepare for Plone with portlets optional.
+  @jensens (#99)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a9dd65cc)
+
+
+4.1.8 (2022-12-16)
+------------------
+
+
+Bug fixes:
+
 - Testing: explicitly set response content type header to html.  [jeromeperrin] (#97)
 
 
 4.1.7 (2022-12-02)
 ------------------
 
 Bug fixes:
```

### Comparing `plone.protect-4.1.8/README.rst` & `plone.protect-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.protect-4.1.8/docs/LICENSE.txt` & `plone.protect-5.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.protect-4.1.8/plone/protect/authenticator.py` & `plone.protect-5.0.0/plone/protect/authenticator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-# -*- coding: utf-8 -*-
 from AccessControl import getSecurityManager
+from hashlib import sha1 as sha
 from plone.keyring.interfaces import IKeyManager
 from plone.protect.interfaces import IAuthenticatorView
 from Products.Five import BrowserView
 from zExceptions import Forbidden
 from zope.component import getUtility
 from zope.interface import implementer
 from ZPublisher.HTTPRequest import HTTPRequest
 
 import hmac
-import six
-
-
-try:
-    from hashlib import sha1 as sha
-except ImportError:
-    import sha
 
 
 ANONYMOUS_USER = "Anonymous User"
 
 
 def isAnonymousUser(user):
     return user is None or user.getUserName() == ANONYMOUS_USER
@@ -32,105 +25,102 @@
     return user.getUserName()
 
 
 def _is_equal(val1, val2):
     """
     constant time comparison
     """
-    if not isinstance(val1, six.string_types) or not isinstance(val2, six.string_types):
+    if not isinstance(val1, str) or not isinstance(val2, str):
         return False
     if len(val1) != len(val2):
         return False
     result = 0
     for x, y in zip(val1, val2):
         result |= ord(x) ^ ord(y)
     return result == 0
 
 
 def _getKeyring(username, manager=None):
     if manager is None:
         manager = getUtility(IKeyManager)
     if username == ANONYMOUS_USER:
         try:
-            ring = manager[u'_anon']
+            ring = manager["_anon"]
         except KeyError:
             # no anonymous key defined.
             # XXX should we even bother allowing to verify?
-            ring = manager[u'_system']
+            ring = manager["_system"]
     else:
         try:
-            ring = manager[u"_forms"]
+            ring = manager["_forms"]
         except KeyError:
-            ring = manager[u'_system']
+            ring = manager["_system"]
     return ring
 
 
-def _verify_request(request, extra='', name='_authenticator', manager=None):
+def _verify_request(request, extra="", name="_authenticator", manager=None):
     auth = request.get(name)
     if auth is None:
-        auth = request.getHeader('X-CSRF-TOKEN')
+        auth = request.getHeader("X-CSRF-TOKEN")
         if auth is None:
             return False
     if isinstance(auth, list):
         # in case 2 auth attributes were added to form. It can happen
         auth = auth[0]
 
     user = _getUserName()
     ring = _getKeyring(user, manager=manager)
 
-    if six.PY3:
-        user = user.encode('utf-8')
-        extra = extra.encode('utf-8')
+    user = user.encode("utf-8")
+    extra = extra.encode("utf-8")
 
     for key in ring:
         if key is None:
             continue
-        correct = hmac.new(key.encode('utf-8'), user + extra, sha).hexdigest()
+        correct = hmac.new(key.encode("utf-8"), user + extra, sha).hexdigest()
         if _is_equal(correct, auth):
             return True
 
     return False
 
+
 # We had to rename because previous hotfixes patched _verify
 _verify = _verify_request
 
 
-def createToken(extra='', manager=None):
+def createToken(extra="", manager=None):
     user = _getUserName()
     ring = _getKeyring(user, manager=manager)
     secret = ring.random()
-    if six.PY3:
-        secret = secret.encode('utf-8')
-        user = user.encode('utf-8')
-        extra = extra.encode('utf-8')
+    secret = secret.encode("utf-8")
+    user = user.encode("utf-8")
+    extra = extra.encode("utf-8")
     return hmac.new(secret, user + extra, sha).hexdigest()
 
 
 @implementer(IAuthenticatorView)
 class AuthenticatorView(BrowserView):
-
-    def token(self, extra=''):
+    def token(self, extra=""):
         return createToken(extra)
 
-    def authenticator(self, extra='', name='_authenticator'):
+    def authenticator(self, extra="", name="_authenticator"):
         auth = createToken(extra)
-        return '<input type="hidden" name="%s" value="%s"/>' % (name, auth)
+        return f'<input type="hidden" name="{name}" value="{auth}"/>'
 
-    def verify(self, extra='', name="_authenticator"):
+    def verify(self, extra="", name="_authenticator"):
         return _verify_request(self.request, extra=extra, name=name)
 
 
-def check(request, extra='', name="_authenticator", manager=None):
+def check(request, extra="", name="_authenticator", manager=None):
     if isinstance(request, HTTPRequest):
-        if not _verify_request(request, extra=extra,
-                               name=name, manager=manager):
-            raise Forbidden('Form authenticator is invalid.')
+        if not _verify_request(request, extra=extra, name=name, manager=manager):
+            raise Forbidden("Form authenticator is invalid.")
 
 
-def CustomCheckAuthenticator(extra='', name='_authenticator'):
+def CustomCheckAuthenticator(extra="", name="_authenticator"):
     def _check(request):
         return check(request, extra=extra, name=name)
+
     return _check
 
 
-__all__ = ["AuthenticatorView", "check", "createToken",
-           "CustomCheckAuthenticator"]
+__all__ = ["AuthenticatorView", "check", "createToken", "CustomCheckAuthenticator"]
```

### Comparing `plone.protect-4.1.8/plone/protect/auto.py` & `plone.protect-5.0.0/plone/protect/auto.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,96 +1,85 @@
-# -*- coding: utf-8 -*-
 from AccessControl import getSecurityManager
 from Acquisition import aq_parent
 from BTrees.OOBTree import OOBTree
 from lxml import etree
 from lxml import html
 from plone.keyring.interfaces import IKeyManager
-from plone.portlets.interfaces import IPortletAssignment
 from plone.protect.authenticator import check
 from plone.protect.authenticator import createToken
 from plone.protect.authenticator import isAnonymousUser
 from plone.protect.interfaces import IConfirmView
 from plone.protect.interfaces import IDisableCSRFProtection
 from plone.protect.utils import getRoot
 from plone.protect.utils import getRootKeyManager
 from plone.protect.utils import SAFE_WRITE_KEY
 from plone.protect.utils import safeWrite  # noqa b/w compat import
+from plone.scale.storage import ScalesDict
 from plone.transformchain.interfaces import ITransform
 from Products.CMFCore.utils import getToolByName
 from repoze.xmliter.serializer import XMLSerializer
 from repoze.xmliter.utils import getHTMLSerializer
-from six.moves.urllib.parse import urlencode
-from six.moves.urllib.parse import urlparse
+from urllib.parse import urlencode
+from urllib.parse import urlparse
 from zExceptions import Forbidden
-from zope.component import adapts
+from zope.component import adapter
 from zope.component import ComponentLookupError
 from zope.component import getUtility
+from zope.component.hooks import getSite
 from zope.interface import implementer
 from zope.interface import Interface
 
 import itertools
 import logging
 import os
-import pkg_resources
-import six
 import traceback
 import transaction
 import types
 
 
+# do not hard depend here on plone.portlets (for Plone 7)
 try:
-    from zope.component.hooks import getSite
-except:
-    from zope.app.component.hooks import getSite
-
-try:
-    pkg_resources.get_distribution('plone.app.blob')
-except pkg_resources.DistributionNotFound:
-    ATBlob = None
-else:
-    from plone.app.blob.content import ATBlob
-
-try:
-    from plone.scale.storage import ScalesDict
+    from plone.portlets.interfaces import IPortletAssignment
 except ImportError:
-    ScalesDict = None
+    IPortletAssignment = None
 
+logger = logging.getLogger("plone.protect")
 
-logger = logging.getLogger('plone.protect')
-
-X_FRAME_OPTIONS = os.environ.get('PLONE_X_FRAME_OPTIONS', 'SAMEORIGIN')
-CSRF_DISABLED = os.environ.get('PLONE_CSRF_DISABLED', 'false').lower() in \
-    ('true', 't', 'yes', 'y', '1')
+X_FRAME_OPTIONS = os.environ.get("PLONE_X_FRAME_OPTIONS", "SAMEORIGIN")
+CSRF_DISABLED = os.environ.get("PLONE_CSRF_DISABLED", "false").lower() in (
+    "true",
+    "t",
+    "yes",
+    "y",
+    "1",
+)
 ANNOTATION_KEYS = (
-    'plone.contentrules.localassignments',
-    'syndication_settings',
-    'plone.portlets.contextassignments',
-    'plone.scale',
+    "plone.contentrules.localassignments",
+    "syndication_settings",
+    "plone.portlets.contextassignments",
+    "plone.scale",
 )
-SAFE_TYPES = tuple(t for t in [ATBlob, ScalesDict] if t is not None)
+SAFE_TYPES = (ScalesDict,)
 
 
 @implementer(ITransform)
-class ProtectTransform(object):
+@adapter(Interface, Interface)  # any context, any request
+class ProtectTransform:
     """
     XXX Need to be extremely careful with everything we do in here
     since an error here would mean the transform is skipped
     and no CSRF protection...
     """
-    adapts(Interface, Interface)  # any context, any request
 
     # should be last lxml related transform
     order = 9000
 
     key_manager = None
     site = None
-    safe_views = (
-        'plone_lock_operations',
-    )
+    safe_views = ("plone_lock_operations",)
 
     def __init__(self, published, request):
         self.published = published
         self.request = request
 
     def parseTree(self, result, encoding):
         # if it's a redirect, the result shall not be transformed
@@ -100,82 +89,82 @@
             return None
 
         if isinstance(result, XMLSerializer):
             return result
 
         # hhmmm, this is kind of taken right out of plone.app.theming
         # maybe this logic(parsing dom) should be someone central?
-        contentType = self.request.response.getHeader('Content-Type')
-        if contentType is None or not contentType.startswith('text/html'):
+        contentType = self.request.response.getHeader("Content-Type")
+        if contentType is None or not contentType.startswith("text/html"):
             return None
 
-        contentEncoding = self.request.response.getHeader('Content-Encoding')
-        if contentEncoding and contentEncoding in ('zip', 'deflate',
-                                                   'compress',):
+        contentEncoding = self.request.response.getHeader("Content-Encoding")
+        if contentEncoding and contentEncoding in (
+            "zip",
+            "deflate",
+            "compress",
+        ):
             return None
 
         if isinstance(result, list) and len(result) == 1:
             # do not parse empty strings to omit warning log message
             if not result[0].strip():
                 return None
         try:
-            result = getHTMLSerializer(
-                result, pretty_print=False, encoding=encoding)
+            result = getHTMLSerializer(result, pretty_print=False, encoding=encoding)
             # We are going to force html output here always as XHTML
             # output does odd character encodings
             result.serializer = html.tostring
             return result
         except (AttributeError, TypeError, etree.ParseError):
             # XXX handle something special?
-            logger.warn('error parsing dom, failure to add csrf '
-                        'token to response for url %s' % self.request.URL)
+            logger.warn(
+                "error parsing dom, failure to add csrf "
+                "token to response for url %s" % self.request.URL
+            )
             return None
 
     def transformBytes(self, result, encoding):
-        result = result.decode(encoding, 'ignore')
+        result = result.decode(encoding, "ignore")
         return self.transformIterable([result], encoding)
 
     def transformString(self, result, encoding):
         return self.transformIterable([result], encoding)
 
     def transformUnicode(self, result, encoding):
         return self.transformIterable([result], encoding)
 
     def transformIterable(self, result, encoding):
-        """Apply the transform if required
-        """
+        """Apply the transform if required"""
         # before anything, do the clickjacking protection
-        if (
-            X_FRAME_OPTIONS and
-            not self.request.response.getHeader('X-Frame-Options')
-        ):
-            self.request.response.setHeader('X-Frame-Options', X_FRAME_OPTIONS)
+        if X_FRAME_OPTIONS and not self.request.response.getHeader("X-Frame-Options"):
+            self.request.response.setHeader("X-Frame-Options", X_FRAME_OPTIONS)
 
         if CSRF_DISABLED:
             return
 
         # only auto CSRF protect authenticated users
         if isAnonymousUser(getSecurityManager().getUser()):
             return
 
         # if on confirm view, do not check, just abort and
         # immediately transform without csrf checking again
-        if IConfirmView.providedBy(self.request.get('PUBLISHED')):
+        if IConfirmView.providedBy(self.request.get("PUBLISHED")):
             # abort it, show the confirmation...
             transaction.abort()
             return self.transform(result, encoding)
 
         # next, check if we're a resource not connected
         # to a ZODB object--no context
         context = self.getContext()
         if not context:
             return
 
         try:
-            tool = getToolByName(context, 'portal_url', None)
+            tool = getToolByName(context, "portal_url", None)
             if tool:
                 self.site = tool.getPortalObject()
         except TypeError:
             self.site = getSite()
 
         try:
             self.key_manager = getUtility(IKeyManager)
@@ -192,15 +181,15 @@
             # we don't need to transform the doc, we're getting redirected
             return
 
         # finally, let's run the transform
         return self.transform(result, encoding)
 
     def getContext(self):
-        published = self.request.get('PUBLISHED')
+        published = self.request.get("PUBLISHED")
         if isinstance(published, types.MethodType):
             return published.__self__
         return aq_parent(published)
 
     def getViewName(self):
         try:
             return self.getContext().__name__
@@ -210,62 +199,71 @@
     def check(self):
         """
         just being very careful here about our check so we don't
         cause errors that prevent this check from happening
         """
         try:
             return self._check()
-        except:
+        except Exception:
             transaction.abort()
-            logger.error("Error checking for CSRF. "
-                         "Transaction will be aborted since the request "
-                         "is now unsafe:\n%s" % (
-                             traceback.format_exc()))
+            logger.error(
+                "Error checking for CSRF. "
+                "Transaction will be aborted since the request "
+                "is now unsafe:\n%s" % (traceback.format_exc())
+            )
             raise
 
     def _registered_objects(self):
         app = self.request.PARENTS[-1]
-        return list(itertools.chain.from_iterable([
-            conn._registered_objects
-            # skip the 'temporary' connection since it stores session objects
-            # which get written all the time
-            for name, conn in app._p_jar.connections.items()
-            if name != 'temporary'
-        ]))
+        return list(
+            itertools.chain.from_iterable(
+                [
+                    conn._registered_objects
+                    # skip the 'temporary' connection since it stores session objects
+                    # which get written all the time
+                    for name, conn in app._p_jar.connections.items()
+                    if name != "temporary"
+                ]
+            )
+        )
 
     def _check(self):
         registered = self._registered_objects()
-        if len(registered) > 0 and \
-                not IDisableCSRFProtection.providedBy(self.request):
+        if len(registered) > 0 and not IDisableCSRFProtection.providedBy(self.request):
             if self.getViewName() in self.safe_views:
                 return True
             # Okay, we're writing here, we need to protect!
             try:
                 check(self.request, manager=self.key_manager)
                 return True
             except ComponentLookupError:
-                logger.info('Can not find key manager for CSRF protection. '
-                            'This should not happen.')
+                logger.info(
+                    "Can not find key manager for CSRF protection. "
+                    "This should not happen."
+                )
                 raise
             except Forbidden:
                 # XXX
                 # okay, so right now, we're going to check if the current
                 # registered objects to write, are just portlet assignments.
                 # I don't know why, but when a site is created, these
                 # cause some writes on read. ALL, registered objects
                 # need to be portlet assignments. XXX needs to be fixed
                 # somehow...
                 safe_oids = []
-                if SAFE_WRITE_KEY in getattr(self.request, 'environ', {}):
+                if SAFE_WRITE_KEY in getattr(self.request, "environ", {}):
                     safe_oids = self.request.environ[SAFE_WRITE_KEY]
                 safe = True
                 for obj in registered:
-                    if IPortletAssignment.providedBy(obj):
+                    if (
+                        IPortletAssignment is not None
+                        and IPortletAssignment.providedBy(obj)
+                    ):
                         continue
-                    if getattr(obj, '_p_oid', False) in safe_oids:
+                    if getattr(obj, "_p_oid", False) in safe_oids:
                         continue
                     if SAFE_TYPES and isinstance(obj, SAFE_TYPES):
                         continue
                     if isinstance(obj, OOBTree):
                         safe = False
                         for key in ANNOTATION_KEYS:
                             try:
@@ -275,109 +273,108 @@
                             except TypeError:
                                 pass
                         if safe:
                             continue
                     safe = False
                     break
                 if not safe:
-                    if self.request.REQUEST_METHOD != 'GET':
+                    if self.request.REQUEST_METHOD != "GET":
                         # only try to be "smart" with GET requests
                         raise
                     logger.info(
-                        '{0:s}\naborting transaction due to no CSRF '
-                        'protection on url {1:s}'.format(
-                            '\n'.join(traceback.format_stack()),
-                            self.request.URL
+                        "{:s}\naborting transaction due to no CSRF "
+                        "protection on url {:s}".format(
+                            "\n".join(traceback.format_stack()), self.request.URL
                         )
                     )
                     transaction.abort()
 
                     # conditions for doing the confirm form are:
                     #   1. 301, 302 response code
                     #   2. text/html response
                     #   3. getSite could be none, zope root maybe, carry on
                     # otherwise,
                     #   just abort with a log entry because we tried to
                     #   write on read, without a POST request and we don't
                     #   know what to do with it gracefully.
                     resp = self.request.response
-                    ct = resp.getHeader('Content-Type', '') or ''
-                    if self.site and (
-                            resp.status in (301, 302) or 'text/html' in ct):
+                    ct = resp.getHeader("Content-Type", "") or ""
+                    if self.site and (resp.status in (301, 302) or "text/html" in ct):
                         data = self.request.form.copy()
-                        data['original_url'] = self.request.URL
-                        resp.redirect('%s/@@confirm-action?%s' % (
-                            self.site.absolute_url(),
-                            urlencode(data)
-                        ))
+                        data["original_url"] = self.request.URL
+                        resp.redirect(
+                            "{}/@@confirm-action?{}".format(
+                                self.site.absolute_url(), urlencode(data)
+                            )
+                        )
                         return False
         return True
 
     def isActionInSite(self, action, current_url):
         # sanitize url
         url = urlparse(action)
         if not url.hostname:
             # no hostname means this is relative
             return True
         if url.hostname != current_url.hostname:
             return False
         return True
 
     def transform(self, result, encoding):
-
         result = self.parseTree(result, encoding)
         if result is None:
             return None
         root = result.tree.getroot()
         url = urlparse(self.request.URL)
         try:
             token = createToken(manager=self.key_manager)
         except ComponentLookupError:
             if self.site is not None:
                 logger.warn(
-                    'Keyring not found on site. This should not happen',
-                    exc_info=True
+                    "Keyring not found on site. This should not happen", exc_info=True
                 )
             return result
 
-        for form in root.cssselect('form'):
+        for form in root.cssselect("form"):
             # XXX should we only do POST? If we're logged in and
             # it's an internal form, I'm inclined to say no...
             # method = form.attrib.get('method', 'GET').lower()
             # if method != 'post':
             #    continue
 
             # some get forms we definitely do not want to protect.
             # for now, we know search we do not want to protect
-            method = form.attrib.get('method', 'GET').lower()
-            action = form.attrib.get('action', '').strip()
-            if method == 'get' and '@@search' in action:
+            method = form.attrib.get("method", "GET").lower()
+            action = form.attrib.get("action", "").strip()
+            if method == "get" and "@@search" in action:
                 continue
-            action = form.attrib.get('action', '').strip()
+            action = form.attrib.get("action", "").strip()
             if not self.isActionInSite(action, url):
                 continue
             # check if the token is already on the form..
             hidden = form.cssselect('[name="_authenticator"]')
             if len(hidden) == 0:
                 hidden = etree.Element("input")
-                hidden.attrib['name'] = '_authenticator'
-                hidden.attrib['type'] = 'hidden'
-                hidden.attrib['value'] = token
+                hidden.attrib["name"] = "_authenticator"
+                hidden.attrib["type"] = "hidden"
+                hidden.attrib["value"] = token
                 form.append(hidden)
 
-        if self.site is not None and not root.cssselect('#protect-script'):
+        if self.site is not None and not root.cssselect("#protect-script"):
             # Alternative: add this in the resource registry.
             site_url = self.site.absolute_url()
-            elements = root.cssselect('body')
+            elements = root.cssselect("body")
             if len(elements):
                 body = elements[0]
                 protect_script = etree.Element("script")
-                protect_script.attrib.update({
-                    'type': "application/javascript",
-                    'src': "%s/++resource++protect.js" % site_url,
-                    'data-site-url': site_url,
-                    'data-token': token,
-                    'id': 'protect-script'
-                })
+                protect_script.attrib.update(
+                    {
+                        "type": "application/javascript",
+                        "src": "%s/++resource++protect.js" % site_url,
+                        "data-site-url": site_url,
+                        "data-token": token,
+                        "id": "protect-script",
+                    }
+                )
                 body.append(protect_script)
 
         return result
```

### Comparing `plone.protect-4.1.8/plone/protect/configure.zcml` & `plone.protect-5.0.0/plone/protect/configure.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:zcml="http://namespaces.zope.org/zcml"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:monkey="http://namespaces.plone.org/monkey"
-    i18n_domain="plone">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone"
+    >
+
+  <include
+      package="AccessControl"
+      zcml:condition="installed AccessControl.rolemanager"
+      />
+  <include package="plone.keyring" />
+  <include package="plone.transformchain" />
+
+  <browser:page
+      name="authenticator"
+      for="*"
+      class=".authenticator.AuthenticatorView"
+      allowed_interface=".interfaces.IAuthenticatorView"
+      permission="zope.Public"
+      />
+
+  <genericsetup:registerProfile
+      name="default"
+      title="plone.protect configuration"
+      description="Local configuration for plone.protect"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      directory="profiles/default"
+      zcml:condition="installed Products.CMFCore"
+      />
+
+  <adapter
+      factory=".auto.ProtectTransform"
+      name="plone.protect.autocsrf"
+      />
+
+  <browser:resource
+      name="protect.js"
+      file="protect.js"
+      />
+
+  <browser:page
+      name="confirm-action"
+      for="*"
+      class=".views.ConfirmView"
+      template="confirm.pt"
+      permission="zope2.View"
+      />
+
+  <subscriber handler=".subscribers.onUserLogsIn" />
+
+  <include package="collective.monkeypatcher" />
+
+  <monkey:patch
+      original="wl_lockmapping"
+      replacement=".monkey.wl_lockmapping"
+      class="OFS.Lockable.LockableItem"
+      description="Special handling for write on read Zope2 locking issues"
+      preserveOriginal="True"
+      zcml:condition="installed OFS.Lockable"
+      />
+
+  <include
+      package="z3c.zcmlhook"
+      file="meta.zcml"
+      />
 
-    <include package="AccessControl"
-             zcml:condition="installed AccessControl.rolemanager" />
-    <include package="plone.keyring" />
-    <include package="plone.transformchain" />
-
-    <browser:page
-       for="*"
-       name="authenticator"
-       class=".authenticator.AuthenticatorView"
-       permission="zope.Public"
-       allowed_interface=".interfaces.IAuthenticatorView"
-       />
-
-    <genericsetup:registerProfile
-        zcml:condition="installed Products.CMFCore"
-        name="default"
-        directory="profiles/default"
-        title="plone.protect configuration"
-        description="Local configuration for plone.protect"
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        for="Products.CMFCore.interfaces.ISiteRoot"
-        />
-
-    <adapter
-        name="plone.protect.autocsrf"
-        factory=".auto.ProtectTransform"
-        />
-
-    <browser:resource
-        name="protect.js"
-        file="protect.js"
-        />
-
-    <browser:page
-        name="confirm-action"
-        for="*"
-        class=".views.ConfirmView"
-        template="confirm.pt"
-        permission="zope2.View"
-    />
-
-    <subscriber handler=".subscribers.onUserLogsIn" />
-
-    <include package="collective.monkeypatcher" />
-
-    <monkey:patch
-        zcml:condition="installed OFS.Lockable"
-        description="Special handling for write on read Zope2 locking issues"
-        class="OFS.Lockable.LockableItem"
-        original="wl_lockmapping"
-        replacement=".monkey.wl_lockmapping"
-        preserveOriginal="True"
-        />
-
-    <include package="z3c.zcmlhook" file="meta.zcml" />
-
-    <zcml:customAction
-        handler=".monkey.disable_zope_csrf_checks"
-        />
+  <zcml:customAction handler=".monkey.disable_zope_csrf_checks" />
 
 </configure>
```

### Comparing `plone.protect-4.1.8/plone/protect/confirm.pt` & `plone.protect-5.0.0/plone/protect/confirm.pt`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,73 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="context/main_template/macros/master"
-      i18n:domain="plone">
-
-<metal:block fill-slot="top_slot"
-             tal:define="dummy python:request.set('disable_border', 1)" />
-
-<body>
-  <metal:title fill-slot="content-title">
-     <h1 class="documentFirstHeading" i18n:translate="">
+      xml:lang="en"
+      i18n:domain="plone"
+>
+
+  <metal:block fill-slot="top_slot"
+               tal:define="
+                 dummy python:request.set('disable_border', 1);
+               "
+  />
+
+  <body>
+    <metal:title fill-slot="content-title">
+      <h1 class="documentFirstHeading"
+          i18n:translate=""
+      >
          Confirming User Action.
-     </h1>
-  </metal:title>
+      </h1>
+    </metal:title>
 
-  <metal:description fill-slot="content-description">
-     <div class="documentDescription" i18n:translate="">
+    <metal:description fill-slot="content-description">
+      <div class="documentDescription"
+           i18n:translate=""
+      >
          Confirm that you'd like to perform this action.
-     </div>
-  </metal:description>
+      </div>
+    </metal:description>
 
-  <metal:content-core fill-slot="content-core">
-    <metal:content-core define-macro="content-core">
-      <p class="discreet" i18n:translate="">
+    <metal:content-core fill-slot="content-core">
+      <metal:content-core define-macro="content-core">
+        <p class="discreet"
+           i18n:translate=""
+        >
         Careful, it's possible someone is executing an exploit against you.
         Verify you just performed an action on this site and that you were
         not referred here by a different website or email.
-      </p>
-      <form tal:attributes="action request/original_url;" method="GET">
-        <tal:values tal:repeat="key python: request.form.keys()">
-          <input type="hidden" tal:attributes="name key; value python: request.form[key]" />
-        </tal:values>
-        <dl>
-          <dt i18n:translate="">Original URL</dt>
-          <dd tal:content="request/original_url" />
-        </dl>
-        <div class="formControls">
-          <input type="submit" value="Confirm action" i18n:attributes="value"
-                 name="form.button.confirm" class="standalone" />
-        </div>
-      </form>
+        </p>
+        <form method="GET"
+              tal:attributes="
+                action request/original_url;
+              "
+        >
+          <tal:values tal:repeat="key python: request.form.keys()">
+            <input type="hidden"
+                   tal:attributes="
+                     name key;
+                     value python: request.form[key];
+                   "
+            />
+          </tal:values>
+          <dl>
+            <dt i18n:translate="">Original URL</dt>
+            <dd tal:content="request/original_url"></dd>
+          </dl>
+          <div class="formControls">
+            <input class="standalone"
+                   name="form.button.confirm"
+                   type="submit"
+                   value="Confirm action"
+                   i18n:attributes="value"
+            />
+          </div>
+        </form>
+      </metal:content-core>
     </metal:content-core>
-  </metal:content-core>
 
-</body>
+  </body>
 </html>
-
```

### Comparing `plone.protect-4.1.8/plone/protect/interfaces.py` & `plone.protect-5.0.0/plone/protect/interfaces.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Interface
 
 
 class IAuthenticatorView(Interface):
-
     def token():
         """return token value"""
 
     def authenticator():
         """Return an xhtml snippet which sets an authenticator.
 
         This must be included inside a <form> element.
```

### Comparing `plone.protect-4.1.8/plone/protect/monkey.py` & `plone.protect-5.0.0/plone/protect/monkey.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# -*- coding: utf-8 -*-
 from plone.protect.auto import safeWrite
 from zope.testing.cleanup import addCleanUp
+
 import inspect
 
 
 def wl_lockmapping(self, killinvalids=0, create=0):
-    has_write_locks = hasattr(self, '_dav_writelocks')
+    has_write_locks = hasattr(self, "_dav_writelocks")
     locks = self._old_wl_lockmapping(killinvalids=killinvalids, create=create)
     try:
         safeWrite(locks)
         if not has_write_locks and create:
             # first time writing to object, need to mark it safe
             safeWrite(self)
     except AttributeError:
@@ -18,18 +18,18 @@
     return locks
 
 
 def pluggableauth__getCSRFToken(request):
     """
     let plone.protect do it's job
     """
-    return ''
+    return ""
 
 
-def pluggableauth__checkCSRFToken(request, token='csrf_token', raises=True):
+def pluggableauth__checkCSRFToken(request, token="csrf_token", raises=True):
     """
     let plone.protect do it's job
     """
     pass
 
 
 def marmoset_patch(func, replacement):
@@ -37,32 +37,37 @@
     exec(source, func.__globals__)
     func._old_code = func.__code__
     func.__code__ = replacement.__code__
 
 
 def disable_zope_csrf_checks():
     from Products.PluggableAuthService import utils as pluggable_utils
-    if hasattr(pluggable_utils, 'checkCSRFToken'):
+
+    if hasattr(pluggable_utils, "checkCSRFToken"):
         marmoset_patch(
             pluggable_utils.checkCSRFToken,
             pluggableauth__checkCSRFToken,
         )
-    if hasattr(pluggable_utils, 'getCSRFToken'):
-        marmoset_patch(
-            pluggable_utils.getCSRFToken, pluggableauth__getCSRFToken)
+    if hasattr(pluggable_utils, "getCSRFToken"):
+        marmoset_patch(pluggable_utils.getCSRFToken, pluggableauth__getCSRFToken)
 
 
 def enable_zope_csrf_checks():
     from Products.PluggableAuthService import utils as pluggable_utils
-    if hasattr(pluggable_utils, 'checkCSRFToken'):
+
+    if hasattr(pluggable_utils, "checkCSRFToken"):
         try:
-            pluggable_utils.checkCSRFToken.__code__ = \
+            pluggable_utils.checkCSRFToken.__code__ = (
                 pluggable_utils.checkCSRFToken._old_code
+            )
         except AttributeError:
             pass
-    if hasattr(pluggable_utils, 'getCSRFToken'):
+    if hasattr(pluggable_utils, "getCSRFToken"):
         try:
-            pluggable_utils.getCSRFToken.__code__ = \
+            pluggable_utils.getCSRFToken.__code__ = (
                 pluggable_utils.getCSRFToken._old_code
+            )
         except AttributeError:
             pass
+
+
 addCleanUp(enable_zope_csrf_checks)
```

### Comparing `plone.protect-4.1.8/plone/protect/protect.js` & `plone.protect-5.0.0/plone/protect/protect.js`

 * *Files identical despite different names*

### Comparing `plone.protect-4.1.8/plone/protect/subscribers.py` & `plone.protect-5.0.0/plone/protect/subscribers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-# -*- coding: utf-8 -*-
 from plone.keyring.interfaces import IKeyManager
 from plone.protect.interfaces import IDisableCSRFProtection
 from plone.protect.utils import getRoot
 from plone.protect.utils import getRootKeyManager
 from Products.PluggableAuthService.interfaces.events import IUserLoggedInEvent
 from zope.component import adapter
 from zope.component import ComponentLookupError
 from zope.component import getUtility
+from zope.component.hooks import getSite
 from zope.globalrequest import getRequest
 from zope.interface import alsoProvides
 
 import logging
 import time
 
 
-try:
-    from zope.component.hooks import getSite
-except ImportError:
-    from zope.app.component.hooks import getSite
-
-
-LOGGER = logging.getLogger('plone.protect')
+LOGGER = logging.getLogger("plone.protect")
 
 _ring_rotation_schedules = (
-    ('_system', 60 * 60 * 24 * 7),  # weekly
-    ('_forms', 60 * 60 * 24),  # daily
-    ('_anon', 60 * 60 * 24),  # daily
+    ("_system", 60 * 60 * 24 * 7),  # weekly
+    ("_forms", 60 * 60 * 24),  # daily
+    ("_anon", 60 * 60 * 24),  # daily
 )
 
 
 def _rotate(manager):
     current_time = time.time()
     for ring_name, check_period in _ring_rotation_schedules:
         try:
             ring = manager[ring_name]
             if (ring.last_rotation + check_period) < current_time:
-                LOGGER.info('auto rotating keyring %s' % ring_name)
+                LOGGER.info("auto rotating keyring %s" % ring_name)
                 ring.rotate()
         except KeyError:
             continue
 
 
 @adapter(IUserLoggedInEvent)
 def onUserLogsIn(event):
@@ -59,9 +53,9 @@
         manager = getRootKeyManager(root)
         if manager:
             _rotate(manager)
     except ComponentLookupError:
         if req:
             url = req.URL
         else:
-            url = ''
-        LOGGER.warn('cannot find key manager for url %s' % url)
+            url = ""
+        LOGGER.warn("cannot find key manager for url %s" % url)
```

### Comparing `plone.protect-4.1.8/plone/protect/testing.py` & `plone.protect-5.0.0/plone/protect/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import applyProfile
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing.layers import FunctionalTesting
 from plone.protect.auto import safeWrite
 from Products.Five import BrowserView
 from zope.configuration import xmlconfig
@@ -10,47 +9,47 @@
 
 class ProtectedLayer(PloneSandboxLayer):
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # load ZCML
         import plone.protect
-        xmlconfig.file('configure.zcml', plone.protect,
-                       context=configurationContext)
-        xmlconfig.file('test.zcml', plone.protect.tests,
-                       context=configurationContext)
+
+        xmlconfig.file("configure.zcml", plone.protect, context=configurationContext)
+        xmlconfig.file("test.zcml", plone.protect.tests, context=configurationContext)
 
     def setUpPloneSite(self, portal):
         # install into the Plone site
-        applyProfile(portal, 'plone.protect:default')
+        applyProfile(portal, "plone.protect:default")
         self.portal = portal
 
     def tearDownZope(self, app):
-        from plone.protect.monkey import enable_zope_csrf_checks
+        from plone.protect.monkey import enable_zope_csrf_checks  # noqa: F401
+
 
 PROTECT_FIXTURE = ProtectedLayer()
 PROTECT_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(PROTECT_FIXTURE,), name="PROTECT_FIXTURE:Functional")
+    bases=(PROTECT_FIXTURE,), name="PROTECT_FIXTURE:Functional"
+)
 
 
 class TestUnprotectedView(BrowserView):
-
     def __call__(self):
         # on posts, write something to the db
-        if 'submit1' in self.request.form or 'submit2' in self.request.form:
-            self.context.foo = 'bar'
+        if "submit1" in self.request.form or "submit2" in self.request.form:
+            self.context.foo = "bar"
             self.context._p_changed = True
-        self.request.response.setHeader('Content-Type', 'text/html')
+        self.request.response.setHeader("Content-Type", "text/html")
         return """
 <html>
 <body>
 <form id="one" method="POST">
     <input type="submit" name="submit1" value="submit1" />
 </form>
-<form id="two" action="%s" METHOD="post">
+<form id="two" action="{}" METHOD="post">
     <input type="submit" name="submit2" value="submit2" />
 </form>
 <form id="three" method="GET">
     <input type="submit" name="submit3" value="submit3" />
 </form>
 <form id="four" action="//foobar/somepath.php" method="POST">
     <input type="submit" name="submit4" value="submit4" />
@@ -61,18 +60,17 @@
 <form id="six" action="https://foobar/somepath.php" method="POST">
     <input type="submit" name="submit6" value="submit6" />
 </form>
 <form id="seven" action="a/relative/path" method="POST">
     <input type="submit" name="submit7" value="submit7" />
 </form>
 </body>
-</html>""" % (
+</html>""".format(
             self.request.URL,
         )
 
 
 class TestSafeToWriteObject(BrowserView):
-
     def __call__(self):
-        self.context.foo = 'bar'
+        self.context.foo = "bar"
         safeWrite(self)
-        return 'done'
+        return "done"
```

### Comparing `plone.protect-4.1.8/plone/protect/tests/case.py` & `plone.protect-5.0.0/plone/protect/tests/case.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# -*- coding: utf-8 -*-
 from AccessControl.SecurityManagement import newSecurityManager
 from AccessControl.SecurityManagement import noSecurityManager
 from AccessControl.User import User
 from plone.keyring.interfaces import IKeyManager
 from plone.keyring.keymanager import KeyManager
 from unittest import TestCase
 from zope.component import getGlobalSiteManager
 
 
 class MockRequest(dict):
-
     def __init__(self, URL=None, *args, **kwargs):
-        super(MockRequest, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.environ = {}
         self.URL = URL
 
     def setReferer(self, url):
-        self.environ['HTTP_REFERER'] = url
+        self.environ["HTTP_REFERER"] = url
 
     def getHeader(self, name):
         return None
 
 
 class KeyringTestCase(TestCase):
-
     key_size = 1
 
     def setUp(self):
         self.sm = getGlobalSiteManager()
         self.manager = KeyManager(self.key_size)
-        self.sm.registerUtility(self.manager, provided=IKeyManager,
-                                event=False)
+        self.sm.registerUtility(self.manager, provided=IKeyManager, event=False)
         # Tests modify the user object so we better make sure it is *our*
         # user object and not the built-in Anonymous User.
-        newSecurityManager(None, User('dummy', 'secret', (), ()))
+        newSecurityManager(None, User("dummy", "secret", (), ()))
 
     def tearDown(self):
         self.sm.unregisterUtility(self.manager, provided=IKeyManager)
         noSecurityManager()
```

### Comparing `plone.protect-4.1.8/plone/protect/tests/testAuthenticator.py` & `plone.protect-5.0.0/plone/protect/tests/testAuthenticator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# -*- coding: utf-8 -*-
 from AccessControl import getSecurityManager
+from hashlib import sha1 as sha
 from plone.protect import createToken
 from plone.protect import CustomCheckAuthenticator
 from plone.protect import protect
 from plone.protect.authenticator import AuthenticatorView
 from plone.protect.authenticator import check
 from plone.protect.tests.case import KeyringTestCase
 from plone.protect.tests.case import MockRequest
@@ -11,34 +11,26 @@
 from unittest import TestSuite
 from zExceptions import Forbidden
 from ZPublisher.HTTPRequest import HTTPRequest
 
 import hmac
 import sys
 
-import six
-
-try:
-    from hashlib import sha1 as sha
-except ImportError:
-    import sha
-
 
 class AuthenticatorTests(KeyringTestCase):
-
     def setUp(self):
         KeyringTestCase.setUp(self)
         self.view = AuthenticatorView(None, None)
 
     def setUsername(self, name):
         user = getSecurityManager().getUser()
         user.name = name
 
     def setSecret(self, secret):
-        self.manager['_forms'].data[0] = secret
+        self.manager["_forms"].data[0] = secret
 
     def testIsHtmlInput(self):
         auth = self.view.authenticator()
         self.assertTrue(auth.startswith("<input"))
         self.assertTrue(auth.endswith("/>"))
 
     def testDiffersPerUser(self):
@@ -51,47 +43,45 @@
         one = self.view.authenticator()
         self.setSecret("other")
         two = self.view.authenticator()
         self.assertNotEqual(one, two)
 
     def testDiffersPerExtra(self):
         one = self.view.authenticator()
-        two = self.view.authenticator('some-extra-value')
+        two = self.view.authenticator("some-extra-value")
         self.assertNotEqual(one, two)
 
 
 class VerifyTests(KeyringTestCase):
-
     key_size = 2
 
     def setUp(self):
         self.request = MockRequest()
-        super(VerifyTests, self).setUp()
+        super().setUp()
         self.view = AuthenticatorView(None, self.request)
 
-    def setAuthenticator(self, key, extra='', name="_authenticator"):
+    def setAuthenticator(self, key, extra="", name="_authenticator"):
         user = getSecurityManager().getUser().getUserName()
-        if six.PY3:
-            user = user.encode('utf-8')
-            extra = extra.encode('utf-8')
-        auth = hmac.new(key.encode('utf-8'), user + extra, sha).hexdigest()
+        user = user.encode("utf-8")
+        extra = extra.encode("utf-8")
+        auth = hmac.new(key.encode("utf-8"), user + extra, sha).hexdigest()
         self.request[name] = auth
 
     def testCorrectAuthenticator(self):
-        self.manager['_forms'].data[0] = "secret"
+        self.manager["_forms"].data[0] = "secret"
         self.setAuthenticator("secret")
         self.assertEqual(self.view.verify(), True)
 
     def testCustomAuthenticatorKeyName(self):
-        self.manager['_forms'].data[0] = "secret"
+        self.manager["_forms"].data[0] = "secret"
         self.setAuthenticator("secret", name="_my_authenticator")
         self.assertEqual(self.view.verify(name="_my_authenticator"), True)
 
     def testOlderSecretVerifies(self):
-        self.manager['_forms'].data[1] = "backup"
+        self.manager["_forms"].data[1] = "backup"
         self.setAuthenticator("backup")
         self.assertEqual(self.view.verify(), True)
 
     def testMissingAuthenticator(self):
         self.assertEqual(self.view.verify(), False)
 
     def testIncorrectAuthenticator(self):
@@ -99,58 +89,62 @@
         self.assertEqual(self.view.verify(), False)
 
     def testAuthenticatorWrongType(self):
         self.request["_authenticator"] = 123
         self.assertEqual(self.view.verify(), False)
 
     def testExtraArgumentCanBeVerified(self):
-        self.manager['_forms'].data[0] = "secret"
-        self.setAuthenticator("secret", 'some-extra-value')
-        self.assertEqual(self.view.verify('some-extra-value'), True)
+        self.manager["_forms"].data[0] = "secret"
+        self.setAuthenticator("secret", "some-extra-value")
+        self.assertEqual(self.view.verify("some-extra-value"), True)
 
 
 class DecoratorTests(KeyringTestCase):
-
     def setUp(self):
         self.request = HTTPRequest(sys.stdin, dict(SERVER_URL="dummy"), None)
         KeyringTestCase.setUp(self)
 
         def func(REQUEST=None):
             return 1
+
         self.func = protect(check)(func)
 
     def testNoRequestParameter(self):
-
         def func():
             pass
+
         self.assertRaises(ValueError, protect(check), func)
 
     def testIgnoreBadRequestType(self):
         self.assertEqual(self.func(), 1)
 
     def testBadAuthenticator(self):
         self.request["_authenticator"] = "incorrect"
         self.assertRaises(Forbidden, self.func, self.request)
 
     def testAuthenticatedCustom(self):
-        self.request['_authenticator'] = createToken('some-value')
+        self.request["_authenticator"] = createToken("some-value")
 
         def func(REQUEST=self.request):
             return True
-        self.assertEquals(
-            protect(CustomCheckAuthenticator('some-value'))(func)(), True)
+
+        self.assertEqual(protect(CustomCheckAuthenticator("some-value"))(func)(), True)
 
     def testAuthenticatedCustomName(self):
-        self.request['_my_authenticator'] = createToken('some-value')
+        self.request["_my_authenticator"] = createToken("some-value")
 
         def func(REQUEST=self.request):
             return True
-        self.assertEquals(
-            protect(CustomCheckAuthenticator(
-                'some-value', '_my_authenticator'))(func)(), True)
+
+        self.assertEqual(
+            protect(CustomCheckAuthenticator("some-value", "_my_authenticator"))(
+                func
+            )(),
+            True,
+        )
 
 
 def test_suite():
     suite = TestSuite()
     suite.addTest(makeSuite(AuthenticatorTests))
     suite.addTest(makeSuite(VerifyTests))
     suite.addTest(makeSuite(DecoratorTests))
```

### Comparing `plone.protect-4.1.8/plone/protect/tests/testAuto.py` & `plone.protect-5.0.0/plone/protect/tests/testAuto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import login
 from plone.app.testing import logout
 from plone.app.testing import SITE_OWNER_NAME
 from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_NAME
 from plone.app.testing import TEST_USER_PASSWORD
 from plone.keyring.interfaces import IKeyManager
@@ -16,169 +15,161 @@
 from zope.annotation.interfaces import IAnnotations
 from zope.component import getUtility
 
 import transaction
 import unittest
 
 
-class _BaseAutoTest(object):
+class _BaseAutoTest:
     layer = PROTECT_FUNCTIONAL_TESTING
 
     def test_adds_csrf_protection_input(self):
-        self.open('test-unprotected')
+        self.open("test-unprotected")
         self.assertTrue('name="_authenticator"' in self.browser.contents)
 
     def test_adds_csrf_protection_for_scheme_relative_same_domain(self):
-        self.open('test-unprotected')
-        form = self.browser.getForm('five')
+        self.open("test-unprotected")
+        form = self.browser.getForm("five")
         form.getControl(name="_authenticator")
 
     def test_adds_csrf_protection_for_relative_path(self):
-        self.open('test-unprotected')
-        form = self.browser.getForm('seven')
+        self.open("test-unprotected")
+        form = self.browser.getForm("seven")
         form.getControl(name="_authenticator")
 
     def test_adds_csrf_protection_for_no_action(self):
-        self.open('test-unprotected')
-        form = self.browser.getForm('one')
+        self.open("test-unprotected")
+        form = self.browser.getForm("one")
         form.getControl(name="_authenticator")
 
     def test_does_not_add_csrf_protection_to_different_domain(self):
-        self.open('test-unprotected')
-        form = self.browser.getForm('six')
+        self.open("test-unprotected")
+        form = self.browser.getForm("six")
         try:
             form.getControl(name="_authenticator")
-            self.assertEqual('should not add authenticator', '')
+            self.assertEqual("should not add authenticator", "")
         except Exception:
             pass
 
-    def test_does_not_add_csrf_protection_to_different_domain_scheme_relative(
-            self):
-        self.open('test-unprotected')
-        form = self.browser.getForm('four')
+    def test_does_not_add_csrf_protection_to_different_domain_scheme_relative(self):
+        self.open("test-unprotected")
+        form = self.browser.getForm("four")
         try:
             form.getControl(name="_authenticator")
-            self.assertEqual('should not add authenticator', '')
+            self.assertEqual("should not add authenticator", "")
         except Exception:
             pass
 
     def test_authentication_works_automatically(self):
-        self.open('test-unprotected')
-        self.browser.getControl('submit1').click()
+        self.open("test-unprotected")
+        self.browser.getControl("submit1").click()
         self.assertEqual(self.portal.foo, "bar")
 
     def test_authentication_works_for_other_form(self):
-        self.open('test-unprotected')
-        self.browser.getControl('submit2').click()
+        self.open("test-unprotected")
+        self.browser.getControl("submit2").click()
         self.assertEqual(self.portal.foo, "bar")
 
     def test_works_for_get_form_yet(self):
-        self.open('test-unprotected')
-        self.browser.getControl('submit3').click()
+        self.open("test-unprotected")
+        self.browser.getControl("submit3").click()
 
     def test_forbidden_raised_if_auth_failure(self):
-        self.open('test-unprotected')
-        self.browser.getForm('one').\
-            getControl(name="_authenticator").value = 'foobar'
+        self.open("test-unprotected")
+        self.browser.getForm("one").getControl(name="_authenticator").value = "foobar"
         # XXX: plone.transformchain don't reraise exceptions
         # try:
         #    self.browser.getControl('submit1').click()
         # except Exception as ex:
         #     self.assertEquals(ex.getcode(), 403)
-        self.browser.getControl('submit1').click()
+        self.browser.getControl("submit1").click()
         self.assertFalse(hasattr(self.portal, "foo"))
 
 
 class AutoCSRFProtectTests(unittest.TestCase, _BaseAutoTest):
-
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.browser = Browser(self.layer['app'])
-        self.request = self.layer['request']
+        self.portal = self.layer["portal"]
+        self.browser = Browser(self.layer["app"])
+        self.request = self.layer["request"]
         login(self.portal, TEST_USER_NAME)
-        self.browser.open(self.portal.absolute_url() + '/login_form')
-        self.browser.getControl(name='__ac_name').value = TEST_USER_NAME
-        self.browser.getControl(
-            name='__ac_password'
-        ).value = TEST_USER_PASSWORD
-        self.browser.getControl('Log in').click()
+        self.browser.open(self.portal.absolute_url() + "/login_form")
+        self.browser.getControl(name="__ac_name").value = TEST_USER_NAME
+        self.browser.getControl(name="__ac_password").value = TEST_USER_PASSWORD
+        self.browser.getControl("Log in").click()
 
     def open(self, path):
-        self.browser.open(self.portal.absolute_url() + '/' + path)
+        self.browser.open(self.portal.absolute_url() + "/" + path)
 
     def test_CSRF_header(self):
-        self.request.environ['HTTP_X_CSRF_TOKEN'] = createToken()
+        self.request.environ["HTTP_X_CSRF_TOKEN"] = createToken()
         view = AuthenticatorView(None, self.request)
         self.assertEqual(view.verify(), True)
 
     def test_incorrect_CSRF_header(self):
-        self.request.environ['HTTP_X_CSRF_TOKEN'] = 'foobar'
+        self.request.environ["HTTP_X_CSRF_TOKEN"] = "foobar"
         view = AuthenticatorView(None, self.request)
         self.assertEqual(view.verify(), False)
 
     def test_only_add_auth_when_user_logged_in(self):
         logout()
-        self.open('logout')
-        self.open('test-unprotected')
+        self.open("logout")
+        self.open("test-unprotected")
         try:
-            self.browser.getForm('one').getControl(name="_authenticator")
-            self.assertEqual('anonymous should not be protected', '')
+            self.browser.getForm("one").getControl(name="_authenticator")
+            self.assertEqual("anonymous should not be protected", "")
         except LookupError:
             pass
 
 
 class TestRoot(unittest.TestCase, _BaseAutoTest):
-
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.browser = Browser(self.layer['app'])
-        self.request = self.layer['request']
+        self.portal = self.layer["portal"]
+        self.browser = Browser(self.layer["app"])
+        self.request = self.layer["request"]
         self.browser.addHeader(
-            'Authorization',
-            'Basic %s:%s' % (SITE_OWNER_NAME, SITE_OWNER_PASSWORD,)
+            "Authorization", f"Basic {SITE_OWNER_NAME}:{SITE_OWNER_PASSWORD}"
         )
 
     def open(self, path):
-        self.browser.open(self.portal.aq_parent.absolute_url() + '/' + path)
+        self.browser.open(self.portal.aq_parent.absolute_url() + "/" + path)
 
 
 class AutoRotateTests(unittest.TestCase):
     layer = PROTECT_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.browser = Browser(self.layer['app'])
-        self.request = self.layer['request']
+        self.portal = self.layer["portal"]
+        self.browser = Browser(self.layer["app"])
+        self.request = self.layer["request"]
 
     def test_keyrings_get_rotated_on_login(self):
         manager = getUtility(IKeyManager)
-        ring = manager['_forms']
+        ring = manager["_forms"]
         keys = ring.data
         ring.last_rotation = 0
         transaction.commit()
 
         # should be rotated on login
         login(self.portal, TEST_USER_NAME)
-        self.browser.open(self.portal.absolute_url() + '/login_form')
-        self.browser.getControl(name='__ac_name').value = TEST_USER_NAME
-        self.browser.getControl(
-            name='__ac_password').value = TEST_USER_PASSWORD
-        self.browser.getControl('Log in').click()
+        self.browser.open(self.portal.absolute_url() + "/login_form")
+        self.browser.getControl(name="__ac_name").value = TEST_USER_NAME
+        self.browser.getControl(name="__ac_password").value = TEST_USER_PASSWORD
+        self.browser.getControl("Log in").click()
 
         self.assertNotEqual(keys, ring.data)
         self.assertNotEqual(ring.last_rotation, 0)
 
 
 class TestAutoChecks(unittest.TestCase):
     layer = PROTECT_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.request = self.layer['request']
-        self.request.REQUEST_METHOD = 'POST'
+        self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
+        self.request.REQUEST_METHOD = "POST"
 
     def test_safe_write_empty_returns_false(self):
         transform = ProtectTransform(self.portal, self.request)
         transform._registered_objects = lambda: [self.portal]
         self.assertRaises(Forbidden, transform._check)
 
     def test_safe_write_empty_returns_true(self):
@@ -187,42 +178,48 @@
         transform._registered_objects = lambda: [self.portal]
         self.assertTrue(transform._check())
 
     def test_safe_write_large_oobtree(self):
         annotations = IAnnotations(self.portal)
         # Make sure the OOBTree has a second bucket. One bucket holds 30 items.
         for idx in range(35):
-            key = '{0}{1}'.format(__name__, idx)
-            value = 'test'
+            key = f"{__name__}{idx}"
+            value = "test"
             annotations[key] = value
         transaction.commit()
         # Key that is alphabetically after the others ends up in the second
         # bucket.
-        annotations['{0}{1}'.format(__name__, 'XXX999')] = 'abcd'
+        annotations["{}{}".format(__name__, "XXX999")] = "abcd"
         safeWrite(annotations.obj.__annotations__)
         transform = ProtectTransform(self.portal, self.request)
         self.assertTrue(transform._check())
 
 
 class TestAutoTransform(unittest.TestCase):
     layer = PROTECT_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.request = self.layer['request']
-        self.request.response.setHeader('Content-Type', 'text/html')
-        self.request.REQUEST_METHOD = 'POST'
+        self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
+        self.request.response.setHeader("Content-Type", "text/html")
+        self.request.REQUEST_METHOD = "POST"
 
     def test_empty_no_error(self):
         # empty pages (eg. tiles or ajax requests) should not lead to
         # transform errors or warnings
         transform = ProtectTransform(self.portal, self.request)
-        result = transform.transform(['\n'], 'utf-8')
+        result = transform.transform(["\n"], "utf-8")
         self.assertEqual(result, None)
 
     def test_html(self):
         transform = ProtectTransform(self.portal, self.request)
-        result = transform.transform([(
-            '<html>\n<body>'
-            '<form action="http://nohost/myaction" method="POST">'
-            '</form></body>\n</html>')], 'utf-8')
-        self.assertTrue(b'_authenticator' in result.serialize())
+        result = transform.transform(
+            [
+                (
+                    "<html>\n<body>"
+                    '<form action="http://nohost/myaction" method="POST">'
+                    "</form></body>\n</html>"
+                )
+            ],
+            "utf-8",
+        )
+        self.assertTrue(b"_authenticator" in result.serialize())
```

### Comparing `plone.protect-4.1.8/plone/protect/tests/testPostOnly.py` & `plone.protect-5.0.0/plone/protect/tests/testPostOnly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*-
 from plone.protect.postonly import check
 from unittest import makeSuite
 from unittest import TestCase
 from unittest import TestSuite
 from zExceptions import Forbidden
 from ZPublisher.HTTPRequest import HTTPRequest
 
 
 class PostOnlyTests(TestCase):
-
     def makeRequest(self, method):
-        return HTTPRequest(None,
-                           dict(REQUEST_METHOD=method,
-                                SERVER_PORT="80",
-                                SERVER_NAME="localhost"),
-                           None)
+        return HTTPRequest(
+            None,
+            dict(REQUEST_METHOD=method, SERVER_PORT="80", SERVER_NAME="localhost"),
+            None,
+        )
 
     def testNonHTTPRequestAllowed(self):
         check("not a request")
 
     def testGETRequestForbidden(self):
         self.assertRaises(Forbidden, check, self.makeRequest("GET"))
```

### Comparing `plone.protect-4.1.8/plone/protect/tests/testUtils.py` & `plone.protect-5.0.0/plone/protect/tests/testUtils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.protect.testing import PROTECT_FUNCTIONAL_TESTING
 from plone.protect.utils import addTokenToUrl
 from plone.protect.utils import protect
 from unittest import makeSuite
 from unittest import TestCase
 from unittest import TestSuite
 
@@ -14,21 +13,19 @@
 
 
 def funcWithRequest(one, two, REQUEST=None):
     return (one, two)
 
 
 class DummyChecker:
-
     def __call__(self, request):
         self.request = request
 
 
 class DecoratorTests(TestCase):
-
     def testFunctionMustHaveRequest(self):
         protector = protect()
         self.assertRaises(ValueError, protector, funcWithoutRequest)
 
     def testArgumentsPassed(self):
         wrapped = protect()(funcWithRequest)
         self.assertEqual(wrapped("one", "two"), ("one", "two"))
@@ -46,36 +43,34 @@
         wrapped = protect(checker)(funcWithRequest)
         request = []
         wrapped("one", "two", request)
         self.assertTrue(checker.request is request)
 
 
 class UrlTests(unittest.TestCase):
-
     layer = PROTECT_FUNCTIONAL_TESTING
 
     def testWithUrlFromSameDomain(self):
-        url = addTokenToUrl('http://nohost/foobar', self.layer['request'])
-        self.assertTrue('_authenticator=' in url)
+        url = addTokenToUrl("http://nohost/foobar", self.layer["request"])
+        self.assertTrue("_authenticator=" in url)
 
     def testWithUrlFromOtherDomain(self):
-        url = addTokenToUrl('http://other/foobar', self.layer['request'])
-        self.assertTrue('_authenticator=' not in url)
+        url = addTokenToUrl("http://other/foobar", self.layer["request"])
+        self.assertTrue("_authenticator=" not in url)
 
     def testAddingWithQueryParams(self):
-        url = addTokenToUrl('http://nohost/foobar?foo=bar',
-                            self.layer['request'])
-        self.assertTrue('_authenticator=' in url)
+        url = addTokenToUrl("http://nohost/foobar?foo=bar", self.layer["request"])
+        self.assertTrue("_authenticator=" in url)
 
     def testWithoutRequest(self):
-        url = addTokenToUrl('http://nohost/foobar')
-        self.assertTrue('_authenticator=' in url)
+        url = addTokenToUrl("http://nohost/foobar")
+        self.assertTrue("_authenticator=" in url)
 
     def testWithNone(self):
-        url = addTokenToUrl(None, self.layer['request'])
+        url = addTokenToUrl(None, self.layer["request"])
         self.assertTrue(not url)
 
 
 def test_suite():
     suite = TestSuite()
     suite.addTest(makeSuite(DecoratorTests))
     suite.addTest(makeSuite(UrlTests))
```

### Comparing `plone.protect-4.1.8/plone/protect/tests/test_confirm_view.py` & `plone.protect-5.0.0/plone/protect/tests/test_confirm_view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,23 @@
-# -*- coding: utf-8 -*-
 from plone.protect.testing import PROTECT_FUNCTIONAL_TESTING
 from zExceptions import Forbidden
 from zope.component import getMultiAdapter
 
 import unittest
 
 
 class TestAttackVector(unittest.TestCase):
     layer = PROTECT_FUNCTIONAL_TESTING
 
     def test_regression(self):
-        portal = self.layer['portal']
-        request = self.layer['request']
-        view = getMultiAdapter(
-            (portal, request), name=u'confirm-action')
-        request.form.update({
-            'original_url': 'foobar'
-        })
+        portal = self.layer["portal"]
+        request = self.layer["request"]
+        view = getMultiAdapter((portal, request), name="confirm-action")
+        request.form.update({"original_url": "foobar"})
         self.assertTrue('value="foobar"' in view())
 
     def test_valid_url(self):
-        portal = self.layer['portal']
-        request = self.layer['request']
-        view = getMultiAdapter(
-            (portal, request), name=u'confirm-action')
-        request.form.update({
-            'original_url': 'javascript:alert(1)'
-        })
+        portal = self.layer["portal"]
+        request = self.layer["request"]
+        view = getMultiAdapter((portal, request), name="confirm-action")
+        request.form.update({"original_url": "javascript:alert(1)"})
         self.assertRaises(Forbidden, view)
```

### Comparing `plone.protect-4.1.8/plone/protect/utils.py` & `plone.protect-5.0.0/plone/protect/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from AccessControl.requestmethod import buildfacade
 from Acquisition import aq_parent
 from BTrees.IFBTree import IFBTree
 from BTrees.IIBTree import IIBTree
 from BTrees.IOBTree import IOBTree
 from BTrees.LFBTree import LFBTree
 from BTrees.LLBTree import LLBTree
@@ -15,36 +14,35 @@
 from plone.protect.authenticator import createToken
 from zope.globalrequest import getRequest
 
 import inspect
 import logging
 
 
-SAFE_WRITE_KEY = 'plone.protect.safe_oids'
+SAFE_WRITE_KEY = "plone.protect.safe_oids"
 BTREE_TYPES = (
     IFBTree,
     IIBTree,
     IOBTree,
     LFBTree,
     LLBTree,
     LOBTree,
     OIBTree,
     OLBTree,
     OOBTree,
 )
-LOGGER = logging.getLogger('plone.protect')
+LOGGER = logging.getLogger("plone.protect")
 
 _default = []
 
 # This is based on AccessControl.requestmethod.postonly
 # It should probably be updated to use the decorator module.
 
 
-class protect(object):
-
+class protect:
     def __init__(self, *checkers):
         self.checkers = checkers
 
     def __call__(self, callable):
         try:
             spec = inspect.getfullargspec(callable)
         except AttributeError:
@@ -57,15 +55,15 @@
         try:
             r_index = args.index("REQUEST")
         except ValueError:
             raise ValueError("No REQUEST parameter in callable signature")
 
         arglen = len(args)
         if defaults is not None:
-            defaults = list(zip(args[arglen - len(defaults):], defaults))
+            defaults = list(zip(args[arglen - len(defaults) :], defaults))
             arglen -= len(defaults)
 
         def _curried(*args, **kw):
             request = None
 
             if len(args) > r_index:
                 request = args[r_index]
@@ -95,31 +93,31 @@
     if not url:
         return url
     if req is None:
         req = getRequest()
     if req is None or not url.startswith(req.SERVER_URL):
         # only transforms urls to same site
         return url
-    if getattr(req, 'environ', _default) is _default:
+    if getattr(req, "environ", _default) is _default:
         # TestRequests have no environ.
         token = createToken(manager=manager)
-    elif '_auth_token' not in req.environ:
+    elif "_auth_token" not in req.environ:
         # Let's cache this value since this could be called
         # many times for one request.
         token = createToken(manager=manager)
-        req.environ['_auth_token'] = token
+        req.environ["_auth_token"] = token
     else:
-        token = req.environ['_auth_token']
+        token = req.environ["_auth_token"]
 
-    if '_authenticator' not in url:
-        if '?' not in url:
-            url += '?'
+    if "_authenticator" not in url:
+        if "?" not in url:
+            url += "?"
         else:
-            url += '&'
-        url += '_authenticator=' + token
+            url += "&"
+        url += "_authenticator=" + token
     return url
 
 
 def getRootKeyManager(root):
     if not IApplication.providedBy(root):
         return
     try:
@@ -136,24 +134,24 @@
         context = aq_parent(context)
     return context
 
 
 def safeWrite(obj, request=None):
     if request is None:
         request = getRequest()
-    if request is None or getattr(request, 'environ', _default) is _default:
+    if request is None or getattr(request, "environ", _default) is _default:
         # Request not found or it is a TestRequest without an environment.
-        LOGGER.debug('could not mark object as a safe write')
+        LOGGER.debug("could not mark object as a safe write")
         return
     if SAFE_WRITE_KEY not in request.environ:
         request.environ[SAFE_WRITE_KEY] = []
     try:
         if obj._p_oid not in request.environ[SAFE_WRITE_KEY]:
             request.environ[SAFE_WRITE_KEY].append(obj._p_oid)
         if isinstance(obj, BTREE_TYPES):
             bucket = obj._firstbucket
             while bucket:
                 if bucket._p_oid not in request.environ[SAFE_WRITE_KEY]:
                     request.environ[SAFE_WRITE_KEY].append(bucket._p_oid)
                 bucket = bucket._next
     except AttributeError:
-        LOGGER.debug('object you attempted to mark safe does not have an oid')
+        LOGGER.debug("object you attempted to mark safe does not have an oid")
```

### Comparing `plone.protect-4.1.8/plone/protect/views.py` & `plone.protect-5.0.0/plone/protect/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
 from plone.protect.interfaces import IConfirmView
 from Products.CMFCore.utils import getToolByName
 from Products.Five import BrowserView
 from zExceptions import Forbidden
 from zope.interface import implementer
 
 
 @implementer(IConfirmView)
 class ConfirmView(BrowserView):
-
     def __call__(self):
-        urltool = getToolByName(self.context, 'portal_url')
-        original_url = getattr(self.request, 'original_url', '')
+        urltool = getToolByName(self.context, "portal_url")
+        original_url = getattr(self.request, "original_url", "")
         if not original_url or not urltool.isURLInPortal(original_url):
-            raise Forbidden('url not in portal: {0}'.format(original_url))
+            raise Forbidden(f"url not in portal: {original_url}")
         return self.index()
```

### Comparing `plone.protect-4.1.8/plone.protect.egg-info/PKG-INFO` & `plone.protect-5.0.0/plone.protect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.protect
-Version: 4.1.8
+Version: 5.0.0
 Summary: Security for browser forms
 Home-page: https://github.com/plone/plone.protect
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: zope security CSRF
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
-Classifier: Framework :: Zope :: 2
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 This package contains utilities that can help protect parts of Plone
 or applications build on top of the Plone framework.
@@ -320,20 +314,44 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
-4.1.8 (2022-12-16)
+5.0.0 (2023-04-15)
 ------------------
 
+New features:
+
+
+- Drop support for Python <3.8. (5390ebc6)
+
+
 Bug fixes:
 
 
+- Do not hard-depend on `plone.portlets`.
+  Prepare for Plone with portlets optional.
+  @jensens (#99)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a9dd65cc)
+
+
+4.1.8 (2022-12-16)
+------------------
+
+
+Bug fixes:
+
 - Testing: explicitly set response content type header to html.  [jeromeperrin] (#97)
 
 
 4.1.7 (2022-12-02)
 ------------------
 
 Bug fixes:
```

### Comparing `plone.protect-4.1.8/plone.protect.egg-info/SOURCES.txt` & `plone.protect-5.0.0/plone.protect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

