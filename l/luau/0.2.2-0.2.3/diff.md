# Comparing `tmp/luau-0.2.2.tar.gz` & `tmp/luau-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.2.2.tar", last modified: Fri Apr 14 22:01:03 2023, max compression
+gzip compressed data, was "luau-0.2.3.tar", last modified: Fri Apr 14 23:57:53 2023, max compression
```

## Comparing `luau-0.2.2.tar` & `luau-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.596468 luau-0.2.2/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-14 22:01:03.595470 luau-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.2/README.md
--rw-rw-rw-   0        0        0      494 2023-04-14 22:00:31.000000 luau-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 22:01:03.596468 luau-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.544659 luau-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.555760 luau-0.2.2/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.2/src/luau/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.2/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.2/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.591559 luau-0.2.2/src/luau/roblox/
--rw-rw-rw-   0        0        0      863 2023-04-14 03:05:42.000000 luau-0.2.2/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-14 03:08:13.000000 luau-0.2.2/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1420 2023-04-14 03:05:42.000000 luau-0.2.2/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.2/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2478 2023-04-14 21:47:59.000000 luau-0.2.2/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-14 22:01:03.582583 luau-0.2.2/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-14 22:01:03.000000 luau-0.2.2/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 23:57:53.195070 luau-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-14 23:57:53.194073 luau-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.3/README.md
+-rw-rw-rw-   0        0        0      494 2023-04-14 23:56:11.000000 luau-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 23:57:53.196068 luau-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 23:57:53.139892 luau-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 23:57:53.155336 luau-0.2.3/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.3/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.3/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.3/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-14 23:57:53.193076 luau-0.2.3/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-14 03:05:42.000000 luau-0.2.3/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-14 03:08:13.000000 luau-0.2.3/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1448 2023-04-14 23:55:14.000000 luau-0.2.3/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.3/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2504 2023-04-14 23:55:14.000000 luau-0.2.3/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-14 23:57:53.184102 luau-0.2.3/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-14 23:57:53.000000 luau-0.2.3/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-14 23:57:53.000000 luau-0.2.3/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 23:57:53.000000 luau-0.2.3/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-14 23:57:53.000000 luau-0.2.3/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-14 23:57:53.000000 luau-0.2.3/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.2.2/LICENSE` & `luau-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.2.2/src/luau/__init__.py` & `luau-0.2.3/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.2/src/luau/convert.py` & `luau-0.2.3/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.2/src/luau/path.py` & `luau-0.2.3/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.2/src/luau/roblox/__init__.py` & `luau-0.2.3/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.2/src/luau/roblox/rojo.py` & `luau-0.2.3/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.2/src/luau/roblox/tool.py` & `luau-0.2.3/src/luau/roblox/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 import os
 import toml
 
 FOREMAN_DEFAULT_PATH = "foreman.toml"
 AFTMAN_DEFAULT_PATH = "aftman.toml"
 
-def get_tool_name(source: str, version: str) -> str:
+def get_tool_name(source: str, version: str, prefix:str = "ToolGen") -> str:
 	alt_nickname = source.split("/")[len(source.split("/"))-1]
 	if os.path.exists(FOREMAN_DEFAULT_PATH):
 		foreman_config = toml.loads(open(FOREMAN_DEFAULT_PATH, "r").read())
 		foreman_tools = foreman_config["tools"]
 		for nickname, entry in foreman_tools.items():
 			if nickname == alt_nickname:
-				alt_nickname = "midas_"+alt_nickname
+				alt_nickname = prefix+"_"+alt_nickname
 
 			if "source" in entry and "version" in entry:
 				if entry["source"] == source and entry["version"] == version:
 					return nickname
 
 		foreman_tools[alt_nickname] = {
 			"source": source,
@@ -33,15 +33,15 @@
 
 	elif os.path.exists(AFTMAN_DEFAULT_PATH):
 		aftman_config = toml.loads(open(AFTMAN_DEFAULT_PATH, "r").read())
 		aftman_tools = aftman_config["tools"]
 		aft_path = source+"@"+version
 		for nickname, path in aftman_tools.items():
 			if nickname == alt_nickname:
-				alt_nickname = "midas_"+alt_nickname
+				alt_nickname = prefix+"_"+alt_nickname
 			if path == aft_path:
 				return path
 		
 		os.system(f"aftman add {aft_path} -{alt_nickname}")
 		return alt_nickname
 	else:
 		raise IndexError("no foreman or aftman config files found")
```

### Comparing `luau-0.2.2/src/luau/roblox/util.py` & `luau-0.2.3/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.2/src/luau/roblox/wally.py` & `luau-0.2.3/src/luau/roblox/wally.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 	rojo_tool_name = get_rojo_name()
 	wpt_tool_name = get_wally_package_types_name()
 
 	os.system(f"{wally_tool_name} install")
 	build_sourcemap()
 	os.system(f"{wpt_tool_name} --sourcemap sourcemap.json Packages")
 
-def get_wally_package_nickname(package_wally_path: str) -> str:
+def get_wally_package_nickname(package_wally_path: str, prefix: str="ToolGen") -> str:
 	wally_config = toml.loads(open("wally.toml", "r").read())
 	generated_nickname = (package_wally_path.split("/")[1].split("@")[0]).title()
 	for nickname, package_path in wally_config["dependencies"].items():
 		if nickname == generated_nickname:
-			generated_nickname = "Midas"+generated_nickname.title()
+			generated_nickname = prefix+"_"+generated_nickname.title()
 		if package_wally_path == package_path:
 			return nickname
 
 	# no maid installed
 	wally_config["dependencies"][generated_nickname] = package_wally_path
 
 	open("wally.toml", "w").write(toml.dumps(wally_config))
```

