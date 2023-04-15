# Comparing `tmp/pymemuc-0.2.4.tar.gz` & `tmp/pymemuc-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.2.4.tar", max compression
+gzip compressed data, was "pymemuc-0.2.5.tar", max compression
```

## Comparing `pymemuc-0.2.4.tar` & `pymemuc-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-04-10 19:07:05.128549 pymemuc-0.2.4/LICENSE
--rw-r--r--   0        0        0     1577 2023-04-10 19:07:05.128549 pymemuc-0.2.4/README.md
--rw-r--r--   0        0        0      386 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/__init__.py
--rw-r--r--   0        0        0    22754 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_control.py
--rw-r--r--   0        0        0     1150 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_decorators.py
--rw-r--r--   0        0        0    12663 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_manage.py
--rw-r--r--   0        0        0     3937 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2194 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-04-10 19:07:05.132549 pymemuc-0.2.4/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1632 2023-04-10 19:07:25.492846 pymemuc-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 pymemuc-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-15 02:12:52.839467 pymemuc-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1580 2023-04-15 02:12:52.839467 pymemuc-0.2.5/README.md
+-rw-r--r--   0        0        0      386 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22754 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_control.py
+-rw-r--r--   0        0        0     1150 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    12663 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_manage.py
+-rw-r--r--   0        0        0     3938 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2194 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1655 2023-04-15 02:13:17.667534 pymemuc-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2432 1970-01-01 00:00:00.000000 pymemuc-0.2.5/PKG-INFO
```

### Comparing `pymemuc-0.2.4/LICENSE` & `pymemuc-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.4/README.md` & `pymemuc-0.2.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 See the [API documentation][full_doc].
 
 [python_link]: https://www.python.org/
 [pypi_link]: https://pypi.org/project/pymemuc/
 [codefactor_link]: https://www.codefactor.io/repository/github/marmig0404/pymemuc
 [memuc_docs]: https://www.memuplay.com/blog/memucommand-reference-manual.html
 [demo_notebook]: demo/demo.ipynb
-[full_doc]: https://pymemuc.readthedocs.io
+[full_doc]: https://pymemuc.martinmiglio.dev/
```

### Comparing `pymemuc-0.2.4/pymemuc/_command.py` & `pymemuc-0.2.5/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.4/pymemuc/_control.py` & `pymemuc-0.2.5/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.4/pymemuc/_decorators.py` & `pymemuc-0.2.5/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.4/pymemuc/_manage.py` & `pymemuc-0.2.5/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.4/pymemuc/_memuc.py` & `pymemuc-0.2.5/pymemuc/_memuc.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         args += "-t"
     if self.debug:
         print("pymemuc._memuc.memuc_run:")
         print(f"\tCommand: \"{' '.join(args)}\"")
     try:
         with Popen(
             args,
-            shell=True,
+            shell=False,
             stdout=PIPE,
             stderr=STDOUT,
             close_fds=True,
             universal_newlines=True,
         ) as process:
             try:
                 result, _ = process.communicate(timeout=timeout)
```

### Comparing `pymemuc-0.2.4/pymemuc/exceptions.py` & `pymemuc-0.2.5/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.4/pymemuc/pymemuc.py` & `pymemuc-0.2.5/pymemuc/pymemuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.4/pyproject.toml` & `pymemuc-0.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.2.4"
+version = "v0.2.5"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -33,14 +33,15 @@
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 sphinxext-opengraph = "^0.8.1"
 sphinx-autobuild = "^2021.3.14"
 sphinx-copybutton = "^0.5.1"
 furo = "^2023.3.27"
+sphinx-intl = "^2.1.0"
 
 
 [tool.poetry.group.tests.dependencies]
 twine = "^4.0.2"
 
 
 [tool.black]
```

### Comparing `pymemuc-0.2.4/PKG-INFO` & `pymemuc-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/marmig0404/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
@@ -63,9 +63,9 @@
 See the [API documentation][full_doc].
 
 [python_link]: https://www.python.org/
 [pypi_link]: https://pypi.org/project/pymemuc/
 [codefactor_link]: https://www.codefactor.io/repository/github/marmig0404/pymemuc
 [memuc_docs]: https://www.memuplay.com/blog/memucommand-reference-manual.html
 [demo_notebook]: demo/demo.ipynb
-[full_doc]: https://pymemuc.readthedocs.io
+[full_doc]: https://pymemuc.martinmiglio.dev/
```

