# Comparing `tmp/fastqueue-lib-0.0.1.tar.gz` & `tmp/fastqueue-lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastqueue-lib-0.0.1.tar", last modified: Sat Apr 15 06:19:04 2023, max compression
+gzip compressed data, was "fastqueue-lib-0.0.2.tar", last modified: Sat Apr 15 06:25:54 2023, max compression
```

## Comparing `fastqueue-lib-0.0.1.tar` & `fastqueue-lib-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:19:04.382896 fastqueue-lib-0.0.1/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     1096 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.1/LICENSE
--rwxrwxrwx   0 matt      (1000) matt      (1000)       34 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.1/MANIFEST.in
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3359 2023-04-15 06:19:04.375902 fastqueue-lib-0.0.1/PKG-INFO
--rwxrwxrwx   0 matt      (1000) matt      (1000)     2505 2023-04-15 05:12:12.000000 fastqueue-lib-0.0.1/README.md
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:19:04.270639 fastqueue-lib-0.0.1/fastqueue/
--rwxrwxrwx   0 matt      (1000) matt      (1000)       67 2023-04-15 04:39:02.000000 fastqueue-lib-0.0.1/fastqueue/__init__.py
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3238 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.1/fastqueue/prototypes.py
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:19:04.324949 fastqueue-lib-0.0.1/fastqueue_lib.egg-info/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3359 2023-04-15 06:19:04.000000 fastqueue-lib-0.0.1/fastqueue_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 matt      (1000) matt      (1000)      352 2023-04-15 06:19:04.000000 fastqueue-lib-0.0.1/fastqueue_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)        1 2023-04-15 06:19:04.000000 fastqueue-lib-0.0.1/fastqueue_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)       39 2023-04-15 06:19:04.000000 fastqueue-lib-0.0.1/fastqueue_lib.egg-info/requires.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)       21 2023-04-15 06:19:04.000000 fastqueue-lib-0.0.1/fastqueue_lib.egg-info/top_level.txt
--rwxrwxrwx   0 matt      (1000) matt      (1000)     1098 2023-04-15 06:17:35.000000 fastqueue-lib-0.0.1/pyproject.toml
--rwxrwxrwx   0 matt      (1000) matt      (1000)       38 2023-04-15 06:19:04.383892 fastqueue-lib-0.0.1/setup.cfg
--rwxrwxrwx   0 matt      (1000) matt      (1000)     1020 2023-04-15 04:36:07.000000 fastqueue-lib-0.0.1/setup.py
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:19:04.352927 fastqueue-lib-0.0.1/src/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     2341 2023-04-15 05:18:24.000000 fastqueue-lib-0.0.1/src/ccqueue.cpp
--rwxrwxrwx   0 matt      (1000) matt      (1000)     2177 2023-04-15 05:18:20.000000 fastqueue-lib-0.0.1/src/cllqueue.cpp
--rwxrwxrwx   0 matt      (1000) matt      (1000)    19493 2023-04-15 05:18:04.000000 fastqueue-lib-0.0.1/src/fastqueue.c
-drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:19:04.361918 fastqueue-lib-0.0.1/tests/
--rwxrwxrwx   0 matt      (1000) matt      (1000)     3303 2023-04-15 04:44:10.000000 fastqueue-lib-0.0.1/tests/test_queue.py
+drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.721992 fastqueue-lib-0.0.2/
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     1096 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.2/LICENSE
+-rwxrwxrwx   0 matt      (1000) matt      (1000)       34 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.2/MANIFEST.in
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     3374 2023-04-15 06:25:54.718995 fastqueue-lib-0.0.2/PKG-INFO
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     2520 2023-04-15 06:21:51.000000 fastqueue-lib-0.0.2/README.md
+drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.617101 fastqueue-lib-0.0.2/fastqueue/
+-rwxrwxrwx   0 matt      (1000) matt      (1000)       67 2023-04-15 04:39:02.000000 fastqueue-lib-0.0.2/fastqueue/__init__.py
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     3238 2023-04-15 02:43:14.000000 fastqueue-lib-0.0.2/fastqueue/prototypes.py
+drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.669049 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     3374 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 matt      (1000) matt      (1000)      352 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 matt      (1000) matt      (1000)        1 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 matt      (1000) matt      (1000)       39 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/requires.txt
+-rwxrwxrwx   0 matt      (1000) matt      (1000)       21 2023-04-15 06:25:54.000000 fastqueue-lib-0.0.2/fastqueue_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     1098 2023-04-15 06:25:02.000000 fastqueue-lib-0.0.2/pyproject.toml
+-rwxrwxrwx   0 matt      (1000) matt      (1000)       38 2023-04-15 06:25:54.721992 fastqueue-lib-0.0.2/setup.cfg
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     1020 2023-04-15 04:36:07.000000 fastqueue-lib-0.0.2/setup.py
+drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.697020 fastqueue-lib-0.0.2/src/
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     2341 2023-04-15 05:18:24.000000 fastqueue-lib-0.0.2/src/ccqueue.cpp
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     2177 2023-04-15 05:18:20.000000 fastqueue-lib-0.0.2/src/cllqueue.cpp
+-rwxrwxrwx   0 matt      (1000) matt      (1000)    19493 2023-04-15 05:18:04.000000 fastqueue-lib-0.0.2/src/fastqueue.c
+drwxrwxrwx   0 matt      (1000) matt      (1000)        0 2023-04-15 06:25:54.707007 fastqueue-lib-0.0.2/tests/
+-rwxrwxrwx   0 matt      (1000) matt      (1000)     3303 2023-04-15 04:44:10.000000 fastqueue-lib-0.0.2/tests/test_queue.py
```

### Comparing `fastqueue-lib-0.0.1/LICENSE` & `fastqueue-lib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.1/PKG-INFO` & `fastqueue-lib-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,18 +19,18 @@
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: tests
 License-File: LICENSE
 
 # fastqueue
 
