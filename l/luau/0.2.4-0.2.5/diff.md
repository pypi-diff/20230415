# Comparing `tmp/luau-0.2.4.tar.gz` & `tmp/luau-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.2.4.tar", last modified: Sat Apr 15 00:04:50 2023, max compression
+gzip compressed data, was "luau-0.2.5.tar", last modified: Sat Apr 15 00:18:56 2023, max compression
```

## Comparing `luau-0.2.4.tar` & `luau-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:50.028165 luau-0.2.4/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-15 00:04:50.027167 luau-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.4/README.md
--rw-rw-rw-   0        0        0      494 2023-04-15 00:02:36.000000 luau-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 00:04:50.029162 luau-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:49.851234 luau-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:49.960007 luau-0.2.4/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.4/src/luau/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.4/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.4/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:50.025185 luau-0.2.4/src/luau/roblox/
--rw-rw-rw-   0        0        0      889 2023-04-15 00:02:36.000000 luau-0.2.4/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      834 2023-04-15 00:02:36.000000 luau-0.2.4/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1448 2023-04-14 23:55:14.000000 luau-0.2.4/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.4/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2726 2023-04-15 00:03:57.000000 luau-0.2.4/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:50.015198 luau-0.2.4/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-15 00:04:49.000000 luau-0.2.4/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-15 00:04:49.000000 luau-0.2.4/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:04:49.000000 luau-0.2.4/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-15 00:04:49.000000 luau-0.2.4/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 00:04:49.000000 luau-0.2.4/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.104634 luau-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-15 00:18:56.104516 luau-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.5/README.md
+-rw-rw-rw-   0        0        0      494 2023-04-15 00:18:28.000000 luau-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 00:18:56.105617 luau-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.064265 luau-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.075201 luau-0.2.5/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.5/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.5/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.5/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.101978 luau-0.2.5/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.2.5/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.2.5/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1586 2023-04-15 00:17:48.000000 luau-0.2.5/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.5/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2848 2023-04-15 00:17:48.000000 luau-0.2.5/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.094995 luau-0.2.5/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.2.4/LICENSE` & `luau-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.2.4/src/luau/__init__.py` & `luau-0.2.5/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.4/src/luau/convert.py` & `luau-0.2.5/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.4/src/luau/path.py` & `luau-0.2.5/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.4/src/luau/roblox/__init__.py` & `luau-0.2.5/src/luau/roblox/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from .tool import get_tool_name
 
-def format(path: str, prefix="ToolGen"):
-	stylua_tool_name = get_tool_name("JohnnyMorganz/StyLua", "0.15.3", prefix)
+def format(path: str):
+	stylua_tool_name = get_tool_name("JohnnyMorganz/StyLua", "0.15.3")
 	os.system(f"{stylua_tool_name} {path}")
 
 def write_script(build_path: str, content: str, write_as_directory: bool=False):
 	dir_name, file_name = os.path.split(build_path)
 	if not os.path.exists(dir_name):
 		os.makedirs(dir_name)
 	elif os.path.exists(build_path):
```

### Comparing `luau-0.2.4/src/luau/roblox/rojo.py` & `luau-0.2.5/src/luau/roblox/rojo.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 		if os.path.isfile(file_path):
 			base, ext = os.path.splitext(file_path)
 			if ext == ".json":
 				sec_base, sec_ext = os.path.splitext(base)
 				if sec_ext== ".project":
 					return file_path
 
-def get_rojo_name(prefix="ToolGen") -> str:
-	return get_tool_name(ROJO_SOURCE, ROJO_VERSION, prefix)
+def get_rojo_name() -> str:
+	return get_tool_name(ROJO_SOURCE, ROJO_VERSION)
 
 def build_sourcemap(project_json_path: str = ""):
 	if project_json_path == "":
 		project_json_path = get_rojo_project_path()
 	os.system(f"{get_rojo_name()} sourcemap {project_json_path} --output sourcemap.json")
```

### Comparing `luau-0.2.4/src/luau/roblox/tool.py` & `luau-0.2.5/src/luau/roblox/tool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 
 import os
 import toml
 
 FOREMAN_DEFAULT_PATH = "foreman.toml"
 AFTMAN_DEFAULT_PATH = "aftman.toml"
 
