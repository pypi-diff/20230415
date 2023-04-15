# Comparing `tmp/luau-0.3.3.tar.gz` & `tmp/luau-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.3.3.tar", last modified: Sat Apr 15 01:17:29 2023, max compression
+gzip compressed data, was "luau-0.3.4.tar", last modified: Sat Apr 15 01:24:42 2023, max compression
```

## Comparing `luau-0.3.3.tar` & `luau-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 01:17:29.577045 luau-0.3.3/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.3/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-15 01:17:29.576047 luau-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.3/README.md
--rw-rw-rw-   0        0        0      512 2023-04-15 01:17:07.000000 luau-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 01:17:29.577045 luau-0.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 01:17:29.532548 luau-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 01:17:29.542523 luau-0.3.3/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.3/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5707 2023-04-15 01:17:01.000000 luau-0.3.3/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.3/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:17:29.569447 luau-0.3.3/src/luau/roblox/
--rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.3.3/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.3/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.3/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.3/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.3/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:17:29.561468 luau-0.3.3/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-15 01:17:29.000000 luau-0.3.3/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-15 01:17:29.000000 luau-0.3.3/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 01:17:29.000000 luau-0.3.3/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-15 01:17:29.000000 luau-0.3.3/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 01:17:29.000000 luau-0.3.3/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 01:24:42.114423 luau-0.3.4/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-15 01:24:42.113431 luau-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.4/README.md
+-rw-rw-rw-   0        0        0      512 2023-04-15 01:24:18.000000 luau-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 01:24:42.114423 luau-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 01:24:42.067383 luau-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 01:24:42.079334 luau-0.3.4/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.4/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5709 2023-04-15 01:24:18.000000 luau-0.3.4/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.4/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:24:42.111931 luau-0.3.4/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.3.4/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.4/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.4/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.4/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.4/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:24:42.103817 luau-0.3.4/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-15 01:24:42.000000 luau-0.3.4/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-15 01:24:42.000000 luau-0.3.4/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 01:24:42.000000 luau-0.3.4/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-15 01:24:42.000000 luau-0.3.4/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 01:24:42.000000 luau-0.3.4/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.3.3/LICENSE` & `luau-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.3.3/pyproject.toml` & `luau-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "luau"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"dpath~=2.1.5",
 	"toml~=0.10.2",
 	"types-toml~=0.10.8.6"
```

### Comparing `luau-0.3.3/src/luau/__init__.py` & `luau-0.3.4/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.3/src/luau/convert.py` & `luau-0.3.4/src/luau/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 		for key in path.split("/"):
 			literal_path_keys.append(mark_as_literal(key))
 
 		literal_path = "/".join(literal_path_keys)
 
 		if value == bool or type(value) == bool:
 			dpath.new(out, literal_path, mark_as_literal("boolean"))
-		elif value == int or value == float or type(value) == int or type(value) == str:
+		elif value == int or value == float or type(value) == int or type(value) == float:
 			dpath.new(out, literal_path, mark_as_literal("number"))
 		elif value == str:
 			dpath.new(out, literal_path, mark_as_literal("string"))	
 		elif type(value) == str:
 			if get_if_literal(value):
 				dpath.new(out, literal_path, value)
 			else:
```

### Comparing `luau-0.3.3/src/luau/path.py` & `luau-0.3.4/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.3/src/luau/roblox/__init__.py` & `luau-0.3.4/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.3/src/luau/roblox/rojo.py` & `luau-0.3.4/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.3/src/luau/roblox/tool.py` & `luau-0.3.4/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.3/src/luau/roblox/util.py` & `luau-0.3.4/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.3/src/luau/roblox/wally.py` & `luau-0.3.4/src/luau/roblox/wally.py`

 * *Files identical despite different names*

