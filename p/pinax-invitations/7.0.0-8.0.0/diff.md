# Comparing `tmp/pinax-invitations-7.0.0.tar.gz` & `tmp/pinax-invitations-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pinax-invitations-7.0.0.tar", last modified: Fri Jul 17 23:31:03 2020, max compression
+gzip compressed data, was "pinax-invitations-8.0.0.tar", last modified: Fri Apr 14 23:56:56 2023, max compression
```

## Comparing `pinax-invitations-7.0.0.tar` & `pinax-invitations-8.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.325653 pinax-invitations-7.0.0/
--rw-r--r--   0 katherinemichel   (501) staff       (20)      427 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/AUTHORS
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1104 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/LICENSE
--rw-r--r--   0 katherinemichel   (501) staff       (20)       50 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/MANIFEST.in
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2951 2020-07-17 23:31:03.325392 pinax-invitations-7.0.0/PKG-INFO
--rw-r--r--   0 katherinemichel   (501) staff       (20)    12449 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/README.md
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.314359 pinax-invitations-7.0.0/pinax/
--rw-r--r--   0 katherinemichel   (501) staff       (20)       87 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/__init__.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.318087 pinax-invitations-7.0.0/pinax/invitations/
--rw-r--r--   0 katherinemichel   (501) staff       (20)      152 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      791 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/admin.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      349 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/apps.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      230 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/conf.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      787 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/forms.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.318359 pinax-invitations-7.0.0/pinax/invitations/management/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/management/__init__.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.319497 pinax-invitations-7.0.0/pinax/invitations/management/commands/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/management/commands/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      477 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/management/commands/add_invites.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      463 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/management/commands/infinite_invites.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      465 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/management/commands/topoff_invites.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.320375 pinax-invitations-7.0.0/pinax/invitations/migrations/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1928 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/migrations/0001_initial.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      513 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/migrations/0002_auto_20170416_1756.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/migrations/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     5025 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/models.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1387 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/receivers.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      241 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/signals.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      270 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/stats.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.320991 pinax-invitations-7.0.0/pinax/invitations/templatetags/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/templatetags/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1004 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/templatetags/pinax_invitations_tags.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.322399 pinax-invitations-7.0.0/pinax/invitations/tests/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/tests/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3411 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/tests/tests.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      189 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/tests/urls.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      656 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/urls.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     4740 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/pinax/invitations/views.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-17 23:31:03.324923 pinax-invitations-7.0.0/pinax_invitations.egg-info/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2951 2020-07-17 23:31:03.000000 pinax-invitations-7.0.0/pinax_invitations.egg-info/PKG-INFO
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1213 2020-07-17 23:31:03.000000 pinax-invitations-7.0.0/pinax_invitations.egg-info/SOURCES.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        1 2020-07-17 23:31:03.000000 pinax-invitations-7.0.0/pinax_invitations.egg-info/dependency_links.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        1 2020-07-17 23:31:03.000000 pinax-invitations-7.0.0/pinax_invitations.egg-info/not-zip-safe
--rw-r--r--   0 katherinemichel   (501) staff       (20)       62 2020-07-17 23:31:03.000000 pinax-invitations-7.0.0/pinax_invitations.egg-info/requires.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        6 2020-07-17 23:31:03.000000 pinax-invitations-7.0.0/pinax_invitations.egg-info/top_level.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)       38 2020-07-17 23:31:03.325740 pinax-invitations-7.0.0/setup.cfg
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3108 2020-07-17 23:29:59.000000 pinax-invitations-7.0.0/setup.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.351470 pinax-invitations-8.0.0/
+-rw-r--r--   0 chris      (502) staff       (20)      471 2023-04-14 16:50:34.000000 pinax-invitations-8.0.0/AUTHORS
+-rw-r--r--   0 chris      (502) staff       (20)     1104 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/LICENSE
+-rw-r--r--   0 chris      (502) staff       (20)       50 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/MANIFEST.in
+-rw-r--r--   0 chris      (502) staff       (20)     2857 2023-04-14 23:56:56.351237 pinax-invitations-8.0.0/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)    12628 2023-04-14 23:13:43.000000 pinax-invitations-8.0.0/README.md
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.334489 pinax-invitations-8.0.0/pinax/
+-rw-r--r--   0 chris      (502) staff       (20)       87 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/__init__.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.343406 pinax-invitations-8.0.0/pinax/invitations/
+-rw-r--r--   0 chris      (502) staff       (20)      152 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)      791 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/admin.py
+-rw-r--r--   0 chris      (502) staff       (20)      349 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/apps.py
+-rw-r--r--   0 chris      (502) staff       (20)      230 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/conf.py
+-rw-r--r--   0 chris      (502) staff       (20)      787 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/forms.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.344226 pinax-invitations-8.0.0/pinax/invitations/management/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/management/__init__.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.345984 pinax-invitations-8.0.0/pinax/invitations/management/commands/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/management/commands/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)      477 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/management/commands/add_invites.py
+-rw-r--r--   0 chris      (502) staff       (20)      463 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/management/commands/infinite_invites.py
+-rw-r--r--   0 chris      (502) staff       (20)      465 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/management/commands/topoff_invites.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.347321 pinax-invitations-8.0.0/pinax/invitations/migrations/
+-rw-r--r--   0 chris      (502) staff       (20)     1928 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/migrations/0001_initial.py
+-rw-r--r--   0 chris      (502) staff       (20)      513 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/migrations/0002_auto_20170416_1756.py
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/migrations/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     5025 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/models.py
+-rw-r--r--   0 chris      (502) staff       (20)     1387 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/receivers.py
+-rw-r--r--   0 chris      (502) staff       (20)      154 2023-04-14 16:36:30.000000 pinax-invitations-8.0.0/pinax/invitations/signals.py
+-rw-r--r--   0 chris      (502) staff       (20)      270 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/stats.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.347900 pinax-invitations-8.0.0/pinax/invitations/templatetags/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/templatetags/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     1004 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/templatetags/pinax_invitations_tags.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.348859 pinax-invitations-8.0.0/pinax/invitations/tests/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/tests/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     3411 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/tests/tests.py
+-rw-r--r--   0 chris      (502) staff       (20)      196 2023-04-14 16:41:08.000000 pinax-invitations-8.0.0/pinax/invitations/tests/urls.py
+-rw-r--r--   0 chris      (502) staff       (20)      679 2023-04-14 16:40:03.000000 pinax-invitations-8.0.0/pinax/invitations/urls.py
+-rw-r--r--   0 chris      (502) staff       (20)     4740 2023-04-07 16:57:18.000000 pinax-invitations-8.0.0/pinax/invitations/views.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-14 23:56:56.350914 pinax-invitations-8.0.0/pinax_invitations.egg-info/
+-rw-r--r--   0 chris      (502) staff       (20)     2857 2023-04-14 23:56:56.000000 pinax-invitations-8.0.0/pinax_invitations.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)     1213 2023-04-14 23:56:56.000000 pinax-invitations-8.0.0/pinax_invitations.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2023-04-14 23:56:56.000000 pinax-invitations-8.0.0/pinax_invitations.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2023-04-07 22:55:33.000000 pinax-invitations-8.0.0/pinax_invitations.egg-info/not-zip-safe
+-rw-r--r--   0 chris      (502) staff       (20)       62 2023-04-14 23:56:56.000000 pinax-invitations-8.0.0/pinax_invitations.egg-info/requires.txt
+-rw-r--r--   0 chris      (502) staff       (20)        6 2023-04-14 23:56:56.000000 pinax-invitations-8.0.0/pinax_invitations.egg-info/top_level.txt
+-rw-r--r--   0 chris      (502) staff       (20)       38 2023-04-14 23:56:56.351531 pinax-invitations-8.0.0/setup.cfg
+-rw-r--r--   0 chris      (502) staff       (20)     3335 2023-04-14 23:56:50.000000 pinax-invitations-8.0.0/setup.py
```

### Comparing `pinax-invitations-7.0.0/LICENSE` & `pinax-invitations-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/PKG-INFO` & `pinax-invitations-8.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,71 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pinax-invitations
-Version: 7.0.0
+Version: 8.0.0
 Summary: a user to user join invitations app
 Home-page: http://github.com/pinax/pinax-invitations/
 Author: Pinax Team
 Author-email: team@pinaxproject.com
 License: MIT
