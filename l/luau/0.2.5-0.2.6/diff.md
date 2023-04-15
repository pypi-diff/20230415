# Comparing `tmp/luau-0.2.5.tar.gz` & `tmp/luau-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.2.5.tar", last modified: Sat Apr 15 00:18:56 2023, max compression
+gzip compressed data, was "luau-0.2.6.tar", last modified: Sat Apr 15 00:38:55 2023, max compression
```

## Comparing `luau-0.2.5.tar` & `luau-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.104634 luau-0.2.5/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-15 00:18:56.104516 luau-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.5/README.md
--rw-rw-rw-   0        0        0      494 2023-04-15 00:18:28.000000 luau-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 00:18:56.105617 luau-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.064265 luau-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.075201 luau-0.2.5/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.5/src/luau/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.5/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.5/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.101978 luau-0.2.5/src/luau/roblox/
--rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.2.5/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.2.5/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1586 2023-04-15 00:17:48.000000 luau-0.2.5/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.5/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2848 2023-04-15 00:17:48.000000 luau-0.2.5/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:18:56.094995 luau-0.2.5/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 00:18:56.000000 luau-0.2.5/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.398238 luau-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-15 00:38:55.397241 luau-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.6/README.md
+-rw-rw-rw-   0        0        0      494 2023-04-15 00:38:24.000000 luau-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 00:38:55.398238 luau-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.325107 luau-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.345564 luau-0.2.6/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.6/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.6/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.6/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.389504 luau-0.2.6/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.2.6/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.2.6/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.2.6/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.6/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.2.6/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.380921 luau-0.2.6/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.2.5/LICENSE` & `luau-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.2.5/src/luau/__init__.py` & `luau-0.2.6/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.5/src/luau/convert.py` & `luau-0.2.6/src/luau/convert.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.5/src/luau/path.py` & `luau-0.2.6/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.5/src/luau/roblox/__init__.py` & `luau-0.2.6/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.5/src/luau/roblox/rojo.py` & `luau-0.2.6/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.5/src/luau/roblox/tool.py` & `luau-0.2.6/src/luau/roblox/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def get_tool_name(source: str, version: str) -> str:
 	alt_nickname = source.split("/")[len(source.split("/"))-1]
 	
 	version_str = version.replace(".","_").lower()
 	if version_str[0] == "v":
 		version_str = version_str[1:]
 
-	version_str = "_VERSION"+version_str
+	version_str = "_VERSION_"+version_str
 
 	if os.path.exists(FOREMAN_DEFAULT_PATH):
 		foreman_config = toml.loads(open(FOREMAN_DEFAULT_PATH, "r").read())
 		foreman_tools = foreman_config["tools"]
 
 
 		for nickname, entry in foreman_tools.items():
```

### Comparing `luau-0.2.5/src/luau/roblox/util.py` & `luau-0.2.6/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.5/src/luau/roblox/wally.py` & `luau-0.2.6/src/luau/roblox/wally.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 	generated_nickname = "".join(name_parts)
 
 	version = package_wally_path.split("@")[1]
 	version_str = version.replace(".","_").lower()
 	if version_str[0] == "v":
 		version_str = version_str[1:]
 
-	version_str = "_VERSION"+version_str
+	version_str = "_VERSION_"+version_str
 
 	for nickname, package_path in wally_config["dependencies"].items():
 		if nickname == generated_nickname:
 			generated_nickname = generated_nickname + version_str
 		if package_wally_path == package_path:
 			return nickname
```