-def get_tool_name(source: str, version: str, prefix:str = "ToolGen") -> str:
+def get_tool_name(source: str, version: str) -> str:
 	alt_nickname = source.split("/")[len(source.split("/"))-1]
+	
+	version_str = version.replace(".","_").lower()
+	if version_str[0] == "v":
+		version_str = version_str[1:]
+
+	version_str = "_VERSION"+version_str
+
 	if os.path.exists(FOREMAN_DEFAULT_PATH):
 		foreman_config = toml.loads(open(FOREMAN_DEFAULT_PATH, "r").read())
 		foreman_tools = foreman_config["tools"]
+
+
 		for nickname, entry in foreman_tools.items():
 			if nickname == alt_nickname:
-				alt_nickname = prefix+"_"+alt_nickname
+				alt_nickname = alt_nickname+version_str
 
 			if "source" in entry and "version" in entry:
 				if entry["source"] == source and entry["version"] == version:
 					return nickname
 
 		foreman_tools[alt_nickname] = {
 			"source": source,
@@ -33,15 +42,15 @@
 
 	elif os.path.exists(AFTMAN_DEFAULT_PATH):
 		aftman_config = toml.loads(open(AFTMAN_DEFAULT_PATH, "r").read())
 		aftman_tools = aftman_config["tools"]
 		aft_path = source+"@"+version
 		for nickname, path in aftman_tools.items():
 			if nickname == alt_nickname:
-				alt_nickname = prefix+"_"+alt_nickname
+				alt_nickname = alt_nickname+version_str
 			if path == aft_path:
 				return path
 		
 		os.system(f"aftman add {aft_path} -{alt_nickname}")
 		return alt_nickname
 	else:
 		raise IndexError("no foreman or aftman config files found")
```

### Comparing `luau-0.2.4/src/luau/roblox/util.py` & `luau-0.2.5/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.4/src/luau/roblox/wally.py` & `luau-0.2.5/src/luau/roblox/wally.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,44 +4,51 @@
 from .rojo import get_rojo_project_path, get_rojo_name, build_sourcemap
 
 WALLY_SOURCE = "UpliftGames/wally"
 WALLY_VERSION = "0.3.1"
 WPT_SOURCE = "JohnnyMorganz/wally-package-types"
 WPT_VERSION = "1.2.0"
 
-def get_wally_name(prefix="ToolGen"):
-	return get_tool_name(WALLY_SOURCE, WALLY_VERSION, prefix)
+def get_wally_name():
+	return get_tool_name(WALLY_SOURCE, WALLY_VERSION)
 
-def get_wally_package_types_name(prefix="ToolGen"):
-	return get_tool_name(WPT_SOURCE, WPT_VERSION, prefix)
+def get_wally_package_types_name():
+	return get_tool_name(WPT_SOURCE, WPT_VERSION)
 
 def update_wally():
 
 	project_path = get_rojo_project_path()
 
 	wally_tool_name = get_wally_name()
 	rojo_tool_name = get_rojo_name()
 	wpt_tool_name = get_wally_package_types_name()
 
 	os.system(f"{wally_tool_name} install")
 	build_sourcemap()
 	os.system(f"{wpt_tool_name} --sourcemap sourcemap.json Packages")
 
-def get_wally_package_nickname(package_wally_path: str, prefix: str="ToolGen") -> str:
+def get_wally_package_nickname(package_wally_path: str) -> str:
 	wally_config = toml.loads(open("wally.toml", "r").read())
 	generated_nickname = (package_wally_path.split("/")[1].split("@")[0]).title()
 	name_parts = generated_nickname.split("-")
 	for i, name_part in enumerate(name_parts):
 		name_parts[i] = name_part.title()
 
 	generated_nickname = "".join(name_parts)
 
+	version = package_wally_path.split("@")[1]
+	version_str = version.replace(".","_").lower()
+	if version_str[0] == "v":
+		version_str = version_str[1:]
+
+	version_str = "_VERSION"+version_str
+
 	for nickname, package_path in wally_config["dependencies"].items():
 		if nickname == generated_nickname:
-			generated_nickname = prefix+"_"+generated_nickname.title()
+			generated_nickname = generated_nickname + version_str
 		if package_wally_path == package_path:
 			return nickname
 
 	# no maid installed
 	wally_config["dependencies"][generated_nickname] = package_wally_path
 
 	open("wally.toml", "w").write(toml.dumps(wally_config))
```

