# Comparing `tmp/navajo-0.4.0.tar.gz` & `tmp/navajo-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navajo-0.4.0.tar", last modified: Sat Apr 15 03:03:45 2023, max compression
+gzip compressed data, was "navajo-0.4.1.tar", last modified: Sat Apr 15 03:09:48 2023, max compression
```

## Comparing `navajo-0.4.0.tar` & `navajo-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:03:45.439557 navajo-0.4.0/
--rw-r--r--   0 albert     (501) staff       (20)      552 2023-04-15 01:39:13.000000 navajo-0.4.0/LICENSE.txt
--rw-r--r--   0 albert     (501) staff       (20)      644 2023-04-15 03:03:45.439437 navajo-0.4.0/PKG-INFO
--rw-r--r--   0 albert     (501) staff       (20)      499 2023-04-15 01:39:58.000000 navajo-0.4.0/README.md
--rw-r--r--   0 albert     (501) staff       (20)       38 2023-04-15 03:03:45.439589 navajo-0.4.0/setup.cfg
--rw-r--r--   0 albert     (501) staff       (20)      887 2023-04-15 01:45:24.000000 navajo-0.4.0/setup.py
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:03:45.436019 navajo-0.4.0/src/
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:03:45.437520 navajo-0.4.0/src/navajo/
--rw-r--r--   0 albert     (501) staff       (20)        0 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/__init__.py
--rw-r--r--   0 albert     (501) staff       (20)      382 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/asset.py
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:03:45.438293 navajo-0.4.0/src/navajo/assets/
--rw-r--r--   0 albert     (501) staff       (20)      150 2023-04-15 02:27:14.000000 navajo-0.4.0/src/navajo/assets/logo.txt
--rw-r--r--   0 albert     (501) staff       (20)        6 2023-04-15 03:02:34.000000 navajo-0.4.0/src/navajo/assets/version.txt
--rw-r--r--   0 albert     (501) staff       (20)     5661 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/backend.py
--rw-r--r--   0 albert     (501) staff       (20)      622 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/config.py
--rw-r--r--   0 albert     (501) staff       (20)     6366 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/filtration.py
--rw-r--r--   0 albert     (501) staff       (20)     6126 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/formatter.py
--rw-r--r--   0 albert     (501) staff       (20)     2277 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/index.py
--rw-r--r--   0 albert     (501) staff       (20)      749 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/logconf.py
--rw-r--r--   0 albert     (501) staff       (20)     3949 2023-04-15 02:30:14.000000 navajo-0.4.0/src/navajo/main.py
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:03:45.439305 navajo-0.4.0/src/navajo/server/
--rw-r--r--   0 albert     (501) staff       (20)        0 2023-04-15 01:43:39.000000 navajo-0.4.0/src/navajo/server/__init__.py
--rw-r--r--   0 albert     (501) staff       (20)     5953 2023-04-15 02:52:55.000000 navajo-0.4.0/src/navajo/server/api.py
--rw-r--r--   0 albert     (501) staff       (20)     9189 2023-04-15 01:48:16.000000 navajo-0.4.0/src/navajo/server/chat.py
--rw-r--r--   0 albert     (501) staff       (20)     1879 2023-04-15 01:48:25.000000 navajo-0.4.0/src/navajo/server/database.py
--rw-r--r--   0 albert     (501) staff       (20)     4048 2023-04-15 01:48:44.000000 navajo-0.4.0/src/navajo/server/dependency.py
--rw-r--r--   0 albert     (501) staff       (20)     9449 2023-04-15 02:47:58.000000 navajo-0.4.0/src/navajo/server/index.py
--rw-r--r--   0 albert     (501) staff       (20)     1477 2023-04-15 02:23:27.000000 navajo-0.4.0/src/navajo/server/logconf.py
--rw-r--r--   0 albert     (501) staff       (20)      468 2023-04-15 02:02:38.000000 navajo-0.4.0/src/navajo/server/prompt.py
--rw-r--r--   0 albert     (501) staff       (20)     4498 2023-04-15 03:00:59.000000 navajo-0.4.0/src/navajo/server/server.py
--rw-r--r--   0 albert     (501) staff       (20)     6179 2023-04-15 01:50:05.000000 navajo-0.4.0/src/navajo/server/split.py
--rw-r--r--   0 albert     (501) staff       (20)     1471 2023-04-15 01:40:36.000000 navajo-0.4.0/src/navajo/server/vector.py
--rw-r--r--   0 albert     (501) staff       (20)     1462 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/spinner.py
--rw-r--r--   0 albert     (501) staff       (20)     3772 2023-04-15 01:38:37.000000 navajo-0.4.0/src/navajo/subcommand.py
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:03:45.438101 navajo-0.4.0/src/navajo.egg-info/
--rw-r--r--   0 albert     (501) staff       (20)      644 2023-04-15 03:03:45.000000 navajo-0.4.0/src/navajo.egg-info/PKG-INFO
--rw-r--r--   0 albert     (501) staff       (20)      846 2023-04-15 03:03:45.000000 navajo-0.4.0/src/navajo.egg-info/SOURCES.txt
--rw-r--r--   0 albert     (501) staff       (20)        1 2023-04-15 03:03:45.000000 navajo-0.4.0/src/navajo.egg-info/dependency_links.txt
--rw-r--r--   0 albert     (501) staff       (20)       44 2023-04-15 03:03:45.000000 navajo-0.4.0/src/navajo.egg-info/entry_points.txt
--rw-r--r--   0 albert     (501) staff       (20)      145 2023-04-15 03:03:45.000000 navajo-0.4.0/src/navajo.egg-info/requires.txt
--rw-r--r--   0 albert     (501) staff       (20)        7 2023-04-15 03:03:45.000000 navajo-0.4.0/src/navajo.egg-info/top_level.txt
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:09:48.038324 navajo-0.4.1/
+-rw-r--r--   0 albert     (501) staff       (20)      552 2023-04-15 01:39:13.000000 navajo-0.4.1/LICENSE.txt
+-rw-r--r--   0 albert     (501) staff       (20)      644 2023-04-15 03:09:48.038193 navajo-0.4.1/PKG-INFO
+-rw-r--r--   0 albert     (501) staff       (20)      499 2023-04-15 01:39:58.000000 navajo-0.4.1/README.md
+-rw-r--r--   0 albert     (501) staff       (20)       38 2023-04-15 03:09:48.038362 navajo-0.4.1/setup.cfg
+-rw-r--r--   0 albert     (501) staff       (20)      907 2023-04-15 03:09:36.000000 navajo-0.4.1/setup.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:09:48.029742 navajo-0.4.1/src/
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:09:48.032976 navajo-0.4.1/src/navajo/
+-rw-r--r--   0 albert     (501) staff       (20)        0 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/__init__.py
+-rw-r--r--   0 albert     (501) staff       (20)      382 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/asset.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:09:48.034103 navajo-0.4.1/src/navajo/assets/
+-rw-r--r--   0 albert     (501) staff       (20)      150 2023-04-15 02:27:14.000000 navajo-0.4.1/src/navajo/assets/logo.txt
+-rw-r--r--   0 albert     (501) staff       (20)        6 2023-04-15 03:09:41.000000 navajo-0.4.1/src/navajo/assets/version.txt
+-rw-r--r--   0 albert     (501) staff       (20)     5661 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/backend.py
+-rw-r--r--   0 albert     (501) staff       (20)      622 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/config.py
+-rw-r--r--   0 albert     (501) staff       (20)     6366 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/filtration.py
+-rw-r--r--   0 albert     (501) staff       (20)     6126 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/formatter.py
+-rw-r--r--   0 albert     (501) staff       (20)     2277 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/index.py
+-rw-r--r--   0 albert     (501) staff       (20)      749 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/logconf.py
+-rw-r--r--   0 albert     (501) staff       (20)     3949 2023-04-15 02:30:14.000000 navajo-0.4.1/src/navajo/main.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:09:48.037454 navajo-0.4.1/src/navajo/server/
+-rw-r--r--   0 albert     (501) staff       (20)        0 2023-04-15 01:43:39.000000 navajo-0.4.1/src/navajo/server/__init__.py
+-rw-r--r--   0 albert     (501) staff       (20)     5953 2023-04-15 02:52:55.000000 navajo-0.4.1/src/navajo/server/api.py
+-rw-r--r--   0 albert     (501) staff       (20)     9189 2023-04-15 01:48:16.000000 navajo-0.4.1/src/navajo/server/chat.py
+-rw-r--r--   0 albert     (501) staff       (20)     1879 2023-04-15 01:48:25.000000 navajo-0.4.1/src/navajo/server/database.py
+-rw-r--r--   0 albert     (501) staff       (20)     4048 2023-04-15 01:48:44.000000 navajo-0.4.1/src/navajo/server/dependency.py
+-rw-r--r--   0 albert     (501) staff       (20)     9449 2023-04-15 02:47:58.000000 navajo-0.4.1/src/navajo/server/index.py
+-rw-r--r--   0 albert     (501) staff       (20)     1477 2023-04-15 02:23:27.000000 navajo-0.4.1/src/navajo/server/logconf.py
+-rw-r--r--   0 albert     (501) staff       (20)      468 2023-04-15 02:02:38.000000 navajo-0.4.1/src/navajo/server/prompt.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:09:48.038029 navajo-0.4.1/src/navajo/server/prompts/
+-rw-r--r--   0 albert     (501) staff       (20)      118 2023-04-15 01:40:36.000000 navajo-0.4.1/src/navajo/server/prompts/ack_block.txt
+-rw-r--r--   0 albert     (501) staff       (20)      121 2023-04-15 01:40:36.000000 navajo-0.4.1/src/navajo/server/prompts/ack_code.txt
+-rw-r--r--   0 albert     (501) staff       (20)      552 2023-04-15 01:40:36.000000 navajo-0.4.1/src/navajo/server/prompts/code_summary.txt
+-rw-r--r--   0 albert     (501) staff       (20)      446 2023-04-15 01:40:36.000000 navajo-0.4.1/src/navajo/server/prompts/system_query.txt
+-rw-r--r--   0 albert     (501) staff       (20)     4498 2023-04-15 03:00:59.000000 navajo-0.4.1/src/navajo/server/server.py
+-rw-r--r--   0 albert     (501) staff       (20)     6179 2023-04-15 01:50:05.000000 navajo-0.4.1/src/navajo/server/split.py
+-rw-r--r--   0 albert     (501) staff       (20)     1471 2023-04-15 01:40:36.000000 navajo-0.4.1/src/navajo/server/vector.py
+-rw-r--r--   0 albert     (501) staff       (20)     1462 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/spinner.py
+-rw-r--r--   0 albert     (501) staff       (20)     3772 2023-04-15 01:38:37.000000 navajo-0.4.1/src/navajo/subcommand.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-15 03:09:48.033790 navajo-0.4.1/src/navajo.egg-info/
+-rw-r--r--   0 albert     (501) staff       (20)      644 2023-04-15 03:09:47.000000 navajo-0.4.1/src/navajo.egg-info/PKG-INFO
+-rw-r--r--   0 albert     (501) staff       (20)     1011 2023-04-15 03:09:47.000000 navajo-0.4.1/src/navajo.egg-info/SOURCES.txt
+-rw-r--r--   0 albert     (501) staff       (20)        1 2023-04-15 03:09:47.000000 navajo-0.4.1/src/navajo.egg-info/dependency_links.txt
+-rw-r--r--   0 albert     (501) staff       (20)       44 2023-04-15 03:09:47.000000 navajo-0.4.1/src/navajo.egg-info/entry_points.txt
+-rw-r--r--   0 albert     (501) staff       (20)      145 2023-04-15 03:09:47.000000 navajo-0.4.1/src/navajo.egg-info/requires.txt
+-rw-r--r--   0 albert     (501) staff       (20)        7 2023-04-15 03:09:47.000000 navajo-0.4.1/src/navajo.egg-info/top_level.txt
```

### Comparing `navajo-0.4.0/LICENSE.txt` & `navajo-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/PKG-INFO` & `navajo-0.4.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navajo
-Version: 0.4.0
+Version: 0.4.1
 Summary: Talk to your code!
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # navajo
 
 Talk to your code!
