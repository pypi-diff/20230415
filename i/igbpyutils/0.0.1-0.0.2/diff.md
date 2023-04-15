# Comparing `tmp/igbpyutils-0.0.1.tar.gz` & `tmp/igbpyutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igbpyutils-0.0.1.tar", last modified: Fri Apr 14 19:42:32 2023, max compression
+gzip compressed data, was "igbpyutils-0.0.2.tar", last modified: Sat Apr 15 09:03:03 2023, max compression
```

## Comparing `igbpyutils-0.0.1.tar` & `igbpyutils-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:42:32.112809 igbpyutils-0.0.1/
--rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.1/LICENSE.txt
--rw-------   0 haukex    (1000) haukex    (1000)     2348 2023-04-14 19:42:32.112809 igbpyutils-0.0.1/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)     1622 2023-04-14 19:42:09.000000 igbpyutils-0.0.1/README.md
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:42:32.112809 igbpyutils-0.0.1/igbpyutils/
--rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.1/igbpyutils/__init__.py
--rw-------   0 haukex    (1000) haukex    (1000)     9115 2023-04-14 17:49:50.000000 igbpyutils-0.0.1/igbpyutils/file.py
--rw-------   0 haukex    (1000) haukex    (1000)     5456 2023-04-14 17:49:50.000000 igbpyutils-0.0.1/igbpyutils/iter.py
--rw-------   0 haukex    (1000) haukex    (1000)     1429 2023-04-14 19:21:32.000000 igbpyutils-0.0.1/igbpyutils/test.py
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:42:32.112809 igbpyutils-0.0.1/igbpyutils.egg-info/
--rw-------   0 haukex    (1000) haukex    (1000)     2348 2023-04-14 19:42:32.000000 igbpyutils-0.0.1/igbpyutils.egg-info/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)      309 2023-04-14 19:42:32.000000 igbpyutils-0.0.1/igbpyutils.egg-info/SOURCES.txt
--rw-------   0 haukex    (1000) haukex    (1000)        1 2023-04-14 19:42:32.000000 igbpyutils-0.0.1/igbpyutils.egg-info/dependency_links.txt
--rw-------   0 haukex    (1000) haukex    (1000)       11 2023-04-14 19:42:32.000000 igbpyutils-0.0.1/igbpyutils.egg-info/top_level.txt
--rw-------   0 haukex    (1000) haukex    (1000)      767 2023-04-14 18:24:40.000000 igbpyutils-0.0.1/pyproject.toml
--rw-------   0 haukex    (1000) haukex    (1000)       38 2023-04-14 19:42:32.112809 igbpyutils-0.0.1/setup.cfg
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:42:32.112809 igbpyutils-0.0.1/tests/
--rwx------   0 haukex    (1000) haukex    (1000)    11362 2023-04-14 19:26:52.000000 igbpyutils-0.0.1/tests/test_file.py
--rwx------   0 haukex    (1000) haukex    (1000)     9021 2023-04-14 19:25:57.000000 igbpyutils-0.0.1/tests/test_iter.py
--rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.1/tests/test_test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/
+-rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.2/LICENSE.txt
+-rw-------   0 haukex    (1000) haukex    (1000)     2222 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)     1496 2023-04-15 09:00:42.000000 igbpyutils-0.0.2/README.md
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/igbpyutils/
+-rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.2/igbpyutils/__init__.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5263 2023-04-15 08:15:49.000000 igbpyutils-0.0.2/igbpyutils/error.py
+-rw-------   0 haukex    (1000) haukex    (1000)     9115 2023-04-14 17:49:50.000000 igbpyutils-0.0.2/igbpyutils/file.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5456 2023-04-14 17:49:50.000000 igbpyutils-0.0.2/igbpyutils/iter.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1429 2023-04-14 19:21:32.000000 igbpyutils-0.0.2/igbpyutils/test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/igbpyutils.egg-info/
+-rw-------   0 haukex    (1000) haukex    (1000)     2222 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)      349 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/SOURCES.txt
+-rw-------   0 haukex    (1000) haukex    (1000)        1 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/dependency_links.txt
+-rw-------   0 haukex    (1000) haukex    (1000)       11 2023-04-15 09:03:03.000000 igbpyutils-0.0.2/igbpyutils.egg-info/top_level.txt
+-rw-------   0 haukex    (1000) haukex    (1000)      767 2023-04-15 08:41:35.000000 igbpyutils-0.0.2/pyproject.toml
+-rw-------   0 haukex    (1000) haukex    (1000)       38 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/setup.cfg
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-15 09:03:03.567283 igbpyutils-0.0.2/tests/
+-rwx------   0 haukex    (1000) haukex    (1000)     6413 2023-04-15 08:58:04.000000 igbpyutils-0.0.2/tests/test_error.py
+-rwx------   0 haukex    (1000) haukex    (1000)    11316 2023-04-15 08:18:39.000000 igbpyutils-0.0.2/tests/test_file.py
+-rwx------   0 haukex    (1000) haukex    (1000)     9021 2023-04-14 19:25:57.000000 igbpyutils-0.0.2/tests/test_iter.py
+-rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.2/tests/test_test.py
```

### Comparing `igbpyutils-0.0.1/LICENSE.txt` & `igbpyutils-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.1/PKG-INFO` & `igbpyutils-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igbpyutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Various Python Utilities
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Homepage, https://github.com/haukex/igbpyutils
 Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
