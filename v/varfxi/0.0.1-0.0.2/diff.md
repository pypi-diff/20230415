# Comparing `tmp/varfxi-0.0.1.tar.gz` & `tmp/varfxi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varfxi-0.0.1.tar", max compression
+gzip compressed data, was "varfxi-0.0.2.tar", max compression
```

## Comparing `varfxi-0.0.1.tar` & `varfxi-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-03-14 06:10:54.473765 varfxi-0.0.1/LICENSE
--rw-r--r--   0        0        0     2131 2023-03-14 06:48:41.529526 varfxi-0.0.1/README.md
--rw-r--r--   0        0        0      665 2023-03-14 07:02:48.739901 varfxi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    54546 2023-03-14 06:10:55.421776 varfxi-0.0.1/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py
--rw-r--r--   0        0        0       23 2023-03-14 06:10:55.421776 varfxi-0.0.1/varfxi/__init__.py
--rw-r--r--   0        0        0    54546 2023-03-14 06:10:55.421776 varfxi-0.0.1/varfxi/distGARCH.py
--rw-r--r--   0        0        0    21321 2023-03-14 06:10:55.421776 varfxi-0.0.1/varfxi/joyplot2.py
--rw-r--r--   0        0        0    34634 2023-03-14 06:10:55.421776 varfxi-0.0.1/varfxi/quantileproj.py
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 varfxi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-14 06:10:54.473765 varfxi-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2131 2023-03-14 06:48:41.529526 varfxi-0.0.2/README.md
+-rw-r--r--   0        0        0     1148 2023-04-15 10:09:04.303637 varfxi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    99899 2023-04-15 09:29:45.646044 varfxi-0.0.2/varfxi/.ipynb_checkpoints/distGARCH-checkpoint.py
+-rw-r--r--   0        0        0       23 2023-03-14 06:10:55.421776 varfxi-0.0.2/varfxi/__init__.py
+-rw-r--r--   0        0        0    99899 2023-04-15 09:39:45.792298 varfxi-0.0.2/varfxi/distGARCH.py
+-rw-r--r--   0        0        0    21321 2023-03-14 06:10:55.421776 varfxi-0.0.2/varfxi/joyplot2.py
+-rw-r--r--   0        0        0    34634 2023-03-14 06:10:55.421776 varfxi-0.0.2/varfxi/quantileproj.py
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 varfxi-0.0.2/PKG-INFO
```

### Comparing `varfxi-0.0.1/LICENSE` & `varfxi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.1/README.md` & `varfxi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.1/pyproject.toml` & `varfxi-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,53 @@
 [tool.poetry]
 name = "varfxi"
-version = "0.0.1"
+version = "0.0.2"
 description = "Volatility based estimation for FX interventions"
 authors = ["romainlafarguette <romain.lafarguette@gmail.com>", "amineraboun <amineraboun@gmail.com>"]
+repository ="https://github.com/romainlafarguette/varfxi"
+homepage  ="https://github.com/romainlafarguette/varfxi"
+
 readme = "README.md"
+keywords = ["var", "garch"]
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 pandas = "^1.5.3"
 numpy = "^1.24.2"
 arch = "^5.3.1"
 matplotlib = "^3.7.1"
 
+# Dev dependencies
+seaborn = "^0.12.2"
+tqdm = "^4.65.0"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry.dev-dependencies]
+pytest = "^7.1.3"
+pytest-cov = "^3.0"
 
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = [
+    "tests",
+]
 
-[project.urls]
-"Homepage" = "https://github.com/romainlafarguette/varfxi"
+[tool.pylint]
+   [tool.pylint."FORMAT"]
+   max-line-length = 120
+   max-args = 5
+   
+# Documentation dependencies
+[tool.poetry.group.docs]
+optional = true
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^5.1.1"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `varfxi-0.0.1/varfxi/joyplot2.py` & `varfxi-0.0.2/varfxi/joyplot2.py`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.1/varfxi/quantileproj.py` & `varfxi-0.0.2/varfxi/quantileproj.py`

 * *Files identical despite different names*

### Comparing `varfxi-0.0.1/PKG-INFO` & `varfxi-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: varfxi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Volatility based estimation for FX interventions
+Home-page: https://github.com/romainlafarguette/varfxi
+Keywords: var,garch
 Author: romainlafarguette
 Author-email: romain.lafarguette@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: arch (>=5.3.1,<6.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Repository, https://github.com/romainlafarguette/varfxi
 Description-Content-Type: text/markdown
 
 VaR-Rule for FX Interventions
 ================================
 
 Link to the Python notebook: https://github.com/romainlafarguette/VaR-FX-Interventions/blob/master/notebooks/VaR-FX%20Interventions.ipynb
```

