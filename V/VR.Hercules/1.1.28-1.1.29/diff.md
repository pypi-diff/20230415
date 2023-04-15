# Comparing `tmp/VR.Hercules-1.1.28.tar.gz` & `tmp/VR.Hercules-1.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VR.Hercules-1.1.28.tar", last modified: Fri Jan 20 17:11:55 2023, max compression
+gzip compressed data, was "VR.Hercules-1.1.29.tar", last modified: Sat Apr 15 19:26:11 2023, max compression
```

## Comparing `VR.Hercules-1.1.28.tar` & `VR.Hercules-1.1.29.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.806572 VR.Hercules-1.1.28/
--rw-r--r--   0 root         (0) root         (0)     4588 2023-01-20 17:11:55.805572 VR.Hercules-1.1.28/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3585 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.795571 VR.Hercules-1.1.28/VR.Hercules.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4588 2023-01-20 17:11:55.000000 VR.Hercules-1.1.28/VR.Hercules.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1521 2023-01-20 17:11:55.000000 VR.Hercules-1.1.28/VR.Hercules.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-20 17:11:55.000000 VR.Hercules-1.1.28/VR.Hercules.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-20 17:11:55.000000 VR.Hercules-1.1.28/VR.Hercules.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-20 17:11:55.806572 VR.Hercules-1.1.28/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.790571 VR.Hercules-1.1.28/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.795571 VR.Hercules-1.1.28/tests/configuration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.796571 VR.Hercules-1.1.28/tests/configuration/hello_world/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/hello_world/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/hello_world/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/hello_world/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)     3122 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/hello_world/test_parse_punctuation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.797571 VR.Hercules-1.1.28/tests/configuration/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/parser/test_parse_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.798571 VR.Hercules-1.1.28/tests/configuration/printing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/printing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/printing/test_config_printing.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/tests/configuration/printing/test_recursive_object_printing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.799571 VR.Hercules-1.1.28/vr_hercules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.801571 VR.Hercules-1.1.28/vr_hercules/hello_world/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/hello_world/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/hello_world/config.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/hello_world/config_with_punctuation.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/hello_world/main.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/hello_world/parse_punctuation.py
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/hello_world/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/hello_world/punctuation_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.803572 VR.Hercules-1.1.28/vr_hercules/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/parser/_create_potentially_nested_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1252 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/parser/_create_type.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/parser/_sub_config_getting.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/parser/_type_class.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/parser/config_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/parser/enumeration_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.804572 VR.Hercules-1.1.28/vr_hercules/printing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/printing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/printing/configuration_printing.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/printing/recursive_dumping.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/printing/recursive_object_printing.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.805572 VR.Hercules-1.1.28/vr_hercules/shims/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/shims/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 17:11:55.805572 VR.Hercules-1.1.28/vr_hercules/shims/path/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/shims/path/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-01-20 17:11:47.000000 VR.Hercules-1.1.28/vr_hercules/shims/path/path_ensuring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.929924 VR.Hercules-1.1.29/
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-04-15 19:26:11.929924 VR.Hercules-1.1.29/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.918923 VR.Hercules-1.1.29/VR.Hercules.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-04-15 19:26:11.000000 VR.Hercules-1.1.29/VR.Hercules.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-04-15 19:26:11.000000 VR.Hercules-1.1.29/VR.Hercules.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 19:26:11.000000 VR.Hercules-1.1.29/VR.Hercules.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-15 19:26:11.000000 VR.Hercules-1.1.29/VR.Hercules.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 19:26:11.929924 VR.Hercules-1.1.29/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.914923 VR.Hercules-1.1.29/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.918923 VR.Hercules-1.1.29/tests/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.920923 VR.Hercules-1.1.29/tests/configuration/hello_world/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/hello_world/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/hello_world/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/hello_world/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3122 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/hello_world/test_parse_punctuation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.920923 VR.Hercules-1.1.29/tests/configuration/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/parser/test_parse_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.921923 VR.Hercules-1.1.29/tests/configuration/printing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/printing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/printing/test_config_printing.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/tests/configuration/printing/test_recursive_object_printing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.922923 VR.Hercules-1.1.29/vr_hercules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.924924 VR.Hercules-1.1.29/vr_hercules/hello_world/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/hello_world/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/hello_world/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/hello_world/config_with_punctuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/hello_world/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/hello_world/parse_punctuation.py
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/hello_world/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/hello_world/punctuation_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.926924 VR.Hercules-1.1.29/vr_hercules/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/parser/_create_potentially_nested_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/parser/_create_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/parser/_sub_config_getting.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/parser/_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/parser/config_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/parser/enumeration_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.927924 VR.Hercules-1.1.29/vr_hercules/printing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/printing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/printing/configuration_printing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/printing/recursive_dumping.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/printing/recursive_object_printing.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.928924 VR.Hercules-1.1.29/vr_hercules/shims/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/shims/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 19:26:11.928924 VR.Hercules-1.1.29/vr_hercules/shims/path/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/shims/path/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-04-15 19:26:02.000000 VR.Hercules-1.1.29/vr_hercules/shims/path/path_ensuring.py
```

### Comparing `VR.Hercules-1.1.28/PKG-INFO` & `VR.Hercules-1.1.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VR.Hercules
-Version: 1.1.28
+Version: 1.1.29
 Summary: A Configuration management system for Python projects.
 Home-page: https://gitlab.com/dfki/ra/ni/ol/iml/vr/vr.configuration/
 Author: Bengt Lüers
 Author-email: bengt.lueers@gmail.com
 Maintainer: Bengt Lüers
 Maintainer-email: bengt.lueers@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `VR.Hercules-1.1.28/README.md` & `VR.Hercules-1.1.29/README.md`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/VR.Hercules.egg-info/PKG-INFO` & `VR.Hercules-1.1.29/VR.Hercules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VR.Hercules
