# Comparing `tmp/pip-chill-1.0.1.tar.gz` & `tmp/pip-chill-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pip-chill-1.0.1.tar", last modified: Mon Jan 18 22:36:08 2021, max compression
+gzip compressed data, was "pip-chill-1.0.3.tar", last modified: Sat Apr 15 12:24:11 2023, max compression
```

## Comparing `pip-chill-1.0.1.tar` & `pip-chill-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2021-01-18 22:36:08.078528 pip-chill-1.0.1/
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)      216 2019-07-23 22:35:40.000000 pip-chill-1.0.1/AUTHORS.rst
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     3255 2016-10-07 07:08:08.000000 pip-chill-1.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1554 2021-01-18 22:35:50.000000 pip-chill-1.0.1/HISTORY.rst
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     1617 2019-07-23 22:18:33.000000 pip-chill-1.0.1/LICENSE
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)      264 2016-10-07 07:08:08.000000 pip-chill-1.0.1/MANIFEST.in
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7823 2021-01-18 22:36:08.078528 pip-chill-1.0.1/PKG-INFO
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     3812 2019-07-23 22:35:40.000000 pip-chill-1.0.1/README.rst
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2021-01-18 22:36:08.074528 pip-chill-1.0.1/docs/
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     6774 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/Makefile
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)       28 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/authors.rst
--rwxr-xr-x   0 ricardo   (1000) ricardo   (1000)     8529 2020-03-01 00:56:21.000000 pip-chill-1.0.1/docs/conf.py
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)       33 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/contributing.rst
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)       28 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/history.rst
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)      500 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/index.rst
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     1127 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/installation.rst
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     6465 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/make.bat
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)       27 2016-10-07 07:08:08.000000 pip-chill-1.0.1/docs/readme.rst
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)      234 2020-03-01 00:56:21.000000 pip-chill-1.0.1/docs/usage.rst
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2021-01-18 22:36:08.074528 pip-chill-1.0.1/pip_chill/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      169 2021-01-18 22:35:50.000000 pip-chill-1.0.1/pip_chill/__init__.py
--rwxrwxr-x   0 ricardo   (1000) ricardo   (1000)     1465 2021-01-18 22:35:50.000000 pip-chill-1.0.1/pip_chill/cli.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2962 2021-01-18 22:35:50.000000 pip-chill-1.0.1/pip_chill/pip_chill.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2021-01-18 22:36:08.074528 pip-chill-1.0.1/pip_chill.egg-info/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7823 2021-01-18 22:36:07.000000 pip-chill-1.0.1/pip_chill.egg-info/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      559 2021-01-18 22:36:07.000000 pip-chill-1.0.1/pip_chill.egg-info/SOURCES.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2021-01-18 22:36:07.000000 pip-chill-1.0.1/pip_chill.egg-info/dependency_links.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       50 2021-01-18 22:36:07.000000 pip-chill-1.0.1/pip_chill.egg-info/entry_points.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2021-01-18 22:36:07.000000 pip-chill-1.0.1/pip_chill.egg-info/not-zip-safe
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       10 2021-01-18 22:36:07.000000 pip-chill-1.0.1/pip_chill.egg-info/top_level.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      381 2021-01-18 22:36:08.078528 pip-chill-1.0.1/setup.cfg
--rwxrwxr-x   0 ricardo   (1000) ricardo   (1000)     1649 2021-01-18 22:35:50.000000 pip-chill-1.0.1/setup.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2021-01-18 22:36:08.078528 pip-chill-1.0.1/tests/
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)       24 2016-10-07 07:08:08.000000 pip-chill-1.0.1/tests/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4951 2021-01-18 22:35:50.000000 pip-chill-1.0.1/tests/test_pip_chill.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.289035 pip-chill-1.0.3/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      262 2023-04-15 10:02:53.000000 pip-chill-1.0.3/AUTHORS.rst
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     3277 2023-04-15 10:02:53.000000 pip-chill-1.0.3/CONTRIBUTING.rst
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1827 2023-04-15 12:23:15.000000 pip-chill-1.0.3/HISTORY.rst
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     1617 2019-07-23 22:18:33.000000 pip-chill-1.0.3/LICENSE
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)      264 2016-10-07 07:08:08.000000 pip-chill-1.0.3/MANIFEST.in
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6578 2023-04-15 12:24:11.289035 pip-chill-1.0.3/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     3739 2023-04-15 10:02:53.000000 pip-chill-1.0.3/README.rst
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.281035 pip-chill-1.0.3/docs/
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     6774 2016-10-07 07:08:08.000000 pip-chill-1.0.3/docs/Makefile
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.269035 pip-chill-1.0.3/docs/_build/
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.269035 pip-chill-1.0.3/docs/_build/html/
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.285035 pip-chill-1.0.3/docs/_build/html/_static/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      286 2023-04-14 20:10:58.000000 pip-chill-1.0.3/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       90 2023-04-14 20:10:58.000000 pip-chill-1.0.3/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       90 2023-04-14 20:10:58.000000 pip-chill-1.0.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)       28 2016-10-07 07:08:08.000000 pip-chill-1.0.3/docs/authors.rst
+-rwxr-xr-x   0 ricardo   (1000) ricardo   (1000)     8529 2020-03-01 00:56:21.000000 pip-chill-1.0.3/docs/conf.py
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)       33 2016-10-07 07:08:08.000000 pip-chill-1.0.3/docs/contributing.rst
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)       28 2016-10-07 07:08:08.000000 pip-chill-1.0.3/docs/history.rst
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)      500 2016-10-07 07:08:08.000000 pip-chill-1.0.3/docs/index.rst
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1126 2023-04-15 10:02:53.000000 pip-chill-1.0.3/docs/installation.rst
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     6465 2016-10-07 07:08:08.000000 pip-chill-1.0.3/docs/make.bat
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       64 2023-04-15 12:16:44.000000 pip-chill-1.0.3/docs/modules.rst
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      455 2023-04-15 12:16:44.000000 pip-chill-1.0.3/docs/pip_chill.rst
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)       27 2016-10-07 07:08:08.000000 pip-chill-1.0.3/docs/readme.rst
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)      234 2020-03-01 00:56:21.000000 pip-chill-1.0.3/docs/usage.rst
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.285035 pip-chill-1.0.3/pip_chill/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      169 2021-01-18 22:35:50.000000 pip-chill-1.0.3/pip_chill/__init__.py
+-rwxrwxr-x   0 ricardo   (1000) ricardo   (1000)     1403 2023-04-14 19:47:09.000000 pip-chill-1.0.3/pip_chill/cli.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2996 2023-04-15 12:10:21.000000 pip-chill-1.0.3/pip_chill/pip_chill.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.289035 pip-chill-1.0.3/pip_chill.egg-info/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6578 2023-04-15 12:24:11.000000 pip-chill-1.0.3/pip_chill.egg-info/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      698 2023-04-15 12:24:11.000000 pip-chill-1.0.3/pip_chill.egg-info/SOURCES.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2023-04-15 12:24:11.000000 pip-chill-1.0.3/pip_chill.egg-info/dependency_links.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       49 2023-04-15 12:24:11.000000 pip-chill-1.0.3/pip_chill.egg-info/entry_points.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2023-04-15 12:24:10.000000 pip-chill-1.0.3/pip_chill.egg-info/not-zip-safe
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       10 2023-04-15 12:24:11.000000 pip-chill-1.0.3/pip_chill.egg-info/top_level.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      381 2023-04-15 12:24:11.289035 pip-chill-1.0.3/setup.cfg
+-rwxrwxr-x   0 ricardo   (1000) ricardo   (1000)     1651 2023-04-15 12:23:13.000000 pip-chill-1.0.3/setup.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2023-04-15 12:24:11.289035 pip-chill-1.0.3/tests/
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)       24 2016-10-07 07:08:08.000000 pip-chill-1.0.3/tests/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4951 2023-04-15 11:22:51.000000 pip-chill-1.0.3/tests/test_pip_chill.py
```

### Comparing `pip-chill-1.0.1/CONTRIBUTING.rst` & `pip-chill-1.0.3/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/rbanffy/pip_chill/issues.
+Report bugs at https://github.com/rbanffy/pip-chill/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
 Fix Bugs
 ~~~~~~~~
 
