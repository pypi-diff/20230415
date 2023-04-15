# Comparing `tmp/subprocesskiller-0.10.tar.gz` & `tmp/subprocesskiller-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprocesskiller-0.10.tar", last modified: Sat Apr 15 09:54:44 2023, max compression
+gzip compressed data, was "subprocesskiller-0.11.tar", last modified: Sat Apr 15 10:04:37 2023, max compression
```

## Comparing `subprocesskiller-0.10.tar` & `subprocesskiller-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 09:54:44.687422 subprocesskiller-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-15 09:54:37.000000 subprocesskiller-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      153 2023-04-15 09:54:37.000000 subprocesskiller-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2911 2023-04-15 09:54:44.687422 subprocesskiller-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2220 2023-04-15 09:54:16.000000 subprocesskiller-0.10/README.md
--rw-rw-rw-   0        0        0       85 2023-04-15 09:54:44.687961 subprocesskiller-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-04-15 09:54:43.000000 subprocesskiller-0.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 09:54:44.683383 subprocesskiller-0.10/subprocesskiller/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 subprocesskiller-0.10/subprocesskiller/LICENSE
--rw-rw-rw-   0        0        0     2220 2023-04-15 09:54:16.000000 subprocesskiller-0.10/subprocesskiller/README.md
--rw-rw-rw-   0        0        0    11851 2023-04-15 09:47:56.000000 subprocesskiller-0.10/subprocesskiller/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-15 09:54:43.000000 subprocesskiller-0.10/subprocesskiller/requirements.txt
--rw-rw-rw-   0        0        0     2610 2023-04-15 09:54:43.000000 subprocesskiller-0.10/subprocesskiller/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-15 09:54:44.686376 subprocesskiller-0.10/subprocesskiller.egg-info/
--rw-rw-rw-   0        0        0     2911 2023-04-15 09:54:44.000000 subprocesskiller-0.10/subprocesskiller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-04-15 09:54:44.000000 subprocesskiller-0.10/subprocesskiller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 09:54:44.000000 subprocesskiller-0.10/subprocesskiller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-04-15 09:54:44.000000 subprocesskiller-0.10/subprocesskiller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-15 09:54:44.000000 subprocesskiller-0.10/subprocesskiller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 10:04:37.346209 subprocesskiller-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 10:04:30.000000 subprocesskiller-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      153 2023-04-15 10:04:29.000000 subprocesskiller-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2911 2023-04-15 10:04:37.346209 subprocesskiller-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2220 2023-04-15 09:54:16.000000 subprocesskiller-0.11/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-15 10:04:37.347206 subprocesskiller-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-04-15 10:04:36.000000 subprocesskiller-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:04:37.341222 subprocesskiller-0.11/subprocesskiller/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 subprocesskiller-0.11/subprocesskiller/LICENSE
+-rw-rw-rw-   0        0        0     2220 2023-04-15 09:54:16.000000 subprocesskiller-0.11/subprocesskiller/README.md
+-rw-rw-rw-   0        0        0    11851 2023-04-15 09:47:56.000000 subprocesskiller-0.11/subprocesskiller/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-04-15 10:04:36.000000 subprocesskiller-0.11/subprocesskiller/requirements.txt
+-rw-rw-rw-   0        0        0     2610 2023-04-15 10:04:36.000000 subprocesskiller-0.11/subprocesskiller/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 10:04:37.345211 subprocesskiller-0.11/subprocesskiller.egg-info/
+-rw-rw-rw-   0        0        0     2911 2023-04-15 10:04:37.000000 subprocesskiller-0.11/subprocesskiller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-04-15 10:04:37.000000 subprocesskiller-0.11/subprocesskiller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 10:04:37.000000 subprocesskiller-0.11/subprocesskiller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-15 10:04:37.000000 subprocesskiller-0.11/subprocesskiller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-15 10:04:37.000000 subprocesskiller-0.11/subprocesskiller.egg-info/top_level.txt
```

### Comparing `subprocesskiller-0.10/LICENSE.rst` & `subprocesskiller-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `subprocesskiller-0.10/PKG-INFO` & `subprocesskiller-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocesskiller
-Version: 0.10
+Version: 0.11
 Summary: Some functions for killing (sub)processes + children with ctypes - works with shell=True
 Home-page: https://github.com/hansalemaos/subprocesskiller
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pid,kill,subprocess,children,parents
 Classifier: Development Status :: 4 - Beta
```

### Comparing `subprocesskiller-0.10/README.md` & `subprocesskiller-0.11/README.md`

 * *Files identical despite different names*

### Comparing `subprocesskiller-0.10/setup.py` & `subprocesskiller-0.11/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Some functions for killing (sub)processes + children with ctypes - works with shell=True'''
 
 # Setting up
 setup(
     name="subprocesskiller",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/subprocesskiller',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
 long_description = long_description,
 long_description_content_type="text/markdown",
-    #packages=['comtypes', 'flatten_any_dict_iterable_or_whatsoever', 'hackyargparser', 'hackyargparser.egg', 'ordered_set', 'subprocess_alive', 'subprocess_alive.egg'],
+    #packages=['comtypes', 'flatten_any_dict_iterable_or_whatsoever', 'hackyargparser', 'ordered_set', 'subprocess_alive'],
     keywords=['pid', 'kill', 'subprocess', 'children', 'parents'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
-    install_requires=['comtypes', 'flatten_any_dict_iterable_or_whatsoever', 'hackyargparser', 'hackyargparser.egg', 'ordered_set', 'subprocess_alive', 'subprocess_alive.egg'],
+    install_requires=['comtypes', 'flatten_any_dict_iterable_or_whatsoever', 'hackyargparser', 'ordered_set', 'subprocess_alive'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

### Comparing `subprocesskiller-0.10/subprocesskiller/LICENSE` & `subprocesskiller-0.11/subprocesskiller/LICENSE`

 * *Files identical despite different names*

### Comparing `subprocesskiller-0.10/subprocesskiller/README.md` & `subprocesskiller-0.11/subprocesskiller/README.md`

 * *Files identical despite different names*

### Comparing `subprocesskiller-0.10/subprocesskiller/__init__.py` & `subprocesskiller-0.11/subprocesskiller/__init__.py`

 * *Files identical despite different names*

### Comparing `subprocesskiller-0.10/subprocesskiller/thirdparty.json` & `subprocesskiller-0.11/subprocesskiller/thirdparty.json`

 * *Files identical despite different names*

### Comparing `subprocesskiller-0.10/subprocesskiller.egg-info/PKG-INFO` & `subprocesskiller-0.11/subprocesskiller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocesskiller
-Version: 0.10
+Version: 0.11
 Summary: Some functions for killing (sub)processes + children with ctypes - works with shell=True
 Home-page: https://github.com/hansalemaos/subprocesskiller
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pid,kill,subprocess,children,parents
 Classifier: Development Status :: 4 - Beta
```