-Version: 1.1.28
+Version: 1.1.29
 Summary: A Configuration management system for Python projects.
 Home-page: https://gitlab.com/dfki/ra/ni/ol/iml/vr/vr.configuration/
 Author: Bengt Lüers
 Author-email: bengt.lueers@gmail.com
 Maintainer: Bengt Lüers
 Maintainer-email: bengt.lueers@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `VR.Hercules-1.1.28/VR.Hercules.egg-info/SOURCES.txt` & `VR.Hercules-1.1.29/VR.Hercules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/setup.py` & `VR.Hercules-1.1.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,9 +38,9 @@
     name='VR.Hercules',
     packages=find_packages(exclude=['test', 'tests']),
     package_data={
         '': ['py.typed'],
     },
     setup_requires=[
     ],
-    version='1.1.28',
+    version='1.1.29',
 )
```

### Comparing `VR.Hercules-1.1.28/tests/configuration/hello_world/test_parse_punctuation.py` & `VR.Hercules-1.1.29/tests/configuration/hello_world/test_parse_punctuation.py`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/tests/configuration/parser/test_parse_config.py` & `VR.Hercules-1.1.29/tests/configuration/parser/test_parse_config.py`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/vr_hercules/hello_world/config_with_punctuation.py` & `VR.Hercules-1.1.29/vr_hercules/hello_world/config_with_punctuation.py`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/vr_hercules/parser/_create_potentially_nested_type.py` & `VR.Hercules-1.1.29/vr_hercules/parser/_create_potentially_nested_type.py`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/vr_hercules/parser/_create_type.py` & `VR.Hercules-1.1.29/vr_hercules/parser/_create_type.py`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/vr_hercules/parser/config_parsing.py` & `VR.Hercules-1.1.29/vr_hercules/parser/config_parsing.py`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/vr_hercules/parser/enumeration_parsing.py` & `VR.Hercules-1.1.29/vr_hercules/parser/enumeration_parsing.py`

 * *Files identical despite different names*

### Comparing `VR.Hercules-1.1.28/vr_hercules/printing/recursive_dumping.py` & `VR.Hercules-1.1.29/vr_hercules/printing/recursive_dumping.py`

 * *Files identical despite different names*

