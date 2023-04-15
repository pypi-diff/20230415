# Comparing `tmp/plone.versioncheck-1.7.0.tar.gz` & `tmp/plone.versioncheck-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.versioncheck-1.7.0.tar", last modified: Fri Mar  8 15:29:28 2019, max compression
+gzip compressed data, was "plone.versioncheck-1.8.0.tar", last modified: Sat Apr 15 08:35:47 2023, max compression
```

## Comparing `plone.versioncheck-1.7.0.tar` & `plone.versioncheck-1.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    21654 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/PKG-INFO
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1737 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tox.ini
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2162 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/setup.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      730 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/setup.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      105 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/foo.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      979 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/buildout.cfg
--rwxrwxr-x   0 jensens   (1000) jensens   (1000)      231 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/bootstrap.sh
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       84 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/baz.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       52 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/bar.cfg
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    11084 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/README.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      138 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/MANIFEST.in
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       70 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4811 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/CHANGES.rst
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      144 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/.coveragerc
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tests/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     2357 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tests/test_version_compare.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tests/test_utils.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4859 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tests/test_script.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1695 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tests/test_parser.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     6164 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tests/test_formatter.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     3777 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/tests/test_analyser.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/zip-safe
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        6 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/top_level.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      164 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/requires.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        6 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/namespace_packages.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      135 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/entry_points.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/dependency_links.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)      986 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/SOURCES.txt
--rw-rw-r--   0 jensens   (1000) jensens   (1000)    21654 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/PKG-INFO
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       80 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4933 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/utils.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     3319 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/tracking.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     4590 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/script.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     9782 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/pypi.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     5980 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/parser.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     9525 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/formatter.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     1566 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/analyser.py
--rw-rw-r--   0 jensens   (1000) jensens   (1000)       24 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/__init__.py
-drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/tpl/
--rw-rw-r--   0 jensens   (1000) jensens   (1000)     3059 2019-03-08 15:29:28.000000 plone.versioncheck-1.7.0/src/plone/versioncheck/tpl/browser.jinja
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)      144 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/.coveragerc
+-rw-r--r--   0 gil       (1000) gil       (1000)     5069 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      138 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    17507 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)    11084 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       52 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/bar.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)       84 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/baz.cfg
+-rwxr-xr-x   0 gil       (1000) gil       (1000)      231 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/bootstrap.sh
+-rw-r--r--   0 gil       (1000) gil       (1000)      979 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/buildout.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)      105 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/foo.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)      615 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     2330 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.486667 plone.versioncheck-1.8.0/src/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.488667 plone.versioncheck-1.8.0/src/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       80 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.489667 plone.versioncheck-1.8.0/src/plone/versioncheck/
+-rw-r--r--   0 gil       (1000) gil       (1000)       24 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1565 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/analyser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9526 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/formatter.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5980 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/parser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    10048 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/pypi.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4590 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/script.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.489667 plone.versioncheck-1.8.0/src/plone/versioncheck/tpl/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3059 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/tpl/browser.jinja
+-rw-r--r--   0 gil       (1000) gil       (1000)     3319 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/tracking.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4949 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/src/plone/versioncheck/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.488667 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    17507 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      986 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      134 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/entry_points.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      164 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:35:47.000000 plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/zip-safe
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:47.490667 plone.versioncheck-1.8.0/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3777 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_analyser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6164 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_formatter.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1695 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_parser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4859 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_script.py
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_utils.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2357 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tests/test_version_compare.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1797 2023-04-15 08:35:46.000000 plone.versioncheck-1.8.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.versioncheck-1.7.0/PKG-INFO` & `plone.versioncheck-1.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,602 +1,614 @@
 Metadata-Version: 2.1
 Name: plone.versioncheck
-Version: 1.7.0
+Version: 1.8.0
 Summary: Checks pinned versions with overrides in a cascaded buildout
 Home-page: https://github.com/plone/plone.versioncheck
 Author: Jens W. Klein
 Author-email: jens@bluedynamics.com
 License: GPL version 2
