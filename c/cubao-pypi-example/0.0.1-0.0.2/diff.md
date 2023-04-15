# Comparing `tmp/cubao-pypi-example-0.0.1.tar.gz` & `tmp/cubao-pypi-example-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubao-pypi-example-0.0.1.tar", last modified: Sat Apr 15 12:22:01 2023, max compression
+gzip compressed data, was "cubao-pypi-example-0.0.2.tar", last modified: Sat Apr 15 12:48:43 2023, max compression
```

## Comparing `cubao-pypi-example-0.0.1.tar` & `cubao-pypi-example-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 tzx       (1000) tzx       (1000)        0 2023-04-15 12:22:01.628557 cubao-pypi-example-0.0.1/
--rw-rw-r--   0 tzx       (1000) tzx       (1000)     1426 2023-04-15 11:57:52.000000 cubao-pypi-example-0.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 tzx       (1000) tzx       (1000)     1081 2023-04-01 12:42:27.000000 cubao-pypi-example-0.0.1/LICENSE.txt
--rw-rw-r--   0 tzx       (1000) tzx       (1000)       32 2023-04-15 11:57:52.000000 cubao-pypi-example-0.0.1/MANIFEST.in
--rw-rw-r--   0 tzx       (1000) tzx       (1000)     1647 2023-04-15 11:58:57.000000 cubao-pypi-example-0.0.1/Makefile
--rw-rw-r--   0 tzx       (1000) tzx       (1000)     4320 2023-04-15 12:22:01.628557 cubao-pypi-example-0.0.1/PKG-INFO
--rw-rw-r--   0 tzx       (1000) tzx       (1000)     1842 2023-04-15 12:02:04.000000 cubao-pypi-example-0.0.1/README.md
--rw-rw-r--   0 tzx       (1000) tzx       (1000)     6194 2023-04-15 12:06:54.000000 cubao-pypi-example-0.0.1/pyproject.toml
--rw-rw-r--   0 tzx       (1000) tzx       (1000)       38 2023-04-15 12:22:01.628557 cubao-pypi-example-0.0.1/setup.cfg
-drwxrwxr-x   0 tzx       (1000) tzx       (1000)        0 2023-04-15 12:22:01.624557 cubao-pypi-example-0.0.1/src/
-drwxrwxr-x   0 tzx       (1000) tzx       (1000)        0 2023-04-15 12:22:01.628557 cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/
--rw-rw-r--   0 tzx       (1000) tzx       (1000)     4320 2023-04-15 12:22:01.000000 cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/PKG-INFO
--rw-rw-r--   0 tzx       (1000) tzx       (1000)      452 2023-04-15 12:22:01.000000 cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/SOURCES.txt
--rw-rw-r--   0 tzx       (1000) tzx       (1000)        1 2023-04-15 12:22:01.000000 cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/dependency_links.txt
--rw-rw-r--   0 tzx       (1000) tzx       (1000)       39 2023-04-15 12:22:01.000000 cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/entry_points.txt
--rw-rw-r--   0 tzx       (1000) tzx       (1000)       51 2023-04-15 12:22:01.000000 cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/requires.txt
--rw-rw-r--   0 tzx       (1000) tzx       (1000)        7 2023-04-15 12:22:01.000000 cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/top_level.txt
-drwxrwxr-x   0 tzx       (1000) tzx       (1000)        0 2023-04-15 12:22:01.628557 cubao-pypi-example-0.0.1/src/sample/
--rw-rw-r--   0 tzx       (1000) tzx       (1000)      111 2023-04-01 12:42:27.000000 cubao-pypi-example-0.0.1/src/sample/__init__.py
--rw-rw-r--   0 tzx       (1000) tzx       (1000)       10 2023-04-15 11:57:52.000000 cubao-pypi-example-0.0.1/src/sample/package_data.dat
--rw-rw-r--   0 tzx       (1000) tzx       (1000)       43 2023-04-01 12:42:27.000000 cubao-pypi-example-0.0.1/src/sample/simple.py
-drwxrwxr-x   0 tzx       (1000) tzx       (1000)        0 2023-04-15 12:22:01.628557 cubao-pypi-example-0.0.1/tests/
--rw-rw-r--   0 tzx       (1000) tzx       (1000)      416 2023-04-15 11:57:52.000000 cubao-pypi-example-0.0.1/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:48:43.511631 cubao-pypi-example-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-15 12:48:43.511631 cubao-pypi-example-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:48:43.511631 cubao-pypi-example-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:48:43.507631 cubao-pypi-example-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:48:43.507631 cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-15 12:48:43.000000 cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-15 12:48:43.000000 cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 12:48:43.000000 cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 12:48:43.000000 cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-15 12:48:43.000000 cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 12:48:43.000000 cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:48:43.511631 cubao-pypi-example-0.0.2/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:48:43.511631 cubao-pypi-example-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 12:48:31.000000 cubao-pypi-example-0.0.2/tests/test_simple.py
```

### Comparing `cubao-pypi-example-0.0.1/LICENSE.txt` & `cubao-pypi-example-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cubao-pypi-example-0.0.1/Makefile` & `cubao-pypi-example-0.0.2/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 clean:
 	rm -rf build dist *.egg-info __pycache__ *.pyc
 force_clean:
 	docker run --rm -v `pwd`:`pwd` -w `pwd` -it alpine/make make clean
 .PHONY: clean force_clean
 
