# Comparing `tmp/dtumathtools-1.0.4.tar.gz` & `tmp/dtumathtools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtumathtools-1.0.4.tar", last modified: Mon Apr 10 14:20:52 2023, max compression
+gzip compressed data, was "dtumathtools-1.0.5.tar", last modified: Sat Apr 15 12:29:47 2023, max compression
```

## Comparing `dtumathtools-1.0.4.tar` & `dtumathtools-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.551698 dtumathtools-1.0.4/
--rw-rw-rw-   0        0        0     1471 2023-01-29 21:40:49.000000 dtumathtools-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3541 2023-04-10 14:20:52.550698 dtumathtools-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2635 2023-01-29 21:46:36.000000 dtumathtools-1.0.4/README.md
--rw-rw-rw-   0        0        0     1162 2023-04-10 14:05:44.000000 dtumathtools-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 14:20:52.551698 dtumathtools-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.500700 dtumathtools-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.513696 dtumathtools-1.0.4/src/dtumathtools/
--rw-rw-rw-   0        0        0       84 2023-01-30 09:29:20.000000 dtumathtools-1.0.4/src/dtumathtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.541695 dtumathtools-1.0.4/src/dtumathtools/dtuplot/
--rw-rw-rw-   0        0        0      162 2023-03-19 12:43:03.000000 dtumathtools-1.0.4/src/dtumathtools/dtuplot/__init__.py
--rw-rw-rw-   0        0        0     6322 2022-12-23 22:17:04.000000 dtumathtools-1.0.4/src/dtumathtools/dtuplot/quiverplot.py
--rw-rw-rw-   0        0        0     2643 2022-12-23 23:07:43.000000 dtumathtools-1.0.4/src/dtumathtools/dtuplot/scatterplot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.546699 dtumathtools-1.0.4/src/dtumathtools/dtutools/
--rw-rw-rw-   0        0        0       73 2023-04-10 14:03:03.000000 dtumathtools-1.0.4/src/dtumathtools/dtutools/__init__.py
--rw-rw-rw-   0        0        0     3091 2023-04-10 14:15:11.000000 dtumathtools-1.0.4/src/dtumathtools/dtutools/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.536710 dtumathtools-1.0.4/src/dtumathtools.egg-info/
--rw-rw-rw-   0        0        0     3541 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 14:20:52.000000 dtumathtools-1.0.4/src/dtumathtools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 14:20:52.548696 dtumathtools-1.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-04-10 14:01:29.000000 dtumathtools-1.0.4/tests/test_dtuplot.py
--rw-rw-rw-   0        0        0     1802 2023-03-19 14:08:01.000000 dtumathtools-1.0.4/tests/test_dtutools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.555012 dtumathtools-1.0.5/
+-rw-rw-rw-   0        0        0     1471 2023-01-29 21:40:49.000000 dtumathtools-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3648 2023-04-15 12:29:47.553015 dtumathtools-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2635 2023-01-29 21:46:36.000000 dtumathtools-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 12:29:47.555012 dtumathtools-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1867 2023-04-15 12:25:48.000000 dtumathtools-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.423995 dtumathtools-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.444996 dtumathtools-1.0.5/src/dtumathtools/
+-rw-rw-rw-   0        0        0       84 2023-01-30 09:29:20.000000 dtumathtools-1.0.5/src/dtumathtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.530011 dtumathtools-1.0.5/src/dtumathtools/dtuplot/
+-rw-rw-rw-   0        0        0      203 2023-04-14 15:52:31.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/__init__.py
+-rw-rw-rw-   0        0        0     2766 2023-04-14 17:21:58.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/boundaryplot.py
+-rw-rw-rw-   0        0        0     6322 2022-12-23 22:17:04.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/quiverplot.py
+-rw-rw-rw-   0        0        0     2643 2022-12-23 23:07:43.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/scatterplot.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.535010 dtumathtools-1.0.5/src/dtumathtools/dtutools/
+-rw-rw-rw-   0        0        0       73 2023-04-10 14:03:03.000000 dtumathtools-1.0.5/src/dtumathtools/dtutools/__init__.py
+-rw-rw-rw-   0        0        0     3166 2023-04-14 15:52:31.000000 dtumathtools-1.0.5/src/dtumathtools/dtutools/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.517015 dtumathtools-1.0.5/src/dtumathtools.egg-info/
+-rw-rw-rw-   0        0        0     3648 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      533 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.551011 dtumathtools-1.0.5/tests/
+-rw-rw-rw-   0        0        0     1028 2023-04-14 17:06:37.000000 dtumathtools-1.0.5/tests/test_dtuplot.py
+-rw-rw-rw-   0        0        0     1802 2023-03-19 14:08:01.000000 dtumathtools-1.0.5/tests/test_dtutools.py
```

### Comparing `dtumathtools-1.0.4/LICENSE` & `dtumathtools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.4/PKG-INFO` & `dtumathtools-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: dtumathtools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark
-Author-email: Christian Mikkelstrup <s194345@student.dtu.dk>, Hans Henrik Hermansen <s194042@student.dtu.dk>
+Home-page: https://github.com/Chrillebon/DTUMathTools
+Author: Christian Mikkelstrup and Hans Henrik Hermansen
+Author-email: s194345@student.dtu.dk, s194042@student.dtu.dk
 License: BSD License (BSD)