-Look through the GitHub issues for bugs. Anything tagged with "bug"
-and "help wanted" is open to whoever wants to implement it.
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it. Remember to start from the
+`develop` branch.
 
 Implement Features
 ~~~~~~~~~~~~~~~~~~
 
 Look through the GitHub issues for features. Anything tagged with "enhancement"
 and "help wanted" is open to whoever wants to implement it.
 
@@ -41,15 +42,15 @@
 PIP Chill could always use more documentation, whether as part of the
 official PIP Chill docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/rbanffy/pip_chill/issues.
+The best way to send feedback is to file an issue at https://github.com/rbanffy/pip-chill/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -97,18 +98,17 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 2.6, 2.7, 3.3, 3.4 and 3.5, and for PyPy. Check
+3. The pull request should work for Python 3.7+, and for PyPy. Check
    https://travis-ci.org/rbanffy/pip_chill/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
 
-
     $ python -m unittest tests.test_pip_chill
```

### Comparing `pip-chill-1.0.1/HISTORY.rst` & `pip-chill-1.0.3/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+1.0.3 (2023-04-15)
+------------------
+* Sort dependencies alphabetically in --verbose
+* Use `ssort` to topologically sort code
+* Update 3.11-dev to 3.11 on TravisCI
+* Remove support for Python 3.5 and 3.6
+* Update README.rst with --no-chill switch
+* Bump version to 1.0.2
+
 1.0.1 (2021-01-18)
 ------------------
 
 * Add `no-chill` option so that pip-chill is not shown as installed
 * Do Linux tests on Focal where possible (2.7 and 3.7 on ppc64le and s390x, 2.7 on arm64 run Bionic)
 * Fix wrong URLs in CONTRIBUTING.rst
 * Add 3.7, 3.8, 3.9 to ppc64le and s390x, 3.10-dev to Linux, macOS