@@ -17,31 +17,23 @@
 License-File: LICENSE.txt
 
 IGB Python Utilities
 ====================
 
 This is a collection of various Python tools, libraries, and utilities
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
-(IGB) in the Forschungsverbund Berlin e.V.
-Please see the individual files for documentation.
+(IGB) in the Forschungsverbund Berlin e.V. (<https://www.igb-berlin.de/en>).
+
+Please see the individual files in this project for documentation.
 
 This is a companion library to the `igbdatatools` library
 (<https://github.com/haukex/igbdatatools>) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
-cover a slightly broader range of Python versions.
-
-
-Internal Development Notes
---------------------------
-
-- Update version number everywhere, `git commit`
-- `git tag vX.X.X`, `git push --tags`
-- `python3 -m build`
-- `twine upload dist/igbpyutils-*.tar.gz`
+cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
 
 
 Author, Copyright, and License
 ------------------------------
 
 Copyright (c) 2022-2023 Hauke Daempfling <haukex@zero-g.net>
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
```

### Comparing `igbpyutils-0.0.1/README.md` & `igbpyutils-0.0.2/igbpyutils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+Metadata-Version: 2.1
+Name: igbpyutils
+Version: 0.0.2
+Summary: Various Python Utilities
+Author-email: Hauke D <haukex@zero-g.net>
+Project-URL: Homepage, https://github.com/haukex/igbpyutils
+Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 IGB Python Utilities
 ====================
 
 This is a collection of various Python tools, libraries, and utilities
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
-(IGB) in the Forschungsverbund Berlin e.V.
-Please see the individual files for documentation.
+(IGB) in the Forschungsverbund Berlin e.V. (<https://www.igb-berlin.de/en>).
+
+Please see the individual files in this project for documentation.
 
 This is a companion library to the `igbdatatools` library
 (<https://github.com/haukex/igbdatatools>) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
-cover a slightly broader range of Python versions.
-
-
-Internal Development Notes
---------------------------
-
-- Update version number everywhere, `git commit`
-- `git tag vX.X.X`, `git push --tags`
-- `python3 -m build`
-- `twine upload dist/igbpyutils-*.tar.gz`
+cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
 
 
 Author, Copyright, and License
 ------------------------------
 
 Copyright (c) 2022-2023 Hauke Daempfling <haukex@zero-g.net>
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
```

### Comparing `igbpyutils-0.0.1/igbpyutils/file.py` & `igbpyutils-0.0.2/igbpyutils/file.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.1/igbpyutils/iter.py` & `igbpyutils-0.0.2/igbpyutils/iter.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.1/igbpyutils/test.py` & `igbpyutils-0.0.2/igbpyutils/test.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.1/pyproject.toml` & `igbpyutils-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "igbpyutils"
 description = "Various Python Utilities"
-version = "0.0.1"
+version = "0.0.2"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
```

### Comparing `igbpyutils-0.0.1/tests/test_file.py` & `igbpyutils-0.0.2/tests/test_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             # noinspection PyTypeChecker
             tuple( to_Paths((123,)) )
 
     def test_autoglob(self):
         testpath = Path(__file__).parent
         testglob = str(testpath/'test_*.py')
         noglob = str(testpath/'zdoesntexist*')
-        files = sorted( str(p) for p in testpath.iterdir() if 'test_' in p.name and p.name.endswith('.py') )
-        self.assertTrue(len(files)==3)  # will need to be changed when we add new test files
+        files = sorted( str(p) for p in testpath.iterdir() if p.name.startswith('test_') and p.name.endswith('.py') )
+        self.assertTrue(len(files)>3)
         # this doesn't really test expanduser but that's ok
         self.assertEqual( files+[noglob], sorted(autoglob([testglob, noglob], force=True)) )
         self.assertEqual( files if sys.platform.startswith('win32') else [testglob], list(autoglob([testglob])) )
 
     def test_pushd(self):
         def realpath(pth):
             if sys.hexversion>=0x030A00F0:  # cover-not-3.9
```

### Comparing `igbpyutils-0.0.1/tests/test_iter.py` & `igbpyutils-0.0.2/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.1/tests/test_test.py` & `igbpyutils-0.0.2/tests/test_test.py`

 * *Files identical despite different names*