```

### Comparing `navajo-0.4.0/setup.py` & `navajo-0.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
    name="navajo",
    version=get_version(),
    package_dir={'': 'src'},
    packages=find_packages(where='src'),
    description="Talk to your code!",
    long_description=long_description,
    long_description_content_type='text/markdown',
-   package_data={'navajo': ['assets/*']},
+   package_data={'navajo': ['assets/*', 'server/prompts/*']},
    install_requires=read_requirements(),
    entry_points={
       'console_scripts': [
          'navajo=navajo.main:main'
       ]
    }
 )
```

### Comparing `navajo-0.4.0/src/navajo/backend.py` & `navajo-0.4.1/src/navajo/backend.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/config.py` & `navajo-0.4.1/src/navajo/config.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/filtration.py` & `navajo-0.4.1/src/navajo/filtration.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/formatter.py` & `navajo-0.4.1/src/navajo/formatter.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/index.py` & `navajo-0.4.1/src/navajo/index.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/logconf.py` & `navajo-0.4.1/src/navajo/logconf.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/main.py` & `navajo-0.4.1/src/navajo/main.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/api.py` & `navajo-0.4.1/src/navajo/server/api.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/chat.py` & `navajo-0.4.1/src/navajo/server/chat.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/database.py` & `navajo-0.4.1/src/navajo/server/database.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/dependency.py` & `navajo-0.4.1/src/navajo/server/dependency.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/index.py` & `navajo-0.4.1/src/navajo/server/index.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/logconf.py` & `navajo-0.4.1/src/navajo/server/logconf.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/server.py` & `navajo-0.4.1/src/navajo/server/server.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/split.py` & `navajo-0.4.1/src/navajo/server/split.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/server/vector.py` & `navajo-0.4.1/src/navajo/server/vector.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/spinner.py` & `navajo-0.4.1/src/navajo/spinner.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo/subcommand.py` & `navajo-0.4.1/src/navajo/subcommand.py`

 * *Files identical despite different names*

### Comparing `navajo-0.4.0/src/navajo.egg-info/PKG-INFO` & `navajo-0.4.1/src/navajo.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navajo
-Version: 0.4.0
+Version: 0.4.1
 Summary: Talk to your code!
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # navajo
 
 Talk to your code!
```