-Description: .. This README is meant for consumption by humans and PyPI.
-           PyPI can render rst files so please do not use Sphinx features.
-           If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
-           This text does not appear on PyPI or github.
-           It is a comment.
-        
-        
-        =============================================================================
-        Checks pinned versions with overrides in a cascaded buildout
-        =============================================================================
-        
-        .. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
-            :target: https://travis-ci.org/plone/plone.versioncheck
-        
-        .. image:: https://coveralls.io/repos/github/plone/plone.versioncheck/badge.svg?branch=master
-           :target: https://coveralls.io/github/plone/plone.versioncheck?branch=master
-        
-        
-        **plone.versioncheck**
-        
-        .. contents::
-        
-        Features
-        ========
-        
-        1) **Checks buildouts ``[versions]`` sections** while stepping through the cascaded ``extends``
-        
-           - command line script collects the inherited version pins, remembers where a version pin comes from.
-           - It displays the result in order to enable a human to check that pins and overrides are OK.
-           - Output is colored; this helps to identify packages which have newer versions available.
-           - Machine readable output as JSON on demand.
-        
-        2) **Checks Python Package Index (PyPI)** for newer versions.
-        
-           - Detects if a newer major, minor or bugfix (or a prerelease) is available.
-        
-        3) **Buildout extension** records the **current versions state** and **requirements**
-        
-           - versions state and requirements are written to a file,
-           - versions from the file will be consumed by the command line tool
-               - orphaned version pins are detected,
-               - it shows which package pulled in another package as dependency.
-        
-        It works best with `semantically <http://semver.org/>`_ and only with `syntactically <https://setuptools.readthedocs.io/en/latest/setuptools.html#specifying-your-project-s-version>`_ correct version numbers!
-        
-        Usage
-        =====
-        
-        Install with your buildout
-        --------------------------
-        
-        Add a section to install it as a script and add it as an extension to your builodut::
-        
-            [buildout]
-            ...
-            extensions =
-                plone.versioncheck
-        
-            parts =
-                ...
-                ploneversioncheck
-                ...
-        
-            ...
-        
-            [ploneversioncheck]
-            recipe = zc.recipe.egg
-            eggs = plone.versioncheck
-        
-            ...
-        
-        
-        Run buildout as usual.
-        
-        Now a file ``.plone.versioncheck.tracked.json`` was generated in the buildout-directory.
-        
-        This file will be used by ``bin/versioncheck`` to figure out which packages were finally used.
-        
-        Run buildout again to regenerate this file.
-        
-        
-        commandline
-        -----------
-        
-        ::
-        
-          usage: versioncheck [-h] [-p] [-n] [-N] [-r] [-d] [-i] [-e EXCLUDE_CFG] [-m]
-                              [--no-cache] [-b] [-o [OUTPUT]] [--no-colors]
-                              [--debug-limit DEBUG_LIMIT]
-                              [buildout]
-        
-          Fetch information about pinned versions and its overrides in simple and complex/cascaded buildouts.
-        
-          positional arguments:
-            buildout              path to buildout.cfg or other *.cfg file
-        
-          optional arguments:
-            -h, --help            show this help message and exit
-            -p, --pypi            check PyPI for newer versions
-            -n, --newer           display only packages with newer version than active
-            -N, --newer-orphaned  display orphaned packages only when newer versions
-                                  available
-            -r, --required-by     show information about requirements (only if tracking
-                                  file is available)
-            -d, --show-release-dates
-                                  show information about release dates (only for package
-                                  lookup from PyPI)
-            -i, --ignore-tracking
-                                  ignore tracking file (if present)
-            -e EXCLUDE_CFG, --exclude-cfg EXCLUDE_CFG
-                                  exclude in listing when cfg-filename pattern matches
-                                  (fnmatch) the given expression
-            -m, --machine         show as machine readable output (json)
-            --no-cache            do not use a cache for PyPI
-            -b, --browser         show as html for webbrowser
-            -o [OUTPUT], --output [OUTPUT]
-                                  safe output to output-file
-            --no-colors           do not show colors
-            --debug-limit DEBUG_LIMIT
-                                  Limit the number of PyPI versions fetched for
-                                  debugging
-        
-          States and color codes:
-            [A]ctive (white)
-            [D]evelop (green)
-            [O]rphaned (magenta)
-            [I]nherited (older or same versions are gray, newer are yellow)
-            [U]pdate of final release on PyPI available (cyan)
-            [P]rerelease update on PyPI available (blue)
-            [X] unpinned (red)
-            [r] Requirement (gray)
-            [a] Annotation (gray)
-        
-          Color of package name helps to indicate overall state of a package.
-        
-        
-        Files created
-        -------------
-        
-        If the script was used with the ``--pypi`` option, a directory ``.plone.versioncheck.cache`` will be created.
-        It contains the cache of the requests to PyPI or external buildout configuration files.
-        To clear the cache, remove the directory.
-        The caching library uses the expiration headers of the response from PyPI, so even with cache it starts fetching new records.
-        
-        If the extension was used, a file ``.plone.versioncheck.tracked.json`` will be created.
-        It contains the information from last buildout run.
-        
-        
-        Output explained
-        ================
-        
-        Legend of states and colors
-        ---------------------------
-        
-        [D]evelopment Egg
-            A development egg is usually active.
-            Description shows location.
-            Color: Green
-        
-        [A]ctive Pin
-             Pinned version. Package is used and recent, all seems fine.
-             Color: White
-        
-        [I]nherited Pin
-             Unused pin. If older than active, the pin color is gray; if newer, it is yellow.
-        
-        [O]rphaned
-            If tracked, it shows whether the package in the given configuration was used at all.
-            Be careful with this information!
-            I.e. in a development buildout file, other packages are used than in a live or continuous integration buildout!
-            Color: Magenta
-        
-        [X] Unpinnend
-            Tracked, but no pin in ``[versions]`` sections were found.
-            Color: Red
-        
-        [U]pdate final release
-            At PyPI there is a newer final version available (major, minor or bugfix).
-            Descriptions shows on which level.
-            Color: Cyan
-        
-        [P]rerelease update
-            At PyPI there is a newer prerelease version available (major, minor or bugfix).
-            Descriptions shows on which level.
-            Only if there is no final release update available.
-            Color: Blue
-        
-        [r] Required by
-            If tracked and option ``--required-by`` was given, show packages this package is required by.
-            Valid for current active/used version.
-            Keep in mind this is based on the declared requirements, missing or implicit requirements are not covered.
-        
-        [a] Annotation
-            It is possible to annotate the reason why a version was chosen.
-            The information is parsed out of a section ``[versionannotations]``.
-            In this section  key is the name of the package and value the text annotations to be displayed.
-            The value can span more than one line using indent (as usal).
-        
-        
-        Order of versions
-        -----------------
-        
-        Order of versions is the buildout resolution order (how they are resolved by buildout in the extends chain/tree).
-        After that, the PyPI releases are shown (major, minor, pre, then the prereleases)
-        
-        Example, given in each a version of ``my.pkg`` was declared:
-        
-        1. ``buildout.cfg`` with ``my.pkg=3.0.3``
-        
-          1. ``buildout.cfg`` extends ``foo.cfg`` with ``my.pkg=3.0.1``
-        
-          2. ``buildout.cfg`` extends ``bar.cfg`` with ``my.pkg=2.0``
-        
-            2. ``foo cfg`` extends ``baz.cfg`` with ``my.pkg=3.1``
-        
-        2. found a newer versions at pypi
-        
-          1. major ``my.pkg=4.0``
-        
-          2. minor ``my.pkg=3.2``
-        
-          3. major ``prerelease my.pkg=5.1b2``
-        
-        Output looks like so::
-        
-            my.pkg
-                3.0.3............... A buildout.cfg
-                2.0 ................ I bar.cfg
-                3.0.1 .............. I foo.cfg
-                3.1 ................ I baz.cfg
-                4.0 ................ U Major
-                3.2 ................ U Minor
-                5.1b2............... P Majorpre
-        
-        
-        
-        Example
-        -------
-        
-        Here w/o colors, run on ``buildout.coredev``::
-        
-            $ ./bin/versioncheck -p buildout.cfg
-        
-            accesscontrol
-                3.0.12 .... A versions.cfg
-                2.13.13 ... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
-            acquisition
-                4.2.2 ..... A versions.cfg
-                2.13.9 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
-            alabaster
-                0.7.7 ..... X unpinned
-            archetypes.multilingual
-                3.0.1 ..... A versions.cfg
-            archetypes.referencebrowserwidget
-                2.5.6 ..... A versions.cfg
-            archetypes.schemaextender
-                2.1.5 ..... A versions.cfg
-            argcomplete
-                1.0.0 ..... A tests.cfg
-            argh
-                0.26.1 .... A tests.cfg
-            argparse
-                (unset) ... A versions.cfg
-                1.1 ....... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
-                Can not check legacy version number.  U Error
-            autopep8
-                1.2.1 ..... A tests.cfg
-        
-            [... skipped a bunch ...]
-        
-            coverage
-                3.7.1 ..... A tests.cfg
-                3.5.2 ..... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
-                4.0.3 ..... U Major
-                4.1b1 ..... P Majorpre
-            cssmin
-                0.2.0 ..... A versions.cfg
-            cssselect
-                0.9.1 ..... A versions.cfg
-            datetime
-                3.0.3 ..... A versions.cfg
-                2.12.8 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
-                4.0.1 ..... U Major
-            decorator
-                4.0.6 ..... A versions.cfg
-        
-            [... skipped a bunch ...]
-        
-            plone.app.textfield
-                1.2.6 ..... A versions.cfg
-            plone.app.theming
-                1.2.17.dev0  D /home/workspacejensens/coredev5/src/plone.app.theming/src
-                1.2.16 .... I versions.cfg
-            plone.app.tiles
-                2.1.0 ..... A versions.cfg
-                2.2.0 ..... U Minor
-        
-            [... skipped a bunch ...]
-        
-        Source Code and Contributions
-        =============================
-        
-        .. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
-            :target: https://travis-ci.org/plone/plone.versioncheck
-        
-        If you want to help with the development (improvement, update, bug-fixing, ...) of ``plone.versioncheck`` this is a great idea!
-        
-        Please follow the `contribution guidelines <http://docs.plone.org/develop/coredev/docs/guidelines.html>`_.
-        
-        - `Source code at Github <https://github.com/plone/plone.versioncheck>`_
-        - `Issue tracker at Github <https://github.com/plone/plone.versioncheck>`_
-        
-        Maintainer of ``plone.versioncheck`` is Jens Klein and the Plone contributors.
-        We appreciate any contribution and if a release is needed to be done on PyPI, please just contact one of us (best by open an issue).
-        
-        Development
-        ===========
-        
-        There must be ``python`` with ``virtualenv`` and ``pip`` available in system path pointing to Python >=2.7.x
-        Clone the project. Then::
-        
-            $ bootstrap.sh
-        
-        For non-unix systems please read the contents of bootstrap.py and execute the steps manually adapted to your OS.
-        
-        License
-        =======
-        
-        The project is licensed under the GPLv2.
-        
-        
-        Changelog
-        =========
-        
-        1.7.0 (2019-03-08)
-        ------------------
-        
-        - Feature: Offers exclude pattern matching for cfg-files.
-          [jensens]
-        
-        - Use pure black as code style.
-          [jensens]
-        
-        - Test on Python 3.7
-          [jensens]
-        
-        - Fix PyPI url and add output of URL in case of a problem.
-          [jensens]
-        
-        
-        1.6.10 (2018-08-20)
-        -------------------
-        
-        - Fixes another bug in ``find_relative``.
-          [jensens]
-        
-        
-        1.6.9 (2018-08-20)
-        ------------------
-        
-        - Fixes bug in ``find_relative`` introducued in last release.
-          [jensens]
-        
-        
-        1.6.8 (2018-08-14)
-        ------------------
-        
-        Bug fixes:
-        
-        - Better handling of relative paths as entry, like ``project/foo/dev.cfg``.
-          [jensens]
-        
-        - If a file does not extend any other file,
-          the return statement was returning only one parameter,
-          while callers expected 2.
-          [gforcada]
-        
-        
-        1.6.7 (2018-03-26)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fix: Do not trust on setuptools internals.
-          Works now with newest setuptools.
-          [jensens]
-        
-        1.6.6 (2018-01-26)
-        ------------------
-        
-        - Fixed: Inherited extends with same name showed up as same.
-          Now show relative to basedir if possible, else full.
-          [jensens]
-        
-        - Fixed: Relative extends in urls were broken.
-          [jensens]
-        
-        
-        1.6.5 (2017-07-03)
-        ------------------
-        
-        Bug fixes:
-        
-        - Relative Paths should work now, tested with subdirectories.
-          [loechel]
-        
-        
-        1.6.4 (2017-05-08)
-        ------------------
-        
-        - Fix: Default versions section name ``versions`` was not respected.
-          [jensens]
-        
-        
-        1.6.3 (2017-05-05)
-        ------------------
-        
-        - Fixes #17: Requirements were missing.
-          [jensens]
-        
-        - Optimization: Reduce load on PyPI when fetching release dates.
-          [jensens]
-        
-        - Feature: Change package and version fields in html output to links so that you could open pypi page for each package.
-          [loechel]
-        
-        
-        1.6.2 (2017-04-12)
-        ------------------
-        
-        - Fix: Regressions with version-annotations and stdout messages from buildout parser.
-          [loechel]
-        
-        - Add more Tests
-          [loechel]
-        
-        1.6.1 (2017-04-07)
-        ------------------
-        
-        - Fix: #36 New buildout parser does not work with buildout.coredev
-          [loechel]
-        
-        1.6.0 (2017-04-07)
-        ------------------
-        
-        - Fix: ``IndexError: string index out of range`` error with empty states in the formatter.
-          [thet]
-        
-        - Development: Added basic tests to package.
-          [loechel]
-        
-        - Fix: Changed parser.py to use functions from zc.buildout to get versions and versionannotations section names.
-          [loechel]
-        
-        - Feature: Add function to extract date information from PyPI to analyze package age.
-          [loechel]
-        
-        - Feature: Add new CLI options for an output file and show release dates.
-          [loechel]
-        
-        1.5.1 (2017-01-23)
-        ------------------
-        
-        - Fix Version Compare.
-          [loechel]
-        
-        1.5.0 (2016-10-15)
-        ------------------
-        
-        - Development: Use code analysis for QA (and fix issues with pep8 et al.)
-          [jensens]
-        
-        - Fix: Manifest (jinja file was missing).
-          [jensens]
-        
-        - Feature: Implement #25: Annotate versions used.
-          [jensens]
-        
-        
-        1.4 (2016-09-30)
-        ----------------
-        
-        - Feature:
-          New option '-N': feature to hide orphaned without updates.
-          This reduces the noise in a environment where orphaned are used by intend.
-          [jensens]
-        
-        
-        1.3 (2016-05-19)
-        ----------------
-        
-        - Development: Add .editorconfig File to maintain code convetions following Plone API
-          [loechel]
-        
-        - Feature: Add Support for Python 3
-          [loechel]
-        
-        - Fix: Various documentation typos.
-          [jean]
-        
-        1.2.1 (2016-01-26)
-        ------------------
-        
-        - Feature: Cache buildout cfg files fetched over the network.
-          [jensens]
-        
-        - Feature: It caches now responses from PyPI.
-          [jensens]
-        
-        
-        1.1.2 (2016-01-21)
-        ------------------
-        
-        - Fix: Resolution order buildout extends chain was wrong. Also documented the
-          resolution order and included in own builodut a small example.
-          [jensens]
-        
-        - Fix: Formatter printed a newline to much after ``required by``.
-          [jensens]
-        
-        - Fix: Do not complain about missing track file.  If it is not there,
-          the buildout is simply not using the buildout extension.  [maurits]
-        
-        - Fix #13: Added missing ``zc.buildout`` requirement.  [maurits]
-        
-        
-        1.1.1 (2016-01-20)
-        ------------------
-        
-        - Fix: Orphan detection failed when no tracking file was present.
-          [jensens]
-        
-        - Fix: Exception raised when no tracking file was present.
-          [jensens]
-        
-        - Fix: Color of requirements was not set explicitly.
-          [jensens]
-        
-        
-        1.1 (2016-01-19)
-        ----------------
-        
-        - Enhancement: show requirements
-          [jensens]
-        
-        - Enhancement: machine readable output (json)
-          [jensens]
-        
-        - Enhancement: write pure processing-info output to sys.stderr
-          [jensens]
-        
-        - Fix #5 - Require setuptools>=12
-          [jensens]
-        
-        - Fix #7 - Available update from 'lazy' 1.0 to 1.2 is not found.
-          [jensens]
-        
-        - Enhancement: Rethink colors and document them, fixes #2 and #3.
-          [jensens]
-        
-        - Enhancement: display output and show tracked info
-          [jensens]
-        
-        - Feature: Add buildout extension to optional track required by and if its use at all
-          [jensens]
-        
-        
-        1.0 (2016-01-13)
-        ----------------
-        
-        - Initial work.
-          [jensens]
-        
 Keywords: plone buildout version
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Buildout :: Extension
 Classifier: Framework :: Buildout :: Recipe
 Classifier: Framework :: Buildout
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Quality Assurance
-Provides-Extra: develop
-Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: release
+Provides-Extra: test
+Provides-Extra: develop
+
+.. This README is meant for consumption by humans and PyPI.
+   PyPI can render rst files so please do not use Sphinx features.
+   If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
+   This text does not appear on PyPI or github.
+   It is a comment.
+
+
+=============================================================================
+Checks pinned versions with overrides in a cascaded buildout
+=============================================================================
+
+.. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
+    :target: https://travis-ci.org/plone/plone.versioncheck
+
+.. image:: https://coveralls.io/repos/github/plone/plone.versioncheck/badge.svg?branch=master
+   :target: https://coveralls.io/github/plone/plone.versioncheck?branch=master
+
+
+**plone.versioncheck**
+
+.. contents::
+
+Features
+========
+
+1) **Checks buildouts ``[versions]`` sections** while stepping through the cascaded ``extends``
+
+   - command line script collects the inherited version pins, remembers where a version pin comes from.
+   - It displays the result in order to enable a human to check that pins and overrides are OK.
+   - Output is colored; this helps to identify packages which have newer versions available.
+   - Machine readable output as JSON on demand.
+
+2) **Checks Python Package Index (PyPI)** for newer versions.
+
+   - Detects if a newer major, minor or bugfix (or a prerelease) is available.
+
+3) **Buildout extension** records the **current versions state** and **requirements**
+
+   - versions state and requirements are written to a file,
+   - versions from the file will be consumed by the command line tool
+       - orphaned version pins are detected,
+       - it shows which package pulled in another package as dependency.
+
+It works best with `semantically <http://semver.org/>`_ and only with `syntactically <https://setuptools.readthedocs.io/en/latest/setuptools.html#specifying-your-project-s-version>`_ correct version numbers!
+
+Usage
+=====
+
+Install with your buildout
+--------------------------
+
+Add a section to install it as a script and add it as an extension to your builodut::
+
+    [buildout]
+    ...
+    extensions =
+        plone.versioncheck
+
+    parts =
+        ...
+        ploneversioncheck
+        ...
+
+    ...
+
+    [ploneversioncheck]
+    recipe = zc.recipe.egg
+    eggs = plone.versioncheck
+
+    ...
+
+
+Run buildout as usual.
+
+Now a file ``.plone.versioncheck.tracked.json`` was generated in the buildout-directory.
+
+This file will be used by ``bin/versioncheck`` to figure out which packages were finally used.
+
+Run buildout again to regenerate this file.
+
+
+commandline
+-----------
+
+::
+
+  usage: versioncheck [-h] [-p] [-n] [-N] [-r] [-d] [-i] [-e EXCLUDE_CFG] [-m]
+                      [--no-cache] [-b] [-o [OUTPUT]] [--no-colors]
+                      [--debug-limit DEBUG_LIMIT]
+                      [buildout]
+
+  Fetch information about pinned versions and its overrides in simple and complex/cascaded buildouts.
+
+  positional arguments:
+    buildout              path to buildout.cfg or other *.cfg file
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -p, --pypi            check PyPI for newer versions
+    -n, --newer           display only packages with newer version than active
+    -N, --newer-orphaned  display orphaned packages only when newer versions
+                          available
+    -r, --required-by     show information about requirements (only if tracking
+                          file is available)
+    -d, --show-release-dates
+                          show information about release dates (only for package
+                          lookup from PyPI)
+    -i, --ignore-tracking
+                          ignore tracking file (if present)
+    -e EXCLUDE_CFG, --exclude-cfg EXCLUDE_CFG
+                          exclude in listing when cfg-filename pattern matches
+                          (fnmatch) the given expression
+    -m, --machine         show as machine readable output (json)
+    --no-cache            do not use a cache for PyPI
+    -b, --browser         show as html for webbrowser
+    -o [OUTPUT], --output [OUTPUT]
+                          safe output to output-file
+    --no-colors           do not show colors
+    --debug-limit DEBUG_LIMIT
+                          Limit the number of PyPI versions fetched for
+                          debugging
+
+  States and color codes:
+    [A]ctive (white)
+    [D]evelop (green)
+    [O]rphaned (magenta)
+    [I]nherited (older or same versions are gray, newer are yellow)
+    [U]pdate of final release on PyPI available (cyan)
+    [P]rerelease update on PyPI available (blue)
+    [X] unpinned (red)
+    [r] Requirement (gray)
+    [a] Annotation (gray)
+
+  Color of package name helps to indicate overall state of a package.
+
+
+Files created
+-------------
+
+If the script was used with the ``--pypi`` option, a directory ``.plone.versioncheck.cache`` will be created.
+It contains the cache of the requests to PyPI or external buildout configuration files.
+To clear the cache, remove the directory.
+The caching library uses the expiration headers of the response from PyPI, so even with cache it starts fetching new records.
+
+If the extension was used, a file ``.plone.versioncheck.tracked.json`` will be created.
+It contains the information from last buildout run.
+
+
+Output explained
+================
+
+Legend of states and colors
+---------------------------
+
+[D]evelopment Egg
+    A development egg is usually active.
+    Description shows location.
+    Color: Green
+
+[A]ctive Pin
+     Pinned version. Package is used and recent, all seems fine.
+     Color: White
+
+[I]nherited Pin
+     Unused pin. If older than active, the pin color is gray; if newer, it is yellow.
+
+[O]rphaned
+    If tracked, it shows whether the package in the given configuration was used at all.
+    Be careful with this information!
+    I.e. in a development buildout file, other packages are used than in a live or continuous integration buildout!
+    Color: Magenta
+
+[X] Unpinnend
+    Tracked, but no pin in ``[versions]`` sections were found.
+    Color: Red
+
+[U]pdate final release
+    At PyPI there is a newer final version available (major, minor or bugfix).
+    Descriptions shows on which level.
+    Color: Cyan
+
+[P]rerelease update
+    At PyPI there is a newer prerelease version available (major, minor or bugfix).
+    Descriptions shows on which level.
+    Only if there is no final release update available.
+    Color: Blue
+
+[r] Required by
+    If tracked and option ``--required-by`` was given, show packages this package is required by.
+    Valid for current active/used version.
+    Keep in mind this is based on the declared requirements, missing or implicit requirements are not covered.
+
+[a] Annotation
+    It is possible to annotate the reason why a version was chosen.
+    The information is parsed out of a section ``[versionannotations]``.
+    In this section  key is the name of the package and value the text annotations to be displayed.
+    The value can span more than one line using indent (as usal).
+
+
+Order of versions
+-----------------
+
+Order of versions is the buildout resolution order (how they are resolved by buildout in the extends chain/tree).
+After that, the PyPI releases are shown (major, minor, pre, then the prereleases)
+
+Example, given in each a version of ``my.pkg`` was declared:
+
+1. ``buildout.cfg`` with ``my.pkg=3.0.3``
+
+  1. ``buildout.cfg`` extends ``foo.cfg`` with ``my.pkg=3.0.1``
+
+  2. ``buildout.cfg`` extends ``bar.cfg`` with ``my.pkg=2.0``
+
+    2. ``foo cfg`` extends ``baz.cfg`` with ``my.pkg=3.1``
+
+2. found a newer versions at pypi
+
+  1. major ``my.pkg=4.0``
+
+  2. minor ``my.pkg=3.2``
+
+  3. major ``prerelease my.pkg=5.1b2``
+
+Output looks like so::
+
+    my.pkg
+        3.0.3............... A buildout.cfg
+        2.0 ................ I bar.cfg
+        3.0.1 .............. I foo.cfg
+        3.1 ................ I baz.cfg
+        4.0 ................ U Major
+        3.2 ................ U Minor
+        5.1b2............... P Majorpre
+
+
+
+Example
+-------
+
+Here w/o colors, run on ``buildout.coredev``::
+
+    $ ./bin/versioncheck -p buildout.cfg
+
+    accesscontrol
+        3.0.12 .... A versions.cfg
+        2.13.13 ... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
+    acquisition
+        4.2.2 ..... A versions.cfg
+        2.13.9 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
+    alabaster
+        0.7.7 ..... X unpinned
+    archetypes.multilingual
+        3.0.1 ..... A versions.cfg
+    archetypes.referencebrowserwidget
+        2.5.6 ..... A versions.cfg
+    archetypes.schemaextender
+        2.1.5 ..... A versions.cfg
+    argcomplete
+        1.0.0 ..... A tests.cfg
+    argh
+        0.26.1 .... A tests.cfg
+    argparse
+        (unset) ... A versions.cfg
+        1.1 ....... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
+        Can not check legacy version number.  U Error
+    autopep8
+        1.2.1 ..... A tests.cfg
+
+    [... skipped a bunch ...]
+
+    coverage
+        3.7.1 ..... A tests.cfg
+        3.5.2 ..... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
+        4.0.3 ..... U Major
+        4.1b1 ..... P Majorpre
+    cssmin
+        0.2.0 ..... A versions.cfg
+    cssselect
+        0.9.1 ..... A versions.cfg
+    datetime
+        3.0.3 ..... A versions.cfg
+        2.12.8 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
+        4.0.1 ..... U Major
+    decorator
+        4.0.6 ..... A versions.cfg
+
+    [... skipped a bunch ...]
+
+    plone.app.textfield
+        1.2.6 ..... A versions.cfg
+    plone.app.theming
+        1.2.17.dev0  D /home/workspacejensens/coredev5/src/plone.app.theming/src
+        1.2.16 .... I versions.cfg
+    plone.app.tiles
+        2.1.0 ..... A versions.cfg
+        2.2.0 ..... U Minor
+
+    [... skipped a bunch ...]
+
+Source Code and Contributions
+=============================
+
+.. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
+    :target: https://travis-ci.org/plone/plone.versioncheck
+
+If you want to help with the development (improvement, update, bug-fixing, ...) of ``plone.versioncheck`` this is a great idea!
+
+Please follow the `contribution guidelines <http://docs.plone.org/develop/coredev/docs/guidelines.html>`_.
+
+- `Source code at Github <https://github.com/plone/plone.versioncheck>`_
+- `Issue tracker at Github <https://github.com/plone/plone.versioncheck>`_
+
+Maintainer of ``plone.versioncheck`` is Jens Klein and the Plone contributors.
+We appreciate any contribution and if a release is needed to be done on PyPI, please just contact one of us (best by open an issue).
+
+Development
+===========
+
+There must be ``python`` with ``virtualenv`` and ``pip`` available in system path pointing to Python >=2.7.x
+Clone the project. Then::
+
+    $ bootstrap.sh
+
+For non-unix systems please read the contents of bootstrap.py and execute the steps manually adapted to your OS.
+
+License
+=======
+
+The project is licensed under the GPLv2.
+
+
+Changelog
+=========
+
+1.8.0 (2023-04-15)
+------------------
+
+- Ignore invalid versions.
+  Needed for ``setuptools`` 66 and higher when checking a package that has invalid versions on PyPI.
+  Fixes `issue 52 <https://github.com/plone/plone.versioncheck/issues/52>`_.
+  [maurits]
+
+
+1.7.0 (2019-03-08)
+------------------
+
+- Feature: Offers exclude pattern matching for cfg-files.
+  [jensens]
+
+- Use pure black as code style.
+  [jensens]
+
+- Test on Python 3.7
+  [jensens]
+
+- Fix PyPI url and add output of URL in case of a problem.
+  [jensens]
+
+
+1.6.10 (2018-08-20)
+-------------------
+
+- Fixes another bug in ``find_relative``.
+  [jensens]
+
+
+1.6.9 (2018-08-20)
+------------------
+
+- Fixes bug in ``find_relative`` introducued in last release.
+  [jensens]
+
+
+1.6.8 (2018-08-14)
+------------------
+
+Bug fixes:
+
+- Better handling of relative paths as entry, like ``project/foo/dev.cfg``.
+  [jensens]
+
+- If a file does not extend any other file,
+  the return statement was returning only one parameter,
+  while callers expected 2.
+  [gforcada]
+
+
+1.6.7 (2018-03-26)
+------------------
+
+Bug fixes:
+
+- Fix: Do not trust on setuptools internals.
+  Works now with newest setuptools.
+  [jensens]
+
+1.6.6 (2018-01-26)
+------------------
+
+- Fixed: Inherited extends with same name showed up as same.
+  Now show relative to basedir if possible, else full.
+  [jensens]
+
+- Fixed: Relative extends in urls were broken.
+  [jensens]
+
+
+1.6.5 (2017-07-03)
+------------------
+
+Bug fixes:
+
+- Relative Paths should work now, tested with subdirectories.
+  [loechel]
+
+
+1.6.4 (2017-05-08)
+------------------
+
+- Fix: Default versions section name ``versions`` was not respected.
+  [jensens]
+
+
+1.6.3 (2017-05-05)
+------------------
+
+- Fixes #17: Requirements were missing.
+  [jensens]
+
+- Optimization: Reduce load on PyPI when fetching release dates.
+  [jensens]
+
+- Feature: Change package and version fields in html output to links so that you could open pypi page for each package.
+  [loechel]
+
+
+1.6.2 (2017-04-12)
+------------------
+
+- Fix: Regressions with version-annotations and stdout messages from buildout parser.
+  [loechel]
+
+- Add more Tests
+  [loechel]
+
+1.6.1 (2017-04-07)
+------------------
+
+- Fix: #36 New buildout parser does not work with buildout.coredev
+  [loechel]
+
+1.6.0 (2017-04-07)
+------------------
+
+- Fix: ``IndexError: string index out of range`` error with empty states in the formatter.
+  [thet]
+
+- Development: Added basic tests to package.
+  [loechel]
+
+- Fix: Changed parser.py to use functions from zc.buildout to get versions and versionannotations section names.
+  [loechel]
+
+- Feature: Add function to extract date information from PyPI to analyze package age.
+  [loechel]
+
+- Feature: Add new CLI options for an output file and show release dates.
+  [loechel]
+
+1.5.1 (2017-01-23)
+------------------
+
+- Fix Version Compare.
+  [loechel]
+
+1.5.0 (2016-10-15)
+------------------
+
+- Development: Use code analysis for QA (and fix issues with pep8 et al.)
+  [jensens]
+
+- Fix: Manifest (jinja file was missing).
+  [jensens]
+
+- Feature: Implement #25: Annotate versions used.
+  [jensens]
+
+
+1.4 (2016-09-30)
+----------------
+
+- Feature:
+  New option '-N': feature to hide orphaned without updates.
+  This reduces the noise in a environment where orphaned are used by intend.
+  [jensens]
+
+
+1.3 (2016-05-19)
+----------------
+
+- Development: Add .editorconfig File to maintain code convetions following Plone API
+  [loechel]
+
+- Feature: Add Support for Python 3
+  [loechel]
+
+- Fix: Various documentation typos.
+  [jean]
+
+1.2.1 (2016-01-26)
+------------------
+
+- Feature: Cache buildout cfg files fetched over the network.
+  [jensens]
+
+- Feature: It caches now responses from PyPI.
+  [jensens]
+
+
+1.1.2 (2016-01-21)
+------------------
+
+- Fix: Resolution order buildout extends chain was wrong. Also documented the
+  resolution order and included in own builodut a small example.
+  [jensens]
+
+- Fix: Formatter printed a newline to much after ``required by``.
+  [jensens]
+
+- Fix: Do not complain about missing track file.  If it is not there,
+  the buildout is simply not using the buildout extension.  [maurits]
+
+- Fix #13: Added missing ``zc.buildout`` requirement.  [maurits]
+
+
+1.1.1 (2016-01-20)
+------------------
+
+- Fix: Orphan detection failed when no tracking file was present.
+  [jensens]
+
+- Fix: Exception raised when no tracking file was present.
+  [jensens]
+
+- Fix: Color of requirements was not set explicitly.
+  [jensens]
+
+
+1.1 (2016-01-19)
+----------------
+
+- Enhancement: show requirements
+  [jensens]
+
+- Enhancement: machine readable output (json)
+  [jensens]
+
+- Enhancement: write pure processing-info output to sys.stderr
+  [jensens]
+
+- Fix #5 - Require setuptools>=12
+  [jensens]
+
+- Fix #7 - Available update from 'lazy' 1.0 to 1.2 is not found.
+  [jensens]
+
+- Enhancement: Rethink colors and document them, fixes #2 and #3.
+  [jensens]
+
+- Enhancement: display output and show tracked info
+  [jensens]
+
+- Feature: Add buildout extension to optional track required by and if its use at all
+  [jensens]
+
+
+1.0 (2016-01-13)
+----------------
+
+- Initial work.
+  [jensens]
```

### Comparing `plone.versioncheck-1.7.0/tox.ini` & `plone.versioncheck-1.8.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 [tox]
 envlist =
     py27,
     py36,
     py37,