-[![Tests](https://github.com/MatthewAndreTaylor/mqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/mqueue/actions)
-[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/mqueue/blob/master/pyproject.toml)
-[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/mqueue/blob/master/LICENSE)\
-[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/mqueue-lib/)
+[![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
+[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
+[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
+[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
 
 
 Single ended fast queue's built in C tuned for python.
 
 ## Requirements
 
 - `python 3.9+`
```

### Comparing `fastqueue-lib-0.0.1/README.md` & `fastqueue-lib-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # fastqueue
 
-[![Tests](https://github.com/MatthewAndreTaylor/mqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/mqueue/actions)
-[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/mqueue/blob/master/pyproject.toml)
-[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/mqueue/blob/master/LICENSE)\
-[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/mqueue-lib/)
+[![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
+[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
+[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
+[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
 
 
 Single ended fast queue's built in C tuned for python.
 
 ## Requirements
 
 - `python 3.9+`
```

### Comparing `fastqueue-lib-0.0.1/fastqueue/prototypes.py` & `fastqueue-lib-0.0.2/fastqueue/prototypes.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.1/fastqueue_lib.egg-info/PKG-INFO` & `fastqueue-lib-0.0.2/fastqueue_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,18 +19,18 @@
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: tests
 License-File: LICENSE
 
 # fastqueue
 
-[![Tests](https://github.com/MatthewAndreTaylor/mqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/mqueue/actions)
-[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/mqueue/blob/master/pyproject.toml)
-[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/mqueue/blob/master/LICENSE)\
-[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/mqueue-lib/)
+[![Tests](https://github.com/MatthewAndreTaylor/fastqueue/actions/workflows/tests.yml/badge.svg)](https://github.com/MatthewAndreTaylor/fastqueue/actions)
+[![PyPI Versions](https://img.shields.io/badge/python-3.9%2B-blue)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/pyproject.toml)
+[![PyPI license](https://img.shields.io/badge/license-MIT-%23373737)](https://github.com/MatthewAndreTaylor/fastqueue/blob/master/LICENSE)\
+[![PyPI](https://img.shields.io/badge/pypi-v0.0.1-blue)](https://pypi.org/project/fastqueue-lib/)
 
 
 Single ended fast queue's built in C tuned for python.
 
 ## Requirements
 
 - `python 3.9+`
```

### Comparing `fastqueue-lib-0.0.1/pyproject.toml` & `fastqueue-lib-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastqueue-lib"
-version = "0.0.1"
+version = "0.0.2"
 description="Fast single ended queue library for python"
 authors = [
     {name = "Matthew Taylor", email = "matthew.taylor.andre@gmail.com"},
 ]
 urls = {Homepage = "https://github.com/MatthewAndreTaylor/mqueue"}
 requires-python = ">=3.9"
 keywords = [ "Queue" ]
```

### Comparing `fastqueue-lib-0.0.1/setup.py` & `fastqueue-lib-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.1/src/ccqueue.cpp` & `fastqueue-lib-0.0.2/src/ccqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.1/src/cllqueue.cpp` & `fastqueue-lib-0.0.2/src/cllqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.1/src/fastqueue.c` & `fastqueue-lib-0.0.2/src/fastqueue.c`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.1/tests/test_queue.py` & `fastqueue-lib-0.0.2/tests/test_queue.py`

 * *Files identical despite different names*

