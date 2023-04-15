# Comparing `tmp/grgrjax-0.4.1.tar.gz` & `tmp/grgrjax-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grgrjax-0.4.1.tar", last modified: Wed Mar 22 13:26:53 2023, max compression
+gzip compressed data, was "grgrjax-0.4.3.tar", last modified: Sat Apr 15 12:22:28 2023, max compression
```

## Comparing `grgrjax-0.4.1.tar` & `grgrjax-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.135577 grgrjax-0.4.1/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.122244 grgrjax-0.4.1/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.128911 grgrjax-0.4.1/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1239 2023-02-17 14:42:48.000000 grgrjax-0.4.1/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      175 2023-02-17 15:12:43.000000 grgrjax-0.4.1/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2023-02-16 13:40:07.000000 grgrjax-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      612 2023-02-18 14:43:16.000000 grgrjax-0.4.1/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-02-11 15:59:58.000000 grgrjax-0.4.1/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-03-22 13:26:53.135577 grgrjax-0.4.1/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      573 2023-03-04 11:00:53.000000 grgrjax-0.4.1/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.132244 grgrjax-0.4.1/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-02-11 15:59:58.000000 grgrjax-0.4.1/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.122244 grgrjax-0.4.1/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.132244 grgrjax-0.4.1/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-02-11 15:59:58.000000 grgrjax-0.4.1/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1614 2023-02-21 09:50:30.000000 grgrjax-0.4.1/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       97 2023-02-18 21:06:44.000000 grgrjax-0.4.1/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2023-02-11 15:59:58.000000 grgrjax-0.4.1/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       65 2023-02-18 15:27:02.000000 grgrjax-0.4.1/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.132244 grgrjax-0.4.1/grgrjax/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      461 2023-03-22 13:26:41.000000 grgrjax-0.4.1/grgrjax/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7782 2023-03-13 19:38:38.000000 grgrjax-0.4.1/grgrjax/helpers.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6365 2023-03-13 19:33:51.000000 grgrjax-0.4.1/grgrjax/newton.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      819 2023-02-17 14:08:34.000000 grgrjax-0.4.1/grgrjax/test_all.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-03-22 13:26:53.135577 grgrjax-0.4.1/grgrjax.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-03-22 13:26:52.000000 grgrjax-0.4.1/grgrjax.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      479 2023-03-22 13:26:53.000000 grgrjax-0.4.1/grgrjax.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-03-22 13:26:52.000000 grgrjax-0.4.1/grgrjax.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-03-22 13:26:52.000000 grgrjax-0.4.1/grgrjax.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        8 2023-03-22 13:26:52.000000 grgrjax-0.4.1/grgrjax.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-02-17 14:43:43.000000 grgrjax-0.4.1/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-03-22 13:26:53.135577 grgrjax-0.4.1/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      926 2023-02-17 14:42:55.000000 grgrjax-0.4.1/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.393202 grgrjax-0.4.3/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.383203 grgrjax-0.4.3/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.386536 grgrjax-0.4.3/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1221 2023-03-27 00:33:48.000000 grgrjax-0.4.3/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      175 2023-02-17 15:12:43.000000 grgrjax-0.4.3/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2023-02-16 13:40:07.000000 grgrjax-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      612 2023-02-18 14:43:16.000000 grgrjax-0.4.3/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-02-11 15:59:58.000000 grgrjax-0.4.3/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-04-15 12:22:28.393202 grgrjax-0.4.3/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      573 2023-03-04 11:00:53.000000 grgrjax-0.4.3/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.389869 grgrjax-0.4.3/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-02-11 15:59:58.000000 grgrjax-0.4.3/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.383203 grgrjax-0.4.3/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.389869 grgrjax-0.4.3/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-02-11 15:59:58.000000 grgrjax-0.4.3/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1614 2023-02-21 09:50:30.000000 grgrjax-0.4.3/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       97 2023-02-18 21:06:44.000000 grgrjax-0.4.3/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2023-02-11 15:59:58.000000 grgrjax-0.4.3/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       65 2023-02-18 15:27:02.000000 grgrjax-0.4.3/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.393202 grgrjax-0.4.3/grgrjax/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      476 2023-03-27 09:28:29.000000 grgrjax-0.4.3/grgrjax/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-04-15 12:22:20.000000 grgrjax-0.4.3/grgrjax/__version__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7782 2023-03-13 19:38:38.000000 grgrjax-0.4.3/grgrjax/helpers.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6323 2023-03-28 17:15:44.000000 grgrjax-0.4.3/grgrjax/newton.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      819 2023-02-17 14:08:34.000000 grgrjax-0.4.3/grgrjax/test_all.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:22:28.393202 grgrjax-0.4.3/grgrjax.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      985 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      502 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        8 2023-04-15 12:22:28.000000 grgrjax-0.4.3/grgrjax.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       11 2023-02-17 14:43:43.000000 grgrjax-0.4.3/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-04-15 12:22:28.393202 grgrjax-0.4.3/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1033 2023-03-27 09:28:05.000000 grgrjax-0.4.3/setup.py
```

### Comparing `grgrjax-0.4.1/.github/workflows/continuous-integration.yml` & `grgrjax-0.4.3/.github/workflows/continuous-integration.yml`

 * *Files 6% similar despite different names*

```diff
@@ -32,11 +32,11 @@
       run: |
         python -m pip install "jax[cpu]===0.3.25" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest
-        python -m pip install -r requirements.txt
+        python -m pip install .
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `grgrjax-0.4.1/.readthedocs.yaml` & `grgrjax-0.4.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/LICENSE` & `grgrjax-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/PKG-INFO` & `grgrjax-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grgrjax
-Version: 0.4.1
+Version: 0.4.3
 Summary: Some generic tools for JAX
 Home-page: https://github.com/gboehl/grgrjax
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `grgrjax-0.4.1/README.rst` & `grgrjax-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/docs/Makefile` & `grgrjax-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/docs/conf.py` & `grgrjax-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/docs/make.bat` & `grgrjax-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/grgrjax/helpers.py` & `grgrjax-0.4.3/grgrjax/helpers.py`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/grgrjax/newton.py` & `grgrjax-0.4.3/grgrjax/newton.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     xi_old = xi
     f, jac = func(xi)
     xi -= jax.scipy.linalg.solve(jac, f)
     eps = amax(xi-xi_old)
     return (xi, eps, cnt+1), (func, verbose, maxit, tol)
 
 
-def callback_func(cnt, err, fev=None, misc=None, ltime=None, verbose=True):
+def callback_func(cnt, err, *args, fev=None, ltime=None, verbose=True):
     """Print a formatted on-line update for a iterative process.
     """
     mess = f'    Iteration {cnt:2d}'
     if fev is not None:
         mess += f' | fev. {fev:3d}'
-    mess += f' | max. error {err:.2e}'
-    if misc is not None:
-        mess += f' | {misc[0]} {misc[1]:1.3f}'
+    mess += f' | error {err:.2e}'
+    for misc in args:
+        mess += misc
     if ltime is not None:
         mess += f' | lapsed {ltime:3.4f}s'
     if verbose:
         print(mess)
 
 
 @jax.jit
@@ -72,30 +72,30 @@
     return xi, func(xi), cnt, eps > tol
 
 
 def _perform_checks_newton(res, eps, cnt, jac_is_nan, tol, rtol, maxit):
 
     if jac_is_nan.any():
         res['success'] = False
-        res['message'] = "The Jacobian contains `NaN`s."
+        res['message'] = "The Jacobian contains NaNs."
         return True
 
     if eps < tol or eps < rtol:
         res['success'] = True
         res['message'] = "The solution converged."
         return True
 
     if cnt == maxit:
         res['success'] = False
         res['message'] = f"Maximum number of {maxit} iterations reached."
         return True
 
     if jnp.isnan(eps):
         res['success'] = False
-        res['message'] = f"Function returns 'NaN's"
+        res['message'] = f"Function returns NaNs"
         return True
 
     return False
 
 
 def newton_jax(func, init, maxit=30, tol=1e-8, rtol=None, solver=None, verbose=True, verbose_jac=False):
     """Newton method for root finding of `func` using automatic differenciation with jax. The argument `func` must be jittable with jax. `newton_jax` itself is not jittable, for this use `newton_jax_jit`.
```

### Comparing `grgrjax-0.4.1/grgrjax/test_all.py` & `grgrjax-0.4.3/grgrjax/test_all.py`

 * *Files identical despite different names*

### Comparing `grgrjax-0.4.1/grgrjax.egg-info/PKG-INFO` & `grgrjax-0.4.3/grgrjax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grgrjax
-Version: 0.4.1
+Version: 0.4.3
 Summary: Some generic tools for JAX
 Home-page: https://github.com/gboehl/grgrjax
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `grgrjax-0.4.1/setup.py` & `grgrjax-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
 from os import path
-from grgrjax import __version__
+
+# get version from dedicated version file
+version = {}
+with open("grgrjax/__version__.py") as fp:
+    exec(fp.read(), version)
 
 # read the contents of the README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/gboehl/grgrjax",
     name='grgrjax',
-    version=__version__,
+    version=version['__version__'],
     author='Gregor Boehl',
     author_email='admin@gregorboehl.com',
     license='MIT',
     description='Some generic tools for JAX',
     classifiers=[
             "License :: OSI Approved :: MIT License",
             "Programming Language :: Python :: 3",
```