-Project-URL: Homepage, https://github.com/Chrillebon/DTUMathTools
-Project-URL: Mathematics 1 homepage, https://01005.compute.dtu.dk/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: qt
+Provides-Extra: plotly
+Provides-Extra: ipympl
+Provides-Extra: mayavi
+Provides-Extra: bokeh
+Provides-Extra: k3d
+Provides-Extra: all
+Provides-Extra: dev
 License-File: LICENSE
 
 # DTUMathTools
 
 ## Description
 This package is a collection of easy-to-use commands for plotting using SymPy. It is designed to fit the requirements of *01005 - Advanced Mathematics in Engineering 1* course at the Technical University of Denmark, found [here](https://01005.compute.dtu.dk/). This includes, but is not limited to:
```

### Comparing `dtumathtools-1.0.4/README.md` & `dtumathtools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.4/pyproject.toml` & `dtumathtools-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,63 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+from setuptools import setup, find_packages
 
-[project]
-name = "dtumathtools"
-version = "1.0.4"
-authors = [
-    {name = "Christian Mikkelstrup", email = "s194345@student.dtu.dk"},
-    {name = "Hans Henrik Hermansen", email = "s194042@student.dtu.dk"},
-]
-description = "A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark"
-readme = "README.md"
-license = {'text' = "BSD License (BSD)"}
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
-    "License :: OSI Approved :: BSD License",
-    "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Education",
-    "Topic :: Education",
-    "Topic :: Scientific/Engineering :: Mathematics",
-]
-
-dependencies = [
-    "sympy-plot-backends>=1.6.6", 
+_minimal_deps = [
+    "sympy-plot-backends>=1.6.6,<=1.6.7",
     "sympy>=1.10.1", 
     "matplotlib>=3.2", 
     "jupyter>=1.0.0", 
-    "numpy>=1.21.1,<1.24"
+    "numpy>=1.21.1,<1.24",
+]
+
+_qt = ["PyQt5>=5.15.7"]
+_ipympl = ["ipympl>=0.7.0"]
+_plotly = ["plotly>=4.14.3"]
+_bokeh = ["panel>=0.13.0", "ipywidgets_bokeh"]
+_k3d = ["k3d>=2.9.7", "vtk"]
+_myavi = ["mayavi>=4.8.0"]
+
+_extra_deps = _qt+_ipympl+_plotly+_bokeh+_k3d+_myavi+[
+    "colorcet",
+    "scipy>=1.7.1",
+]
+
+_dev_deps = _extra_deps + [
+    "pytest",
+    "flake8",
 ]
 
-[project.urls]
-"Homepage" = "https://github.com/Chrillebon/DTUMathTools"
-"Mathematics 1 homepage" = "https://01005.compute.dtu.dk/"
+setup(
+    name="dtumathtools",
+    version="1.0.5",
+    author="Christian Mikkelstrup and Hans Henrik Hermansen",
+    author_email="s194345@student.dtu.dk, s194042@student.dtu.dk",
+    description="A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/Chrillebon/DTUMathTools",
+    license="BSD License (BSD)",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Education",
+        "Topic :: Education",
+        "Topic :: Scientific/Engineering :: Mathematics",
+    ],
+    packages=find_packages(where="src"),
+    package_dir={"": "src"},
+    include_package_data=True,
+    python_requires=">=3.8",
+    install_requires=_minimal_deps,
+    extras_require={
+        "qt": _qt,
+        "plotly": _plotly,
+        "ipympl": _ipympl,
+        "mayavi": _myavi,
+        "bokeh": _bokeh,
+        "k3d": _k3d,
+        "all": _extra_deps,
+        "dev": _dev_deps,
+    },
+)
```

### Comparing `dtumathtools-1.0.4/src/dtumathtools/dtuplot/quiverplot.py` & `dtumathtools-1.0.5/src/dtumathtools/dtuplot/quiverplot.py`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.4/src/dtumathtools/dtuplot/scatterplot.py` & `dtumathtools-1.0.5/src/dtumathtools/dtuplot/scatterplot.py`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.4/src/dtumathtools/dtutools/helpers.py` & `dtumathtools-1.0.5/src/dtumathtools/dtutools/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from sympy import *
+from sympy import dsolve as sym_dsolve
 from functools import reduce
 from typing import Union
 
 def _extract_vars(expr):
     return [e[1] for e in sorted(list(map(lambda x: (str(x),x), expr.free_symbols)))]
 
 