-Description: 
-        .. image:: http://pinaxproject.com/pinax-design/patches/pinax-invitations.svg
-            :target: https://pypi.python.org/pypi/pinax-invitations/
-        
-        =================
-        Pinax Invitations
-        =================
-        
-        .. image:: https://img.shields.io/pypi/v/pinax-invitations.svg
-            :target: https://pypi.python.org/pypi/pinax-invitations/
-        
-        
-        .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-invitations.svg
-            :target: https://circleci.com/gh/pinax/pinax-invitations
-        .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-invitations.svg
-            :target: https://codecov.io/gh/pinax/pinax-invitations
-        .. image:: https://img.shields.io/github/contributors/pinax/pinax-invitations.svg
-            :target: https://github.com/pinax/pinax-invitations/graphs/contributors
-        .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-invitations.svg
-            :target: https://github.com/pinax/pinax-invitations/pulls
-        .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-invitations.svg
-            :target: https://github.com/pinax/pinax-invitations/pulls?q=is%3Apr+is%3Aclosed
-        
-        
-        .. image:: http://slack.pinaxproject.com/badge.svg
-            :target: http://slack.pinaxproject.com/
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://opensource.org/licenses/MIT/
-        
-        
-        ``pinax-invitations`` is a user to user join invitations app.
-        
-        Supported Django and Python Versions
-        ------------------------------------
-        
-        +-----------------+-----+-----+-----+
-        | Django / Python | 3.6 | 3.7 | 3.8 |
-        +=================+=====+=====+=====+
-        |  2.2            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        |  3.0            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+
+.. image:: http://pinaxproject.com/pinax-design/patches/pinax-invitations.svg
+    :target: https://pypi.python.org/pypi/pinax-invitations/
+
+=================
+Pinax Invitations
+=================
+
+.. image:: https://img.shields.io/pypi/v/pinax-invitations.svg
+    :target: https://pypi.python.org/pypi/pinax-invitations/
+
+
+.. image:: https://img.shields.io/circleci/project/github/pinax/pinax-invitations.svg
+    :target: https://circleci.com/gh/pinax/pinax-invitations
+.. image:: https://img.shields.io/codecov/c/github/pinax/pinax-invitations.svg
+    :target: https://codecov.io/gh/pinax/pinax-invitations
+.. image:: https://img.shields.io/github/contributors/pinax/pinax-invitations.svg
+    :target: https://github.com/pinax/pinax-invitations/graphs/contributors
+.. image:: https://img.shields.io/github/issues-pr/pinax/pinax-invitations.svg
+    :target: https://github.com/pinax/pinax-invitations/pulls
+.. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-invitations.svg
+    :target: https://github.com/pinax/pinax-invitations/pulls?q=is%3Apr+is%3Aclosed
+
+
+.. image:: http://slack.pinaxproject.com/badge.svg
+    :target: http://slack.pinaxproject.com/
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://opensource.org/licenses/MIT/
+
+
+``pinax-invitations`` is a user to user join invitations app.
+
+Supported Django and Python Versions
+------------------------------------
+
++-----------------+-----+-----+-----+------+
+| Django / Python | 3.7 | 3.8 | 3.9 | 3.10 |
++=================+=====+=====+=====+======+
+|  3.2            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
+|  4.0            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
+|  4.1            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
```

### Comparing `pinax-invitations-7.0.0/README.md` & `pinax-invitations-8.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,19 @@
 #### Dependencies
 
 * django-user-accounts
 * django-appconf
 
 #### Supported Django and Python Versions
 