+tox_check:
+	python -m tox -e py
+
 data_pull:
 	make pull -C data
 data_clean:
 	make clean -C data
 
 docs_build:
 	mkdocs build
```

### Comparing `cubao-pypi-example-0.0.1/PKG-INFO` & `cubao-pypi-example-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubao-pypi-example
-Version: 0.0.1
+Version: 0.0.2
 Summary: A sample Python project
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -20,19 +20,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/sampleproject/
+Project-URL: Homepage, https://github.com/cubao/cubao-pypi-example
+Project-URL: Bug Reports, https://github.com/cubao/cubao-pypi-example/issues
+Project-URL: Source, https://github.com/cubao/cubao-pypi-example/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cubao-pypi-example-0.0.1/README.md` & `cubao-pypi-example-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cubao-pypi-example-0.0.1/pyproject.toml` & `cubao-pypi-example-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "cubao-pypi-example"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.1"  # Required
+version = "0.0.2"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A sample Python project"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -126,19 +126,17 @@
 # https://packaging.python.org/specifications/core-metadata/#home-page-optional
 #
 # Examples listed include a pattern for specifying where the package tracks
 # issues, where the source is hosted, where to say thanks to the package
 # maintainers, and where to support the project financially. The key is
 # what's used to render the link text on PyPI.
 [project.urls]  # Optional
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Reports" = "https://github.com/pypa/sampleproject/issues"
-"Funding" = "https://donate.pypi.org"
-"Say Thanks!" = "http://saythanks.io/to/example"
-"Source" = "https://github.com/pypa/sampleproject/"
+"Homepage" = "https://github.com/cubao/cubao-pypi-example"
+"Bug Reports" = "https://github.com/cubao/cubao-pypi-example/issues"
+"Source" = "https://github.com/cubao/cubao-pypi-example/"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 sample = "sample:main"
 
 # This is configuration specific to the `setuptools` build backend.
```

### Comparing `cubao-pypi-example-0.0.1/src/cubao_pypi_example.egg-info/PKG-INFO` & `cubao-pypi-example-0.0.2/src/cubao_pypi_example.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubao-pypi-example
-Version: 0.0.1
+Version: 0.0.2
 Summary: A sample Python project
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -20,19 +20,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/sampleproject/
+Project-URL: Homepage, https://github.com/cubao/cubao-pypi-example
+Project-URL: Bug Reports, https://github.com/cubao/cubao-pypi-example/issues
+Project-URL: Source, https://github.com/cubao/cubao-pypi-example/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

