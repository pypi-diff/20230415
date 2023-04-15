# Comparing `tmp/oldschool_management_tools-0.1.4.tar.gz` & `tmp/oldschool_management_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldschool_management_tools-0.1.4.tar", max compression
+gzip compressed data, was "oldschool_management_tools-0.1.5.tar", max compression
```

## Comparing `oldschool_management_tools-0.1.4.tar` & `oldschool_management_tools-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1315 2023-04-10 13:00:12.829587 oldschool_management_tools-0.1.4/oldschool_management_tools/calendar_items/calendar_item.py
--rw-r--r--   0        0        0      907 2023-04-10 14:57:09.545095 oldschool_management_tools-0.1.4/oldschool_management_tools/mgmt_tools_cmd.py
--rw-r--r--   0        0        0     4804 2023-04-10 14:52:09.479176 oldschool_management_tools-0.1.4/oldschool_management_tools/oldschool_management_tools.py
--rw-r--r--   0        0        0      352 2023-04-10 12:00:27.263061 oldschool_management_tools-0.1.4/oldschool_management_tools/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.4/oldschool_management_tools/README.md
--rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.4/oldschool_management_tools/special_prompts/special_prompts.py
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.4/oldschool_management_tools/tests/__init__.py
--rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.4/oldschool_management_tools/testy.py
--rw-r--r--   0        0        0      440 2023-04-10 14:58:11.210753 oldschool_management_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.4/README.md
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1315 2023-04-10 13:00:12.829587 oldschool_management_tools-0.1.5/oldschool_management_tools/calendar_items/calendar_item.py
+-rw-r--r--   0        0        0      907 2023-04-10 14:57:09.545095 oldschool_management_tools-0.1.5/oldschool_management_tools/mgmt_tools_cmd.py
+-rw-r--r--   0        0        0     4804 2023-04-10 14:52:09.479176 oldschool_management_tools-0.1.5/oldschool_management_tools/oldschool_management_tools.py
+-rw-r--r--   0        0        0      352 2023-04-15 13:08:32.632526 oldschool_management_tools-0.1.5/oldschool_management_tools/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.5/oldschool_management_tools/README.md
+-rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.5/oldschool_management_tools/special_prompts/special_prompts.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.5/oldschool_management_tools/tests/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.5/oldschool_management_tools/testy.py
+-rw-r--r--   0        0        0      440 2023-04-15 13:12:16.920724 oldschool_management_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.5/README.md
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.5/PKG-INFO
```

### Comparing `oldschool_management_tools-0.1.4/oldschool_management_tools/calendar_items/calendar_item.py` & `oldschool_management_tools-0.1.5/oldschool_management_tools/calendar_items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.4/oldschool_management_tools/mgmt_tools_cmd.py` & `oldschool_management_tools-0.1.5/oldschool_management_tools/mgmt_tools_cmd.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.4/oldschool_management_tools/oldschool_management_tools.py` & `oldschool_management_tools-0.1.5/oldschool_management_tools/oldschool_management_tools.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.4/oldschool_management_tools/special_prompts/special_prompts.py` & `oldschool_management_tools-0.1.5/oldschool_management_tools/special_prompts/special_prompts.py`

 * *Files identical despite different names*

