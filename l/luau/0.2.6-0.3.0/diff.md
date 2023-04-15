# Comparing `tmp/luau-0.2.6.tar.gz` & `tmp/luau-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luau-0.2.6.tar", last modified: Sat Apr 15 00:38:55 2023, max compression
+gzip compressed data, was "luau-0.3.0.tar", last modified: Sat Apr 15 01:03:34 2023, max compression
```

## Comparing `luau-0.2.6.tar` & `luau-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.398238 luau-0.2.6/
--rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      405 2023-04-15 00:38:55.397241 luau-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.2.6/README.md
--rw-rw-rw-   0        0        0      494 2023-04-15 00:38:24.000000 luau-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 00:38:55.398238 luau-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.325107 luau-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.345564 luau-0.2.6/src/luau/
--rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.2.6/src/luau/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-04-14 03:16:04.000000 luau-0.2.6/src/luau/convert.py
--rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.2.6/src/luau/path.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.389504 luau-0.2.6/src/luau/roblox/
--rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.2.6/src/luau/roblox/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.2.6/src/luau/roblox/rojo.py
--rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.2.6/src/luau/roblox/tool.py
--rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.2.6/src/luau/roblox/util.py
--rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.2.6/src/luau/roblox/wally.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:55.380921 luau-0.2.6/src/luau.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 00:38:55.000000 luau-0.2.6/src/luau.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:34.084484 luau-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 07:23:56.000000 luau-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-04-15 01:03:34.084484 luau-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-07 07:23:56.000000 luau-0.3.0/README.md
+-rw-rw-rw-   0        0        0      494 2023-04-15 01:03:02.000000 luau-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 01:03:34.085479 luau-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:34.048577 luau-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:34.059559 luau-0.3.0/src/luau/
+-rw-rw-rw-   0        0        0     2124 2023-04-14 03:14:17.000000 luau-0.3.0/src/luau/__init__.py
+-rw-rw-rw-   0        0        0     5250 2023-04-15 01:02:29.000000 luau-0.3.0/src/luau/convert.py
+-rw-rw-rw-   0        0        0     2515 2023-04-14 03:02:52.000000 luau-0.3.0/src/luau/path.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:34.082487 luau-0.3.0/src/luau/roblox/
+-rw-rw-rw-   0        0        0      863 2023-04-15 00:17:07.000000 luau-0.3.0/src/luau/roblox/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-15 00:17:07.000000 luau-0.3.0/src/luau/roblox/rojo.py
+-rw-rw-rw-   0        0        0     1587 2023-04-15 00:38:19.000000 luau-0.3.0/src/luau/roblox/tool.py
+-rw-rw-rw-   0        0        0      863 2023-04-14 22:00:20.000000 luau-0.3.0/src/luau/roblox/util.py
+-rw-rw-rw-   0        0        0     2849 2023-04-15 00:38:19.000000 luau-0.3.0/src/luau/roblox/wally.py
+drwxrwxrwx   0        0        0        0 2023-04-15 01:03:34.074508 luau-0.3.0/src/luau.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-04-15 01:03:34.000000 luau-0.3.0/src/luau.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-15 01:03:34.000000 luau-0.3.0/src/luau.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 01:03:34.000000 luau-0.3.0/src/luau.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-15 01:03:34.000000 luau-0.3.0/src/luau.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 01:03:34.000000 luau-0.3.0/src/luau.egg-info/top_level.txt
```

### Comparing `luau-0.2.6/LICENSE` & `luau-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luau-0.2.6/src/luau/__init__.py` & `luau-0.3.0/src/luau/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.6/src/luau/convert.py` & `luau-0.3.0/src/luau/convert.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import dpath
 
 READ_STR_AS_LITERAL_PREFIX = "<LITERAL_STRING_START>_!_"
 READ_STR_AS_LITERAL_SUFFIX = "_!_<LITERAL_STRING_END>"
 
 def _insert_comma(enabled: bool) -> str:
 	if enabled:
 		return ","
@@ -10,31 +11,30 @@
 
 def _get_indent(indent_count: int) -> str:
 	return "\t"*indent_count
 
 def from_bool(value: bool, indent_count=0, add_comma_at_end=False) -> str:
 	return _get_indent(indent_count) + str(value).lower() + _insert_comma(add_comma_at_end)
 
+def get_if_literal(value: str):
+	return (READ_STR_AS_LITERAL_PREFIX == value[0:len(READ_STR_AS_LITERAL_PREFIX)]) or value.find(READ_STR_AS_LITERAL_SUFFIX) != -1
+
 def from_str(value: str, indent_count=0, add_comma_at_end=False) -> str:
