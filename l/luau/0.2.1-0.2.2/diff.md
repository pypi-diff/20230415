# Comparing `tmp/luau-0.2.1.tar.gz` & `tmp/luau-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.2.1.tar", last modified: Fri Apr 14 21:49:34 2023, max compression
+gzip compressed data, was "luau-0.2.2.tar", last modified: Fri Apr 14 22:01:03 2023, max compression
```

## Comparing `luau-0.2.1.tar` & `luau-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 21:49:34.008348 luau-0.2.1/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-14 21:49:34.007351 luau-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.1/README.md
--rw-rw-rw-   0        0        0      494 2023-04-14 21:48:10.000000 luau-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 21:49:34.008348 luau-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 21:49:33.921402 luau-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 21:49:33.952318 luau-0.2.1/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.1/src/luau/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.1/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.1/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-14 21:49:34.005357 luau-0.2.1/src/luau/roblox/
--rw-rw-rw-   0        0        0      863 2023-04-14 03:05:42.000000 luau-0.2.1/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-14 03:08:13.000000 luau-0.2.1/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1420 2023-04-14 03:05:42.000000 luau-0.2.1/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      839 2023-04-14 02:57:33.000000 luau-0.2.1/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2478 2023-04-14 21:47:59.000000 luau-0.2.1/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-14 21:49:33.980390 luau-0.2.1/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-14 21:49:33.000000 luau-0.2.1/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.596468 luau-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-14 22:01:03.595470 luau-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.2/README.md
+-rw-rw-rw-   0        0        0      494 2023-04-14 22:00:31.000000 luau-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 22:01:03.596468 luau-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.544659 luau-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.555760 luau-0.2.2/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.2/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.2/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.2/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.591559 luau-0.2.2/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-14 03:05:42.000000 luau-0.2.2/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-14 03:08:13.000000 luau-0.2.2/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1420 2023-04-14 03:05:42.000000 luau-0.2.2/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.2/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2478 2023-04-14 21:47:59.000000 luau-0.2.2/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.582583 luau-0.2.2/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.2.1/LICENSE` & `luau-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.2.1/src/luau/__init__.py` & `luau-0.2.2/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.1/src/luau/convert.py` & `luau-0.2.2/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.1/src/luau/path.py` & `luau-0.2.2/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.1/src/luau/roblox/__init__.py` & `luau-0.2.2/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.1/src/luau/roblox/rojo.py` & `luau-0.2.2/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.1/src/luau/roblox/tool.py` & `luau-0.2.2/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.1/src/luau/roblox/util.py` & `luau-0.2.2/src/luau/roblox/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 	for service in ["ReplicatedStorage", "ServerStorage", "ServerScriptService", "ReplicatedFirst", "Lighting", "StarterGui", "StarterPlayer", "Workspace"]:
 		roblox_path = roblox_path.replace(f"game:WaitForChild(\"{service}\")", f"game:GetService(\"{service}\")")
 
 	return roblox_path
 
 def get_module_require(path: str):
-	return f"require({path})"
+	return f"require({get_instance_from_path(path)})"
 
 def get_header_module(path: str, variable_name: str = ""):
 	if variable_name == "":
 		keys = path.split("/")
 		variable_name = keys[len(keys)-1]
 
 	value = get_module_require(path)
```

### Comparing `luau-0.2.1/src/luau/roblox/wally.py` & `luau-0.2.2/src/luau/roblox/wally.py`

 * *Files identical despite different names*

