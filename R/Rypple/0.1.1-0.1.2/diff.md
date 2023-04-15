# Comparing `tmp/Rypple-0.1.1.tar.gz` & `tmp/Rypple-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Rypple-0.1.1.tar", last modified: Sat Apr 15 17:32:41 2023, max compression
+gzip compressed data, was "Rypple-0.1.2.tar", last modified: Sat Apr 15 18:07:58 2023, max compression
```

## Comparing `Rypple-0.1.1.tar` & `Rypple-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 17:32:41.947087 Rypple-0.1.1/
--rw-rw-rw-   0        0        0    35826 2023-04-15 17:04:00.000000 Rypple-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      327 2023-04-15 17:32:41.946106 Rypple-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-15 16:47:53.000000 Rypple-0.1.1/README.md
--rw-rw-rw-   0        0        0      477 2023-04-15 17:32:15.000000 Rypple-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 17:32:41.947087 Rypple-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 17:32:41.861089 Rypple-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:32:41.907086 Rypple-0.1.1/src/Rypple/
--rw-rw-rw-   0        0        0     5890 2023-04-03 03:06:07.000000 Rypple-0.1.1/src/Rypple/__init__.py
--rw-rw-rw-   0        0        0      754 2023-02-13 21:45:33.000000 Rypple-0.1.1/src/Rypple/decorators.py
--rw-rw-rw-   0        0        0     1826 2023-02-21 15:11:36.000000 Rypple-0.1.1/src/Rypple/exceptions.py
--rw-rw-rw-   0        0        0     1321 2023-02-15 02:18:36.000000 Rypple-0.1.1/src/Rypple/extension.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:32:41.922087 Rypple-0.1.1/src/Rypple/extensions/
--rw-rw-rw-   0        0        0      601 2023-03-09 17:00:10.000000 Rypple-0.1.1/src/Rypple/extensions/console.py
--rw-rw-rw-   0        0        0    10295 2023-02-27 16:40:42.000000 Rypple-0.1.1/src/Rypple/extensions/core.py
--rw-rw-rw-   0        0        0     1195 2023-03-09 17:12:06.000000 Rypple-0.1.1/src/Rypple/extensions/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:32:41.943087 Rypple-0.1.1/src/Rypple/extensions/rypile/
--rw-rw-rw-   0        0        0     1965 2023-03-01 03:36:42.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/c#.py
--rw-rw-rw-   0        0        0      565 2023-02-27 16:41:51.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/c++.py
--rw-rw-rw-   0        0        0     5865 2023-02-27 14:28:54.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/c.py
--rw-rw-rw-   0        0        0     6100 2023-03-03 21:44:43.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/core.py
--rw-rw-rw-   0        0        0     1220 2023-03-09 16:48:10.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/gradle.py
--rw-rw-rw-   0        0        0      987 2023-02-27 16:42:32.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/java.py
--rw-rw-rw-   0        0        0      993 2023-02-27 16:43:00.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/javascript.py
--rw-rw-rw-   0        0        0      991 2023-02-27 17:00:07.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/kotlin.py
--rw-rw-rw-   0        0        0      985 2023-02-27 16:50:20.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/lua.py
--rw-rw-rw-   0        0        0     1028 2023-02-27 15:25:35.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/msbuild.py
--rw-rw-rw-   0        0        0     3970 2023-03-03 21:49:34.000000 Rypple-0.1.1/src/Rypple/extensions/rypile/python.py
--rw-rw-rw-   0        0        0     5675 2023-04-02 22:06:33.000000 Rypple-0.1.1/src/Rypple/namespace.py
--rw-rw-rw-   0        0        0    11650 2023-02-28 14:06:35.000000 Rypple-0.1.1/src/Rypple/scope.py
--rw-rw-rw-   0        0        0     3766 2023-03-03 22:56:20.000000 Rypple-0.1.1/src/Rypple/step.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:32:41.917088 Rypple-0.1.1/src/Rypple.egg-info/
--rw-rw-rw-   0        0        0      327 2023-04-15 17:32:41.000000 Rypple-0.1.1/src/Rypple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-04-15 17:32:41.000000 Rypple-0.1.1/src/Rypple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 17:32:41.000000 Rypple-0.1.1/src/Rypple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 17:32:41.000000 Rypple-0.1.1/src/Rypple.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:07:58.317837 Rypple-0.1.2/
+-rw-rw-rw-   0        0        0    35826 2023-04-15 17:04:00.000000 Rypple-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      327 2023-04-15 18:07:58.316909 Rypple-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:47:53.000000 Rypple-0.1.2/README.md
+-rw-rw-rw-   0        0        0      503 2023-04-15 18:07:31.000000 Rypple-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:07:58.317837 Rypple-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 18:07:58.254815 Rypple-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:07:58.275811 Rypple-0.1.2/src/Rypple/
+-rw-rw-rw-   0        0        0     5890 2023-04-03 03:06:07.000000 Rypple-0.1.2/src/Rypple/__init__.py
+-rw-rw-rw-   0        0        0      754 2023-02-13 21:45:33.000000 Rypple-0.1.2/src/Rypple/decorators.py
+-rw-rw-rw-   0        0        0     1826 2023-02-21 15:11:36.000000 Rypple-0.1.2/src/Rypple/exceptions.py
+-rw-rw-rw-   0        0        0     1321 2023-02-15 02:18:36.000000 Rypple-0.1.2/src/Rypple/extension.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:07:58.294808 Rypple-0.1.2/src/Rypple/extensions/
+-rw-rw-rw-   0        0        0      601 2023-03-09 17:00:10.000000 Rypple-0.1.2/src/Rypple/extensions/console.py
+-rw-rw-rw-   0        0        0    10295 2023-02-27 16:40:42.000000 Rypple-0.1.2/src/Rypple/extensions/core.py
+-rw-rw-rw-   0        0        0     1195 2023-03-09 17:12:06.000000 Rypple-0.1.2/src/Rypple/extensions/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:07:58.313809 Rypple-0.1.2/src/Rypple/extensions/rypile/
+-rw-rw-rw-   0        0        0     1965 2023-03-01 03:36:42.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/c#.py
+-rw-rw-rw-   0        0        0      565 2023-02-27 16:41:51.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/c++.py
+-rw-rw-rw-   0        0        0     5865 2023-02-27 14:28:54.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/c.py
+-rw-rw-rw-   0        0        0     6100 2023-03-03 21:44:43.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/core.py
+-rw-rw-rw-   0        0        0     1220 2023-03-09 16:48:10.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/gradle.py
+-rw-rw-rw-   0        0        0      987 2023-02-27 16:42:32.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/java.py
+-rw-rw-rw-   0        0        0      993 2023-02-27 16:43:00.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/javascript.py
+-rw-rw-rw-   0        0        0      991 2023-02-27 17:00:07.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/kotlin.py
+-rw-rw-rw-   0        0        0      985 2023-02-27 16:50:20.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/lua.py
+-rw-rw-rw-   0        0        0     1028 2023-02-27 15:25:35.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/msbuild.py
+-rw-rw-rw-   0        0        0     3970 2023-03-03 21:49:34.000000 Rypple-0.1.2/src/Rypple/extensions/rypile/python.py
+-rw-rw-rw-   0        0        0     5675 2023-04-02 22:06:33.000000 Rypple-0.1.2/src/Rypple/namespace.py
+-rw-rw-rw-   0        0        0    11650 2023-02-28 14:06:35.000000 Rypple-0.1.2/src/Rypple/scope.py
+-rw-rw-rw-   0        0        0     3766 2023-03-03 22:56:20.000000 Rypple-0.1.2/src/Rypple/step.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:07:58.289845 Rypple-0.1.2/src/Rypple.egg-info/
+-rw-rw-rw-   0        0        0      327 2023-04-15 18:07:58.000000 Rypple-0.1.2/src/Rypple.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      875 2023-04-15 18:07:58.000000 Rypple-0.1.2/src/Rypple.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:07:58.000000 Rypple-0.1.2/src/Rypple.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-15 18:07:58.000000 Rypple-0.1.2/src/Rypple.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 18:07:58.000000 Rypple-0.1.2/src/Rypple.egg-info/top_level.txt
```

### Comparing `Rypple-0.1.1/LICENSE` & `Rypple-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/__init__.py` & `Rypple-0.1.2/src/Rypple/__init__.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/decorators.py` & `Rypple-0.1.2/src/Rypple/decorators.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/exceptions.py` & `Rypple-0.1.2/src/Rypple/exceptions.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extension.py` & `Rypple-0.1.2/src/Rypple/extension.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/console.py` & `Rypple-0.1.2/src/Rypple/extensions/console.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/core.py` & `Rypple-0.1.2/src/Rypple/extensions/core.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/filesystem.py` & `Rypple-0.1.2/src/Rypple/extensions/filesystem.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/c#.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/c#.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/c++.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/c++.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/c.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/c.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/core.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/core.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/gradle.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/gradle.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/java.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/java.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/javascript.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/javascript.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/kotlin.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/kotlin.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/lua.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/lua.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/msbuild.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/msbuild.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/extensions/rypile/python.py` & `Rypple-0.1.2/src/Rypple/extensions/rypile/python.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/namespace.py` & `Rypple-0.1.2/src/Rypple/namespace.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/scope.py` & `Rypple-0.1.2/src/Rypple/scope.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple/step.py` & `Rypple-0.1.2/src/Rypple/step.py`

 * *Files identical despite different names*

### Comparing `Rypple-0.1.1/src/Rypple.egg-info/SOURCES.txt` & `Rypple-0.1.2/src/Rypple.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/Rypple/extension.py
 src/Rypple/namespace.py
 src/Rypple/scope.py
 src/Rypple/step.py
 src/Rypple.egg-info/PKG-INFO
 src/Rypple.egg-info/SOURCES.txt
 src/Rypple.egg-info/dependency_links.txt
+src/Rypple.egg-info/requires.txt
 src/Rypple.egg-info/top_level.txt
 src/Rypple/extensions/console.py
 src/Rypple/extensions/core.py
 src/Rypple/extensions/filesystem.py
 src/Rypple/extensions/rypile/c#.py
 src/Rypple/extensions/rypile/c++.py
 src/Rypple/extensions/rypile/c.py
```