@@ -80,18 +81,18 @@
         ## Returns:
             sol: a dictionary containing solutions to 'ODE'
         
     """
     
     # Common problem for people is making an single equation, but with both sides
     # being Matrices. This alleviates that issue, and lets users think less
-    if type(ODE) == Eq and type(ODE.lhs) == type(ODE.rhs) == Matrix:
-            sol = dsolve(ODE.lhs - ODE.rhs, ics=ics)
+    if type(ODE) == Eq and isinstance(ODE.lhs, MatrixBase) and isinstance(ODE.rhs, MatrixBase):
+            sol = sym_dsolve(ODE.lhs - ODE.rhs, ics=ics)
     else:
-        sol = dsolve(ODE, ics=ics)
+        sol = sym_dsolve(ODE, ics=ics)
 
     return {eq.lhs : eq.rhs for eq in sol}
 
 
 def l2_norm( v: Matrix ):
     """ Computes the l2-norm for a Matrix-class object, without using
         absolute values on entries, for easier simplification and integration
```

### Comparing `dtumathtools-1.0.4/src/dtumathtools.egg-info/PKG-INFO` & `dtumathtools-1.0.5/src/dtumathtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: dtumathtools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark
-Author-email: Christian Mikkelstrup <s194345@student.dtu.dk>, Hans Henrik Hermansen <s194042@student.dtu.dk>
+Home-page: https://github.com/Chrillebon/DTUMathTools
+Author: Christian Mikkelstrup and Hans Henrik Hermansen
+Author-email: s194345@student.dtu.dk, s194042@student.dtu.dk
 License: BSD License (BSD)
-Project-URL: Homepage, https://github.com/Chrillebon/DTUMathTools
-Project-URL: Mathematics 1 homepage, https://01005.compute.dtu.dk/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: qt
+Provides-Extra: plotly
+Provides-Extra: ipympl
+Provides-Extra: mayavi
+Provides-Extra: bokeh
+Provides-Extra: k3d
+Provides-Extra: all
+Provides-Extra: dev
 License-File: LICENSE
 
 # DTUMathTools
 
 ## Description
 This package is a collection of easy-to-use commands for plotting using SymPy. It is designed to fit the requirements of *01005 - Advanced Mathematics in Engineering 1* course at the Technical University of Denmark, found [here](https://01005.compute.dtu.dk/). This includes, but is not limited to:
```

### Comparing `dtumathtools-1.0.4/tests/test_dtutools.py` & `dtumathtools-1.0.5/tests/test_dtutools.py`

 * *Files identical despite different names*