+    py38,
+    py39,
+# These currently fail because they get setuptools 66+:
+#    py310,
+#    py311,
     pypy,
     lint,
     coverage-report,
 
 skip_missing_interpreters = False
 
 [testenv]
@@ -38,43 +43,44 @@
     coverage erase
     coverage combine
     coverage report
     coverage html
     coverage xml
 
 [testenv:isort-apply]
-basepython = python3.6
+basepython = python3.8
 skip_install = true
 deps =
     isort
 
 commands =
-    isort --apply --recursive {toxinidir}/src {toxinidir}/tests {posargs}
+    isort src tests setup.py {posargs}
 
 [testenv:autopep8]
 basepython = python3.6
 skip_install = true
 deps =
     autopep8
     docformatter
 
 commands =
     autopep8 --verbose --in-place --recursive --aggressive --aggressive {toxinidir}/src {toxinidir}/tests setup.py
     docformatter --in-place --recursive {toxinidir}/src {toxinidir}/tests setup.py
 
-[lint]
+[testenv:lint]
 skip_install = true
-basepython = python3.6
+basepython = python3.8
 
 deps =
     isort
-    black
+    black==21.12b0
+    click<8.1
 
 commands =
-    isort --check-only --recursive {toxinidir}/src {toxinidir}/tests setup.py
+    isort --check-only src tests setup.py
     black --check src tests setup.py
 
 whitelist_externals =
     mkdir
 
 [testenv:docs]
 deps =
