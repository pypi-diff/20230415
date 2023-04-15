# Comparing `tmp/luau-0.3.1.tar.gz` & `tmp/luau-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.3.1.tar", last modified: Sat Apr 15 01:07:51 2023, max compression
+gzip compressed data, was "luau-0.3.2.tar", last modified: Sat Apr 15 01:10:18 2023, max compression
```

## Comparing `luau-0.3.1.tar` & `luau-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 01:07:51.625454 luau-0.3.1/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-15 01:07:51.624456 luau-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.1/README.md
--rw-rw-rw-   0        0        0      512 2023-04-15 01:07:24.000000 luau-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 01:07:51.625454 luau-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 01:07:51.579623 luau-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 01:07:51.590595 luau-0.3.1/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.1/src/luau/__init__.py
--rw-rw-rw-   0        0        0     5326 2023-04-15 01:06:54.000000 luau-0.3.1/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.1/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:07:51.622465 luau-0.3.1/src/luau/roblox/
--rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.3.1/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.1/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.1/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.1/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.1/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:07:51.613962 luau-0.3.1/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-15 01:07:51.000000 luau-0.3.1/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-15 01:07:51.000000 luau-0.3.1/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 01:07:51.000000 luau-0.3.1/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-15 01:07:51.000000 luau-0.3.1/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 01:07:51.000000 luau-0.3.1/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 01:10:18.825499 luau-0.3.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-15 01:10:18.824525 luau-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.2/README.md
+-rw-rw-rw-   0        0        0      512 2023-04-15 01:09:52.000000 luau-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 01:10:18.825499 luau-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 01:10:18.777626 luau-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 01:10:18.795579 luau-0.3.2/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.2/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5336 2023-04-15 01:09:43.000000 luau-0.3.2/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.2/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:10:18.822512 luau-0.3.2/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.3.2/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.2/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.2/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.2/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.2/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:10:18.814528 luau-0.3.2/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-15 01:10:18.000000 luau-0.3.2/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-15 01:10:18.000000 luau-0.3.2/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 01:10:18.000000 luau-0.3.2/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-15 01:10:18.000000 luau-0.3.2/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 01:10:18.000000 luau-0.3.2/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.3.1/LICENSE` & `luau-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.3.1/pyproject.toml` & `luau-0.3.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "luau"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"dpath~=2.1.5",
 	"toml~=0.10.2",
 	"types-toml~=0.10.8.6"
```

### Comparing `luau-0.3.1/src/luau/__init__.py` & `luau-0.3.2/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.1/src/luau/convert.py` & `luau-0.3.2/src/luau/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,17 @@
 
 	# indent as needed and return value
 	if skip_initial_indent:
 		return _get_indent(0) + list_val + _insert_comma(add_comma_at_end)
 	else:
 		return _get_indent(indent_count) + list_val + _insert_comma(add_comma_at_end)
 
-def from_dict_to_type(value: dict, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False) -> str:
+def from_dict_to_type(type_value: dict, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False) -> str:
 	out = {}
-	for path, value in dpath.search(value, '**', yielded=True):
+	for path, value in dpath.search(type_value, '**', yielded=True):
 		literal_path_keys = []
 		for key in path.split("/"):
 			literal_path_keys.append(mark_as_literal(key))
 
 		literal_path = "/".join(literal_path_keys)
 
 		if type(value) != str:
```

### Comparing `luau-0.3.1/src/luau/path.py` & `luau-0.3.2/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.1/src/luau/roblox/__init__.py` & `luau-0.3.2/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.1/src/luau/roblox/rojo.py` & `luau-0.3.2/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.1/src/luau/roblox/tool.py` & `luau-0.3.2/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.1/src/luau/roblox/util.py` & `luau-0.3.2/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.3.1/src/luau/roblox/wally.py` & `luau-0.3.2/src/luau/roblox/wally.py`

 * *Files identical despite different names*

