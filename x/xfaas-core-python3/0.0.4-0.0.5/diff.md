# Comparing `tmp/xfaas_core_python3-0.0.4.tar.gz` & `tmp/xfaas_core_python3-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfaas_core_python3-0.0.4.tar", last modified: Sun Mar 19 17:50:05 2023, max compression
+gzip compressed data, was "xfaas_core_python3-0.0.5.tar", last modified: Sat Apr 15 11:35:17 2023, max compression
```

## Comparing `xfaas_core_python3-0.0.4.tar` & `xfaas_core_python3-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-19 17:50:05.761234 xfaas_core_python3-0.0.4/
--rw-r--r--   0 paul       (501) staff       (20)     1073 2023-03-17 17:57:12.000000 xfaas_core_python3-0.0.4/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)     1038 2023-03-19 17:50:05.760995 xfaas_core_python3-0.0.4/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      503 2023-03-19 17:03:37.000000 xfaas_core_python3-0.0.4/README.md
--rw-r--r--   0 paul       (501) staff       (20)      522 2023-03-19 17:49:38.000000 xfaas_core_python3-0.0.4/pyproject.toml
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-03-19 17:50:05.761307 xfaas_core_python3-0.0.4/setup.cfg
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-19 17:50:05.758584 xfaas_core_python3-0.0.4/xfaas_core_python3/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-19 17:50:05.760664 xfaas_core_python3-0.0.4/xfaas_core_python3/adapter/
--rw-r--r--   0 paul       (501) staff       (20)        0 2023-03-19 16:59:54.000000 xfaas_core_python3-0.0.4/xfaas_core_python3/adapter/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      600 2023-03-19 17:48:52.000000 xfaas_core_python3-0.0.4/xfaas_core_python3/adapter/xfaas_entry.py
--rw-r--r--   0 paul       (501) staff       (20)      364 2023-03-19 17:47:24.000000 xfaas_core_python3-0.0.4/xfaas_core_python3/xfunction.py
--rw-r--r--   0 paul       (501) staff       (20)      976 2023-03-19 17:48:16.000000 xfaas_core_python3-0.0.4/xfaas_core_python3/xrunner.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-19 17:50:05.759992 xfaas_core_python3-0.0.4/xfaas_core_python3.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     1038 2023-03-19 17:50:05.000000 xfaas_core_python3-0.0.4/xfaas_core_python3.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      343 2023-03-19 17:50:05.000000 xfaas_core_python3-0.0.4/xfaas_core_python3.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-03-19 17:50:05.000000 xfaas_core_python3-0.0.4/xfaas_core_python3.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)       19 2023-03-19 17:50:05.000000 xfaas_core_python3-0.0.4/xfaas_core_python3.egg-info/top_level.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-15 11:35:17.772346 xfaas_core_python3-0.0.5/
+-rw-r--r--   0 paul       (501) staff       (20)     1073 2023-03-17 17:57:12.000000 xfaas_core_python3-0.0.5/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)     1038 2023-04-15 11:35:17.771795 xfaas_core_python3-0.0.5/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      503 2023-03-19 17:03:37.000000 xfaas_core_python3-0.0.5/README.md
+-rw-r--r--   0 paul       (501) staff       (20)      522 2023-04-15 11:35:09.000000 xfaas_core_python3-0.0.5/pyproject.toml
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-04-15 11:35:17.772707 xfaas_core_python3-0.0.5/setup.cfg
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-15 11:35:17.766534 xfaas_core_python3-0.0.5/xfaas_core_python3/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-15 11:35:17.770232 xfaas_core_python3-0.0.5/xfaas_core_python3/adapter/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2023-03-19 16:59:54.000000 xfaas_core_python3-0.0.5/xfaas_core_python3/adapter/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      600 2023-03-19 17:48:52.000000 xfaas_core_python3-0.0.5/xfaas_core_python3/adapter/xfaas_entry.py
+-rw-r--r--   0 paul       (501) staff       (20)      364 2023-03-19 17:47:24.000000 xfaas_core_python3-0.0.5/xfaas_core_python3/xfunction.py
+-rw-r--r--   0 paul       (501) staff       (20)     1059 2023-04-15 11:34:49.000000 xfaas_core_python3-0.0.5/xfaas_core_python3/xrunner.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-15 11:35:17.769555 xfaas_core_python3-0.0.5/xfaas_core_python3.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     1038 2023-04-15 11:35:17.000000 xfaas_core_python3-0.0.5/xfaas_core_python3.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      343 2023-04-15 11:35:17.000000 xfaas_core_python3-0.0.5/xfaas_core_python3.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-04-15 11:35:17.000000 xfaas_core_python3-0.0.5/xfaas_core_python3.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)       19 2023-04-15 11:35:17.000000 xfaas_core_python3-0.0.5/xfaas_core_python3.egg-info/top_level.txt
```

### Comparing `xfaas_core_python3-0.0.4/LICENSE` & `xfaas_core_python3-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xfaas_core_python3-0.0.4/PKG-INFO` & `xfaas_core_python3-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfaas_core_python3
-Version: 0.0.4
+Version: 0.0.5
 Summary: XFaaS package for Python3
 Author-email: Paul Wieland <paul.wieland@tum.de>
 Project-URL: Homepage, https://github.com/Function-Delivery-Network/FaaS-Shim
 Project-URL: Function Templates , https://github.com/paul-wie/xfaas-templates
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xfaas_core_python3-0.0.4/pyproject.toml` & `xfaas_core_python3-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xfaas_core_python3"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Paul Wieland", email="paul.wieland@tum.de" },
 ]
 description = "XFaaS package for Python3"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `xfaas_core_python3-0.0.4/xfaas_core_python3/adapter/xfaas_entry.py` & `xfaas_core_python3-0.0.5/xfaas_core_python3/adapter/xfaas_entry.py`

 * *Files identical despite different names*

### Comparing `xfaas_core_python3-0.0.4/xfaas_core_python3/xrunner.py` & `xfaas_core_python3-0.0.5/xfaas_core_python3/xrunner.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 # Required for Nuclio health check
 @app.route("/__internal/health")
 def nuclio_health():
     return app.make_response(("Ok", 200))
 
 
+@app.route("/live")
+def nuclio_live():
+    return app.make_response(("Ok", 200))
+
+
 def get_app(function: XFunction):
     global target_function
     target_function = function
     return app
 
 
 def run_app(function):
```

### Comparing `xfaas_core_python3-0.0.4/xfaas_core_python3.egg-info/PKG-INFO` & `xfaas_core_python3-0.0.5/xfaas_core_python3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfaas-core-python3
-Version: 0.0.4
+Version: 0.0.5
 Summary: XFaaS package for Python3
 Author-email: Paul Wieland <paul.wieland@tum.de>
 Project-URL: Homepage, https://github.com/Function-Delivery-Network/FaaS-Shim
 Project-URL: Function Templates , https://github.com/paul-wie/xfaas-templates
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