```

### Comparing `pip-chill-1.0.1/LICENSE` & `pip-chill-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-chill-1.0.1/docs/Makefile` & `pip-chill-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pip-chill-1.0.1/docs/conf.py` & `pip-chill-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pip-chill-1.0.1/docs/installation.rst` & `pip-chill-1.0.3/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 To install PIP Chill, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install pip_chill
 
-This is the preferred method to install PIP Chill, as it will always install the most recent stable release. 
+This is the preferred method to install PIP Chill, as it will always install the most recent stable release.
 
 If you don't have `pip`_ installed, this `Python installation guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 
@@ -28,24 +28,24 @@
 
 The sources for PIP Chill can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
-    $ git clone git://github.com/rbanffy/pip_chill
+    $ git clone git://github.com/rbanffy/pip-chill
 
 Or download the `tarball`_:
 
 .. code-block:: console
 
-    $ curl  -OL https://github.com/rbanffy/pip_chill/tarball/master
+    $ curl  -OL https://github.com/rbanffy/pip-chill/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
-.. _Github repo: https://github.com/rbanffy/pip_chill
-.. _tarball: https://github.com/rbanffy/pip_chill/tarball/master
+.. _Github repo: https://github.com/rbanffy/pip-chill
+.. _tarball: https://github.com/rbanffy/pip-chill/tarball/master
```

### Comparing `pip-chill-1.0.1/docs/make.bat` & `pip-chill-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pip-chill-1.0.1/pip_chill/cli.py` & `pip-chill-1.0.3/pip_chill/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-from __future__ import print_function
+#!/usr/bin/env python3
 
 import argparse
 
 import pip_chill
 
 
 def main():