-	suffix_index = value.find(READ_STR_AS_LITERAL_SUFFIX)
-	
-	starts_with_prefix = READ_STR_AS_LITERAL_PREFIX == value[0:len(READ_STR_AS_LITERAL_PREFIX)]
-	if starts_with_prefix and suffix_index != -1:
+	if get_if_literal(value):
 		raw_val = value.replace(READ_STR_AS_LITERAL_PREFIX, "").replace(READ_STR_AS_LITERAL_SUFFIX, "")
 		return _get_indent(indent_count) + raw_val + _insert_comma(add_comma_at_end)
 	else:
 		return _get_indent(indent_count) + f"\"{value}\"" + _insert_comma(add_comma_at_end)
 
 def from_number(value: int | float, indent_count=0, add_comma_at_end=False) -> str:
 	return _get_indent(indent_count) + str(value) + _insert_comma(add_comma_at_end)
 
 def from_nil(indent_count=0, add_comma_at_end=False) -> str:
 	return f"{_get_indent(indent_count)} nil" + _insert_comma(add_comma_at_end)
 
-
 def from_list(value: list, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False):
 	
 	# start list
 	list_val = ""
 	if skip_initial_indent:
 		list_val += "{"
 	else:
@@ -73,19 +73,27 @@
 		list_val += "{"
 	else:
 		list_val += _get_indent(indent_count) + "{"
 
 	# iterate through key-val pairs
 	for k, v in value.items():
 
+		is_literal = get_if_literal(k)
+
 		# write entry
 		if type(v) == dict or type(v) == list:
-			entry = f"[{from_any(k, 0, False)}] = {from_any(v, indent_count+1, False, multi_line, True)}" + _insert_comma(True)
+			if is_literal:
+				entry = f"{from_any(k, 0, False)} = {from_any(v, indent_count+1, False, multi_line, True)}" + _insert_comma(True)
+			else:
+				entry = f"[{from_any(k, 0, False)}] = {from_any(v, indent_count+1, False, multi_line, True)}" + _insert_comma(True)
 		else:
-			entry = f"[{from_any(k, 0, False)}] = {from_any(v, 0, False, multi_line, True)}" + _insert_comma(True)
+			if is_literal:
+				entry = f"{from_any(k, 0, False)} = {from_any(v, 0, False, multi_line, True)}" + _insert_comma(True)
+			else:
+				entry = f"[{from_any(k, 0, False)}] = {from_any(v, 0, False, multi_line, True)}" + _insert_comma(True)
 
 		# add it to existing string
 		if multi_line:
 			list_val += "\n" + _get_indent(indent_count+1) + entry
 		else:
 			list_val += entry
 
@@ -98,14 +106,27 @@
 
 	# indent as needed and return value
 	if skip_initial_indent:
 		return _get_indent(0) + list_val + _insert_comma(add_comma_at_end)
 	else:
 		return _get_indent(indent_count) + list_val + _insert_comma(add_comma_at_end)
 
+def from_dict_to_type(value: dict, indent_count=0, add_comma_at_end=False, multi_line=True, skip_initial_indent=False) -> str:
+	out = {}
+	for path, value in dpath.search(value, '**', yielded=True):
+		literal_path_keys = []
+		for key in path.split("/"):
+			literal_path_keys.append(mark_as_literal(key))
+
+		literal_path = "/".join(literal_path_keys)
+
+		dpath.new(out, literal_path, mark_as_literal(value))
+
+	return from_dict(out, indent_count, add_comma_at_end, multi_line, skip_initial_indent).replace(" = ", ": ")
+
 def from_any(
 	value: int | str | None | float | dict | list = None, 
 	indent_count = 0, 
 	add_comma_at_end = False, 
 	multi_line=True,
 	skip_initial_indent=False
 ) -> str:
```

### Comparing `luau-0.2.6/src/luau/path.py` & `luau-0.3.0/src/luau/path.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.6/src/luau/roblox/__init__.py` & `luau-0.3.0/src/luau/roblox/__init__.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.6/src/luau/roblox/rojo.py` & `luau-0.3.0/src/luau/roblox/rojo.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.6/src/luau/roblox/tool.py` & `luau-0.3.0/src/luau/roblox/tool.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.6/src/luau/roblox/util.py` & `luau-0.3.0/src/luau/roblox/util.py`

 * *Files identical despite different names*

### Comparing `luau-0.2.6/src/luau/roblox/wally.py` & `luau-0.3.0/src/luau/roblox/wally.py`

 * *Files identical despite different names*