@@ -83,15 +89,15 @@
 commands =
     python -V
     sphinx-build -b html -d _build/docs/doctrees docs _build/docs/html
     #sphinx-build -b doctest docs _build/docs/doctrees
 
 [testenv:release]
 skip_install = true
-basepython = python3.6
+basepython = python3.8
 
 deps =
     zest.releaser[recommended]
 
 commands =
     python -V
     fullrelease --no-input -v
```

### Comparing `plone.versioncheck-1.7.0/setup.py` & `plone.versioncheck-1.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '1.7.0'
+version = "1.8.0"
 
 long_description = "{0}\n\n{1}".format(
     open("README.rst").read(), open("CHANGES.rst").read()
 )
 
 setup(
     name="plone.versioncheck",
     version=version,
     description="Checks pinned versions with overrides in a cascaded buildout",
     long_description=long_description,
-    # Get more strings from
-    # https://pypi.python.org/pypi?:action=list_classifiers
+    # Get more strings from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Buildout :: Extension",
         "Framework :: Buildout :: Recipe",
         "Framework :: Buildout",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Quality Assurance",
     ],
     keywords="plone buildout version ",
     author="Jens W. Klein",
     author_email="jens@bluedynamics.com",
```

### Comparing `plone.versioncheck-1.7.0/setup.cfg` & `plone.versioncheck-1.8.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -21,21 +21,15 @@
 testpaths = 
 	tests
 norecursedirs = 
 	fixures
 xfail_strict = True
 
 [isort]