```

### Comparing `pip-chill-1.0.1/pip_chill/pip_chill.py` & `pip-chill-1.0.3/pip_chill/pip_chill.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,45 +15,48 @@
         self.required_by = set(required_by) if required_by else set()
 
     def get_name_without_version(self):
         """
         Return the name of the package without a version.
         """
         if self.required_by:
-            return "# {} # Installed as dependency for {}".format(
-                self.name, ", ".join(self.required_by)
+            return (
+                f"# {self.name} # Installed as dependency for "
+                f"{', '.join(sorted(self.required_by))}"
             )
         return self.name
 
-    def __str__(self):
-        if self.required_by:
-            return "# {}=={} # Installed as dependency for {}".format(
-                self.name, self.version, ", ".join(self.required_by)
-            )
-        return "{}=={}".format(self.name, self.version)
-
-    def __repr__(self):
-        return '<{}.{} instance "{}">'.format(
-            self.__module__, self.__class__.__name__, self.name
-        )
+    def __lt__(self, other):
+        return self.name < other.name
 
     def __eq__(self, other):
         if self is other:
             return True
         elif isinstance(other, Distribution):
             return self.name == other.name
         else:
             return self.name == other
 
-    def __lt__(self, other):
-        return self.name < other.name
-
     def __hash__(self):
         return hash(self.name)
 
+    def __repr__(self):
+        return (
+            f'<{self.__module__}.{self.__class__.__name__} instance "'
+            f'{self.name}">'
+        )
+
+    def __str__(self):
+        if self.required_by:
+            return (
+                f"# {self.name}=={self.version} # Installed as "
+                f"dependency for {', '.join(sorted(self.required_by))}"
+            )
+        return f"{self.name}=={self.version}"
+
 
 def chill(show_all=False, no_chill=False):
     if show_all:
         ignored_packages = ()
     else:
         ignored_packages = {"pip", "wheel", "setuptools", "pkg-resources"}
```

### Comparing `pip-chill-1.0.1/pip_chill.egg-info/SOURCES.txt` & `pip-chill-1.0.3/pip_chill.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,21 @@
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/modules.rst
+docs/pip_chill.rst
 docs/readme.rst
 docs/usage.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 pip_chill/__init__.py
 pip_chill/cli.py
 pip_chill/pip_chill.py
 pip_chill.egg-info/PKG-INFO
 pip_chill.egg-info/SOURCES.txt
 pip_chill.egg-info/dependency_links.txt
 pip_chill.egg-info/entry_points.txt
```

### Comparing `pip-chill-1.0.1/setup.py` & `pip-chill-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 requirements = []
 
 test_requirements = ["pip"]
 
 setup(
     name="pip-chill",
-    version="1.0.1",
+    version="1.0.3",
     description="Like `pip freeze` but lists only the packages that are not "
     "dependencies of installed packages.",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/x-rst",
     author="Ricardo Bánffy",
     author_email="rbanffy@gmail.com",
     url="https://github.com/rbanffy/pip-chill",
@@ -35,17 +35,17 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: "
         "OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development",
     ],
     test_suite="tests",
     tests_require=test_requirements,
 )
```

### Comparing `pip-chill-1.0.1/tests/test_pip_chill.py` & `pip-chill-1.0.3/tests/test_pip_chill.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         command = "pip_chill/cli.py"
 
         returncode = os.system(command)
         self.assertEqual(returncode, 0)
 
         result = os.popen(command).read()
         for package in ["wheel", "setuptools", "pip"]:
-            self.assertFalse(any(p.startswith(package + "==") for p in result.split("\n")))
+            self.assertFalse(any(p.startswith(f"{package}==") for p in result.split("\n")))
 
     def test_command_line_interface_all(self):
         command = "pip_chill/cli.py --all"
 
         returncode = os.system(command)
         self.assertEqual(returncode, 0)
```