-Django / Python | 3.6 | 3.7 | 3.8
---------------- | --- | --- | ---
-2.2  |  *  |  *  |  *
-3.0  |  *  |  *  |  *
+Django / Python | 3.6 | 3.7 | 3.8 | 3.9
+--------------- | --- | --- | --- | ---  
+2.2  |  *  |  *  |  *  |  *   
+3.1  |  *  |  *  |  *  |  *  
+3.2  |  *  |  *  |  *  |  * 
 
 
 ## Documentation
 
 ### Installation
 
 To install pinax-invitations:
@@ -332,14 +333,19 @@
 #### `_invites_remaining.html`
 
 Fragment displays how many invites a particular user has.
 
 
 ## Change Log
 
+### 8.0.0
+
+* Drop Django 2.* and Python 2,*, 3.4, 3.5 and 3.6 support
+* Add Django 4.* , and Python 3.9, 3.10 support
+
 ### 7.0.0
 
 * Drop Django 1.11, 2.0, and 2.1, and Python 2,7, 3.4, and 3.5 support
 * Add Django 2.2 and 3.0, and Python 3.6, 3.7, and 3.8 support
 * Update packaging configs
 * Direct users to community resources
```

### Comparing `pinax-invitations-7.0.0/pinax/invitations/admin.py` & `pinax-invitations-8.0.0/pinax/invitations/admin.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/forms.py` & `pinax-invitations-8.0.0/pinax/invitations/forms.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/migrations/0001_initial.py` & `pinax-invitations-8.0.0/pinax/invitations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/migrations/0002_auto_20170416_1756.py` & `pinax-invitations-8.0.0/pinax/invitations/migrations/0002_auto_20170416_1756.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/models.py` & `pinax-invitations-8.0.0/pinax/invitations/models.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/receivers.py` & `pinax-invitations-8.0.0/pinax/invitations/receivers.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/templatetags/pinax_invitations_tags.py` & `pinax-invitations-8.0.0/pinax/invitations/templatetags/pinax_invitations_tags.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/tests/tests.py` & `pinax-invitations-8.0.0/pinax/invitations/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax/invitations/urls.py` & `pinax-invitations-8.0.0/pinax/invitations/urls.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from django.conf.urls import url
+from django.urls import re_path
 
 from .views import (
     AddToAllView,
     AddToUserView,
     InviteStatView,
     InviteView,
     TopOffAllView,
     TopOffUserView,
 )
 
 app_name = "pinax_invitations"
 
 urlpatterns = [
-    url(r"^invite/$", InviteView.as_view(), name="invite"),
-    url(r"^invite-stat/(?P<pk>\d+)/$", InviteStatView.as_view(), name="invite_stat"),
-    url(r"^topoff/$", TopOffAllView.as_view(), name="topoff_all"),
-    url(r"^topoff/(?P<pk>\d+)/$", TopOffUserView.as_view(), name="topoff_user"),
-    url(r"^addto/$", AddToAllView.as_view(), name="addto_all"),
-    url(r"^addto/(?P<pk>\d+)/$", AddToUserView.as_view(), name="addto_user"),
+    re_path(r"^invite/$", InviteView.as_view(), name="invite"),
+    re_path(r"^invite-stat/(?P<pk>\d+)/$", InviteStatView.as_view(), name="invite_stat"),
+    re_path(r"^topoff/$", TopOffAllView.as_view(), name="topoff_all"),
+    re_path(r"^topoff/(?P<pk>\d+)/$", TopOffUserView.as_view(), name="topoff_user"),
+    re_path(r"^addto/$", AddToAllView.as_view(), name="addto_all"),
+    re_path(r"^addto/(?P<pk>\d+)/$", AddToUserView.as_view(), name="addto_user"),
 ]