-force_alphabetical_sort = True
-force_single_line = True
-lines_after_imports = 2
-line_length = 200
-not_skip = 
-	__init__.py
-skip = 
+profile = plone
 
 [flake8]
 exclude = 
 ignore = 
 
 [coverage:run]
 branch = True
```

### Comparing `plone.versioncheck-1.7.0/buildout.cfg` & `plone.versioncheck-1.8.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/README.rst` & `plone.versioncheck-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/CHANGES.rst` & `plone.versioncheck-1.8.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+1.8.0 (2023-04-15)
+------------------
+
+- Ignore invalid versions.
+  Needed for ``setuptools`` 66 and higher when checking a package that has invalid versions on PyPI.
+  Fixes `issue 52 <https://github.com/plone/plone.versioncheck/issues/52>`_.
+  [maurits]
+
+
 1.7.0 (2019-03-08)
 ------------------
 
 - Feature: Offers exclude pattern matching for cfg-files.
   [jensens]
 
 - Use pure black as code style.
```

### Comparing `plone.versioncheck-1.7.0/tests/test_version_compare.py` & `plone.versioncheck-1.8.0/tests/test_version_compare.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/tests/test_script.py` & `plone.versioncheck-1.8.0/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/tests/test_parser.py` & `plone.versioncheck-1.8.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/tests/test_formatter.py` & `plone.versioncheck-1.8.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/tests/test_analyser.py` & `plone.versioncheck-1.8.0/tests/test_analyser.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/SOURCES.txt` & `plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/src/plone.versioncheck.egg-info/PKG-INFO` & `plone.versioncheck-1.8.0/src/plone.versioncheck.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,602 +1,614 @@
 Metadata-Version: 2.1
 Name: plone.versioncheck
-Version: 1.7.0
+Version: 1.8.0
 Summary: Checks pinned versions with overrides in a cascaded buildout
 Home-page: https://github.com/plone/plone.versioncheck
 Author: Jens W. Klein
 Author-email: jens@bluedynamics.com
 License: GPL version 2
