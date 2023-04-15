# Comparing `tmp/fmdt_python-0.0.8.tar.gz` & `tmp/fmdt_python-0.0.9.tar.gz`

## Comparing `fmdt_python-0.0.8.tar` & `fmdt_python-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/__init__.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/__test__.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/api.py
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/core.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/utils.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/LICENSE
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/../README.md
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 fmdt_python-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/__init__.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/__test__.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/api.py
+-rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/args.py
+-rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/core.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/utils.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/LICENSE
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/../README.md
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 fmdt_python-0.0.9/PKG-INFO
```

### Comparing `fmdt_python-0.0.8/__test__.py` & `fmdt_python-0.0.9/__test__.py`

 * *Files identical despite different names*

### Comparing `fmdt_python-0.0.8/core.py` & `fmdt_python-0.0.9/core.py`

 * *Files identical despite different names*

### Comparing `fmdt_python-0.0.8/utils.py` & `fmdt_python-0.0.9/utils.py`

 * *Files identical despite different names*

### Comparing `fmdt_python-0.0.8/LICENSE` & `fmdt_python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fmdt_python-0.0.8/pyproject.toml` & `fmdt_python-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fmdt-python"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Evan Voyles", email="ejovo13@yahoo.com" },
 ]
 description = "utlity functions for fast meteor detection toolbox"
 readme = "../README.md"
 requires-python = ">=3.7"
 dependencies = ["numpy", "ffmpeg-python"]
```

### Comparing `fmdt_python-0.0.8/../README.md` & `fmdt_python-0.0.9/../README.md`

 * *Files identical despite different names*

### Comparing `fmdt_python-0.0.8/PKG-INFO` & `fmdt_python-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmdt-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: utlity functions for fast meteor detection toolbox
 Project-URL: fmdt, https://github.com/alsoc/fmdt
 Project-URL: Homepage, https://github.com/ejovo13/fmdt_scripts
 Author-email: Evan Voyles <ejovo13@yahoo.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