```

### Comparing `pinax-invitations-7.0.0/pinax/invitations/views.py` & `pinax-invitations-8.0.0/pinax/invitations/views.py`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/pinax_invitations.egg-info/PKG-INFO` & `pinax-invitations-8.0.0/pinax_invitations.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,71 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pinax-invitations
-Version: 7.0.0
+Version: 8.0.0
 Summary: a user to user join invitations app
 Home-page: http://github.com/pinax/pinax-invitations/
 Author: Pinax Team
 Author-email: team@pinaxproject.com
 License: MIT
-Description: 
-        .. image:: http://pinaxproject.com/pinax-design/patches/pinax-invitations.svg
-            :target: https://pypi.python.org/pypi/pinax-invitations/
-        
-        =================
-        Pinax Invitations
-        =================
-        
-        .. image:: https://img.shields.io/pypi/v/pinax-invitations.svg
-            :target: https://pypi.python.org/pypi/pinax-invitations/
-        
-        
-        .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-invitations.svg
-            :target: https://circleci.com/gh/pinax/pinax-invitations
-        .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-invitations.svg
-            :target: https://codecov.io/gh/pinax/pinax-invitations
-        .. image:: https://img.shields.io/github/contributors/pinax/pinax-invitations.svg
-            :target: https://github.com/pinax/pinax-invitations/graphs/contributors
-        .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-invitations.svg
-            :target: https://github.com/pinax/pinax-invitations/pulls
-        .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-invitations.svg
-            :target: https://github.com/pinax/pinax-invitations/pulls?q=is%3Apr+is%3Aclosed
-        
-        
-        .. image:: http://slack.pinaxproject.com/badge.svg
-            :target: http://slack.pinaxproject.com/
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://opensource.org/licenses/MIT/
-        
-        
-        ``pinax-invitations`` is a user to user join invitations app.
-        
-        Supported Django and Python Versions
-        ------------------------------------
-        
-        +-----------------+-----+-----+-----+
-        | Django / Python | 3.6 | 3.7 | 3.8 |
-        +=================+=====+=====+=====+
-        |  2.2            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        |  3.0            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+
+.. image:: http://pinaxproject.com/pinax-design/patches/pinax-invitations.svg
+    :target: https://pypi.python.org/pypi/pinax-invitations/
+
+=================
+Pinax Invitations
+=================
+
+.. image:: https://img.shields.io/pypi/v/pinax-invitations.svg
+    :target: https://pypi.python.org/pypi/pinax-invitations/
+
+
+.. image:: https://img.shields.io/circleci/project/github/pinax/pinax-invitations.svg
+    :target: https://circleci.com/gh/pinax/pinax-invitations
+.. image:: https://img.shields.io/codecov/c/github/pinax/pinax-invitations.svg
+    :target: https://codecov.io/gh/pinax/pinax-invitations
+.. image:: https://img.shields.io/github/contributors/pinax/pinax-invitations.svg
+    :target: https://github.com/pinax/pinax-invitations/graphs/contributors
+.. image:: https://img.shields.io/github/issues-pr/pinax/pinax-invitations.svg
+    :target: https://github.com/pinax/pinax-invitations/pulls
+.. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-invitations.svg
+    :target: https://github.com/pinax/pinax-invitations/pulls?q=is%3Apr+is%3Aclosed
+
+
+.. image:: http://slack.pinaxproject.com/badge.svg
+    :target: http://slack.pinaxproject.com/
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://opensource.org/licenses/MIT/
+
+
+``pinax-invitations`` is a user to user join invitations app.
+
+Supported Django and Python Versions
+------------------------------------
+
++-----------------+-----+-----+-----+------+
+| Django / Python | 3.7 | 3.8 | 3.9 | 3.10 |
++=================+=====+=====+=====+======+
+|  3.2            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
+|  4.0            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
+|  4.1            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
```