-Description: .. This README is meant for consumption by humans and PyPI.
-           PyPI can render rst files so please do not use Sphinx features.
-           If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
-           This text does not appear on PyPI or github.
-           It is a comment.
-        
-        
-        =============================================================================
-        Checks pinned versions with overrides in a cascaded buildout
-        =============================================================================
-        
-        .. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
-            :target: https://travis-ci.org/plone/plone.versioncheck
-        
-        .. image:: https://coveralls.io/repos/github/plone/plone.versioncheck/badge.svg?branch=master
-           :target: https://coveralls.io/github/plone/plone.versioncheck?branch=master
-        
-        
-        **plone.versioncheck**
-        
-        .. contents::
-        
-        Features
-        ========
-        
-        1) **Checks buildouts ``[versions]`` sections** while stepping through the cascaded ``extends``
-        
-           - command line script collects the inherited version pins, remembers where a version pin comes from.
-           - It displays the result in order to enable a human to check that pins and overrides are OK.
-           - Output is colored; this helps to identify packages which have newer versions available.
-           - Machine readable output as JSON on demand.
-        
-        2) **Checks Python Package Index (PyPI)** for newer versions.
-        
-           - Detects if a newer major, minor or bugfix (or a prerelease) is available.
-        
-        3) **Buildout extension** records the **current versions state** and **requirements**
-        
-           - versions state and requirements are written to a file,
-           - versions from the file will be consumed by the command line tool
-               - orphaned version pins are detected,
-               - it shows which package pulled in another package as dependency.
-        
-        It works best with `semantically <http://semver.org/>`_ and only with `syntactically <https://setuptools.readthedocs.io/en/latest/setuptools.html#specifying-your-project-s-version>`_ correct version numbers!
-        
-        Usage
-        =====
-        
-        Install with your buildout
-        --------------------------
-        
-        Add a section to install it as a script and add it as an extension to your builodut::
-        
-            [buildout]
-            ...
-            extensions =
-                plone.versioncheck
-        
-            parts =
-                ...
-                ploneversioncheck
-                ...
-        
-            ...
-        
-            [ploneversioncheck]
-            recipe = zc.recipe.egg
-            eggs = plone.versioncheck
-        
-            ...
-        
-        
-        Run buildout as usual.
-        
-        Now a file ``.plone.versioncheck.tracked.json`` was generated in the buildout-directory.
-        
-        This file will be used by ``bin/versioncheck`` to figure out which packages were finally used.
-        
-        Run buildout again to regenerate this file.
-        
-        
-        commandline
-        -----------
-        
-        ::
-        
-          usage: versioncheck [-h] [-p] [-n] [-N] [-r] [-d] [-i] [-e EXCLUDE_CFG] [-m]
-                              [--no-cache] [-b] [-o [OUTPUT]] [--no-colors]
-                              [--debug-limit DEBUG_LIMIT]
-                              [buildout]
-        
-          Fetch information about pinned versions and its overrides in simple and complex/cascaded buildouts.
-        
-          positional arguments:
-            buildout              path to buildout.cfg or other *.cfg file
-        
-          optional arguments:
-            -h, --help            show this help message and exit
-            -p, --pypi            check PyPI for newer versions
-            -n, --newer           display only packages with newer version than active
-            -N, --newer-orphaned  display orphaned packages only when newer versions
-                                  available
-            -r, --required-by     show information about requirements (only if tracking
-                                  file is available)
-            -d, --show-release-dates
-                                  show information about release dates (only for package
-                                  lookup from PyPI)
-            -i, --ignore-tracking
-                                  ignore tracking file (if present)
-            -e EXCLUDE_CFG, --exclude-cfg EXCLUDE_CFG
-                                  exclude in listing when cfg-filename pattern matches
-                                  (fnmatch) the given expression
-            -m, --machine         show as machine readable output (json)
-            --no-cache            do not use a cache for PyPI
-            -b, --browser         show as html for webbrowser
-            -o [OUTPUT], --output [OUTPUT]
-                                  safe output to output-file
-            --no-colors           do not show colors
-            --debug-limit DEBUG_LIMIT
-                                  Limit the number of PyPI versions fetched for
-                                  debugging
-        
-          States and color codes:
-            [A]ctive (white)
-            [D]evelop (green)
-            [O]rphaned (magenta)
-            [I]nherited (older or same versions are gray, newer are yellow)
-            [U]pdate of final release on PyPI available (cyan)
-            [P]rerelease update on PyPI available (blue)
-            [X] unpinned (red)
-            [r] Requirement (gray)
-            [a] Annotation (gray)
-        
-          Color of package name helps to indicate overall state of a package.
-        
-        
-        Files created
-        -------------
-        
-        If the script was used with the ``--pypi`` option, a directory ``.plone.versioncheck.cache`` will be created.
-        It contains the cache of the requests to PyPI or external buildout configuration files.
-        To clear the cache, remove the directory.
-        The caching library uses the expiration headers of the response from PyPI, so even with cache it starts fetching new records.
-        
-        If the extension was used, a file ``.plone.versioncheck.tracked.json`` will be created.
-        It contains the information from last buildout run.
-        
-        
-        Output explained
-        ================
-        
-        Legend of states and colors
-        ---------------------------
-        
-        [D]evelopment Egg
-            A development egg is usually active.
-            Description shows location.
-            Color: Green
-        
-        [A]ctive Pin
-             Pinned version. Package is used and recent, all seems fine.
-             Color: White
-        
-        [I]nherited Pin
-             Unused pin. If older than active, the pin color is gray; if newer, it is yellow.
-        
-        [O]rphaned
-            If tracked, it shows whether the package in the given configuration was used at all.
-            Be careful with this information!
-            I.e. in a development buildout file, other packages are used than in a live or continuous integration buildout!
-            Color: Magenta
-        
-        [X] Unpinnend
-            Tracked, but no pin in ``[versions]`` sections were found.
-            Color: Red
-        
-        [U]pdate final release
-            At PyPI there is a newer final version available (major, minor or bugfix).
-            Descriptions shows on which level.
-            Color: Cyan
-        
-        [P]rerelease update
-            At PyPI there is a newer prerelease version available (major, minor or bugfix).
-            Descriptions shows on which level.
-            Only if there is no final release update available.
-            Color: Blue
-        
-        [r] Required by
-            If tracked and option ``--required-by`` was given, show packages this package is required by.
-            Valid for current active/used version.
-            Keep in mind this is based on the declared requirements, missing or implicit requirements are not covered.
-        
-        [a] Annotation
-            It is possible to annotate the reason why a version was chosen.
-            The information is parsed out of a section ``[versionannotations]``.
-            In this section  key is the name of the package and value the text annotations to be displayed.
-            The value can span more than one line using indent (as usal).
-        
-        
-        Order of versions
-        -----------------
-        
-        Order of versions is the buildout resolution order (how they are resolved by buildout in the extends chain/tree).
-        After that, the PyPI releases are shown (major, minor, pre, then the prereleases)
-        
-        Example, given in each a version of ``my.pkg`` was declared:
-        
-        1. ``buildout.cfg`` with ``my.pkg=3.0.3``
-        
-          1. ``buildout.cfg`` extends ``foo.cfg`` with ``my.pkg=3.0.1``
-        
-          2. ``buildout.cfg`` extends ``bar.cfg`` with ``my.pkg=2.0``
-        
-            2. ``foo cfg`` extends ``baz.cfg`` with ``my.pkg=3.1``
-        
-        2. found a newer versions at pypi
-        
-          1. major ``my.pkg=4.0``
-        
-          2. minor ``my.pkg=3.2``
-        
-          3. major ``prerelease my.pkg=5.1b2``
-        
-        Output looks like so::
-        
-            my.pkg
-                3.0.3............... A buildout.cfg
-                2.0 ................ I bar.cfg
-                3.0.1 .............. I foo.cfg
-                3.1 ................ I baz.cfg
-                4.0 ................ U Major
-                3.2 ................ U Minor
-                5.1b2............... P Majorpre
-        
-        
-        
-        Example
-        -------
-        
-        Here w/o colors, run on ``buildout.coredev``::
-        
-            $ ./bin/versioncheck -p buildout.cfg
-        
-            accesscontrol
-                3.0.12 .... A versions.cfg
-                2.13.13 ... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
-            acquisition
-                4.2.2 ..... A versions.cfg
-                2.13.9 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
-            alabaster
-                0.7.7 ..... X unpinned
-            archetypes.multilingual
-                3.0.1 ..... A versions.cfg
-            archetypes.referencebrowserwidget
-                2.5.6 ..... A versions.cfg
-            archetypes.schemaextender
-                2.1.5 ..... A versions.cfg
-            argcomplete
-                1.0.0 ..... A tests.cfg
-            argh
-                0.26.1 .... A tests.cfg
-            argparse
-                (unset) ... A versions.cfg
-                1.1 ....... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
-                Can not check legacy version number.  U Error
-            autopep8
-                1.2.1 ..... A tests.cfg
-        
-            [... skipped a bunch ...]
-        
-            coverage
-                3.7.1 ..... A tests.cfg
-                3.5.2 ..... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
-                4.0.3 ..... U Major
-                4.1b1 ..... P Majorpre
-            cssmin
-                0.2.0 ..... A versions.cfg
-            cssselect
-                0.9.1 ..... A versions.cfg
-            datetime
-                3.0.3 ..... A versions.cfg
-                2.12.8 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
-                4.0.1 ..... U Major
-            decorator
-                4.0.6 ..... A versions.cfg
-        
-            [... skipped a bunch ...]
-        
-            plone.app.textfield
-                1.2.6 ..... A versions.cfg
-            plone.app.theming
-                1.2.17.dev0  D /home/workspacejensens/coredev5/src/plone.app.theming/src
-                1.2.16 .... I versions.cfg
-            plone.app.tiles
-                2.1.0 ..... A versions.cfg
-                2.2.0 ..... U Minor
-        
-            [... skipped a bunch ...]
-        
-        Source Code and Contributions
-        =============================
-        
-        .. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
-            :target: https://travis-ci.org/plone/plone.versioncheck
-        
-        If you want to help with the development (improvement, update, bug-fixing, ...) of ``plone.versioncheck`` this is a great idea!
-        
-        Please follow the `contribution guidelines <http://docs.plone.org/develop/coredev/docs/guidelines.html>`_.
-        
-        - `Source code at Github <https://github.com/plone/plone.versioncheck>`_
-        - `Issue tracker at Github <https://github.com/plone/plone.versioncheck>`_
-        
-        Maintainer of ``plone.versioncheck`` is Jens Klein and the Plone contributors.
-        We appreciate any contribution and if a release is needed to be done on PyPI, please just contact one of us (best by open an issue).
-        
-        Development
-        ===========
-        
-        There must be ``python`` with ``virtualenv`` and ``pip`` available in system path pointing to Python >=2.7.x
-        Clone the project. Then::
-        
-            $ bootstrap.sh
-        
-        For non-unix systems please read the contents of bootstrap.py and execute the steps manually adapted to your OS.
-        
-        License
-        =======
-        
-        The project is licensed under the GPLv2.
-        
-        
-        Changelog
-        =========
-        
-        1.7.0 (2019-03-08)
-        ------------------
-        
-        - Feature: Offers exclude pattern matching for cfg-files.
-          [jensens]
-        
-        - Use pure black as code style.
-          [jensens]
-        
-        - Test on Python 3.7
-          [jensens]
-        
-        - Fix PyPI url and add output of URL in case of a problem.
-          [jensens]
-        
-        
-        1.6.10 (2018-08-20)
-        -------------------
-        
-        - Fixes another bug in ``find_relative``.
-          [jensens]
-        
-        
-        1.6.9 (2018-08-20)
-        ------------------
-        
-        - Fixes bug in ``find_relative`` introducued in last release.
-          [jensens]
-        
-        
-        1.6.8 (2018-08-14)
-        ------------------
-        
-        Bug fixes:
-        
-        - Better handling of relative paths as entry, like ``project/foo/dev.cfg``.
-          [jensens]
-        
-        - If a file does not extend any other file,
-          the return statement was returning only one parameter,
-          while callers expected 2.
-          [gforcada]
-        
-        
-        1.6.7 (2018-03-26)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fix: Do not trust on setuptools internals.
-          Works now with newest setuptools.
-          [jensens]
-        
-        1.6.6 (2018-01-26)
-        ------------------
-        
-        - Fixed: Inherited extends with same name showed up as same.
-          Now show relative to basedir if possible, else full.
-          [jensens]
-        
-        - Fixed: Relative extends in urls were broken.
-          [jensens]
-        
-        
-        1.6.5 (2017-07-03)
-        ------------------
-        
-        Bug fixes:
-        
-        - Relative Paths should work now, tested with subdirectories.
-          [loechel]
-        
-        
-        1.6.4 (2017-05-08)
-        ------------------
-        
-        - Fix: Default versions section name ``versions`` was not respected.
-          [jensens]
-        
-        
-        1.6.3 (2017-05-05)
-        ------------------
-        
-        - Fixes #17: Requirements were missing.
-          [jensens]
-        
-        - Optimization: Reduce load on PyPI when fetching release dates.
-          [jensens]
-        
-        - Feature: Change package and version fields in html output to links so that you could open pypi page for each package.
-          [loechel]
-        
-        
-        1.6.2 (2017-04-12)
-        ------------------
-        
-        - Fix: Regressions with version-annotations and stdout messages from buildout parser.
-          [loechel]
-        
-        - Add more Tests
-          [loechel]
-        
-        1.6.1 (2017-04-07)
-        ------------------
-        
-        - Fix: #36 New buildout parser does not work with buildout.coredev
-          [loechel]
-        
-        1.6.0 (2017-04-07)
-        ------------------
-        
-        - Fix: ``IndexError: string index out of range`` error with empty states in the formatter.
-          [thet]
-        
-        - Development: Added basic tests to package.
-          [loechel]
-        
-        - Fix: Changed parser.py to use functions from zc.buildout to get versions and versionannotations section names.
-          [loechel]
-        
-        - Feature: Add function to extract date information from PyPI to analyze package age.
-          [loechel]
-        
-        - Feature: Add new CLI options for an output file and show release dates.
-          [loechel]
-        
-        1.5.1 (2017-01-23)
-        ------------------
-        
-        - Fix Version Compare.
-          [loechel]
-        
-        1.5.0 (2016-10-15)
-        ------------------
-        
-        - Development: Use code analysis for QA (and fix issues with pep8 et al.)
-          [jensens]
-        
-        - Fix: Manifest (jinja file was missing).
-          [jensens]
-        
-        - Feature: Implement #25: Annotate versions used.
-          [jensens]
-        
-        
-        1.4 (2016-09-30)
-        ----------------
-        
-        - Feature:
-          New option '-N': feature to hide orphaned without updates.
-          This reduces the noise in a environment where orphaned are used by intend.
-          [jensens]
-        
-        
-        1.3 (2016-05-19)
-        ----------------
-        
-        - Development: Add .editorconfig File to maintain code convetions following Plone API
-          [loechel]
-        
-        - Feature: Add Support for Python 3
-          [loechel]
-        
-        - Fix: Various documentation typos.
-          [jean]
-        
-        1.2.1 (2016-01-26)
-        ------------------
-        
-        - Feature: Cache buildout cfg files fetched over the network.
-          [jensens]
-        
-        - Feature: It caches now responses from PyPI.
-          [jensens]
-        
-        
-        1.1.2 (2016-01-21)
-        ------------------
-        
-        - Fix: Resolution order buildout extends chain was wrong. Also documented the
-          resolution order and included in own builodut a small example.
-          [jensens]
-        
-        - Fix: Formatter printed a newline to much after ``required by``.
-          [jensens]
-        
-        - Fix: Do not complain about missing track file.  If it is not there,
-          the buildout is simply not using the buildout extension.  [maurits]
-        
-        - Fix #13: Added missing ``zc.buildout`` requirement.  [maurits]
-        
-        
-        1.1.1 (2016-01-20)
-        ------------------
-        
-        - Fix: Orphan detection failed when no tracking file was present.
-          [jensens]
-        
-        - Fix: Exception raised when no tracking file was present.
-          [jensens]
-        
-        - Fix: Color of requirements was not set explicitly.
-          [jensens]
-        
-        
-        1.1 (2016-01-19)
-        ----------------
-        
-        - Enhancement: show requirements
-          [jensens]
-        
-        - Enhancement: machine readable output (json)
-          [jensens]
-        
-        - Enhancement: write pure processing-info output to sys.stderr
-          [jensens]
-        
-        - Fix #5 - Require setuptools>=12
-          [jensens]
-        
-        - Fix #7 - Available update from 'lazy' 1.0 to 1.2 is not found.
-          [jensens]
-        
-        - Enhancement: Rethink colors and document them, fixes #2 and #3.
-          [jensens]
-        
-        - Enhancement: display output and show tracked info
-          [jensens]
-        
-        - Feature: Add buildout extension to optional track required by and if its use at all
-          [jensens]
-        
-        
-        1.0 (2016-01-13)
-        ----------------
-        
-        - Initial work.
-          [jensens]
-        
 Keywords: plone buildout version
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Buildout :: Extension
 Classifier: Framework :: Buildout :: Recipe
 Classifier: Framework :: Buildout
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Quality Assurance
-Provides-Extra: develop
-Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: release
+Provides-Extra: test
+Provides-Extra: develop
+
+.. This README is meant for consumption by humans and PyPI.
+   PyPI can render rst files so please do not use Sphinx features.
+   If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
+   This text does not appear on PyPI or github.
+   It is a comment.
+
+
+=============================================================================
+Checks pinned versions with overrides in a cascaded buildout
+=============================================================================
+
+.. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
+    :target: https://travis-ci.org/plone/plone.versioncheck
+
+.. image:: https://coveralls.io/repos/github/plone/plone.versioncheck/badge.svg?branch=master
+   :target: https://coveralls.io/github/plone/plone.versioncheck?branch=master
+
+
+**plone.versioncheck**
+
+.. contents::
+
+Features
+========
+
+1) **Checks buildouts ``[versions]`` sections** while stepping through the cascaded ``extends``
+
+   - command line script collects the inherited version pins, remembers where a version pin comes from.
+   - It displays the result in order to enable a human to check that pins and overrides are OK.
+   - Output is colored; this helps to identify packages which have newer versions available.
+   - Machine readable output as JSON on demand.
+
+2) **Checks Python Package Index (PyPI)** for newer versions.
+
+   - Detects if a newer major, minor or bugfix (or a prerelease) is available.
+
+3) **Buildout extension** records the **current versions state** and **requirements**
+
+   - versions state and requirements are written to a file,
+   - versions from the file will be consumed by the command line tool
+       - orphaned version pins are detected,
+       - it shows which package pulled in another package as dependency.
+
+It works best with `semantically <http://semver.org/>`_ and only with `syntactically <https://setuptools.readthedocs.io/en/latest/setuptools.html#specifying-your-project-s-version>`_ correct version numbers!
+
+Usage
+=====
+
+Install with your buildout
+--------------------------
+
+Add a section to install it as a script and add it as an extension to your builodut::
+
+    [buildout]
+    ...
+    extensions =
+        plone.versioncheck
+
+    parts =
+        ...
+        ploneversioncheck
+        ...
+
+    ...
+
+    [ploneversioncheck]
+    recipe = zc.recipe.egg
+    eggs = plone.versioncheck
+
+    ...
+
+
+Run buildout as usual.
+
+Now a file ``.plone.versioncheck.tracked.json`` was generated in the buildout-directory.
+
+This file will be used by ``bin/versioncheck`` to figure out which packages were finally used.
+
+Run buildout again to regenerate this file.
+
+
+commandline
+-----------
+
+::
+
+  usage: versioncheck [-h] [-p] [-n] [-N] [-r] [-d] [-i] [-e EXCLUDE_CFG] [-m]
+                      [--no-cache] [-b] [-o [OUTPUT]] [--no-colors]
+                      [--debug-limit DEBUG_LIMIT]
+                      [buildout]
+
+  Fetch information about pinned versions and its overrides in simple and complex/cascaded buildouts.
+
+  positional arguments:
+    buildout              path to buildout.cfg or other *.cfg file
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -p, --pypi            check PyPI for newer versions
+    -n, --newer           display only packages with newer version than active
+    -N, --newer-orphaned  display orphaned packages only when newer versions
+                          available
+    -r, --required-by     show information about requirements (only if tracking
+                          file is available)
+    -d, --show-release-dates
+                          show information about release dates (only for package
+                          lookup from PyPI)
+    -i, --ignore-tracking
+                          ignore tracking file (if present)
+    -e EXCLUDE_CFG, --exclude-cfg EXCLUDE_CFG
+                          exclude in listing when cfg-filename pattern matches
+                          (fnmatch) the given expression
+    -m, --machine         show as machine readable output (json)
+    --no-cache            do not use a cache for PyPI
+    -b, --browser         show as html for webbrowser
+    -o [OUTPUT], --output [OUTPUT]
+                          safe output to output-file
+    --no-colors           do not show colors
+    --debug-limit DEBUG_LIMIT
+                          Limit the number of PyPI versions fetched for
+                          debugging
+
+  States and color codes:
+    [A]ctive (white)
+    [D]evelop (green)
+    [O]rphaned (magenta)
+    [I]nherited (older or same versions are gray, newer are yellow)
+    [U]pdate of final release on PyPI available (cyan)
+    [P]rerelease update on PyPI available (blue)
+    [X] unpinned (red)
+    [r] Requirement (gray)
+    [a] Annotation (gray)
+
+  Color of package name helps to indicate overall state of a package.
+
+
+Files created
+-------------
+
+If the script was used with the ``--pypi`` option, a directory ``.plone.versioncheck.cache`` will be created.
+It contains the cache of the requests to PyPI or external buildout configuration files.
+To clear the cache, remove the directory.
+The caching library uses the expiration headers of the response from PyPI, so even with cache it starts fetching new records.
+
+If the extension was used, a file ``.plone.versioncheck.tracked.json`` will be created.
+It contains the information from last buildout run.
+
+
+Output explained
+================
+
+Legend of states and colors
+---------------------------
+
+[D]evelopment Egg
+    A development egg is usually active.
+    Description shows location.
+    Color: Green
+
+[A]ctive Pin
+     Pinned version. Package is used and recent, all seems fine.
+     Color: White
+
+[I]nherited Pin
+     Unused pin. If older than active, the pin color is gray; if newer, it is yellow.
+
+[O]rphaned
+    If tracked, it shows whether the package in the given configuration was used at all.
+    Be careful with this information!
+    I.e. in a development buildout file, other packages are used than in a live or continuous integration buildout!
+    Color: Magenta
+
+[X] Unpinnend
+    Tracked, but no pin in ``[versions]`` sections were found.
+    Color: Red
+
+[U]pdate final release
+    At PyPI there is a newer final version available (major, minor or bugfix).
+    Descriptions shows on which level.
+    Color: Cyan
+
+[P]rerelease update
+    At PyPI there is a newer prerelease version available (major, minor or bugfix).
+    Descriptions shows on which level.
+    Only if there is no final release update available.
+    Color: Blue
+
+[r] Required by
+    If tracked and option ``--required-by`` was given, show packages this package is required by.
+    Valid for current active/used version.
+    Keep in mind this is based on the declared requirements, missing or implicit requirements are not covered.
+
+[a] Annotation
+    It is possible to annotate the reason why a version was chosen.
+    The information is parsed out of a section ``[versionannotations]``.
+    In this section  key is the name of the package and value the text annotations to be displayed.
+    The value can span more than one line using indent (as usal).
+
+
+Order of versions
+-----------------
+
+Order of versions is the buildout resolution order (how they are resolved by buildout in the extends chain/tree).
+After that, the PyPI releases are shown (major, minor, pre, then the prereleases)
+
+Example, given in each a version of ``my.pkg`` was declared:
+
+1. ``buildout.cfg`` with ``my.pkg=3.0.3``
+
+  1. ``buildout.cfg`` extends ``foo.cfg`` with ``my.pkg=3.0.1``
+
+  2. ``buildout.cfg`` extends ``bar.cfg`` with ``my.pkg=2.0``
+
+    2. ``foo cfg`` extends ``baz.cfg`` with ``my.pkg=3.1``
+
+2. found a newer versions at pypi
+
+  1. major ``my.pkg=4.0``
+
+  2. minor ``my.pkg=3.2``
+
+  3. major ``prerelease my.pkg=5.1b2``
+
+Output looks like so::
+
+    my.pkg
+        3.0.3............... A buildout.cfg
+        2.0 ................ I bar.cfg
+        3.0.1 .............. I foo.cfg
+        3.1 ................ I baz.cfg
+        4.0 ................ U Major
+        3.2 ................ U Minor
+        5.1b2............... P Majorpre
+
+
+
+Example
+-------
+
+Here w/o colors, run on ``buildout.coredev``::
+
+    $ ./bin/versioncheck -p buildout.cfg
+
+    accesscontrol
+        3.0.12 .... A versions.cfg
+        2.13.13 ... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
+    acquisition
+        4.2.2 ..... A versions.cfg
+        2.13.9 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
+    alabaster
+        0.7.7 ..... X unpinned
+    archetypes.multilingual
+        3.0.1 ..... A versions.cfg
+    archetypes.referencebrowserwidget
+        2.5.6 ..... A versions.cfg
+    archetypes.schemaextender
+        2.1.5 ..... A versions.cfg
+    argcomplete
+        1.0.0 ..... A tests.cfg
+    argh
+        0.26.1 .... A tests.cfg
+    argparse
+        (unset) ... A versions.cfg
+        1.1 ....... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
+        Can not check legacy version number.  U Error
+    autopep8
+        1.2.1 ..... A tests.cfg
+
+    [... skipped a bunch ...]
+
+    coverage
+        3.7.1 ..... A tests.cfg
+        3.5.2 ..... I http://dist.plone.org/versions/zopetoolkit-1-0-8-ztk-versions.cfg
+        4.0.3 ..... U Major
+        4.1b1 ..... P Majorpre
+    cssmin
+        0.2.0 ..... A versions.cfg
+    cssselect
+        0.9.1 ..... A versions.cfg
+    datetime
+        3.0.3 ..... A versions.cfg
+        2.12.8 .... I http://dist.plone.org/versions/zope-2-13-23-versions.cfg
+        4.0.1 ..... U Major
+    decorator
+        4.0.6 ..... A versions.cfg
+
+    [... skipped a bunch ...]
+
+    plone.app.textfield
+        1.2.6 ..... A versions.cfg
+    plone.app.theming
+        1.2.17.dev0  D /home/workspacejensens/coredev5/src/plone.app.theming/src
+        1.2.16 .... I versions.cfg
+    plone.app.tiles
+        2.1.0 ..... A versions.cfg
+        2.2.0 ..... U Minor
+
+    [... skipped a bunch ...]
+
+Source Code and Contributions
+=============================
+
+.. image:: https://travis-ci.org/plone/plone.versioncheck.svg?branch=master
+    :target: https://travis-ci.org/plone/plone.versioncheck
+
+If you want to help with the development (improvement, update, bug-fixing, ...) of ``plone.versioncheck`` this is a great idea!
+
+Please follow the `contribution guidelines <http://docs.plone.org/develop/coredev/docs/guidelines.html>`_.
+
+- `Source code at Github <https://github.com/plone/plone.versioncheck>`_
+- `Issue tracker at Github <https://github.com/plone/plone.versioncheck>`_
+
+Maintainer of ``plone.versioncheck`` is Jens Klein and the Plone contributors.
+We appreciate any contribution and if a release is needed to be done on PyPI, please just contact one of us (best by open an issue).
+
+Development
+===========
+
+There must be ``python`` with ``virtualenv`` and ``pip`` available in system path pointing to Python >=2.7.x
+Clone the project. Then::
+
+    $ bootstrap.sh
+
+For non-unix systems please read the contents of bootstrap.py and execute the steps manually adapted to your OS.
+
+License
+=======
+
+The project is licensed under the GPLv2.
+
+
+Changelog
+=========
+
+1.8.0 (2023-04-15)
+------------------
+
+- Ignore invalid versions.
+  Needed for ``setuptools`` 66 and higher when checking a package that has invalid versions on PyPI.
+  Fixes `issue 52 <https://github.com/plone/plone.versioncheck/issues/52>`_.
+  [maurits]
+
+
+1.7.0 (2019-03-08)
+------------------
+
+- Feature: Offers exclude pattern matching for cfg-files.
+  [jensens]
+
+- Use pure black as code style.
+  [jensens]
+
+- Test on Python 3.7
+  [jensens]
+
+- Fix PyPI url and add output of URL in case of a problem.
+  [jensens]
+
+
+1.6.10 (2018-08-20)
+-------------------
+
+- Fixes another bug in ``find_relative``.
+  [jensens]
+
+
+1.6.9 (2018-08-20)
+------------------
+
+- Fixes bug in ``find_relative`` introducued in last release.
+  [jensens]
+
+
+1.6.8 (2018-08-14)
+------------------
+
+Bug fixes:
+
+- Better handling of relative paths as entry, like ``project/foo/dev.cfg``.
+  [jensens]
+
+- If a file does not extend any other file,
+  the return statement was returning only one parameter,
+  while callers expected 2.
+  [gforcada]
+
+
+1.6.7 (2018-03-26)
+------------------
+
+Bug fixes:
+
+- Fix: Do not trust on setuptools internals.
+  Works now with newest setuptools.
+  [jensens]
+
+1.6.6 (2018-01-26)
+------------------
+
+- Fixed: Inherited extends with same name showed up as same.
+  Now show relative to basedir if possible, else full.
+  [jensens]
+
+- Fixed: Relative extends in urls were broken.
+  [jensens]
+
+
+1.6.5 (2017-07-03)
+------------------
+
+Bug fixes:
+
+- Relative Paths should work now, tested with subdirectories.
+  [loechel]
+
+
+1.6.4 (2017-05-08)
+------------------
+
+- Fix: Default versions section name ``versions`` was not respected.
+  [jensens]
+
+
+1.6.3 (2017-05-05)
+------------------
+
+- Fixes #17: Requirements were missing.
+  [jensens]
+
+- Optimization: Reduce load on PyPI when fetching release dates.
+  [jensens]
+
+- Feature: Change package and version fields in html output to links so that you could open pypi page for each package.
+  [loechel]
+
+
+1.6.2 (2017-04-12)
+------------------
+
+- Fix: Regressions with version-annotations and stdout messages from buildout parser.
+  [loechel]
+
+- Add more Tests
+  [loechel]
+
+1.6.1 (2017-04-07)
+------------------
+
+- Fix: #36 New buildout parser does not work with buildout.coredev
+  [loechel]
+
+1.6.0 (2017-04-07)
+------------------
+
+- Fix: ``IndexError: string index out of range`` error with empty states in the formatter.
+  [thet]
+
+- Development: Added basic tests to package.
+  [loechel]
+
+- Fix: Changed parser.py to use functions from zc.buildout to get versions and versionannotations section names.
+  [loechel]
+
+- Feature: Add function to extract date information from PyPI to analyze package age.
+  [loechel]
+
+- Feature: Add new CLI options for an output file and show release dates.
+  [loechel]
+
+1.5.1 (2017-01-23)
+------------------
+
+- Fix Version Compare.
+  [loechel]
+
+1.5.0 (2016-10-15)
+------------------
+
+- Development: Use code analysis for QA (and fix issues with pep8 et al.)
+  [jensens]
+
+- Fix: Manifest (jinja file was missing).
+  [jensens]
+
+- Feature: Implement #25: Annotate versions used.
+  [jensens]
+
+
+1.4 (2016-09-30)
+----------------
+
+- Feature:
+  New option '-N': feature to hide orphaned without updates.
+  This reduces the noise in a environment where orphaned are used by intend.
+  [jensens]
+
+
+1.3 (2016-05-19)
+----------------
+
+- Development: Add .editorconfig File to maintain code convetions following Plone API
+  [loechel]
+
+- Feature: Add Support for Python 3
+  [loechel]
+
+- Fix: Various documentation typos.
+  [jean]
+
+1.2.1 (2016-01-26)
+------------------
+
+- Feature: Cache buildout cfg files fetched over the network.
+  [jensens]
+
+- Feature: It caches now responses from PyPI.
+  [jensens]
+
+
+1.1.2 (2016-01-21)
+------------------
+
+- Fix: Resolution order buildout extends chain was wrong. Also documented the
+  resolution order and included in own builodut a small example.
+  [jensens]
+
+- Fix: Formatter printed a newline to much after ``required by``.
+  [jensens]
+
+- Fix: Do not complain about missing track file.  If it is not there,
+  the buildout is simply not using the buildout extension.  [maurits]
+
+- Fix #13: Added missing ``zc.buildout`` requirement.  [maurits]
+
+
+1.1.1 (2016-01-20)
+------------------
+
+- Fix: Orphan detection failed when no tracking file was present.
+  [jensens]
+
+- Fix: Exception raised when no tracking file was present.
+  [jensens]
+
+- Fix: Color of requirements was not set explicitly.
+  [jensens]
+
+
+1.1 (2016-01-19)
+----------------
+
+- Enhancement: show requirements
+  [jensens]
+
+- Enhancement: machine readable output (json)
+  [jensens]
+
+- Enhancement: write pure processing-info output to sys.stderr
+  [jensens]
+
+- Fix #5 - Require setuptools>=12
+  [jensens]
+
+- Fix #7 - Available update from 'lazy' 1.0 to 1.2 is not found.
+  [jensens]
+
+- Enhancement: Rethink colors and document them, fixes #2 and #3.
+  [jensens]
+
+- Enhancement: display output and show tracked info
+  [jensens]
+
+- Feature: Add buildout extension to optional track required by and if its use at all
+  [jensens]
+
+
+1.0 (2016-01-13)
+----------------
+
+- Initial work.
+  [jensens]
```

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/utils.py` & `plone.versioncheck-1.8.0/src/plone/versioncheck/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,15 @@
 def requests_session(nocache=False):
     if nocache:
         return requests.Session()
     return CacheControl(requests.Session(), cache=FileCache(CACHE_FILENAME))
 
 
 def find_relative(extend, relative=""):
-    """the base dir or url and the actual filename as tuple
-    """
+    """the base dir or url and the actual filename as tuple"""
     if "://" in extend:
         parts = list(urlparse(extend))
         path = parts[2].split("/")
         parts[2] = "/".join(path[:-1])
         return urlunparse(parts), path[-1]
     if "://" in relative:
         return (relative.strip("/"), extend.strip("/"))
@@ -94,19 +93,19 @@
 
 
 ###########################################################
 # below copied from https://gist.github.com/jtriley/1108174
 
 
 def get_terminal_size():
-    """ getTerminalSize()
-     - get width and height of console
-     - works on linux,os x,windows,cygwin(windows)
-     originally retrieved from:
-     http://stackoverflow.com/questions/566746/how-to-get-console-window-width-in-python
+    """getTerminalSize()
+    - get width and height of console
+    - works on linux,os x,windows,cygwin(windows)
+    originally retrieved from:
+    http://stackoverflow.com/questions/566746/how-to-get-console-window-width-in-python
     """
     current_os = platform.system()
     tuple_xy = None
     if current_os == "Windows":
         tuple_xy = _get_terminal_size_windows()
         if tuple_xy is None:
             tuple_xy = _get_terminal_size_tput()
@@ -116,15 +115,16 @@
     if tuple_xy is None:
         tuple_xy = (80, 25)  # default value
     return tuple_xy
 
 
 def _get_terminal_size_windows():
     try:
-        from ctypes import windll, create_string_buffer
+        from ctypes import create_string_buffer
+        from ctypes import windll
 
         # stdin handle is -10
         # stdout handle is -11
         # stderr handle is -12
         h = windll.kernel32.GetStdHandle(-12)
         csbi = create_string_buffer(22)
         res = windll.kernel32.GetConsoleScreenBufferInfo(h, csbi)
```

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/tracking.py` & `plone.versioncheck-1.8.0/src/plone/versioncheck/tracking.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/script.py` & `plone.versioncheck-1.8.0/src/plone/versioncheck/script.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/pypi.py` & `plone.versioncheck-1.8.0/src/plone/versioncheck/pypi.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,21 @@
         return False, str(resp.status_code)
     data = resp.json()
 
     # get information about possible updates
     releases = sorted(data["releases"])
     for release in releases:
         # major check (overall)
