# Comparing `tmp/pyapikey-0.0.2.tar.gz` & `tmp/pyapikey-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyapikey-0.0.2.tar", last modified: Fri Jul 31 02:15:11 2020, max compression
+gzip compressed data, was "pyapikey-0.0.4.tar", last modified: Sat Apr 15 11:38:43 2023, max compression
```

## Comparing `pyapikey-0.0.2.tar` & `pyapikey-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-31 02:15:11.079969 pyapikey-0.0.2/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-07-31 01:48:48.000000 pyapikey-0.0.2/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1399 2020-07-31 02:15:11.079969 pyapikey-0.0.2/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      315 2020-07-31 02:14:41.000000 pyapikey-0.0.2/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-31 02:15:11.078969 pyapikey-0.0.2/pyapikey/
--rw-r--r--   0 mark      (1000) mark      (1000)       34 2020-07-31 02:14:12.000000 pyapikey-0.0.2/pyapikey/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      210 2020-07-31 02:13:39.000000 pyapikey-0.0.2/pyapikey/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)       83 2020-07-31 02:14:41.000000 pyapikey-0.0.2/pyapikey/version.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-31 02:15:11.079969 pyapikey-0.0.2/pyapikey.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1399 2020-07-31 02:15:11.000000 pyapikey-0.0.2/pyapikey.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      262 2020-07-31 02:15:11.000000 pyapikey-0.0.2/pyapikey.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2020-07-31 02:15:11.000000 pyapikey-0.0.2/pyapikey.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       20 2020-07-31 02:15:11.000000 pyapikey-0.0.2/pyapikey.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2020-07-31 02:15:11.000000 pyapikey-0.0.2/pyapikey.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2020-07-31 02:15:11.079969 pyapikey-0.0.2/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1508 2020-07-31 02:14:41.000000 pyapikey-0.0.2/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:38:43.258311 pyapikey-0.0.4/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-15 11:29:31.000000 pyapikey-0.0.4/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-15 11:38:43.258311 pyapikey-0.0.4/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      390 2023-04-15 11:29:31.000000 pyapikey-0.0.4/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:38:43.257311 pyapikey-0.0.4/pyapikey/
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2020-10-02 10:21:11.000000 pyapikey-0.0.4/pyapikey/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1154 2023-04-15 11:38:14.000000 pyapikey-0.0.4/pyapikey/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      172 2023-04-15 11:29:31.000000 pyapikey-0.0.4/pyapikey/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-15 11:38:43.258311 pyapikey-0.0.4/pyapikey.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-15 11:38:43.000000 pyapikey-0.0.4/pyapikey.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      222 2023-04-15 11:38:43.000000 pyapikey-0.0.4/pyapikey.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-15 11:38:43.000000 pyapikey-0.0.4/pyapikey.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-15 11:38:43.000000 pyapikey-0.0.4/pyapikey.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-15 11:38:43.258311 pyapikey-0.0.4/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1351 2023-04-15 11:29:31.000000 pyapikey-0.0.4/setup.py
```

### Comparing `pyapikey-0.0.2/PKG-INFO` & `pyapikey-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyapikey
-Version: 0.0.2
+Version: 0.0.4
 Summary: access api keys from code
 Home-page: https://veltzer.github.io/pyapikey
+Download-URL: https://github.com/veltzer/pyapikey
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyapikey
-Description: ==========
-        *pyapikey*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pyapikey
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyapikey
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyapikey
-        
-        author: Mark Veltzer
-        
-        version: 0.0.2
-        
-        
-        
 Keywords: api,key,python,secret
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========
+*pyapikey*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pyapikey
+
+.. image:: https://img.shields.io/github/license/veltzer/pyapikey
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyapikey
+
+author: Mark Veltzer
+
+version: 0.0.4
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyapikey-0.0.2/pyapikey.egg-info/PKG-INFO` & `pyapikey-0.0.4/pyapikey.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyapikey
-Version: 0.0.2
+Version: 0.0.4
 Summary: access api keys from code
 Home-page: https://veltzer.github.io/pyapikey
+Download-URL: https://github.com/veltzer/pyapikey
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyapikey
-Description: ==========
-        *pyapikey*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pyapikey
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyapikey
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyapikey
-        
-        author: Mark Veltzer
-        
-        version: 0.0.2
-        
-        
-        
 Keywords: api,key,python,secret
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========
+*pyapikey*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pyapikey
+
+.. image:: https://img.shields.io/github/license/veltzer/pyapikey
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyapikey
+
+author: Mark Veltzer
+
+version: 0.0.4
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyapikey-0.0.2/setup.py` & `pyapikey-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,54 +5,45 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyapikey",
-    version="0.0.2",
+    version="0.0.4",
     packages=[
-        'pyapikey',
+        "pyapikey",
     ],
     # from here all is optional
     description="access api keys from code",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'api',
-        'key',
-        'python',
-        'secret',
+        "api",
+        "key",
+        "python",
+        "secret",
     ],
     url="https://veltzer.github.io/pyapikey",
     download_url="https://github.com/veltzer/pyapikey",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
-    install_requires=[
-    ],
-    extras_require={
-    },
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
-    ],
-    data_files=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
     ],
-    entry_points={"console_scripts": [
-    ]},
-    python_requires=">=3.6",
 )
```