### Comparing `pinax-invitations-7.0.0/pinax_invitations.egg-info/SOURCES.txt` & `pinax-invitations-8.0.0/pinax_invitations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinax-invitations-7.0.0/setup.py` & `pinax-invitations-8.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "7.0.0"
+VERSION = "8.0.0"
 LONG_DESCRIPTION = """
 .. image:: http://pinaxproject.com/pinax-design/patches/pinax-invitations.svg
     :target: https://pypi.python.org/pypi/pinax-invitations/
 
 =================
 Pinax Invitations
 =================
@@ -35,21 +35,23 @@
 \
 
 ``pinax-invitations`` is a user to user join invitations app.
 
 Supported Django and Python Versions
 ------------------------------------
 
-+-----------------+-----+-----+-----+
-| Django / Python | 3.6 | 3.7 | 3.8 |
-+=================+=====+=====+=====+
-|  2.2            |  *  |  *  |  *  |
-+-----------------+-----+-----+-----+
-|  3.0            |  *  |  *  |  *  |
-+-----------------+-----+-----+-----+
++-----------------+-----+-----+-----+------+
+| Django / Python | 3.7 | 3.8 | 3.9 | 3.10 |
++=================+=====+=====+=====+======+
+|  3.2            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
+|  4.0            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
+|  4.1            |  *  |  *  |  *  |  *   |
++-----------------+-----+-----+-----+------+
 """
 
 setup(
     author="Pinax Team",
     author_email="team@pinaxproject.com",
     description="a user to user join invitations app",
     name="pinax-invitations",
@@ -61,31 +63,33 @@
     package_data={
         "invitations": []
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=[
-        "django>=2.2",
-        "django-appconf>=1.0.1",
-        "django-user-accounts>=2.0.3",
+        "django>=3.2",
+        "django-appconf>=1.0.5",
+        "django-user-accounts>=3.2.0",
     ],
     test_suite="runtests.runtests",
     tests_require=[
         "django-test-plus",
-        "pinax-templates>=1.0.2",
+        "pinax-templates>=3.0.0",
     ],
     zip_safe=False,
 )
```