-        rel_v = parse_version(release)
+        try:
+            rel_v = parse_version(release)
+        except Exception:
+            # likely pkg_resources.extern.packaging.version.InvalidVersion
+            # but really any exception can be ignored.
+            # See https://github.com/plone/plone.versioncheck/issues/52
+            continue
         if rel_v <= version:
             continue
         rel_vtuple = mmbp_tuple(rel_v)
         rel_data = data["releases"][release]
         rel_date = datetime.date(1970, 1, 1)
         for rel_pkg in rel_data:
             time_string = rel_pkg.get("upload_time")
```

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/parser.py` & `plone.versioncheck-1.8.0/src/plone/versioncheck/parser.py`

 * *Files identical despite different names*

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/formatter.py` & `plone.versioncheck-1.8.0/src/plone/versioncheck/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function
+
 from collections import OrderedDict
 from fnmatch import fnmatch
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from plone.versioncheck import analyser
 from plone.versioncheck.utils import color_by_state
 from plone.versioncheck.utils import color_dimmed
```

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/analyser.py` & `plone.versioncheck-1.8.0/src/plone/versioncheck/analyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             vcur = parse_version(version)
         if idx == target_idx:
             return parse_version(version) > vcur
     return False
 
 
 def is_cfg_newer(pkginfo):
-    """ checks if one of the cfg is newer
+    """checks if one of the cfg is newer
 
     returns boolean
     """
     for idx in range(1, len(pkginfo)):
         if is_cfgidx_newer(pkginfo, idx):
             return True
```

### Comparing `plone.versioncheck-1.7.0/src/plone/versioncheck/tpl/browser.jinja` & `plone.versioncheck-1.8.0/src/plone/versioncheck/tpl/browser.jinja`

 * *Files identical despite different names*

